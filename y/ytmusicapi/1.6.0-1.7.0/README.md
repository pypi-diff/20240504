# Comparing `tmp/ytmusicapi-1.6.0.tar.gz` & `tmp/ytmusicapi-1.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ytmusicapi-1.6.0.tar", last modified: Fri Mar  8 20:36:19 2024, max compression
+gzip compressed data, was "ytmusicapi-1.7.0.tar", last modified: Sat May  4 11:36:37 2024, max compression
```

## Comparing `ytmusicapi-1.6.0.tar` & `ytmusicapi-1.7.0.tar`

### file list

```diff
@@ -1,179 +1,183 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-08 20:36:19.308008 ytmusicapi-1.6.0/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-08 20:36:19.288007 ytmusicapi-1.6.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-08 20:36:19.288007 ytmusicapi-1.6.0/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (127)      646 2024-03-08 20:36:14.000000 ytmusicapi-1.6.0/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0 runner    (1001) docker     (127)      848 2024-03-08 20:36:14.000000 ytmusicapi-1.6.0/.github/ISSUE_TEMPLATE/feature_request.md
--rw-r--r--   0 runner    (1001) docker     (127)      514 2024-03-08 20:36:14.000000 ytmusicapi-1.6.0/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-08 20:36:19.288007 ytmusicapi-1.6.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     1380 2024-03-08 20:36:14.000000 ytmusicapi-1.6.0/.github/workflows/coverage.yml
--rw-r--r--   0 runner    (1001) docker     (127)      612 2024-03-08 20:36:14.000000 ytmusicapi-1.6.0/.github/workflows/docsbuild.yml
--rw-r--r--   0 runner    (1001) docker     (127)      575 2024-03-08 20:36:14.000000 ytmusicapi-1.6.0/.github/workflows/lint.yml
--rw-r--r--   0 runner    (1001) docker     (127)      254 2024-03-08 20:36:14.000000 ytmusicapi-1.6.0/.github/workflows/pdm.yml
--rw-r--r--   0 runner    (1001) docker     (127)      626 2024-03-08 20:36:14.000000 ytmusicapi-1.6.0/.github/workflows/pythonpublish.yml
--rw-r--r--   0 runner    (1001) docker     (127)      135 2024-03-08 20:36:14.000000 ytmusicapi-1.6.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      347 2024-03-08 20:36:14.000000 ytmusicapi-1.6.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      227 2024-03-08 20:36:14.000000 ytmusicapi-1.6.0/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1223 2024-03-08 20:36:14.000000 ytmusicapi-1.6.0/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-03-08 20:36:14.000000 ytmusicapi-1.6.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     5347 2024-03-08 20:36:19.308008 ytmusicapi-1.6.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3566 2024-03-08 20:36:14.000000 ytmusicapi-1.6.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-08 20:36:19.288007 ytmusicapi-1.6.0/docs/
--rw-r--r--   0 runner    (1001) docker     (127)      638 2024-03-08 20:36:14.000000 ytmusicapi-1.6.0/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)      764 2024-03-08 20:36:14.000000 ytmusicapi-1.6.0/docs/make.bat
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-08 20:36:19.288007 ytmusicapi-1.6.0/docs/source/
--rw-r--r--   0 runner    (1001) docker     (127)     1762 2024-03-08 20:36:14.000000 ytmusicapi-1.6.0/docs/source/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)    11467 2024-03-08 20:36:14.000000 ytmusicapi-1.6.0/docs/source/faq.rst
--rw-r--r--   0 runner    (1001) docker     (127)      828 2024-03-08 20:36:14.000000 ytmusicapi-1.6.0/docs/source/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2645 2024-03-08 20:36:14.000000 ytmusicapi-1.6.0/docs/source/reference.rst
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-03-08 20:36:14.000000 ytmusicapi-1.6.0/docs/source/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-08 20:36:19.292008 ytmusicapi-1.6.0/docs/source/setup/
--rw-r--r--   0 runner    (1001) docker     (127)     3242 2024-03-08 20:36:14.000000 ytmusicapi-1.6.0/docs/source/setup/browser.rst
--rw-r--r--   0 runner    (1001) docker     (127)      308 2024-03-08 20:36:14.000000 ytmusicapi-1.6.0/docs/source/setup/headers_auth.json.example
--rw-r--r--   0 runner    (1001) docker     (127)      442 2024-03-08 20:36:14.000000 ytmusicapi-1.6.0/docs/source/setup/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)      437 2024-03-08 20:36:14.000000 ytmusicapi-1.6.0/docs/source/setup/oauth.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1405 2024-03-08 20:36:14.000000 ytmusicapi-1.6.0/docs/source/usage.rst
--rw-r--r--   0 runner    (1001) docker     (127)    61953 2024-03-08 20:36:14.000000 ytmusicapi-1.6.0/pdm.lock
--rw-r--r--   0 runner    (1001) docker     (127)     1612 2024-03-08 20:36:14.000000 ytmusicapi-1.6.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-08 20:36:19.308008 ytmusicapi-1.6.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-08 20:36:19.292008 ytmusicapi-1.6.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     2102 2024-03-08 20:36:14.000000 ytmusicapi-1.6.0/tests/README.rst
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-08 20:36:14.000000 ytmusicapi-1.6.0/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-08 20:36:19.292008 ytmusicapi-1.6.0/tests/auth/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-08 20:36:14.000000 ytmusicapi-1.6.0/tests/auth/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      619 2024-03-08 20:36:14.000000 ytmusicapi-1.6.0/tests/auth/test_browser.py
--rw-r--r--   0 runner    (1001) docker     (127)     4076 2024-03-08 20:36:14.000000 ytmusicapi-1.6.0/tests/auth/test_oauth.py
--rw-r--r--   0 runner    (1001) docker     (127)     1906 2024-03-08 20:36:14.000000 ytmusicapi-1.6.0/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-08 20:36:19.292008 ytmusicapi-1.6.0/tests/mixins/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-08 20:36:14.000000 ytmusicapi-1.6.0/tests/mixins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7466 2024-03-08 20:36:14.000000 ytmusicapi-1.6.0/tests/mixins/test_browsing.py
--rw-r--r--   0 runner    (1001) docker     (127)      664 2024-03-08 20:36:14.000000 ytmusicapi-1.6.0/tests/mixins/test_explore.py
--rw-r--r--   0 runner    (1001) docker     (127)     6003 2024-03-08 20:36:14.000000 ytmusicapi-1.6.0/tests/mixins/test_library.py
--rw-r--r--   0 runner    (1001) docker     (127)     3227 2024-03-08 20:36:14.000000 ytmusicapi-1.6.0/tests/mixins/test_playlists.py
--rw-r--r--   0 runner    (1001) docker     (127)     1990 2024-03-08 20:36:14.000000 ytmusicapi-1.6.0/tests/mixins/test_podcasts.py
--rw-r--r--   0 runner    (1001) docker     (127)     4703 2024-03-08 20:36:14.000000 ytmusicapi-1.6.0/tests/mixins/test_search.py
--rw-r--r--   0 runner    (1001) docker     (127)     2577 2024-03-08 20:36:14.000000 ytmusicapi-1.6.0/tests/mixins/test_uploads.py
--rw-r--r--   0 runner    (1001) docker     (127)     1143 2024-03-08 20:36:14.000000 ytmusicapi-1.6.0/tests/mixins/test_watch.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-08 20:36:19.292008 ytmusicapi-1.6.0/tests/setup/
--rw-r--r--   0 runner    (1001) docker     (127)     2735 2024-03-08 20:36:14.000000 ytmusicapi-1.6.0/tests/setup/setup_account.py
--rw-r--r--   0 runner    (1001) docker     (127)     1291 2024-03-08 20:36:14.000000 ytmusicapi-1.6.0/tests/test.example.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      148 2024-03-08 20:36:14.000000 ytmusicapi-1.6.0/tests/test_ytmusic.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-08 20:36:19.296007 ytmusicapi-1.6.0/ytmusicapi/
--rw-r--r--   0 runner    (1001) docker     (127)      397 2024-03-08 20:36:14.000000 ytmusicapi-1.6.0/ytmusicapi/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-08 20:36:19.296007 ytmusicapi-1.6.0/ytmusicapi/auth/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-08 20:36:14.000000 ytmusicapi-1.6.0/ytmusicapi/auth/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2591 2024-03-08 20:36:14.000000 ytmusicapi-1.6.0/ytmusicapi/auth/browser.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-08 20:36:19.296007 ytmusicapi-1.6.0/ytmusicapi/auth/oauth/
--rw-r--r--   0 runner    (1001) docker     (127)      154 2024-03-08 20:36:14.000000 ytmusicapi-1.6.0/ytmusicapi/auth/oauth/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4865 2024-03-08 20:36:14.000000 ytmusicapi-1.6.0/ytmusicapi/auth/oauth/credentials.py
--rw-r--r--   0 runner    (1001) docker     (127)      360 2024-03-08 20:36:14.000000 ytmusicapi-1.6.0/ytmusicapi/auth/oauth/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     1346 2024-03-08 20:36:14.000000 ytmusicapi-1.6.0/ytmusicapi/auth/oauth/models.py
--rw-r--r--   0 runner    (1001) docker     (127)     5008 2024-03-08 20:36:14.000000 ytmusicapi-1.6.0/ytmusicapi/auth/oauth/token.py
--rw-r--r--   0 runner    (1001) docker     (127)      717 2024-03-08 20:36:14.000000 ytmusicapi-1.6.0/ytmusicapi/auth/types.py
--rw-r--r--   0 runner    (1001) docker     (127)     1499 2024-03-08 20:36:14.000000 ytmusicapi-1.6.0/ytmusicapi/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     3405 2024-03-08 20:36:14.000000 ytmusicapi-1.6.0/ytmusicapi/continuations.py
--rw-r--r--   0 runner    (1001) docker     (127)     2000 2024-03-08 20:36:14.000000 ytmusicapi-1.6.0/ytmusicapi/helpers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-08 20:36:19.296007 ytmusicapi-1.6.0/ytmusicapi/locales/
--rw-r--r--   0 runner    (1001) docker     (127)     1298 2024-03-08 20:36:14.000000 ytmusicapi-1.6.0/ytmusicapi/locales/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-08 20:36:19.280007 ytmusicapi-1.6.0/ytmusicapi/locales/ar/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-08 20:36:19.296007 ytmusicapi-1.6.0/ytmusicapi/locales/ar/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)      984 2024-03-08 20:36:14.000000 ytmusicapi-1.6.0/ytmusicapi/locales/ar/LC_MESSAGES/base.mo
--rw-r--r--   0 runner    (1001) docker     (127)     1468 2024-03-08 20:36:14.000000 ytmusicapi-1.6.0/ytmusicapi/locales/ar/LC_MESSAGES/base.po
--rw-r--r--   0 runner    (1001) docker     (127)     1312 2024-03-08 20:36:14.000000 ytmusicapi-1.6.0/ytmusicapi/locales/base.pot
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-08 20:36:19.280007 ytmusicapi-1.6.0/ytmusicapi/locales/de/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-08 20:36:19.300007 ytmusicapi-1.6.0/ytmusicapi/locales/de/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)      887 2024-03-08 20:36:14.000000 ytmusicapi-1.6.0/ytmusicapi/locales/de/LC_MESSAGES/base.mo
--rw-r--r--   0 runner    (1001) docker     (127)     1401 2024-03-08 20:36:14.000000 ytmusicapi-1.6.0/ytmusicapi/locales/de/LC_MESSAGES/base.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-08 20:36:19.284007 ytmusicapi-1.6.0/ytmusicapi/locales/en/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-08 20:36:19.300007 ytmusicapi-1.6.0/ytmusicapi/locales/en/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)      431 2024-03-08 20:36:14.000000 ytmusicapi-1.6.0/ytmusicapi/locales/en/LC_MESSAGES/base.mo
--rw-r--r--   0 runner    (1001) docker     (127)     1313 2024-03-08 20:36:14.000000 ytmusicapi-1.6.0/ytmusicapi/locales/en/LC_MESSAGES/base.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-08 20:36:19.284007 ytmusicapi-1.6.0/ytmusicapi/locales/es/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-08 20:36:19.300007 ytmusicapi-1.6.0/ytmusicapi/locales/es/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)      962 2024-03-08 20:36:14.000000 ytmusicapi-1.6.0/ytmusicapi/locales/es/LC_MESSAGES/base.mo
--rw-r--r--   0 runner    (1001) docker     (127)     1451 2024-03-08 20:36:14.000000 ytmusicapi-1.6.0/ytmusicapi/locales/es/LC_MESSAGES/base.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-08 20:36:19.284007 ytmusicapi-1.6.0/ytmusicapi/locales/fr/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-08 20:36:19.300007 ytmusicapi-1.6.0/ytmusicapi/locales/fr/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)      746 2024-03-08 20:36:14.000000 ytmusicapi-1.6.0/ytmusicapi/locales/fr/LC_MESSAGES/base.mo
--rw-r--r--   0 runner    (1001) docker     (127)     1386 2024-03-08 20:36:14.000000 ytmusicapi-1.6.0/ytmusicapi/locales/fr/LC_MESSAGES/base.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-08 20:36:19.284007 ytmusicapi-1.6.0/ytmusicapi/locales/hi/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-08 20:36:19.300007 ytmusicapi-1.6.0/ytmusicapi/locales/hi/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-03-08 20:36:14.000000 ytmusicapi-1.6.0/ytmusicapi/locales/hi/LC_MESSAGES/base.mo
--rw-r--r--   0 runner    (1001) docker     (127)     1552 2024-03-08 20:36:14.000000 ytmusicapi-1.6.0/ytmusicapi/locales/hi/LC_MESSAGES/base.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-08 20:36:19.284007 ytmusicapi-1.6.0/ytmusicapi/locales/it/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-08 20:36:19.300007 ytmusicapi-1.6.0/ytmusicapi/locales/it/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)      806 2024-03-08 20:36:14.000000 ytmusicapi-1.6.0/ytmusicapi/locales/it/LC_MESSAGES/base.mo
--rw-r--r--   0 runner    (1001) docker     (127)     1393 2024-03-08 20:36:14.000000 ytmusicapi-1.6.0/ytmusicapi/locales/it/LC_MESSAGES/base.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-08 20:36:19.284007 ytmusicapi-1.6.0/ytmusicapi/locales/ja/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-08 20:36:19.300007 ytmusicapi-1.6.0/ytmusicapi/locales/ja/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)     1029 2024-03-08 20:36:14.000000 ytmusicapi-1.6.0/ytmusicapi/locales/ja/LC_MESSAGES/base.mo
--rw-r--r--   0 runner    (1001) docker     (127)     1518 2024-03-08 20:36:14.000000 ytmusicapi-1.6.0/ytmusicapi/locales/ja/LC_MESSAGES/base.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-08 20:36:19.284007 ytmusicapi-1.6.0/ytmusicapi/locales/ko/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-08 20:36:19.300007 ytmusicapi-1.6.0/ytmusicapi/locales/ko/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)      957 2024-03-08 20:36:14.000000 ytmusicapi-1.6.0/ytmusicapi/locales/ko/LC_MESSAGES/base.mo
--rw-r--r--   0 runner    (1001) docker     (127)     1446 2024-03-08 20:36:14.000000 ytmusicapi-1.6.0/ytmusicapi/locales/ko/LC_MESSAGES/base.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-08 20:36:19.284007 ytmusicapi-1.6.0/ytmusicapi/locales/nl/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-08 20:36:19.300007 ytmusicapi-1.6.0/ytmusicapi/locales/nl/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)      943 2024-03-08 20:36:14.000000 ytmusicapi-1.6.0/ytmusicapi/locales/nl/LC_MESSAGES/base.mo
--rw-r--r--   0 runner    (1001) docker     (127)     1456 2024-03-08 20:36:14.000000 ytmusicapi-1.6.0/ytmusicapi/locales/nl/LC_MESSAGES/base.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-08 20:36:19.284007 ytmusicapi-1.6.0/ytmusicapi/locales/pt/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-08 20:36:19.300007 ytmusicapi-1.6.0/ytmusicapi/locales/pt/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)      877 2024-03-08 20:36:14.000000 ytmusicapi-1.6.0/ytmusicapi/locales/pt/LC_MESSAGES/base.mo
--rw-r--r--   0 runner    (1001) docker     (127)     1386 2024-03-08 20:36:14.000000 ytmusicapi-1.6.0/ytmusicapi/locales/pt/LC_MESSAGES/base.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-08 20:36:19.284007 ytmusicapi-1.6.0/ytmusicapi/locales/ru/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-08 20:36:19.300007 ytmusicapi-1.6.0/ytmusicapi/locales/ru/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)      981 2024-03-08 20:36:14.000000 ytmusicapi-1.6.0/ytmusicapi/locales/ru/LC_MESSAGES/base.mo
--rw-r--r--   0 runner    (1001) docker     (127)     1465 2024-03-08 20:36:14.000000 ytmusicapi-1.6.0/ytmusicapi/locales/ru/LC_MESSAGES/base.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-08 20:36:19.284007 ytmusicapi-1.6.0/ytmusicapi/locales/tr/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-08 20:36:19.300007 ytmusicapi-1.6.0/ytmusicapi/locales/tr/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)      863 2024-03-08 20:36:14.000000 ytmusicapi-1.6.0/ytmusicapi/locales/tr/LC_MESSAGES/base.mo
--rw-r--r--   0 runner    (1001) docker     (127)     1372 2024-03-08 20:36:14.000000 ytmusicapi-1.6.0/ytmusicapi/locales/tr/LC_MESSAGES/base.po
--rw-r--r--   0 runner    (1001) docker     (127)      141 2024-03-08 20:36:14.000000 ytmusicapi-1.6.0/ytmusicapi/locales/update_mo.sh
--rw-r--r--   0 runner    (1001) docker     (127)      169 2024-03-08 20:36:14.000000 ytmusicapi-1.6.0/ytmusicapi/locales/update_po.sh
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-08 20:36:19.284007 ytmusicapi-1.6.0/ytmusicapi/locales/ur/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-08 20:36:19.304008 ytmusicapi-1.6.0/ytmusicapi/locales/ur/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)      961 2024-03-08 20:36:14.000000 ytmusicapi-1.6.0/ytmusicapi/locales/ur/LC_MESSAGES/base.mo
--rw-r--r--   0 runner    (1001) docker     (127)     1445 2024-03-08 20:36:14.000000 ytmusicapi-1.6.0/ytmusicapi/locales/ur/LC_MESSAGES/base.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-08 20:36:19.284007 ytmusicapi-1.6.0/ytmusicapi/locales/zh_CN/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-08 20:36:19.304008 ytmusicapi-1.6.0/ytmusicapi/locales/zh_CN/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)      737 2024-03-08 20:36:14.000000 ytmusicapi-1.6.0/ytmusicapi/locales/zh_CN/LC_MESSAGES/base.mo
--rw-r--r--   0 runner    (1001) docker     (127)     1410 2024-03-08 20:36:14.000000 ytmusicapi-1.6.0/ytmusicapi/locales/zh_CN/LC_MESSAGES/base.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-08 20:36:19.284007 ytmusicapi-1.6.0/ytmusicapi/locales/zh_TW/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-08 20:36:19.304008 ytmusicapi-1.6.0/ytmusicapi/locales/zh_TW/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)      728 2024-03-08 20:36:14.000000 ytmusicapi-1.6.0/ytmusicapi/locales/zh_TW/LC_MESSAGES/base.mo
--rw-r--r--   0 runner    (1001) docker     (127)     1405 2024-03-08 20:36:14.000000 ytmusicapi-1.6.0/ytmusicapi/locales/zh_TW/LC_MESSAGES/base.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-08 20:36:19.304008 ytmusicapi-1.6.0/ytmusicapi/mixins/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-08 20:36:14.000000 ytmusicapi-1.6.0/ytmusicapi/mixins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      892 2024-03-08 20:36:14.000000 ytmusicapi-1.6.0/ytmusicapi/mixins/_protocol.py
--rw-r--r--   0 runner    (1001) docker     (127)     1393 2024-03-08 20:36:14.000000 ytmusicapi-1.6.0/ytmusicapi/mixins/_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    38507 2024-03-08 20:36:14.000000 ytmusicapi-1.6.0/ytmusicapi/mixins/browsing.py
--rw-r--r--   0 runner    (1001) docker     (127)     9716 2024-03-08 20:36:14.000000 ytmusicapi-1.6.0/ytmusicapi/mixins/explore.py
--rw-r--r--   0 runner    (1001) docker     (127)    17461 2024-03-08 20:36:14.000000 ytmusicapi-1.6.0/ytmusicapi/mixins/library.py
--rw-r--r--   0 runner    (1001) docker     (127)    15475 2024-03-08 20:36:14.000000 ytmusicapi-1.6.0/ytmusicapi/mixins/playlists.py
--rw-r--r--   0 runner    (1001) docker     (127)     9835 2024-03-08 20:36:14.000000 ytmusicapi-1.6.0/ytmusicapi/mixins/podcasts.py
--rw-r--r--   0 runner    (1001) docker     (127)    12177 2024-03-08 20:36:14.000000 ytmusicapi-1.6.0/ytmusicapi/mixins/search.py
--rw-r--r--   0 runner    (1001) docker     (127)    10724 2024-03-08 20:36:14.000000 ytmusicapi-1.6.0/ytmusicapi/mixins/uploads.py
--rw-r--r--   0 runner    (1001) docker     (127)     7246 2024-03-08 20:36:14.000000 ytmusicapi-1.6.0/ytmusicapi/mixins/watch.py
--rw-r--r--   0 runner    (1001) docker     (127)     5383 2024-03-08 20:36:14.000000 ytmusicapi-1.6.0/ytmusicapi/navigation.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-08 20:36:19.308008 ytmusicapi-1.6.0/ytmusicapi/parsers/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-08 20:36:14.000000 ytmusicapi-1.6.0/ytmusicapi/parsers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2566 2024-03-08 20:36:14.000000 ytmusicapi-1.6.0/ytmusicapi/parsers/_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1428 2024-03-08 20:36:14.000000 ytmusicapi-1.6.0/ytmusicapi/parsers/albums.py
--rw-r--r--   0 runner    (1001) docker     (127)     5635 2024-03-08 20:36:14.000000 ytmusicapi-1.6.0/ytmusicapi/parsers/browsing.py
--rw-r--r--   0 runner    (1001) docker     (127)     1554 2024-03-08 20:36:14.000000 ytmusicapi-1.6.0/ytmusicapi/parsers/explore.py
--rw-r--r--   0 runner    (1001) docker     (127)     2431 2024-03-08 20:36:14.000000 ytmusicapi-1.6.0/ytmusicapi/parsers/i18n.py
--rw-r--r--   0 runner    (1001) docker     (127)     4436 2024-03-08 20:36:14.000000 ytmusicapi-1.6.0/ytmusicapi/parsers/library.py
--rw-r--r--   0 runner    (1001) docker     (127)     5659 2024-03-08 20:36:14.000000 ytmusicapi-1.6.0/ytmusicapi/parsers/playlists.py
--rw-r--r--   0 runner    (1001) docker     (127)     4612 2024-03-08 20:36:14.000000 ytmusicapi-1.6.0/ytmusicapi/parsers/podcasts.py
--rw-r--r--   0 runner    (1001) docker     (127)     9739 2024-03-08 20:36:14.000000 ytmusicapi-1.6.0/ytmusicapi/parsers/search.py
--rw-r--r--   0 runner    (1001) docker     (127)     2731 2024-03-08 20:36:14.000000 ytmusicapi-1.6.0/ytmusicapi/parsers/songs.py
--rw-r--r--   0 runner    (1001) docker     (127)     1489 2024-03-08 20:36:14.000000 ytmusicapi-1.6.0/ytmusicapi/parsers/uploads.py
--rw-r--r--   0 runner    (1001) docker     (127)     2123 2024-03-08 20:36:14.000000 ytmusicapi-1.6.0/ytmusicapi/parsers/watch.py
--rw-r--r--   0 runner    (1001) docker     (127)     2662 2024-03-08 20:36:14.000000 ytmusicapi-1.6.0/ytmusicapi/setup.py
--rw-r--r--   0 runner    (1001) docker     (127)    11518 2024-03-08 20:36:14.000000 ytmusicapi-1.6.0/ytmusicapi/ytmusic.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-08 20:36:19.308008 ytmusicapi-1.6.0/ytmusicapi.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5347 2024-03-08 20:36:19.000000 ytmusicapi-1.6.0/ytmusicapi.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3927 2024-03-08 20:36:19.000000 ytmusicapi-1.6.0/ytmusicapi.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-08 20:36:19.000000 ytmusicapi-1.6.0/ytmusicapi.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       53 2024-03-08 20:36:19.000000 ytmusicapi-1.6.0/ytmusicapi.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-03-08 20:36:19.000000 ytmusicapi-1.6.0/ytmusicapi.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-03-08 20:36:19.000000 ytmusicapi-1.6.0/ytmusicapi.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 11:36:37.024805 ytmusicapi-1.7.0/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 11:36:37.004805 ytmusicapi-1.7.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 11:36:37.004805 ytmusicapi-1.7.0/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (127)      646 2024-05-04 11:36:31.000000 ytmusicapi-1.7.0/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0 runner    (1001) docker     (127)      848 2024-05-04 11:36:31.000000 ytmusicapi-1.7.0/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0 runner    (1001) docker     (127)      514 2024-05-04 11:36:31.000000 ytmusicapi-1.7.0/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 11:36:37.004805 ytmusicapi-1.7.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1380 2024-05-04 11:36:31.000000 ytmusicapi-1.7.0/.github/workflows/coverage.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      612 2024-05-04 11:36:31.000000 ytmusicapi-1.7.0/.github/workflows/docsbuild.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      640 2024-05-04 11:36:31.000000 ytmusicapi-1.7.0/.github/workflows/lint.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      254 2024-05-04 11:36:31.000000 ytmusicapi-1.7.0/.github/workflows/pdm.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      626 2024-05-04 11:36:31.000000 ytmusicapi-1.7.0/.github/workflows/pythonpublish.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      159 2024-05-04 11:36:31.000000 ytmusicapi-1.7.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      348 2024-05-04 11:36:31.000000 ytmusicapi-1.7.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      227 2024-05-04 11:36:31.000000 ytmusicapi-1.7.0/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1223 2024-05-04 11:36:31.000000 ytmusicapi-1.7.0/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-05-04 11:36:31.000000 ytmusicapi-1.7.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     5512 2024-05-04 11:36:37.024805 ytmusicapi-1.7.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3731 2024-05-04 11:36:31.000000 ytmusicapi-1.7.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 11:36:37.004805 ytmusicapi-1.7.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)      638 2024-05-04 11:36:31.000000 ytmusicapi-1.7.0/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)      764 2024-05-04 11:36:31.000000 ytmusicapi-1.7.0/docs/make.bat
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 11:36:37.004805 ytmusicapi-1.7.0/docs/source/
+-rw-r--r--   0 runner    (1001) docker     (127)     1762 2024-05-04 11:36:31.000000 ytmusicapi-1.7.0/docs/source/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11467 2024-05-04 11:36:31.000000 ytmusicapi-1.7.0/docs/source/faq.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      828 2024-05-04 11:36:31.000000 ytmusicapi-1.7.0/docs/source/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2645 2024-05-04 11:36:31.000000 ytmusicapi-1.7.0/docs/source/reference.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-05-04 11:36:31.000000 ytmusicapi-1.7.0/docs/source/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 11:36:37.004805 ytmusicapi-1.7.0/docs/source/setup/
+-rw-r--r--   0 runner    (1001) docker     (127)     3242 2024-05-04 11:36:31.000000 ytmusicapi-1.7.0/docs/source/setup/browser.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      308 2024-05-04 11:36:31.000000 ytmusicapi-1.7.0/docs/source/setup/headers_auth.json.example
+-rw-r--r--   0 runner    (1001) docker     (127)      442 2024-05-04 11:36:31.000000 ytmusicapi-1.7.0/docs/source/setup/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      437 2024-05-04 11:36:31.000000 ytmusicapi-1.7.0/docs/source/setup/oauth.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1405 2024-05-04 11:36:31.000000 ytmusicapi-1.7.0/docs/source/usage.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    61554 2024-05-04 11:36:31.000000 ytmusicapi-1.7.0/pdm.lock
+-rw-r--r--   0 runner    (1001) docker     (127)     1612 2024-05-04 11:36:31.000000 ytmusicapi-1.7.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-04 11:36:37.024805 ytmusicapi-1.7.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 11:36:37.008805 ytmusicapi-1.7.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     2102 2024-05-04 11:36:31.000000 ytmusicapi-1.7.0/tests/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-04 11:36:31.000000 ytmusicapi-1.7.0/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 11:36:37.008805 ytmusicapi-1.7.0/tests/auth/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-04 11:36:31.000000 ytmusicapi-1.7.0/tests/auth/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      619 2024-05-04 11:36:31.000000 ytmusicapi-1.7.0/tests/auth/test_browser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4076 2024-05-04 11:36:31.000000 ytmusicapi-1.7.0/tests/auth/test_oauth.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1906 2024-05-04 11:36:31.000000 ytmusicapi-1.7.0/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 11:36:37.008805 ytmusicapi-1.7.0/tests/data/
+-rw-r--r--   0 runner    (1001) docker     (127)   226650 2024-05-04 11:36:32.000000 ytmusicapi-1.7.0/tests/data/2024_03_get_album.json
+-rw-r--r--   0 runner    (1001) docker     (127)  1039226 2024-05-04 11:36:32.000000 ytmusicapi-1.7.0/tests/data/2024_03_get_playlist.json
+-rw-r--r--   0 runner    (1001) docker     (127)  1004367 2024-05-04 11:36:32.000000 ytmusicapi-1.7.0/tests/data/2024_03_get_playlist_public.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 11:36:37.012805 ytmusicapi-1.7.0/tests/mixins/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-04 11:36:32.000000 ytmusicapi-1.7.0/tests/mixins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8338 2024-05-04 11:36:32.000000 ytmusicapi-1.7.0/tests/mixins/test_browsing.py
+-rw-r--r--   0 runner    (1001) docker     (127)      664 2024-05-04 11:36:32.000000 ytmusicapi-1.7.0/tests/mixins/test_explore.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6003 2024-05-04 11:36:32.000000 ytmusicapi-1.7.0/tests/mixins/test_library.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4776 2024-05-04 11:36:32.000000 ytmusicapi-1.7.0/tests/mixins/test_playlists.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1990 2024-05-04 11:36:32.000000 ytmusicapi-1.7.0/tests/mixins/test_podcasts.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4703 2024-05-04 11:36:32.000000 ytmusicapi-1.7.0/tests/mixins/test_search.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2577 2024-05-04 11:36:32.000000 ytmusicapi-1.7.0/tests/mixins/test_uploads.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1143 2024-05-04 11:36:32.000000 ytmusicapi-1.7.0/tests/mixins/test_watch.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 11:36:37.012805 ytmusicapi-1.7.0/tests/setup/
+-rw-r--r--   0 runner    (1001) docker     (127)     2735 2024-05-04 11:36:32.000000 ytmusicapi-1.7.0/tests/setup/setup_account.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1291 2024-05-04 11:36:32.000000 ytmusicapi-1.7.0/tests/test.example.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      148 2024-05-04 11:36:32.000000 ytmusicapi-1.7.0/tests/test_ytmusic.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 11:36:37.012805 ytmusicapi-1.7.0/ytmusicapi/
+-rw-r--r--   0 runner    (1001) docker     (127)      397 2024-05-04 11:36:32.000000 ytmusicapi-1.7.0/ytmusicapi/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 11:36:37.016805 ytmusicapi-1.7.0/ytmusicapi/auth/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-04 11:36:32.000000 ytmusicapi-1.7.0/ytmusicapi/auth/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2591 2024-05-04 11:36:32.000000 ytmusicapi-1.7.0/ytmusicapi/auth/browser.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 11:36:37.016805 ytmusicapi-1.7.0/ytmusicapi/auth/oauth/
+-rw-r--r--   0 runner    (1001) docker     (127)      154 2024-05-04 11:36:32.000000 ytmusicapi-1.7.0/ytmusicapi/auth/oauth/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4865 2024-05-04 11:36:32.000000 ytmusicapi-1.7.0/ytmusicapi/auth/oauth/credentials.py
+-rw-r--r--   0 runner    (1001) docker     (127)      360 2024-05-04 11:36:32.000000 ytmusicapi-1.7.0/ytmusicapi/auth/oauth/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1346 2024-05-04 11:36:32.000000 ytmusicapi-1.7.0/ytmusicapi/auth/oauth/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5008 2024-05-04 11:36:32.000000 ytmusicapi-1.7.0/ytmusicapi/auth/oauth/token.py
+-rw-r--r--   0 runner    (1001) docker     (127)      717 2024-05-04 11:36:32.000000 ytmusicapi-1.7.0/ytmusicapi/auth/types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1499 2024-05-04 11:36:32.000000 ytmusicapi-1.7.0/ytmusicapi/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3405 2024-05-04 11:36:32.000000 ytmusicapi-1.7.0/ytmusicapi/continuations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2000 2024-05-04 11:36:32.000000 ytmusicapi-1.7.0/ytmusicapi/helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 11:36:37.016805 ytmusicapi-1.7.0/ytmusicapi/locales/
+-rw-r--r--   0 runner    (1001) docker     (127)     1265 2024-05-04 11:36:32.000000 ytmusicapi-1.7.0/ytmusicapi/locales/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 11:36:36.996805 ytmusicapi-1.7.0/ytmusicapi/locales/ar/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 11:36:37.016805 ytmusicapi-1.7.0/ytmusicapi/locales/ar/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     1049 2024-05-04 11:36:32.000000 ytmusicapi-1.7.0/ytmusicapi/locales/ar/LC_MESSAGES/base.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     1558 2024-05-04 11:36:32.000000 ytmusicapi-1.7.0/ytmusicapi/locales/ar/LC_MESSAGES/base.po
+-rw-r--r--   0 runner    (1001) docker     (127)     1359 2024-05-04 11:36:32.000000 ytmusicapi-1.7.0/ytmusicapi/locales/base.pot
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 11:36:36.996805 ytmusicapi-1.7.0/ytmusicapi/locales/de/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 11:36:37.016805 ytmusicapi-1.7.0/ytmusicapi/locales/de/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)      932 2024-05-04 11:36:32.000000 ytmusicapi-1.7.0/ytmusicapi/locales/de/LC_MESSAGES/base.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     1471 2024-05-04 11:36:32.000000 ytmusicapi-1.7.0/ytmusicapi/locales/de/LC_MESSAGES/base.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 11:36:36.996805 ytmusicapi-1.7.0/ytmusicapi/locales/en/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 11:36:37.016805 ytmusicapi-1.7.0/ytmusicapi/locales/en/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)      474 2024-05-04 11:36:32.000000 ytmusicapi-1.7.0/ytmusicapi/locales/en/LC_MESSAGES/base.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     1381 2024-05-04 11:36:32.000000 ytmusicapi-1.7.0/ytmusicapi/locales/en/LC_MESSAGES/base.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 11:36:36.996805 ytmusicapi-1.7.0/ytmusicapi/locales/es/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 11:36:37.016805 ytmusicapi-1.7.0/ytmusicapi/locales/es/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     1005 2024-05-04 11:36:32.000000 ytmusicapi-1.7.0/ytmusicapi/locales/es/LC_MESSAGES/base.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     1519 2024-05-04 11:36:32.000000 ytmusicapi-1.7.0/ytmusicapi/locales/es/LC_MESSAGES/base.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 11:36:37.000805 ytmusicapi-1.7.0/ytmusicapi/locales/fr/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 11:36:37.016805 ytmusicapi-1.7.0/ytmusicapi/locales/fr/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)      795 2024-05-04 11:36:32.000000 ytmusicapi-1.7.0/ytmusicapi/locales/fr/LC_MESSAGES/base.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     1460 2024-05-04 11:36:32.000000 ytmusicapi-1.7.0/ytmusicapi/locales/fr/LC_MESSAGES/base.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 11:36:37.000805 ytmusicapi-1.7.0/ytmusicapi/locales/hi/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 11:36:37.020805 ytmusicapi-1.7.0/ytmusicapi/locales/hi/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     1146 2024-05-04 11:36:32.000000 ytmusicapi-1.7.0/ytmusicapi/locales/hi/LC_MESSAGES/base.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     1655 2024-05-04 11:36:32.000000 ytmusicapi-1.7.0/ytmusicapi/locales/hi/LC_MESSAGES/base.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 11:36:37.000805 ytmusicapi-1.7.0/ytmusicapi/locales/it/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 11:36:37.020805 ytmusicapi-1.7.0/ytmusicapi/locales/it/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)      859 2024-05-04 11:36:32.000000 ytmusicapi-1.7.0/ytmusicapi/locales/it/LC_MESSAGES/base.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     1463 2024-05-04 11:36:32.000000 ytmusicapi-1.7.0/ytmusicapi/locales/it/LC_MESSAGES/base.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 11:36:37.000805 ytmusicapi-1.7.0/ytmusicapi/locales/ja/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 11:36:37.020805 ytmusicapi-1.7.0/ytmusicapi/locales/ja/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     1085 2024-05-04 11:36:32.000000 ytmusicapi-1.7.0/ytmusicapi/locales/ja/LC_MESSAGES/base.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     1599 2024-05-04 11:36:32.000000 ytmusicapi-1.7.0/ytmusicapi/locales/ja/LC_MESSAGES/base.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 11:36:37.000805 ytmusicapi-1.7.0/ytmusicapi/locales/ko/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 11:36:37.020805 ytmusicapi-1.7.0/ytmusicapi/locales/ko/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     1009 2024-05-04 11:36:32.000000 ytmusicapi-1.7.0/ytmusicapi/locales/ko/LC_MESSAGES/base.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     1523 2024-05-04 11:36:32.000000 ytmusicapi-1.7.0/ytmusicapi/locales/ko/LC_MESSAGES/base.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 11:36:37.000805 ytmusicapi-1.7.0/ytmusicapi/locales/nl/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 11:36:37.020805 ytmusicapi-1.7.0/ytmusicapi/locales/nl/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)      988 2024-05-04 11:36:32.000000 ytmusicapi-1.7.0/ytmusicapi/locales/nl/LC_MESSAGES/base.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     1526 2024-05-04 11:36:32.000000 ytmusicapi-1.7.0/ytmusicapi/locales/nl/LC_MESSAGES/base.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 11:36:37.000805 ytmusicapi-1.7.0/ytmusicapi/locales/pt/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 11:36:37.020805 ytmusicapi-1.7.0/ytmusicapi/locales/pt/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)      923 2024-05-04 11:36:32.000000 ytmusicapi-1.7.0/ytmusicapi/locales/pt/LC_MESSAGES/base.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     1457 2024-05-04 11:36:32.000000 ytmusicapi-1.7.0/ytmusicapi/locales/pt/LC_MESSAGES/base.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 11:36:37.000805 ytmusicapi-1.7.0/ytmusicapi/locales/ru/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 11:36:37.020805 ytmusicapi-1.7.0/ytmusicapi/locales/ru/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     1044 2024-05-04 11:36:32.000000 ytmusicapi-1.7.0/ytmusicapi/locales/ru/LC_MESSAGES/base.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     1553 2024-05-04 11:36:32.000000 ytmusicapi-1.7.0/ytmusicapi/locales/ru/LC_MESSAGES/base.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 11:36:37.000805 ytmusicapi-1.7.0/ytmusicapi/locales/tr/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 11:36:37.020805 ytmusicapi-1.7.0/ytmusicapi/locales/tr/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)      914 2024-05-04 11:36:32.000000 ytmusicapi-1.7.0/ytmusicapi/locales/tr/LC_MESSAGES/base.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     1448 2024-05-04 11:36:32.000000 ytmusicapi-1.7.0/ytmusicapi/locales/tr/LC_MESSAGES/base.po
+-rw-r--r--   0 runner    (1001) docker     (127)      141 2024-05-04 11:36:32.000000 ytmusicapi-1.7.0/ytmusicapi/locales/update_mo.sh
+-rw-r--r--   0 runner    (1001) docker     (127)      169 2024-05-04 11:36:32.000000 ytmusicapi-1.7.0/ytmusicapi/locales/update_po.sh
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 11:36:37.000805 ytmusicapi-1.7.0/ytmusicapi/locales/ur/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 11:36:37.020805 ytmusicapi-1.7.0/ytmusicapi/locales/ur/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     1013 2024-05-04 11:36:32.000000 ytmusicapi-1.7.0/ytmusicapi/locales/ur/LC_MESSAGES/base.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     1522 2024-05-04 11:36:32.000000 ytmusicapi-1.7.0/ytmusicapi/locales/ur/LC_MESSAGES/base.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 11:36:37.000805 ytmusicapi-1.7.0/ytmusicapi/locales/zh_CN/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 11:36:37.020805 ytmusicapi-1.7.0/ytmusicapi/locales/zh_CN/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)      737 2024-05-04 11:36:32.000000 ytmusicapi-1.7.0/ytmusicapi/locales/zh_CN/LC_MESSAGES/base.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     1479 2024-05-04 11:36:32.000000 ytmusicapi-1.7.0/ytmusicapi/locales/zh_CN/LC_MESSAGES/base.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 11:36:37.000805 ytmusicapi-1.7.0/ytmusicapi/locales/zh_TW/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 11:36:37.020805 ytmusicapi-1.7.0/ytmusicapi/locales/zh_TW/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)      728 2024-05-04 11:36:32.000000 ytmusicapi-1.7.0/ytmusicapi/locales/zh_TW/LC_MESSAGES/base.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     1471 2024-05-04 11:36:32.000000 ytmusicapi-1.7.0/ytmusicapi/locales/zh_TW/LC_MESSAGES/base.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 11:36:37.024805 ytmusicapi-1.7.0/ytmusicapi/mixins/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-04 11:36:32.000000 ytmusicapi-1.7.0/ytmusicapi/mixins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      892 2024-05-04 11:36:32.000000 ytmusicapi-1.7.0/ytmusicapi/mixins/_protocol.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1393 2024-05-04 11:36:32.000000 ytmusicapi-1.7.0/ytmusicapi/mixins/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    39178 2024-05-04 11:36:32.000000 ytmusicapi-1.7.0/ytmusicapi/mixins/browsing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9716 2024-05-04 11:36:32.000000 ytmusicapi-1.7.0/ytmusicapi/mixins/explore.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17492 2024-05-04 11:36:32.000000 ytmusicapi-1.7.0/ytmusicapi/mixins/library.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20529 2024-05-04 11:36:32.000000 ytmusicapi-1.7.0/ytmusicapi/mixins/playlists.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9836 2024-05-04 11:36:32.000000 ytmusicapi-1.7.0/ytmusicapi/mixins/podcasts.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12177 2024-05-04 11:36:32.000000 ytmusicapi-1.7.0/ytmusicapi/mixins/search.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10742 2024-05-04 11:36:32.000000 ytmusicapi-1.7.0/ytmusicapi/mixins/uploads.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7246 2024-05-04 11:36:32.000000 ytmusicapi-1.7.0/ytmusicapi/mixins/watch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5617 2024-05-04 11:36:32.000000 ytmusicapi-1.7.0/ytmusicapi/navigation.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 11:36:37.024805 ytmusicapi-1.7.0/ytmusicapi/parsers/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-04 11:36:32.000000 ytmusicapi-1.7.0/ytmusicapi/parsers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2566 2024-05-04 11:36:32.000000 ytmusicapi-1.7.0/ytmusicapi/parsers/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2766 2024-05-04 11:36:32.000000 ytmusicapi-1.7.0/ytmusicapi/parsers/albums.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5635 2024-05-04 11:36:32.000000 ytmusicapi-1.7.0/ytmusicapi/parsers/browsing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1554 2024-05-04 11:36:32.000000 ytmusicapi-1.7.0/ytmusicapi/parsers/explore.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2494 2024-05-04 11:36:32.000000 ytmusicapi-1.7.0/ytmusicapi/parsers/i18n.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4688 2024-05-04 11:36:32.000000 ytmusicapi-1.7.0/ytmusicapi/parsers/library.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5606 2024-05-04 11:36:32.000000 ytmusicapi-1.7.0/ytmusicapi/parsers/playlists.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4609 2024-05-04 11:36:32.000000 ytmusicapi-1.7.0/ytmusicapi/parsers/podcasts.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9739 2024-05-04 11:36:32.000000 ytmusicapi-1.7.0/ytmusicapi/parsers/search.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2731 2024-05-04 11:36:32.000000 ytmusicapi-1.7.0/ytmusicapi/parsers/songs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1489 2024-05-04 11:36:32.000000 ytmusicapi-1.7.0/ytmusicapi/parsers/uploads.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2123 2024-05-04 11:36:32.000000 ytmusicapi-1.7.0/ytmusicapi/parsers/watch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2662 2024-05-04 11:36:32.000000 ytmusicapi-1.7.0/ytmusicapi/setup.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11518 2024-05-04 11:36:32.000000 ytmusicapi-1.7.0/ytmusicapi/ytmusic.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 11:36:37.024805 ytmusicapi-1.7.0/ytmusicapi.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5512 2024-05-04 11:36:36.000000 ytmusicapi-1.7.0/ytmusicapi.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4042 2024-05-04 11:36:36.000000 ytmusicapi-1.7.0/ytmusicapi.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-04 11:36:36.000000 ytmusicapi-1.7.0/ytmusicapi.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-05-04 11:36:36.000000 ytmusicapi-1.7.0/ytmusicapi.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-04 11:36:36.000000 ytmusicapi-1.7.0/ytmusicapi.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-04 11:36:36.000000 ytmusicapi-1.7.0/ytmusicapi.egg-info/top_level.txt
```

### Comparing `ytmusicapi-1.6.0/.github/ISSUE_TEMPLATE/bug_report.md` & `ytmusicapi-1.7.0/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `ytmusicapi-1.6.0/.github/ISSUE_TEMPLATE/feature_request.md` & `ytmusicapi-1.7.0/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `ytmusicapi-1.6.0/.github/dependabot.yml` & `ytmusicapi-1.7.0/.github/dependabot.yml`

 * *Files identical despite different names*

### Comparing `ytmusicapi-1.6.0/.github/workflows/coverage.yml` & `ytmusicapi-1.7.0/.github/workflows/coverage.yml`

 * *Files identical despite different names*

### Comparing `ytmusicapi-1.6.0/.github/workflows/docsbuild.yml` & `ytmusicapi-1.7.0/.github/workflows/docsbuild.yml`

 * *Files identical despite different names*

### Comparing `ytmusicapi-1.6.0/.github/workflows/lint.yml` & `ytmusicapi-1.7.0/.github/workflows/lint.yml`

 * *Files 14% similar despite different names*

```diff
@@ -10,19 +10,22 @@
 
 jobs:
   ruff:
     runs-on: ubuntu-latest
     steps:
       - uses: actions/checkout@v4
       - uses: chartboost/ruff-action@v1
