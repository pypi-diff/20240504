# Comparing `tmp/wordc-0.1.2.tar.gz` & `tmp/wordc-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wordc-0.1.2.tar", last modified: Mon Apr 29 19:40:40 2024, max compression
+gzip compressed data, was "wordc-1.0.0.tar", last modified: Sat May  4 15:16:07 2024, max compression
```

## Comparing `wordc-0.1.2.tar` & `wordc-1.0.0.tar`

### file list

```diff
@@ -1,30 +1,39 @@
-drwxrwxrwx   0        0        0        0 2024-04-29 19:40:40.755602 wordc-0.1.2/
--rw-rw-rw-   0        0        0      161 2024-04-29 17:50:18.000000 wordc-0.1.2/AUTHORS.md
--rw-rw-rw-   0        0        0      105 2024-04-27 12:45:04.000000 wordc-0.1.2/CHANGELOG.md
--rw-rw-rw-   0        0        0     1095 2024-04-27 12:45:04.000000 wordc-0.1.2/LICENSE
--rw-rw-rw-   0        0        0      237 2024-04-27 12:45:04.000000 wordc-0.1.2/MANIFEST.in
--rw-rw-rw-   0        0        0     6687 2024-04-29 19:40:40.754600 wordc-0.1.2/PKG-INFO
--rw-rw-rw-   0        0        0     5063 2024-04-29 18:43:35.000000 wordc-0.1.2/README.md
--rw-rw-rw-   0        0        0     2175 2024-04-27 12:45:04.000000 wordc-0.1.2/pyproject.toml
--rw-rw-rw-   0        0        0     1985 2024-04-29 19:40:40.759610 wordc-0.1.2/setup.cfg
--rw-rw-rw-   0        0        0      117 2024-04-27 12:45:05.000000 wordc-0.1.2/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-29 19:40:40.691108 wordc-0.1.2/src/
-drwxrwxrwx   0        0        0        0 2024-04-29 19:40:40.718599 wordc-0.1.2/src/wordc/
--rw-rw-rw-   0        0        0      321 2024-04-29 19:17:50.000000 wordc-0.1.2/src/wordc/__init__.py
--rw-rw-rw-   0        0        0       50 2024-04-28 10:02:57.000000 wordc-0.1.2/src/wordc/__main__.py
--rw-rw-rw-   0        0        0     1513 2024-04-29 17:50:02.000000 wordc-0.1.2/src/wordc/cli.py
--rw-rw-rw-   0        0        0      273 2024-04-29 17:50:02.000000 wordc-0.1.2/src/wordc/config.py
--rw-rw-rw-   0        0        0      975 2024-04-28 11:51:31.000000 wordc-0.1.2/src/wordc/exceptions.py
--rw-rw-rw-   0        0        0     1488 2024-04-29 18:01:07.000000 wordc-0.1.2/src/wordc/utils.py
--rw-rw-rw-   0        0        0     2820 2024-04-29 18:43:32.000000 wordc-0.1.2/src/wordc/wordc.py
-drwxrwxrwx   0        0        0        0 2024-04-29 19:40:40.752613 wordc-0.1.2/src/wordc.egg-info/
--rw-rw-rw-   0        0        0     6687 2024-04-29 19:40:40.000000 wordc-0.1.2/src/wordc.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      513 2024-04-29 19:40:40.000000 wordc-0.1.2/src/wordc.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-29 19:40:40.000000 wordc-0.1.2/src/wordc.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       43 2024-04-29 19:40:40.000000 wordc-0.1.2/src/wordc.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       29 2024-04-29 19:40:40.000000 wordc-0.1.2/src/wordc.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2024-04-29 19:40:40.000000 wordc-0.1.2/src/wordc.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-04-29 19:40:40.749604 wordc-0.1.2/tests/
--rw-rw-rw-   0        0        0     1339 2024-04-29 15:47:17.000000 wordc-0.1.2/tests/test_args.py
--rw-rw-rw-   0        0        0      235 2024-04-29 16:02:44.000000 wordc-0.1.2/tests/test_process_contents.py
--rw-rw-rw-   0        0        0      255 2024-04-29 16:44:43.000000 wordc-0.1.2/tests/test_read_file_contents.py
+drwxrwxrwx   0        0        0        0 2024-05-04 15:16:07.382231 wordc-1.0.0/
+-rw-rw-rw-   0        0        0      161 2024-04-29 17:50:18.000000 wordc-1.0.0/AUTHORS.md
+-rw-rw-rw-   0        0        0      105 2024-04-27 12:45:04.000000 wordc-1.0.0/CHANGELOG.md
+-rw-rw-rw-   0        0        0     1095 2024-04-27 12:45:04.000000 wordc-1.0.0/LICENSE
+-rw-rw-rw-   0        0        0      237 2024-04-27 12:45:04.000000 wordc-1.0.0/MANIFEST.in
+-rw-rw-rw-   0        0        0     7893 2024-05-04 15:16:07.382231 wordc-1.0.0/PKG-INFO
+-rw-rw-rw-   0        0        0     6216 2024-04-29 20:03:48.000000 wordc-1.0.0/README.md
+-rw-rw-rw-   0        0        0     2175 2024-04-27 12:45:04.000000 wordc-1.0.0/pyproject.toml
+-rw-rw-rw-   0        0        0     1985 2024-05-04 15:16:07.392006 wordc-1.0.0/setup.cfg
+-rw-rw-rw-   0        0        0      117 2024-04-27 12:45:05.000000 wordc-1.0.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-04 15:16:07.289325 wordc-1.0.0/src/
+drwxrwxrwx   0        0        0        0 2024-05-04 15:16:07.329107 wordc-1.0.0/src/wordc/
+-rw-rw-rw-   0        0        0      322 2024-05-04 15:12:03.000000 wordc-1.0.0/src/wordc/__init__.py
+-rw-rw-rw-   0        0        0       50 2024-04-28 10:02:57.000000 wordc-1.0.0/src/wordc/__main__.py
+-rw-rw-rw-   0        0        0     1588 2024-05-04 14:54:18.000000 wordc-1.0.0/src/wordc/cli.py
+-rw-rw-rw-   0        0        0      635 2024-05-04 14:55:37.000000 wordc-1.0.0/src/wordc/config.py
+-rw-rw-rw-   0        0        0      975 2024-04-28 11:51:31.000000 wordc-1.0.0/src/wordc/exceptions.py
+-rw-rw-rw-   0        0        0     1614 2024-05-04 14:55:37.000000 wordc-1.0.0/src/wordc/utils.py
+-rw-rw-rw-   0        0        0     3068 2024-05-04 14:52:28.000000 wordc-1.0.0/src/wordc/wordc.py
+drwxrwxrwx   0        0        0        0 2024-05-04 15:16:07.381137 wordc-1.0.0/src/wordc.egg-info/
+-rw-rw-rw-   0        0        0     7893 2024-05-04 15:16:07.000000 wordc-1.0.0/src/wordc.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      833 2024-05-04 15:16:07.000000 wordc-1.0.0/src/wordc.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-04 15:16:07.000000 wordc-1.0.0/src/wordc.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       43 2024-05-04 15:16:07.000000 wordc-1.0.0/src/wordc.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       29 2024-05-04 15:16:07.000000 wordc-1.0.0/src/wordc.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2024-05-04 15:16:07.000000 wordc-1.0.0/src/wordc.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-04 15:16:07.379056 wordc-1.0.0/tests/
+-rw-rw-rw-   0        0        0     1333 2024-05-04 14:21:07.000000 wordc-1.0.0/tests/test_args.py
+-rw-rw-rw-   0        0        0      531 2024-05-03 13:46:58.000000 wordc-1.0.0/tests/test_integration_01_nominal.py
+-rw-rw-rw-   0        0        0      531 2024-05-03 13:46:58.000000 wordc-1.0.0/tests/test_integration_02_At_Ac.py
+-rw-rw-rw-   0        0        0      402 2024-05-03 14:03:31.000000 wordc-1.0.0/tests/test_integration_03_ne.py
+-rw-rw-rw-   0        0        0      394 2024-05-03 17:10:25.000000 wordc-1.0.0/tests/test_integration_04_dir.py
+-rw-rw-rw-   0        0        0      395 2024-05-03 17:12:51.000000 wordc-1.0.0/tests/test_integration_05_bin.py
+-rw-rw-rw-   0        0        0      235 2024-04-29 16:02:44.000000 wordc-1.0.0/tests/test_main_process_contents.py
+-rw-rw-rw-   0        0        0      279 2024-04-29 16:50:37.000000 wordc-1.0.0/tests/test_main_read_file_chunks.py
+-rw-rw-rw-   0        0        0      260 2024-05-03 16:52:56.000000 wordc-1.0.0/tests/test_main_read_file_contents.py
+-rw-rw-rw-   0        0        0      242 2024-05-04 14:30:37.000000 wordc-1.0.0/tests/test_utils_detect_encoding.py
+-rw-rw-rw-   0        0        0      716 2024-05-04 12:10:00.000000 wordc-1.0.0/tests/test_utils_determine_chunking.py
+-rw-rw-rw-   0        0        0      369 2024-05-04 11:45:31.000000 wordc-1.0.0/tests/test_utils_isbinary.py
```

### Comparing `wordc-0.1.2/LICENSE` & `wordc-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `wordc-0.1.2/PKG-INFO` & `wordc-1.0.0/README.md`

 * *Files 17% similar despite different names*

