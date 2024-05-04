# Comparing `tmp/citric-1.0.0.tar.gz` & `tmp/citric-1.0.1a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, last modified: Tue Feb 13 02:29:16 2024, max compression
+gzip compressed data, last modified: Wed May  1 17:46:34 2024, max compression
```

## Comparing `citric-1.0.0.tar` & `citric-1.0.1a1.tar`

### file list

```diff
@@ -1,138 +1,140 @@
--rw-r--r--   0        0        0     1081 2024-02-13 02:29:16.000000 citric-1.0.0/.changie.yaml
--rw-r--r--   0        0        0       85 2024-02-13 02:29:16.000000 citric-1.0.0/.flake8
--rw-r--r--   0        0        0       36 2024-02-13 02:29:16.000000 citric-1.0.0/.gitattributes
--rw-r--r--   0        0        0     1684 2024-02-13 02:29:16.000000 citric-1.0.0/.pre-commit-config.yaml
--rw-r--r--   0        0        0      290 2024-02-13 02:29:16.000000 citric-1.0.0/.readthedocs.yaml
--rw-r--r--   0        0        0       54 2024-02-13 02:29:16.000000 citric-1.0.0/.sonarcloud.properties
--rw-r--r--   0        0        0    10546 2024-02-13 02:29:16.000000 citric-1.0.0/CHANGELOG.md
--rw-r--r--   0        0        0      337 2024-02-13 02:29:16.000000 citric-1.0.0/CITATION.cff
--rw-r--r--   0        0        0     5225 2024-02-13 02:29:16.000000 citric-1.0.0/CODE_OF_CONDUCT.md
--rw-r--r--   0        0        0      837 2024-02-13 02:29:16.000000 citric-1.0.0/SECURITY.md
--rw-r--r--   0        0        0      247 2024-02-13 02:29:16.000000 citric-1.0.0/codecov.yml
--rw-r--r--   0        0        0      889 2024-02-13 02:29:16.000000 citric-1.0.0/docker-compose.mysql.yml
--rw-r--r--   0        0        0      323 2024-02-13 02:29:16.000000 citric-1.0.0/docker-compose.ref.yml
--rw-r--r--   0        0        0     1702 2024-02-13 02:29:16.000000 citric-1.0.0/docker-compose.yml
--rw-r--r--   0        0        0     4653 2024-02-13 02:29:16.000000 citric-1.0.0/noxfile.py
--rw-r--r--   0        0        0      491 2024-02-13 02:29:16.000000 citric-1.0.0/.changes/0.0.1.md
--rw-r--r--   0        0        0     1152 2024-02-13 02:29:16.000000 citric-1.0.0/.changes/0.0.10.md
--rw-r--r--   0        0        0      246 2024-02-13 02:29:16.000000 citric-1.0.0/.changes/0.0.11.md
--rw-r--r--   0        0        0      132 2024-02-13 02:29:16.000000 citric-1.0.0/.changes/0.0.12.md
--rw-r--r--   0        0        0      135 2024-02-13 02:29:16.000000 citric-1.0.0/.changes/0.0.13.md
--rw-r--r--   0        0        0      129 2024-02-13 02:29:16.000000 citric-1.0.0/.changes/0.0.14.md
--rw-r--r--   0        0        0      157 2024-02-13 02:29:16.000000 citric-1.0.0/.changes/0.0.2.md
--rw-r--r--   0        0        0      126 2024-02-13 02:29:16.000000 citric-1.0.0/.changes/0.0.3.md
--rw-r--r--   0        0        0      186 2024-02-13 02:29:16.000000 citric-1.0.0/.changes/0.0.4.md
--rw-r--r--   0        0        0      245 2024-02-13 02:29:16.000000 citric-1.0.0/.changes/0.0.5.md
--rw-r--r--   0        0        0      114 2024-02-13 02:29:16.000000 citric-1.0.0/.changes/0.0.6.md
--rw-r--r--   0        0        0      141 2024-02-13 02:29:16.000000 citric-1.0.0/.changes/0.0.7.md
--rw-r--r--   0        0        0      224 2024-02-13 02:29:16.000000 citric-1.0.0/.changes/0.0.8.md
--rw-r--r--   0        0        0      314 2024-02-13 02:29:16.000000 citric-1.0.0/.changes/0.0.9.md
--rw-r--r--   0        0        0      132 2024-02-13 02:29:16.000000 citric-1.0.0/.changes/0.1.0.md
--rw-r--r--   0        0        0      669 2024-02-13 02:29:16.000000 citric-1.0.0/.changes/0.10.0.md
--rw-r--r--   0        0        0      269 2024-02-13 02:29:16.000000 citric-1.0.0/.changes/0.2.0.md
--rw-r--r--   0        0        0      129 2024-02-13 02:29:16.000000 citric-1.0.0/.changes/0.3.0.md
--rw-r--r--   0        0        0      506 2024-02-13 02:29:16.000000 citric-1.0.0/.changes/0.4.0.md
--rw-r--r--   0        0        0      142 2024-02-13 02:29:16.000000 citric-1.0.0/.changes/0.4.1.md
--rw-r--r--   0        0        0      251 2024-02-13 02:29:16.000000 citric-1.0.0/.changes/0.4.2.md
--rw-r--r--   0        0        0      167 2024-02-13 02:29:16.000000 citric-1.0.0/.changes/0.4.3.md
--rw-r--r--   0        0        0      295 2024-02-13 02:29:16.000000 citric-1.0.0/.changes/0.4.4.md
--rw-r--r--   0        0        0      152 2024-02-13 02:29:16.000000 citric-1.0.0/.changes/0.4.5.md
--rw-r--r--   0        0        0      227 2024-02-13 02:29:16.000000 citric-1.0.0/.changes/0.5.0.md
--rw-r--r--   0        0        0      364 2024-02-13 02:29:16.000000 citric-1.0.0/.changes/0.6.0.md
--rw-r--r--   0        0        0      260 2024-02-13 02:29:16.000000 citric-1.0.0/.changes/0.7.0.md
--rw-r--r--   0        0        0      141 2024-02-13 02:29:16.000000 citric-1.0.0/.changes/0.7.1-b1.md
--rw-r--r--   0        0        0      141 2024-02-13 02:29:16.000000 citric-1.0.0/.changes/0.7.1-b2.md
--rw-r--r--   0        0        0      231 2024-02-13 02:29:16.000000 citric-1.0.0/.changes/0.7.1-b3.md
--rw-r--r--   0        0        0      136 2024-02-13 02:29:16.000000 citric-1.0.0/.changes/0.7.1.md
--rw-r--r--   0        0        0      151 2024-02-13 02:29:16.000000 citric-1.0.0/.changes/0.7.2.md
--rw-r--r--   0        0        0      756 2024-02-13 02:29:16.000000 citric-1.0.0/.changes/0.8.0.md
--rw-r--r--   0        0        0      590 2024-02-13 02:29:16.000000 citric-1.0.0/.changes/0.9.0.md
--rw-r--r--   0        0        0      672 2024-02-13 02:29:16.000000 citric-1.0.0/.changes/1.0.0.md
--rw-r--r--   0        0        0      304 2024-02-13 02:29:16.000000 citric-1.0.0/.changes/header.tpl.md
--rw-r--r--   0        0        0        0 2024-02-13 02:29:16.000000 citric-1.0.0/.changes/unreleased/.gitkeep
--rw-r--r--   0        0        0     2399 2024-02-13 02:29:16.000000 citric-1.0.0/.circleci/config.yml
--rw-r--r--   0        0        0       74 2024-02-13 02:29:16.000000 citric-1.0.0/.github/FUNDING.yml
--rw-r--r--   0        0        0     1326 2024-02-13 02:29:16.000000 citric-1.0.0/.github/dependabot.yml
--rw-r--r--   0        0        0       59 2024-02-13 02:29:16.000000 citric-1.0.0/.github/semantic.yml
--rw-r--r--   0        0        0     2154 2024-02-13 02:29:16.000000 citric-1.0.0/.github/ISSUE_TEMPLATE/BUG.yml
--rw-r--r--   0        0        0       27 2024-02-13 02:29:16.000000 citric-1.0.0/.github/ISSUE_TEMPLATE/config.yml
--rw-r--r--   0        0        0     1013 2024-02-13 02:29:16.000000 citric-1.0.0/.github/ISSUE_TEMPLATE/feature.yml
--rw-r--r--   0        0        0      873 2024-02-13 02:29:16.000000 citric-1.0.0/.github/actions/install-tools/action.yml
--rw-r--r--   0        0        0        0 2024-02-13 02:29:16.000000 citric-1.0.0/.github/badges/.gitkeep
--rw-r--r--   0        0        0     1307 2024-02-13 02:29:16.000000 citric-1.0.0/.github/workflows/api-changes.yml
--rw-r--r--   0        0        0     2181 2024-02-13 02:29:16.000000 citric-1.0.0/.github/workflows/build.yml
--rw-r--r--   0        0        0       59 2024-02-13 02:29:16.000000 citric-1.0.0/.github/workflows/constraints.txt
--rw-r--r--   0        0        0     3482 2024-02-13 02:29:16.000000 citric-1.0.0/.github/workflows/gen-release-pr.yml
--rw-r--r--   0        0        0      326 2024-02-13 02:29:16.000000 citric-1.0.0/.github/workflows/pr-preview-links.yml
--rw-r--r--   0        0        0     2928 2024-02-13 02:29:16.000000 citric-1.0.0/.github/workflows/scorecard.yml
--rw-r--r--   0        0        0    10316 2024-02-13 02:29:16.000000 citric-1.0.0/.github/workflows/tests.yml
--rw-r--r--   0        0        0      267 2024-02-13 02:29:16.000000 citric-1.0.0/code_samples/auth_plugin.py
--rw-r--r--   0        0        0      336 2024-02-13 02:29:16.000000 citric-1.0.0/code_samples/context_manager.py
--rw-r--r--   0        0        0      563 2024-02-13 02:29:16.000000 citric-1.0.0/code_samples/custom_requests_session.py
--rw-r--r--   0        0        0      626 2024-02-13 02:29:16.000000 citric-1.0.0/code_samples/duckdb_sql.py
--rw-r--r--   0        0        0      573 2024-02-13 02:29:16.000000 citric-1.0.0/code_samples/get_surveys.py
--rw-r--r--   0        0        0      583 2024-02-13 02:29:16.000000 citric-1.0.0/code_samples/pandas_df.py
--rw-r--r--   0        0        0      517 2024-02-13 02:29:16.000000 citric-1.0.0/code_samples/requests_session_attributes.py
--rw-r--r--   0        0        0      159 2024-02-13 02:29:16.000000 citric-1.0.0/code_samples/ruff.toml
--rw-r--r--   0        0        0      521 2024-02-13 02:29:16.000000 citric-1.0.0/code_samples/session_attr.py
--rw-r--r--   0        0        0      561 2024-02-13 02:29:16.000000 citric-1.0.0/code_samples/upload_s3.py
--rw-r--r--   0        0        0       33 2024-02-13 02:29:16.000000 citric-1.0.0/docs/changelog.md
--rw-r--r--   0        0        0   106926 2024-02-13 02:29:16.000000 citric-1.0.0/docs/code.png
--rw-r--r--   0        0        0     6110 2024-02-13 02:29:16.000000 citric-1.0.0/docs/conf.py
--rw-r--r--   0        0        0       54 2024-02-13 02:29:16.000000 citric-1.0.0/docs/googled10b55fb460af091.html
--rw-r--r--   0        0        0     2876 2024-02-13 02:29:16.000000 citric-1.0.0/docs/how-to.md
--rw-r--r--   0        0        0     2571 2024-02-13 02:29:16.000000 citric-1.0.0/docs/index.md
--rw-r--r--   0        0        0       41 2024-02-13 02:29:16.000000 citric-1.0.0/docs/license.rst
--rw-r--r--   0        0        0     2489 2024-02-13 02:29:16.000000 citric-1.0.0/docs/requirements.txt
--rw-r--r--   0        0        0      740 2024-02-13 02:29:16.000000 citric-1.0.0/docs/rest_coverage.md
--rw-r--r--   0        0        0    11121 2024-02-13 02:29:16.000000 citric-1.0.0/docs/rpc_coverage.md
--rw-r--r--   0        0        0        0 2024-02-13 02:29:16.000000 citric-1.0.0/docs/_ext/__init__.py
--rw-r--r--   0        0        0     2521 2024-02-13 02:29:16.000000 citric-1.0.0/docs/_ext/limesurvey_future.py
--rw-r--r--   0        0        0       42 2024-02-13 02:29:16.000000 citric-1.0.0/docs/contributing/code-of-conduct.md
--rw-r--r--   0        0        0     2418 2024-02-13 02:29:16.000000 citric-1.0.0/docs/contributing/docker.md
--rw-r--r--   0        0        0      299 2024-02-13 02:29:16.000000 citric-1.0.0/docs/contributing/docs.md
--rw-r--r--   0        0        0     1244 2024-02-13 02:29:16.000000 citric-1.0.0/docs/contributing/environment.md
--rw-r--r--   0        0        0     1472 2024-02-13 02:29:16.000000 citric-1.0.0/docs/contributing/getting-started.md
--rw-r--r--   0        0        0      822 2024-02-13 02:29:16.000000 citric-1.0.0/docs/contributing/release.md
--rw-r--r--   0        0        0      626 2024-02-13 02:29:16.000000 citric-1.0.0/docs/contributing/testing.md
--rw-r--r--   0        0        0      881 2024-02-13 02:29:16.000000 citric-1.0.0/docs/contributing/unreleased-features.md
--rw-r--r--   0        0        0       19 2024-02-13 02:29:16.000000 citric-1.0.0/docs/notebooks/.gitignore
--rw-r--r--   0        0        0    18574 2024-02-13 02:29:16.000000 citric-1.0.0/docs/notebooks/duckdb.ipynb
--rw-r--r--   0        0        0     6352 2024-02-13 02:29:16.000000 citric-1.0.0/docs/notebooks/import_s3.ipynb
--rw-r--r--   0        0        0    10331 2024-02-13 02:29:16.000000 citric-1.0.0/docs/notebooks/pandas_sqlite.ipynb
--rw-r--r--   0        0        0     5862 2024-02-13 02:29:16.000000 citric-1.0.0/docs/notebooks/parse_files.ipynb
--rw-r--r--   0        0        0     6976 2024-02-13 02:29:16.000000 citric-1.0.0/examples/free_text.lsq
--rw-r--r--   0        0        0    11072 2024-02-13 02:29:16.000000 citric-1.0.0/examples/group.lsg
--rw-r--r--   0        0        0    24464 2024-02-13 02:29:16.000000 citric-1.0.0/examples/limesurvey_survey_432535.lss
--rw-r--r--   0        0        0    25801 2024-02-13 02:29:16.000000 citric-1.0.0/examples/survey.lss
--rw-r--r--   0        0        0     1824 2024-02-13 02:29:16.000000 citric-1.0.0/scripts/docker_tags.py
--rw-r--r--   0        0        0      299 2024-02-13 02:29:16.000000 citric-1.0.0/src/citric/__init__.py
--rw-r--r--   0        0        0     2450 2024-02-13 02:29:16.000000 citric-1.0.0/src/citric/_compat.py
--rw-r--r--   0        0        0    50489 2024-02-13 02:29:16.000000 citric-1.0.0/src/citric/client.py
--rw-r--r--   0        0        0     2373 2024-02-13 02:29:16.000000 citric-1.0.0/src/citric/enums.py
--rw-r--r--   0        0        0     1192 2024-02-13 02:29:16.000000 citric-1.0.0/src/citric/exceptions.py
--rw-r--r--   0        0        0     1123 2024-02-13 02:29:16.000000 citric-1.0.0/src/citric/method.py
--rw-r--r--   0        0        0     1183 2024-02-13 02:29:16.000000 citric-1.0.0/src/citric/objects.py
--rw-r--r--   0        0        0        0 2024-02-13 02:29:16.000000 citric-1.0.0/src/citric/py.typed
--rw-r--r--   0        0        0     7152 2024-02-13 02:29:16.000000 citric-1.0.0/src/citric/session.py
--rw-r--r--   0        0        0    12698 2024-02-13 02:29:16.000000 citric-1.0.0/src/citric/types.py
--rw-r--r--   0        0        0      128 2024-02-13 02:29:16.000000 citric-1.0.0/src/citric/_rest/__init__.py
--rw-r--r--   0        0        0     5258 2024-02-13 02:29:16.000000 citric-1.0.0/src/citric/_rest/client.py
--rw-r--r--   0        0        0       72 2024-02-13 02:29:16.000000 citric-1.0.0/tests/__init__.py
--rw-r--r--   0        0        0     7402 2024-02-13 02:29:16.000000 citric-1.0.0/tests/conftest.py
--rw-r--r--   0        0        0      498 2024-02-13 02:29:16.000000 citric-1.0.0/tests/fixtures.py
--rw-r--r--   0        0        0    17380 2024-02-13 02:29:16.000000 citric-1.0.0/tests/test_client.py
--rw-r--r--   0        0        0     1034 2024-02-13 02:29:16.000000 citric-1.0.0/tests/test_compat.py
--rw-r--r--   0        0        0     5348 2024-02-13 02:29:16.000000 citric-1.0.0/tests/test_rest.py
--rw-r--r--   0        0        0     5380 2024-02-13 02:29:16.000000 citric-1.0.0/tests/test_rpc.py
--rw-r--r--   0        0        0       38 2024-02-13 02:29:16.000000 citric-1.0.0/tests/integration/__init__.py
--rw-r--r--   0        0        0     1762 2024-02-13 02:29:16.000000 citric-1.0.0/tests/integration/conftest.py
--rw-r--r--   0        0        0     2097 2024-02-13 02:29:16.000000 citric-1.0.0/tests/integration/test_rest_client.py
--rw-r--r--   0        0        0    27436 2024-02-13 02:29:16.000000 citric-1.0.0/tests/integration/test_rpc_client.py
--rw-r--r--   0        0        0     1393 2024-02-13 02:29:16.000000 citric-1.0.0/tests/resources/config.php
--rw-r--r--   0        0        0     1950 2024-02-13 02:29:16.000000 citric-1.0.0/.gitignore
--rw-r--r--   0        0        0      131 2024-02-13 02:29:16.000000 citric-1.0.0/AUTHORS.md
--rw-r--r--   0        0        0     1083 2024-02-13 02:29:16.000000 citric-1.0.0/LICENSE
--rw-r--r--   0        0        0     5434 2024-02-13 02:29:16.000000 citric-1.0.0/README.md
--rw-r--r--   0        0        0     8038 2024-02-13 02:29:16.000000 citric-1.0.0/pyproject.toml
--rw-r--r--   0        0        0     9985 2024-02-13 02:29:16.000000 citric-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0     1081 2024-05-01 17:46:34.000000 citric-1.0.1a1/.changie.yaml
+-rw-r--r--   0        0        0       85 2024-05-01 17:46:34.000000 citric-1.0.1a1/.flake8
+-rw-r--r--   0        0        0       36 2024-05-01 17:46:34.000000 citric-1.0.1a1/.gitattributes
+-rw-r--r--   0        0        0     1699 2024-05-01 17:46:34.000000 citric-1.0.1a1/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      290 2024-05-01 17:46:34.000000 citric-1.0.1a1/.readthedocs.yaml
+-rw-r--r--   0        0        0       54 2024-05-01 17:46:34.000000 citric-1.0.1a1/.sonarcloud.properties
+-rw-r--r--   0        0        0    10546 2024-05-01 17:46:34.000000 citric-1.0.1a1/CHANGELOG.md
+-rw-r--r--   0        0        0      337 2024-05-01 17:46:34.000000 citric-1.0.1a1/CITATION.cff
+-rw-r--r--   0        0        0     5225 2024-05-01 17:46:34.000000 citric-1.0.1a1/CODE_OF_CONDUCT.md
+-rw-r--r--   0        0        0      837 2024-05-01 17:46:34.000000 citric-1.0.1a1/SECURITY.md
+-rw-r--r--   0        0        0      247 2024-05-01 17:46:34.000000 citric-1.0.1a1/codecov.yml
+-rw-r--r--   0        0        0      889 2024-05-01 17:46:34.000000 citric-1.0.1a1/docker-compose.mysql.yml
+-rw-r--r--   0        0        0      323 2024-05-01 17:46:34.000000 citric-1.0.1a1/docker-compose.ref.yml
+-rw-r--r--   0        0        0     1701 2024-05-01 17:46:34.000000 citric-1.0.1a1/docker-compose.yml
+-rw-r--r--   0        0        0     4847 2024-05-01 17:46:34.000000 citric-1.0.1a1/noxfile.py
+-rw-r--r--   0        0        0      491 2024-05-01 17:46:34.000000 citric-1.0.1a1/.changes/0.0.1.md
+-rw-r--r--   0        0        0     1152 2024-05-01 17:46:34.000000 citric-1.0.1a1/.changes/0.0.10.md
+-rw-r--r--   0        0        0      246 2024-05-01 17:46:34.000000 citric-1.0.1a1/.changes/0.0.11.md
+-rw-r--r--   0        0        0      132 2024-05-01 17:46:34.000000 citric-1.0.1a1/.changes/0.0.12.md
+-rw-r--r--   0        0        0      135 2024-05-01 17:46:34.000000 citric-1.0.1a1/.changes/0.0.13.md
+-rw-r--r--   0        0        0      129 2024-05-01 17:46:34.000000 citric-1.0.1a1/.changes/0.0.14.md
+-rw-r--r--   0        0        0      157 2024-05-01 17:46:34.000000 citric-1.0.1a1/.changes/0.0.2.md
+-rw-r--r--   0        0        0      126 2024-05-01 17:46:34.000000 citric-1.0.1a1/.changes/0.0.3.md
+-rw-r--r--   0        0        0      186 2024-05-01 17:46:34.000000 citric-1.0.1a1/.changes/0.0.4.md
+-rw-r--r--   0        0        0      245 2024-05-01 17:46:34.000000 citric-1.0.1a1/.changes/0.0.5.md
+-rw-r--r--   0        0        0      114 2024-05-01 17:46:34.000000 citric-1.0.1a1/.changes/0.0.6.md
+-rw-r--r--   0        0        0      141 2024-05-01 17:46:34.000000 citric-1.0.1a1/.changes/0.0.7.md
+-rw-r--r--   0        0        0      224 2024-05-01 17:46:34.000000 citric-1.0.1a1/.changes/0.0.8.md
+-rw-r--r--   0        0        0      314 2024-05-01 17:46:34.000000 citric-1.0.1a1/.changes/0.0.9.md
+-rw-r--r--   0        0        0      132 2024-05-01 17:46:34.000000 citric-1.0.1a1/.changes/0.1.0.md
+-rw-r--r--   0        0        0      669 2024-05-01 17:46:34.000000 citric-1.0.1a1/.changes/0.10.0.md
+-rw-r--r--   0        0        0      269 2024-05-01 17:46:34.000000 citric-1.0.1a1/.changes/0.2.0.md
+-rw-r--r--   0        0        0      129 2024-05-01 17:46:34.000000 citric-1.0.1a1/.changes/0.3.0.md
+-rw-r--r--   0        0        0      506 2024-05-01 17:46:34.000000 citric-1.0.1a1/.changes/0.4.0.md
+-rw-r--r--   0        0        0      142 2024-05-01 17:46:34.000000 citric-1.0.1a1/.changes/0.4.1.md
+-rw-r--r--   0        0        0      251 2024-05-01 17:46:34.000000 citric-1.0.1a1/.changes/0.4.2.md
+-rw-r--r--   0        0        0      167 2024-05-01 17:46:34.000000 citric-1.0.1a1/.changes/0.4.3.md
+-rw-r--r--   0        0        0      295 2024-05-01 17:46:34.000000 citric-1.0.1a1/.changes/0.4.4.md
+-rw-r--r--   0        0        0      152 2024-05-01 17:46:34.000000 citric-1.0.1a1/.changes/0.4.5.md
+-rw-r--r--   0        0        0      227 2024-05-01 17:46:34.000000 citric-1.0.1a1/.changes/0.5.0.md
+-rw-r--r--   0        0        0      364 2024-05-01 17:46:34.000000 citric-1.0.1a1/.changes/0.6.0.md
+-rw-r--r--   0        0        0      260 2024-05-01 17:46:34.000000 citric-1.0.1a1/.changes/0.7.0.md
+-rw-r--r--   0        0        0      141 2024-05-01 17:46:34.000000 citric-1.0.1a1/.changes/0.7.1-b1.md
+-rw-r--r--   0        0        0      141 2024-05-01 17:46:34.000000 citric-1.0.1a1/.changes/0.7.1-b2.md
+-rw-r--r--   0        0        0      231 2024-05-01 17:46:34.000000 citric-1.0.1a1/.changes/0.7.1-b3.md
+-rw-r--r--   0        0        0      136 2024-05-01 17:46:34.000000 citric-1.0.1a1/.changes/0.7.1.md
+-rw-r--r--   0        0        0      151 2024-05-01 17:46:34.000000 citric-1.0.1a1/.changes/0.7.2.md
+-rw-r--r--   0        0        0      756 2024-05-01 17:46:34.000000 citric-1.0.1a1/.changes/0.8.0.md
+-rw-r--r--   0        0        0      590 2024-05-01 17:46:34.000000 citric-1.0.1a1/.changes/0.9.0.md
+-rw-r--r--   0        0        0      672 2024-05-01 17:46:34.000000 citric-1.0.1a1/.changes/1.0.0.md
+-rw-r--r--   0        0        0      304 2024-05-01 17:46:34.000000 citric-1.0.1a1/.changes/header.tpl.md
+-rw-r--r--   0        0        0        0 2024-05-01 17:46:34.000000 citric-1.0.1a1/.changes/unreleased/.gitkeep
+-rw-r--r--   0        0        0      142 2024-05-01 17:46:34.000000 citric-1.0.1a1/.changes/unreleased/Fixed-20240222-213639.yaml
+-rw-r--r--   0        0        0     2399 2024-05-01 17:46:34.000000 citric-1.0.1a1/.circleci/config.yml
+-rw-r--r--   0        0        0      138 2024-05-01 17:46:34.000000 citric-1.0.1a1/.github/CONTRIBUTING.md
+-rw-r--r--   0        0        0     1326 2024-05-01 17:46:34.000000 citric-1.0.1a1/.github/dependabot.yml
+-rw-r--r--   0        0        0     1007 2024-05-01 17:46:34.000000 citric-1.0.1a1/.github/pull_request_template.md
+-rw-r--r--   0        0        0       59 2024-05-01 17:46:34.000000 citric-1.0.1a1/.github/semantic.yml
+-rw-r--r--   0        0        0     2154 2024-05-01 17:46:34.000000 citric-1.0.1a1/.github/ISSUE_TEMPLATE/BUG.yml
+-rw-r--r--   0        0        0       27 2024-05-01 17:46:34.000000 citric-1.0.1a1/.github/ISSUE_TEMPLATE/config.yml
+-rw-r--r--   0        0        0     1013 2024-05-01 17:46:34.000000 citric-1.0.1a1/.github/ISSUE_TEMPLATE/feature.yml
+-rw-r--r--   0        0        0     1044 2024-05-01 17:46:34.000000 citric-1.0.1a1/.github/actions/install-tools/action.yml
+-rw-r--r--   0        0        0        0 2024-05-01 17:46:34.000000 citric-1.0.1a1/.github/badges/.gitkeep
+-rw-r--r--   0        0        0     1295 2024-05-01 17:46:34.000000 citric-1.0.1a1/.github/workflows/api-changes.yml
+-rw-r--r--   0        0        0     2121 2024-05-01 17:46:34.000000 citric-1.0.1a1/.github/workflows/build.yml
+-rw-r--r--   0        0        0       68 2024-05-01 17:46:34.000000 citric-1.0.1a1/.github/workflows/constraints.txt
+-rw-r--r--   0        0        0     3461 2024-05-01 17:46:34.000000 citric-1.0.1a1/.github/workflows/gen-release-pr.yml
+-rw-r--r--   0        0        0      319 2024-05-01 17:46:34.000000 citric-1.0.1a1/.github/workflows/pr-preview-links.yml
+-rw-r--r--   0        0        0     2891 2024-05-01 17:46:34.000000 citric-1.0.1a1/.github/workflows/scorecard.yml
+-rw-r--r--   0        0        0    10275 2024-05-01 17:46:34.000000 citric-1.0.1a1/.github/workflows/tests.yml
+-rw-r--r--   0        0        0      267 2024-05-01 17:46:34.000000 citric-1.0.1a1/code_samples/auth_plugin.py
+-rw-r--r--   0        0        0      336 2024-05-01 17:46:34.000000 citric-1.0.1a1/code_samples/context_manager.py
+-rw-r--r--   0        0        0      563 2024-05-01 17:46:34.000000 citric-1.0.1a1/code_samples/custom_requests_session.py
+-rw-r--r--   0        0        0      626 2024-05-01 17:46:34.000000 citric-1.0.1a1/code_samples/duckdb_sql.py
+-rw-r--r--   0        0        0      573 2024-05-01 17:46:34.000000 citric-1.0.1a1/code_samples/get_surveys.py
+-rw-r--r--   0        0        0      583 2024-05-01 17:46:34.000000 citric-1.0.1a1/code_samples/pandas_df.py
+-rw-r--r--   0        0        0      517 2024-05-01 17:46:34.000000 citric-1.0.1a1/code_samples/requests_session_attributes.py
+-rw-r--r--   0        0        0      159 2024-05-01 17:46:34.000000 citric-1.0.1a1/code_samples/ruff.toml
+-rw-r--r--   0        0        0      521 2024-05-01 17:46:34.000000 citric-1.0.1a1/code_samples/session_attr.py
+-rw-r--r--   0        0        0      561 2024-05-01 17:46:34.000000 citric-1.0.1a1/code_samples/upload_s3.py
+-rw-r--r--   0        0        0       33 2024-05-01 17:46:34.000000 citric-1.0.1a1/docs/changelog.md
+-rw-r--r--   0        0        0   106926 2024-05-01 17:46:34.000000 citric-1.0.1a1/docs/code.png
+-rw-r--r--   0        0        0     6110 2024-05-01 17:46:34.000000 citric-1.0.1a1/docs/conf.py
+-rw-r--r--   0        0        0       54 2024-05-01 17:46:34.000000 citric-1.0.1a1/docs/googled10b55fb460af091.html
+-rw-r--r--   0        0        0     2876 2024-05-01 17:46:34.000000 citric-1.0.1a1/docs/how-to.md
+-rw-r--r--   0        0        0     2571 2024-05-01 17:46:34.000000 citric-1.0.1a1/docs/index.md
+-rw-r--r--   0        0        0       41 2024-05-01 17:46:34.000000 citric-1.0.1a1/docs/license.rst
+-rw-r--r--   0        0        0     2080 2024-05-01 17:46:34.000000 citric-1.0.1a1/docs/requirements.txt
+-rw-r--r--   0        0        0      740 2024-05-01 17:46:34.000000 citric-1.0.1a1/docs/rest_coverage.md
+-rw-r--r--   0        0        0    11121 2024-05-01 17:46:34.000000 citric-1.0.1a1/docs/rpc_coverage.md
+-rw-r--r--   0        0        0        0 2024-05-01 17:46:34.000000 citric-1.0.1a1/docs/_ext/__init__.py
+-rw-r--r--   0        0        0     2521 2024-05-01 17:46:34.000000 citric-1.0.1a1/docs/_ext/limesurvey_future.py
+-rw-r--r--   0        0        0       42 2024-05-01 17:46:34.000000 citric-1.0.1a1/docs/contributing/code-of-conduct.md
+-rw-r--r--   0        0        0     2418 2024-05-01 17:46:34.000000 citric-1.0.1a1/docs/contributing/docker.md
+-rw-r--r--   0        0        0      299 2024-05-01 17:46:34.000000 citric-1.0.1a1/docs/contributing/docs.md
+-rw-r--r--   0        0        0     1244 2024-05-01 17:46:34.000000 citric-1.0.1a1/docs/contributing/environment.md
+-rw-r--r--   0        0        0     1472 2024-05-01 17:46:34.000000 citric-1.0.1a1/docs/contributing/getting-started.md
+-rw-r--r--   0        0        0      822 2024-05-01 17:46:34.000000 citric-1.0.1a1/docs/contributing/release.md
+-rw-r--r--   0        0        0      626 2024-05-01 17:46:34.000000 citric-1.0.1a1/docs/contributing/testing.md
+-rw-r--r--   0        0        0      881 2024-05-01 17:46:34.000000 citric-1.0.1a1/docs/contributing/unreleased-features.md
+-rw-r--r--   0        0        0       19 2024-05-01 17:46:34.000000 citric-1.0.1a1/docs/notebooks/.gitignore
+-rw-r--r--   0        0        0    18574 2024-05-01 17:46:34.000000 citric-1.0.1a1/docs/notebooks/duckdb.ipynb
+-rw-r--r--   0        0        0     6352 2024-05-01 17:46:34.000000 citric-1.0.1a1/docs/notebooks/import_s3.ipynb
+-rw-r--r--   0        0        0    10331 2024-05-01 17:46:34.000000 citric-1.0.1a1/docs/notebooks/pandas_sqlite.ipynb
+-rw-r--r--   0        0        0     5862 2024-05-01 17:46:34.000000 citric-1.0.1a1/docs/notebooks/parse_files.ipynb
+-rw-r--r--   0        0        0     6976 2024-05-01 17:46:34.000000 citric-1.0.1a1/examples/free_text.lsq
+-rw-r--r--   0        0        0    11072 2024-05-01 17:46:34.000000 citric-1.0.1a1/examples/group.lsg
+-rw-r--r--   0        0        0    24464 2024-05-01 17:46:34.000000 citric-1.0.1a1/examples/limesurvey_survey_432535.lss
+-rw-r--r--   0        0        0    25801 2024-05-01 17:46:34.000000 citric-1.0.1a1/examples/survey.lss
+-rw-r--r--   0        0        0     1824 2024-05-01 17:46:34.000000 citric-1.0.1a1/scripts/docker_tags.py
+-rw-r--r--   0        0        0      299 2024-05-01 17:46:34.000000 citric-1.0.1a1/src/citric/__init__.py
+-rw-r--r--   0        0        0     2450 2024-05-01 17:46:34.000000 citric-1.0.1a1/src/citric/_compat.py
+-rw-r--r--   0        0        0    50489 2024-05-01 17:46:34.000000 citric-1.0.1a1/src/citric/client.py
+-rw-r--r--   0        0        0     2373 2024-05-01 17:46:34.000000 citric-1.0.1a1/src/citric/enums.py
+-rw-r--r--   0        0        0     1192 2024-05-01 17:46:34.000000 citric-1.0.1a1/src/citric/exceptions.py
+-rw-r--r--   0        0        0     1123 2024-05-01 17:46:34.000000 citric-1.0.1a1/src/citric/method.py
+-rw-r--r--   0        0        0     1183 2024-05-01 17:46:34.000000 citric-1.0.1a1/src/citric/objects.py
+-rw-r--r--   0        0        0        0 2024-05-01 17:46:34.000000 citric-1.0.1a1/src/citric/py.typed
+-rw-r--r--   0        0        0     7152 2024-05-01 17:46:34.000000 citric-1.0.1a1/src/citric/session.py
+-rw-r--r--   0        0        0    12698 2024-05-01 17:46:34.000000 citric-1.0.1a1/src/citric/types.py
+-rw-r--r--   0        0        0      128 2024-05-01 17:46:34.000000 citric-1.0.1a1/src/citric/_rest/__init__.py
+-rw-r--r--   0        0        0     5258 2024-05-01 17:46:34.000000 citric-1.0.1a1/src/citric/_rest/client.py
+-rw-r--r--   0        0        0       72 2024-05-01 17:46:34.000000 citric-1.0.1a1/tests/__init__.py
+-rw-r--r--   0        0        0     7664 2024-05-01 17:46:34.000000 citric-1.0.1a1/tests/conftest.py
+-rw-r--r--   0        0        0      498 2024-05-01 17:46:34.000000 citric-1.0.1a1/tests/fixtures.py
+-rw-r--r--   0        0        0    17380 2024-05-01 17:46:34.000000 citric-1.0.1a1/tests/test_client.py
+-rw-r--r--   0        0        0     1034 2024-05-01 17:46:34.000000 citric-1.0.1a1/tests/test_compat.py
+-rw-r--r--   0        0        0     5348 2024-05-01 17:46:34.000000 citric-1.0.1a1/tests/test_rest.py
+-rw-r--r--   0        0        0     5380 2024-05-01 17:46:34.000000 citric-1.0.1a1/tests/test_rpc.py
+-rw-r--r--   0        0        0       38 2024-05-01 17:46:34.000000 citric-1.0.1a1/tests/integration/__init__.py
+-rw-r--r--   0        0        0     1762 2024-05-01 17:46:34.000000 citric-1.0.1a1/tests/integration/conftest.py
+-rw-r--r--   0        0        0     2231 2024-05-01 17:46:34.000000 citric-1.0.1a1/tests/integration/test_rest_client.py
+-rw-r--r--   0        0        0    27436 2024-05-01 17:46:34.000000 citric-1.0.1a1/tests/integration/test_rpc_client.py
+-rw-r--r--   0        0        0     1393 2024-05-01 17:46:34.000000 citric-1.0.1a1/tests/resources/config.php
+-rw-r--r--   0        0        0     1950 2024-05-01 17:46:34.000000 citric-1.0.1a1/.gitignore
+-rw-r--r--   0        0        0      131 2024-05-01 17:46:34.000000 citric-1.0.1a1/AUTHORS.md
+-rw-r--r--   0        0        0     1083 2024-05-01 17:46:34.000000 citric-1.0.1a1/LICENSE
+-rw-r--r--   0        0        0     5453 2024-05-01 17:46:34.000000 citric-1.0.1a1/README.md
+-rw-r--r--   0        0        0     8059 2024-05-01 17:46:34.000000 citric-1.0.1a1/pyproject.toml
+-rw-r--r--   0        0        0    11802 2024-05-01 17:46:34.000000 citric-1.0.1a1/PKG-INFO
```

### Comparing `citric-1.0.0/.changie.yaml` & `citric-1.0.1a1/.changie.yaml`

 * *Files identical despite different names*

### Comparing `citric-1.0.0/.pre-commit-config.yaml` & `citric-1.0.1a1/.pre-commit-config.yaml`

 * *Files 6% similar despite different names*

```diff
@@ -17,22 +17,22 @@
   - id: end-of-file-fixer
     exclude: \.changes/.*\.md
   - id: no-commit-to-branch
     args: [--branch, main]
   - id: trailing-whitespace
 
 - repo: https://github.com/python-jsonschema/check-jsonschema
