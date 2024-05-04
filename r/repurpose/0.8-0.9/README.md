# Comparing `tmp/repurpose-0.8.tar.gz` & `tmp/repurpose-0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/repurpose-0.8.tar", last modified: Mon Sep 21 12:39:50 2020, max compression
+gzip compressed data, was "repurpose-0.9.tar", last modified: Tue Feb  7 11:53:37 2023, max compression
```

## Comparing `repurpose-0.8.tar` & `repurpose-0.9.tar`

### file list

```diff
@@ -1,46 +1,49 @@
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-09-21 12:39:50.000000 repurpose-0.8/
--rw-rw-r--   0 travis    (2000) travis    (2000)      817 2020-09-21 12:37:46.000000 repurpose-0.8/CHANGELOG.rst
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-09-21 12:39:50.000000 repurpose-0.8/docs/
--rw-rw-r--   0 travis    (2000) travis    (2000)       43 2020-09-21 12:37:46.000000 repurpose-0.8/docs/changelog.rst
--rw-rw-r--   0 travis    (2000) travis    (2000)       41 2020-09-21 12:37:46.000000 repurpose-0.8/docs/authors.rst
--rw-rw-r--   0 travis    (2000) travis    (2000)       16 2020-09-21 12:37:46.000000 repurpose-0.8/docs/requirements.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)     7612 2020-09-21 12:37:46.000000 repurpose-0.8/docs/Makefile
--rw-rw-r--   0 travis    (2000) travis    (2000)     9187 2020-09-21 12:37:46.000000 repurpose-0.8/docs/conf.py
--rw-rw-r--   0 travis    (2000) travis    (2000)       67 2020-09-21 12:37:46.000000 repurpose-0.8/docs/license.rst
--rw-rw-r--   0 travis    (2000) travis    (2000)      363 2020-09-21 12:37:46.000000 repurpose-0.8/docs/index.rst
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-09-21 12:39:50.000000 repurpose-0.8/docs/_static/
--rw-rw-r--   0 travis    (2000) travis    (2000)       18 2020-09-21 12:37:46.000000 repurpose-0.8/docs/_static/.gitignore
--rw-rw-r--   0 travis    (2000) travis    (2000)     9861 2020-09-21 12:37:46.000000 repurpose-0.8/docs/ts2img.rst
--rw-rw-r--   0 travis    (2000) travis    (2000)      182 2020-09-21 12:37:46.000000 repurpose-0.8/docs/resample.rst
--rw-rw-r--   0 travis    (2000) travis    (2000)     1593 2020-09-21 12:37:46.000000 repurpose-0.8/LICENSE.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)      699 2020-09-21 12:37:46.000000 repurpose-0.8/requirements.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)     5392 2020-09-21 12:39:50.000000 repurpose-0.8/PKG-INFO
--rw-rw-r--   0 travis    (2000) travis    (2000)      149 2020-09-21 12:37:46.000000 repurpose-0.8/AUTHORS.rst
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-09-21 12:39:50.000000 repurpose-0.8/src/
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-09-21 12:39:50.000000 repurpose-0.8/src/repurpose/
--rw-rw-r--   0 travis    (2000) travis    (2000)    23235 2020-09-21 12:37:46.000000 repurpose-0.8/src/repurpose/img2ts.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     6059 2020-09-21 12:37:46.000000 repurpose-0.8/src/repurpose/ts2img.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      136 2020-09-21 12:37:46.000000 repurpose-0.8/src/repurpose/__init__.py
--rwxrwxr-x   0 travis    (2000) travis    (2000)    11425 2020-09-21 12:37:46.000000 repurpose-0.8/src/repurpose/resample.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-09-21 12:39:50.000000 repurpose-0.8/src/repurpose.egg-info/
--rw-rw-r--   0 travis    (2000) travis    (2000)     5392 2020-09-21 12:39:50.000000 repurpose-0.8/src/repurpose.egg-info/PKG-INFO
--rw-rw-r--   0 travis    (2000) travis    (2000)        1 2020-09-21 12:39:50.000000 repurpose-0.8/src/repurpose.egg-info/dependency_links.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)       10 2020-09-21 12:39:50.000000 repurpose-0.8/src/repurpose.egg-info/top_level.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)        1 2020-09-21 12:39:50.000000 repurpose-0.8/src/repurpose.egg-info/not-zip-safe
--rw-rw-r--   0 travis    (2000) travis    (2000)      762 2020-09-21 12:39:50.000000 repurpose-0.8/src/repurpose.egg-info/SOURCES.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)       80 2020-09-21 12:39:50.000000 repurpose-0.8/src/repurpose.egg-info/requires.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)       34 2020-09-21 12:37:46.000000 repurpose-0.8/.gitattributes
--rw-rw-r--   0 travis    (2000) travis    (2000)      520 2020-09-21 12:37:46.000000 repurpose-0.8/.gitignore
--rw-rw-r--   0 travis    (2000) travis    (2000)      329 2020-09-21 12:37:46.000000 repurpose-0.8/environment.yml
--rw-rw-r--   0 travis    (2000) travis    (2000)     1359 2020-09-21 12:39:50.000000 repurpose-0.8/setup.cfg
--rw-rw-r--   0 travis    (2000) travis    (2000)     1543 2020-09-21 12:37:46.000000 repurpose-0.8/.travis.yml
--rw-rw-r--   0 travis    (2000) travis    (2000)       83 2020-09-21 12:37:46.000000 repurpose-0.8/readthedocs.yml
--rw-rw-r--   0 travis    (2000) travis    (2000)      592 2020-09-21 12:37:46.000000 repurpose-0.8/.coveragerc
--rw-rw-r--   0 travis    (2000) travis    (2000)     3985 2020-09-21 12:37:46.000000 repurpose-0.8/README.rst
--rw-rw-r--   0 travis    (2000) travis    (2000)      573 2020-09-21 12:37:46.000000 repurpose-0.8/setup.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-09-21 12:39:50.000000 repurpose-0.8/tests/
--rw-rw-r--   0 travis    (2000) travis    (2000)     6174 2020-09-21 12:37:46.000000 repurpose-0.8/tests/test_img2ts.py
--rwxrwxr-x   0 travis    (2000) travis    (2000)     5771 2020-09-21 12:37:46.000000 repurpose-0.8/tests/test_resample.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3319 2020-09-21 12:37:46.000000 repurpose-0.8/tests/test_ts2img.py
--rw-rw-r--   0 travis    (2000) travis    (2000)        0 2020-09-21 12:37:46.000000 repurpose-0.8/tests/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      230 2020-09-21 12:37:46.000000 repurpose-0.8/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-07 11:53:37.290358 repurpose-0.9/
+-rw-r--r--   0 runner    (1001) docker     (123)      592 2023-02-07 11:49:06.000000 repurpose-0.9/.coveragerc
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-02-07 11:49:06.000000 repurpose-0.9/.gitattributes
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-07 11:53:37.282358 repurpose-0.9/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-07 11:53:37.282358 repurpose-0.9/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     3725 2023-02-07 11:49:06.000000 repurpose-0.9/.github/workflows/build.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      520 2023-02-07 11:49:06.000000 repurpose-0.9/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      205 2023-02-07 11:49:06.000000 repurpose-0.9/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      149 2023-02-07 11:49:06.000000 repurpose-0.9/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1007 2023-02-07 11:49:06.000000 repurpose-0.9/CHANGELOG.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1593 2023-02-07 11:49:06.000000 repurpose-0.9/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     4768 2023-02-07 11:53:37.290358 repurpose-0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4202 2023-02-07 11:49:06.000000 repurpose-0.9/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-07 11:53:37.286358 repurpose-0.9/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-02-07 11:49:06.000000 repurpose-0.9/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-07 11:53:37.286358 repurpose-0.9/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-02-07 11:49:06.000000 repurpose-0.9/docs/_static/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-02-07 11:49:06.000000 repurpose-0.9/docs/authors.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-02-07 11:49:06.000000 repurpose-0.9/docs/changelog.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     9734 2023-02-07 11:49:06.000000 repurpose-0.9/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      363 2023-02-07 11:49:06.000000 repurpose-0.9/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-02-07 11:49:06.000000 repurpose-0.9/docs/license.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-02-07 11:49:06.000000 repurpose-0.9/docs/readme.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      182 2023-02-07 11:49:06.000000 repurpose-0.9/docs/resample.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     9861 2023-02-07 11:49:06.000000 repurpose-0.9/docs/ts2img.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      404 2023-02-07 11:49:06.000000 repurpose-0.9/environment.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      346 2023-02-07 11:49:06.000000 repurpose-0.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1450 2023-02-07 11:53:37.290358 repurpose-0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      704 2023-02-07 11:49:06.000000 repurpose-0.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-07 11:53:37.282358 repurpose-0.9/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-07 11:53:37.286358 repurpose-0.9/src/repurpose/
+-rw-r--r--   0 runner    (1001) docker     (123)      577 2023-02-07 11:49:06.000000 repurpose-0.9/src/repurpose/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22518 2023-02-07 11:49:06.000000 repurpose-0.9/src/repurpose/img2ts.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    11425 2023-02-07 11:49:06.000000 repurpose-0.9/src/repurpose/resample.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6056 2023-02-07 11:49:06.000000 repurpose-0.9/src/repurpose/ts2img.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-07 11:53:37.286358 repurpose-0.9/src/repurpose.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4768 2023-02-07 11:53:37.000000 repurpose-0.9/src/repurpose.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      779 2023-02-07 11:53:37.000000 repurpose-0.9/src/repurpose.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-07 11:53:37.000000 repurpose-0.9/src/repurpose.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-07 11:53:26.000000 repurpose-0.9/src/repurpose.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      141 2023-02-07 11:53:37.000000 repurpose-0.9/src/repurpose.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-02-07 11:53:37.000000 repurpose-0.9/src/repurpose.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-07 11:53:37.286358 repurpose-0.9/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-07 11:49:06.000000 repurpose-0.9/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      230 2023-02-07 11:49:06.000000 repurpose-0.9/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6421 2023-02-07 11:49:06.000000 repurpose-0.9/tests/test_img2ts.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5771 2023-02-07 11:49:06.000000 repurpose-0.9/tests/test_resample.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3319 2023-02-07 11:49:06.000000 repurpose-0.9/tests/test_ts2img.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2851 2023-02-07 11:49:06.000000 repurpose-0.9/tox.ini
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `repurpose-0.8/CHANGELOG.rst` & `repurpose-0.9/CHANGELOG.rst`

 * *Files 25% similar despite different names*