+        with:
+          version: 0.4.3
       - uses: chartboost/ruff-action@v1
         with:
+          version: 0.4.3
           args: format --check
   mypy:
     runs-on: ubuntu-latest
     steps:
       - uses: actions/checkout@v4
       - uses: actions/setup-python@v5
         with:
           python-version: "3.8"
-      - run: pip install mypy==1.8.0
+      - run: pip install mypy==1.10.0
       - run:  mypy --install-types --non-interactive
```

### Comparing `ytmusicapi-1.6.0/.github/workflows/pythonpublish.yml` & `ytmusicapi-1.7.0/.github/workflows/pythonpublish.yml`

 * *Files identical despite different names*

### Comparing `ytmusicapi-1.6.0/CONTRIBUTING.rst` & `ytmusicapi-1.7.0/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `ytmusicapi-1.6.0/LICENSE` & `ytmusicapi-1.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ytmusicapi-1.6.0/PKG-INFO` & `ytmusicapi-1.7.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ytmusicapi
-Version: 1.6.0
+Version: 1.7.0
 Summary: Unofficial API for YouTube Music
 Author-email: sigma67 <ytmusicapi@gmail.com>
 License: MIT License
         
         Copyright (c) 2024 sigma67
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -34,35 +34,37 @@
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 Requires-Dist: requests>=2.22
 
 ytmusicapi: Unofficial API for YouTube Music
 ############################################
 
-.. image:: https://img.shields.io/pypi/dm/ytmusicapi?style=flat-square
+.. |pypi-downloads| image:: https://img.shields.io/pypi/dm/ytmusicapi?style=flat-square
     :alt: PyPI Downloads
     :target: https://pypi.org/project/ytmusicapi/
 
-.. image:: https://badges.gitter.im/sigma67/ytmusicapi.svg
+.. |gitter| image:: https://badges.gitter.im/sigma67/ytmusicapi.svg
    :alt: Ask questions at https://gitter.im/sigma67/ytmusicapi
    :target: https://gitter.im/sigma67/ytmusicapi
 
-.. image:: https://img.shields.io/codecov/c/github/sigma67/ytmusicapi?style=flat-square
+.. |code-coverage| image:: https://img.shields.io/codecov/c/github/sigma67/ytmusicapi?style=flat-square
     :alt: Code coverage
     :target: https://codecov.io/gh/sigma67/ytmusicapi
 
-.. image:: https://img.shields.io/github/v/release/sigma67/ytmusicapi?style=flat-square
+.. |latest-release| image:: https://img.shields.io/github/v/release/sigma67/ytmusicapi?style=flat-square
     :alt: Latest release
     :target: https://github.com/sigma67/ytmusicapi/releases/latest
 
-.. image:: https://img.shields.io/github/commits-since/sigma67/ytmusicapi/latest?style=flat-square
+.. |commits-since-latest| image:: https://img.shields.io/github/commits-since/sigma67/ytmusicapi/latest?style=flat-square
     :alt: Commits since latest release
     :target: https://github.com/sigma67/ytmusicapi/commits
 
 
+|pypi-downloads| |gitter| |code-coverage| |latest-release| |commits-since-latest|
+
 ytmusicapi is a Python 3 library to send requests to the YouTube Music API.
 It emulates YouTube Music web client requests using the user's cookie data for authentication.
 
 .. features
 
 Features
 --------
```

### Comparing `ytmusicapi-1.6.0/README.rst` & `ytmusicapi-1.7.0/README.rst`

 * *Files 9% similar despite different names*

```diff
@@ -1,31 +1,33 @@
 ytmusicapi: Unofficial API for YouTube Music
 ############################################
 
-.. image:: https://img.shields.io/pypi/dm/ytmusicapi?style=flat-square
+.. |pypi-downloads| image:: https://img.shields.io/pypi/dm/ytmusicapi?style=flat-square
     :alt: PyPI Downloads
     :target: https://pypi.org/project/ytmusicapi/
 
-.. image:: https://badges.gitter.im/sigma67/ytmusicapi.svg
+.. |gitter| image:: https://badges.gitter.im/sigma67/ytmusicapi.svg
    :alt: Ask questions at https://gitter.im/sigma67/ytmusicapi
    :target: https://gitter.im/sigma67/ytmusicapi
 
-.. image:: https://img.shields.io/codecov/c/github/sigma67/ytmusicapi?style=flat-square
+.. |code-coverage| image:: https://img.shields.io/codecov/c/github/sigma67/ytmusicapi?style=flat-square
     :alt: Code coverage
     :target: https://codecov.io/gh/sigma67/ytmusicapi
 
-.. image:: https://img.shields.io/github/v/release/sigma67/ytmusicapi?style=flat-square
+.. |latest-release| image:: https://img.shields.io/github/v/release/sigma67/ytmusicapi?style=flat-square
     :alt: Latest release
     :target: https://github.com/sigma67/ytmusicapi/releases/latest
 
-.. image:: https://img.shields.io/github/commits-since/sigma67/ytmusicapi/latest?style=flat-square
+.. |commits-since-latest| image:: https://img.shields.io/github/commits-since/sigma67/ytmusicapi/latest?style=flat-square
     :alt: Commits since latest release
     :target: https://github.com/sigma67/ytmusicapi/commits
 
 
+|pypi-downloads| |gitter| |code-coverage| |latest-release| |commits-since-latest|
+
 ytmusicapi is a Python 3 library to send requests to the YouTube Music API.
 It emulates YouTube Music web client requests using the user's cookie data for authentication.
 
 .. features
 
 Features
 --------
```

### Comparing `ytmusicapi-1.6.0/docs/Makefile` & `ytmusicapi-1.7.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `ytmusicapi-1.6.0/docs/make.bat` & `ytmusicapi-1.7.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `ytmusicapi-1.6.0/docs/source/conf.py` & `ytmusicapi-1.7.0/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `ytmusicapi-1.6.0/docs/source/faq.rst` & `ytmusicapi-1.7.0/docs/source/faq.rst`

 * *Files identical despite different names*

### Comparing `ytmusicapi-1.6.0/docs/source/index.rst` & `ytmusicapi-1.7.0/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `ytmusicapi-1.6.0/docs/source/reference.rst` & `ytmusicapi-1.7.0/docs/source/reference.rst`

 * *Files identical despite different names*

### Comparing `ytmusicapi-1.6.0/docs/source/setup/browser.rst` & `ytmusicapi-1.7.0/docs/source/setup/browser.rst`

 * *Files identical despite different names*

### Comparing `ytmusicapi-1.6.0/docs/source/usage.rst` & `ytmusicapi-1.7.0/docs/source/usage.rst`

 * *Files identical despite different names*

### Comparing `ytmusicapi-1.6.0/pdm.lock` & `ytmusicapi-1.7.0/pdm.lock`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # This file is @generated by PDM.
 # It is not intended for manual editing.
 
 [metadata]
 groups = ["default", "dev"]
 strategy = ["cross_platform", "inherit_metadata"]
 lock_version = "4.4.1"
-content_hash = "sha256:0685d381623716626cfb292c864b09d36ff40e8d2e7e0a285c97f236aa4d6ddb"
+content_hash = "sha256:ef78505acc5689bac7e9d73819b1e70ca72e3422a79a50b5f2ea451279f0ec18"
 
 [[package]]
 name = "alabaster"
 version = "0.7.13"
 requires_python = ">=3.6"
 summary = "A configurable sidebar-enabled Sphinx theme"
 groups = ["dev"]
@@ -139,137 +139,137 @@
 files = [
     {file = "colorama-0.4.6-py2.py3-none-any.whl", hash = "sha256:4f1d9991f5acc0ca119f9d443620b77f9d6b33703e51011c16baf57afb285fc6"},
     {file = "colorama-0.4.6.tar.gz", hash = "sha256:08695f5cb7ed6e0531a20572697297273c47b8cae5a63ffc6d6ed5c201be6e44"},
 ]
 
 [[package]]
 name = "coverage"