-  rev: 0.28.0
+  rev: 0.28.1
   hooks:
   - id: check-dependabot
   - id: check-github-workflows
   - id: check-readthedocs
 
 - repo: https://github.com/astral-sh/ruff-pre-commit
-  rev: v0.2.1
+  rev: v0.3.5
   hooks:
   - id: ruff
     name: Ruff lint
     args: [--fix, --exit-non-zero-on-fix, --show-fixes]
   - id: ruff
     name: Ruff format
     entry: ruff format
@@ -45,32 +45,32 @@
     - tomli
 
 - repo: https://github.com/pycqa/flake8
   rev: 7.0.0
   hooks:
   - id: flake8
     additional_dependencies:
-    - pydoclint==0.3.9
+    - pydoclint==0.4.1
 
 - repo: https://github.com/pre-commit/pre-commit
-  rev: v3.6.0
+  rev: v3.7.0
   hooks:
   - id: validate_manifest
 
 - repo: https://github.com/hadialqattan/pycln
   rev: v2.4.0
   hooks:
   - id: pycln
     args: [--all]
 
 - repo: https://github.com/tox-dev/pyproject-fmt
   rev: "1.7.0"
   hooks:
   - id: pyproject-fmt
 
-- repo: https://github.com/jazzband/pip-tools
-  rev: 7.3.0
+- repo: https://github.com/astral-sh/uv-pre-commit
+  rev: 0.1.26
   hooks:
   - id: pip-compile
     files: ^pyproject\.toml$