```diff
@@ -1,136 +1,153 @@
-Metadata-Version: 2.1
-Name: wordc
-Version: 0.1.2
-Summary: boilerplate you need to create a Python package.
-Home-page: https://github.com/Stephen-RA-King/wordc
-Download-URL: https://github.com/Stephen-RA-King/wordc/archive/refs/heads/main.zip
-Author: Stephen R A King
-Author-email: sking.github@gmail.com
-Maintainer: Stephen R A King
-Maintainer-email: sking.github@gmail.com
-License: MIT
-Project-URL: Bug Tracker, https://github.com/Stephen-RA-King/wordc/issues
-Project-URL: CI, https://github.com/Stephen-RA-King/wordc/actions
-Project-URL: Documentation, https://wordc.readthedocs.io/en/latest/
-Project-URL: Release Notes, https://github.com/Stephen-RA-King/wordc/releases
-Project-URL: Source Code, https://github.com/Stephen-RA-King/wordc/
-Keywords: utility
-Platform: Any
-Classifier: Development Status :: 1 - Planning
-Classifier: Environment :: Console
-Classifier: Intended Audience :: Developers
-Classifier: Operating System :: OS Independent
-Classifier: Natural Language :: English
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.12
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-License-File: LICENSE
-Requires-Dist: chardet>=5.2.0
-Requires-Dist: psutil>=5.9.8
-
-# wordc
-
-> Small utility to analyze the word frequency in a text file
-
-# 🚀 Quickstart
-
----
-
-## 💾 Installation
-
-OS X & Linux:
-
-```sh
-pip3 install wordc
-```
-
-Windows:
-
-```sh
-pip install wordc
-```
-
-# 🔧 Development setup
-
----
-
-```sh
-pip install --editable wordc
-```
-
-# <ℹ️> Meta
-
----
-
-[![](assets/linkedin.png)](https://www.linkedin.com/in/sr-king)
-[![](assets/github.png)](https://github.com/Stephen-RA-King)
-[![](assets/pypi.png)](https://pypi.org/project/wordc)
-[![Docker](assets/docker.png)](https://hub.docker.com/r/sraking/wordc)
-[![](assets/www.png)](https://stephen-ra-king.github.io/justpython/)
-[![](assets/email2.png)](mailto:sking.github@gmail.com)
-[![](assets/github.png)](https://github.com/Stephen-RA-King/wordc)
-
-Author: Stephen R A King ([sking.github@gmail.com](mailto:sking.github@gmail.com))
-
-Created with Cookiecutter template: [![pydough][pydough-image]][pydough-url] version 1.3.4
-
-<!-- Markdown link & img dfn's -->
-
-[bandit-image]: https://img.shields.io/badge/security-bandit-yellow.svg
-[bandit-url]: https://github.com/PyCQA/bandit
-[black-image]: https://img.shields.io/badge/code%20style-black-000000.svg
-[black-url]: https://github.com/psf/black
-[codeclimate-image]: https://api.codeclimate.com/v1/badges/7fc352185512a1dab75d/maintainability
-[codeclimate-url]: https://codeclimate.com/github/Stephen-RA-King/wordc/maintainability
-[codecov-image]: https://codecov.io/gh/Stephen-RA-King/wordc/branch/main/graph/badge.svg
-[codecov-url]: https://app.codecov.io/gh/Stephen-RA-King/wordc
-[codefactor-image]: https://www.codefactor.io/repository/github/Stephen-RA-King/wordc/badge
-[codefactor-url]: https://www.codefactor.io/repository/github/Stephen-RA-King/wordc
-[codeql-image]: https://github.com/Stephen-RA-King/wordc/actions/workflows/github-code-scanning/codeql/badge.svg
-[codeql-url]: https://github.com/Stephen-RA-King/wordc/actions/workflows/github-code-scanning/codeql
-[commitizen-image]: https://img.shields.io/badge/commitizen-friendly-brightgreen.svg
-[commitizen-url]: http://commitizen.github.io/cz-cli/
-[conventional-commits-image]: https://img.shields.io/badge/Conventional%20Commits-1.0.0-yellow.svg?style=flat-square
-[conventional-commits-url]: https://conventionalcommits.org
-[deepsource-image]: https://app.deepsource.com/gh/Stephen-RA-King/wordc.svg/?label=active+issues&show_trend=true
-[deepsource-url]: https://app.deepsource.com/gh/Stephen-RA-King/wordc/?ref=repository-badge
-[docker-image]: https://github.com/Stephen-RA-King/wordc/actions/workflows/docker-image.yml/badge.svg
-[docker-url]: https://github.com/Stephen-RA-King/wordc/actions/workflows/docker-image.yml
-[downloads-image]: https://static.pepy.tech/personalized-badge/wordc?period=total&units=international_system&left_color=black&right_color=orange&left_text=Downloads
-[downloads-url]: https://pepy.tech/project/wordc
-[format-image]: https://img.shields.io/pypi/format/wordc
-[isort-image]: https://img.shields.io/badge/%20imports-isort-%231674b1?style=flat&labelColor=ef8336
-[isort-url]: https://github.com/pycqa/isort/
-[lgtm-alerts-image]: https://img.shields.io/lgtm/alerts/g/Stephen-RA-King/wordc.svg?logo=lgtm&logoWidth=18
-[lgtm-alerts-url]: https://lgtm.com/projects/g/Stephen-RA-King/wordc/alerts/
-[lgtm-quality-image]: https://img.shields.io/lgtm/grade/python/g/Stephen-RA-King/wordc.svg?logo=lgtm&logoWidth=18
-[lgtm-quality-url]: https://lgtm.com/projects/g/Stephen-RA-King/wordc/context:python
-[license-image]: https://img.shields.io/pypi/l/wordc
-[license-url]: https://github.com/Stephen-RA-King/wordc/blob/main/LICENSE
-[mypy-image]: http://www.mypy-lang.org/static/mypy_badge.svg
-[mypy-url]: http://mypy-lang.org/
-[openssf-image]: https://api.securityscorecards.dev/projects/github.com/Stephen-RA-King/wordc/badge
-[openssf-url]: https://api.securityscorecards.dev/projects/github.com/Stephen-RA-King/wordc
-[pre-commit-image]: https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit&logoColor=white
-[pre-commit-url]: https://github.com/pre-commit/pre-commit
-[pre-commit.ci-image]: https://results.pre-commit.ci/badge/github/Stephen-RA-King/wordc/main.svg
-[pre-commit.ci-url]: https://results.pre-commit.ci/latest/github/Stephen-RA-King/wordc/main
-[pydough-image]: https://img.shields.io/badge/pydough-2023-orange?logo=cookiecutter
-[pydough-url]: https://github.com/Stephen-RA-King/pydough
-[pypi-url]: https://pypi.org/project/wordc/
-[pypi-image]: https://img.shields.io/pypi/v/wordc.svg
-[python-version-image]: https://img.shields.io/pypi/pyversions/wordc
-[readthedocs-image]: https://readthedocs.org/projects/wordc/badge/?version=latest
-[readthedocs-url]: https://wordc.readthedocs.io/en/latest/?badge=latest
-[status-image]: https://img.shields.io/pypi/status/wordc.svg
-[tests-image]: https://github.com/Stephen-RA-King/wordc/actions/workflows/tests.yml/badge.svg
-[tests-url]: https://github.com/Stephen-RA-King/wordc/actions/workflows/tests.yml
-[versioning-image]: https://img.shields.io/badge/versioning-semver_2-blue
-[versioning-url]: https://semver.org/
-[wiki]: https://github.com/Stephen-RA-King/wordc/wiki
+# wordc
+
+> Small utility to analyze the word frequency in a text file
+
+# 🚀 Quickstart
+
+---
+
+## 💾 Installation
+
+Using pipx (undoubtedly the best way):
+
+```sh
+pipx install wordc
+```
+
+OS X & Linux:
+
+```sh
+pip3 install wordc
+```
+
+Windows:
+
+```sh
+pip install wordc
+```
+
+# 🔧 Development setup
+
+---
+
+```sh
+pip install --editable wordc
+```
+
+# 📝 Usage
+
+---
+
+Display the help menu with the `-h` argument
+
+```bash
+~ $ wordc -h
+```
+
+```bash
+usage: wordc [-h] [-e ENCODING] [-c] [-s SIZE] [-t TOP_WORDS] [--version] FILENAME
+
+Utility to list the top word frequency in a document
+
+positional arguments:
+  FILENAME              file to analyze for word frequency
+
+optional arguments:
+  -h, --help            show this help message and exit
+  -e ENCODING, --encoding ENCODING
+                        Encoding to use when reading file
+  -c, --chunk           Force file chunking irrespective of file size
+  -s SIZE, --size SIZE  Chunk size to use when reading file
+  -t TOP_WORDS, --top_words TOP_WORDS
+                        Number of top words to list
+  --version             display version number
+```
+
+specify the file
+
+```bash
+~ $ wordc text_file.txt
+4284 the
+2192 and
+2185 of
+1861 a
+1685 to
+```
+
+File chunking will happen automatically in certain situations:
+
+1. When the (file size / availanle memory) ratio is over 25%
+2. When the file size is over 100Mb
+
+File chunking can be forced however by using the `-c` argument.
+
+# <ℹ️> Meta
+
+---
+
+[![](assets/linkedin.png)](https://www.linkedin.com/in/sr-king)
+[![](assets/github.png)](https://github.com/Stephen-RA-King)
+[![](assets/pypi.png)](https://pypi.org/project/wordc)
+[![Docker](assets/docker.png)](https://hub.docker.com/r/sraking/wordc)
+[![](assets/www.png)](https://stephen-ra-king.github.io/justpython/)
+[![](assets/email2.png)](mailto:sking.github@gmail.com)
+[![](assets/github.png)](https://github.com/Stephen-RA-King/wordc)
+
+Author: Stephen R A King ([sking.github@gmail.com](mailto:sking.github@gmail.com))
+
+Created with Cookiecutter template: [![pydough][pydough-image]][pydough-url] version 1.3.4
+
+<!-- Markdown link & img dfn's -->
+
+[bandit-image]: https://img.shields.io/badge/security-bandit-yellow.svg
+[bandit-url]: https://github.com/PyCQA/bandit
+[black-image]: https://img.shields.io/badge/code%20style-black-000000.svg
+[black-url]: https://github.com/psf/black
+[codeclimate-image]: https://api.codeclimate.com/v1/badges/7fc352185512a1dab75d/maintainability
+[codeclimate-url]: https://codeclimate.com/github/Stephen-RA-King/wordc/maintainability
+[codecov-image]: https://codecov.io/gh/Stephen-RA-King/wordc/branch/main/graph/badge.svg
+[codecov-url]: https://app.codecov.io/gh/Stephen-RA-King/wordc
+[codefactor-image]: https://www.codefactor.io/repository/github/Stephen-RA-King/wordc/badge
+[codefactor-url]: https://www.codefactor.io/repository/github/Stephen-RA-King/wordc
+[codeql-image]: https://github.com/Stephen-RA-King/wordc/actions/workflows/github-code-scanning/codeql/badge.svg
+[codeql-url]: https://github.com/Stephen-RA-King/wordc/actions/workflows/github-code-scanning/codeql
+[commitizen-image]: https://img.shields.io/badge/commitizen-friendly-brightgreen.svg
+[commitizen-url]: http://commitizen.github.io/cz-cli/
+[conventional-commits-image]: https://img.shields.io/badge/Conventional%20Commits-1.0.0-yellow.svg?style=flat-square
+[conventional-commits-url]: https://conventionalcommits.org
+[deepsource-image]: https://app.deepsource.com/gh/Stephen-RA-King/wordc.svg/?label=active+issues&show_trend=true
+[deepsource-url]: https://app.deepsource.com/gh/Stephen-RA-King/wordc/?ref=repository-badge
+[docker-image]: https://github.com/Stephen-RA-King/wordc/actions/workflows/docker-image.yml/badge.svg
+[docker-url]: https://github.com/Stephen-RA-King/wordc/actions/workflows/docker-image.yml
+[downloads-image]: https://static.pepy.tech/personalized-badge/wordc?period=total&units=international_system&left_color=black&right_color=orange&left_text=Downloads
+[downloads-url]: https://pepy.tech/project/wordc
+[format-image]: https://img.shields.io/pypi/format/wordc
+[isort-image]: https://img.shields.io/badge/%20imports-isort-%231674b1?style=flat&labelColor=ef8336
+[isort-url]: https://github.com/pycqa/isort/
+[lgtm-alerts-image]: https://img.shields.io/lgtm/alerts/g/Stephen-RA-King/wordc.svg?logo=lgtm&logoWidth=18
+[lgtm-alerts-url]: https://lgtm.com/projects/g/Stephen-RA-King/wordc/alerts/
+[lgtm-quality-image]: https://img.shields.io/lgtm/grade/python/g/Stephen-RA-King/wordc.svg?logo=lgtm&logoWidth=18
+[lgtm-quality-url]: https://lgtm.com/projects/g/Stephen-RA-King/wordc/context:python
+[license-image]: https://img.shields.io/pypi/l/wordc
+[license-url]: https://github.com/Stephen-RA-King/wordc/blob/main/LICENSE
+[mypy-image]: http://www.mypy-lang.org/static/mypy_badge.svg
+[mypy-url]: http://mypy-lang.org/
+[openssf-image]: https://api.securityscorecards.dev/projects/github.com/Stephen-RA-King/wordc/badge
+[openssf-url]: https://api.securityscorecards.dev/projects/github.com/Stephen-RA-King/wordc
+[pre-commit-image]: https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit&logoColor=white
+[pre-commit-url]: https://github.com/pre-commit/pre-commit
+[pre-commit.ci-image]: https://results.pre-commit.ci/badge/github/Stephen-RA-King/wordc/main.svg
+[pre-commit.ci-url]: https://results.pre-commit.ci/latest/github/Stephen-RA-King/wordc/main
+[pydough-image]: https://img.shields.io/badge/pydough-2023-orange?logo=cookiecutter
+[pydough-url]: https://github.com/Stephen-RA-King/pydough
+[pypi-url]: https://pypi.org/project/wordc/
+[pypi-image]: https://img.shields.io/pypi/v/wordc.svg
+[python-version-image]: https://img.shields.io/pypi/pyversions/wordc
+[readthedocs-image]: https://readthedocs.org/projects/wordc/badge/?version=latest
+[readthedocs-url]: https://wordc.readthedocs.io/en/latest/?badge=latest
+[status-image]: https://img.shields.io/pypi/status/wordc.svg
+[tests-image]: https://github.com/Stephen-RA-King/wordc/actions/workflows/tests.yml/badge.svg
+[tests-url]: https://github.com/Stephen-RA-King/wordc/actions/workflows/tests.yml
+[versioning-image]: https://img.shields.io/badge/versioning-semver_2-blue
+[versioning-url]: https://semver.org/
+[wiki]: https://github.com/Stephen-RA-King/wordc/wiki
```