-version = "7.4.3"
+version = "7.5.0"
 requires_python = ">=3.8"
 summary = "Code coverage measurement for Python"
 groups = ["dev"]
 files = [
-    {file = "coverage-7.4.3-cp310-cp310-macosx_10_9_x86_64.whl", hash = "sha256:8580b827d4746d47294c0e0b92854c85a92c2227927433998f0d3320ae8a71b6"},
-    {file = "coverage-7.4.3-cp310-cp310-macosx_11_0_arm64.whl", hash = "sha256:718187eeb9849fc6cc23e0d9b092bc2348821c5e1a901c9f8975df0bc785bfd4"},
-    {file = "coverage-7.4.3-cp310-cp310-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:767b35c3a246bcb55b8044fd3a43b8cd553dd1f9f2c1eeb87a302b1f8daa0524"},
-    {file = "coverage-7.4.3-cp310-cp310-manylinux_2_5_i686.manylinux1_i686.manylinux_2_17_i686.manylinux2014_i686.whl", hash = "sha256:ae7f19afe0cce50039e2c782bff379c7e347cba335429678450b8fe81c4ef96d"},
-    {file = "coverage-7.4.3-cp310-cp310-manylinux_2_5_x86_64.manylinux1_x86_64.manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:ba3a8aaed13770e970b3df46980cb068d1c24af1a1968b7818b69af8c4347efb"},
-    {file = "coverage-7.4.3-cp310-cp310-musllinux_1_1_aarch64.whl", hash = "sha256:ee866acc0861caebb4f2ab79f0b94dbfbdbfadc19f82e6e9c93930f74e11d7a0"},
-    {file = "coverage-7.4.3-cp310-cp310-musllinux_1_1_i686.whl", hash = "sha256:506edb1dd49e13a2d4cac6a5173317b82a23c9d6e8df63efb4f0380de0fbccbc"},
-    {file = "coverage-7.4.3-cp310-cp310-musllinux_1_1_x86_64.whl", hash = "sha256:fd6545d97c98a192c5ac995d21c894b581f1fd14cf389be90724d21808b657e2"},
-    {file = "coverage-7.4.3-cp310-cp310-win32.whl", hash = "sha256:f6a09b360d67e589236a44f0c39218a8efba2593b6abdccc300a8862cffc2f94"},
-    {file = "coverage-7.4.3-cp310-cp310-win_amd64.whl", hash = "sha256:18d90523ce7553dd0b7e23cbb28865db23cddfd683a38fb224115f7826de78d0"},
-    {file = "coverage-7.4.3-cp311-cp311-macosx_10_9_x86_64.whl", hash = "sha256:cbbe5e739d45a52f3200a771c6d2c7acf89eb2524890a4a3aa1a7fa0695d2a47"},
-    {file = "coverage-7.4.3-cp311-cp311-macosx_11_0_arm64.whl", hash = "sha256:489763b2d037b164846ebac0cbd368b8a4ca56385c4090807ff9fad817de4113"},
-    {file = "coverage-7.4.3-cp311-cp311-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:451f433ad901b3bb00184d83fd83d135fb682d780b38af7944c9faeecb1e0bfe"},
-    {file = "coverage-7.4.3-cp311-cp311-manylinux_2_5_i686.manylinux1_i686.manylinux_2_17_i686.manylinux2014_i686.whl", hash = "sha256:fcc66e222cf4c719fe7722a403888b1f5e1682d1679bd780e2b26c18bb648cdc"},
-    {file = "coverage-7.4.3-cp311-cp311-manylinux_2_5_x86_64.manylinux1_x86_64.manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:b3ec74cfef2d985e145baae90d9b1b32f85e1741b04cd967aaf9cfa84c1334f3"},
-    {file = "coverage-7.4.3-cp311-cp311-musllinux_1_1_aarch64.whl", hash = "sha256:abbbd8093c5229c72d4c2926afaee0e6e3140de69d5dcd918b2921f2f0c8baba"},
-    {file = "coverage-7.4.3-cp311-cp311-musllinux_1_1_i686.whl", hash = "sha256:35eb581efdacf7b7422af677b92170da4ef34500467381e805944a3201df2079"},
-    {file = "coverage-7.4.3-cp311-cp311-musllinux_1_1_x86_64.whl", hash = "sha256:8249b1c7334be8f8c3abcaaa996e1e4927b0e5a23b65f5bf6cfe3180d8ca7840"},
-    {file = "coverage-7.4.3-cp311-cp311-win32.whl", hash = "sha256:cf30900aa1ba595312ae41978b95e256e419d8a823af79ce670835409fc02ad3"},
-    {file = "coverage-7.4.3-cp311-cp311-win_amd64.whl", hash = "sha256:18c7320695c949de11a351742ee001849912fd57e62a706d83dfc1581897fa2e"},
-    {file = "coverage-7.4.3-cp312-cp312-macosx_10_9_x86_64.whl", hash = "sha256:b51bfc348925e92a9bd9b2e48dad13431b57011fd1038f08316e6bf1df107d10"},
-    {file = "coverage-7.4.3-cp312-cp312-macosx_11_0_arm64.whl", hash = "sha256:d6cdecaedea1ea9e033d8adf6a0ab11107b49571bbb9737175444cea6eb72328"},
-    {file = "coverage-7.4.3-cp312-cp312-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:3b2eccb883368f9e972e216c7b4c7c06cabda925b5f06dde0650281cb7666a30"},
-    {file = "coverage-7.4.3-cp312-cp312-manylinux_2_5_i686.manylinux1_i686.manylinux_2_17_i686.manylinux2014_i686.whl", hash = "sha256:6c00cdc8fa4e50e1cc1f941a7f2e3e0f26cb2a1233c9696f26963ff58445bac7"},
-    {file = "coverage-7.4.3-cp312-cp312-manylinux_2_5_x86_64.manylinux1_x86_64.manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:b9a4a8dd3dcf4cbd3165737358e4d7dfbd9d59902ad11e3b15eebb6393b0446e"},
-    {file = "coverage-7.4.3-cp312-cp312-musllinux_1_1_aarch64.whl", hash = "sha256:062b0a75d9261e2f9c6d071753f7eef0fc9caf3a2c82d36d76667ba7b6470003"},
-    {file = "coverage-7.4.3-cp312-cp312-musllinux_1_1_i686.whl", hash = "sha256:ebe7c9e67a2d15fa97b77ea6571ce5e1e1f6b0db71d1d5e96f8d2bf134303c1d"},
-    {file = "coverage-7.4.3-cp312-cp312-musllinux_1_1_x86_64.whl", hash = "sha256:c0a120238dd71c68484f02562f6d446d736adcc6ca0993712289b102705a9a3a"},
-    {file = "coverage-7.4.3-cp312-cp312-win32.whl", hash = "sha256:37389611ba54fd6d278fde86eb2c013c8e50232e38f5c68235d09d0a3f8aa352"},
-    {file = "coverage-7.4.3-cp312-cp312-win_amd64.whl", hash = "sha256:d25b937a5d9ffa857d41be042b4238dd61db888533b53bc76dc082cb5a15e914"},
-    {file = "coverage-7.4.3-cp38-cp38-macosx_10_9_x86_64.whl", hash = "sha256:28ca2098939eabab044ad68850aac8f8db6bf0b29bc7f2887d05889b17346454"},
-    {file = "coverage-7.4.3-cp38-cp38-macosx_11_0_arm64.whl", hash = "sha256:280459f0a03cecbe8800786cdc23067a8fc64c0bd51dc614008d9c36e1659d7e"},
-    {file = "coverage-7.4.3-cp38-cp38-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:6c0cdedd3500e0511eac1517bf560149764b7d8e65cb800d8bf1c63ebf39edd2"},
-    {file = "coverage-7.4.3-cp38-cp38-manylinux_2_5_i686.manylinux1_i686.manylinux_2_17_i686.manylinux2014_i686.whl", hash = "sha256:9a9babb9466fe1da12417a4aed923e90124a534736de6201794a3aea9d98484e"},
-    {file = "coverage-7.4.3-cp38-cp38-manylinux_2_5_x86_64.manylinux1_x86_64.manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:dec9de46a33cf2dd87a5254af095a409ea3bf952d85ad339751e7de6d962cde6"},
-    {file = "coverage-7.4.3-cp38-cp38-musllinux_1_1_aarch64.whl", hash = "sha256:16bae383a9cc5abab9bb05c10a3e5a52e0a788325dc9ba8499e821885928968c"},
-    {file = "coverage-7.4.3-cp38-cp38-musllinux_1_1_i686.whl", hash = "sha256:2c854ce44e1ee31bda4e318af1dbcfc929026d12c5ed030095ad98197eeeaed0"},
-    {file = "coverage-7.4.3-cp38-cp38-musllinux_1_1_x86_64.whl", hash = "sha256:ce8c50520f57ec57aa21a63ea4f325c7b657386b3f02ccaedeccf9ebe27686e1"},
-    {file = "coverage-7.4.3-cp38-cp38-win32.whl", hash = "sha256:708a3369dcf055c00ddeeaa2b20f0dd1ce664eeabde6623e516c5228b753654f"},
-    {file = "coverage-7.4.3-cp38-cp38-win_amd64.whl", hash = "sha256:1bf25fbca0c8d121a3e92a2a0555c7e5bc981aee5c3fdaf4bb7809f410f696b9"},
-    {file = "coverage-7.4.3-cp39-cp39-macosx_10_9_x86_64.whl", hash = "sha256:3b253094dbe1b431d3a4ac2f053b6d7ede2664ac559705a704f621742e034f1f"},
-    {file = "coverage-7.4.3-cp39-cp39-macosx_11_0_arm64.whl", hash = "sha256:77fbfc5720cceac9c200054b9fab50cb2a7d79660609200ab83f5db96162d20c"},
-    {file = "coverage-7.4.3-cp39-cp39-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:6679060424faa9c11808598504c3ab472de4531c571ab2befa32f4971835788e"},
-    {file = "coverage-7.4.3-cp39-cp39-manylinux_2_5_i686.manylinux1_i686.manylinux_2_17_i686.manylinux2014_i686.whl", hash = "sha256:4af154d617c875b52651dd8dd17a31270c495082f3d55f6128e7629658d63765"},
-    {file = "coverage-7.4.3-cp39-cp39-manylinux_2_5_x86_64.manylinux1_x86_64.manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:8640f1fde5e1b8e3439fe482cdc2b0bb6c329f4bb161927c28d2e8879c6029ee"},
-    {file = "coverage-7.4.3-cp39-cp39-musllinux_1_1_aarch64.whl", hash = "sha256:69b9f6f66c0af29642e73a520b6fed25ff9fd69a25975ebe6acb297234eda501"},
-    {file = "coverage-7.4.3-cp39-cp39-musllinux_1_1_i686.whl", hash = "sha256:0842571634f39016a6c03e9d4aba502be652a6e4455fadb73cd3a3a49173e38f"},
-    {file = "coverage-7.4.3-cp39-cp39-musllinux_1_1_x86_64.whl", hash = "sha256:a78ed23b08e8ab524551f52953a8a05d61c3a760781762aac49f8de6eede8c45"},
-    {file = "coverage-7.4.3-cp39-cp39-win32.whl", hash = "sha256:c0524de3ff096e15fcbfe8f056fdb4ea0bf497d584454f344d59fce069d3e6e9"},
-    {file = "coverage-7.4.3-cp39-cp39-win_amd64.whl", hash = "sha256:0209a6369ccce576b43bb227dc8322d8ef9e323d089c6f3f26a597b09cb4d2aa"},
-    {file = "coverage-7.4.3-pp38.pp39.pp310-none-any.whl", hash = "sha256:7cbde573904625509a3f37b6fecea974e363460b556a627c60dc2f47e2fffa51"},
-    {file = "coverage-7.4.3.tar.gz", hash = "sha256:276f6077a5c61447a48d133ed13e759c09e62aff0dc84274a68dc18660104d52"},
+    {file = "coverage-7.5.0-cp310-cp310-macosx_10_9_x86_64.whl", hash = "sha256:432949a32c3e3f820af808db1833d6d1631664d53dd3ce487aa25d574e18ad1c"},
+    {file = "coverage-7.5.0-cp310-cp310-macosx_11_0_arm64.whl", hash = "sha256:2bd7065249703cbeb6d4ce679c734bef0ee69baa7bff9724361ada04a15b7e3b"},
+    {file = "coverage-7.5.0-cp310-cp310-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:bbfe6389c5522b99768a93d89aca52ef92310a96b99782973b9d11e80511f932"},
+    {file = "coverage-7.5.0-cp310-cp310-manylinux_2_5_i686.manylinux1_i686.manylinux_2_17_i686.manylinux2014_i686.whl", hash = "sha256:39793731182c4be939b4be0cdecde074b833f6171313cf53481f869937129ed3"},
+    {file = "coverage-7.5.0-cp310-cp310-manylinux_2_5_x86_64.manylinux1_x86_64.manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:85a5dbe1ba1bf38d6c63b6d2c42132d45cbee6d9f0c51b52c59aa4afba057517"},
+    {file = "coverage-7.5.0-cp310-cp310-musllinux_1_1_aarch64.whl", hash = "sha256:357754dcdfd811462a725e7501a9b4556388e8ecf66e79df6f4b988fa3d0b39a"},
+    {file = "coverage-7.5.0-cp310-cp310-musllinux_1_1_i686.whl", hash = "sha256:a81eb64feded34f40c8986869a2f764f0fe2db58c0530d3a4afbcde50f314880"},
+    {file = "coverage-7.5.0-cp310-cp310-musllinux_1_1_x86_64.whl", hash = "sha256:51431d0abbed3a868e967f8257c5faf283d41ec882f58413cf295a389bb22e58"},
+    {file = "coverage-7.5.0-cp310-cp310-win32.whl", hash = "sha256:f609ebcb0242d84b7adeee2b06c11a2ddaec5464d21888b2c8255f5fd6a98ae4"},
+    {file = "coverage-7.5.0-cp310-cp310-win_amd64.whl", hash = "sha256:6782cd6216fab5a83216cc39f13ebe30adfac2fa72688c5a4d8d180cd52e8f6a"},
+    {file = "coverage-7.5.0-cp311-cp311-macosx_10_9_x86_64.whl", hash = "sha256:e768d870801f68c74c2b669fc909839660180c366501d4cc4b87efd6b0eee375"},
+    {file = "coverage-7.5.0-cp311-cp311-macosx_11_0_arm64.whl", hash = "sha256:84921b10aeb2dd453247fd10de22907984eaf80901b578a5cf0bb1e279a587cb"},
+    {file = "coverage-7.5.0-cp311-cp311-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:710c62b6e35a9a766b99b15cdc56d5aeda0914edae8bb467e9c355f75d14ee95"},
+    {file = "coverage-7.5.0-cp311-cp311-manylinux_2_5_i686.manylinux1_i686.manylinux_2_17_i686.manylinux2014_i686.whl", hash = "sha256:c379cdd3efc0658e652a14112d51a7668f6bfca7445c5a10dee7eabecabba19d"},
+    {file = "coverage-7.5.0-cp311-cp311-manylinux_2_5_x86_64.manylinux1_x86_64.manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:fea9d3ca80bcf17edb2c08a4704259dadac196fe5e9274067e7a20511fad1743"},
+    {file = "coverage-7.5.0-cp311-cp311-musllinux_1_1_aarch64.whl", hash = "sha256:41327143c5b1d715f5f98a397608f90ab9ebba606ae4e6f3389c2145410c52b1"},
+    {file = "coverage-7.5.0-cp311-cp311-musllinux_1_1_i686.whl", hash = "sha256:565b2e82d0968c977e0b0f7cbf25fd06d78d4856289abc79694c8edcce6eb2de"},
+    {file = "coverage-7.5.0-cp311-cp311-musllinux_1_1_x86_64.whl", hash = "sha256:cf3539007202ebfe03923128fedfdd245db5860a36810136ad95a564a2fdffff"},
+    {file = "coverage-7.5.0-cp311-cp311-win32.whl", hash = "sha256:bf0b4b8d9caa8d64df838e0f8dcf68fb570c5733b726d1494b87f3da85db3a2d"},
+    {file = "coverage-7.5.0-cp311-cp311-win_amd64.whl", hash = "sha256:9c6384cc90e37cfb60435bbbe0488444e54b98700f727f16f64d8bfda0b84656"},
+    {file = "coverage-7.5.0-cp312-cp312-macosx_10_9_x86_64.whl", hash = "sha256:fed7a72d54bd52f4aeb6c6e951f363903bd7d70bc1cad64dd1f087980d309ab9"},
+    {file = "coverage-7.5.0-cp312-cp312-macosx_11_0_arm64.whl", hash = "sha256:cbe6581fcff7c8e262eb574244f81f5faaea539e712a058e6707a9d272fe5b64"},
+    {file = "coverage-7.5.0-cp312-cp312-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:ad97ec0da94b378e593ef532b980c15e377df9b9608c7c6da3506953182398af"},
+    {file = "coverage-7.5.0-cp312-cp312-manylinux_2_5_i686.manylinux1_i686.manylinux_2_17_i686.manylinux2014_i686.whl", hash = "sha256:bd4bacd62aa2f1a1627352fe68885d6ee694bdaebb16038b6e680f2924a9b2cc"},
+    {file = "coverage-7.5.0-cp312-cp312-manylinux_2_5_x86_64.manylinux1_x86_64.manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:adf032b6c105881f9d77fa17d9eebe0ad1f9bfb2ad25777811f97c5362aa07f2"},
+    {file = "coverage-7.5.0-cp312-cp312-musllinux_1_1_aarch64.whl", hash = "sha256:4ba01d9ba112b55bfa4b24808ec431197bb34f09f66f7cb4fd0258ff9d3711b1"},
+    {file = "coverage-7.5.0-cp312-cp312-musllinux_1_1_i686.whl", hash = "sha256:f0bfe42523893c188e9616d853c47685e1c575fe25f737adf473d0405dcfa7eb"},
+    {file = "coverage-7.5.0-cp312-cp312-musllinux_1_1_x86_64.whl", hash = "sha256:a9a7ef30a1b02547c1b23fa9a5564f03c9982fc71eb2ecb7f98c96d7a0db5cf2"},
+    {file = "coverage-7.5.0-cp312-cp312-win32.whl", hash = "sha256:3c2b77f295edb9fcdb6a250f83e6481c679335ca7e6e4a955e4290350f2d22a4"},
+    {file = "coverage-7.5.0-cp312-cp312-win_amd64.whl", hash = "sha256:427e1e627b0963ac02d7c8730ca6d935df10280d230508c0ba059505e9233475"},
+    {file = "coverage-7.5.0-cp38-cp38-macosx_10_9_x86_64.whl", hash = "sha256:9dd88fce54abbdbf4c42fb1fea0e498973d07816f24c0e27a1ecaf91883ce69e"},
+    {file = "coverage-7.5.0-cp38-cp38-macosx_11_0_arm64.whl", hash = "sha256:a898c11dca8f8c97b467138004a30133974aacd572818c383596f8d5b2eb04a9"},
+    {file = "coverage-7.5.0-cp38-cp38-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:07dfdd492d645eea1bd70fb1d6febdcf47db178b0d99161d8e4eed18e7f62fe7"},
+    {file = "coverage-7.5.0-cp38-cp38-manylinux_2_5_i686.manylinux1_i686.manylinux_2_17_i686.manylinux2014_i686.whl", hash = "sha256:d3d117890b6eee85887b1eed41eefe2e598ad6e40523d9f94c4c4b213258e4a4"},
+    {file = "coverage-7.5.0-cp38-cp38-manylinux_2_5_x86_64.manylinux1_x86_64.manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:6afd2e84e7da40fe23ca588379f815fb6dbbb1b757c883935ed11647205111cb"},
+    {file = "coverage-7.5.0-cp38-cp38-musllinux_1_1_aarch64.whl", hash = "sha256:a9960dd1891b2ddf13a7fe45339cd59ecee3abb6b8326d8b932d0c5da208104f"},
+    {file = "coverage-7.5.0-cp38-cp38-musllinux_1_1_i686.whl", hash = "sha256:ced268e82af993d7801a9db2dbc1d2322e786c5dc76295d8e89473d46c6b84d4"},
+    {file = "coverage-7.5.0-cp38-cp38-musllinux_1_1_x86_64.whl", hash = "sha256:e7c211f25777746d468d76f11719e64acb40eed410d81c26cefac641975beb88"},
+    {file = "coverage-7.5.0-cp38-cp38-win32.whl", hash = "sha256:262fffc1f6c1a26125d5d573e1ec379285a3723363f3bd9c83923c9593a2ac25"},
+    {file = "coverage-7.5.0-cp38-cp38-win_amd64.whl", hash = "sha256:eed462b4541c540d63ab57b3fc69e7d8c84d5957668854ee4e408b50e92ce26a"},
+    {file = "coverage-7.5.0-cp39-cp39-macosx_10_9_x86_64.whl", hash = "sha256:d0194d654e360b3e6cc9b774e83235bae6b9b2cac3be09040880bb0e8a88f4a1"},
+    {file = "coverage-7.5.0-cp39-cp39-macosx_11_0_arm64.whl", hash = "sha256:33c020d3322662e74bc507fb11488773a96894aa82a622c35a5a28673c0c26f5"},
+    {file = "coverage-7.5.0-cp39-cp39-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:0cbdf2cae14a06827bec50bd58e49249452d211d9caddd8bd80e35b53cb04631"},
+    {file = "coverage-7.5.0-cp39-cp39-manylinux_2_5_i686.manylinux1_i686.manylinux_2_17_i686.manylinux2014_i686.whl", hash = "sha256:3235d7c781232e525b0761730e052388a01548bd7f67d0067a253887c6e8df46"},
+    {file = "coverage-7.5.0-cp39-cp39-manylinux_2_5_x86_64.manylinux1_x86_64.manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:db2de4e546f0ec4b2787d625e0b16b78e99c3e21bc1722b4977c0dddf11ca84e"},
+    {file = "coverage-7.5.0-cp39-cp39-musllinux_1_1_aarch64.whl", hash = "sha256:4d0e206259b73af35c4ec1319fd04003776e11e859936658cb6ceffdeba0f5be"},
+    {file = "coverage-7.5.0-cp39-cp39-musllinux_1_1_i686.whl", hash = "sha256:2055c4fb9a6ff624253d432aa471a37202cd8f458c033d6d989be4499aed037b"},
+    {file = "coverage-7.5.0-cp39-cp39-musllinux_1_1_x86_64.whl", hash = "sha256:075299460948cd12722a970c7eae43d25d37989da682997687b34ae6b87c0ef0"},
+    {file = "coverage-7.5.0-cp39-cp39-win32.whl", hash = "sha256:280132aada3bc2f0fac939a5771db4fbb84f245cb35b94fae4994d4c1f80dae7"},
+    {file = "coverage-7.5.0-cp39-cp39-win_amd64.whl", hash = "sha256:c58536f6892559e030e6924896a44098bc1290663ea12532c78cef71d0df8493"},
+    {file = "coverage-7.5.0-pp38.pp39.pp310-none-any.whl", hash = "sha256:2b57780b51084d5223eee7b59f0d4911c31c16ee5aa12737c7a02455829ff067"},
+    {file = "coverage-7.5.0.tar.gz", hash = "sha256:cf62d17310f34084c59c01e027259076479128d11e4661bb6c9acb38c5e19bb8"},
 ]
 
 [[package]]
 name = "coverage"
-version = "7.4.3"
+version = "7.5.0"
 extras = ["toml"]
 requires_python = ">=3.8"
 summary = "Code coverage measurement for Python"
 groups = ["dev"]
 dependencies = [
-    "coverage==7.4.3",
+    "coverage==7.5.0",
     "tomli; python_full_version <= \"3.11.0a6\"",
 ]
 files = [
-    {file = "coverage-7.4.3-cp310-cp310-macosx_10_9_x86_64.whl", hash = "sha256:8580b827d4746d47294c0e0b92854c85a92c2227927433998f0d3320ae8a71b6"},
-    {file = "coverage-7.4.3-cp310-cp310-macosx_11_0_arm64.whl", hash = "sha256:718187eeb9849fc6cc23e0d9b092bc2348821c5e1a901c9f8975df0bc785bfd4"},
-    {file = "coverage-7.4.3-cp310-cp310-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:767b35c3a246bcb55b8044fd3a43b8cd553dd1f9f2c1eeb87a302b1f8daa0524"},
-    {file = "coverage-7.4.3-cp310-cp310-manylinux_2_5_i686.manylinux1_i686.manylinux_2_17_i686.manylinux2014_i686.whl", hash = "sha256:ae7f19afe0cce50039e2c782bff379c7e347cba335429678450b8fe81c4ef96d"},
-    {file = "coverage-7.4.3-cp310-cp310-manylinux_2_5_x86_64.manylinux1_x86_64.manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:ba3a8aaed13770e970b3df46980cb068d1c24af1a1968b7818b69af8c4347efb"},
-    {file = "coverage-7.4.3-cp310-cp310-musllinux_1_1_aarch64.whl", hash = "sha256:ee866acc0861caebb4f2ab79f0b94dbfbdbfadc19f82e6e9c93930f74e11d7a0"},
-    {file = "coverage-7.4.3-cp310-cp310-musllinux_1_1_i686.whl", hash = "sha256:506edb1dd49e13a2d4cac6a5173317b82a23c9d6e8df63efb4f0380de0fbccbc"},
-    {file = "coverage-7.4.3-cp310-cp310-musllinux_1_1_x86_64.whl", hash = "sha256:fd6545d97c98a192c5ac995d21c894b581f1fd14cf389be90724d21808b657e2"},
-    {file = "coverage-7.4.3-cp310-cp310-win32.whl", hash = "sha256:f6a09b360d67e589236a44f0c39218a8efba2593b6abdccc300a8862cffc2f94"},
-    {file = "coverage-7.4.3-cp310-cp310-win_amd64.whl", hash = "sha256:18d90523ce7553dd0b7e23cbb28865db23cddfd683a38fb224115f7826de78d0"},
-    {file = "coverage-7.4.3-cp311-cp311-macosx_10_9_x86_64.whl", hash = "sha256:cbbe5e739d45a52f3200a771c6d2c7acf89eb2524890a4a3aa1a7fa0695d2a47"},
-    {file = "coverage-7.4.3-cp311-cp311-macosx_11_0_arm64.whl", hash = "sha256:489763b2d037b164846ebac0cbd368b8a4ca56385c4090807ff9fad817de4113"},
-    {file = "coverage-7.4.3-cp311-cp311-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:451f433ad901b3bb00184d83fd83d135fb682d780b38af7944c9faeecb1e0bfe"},
-    {file = "coverage-7.4.3-cp311-cp311-manylinux_2_5_i686.manylinux1_i686.manylinux_2_17_i686.manylinux2014_i686.whl", hash = "sha256:fcc66e222cf4c719fe7722a403888b1f5e1682d1679bd780e2b26c18bb648cdc"},
-    {file = "coverage-7.4.3-cp311-cp311-manylinux_2_5_x86_64.manylinux1_x86_64.manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:b3ec74cfef2d985e145baae90d9b1b32f85e1741b04cd967aaf9cfa84c1334f3"},
-    {file = "coverage-7.4.3-cp311-cp311-musllinux_1_1_aarch64.whl", hash = "sha256:abbbd8093c5229c72d4c2926afaee0e6e3140de69d5dcd918b2921f2f0c8baba"},
-    {file = "coverage-7.4.3-cp311-cp311-musllinux_1_1_i686.whl", hash = "sha256:35eb581efdacf7b7422af677b92170da4ef34500467381e805944a3201df2079"},
-    {file = "coverage-7.4.3-cp311-cp311-musllinux_1_1_x86_64.whl", hash = "sha256:8249b1c7334be8f8c3abcaaa996e1e4927b0e5a23b65f5bf6cfe3180d8ca7840"},
-    {file = "coverage-7.4.3-cp311-cp311-win32.whl", hash = "sha256:cf30900aa1ba595312ae41978b95e256e419d8a823af79ce670835409fc02ad3"},
-    {file = "coverage-7.4.3-cp311-cp311-win_amd64.whl", hash = "sha256:18c7320695c949de11a351742ee001849912fd57e62a706d83dfc1581897fa2e"},
-    {file = "coverage-7.4.3-cp312-cp312-macosx_10_9_x86_64.whl", hash = "sha256:b51bfc348925e92a9bd9b2e48dad13431b57011fd1038f08316e6bf1df107d10"},
-    {file = "coverage-7.4.3-cp312-cp312-macosx_11_0_arm64.whl", hash = "sha256:d6cdecaedea1ea9e033d8adf6a0ab11107b49571bbb9737175444cea6eb72328"},
-    {file = "coverage-7.4.3-cp312-cp312-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:3b2eccb883368f9e972e216c7b4c7c06cabda925b5f06dde0650281cb7666a30"},
-    {file = "coverage-7.4.3-cp312-cp312-manylinux_2_5_i686.manylinux1_i686.manylinux_2_17_i686.manylinux2014_i686.whl", hash = "sha256:6c00cdc8fa4e50e1cc1f941a7f2e3e0f26cb2a1233c9696f26963ff58445bac7"},
-    {file = "coverage-7.4.3-cp312-cp312-manylinux_2_5_x86_64.manylinux1_x86_64.manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:b9a4a8dd3dcf4cbd3165737358e4d7dfbd9d59902ad11e3b15eebb6393b0446e"},
-    {file = "coverage-7.4.3-cp312-cp312-musllinux_1_1_aarch64.whl", hash = "sha256:062b0a75d9261e2f9c6d071753f7eef0fc9caf3a2c82d36d76667ba7b6470003"},
-    {file = "coverage-7.4.3-cp312-cp312-musllinux_1_1_i686.whl", hash = "sha256:ebe7c9e67a2d15fa97b77ea6571ce5e1e1f6b0db71d1d5e96f8d2bf134303c1d"},
-    {file = "coverage-7.4.3-cp312-cp312-musllinux_1_1_x86_64.whl", hash = "sha256:c0a120238dd71c68484f02562f6d446d736adcc6ca0993712289b102705a9a3a"},
-    {file = "coverage-7.4.3-cp312-cp312-win32.whl", hash = "sha256:37389611ba54fd6d278fde86eb2c013c8e50232e38f5c68235d09d0a3f8aa352"},
-    {file = "coverage-7.4.3-cp312-cp312-win_amd64.whl", hash = "sha256:d25b937a5d9ffa857d41be042b4238dd61db888533b53bc76dc082cb5a15e914"},
-    {file = "coverage-7.4.3-cp38-cp38-macosx_10_9_x86_64.whl", hash = "sha256:28ca2098939eabab044ad68850aac8f8db6bf0b29bc7f2887d05889b17346454"},
-    {file = "coverage-7.4.3-cp38-cp38-macosx_11_0_arm64.whl", hash = "sha256:280459f0a03cecbe8800786cdc23067a8fc64c0bd51dc614008d9c36e1659d7e"},
-    {file = "coverage-7.4.3-cp38-cp38-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:6c0cdedd3500e0511eac1517bf560149764b7d8e65cb800d8bf1c63ebf39edd2"},
-    {file = "coverage-7.4.3-cp38-cp38-manylinux_2_5_i686.manylinux1_i686.manylinux_2_17_i686.manylinux2014_i686.whl", hash = "sha256:9a9babb9466fe1da12417a4aed923e90124a534736de6201794a3aea9d98484e"},
-    {file = "coverage-7.4.3-cp38-cp38-manylinux_2_5_x86_64.manylinux1_x86_64.manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:dec9de46a33cf2dd87a5254af095a409ea3bf952d85ad339751e7de6d962cde6"},
-    {file = "coverage-7.4.3-cp38-cp38-musllinux_1_1_aarch64.whl", hash = "sha256:16bae383a9cc5abab9bb05c10a3e5a52e0a788325dc9ba8499e821885928968c"},
-    {file = "coverage-7.4.3-cp38-cp38-musllinux_1_1_i686.whl", hash = "sha256:2c854ce44e1ee31bda4e318af1dbcfc929026d12c5ed030095ad98197eeeaed0"},
-    {file = "coverage-7.4.3-cp38-cp38-musllinux_1_1_x86_64.whl", hash = "sha256:ce8c50520f57ec57aa21a63ea4f325c7b657386b3f02ccaedeccf9ebe27686e1"},
-    {file = "coverage-7.4.3-cp38-cp38-win32.whl", hash = "sha256:708a3369dcf055c00ddeeaa2b20f0dd1ce664eeabde6623e516c5228b753654f"},
-    {file = "coverage-7.4.3-cp38-cp38-win_amd64.whl", hash = "sha256:1bf25fbca0c8d121a3e92a2a0555c7e5bc981aee5c3fdaf4bb7809f410f696b9"},
-    {file = "coverage-7.4.3-cp39-cp39-macosx_10_9_x86_64.whl", hash = "sha256:3b253094dbe1b431d3a4ac2f053b6d7ede2664ac559705a704f621742e034f1f"},
-    {file = "coverage-7.4.3-cp39-cp39-macosx_11_0_arm64.whl", hash = "sha256:77fbfc5720cceac9c200054b9fab50cb2a7d79660609200ab83f5db96162d20c"},
-    {file = "coverage-7.4.3-cp39-cp39-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:6679060424faa9c11808598504c3ab472de4531c571ab2befa32f4971835788e"},
-    {file = "coverage-7.4.3-cp39-cp39-manylinux_2_5_i686.manylinux1_i686.manylinux_2_17_i686.manylinux2014_i686.whl", hash = "sha256:4af154d617c875b52651dd8dd17a31270c495082f3d55f6128e7629658d63765"},
-    {file = "coverage-7.4.3-cp39-cp39-manylinux_2_5_x86_64.manylinux1_x86_64.manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:8640f1fde5e1b8e3439fe482cdc2b0bb6c329f4bb161927c28d2e8879c6029ee"},
-    {file = "coverage-7.4.3-cp39-cp39-musllinux_1_1_aarch64.whl", hash = "sha256:69b9f6f66c0af29642e73a520b6fed25ff9fd69a25975ebe6acb297234eda501"},
-    {file = "coverage-7.4.3-cp39-cp39-musllinux_1_1_i686.whl", hash = "sha256:0842571634f39016a6c03e9d4aba502be652a6e4455fadb73cd3a3a49173e38f"},
-    {file = "coverage-7.4.3-cp39-cp39-musllinux_1_1_x86_64.whl", hash = "sha256:a78ed23b08e8ab524551f52953a8a05d61c3a760781762aac49f8de6eede8c45"},
-    {file = "coverage-7.4.3-cp39-cp39-win32.whl", hash = "sha256:c0524de3ff096e15fcbfe8f056fdb4ea0bf497d584454f344d59fce069d3e6e9"},
-    {file = "coverage-7.4.3-cp39-cp39-win_amd64.whl", hash = "sha256:0209a6369ccce576b43bb227dc8322d8ef9e323d089c6f3f26a597b09cb4d2aa"},
-    {file = "coverage-7.4.3-pp38.pp39.pp310-none-any.whl", hash = "sha256:7cbde573904625509a3f37b6fecea974e363460b556a627c60dc2f47e2fffa51"},
-    {file = "coverage-7.4.3.tar.gz", hash = "sha256:276f6077a5c61447a48d133ed13e759c09e62aff0dc84274a68dc18660104d52"},
+    {file = "coverage-7.5.0-cp310-cp310-macosx_10_9_x86_64.whl", hash = "sha256:432949a32c3e3f820af808db1833d6d1631664d53dd3ce487aa25d574e18ad1c"},
+    {file = "coverage-7.5.0-cp310-cp310-macosx_11_0_arm64.whl", hash = "sha256:2bd7065249703cbeb6d4ce679c734bef0ee69baa7bff9724361ada04a15b7e3b"},
+    {file = "coverage-7.5.0-cp310-cp310-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:bbfe6389c5522b99768a93d89aca52ef92310a96b99782973b9d11e80511f932"},
+    {file = "coverage-7.5.0-cp310-cp310-manylinux_2_5_i686.manylinux1_i686.manylinux_2_17_i686.manylinux2014_i686.whl", hash = "sha256:39793731182c4be939b4be0cdecde074b833f6171313cf53481f869937129ed3"},
+    {file = "coverage-7.5.0-cp310-cp310-manylinux_2_5_x86_64.manylinux1_x86_64.manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:85a5dbe1ba1bf38d6c63b6d2c42132d45cbee6d9f0c51b52c59aa4afba057517"},
+    {file = "coverage-7.5.0-cp310-cp310-musllinux_1_1_aarch64.whl", hash = "sha256:357754dcdfd811462a725e7501a9b4556388e8ecf66e79df6f4b988fa3d0b39a"},
+    {file = "coverage-7.5.0-cp310-cp310-musllinux_1_1_i686.whl", hash = "sha256:a81eb64feded34f40c8986869a2f764f0fe2db58c0530d3a4afbcde50f314880"},
+    {file = "coverage-7.5.0-cp310-cp310-musllinux_1_1_x86_64.whl", hash = "sha256:51431d0abbed3a868e967f8257c5faf283d41ec882f58413cf295a389bb22e58"},
+    {file = "coverage-7.5.0-cp310-cp310-win32.whl", hash = "sha256:f609ebcb0242d84b7adeee2b06c11a2ddaec5464d21888b2c8255f5fd6a98ae4"},
+    {file = "coverage-7.5.0-cp310-cp310-win_amd64.whl", hash = "sha256:6782cd6216fab5a83216cc39f13ebe30adfac2fa72688c5a4d8d180cd52e8f6a"},
+    {file = "coverage-7.5.0-cp311-cp311-macosx_10_9_x86_64.whl", hash = "sha256:e768d870801f68c74c2b669fc909839660180c366501d4cc4b87efd6b0eee375"},
+    {file = "coverage-7.5.0-cp311-cp311-macosx_11_0_arm64.whl", hash = "sha256:84921b10aeb2dd453247fd10de22907984eaf80901b578a5cf0bb1e279a587cb"},
+    {file = "coverage-7.5.0-cp311-cp311-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:710c62b6e35a9a766b99b15cdc56d5aeda0914edae8bb467e9c355f75d14ee95"},
+    {file = "coverage-7.5.0-cp311-cp311-manylinux_2_5_i686.manylinux1_i686.manylinux_2_17_i686.manylinux2014_i686.whl", hash = "sha256:c379cdd3efc0658e652a14112d51a7668f6bfca7445c5a10dee7eabecabba19d"},
+    {file = "coverage-7.5.0-cp311-cp311-manylinux_2_5_x86_64.manylinux1_x86_64.manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:fea9d3ca80bcf17edb2c08a4704259dadac196fe5e9274067e7a20511fad1743"},
+    {file = "coverage-7.5.0-cp311-cp311-musllinux_1_1_aarch64.whl", hash = "sha256:41327143c5b1d715f5f98a397608f90ab9ebba606ae4e6f3389c2145410c52b1"},
+    {file = "coverage-7.5.0-cp311-cp311-musllinux_1_1_i686.whl", hash = "sha256:565b2e82d0968c977e0b0f7cbf25fd06d78d4856289abc79694c8edcce6eb2de"},
+    {file = "coverage-7.5.0-cp311-cp311-musllinux_1_1_x86_64.whl", hash = "sha256:cf3539007202ebfe03923128fedfdd245db5860a36810136ad95a564a2fdffff"},
+    {file = "coverage-7.5.0-cp311-cp311-win32.whl", hash = "sha256:bf0b4b8d9caa8d64df838e0f8dcf68fb570c5733b726d1494b87f3da85db3a2d"},
+    {file = "coverage-7.5.0-cp311-cp311-win_amd64.whl", hash = "sha256:9c6384cc90e37cfb60435bbbe0488444e54b98700f727f16f64d8bfda0b84656"},
+    {file = "coverage-7.5.0-cp312-cp312-macosx_10_9_x86_64.whl", hash = "sha256:fed7a72d54bd52f4aeb6c6e951f363903bd7d70bc1cad64dd1f087980d309ab9"},
+    {file = "coverage-7.5.0-cp312-cp312-macosx_11_0_arm64.whl", hash = "sha256:cbe6581fcff7c8e262eb574244f81f5faaea539e712a058e6707a9d272fe5b64"},
+    {file = "coverage-7.5.0-cp312-cp312-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:ad97ec0da94b378e593ef532b980c15e377df9b9608c7c6da3506953182398af"},
+    {file = "coverage-7.5.0-cp312-cp312-manylinux_2_5_i686.manylinux1_i686.manylinux_2_17_i686.manylinux2014_i686.whl", hash = "sha256:bd4bacd62aa2f1a1627352fe68885d6ee694bdaebb16038b6e680f2924a9b2cc"},
+    {file = "coverage-7.5.0-cp312-cp312-manylinux_2_5_x86_64.manylinux1_x86_64.manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:adf032b6c105881f9d77fa17d9eebe0ad1f9bfb2ad25777811f97c5362aa07f2"},
+    {file = "coverage-7.5.0-cp312-cp312-musllinux_1_1_aarch64.whl", hash = "sha256:4ba01d9ba112b55bfa4b24808ec431197bb34f09f66f7cb4fd0258ff9d3711b1"},
+    {file = "coverage-7.5.0-cp312-cp312-musllinux_1_1_i686.whl", hash = "sha256:f0bfe42523893c188e9616d853c47685e1c575fe25f737adf473d0405dcfa7eb"},
+    {file = "coverage-7.5.0-cp312-cp312-musllinux_1_1_x86_64.whl", hash = "sha256:a9a7ef30a1b02547c1b23fa9a5564f03c9982fc71eb2ecb7f98c96d7a0db5cf2"},
+    {file = "coverage-7.5.0-cp312-cp312-win32.whl", hash = "sha256:3c2b77f295edb9fcdb6a250f83e6481c679335ca7e6e4a955e4290350f2d22a4"},
+    {file = "coverage-7.5.0-cp312-cp312-win_amd64.whl", hash = "sha256:427e1e627b0963ac02d7c8730ca6d935df10280d230508c0ba059505e9233475"},
+    {file = "coverage-7.5.0-cp38-cp38-macosx_10_9_x86_64.whl", hash = "sha256:9dd88fce54abbdbf4c42fb1fea0e498973d07816f24c0e27a1ecaf91883ce69e"},
+    {file = "coverage-7.5.0-cp38-cp38-macosx_11_0_arm64.whl", hash = "sha256:a898c11dca8f8c97b467138004a30133974aacd572818c383596f8d5b2eb04a9"},
+    {file = "coverage-7.5.0-cp38-cp38-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:07dfdd492d645eea1bd70fb1d6febdcf47db178b0d99161d8e4eed18e7f62fe7"},
+    {file = "coverage-7.5.0-cp38-cp38-manylinux_2_5_i686.manylinux1_i686.manylinux_2_17_i686.manylinux2014_i686.whl", hash = "sha256:d3d117890b6eee85887b1eed41eefe2e598ad6e40523d9f94c4c4b213258e4a4"},
+    {file = "coverage-7.5.0-cp38-cp38-manylinux_2_5_x86_64.manylinux1_x86_64.manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:6afd2e84e7da40fe23ca588379f815fb6dbbb1b757c883935ed11647205111cb"},
+    {file = "coverage-7.5.0-cp38-cp38-musllinux_1_1_aarch64.whl", hash = "sha256:a9960dd1891b2ddf13a7fe45339cd59ecee3abb6b8326d8b932d0c5da208104f"},
+    {file = "coverage-7.5.0-cp38-cp38-musllinux_1_1_i686.whl", hash = "sha256:ced268e82af993d7801a9db2dbc1d2322e786c5dc76295d8e89473d46c6b84d4"},
+    {file = "coverage-7.5.0-cp38-cp38-musllinux_1_1_x86_64.whl", hash = "sha256:e7c211f25777746d468d76f11719e64acb40eed410d81c26cefac641975beb88"},
+    {file = "coverage-7.5.0-cp38-cp38-win32.whl", hash = "sha256:262fffc1f6c1a26125d5d573e1ec379285a3723363f3bd9c83923c9593a2ac25"},
+    {file = "coverage-7.5.0-cp38-cp38-win_amd64.whl", hash = "sha256:eed462b4541c540d63ab57b3fc69e7d8c84d5957668854ee4e408b50e92ce26a"},
+    {file = "coverage-7.5.0-cp39-cp39-macosx_10_9_x86_64.whl", hash = "sha256:d0194d654e360b3e6cc9b774e83235bae6b9b2cac3be09040880bb0e8a88f4a1"},
+    {file = "coverage-7.5.0-cp39-cp39-macosx_11_0_arm64.whl", hash = "sha256:33c020d3322662e74bc507fb11488773a96894aa82a622c35a5a28673c0c26f5"},
+    {file = "coverage-7.5.0-cp39-cp39-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:0cbdf2cae14a06827bec50bd58e49249452d211d9caddd8bd80e35b53cb04631"},
+    {file = "coverage-7.5.0-cp39-cp39-manylinux_2_5_i686.manylinux1_i686.manylinux_2_17_i686.manylinux2014_i686.whl", hash = "sha256:3235d7c781232e525b0761730e052388a01548bd7f67d0067a253887c6e8df46"},
+    {file = "coverage-7.5.0-cp39-cp39-manylinux_2_5_x86_64.manylinux1_x86_64.manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:db2de4e546f0ec4b2787d625e0b16b78e99c3e21bc1722b4977c0dddf11ca84e"},
+    {file = "coverage-7.5.0-cp39-cp39-musllinux_1_1_aarch64.whl", hash = "sha256:4d0e206259b73af35c4ec1319fd04003776e11e859936658cb6ceffdeba0f5be"},
+    {file = "coverage-7.5.0-cp39-cp39-musllinux_1_1_i686.whl", hash = "sha256:2055c4fb9a6ff624253d432aa471a37202cd8f458c033d6d989be4499aed037b"},
+    {file = "coverage-7.5.0-cp39-cp39-musllinux_1_1_x86_64.whl", hash = "sha256:075299460948cd12722a970c7eae43d25d37989da682997687b34ae6b87c0ef0"},
+    {file = "coverage-7.5.0-cp39-cp39-win32.whl", hash = "sha256:280132aada3bc2f0fac939a5771db4fbb84f245cb35b94fae4994d4c1f80dae7"},
+    {file = "coverage-7.5.0-cp39-cp39-win_amd64.whl", hash = "sha256:c58536f6892559e030e6924896a44098bc1290663ea12532c78cef71d0df8493"},
+    {file = "coverage-7.5.0-pp38.pp39.pp310-none-any.whl", hash = "sha256:2b57780b51084d5223eee7b59f0d4911c31c16ee5aa12737c7a02455829ff067"},
+    {file = "coverage-7.5.0.tar.gz", hash = "sha256:cf62d17310f34084c59c01e027259076479128d11e4661bb6c9acb38c5e19bb8"},
 ]
 
 [[package]]
 name = "docutils"
 version = "0.19"
 requires_python = ">=3.7"
 summary = "Docutils -- Python Documentation Utilities"
