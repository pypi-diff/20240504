# Comparing `tmp/idc_index-0.5.3.tar.gz` & `tmp/idc_index-0.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, last modified: Wed May  1 17:07:39 2024, max compression
+gzip compressed data, last modified: Fri May  3 21:49:01 2024, max compression
```

## Comparing `idc_index-0.5.3.tar` & `idc_index-0.5.4.tar`

### file list

```diff
@@ -1,28 +1,29 @@
--rw-r--r--   0        0        0      125 2024-05-01 17:07:39.000000 idc_index-0.5.3/.git_archival.txt
--rw-r--r--   0        0        0       32 2024-05-01 17:07:39.000000 idc_index-0.5.3/.gitattributes
--rw-r--r--   0        0        0     2357 2024-05-01 17:07:39.000000 idc_index-0.5.3/.pre-commit-config.yaml
--rw-r--r--   0        0        0      309 2024-05-01 17:07:39.000000 idc_index-0.5.3/.readthedocs.yaml
--rw-r--r--   0        0        0     2742 2024-05-01 17:07:39.000000 idc_index-0.5.3/noxfile.py
--rw-r--r--   0        0        0     2394 2024-05-01 17:07:39.000000 idc_index-0.5.3/.github/CONTRIBUTING.md
--rw-r--r--   0        0        0      224 2024-05-01 17:07:39.000000 idc_index-0.5.3/.github/dependabot.yml
--rw-r--r--   0        0        0      668 2024-05-01 17:07:39.000000 idc_index-0.5.3/.github/matchers/pylint.json
--rw-r--r--   0        0        0      847 2024-05-01 17:07:39.000000 idc_index-0.5.3/.github/workflows/cd.yml
--rw-r--r--   0        0        0     1581 2024-05-01 17:07:39.000000 idc_index-0.5.3/.github/workflows/ci.yml
--rw-r--r--   0        0        0      355 2024-05-01 17:07:39.000000 idc_index-0.5.3/.github/workflows/keep-alive.yaml
--rw-r--r--   0        0        0      851 2024-05-01 17:07:39.000000 idc_index-0.5.3/docs/conf.py
--rw-r--r--   0        0        0      196 2024-05-01 17:07:39.000000 idc_index-0.5.3/docs/index.md
--rw-r--r--   0        0        0      263 2024-05-01 17:07:39.000000 idc_index-0.5.3/idc_index/__init__.py
--rw-r--r--   0        0        0      411 2024-05-01 17:07:39.000000 idc_index-0.5.3/idc_index/_version.py
--rw-r--r--   0        0        0      118 2024-05-01 17:07:39.000000 idc_index-0.5.3/idc_index/_version.pyi
--rw-r--r--   0        0        0    28034 2024-05-01 17:07:39.000000 idc_index-0.5.3/idc_index/index.py
--rw-r--r--   0        0        0        0 2024-05-01 17:07:39.000000 idc_index-0.5.3/idc_index/py.typed
--rw-r--r--   0        0        0        0 2024-05-01 17:07:39.000000 idc_index-0.5.3/tests/__init__.py
--rw-r--r--   0        0        0     3779 2024-05-01 17:07:39.000000 idc_index-0.5.3/tests/idcindex.py
--rw-r--r--   0        0        0      413 2024-05-01 17:07:39.000000 idc_index-0.5.3/tests/study_manifest_aws.s5cmd
--rw-r--r--   0        0        0      437 2024-05-01 17:07:39.000000 idc_index-0.5.3/tests/study_manifest_gcs.s5cmd
--rw-r--r--   0        0        0      175 2024-05-01 17:07:39.000000 idc_index-0.5.3/tests/test_package.py
--rw-r--r--   0        0        0     2265 2024-05-01 17:07:39.000000 idc_index-0.5.3/.gitignore
--rw-r--r--   0        0        0     1077 2024-05-01 17:07:39.000000 idc_index-0.5.3/LICENSE
--rw-r--r--   0        0        0     4290 2024-05-01 17:07:39.000000 idc_index-0.5.3/README.md
--rw-r--r--   0        0        0     6121 2024-05-01 17:07:39.000000 idc_index-0.5.3/pyproject.toml
--rw-r--r--   0        0        0     7531 2024-05-01 17:07:39.000000 idc_index-0.5.3/PKG-INFO
+-rw-r--r--   0        0        0      125 2024-05-03 21:49:01.000000 idc_index-0.5.4/.git_archival.txt
+-rw-r--r--   0        0        0       32 2024-05-03 21:49:01.000000 idc_index-0.5.4/.gitattributes
+-rw-r--r--   0        0        0     2357 2024-05-03 21:49:01.000000 idc_index-0.5.4/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      309 2024-05-03 21:49:01.000000 idc_index-0.5.4/.readthedocs.yaml
+-rw-r--r--   0        0        0     2742 2024-05-03 21:49:01.000000 idc_index-0.5.4/noxfile.py
+-rw-r--r--   0        0        0     2394 2024-05-03 21:49:01.000000 idc_index-0.5.4/.github/CONTRIBUTING.md
+-rw-r--r--   0        0        0      224 2024-05-03 21:49:01.000000 idc_index-0.5.4/.github/dependabot.yml
+-rw-r--r--   0        0        0      668 2024-05-03 21:49:01.000000 idc_index-0.5.4/.github/matchers/pylint.json
+-rw-r--r--   0        0        0      847 2024-05-03 21:49:01.000000 idc_index-0.5.4/.github/workflows/cd.yml
+-rw-r--r--   0        0        0     1585 2024-05-03 21:49:01.000000 idc_index-0.5.4/.github/workflows/ci.yml
+-rw-r--r--   0        0        0      355 2024-05-03 21:49:01.000000 idc_index-0.5.4/.github/workflows/keep-alive.yaml
+-rw-r--r--   0        0        0      851 2024-05-03 21:49:01.000000 idc_index-0.5.4/docs/conf.py
+-rw-r--r--   0        0        0      196 2024-05-03 21:49:01.000000 idc_index-0.5.4/docs/index.md
+-rw-r--r--   0        0        0      263 2024-05-03 21:49:01.000000 idc_index-0.5.4/idc_index/__init__.py
+-rw-r--r--   0        0        0      411 2024-05-03 21:49:01.000000 idc_index-0.5.4/idc_index/_version.py
+-rw-r--r--   0        0        0      118 2024-05-03 21:49:01.000000 idc_index-0.5.4/idc_index/_version.pyi
+-rw-r--r--   0        0        0    51631 2024-05-03 21:49:01.000000 idc_index-0.5.4/idc_index/index.py
+-rw-r--r--   0        0        0        0 2024-05-03 21:49:01.000000 idc_index-0.5.4/idc_index/py.typed
+-rw-r--r--   0        0        0        0 2024-05-03 21:49:01.000000 idc_index-0.5.4/tests/__init__.py
+-rw-r--r--   0        0        0     8415 2024-05-03 21:49:01.000000 idc_index-0.5.4/tests/idcindex.py
+-rw-r--r--   0        0        0      413 2024-05-03 21:49:01.000000 idc_index-0.5.4/tests/study_manifest_aws.s5cmd
+-rw-r--r--   0        0        0      279 2024-05-03 21:49:01.000000 idc_index-0.5.4/tests/study_manifest_bogus.s5cmd
+-rw-r--r--   0        0        0      419 2024-05-03 21:49:01.000000 idc_index-0.5.4/tests/study_manifest_gcs.s5cmd
+-rw-r--r--   0        0        0      175 2024-05-03 21:49:01.000000 idc_index-0.5.4/tests/test_package.py
+-rw-r--r--   0        0        0     2265 2024-05-03 21:49:01.000000 idc_index-0.5.4/.gitignore
+-rw-r--r--   0        0        0     1077 2024-05-03 21:49:01.000000 idc_index-0.5.4/LICENSE
+-rw-r--r--   0        0        0     4290 2024-05-03 21:49:01.000000 idc_index-0.5.4/README.md
+-rw-r--r--   0        0        0     6130 2024-05-03 21:49:01.000000 idc_index-0.5.4/pyproject.toml
+-rw-r--r--   0        0        0     7551 2024-05-03 21:49:01.000000 idc_index-0.5.4/PKG-INFO
```

### Comparing `idc_index-0.5.3/.pre-commit-config.yaml` & `idc_index-0.5.4/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `idc_index-0.5.3/noxfile.py` & `idc_index-0.5.4/noxfile.py`

 * *Files identical despite different names*

