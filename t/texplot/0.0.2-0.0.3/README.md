# Comparing `tmp/texplot-0.0.2.tar.gz` & `tmp/texplot-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "texplot-0.0.2.tar", last modified: Fri May  3 22:08:45 2024, max compression
+gzip compressed data, was "texplot-0.0.3.tar", last modified: Fri May  3 22:26:12 2024, max compression
```

## Comparing `texplot-0.0.2.tar` & `texplot-0.0.3.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 22:08:45.716941 texplot-0.0.2/
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-05-03 22:08:40.000000 texplot-0.0.2/AUTHORS.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1036 2024-05-03 22:08:40.000000 texplot-0.0.2/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)      457 2024-05-03 22:08:40.000000 texplot-0.0.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    12359 2024-05-03 22:08:45.716941 texplot-0.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     9900 2024-05-03 22:08:40.000000 texplot-0.0.2/README.rst
--rw-r--r--   0 runner    (1001) docker     (127)       81 2024-05-03 22:08:40.000000 texplot-0.0.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-03 22:08:40.000000 texplot-0.0.2/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)      503 2024-05-03 22:08:45.716941 texplot-0.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     5292 2024-05-03 22:08:40.000000 texplot-0.0.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 22:08:45.712941 texplot-0.0.2/texplot/
--rw-r--r--   0 runner    (1001) docker     (127)      687 2024-05-03 22:08:40.000000 texplot-0.0.2/texplot/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      389 2024-05-03 22:08:40.000000 texplot-0.0.2/texplot/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-03 22:08:40.000000 texplot-0.0.2/texplot/__version__.py
--rw-r--r--   0 runner    (1001) docker     (127)      947 2024-05-03 22:08:40.000000 texplot-0.0.2/texplot/display_utilities.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 22:08:45.712941 texplot-0.0.2/texplot/examples/
--rw-r--r--   0 runner    (1001) docker     (127)      572 2024-05-03 22:08:40.000000 texplot-0.0.2/texplot/examples/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1329 2024-05-03 22:08:40.000000 texplot-0.0.2/texplot/examples/plot_bifurcation_diagram.py
--rw-r--r--   0 runner    (1001) docker     (127)     1250 2024-05-03 22:08:40.000000 texplot-0.0.2/texplot/examples/plot_function.py
--rw-r--r--   0 runner    (1001) docker     (127)     5006 2024-05-03 22:08:40.000000 texplot-0.0.2/texplot/examples/plot_lorenz.py
--rw-r--r--   0 runner    (1001) docker     (127)    15455 2024-05-03 22:08:40.000000 texplot-0.0.2/texplot/plot_utilities.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 22:08:45.712941 texplot-0.0.2/texplot.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    12359 2024-05-03 22:08:45.000000 texplot-0.0.2/texplot.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      573 2024-05-03 22:08:45.000000 texplot-0.0.2/texplot.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-03 22:08:45.000000 texplot-0.0.2/texplot.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       92 2024-05-03 22:08:45.000000 texplot-0.0.2/texplot.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-03 22:08:45.000000 texplot-0.0.2/texplot.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      311 2024-05-03 22:08:45.000000 texplot-0.0.2/texplot.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-03 22:08:45.000000 texplot-0.0.2/texplot.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 22:26:12.153371 texplot-0.0.3/
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-05-03 22:26:07.000000 texplot-0.0.3/AUTHORS.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1036 2024-05-03 22:26:07.000000 texplot-0.0.3/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      457 2024-05-03 22:26:07.000000 texplot-0.0.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    12567 2024-05-03 22:26:12.153371 texplot-0.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    10108 2024-05-03 22:26:07.000000 texplot-0.0.3/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       81 2024-05-03 22:26:07.000000 texplot-0.0.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-03 22:26:07.000000 texplot-0.0.3/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      503 2024-05-03 22:26:12.153371 texplot-0.0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     5292 2024-05-03 22:26:07.000000 texplot-0.0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 22:26:12.145372 texplot-0.0.3/texplot/
+-rw-r--r--   0 runner    (1001) docker     (127)      687 2024-05-03 22:26:07.000000 texplot-0.0.3/texplot/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      389 2024-05-03 22:26:07.000000 texplot-0.0.3/texplot/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-03 22:26:07.000000 texplot-0.0.3/texplot/__version__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      947 2024-05-03 22:26:07.000000 texplot-0.0.3/texplot/display_utilities.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 22:26:12.149371 texplot-0.0.3/texplot/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)      572 2024-05-03 22:26:07.000000 texplot-0.0.3/texplot/examples/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1329 2024-05-03 22:26:07.000000 texplot-0.0.3/texplot/examples/plot_bifurcation_diagram.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1250 2024-05-03 22:26:07.000000 texplot-0.0.3/texplot/examples/plot_function.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5006 2024-05-03 22:26:07.000000 texplot-0.0.3/texplot/examples/plot_lorenz.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15455 2024-05-03 22:26:07.000000 texplot-0.0.3/texplot/plot_utilities.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 22:26:12.149371 texplot-0.0.3/texplot.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    12567 2024-05-03 22:26:12.000000 texplot-0.0.3/texplot.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      573 2024-05-03 22:26:12.000000 texplot-0.0.3/texplot.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-03 22:26:12.000000 texplot-0.0.3/texplot.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       92 2024-05-03 22:26:12.000000 texplot-0.0.3/texplot.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-03 22:26:12.000000 texplot-0.0.3/texplot.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      311 2024-05-03 22:26:12.000000 texplot-0.0.3/texplot.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-03 22:26:12.000000 texplot-0.0.3/texplot.egg-info/top_level.txt
```

### Comparing `texplot-0.0.2/LICENSE.txt` & `texplot-0.0.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `texplot-0.0.2/PKG-INFO` & `texplot-0.0.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: texplot
-Version: 0.0.2
+Version: 0.0.3
 Summary: Enhance your matplotlib plots with publication-quality style
 Home-page: https://github.com/ameli/texplot
 Download-URL: https://github.com/ameli/texplot/archive/main.zip
 Author: Siavash Ameli
 Author-email: sameli@berkeley.edu
 Project-URL: Documentation, https://github.com/ameli/texplot/blob/main/README.rst
 Project-URL: Source, https://github.com/ameli/texplot
@@ -65,14 +65,15 @@
 
 Links
 =====
 
 * `Documentation <https://ameli.github.io/texplot>`__
 * `PyPI <https://pypi.org/project/texplot/>`__
 * `Anaconda <https://anaconda.org/s-ameli/texplot>`__