```diff
@@ -1,16 +1,22 @@
 =========
 Changelog
 =========
 
-Unreleased
-==========
+Unreleased changes in master branch
+===================================
 
 -
 
+Version 0.9
+===========
+
+- Update for new pyscaffold
+- Fixed bug where resampling failed when a BasicGrid was passed instead of a CellGrid
+
 Version 0.8
 ===========
 
 - Update pyscaffold package structure (pyscaffold 3)
 - Drop py2 support
 - Add pypi deployment to travis.
```

### Comparing `repurpose-0.8/docs/conf.py` & `repurpose-0.9/docs/conf.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,34 +1,33 @@
-# -*- coding: utf-8 -*-
-#
 # This file is execfile()d with the current directory set to its containing dir.
 #
-# Note that not all possible configuration values are present in this
-# autogenerated file.
+# This file only contains a selection of the most common options. For a full
+# list see the documentation:
+# https://www.sphinx-doc.org/en/master/usage/configuration.html
 #
 # All configuration values have a default; values that are commented out
 # serve to show the default.
 
 import os
 import sys
-import inspect
 import shutil
 
-__location__ = os.path.join(os.getcwd(), os.path.dirname(
-    inspect.getfile(inspect.currentframe())))
+# -- Path setup --------------------------------------------------------------
+
+__location__ = os.path.dirname(__file__)
 
 # If extensions (or modules to document with autodoc) are in another directory,
 # add these directories to sys.path here. If the directory is relative to the
 # documentation root, use os.path.abspath to make it absolute, like shown here.
-sys.path.insert(0, os.path.join(__location__, '../src'))
+sys.path.insert(0, os.path.join(__location__, "../src"))
 
-# -- Run sphinx-apidoc ------------------------------------------------------
+# -- Run sphinx-apidoc -------------------------------------------------------
 # This hack is necessary since RTD does not issue `sphinx-apidoc` before running
 # `sphinx-build -b html . _build/html`. See Issue:
-# https://github.com/rtfd/readthedocs.org/issues/1139
+# https://github.com/readthedocs/readthedocs.org/issues/1139
 # DON'T FORGET: Check the box "Install your project inside a virtualenv using
 # setup.py install" in the RTD Advanced Settings.
 # Additionally it helps us to avoid running apidoc manually
 
 try:  # for Sphinx >= 1.7
     from sphinx.ext import apidoc
 except ImportError:
@@ -39,77 +38,93 @@
 try:
     shutil.rmtree(output_dir)
 except FileNotFoundError:
     pass
 
 try:
     import sphinx
-    from pkg_resources import parse_version
 
-    cmd_line_template = "sphinx-apidoc -f -o {outputdir} {moduledir}"
-    cmd_line = cmd_line_template.format(outputdir=output_dir, moduledir=module_dir)
+    cmd_line = f"sphinx-apidoc --implicit-namespaces -f -o {output_dir} {module_dir}"
 
     args = cmd_line.split(" ")