### Comparing `wordc-0.1.2/pyproject.toml` & `wordc-1.0.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `wordc-0.1.2/setup.cfg` & `wordc-1.0.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `wordc-0.1.2/src/wordc/exceptions.py` & `wordc-1.0.0/src/wordc/exceptions.py`

 * *Files identical despite different names*

### Comparing `wordc-0.1.2/src/wordc/wordc.py` & `wordc-1.0.0/src/wordc/wordc.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,19 +1,22 @@
 #!/usr/bin/env python3
 # Core Library modules
 import sys
 from collections import Counter
 from collections.abc import Generator
 from pathlib import Path
 
+# Third party modules
+import psutil
+
 # Local modules
-from .cli import _parse_args
+from .cli import parse_args
 from .config import config
 from .exceptions import file_exception
-from .utils import determine_chunking, is_binary
+from .utils import detect_encoding, determine_chunking, is_binary
 
 
 @file_exception
 def read_file_contents(doc: str, encoding: str) -> str:
     """Read a file normally - used for relatively small files"""
     with open(doc, encoding=encoding) as file:
         return file.read()
@@ -35,41 +38,46 @@
                     break
                 yield chunk[: space_index + 1]
                 remainder = chunk[space_index + 1 :]
                 chunk = chunk[space_index + 1 :]
             remainder = chunk
 
 
