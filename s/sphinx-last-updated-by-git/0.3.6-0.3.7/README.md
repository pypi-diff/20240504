# Comparing `tmp/sphinx-last-updated-by-git-0.3.6.tar.gz` & `tmp/sphinx_last_updated_by_git-0.3.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sphinx-last-updated-by-git-0.3.6.tar", last modified: Sat Aug 26 15:19:50 2023, max compression
+gzip compressed data, was "sphinx_last_updated_by_git-0.3.7.tar", last modified: Sat May  4 15:52:21 2024, max compression
```

## Comparing `sphinx-last-updated-by-git-0.3.6.tar` & `sphinx_last_updated_by_git-0.3.7.tar`

### file list

```diff
@@ -1,31 +1,22 @@
-drwxr-xr-x   0 mg        (1000) mg        (1000)        0 2023-08-26 15:19:50.752996 sphinx-last-updated-by-git-0.3.6/
--rw-r--r--   0 mg        (1000) mg        (1000)       40 2023-02-26 18:19:08.000000 sphinx-last-updated-by-git-0.3.6/.coveragerc
-drwxr-xr-x   0 mg        (1000) mg        (1000)        0 2023-08-26 15:19:50.748996 sphinx-last-updated-by-git-0.3.6/.github/
-drwxr-xr-x   0 mg        (1000) mg        (1000)        0 2023-08-26 15:19:50.748996 sphinx-last-updated-by-git-0.3.6/.github/workflows/
--rw-r--r--   0 mg        (1000) mg        (1000)     1050 2023-08-26 14:54:51.000000 sphinx-last-updated-by-git-0.3.6/.github/workflows/main.yml
--rw-r--r--   0 mg        (1000) mg        (1000)       91 2020-04-24 07:52:15.000000 sphinx-last-updated-by-git-0.3.6/.gitignore
--rw-r--r--   0 mg        (1000) mg        (1000)      270 2020-04-24 07:52:15.000000 sphinx-last-updated-by-git-0.3.6/.gitmodules
--rw-r--r--   0 mg        (1000) mg        (1000)     1286 2023-05-18 12:12:57.000000 sphinx-last-updated-by-git-0.3.6/LICENSE
--rw-r--r--   0 mg        (1000) mg        (1000)       17 2020-04-24 12:10:06.000000 sphinx-last-updated-by-git-0.3.6/MANIFEST.in
--rw-r--r--   0 mg        (1000) mg        (1000)     1844 2023-08-26 15:16:45.000000 sphinx-last-updated-by-git-0.3.6/NEWS.rst
--rw-r--r--   0 mg        (1000) mg        (1000)     6459 2023-08-26 15:19:50.752996 sphinx-last-updated-by-git-0.3.6/PKG-INFO
--rw-r--r--   0 mg        (1000) mg        (1000)     5781 2023-08-26 15:01:03.000000 sphinx-last-updated-by-git-0.3.6/README.rst
--rw-r--r--   0 mg        (1000) mg        (1000)       91 2023-03-08 19:19:39.000000 sphinx-last-updated-by-git-0.3.6/pyproject.toml
--rw-r--r--   0 mg        (1000) mg        (1000)      136 2022-07-22 19:51:31.000000 sphinx-last-updated-by-git-0.3.6/pytest.ini
--rw-r--r--   0 mg        (1000) mg        (1000)       38 2023-08-26 15:19:50.752996 sphinx-last-updated-by-git-0.3.6/setup.cfg
--rw-r--r--   0 mg        (1000) mg        (1000)     1200 2023-04-02 09:33:33.000000 sphinx-last-updated-by-git-0.3.6/setup.py
-drwxr-xr-x   0 mg        (1000) mg        (1000)        0 2023-08-26 15:19:50.748996 sphinx-last-updated-by-git-0.3.6/src/
-drwxr-xr-x   0 mg        (1000) mg        (1000)        0 2023-08-26 15:19:50.752996 sphinx-last-updated-by-git-0.3.6/src/sphinx_last_updated_by_git.egg-info/
--rw-r--r--   0 mg        (1000) mg        (1000)     6459 2023-08-26 15:19:50.000000 sphinx-last-updated-by-git-0.3.6/src/sphinx_last_updated_by_git.egg-info/PKG-INFO
--rw-r--r--   0 mg        (1000) mg        (1000)      614 2023-08-26 15:19:50.000000 sphinx-last-updated-by-git-0.3.6/src/sphinx_last_updated_by_git.egg-info/SOURCES.txt
--rw-r--r--   0 mg        (1000) mg        (1000)        1 2023-08-26 15:19:50.000000 sphinx-last-updated-by-git-0.3.6/src/sphinx_last_updated_by_git.egg-info/dependency_links.txt
--rw-r--r--   0 mg        (1000) mg        (1000)       12 2023-08-26 15:19:50.000000 sphinx-last-updated-by-git-0.3.6/src/sphinx_last_updated_by_git.egg-info/requires.txt
--rw-r--r--   0 mg        (1000) mg        (1000)       27 2023-08-26 15:19:50.000000 sphinx-last-updated-by-git-0.3.6/src/sphinx_last_updated_by_git.egg-info/top_level.txt
--rw-r--r--   0 mg        (1000) mg        (1000)        1 2022-09-02 15:46:29.000000 sphinx-last-updated-by-git-0.3.6/src/sphinx_last_updated_by_git.egg-info/zip-safe
--rw-r--r--   0 mg        (1000) mg        (1000)    11840 2023-08-26 15:15:33.000000 sphinx-last-updated-by-git-0.3.6/src/sphinx_last_updated_by_git.py
-drwxr-xr-x   0 mg        (1000) mg        (1000)        0 2023-08-26 15:19:50.752996 sphinx-last-updated-by-git-0.3.6/tests/
--rw-r--r--   0 mg        (1000) mg        (1000)      104 2023-04-02 09:33:51.000000 sphinx-last-updated-by-git-0.3.6/tests/requirements.txt
--rw-r--r--   0 mg        (1000) mg        (1000)     5095 2022-09-02 13:50:39.000000 sphinx-last-updated-by-git-0.3.6/tests/test_example_repo.py
--rw-r--r--   0 mg        (1000) mg        (1000)      518 2021-02-08 18:20:35.000000 sphinx-last-updated-by-git-0.3.6/tests/test_singlehtml.py
--rw-r--r--   0 mg        (1000) mg        (1000)     1584 2023-03-08 19:19:39.000000 sphinx-last-updated-by-git-0.3.6/tests/test_untracked.py
--rwxr-xr-x   0 mg        (1000) mg        (1000)      392 2021-02-03 14:42:50.000000 sphinx-last-updated-by-git-0.3.6/tests/update_submodules.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 15:52:21.961398 sphinx_last_updated_by_git-0.3.7/
+-rw-r--r--   0 runner    (1001) docker     (127)     1286 2024-05-04 15:52:18.000000 sphinx_last_updated_by_git-0.3.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-04 15:52:18.000000 sphinx_last_updated_by_git-0.3.7/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1910 2024-05-04 15:52:18.000000 sphinx_last_updated_by_git-0.3.7/NEWS.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     6865 2024-05-04 15:52:21.961398 sphinx_last_updated_by_git-0.3.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6160 2024-05-04 15:52:18.000000 sphinx_last_updated_by_git-0.3.7/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       91 2024-05-04 15:52:18.000000 sphinx_last_updated_by_git-0.3.7/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-04 15:52:21.961398 sphinx_last_updated_by_git-0.3.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1200 2024-05-04 15:52:18.000000 sphinx_last_updated_by_git-0.3.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 15:52:21.957398 sphinx_last_updated_by_git-0.3.7/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 15:52:21.961398 sphinx_last_updated_by_git-0.3.7/src/sphinx_last_updated_by_git.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6865 2024-05-04 15:52:21.000000 sphinx_last_updated_by_git-0.3.7/src/sphinx_last_updated_by_git.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      491 2024-05-04 15:52:21.000000 sphinx_last_updated_by_git-0.3.7/src/sphinx_last_updated_by_git.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-04 15:52:21.000000 sphinx_last_updated_by_git-0.3.7/src/sphinx_last_updated_by_git.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-04 15:52:21.000000 sphinx_last_updated_by_git-0.3.7/src/sphinx_last_updated_by_git.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-05-04 15:52:21.000000 sphinx_last_updated_by_git-0.3.7/src/sphinx_last_updated_by_git.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-04 15:52:21.000000 sphinx_last_updated_by_git-0.3.7/src/sphinx_last_updated_by_git.egg-info/zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)    11840 2024-05-04 15:52:18.000000 sphinx_last_updated_by_git-0.3.7/src/sphinx_last_updated_by_git.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 15:52:21.961398 sphinx_last_updated_by_git-0.3.7/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     5095 2024-05-04 15:52:18.000000 sphinx_last_updated_by_git-0.3.7/tests/test_example_repo.py
+-rw-r--r--   0 runner    (1001) docker     (127)      518 2024-05-04 15:52:18.000000 sphinx_last_updated_by_git-0.3.7/tests/test_singlehtml.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1584 2024-05-04 15:52:18.000000 sphinx_last_updated_by_git-0.3.7/tests/test_untracked.py
```

### Comparing `sphinx-last-updated-by-git-0.3.6/LICENSE` & `sphinx_last_updated_by_git-0.3.7/LICENSE`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-Copyright (c) 2020-2023, Matthias Geier
+Copyright (c) 2020-2024, Matthias Geier
 
 Redistribution and use in source and binary forms, with or without
 modification, are permitted provided that the following conditions are met:
 
 1. Redistributions of source code must retain the above copyright notice, this
    list of conditions and the following disclaimer.
```