-    args: ["--extra", "docs", "-o", "docs/requirements.txt", "--pre"]
+    args: ["pyproject.toml", "--extra", "docs", "-o", "docs/requirements.txt"]
     language_version: python3.12
```

### Comparing `citric-1.0.0/CHANGELOG.md` & `citric-1.0.1a1/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `citric-1.0.0/CODE_OF_CONDUCT.md` & `citric-1.0.1a1/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `citric-1.0.0/SECURITY.md` & `citric-1.0.1a1/SECURITY.md`

 * *Files identical despite different names*

### Comparing `citric-1.0.0/docker-compose.mysql.yml` & `citric-1.0.1a1/docker-compose.mysql.yml`

 * *Files identical despite different names*

### Comparing `citric-1.0.0/docker-compose.yml` & `citric-1.0.1a1/docker-compose.yml`

 * *Files 12% similar despite different names*

```diff
@@ -22,33 +22,33 @@
       ADMIN_NAME: Lime Administrator
       ADMIN_PASSWORD: ${LS_PASSWORD:-secret}
       EMAIL_SMTPHOST: ${LS_SMTP_HOST:-mailhog:1025}
       EMAIL_SMTPUSER: ${LS_SMTP_USER:-citric@example.com}
       EMAIL_SMTPPASSWORD: ${LS_SMTP_PASSWORD:-secret}
     healthcheck:
       test: ["CMD", "curl", "-f", "http://localhost:8080/index.php/admin"]