+def fail_early_tests(file_path: Path) -> None:
+    if not file_path.exists() or not file_path.is_file():
+        print(f"The file '{file_path.name}' does not appear to be a file")
+        sys.exit(1)
+    if is_binary(file_path):
+        print(f"The file '{file_path.name}' appears to be a binary file")
+        sys.exit(1)
+
+
 def process_contents(content: str) -> Counter:
     """Process the text to remove punctuation etc"""
     words = "".join(c if c.isalnum() else " " for c in content).split()
     words = [word.lower() for word in words]
     word_counts = Counter(words)
     return word_counts
 
 
 def main() -> None:
-    args, parser = _parse_args(sys.argv[1:])
+    args, parser = parse_args(sys.argv[1:])
     config.chunk = args.chunk
     config.chunk_size = args.size
     config.encoding = args.encoding
     config.top_words = args.top_words
     file_path = Path(args.filename)
 
-    # fail early tests
-    if not file_path.exists() or not file_path.is_file():
-        print(f"The file '{file_path.name}' does not appear to be a file")
-        sys.exit(0)
-    if is_binary(file_path):
-        print(f"The file '{file_path.name}' appears to be a binary file")
-        sys.exit(0)
-    auto_chunking = determine_chunking(file_path)
+    fail_early_tests(file_path)
+    available_memory = psutil.virtual_memory().available
+    auto_chunking = determine_chunking(file_path, available_memory)
+    config.encoding = detect_encoding(file_path)
 
     if config.chunk or auto_chunking:
-        print(f"chunking...with chunk size {config.chunk_size}")
+        print(f"chunking...with chunk size {config.chunk_size} bytes")
         word_counter: Counter = Counter()
         for content in read_file_chunks(file_path, config.encoding, config.chunk_size):
             processed = process_contents(content)
             word_counter.update(processed)
 
     else:
         content = read_file_contents(file_path, config.encoding)
```

### Comparing `wordc-0.1.2/src/wordc.egg-info/PKG-INFO` & `wordc-1.0.0/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wordc
-Version: 0.1.2
+Version: 1.0.0
 Summary: boilerplate you need to create a Python package.
 Home-page: https://github.com/Stephen-RA-King/wordc
 Download-URL: https://github.com/Stephen-RA-King/wordc/archive/refs/heads/main.zip
 Author: Stephen R A King
 Author-email: sking.github@gmail.com
 Maintainer: Stephen R A King
 Maintainer-email: sking.github@gmail.com
@@ -40,14 +40,20 @@
 
 # 🚀 Quickstart
 
 ---
 
 ## 💾 Installation
 
+Using pipx (undoubtedly the best way):
+
+```sh
+pipx install wordc
+```
+
 OS X & Linux:
 
 ```sh
 pip3 install wordc
 ```
 
 Windows:
@@ -60,14 +66,61 @@
 
 ---
 
 ```sh
 pip install --editable wordc
 ```
 