@@ -277,33 +277,33 @@
 files = [
     {file = "docutils-0.19-py3-none-any.whl", hash = "sha256:5e1de4d849fee02c63b040a4a3fd567f4ab104defd8a5511fbbc24a8a017efbc"},
     {file = "docutils-0.19.tar.gz", hash = "sha256:33995a6753c30b7f577febfc2c50411fec6aac7f7ffeb7c4cfe5991072dcf9e6"},
 ]
 
 [[package]]
 name = "exceptiongroup"
-version = "1.2.0"
+version = "1.2.1"
 requires_python = ">=3.7"
 summary = "Backport of PEP 654 (exception groups)"
 groups = ["dev"]
 marker = "python_version < \"3.11\""
 files = [
-    {file = "exceptiongroup-1.2.0-py3-none-any.whl", hash = "sha256:4bfd3996ac73b41e9b9628b04e079f193850720ea5945fc96a08633c66912f14"},
-    {file = "exceptiongroup-1.2.0.tar.gz", hash = "sha256:91f5c769735f051a4290d52edd0858999b57e5876e9f85937691bd4c9fa3ed68"},
+    {file = "exceptiongroup-1.2.1-py3-none-any.whl", hash = "sha256:5258b9ed329c5bbdd31a309f53cbfb0b155341807f6ff7606a1e801a891b29ad"},
+    {file = "exceptiongroup-1.2.1.tar.gz", hash = "sha256:a4785e48b045528f5bfe627b6ad554ff32def154f42372786903b7abcfe1aa16"},
 ]
 
 [[package]]
 name = "idna"
-version = "3.6"
+version = "3.7"
 requires_python = ">=3.5"
 summary = "Internationalized Domain Names in Applications (IDNA)"
 groups = ["default", "dev"]
 files = [
-    {file = "idna-3.6-py3-none-any.whl", hash = "sha256:c05567e9c24a6b9faaa835c4821bad0590fbb9d5779e7caa6e1cc4978e7eb24f"},
-    {file = "idna-3.6.tar.gz", hash = "sha256:9ecdbbd083b06798ae1e86adcbfe8ab1479cf864e4ee30fe4e46a003d12491ca"},
+    {file = "idna-3.7-py3-none-any.whl", hash = "sha256:82fee1fc78add43492d3a1898bfa6d8a904cc97d8427f683ed8e798d07761aa0"},
+    {file = "idna-3.7.tar.gz", hash = "sha256:028ff3aadf0609c1fd278d8ea3089299412a7a8b9bd005dd08b9f8285bcb5cfc"},
 ]
 
 [[package]]
 name = "imagesize"
 version = "1.4.1"
 requires_python = ">=2.7, !=3.0.*, !=3.1.*, !=3.2.*, !=3.3.*"
 summary = "Getting image size from png/jpeg/jpeg2000/gif file"
@@ -311,25 +311,25 @@
 files = [
     {file = "imagesize-1.4.1-py2.py3-none-any.whl", hash = "sha256:0d8d18d08f840c19d0ee7ca1fd82490fdc3729b7ac93f49870406ddde8ef8d8b"},
     {file = "imagesize-1.4.1.tar.gz", hash = "sha256:69150444affb9cb0d5cc5a92b3676f0b2fb7cd9ae39e947a5e11a36b4497cd4a"},
 ]
 
 [[package]]
 name = "importlib-metadata"
-version = "7.0.1"
+version = "7.1.0"
 requires_python = ">=3.8"
 summary = "Read metadata from Python packages"
 groups = ["dev"]
 marker = "python_version < \"3.10\""
 dependencies = [
     "zipp>=0.5",
 ]
 files = [
-    {file = "importlib_metadata-7.0.1-py3-none-any.whl", hash = "sha256:4805911c3a4ec7c3966410053e9ec6a1fecd629117df5adee56dfc9432a1081e"},
-    {file = "importlib_metadata-7.0.1.tar.gz", hash = "sha256:f238736bb06590ae52ac1fab06a3a9ef1d8dce2b7a35b5ab329371d6c8f5d2cc"},
+    {file = "importlib_metadata-7.1.0-py3-none-any.whl", hash = "sha256:30962b96c0c223483ed6cc7280e7f0199feb01a0e40cfae4d4450fc6fab1f570"},
+    {file = "importlib_metadata-7.1.0.tar.gz", hash = "sha256:b78938b926ee8d5f020fc4772d487045805a55ddbad2ecf21c6d60938dc7fcd2"},
 ]
 
 [[package]]
 name = "iniconfig"
 version = "2.0.0"
 requires_python = ">=3.7"
 summary = "brain-dead simple config-ini parsing"
@@ -411,51 +411,51 @@
     {file = "MarkupSafe-2.1.5-cp39-cp39-win32.whl", hash = "sha256:00e046b6dd71aa03a41079792f8473dc494d564611a8f89bbbd7cb93295ebdcf"},
     {file = "MarkupSafe-2.1.5-cp39-cp39-win_amd64.whl", hash = "sha256:fa173ec60341d6bb97a89f5ea19c85c5643c1e7dedebc22f5181eb73573142c5"},
     {file = "MarkupSafe-2.1.5.tar.gz", hash = "sha256:d283d37a890ba4c1ae73ffadf8046435c76e7bc2247bbb63c00bd1a709c6544b"},
 ]
 
 [[package]]
 name = "mypy"
-version = "1.8.0"
+version = "1.10.0"
 requires_python = ">=3.8"
 summary = "Optional static typing for Python"
 groups = ["dev"]
 dependencies = [
     "mypy-extensions>=1.0.0",
     "tomli>=1.1.0; python_version < \"3.11\"",
     "typing-extensions>=4.1.0",
 ]
 files = [
-    {file = "mypy-1.8.0-cp310-cp310-macosx_10_9_x86_64.whl", hash = "sha256:485a8942f671120f76afffff70f259e1cd0f0cfe08f81c05d8816d958d4577d3"},
-    {file = "mypy-1.8.0-cp310-cp310-macosx_11_0_arm64.whl", hash = "sha256:df9824ac11deaf007443e7ed2a4a26bebff98d2bc43c6da21b2b64185da011c4"},
-    {file = "mypy-1.8.0-cp310-cp310-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:2afecd6354bbfb6e0160f4e4ad9ba6e4e003b767dd80d85516e71f2e955ab50d"},
-    {file = "mypy-1.8.0-cp310-cp310-musllinux_1_1_x86_64.whl", hash = "sha256:8963b83d53ee733a6e4196954502b33567ad07dfd74851f32be18eb932fb1cb9"},
-    {file = "mypy-1.8.0-cp310-cp310-win_amd64.whl", hash = "sha256:e46f44b54ebddbeedbd3d5b289a893219065ef805d95094d16a0af6630f5d410"},
-    {file = "mypy-1.8.0-cp311-cp311-macosx_10_9_x86_64.whl", hash = "sha256:855fe27b80375e5c5878492f0729540db47b186509c98dae341254c8f45f42ae"},
-    {file = "mypy-1.8.0-cp311-cp311-macosx_11_0_arm64.whl", hash = "sha256:4c886c6cce2d070bd7df4ec4a05a13ee20c0aa60cb587e8d1265b6c03cf91da3"},
-    {file = "mypy-1.8.0-cp311-cp311-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:d19c413b3c07cbecf1f991e2221746b0d2a9410b59cb3f4fb9557f0365a1a817"},
-    {file = "mypy-1.8.0-cp311-cp311-musllinux_1_1_x86_64.whl", hash = "sha256:9261ed810972061388918c83c3f5cd46079d875026ba97380f3e3978a72f503d"},
-    {file = "mypy-1.8.0-cp311-cp311-win_amd64.whl", hash = "sha256:51720c776d148bad2372ca21ca29256ed483aa9a4cdefefcef49006dff2a6835"},
-    {file = "mypy-1.8.0-cp312-cp312-macosx_10_9_x86_64.whl", hash = "sha256:52825b01f5c4c1c4eb0db253ec09c7aa17e1a7304d247c48b6f3599ef40db8bd"},
-    {file = "mypy-1.8.0-cp312-cp312-macosx_11_0_arm64.whl", hash = "sha256:f5ac9a4eeb1ec0f1ccdc6f326bcdb464de5f80eb07fb38b5ddd7b0de6bc61e55"},
-    {file = "mypy-1.8.0-cp312-cp312-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:afe3fe972c645b4632c563d3f3eff1cdca2fa058f730df2b93a35e3b0c538218"},
-    {file = "mypy-1.8.0-cp312-cp312-musllinux_1_1_x86_64.whl", hash = "sha256:42c6680d256ab35637ef88891c6bd02514ccb7e1122133ac96055ff458f93fc3"},
-    {file = "mypy-1.8.0-cp312-cp312-win_amd64.whl", hash = "sha256:720a5ca70e136b675af3af63db533c1c8c9181314d207568bbe79051f122669e"},
-    {file = "mypy-1.8.0-cp38-cp38-macosx_10_9_x86_64.whl", hash = "sha256:028cf9f2cae89e202d7b6593cd98db6759379f17a319b5faf4f9978d7084cdc6"},
-    {file = "mypy-1.8.0-cp38-cp38-macosx_11_0_arm64.whl", hash = "sha256:4e6d97288757e1ddba10dd9549ac27982e3e74a49d8d0179fc14d4365c7add66"},
-    {file = "mypy-1.8.0-cp38-cp38-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:7f1478736fcebb90f97e40aff11a5f253af890c845ee0c850fe80aa060a267c6"},
-    {file = "mypy-1.8.0-cp38-cp38-musllinux_1_1_x86_64.whl", hash = "sha256:42419861b43e6962a649068a61f4a4839205a3ef525b858377a960b9e2de6e0d"},
-    {file = "mypy-1.8.0-cp38-cp38-win_amd64.whl", hash = "sha256:2b5b6c721bd4aabaadead3a5e6fa85c11c6c795e0c81a7215776ef8afc66de02"},
-    {file = "mypy-1.8.0-cp39-cp39-macosx_10_9_x86_64.whl", hash = "sha256:5c1538c38584029352878a0466f03a8ee7547d7bd9f641f57a0f3017a7c905b8"},
-    {file = "mypy-1.8.0-cp39-cp39-macosx_11_0_arm64.whl", hash = "sha256:4ef4be7baf08a203170f29e89d79064463b7fc7a0908b9d0d5114e8009c3a259"},
-    {file = "mypy-1.8.0-cp39-cp39-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:7178def594014aa6c35a8ff411cf37d682f428b3b5617ca79029d8ae72f5402b"},
-    {file = "mypy-1.8.0-cp39-cp39-musllinux_1_1_x86_64.whl", hash = "sha256:ab3c84fa13c04aeeeabb2a7f67a25ef5d77ac9d6486ff33ded762ef353aa5592"},
-    {file = "mypy-1.8.0-cp39-cp39-win_amd64.whl", hash = "sha256:99b00bc72855812a60d253420d8a2eae839b0afa4938f09f4d2aa9bb4654263a"},
-    {file = "mypy-1.8.0-py3-none-any.whl", hash = "sha256:538fd81bb5e430cc1381a443971c0475582ff9f434c16cd46d2c66763ce85d9d"},
-    {file = "mypy-1.8.0.tar.gz", hash = "sha256:6ff8b244d7085a0b425b56d327b480c3b29cafbd2eff27316a004f9a7391ae07"},
+    {file = "mypy-1.10.0-cp310-cp310-macosx_10_9_x86_64.whl", hash = "sha256:da1cbf08fb3b851ab3b9523a884c232774008267b1f83371ace57f412fe308c2"},
+    {file = "mypy-1.10.0-cp310-cp310-macosx_11_0_arm64.whl", hash = "sha256:12b6bfc1b1a66095ab413160a6e520e1dc076a28f3e22f7fb25ba3b000b4ef99"},
+    {file = "mypy-1.10.0-cp310-cp310-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:9e36fb078cce9904c7989b9693e41cb9711e0600139ce3970c6ef814b6ebc2b2"},
+    {file = "mypy-1.10.0-cp310-cp310-musllinux_1_1_x86_64.whl", hash = "sha256:2b0695d605ddcd3eb2f736cd8b4e388288c21e7de85001e9f85df9187f2b50f9"},
+    {file = "mypy-1.10.0-cp310-cp310-win_amd64.whl", hash = "sha256:cd777b780312ddb135bceb9bc8722a73ec95e042f911cc279e2ec3c667076051"},
+    {file = "mypy-1.10.0-cp311-cp311-macosx_10_9_x86_64.whl", hash = "sha256:3be66771aa5c97602f382230165b856c231d1277c511c9a8dd058be4784472e1"},
+    {file = "mypy-1.10.0-cp311-cp311-macosx_11_0_arm64.whl", hash = "sha256:8b2cbaca148d0754a54d44121b5825ae71868c7592a53b7292eeb0f3fdae95ee"},
+    {file = "mypy-1.10.0-cp311-cp311-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:1ec404a7cbe9fc0e92cb0e67f55ce0c025014e26d33e54d9e506a0f2d07fe5de"},
+    {file = "mypy-1.10.0-cp311-cp311-musllinux_1_1_x86_64.whl", hash = "sha256:e22e1527dc3d4aa94311d246b59e47f6455b8729f4968765ac1eacf9a4760bc7"},
+    {file = "mypy-1.10.0-cp311-cp311-win_amd64.whl", hash = "sha256:a87dbfa85971e8d59c9cc1fcf534efe664d8949e4c0b6b44e8ca548e746a8d53"},
+    {file = "mypy-1.10.0-cp312-cp312-macosx_10_9_x86_64.whl", hash = "sha256:a781f6ad4bab20eef8b65174a57e5203f4be627b46291f4589879bf4e257b97b"},
+    {file = "mypy-1.10.0-cp312-cp312-macosx_11_0_arm64.whl", hash = "sha256:b808e12113505b97d9023b0b5e0c0705a90571c6feefc6f215c1df9381256e30"},
+    {file = "mypy-1.10.0-cp312-cp312-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:8f55583b12156c399dce2df7d16f8a5095291354f1e839c252ec6c0611e86e2e"},
+    {file = "mypy-1.10.0-cp312-cp312-musllinux_1_1_x86_64.whl", hash = "sha256:4cf18f9d0efa1b16478c4c129eabec36148032575391095f73cae2e722fcf9d5"},
+    {file = "mypy-1.10.0-cp312-cp312-win_amd64.whl", hash = "sha256:bc6ac273b23c6b82da3bb25f4136c4fd42665f17f2cd850771cb600bdd2ebeda"},
+    {file = "mypy-1.10.0-cp38-cp38-macosx_10_9_x86_64.whl", hash = "sha256:9fd50226364cd2737351c79807775136b0abe084433b55b2e29181a4c3c878c0"},
+    {file = "mypy-1.10.0-cp38-cp38-macosx_11_0_arm64.whl", hash = "sha256:f90cff89eea89273727d8783fef5d4a934be2fdca11b47def50cf5d311aff727"},
+    {file = "mypy-1.10.0-cp38-cp38-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:fcfc70599efde5c67862a07a1aaf50e55bce629ace26bb19dc17cece5dd31ca4"},
+    {file = "mypy-1.10.0-cp38-cp38-musllinux_1_1_x86_64.whl", hash = "sha256:075cbf81f3e134eadaf247de187bd604748171d6b79736fa9b6c9685b4083061"},
+    {file = "mypy-1.10.0-cp38-cp38-win_amd64.whl", hash = "sha256:3f298531bca95ff615b6e9f2fc0333aae27fa48052903a0ac90215021cdcfa4f"},
+    {file = "mypy-1.10.0-cp39-cp39-macosx_10_9_x86_64.whl", hash = "sha256:fa7ef5244615a2523b56c034becde4e9e3f9b034854c93639adb667ec9ec2976"},
+    {file = "mypy-1.10.0-cp39-cp39-macosx_11_0_arm64.whl", hash = "sha256:3236a4c8f535a0631f85f5fcdffba71c7feeef76a6002fcba7c1a8e57c8be1ec"},
+    {file = "mypy-1.10.0-cp39-cp39-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:4a2b5cdbb5dd35aa08ea9114436e0d79aceb2f38e32c21684dcf8e24e1e92821"},
+    {file = "mypy-1.10.0-cp39-cp39-musllinux_1_1_x86_64.whl", hash = "sha256:92f93b21c0fe73dc00abf91022234c79d793318b8a96faac147cd579c1671746"},
+    {file = "mypy-1.10.0-cp39-cp39-win_amd64.whl", hash = "sha256:28d0e038361b45f099cc086d9dd99c15ff14d0188f44ac883010e172ce86c38a"},
+    {file = "mypy-1.10.0-py3-none-any.whl", hash = "sha256:f8c083976eb530019175aabadb60921e73b4f45736760826aa1689dda8208aee"},
+    {file = "mypy-1.10.0.tar.gz", hash = "sha256:3d087fcbec056c4ee34974da493a826ce316947485cef3901f511848e687c131"},
 ]
 
 [[package]]
 name = "mypy-extensions"
 version = "1.0.0"
 requires_python = ">=3.5"
 summary = "Type system extensions for programs checked with the mypy type checker."
@@ -463,43 +463,32 @@
 files = [
     {file = "mypy_extensions-1.0.0-py3-none-any.whl", hash = "sha256:4392f6c0eb8a5668a69e23d168ffa70f0be9ccfd32b5cc2d26a34ae5b844552d"},
     {file = "mypy_extensions-1.0.0.tar.gz", hash = "sha256:75dbf8955dc00442a438fc4d0666508a9a97b6bd41aa2f0ffe9d2f2725af0782"},
 ]
 
 [[package]]
 name = "packaging"
-version = "23.2"
+version = "24.0"
 requires_python = ">=3.7"
 summary = "Core utilities for Python packages"
 groups = ["dev"]
 files = [
-    {file = "packaging-23.2-py3-none-any.whl", hash = "sha256:8c491190033a9af7e1d931d0b5dacc2ef47509b34dd0de67ed209b5203fc88c7"},
-    {file = "packaging-23.2.tar.gz", hash = "sha256:048fb0e9405036518eaaf48a55953c750c11e1a1b68e0dd1a9d62ed0c092cfc5"},
+    {file = "packaging-24.0-py3-none-any.whl", hash = "sha256:2ddfb553fdf02fb784c234c7ba6ccc288296ceabec964ad2eae3777778130bc5"},
+    {file = "packaging-24.0.tar.gz", hash = "sha256:eb82c5e3e56209074766e6885bb04b8c38a0c015d0a30036ebe7ece34c9989e9"},
 ]
 
 [[package]]
 name = "pluggy"
-version = "1.4.0"
+version = "1.5.0"
 requires_python = ">=3.8"
 summary = "plugin and hook calling mechanisms for python"
 groups = ["dev"]
 files = [
-    {file = "pluggy-1.4.0-py3-none-any.whl", hash = "sha256:7db9f7b503d67d1c5b95f59773ebb58a8c1c288129a88665838012cfb07b8981"},
-    {file = "pluggy-1.4.0.tar.gz", hash = "sha256:8c85c2876142a764e5b7548e7d9a0e0ddb46f5185161049a79b7e974454223be"},
-]
-
-[[package]]
-name = "pycowsay"
-version = "0.0.0.2"
-requires_python = ">=3.6"
-summary = ""
-groups = ["default"]
-files = [
-    {file = "pycowsay-0.0.0.2-py3-none-any.whl", hash = "sha256:5c03d8a9c7666ec102aaed4bbd6c7d35228489ce236f95f6e5d079529c6a5050"},
-    {file = "pycowsay-0.0.0.2.tar.gz", hash = "sha256:d112c4ce55b04dbc363c5a8957b80a0dc7459e864866d6e0202d15a95633bcf4"},
+    {file = "pluggy-1.5.0-py3-none-any.whl", hash = "sha256:44e1ad92c8ca002de6377e165f3e0f1be63266ab4d554740532335b9d75ea669"},
+    {file = "pluggy-1.5.0.tar.gz", hash = "sha256:2cffa88e94fdc978c4c574f15f9e59b7f4201d439195c3715ca9e2486f1d0cf1"},
 ]
 
 [[package]]
 name = "pygments"
 version = "2.17.2"
 requires_python = ">=3.7"
 summary = "Pygments is a syntax highlighting package written in Python."
@@ -507,44 +496,44 @@
 files = [
     {file = "pygments-2.17.2-py3-none-any.whl", hash = "sha256:b27c2826c47d0f3219f29554824c30c5e8945175d888647acd804ddd04af846c"},
     {file = "pygments-2.17.2.tar.gz", hash = "sha256:da46cec9fd2de5be3a8a784f434e4c4ab670b4ff54d605c4c2717e9d49c4c367"},
 ]
 
 [[package]]
 name = "pytest"
-version = "8.0.2"
+version = "8.2.0"
 requires_python = ">=3.8"
 summary = "pytest: simple powerful testing with Python"
 groups = ["dev"]
 dependencies = [
     "colorama; sys_platform == \"win32\"",
     "exceptiongroup>=1.0.0rc8; python_version < \"3.11\"",
     "iniconfig",
     "packaging",
-    "pluggy<2.0,>=1.3.0",
-    "tomli>=1.0.0; python_version < \"3.11\"",
+    "pluggy<2.0,>=1.5",
+    "tomli>=1; python_version < \"3.11\"",
 ]
 files = [
-    {file = "pytest-8.0.2-py3-none-any.whl", hash = "sha256:edfaaef32ce5172d5466b5127b42e0d6d35ebbe4453f0e3505d96afd93f6b096"},
-    {file = "pytest-8.0.2.tar.gz", hash = "sha256:d4051d623a2e0b7e51960ba963193b09ce6daeb9759a451844a21e4ddedfc1bd"},
+    {file = "pytest-8.2.0-py3-none-any.whl", hash = "sha256:1733f0620f6cda4095bbf0d9ff8022486e91892245bb9e7d5542c018f612f233"},
+    {file = "pytest-8.2.0.tar.gz", hash = "sha256:d507d4482197eac0ba2bae2e9babf0672eb333017bcedaa5fb1a3d42c1174b3f"},
 ]
 
 [[package]]
 name = "pytest-cov"
-version = "4.1.0"
-requires_python = ">=3.7"
+version = "5.0.0"
+requires_python = ">=3.8"
 summary = "Pytest plugin for measuring coverage."
 groups = ["dev"]
 dependencies = [
     "coverage[toml]>=5.2.1",
     "pytest>=4.6",
 ]
 files = [
-    {file = "pytest-cov-4.1.0.tar.gz", hash = "sha256:3904b13dfbfec47f003b8e77fd5b589cd11904a21ddf1ab38a64f204d6a10ef6"},
-    {file = "pytest_cov-4.1.0-py3-none-any.whl", hash = "sha256:6ba70b9e97e69fcc3fb45bfeab2d0a138fb65c4d0d6a41ef33983ad114be8c3a"},
+    {file = "pytest-cov-5.0.0.tar.gz", hash = "sha256:5837b58e9f6ebd335b0f8060eecce69b662415b16dc503883a02f45dfeb14857"},
+    {file = "pytest_cov-5.0.0-py3-none-any.whl", hash = "sha256:4f0764a1219df53214206bf1feea4633c3b558a2925c8b59f144f682861ce652"},
 ]
 
 [[package]]
 name = "pytz"
 version = "2024.1"
 summary = "World timezone definitions, modern and historical"
 groups = ["dev"]