-      interval: 30s
+      interval: 15s
       timeout: 10s
       retries: 3
-      start_period: 15s
+      start_period: 5s
 
   db:
     image: postgres:16
     environment:
       POSTGRES_USER: limesurvey
       POSTGRES_DB: limesurvey
       POSTGRES_PASSWORD: secret
     volumes:
       - "limedb:/var/lib/postgresql/data"
     ports:
       - 5432:5432
     healthcheck:
       test: ["CMD", "pg_isready", "-U", "limesurvey"]
-      interval: 30s
-      timeout: 30s
+      interval: 15s
+      timeout: 10s
       retries: 3
 
   storage:
     image: quay.io/minio/minio:latest
     volumes:
       - "object_storage:/data/"
     ports:
```

### Comparing `citric-1.0.0/noxfile.py` & `citric-1.0.1a1/noxfile.py`

 * *Files 22% similar despite different names*

```diff
@@ -2,157 +2,159 @@
 
 from __future__ import annotations
 
 import os
 import shutil
 from pathlib import Path
 
-from nox import Session, session
+import nox
 
 GH_ACTIONS_ENV_VAR = "GITHUB_ACTIONS"
 FORCE_COLOR = "FORCE_COLOR"
 
+nox.options.default_venv_backend = "uv"
+
 package = "citric"
 
 python_versions = ["3.13", "3.12", "3.11", "3.10", "3.9", "3.8"]
 pypy_versions = ["pypy3.9", "pypy3.10"]
 all_python_versions = python_versions + pypy_versions
 
 main_cpython_version = "3.12"
 main_pypy_version = "pypy3.9"
 
 locations = "src", "tests", "noxfile.py", "docs/conf.py"
 
 
-def _run_tests(session: Session, *args: str) -> None:
-    env = {"COVERAGE_CORE": "sysmon"} if session.python in {"3.12", "3.13"} else {}
+def _run_tests(session: nox.Session, *args: str) -> None:
+    env = {"COVERAGE_CORE": "sysmon"}
     try:
         session.run("coverage", "run", "-m", "pytest", *args, env=env)
     finally:
         if session.interactive:
             session.notify("coverage", posargs=[])
 
 
-@session(python=all_python_versions, tags=["test"])
-def tests(session: Session) -> None:
+@nox.session(python=all_python_versions, tags=["test"])
+def tests(session: nox.Session) -> None:
     """Execute pytest tests and compute coverage."""
-    session.install(".[tests]")
+    session.install("-v", "citric[tests] @ .")
     args = session.posargs or ["-m", "not integration_test"]
     _run_tests(session, *args)
 
 
-@session(python=[main_cpython_version, main_pypy_version], tags=["test"])
-def integration(session: Session) -> None:
+@nox.session(python=[main_cpython_version, main_pypy_version], tags=["test"])
+def integration(session: nox.Session) -> None:
     """Execute integration tests and compute coverage."""
-    session.install(".[tests]")
+    session.install("-v", "citric[tests] @ .")
     args = session.posargs or ["-m", "integration_test"]
     _run_tests(session, *args)
 
 
-@session(python=[main_cpython_version, main_pypy_version], tags=["test"])
-def xdoctest(session: Session) -> None:
+@nox.session(python=[main_cpython_version, main_pypy_version], tags=["test"])
+def xdoctest(session: nox.Session) -> None:
     """Run examples with xdoctest."""
     if session.posargs:
         args = [package, *session.posargs]
     else:
         args = [f"--modname={package}", "--command=all"]
         if FORCE_COLOR in os.environ:
             args.append("--colored=1")
 
-    session.install(".")
-    session.install("xdoctest[colors]")
+    session.install("-v", "citric @ .")
+    session.install("-v", "xdoctest[colors]")
     session.run("python", "-m", "xdoctest", *args)
 
 
-@session()
-def coverage(session: Session) -> None:
+@nox.session()
+def coverage(session: nox.Session) -> None:
     """Upload coverage data."""
     args = session.posargs or ["report"]
 
-    session.install("coverage[toml]")
+    session.install("-v", "coverage[toml]")
 
     if not session.posargs and any(Path().glob(".coverage.*")):
         session.run("coverage", "combine", "--debug=pathmap")
 
     session.run("coverage", *args)
 
 
-@session(name="deps", python=python_versions)
-def dependencies(session: Session) -> None:
+@nox.session(name="deps", python=python_versions)
+def dependencies(session: nox.Session) -> None:
     """Check issues with dependencies."""
-    session.install(".[dev]")
-    session.install("deptry")
+    session.install("-v", "citric[dev] @ .")
+    session.install("-v", "deptry")
     session.run("deptry", "src", "tests", "docs")
 
 
-@session(python=python_versions, tags=["lint"])
-def mypy(session: Session) -> None:
+@nox.session(python=python_versions, tags=["lint"])
+def mypy(session: nox.Session) -> None:
     """Type-check using mypy."""
     args = session.posargs or locations
-    session.install(".[typing]")
+    session.install("-v", "citric[typing] @ .")
     session.run("mypy", *args)
 
 
-@session(name="docs-build")
-def docs_build(session: Session) -> None:
+@nox.session(name="docs-build")
+def docs_build(session: nox.Session) -> None:
     """Build the documentation."""
     args = session.posargs or ["docs", "build"]
     if not session.posargs and FORCE_COLOR in os.environ:
         args.insert(0, "--color")
 
-    session.install(".[docs]")
+    session.install("-v", "citric[docs] @ .")
 
     build_dir = Path("build")
     if build_dir.exists():
         shutil.rmtree(build_dir)
 
     session.run("sphinx-build", *args)
 
 
-@session(name="docs-serve")
-def docs_serve(session: Session) -> None:
+@nox.session(name="docs-serve")
+def docs_serve(session: nox.Session) -> None:
     """Build the documentation."""
     args = session.posargs or [
         "--open-browser",
         "--watch",
         ".",
         "--ignore",
         "**/.nox/*",
         "--ignore",
         "**/.mypy_cache/*",
         "docs",
         "build",
     ]
-    session.install(".[docs]")
+    session.install("-v", "citric[docs] @ .")
 
     build_dir = Path("build")
     if build_dir.exists():
         shutil.rmtree(build_dir)
 
     session.run("sphinx-autobuild", *args)
 
 
-@session(name="api")
-def api_changes(session: Session) -> None:
+@nox.session(name="api")
+def api_changes(session: nox.Session) -> None:
     """Check for API changes."""
     args = [
         "griffe",
         "check",
         "citric",
         "-s=src",
     ]
 
     if session.posargs:
         args.append(f"-a={session.posargs[0]}")
 
     session.run(*args, external=True)
 
 
-@session(python=["3.11"])
-def notebook(session: Session) -> None:
+@nox.session(python=["3.11"])
+def notebook(session: nox.Session) -> None:
     """Start a Jupyter notebook."""
     session.install(
         "boto3",
         "duckdb",
         "duckdb-engine",
         "faker",
         "jupysql",
@@ -170,12 +172,12 @@
             "AWS_ENDPOINT_URL": "http://localhost:9000",
             "AWS_ACCESS_KEY_ID": "minioadmin",
             "AWS_SECRET_ACCESS_KEY": "minioadmin",
         },
     )
 
 