### Comparing `sphinx-last-updated-by-git-0.3.6/NEWS.rst` & `sphinx_last_updated_by_git-0.3.7/NEWS.rst`

 * *Files 10% similar despite different names*

```diff
@@ -1,7 +1,10 @@
+Version 0.3.7 (2024-05-04):
+ * Only documentation and CI updates
+
 Version 0.3.6 (2023-08-26):
  * Support for changed behavior of ``source-read`` event in Sphinx 7.2
 
 Version 0.3.5 (2023-05-18):
  * A few build system and test updates
 
 Version 0.3.4 (2022-09-02):
```

### Comparing `sphinx-last-updated-by-git-0.3.6/PKG-INFO` & `sphinx_last_updated_by_git-0.3.7/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sphinx-last-updated-by-git
-Version: 0.3.6
+Version: 0.3.7
 Summary: Get the "last updated" time for each Sphinx page from Git
 Home-page: https://github.com/mgeier/sphinx-last-updated-by-git/
 Author: Matthias Geier
 Author-email: Matthias.Geier@gmail.com
 License: BSD-2-Clause
 Keywords: Sphinx,Git
 Platform: any
@@ -13,14 +13,15 @@
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Documentation :: Sphinx
 Requires-Python: >=3.7
 License-File: LICENSE