+* `Github <https://github.com/ameli/texplot>`__
 
 Install
 =======
 
 This package requires :math:`\LaTeX` to be installed. Ensure that the ``latex`` executable is available on your system's ``PATH``.
 
 Install with ``pip``
@@ -87,15 +88,15 @@
 Install with ``conda``
 ----------------------
 
 |conda-version|
 
 ::
 
-    conda install -c s-ameli texplot
+    conda install s-ameli::texplot
 
 Set Theme
 =========
 
 `texplot` can set theme either globally or locally:
 
 Set Theme Globally
@@ -110,15 +111,15 @@
     >>> texplot.set_theme()
 
     >>> # Plot an example function
     >>> fig, ax = plt.subplots()
     >>> texplot.examples.plot_function(ax)
     >>> plt.show()
 
-.. figure:: /docs/source/_static/images/plots/function.png
+.. figure:: https://github.com/ameli/texplot/raw/main/docs/source/_static/images/plots/function.png
    :align: left
    :figwidth: 100%
    :width: 100%
 
 The theme set as described above will affect your entire Python script for its duration. However, you can revert to the default *matplotlib* theme at any time by calling the `texplot.reset_theme <https://ameli.github.io/texplot/generated/texplot.reset_theme.html#texplot.reset_theme>`__ function as shown below:
 
 .. code-block:: python
@@ -127,15 +128,15 @@
     >>> texplot.reset_theme()
 
     >>> # Plot another example function
     >>> fig2, ax2 = plt.subplots()
     >>> texplot.examples.plot_function(ax2)
     >>> plt.show()
 
-.. figure:: /docs/source/_static/images/plots/function_no_theme.png
+.. figure:: https://github.com/ameli/texplot/raw/main/docs/source/_static/images/plots/function_no_theme.png
    :align: left
    :figwidth: 100%
    :width: 100%
 
 
 Set Theme Within a Local Scope
 ------------------------------
@@ -207,15 +208,15 @@
     ...         font_scale=1.2):
     >>>
     >>>     # Plot an example diagram
     >>>     fig, ax = plt.subplots()
     >>>     texplot.examples.plot_bifurcation_diagram(ax)
     >>>     plt.show()
 
-.. figure:: ./docs/source/_static/images/plots/logistic.png
+.. figure:: https://github.com/ameli/texplot/raw/main/docs/source/_static/images/plots/logistic.png
    :align: left
    :figwidth: 100%
    :width: 100%
 
 Show and Save Plots
 ===================
 
@@ -234,15 +235,15 @@
     >>>
     >>>     # Show and save plot
     >>>     texplot.show_or_save_plot(plt, default_filename='lorenz.pdf',
     ...                               transparent_background=True, dpi=200,
     ...                               show_and_save=True, verbose=True)
     plot saved to '/home/user/lorenz.pdf'.
 