-@session(name="generate-tags", tags=["status"])
-def tags(session: Session) -> None:
+@nox.session(name="generate-tags", tags=["status"])
+def tags(session: nox.Session) -> None:
     """Print tags."""
-    session.install("requests", "requests-cache")
+    session.install("-v", "requests", "requests-cache")
     session.run("python", "scripts/docker_tags.py")
```

### Comparing `citric-1.0.0/.changes/0.0.10.md` & `citric-1.0.1a1/.changes/0.0.10.md`

 * *Files identical despite different names*

### Comparing `citric-1.0.0/.changes/0.10.0.md` & `citric-1.0.1a1/.changes/0.10.0.md`

 * *Files identical despite different names*

### Comparing `citric-1.0.0/.changes/0.8.0.md` & `citric-1.0.1a1/.changes/0.8.0.md`

 * *Files identical despite different names*

### Comparing `citric-1.0.0/.changes/0.9.0.md` & `citric-1.0.1a1/.changes/0.9.0.md`

 * *Files identical despite different names*

### Comparing `citric-1.0.0/.changes/1.0.0.md` & `citric-1.0.1a1/.changes/1.0.0.md`

 * *Files identical despite different names*

### Comparing `citric-1.0.0/.circleci/config.yml` & `citric-1.0.1a1/.circleci/config.yml`

 * *Files identical despite different names*

### Comparing `citric-1.0.0/.github/dependabot.yml` & `citric-1.0.1a1/.github/dependabot.yml`

 * *Files identical despite different names*

### Comparing `citric-1.0.0/.github/ISSUE_TEMPLATE/BUG.yml` & `citric-1.0.1a1/.github/ISSUE_TEMPLATE/BUG.yml`

 * *Files identical despite different names*

### Comparing `citric-1.0.0/.github/ISSUE_TEMPLATE/feature.yml` & `citric-1.0.1a1/.github/ISSUE_TEMPLATE/feature.yml`

 * *Files identical despite different names*

### Comparing `citric-1.0.0/.github/actions/install-tools/action.yml` & `citric-1.0.1a1/.github/actions/install-tools/action.yml`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 name: Install tools
 description: Install tools for Python projects
 
 inputs:
   constraints:
-    default: ".github/workflows/constraints.txt"
+    default: "${{ github.workspace }}/.github/workflows/constraints.txt"
     description: "Path to pip constraints file"
     required: true
   os:
     default: "ubuntu-latest"
     description: "Operating system"
     required: true
 
@@ -34,7 +34,15 @@
   - name: Install Nox
     shell: bash
     env:
       PIP_CONSTRAINT: ${{ inputs.constraints }}
     run: |
       pipx install nox
       nox --version
+
+  - name: Install uv
+    shell: bash
+    env:
+      PIP_CONSTRAINT: ${{ inputs.constraints }}
+    run: |
+      pipx install uv
+      uv --version
```

### Comparing `citric-1.0.0/.github/workflows/api-changes.yml` & `citric-1.0.1a1/.github/workflows/api-changes.yml`

 * *Files 16% similar despite different names*

```diff
@@ -18,30 +18,29 @@
   check-api-changes:
     name: Check API Changes
     runs-on: ubuntu-latest
     env:
       NOXSESSION: api
     steps:
     - name: Check out the repository
-      uses: actions/checkout@b4ffde65f46336ab88eb53be808477a3936bae11 # v4.1.1
+      uses: actions/checkout@0ad4b8fadaa221de15dcec353f45205ec38ea70b
       with:
         fetch-depth: 0
 
     - name: Setup Python
-      uses: actions/setup-python@0a5c61591373683505ea898e09a3ea4f39ef2b9c # v5.0.0
+      uses: actions/setup-python@82c7e631bb3cdc910f68e0081d67478d79c6982d
       with:
         python-version: 3.12
 
     - name: Install tools
       env:
-        PIP_CONSTRAINT: .github/workflows/constraints.txt
+        PIP_CONSTRAINT: ${{ github.workspace }}/.github/workflows/constraints.txt
       run: |
         python -Im pip install -U pip
-        pipx install griffe
-        pipx install nox
+        pipx install griffe nox uv
         pipx list
 
     - name: Set REF
       id: set-ref
       if: always() && !startsWith(github.head_ref, 'release/')
       run: |
         echo "ref=${{ github.event.pull_request.base.sha }}" >> $GITHUB_OUTPUT
```

### Comparing `citric-1.0.0/.github/workflows/build.yml` & `citric-1.0.1a1/.github/workflows/build.yml`

 * *Files 25% similar despite different names*

```diff
@@ -16,57 +16,57 @@
 permissions: read-all
 
 jobs:
   build:
     name: Build wheel and sdist
     runs-on: ubuntu-latest
     steps:
-    - uses: actions/checkout@b4ffde65f46336ab88eb53be808477a3936bae11 # v4.1.1
+    - uses: actions/checkout@0ad4b8fadaa221de15dcec353f45205ec38ea70b
       with:
         fetch-depth: 0
         ref: ${{ github.event.inputs.tag || github.ref }}
-    - uses: hynek/build-and-inspect-python-package@3a76fe0f90ca169edffd7d518137a64c0c4a3a41 # v2.0.1
+    - uses: hynek/build-and-inspect-python-package@eb6b0c7cc5e1f38eec42c970925e1b3420faa015
 
   publish:
     name: Publish to PyPI
     if: startsWith(github.ref, 'refs/tags/') || github.event.inputs.publish == 'true'
     runs-on: ubuntu-latest
     needs: [build]
     environment:
       name: pypi
       url: https://pypi.org/p/citric
     permissions:
       id-token: write # IMPORTANT: mandatory for trusted publishing
 
     steps:
-    - uses: actions/download-artifact@6b208ae046db98c579e8a3aa621ab581ff575935 # v4.1.1
+    - uses: actions/download-artifact@65a9edc5881444af0b9093a5e628f2fe47ea3b2e
       with:
         name: Packages
         path: dist
-    - uses: pypa/gh-action-pypi-publish@2f6f737ca5f74c637829c0f5c3acd0e29ea5e8bf # v1.8.11
+    - uses: pypa/gh-action-pypi-publish@81e9d935c883d0b210363ab89cf05f3894778450
 
   # Move this up when PyPI supports signing
   sign:
     name: Sign the distribution package
     if: startsWith(github.ref, 'refs/tags/') || github.event_name == 'workflow_dispatch'
     runs-on: ubuntu-latest
     needs: [build]
     permissions:
       contents: write # IMPORTANT: mandatory for making GitHub Releases
       id-token: write # IMPORTANT: mandatory for sigstore
 
     steps:
-      - uses: actions/download-artifact@6b208ae046db98c579e8a3aa621ab581ff575935 # v4.1.1
+      - uses: actions/download-artifact@65a9edc5881444af0b9093a5e628f2fe47ea3b2e
         with:
           name: Packages
           path: dist
-      - uses: sigstore/gh-action-sigstore-python@61f6a500bbfdd9a2a339cf033e5421951fbc1cd2 # v2.1.1
+      - uses: sigstore/gh-action-sigstore-python@61f6a500bbfdd9a2a339cf033e5421951fbc1cd2
         with:
           inputs: >-
             ./dist/*.tar.gz
             ./dist/*.whl
-      - uses: svenstaro/upload-release-action@1beeb572c19a9242f4361f4cee78f8e0d9aec5df # v2
+      - uses: svenstaro/upload-release-action@04733e069f2d7f7f0b4aebc4fbdbce8613b03ccd
         with:
           file: dist/**
           tag: ${{ github.event.inputs.tag || github.ref }}
           overwrite: false
           file_glob: true
```

### Comparing `citric-1.0.0/.github/workflows/gen-release-pr.yml` & `citric-1.0.1a1/.github/workflows/gen-release-pr.yml`

 * *Files 8% similar despite different names*

```diff
@@ -14,72 +14,73 @@
       prerelease:
         description: Prerelease values to append to version
         required: false
       metadata:
         description: Metadata values to append to version
         required: false
 
-permissions:
-  contents: write       # to create a github release
-  pull-requests: write  # to create and update PRs
-  discussions: write    # to create a discussion
+permissions: read-all
 
 jobs:
   generate-pr:
     runs-on: ubuntu-latest
+    permissions:
+      contents: write       # to create a github release
+      pull-requests: write  # to create and update PRs
+      discussions: write    # to create a discussion
     steps:
-    - uses: actions/checkout@b4ffde65f46336ab88eb53be808477a3936bae11 # v4.1.1
+    - uses: actions/checkout@0ad4b8fadaa221de15dcec353f45205ec38ea70b
     - name: Batch changes
-      uses: miniscruff/changie-action@6dcc2533cac0495148ed4046c438487e4dceaa23 # v2.0.0
+      uses: miniscruff/changie-action@6dcc2533cac0495148ed4046c438487e4dceaa23
       with:
         version: ${{ github.event.inputs.changie-version }}
         args: "\
           batch
           ${{ github.event.inputs.next-version }}
           ${{ github.event.inputs.prerelease && format('-p {0}', github.event.inputs.prerelease) }}
           ${{ github.event.inputs.metadata && format('-m {0}', github.event.inputs.metadata) }}"
       env:
         GITHUB_TOKEN: ${{ secrets.GITHUB_TOKEN }}
 
     - name: Merge changes
-      uses: miniscruff/changie-action@6dcc2533cac0495148ed4046c438487e4dceaa23 # v2.0.0
+      uses: miniscruff/changie-action@6dcc2533cac0495148ed4046c438487e4dceaa23
       with:
         version: ${{ github.event.inputs.changie-version }}
         args: merge
       env:
         GITHUB_TOKEN: ${{ secrets.GITHUB_TOKEN }}
 
     - name: Get the latest version
       id: latest
-      uses: miniscruff/changie-action@6dcc2533cac0495148ed4046c438487e4dceaa23 # v2.0.0
+      uses: miniscruff/changie-action@6dcc2533cac0495148ed4046c438487e4dceaa23
       with:
         version: ${{ github.event.inputs.changie-version }}
         args: latest
       env:
         GITHUB_TOKEN: ${{ secrets.GITHUB_TOKEN }}
 
     - name: Draft Release
       id: draft-release
-      uses: softprops/action-gh-release@de2c0eb89ae2a093876385947365aca7b0e5f844 # v1
+      uses: softprops/action-gh-release@9d7c94cfd0a1f3ed45544c887983e9fa900f0564
       with:
         draft: true
         body_path: ".changes/${{ steps.latest.outputs.output }}.md"
         tag_name: ${{ steps.latest.outputs.output }}
         prerelease: "${{ github.event.inputs.prerelease != '' }}"
       env:
         GITHUB_TOKEN: ${{ secrets.GITHUB_TOKEN }}
 
-    - uses: tibdex/github-app-token@3beb63f4bd073e61482598c45c71c1019b59b73a # v2.1.0
+    - uses: tibdex/github-app-token@3beb63f4bd073e61482598c45c71c1019b59b73a
       id: generate-token
       with:
         app_id: ${{ secrets.APP_ID }}
         private_key: ${{ secrets.APP_PRIVATE_KEY }}
 
     - name: Create Pull Request
-      uses: peter-evans/create-pull-request@b1ddad2c994a25fbc81a28b3ec0e368bb2021c50 # v6.0.0
+      uses: peter-evans/create-pull-request@6d6857d36972b65feb161a90e484f2984215f83e
       with:
         token: ${{ steps.generate-token.outputs.token }}
         title: "chore: Release ${{ steps.latest.outputs.output }}"
         branch: release/${{ steps.latest.outputs.output }}
         commit-message: "chore: Release ${{ steps.latest.outputs.output }}"
         body: |
           Prepare release for `${{ steps.latest.outputs.output }}`.
```

### Comparing `citric-1.0.0/.github/workflows/scorecard.yml` & `citric-1.0.1a1/.github/workflows/scorecard.yml`

 * *Files 8% similar despite different names*