### Comparing `idc_index-0.5.3/.github/CONTRIBUTING.md` & `idc_index-0.5.4/.github/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `idc_index-0.5.3/.github/matchers/pylint.json` & `idc_index-0.5.4/.github/matchers/pylint.json`

 * *Files identical despite different names*

### Comparing `idc_index-0.5.3/.github/workflows/cd.yml` & `idc_index-0.5.4/.github/workflows/cd.yml`

 * *Files identical despite different names*

### Comparing `idc_index-0.5.3/.github/workflows/ci.yml` & `idc_index-0.5.4/.github/workflows/ci.yml`

 * *Files 2% similar despite different names*

```diff
@@ -55,13 +55,13 @@
 
       - name: Install package
         run: python -m pip install .[test]
 
       - name: Test package
         run: >-
           python -m pytest -ra --cov --cov-report=xml --cov-report=term
-          --durations=20
+          --durations=20 -vv
 
 #      - name: Upload coverage report
 #        uses: codecov/codecov-action@v4.1.0
 #        with:
 #          token: ${{ secrets.CODECOV_TOKEN }}
```

### Comparing `idc_index-0.5.3/docs/conf.py` & `idc_index-0.5.4/docs/conf.py`

 * *Files identical despite different names*

### Comparing `idc_index-0.5.3/.gitignore` & `idc_index-0.5.4/.gitignore`

 * *Files identical despite different names*