+Requires-Dist: sphinx>=1.8
 
 Get the "last updated" time for each Sphinx page from Git
 =========================================================
 
 This is a little Sphinx_ extension that does exactly that.
 It also checks for included files and other dependencies and
 uses their "last updated" time if it's more recent.
@@ -49,15 +50,15 @@
       html_copy_source_ and html_show_sourcelink_ must also be ``True``, and
       the theme you are using must support source links in the first place.
 
     * By default, timestamps are displayed using the local time zone.
       You can specify a datetime.timezone_ object (or any ``tzinfo`` subclass
       instance) with the configuration option ``git_last_updated_timezone``.
       You can also use any string recognized by babel_,
-      e.g.  ``git_last_updated_timezone = 'NZ'``.
+      e.g. ``git_last_updated_timezone = 'Pacific/Auckland'``.
 
     * By default, the "last updated" timestamp is added as an HTML ``<meta>``
       tag.  This can be disabled by setting the configuration option
       ``git_last_updated_metatags`` to ``False``.
 
     * Files can be excluded from the last updated date calculation by passing
       a list of exclusion patterns to the configuration option
@@ -91,15 +92,28 @@
               post_checkout:
                 - git fetch --unshallow || true
 
       For more details, `read the docs`__.
 
       __ https://docs.readthedocs.io/en/latest/build-customization.html#unshallow-git-clone
 