@@ -569,36 +558,36 @@
 files = [
     {file = "requests-2.31.0-py3-none-any.whl", hash = "sha256:58cd2187c01e70e6e26505bca751777aa9f2ee0b7f4300988b709f44e013003f"},
     {file = "requests-2.31.0.tar.gz", hash = "sha256:942c5a758f98d790eaed1a29cb6eefc7ffb0d1cf7af05c3d2791656dbd6ad1e1"},
 ]
 
 [[package]]
 name = "ruff"
-version = "0.3.0"
+version = "0.4.3"
 requires_python = ">=3.7"
 summary = "An extremely fast Python linter and code formatter, written in Rust."
 groups = ["dev"]
 files = [
-    {file = "ruff-0.3.0-py3-none-macosx_10_12_x86_64.macosx_11_0_arm64.macosx_10_12_universal2.whl", hash = "sha256:7deb528029bacf845bdbb3dbb2927d8ef9b4356a5e731b10eef171e3f0a85944"},
-    {file = "ruff-0.3.0-py3-none-macosx_10_12_x86_64.whl", hash = "sha256:e1e0d4381ca88fb2b73ea0766008e703f33f460295de658f5467f6f229658c19"},
-    {file = "ruff-0.3.0-py3-none-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:2f7dbba46e2827dfcb0f0cc55fba8e96ba7c8700e0a866eb8cef7d1d66c25dcb"},
-    {file = "ruff-0.3.0-py3-none-manylinux_2_17_armv7l.manylinux2014_armv7l.whl", hash = "sha256:23dbb808e2f1d68eeadd5f655485e235c102ac6f12ad31505804edced2a5ae77"},
-    {file = "ruff-0.3.0-py3-none-manylinux_2_17_i686.manylinux2014_i686.whl", hash = "sha256:3ef655c51f41d5fa879f98e40c90072b567c666a7114fa2d9fe004dffba00932"},
-    {file = "ruff-0.3.0-py3-none-manylinux_2_17_ppc64.manylinux2014_ppc64.whl", hash = "sha256:d0d3d7ef3d4f06433d592e5f7d813314a34601e6c5be8481cccb7fa760aa243e"},
-    {file = "ruff-0.3.0-py3-none-manylinux_2_17_ppc64le.manylinux2014_ppc64le.whl", hash = "sha256:b08b356d06a792e49a12074b62222f9d4ea2a11dca9da9f68163b28c71bf1dd4"},
-    {file = "ruff-0.3.0-py3-none-manylinux_2_17_s390x.manylinux2014_s390x.whl", hash = "sha256:9343690f95710f8cf251bee1013bf43030072b9f8d012fbed6ad702ef70d360a"},
-    {file = "ruff-0.3.0-py3-none-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:a1f3ed501a42f60f4dedb7805fa8d4534e78b4e196f536bac926f805f0743d49"},
-    {file = "ruff-0.3.0-py3-none-musllinux_1_2_aarch64.whl", hash = "sha256:cc30a9053ff2f1ffb505a585797c23434d5f6c838bacfe206c0e6cf38c921a1e"},
-    {file = "ruff-0.3.0-py3-none-musllinux_1_2_armv7l.whl", hash = "sha256:5da894a29ec018a8293d3d17c797e73b374773943e8369cfc50495573d396933"},
-    {file = "ruff-0.3.0-py3-none-musllinux_1_2_i686.whl", hash = "sha256:755c22536d7f1889be25f2baf6fedd019d0c51d079e8417d4441159f3bcd30c2"},
-    {file = "ruff-0.3.0-py3-none-musllinux_1_2_x86_64.whl", hash = "sha256:dd73fe7f4c28d317855da6a7bc4aa29a1500320818dd8f27df95f70a01b8171f"},
-    {file = "ruff-0.3.0-py3-none-win32.whl", hash = "sha256:19eacceb4c9406f6c41af806418a26fdb23120dfe53583df76d1401c92b7c14b"},
-    {file = "ruff-0.3.0-py3-none-win_amd64.whl", hash = "sha256:128265876c1d703e5f5e5a4543bd8be47c73a9ba223fd3989d4aa87dd06f312f"},
-    {file = "ruff-0.3.0-py3-none-win_arm64.whl", hash = "sha256:e3a4a6d46aef0a84b74fcd201a4401ea9a6cd85614f6a9435f2d33dd8cefbf83"},
-    {file = "ruff-0.3.0.tar.gz", hash = "sha256:0886184ba2618d815067cf43e005388967b67ab9c80df52b32ec1152ab49f53a"},
+    {file = "ruff-0.4.3-py3-none-macosx_10_12_x86_64.whl", hash = "sha256:b70800c290f14ae6fcbb41bbe201cf62dfca024d124a1f373e76371a007454ce"},
+    {file = "ruff-0.4.3-py3-none-macosx_11_0_arm64.whl", hash = "sha256:08a0d6a22918ab2552ace96adeaca308833873a4d7d1d587bb1d37bae8728eb3"},
+    {file = "ruff-0.4.3-py3-none-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:eba1f14df3c758dd7de5b55fbae7e1c8af238597961e5fb628f3de446c3c40c5"},
+    {file = "ruff-0.4.3-py3-none-manylinux_2_17_armv7l.manylinux2014_armv7l.whl", hash = "sha256:819fb06d535cc76dfddbfe8d3068ff602ddeb40e3eacbc90e0d1272bb8d97113"},
+    {file = "ruff-0.4.3-py3-none-manylinux_2_17_i686.manylinux2014_i686.whl", hash = "sha256:0bfc9e955e6dc6359eb6f82ea150c4f4e82b660e5b58d9a20a0e42ec3bb6342b"},
+    {file = "ruff-0.4.3-py3-none-manylinux_2_17_ppc64.manylinux2014_ppc64.whl", hash = "sha256:510a67d232d2ebe983fddea324dbf9d69b71c4d2dfeb8a862f4a127536dd4cfb"},
+    {file = "ruff-0.4.3-py3-none-manylinux_2_17_ppc64le.manylinux2014_ppc64le.whl", hash = "sha256:dc9ff11cd9a092ee7680a56d21f302bdda14327772cd870d806610a3503d001f"},
+    {file = "ruff-0.4.3-py3-none-manylinux_2_17_s390x.manylinux2014_s390x.whl", hash = "sha256:29efff25bf9ee685c2c8390563a5b5c006a3fee5230d28ea39f4f75f9d0b6f2f"},
+    {file = "ruff-0.4.3-py3-none-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:18b00e0bcccf0fc8d7186ed21e311dffd19761cb632241a6e4fe4477cc80ef6e"},
+    {file = "ruff-0.4.3-py3-none-musllinux_1_2_aarch64.whl", hash = "sha256:262f5635e2c74d80b7507fbc2fac28fe0d4fef26373bbc62039526f7722bca1b"},
+    {file = "ruff-0.4.3-py3-none-musllinux_1_2_armv7l.whl", hash = "sha256:7363691198719c26459e08cc17c6a3dac6f592e9ea3d2fa772f4e561b5fe82a3"},
+    {file = "ruff-0.4.3-py3-none-musllinux_1_2_i686.whl", hash = "sha256:eeb039f8428fcb6725bb63cbae92ad67b0559e68b5d80f840f11914afd8ddf7f"},
+    {file = "ruff-0.4.3-py3-none-musllinux_1_2_x86_64.whl", hash = "sha256:927b11c1e4d0727ce1a729eace61cee88a334623ec424c0b1c8fe3e5f9d3c865"},
+    {file = "ruff-0.4.3-py3-none-win32.whl", hash = "sha256:25cacda2155778beb0d064e0ec5a3944dcca9c12715f7c4634fd9d93ac33fd30"},
+    {file = "ruff-0.4.3-py3-none-win_amd64.whl", hash = "sha256:7a1c3a450bc6539ef00da6c819fb1b76b6b065dec585f91456e7c0d6a0bbc725"},
+    {file = "ruff-0.4.3-py3-none-win_arm64.whl", hash = "sha256:71ca5f8ccf1121b95a59649482470c5601c60a416bf189d553955b0338e34614"},
+    {file = "ruff-0.4.3.tar.gz", hash = "sha256:ff0a3ef2e3c4b6d133fbedcf9586abfbe38d076041f2dc18ffb2c7e0485d5a07"},
 ]
 
 [[package]]
 name = "snowballstemmer"
 version = "2.2.0"
 summary = "This package provides 29 stemmers for 28 languages generated from Snowball algorithms."
 groups = ["dev"]
@@ -743,35 +732,35 @@
 files = [
     {file = "tomli-2.0.1-py3-none-any.whl", hash = "sha256:939de3e7a6161af0c887ef91b7d41a53e7c5a1ca976325f429cb46ea9bc30ecc"},
     {file = "tomli-2.0.1.tar.gz", hash = "sha256:de526c12914f0c550d15924c62d72abc48d6fe7364aa87328337a31007fe8a4f"},
 ]
 
 [[package]]
 name = "types-requests"
-version = "2.31.0.20240218"
+version = "2.31.0.20240406"
 requires_python = ">=3.8"
 summary = "Typing stubs for requests"
 groups = ["dev"]
 dependencies = [
     "urllib3>=2",
 ]
 files = [
-    {file = "types-requests-2.31.0.20240218.tar.gz", hash = "sha256:f1721dba8385958f504a5386240b92de4734e047a08a40751c1654d1ac3349c5"},
-    {file = "types_requests-2.31.0.20240218-py3-none-any.whl", hash = "sha256:a82807ec6ddce8f00fe0e949da6d6bc1fbf1715420218a9640d695f70a9e5a9b"},
+    {file = "types-requests-2.31.0.20240406.tar.gz", hash = "sha256:4428df33c5503945c74b3f42e82b181e86ec7b724620419a2966e2de604ce1a1"},
+    {file = "types_requests-2.31.0.20240406-py3-none-any.whl", hash = "sha256:6216cdac377c6b9a040ac1c0404f7284bd13199c0e1bb235f4324627e8898cf5"},
 ]
 
 [[package]]
 name = "typing-extensions"
-version = "4.10.0"
+version = "4.11.0"
 requires_python = ">=3.8"
 summary = "Backported and Experimental Type Hints for Python 3.8+"
 groups = ["dev"]
 files = [
-    {file = "typing_extensions-4.10.0-py3-none-any.whl", hash = "sha256:69b1a937c3a517342112fb4c6df7e72fc39a38e7891a5730ed4985b5214b5475"},
-    {file = "typing_extensions-4.10.0.tar.gz", hash = "sha256:b0abd7c89e8fb96f98db18d86106ff1d90ab692004eb746cf6eda2682f91b3cb"},
+    {file = "typing_extensions-4.11.0-py3-none-any.whl", hash = "sha256:c1f94d72897edaf4ce775bb7558d5b79d8126906a14ea5ed1635921406c0387a"},
+    {file = "typing_extensions-4.11.0.tar.gz", hash = "sha256:83f085bd5ca59c80295fc2a82ab5dac679cbe02b9f33f7d83af68e241bea51b0"},
 ]
 
 [[package]]
 name = "urllib3"
 version = "2.2.1"
 requires_python = ">=3.8"
 summary = "HTTP library with thread-safe connection pooling, file post, and more."
@@ -779,16 +768,16 @@
 files = [
     {file = "urllib3-2.2.1-py3-none-any.whl", hash = "sha256:450b20ec296a467077128bff42b73080516e71b56ff59a60a02bef2232c4fa9d"},
     {file = "urllib3-2.2.1.tar.gz", hash = "sha256:d0570876c61ab9e520d776c38acbbb5b05a776d3f9ff98a5c8fd5162a444cf19"},
 ]
 
 [[package]]
 name = "zipp"
-version = "3.17.0"
+version = "3.18.1"
 requires_python = ">=3.8"
 summary = "Backport of pathlib-compatible object wrapper for zip files"
 groups = ["dev"]
 marker = "python_version < \"3.10\""
 files = [
-    {file = "zipp-3.17.0-py3-none-any.whl", hash = "sha256:0e923e726174922dce09c53c59ad483ff7bbb8e572e00c7f7c46b88556409f31"},
-    {file = "zipp-3.17.0.tar.gz", hash = "sha256:84e64a1c28cf7e91ed2078bb8cc8c259cb19b76942096c8d7b84947690cabaf0"},
+    {file = "zipp-3.18.1-py3-none-any.whl", hash = "sha256:206f5a15f2af3dbaee80769fb7dc6f249695e940acca08dfb2a4769fe61e538b"},
+    {file = "zipp-3.18.1.tar.gz", hash = "sha256:2884ed22e7d8961de1c9a05142eb69a247f120291bc0206a00a7642f09b5b715"},
 ]
```

### Comparing `ytmusicapi-1.6.0/pyproject.toml` & `ytmusicapi-1.7.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `ytmusicapi-1.6.0/tests/README.rst` & `ytmusicapi-1.7.0/tests/README.rst`

 * *Files identical despite different names*

### Comparing `ytmusicapi-1.6.0/tests/auth/test_browser.py` & `ytmusicapi-1.7.0/tests/auth/test_browser.py`

 * *Files identical despite different names*

### Comparing `ytmusicapi-1.6.0/tests/auth/test_oauth.py` & `ytmusicapi-1.7.0/tests/auth/test_oauth.py`

 * *Files identical despite different names*

### Comparing `ytmusicapi-1.6.0/tests/conftest.py` & `ytmusicapi-1.7.0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `ytmusicapi-1.6.0/tests/mixins/test_browsing.py` & `ytmusicapi-1.7.0/tests/mixins/test_browsing.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,8 +1,11 @@
+import json
 import warnings
+from pathlib import Path
+from unittest import mock
 
 import pytest
 
 
 class TestBrowsing:
     def test_get_home(self, yt, yt_auth):
         result = yt.get_home()
@@ -19,14 +22,22 @@
         assert len(
             [x for x in related if set(x.keys()) == {"browseId", "subscribers", "title", "thumbnails"}]
         ) == len(related)
 
         results = yt.get_artist("UCLZ7tlKC06ResyDmEStSrOw")  # no album year
         assert len(results) >= 11
 
+    def test_get_artist_shows(self, yt_oauth):
+        # with audiobooks - only with authentication
+        results = yt_oauth.get_artist("UCyiY-0Af0O6emoI3YvCEDaA")
+        assert len(results["shows"]["results"]) == 10
+
+        results = yt_oauth.get_artist_albums(results["shows"]["browseId"], results["shows"]["params"])
+        assert len(results) == 100
+
     def test_get_artist_albums(self, yt):
         artist = yt.get_artist("UCAeLFBCQS7FvI8PvBrWvSBg")
         results = yt.get_artist_albums(artist["albums"]["browseId"], artist["albums"]["params"])
         assert len(results) == 100
         results = yt.get_artist_albums(artist["singles"]["browseId"], artist["singles"]["params"])
         assert len(results) == 100
 
@@ -62,14 +73,23 @@
         browse_id = yt.get_album_browse_id("OLAK5uy_nMr9h2VlS-2PULNz3M3XVXQj_P3C2bqaY")
         assert browse_id == sample_album
 
     def test_get_album_browse_id_issue_470(self, yt):
         escaped_browse_id = yt.get_album_browse_id("OLAK5uy_nbMYyrfeg5ZgknoOsOGBL268hGxtcbnDM")
         assert escaped_browse_id == "MPREb_scJdtUCpPE2"
 
+    def test_get_album_2024(self, yt):
+        with open(Path(__file__).parent.parent / "data" / "2024_03_get_album.json", encoding="utf8") as f:
+            mock_response = json.load(f)
+        with mock.patch("ytmusicapi.YTMusic._send_request", return_value=mock_response):
+            album = yt.get_album("MPREabc")
+            assert len(album["tracks"]) == 19
+            assert len(album["artists"]) == 1
+            assert len(album) == 13
+
     def test_get_album(self, yt, yt_auth, sample_album):
         album = yt_auth.get_album(sample_album)
         assert len(album) >= 9
         assert "isExplicit" in album
         assert album["tracks"][0]["isExplicit"]
         assert all(item["views"] is not None for item in album["tracks"])
         assert all(item["album"] is not None for item in album["tracks"])
```

### Comparing `ytmusicapi-1.6.0/tests/mixins/test_explore.py` & `ytmusicapi-1.7.0/tests/mixins/test_explore.py`

 * *Files identical despite different names*

### Comparing `ytmusicapi-1.6.0/tests/mixins/test_library.py` & `ytmusicapi-1.7.0/tests/mixins/test_library.py`

 * *Files identical despite different names*

### Comparing `ytmusicapi-1.6.0/tests/mixins/test_playlists.py` & `ytmusicapi-1.7.0/tests/mixins/test_playlists.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,13 +1,34 @@
+import json
 import time
+from pathlib import Path
+from unittest import mock
 
 import pytest
 
 
 class TestPlaylists:
+    @pytest.mark.parametrize(
+        ("test_file", "owned"),
+        [
+            ("2024_03_get_playlist.json", True),
+            ("2024_03_get_playlist_public.json", False),
+        ],
+    )
+    def test_get_playlist_2024(self, yt, test_file, owned):
+        with open(Path(__file__).parent.parent / "data" / test_file, encoding="utf8") as f:
+            mock_response = json.load(f)
+        with mock.patch("ytmusicapi.YTMusic._send_request", return_value=mock_response):
+            playlist = yt.get_playlist("MPREabc")
+            assert playlist["year"] == "2024"
+            assert playlist["owned"] == owned
+            assert "hours" in playlist["duration"]
+            assert playlist["id"]
+            assert isinstance(playlist["description"], str)
+
     def test_get_playlist_foreign(self, yt, yt_auth, yt_oauth):
         with pytest.raises(Exception):
             yt.get_playlist("PLABC")
         playlist = yt_auth.get_playlist("PLk5BdzXBUiUe8Q5I13ZSCD8HbxMqJUUQA", limit=300, suggestions_limit=7)
         assert len(playlist["duration"]) > 5
         assert len(playlist["tracks"]) > 200
         assert "suggestions" not in playlist
@@ -16,14 +37,30 @@
         yt.get_playlist("RDATgXd-")
         assert len(playlist["tracks"]) >= 100
 
         playlist = yt_oauth.get_playlist("PLj4BSJLnVpNyIjbCWXWNAmybc97FXLlTk", limit=None, related=True)
         assert len(playlist["tracks"]) > 200
         assert len(playlist["related"]) == 0
 
+    def test_get_playlist_foreign_new_format(self, yt_empty):
+        with pytest.raises(Exception):
+            yt_empty.get_playlist("PLABC")
+        playlist = yt_empty.get_playlist("PLk5BdzXBUiUe8Q5I13ZSCD8HbxMqJUUQA", limit=300, suggestions_limit=7)
+        assert len(playlist["duration"]) > 5
+        assert len(playlist["tracks"]) > 200
+        assert "suggestions" not in playlist
+        assert playlist["owned"] is False
+
+        playlist = yt_empty.get_playlist("RDATgXd-")
+        assert len(playlist["tracks"]) >= 100
+
+        playlist = yt_empty.get_playlist("PLj4BSJLnVpNyIjbCWXWNAmybc97FXLlTk", limit=None, related=True)
+        assert len(playlist["tracks"]) > 200
+        assert len(playlist["related"]) == 0
+
     def test_get_playlist_owned(self, config, yt_brand):
         playlist = yt_brand.get_playlist(config["playlists"]["own"], related=True, suggestions_limit=21)
         assert len(playlist["tracks"]) < 100
         assert len(playlist["suggestions"]) == 21
         assert len(playlist["related"]) == 10
         assert playlist["owned"] is True
 
@@ -48,15 +85,15 @@
             moveItem=(
                 playlist["tracks"][0]["setVideoId"],
                 playlist["tracks"][1]["setVideoId"],
             ),
         )
         assert response == "STATUS_SUCCEEDED", "Playlist edit failed"
 
-    def test_end2end(self, config, yt_brand, sample_video):
+    def test_end2end(self, yt_brand, sample_video):
         playlist_id = yt_brand.create_playlist(
             "test",
             "test description",
             source_playlist="OLAK5uy_lGQfnMNGvYCRdDq9ZLzJV2BJL2aHQsz9Y",
         )
         assert len(playlist_id) == 34, "Playlist creation failed"
         yt_brand.edit_playlist(playlist_id, addToTop=True)
```

### Comparing `ytmusicapi-1.6.0/tests/mixins/test_podcasts.py` & `ytmusicapi-1.7.0/tests/mixins/test_podcasts.py`

 * *Files identical despite different names*

### Comparing `ytmusicapi-1.6.0/tests/mixins/test_search.py` & `ytmusicapi-1.7.0/tests/mixins/test_search.py`

 * *Files identical despite different names*

### Comparing `ytmusicapi-1.6.0/tests/mixins/test_uploads.py` & `ytmusicapi-1.7.0/tests/mixins/test_uploads.py`

 * *Files identical despite different names*

### Comparing `ytmusicapi-1.6.0/tests/mixins/test_watch.py` & `ytmusicapi-1.7.0/tests/mixins/test_watch.py`

 * *Files identical despite different names*

### Comparing `ytmusicapi-1.6.0/tests/setup/setup_account.py` & `ytmusicapi-1.7.0/tests/setup/setup_account.py`

 * *Files identical despite different names*

### Comparing `ytmusicapi-1.6.0/tests/test.example.cfg` & `ytmusicapi-1.7.0/tests/test.example.cfg`

 * *Files identical despite different names*

### Comparing `ytmusicapi-1.6.0/ytmusicapi/auth/browser.py` & `ytmusicapi-1.7.0/ytmusicapi/auth/browser.py`

 * *Files identical despite different names*

### Comparing `ytmusicapi-1.6.0/ytmusicapi/auth/oauth/credentials.py` & `ytmusicapi-1.7.0/ytmusicapi/auth/oauth/credentials.py`

 * *Files identical despite different names*

### Comparing `ytmusicapi-1.6.0/ytmusicapi/auth/oauth/models.py` & `ytmusicapi-1.7.0/ytmusicapi/auth/oauth/models.py`

 * *Files identical despite different names*

### Comparing `ytmusicapi-1.6.0/ytmusicapi/auth/oauth/token.py` & `ytmusicapi-1.7.0/ytmusicapi/auth/oauth/token.py`

 * *Files identical despite different names*

### Comparing `ytmusicapi-1.6.0/ytmusicapi/auth/types.py` & `ytmusicapi-1.7.0/ytmusicapi/auth/types.py`

 * *Files identical despite different names*

### Comparing `ytmusicapi-1.6.0/ytmusicapi/constants.py` & `ytmusicapi-1.7.0/ytmusicapi/constants.py`

 * *Files identical despite different names*

### Comparing `ytmusicapi-1.6.0/ytmusicapi/continuations.py` & `ytmusicapi-1.7.0/ytmusicapi/continuations.py`

 * *Files identical despite different names*

### Comparing `ytmusicapi-1.6.0/ytmusicapi/helpers.py` & `ytmusicapi-1.7.0/ytmusicapi/helpers.py`

 * *Files identical despite different names*

### Comparing `ytmusicapi-1.6.0/ytmusicapi/locales/README.rst` & `ytmusicapi-1.7.0/ytmusicapi/locales/README.rst`

 * *Files 17% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Translations
 ============================================
 Translations are required for ytmusicapi since it relies on parsing user interface text.
 In some places, for example the search() or get_artist() features, there is no other way to tell which content type is
 offered other than parsing display text, which depends on the user's language. Changing the API language is desirable,
 since artist and song titles are also language dependent.
 
-This package uses the Linux command line utility xgettext, which you can install for example using your package manager.
+This package uses the Linux command line utility xgettext (install via package manager).
 
 Add new translatable texts from code
 ----------------------------------------
 
 ``xgettext -d base -o locales/base.pot *.py mixins/*.py parsers/*.py  --from-code "utf-8"``
 
 ``sed --in-place locales/base.pot --expression=s/CHARSET/UTF-8/``
@@ -23,18 +23,18 @@
 Copy the base template:
 
 ``cp locales/base.pot locales/LANG/LC_MESSAGES/base.po``
 
 Update translation
 ------------------
 
-``cd locales && sh update_po.sh``
+``cd locales && ./update_po.sh``
 
 Edit translation
 ----------------
 You can use POEdit or edit the .po file manually
 
 Finalize translation
 ---------------------
 To generate mo files, run
 
-``cd locales && sh update_mo.sh``
+``cd locales && ./update_mo.sh``
```

### Comparing `ytmusicapi-1.6.0/ytmusicapi/locales/ar/LC_MESSAGES/base.mo` & `ytmusicapi-1.7.0/ytmusicapi/locales/ar/LC_MESSAGES/base.mo`

 * *Files 18% similar despite different names*

#### msgunfmt {}

```diff
@@ -37,14 +37,17 @@
 
 msgid "profile"
 msgstr "الملف الشخصي"
 
 msgid "related"
 msgstr "ذات صلة"
 
+msgid "shows"
+msgstr "الكتب المسموعة والعروض"
+
 msgid "singles"
 msgstr "الفردي"
 
 msgid "song"
 msgstr "أغنية"
 
 msgid "station"
```

### Comparing `ytmusicapi-1.6.0/ytmusicapi/locales/ar/LC_MESSAGES/base.po` & `ytmusicapi-1.7.0/ytmusicapi/locales/pt/LC_MESSAGES/base.po`

 * *Files 10% similar despite different names*

```diff
@@ -1,78 +1,82 @@
 # Translations for ytmusicapi
 # Copyright (C) 2023 sigma67
 # This file is distributed under the same license as ytmusicapi
 # sigma67 <ytmusicapi@gmail.com>
-#
+# 
 msgid ""
 msgstr ""
 "Project-Id-Version: \n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2024-03-05 20:13+0100\n"
-"PO-Revision-Date: 2023-01-02 22:14+0530\n"
+"POT-Creation-Date: 2024-03-13 20:07+0100\n"
+"PO-Revision-Date: 2023-01-01 12:15+0530\n"
 "Last-Translator: \n"
 "Language-Team: \n"
-"Language: ar\n"
+"Language: pt\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "X-Generator: Poedit 3.2.2\n"
 
-#: parsers/i18n.py:22
+#: parsers/i18n.py:32
 msgid "artist"
-msgstr "فنان"
+msgstr "artista"
 
-#: parsers/i18n.py:23
+#: parsers/i18n.py:33
 msgid "playlist"
-msgstr "قائمةالتشغيل"
+msgstr "lista de reprodução"
 
-#: parsers/i18n.py:24
+#: parsers/i18n.py:34
 msgid "song"
-msgstr "أغنية"
+msgstr "música"
 
-#: parsers/i18n.py:25
+#: parsers/i18n.py:35
 msgid "video"
-msgstr "فيديو"
+msgstr "vídeo"
 
-#: parsers/i18n.py:26
+#: parsers/i18n.py:36
 msgid "station"
-msgstr "محطة"
+msgstr "estação"
 
-#: parsers/i18n.py:27
+#: parsers/i18n.py:37
 msgid "profile"
-msgstr "الملف الشخصي"
+msgstr "perfil"
 
-#: parsers/i18n.py:28
+#: parsers/i18n.py:38
 msgid "podcast"
-msgstr "بودكاست"
+msgstr ""
 
-#: parsers/i18n.py:29
+#: parsers/i18n.py:39
 msgid "episode"
-msgstr "حلقة"
+msgstr "Episódio"
 
-#: parsers/i18n.py:35
+#: parsers/i18n.py:46
 msgid "albums"
-msgstr "ألبومات"
+msgstr "álbuns"
 
-#: parsers/i18n.py:35
+#: parsers/i18n.py:47
 msgid "singles"
-msgstr "الفردي"
+msgstr "solteiros"
 
-#: parsers/i18n.py:35
+#: parsers/i18n.py:48
+msgid "shows"
+msgstr "Audiolivros e programas"
+
+#: parsers/i18n.py:49
 msgid "videos"
-msgstr "أشرطة فيديو"
+msgstr "vídeos"
 
-#: parsers/i18n.py:35
+#: parsers/i18n.py:50
 msgid "playlists"
-msgstr "قوائم التشغيل"
+msgstr "listas de reprodução"
 
-#: parsers/i18n.py:35
+#: parsers/i18n.py:51
 msgid "related"
-msgstr "ذات صلة"
+msgstr "relacionado"
 
-#: parsers/i18n.py:35
+#: parsers/i18n.py:52
 msgid "episodes"
-msgstr "أحدث الحلقات"
+msgstr "episódios novos"
 
-#: parsers/i18n.py:35
+#: parsers/i18n.py:53
 msgid "podcasts"
-msgstr "بودكاست"
+msgstr "podcasts"
```

### Comparing `ytmusicapi-1.6.0/ytmusicapi/locales/base.pot` & `ytmusicapi-1.7.0/ytmusicapi/locales/en/LC_MESSAGES/base.po`

 * *Files 7% similar despite different names*

```diff
@@ -1,78 +1,82 @@
-# SOME DESCRIPTIVE TITLE.
-# Copyright (C) YEAR THE PACKAGE'S COPYRIGHT HOLDER
-# This file is distributed under the same license as the PACKAGE package.
-# FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
-#
+# Translations for ytmusicapi
+# Copyright (C) 2023 sigma67
+# This file is distributed under the same license as ytmusicapi
+# sigma67 <ytmusicapi@gmail.com>
+# 
 #, fuzzy
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2024-03-05 20:13+0100\n"
+"POT-Creation-Date: 2024-03-13 20:07+0100\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language-Team: LANGUAGE <LL@li.org>\n"
 "Language: \n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 
-#: parsers/i18n.py:22
+#: parsers/i18n.py:32
 msgid "artist"
 msgstr ""
 
-#: parsers/i18n.py:23
+#: parsers/i18n.py:33
 msgid "playlist"
 msgstr ""
 
-#: parsers/i18n.py:24
+#: parsers/i18n.py:34
 msgid "song"
 msgstr ""
 
-#: parsers/i18n.py:25
+#: parsers/i18n.py:35
 msgid "video"
 msgstr ""
 
-#: parsers/i18n.py:26
+#: parsers/i18n.py:36
 msgid "station"
 msgstr ""
 
-#: parsers/i18n.py:27
+#: parsers/i18n.py:37
 msgid "profile"
 msgstr ""
 
-#: parsers/i18n.py:28
+#: parsers/i18n.py:38
 msgid "podcast"
 msgstr ""
 
-#: parsers/i18n.py:29
+#: parsers/i18n.py:39
 msgid "episode"
 msgstr ""
 
-#: parsers/i18n.py:35
+#: parsers/i18n.py:46
 msgid "albums"
 msgstr ""
 
-#: parsers/i18n.py:35
+#: parsers/i18n.py:47
 msgid "singles"
 msgstr ""
 
-#: parsers/i18n.py:35
+#: parsers/i18n.py:48
+msgid "shows"
+msgstr "Audiobooks and shows"
+
+#: parsers/i18n.py:49
 msgid "videos"
 msgstr ""
 
-#: parsers/i18n.py:35
+#: parsers/i18n.py:50
 msgid "playlists"
 msgstr ""
 
-#: parsers/i18n.py:35
+#: parsers/i18n.py:51
 msgid "related"
-msgstr ""
+msgstr "fans might also like"
 
-#: parsers/i18n.py:35
+#: parsers/i18n.py:52
 msgid "episodes"
-msgstr ""
+msgstr "latest episodes"
 
-#: parsers/i18n.py:35
+#: parsers/i18n.py:53
 msgid "podcasts"
 msgstr ""
```

### Comparing `ytmusicapi-1.6.0/ytmusicapi/locales/de/LC_MESSAGES/base.mo` & `ytmusicapi-1.7.0/ytmusicapi/locales/pt/LC_MESSAGES/base.mo`

 * *Files 23% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,53 +1,57 @@
 msgid ""
 msgstr ""