-.. figure:: ./docs/source/_static/images/plots/lorenz.png
+.. figure:: https://github.com/ameli/texplot/raw/main/docs/source/_static/images/plots/lorenz.png
    :align: left
    :figwidth: 100%
    :width: 100%
 
 Test Package
 ============
```

### Comparing `texplot-0.0.2/README.rst` & `texplot-0.0.3/README.rst`

 * *Files 3% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 
 Links
 =====
 
 * `Documentation <https://ameli.github.io/texplot>`__
 * `PyPI <https://pypi.org/project/texplot/>`__
 * `Anaconda <https://anaconda.org/s-ameli/texplot>`__
+* `Github <https://github.com/ameli/texplot>`__
 
 Install
 =======
 
 This package requires :math:`\LaTeX` to be installed. Ensure that the ``latex`` executable is available on your system's ``PATH``.
 
 Install with ``pip``
@@ -29,15 +30,15 @@
 Install with ``conda``
 ----------------------
 
 |conda-version|
 
 ::
 
-    conda install -c s-ameli texplot
+    conda install s-ameli::texplot
 
 Set Theme
 =========
 
 `texplot` can set theme either globally or locally:
 
 Set Theme Globally
@@ -52,15 +53,15 @@
     >>> texplot.set_theme()
 
     >>> # Plot an example function
     >>> fig, ax = plt.subplots()
     >>> texplot.examples.plot_function(ax)
     >>> plt.show()
 
-.. figure:: /docs/source/_static/images/plots/function.png
+.. figure:: https://github.com/ameli/texplot/raw/main/docs/source/_static/images/plots/function.png
    :align: left
    :figwidth: 100%
    :width: 100%
 
 The theme set as described above will affect your entire Python script for its duration. However, you can revert to the default *matplotlib* theme at any time by calling the `texplot.reset_theme <https://ameli.github.io/texplot/generated/texplot.reset_theme.html#texplot.reset_theme>`__ function as shown below:
 
 .. code-block:: python
@@ -69,15 +70,15 @@
     >>> texplot.reset_theme()
 
     >>> # Plot another example function
     >>> fig2, ax2 = plt.subplots()
     >>> texplot.examples.plot_function(ax2)
     >>> plt.show()
 
-.. figure:: /docs/source/_static/images/plots/function_no_theme.png
+.. figure:: https://github.com/ameli/texplot/raw/main/docs/source/_static/images/plots/function_no_theme.png
    :align: left
    :figwidth: 100%
    :width: 100%
 
 
 Set Theme Within a Local Scope
 ------------------------------
@@ -149,15 +150,15 @@
     ...         font_scale=1.2):
     >>>
     >>>     # Plot an example diagram
     >>>     fig, ax = plt.subplots()
     >>>     texplot.examples.plot_bifurcation_diagram(ax)
     >>>     plt.show()
 
-.. figure:: ./docs/source/_static/images/plots/logistic.png
+.. figure:: https://github.com/ameli/texplot/raw/main/docs/source/_static/images/plots/logistic.png
    :align: left
    :figwidth: 100%
    :width: 100%
 
 Show and Save Plots
 ===================
 
@@ -176,15 +177,15 @@
     >>>
     >>>     # Show and save plot
     >>>     texplot.show_or_save_plot(plt, default_filename='lorenz.pdf',
     ...                               transparent_background=True, dpi=200,
     ...                               show_and_save=True, verbose=True)
     plot saved to '/home/user/lorenz.pdf'.
 
-.. figure:: ./docs/source/_static/images/plots/lorenz.png
+.. figure:: https://github.com/ameli/texplot/raw/main/docs/source/_static/images/plots/lorenz.png
    :align: left
    :figwidth: 100%
    :width: 100%
 
 Test Package
 ============