-    if parse_version(sphinx.__version__) >= parse_version('1.7'):
+    if tuple(sphinx.__version__.split(".")) >= ("1", "7"):
+        # This is a rudimentary parse_version to avoid external dependencies
         args = args[1:]
 
     apidoc.main(args)
 except Exception as e:
     print("Running `sphinx-apidoc` failed!\n{}".format(e))
 
-# -- General configuration -----------------------------------------------------
+# -- General configuration ---------------------------------------------------
 
 # If your documentation needs a minimal Sphinx version, state it here.
 # needs_sphinx = '1.0'
 
 # Add any Sphinx extension module names here, as strings. They can be extensions
 # coming with Sphinx (named 'sphinx.ext.*') or your custom ones.
-extensions = ['sphinx.ext.autodoc', 'sphinx.ext.intersphinx', 'sphinx.ext.todo',
-              'sphinx.ext.autosummary', 'sphinx.ext.viewcode', 'sphinx.ext.coverage',
-              'sphinx.ext.doctest', 'sphinx.ext.ifconfig', 'sphinx.ext.mathjax',
-              'sphinx.ext.napoleon']
+extensions = [
+    "sphinx.ext.autodoc",
+    "sphinx.ext.intersphinx",
+    "sphinx.ext.todo",
+    "sphinx.ext.autosummary",
+    "sphinx.ext.viewcode",
+    "sphinx.ext.coverage",
+    "sphinx.ext.doctest",
+    "sphinx.ext.ifconfig",
+    "sphinx.ext.mathjax",
+    "sphinx.ext.napoleon",
+]
 
 # Add any paths that contain templates here, relative to this directory.
-templates_path = ['_templates']
+templates_path = ["_templates"]
 
 # The suffix of source filenames.
-source_suffix = '.rst'
+source_suffix = ".rst"
 
 # The encoding of source files.
 # source_encoding = 'utf-8-sig'
 
 # The master toctree document.
-master_doc = 'index'
+master_doc = "index"
 
 # General information about the project.
-project = u'repurpose'
-copyright = u'2019, TU Wien'
+project = "repurpose"
+copyright = "2023, TU Wien"
 
 # The version info for the project you're documenting, acts as replacement for
 # |version| and |release|, also used in various other places throughout the
 # built documents.
 #
-# The short X.Y version.
-version = ''  # Is set by calling `setup.py docs`
-# The full version, including alpha/beta/rc tags.
-release = ''  # Is set by calling `setup.py docs`
+# version: The short X.Y version.
+# release: The full version, including alpha/beta/rc tags.
+# If you don’t need the separation provided between version and release,
+# just set them both to the same value.
+try:
+    from repurpose import __version__ as version
+except ImportError:
+    version = ""
+
+if not version or version.lower() == "unknown":
+    version = os.getenv("READTHEDOCS_VERSION", "unknown")  # automatically set by RTD
+
+release = version
 
 # The language for content autogenerated by Sphinx. Refer to documentation
 # for a list of supported languages.
 # language = None
 
 # There are two options for replacing |today|: either, you set today to some
 # non-false value, then it is used:
 # today = ''
 # Else, today_fmt is used as the format for a strftime call.
 # today_fmt = '%B %d, %Y'
 
 # List of patterns, relative to source directory, that match files and
 # directories to ignore when looking for source files.
-exclude_patterns = ['_build']
+exclude_patterns = ["_build", "Thumbs.db", ".DS_Store", ".venv"]
 
 # The reST default role (used for this markup: `text`) to use for all documents.
 # default_role = None
 
 # If true, '()' will be appended to :func: etc. cross-reference text.
 # add_function_parentheses = True
 
@@ -118,48 +133,46 @@
 # add_module_names = True
 
 # If true, sectionauthor and moduleauthor directives will be shown in the
 # output. They are ignored by default.
 # show_authors = False
 
 # The name of the Pygments (syntax highlighting) style to use.
-pygments_style = 'sphinx'
+pygments_style = "sphinx"
 
 # A list of ignored prefixes for module index sorting.
 # modindex_common_prefix = []
 
 # If true, keep warnings as "system message" paragraphs in the built documents.
 # keep_warnings = False
 
+# If this is True, todo emits a warning for each TODO entries. The default is False.
+todo_emit_warnings = True
 
-# -- Options for HTML output ---------------------------------------------------
+
+# -- Options for HTML output -------------------------------------------------
 
 # The theme to use for HTML and HTML Help pages.  See the documentation for
 # a list of builtin themes.
-html_theme = 'sphinx_rtd_theme'
+html_theme = "alabaster"
 
 # Theme options are theme-specific and customize the look and feel of a theme
 # further.  For a list of options available for each theme, see the
 # documentation.
 html_theme_options = {
-    'sidebar_width': '300px',
-    'page_width': '1200px'
+    "sidebar_width": "300px",
+    "page_width": "1200px"
 }
 
 # Add any paths that contain custom themes here, relative to this directory.
 # html_theme_path = []
 
 # The name for this set of Sphinx documents.  If None, it defaults to
 # "<project> v<release> documentation".
-try:
-    from repurpose import __version__ as version
-except ImportError:
-    pass
-else:
-    release = version
+# html_title = None
 
 # A shorter title for the navigation bar.  Default is the same as html_title.
 # html_short_title = None
 
 # The name of an image file (relative to this directory) to place at the top
 # of the sidebar.
 # html_logo = ""
@@ -168,15 +181,15 @@
 # docs.  This file should be a Windows icon file (.ico) being 16x16 or 32x32
 # pixels large.
 # html_favicon = None
 
 # Add any paths that contain custom static files (such as style sheets) here,
 # relative to this directory. They are copied after the builtin static files,
 # so a file named "default.css" will overwrite the builtin "default.css".
-html_static_path = ['_static']
+html_static_path = ["_static"]
 
 # If not '', a 'Last updated on:' timestamp is inserted at every page bottom,
 # using the given strftime format.
 # html_last_updated_fmt = '%b %d, %Y'
 
 # If true, SmartyPants will be used to convert quotes and dashes to
 # typographically correct entities.
@@ -212,35 +225,32 @@
 # base URL from which the finished HTML is served.
 # html_use_opensearch = ''
 
 # This is the file name suffix for HTML files (e.g. ".xhtml").
 # html_file_suffix = None
 
 # Output file base name for HTML help builder.