-      If you want to get rid of the warning (without actually fixing the problem),
+      This might also happen when using Github Actions,
+      because `actions/checkout`__ also uses shallow clones by default.
+      This can be changed by using ``fetch-depth: 0``:
+
+      .. code:: yaml
+
+          steps:
+            - uses: actions/checkout@v3
+              with:
+                fetch-depth: 0
+
+      __ https://github.com/actions/checkout
+
+      If you only want to get rid of the warning (without actually fixing the problem),
       use this in your ``conf.py``::
 
           suppress_warnings = ['git.too_shallow']
 
     * When a project on https://readthedocs.org/ using their default theme
       ``sphinx_rtd_theme`` was created before October 20th 2020,
       the date will not be displayed in the footer.
```

### Comparing `sphinx-last-updated-by-git-0.3.6/README.rst` & `sphinx_last_updated_by_git-0.3.7/README.rst`

 * *Files 6% similar despite different names*

```diff
@@ -29,15 +29,15 @@
       html_copy_source_ and html_show_sourcelink_ must also be ``True``, and
       the theme you are using must support source links in the first place.
 
     * By default, timestamps are displayed using the local time zone.
       You can specify a datetime.timezone_ object (or any ``tzinfo`` subclass
       instance) with the configuration option ``git_last_updated_timezone``.
       You can also use any string recognized by babel_,
-      e.g.  ``git_last_updated_timezone = 'NZ'``.
+      e.g. ``git_last_updated_timezone = 'Pacific/Auckland'``.
 
     * By default, the "last updated" timestamp is added as an HTML ``<meta>``
       tag.  This can be disabled by setting the configuration option
       ``git_last_updated_metatags`` to ``False``.
 
     * Files can be excluded from the last updated date calculation by passing
       a list of exclusion patterns to the configuration option
@@ -71,15 +71,28 @@
               post_checkout:
                 - git fetch --unshallow || true
 
       For more details, `read the docs`__.
 
       __ https://docs.readthedocs.io/en/latest/build-customization.html#unshallow-git-clone
 
-      If you want to get rid of the warning (without actually fixing the problem),
+      This might also happen when using Github Actions,
+      because `actions/checkout`__ also uses shallow clones by default.
+      This can be changed by using ``fetch-depth: 0``:
+
+      .. code:: yaml
+
+          steps:
+            - uses: actions/checkout@v3
+              with:
+                fetch-depth: 0
+
+      __ https://github.com/actions/checkout
+
+      If you only want to get rid of the warning (without actually fixing the problem),
       use this in your ``conf.py``::
 
           suppress_warnings = ['git.too_shallow']
 
     * When a project on https://readthedocs.org/ using their default theme
       ``sphinx_rtd_theme`` was created before October 20th 2020,
       the date will not be displayed in the footer.
```

### Comparing `sphinx-last-updated-by-git-0.3.6/setup.py` & `sphinx_last_updated_by_git-0.3.7/setup.py`

 * *Files identical despite different names*

### Comparing `sphinx-last-updated-by-git-0.3.6/src/sphinx_last_updated_by_git.egg-info/PKG-INFO` & `sphinx_last_updated_by_git-0.3.7/src/sphinx_last_updated_by_git.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sphinx-last-updated-by-git
-Version: 0.3.6
+Version: 0.3.7
 Summary: Get the "last updated" time for each Sphinx page from Git
 Home-page: https://github.com/mgeier/sphinx-last-updated-by-git/
 Author: Matthias Geier
 Author-email: Matthias.Geier@gmail.com
 License: BSD-2-Clause
 Keywords: Sphinx,Git
 Platform: any