+# 📝 Usage
+
+---
+
+Display the help menu with the `-h` argument
+
+```bash
+~ $ wordc -h
+```
+
+```bash
+usage: wordc [-h] [-e ENCODING] [-c] [-s SIZE] [-t TOP_WORDS] [--version] FILENAME
+
+Utility to list the top word frequency in a document
+
+positional arguments:
+  FILENAME              file to analyze for word frequency
+
+optional arguments:
+  -h, --help            show this help message and exit
+  -e ENCODING, --encoding ENCODING
+                        Encoding to use when reading file
+  -c, --chunk           Force file chunking irrespective of file size
+  -s SIZE, --size SIZE  Chunk size to use when reading file
+  -t TOP_WORDS, --top_words TOP_WORDS
+                        Number of top words to list
+  --version             display version number
+```
+
+specify the file
+
+```bash
+~ $ wordc text_file.txt
+4284 the
+2192 and
+2185 of
+1861 a
+1685 to
+```
+
+File chunking will happen automatically in certain situations:
+
+1. When the (file size / availanle memory) ratio is over 25%
+2. When the file size is over 100Mb
+
+File chunking can be forced however by using the `-c` argument.
+
 # <ℹ️> Meta
 
 ---
 
 [![](assets/linkedin.png)](https://www.linkedin.com/in/sr-king)
 [![](assets/github.png)](https://github.com/Stephen-RA-King)
 [![](assets/pypi.png)](https://pypi.org/project/wordc)
```

### Comparing `wordc-0.1.2/src/wordc.egg-info/SOURCES.txt` & `wordc-1.0.0/src/wordc.egg-info/SOURCES.txt`

 * *Files 24% similar despite different names*

```diff
@@ -16,9 +16,18 @@
 src/wordc.egg-info/PKG-INFO
 src/wordc.egg-info/SOURCES.txt
 src/wordc.egg-info/dependency_links.txt
 src/wordc.egg-info/entry_points.txt
 src/wordc.egg-info/requires.txt
 src/wordc.egg-info/top_level.txt
 tests/test_args.py
-tests/test_process_contents.py
-tests/test_read_file_contents.py
+tests/test_integration_01_nominal.py
+tests/test_integration_02_At_Ac.py
+tests/test_integration_03_ne.py
+tests/test_integration_04_dir.py
+tests/test_integration_05_bin.py
+tests/test_main_process_contents.py
+tests/test_main_read_file_chunks.py
+tests/test_main_read_file_contents.py
+tests/test_utils_detect_encoding.py
+tests/test_utils_determine_chunking.py
+tests/test_utils_isbinary.py
```

### Comparing `wordc-0.1.2/tests/test_args.py` & `wordc-1.0.0/tests/test_args.py`

 * *Files 9% similar despite different names*

```diff
@@ -5,65 +5,65 @@
 
 
 # First party modules
 from wordc import wordc
 
 
 def test_default_args():
-    args, parser = wordc._parse_args(["mobydick.txt"])
+    args, parser = wordc.parse_args(["mobydick.txt"])
     assert args.filename == "mobydick.txt"
     assert args.encoding == "utf-8"
     assert args.chunk is False
     assert args.size == 1024
     assert args.top_words == 20
 
 
 def test_args_project():
-    args, parser = wordc._parse_args(
+    args, parser = wordc.parse_args(
         [
             "mobydick.txt",
         ]
     )
     assert args.filename == "mobydick.txt"
 
 
 def test_args_register():
-    args, parser = wordc._parse_args(
+    args, parser = wordc.parse_args(
         [
             "mobydick.txt",
             "-e",
             "utf-16"
         ]
     )
     assert args.encoding == "utf-16"
 
 
 def test_args_dryrun():
-    args, parser = wordc._parse_args(
+    args, parser = wordc.parse_args(
         [
             "mobydick.txt",
             "-c",
         ]
     )
     assert args.chunk is True
 
 
 def test_args_nocleanup():
-    args, parser = wordc._parse_args(
+    args, parser = wordc.parse_args(
         [
             "mobydick.txt",
             "-s",
             "4096"
         ]
     )
     assert args.size == 4096
 
 
 def test_args_verbose():
-    args, parser = wordc._parse_args(
+    args, parser = wordc.parse_args(
         [
             "mobydick.txt",
             "-t",
             "10"
         ]
     )
     assert args.top_words == 10
```