```diff
@@ -29,20 +29,20 @@
       id-token: write
       # Uncomment the permissions below if installing in a private repository.
       # contents: read
       # actions: read
 
     steps:
     - name: "Checkout code"
-      uses: actions/checkout@b4ffde65f46336ab88eb53be808477a3936bae11 # v4.1.1
+      uses: actions/checkout@0ad4b8fadaa221de15dcec353f45205ec38ea70b
       with:
         persist-credentials: false
 
     - name: "Run analysis"
-      uses: ossf/scorecard-action@0864cf19026789058feabb7e87baa5f140aac736 # v2.3.1
+      uses: ossf/scorecard-action@0864cf19026789058feabb7e87baa5f140aac736
       with:
         results_file: results.sarif
         results_format: sarif
         # (Optional) "write" PAT token. Uncomment the `repo_token` line below if:
         # - you want to enable the Branch-Protection check on a *public* repository, or
         # - you are installing Scorecard on a *private* repository
         # To create the PAT, follow the steps in https://github.com/ossf/scorecard-action#authentication-with-pat.
@@ -56,18 +56,18 @@
         #   - `publish_results` will always be set to `false`, regardless
         #     of the value entered here.
         publish_results: true
 
     # Upload the results as artifacts (optional). Commenting out will disable uploads of run results in SARIF
     # format to the repository Actions tab.
     - name: "Upload artifact"
-      uses: actions/upload-artifact@26f96dfa697d77e81fd5907df203aa23a56210a8 # v4.3.0
+      uses: actions/upload-artifact@65462800fd760344b1a7b4382951275a0abb4808
       with:
         name: SARIF file
         path: results.sarif
         retention-days: 5
 
     # Upload the results to GitHub's code scanning dashboard.
     - name: "Upload to code-scanning"
-      uses: github/codeql-action/upload-sarif@b7bf0a3ed3ecfa44160715d7c442788f65f0f923 # v3.23.2
+      uses: github/codeql-action/upload-sarif@d39d31e687223d841ef683f52467bd88e9b21c14
       with:
         sarif_file: results.sarif
```

### Comparing `citric-1.0.0/.github/workflows/tests.yml` & `citric-1.0.1a1/.github/workflows/tests.yml`

 * *Files 9% similar despite different names*

```diff
@@ -7,25 +7,27 @@
     - src/**
     - tests/**
     - docker-compose*.yml
     - noxfile.py
     - pyproject.toml
     - .github/workflows/tests.yml
     - .github/workflows/constraints.txt
+    - .github/actions/install-tools/action.yml
   push:
     branches:
     - 'main'
     paths:
     - src/**
     - tests/**
     - docker-compose*.yml
     - noxfile.py
     - pyproject.toml
     - .github/workflows/tests.yml
     - .github/workflows/constraints.txt
+    - .github/actions/install-tools/action.yml
   schedule:
   - cron: "25 7 */3 * *"
   workflow_dispatch:
     inputs:
       all_integrations:
         description: "Test against all the latest LimeSurvey docker image tags and all database engines"
         required: true
@@ -72,20 +74,20 @@
 
         - python-version: "3.12"
           os: "macos-latest"
           session: "tests"
 
     steps:
     - name: Check out the repository
-      uses: actions/checkout@b4ffde65f46336ab88eb53be808477a3936bae11 # v4.1.1
+      uses: actions/checkout@0ad4b8fadaa221de15dcec353f45205ec38ea70b
       with:
         fetch-tags: true
 
     - name: Setup Python ${{ matrix.python-version }}
-      uses: actions/setup-python@0a5c61591373683505ea898e09a3ea4f39ef2b9c # v5.0.0
+      uses: actions/setup-python@82c7e631bb3cdc910f68e0081d67478d79c6982d
       with:
         python-version: ${{ matrix.python-version }}
         architecture: x64
         allow-prereleases: true
         cache: pip
         cache-dependency-path: |
           pyproject.toml
@@ -95,15 +97,15 @@
       uses: ./.github/actions/install-tools
 
     - name: Run Tests
       run: |
         nox --verbose -s tests
 
     - name: Upload coverage data
-      uses: actions/upload-artifact@26f96dfa697d77e81fd5907df203aa23a56210a8 # v4.3.0
+      uses: actions/upload-artifact@65462800fd760344b1a7b4382951275a0abb4808
       with:
         name: "coverage-unit-${{ matrix.os }}-${{ matrix.python-version }}-${{ matrix.nightly && 'nightly' || 'stable' }}"
         path: ".coverage.*"
 
     - name: Run Doctests
       run: |
         nox -s xdoctest
@@ -119,18 +121,18 @@
   docker_tags:
     name: Get Docker tags
     runs-on: ubuntu-latest
     outputs:
       tags: ${{ steps.tags.outputs.tags }}
     steps:
     - name: Check out the repository
-      uses: actions/checkout@b4ffde65f46336ab88eb53be808477a3936bae11 # v4.1.1
+      uses: actions/checkout@0ad4b8fadaa221de15dcec353f45205ec38ea70b
 
     - name: Setup Python
-      uses: actions/setup-python@0a5c61591373683505ea898e09a3ea4f39ef2b9c # v5.0.0
+      uses: actions/setup-python@82c7e631bb3cdc910f68e0081d67478d79c6982d
       with:
         python-version: 3.12
         architecture: x64
         allow-prereleases: true
         cache: pip
         cache-dependency-path: |
           pyproject.toml
@@ -157,15 +159,15 @@
   databases:
     name: Get database engines
     runs-on: ubuntu-latest
     outputs:
       engines: ${{ steps.engines.outputs.engines }}
     steps:
     - name: Check out the repository
-      uses: actions/checkout@b4ffde65f46336ab88eb53be808477a3936bae11 # v4.1.1
+      uses: actions/checkout@0ad4b8fadaa221de15dcec353f45205ec38ea70b
 
     - name: Test against all engines
       if: ${{ contains(github.event.pull_request.labels.*.name, 'Release') || inputs.all_integrations }}
       run: |
         echo '["postgres", "mysql"]' > database-engines.json
 
     - name: Test against PostgreSQL
@@ -238,20 +240,20 @@
         - python-version: "3.12"
           ref: refs/heads/master
           context: https://github.com/martialblog/docker-limesurvey.git#master:6.0/apache
           database: postgres
 
     steps:
     - name: Check out the repository
-      uses: actions/checkout@b4ffde65f46336ab88eb53be808477a3936bae11 # v4.1.1
+      uses: actions/checkout@0ad4b8fadaa221de15dcec353f45205ec38ea70b
       with:
         fetch-tags: true
 
     - name: Setup Python ${{ matrix.python-version }}
-      uses: actions/setup-python@0a5c61591373683505ea898e09a3ea4f39ef2b9c # v5.0.0
+      uses: actions/setup-python@82c7e631bb3cdc910f68e0081d67478d79c6982d
       with:
         python-version: ${{ matrix.python-version }}
         architecture: x64
         allow-prereleases: true
         cache: pip
         cache-dependency-path: |
           pyproject.toml
@@ -263,18 +265,18 @@
     - name: Download LimeSurvey archive
       if: ${{ matrix.ref }}
       run: |
         wget https://github.com/LimeSurvey/LimeSurvey/archive/${{ matrix.ref }}.tar.gz -O ls.tar.gz -nv
         echo "LS_CHECKSUM=$(shasum -a 256 ls.tar.gz | cut -d' ' -f1)" >> $GITHUB_ENV
 
     - name: Set up Docker Buildx
-      uses: docker/setup-buildx-action@f95db51fddba0c2d1ec667646a06c2ce06100226 # v3.0.0
+      uses: docker/setup-buildx-action@d70bba72b1f3fd22344832f00baa16ece964efeb
 
     - name: Get Docker
-      uses: actions-hub/docker/cli@f5fdbfc3f9d2a9265ead8962c1314108a7b7ec5d # v1.0.3
+      uses: actions-hub/docker/cli@f5fdbfc3f9d2a9265ead8962c1314108a7b7ec5d
       env:
         SKIP_LOGIN: true
 
     - name: Start services
       env:
         LS_IMAGE_TAG: ${{ matrix.image_tag }}
         LS_DOCKERFILE_CONTEXT: ${{ matrix.context }}
@@ -295,15 +297,15 @@
         BACKEND: ${{ matrix.database }}
         LS_URL: http://localhost:${{ env.LS_PORT }}
       run: |
         nox
 
     - name: Upload coverage data
       if: always()
-      uses: actions/upload-artifact@26f96dfa697d77e81fd5907df203aa23a56210a8 # v4.3.0
+      uses: actions/upload-artifact@65462800fd760344b1a7b4382951275a0abb4808
       with:
         name: "coverage-integration-${{ matrix.python-version }}-${{ matrix.image_tag || env.LS_CHECKSUM }}-${{ matrix.database }}"
         path: ".coverage.*"
 
   coverage:
     name: Coverage
     runs-on: ubuntu-latest
@@ -312,40 +314,40 @@
       NOXSESSION: coverage
     strategy:
       matrix:
         flag: ["unit", "integration"]
       fail-fast: false
     steps:
     - name: Check out the repository
-      uses: actions/checkout@b4ffde65f46336ab88eb53be808477a3936bae11 # v4.1.1
+      uses: actions/checkout@0ad4b8fadaa221de15dcec353f45205ec38ea70b
 
     - name: Set up Python
-      uses: actions/setup-python@0a5c61591373683505ea898e09a3ea4f39ef2b9c # v5.0.0
+      uses: actions/setup-python@82c7e631bb3cdc910f68e0081d67478d79c6982d
       with:
         python-version: "3.12"
         cache: pip
 
     - name: Install tools
       uses: ./.github/actions/install-tools
 
     - name: Download coverage data
-      uses: actions/download-artifact@6b208ae046db98c579e8a3aa621ab581ff575935 # v4.1.1
+      uses: actions/download-artifact@65a9edc5881444af0b9093a5e628f2fe47ea3b2e
       with:
         pattern: "coverage-${{ matrix.flag }}-*"
         merge-multiple: true
 
     - name: Combine coverage data and display human readable report
       continue-on-error: true
       run: |
         nox
 
     - name: Create coverage report
       run: |
         nox -- xml
 
     - name: Upload coverage report
-      uses: codecov/codecov-action@f30e4959ba63075080d4f7f90cacc18d9f3fafd7 # v4.0.0
+      uses: codecov/codecov-action@84508663e988701840491b86de86b666e8a86bed
       with:
         token: ${{ secrets.CODECOV_TOKEN }}
         files: ./coverage.xml
         fail_ci_if_error: true
         flags: ${{ matrix.flag }}
```

### Comparing `citric-1.0.0/code_samples/custom_requests_session.py` & `citric-1.0.1a1/code_samples/custom_requests_session.py`

 * *Files identical despite different names*

### Comparing `citric-1.0.0/code_samples/duckdb_sql.py` & `citric-1.0.1a1/code_samples/duckdb_sql.py`

 * *Files identical despite different names*

### Comparing `citric-1.0.0/code_samples/get_surveys.py` & `citric-1.0.1a1/code_samples/get_surveys.py`

 * *Files identical despite different names*

### Comparing `citric-1.0.0/code_samples/pandas_df.py` & `citric-1.0.1a1/code_samples/pandas_df.py`

 * *Files identical despite different names*

### Comparing `citric-1.0.0/code_samples/requests_session_attributes.py` & `citric-1.0.1a1/code_samples/requests_session_attributes.py`

 * *Files identical despite different names*

### Comparing `citric-1.0.0/code_samples/session_attr.py` & `citric-1.0.1a1/code_samples/session_attr.py`

 * *Files identical despite different names*

### Comparing `citric-1.0.0/code_samples/upload_s3.py` & `citric-1.0.1a1/code_samples/upload_s3.py`

 * *Files identical despite different names*

### Comparing `citric-1.0.0/docs/code.png` & `citric-1.0.1a1/docs/code.png`

 * *Files identical despite different names*

### Comparing `citric-1.0.0/docs/conf.py` & `citric-1.0.1a1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `citric-1.0.0/docs/how-to.md` & `citric-1.0.1a1/docs/how-to.md`

 * *Files identical despite different names*

### Comparing `citric-1.0.0/docs/index.md` & `citric-1.0.1a1/docs/index.md`

 * *Files identical despite different names*

### Comparing `citric-1.0.0/docs/requirements.txt` & `citric-1.0.1a1/docs/requirements.txt`

 * *Files 22% similar despite different names*