-htmlhelp_basename = 'repurpose-doc'
+htmlhelp_basename = "repurpose-doc"
 
 
-# -- Options for LaTeX output --------------------------------------------------
+# -- Options for LaTeX output ------------------------------------------------
 
 latex_elements = {
-# The paper size ('letterpaper' or 'a4paper').
-# 'papersize': 'letterpaper',
-
-# The font size ('10pt', '11pt' or '12pt').
-# 'pointsize': '10pt',
-
-# Additional stuff for the LaTeX preamble.
-# 'preamble': '',
+    # The paper size ("letterpaper" or "a4paper").
+    # "papersize": "letterpaper",
+    # The font size ("10pt", "11pt" or "12pt").
+    # "pointsize": "10pt",
+    # Additional stuff for the LaTeX preamble.
+    # "preamble": "",
 }
 
 # Grouping the document tree into LaTeX files. List of tuples
 # (source start file, target name, title, author, documentclass [howto/manual]).
 latex_documents = [
-  ('index', 'user_guide.tex', u'repurpose Documentation',
-   u'Wolfgang Preimesberger', 'manual'),
+    ("index", "user_guide.tex", "repurpose Documentation", "TU Wien", "manual")
 ]
 
 # The name of an image file (relative to this directory) to place at the top of
 # the title page.
 # latex_logo = ""
 
 # For "manual" documents, if this is true, then toplevel headings are parts,
@@ -255,18 +265,22 @@
 
 # Documents to append as an appendix to all manuals.
 # latex_appendices = []
 
 # If false, no module index is generated.
 # latex_domain_indices = True
 
-# -- External mapping ------------------------------------------------------------
-python_version = '.'.join(map(str, sys.version_info[0:2]))
+# -- External mapping --------------------------------------------------------
+python_version = ".".join(map(str, sys.version_info[0:2]))
 intersphinx_mapping = {
-    'sphinx': ('http://www.sphinx-doc.org/en/stable', None),
-    'python': ('https://docs.python.org/' + python_version, None),
-    'matplotlib': ('https://matplotlib.org', None),
-    'numpy': ('https://docs.scipy.org/doc/numpy', None),
-    'sklearn': ('http://scikit-learn.org/stable', None),
-    'pandas': ('http://pandas.pydata.org/pandas-docs/stable', None),
-    'scipy': ('https://docs.scipy.org/doc/scipy/reference', None),
+    "sphinx": ("https://www.sphinx-doc.org/en/master", None),
+    "python": ("https://docs.python.org/" + python_version, None),
+    "matplotlib": ("https://matplotlib.org", None),
+    "numpy": ("https://numpy.org/doc/stable", None),
+    "sklearn": ("https://scikit-learn.org/stable", None),
+    "pandas": ("https://pandas.pydata.org/pandas-docs/stable", None),
+    "scipy": ("https://docs.scipy.org/doc/scipy/reference", None),
+    "setuptools": ("https://setuptools.pypa.io/en/stable/", None),
+    "pyscaffold": ("https://pyscaffold.org/en/stable", None),
 }
+
+print(f"loading configurations for {project} {version} ...", file=sys.stderr)
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `repurpose-0.8/docs/ts2img.rst` & `repurpose-0.9/docs/ts2img.rst`

 * *Files identical despite different names*

### Comparing `repurpose-0.8/LICENSE.txt` & `repurpose-0.9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `repurpose-0.8/PKG-INFO` & `repurpose-0.9/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,126 +1,136 @@
 Metadata-Version: 2.1
 Name: repurpose
-Version: 0.8
+Version: 0.9
 Summary: Package for image to timeseries to image conversion
 Home-page: https://repurpose.readthedocs.io/en/latest/
 Author: TU Wien
 Author-email: remote.sensing@geo.tuwien.ac.at
 License: mit
 Project-URL: Documentation, https://repurpose.readthedocs.io/en/latest/
-Description: =========
-        repurpose
-        =========
-        
-        .. image:: https://travis-ci.org/TUW-GEO/repurpose.svg?branch=master
-            :target: https://travis-ci.org/TUW-GEO/repurpose
-        
-        .. image:: https://coveralls.io/repos/github/TUW-GEO/repurpose/badge.svg?branch=master
-           :target: https://coveralls.io/github/TUW-GEO/repurpose?branch=master
-        
-        .. image:: https://badge.fury.io/py/repurpose.svg
-            :target: http://badge.fury.io/py/repurpose
-        
-        .. image:: https://readthedocs.org/projects/repurpose/badge/?version=latest
-           :target: http://repurpose.readthedocs.org/
-        
-        
-        This package provides routines for the conversion of image formats to time
-        series and vice versa. It is part of the `poets project
-        <http://tuw-geo.github.io/poets/>`_ and works best with the readers and writers
-        supported there. The main use case is for data that is sampled irregularly in
-        space or time. If you have data that is sampled in regular intervals then there
-        are alternatives to this package which might be better for your use case. See
-        `Alternatives`_ for more detail.
-        
-        The readers and writers have to conform to the API specifications of the base
-        classes defined in `pygeobase <https://github.com/TUW-GEO/pygeobase>`_ to work
-        without adpation.
-        
-        Citation
-        ========
-        
-        .. image:: https://zenodo.org/badge/DOI/10.5281/zenodo.593577.svg
-           :target: https://doi.org/10.5281/zenodo.593577
-        
-        If you use the software in a publication then please cite it using the Zenodo DOI.
-        Be aware that this badge links to the latest package version.
-        
-        Please select your specific version at https://doi.org/10.5281/zenodo.593577 to get the DOI of that version.
-        You should normally always use the DOI for the specific version of your record in citations.
-        This is to ensure that other researchers can access the exact research artefact you used for reproducibility.
-        
-        You can find additional information regarding DOI versioning at http://help.zenodo.org/#versioning
-        
-        Installation
-        ============
-        
-        This package should be installable through pip:
-        
-        .. code::
-        
-            pip install repurpose
-        
-        Modules
-        =======
-        
-        It includes two main modules:
-        
-        - ``img2ts`` for image/swath to time series conversion, including support for
-          spatial resampling.
-        - ``ts2img`` for time series to image conversion, including support for temporal
-          resampling. This module is very experimental at the moment.
-        - ``resample`` for spatial resampling of (regular or irregular) gridded data to different resolutions.
-        
-        Alternatives
-        ============
-        
-        If you have data that can be represented as a 3D datacube then these projects
-        might be better suited to your needs.
-        
-        - `PyReshaper <https://github.com/NCAR/PyReshaper>`_ is a package that works
-          with NetCDF input and output and converts time slices into a time series
-          representation.
-        - `Climate Data Operators (CDO)
-          <https://code.zmaw.de/projects/cdo/embedded/index.html>`_ can work with
-          several input formats, stack them and change the chunking to allow time series
-          optimized access. It assumes regular sampling in space and time as far as we
-          know.
-        - `netCDF Operators (NCO) <http://nco.sourceforge.net/#Definition>`_ are similar
-          to CDO with a stronger focus on netCDF.
-        
-        Contribute
-        ==========
-        
-        We are happy if you want to contribute. Please raise an issue explaining what
-        is missing or if you find a bug. We will also gladly accept pull requests
-        against our master branch for new features or bug fixes.
-        
-        Development setup
-        -----------------
-        
-        For Development we recommend a ``conda`` environment
-        
-        Guidelines
-        ----------
-        
-        If you want to contribute please follow these steps:
-        
-        - Fork the repurpose repository to your account
-        - make a new feature branch from the repurpose master branch
-        - Add your feature
-        - Please include tests for your contributions in one of the test directories.
-          We use py.test so a simple function called test_my_feature is enough
-        - submit a pull request to our master branch
-        
-        Note
-        ====
-        
-        This project has been set up using PyScaffold 2.4.4. For details and usage
-        information on PyScaffold see http://pyscaffold.readthedocs.org/.
-        
 Platform: any
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python
 Requires-Python: >=3.6
 Description-Content-Type: text/x-rst; charset=UTF-8
 Provides-Extra: testing