-"Project-Id-Version: PACKAGE VERSION\n"
+"Project-Id-Version: \n"
 "Report-Msgid-Bugs-To: \n"
-"PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
-"Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
-"Language-Team: LANGUAGE <LL@li.org>\n"
-"Language: \n"
+"PO-Revision-Date: 2023-01-01 12:15+0530\n"
+"Last-Translator: \n"
+"Language-Team: \n"
+"Language: pt\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
+"X-Generator: Poedit 3.2.2\n"
 
 msgid "albums"
-msgstr "alben"
+msgstr "álbuns"
 
 msgid "artist"
-msgstr "künstler"
+msgstr "artista"
 
 msgid "episode"
-msgstr "Folge"
+msgstr "Episódio"
 
 msgid "episodes"
-msgstr "neueste folgen"
+msgstr "episódios novos"
 
 msgid "playlist"
-msgstr "playlist"
+msgstr "lista de reprodução"
 
 msgid "playlists"
-msgstr "playlists"
+msgstr "listas de reprodução"
 
 msgid "podcasts"
 msgstr "podcasts"
 
 msgid "profile"
-msgstr "profil"
+msgstr "perfil"
 
 msgid "related"
-msgstr "das könnte fans auch gefallen"
+msgstr "relacionado"
+
+msgid "shows"
+msgstr "Audiolivros e programas"
 
 msgid "singles"
-msgstr "singles"
+msgstr "solteiros"
 
 msgid "song"
-msgstr "titel"
+msgstr "música"
 
 msgid "station"
-msgstr "sender"
+msgstr "estação"
 
 msgid "video"
-msgstr "video"
+msgstr "vídeo"
 
 msgid "videos"
-msgstr "videos"
+msgstr "vídeos"
```

### Comparing `ytmusicapi-1.6.0/ytmusicapi/locales/de/LC_MESSAGES/base.po` & `ytmusicapi-1.7.0/ytmusicapi/locales/de/LC_MESSAGES/base.po`

 * *Files 12% similar despite different names*

```diff
@@ -1,78 +1,82 @@
 # Translations for ytmusicapi
 # Copyright (C) 2023 sigma67
 # This file is distributed under the same license as ytmusicapi
 # sigma67 <ytmusicapi@gmail.com>
-#
+# 
 #, fuzzy
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2024-03-05 20:13+0100\n"
+"POT-Creation-Date: 2024-03-13 20:07+0100\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language-Team: LANGUAGE <LL@li.org>\n"
 "Language: \n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 
-#: parsers/i18n.py:22
+#: parsers/i18n.py:32
 msgid "artist"
 msgstr "künstler"
 
-#: parsers/i18n.py:23
+#: parsers/i18n.py:33
 msgid "playlist"
 msgstr "playlist"
 
-#: parsers/i18n.py:24
+#: parsers/i18n.py:34
 msgid "song"
 msgstr "titel"
 
-#: parsers/i18n.py:25
+#: parsers/i18n.py:35
 msgid "video"
 msgstr "video"
 
-#: parsers/i18n.py:26
+#: parsers/i18n.py:36
 msgid "station"
 msgstr "sender"
 
-#: parsers/i18n.py:27
+#: parsers/i18n.py:37
 msgid "profile"
 msgstr "profil"
 
-#: parsers/i18n.py:28
+#: parsers/i18n.py:38
 msgid "podcast"
 msgstr ""
 
-#: parsers/i18n.py:29
+#: parsers/i18n.py:39
 msgid "episode"
 msgstr "Folge"
 
-#: parsers/i18n.py:35
+#: parsers/i18n.py:46
 msgid "albums"
 msgstr "alben"
 
-#: parsers/i18n.py:35
+#: parsers/i18n.py:47
 msgid "singles"
 msgstr "singles"
 
-#: parsers/i18n.py:35
+#: parsers/i18n.py:48
+msgid "shows"
+msgstr "Hörbücher und Serien"
+
+#: parsers/i18n.py:49
 msgid "videos"
 msgstr "videos"
 
-#: parsers/i18n.py:35
+#: parsers/i18n.py:50
 msgid "playlists"
 msgstr "playlists"
 
-#: parsers/i18n.py:35
+#: parsers/i18n.py:51
 msgid "related"
 msgstr "das könnte fans auch gefallen"
 
-#: parsers/i18n.py:35
+#: parsers/i18n.py:52
 msgid "episodes"
 msgstr "neueste folgen"
 
-#: parsers/i18n.py:35
+#: parsers/i18n.py:53
 msgid "podcasts"
 msgstr "podcasts"
```

### Comparing `ytmusicapi-1.6.0/ytmusicapi/locales/en/LC_MESSAGES/base.po` & `ytmusicapi-1.7.0/ytmusicapi/locales/fr/LC_MESSAGES/base.po`

 * *Files 17% similar despite different names*

```diff
@@ -1,78 +1,82 @@
 # Translations for ytmusicapi
 # Copyright (C) 2023 sigma67
 # This file is distributed under the same license as ytmusicapi
 # sigma67 <ytmusicapi@gmail.com>
-#
+# 
 #, fuzzy
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2024-03-05 20:13+0100\n"
+"POT-Creation-Date: 2024-03-13 20:07+0100\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language-Team: LANGUAGE <LL@li.org>\n"
 "Language: \n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 
-#: parsers/i18n.py:22
+#: parsers/i18n.py:32
 msgid "artist"
-msgstr ""
+msgstr "artiste"
 
-#: parsers/i18n.py:23
+#: parsers/i18n.py:33
 msgid "playlist"
-msgstr ""
+msgstr "playlist"
 
-#: parsers/i18n.py:24
+#: parsers/i18n.py:34
 msgid "song"
-msgstr ""
+msgstr "titre"
 
-#: parsers/i18n.py:25
+#: parsers/i18n.py:35
 msgid "video"
-msgstr ""
+msgstr "vidéo"
 
-#: parsers/i18n.py:26
+#: parsers/i18n.py:36
 msgid "station"
-msgstr ""
+msgstr "radio"
 
-#: parsers/i18n.py:27
+#: parsers/i18n.py:37
 msgid "profile"
-msgstr ""
+msgstr "profil"
 
-#: parsers/i18n.py:28
+#: parsers/i18n.py:38
 msgid "podcast"
 msgstr ""
 
-#: parsers/i18n.py:29
+#: parsers/i18n.py:39
 msgid "episode"
-msgstr ""
+msgstr "Épisode"
 
-#: parsers/i18n.py:35
+#: parsers/i18n.py:46
 msgid "albums"
 msgstr ""
 
-#: parsers/i18n.py:35
+#: parsers/i18n.py:47
 msgid "singles"
 msgstr ""
 
-#: parsers/i18n.py:35
+#: parsers/i18n.py:48
+msgid "shows"
+msgstr "Livres audio et émissions"
+
+#: parsers/i18n.py:49
 msgid "videos"
-msgstr ""
+msgstr "vidéos"
 
-#: parsers/i18n.py:35
+#: parsers/i18n.py:50
 msgid "playlists"
 msgstr ""
 
-#: parsers/i18n.py:35
+#: parsers/i18n.py:51
 msgid "related"
-msgstr "fans might also like"
+msgstr "vous aimerez peut-être aussi"
 
-#: parsers/i18n.py:35
+#: parsers/i18n.py:52
 msgid "episodes"
-msgstr "latest episodes"
+msgstr "épisodes les plus récents"
 
-#: parsers/i18n.py:35
+#: parsers/i18n.py:53
 msgid "podcasts"
 msgstr ""
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `ytmusicapi-1.6.0/ytmusicapi/locales/es/LC_MESSAGES/base.mo` & `ytmusicapi-1.7.0/ytmusicapi/locales/es/LC_MESSAGES/base.mo`

 * *Files 21% similar despite different names*

#### msgunfmt {}

```diff
@@ -36,14 +36,17 @@
 
 msgid "profile"
 msgstr "perfil"
 
 msgid "related"
 msgstr "puede que también te guste"
 
+msgid "shows"
+msgstr "Audiolibros y series"
+
 msgid "singles"
 msgstr "sencillos"
 
 msgid "song"
 msgstr "canción"
 
 msgid "station"
```

### Comparing `ytmusicapi-1.6.0/ytmusicapi/locales/es/LC_MESSAGES/base.po` & `ytmusicapi-1.7.0/ytmusicapi/locales/es/LC_MESSAGES/base.po`

 * *Files 12% similar despite different names*

```diff
@@ -1,78 +1,82 @@
 # Translations for ytmusicapi
 # Copyright (C) 2023 sigma67
 # This file is distributed under the same license as ytmusicapi
 # sigma67 <ytmusicapi@gmail.com>
-#
+# 
 #, fuzzy
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2024-03-05 20:13+0100\n"
+"POT-Creation-Date: 2024-03-13 20:07+0100\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language-Team: LANGUAGE <LL@li.org>\n"
 "Language: \n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 
-#: parsers/i18n.py:22
+#: parsers/i18n.py:32
 msgid "artist"
 msgstr "artista"
 
-#: parsers/i18n.py:23
+#: parsers/i18n.py:33
 msgid "playlist"
 msgstr "lista de reproducción"
 
-#: parsers/i18n.py:24
+#: parsers/i18n.py:34
 msgid "song"
 msgstr "canción"
 
-#: parsers/i18n.py:25
+#: parsers/i18n.py:35
 msgid "video"
 msgstr "vídeo"
 
-#: parsers/i18n.py:26
+#: parsers/i18n.py:36
 msgid "station"
 msgstr "emisora"
 
-#: parsers/i18n.py:27
+#: parsers/i18n.py:37
 msgid "profile"
 msgstr "perfil"
 
-#: parsers/i18n.py:28
+#: parsers/i18n.py:38
 msgid "podcast"
 msgstr "Pódcast"
 
-#: parsers/i18n.py:29
+#: parsers/i18n.py:39
 msgid "episode"
 msgstr "Episodio"
 
-#: parsers/i18n.py:35
+#: parsers/i18n.py:46
 msgid "albums"
 msgstr "álbumes"
 
-#: parsers/i18n.py:35
+#: parsers/i18n.py:47
 msgid "singles"
 msgstr "sencillos"
 
-#: parsers/i18n.py:35
+#: parsers/i18n.py:48
+msgid "shows"
+msgstr "Audiolibros y series"
+
+#: parsers/i18n.py:49
 msgid "videos"
 msgstr "vídeos"
 
-#: parsers/i18n.py:35
+#: parsers/i18n.py:50
 msgid "playlists"
 msgstr "listas de reproducción"
 
-#: parsers/i18n.py:35
+#: parsers/i18n.py:51
 msgid "related"
 msgstr "puede que también te guste"
 
-#: parsers/i18n.py:35
+#: parsers/i18n.py:52
 msgid "episodes"
 msgstr "últimos episodios"
 
-#: parsers/i18n.py:35
+#: parsers/i18n.py:53
 msgid "podcasts"
 msgstr "pódcasts"
```

### Comparing `ytmusicapi-1.6.0/ytmusicapi/locales/fr/LC_MESSAGES/base.mo` & `ytmusicapi-1.7.0/ytmusicapi/locales/zh_TW/LC_MESSAGES/base.mo`

 * *Files 24% similar despite different names*

#### msgunfmt {}

```diff
@@ -6,36 +6,36 @@
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language-Team: LANGUAGE <LL@li.org>\n"
 "Language: \n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 
-msgid "artist"
-msgstr "artiste"
-
-msgid "episode"
-msgstr "Épisode"
+msgid "albums"
+msgstr "專輯"
 
-msgid "episodes"
-msgstr "épisodes les plus récents"
+msgid "artist"
+msgstr "藝人"
 
 msgid "playlist"
-msgstr "playlist"
+msgstr "播放清單"
 
-msgid "profile"
-msgstr "profil"
+msgid "playlists"
+msgstr "精選收錄"
 
 msgid "related"
-msgstr "vous aimerez peut-être aussi"
+msgstr "粉絲可能也會喜歡"
+
+msgid "singles"
+msgstr "單曲"
 
 msgid "song"
-msgstr "titre"
+msgstr "歌曲"
 
 msgid "station"
-msgstr "radio"
+msgstr "電台"
 
 msgid "video"
-msgstr "vidéo"
+msgstr "影片"
 
 msgid "videos"
-msgstr "vidéos"
+msgstr "影片"
```

### Comparing `ytmusicapi-1.6.0/ytmusicapi/locales/fr/LC_MESSAGES/base.po` & `ytmusicapi-1.7.0/ytmusicapi/locales/tr/LC_MESSAGES/base.po`

 * *Files 23% similar despite different names*

```diff
@@ -1,78 +1,82 @@
 # Translations for ytmusicapi
 # Copyright (C) 2023 sigma67
 # This file is distributed under the same license as ytmusicapi
 # sigma67 <ytmusicapi@gmail.com>
-#
-#, fuzzy
+# 
 msgid ""
 msgstr ""
-"Project-Id-Version: PACKAGE VERSION\n"
+"Project-Id-Version: \n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2024-03-05 20:13+0100\n"
-"PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
-"Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
-"Language-Team: LANGUAGE <LL@li.org>\n"
-"Language: \n"
+"POT-Creation-Date: 2024-03-13 20:07+0100\n"
+"PO-Revision-Date: 2023-01-02 13:06+0530\n"
+"Last-Translator: \n"
+"Language-Team: \n"
+"Language: tr\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
+"X-Generator: Poedit 3.2.2\n"
 
-#: parsers/i18n.py:22
+#: parsers/i18n.py:32
 msgid "artist"
-msgstr "artiste"
+msgstr "sanatçı"
 
-#: parsers/i18n.py:23
+#: parsers/i18n.py:33
 msgid "playlist"
-msgstr "playlist"
+msgstr "çalma listesi"
 
-#: parsers/i18n.py:24
+#: parsers/i18n.py:34
 msgid "song"
-msgstr "titre"
+msgstr "şarkı"
 
-#: parsers/i18n.py:25
+#: parsers/i18n.py:35
 msgid "video"
-msgstr "vidéo"
+msgstr "video"
 
-#: parsers/i18n.py:26
+#: parsers/i18n.py:36
 msgid "station"
-msgstr "radio"
+msgstr "istasyon"
 
-#: parsers/i18n.py:27
+#: parsers/i18n.py:37
 msgid "profile"
 msgstr "profil"
 
-#: parsers/i18n.py:28
+#: parsers/i18n.py:38
 msgid "podcast"
 msgstr ""
 
-#: parsers/i18n.py:29
+#: parsers/i18n.py:39
 msgid "episode"
-msgstr "Épisode"
+msgstr "Bölüm"
 
-#: parsers/i18n.py:35
+#: parsers/i18n.py:46
 msgid "albums"
-msgstr ""
+msgstr "albümler"
 
-#: parsers/i18n.py:35
+#: parsers/i18n.py:47
 msgid "singles"
-msgstr ""
+msgstr "bekarlar"
 
-#: parsers/i18n.py:35
+#: parsers/i18n.py:48
+msgid "shows"
+msgstr "Sesli kitaplar ve programlar"
+
+#: parsers/i18n.py:49
 msgid "videos"
-msgstr "vidéos"
+msgstr "videolar"
 
-#: parsers/i18n.py:35
+#: parsers/i18n.py:50
 msgid "playlists"
-msgstr ""
+msgstr "çalma listeleri"
 
-#: parsers/i18n.py:35
+#: parsers/i18n.py:51
 msgid "related"
-msgstr "vous aimerez peut-être aussi"
+msgstr "ilişkili"
 
-#: parsers/i18n.py:35
+#: parsers/i18n.py:52
 msgid "episodes"
-msgstr "épisodes les plus récents"
+msgstr "son bölümler"
 
-#: parsers/i18n.py:35
+#: parsers/i18n.py:53
 msgid "podcasts"
-msgstr ""
+msgstr "podcast'ler"
```

### Comparing `ytmusicapi-1.6.0/ytmusicapi/locales/hi/LC_MESSAGES/base.mo` & `ytmusicapi-1.7.0/ytmusicapi/locales/hi/LC_MESSAGES/base.mo`

 * *Files 15% similar despite different names*

#### msgunfmt {}

```diff
@@ -37,14 +37,17 @@
 
 msgid "profile"
 msgstr "प्रोफ़ाइल"
 
 msgid "related"
 msgstr "सम्बंधित"
 
+msgid "shows"
+msgstr "ऑडियो बुक और ऑडियो शो"
+
 msgid "singles"
 msgstr "एकल"
 
 msgid "song"
 msgstr "गीत"
 
 msgid "station"
```

### Comparing `ytmusicapi-1.6.0/ytmusicapi/locales/hi/LC_MESSAGES/base.po` & `ytmusicapi-1.7.0/ytmusicapi/locales/hi/LC_MESSAGES/base.po`

 * *Files 9% similar despite different names*

```diff
@@ -1,78 +1,82 @@
 # Translations for ytmusicapi
 # Copyright (C) 2023 sigma67
 # This file is distributed under the same license as ytmusicapi
 # sigma67 <ytmusicapi@gmail.com>
-#
+# 
 msgid ""
 msgstr ""
 "Project-Id-Version: \n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2024-03-05 20:13+0100\n"
+"POT-Creation-Date: 2024-03-13 20:07+0100\n"
 "PO-Revision-Date: 2023-01-01 11:04+0530\n"
 "Last-Translator: \n"
 "Language-Team: \n"
 "Language: hi\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "X-Generator: Poedit 3.2.2\n"
 
-#: parsers/i18n.py:22
+#: parsers/i18n.py:32
 msgid "artist"
 msgstr "कलाकार"
 
-#: parsers/i18n.py:23
+#: parsers/i18n.py:33
 msgid "playlist"
 msgstr "प्लेलिस्ट"
 
-#: parsers/i18n.py:24
+#: parsers/i18n.py:34
 msgid "song"
 msgstr "गीत"
 
-#: parsers/i18n.py:25
+#: parsers/i18n.py:35
 msgid "video"
 msgstr "वीडियो"
 
-#: parsers/i18n.py:26
+#: parsers/i18n.py:36
 msgid "station"
 msgstr "स्टेशन"
 
-#: parsers/i18n.py:27
+#: parsers/i18n.py:37
 msgid "profile"
 msgstr "प्रोफ़ाइल"
 
-#: parsers/i18n.py:28
+#: parsers/i18n.py:38
 msgid "podcast"
 msgstr "पॉडकास्ट"
 
-#: parsers/i18n.py:29
+#: parsers/i18n.py:39
 msgid "episode"
 msgstr "एपिसोड"
 
-#: parsers/i18n.py:35
+#: parsers/i18n.py:46
 msgid "albums"
 msgstr "एलबम"
 
-#: parsers/i18n.py:35
+#: parsers/i18n.py:47
 msgid "singles"
 msgstr "एकल"
 
-#: parsers/i18n.py:35
+#: parsers/i18n.py:48
+msgid "shows"
+msgstr "ऑडियो बुक और ऑडियो शो"
+
+#: parsers/i18n.py:49
 msgid "videos"
 msgstr "वीडियो"
 
-#: parsers/i18n.py:35
+#: parsers/i18n.py:50
 msgid "playlists"
 msgstr "प्लेलिस्ट"
 
-#: parsers/i18n.py:35
+#: parsers/i18n.py:51
 msgid "related"
 msgstr "सम्बंधित"
 
-#: parsers/i18n.py:35
+#: parsers/i18n.py:52
 msgid "episodes"
 msgstr "सबसे नए एपिसोड"
 
-#: parsers/i18n.py:35
+#: parsers/i18n.py:53
 msgid "podcasts"
 msgstr "पॉडकास्ट"
```

### Comparing `ytmusicapi-1.6.0/ytmusicapi/locales/it/LC_MESSAGES/base.mo` & `ytmusicapi-1.7.0/ytmusicapi/locales/ko/LC_MESSAGES/base.mo`

 * *Files 23% similar despite different names*

#### msgunfmt {}

```diff
@@ -7,41 +7,53 @@
 "Language-Team: LANGUAGE <LL@li.org>\n"
 "Language: \n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 
 msgid "albums"
-msgstr "album"
+msgstr "앨범"
 
 msgid "artist"
-msgstr "artista"
+msgstr "아티스트"
 
 msgid "episode"
-msgstr "Puntata"
+msgstr "에피소드"
 
 msgid "episodes"
-msgstr "puntate più recenti"
+msgstr "최신 에피소드"
+
+msgid "playlist"
+msgstr "재생목록"
 
 msgid "playlists"
-msgstr "playlist"
+msgstr "재싱목록"
+
+msgid "podcast"
+msgstr "팟캐스트"
 
 msgid "podcasts"
-msgstr "podcast"
+msgstr "팟캐스트"
 
 msgid "profile"
-msgstr "profilo"
+msgstr "프로필"
 
 msgid "related"
-msgstr "ai fan potrebbe anche piacere"
+msgstr "fans might also like"
+
+msgid "shows"
+msgstr "오디오북 및 프로그램"
 
 msgid "singles"
-msgstr "singoli"
+msgstr "싱글"
 
 msgid "song"
-msgstr "brano"
+msgstr "노래"
 
 msgid "station"
-msgstr "stazione"
+msgstr "스테이션"
+
+msgid "video"
+msgstr "동영상"
 
 msgid "videos"
-msgstr "video"
+msgstr "동영상"
```

### Comparing `ytmusicapi-1.6.0/ytmusicapi/locales/it/LC_MESSAGES/base.po` & `ytmusicapi-1.7.0/ytmusicapi/locales/it/LC_MESSAGES/base.po`

 * *Files 14% similar despite different names*

```diff
@@ -1,78 +1,82 @@
 # Translations for ytmusicapi
 # Copyright (C) 2023 sigma67
 # This file is distributed under the same license as ytmusicapi
 # sigma67 <ytmusicapi@gmail.com>
-#
+# 
 #, fuzzy
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2024-03-05 20:13+0100\n"
+"POT-Creation-Date: 2024-03-13 20:07+0100\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language-Team: LANGUAGE <LL@li.org>\n"
 "Language: \n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 
-#: parsers/i18n.py:22
+#: parsers/i18n.py:32
 msgid "artist"
 msgstr "artista"
 
-#: parsers/i18n.py:23
+#: parsers/i18n.py:33
 msgid "playlist"
 msgstr ""
 
-#: parsers/i18n.py:24
+#: parsers/i18n.py:34
 msgid "song"
 msgstr "brano"
 
-#: parsers/i18n.py:25
+#: parsers/i18n.py:35
 msgid "video"
 msgstr ""
 
-#: parsers/i18n.py:26
+#: parsers/i18n.py:36
 msgid "station"
 msgstr "stazione"
 
-#: parsers/i18n.py:27
+#: parsers/i18n.py:37
 msgid "profile"
 msgstr "profilo"
 
-#: parsers/i18n.py:28
+#: parsers/i18n.py:38
 msgid "podcast"
 msgstr ""
 
-#: parsers/i18n.py:29
+#: parsers/i18n.py:39
 msgid "episode"
 msgstr "Puntata"
 
-#: parsers/i18n.py:35
+#: parsers/i18n.py:46
 msgid "albums"
 msgstr "album"
 
-#: parsers/i18n.py:35
+#: parsers/i18n.py:47
 msgid "singles"
 msgstr "singoli"
 
-#: parsers/i18n.py:35
+#: parsers/i18n.py:48
+msgid "shows"
+msgstr "Audiolibri e programmi"
+
+#: parsers/i18n.py:49
 msgid "videos"
 msgstr "video"
 
-#: parsers/i18n.py:35
+#: parsers/i18n.py:50
 msgid "playlists"
 msgstr "playlist"
 
-#: parsers/i18n.py:35
+#: parsers/i18n.py:51
 msgid "related"
 msgstr "ai fan potrebbe anche piacere"
 
-#: parsers/i18n.py:35
+#: parsers/i18n.py:52
 msgid "episodes"
 msgstr "puntate più recenti"
 
-#: parsers/i18n.py:35
+#: parsers/i18n.py:53
 msgid "podcasts"
 msgstr "podcast"
```

### Comparing `ytmusicapi-1.6.0/ytmusicapi/locales/ja/LC_MESSAGES/base.mo` & `ytmusicapi-1.7.0/ytmusicapi/locales/ja/LC_MESSAGES/base.mo`

 * *Files 10% similar despite different names*

#### msgunfmt {}

```diff
@@ -36,14 +36,17 @@
 
 msgid "profile"
 msgstr "プロフィール"
 
 msgid "related"
 msgstr "おすすめのアーティスト"
 
+msgid "shows"
+msgstr "オーディオブックと番組"
+
 msgid "singles"
 msgstr "シングル"
 
 msgid "song"
 msgstr "曲"
 
 msgid "station"
```

### Comparing `ytmusicapi-1.6.0/ytmusicapi/locales/ja/LC_MESSAGES/base.po` & `ytmusicapi-1.7.0/ytmusicapi/locales/ja/LC_MESSAGES/base.po`

 * *Files 8% similar despite different names*

```diff
@@ -1,78 +1,82 @@
 # Translations for ytmusicapi
 # Copyright (C) 2023 sigma67
 # This file is distributed under the same license as ytmusicapi
 # sigma67 <ytmusicapi@gmail.com>
-#
+# 
 #, fuzzy
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2024-03-05 20:13+0100\n"
+"POT-Creation-Date: 2024-03-13 20:07+0100\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language-Team: LANGUAGE <LL@li.org>\n"
 "Language: \n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 
-#: parsers/i18n.py:22
+#: parsers/i18n.py:32
 msgid "artist"
 msgstr "アーティスト"
 
-#: parsers/i18n.py:23
+#: parsers/i18n.py:33
 msgid "playlist"
 msgstr "プレイリスト"
 
-#: parsers/i18n.py:24
+#: parsers/i18n.py:34
 msgid "song"
 msgstr "曲"
 
-#: parsers/i18n.py:25
+#: parsers/i18n.py:35
 msgid "video"
 msgstr "動画"
 
-#: parsers/i18n.py:26
+#: parsers/i18n.py:36
 msgid "station"
 msgstr "ステーション"
 
-#: parsers/i18n.py:27
+#: parsers/i18n.py:37
 msgid "profile"
 msgstr "プロフィール"
 
-#: parsers/i18n.py:28
+#: parsers/i18n.py:38
 msgid "podcast"
 msgstr "ポッドキャスト"
 
-#: parsers/i18n.py:29
+#: parsers/i18n.py:39
 msgid "episode"
 msgstr "エピソード"
 
-#: parsers/i18n.py:35
+#: parsers/i18n.py:46
 msgid "albums"
 msgstr "アルバム"
 
-#: parsers/i18n.py:35
+#: parsers/i18n.py:47
 msgid "singles"
 msgstr "シングル"
 
-#: parsers/i18n.py:35
+#: parsers/i18n.py:48
+msgid "shows"
+msgstr "オーディオブックと番組"
+
+#: parsers/i18n.py:49
 msgid "videos"
 msgstr "動画"
 
-#: parsers/i18n.py:35
+#: parsers/i18n.py:50
 msgid "playlists"
 msgstr "プレイリスト"
 
-#: parsers/i18n.py:35
+#: parsers/i18n.py:51
 msgid "related"
 msgstr "おすすめのアーティスト"
 
-#: parsers/i18n.py:35
+#: parsers/i18n.py:52
 msgid "episodes"
 msgstr "最新エピソード"
 
-#: parsers/i18n.py:35
+#: parsers/i18n.py:53
 msgid "podcasts"
 msgstr "ポッドキャスト"
```

### Comparing `ytmusicapi-1.6.0/ytmusicapi/locales/ko/LC_MESSAGES/base.mo` & `ytmusicapi-1.7.0/ytmusicapi/locales/nl/LC_MESSAGES/base.mo`

 * *Files 26% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,56 +1,58 @@
 msgid ""
 msgstr ""
-"Project-Id-Version: PACKAGE VERSION\n"
+"Project-Id-Version: \n"
 "Report-Msgid-Bugs-To: \n"
-"PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
-"Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
-"Language-Team: LANGUAGE <LL@li.org>\n"
-"Language: \n"
+"PO-Revision-Date: 2023-04-23 14:55+0200\n"
+"Last-Translator: Heimen Stoffels <vistausss@fastmail.com>\n"
+"Language-Team: \n"
+"Language: nl\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
+"Plural-Forms: nplurals=2; plural=(n != 1);\n"
+"X-Generator: Poedit 3.2.2\n"
 
 msgid "albums"
-msgstr "앨범"
+msgstr "albums"
 
 msgid "artist"
-msgstr "아티스트"
+msgstr "artiest"
 
 msgid "episode"
-msgstr "에피소드"
+msgstr "Aflevering"
 
 msgid "episodes"
-msgstr "최신 에피소드"
+msgstr "nieuwste afleveringen"
 
 msgid "playlist"
-msgstr "재생목록"
+msgstr "afspeellijst"
 
 msgid "playlists"
-msgstr "재싱목록"
-
-msgid "podcast"
-msgstr "팟캐스트"
+msgstr "afspeellijsten"
 
 msgid "podcasts"
-msgstr "팟캐스트"
+msgstr "podcasts"
 
 msgid "profile"
-msgstr "프로필"
+msgstr "profiel"
 
 msgid "related"
-msgstr "fans might also like"
+msgstr "gerelateerd"
+
+msgid "shows"
+msgstr "Audioboeken en -series"
 
 msgid "singles"
-msgstr "싱글"
+msgstr "singles"
 
 msgid "song"
-msgstr "노래"
+msgstr "nummer"
 
 msgid "station"
-msgstr "스테이션"
+msgstr "station"
 
 msgid "video"
-msgstr "동영상"
+msgstr "video"
 
 msgid "videos"
-msgstr "동영상"
+msgstr "video's"
```

### Comparing `ytmusicapi-1.6.0/ytmusicapi/locales/ko/LC_MESSAGES/base.po` & `ytmusicapi-1.7.0/ytmusicapi/locales/ko/LC_MESSAGES/base.po`

 * *Files 6% similar despite different names*

```diff
@@ -1,78 +1,82 @@
 # Translations for ytmusicapi
 # Copyright (C) 2023 sigma67
 # This file is distributed under the same license as ytmusicapi
 # sigma67 <ytmusicapi@gmail.com>
-#
+# 
 #, fuzzy
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2024-03-05 20:13+0100\n"
+"POT-Creation-Date: 2024-03-13 20:07+0100\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language-Team: LANGUAGE <LL@li.org>\n"
 "Language: \n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 
-#: parsers/i18n.py:22
+#: parsers/i18n.py:32
 msgid "artist"
 msgstr "아티스트"
 
-#: parsers/i18n.py:23
+#: parsers/i18n.py:33
 msgid "playlist"
 msgstr "재생목록"
 
-#: parsers/i18n.py:24
+#: parsers/i18n.py:34
 msgid "song"
 msgstr "노래"
 
-#: parsers/i18n.py:25
+#: parsers/i18n.py:35
 msgid "video"
 msgstr "동영상"
 
-#: parsers/i18n.py:26
+#: parsers/i18n.py:36
 msgid "station"
 msgstr "스테이션"
 
-#: parsers/i18n.py:27
+#: parsers/i18n.py:37
 msgid "profile"
 msgstr "프로필"
 