### Comparing `idc_index-0.5.3/LICENSE` & `idc_index-0.5.4/LICENSE`

 * *Files identical despite different names*

### Comparing `idc_index-0.5.3/README.md` & `idc_index-0.5.4/README.md`

 * *Files identical despite different names*

### Comparing `idc_index-0.5.3/pyproject.toml` & `idc_index-0.5.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -35,14 +35,15 @@
   'duckdb>=0.10.0',
   "idc-index-data==18.0.1",
   "packaging",
   "pandas<2.2",
   "psutil",
   "pyarrow",
   "s5cmd",
+  "tqdm"
 ]
 
 [project.optional-dependencies]
 test = [
   "pytest >=6",
   "pytest-cov >=3",
 ]
```

### Comparing `idc_index-0.5.3/PKG-INFO` & `idc_index-0.5.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: idc-index
-Version: 0.5.3
+Version: 0.5.4
 Summary: Package to query and download data from an index of ImagingDataCommons
 Project-URL: Homepage, https://github.com/ImagingDataCommons/idc-index
 Project-URL: Bug Tracker, https://github.com/ImagingDataCommons/idc-index/issues
 Project-URL: Discussions, https://discourse.canceridc.dev/
 Project-URL: Changelog, https://github.com/ImagingDataCommons/idc-index/releases
 Author-email: Andrey Fedorov <andrey.fedorov@gmail.com>, Vamsi Thiriveedhi <vthiriveedhi@mgh.harvard.edu>
 License: MIT License
@@ -48,14 +48,15 @@
 Requires-Dist: duckdb>=0.10.0
 Requires-Dist: idc-index-data==18.0.1
 Requires-Dist: packaging
 Requires-Dist: pandas<2.2
 Requires-Dist: psutil
 Requires-Dist: pyarrow
 Requires-Dist: s5cmd
+Requires-Dist: tqdm
 Provides-Extra: dev
 Requires-Dist: pytest-cov>=3; extra == 'dev'
 Requires-Dist: pytest>=6; extra == 'dev'
 Provides-Extra: docs
 Requires-Dist: furo>=2023.08.17; extra == 'docs'
 Requires-Dist: myst-parser>=0.13; extra == 'docs'
 Requires-Dist: sphinx-autodoc-typehints; extra == 'docs'
```