+License-File: LICENSE.txt
+License-File: AUTHORS.rst
+
+=========
+repurpose
+=========
+
+.. image:: https://github.com/TUW-GEO/repurpose/workflows/Automated%20Tests/badge.svg?branch=master
+   :target: https://github.com/TUW-GEO/repurpose/actions
+
+.. image:: https://coveralls.io/repos/github/TUW-GEO/repurpose/badge.svg?branch=master
+   :target: https://coveralls.io/github/TUW-GEO/repurpose?branch=master
+
+.. image:: https://badge.fury.io/py/repurpose.svg
+    :target: http://badge.fury.io/py/repurpose
+
+.. image:: https://readthedocs.org/projects/repurpose/badge/?version=latest
+   :target: http://repurpose.readthedocs.org/
+
+
+This package provides routines for the conversion of image formats to time
+series and vice versa. It is part of the `poets project
+<http://tuw-geo.github.io/poets/>`_ and works best with the readers and writers
+supported there. The main use case is for data that is sampled irregularly in
+space or time. If you have data that is sampled in regular intervals then there
+are alternatives to this package which might be better for your use case. See
+`Alternatives`_ for more detail.
+
+The readers and writers have to conform to the API specifications of the base
+classes defined in `pygeobase <https://github.com/TUW-GEO/pygeobase>`_ to work
+without adpation.
+
+Citation
+========
+
+.. image:: https://zenodo.org/badge/DOI/10.5281/zenodo.593577.svg
+   :target: https://doi.org/10.5281/zenodo.593577
+
+If you use the software in a publication then please cite it using the Zenodo DOI.
+Be aware that this badge links to the latest package version.
+
+Please select your specific version at https://doi.org/10.5281/zenodo.593577 to get the DOI of that version.
+You should normally always use the DOI for the specific version of your record in citations.
+This is to ensure that other researchers can access the exact research artefact you used for reproducibility.
+
+You can find additional information regarding DOI versioning at http://help.zenodo.org/#versioning
+
+Installation
+============
+
+This package depends on the following libraries that can be installed via
+conda or mamba
+
+.. code::
+
+    conda install -c conda-forge numpy netCDF4 pyresample
+
+Afterwards you can install this package and its pip dependecies via:
+
+.. code::
+
+    pip install repurpose
+
+
+Modules
+=======
+
+It includes two main modules:
+
+- ``img2ts`` for image/swath to time series conversion, including support for
+  spatial resampling.
+- ``ts2img`` for time series to image conversion, including support for temporal
+  resampling. This module is very experimental at the moment.
+- ``resample`` for spatial resampling of (regular or irregular) gridded data to different resolutions.
+
+Alternatives
+============
+
+If you have data that can be represented as a 3D datacube then these projects
+might be better suited to your needs.
+
+- `PyReshaper <https://github.com/NCAR/PyReshaper>`_ is a package that works
+  with NetCDF input and output and converts time slices into a time series
+  representation.
+- `Climate Data Operators (CDO)
+  <https://code.zmaw.de/projects/cdo/embedded/index.html>`_ can work with
+  several input formats, stack them and change the chunking to allow time series
+  optimized access. It assumes regular sampling in space and time as far as we
+  know.
+- `netCDF Operators (NCO) <http://nco.sourceforge.net/#Definition>`_ are similar
+  to CDO with a stronger focus on netCDF.
+
+Contribute
+==========
+
+We are happy if you want to contribute. Please raise an issue explaining what
+is missing or if you find a bug. We will also gladly accept pull requests
+against our master branch for new features or bug fixes.
+
+Development setup
+-----------------
+
+For Development we recommend a ``conda`` environment
+
+Guidelines
+----------
+
+If you want to contribute please follow these steps:
+
+- Fork the repurpose repository to your account
+- make a new feature branch from the repurpose master branch
+- Add your feature
+- Please include tests for your contributions in one of the test directories.
+  We use py.test so a simple function called test_my_feature is enough
+- submit a pull request to our master branch
+
+Note
+====
+
+This project has been set up using PyScaffold 2.4.4. For details and usage
+information on PyScaffold see http://pyscaffold.readthedocs.org/.
```

### Comparing `repurpose-0.8/src/repurpose/img2ts.py` & `repurpose-0.9/src/repurpose/img2ts.py`

 * *Files 2% similar despite different names*

```diff
@@ -48,26 +48,16 @@
     to read all images between startdate and enddate and saves them
     in netCDF time series files according to the given netCDF class
     and the cell structure of the outputgrid
 
     Parameters
     ----------
     input_dataset : DatasetImgBase like class instance
-        must implement a daily_images iterator that yields
-        data : dict
-            dictionary of numpy arrays that hold the image data for each variable
-            of the dataset
-        timestamp : exact timestamp of the image
-        lon : numpy.array or None
-            array of longitudes, if None self.grid will be assumed
-        lat : numpy.array or None
-            array of latitudes, if None self.grid will be assumed
-        jd : numpy.array or None
-            array of observation times in julian days, if None all
-            observations have the same timestamp
+        must implement a ``read(date, **input_kwargs)`` iterator that returns a
+        `pygeobase.object_base.Image`.
     outputpath : string
         path where to save the time series to
     startdate : date
         date from which the time series should start. Of course images
         have to be available from this date onwards.
     enddate : date
         date when the time series should end. Images should be availabe
@@ -174,21 +164,16 @@
             self.resample = False
         else:
             # if input and target grid are not equal resampling is required
             if self.input_grid != self.target_grid:
                 self.resample = True
 
         # if the target grid is not a cell grid make it one
-        # default is just one cell for the
-        # this is just a dirty hack until grids have a method
-        # to check their grid type
-        if (type(self.target_grid) == grids.BasicGrid or
-            (pygeogrids.grids.BasicGrid in type(self.target_grid).__bases__ and
-             len(type(self.target_grid).__bases__))) == 1:
-
+        # default is just one cell for the entire grid
+        if not isinstance(self.target_grid, grids.CellGrid):
             self.target_grid = self.target_grid.to_cell_grid(cellsize_lat=cellsize_lat,
                                                              cellsize_lon=cellsize_lon)
         self.currentdate = startdate
         self.startdate = startdate
         self.enddate = enddate
         self.imgbuffer = imgbuffer
         self.outputpath = outputpath