```diff
@@ -1,39 +1,32 @@
-#
-# This file is autogenerated by pip-compile with Python 3.12
-# by the following command:
-#
-#    pip-compile --extra=docs --output-file=docs/requirements.txt --pre
-#
+# This file was autogenerated by uv via the following command:
+#    uv pip compile pyproject.toml --extra docs -o docs/requirements.txt
 alabaster==0.7.16
     # via sphinx
 anyascii==0.3.2
     # via sphinx-autoapi
-astroid==3.0.3
+astroid==3.1.0
     # via sphinx-autoapi
 autodocsumm==0.2.12
-    # via citric (pyproject.toml)
 babel==2.14.0
     # via sphinx
 beautifulsoup4==4.12.3
     # via furo
 certifi==2024.2.2
     # via requests
 charset-normalizer==3.3.2
     # via requests
 colorama==0.4.6
     # via sphinx-autobuild
 docutils==0.20.1
     # via
-    #   citric (pyproject.toml)
     #   myst-parser
     #   sphinx
 furo==2024.1.29
-    # via citric (pyproject.toml)
-idna==3.6
+idna==3.7
     # via requests
 imagesize==1.4.1
     # via sphinx
 jinja2==3.1.3
     # via
     #   myst-parser
     #   sphinx
@@ -47,60 +40,51 @@
 markupsafe==2.1.5
     # via jinja2
 mdit-py-plugins==0.4.0
     # via myst-parser
 mdurl==0.1.2
     # via markdown-it-py
 myst-parser==2.0.0
-    # via citric (pyproject.toml)
-packaging==23.2
+packaging==24.0
     # via sphinx
 pygments==2.17.2
     # via
     #   furo
     #   sphinx
 pyyaml==6.0.1
     # via
     #   myst-parser
     #   sphinx-autoapi
 requests==2.31.0
-    # via
-    #   citric (pyproject.toml)
-    #   sphinx
+    # via sphinx
 six==1.16.0
     # via livereload
 snowballstemmer==2.2.0
     # via sphinx
 soupsieve==2.5
     # via beautifulsoup4
 sphinx==7.2.6
     # via
     #   autodocsumm
-    #   citric (pyproject.toml)
     #   furo
     #   myst-parser
     #   sphinx-autoapi
     #   sphinx-autobuild
     #   sphinx-basic-ng
     #   sphinx-copybutton
     #   sphinx-hoverxref
     #   sphinx-notfound-page
     #   sphinxcontrib-jquery
-sphinx-autoapi==3.1.0a1
-    # via citric (pyproject.toml)
+sphinx-autoapi==3.0.0
 sphinx-autobuild==2024.2.4
-    # via citric (pyproject.toml)
 sphinx-basic-ng==1.0.0b2
     # via furo
 sphinx-copybutton==0.5.2
-    # via citric (pyproject.toml)
 sphinx-hoverxref==1.3.0
-    # via citric (pyproject.toml)
 sphinx-notfound-page==1.0.0
-    # via citric (pyproject.toml)
 sphinxcontrib-applehelp==1.0.8
     # via sphinx
 sphinxcontrib-devhelp==1.0.6
     # via sphinx
 sphinxcontrib-htmlhelp==2.0.5
     # via sphinx
 sphinxcontrib-jquery==4.1
@@ -109,9 +93,9 @@
     # via sphinx
 sphinxcontrib-qthelp==1.0.7
     # via sphinx
 sphinxcontrib-serializinghtml==1.1.10
     # via sphinx
 tornado==6.4
     # via livereload
-urllib3==2.2.0
+urllib3==2.2.1
     # via requests
```

### Comparing `citric-1.0.0/docs/rest_coverage.md` & `citric-1.0.1a1/docs/rest_coverage.md`

 * *Files identical despite different names*

### Comparing `citric-1.0.0/docs/rpc_coverage.md` & `citric-1.0.1a1/docs/rpc_coverage.md`

 * *Files identical despite different names*

### Comparing `citric-1.0.0/docs/_ext/limesurvey_future.py` & `citric-1.0.1a1/docs/_ext/limesurvey_future.py`

 * *Files identical despite different names*

### Comparing `citric-1.0.0/docs/contributing/docker.md` & `citric-1.0.1a1/docs/contributing/docker.md`

 * *Files identical despite different names*

### Comparing `citric-1.0.0/docs/contributing/environment.md` & `citric-1.0.1a1/docs/contributing/environment.md`

 * *Files identical despite different names*

### Comparing `citric-1.0.0/docs/contributing/getting-started.md` & `citric-1.0.1a1/docs/contributing/getting-started.md`

 * *Files identical despite different names*

### Comparing `citric-1.0.0/docs/contributing/release.md` & `citric-1.0.1a1/docs/contributing/release.md`

 * *Files identical despite different names*

### Comparing `citric-1.0.0/docs/contributing/testing.md` & `citric-1.0.1a1/docs/contributing/testing.md`

 * *Files identical despite different names*

### Comparing `citric-1.0.0/docs/contributing/unreleased-features.md` & `citric-1.0.1a1/docs/contributing/unreleased-features.md`

 * *Files identical despite different names*

### Comparing `citric-1.0.0/docs/notebooks/duckdb.ipynb` & `citric-1.0.1a1/docs/notebooks/duckdb.ipynb`

 * *Files identical despite different names*

### Comparing `citric-1.0.0/docs/notebooks/import_s3.ipynb` & `citric-1.0.1a1/docs/notebooks/import_s3.ipynb`

 * *Files identical despite different names*

### Comparing `citric-1.0.0/docs/notebooks/pandas_sqlite.ipynb` & `citric-1.0.1a1/docs/notebooks/pandas_sqlite.ipynb`

 * *Files identical despite different names*

### Comparing `citric-1.0.0/docs/notebooks/parse_files.ipynb` & `citric-1.0.1a1/docs/notebooks/parse_files.ipynb`

 * *Files identical despite different names*

### Comparing `citric-1.0.0/examples/free_text.lsq` & `citric-1.0.1a1/examples/free_text.lsq`

 * *Files identical despite different names*

### Comparing `citric-1.0.0/examples/group.lsg` & `citric-1.0.1a1/examples/group.lsg`

 * *Files identical despite different names*

### Comparing `citric-1.0.0/examples/limesurvey_survey_432535.lss` & `citric-1.0.1a1/examples/limesurvey_survey_432535.lss`

 * *Files identical despite different names*

### Comparing `citric-1.0.0/examples/survey.lss` & `citric-1.0.1a1/examples/survey.lss`

 * *Files identical despite different names*

### Comparing `citric-1.0.0/scripts/docker_tags.py` & `citric-1.0.1a1/scripts/docker_tags.py`

 * *Files identical despite different names*

### Comparing `citric-1.0.0/src/citric/_compat.py` & `citric-1.0.1a1/src/citric/_compat.py`

 * *Files identical despite different names*

### Comparing `citric-1.0.0/src/citric/client.py` & `citric-1.0.1a1/src/citric/client.py`

 * *Files identical despite different names*

### Comparing `citric-1.0.0/src/citric/enums.py` & `citric-1.0.1a1/src/citric/enums.py`

 * *Files identical despite different names*

### Comparing `citric-1.0.0/src/citric/exceptions.py` & `citric-1.0.1a1/src/citric/exceptions.py`

 * *Files identical despite different names*

### Comparing `citric-1.0.0/src/citric/method.py` & `citric-1.0.1a1/src/citric/method.py`

 * *Files identical despite different names*

### Comparing `citric-1.0.0/src/citric/objects.py` & `citric-1.0.1a1/src/citric/objects.py`

 * *Files identical despite different names*

### Comparing `citric-1.0.0/src/citric/session.py` & `citric-1.0.1a1/src/citric/session.py`

 * *Files identical despite different names*

### Comparing `citric-1.0.0/src/citric/types.py` & `citric-1.0.1a1/src/citric/types.py`

 * *Files identical despite different names*

### Comparing `citric-1.0.0/src/citric/_rest/client.py` & `citric-1.0.1a1/src/citric/_rest/client.py`

 * *Files identical despite different names*

### Comparing `citric-1.0.0/tests/conftest.py` & `citric-1.0.1a1/tests/conftest.py`

 * *Files 8% similar despite different names*

```diff
@@ -94,14 +94,23 @@
             item.add_marker(xfail_mysql)
 
         if "integration_test" in item.keywords:
             for value, reason in skip_integration:
                 _add_integration_skip(item, value, reason)
 
 
+def pytest_report_header() -> list[str]:
+    """Return a list of strings to be displayed in the header of the report."""
+    return [
+        f"{key}: {value}"
+        for key, value in os.environ.items()
+        if key.startswith(("COVERAGE_", "NOX_"))
+    ]
+
+
 @pytest.fixture(scope="session")
 def integration_url(request: pytest.FixtureRequest) -> str:
     """LimeSurvey URL."""
     return request.config.getoption("--limesurvey-url")
 
 
 @pytest.fixture(scope="session")
```

### Comparing `citric-1.0.0/tests/test_client.py` & `citric-1.0.1a1/tests/test_client.py`

 * *Files identical despite different names*

### Comparing `citric-1.0.0/tests/test_compat.py` & `citric-1.0.1a1/tests/test_compat.py`

 * *Files identical despite different names*

### Comparing `citric-1.0.0/tests/test_rest.py` & `citric-1.0.1a1/tests/test_rest.py`

 * *Files identical despite different names*

### Comparing `citric-1.0.0/tests/test_rpc.py` & `citric-1.0.1a1/tests/test_rpc.py`

 * *Files identical despite different names*

### Comparing `citric-1.0.0/tests/integration/conftest.py` & `citric-1.0.1a1/tests/integration/conftest.py`

 * *Files identical despite different names*

### Comparing `citric-1.0.0/tests/integration/test_rest_client.py` & `citric-1.0.1a1/tests/integration/test_rest_client.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,20 +1,18 @@
 """Integration tests for the REST client."""
 
 from __future__ import annotations
 
 import typing as t
 
 import pytest
+import semver
 
 from citric._rest import RESTClient  # noqa: PLC2701
 