-#: parsers/i18n.py:28
+#: parsers/i18n.py:38
 msgid "podcast"
 msgstr "팟캐스트"
 
-#: parsers/i18n.py:29
+#: parsers/i18n.py:39
 msgid "episode"
 msgstr "에피소드"
 
-#: parsers/i18n.py:35
+#: parsers/i18n.py:46
 msgid "albums"
 msgstr "앨범"
 
-#: parsers/i18n.py:35
+#: parsers/i18n.py:47
 msgid "singles"
 msgstr "싱글"
 
-#: parsers/i18n.py:35
+#: parsers/i18n.py:48
+msgid "shows"
+msgstr "오디오북 및 프로그램"
+
+#: parsers/i18n.py:49
 msgid "videos"
 msgstr "동영상"
 
-#: parsers/i18n.py:35
+#: parsers/i18n.py:50
 msgid "playlists"
 msgstr "재싱목록"
 
-#: parsers/i18n.py:35
+#: parsers/i18n.py:51
 msgid "related"
 msgstr "fans might also like"
 
-#: parsers/i18n.py:35
+#: parsers/i18n.py:52
 msgid "episodes"
 msgstr "최신 에피소드"
 
-#: parsers/i18n.py:35
+#: parsers/i18n.py:53
 msgid "podcasts"
 msgstr "팟캐스트"
```

### Comparing `ytmusicapi-1.6.0/ytmusicapi/locales/nl/LC_MESSAGES/base.po` & `ytmusicapi-1.7.0/ytmusicapi/locales/zh_CN/LC_MESSAGES/base.po`

 * *Files 10% similar despite different names*

```diff
@@ -1,79 +1,81 @@
 # Translations for ytmusicapi
 # Copyright (C) 2023 sigma67
 # This file is distributed under the same license as ytmusicapi
 # sigma67 <ytmusicapi@gmail.com>
-#
+# 
 msgid ""
 msgstr ""
-"Project-Id-Version: \n"
+"Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2024-03-05 20:13+0100\n"
-"PO-Revision-Date: 2023-04-23 14:55+0200\n"
-"Last-Translator: Heimen Stoffels <vistausss@fastmail.com>\n"
-"Language-Team: \n"
-"Language: nl\n"
+"POT-Creation-Date: 2024-03-13 20:07+0100\n"
+"PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
+"Last-Translator: Bruce Zhang <zttt183525594@gmail.com>\n"
+"Language-Team: LANGUAGE <LL@li.org>\n"
+"Language: \n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Plural-Forms: nplurals=2; plural=(n != 1);\n"
-"X-Generator: Poedit 3.2.2\n"
 
-#: parsers/i18n.py:22
+#: parsers/i18n.py:32
 msgid "artist"
-msgstr "artiest"
+msgstr "音乐人"
 
-#: parsers/i18n.py:23
+#: parsers/i18n.py:33
 msgid "playlist"
-msgstr "afspeellijst"
+msgstr "播放列表"
 
-#: parsers/i18n.py:24
+#: parsers/i18n.py:34
 msgid "song"
-msgstr "nummer"
+msgstr "歌曲"
 
-#: parsers/i18n.py:25
+#: parsers/i18n.py:35
 msgid "video"
-msgstr "video"
+msgstr "视频"
 
-#: parsers/i18n.py:26
+#: parsers/i18n.py:36
 msgid "station"
-msgstr "station"
+msgstr "电台"
 
-#: parsers/i18n.py:27
+#: parsers/i18n.py:37
 msgid "profile"
-msgstr "profiel"
+msgstr "个人资料"
 
-#: parsers/i18n.py:28
+#: parsers/i18n.py:38
 msgid "podcast"
-msgstr ""
+msgstr "播客"
 
-#: parsers/i18n.py:29
+#: parsers/i18n.py:39
 msgid "episode"
-msgstr "Aflevering"
+msgstr "分集"
 
-#: parsers/i18n.py:35
+#: parsers/i18n.py:46
 msgid "albums"
-msgstr "albums"
+msgstr "专辑"
 
-#: parsers/i18n.py:35
+#: parsers/i18n.py:47
 msgid "singles"
-msgstr "singles"
+msgstr "单曲"
 
-#: parsers/i18n.py:35
+#: parsers/i18n.py:48
+msgid "shows"
+msgstr "有声读物和节目"
+
+#: parsers/i18n.py:49
 msgid "videos"
-msgstr "video's"
+msgstr "视频"
 
-#: parsers/i18n.py:35
+#: parsers/i18n.py:50
 msgid "playlists"
-msgstr "afspeellijsten"
+msgstr "精选"
 
-#: parsers/i18n.py:35
+#: parsers/i18n.py:51
 msgid "related"
-msgstr "gerelateerd"
+msgstr "粉丝可能还会喜欢"
 
-#: parsers/i18n.py:35
+#: parsers/i18n.py:52
 msgid "episodes"
-msgstr "nieuwste afleveringen"
+msgstr "最新分集"
 
-#: parsers/i18n.py:35
+#: parsers/i18n.py:53
 msgid "podcasts"
-msgstr "podcasts"
+msgstr "播客"
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `ytmusicapi-1.6.0/ytmusicapi/locales/pt/LC_MESSAGES/base.po` & `ytmusicapi-1.7.0/ytmusicapi/locales/zh_TW/LC_MESSAGES/base.po`

 * *Files 16% similar despite different names*

```diff
@@ -1,78 +1,82 @@
 # Translations for ytmusicapi
 # Copyright (C) 2023 sigma67
 # This file is distributed under the same license as ytmusicapi
 # sigma67 <ytmusicapi@gmail.com>
-#
+# 
+#, fuzzy
 msgid ""
 msgstr ""
-"Project-Id-Version: \n"
+"Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2024-03-05 20:13+0100\n"
-"PO-Revision-Date: 2023-01-01 12:15+0530\n"
-"Last-Translator: \n"
-"Language-Team: \n"
-"Language: pt\n"
+"POT-Creation-Date: 2024-03-13 20:07+0100\n"
+"PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
+"Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
+"Language-Team: LANGUAGE <LL@li.org>\n"
+"Language: \n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"X-Generator: Poedit 3.2.2\n"
 
-#: parsers/i18n.py:22
+#: parsers/i18n.py:32
 msgid "artist"
-msgstr "artista"
+msgstr "藝人"
 
-#: parsers/i18n.py:23
+#: parsers/i18n.py:33
 msgid "playlist"
-msgstr "lista de reprodução"
+msgstr "播放清單"
 
-#: parsers/i18n.py:24
+#: parsers/i18n.py:34
 msgid "song"
-msgstr "música"
+msgstr "歌曲"
 
-#: parsers/i18n.py:25
+#: parsers/i18n.py:35
 msgid "video"
-msgstr "vídeo"
+msgstr "影片"
 
-#: parsers/i18n.py:26
+#: parsers/i18n.py:36
 msgid "station"
-msgstr "estação"
+msgstr "電台"
 
-#: parsers/i18n.py:27
+#: parsers/i18n.py:37
 msgid "profile"
-msgstr "perfil"
+msgstr "個人資料"
 
-#: parsers/i18n.py:28
+#: parsers/i18n.py:38
 msgid "podcast"
 msgstr ""
 
-#: parsers/i18n.py:29
+#: parsers/i18n.py:39
 msgid "episode"
-msgstr "Episódio"
+msgstr "單集"
 
-#: parsers/i18n.py:35
+#: parsers/i18n.py:46
 msgid "albums"
-msgstr "álbuns"
+msgstr "專輯"
 
-#: parsers/i18n.py:35
+#: parsers/i18n.py:47
 msgid "singles"
-msgstr "solteiros"
+msgstr "單曲"
 
-#: parsers/i18n.py:35
+#: parsers/i18n.py:48
+msgid "shows"
+msgstr "有聲書與節目"
+
+#: parsers/i18n.py:49
 msgid "videos"
-msgstr "vídeos"
+msgstr "影片"
 
-#: parsers/i18n.py:35
+#: parsers/i18n.py:50
 msgid "playlists"
-msgstr "listas de reprodução"
+msgstr "精選收錄"
 
-#: parsers/i18n.py:35
+#: parsers/i18n.py:51
 msgid "related"
-msgstr "relacionado"
+msgstr "粉絲可能也會喜歡"
 
-#: parsers/i18n.py:35
+#: parsers/i18n.py:52
 msgid "episodes"
-msgstr "episódios novos"
+msgstr "最新集數"
 
-#: parsers/i18n.py:35
+#: parsers/i18n.py:53
 msgid "podcasts"
-msgstr "podcasts"
+msgstr "Podcast"
```

### Comparing `ytmusicapi-1.6.0/ytmusicapi/locales/ru/LC_MESSAGES/base.mo` & `ytmusicapi-1.7.0/ytmusicapi/locales/ru/LC_MESSAGES/base.mo`

 * *Files 15% similar despite different names*

#### msgunfmt {}

```diff
@@ -37,14 +37,17 @@
 
 msgid "profile"
 msgstr "профиль"
 
 msgid "related"
 msgstr "связанные с"
 
+msgid "shows"
+msgstr "Аудиокниги и аудиошоу"
+
 msgid "singles"
 msgstr "синглы"
 
 msgid "song"
 msgstr "песня"
 
 msgid "station"
```

### Comparing `ytmusicapi-1.6.0/ytmusicapi/locales/ru/LC_MESSAGES/base.po` & `ytmusicapi-1.7.0/ytmusicapi/locales/ru/LC_MESSAGES/base.po`

 * *Files 8% similar despite different names*

```diff
@@ -1,78 +1,82 @@
 # Translations for ytmusicapi
 # Copyright (C) 2023 sigma67
 # This file is distributed under the same license as ytmusicapi
 # sigma67 <ytmusicapi@gmail.com>
-#
+# 
 msgid ""
 msgstr ""
 "Project-Id-Version: \n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2024-03-05 20:13+0100\n"
+"POT-Creation-Date: 2024-03-13 20:07+0100\n"
 "PO-Revision-Date: 2023-01-01 09:48+0530\n"
 "Last-Translator: \n"
 "Language-Team: \n"
 "Language: ru\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "X-Generator: Poedit 3.2.2\n"
 
-#: parsers/i18n.py:22
+#: parsers/i18n.py:32
 msgid "artist"
 msgstr "художник"
 
-#: parsers/i18n.py:23
+#: parsers/i18n.py:33
 msgid "playlist"
 msgstr "плейлист"
 
-#: parsers/i18n.py:24
+#: parsers/i18n.py:34
 msgid "song"
 msgstr "песня"
 
-#: parsers/i18n.py:25
+#: parsers/i18n.py:35
 msgid "video"
 msgstr "видео"
 
-#: parsers/i18n.py:26
+#: parsers/i18n.py:36
 msgid "station"
 msgstr "станция"
 
-#: parsers/i18n.py:27
+#: parsers/i18n.py:37
 msgid "profile"
 msgstr "профиль"
 
-#: parsers/i18n.py:28
+#: parsers/i18n.py:38
 msgid "podcast"
 msgstr "Подкаст"
 
-#: parsers/i18n.py:29
+#: parsers/i18n.py:39
 msgid "episode"
 msgstr "Выпуск"
 
-#: parsers/i18n.py:35
+#: parsers/i18n.py:46
 msgid "albums"
 msgstr "альбомы"
 
-#: parsers/i18n.py:35
+#: parsers/i18n.py:47
 msgid "singles"
 msgstr "синглы"
 
-#: parsers/i18n.py:35
+#: parsers/i18n.py:48
+msgid "shows"
+msgstr "Аудиокниги и аудиошоу"
+
+#: parsers/i18n.py:49
 msgid "videos"
 msgstr "ролики"
 
-#: parsers/i18n.py:35
+#: parsers/i18n.py:50
 msgid "playlists"
 msgstr "плейлисты"
 
-#: parsers/i18n.py:35
+#: parsers/i18n.py:51
 msgid "related"
 msgstr "связанные с"
 
-#: parsers/i18n.py:35
+#: parsers/i18n.py:52
 msgid "episodes"
 msgstr "новые выпуски"
 
-#: parsers/i18n.py:35
+#: parsers/i18n.py:53
 msgid "podcasts"
 msgstr "подкасты"
```

### Comparing `ytmusicapi-1.6.0/ytmusicapi/locales/tr/LC_MESSAGES/base.mo` & `ytmusicapi-1.7.0/ytmusicapi/locales/tr/LC_MESSAGES/base.mo`

 * *Files 25% similar despite different names*

#### msgunfmt {}

```diff
@@ -34,14 +34,17 @@
 
 msgid "profile"
 msgstr "profil"
 
 msgid "related"
 msgstr "ilişkili"
 
+msgid "shows"
+msgstr "Sesli kitaplar ve programlar"
+
 msgid "singles"
 msgstr "bekarlar"
 
 msgid "song"
 msgstr "şarkı"
 
 msgid "station"
```

### Comparing `ytmusicapi-1.6.0/ytmusicapi/locales/tr/LC_MESSAGES/base.po` & `ytmusicapi-1.7.0/ytmusicapi/locales/base.pot`

 * *Files 14% similar despite different names*

```diff
@@ -1,78 +1,82 @@
-# Translations for ytmusicapi
-# Copyright (C) 2023 sigma67
-# This file is distributed under the same license as ytmusicapi
-# sigma67 <ytmusicapi@gmail.com>
+# SOME DESCRIPTIVE TITLE.
+# Copyright (C) YEAR THE PACKAGE'S COPYRIGHT HOLDER
+# This file is distributed under the same license as the PACKAGE package.
+# FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
 #
+#, fuzzy
 msgid ""
 msgstr ""
-"Project-Id-Version: \n"
+"Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2024-03-05 20:13+0100\n"
-"PO-Revision-Date: 2023-01-02 13:06+0530\n"
-"Last-Translator: \n"
-"Language-Team: \n"
-"Language: tr\n"
+"POT-Creation-Date: 2024-03-13 20:07+0100\n"
+"PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
+"Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
+"Language-Team: LANGUAGE <LL@li.org>\n"
+"Language: \n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"X-Generator: Poedit 3.2.2\n"
 
-#: parsers/i18n.py:22
+#: parsers/i18n.py:32
 msgid "artist"
-msgstr "sanatçı"
+msgstr ""
 
-#: parsers/i18n.py:23
+#: parsers/i18n.py:33
 msgid "playlist"
-msgstr "çalma listesi"
+msgstr ""
 
-#: parsers/i18n.py:24
+#: parsers/i18n.py:34
 msgid "song"
-msgstr "şarkı"
+msgstr ""
 
-#: parsers/i18n.py:25
+#: parsers/i18n.py:35
 msgid "video"
-msgstr "video"
+msgstr ""
 
-#: parsers/i18n.py:26
+#: parsers/i18n.py:36
 msgid "station"
-msgstr "istasyon"
+msgstr ""
 
-#: parsers/i18n.py:27
+#: parsers/i18n.py:37
 msgid "profile"
-msgstr "profil"
+msgstr ""
 
-#: parsers/i18n.py:28
+#: parsers/i18n.py:38
 msgid "podcast"
 msgstr ""
 
-#: parsers/i18n.py:29
+#: parsers/i18n.py:39
 msgid "episode"
-msgstr "Bölüm"
+msgstr ""
 
-#: parsers/i18n.py:35
+#: parsers/i18n.py:46
 msgid "albums"
-msgstr "albümler"
+msgstr ""
 
-#: parsers/i18n.py:35
+#: parsers/i18n.py:47
 msgid "singles"
-msgstr "bekarlar"
+msgstr ""
 
-#: parsers/i18n.py:35
+#: parsers/i18n.py:48
+msgid "shows"
+msgstr ""
+
+#: parsers/i18n.py:49
 msgid "videos"
-msgstr "videolar"
+msgstr ""
 
-#: parsers/i18n.py:35
+#: parsers/i18n.py:50
 msgid "playlists"
-msgstr "çalma listeleri"
+msgstr ""
 
-#: parsers/i18n.py:35
+#: parsers/i18n.py:51
 msgid "related"
-msgstr "ilişkili"
+msgstr ""
 
-#: parsers/i18n.py:35
+#: parsers/i18n.py:52
 msgid "episodes"
-msgstr "son bölümler"
+msgstr ""
 
-#: parsers/i18n.py:35
+#: parsers/i18n.py:53
 msgid "podcasts"
-msgstr "podcast'ler"
+msgstr ""
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `ytmusicapi-1.6.0/ytmusicapi/locales/ur/LC_MESSAGES/base.mo` & `ytmusicapi-1.7.0/ytmusicapi/locales/ur/LC_MESSAGES/base.mo`

 * *Files 19% similar despite different names*

#### msgunfmt {}

```diff
@@ -37,14 +37,17 @@
 
 msgid "profile"
 msgstr "پروفائ"
 
 msgid "related"
 msgstr "متعلقہ"
 
+msgid "shows"
+msgstr "آڈیو بکس اور شوز"
+
 msgid "singles"
 msgstr "سنگلز"
 
 msgid "song"
 msgstr "نغمہ"
 
 msgid "station"
```

### Comparing `ytmusicapi-1.6.0/ytmusicapi/locales/ur/LC_MESSAGES/base.po` & `ytmusicapi-1.7.0/ytmusicapi/locales/ur/LC_MESSAGES/base.po`

 * *Files 6% similar despite different names*

```diff
@@ -1,78 +1,82 @@
 # Translations for ytmusicapi
 # Copyright (C) 2023 sigma67
 # This file is distributed under the same license as ytmusicapi
 # sigma67 <ytmusicapi@gmail.com>
-#
+# 
 msgid ""
 msgstr ""
 "Project-Id-Version: \n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2024-03-05 20:13+0100\n"
+"POT-Creation-Date: 2024-03-13 20:07+0100\n"
 "PO-Revision-Date: 2023-01-02 22:18+0530\n"
 "Last-Translator: \n"
 "Language-Team: \n"
 "Language: ur\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "X-Generator: Poedit 3.2.2\n"
 
-#: parsers/i18n.py:22
+#: parsers/i18n.py:32
 msgid "artist"
 msgstr "فنکار"
 
-#: parsers/i18n.py:23
+#: parsers/i18n.py:33
 msgid "playlist"
 msgstr "پلے لسٹ"
 
-#: parsers/i18n.py:24
+#: parsers/i18n.py:34
 msgid "song"
 msgstr "نغمہ"
 
-#: parsers/i18n.py:25
+#: parsers/i18n.py:35
 msgid "video"
 msgstr "ویڈیو"
 
-#: parsers/i18n.py:26
+#: parsers/i18n.py:36
 msgid "station"
 msgstr "اسٹیشن"
 
-#: parsers/i18n.py:27
+#: parsers/i18n.py:37
 msgid "profile"
 msgstr "پروفائ"
 
-#: parsers/i18n.py:28
+#: parsers/i18n.py:38
 msgid "podcast"
 msgstr "پوڈکاسٹ"
 
-#: parsers/i18n.py:29
+#: parsers/i18n.py:39
 msgid "episode"
 msgstr "ایپی سوڈ"
 
-#: parsers/i18n.py:35
+#: parsers/i18n.py:46
 msgid "albums"
 msgstr "البمز"
 
-#: parsers/i18n.py:35
+#: parsers/i18n.py:47
 msgid "singles"
 msgstr "سنگلز"
 
-#: parsers/i18n.py:35
+#: parsers/i18n.py:48
+msgid "shows"
+msgstr "آڈیو بکس اور شوز"
+
+#: parsers/i18n.py:49
 msgid "videos"
 msgstr "ویڈیوز"
 
-#: parsers/i18n.py:35
+#: parsers/i18n.py:50
 msgid "playlists"
 msgstr "پلے لسٹس"
 
-#: parsers/i18n.py:35
+#: parsers/i18n.py:51
 msgid "related"
 msgstr "متعلقہ"
 
-#: parsers/i18n.py:35
+#: parsers/i18n.py:52
 msgid "episodes"
 msgstr "تازہ ترین ایپی سوڈز"
 
-#: parsers/i18n.py:35
+#: parsers/i18n.py:53
 msgid "podcasts"
 msgstr "پوڈکاسٹس"
```

### Comparing `ytmusicapi-1.6.0/ytmusicapi/locales/zh_CN/LC_MESSAGES/base.mo` & `ytmusicapi-1.7.0/ytmusicapi/locales/zh_CN/LC_MESSAGES/base.mo`

 * *Files identical despite different names*

### Comparing `ytmusicapi-1.6.0/ytmusicapi/locales/zh_CN/LC_MESSAGES/base.po` & `ytmusicapi-1.7.0/ytmusicapi/locales/ar/LC_MESSAGES/base.po`

 * *Files 24% similar despite different names*

```diff
@@ -1,77 +1,82 @@
 # Translations for ytmusicapi
 # Copyright (C) 2023 sigma67
 # This file is distributed under the same license as ytmusicapi
 # sigma67 <ytmusicapi@gmail.com>
-#
+# 
 msgid ""
 msgstr ""
-"Project-Id-Version: PACKAGE VERSION\n"
+"Project-Id-Version: \n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2024-03-05 20:13+0100\n"
-"PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
-"Last-Translator: Bruce Zhang <zttt183525594@gmail.com>\n"
-"Language-Team: LANGUAGE <LL@li.org>\n"
-"Language: \n"
+"POT-Creation-Date: 2024-03-13 20:07+0100\n"
+"PO-Revision-Date: 2023-01-02 22:14+0530\n"
+"Last-Translator: \n"
+"Language-Team: \n"
+"Language: ar\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
+"X-Generator: Poedit 3.2.2\n"
 
-#: parsers/i18n.py:22
+#: parsers/i18n.py:32
 msgid "artist"
-msgstr "音乐人"
+msgstr "فنان"
 
-#: parsers/i18n.py:23
+#: parsers/i18n.py:33
 msgid "playlist"
-msgstr "播放列表"
+msgstr "قائمةالتشغيل"
 
-#: parsers/i18n.py:24
+#: parsers/i18n.py:34
 msgid "song"
-msgstr "歌曲"
+msgstr "أغنية"
 
-#: parsers/i18n.py:25
+#: parsers/i18n.py:35
 msgid "video"
-msgstr "视频"
+msgstr "فيديو"
 
-#: parsers/i18n.py:26
+#: parsers/i18n.py:36
 msgid "station"
-msgstr "电台"
+msgstr "محطة"
 
-#: parsers/i18n.py:27
+#: parsers/i18n.py:37
 msgid "profile"
-msgstr "个人资料"
+msgstr "الملف الشخصي"
 
-#: parsers/i18n.py:28
+#: parsers/i18n.py:38
 msgid "podcast"
-msgstr "播客"
+msgstr "بودكاست"
 
-#: parsers/i18n.py:29
+#: parsers/i18n.py:39
 msgid "episode"
-msgstr "分集"
+msgstr "حلقة"
 
-#: parsers/i18n.py:35
+#: parsers/i18n.py:46
 msgid "albums"
-msgstr "专辑"
+msgstr "ألبومات"
 
-#: parsers/i18n.py:35
+#: parsers/i18n.py:47
 msgid "singles"
-msgstr "单曲"
+msgstr "الفردي"
 
-#: parsers/i18n.py:35
+#: parsers/i18n.py:48
+msgid "shows"
+msgstr "الكتب المسموعة والعروض"
+
+#: parsers/i18n.py:49
 msgid "videos"
-msgstr "视频"
+msgstr "أشرطة فيديو"
 
-#: parsers/i18n.py:35
+#: parsers/i18n.py:50
 msgid "playlists"
-msgstr "精选"
+msgstr "قوائم التشغيل"
 
-#: parsers/i18n.py:35
+#: parsers/i18n.py:51
 msgid "related"
-msgstr "粉丝可能还会喜欢"
+msgstr "ذات صلة"
 
-#: parsers/i18n.py:35
+#: parsers/i18n.py:52
 msgid "episodes"
-msgstr "最新分集"
+msgstr "أحدث الحلقات"
 
-#: parsers/i18n.py:35
+#: parsers/i18n.py:53
 msgid "podcasts"
-msgstr "播客"
+msgstr "بودكاست"
```

### Comparing `ytmusicapi-1.6.0/ytmusicapi/locales/zh_TW/LC_MESSAGES/base.po` & `ytmusicapi-1.7.0/ytmusicapi/locales/nl/LC_MESSAGES/base.po`

 * *Files 14% similar despite different names*

```diff
@@ -1,78 +1,83 @@
 # Translations for ytmusicapi
 # Copyright (C) 2023 sigma67
 # This file is distributed under the same license as ytmusicapi
 # sigma67 <ytmusicapi@gmail.com>
-#
-#, fuzzy
+# 
 msgid ""
 msgstr ""
-"Project-Id-Version: PACKAGE VERSION\n"
+"Project-Id-Version: \n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2024-03-05 20:13+0100\n"
-"PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
-"Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
-"Language-Team: LANGUAGE <LL@li.org>\n"
-"Language: \n"
+"POT-Creation-Date: 2024-03-13 20:07+0100\n"
+"PO-Revision-Date: 2023-04-23 14:55+0200\n"
+"Last-Translator: Heimen Stoffels <vistausss@fastmail.com>\n"
+"Language-Team: \n"
+"Language: nl\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
+"Plural-Forms: nplurals=2; plural=(n != 1);\n"
+"X-Generator: Poedit 3.2.2\n"
 
-#: parsers/i18n.py:22
+#: parsers/i18n.py:32
 msgid "artist"
-msgstr "藝人"
+msgstr "artiest"
 
-#: parsers/i18n.py:23
+#: parsers/i18n.py:33
 msgid "playlist"
-msgstr "播放清單"
+msgstr "afspeellijst"
 
-#: parsers/i18n.py:24
+#: parsers/i18n.py:34
 msgid "song"
-msgstr "歌曲"
+msgstr "nummer"
 
-#: parsers/i18n.py:25
+#: parsers/i18n.py:35
 msgid "video"
-msgstr "影片"
+msgstr "video"
 
-#: parsers/i18n.py:26
+#: parsers/i18n.py:36
 msgid "station"
-msgstr "電台"
+msgstr "station"
 
-#: parsers/i18n.py:27
+#: parsers/i18n.py:37
 msgid "profile"
-msgstr "個人資料"
+msgstr "profiel"
 
-#: parsers/i18n.py:28
+#: parsers/i18n.py:38
 msgid "podcast"
 msgstr ""
 
-#: parsers/i18n.py:29
+#: parsers/i18n.py:39
 msgid "episode"
-msgstr "單集"
+msgstr "Aflevering"
 
-#: parsers/i18n.py:35
+#: parsers/i18n.py:46
 msgid "albums"
-msgstr "專輯"
+msgstr "albums"
 
-#: parsers/i18n.py:35
+#: parsers/i18n.py:47
 msgid "singles"
-msgstr "單曲"
+msgstr "singles"
 
-#: parsers/i18n.py:35
+#: parsers/i18n.py:48
+msgid "shows"
+msgstr "Audioboeken en -series"
+
+#: parsers/i18n.py:49
 msgid "videos"
-msgstr "影片"
+msgstr "video's"
 
-#: parsers/i18n.py:35
+#: parsers/i18n.py:50
 msgid "playlists"
-msgstr "精選收錄"
+msgstr "afspeellijsten"
 
-#: parsers/i18n.py:35
+#: parsers/i18n.py:51
 msgid "related"
-msgstr "粉絲可能也會喜歡"
+msgstr "gerelateerd"
 
-#: parsers/i18n.py:35
+#: parsers/i18n.py:52
 msgid "episodes"
-msgstr "最新集數"
+msgstr "nieuwste afleveringen"
 
-#: parsers/i18n.py:35
+#: parsers/i18n.py:53
 msgid "podcasts"
-msgstr "Podcast"
+msgstr "podcasts"
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `ytmusicapi-1.6.0/ytmusicapi/mixins/_protocol.py` & `ytmusicapi-1.7.0/ytmusicapi/mixins/_protocol.py`

 * *Files identical despite different names*

### Comparing `ytmusicapi-1.6.0/ytmusicapi/mixins/_utils.py` & `ytmusicapi-1.7.0/ytmusicapi/mixins/_utils.py`

 * *Files identical despite different names*

### Comparing `ytmusicapi-1.6.0/ytmusicapi/mixins/browsing.py` & `ytmusicapi-1.7.0/ytmusicapi/mixins/browsing.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from typing import Any, Dict, List, Optional
 
 from ytmusicapi.continuations import (
     get_continuations,
     get_reloadable_continuation_params,
 )
 from ytmusicapi.helpers import YTM_DOMAIN, sum_total_duration
-from ytmusicapi.parsers.albums import parse_album_header
+from ytmusicapi.parsers.albums import parse_album_header, parse_album_header_2024
 from ytmusicapi.parsers.browsing import parse_album, parse_content_list, parse_mixed_content, parse_playlist
 from ytmusicapi.parsers.library import parse_albums
 from ytmusicapi.parsers.playlists import parse_playlist_items
 
 from ..navigation import *
 from ._protocol import MixinProtocol
 from ._utils import get_datestamp
@@ -127,16 +127,30 @@
 
     def get_artist(self, channelId: str) -> Dict:
         """
         Get information about an artist and their top releases (songs,
         albums, singles, videos, and related artists). The top lists
         contain pointers for getting the full list of releases.
 
-        For songs/videos, pass the browseId to :py:func:`get_playlist`.
-        For albums/singles, pass browseId and params to :py:func:`get_artist_albums`.
+        Possible content types for get_artist are:
+
+            - songs
+            - albums
+            - singles
+            - shows
+            - videos
+            - episodes
+            - podcasts
+            - related
+
+        Each of these content keys in the response contains
+        ``results`` and possibly ``browseId`` and ``params``.
+
+        - For songs/videos, pass the browseId to :py:func:`get_playlist`.
+        - For albums/singles/shows, pass browseId and params to :py:func:`get_artist_albums`.
 
         :param channelId: channel id of the artist
         :return: Dictionary with requested information.
 
         .. warning::
 
             The returned channelId is not the same as the one passed to the function.
@@ -256,15 +270,15 @@
         artist.update(self.parser.parse_channel_contents(results))
         return artist
 
     def get_artist_albums(
         self, channelId: str, params: str, limit: Optional[int] = 100, order: Optional[str] = None
     ) -> List[Dict]:
         """
-        Get the full list of an artist's albums or singles
+        Get the full list of an artist's albums, singles or shows
 
         :param channelId: browseId of the artist as returned by :py:func:`get_artist`
         :param params: params obtained by :py:func:`get_artist`
         :param limit: Number of albums to return. `None` retrieves them all. Default: 100
         :param order: Order of albums to return. Allowed values: 'Recency', 'Popularity', 'Alphabetical order'. Default: Default order.
         :return: List of albums in the format of :py:func:`get_library_albums`,
           except artists key is missing.