@@ -283,18 +268,18 @@
                         dataout.add_global_attr(
                             'geospatial_lat_max', np.max(cell_lats))
                         dataout.add_global_attr(
                             'geospatial_lon_min', np.min(cell_lons))
                         dataout.add_global_attr(
                             'geospatial_lon_max', np.max(cell_lons))
 
-                        dataout.write_ts_all_loc(cell_gpis, data, dates,
-                                                 lons=cell_lons,
-                                                 lats=cell_lats,
-                                                 attributes=self.ts_attributes)
+                        dataout.write_all(cell_gpis, data, dates,
+                                          lons=cell_lons,
+                                          lats=cell_lats,
+                                          attributes=self.ts_attributes)
                 elif not self.orthogonal:
 
                     with nc.IndexedRaggedTs(os.path.join(self.outputpath,
                                                          self.filename_templ %
                                                          cell),
                                             n_loc=cell_gpis.size, mode='a',
                                             zlib=self.zlib,
```

### Comparing `repurpose-0.8/src/repurpose/ts2img.py` & `repurpose-0.9/src/repurpose/ts2img.py`

 * *Files 2% similar despite different names*

```diff
@@ -126,15 +126,15 @@
         gpi_bulk = []
         ts_bulk = {}
         ts_index = None
         if gpis is None:
             # get grid points can return either 3 or 4 values
             # depending on the grid type, gpis is the first in both cases
             gpi_info = list(self.tsreader.grid.grid_points())
-            gpis = np.array(gpi_info[0], dtype=np.int)
+            gpis = np.array(gpi_info[0], dtype=int)
         for gpi in gpis:
             gpi_bulk.append(gpi)
             ts = self.tsreader.read_ts(gpi)
             ts_agg = self.agg_func(ts, **tsaggkw)
             for column in ts_agg.columns:
                 try:
                     ts_bulk[column].append(ts_agg[column].values)
```

### Comparing `repurpose-0.8/src/repurpose/resample.py` & `repurpose-0.9/src/repurpose/resample.py`

 * *Files identical despite different names*

### Comparing `repurpose-0.8/src/repurpose.egg-info/PKG-INFO` & `repurpose-0.9/src/repurpose.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,126 +1,136 @@
 Metadata-Version: 2.1
 Name: repurpose
-Version: 0.8
+Version: 0.9
 Summary: Package for image to timeseries to image conversion
 Home-page: https://repurpose.readthedocs.io/en/latest/
 Author: TU Wien
 Author-email: remote.sensing@geo.tuwien.ac.at
 License: mit
 Project-URL: Documentation, https://repurpose.readthedocs.io/en/latest/
-Description: =========
-        repurpose
-        =========
-        
-        .. image:: https://travis-ci.org/TUW-GEO/repurpose.svg?branch=master
-            :target: https://travis-ci.org/TUW-GEO/repurpose
-        
-        .. image:: https://coveralls.io/repos/github/TUW-GEO/repurpose/badge.svg?branch=master
-           :target: https://coveralls.io/github/TUW-GEO/repurpose?branch=master
-        
-        .. image:: https://badge.fury.io/py/repurpose.svg
-            :target: http://badge.fury.io/py/repurpose
-        
-        .. image:: https://readthedocs.org/projects/repurpose/badge/?version=latest
-           :target: http://repurpose.readthedocs.org/
-        
-        
-        This package provides routines for the conversion of image formats to time
-        series and vice versa. It is part of the `poets project
-        <http://tuw-geo.github.io/poets/>`_ and works best with the readers and writers
-        supported there. The main use case is for data that is sampled irregularly in
-        space or time. If you have data that is sampled in regular intervals then there
-        are alternatives to this package which might be better for your use case. See
-        `Alternatives`_ for more detail.
-        
-        The readers and writers have to conform to the API specifications of the base
-        classes defined in `pygeobase <https://github.com/TUW-GEO/pygeobase>`_ to work
-        without adpation.
-        
-        Citation
-        ========
-        
-        .. image:: https://zenodo.org/badge/DOI/10.5281/zenodo.593577.svg
-           :target: https://doi.org/10.5281/zenodo.593577
-        
-        If you use the software in a publication then please cite it using the Zenodo DOI.
-        Be aware that this badge links to the latest package version.
-        
-        Please select your specific version at https://doi.org/10.5281/zenodo.593577 to get the DOI of that version.
-        You should normally always use the DOI for the specific version of your record in citations.
-        This is to ensure that other researchers can access the exact research artefact you used for reproducibility.
-        
-        You can find additional information regarding DOI versioning at http://help.zenodo.org/#versioning
-        
-        Installation
-        ============
-        
-        This package should be installable through pip:
-        
-        .. code::
-        
-            pip install repurpose
-        
-        Modules
-        =======
-        
-        It includes two main modules:
-        
-        - ``img2ts`` for image/swath to time series conversion, including support for
-          spatial resampling.
-        - ``ts2img`` for time series to image conversion, including support for temporal
-          resampling. This module is very experimental at the moment.
-        - ``resample`` for spatial resampling of (regular or irregular) gridded data to different resolutions.
-        
-        Alternatives
-        ============
-        
-        If you have data that can be represented as a 3D datacube then these projects
-        might be better suited to your needs.
-        
-        - `PyReshaper <https://github.com/NCAR/PyReshaper>`_ is a package that works
-          with NetCDF input and output and converts time slices into a time series
-          representation.
-        - `Climate Data Operators (CDO)
-          <https://code.zmaw.de/projects/cdo/embedded/index.html>`_ can work with
-          several input formats, stack them and change the chunking to allow time series
-          optimized access. It assumes regular sampling in space and time as far as we
-          know.
-        - `netCDF Operators (NCO) <http://nco.sourceforge.net/#Definition>`_ are similar
-          to CDO with a stronger focus on netCDF.
-        
-        Contribute
-        ==========
-        
-        We are happy if you want to contribute. Please raise an issue explaining what
-        is missing or if you find a bug. We will also gladly accept pull requests
-        against our master branch for new features or bug fixes.
-        
-        Development setup
-        -----------------
-        
-        For Development we recommend a ``conda`` environment
-        
-        Guidelines
-        ----------
-        
-        If you want to contribute please follow these steps:
-        
-        - Fork the repurpose repository to your account
-        - make a new feature branch from the repurpose master branch
-        - Add your feature
-        - Please include tests for your contributions in one of the test directories.
-          We use py.test so a simple function called test_my_feature is enough
-        - submit a pull request to our master branch
-        
-        Note
-        ====
-        
-        This project has been set up using PyScaffold 2.4.4. For details and usage
-        information on PyScaffold see http://pyscaffold.readthedocs.org/.
-        
 Platform: any
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python
 Requires-Python: >=3.6
 Description-Content-Type: text/x-rst; charset=UTF-8
 Provides-Extra: testing
+License-File: LICENSE.txt
+License-File: AUTHORS.rst
+
+=========
+repurpose
+=========
+
+.. image:: https://github.com/TUW-GEO/repurpose/workflows/Automated%20Tests/badge.svg?branch=master
+   :target: https://github.com/TUW-GEO/repurpose/actions
+
+.. image:: https://coveralls.io/repos/github/TUW-GEO/repurpose/badge.svg?branch=master
+   :target: https://coveralls.io/github/TUW-GEO/repurpose?branch=master
+
+.. image:: https://badge.fury.io/py/repurpose.svg
+    :target: http://badge.fury.io/py/repurpose
+
+.. image:: https://readthedocs.org/projects/repurpose/badge/?version=latest
+   :target: http://repurpose.readthedocs.org/
+
+
+This package provides routines for the conversion of image formats to time
+series and vice versa. It is part of the `poets project
+<http://tuw-geo.github.io/poets/>`_ and works best with the readers and writers
+supported there. The main use case is for data that is sampled irregularly in
+space or time. If you have data that is sampled in regular intervals then there
+are alternatives to this package which might be better for your use case. See
+`Alternatives`_ for more detail.
+
+The readers and writers have to conform to the API specifications of the base
+classes defined in `pygeobase <https://github.com/TUW-GEO/pygeobase>`_ to work
+without adpation.
+
+Citation
+========
+
+.. image:: https://zenodo.org/badge/DOI/10.5281/zenodo.593577.svg
+   :target: https://doi.org/10.5281/zenodo.593577
+
+If you use the software in a publication then please cite it using the Zenodo DOI.
+Be aware that this badge links to the latest package version.
+
+Please select your specific version at https://doi.org/10.5281/zenodo.593577 to get the DOI of that version.
+You should normally always use the DOI for the specific version of your record in citations.
+This is to ensure that other researchers can access the exact research artefact you used for reproducibility.
+
+You can find additional information regarding DOI versioning at http://help.zenodo.org/#versioning
+
+Installation
+============
+
+This package depends on the following libraries that can be installed via
+conda or mamba
+
+.. code::
+
+    conda install -c conda-forge numpy netCDF4 pyresample
+
+Afterwards you can install this package and its pip dependecies via:
+
+.. code::
+
+    pip install repurpose
+
+
+Modules
+=======
+
+It includes two main modules:
+
+- ``img2ts`` for image/swath to time series conversion, including support for
+  spatial resampling.
+- ``ts2img`` for time series to image conversion, including support for temporal
+  resampling. This module is very experimental at the moment.
+- ``resample`` for spatial resampling of (regular or irregular) gridded data to different resolutions.
+
+Alternatives
+============
+
+If you have data that can be represented as a 3D datacube then these projects
+might be better suited to your needs.
+
+- `PyReshaper <https://github.com/NCAR/PyReshaper>`_ is a package that works
+  with NetCDF input and output and converts time slices into a time series
+  representation.
+- `Climate Data Operators (CDO)
+  <https://code.zmaw.de/projects/cdo/embedded/index.html>`_ can work with
+  several input formats, stack them and change the chunking to allow time series
+  optimized access. It assumes regular sampling in space and time as far as we
+  know.
+- `netCDF Operators (NCO) <http://nco.sourceforge.net/#Definition>`_ are similar
+  to CDO with a stronger focus on netCDF.
+
+Contribute
+==========
+
+We are happy if you want to contribute. Please raise an issue explaining what
+is missing or if you find a bug. We will also gladly accept pull requests
+against our master branch for new features or bug fixes.
+
+Development setup
+-----------------
+
+For Development we recommend a ``conda`` environment
+
+Guidelines
+----------
+
+If you want to contribute please follow these steps:
+
+- Fork the repurpose repository to your account
+- make a new feature branch from the repurpose master branch
+- Add your feature
+- Please include tests for your contributions in one of the test directories.
+  We use py.test so a simple function called test_my_feature is enough
+- submit a pull request to our master branch
+
+Note
+====
+
+This project has been set up using PyScaffold 2.4.4. For details and usage
+information on PyScaffold see http://pyscaffold.readthedocs.org/.
```

### Comparing `repurpose-0.8/src/repurpose.egg-info/SOURCES.txt` & `repurpose-0.9/src/repurpose.egg-info/SOURCES.txt`

 * *Files 26% similar despite different names*

```diff
@@ -1,27 +1,28 @@
 .coveragerc
 .gitattributes
 .gitignore
-.travis.yml
+.readthedocs.yml
 AUTHORS.rst
 CHANGELOG.rst
 LICENSE.txt
 README.rst
 environment.yml
-readthedocs.yml
-requirements.txt
+pyproject.toml
 setup.cfg
 setup.py
+tox.ini
+.github/workflows/build.yml
 docs/Makefile
 docs/authors.rst
 docs/changelog.rst
 docs/conf.py
 docs/index.rst
 docs/license.rst
-docs/requirements.txt
+docs/readme.rst
 docs/resample.rst
 docs/ts2img.rst
 docs/_static/.gitignore
 src/repurpose/__init__.py
 src/repurpose/img2ts.py
 src/repurpose/resample.py
 src/repurpose/ts2img.py
```

### Comparing `repurpose-0.8/.gitignore` & `repurpose-0.9/.gitignore`

 * *Files identical despite different names*

### Comparing `repurpose-0.8/setup.cfg` & `repurpose-0.9/setup.cfg`

 * *Files 12% similar despite different names*

```diff
@@ -12,20 +12,26 @@
 platforms = any
 classifiers = 
 	Development Status :: 4 - Beta
 	Programming Language :: Python
 
 [options]
 zip_safe = False
-packages = find:
+packages = find_namespace:
 include_package_data = True
 package_dir = 
 	=src
-setup_requires = pyscaffold>=3.2a0,<3.3a0
-install_requires = numpy; pygeogrids; pynetcf; pyresample; more_itertools
+install_requires = 
+	importlib-metadata; python_version<"3.8"
+	numpy
+	pygeogrids>=0.1.3
+	netCDF4
+	pynetcf
+	pyresample
+	more_itertools
 python_requires = >=3.6
 
 [options.packages.find]
 where = src
 exclude = 
 	tests
 
@@ -68,16 +74,21 @@
 	.tox
 	build
 	dist
 	.eggs
 	docs/conf.py
 
 [pyscaffold]
-version = 3.2.3
+version = 4.4
 package = repurpose
 extensions = 
 	no_skeleton
 
+[yapf]
+based_on_style = yapf
+indent_width = 4
+column_limit = 79
+
 [egg_info]
 tag_build = 
 tag_date = 0
```

### Comparing `repurpose-0.8/.coveragerc` & `repurpose-0.9/.coveragerc`

 * *Files identical despite different names*

### Comparing `repurpose-0.8/README.rst` & `repurpose-0.9/README.rst`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 =========
 repurpose
 =========
 
-.. image:: https://travis-ci.org/TUW-GEO/repurpose.svg?branch=master
-    :target: https://travis-ci.org/TUW-GEO/repurpose
+.. image:: https://github.com/TUW-GEO/repurpose/workflows/Automated%20Tests/badge.svg?branch=master
+   :target: https://github.com/TUW-GEO/repurpose/actions
 
 .. image:: https://coveralls.io/repos/github/TUW-GEO/repurpose/badge.svg?branch=master
    :target: https://coveralls.io/github/TUW-GEO/repurpose?branch=master
 
 .. image:: https://badge.fury.io/py/repurpose.svg
     :target: http://badge.fury.io/py/repurpose
 
@@ -41,20 +41,28 @@
 This is to ensure that other researchers can access the exact research artefact you used for reproducibility.
 
 You can find additional information regarding DOI versioning at http://help.zenodo.org/#versioning
 
 Installation
 ============
 
-This package should be installable through pip:
+This package depends on the following libraries that can be installed via
+conda or mamba
+
+.. code::
+
+    conda install -c conda-forge numpy netCDF4 pyresample
+
+Afterwards you can install this package and its pip dependecies via:
 
 .. code::
 
     pip install repurpose
 
+
 Modules
 =======
 
 It includes two main modules:
 
 - ``img2ts`` for image/swath to time series conversion, including support for
   spatial resampling.
```

### Comparing `repurpose-0.8/tests/test_img2ts.py` & `repurpose-0.9/tests/test_img2ts.py`

 * *Files 4% similar despite different names*

```diff
@@ -110,58 +110,62 @@
         return timestamps
 
 
 def test_img2ts_daily_no_resampling():
     input_grid = BasicGrid(np.array([0.5, 0.5, -0.5, -0.5]),
                            np.array([1, -1, 1, -1]), )
 
-    outputpath = tempfile.mkdtemp()
-    start = datetime(2014, 2, 5)
-    end = datetime(2014, 4, 21)
-
-    ds_in = TestMultiTemporalImageDatasetDaily()
-    img2ts = Img2Ts(ds_in,
-                    outputpath, start, end, imgbuffer=15,
-                    input_grid=input_grid)
-
-    ts_should = np.concatenate([np.arange(5, 29, dtype=np.float),
-                                np.arange(1, 32, dtype=np.float),
-                                np.arange(1, 22, dtype=np.float)])
-    dates_should = ds_in.tstamps_for_daterange(start, end)
-    img2ts.calc()
-    ts_file = os.path.join(outputpath, '0000.nc')
-    with OrthoMultiTs(ts_file) as ds:
-        ts = ds.read_ts('var1', 0)
-        nptest.assert_allclose(ts['var1'], ts_should)
-        assert dates_should == list(ts['time'])
-        nptest.assert_allclose(ds.dataset.variables['location_id'][:],
-                               np.array([0, 1, 2, 3]))
+    with tempfile.TemporaryDirectory() as outputpath:
+        start = datetime(2014, 2, 5)
+        end = datetime(2014, 4, 21)
+
+        ds_in = TestMultiTemporalImageDatasetDaily()
+        img2ts = Img2Ts(ds_in,
+                        outputpath, start, end, imgbuffer=15,
+                        input_grid=input_grid)
+
+        ts_should = np.concatenate([np.arange(5, 29, dtype=float),
+                                    np.arange(1, 32, dtype=float),
+                                    np.arange(1, 22, dtype=float)])
+        dates_should = ds_in.tstamps_for_daterange(start, end)
+        img2ts.calc()
+        ts_file = os.path.join(outputpath, '0000.nc')
+        with OrthoMultiTs(ts_file) as ds:
+            ts = ds.read('var1', 0)
+            nptest.assert_allclose(ts['var1'], ts_should)
+            assert dates_should == list(ts['time'])
+            nptest.assert_allclose(ds.dataset.variables['location_id'][:],
+                                   np.array([0, 1, 2, 3]))
+        ds_in.close()
 
 
 def test_img2ts_daily_no_resampling_missing_day():
     """
     Test resampling over missing day 2016-01-01 (see reader above)
     """
     input_grid = BasicGrid(np.array([0.5, 0.5, -0.5, -0.5]),
                            np.array([1, -1, 1, -1]), )
 
-    outputpath = tempfile.mkdtemp()
-    start = datetime(2015, 12, 5)
-    end = datetime(2016, 1, 10)
-
-    ds_in = TestMultiTemporalImageDatasetDaily()
-    img2ts = Img2Ts(ds_in,
-                    outputpath, start, end, imgbuffer=15,
-                    input_grid=input_grid)
-
-    ts_should = np.concatenate([np.arange(5, 32, dtype=np.float),
-                                np.arange(2, 11, dtype=np.float)])
-    dates_should = ds_in.tstamps_for_daterange(start, end)
-    dates_should.remove(datetime(2016, 1, 1))
-    img2ts.calc()
-    ts_file = os.path.join(outputpath, '0000.nc')
-    with OrthoMultiTs(ts_file) as ds:
-        ts = ds.read_ts('var1', 0)
-        nptest.assert_allclose(ts['var1'], ts_should)
-        assert dates_should == list(ts['time'])
-        nptest.assert_allclose(ds.dataset.variables['location_id'][:],
-                               np.array([0, 1, 2, 3]))
+    with tempfile.TemporaryDirectory() as outputpath:
+        start = datetime(2015, 12, 5)
+        end = datetime(2016, 1, 10)
+
+        ds_in = TestMultiTemporalImageDatasetDaily()
+        img2ts = Img2Ts(ds_in,
+                        outputpath, start, end, imgbuffer=15,
+                        input_grid=input_grid)
+
+        ts_should = np.concatenate([np.arange(5, 32, dtype=float),
+                                    np.arange(2, 11, dtype=float)])
+        dates_should = ds_in.tstamps_for_daterange(start, end)
+        dates_should.remove(datetime(2016, 1, 1))
+        img2ts.calc()
+        ts_file = os.path.join(outputpath, '0000.nc')
+        with OrthoMultiTs(ts_file) as ds:
+            ts = ds.read('var1', 0)
+            nptest.assert_allclose(ts['var1'], ts_should)
+            assert dates_should == list(ts['time'])
+            nptest.assert_allclose(ds.dataset.variables['location_id'][:],
+                                   np.array([0, 1, 2, 3]))
+
+if __name__ == '__main__':
+    test_img2ts_daily_no_resampling()
```

### Comparing `repurpose-0.8/tests/test_resample.py` & `repurpose-0.9/tests/test_resample.py`

 * *Files identical despite different names*

### Comparing `repurpose-0.8/tests/test_ts2img.py` & `repurpose-0.9/tests/test_ts2img.py`

 * *Files identical despite different names*