-if t.TYPE_CHECKING:
-    import semver
-
 
 @pytest.fixture(scope="module")
 def rest_client(
     integration_url: str,
     integration_username: str,
     integration_password: str,
     server_version: semver.Version,
@@ -59,19 +57,23 @@
 
     result = rest_client.update_survey_details(
         survey_id=survey_id,
         anonymized=not anonymized,
         tokenLength=token_length + 10,
     )
     expected = (
-        {
+        True
+        if server_version < semver.Version(6, 4, prerelease="dev")
+        else {
             "operationsApplied": 1,
             "erronousOperations": [],
         }
-        if server_version >= (6, 4)
-        else True
+        if server_version < semver.Version(6, 5, prerelease="dev")
+        else {
+            "operationsApplied": 1,
+        }
     )
     assert result == expected
 
     updated = rest_client.get_survey_details(survey_id=survey_id)
     assert updated["anonymized"] is (not anonymized)
     assert updated["tokenLength"] == token_length + 10
```

### Comparing `citric-1.0.0/tests/integration/test_rpc_client.py` & `citric-1.0.1a1/tests/integration/test_rpc_client.py`

 * *Files identical despite different names*

### Comparing `citric-1.0.0/tests/resources/config.php` & `citric-1.0.1a1/tests/resources/config.php`

 * *Files identical despite different names*

### Comparing `citric-1.0.0/.gitignore` & `citric-1.0.1a1/.gitignore`

 * *Files identical despite different names*

### Comparing `citric-1.0.0/LICENSE` & `citric-1.0.1a1/LICENSE`

 * *Files identical despite different names*

### Comparing `citric-1.0.0/README.md` & `citric-1.0.1a1/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -3,16 +3,16 @@
 # Citric
 
 <table>
   <tbody>
     <tr>
       <td>Project Health</td>
       <td>
-        <a href="https://polar.sh/edgarrmondragon">
-          <img src="https://polar.sh/embed/seeks-funding-shield.svg?org=edgarrmondragon"/>
+        <a href="https://polar.sh/edgarrmondragon/citric">
+          <img src="https://polar.sh/embed/seeks-funding-shield.svg?org=edgarrmondragon&repo=citric"/>
         </a>
         <a href="https://results.pre-commit.ci/latest/github/edgarrmondragon/citric/main">
           <img alt="pre-commit.ci status" src="https://results.pre-commit.ci/badge/github/edgarrmondragon/citric/main.svg"/>
         </a>
         <a href="https://citric.readthedocs.io/en/latest/?badge=latest">
           <img alt="Documentation Status" src="https://readthedocs.org/projects/citric/badge/?version=latest"/>
         </a>
```

#### html2text {}

```diff
@@ -1,11 +1,11 @@
                                    # Citric
                _[_h_t_t_p_s_:_/_/_p_o_l_a_r_._s_h_/_e_m_b_e_d_/_s_e_e_k_s_-_f_u_n_d_i_n_g_-
-Project Health _s_h_i_e_l_d_._s_v_g_?_o_r_g_=_e_d_g_a_r_r_m_o_n_d_r_a_g_o_n_]_[_p_r_e_-_c_o_m_m_i_t_._c_i_ _s_t_a_t_u_s_]
-               _[_D_o_c_u_m_e_n_t_a_t_i_o_n_ _S_t_a_t_u_s_]_[_c_o_d_e_c_o_v_]
+Project Health _s_h_i_e_l_d_._s_v_g_?_o_r_g_=_e_d_g_a_r_r_m_o_n_d_r_a_g_o_n_&_r_e_p_o_=_c_i_t_r_i_c_]_[_p_r_e_-_c_o_m_m_i_t_._c_i
+               _s_t_a_t_u_s_]_[_D_o_c_u_m_e_n_t_a_t_i_o_n_ _S_t_a_t_u_s_]_[_c_o_d_e_c_o_v_]
 Packaging      _[_P_y_P_I_ _v_e_r_s_i_o_n_]_[_P_y_t_h_o_n_ _v_e_r_s_i_o_n_s_]_[_P_y_P_I_ _-_ _D_o_w_n_l_o_a_d_s_]_[_C_o_n_d_a_ _V_e_r_s_i_o_n_]
                _[_R_u_f_f_]_[_N_o_x_]_[_H_a_t_c_h_ _p_r_o_j_e_c_t_]_[_L_i_c_e_n_s_e_]_[_D_O_I_]
 Misc           _[_h_t_t_p_s_:_/_/_w_w_w_._b_e_s_t_p_r_a_c_t_i_c_e_s_._d_e_v_/_p_r_o_j_e_c_t_s_/_8_1_4_4_/_b_a_d_g_e_]
                alt="OpenSSF Scorecard">
           *A client to the [LimeSurvey Remote Control API 2](https://
     manual.limesurvey.org/RemoteControl_2_API), written in modern Python.*
 ## Features - Supports the full RPC API via the [`Session` class](https://
```

### Comparing `citric-1.0.0/pyproject.toml` & `citric-1.0.1a1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -38,15 +38,15 @@
   "Topic :: Software Development :: Libraries :: Python Modules",
   "Typing :: Typed",
 ]
 dynamic = [
   "version",
 ]
 dependencies = [
-  "requests>=2.23",
+  "requests>=2.25.1",
 ]
 optional-dependencies.dev = [
   "citric[docs,tests,typing]",
   "colorama>=0.4.6",
   "requests-cache>=1.1",
 ]
 optional-dependencies.docs = [
@@ -58,30 +58,30 @@
   "sphinx-autoapi",
   "sphinx-autobuild",
   "sphinx-copybutton",
   "sphinx-hoverxref",
   "sphinx-notfound-page",
 ]
 optional-dependencies.tests = [
-  "coverage[toml]>=7.4",
+  "coverage[toml]>=7.4.2",
   "deptry>=0.12",
   "faker>=19",
-  "pytest>=7.3.1",
+  "pytest>=8",
   "pytest-github-actions-annotate-failures>=0.1.7",
-  "pytest-httpserver",
-  "pytest-reverse",
-  "pytest-subtests",
+  "pytest-httpserver>=1.0.8",
+  "pytest-reverse>=1.7",
+  "pytest-subtests>=0.11",
   "python-dotenv>=1",
   "semver>=3.0.1",
   "tinydb>=4.8",
   "xdoctest[colors]>=1.1.1",
 ]
 optional-dependencies.typing = [
   "citric[tests]",
-  "mypy>=1.8",
+  "mypy>=1.9",
   "sphinx",
   "types-requests>=2.31.0.2",
   'typing-extensions>=4.6; python_version < "3.12"',
 ]
 urls.Documentation = "https://citric.readthedocs.io"
 urls.Homepage = 'https://github.com/edgarrmondragon/citric'
 urls."Issue Tracker" = "https://github.com/edgarrmondragon/citric/issues"
@@ -90,15 +90,14 @@
 [tool.hatch.version]
 source = "vcs"
 
 [tool.ruff]
 include = ["*.py", "*.pyi", "**/pyproject.toml", "*.ipynb"]
 line-length = 88
 src = ["src", "tests", "docs"]
-target-version = "py38"
 
 [tool.ruff.lint]
 explicit-preview-rules = false
 ignore = [
   "ANN101",  # missing-type-self
   "DJ",      # flake8-django
   "FIX002",  # line-contains-todo
@@ -310,14 +309,15 @@
 exclude_also = ['''if (t\.)?TYPE_CHECKING:''']
 fail_under = 85
 omit = ["src/citric/types.py"]
 precision = 2
 show_missing = true
 
 [tool.mypy]
+local_partial_types = true
 warn_no_return = true
 warn_redundant_casts = true
 warn_unreachable = true
 warn_unused_configs = true
 warn_unused_ignores = true
 
 [[tool.mypy.overrides]]
```

### Comparing `citric-1.0.0/PKG-INFO` & `citric-1.0.1a1/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: citric
-Version: 1.0.0
+Version: 1.0.1a1
 Summary: A client to the LimeSurvey Remote Control API 2, written in modern Python.
 Project-URL: Documentation, https://citric.readthedocs.io
 Project-URL: Homepage, https://github.com/edgarrmondragon/citric
 Project-URL: Issue Tracker, https://github.com/edgarrmondragon/citric/issues
 Project-URL: Repository, https://github.com/edgarrmondragon/citric
 Author-email: Edgar Ramírez-Mondragón <edgarrm358@gmail.com>
 Maintainer-email: Edgar Ramírez-Mondragón <edgarrm358@gmail.com>
@@ -48,62 +48,97 @@
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: 3.13
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Typing :: Typed
 Requires-Python: >=3.8
-Requires-Dist: requests>=2.23
+Requires-Dist: requests>=2.25.1
 Provides-Extra: dev
-Requires-Dist: citric[docs,tests,typing]; extra == 'dev'
+Requires-Dist: autodocsumm>=0.2.5; extra == 'dev'
 Requires-Dist: colorama>=0.4.6; extra == 'dev'
+Requires-Dist: coverage[toml]>=7.4.2; extra == 'dev'
+Requires-Dist: deptry>=0.12; extra == 'dev'
+Requires-Dist: docutils; extra == 'dev'
+Requires-Dist: faker>=19; extra == 'dev'
+Requires-Dist: furo; extra == 'dev'
+Requires-Dist: mypy>=1.9; extra == 'dev'
+Requires-Dist: myst-parser; extra == 'dev'
+Requires-Dist: pytest-github-actions-annotate-failures>=0.1.7; extra == 'dev'
+Requires-Dist: pytest-httpserver>=1.0.8; extra == 'dev'
+Requires-Dist: pytest-reverse>=1.7; extra == 'dev'
+Requires-Dist: pytest-subtests>=0.11; extra == 'dev'
+Requires-Dist: pytest>=8; extra == 'dev'
+Requires-Dist: python-dotenv>=1; extra == 'dev'
 Requires-Dist: requests-cache>=1.1; extra == 'dev'
+Requires-Dist: semver>=3.0.1; extra == 'dev'
+Requires-Dist: sphinx; extra == 'dev'
+Requires-Dist: sphinx-autoapi; extra == 'dev'
+Requires-Dist: sphinx-autobuild; extra == 'dev'
+Requires-Dist: sphinx-copybutton; extra == 'dev'
+Requires-Dist: sphinx-hoverxref; extra == 'dev'
+Requires-Dist: sphinx-notfound-page; extra == 'dev'
+Requires-Dist: tinydb>=4.8; extra == 'dev'
+Requires-Dist: types-requests>=2.31.0.2; extra == 'dev'
+Requires-Dist: typing-extensions>=4.6; (python_version < '3.12') and extra == 'dev'
+Requires-Dist: xdoctest[colors]>=1.1.1; extra == 'dev'
 Provides-Extra: docs
 Requires-Dist: autodocsumm>=0.2.5; extra == 'docs'
 Requires-Dist: docutils; extra == 'docs'
 Requires-Dist: furo; extra == 'docs'
 Requires-Dist: myst-parser; extra == 'docs'
 Requires-Dist: sphinx; extra == 'docs'
 Requires-Dist: sphinx-autoapi; extra == 'docs'
 Requires-Dist: sphinx-autobuild; extra == 'docs'
 Requires-Dist: sphinx-copybutton; extra == 'docs'
 Requires-Dist: sphinx-hoverxref; extra == 'docs'
 Requires-Dist: sphinx-notfound-page; extra == 'docs'
 Provides-Extra: tests
-Requires-Dist: coverage[toml]>=7.4; extra == 'tests'
+Requires-Dist: coverage[toml]>=7.4.2; extra == 'tests'
 Requires-Dist: deptry>=0.12; extra == 'tests'
 Requires-Dist: faker>=19; extra == 'tests'
 Requires-Dist: pytest-github-actions-annotate-failures>=0.1.7; extra == 'tests'
-Requires-Dist: pytest-httpserver; extra == 'tests'
-Requires-Dist: pytest-reverse; extra == 'tests'
-Requires-Dist: pytest-subtests; extra == 'tests'
-Requires-Dist: pytest>=7.3.1; extra == 'tests'
+Requires-Dist: pytest-httpserver>=1.0.8; extra == 'tests'
+Requires-Dist: pytest-reverse>=1.7; extra == 'tests'
+Requires-Dist: pytest-subtests>=0.11; extra == 'tests'
+Requires-Dist: pytest>=8; extra == 'tests'
 Requires-Dist: python-dotenv>=1; extra == 'tests'
 Requires-Dist: semver>=3.0.1; extra == 'tests'
 Requires-Dist: tinydb>=4.8; extra == 'tests'
 Requires-Dist: xdoctest[colors]>=1.1.1; extra == 'tests'
 Provides-Extra: typing
-Requires-Dist: citric[tests]; extra == 'typing'
-Requires-Dist: mypy>=1.8; extra == 'typing'
+Requires-Dist: coverage[toml]>=7.4.2; extra == 'typing'
+Requires-Dist: deptry>=0.12; extra == 'typing'
+Requires-Dist: faker>=19; extra == 'typing'
+Requires-Dist: mypy>=1.9; extra == 'typing'
+Requires-Dist: pytest-github-actions-annotate-failures>=0.1.7; extra == 'typing'
+Requires-Dist: pytest-httpserver>=1.0.8; extra == 'typing'
+Requires-Dist: pytest-reverse>=1.7; extra == 'typing'
+Requires-Dist: pytest-subtests>=0.11; extra == 'typing'
+Requires-Dist: pytest>=8; extra == 'typing'
+Requires-Dist: python-dotenv>=1; extra == 'typing'
+Requires-Dist: semver>=3.0.1; extra == 'typing'
 Requires-Dist: sphinx; extra == 'typing'
+Requires-Dist: tinydb>=4.8; extra == 'typing'
 Requires-Dist: types-requests>=2.31.0.2; extra == 'typing'
 Requires-Dist: typing-extensions>=4.6; (python_version < '3.12') and extra == 'typing'
+Requires-Dist: xdoctest[colors]>=1.1.1; extra == 'typing'
 Description-Content-Type: text/markdown
 
 <div align="center">
 
 # Citric
 
 <table>
   <tbody>
     <tr>
       <td>Project Health</td>
       <td>
-        <a href="https://polar.sh/edgarrmondragon">
-          <img src="https://polar.sh/embed/seeks-funding-shield.svg?org=edgarrmondragon"/>
+        <a href="https://polar.sh/edgarrmondragon/citric">
+          <img src="https://polar.sh/embed/seeks-funding-shield.svg?org=edgarrmondragon&repo=citric"/>
         </a>
         <a href="https://results.pre-commit.ci/latest/github/edgarrmondragon/citric/main">
           <img alt="pre-commit.ci status" src="https://results.pre-commit.ci/badge/github/edgarrmondragon/citric/main.svg"/>
         </a>
         <a href="https://citric.readthedocs.io/en/latest/?badge=latest">
           <img alt="Documentation Status" src="https://readthedocs.org/projects/citric/badge/?version=latest"/>
         </a>
```