@@ -13,14 +13,15 @@
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Documentation :: Sphinx
 Requires-Python: >=3.7
 License-File: LICENSE
+Requires-Dist: sphinx>=1.8
 
 Get the "last updated" time for each Sphinx page from Git
 =========================================================
 
 This is a little Sphinx_ extension that does exactly that.
 It also checks for included files and other dependencies and
 uses their "last updated" time if it's more recent.
@@ -49,15 +50,15 @@
       html_copy_source_ and html_show_sourcelink_ must also be ``True``, and
       the theme you are using must support source links in the first place.
 
     * By default, timestamps are displayed using the local time zone.
       You can specify a datetime.timezone_ object (or any ``tzinfo`` subclass
       instance) with the configuration option ``git_last_updated_timezone``.
       You can also use any string recognized by babel_,
-      e.g.  ``git_last_updated_timezone = 'NZ'``.
+      e.g. ``git_last_updated_timezone = 'Pacific/Auckland'``.
 
     * By default, the "last updated" timestamp is added as an HTML ``<meta>``
       tag.  This can be disabled by setting the configuration option
       ``git_last_updated_metatags`` to ``False``.
 
     * Files can be excluded from the last updated date calculation by passing
       a list of exclusion patterns to the configuration option
@@ -91,15 +92,28 @@
               post_checkout:
                 - git fetch --unshallow || true
 
       For more details, `read the docs`__.
 
       __ https://docs.readthedocs.io/en/latest/build-customization.html#unshallow-git-clone
 
-      If you want to get rid of the warning (without actually fixing the problem),
+      This might also happen when using Github Actions,
+      because `actions/checkout`__ also uses shallow clones by default.
+      This can be changed by using ``fetch-depth: 0``:
+
+      .. code:: yaml
+
+          steps:
+            - uses: actions/checkout@v3
+              with:
+                fetch-depth: 0
+
+      __ https://github.com/actions/checkout
+
+      If you only want to get rid of the warning (without actually fixing the problem),
       use this in your ``conf.py``::
 
           suppress_warnings = ['git.too_shallow']
 
     * When a project on https://readthedocs.org/ using their default theme
       ``sphinx_rtd_theme`` was created before October 20th 2020,
       the date will not be displayed in the footer.
```

### Comparing `sphinx-last-updated-by-git-0.3.6/src/sphinx_last_updated_by_git.py` & `sphinx_last_updated_by_git-0.3.7/src/sphinx_last_updated_by_git.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 try:
     from sphinx.util.display import status_iterator
 except ImportError:
     # For older Sphinx versions, will be removed in Sphinx 8:
     from sphinx.util import status_iterator
 
 
-__version__ = '0.3.6'
+__version__ = '0.3.7'
 
 
 logger = getLogger(__name__)
 
 
 def update_file_dates(git_dir, exclude_commits, file_dates):
     """Ask Git for "author date" of given files in given directory.
```

### Comparing `sphinx-last-updated-by-git-0.3.6/tests/test_example_repo.py` & `sphinx_last_updated_by_git-0.3.7/tests/test_example_repo.py`

 * *Files identical despite different names*

### Comparing `sphinx-last-updated-by-git-0.3.6/tests/test_singlehtml.py` & `sphinx_last_updated_by_git-0.3.7/tests/test_singlehtml.py`

 * *Files identical despite different names*

### Comparing `sphinx-last-updated-by-git-0.3.6/tests/test_untracked.py` & `sphinx_last_updated_by_git-0.3.7/tests/test_untracked.py`

 * *Files identical despite different names*