```

### Comparing `texplot-0.0.2/setup.py` & `texplot-0.0.3/setup.py`

 * *Files identical despite different names*

### Comparing `texplot-0.0.2/texplot/__init__.py` & `texplot-0.0.3/texplot/__init__.py`

 * *Files identical despite different names*

### Comparing `texplot-0.0.2/texplot/display_utilities.py` & `texplot-0.0.3/texplot/display_utilities.py`

 * *Files identical despite different names*

### Comparing `texplot-0.0.2/texplot/examples/__init__.py` & `texplot-0.0.3/texplot/examples/__init__.py`

 * *Files identical despite different names*

### Comparing `texplot-0.0.2/texplot/examples/plot_bifurcation_diagram.py` & `texplot-0.0.3/texplot/examples/plot_bifurcation_diagram.py`

 * *Files identical despite different names*

### Comparing `texplot-0.0.2/texplot/examples/plot_function.py` & `texplot-0.0.3/texplot/examples/plot_function.py`

 * *Files identical despite different names*

### Comparing `texplot-0.0.2/texplot/examples/plot_lorenz.py` & `texplot-0.0.3/texplot/examples/plot_lorenz.py`

 * *Files identical despite different names*

### Comparing `texplot-0.0.2/texplot/plot_utilities.py` & `texplot-0.0.3/texplot/plot_utilities.py`

 * *Files identical despite different names*

### Comparing `texplot-0.0.2/texplot.egg-info/PKG-INFO` & `texplot-0.0.3/texplot.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: texplot
-Version: 0.0.2
+Version: 0.0.3
 Summary: Enhance your matplotlib plots with publication-quality style
 Home-page: https://github.com/ameli/texplot
 Download-URL: https://github.com/ameli/texplot/archive/main.zip
 Author: Siavash Ameli
 Author-email: sameli@berkeley.edu
 Project-URL: Documentation, https://github.com/ameli/texplot/blob/main/README.rst
 Project-URL: Source, https://github.com/ameli/texplot
@@ -65,14 +65,15 @@
 
 Links
 =====
 
 * `Documentation <https://ameli.github.io/texplot>`__
 * `PyPI <https://pypi.org/project/texplot/>`__
 * `Anaconda <https://anaconda.org/s-ameli/texplot>`__
+* `Github <https://github.com/ameli/texplot>`__
 
 Install
 =======
 
 This package requires :math:`\LaTeX` to be installed. Ensure that the ``latex`` executable is available on your system's ``PATH``.
 
 Install with ``pip``
@@ -87,15 +88,15 @@
 Install with ``conda``
 ----------------------
 
 |conda-version|
 
 ::
 
-    conda install -c s-ameli texplot
+    conda install s-ameli::texplot
 
 Set Theme
 =========
 
 `texplot` can set theme either globally or locally:
 
 Set Theme Globally
@@ -110,15 +111,15 @@
     >>> texplot.set_theme()
 
     >>> # Plot an example function
     >>> fig, ax = plt.subplots()
     >>> texplot.examples.plot_function(ax)
     >>> plt.show()
 
-.. figure:: /docs/source/_static/images/plots/function.png
+.. figure:: https://github.com/ameli/texplot/raw/main/docs/source/_static/images/plots/function.png
    :align: left
    :figwidth: 100%
    :width: 100%
 
 The theme set as described above will affect your entire Python script for its duration. However, you can revert to the default *matplotlib* theme at any time by calling the `texplot.reset_theme <https://ameli.github.io/texplot/generated/texplot.reset_theme.html#texplot.reset_theme>`__ function as shown below:
 
 .. code-block:: python
@@ -127,15 +128,15 @@
     >>> texplot.reset_theme()
 
     >>> # Plot another example function
     >>> fig2, ax2 = plt.subplots()
     >>> texplot.examples.plot_function(ax2)
     >>> plt.show()
 
-.. figure:: /docs/source/_static/images/plots/function_no_theme.png
+.. figure:: https://github.com/ameli/texplot/raw/main/docs/source/_static/images/plots/function_no_theme.png
    :align: left
    :figwidth: 100%
    :width: 100%
 
 
 Set Theme Within a Local Scope
 ------------------------------
@@ -207,15 +208,15 @@
     ...         font_scale=1.2):
     >>>
     >>>     # Plot an example diagram
     >>>     fig, ax = plt.subplots()
     >>>     texplot.examples.plot_bifurcation_diagram(ax)
     >>>     plt.show()
 
-.. figure:: ./docs/source/_static/images/plots/logistic.png
+.. figure:: https://github.com/ameli/texplot/raw/main/docs/source/_static/images/plots/logistic.png
    :align: left
    :figwidth: 100%
    :width: 100%
 
 Show and Save Plots
 ===================
 
@@ -234,15 +235,15 @@
     >>>
     >>>     # Show and save plot
     >>>     texplot.show_or_save_plot(plt, default_filename='lorenz.pdf',
     ...                               transparent_background=True, dpi=200,
     ...                               show_and_save=True, verbose=True)
     plot saved to '/home/user/lorenz.pdf'.
 
-.. figure:: ./docs/source/_static/images/plots/lorenz.png
+.. figure:: https://github.com/ameli/texplot/raw/main/docs/source/_static/images/plots/lorenz.png
    :align: left
    :figwidth: 100%
    :width: 100%
 
 Test Package
 ============
```

### Comparing `texplot-0.0.2/texplot.egg-info/SOURCES.txt` & `texplot-0.0.3/texplot.egg-info/SOURCES.txt`

 * *Files identical despite different names*