@@ -498,16 +512,23 @@
         """
         if not browseId or not browseId.startswith("MPRE"):
             raise Exception("Invalid album browseId provided, must start with MPRE.")
 
         body = {"browseId": browseId}
         endpoint = "browse"
         response = self._send_request(endpoint, body)
-        album = parse_album_header(response)
-        results = nav(response, SINGLE_COLUMN_TAB + SECTION_LIST_ITEM + MUSIC_SHELF)
+        if "header" in response:
+            album = parse_album_header(response)
+        else:
+            album = parse_album_header_2024(response)
+        results = nav(response, SINGLE_COLUMN_TAB + SECTION_LIST_ITEM + MUSIC_SHELF, True) or nav(
+            # fallback for 2024 format
+            response,
+            [*TWO_COLUMN_RENDERER, "secondaryContents", *SECTION_LIST_ITEM, *MUSIC_SHELF],
+        )
         album["tracks"] = parse_playlist_items(results["contents"], is_album=True)
         results = nav(response, SINGLE_COLUMN_TAB + SECTION_LIST + [1] + CAROUSEL, True)
         if results is not None:
             album["other_versions"] = parse_content_list(results["contents"], parse_album)
         album["duration_seconds"] = sum_total_duration(album)
         for i, track in enumerate(album["tracks"]):
             album["tracks"][i]["album"] = album["title"]
```

### Comparing `ytmusicapi-1.6.0/ytmusicapi/mixins/explore.py` & `ytmusicapi-1.7.0/ytmusicapi/mixins/explore.py`

 * *Files identical despite different names*

### Comparing `ytmusicapi-1.6.0/ytmusicapi/mixins/library.py` & `ytmusicapi-1.7.0/ytmusicapi/mixins/library.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from ytmusicapi.parsers.library import *
 
 from ._protocol import MixinProtocol
 from ._utils import *
 
 
 class LibraryMixin(MixinProtocol):
-    def get_library_playlists(self, limit: int = 25) -> List[Dict]:
+    def get_library_playlists(self, limit: Optional[int] = 25) -> List[Dict]:
         """
         Retrieves the playlists in the user's library.
 
         :param limit: Number of playlists to retrieve. `None` retrieves them all.
         :return: List of owned playlists.
 
         Each item is in the following format::
@@ -436,15 +436,15 @@
         ]
         ACCOUNT_RUNS_TEXT = ["runs", 0, "text"]
         ACCOUNT_NAME = [*ACCOUNT_INFO, "accountName", *ACCOUNT_RUNS_TEXT]
         ACCOUNT_CHANNEL_HANDLE = [*ACCOUNT_INFO, "channelHandle", *ACCOUNT_RUNS_TEXT]
         ACCOUNT_PHOTO_URL = [*ACCOUNT_INFO, "accountPhoto", "thumbnails", 0, "url"]
 
         account_name = nav(response, ACCOUNT_NAME)
-        channel_handle = nav(response, ACCOUNT_CHANNEL_HANDLE)
+        channel_handle = nav(response, ACCOUNT_CHANNEL_HANDLE, none_if_absent=True)
         account_photo_url = nav(response, ACCOUNT_PHOTO_URL)
 
         return {
             "accountName": account_name,
             "channelHandle": channel_handle,
             "accountPhotoUrl": account_photo_url,
         }
```

### Comparing `ytmusicapi-1.6.0/ytmusicapi/mixins/playlists.py` & `ytmusicapi-1.7.0/ytmusicapi/mixins/playlists.py`

 * *Files 18% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 from ._protocol import MixinProtocol
 from ._utils import *
 
 
 class PlaylistsMixin(MixinProtocol):
     def get_playlist(
-        self, playlistId: str, limit: int = 100, related: bool = False, suggestions_limit: int = 0
+        self, playlistId: str, limit: Optional[int] = 100, related: bool = False, suggestions_limit: int = 0
     ) -> Dict:
         """
         Returns a list of playlist items
 
         :param playlistId: Playlist id
         :param limit: How many songs to return. `None` retrieves them all. Default: 100
         :param related: Whether to fetch 10 related playlists or not. Default: False
@@ -102,29 +102,33 @@
         The setVideoId is the unique id of this playlist item and
         needed for moving/removing playlist items
         """
         browseId = "VL" + playlistId if not playlistId.startswith("VL") else playlistId
         body = {"browseId": browseId}
         endpoint = "browse"
         response = self._send_request(endpoint, body)
-        results = nav(response, SINGLE_COLUMN_TAB + SECTION_LIST_ITEM + ["musicPlaylistShelfRenderer"])
+        results = nav(response, SINGLE_COLUMN_TAB + SECTION_LIST_ITEM + ["musicPlaylistShelfRenderer"], True)
+        if not results:
+            return self._parse_new_playlist_format(
+                response, endpoint, body, suggestions_limit, related, limit
+            )
+
         playlist = {"id": results["playlistId"]}
         playlist.update(parse_playlist_header(response))
         if playlist["trackCount"] is None:
             playlist["trackCount"] = len(results["contents"])
 
         request_func = lambda additionalParams: self._send_request(endpoint, body, additionalParams)
 
         # suggestions and related are missing e.g. on liked songs
         section_list = nav(response, [*SINGLE_COLUMN_TAB, "sectionListRenderer"])
         playlist["related"] = []
         if "continuations" in section_list:
             additionalParams = get_continuation_params(section_list)
-            own_playlist = "musicEditablePlaylistDetailHeaderRenderer" in response["header"]
-            if own_playlist and (suggestions_limit > 0 or related):
+            if playlist["owned"] and (suggestions_limit > 0 or related):
                 parse_func = lambda results: parse_playlist_items(results)
                 suggested = request_func(additionalParams)
                 continuation = nav(suggested, SECTION_LIST_CONTINUATION)
                 additionalParams = get_continuation_params(continuation)
                 suggestions_shelf = nav(continuation, CONTENT + MUSIC_SHELF)
                 playlist["suggestions"] = get_continuation_contents(suggestions_shelf, parse_func)
 
@@ -160,14 +164,115 @@
                         results, "musicPlaylistShelfContinuation", limit, request_func, parse_func
                     )
                 )
 
         playlist["duration_seconds"] = sum_total_duration(playlist)
         return playlist
 
+    def _parse_new_playlist_format(
+        self, response: Dict, endpoint, body, suggestions_limit, related, limit
+    ) -> Dict:  # pragma: no cover
+        """temporary function to avoid too many ifs in get_playlist during a/b test"""
+
+        header_data = nav(response, [*TWO_COLUMN_RENDERER, *TAB_CONTENT, *SECTION_LIST_ITEM])
+        section_list = nav(response, [*TWO_COLUMN_RENDERER, "secondaryContents", *SECTION])
+        playlist: Dict = {}
+        playlist["owned"] = EDITABLE_PLAYLIST_DETAIL_HEADER[0] in header_data
+        if not playlist["owned"]:
+            header = nav(header_data, RESPONSIVE_HEADER)
+            playlist["id"] = nav(
+                header,
+                ["buttons", 1, "musicPlayButtonRenderer", "playNavigationEndpoint", *WATCH_PLAYLIST_ID],
+                True,
+            )
+            playlist["privacy"] = "PUBLIC"
+        else:
+            playlist["id"] = nav(header_data, [*EDITABLE_PLAYLIST_DETAIL_HEADER, *PLAYLIST_ID])
+            header = nav(header_data, [*EDITABLE_PLAYLIST_DETAIL_HEADER, *HEADER, *RESPONSIVE_HEADER])
+            playlist["privacy"] = header_data[EDITABLE_PLAYLIST_DETAIL_HEADER[0]]["editHeader"][
+                "musicPlaylistEditHeaderRenderer"
+            ]["privacy"]
+
+        description_shelf = nav(header, ["description", *DESCRIPTION_SHELF], True)
+        playlist["description"] = (
+            "".join([run["text"] for run in description_shelf["description"]["runs"]])
+            if description_shelf
+            else None
+        )
+        playlist["title"] = nav(header, TITLE_TEXT)
+        playlist.update(parse_song_runs(nav(header, SUBTITLE_RUNS)[2 + playlist["owned"] * 2 :]))
+
+        playlist["views"] = None
+        playlist["duration"] = None
+        if "runs" in header["secondSubtitle"]:
+            second_subtitle_runs = header["secondSubtitle"]["runs"]
+            has_views = (len(second_subtitle_runs) > 3) * 2
+            playlist["views"] = None if not has_views else to_int(second_subtitle_runs[0]["text"])
+            has_duration = (len(second_subtitle_runs) > 1) * 2
+            playlist["duration"] = (
+                None if not has_duration else second_subtitle_runs[has_views + has_duration]["text"]
+            )
+            song_count = second_subtitle_runs[has_views + 0]["text"].split(" ")
+            song_count = to_int(song_count[0]) if len(song_count) > 1 else 0
+        else:
+            song_count = len(section_list["contents"])
+
+        playlist["trackCount"] = song_count
+
+        request_func = lambda additionalParams: self._send_request(endpoint, body, additionalParams)
+
+        # suggestions and related are missing e.g. on liked songs
+        playlist["related"] = []
+        if "continuations" in section_list:
+            additionalParams = get_continuation_params(section_list)
+            if playlist["owned"] and (suggestions_limit > 0 or related):
+                parse_func = lambda results: parse_playlist_items(results)
+                suggested = request_func(additionalParams)
+                continuation = nav(suggested, SECTION_LIST_CONTINUATION)
+                additionalParams = get_continuation_params(continuation)
+                suggestions_shelf = nav(continuation, CONTENT + MUSIC_SHELF)
+                playlist["suggestions"] = get_continuation_contents(suggestions_shelf, parse_func)
+
+                parse_func = lambda results: parse_playlist_items(results)
+                playlist["suggestions"].extend(
+                    get_continuations(
+                        suggestions_shelf,
+                        "musicShelfContinuation",
+                        suggestions_limit - len(playlist["suggestions"]),
+                        request_func,
+                        parse_func,
+                        reloadable=True,
+                    )
+                )
+
+            if related:
+                response = request_func(additionalParams)
+                continuation = nav(response, SECTION_LIST_CONTINUATION, True)
+                if continuation:
+                    parse_func = lambda results: parse_content_list(results, parse_playlist)
+                    playlist["related"] = get_continuation_contents(
+                        nav(continuation, CONTENT + CAROUSEL), parse_func
+                    )
+
+        playlist["tracks"] = []
+        content_data = nav(section_list, [*CONTENT, "musicPlaylistShelfRenderer"])
+        if "contents" in content_data:
+            playlist["tracks"] = parse_playlist_items(content_data["contents"])
+
+            parse_func = lambda contents: parse_playlist_items(contents)
+            if "continuations" in content_data:
+                playlist["tracks"].extend(
+                    get_continuations(
+                        content_data, "musicPlaylistShelfContinuation", limit, request_func, parse_func
+                    )
+                )
+
+        playlist["duration_seconds"] = sum_total_duration(playlist)
+        return playlist
+
     def get_liked_songs(self, limit: int = 100) -> Dict:
         """
         Gets playlist items for the 'Liked Songs' playlist
 
         :param limit: How many items to return. Default: 100
         :return: List of playlistItem dictionaries. See :py:func:`get_playlist`
         """
```

### Comparing `ytmusicapi-1.6.0/ytmusicapi/mixins/podcasts.py` & `ytmusicapi-1.7.0/ytmusicapi/mixins/podcasts.py`

 * *Files 0% similar despite different names*

```diff
@@ -168,15 +168,15 @@
            To save an episode, you need to call `add_playlist_items` to add
            it to the `SE` (saved episodes) playlist.
 
         :param videoId: browseId (MPED..) or videoId for a single episode
         :return: Dict containing information about the episode
 
         The description elements are based on a custom dataclass, not shown in the example below
-        The description text items also contain "\n" to indicate newlines, removed below due to RST issues
+        The description text items also contain "\\n" to indicate newlines, removed below due to RST issues
 
         Example::
 
             {
                 "author":
                 {
                     "name": "Stanford GSB Podcasts",
```

### Comparing `ytmusicapi-1.6.0/ytmusicapi/mixins/search.py` & `ytmusicapi-1.7.0/ytmusicapi/mixins/search.py`

 * *Files identical despite different names*

### Comparing `ytmusicapi-1.6.0/ytmusicapi/mixins/uploads.py` & `ytmusicapi-1.7.0/ytmusicapi/mixins/uploads.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 
 from ..auth.types import AuthType
 from ._protocol import MixinProtocol
 from ._utils import prepare_order_params, validate_order_parameter
 
 
 class UploadsMixin(MixinProtocol):
-    def get_library_upload_songs(self, limit: int = 25, order: Optional[str] = None) -> List[Dict]:
+    def get_library_upload_songs(self, limit: Optional[int] = 25, order: Optional[str] = None) -> List[Dict]:
         """
         Returns a list of uploaded songs
 
         :param limit: How many songs to return. `None` retrieves them all. Default: 25
         :param order: Order of songs to return. Allowed values: 'a_to_z', 'z_to_a', 'recently_added'. Default: Default order.
         :return: List of uploaded songs.
 
@@ -65,15 +65,15 @@
                 get_continuations(
                     results, "musicShelfContinuation", remaining_limit, request_func, parse_uploaded_items
                 )
             )
 
         return songs
 
-    def get_library_upload_albums(self, limit: int = 25, order: Optional[str] = None) -> List[Dict]:
+    def get_library_upload_albums(self, limit: Optional[int] = 25, order: Optional[str] = None) -> List[Dict]:
         """
         Gets the albums of uploaded songs in the user's library.
 
         :param limit: Number of albums to return. `None` retrives them all. Default: 25
         :param order: Order of albums to return. Allowed values: 'a_to_z', 'z_to_a', 'recently_added'. Default: Default order.
         :return: List of albums as returned by :py:func:`get_library_albums`
         """
@@ -84,15 +84,17 @@
             body["params"] = prepare_order_params(order)
         endpoint = "browse"
         response = self._send_request(endpoint, body)
         return parse_library_albums(
             response, lambda additionalParams: self._send_request(endpoint, body, additionalParams), limit
         )
 
-    def get_library_upload_artists(self, limit: int = 25, order: Optional[str] = None) -> List[Dict]:
+    def get_library_upload_artists(
+        self, limit: Optional[int] = 25, order: Optional[str] = None
+    ) -> List[Dict]:
         """
         Gets the artists of uploaded songs in the user's library.
 
         :param limit: Number of artists to return. `None` retrieves them all. Default: 25
         :param order: Order of artists to return. Allowed values: 'a_to_z', 'z_to_a', 'recently_added'. Default: Default order.
         :return: List of artists as returned by :py:func:`get_library_artists`
         """
@@ -215,17 +217,15 @@
         if os.path.splitext(filepath)[1][1:] not in supported_filetypes:
             raise Exception(
                 "The provided file type is not supported by YouTube Music. Supported file types are "
                 + ", ".join(supported_filetypes)
             )
 
         headers = self.headers.copy()
-        upload_url = (
-            "https://upload.youtube.com/upload/usermusic/http?authuser=%s" % headers["x-goog-authuser"]
-        )
+        upload_url = f"https://upload.youtube.com/upload/usermusic/http?authuser={headers['x-goog-authuser']}"
         filesize = os.path.getsize(filepath)
         body = ("filename=" + ntpath.basename(filepath)).encode("utf-8")
         headers.pop("content-encoding", None)
         headers["content-type"] = "application/x-www-form-urlencoded;charset=utf-8"
         headers["X-Goog-Upload-Command"] = "start"
         headers["X-Goog-Upload-Header-Content-Length"] = str(filesize)
         headers["X-Goog-Upload-Protocol"] = "resumable"
```

### Comparing `ytmusicapi-1.6.0/ytmusicapi/mixins/watch.py` & `ytmusicapi-1.7.0/ytmusicapi/mixins/watch.py`

 * *Files identical despite different names*

### Comparing `ytmusicapi-1.6.0/ytmusicapi/navigation.py` & `ytmusicapi-1.7.0/ytmusicapi/navigation.py`

 * *Files 14% similar despite different names*

```diff
@@ -24,18 +24,20 @@
 TOGGLE_MENU = "toggleMenuServiceItemRenderer"
 OVERLAY_RENDERER = ["musicItemThumbnailOverlayRenderer", "content", "musicPlayButtonRenderer"]
 PLAY_BUTTON = ["overlay", *OVERLAY_RENDERER]
 NAVIGATION_BROWSE = ["navigationEndpoint", "browseEndpoint"]
 NAVIGATION_BROWSE_ID = [*NAVIGATION_BROWSE, "browseId"]
 PAGE_TYPE = ["browseEndpointContextSupportedConfigs", "browseEndpointContextMusicConfig", "pageType"]
 WATCH_VIDEO_ID = ["watchEndpoint", "videoId"]
+PLAYLIST_ID = ["playlistId"]
+WATCH_PLAYLIST_ID = ["watchEndpoint", *PLAYLIST_ID]
 NAVIGATION_VIDEO_ID = ["navigationEndpoint", *WATCH_VIDEO_ID]
 QUEUE_VIDEO_ID = ["queueAddEndpoint", "queueTarget", "videoId"]
-NAVIGATION_PLAYLIST_ID = ["navigationEndpoint", "watchEndpoint", "playlistId"]
-WATCH_PID = ["watchPlaylistEndpoint", "playlistId"]
+NAVIGATION_PLAYLIST_ID = ["navigationEndpoint", *WATCH_PLAYLIST_ID]
+WATCH_PID = ["watchPlaylistEndpoint", *PLAYLIST_ID]
 NAVIGATION_WATCH_PLAYLIST_ID = ["navigationEndpoint", *WATCH_PID]
 NAVIGATION_VIDEO_TYPE = [
     "watchEndpoint",
     "watchEndpointMusicSupportedConfigs",
     "watchEndpointMusicConfig",
     "musicVideoType",
 ]
@@ -67,24 +69,27 @@
 MTRIR = "musicTwoRowItemRenderer"
 MNIR = "menuNavigationItemRenderer"
 TASTE_PROFILE_ITEMS = ["contents", "tastebuilderRenderer", "contents"]
 TASTE_PROFILE_ARTIST = ["title", "runs"]
 SECTION_LIST_CONTINUATION = ["continuationContents", "sectionListContinuation"]
 MENU_PLAYLIST_ID = [*MENU_ITEMS, 0, MNIR, *NAVIGATION_WATCH_PLAYLIST_ID]
 MULTI_SELECT = ["musicMultiSelectMenuItemRenderer"]
-HEADER_DETAIL = ["header", "musicDetailHeaderRenderer"]
-HEADER_SIDE = ["header", "musicSideAlignedItemRenderer"]
-HEADER_MUSIC_VISUAL = ["header", "musicVisualHeaderRenderer"]
+HEADER = ["header"]
+HEADER_DETAIL = [*HEADER, "musicDetailHeaderRenderer"]
+EDITABLE_PLAYLIST_DETAIL_HEADER = ["musicEditablePlaylistDetailHeaderRenderer"]
+HEADER_EDITABLE_DETAIL = [*HEADER, *EDITABLE_PLAYLIST_DETAIL_HEADER]
+HEADER_SIDE = [*HEADER, "musicSideAlignedItemRenderer"]
+HEADER_MUSIC_VISUAL = [*HEADER, "musicVisualHeaderRenderer"]
 DESCRIPTION_SHELF = ["musicDescriptionShelfRenderer"]
 DESCRIPTION = ["description", *RUN_TEXT]
 CAROUSEL = ["musicCarouselShelfRenderer"]
 IMMERSIVE_CAROUSEL = ["musicImmersiveCarouselShelfRenderer"]
 CAROUSEL_CONTENTS = [*CAROUSEL, "contents"]
-CAROUSEL_TITLE = ["header", "musicCarouselShelfBasicHeaderRenderer", *TITLE]
-CARD_SHELF_TITLE = ["header", "musicCardShelfHeaderBasicRenderer", *TITLE_TEXT]
+CAROUSEL_TITLE = [*HEADER, "musicCarouselShelfBasicHeaderRenderer", *TITLE]
+CARD_SHELF_TITLE = [*HEADER, "musicCardShelfHeaderBasicRenderer", *TITLE_TEXT]
 FRAMEWORK_MUTATIONS = ["frameworkUpdates", "entityBatchUpdate", "mutations"]
 
 
 @overload
 def nav(root: Dict[str, Any], items: List[Any], none_if_absent: Literal[False] = False) -> Any:
     """overload for mypy only"""
```

### Comparing `ytmusicapi-1.6.0/ytmusicapi/parsers/_utils.py` & `ytmusicapi-1.7.0/ytmusicapi/parsers/_utils.py`

 * *Files identical despite different names*

### Comparing `ytmusicapi-1.6.0/ytmusicapi/parsers/browsing.py` & `ytmusicapi-1.7.0/ytmusicapi/parsers/browsing.py`

 * *Files identical despite different names*

### Comparing `ytmusicapi-1.6.0/ytmusicapi/parsers/explore.py` & `ytmusicapi-1.7.0/ytmusicapi/parsers/explore.py`

 * *Files identical despite different names*

### Comparing `ytmusicapi-1.6.0/ytmusicapi/parsers/i18n.py` & `ytmusicapi-1.7.0/ytmusicapi/parsers/i18n.py`

 * *Files 3% similar despite different names*

```diff
@@ -41,27 +41,28 @@
 
     @i18n
     def parse_channel_contents(self, results: List) -> Dict:
         # type: ignore[name-defined]
         categories = [
             ("albums", _("albums"), parse_album, MTRIR),
             ("singles", _("singles"), parse_single, MTRIR),
+            ("shows", _("shows"), parse_album, MTRIR),
             ("videos", _("videos"), parse_video, MTRIR),
             ("playlists", _("playlists"), parse_playlist, MTRIR),
             ("related", _("related"), parse_related_artist, MTRIR),
             ("episodes", _("episodes"), parse_episode, MMRIR),
             ("podcasts", _("podcasts"), parse_podcast, MTRIR),
         ]
         artist: Dict[str, Any] = {}
         for category, category_local, category_parser, category_key in categories:
             data = [
                 r["musicCarouselShelfRenderer"]
                 for r in results
                 if "musicCarouselShelfRenderer" in r
-                and nav(r, CAROUSEL + CAROUSEL_TITLE)["text"].lower() == category_local
+                and nav(r, CAROUSEL + CAROUSEL_TITLE)["text"].lower() == category_local.lower()
             ]
             if len(data) > 0:
                 artist[category] = {"browseId": None, "results": []}
                 if "navigationEndpoint" in nav(data[0], CAROUSEL_TITLE):
                     artist[category]["browseId"] = nav(data[0], CAROUSEL_TITLE + NAVIGATION_BROWSE_ID)
                     artist[category]["params"] = nav(
                         data[0], CAROUSEL_TITLE + NAVIGATION_BROWSE + ["params"], True
```

### Comparing `ytmusicapi-1.6.0/ytmusicapi/parsers/library.py` & `ytmusicapi-1.7.0/ytmusicapi/parsers/library.py`

 * *Files 6% similar despite different names*

```diff
@@ -10,14 +10,19 @@
 def parse_artists(results, uploaded=False):
     artists = []
     for result in results:
         data = result[MRLIR]
         artist = {}
         artist["browseId"] = nav(data, NAVIGATION_BROWSE_ID)
         artist["artist"] = get_item_text(data, 0)
+        page_type = nav(data, NAVIGATION_BROWSE + PAGE_TYPE, True)
+        if page_type == "MUSIC_PAGE_TYPE_USER_CHANNEL":
+            artist["type"] = "channel"
+        elif page_type == "MUSIC_PAGE_TYPE_ARTIST":
+            artist["type"] = "artist"
         parse_menu_playlists(data, artist)
         if uploaded:
             artist["songs"] = get_item_text(data, 1).split(" ")[0]
         else:
             subtitle = get_item_text(data, 1)
             if subtitle:
                 artist["subscribers"] = subtitle.split(" ")[0]
```

### Comparing `ytmusicapi-1.6.0/ytmusicapi/parsers/playlists.py` & `ytmusicapi-1.7.0/ytmusicapi/parsers/playlists.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,23 +2,22 @@
 
 from ..helpers import to_int
 from .songs import *
 
 
 def parse_playlist_header(response: Dict) -> Dict[str, Any]:
     playlist: Dict[str, Any] = {}
-    own_playlist = "musicEditablePlaylistDetailHeaderRenderer" in response["header"]
-    if not own_playlist:
-        header = response["header"]["musicDetailHeaderRenderer"]
-        playlist["privacy"] = "PUBLIC"
+    editable_header = nav(response, [*HEADER, *EDITABLE_PLAYLIST_DETAIL_HEADER], True)
+    playlist["owned"] = editable_header is not None
+    playlist["privacy"] = "PUBLIC"
+    if editable_header is not None:  # owned playlist
+        header = nav(editable_header, HEADER_DETAIL)
+        playlist["privacy"] = editable_header["editHeader"]["musicPlaylistEditHeaderRenderer"]["privacy"]
     else:
-        header = response["header"]["musicEditablePlaylistDetailHeaderRenderer"]
-        playlist["privacy"] = header["editHeader"]["musicPlaylistEditHeaderRenderer"]["privacy"]
-        header = header["header"]["musicDetailHeaderRenderer"]
-    playlist["owned"] = own_playlist
+        header = nav(response, HEADER_DETAIL, True)
 
     playlist["title"] = nav(header, TITLE_TEXT)
     playlist["thumbnails"] = nav(header, THUMBNAIL_CROPPED)
     playlist["description"] = nav(header, DESCRIPTION, True)
     run_count = len(nav(header, SUBTITLE_RUNS))
     if run_count > 1:
         playlist["author"] = {
```

### Comparing `ytmusicapi-1.6.0/ytmusicapi/parsers/podcasts.py` & `ytmusicapi-1.7.0/ytmusicapi/parsers/podcasts.py`

 * *Files 1% similar despite different names*

```diff
@@ -54,36 +54,36 @@
                 element = DescriptionElement(text=nav(run, ["text"], True))  # type: ignore
 
             elements.append(element)
 
         return cls(elements)
 
 
-def _parse_base_header(header: Dict) -> Dict:
+def parse_base_header(header: Dict) -> Dict:
     """parse common left hand side (header) items of an episode or podcast page"""
     strapline = nav(header, ["straplineTextOne"])
     return {
         "author": {
             "name": nav(strapline, [*RUN_TEXT]),
             "id": nav(strapline, ["runs", 0, *NAVIGATION_BROWSE_ID]),
         },
         "title": nav(header, TITLE_TEXT),
     }
 
 
 def parse_podcast_header(header: Dict) -> Dict:
-    metadata = _parse_base_header(header)
+    metadata = parse_base_header(header)
     metadata["description"] = nav(header, ["description", *DESCRIPTION_SHELF, *DESCRIPTION], True)
     metadata["saved"] = nav(header, ["buttons", 1, *TOGGLED_BUTTON])
 
     return metadata
 
 
 def parse_episode_header(header: Dict) -> Dict:
-    metadata = _parse_base_header(header)
+    metadata = parse_base_header(header)
     metadata["date"] = nav(header, [*SUBTITLE2])
     metadata["duration"] = nav(header, [*SUBTITLE3], True)
     if not metadata["duration"]:  # progress started
         progress_renderer = nav(header, ["progress", "musicPlaybackProgressRenderer"])
         metadata["duration"] = nav(progress_renderer, ["durationText", "runs", 1, "text"], True)
         metadata["progressPercentage"] = nav(progress_renderer, ["playbackProgressPercentage"])
     metadata["saved"] = nav(header, ["buttons", 0, *TOGGLED_BUTTON], True) or False
```

### Comparing `ytmusicapi-1.6.0/ytmusicapi/parsers/search.py` & `ytmusicapi-1.7.0/ytmusicapi/parsers/search.py`

 * *Files identical despite different names*

### Comparing `ytmusicapi-1.6.0/ytmusicapi/parsers/songs.py` & `ytmusicapi-1.7.0/ytmusicapi/parsers/songs.py`

 * *Files identical despite different names*

### Comparing `ytmusicapi-1.6.0/ytmusicapi/parsers/uploads.py` & `ytmusicapi-1.7.0/ytmusicapi/parsers/uploads.py`

 * *Files identical despite different names*

### Comparing `ytmusicapi-1.6.0/ytmusicapi/parsers/watch.py` & `ytmusicapi-1.7.0/ytmusicapi/parsers/watch.py`

 * *Files identical despite different names*

### Comparing `ytmusicapi-1.6.0/ytmusicapi/setup.py` & `ytmusicapi-1.7.0/ytmusicapi/setup.py`

 * *Files identical despite different names*

### Comparing `ytmusicapi-1.6.0/ytmusicapi/ytmusic.py` & `ytmusicapi-1.7.0/ytmusicapi/ytmusic.py`

 * *Files identical despite different names*

### Comparing `ytmusicapi-1.6.0/ytmusicapi.egg-info/PKG-INFO` & `ytmusicapi-1.7.0/ytmusicapi.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ytmusicapi
-Version: 1.6.0
+Version: 1.7.0
 Summary: Unofficial API for YouTube Music
 Author-email: sigma67 <ytmusicapi@gmail.com>
 License: MIT License
         
         Copyright (c) 2024 sigma67
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -34,35 +34,37 @@
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 Requires-Dist: requests>=2.22
 
 ytmusicapi: Unofficial API for YouTube Music
 ############################################
 
-.. image:: https://img.shields.io/pypi/dm/ytmusicapi?style=flat-square
+.. |pypi-downloads| image:: https://img.shields.io/pypi/dm/ytmusicapi?style=flat-square
     :alt: PyPI Downloads
     :target: https://pypi.org/project/ytmusicapi/
 
-.. image:: https://badges.gitter.im/sigma67/ytmusicapi.svg
+.. |gitter| image:: https://badges.gitter.im/sigma67/ytmusicapi.svg
    :alt: Ask questions at https://gitter.im/sigma67/ytmusicapi
    :target: https://gitter.im/sigma67/ytmusicapi
 
-.. image:: https://img.shields.io/codecov/c/github/sigma67/ytmusicapi?style=flat-square
+.. |code-coverage| image:: https://img.shields.io/codecov/c/github/sigma67/ytmusicapi?style=flat-square
     :alt: Code coverage
     :target: https://codecov.io/gh/sigma67/ytmusicapi
 
-.. image:: https://img.shields.io/github/v/release/sigma67/ytmusicapi?style=flat-square
+.. |latest-release| image:: https://img.shields.io/github/v/release/sigma67/ytmusicapi?style=flat-square
     :alt: Latest release
     :target: https://github.com/sigma67/ytmusicapi/releases/latest
 
-.. image:: https://img.shields.io/github/commits-since/sigma67/ytmusicapi/latest?style=flat-square
+.. |commits-since-latest| image:: https://img.shields.io/github/commits-since/sigma67/ytmusicapi/latest?style=flat-square
     :alt: Commits since latest release
     :target: https://github.com/sigma67/ytmusicapi/commits
 
 
+|pypi-downloads| |gitter| |code-coverage| |latest-release| |commits-since-latest|
+
 ytmusicapi is a Python 3 library to send requests to the YouTube Music API.
 It emulates YouTube Music web client requests using the user's cookie data for authentication.
 
 .. features
 
 Features
 --------
```

### Comparing `ytmusicapi-1.6.0/ytmusicapi.egg-info/SOURCES.txt` & `ytmusicapi-1.7.0/ytmusicapi.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -30,14 +30,17 @@
 tests/__init__.py
 tests/conftest.py
 tests/test.example.cfg
 tests/test_ytmusic.py
 tests/auth/__init__.py
 tests/auth/test_browser.py
 tests/auth/test_oauth.py
+tests/data/2024_03_get_album.json
+tests/data/2024_03_get_playlist.json
+tests/data/2024_03_get_playlist_public.json
 tests/mixins/__init__.py
 tests/mixins/test_browsing.py
 tests/mixins/test_explore.py
 tests/mixins/test_library.py
 tests/mixins/test_playlists.py
 tests/mixins/test_podcasts.py
 tests/mixins/test_search.py
```

