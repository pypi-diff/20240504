# Comparing `tmp/texplot-0.0.1.tar.gz` & `tmp/texplot-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "texplot-0.0.1.tar", last modified: Sun Apr 21 03:25:44 2024, max compression
+gzip compressed data, was "texplot-0.0.2.tar", last modified: Fri May  3 22:08:45 2024, max compression
```

## Comparing `texplot-0.0.1.tar` & `texplot-0.0.2.tar`

### file list

```diff
@@ -1,20 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 03:25:44.277705 texplot-0.0.1/
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-21 03:25:40.000000 texplot-0.0.1/AUTHORS.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1036 2024-04-21 03:25:40.000000 texplot-0.0.1/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)       84 2024-04-21 03:25:40.000000 texplot-0.0.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)      275 2024-04-21 03:25:44.277705 texplot-0.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-21 03:25:40.000000 texplot-0.0.1/README.rst
--rw-r--r--   0 runner    (1001) docker     (127)       81 2024-04-21 03:25:40.000000 texplot-0.0.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-21 03:25:40.000000 texplot-0.0.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)      503 2024-04-21 03:25:44.277705 texplot-0.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      308 2024-04-21 03:25:40.000000 texplot-0.0.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 03:25:44.277705 texplot-0.0.1/texplot/
--rw-r--r--   0 runner    (1001) docker     (127)      522 2024-04-21 03:25:40.000000 texplot-0.0.1/texplot/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      389 2024-04-21 03:25:40.000000 texplot-0.0.1/texplot/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)      947 2024-04-21 03:25:40.000000 texplot-0.0.1/texplot/display_utilities.py
--rw-r--r--   0 runner    (1001) docker     (127)    15430 2024-04-21 03:25:40.000000 texplot-0.0.1/texplot/plot_utilities.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 03:25:44.277705 texplot-0.0.1/texplot.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      275 2024-04-21 03:25:44.000000 texplot-0.0.1/texplot.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      316 2024-04-21 03:25:44.000000 texplot-0.0.1/texplot.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-21 03:25:44.000000 texplot-0.0.1/texplot.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-21 03:25:44.000000 texplot-0.0.1/texplot.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 22:08:45.716941 texplot-0.0.2/
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-05-03 22:08:40.000000 texplot-0.0.2/AUTHORS.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1036 2024-05-03 22:08:40.000000 texplot-0.0.2/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      457 2024-05-03 22:08:40.000000 texplot-0.0.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    12359 2024-05-03 22:08:45.716941 texplot-0.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     9900 2024-05-03 22:08:40.000000 texplot-0.0.2/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       81 2024-05-03 22:08:40.000000 texplot-0.0.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-03 22:08:40.000000 texplot-0.0.2/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      503 2024-05-03 22:08:45.716941 texplot-0.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     5292 2024-05-03 22:08:40.000000 texplot-0.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 22:08:45.712941 texplot-0.0.2/texplot/
+-rw-r--r--   0 runner    (1001) docker     (127)      687 2024-05-03 22:08:40.000000 texplot-0.0.2/texplot/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      389 2024-05-03 22:08:40.000000 texplot-0.0.2/texplot/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-03 22:08:40.000000 texplot-0.0.2/texplot/__version__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      947 2024-05-03 22:08:40.000000 texplot-0.0.2/texplot/display_utilities.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 22:08:45.712941 texplot-0.0.2/texplot/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)      572 2024-05-03 22:08:40.000000 texplot-0.0.2/texplot/examples/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1329 2024-05-03 22:08:40.000000 texplot-0.0.2/texplot/examples/plot_bifurcation_diagram.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1250 2024-05-03 22:08:40.000000 texplot-0.0.2/texplot/examples/plot_function.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5006 2024-05-03 22:08:40.000000 texplot-0.0.2/texplot/examples/plot_lorenz.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15455 2024-05-03 22:08:40.000000 texplot-0.0.2/texplot/plot_utilities.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 22:08:45.712941 texplot-0.0.2/texplot.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    12359 2024-05-03 22:08:45.000000 texplot-0.0.2/texplot.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      573 2024-05-03 22:08:45.000000 texplot-0.0.2/texplot.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-03 22:08:45.000000 texplot-0.0.2/texplot.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       92 2024-05-03 22:08:45.000000 texplot-0.0.2/texplot.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-03 22:08:45.000000 texplot-0.0.2/texplot.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      311 2024-05-03 22:08:45.000000 texplot-0.0.2/texplot.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-03 22:08:45.000000 texplot-0.0.2/texplot.egg-info/top_level.txt
```

### Comparing `texplot-0.0.1/LICENSE.txt` & `texplot-0.0.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `texplot-0.0.1/texplot/display_utilities.py` & `texplot-0.0.2/texplot/display_utilities.py`

 * *Files identical despite different names*

### Comparing `texplot-0.0.1/texplot/plot_utilities.py` & `texplot-0.0.2/texplot/plot_utilities.py`

 * *Files 2% similar despite different names*

```diff
@@ -238,22 +238,26 @@
         context="notebook",
         font_scale=1,
         use_latex=True,
         rc=None):
     """
     Returns a dictionary that can be used to update plt.rcParams.
 
-    Usage:
+    Example
+    =======
+
     Before a function, add this line:
 
-    @matplotlib.rc_context(get_theme(font_scale=1.2))
-    def some_plotting_function():
-        ...
+    .. code-block:: python
+
+        >>> @matplotlib.rc_context(get_theme(font_scale=1.2))
+        >>> def some_plotting_function():
+        >>>     ...
 
-        plot.show()
+        >>> plot.show()
 
     Note that the plot.show() must be within the "context" (meaning the scope)
     of the above rc_context declaration. That is, if plt.show() is postponed
     to be a global plt.show() outside of the above function, the matplotlib
     parameter settings will be set back to their defaults. Hence, make sure to
     plot within the scope of the intended function where the rcParams context
     is customized.
@@ -392,24 +396,23 @@
 
         # Determine whether a file extension is provided or not.
         if bool(extension):
             # filename contains an extension
             extensions = [extension]
         else:
             # No extension is provided. Save to both svg and pdf
-            extensions = ['svg', 'pdf']
+            extensions = ['.svg', '.pdf']
 
     if not os.access(directory, os.W_OK):
         raise RuntimeError(
             'Cannot save plot to %s. Directory is not writable.' % directory)
 
     # For each extension, save a file
     for extension in extensions:
-        fullpath_filename = os.path.join(directory,
-                                         base_filename + '.' + extension)
+        fullpath_filename = os.path.join(directory, base_filename + extension)
 
         plt.savefig(
                 fullpath_filename, dpi=dpi,
                 transparent=transparent_background,
                 bbox_extra_artists=bbox_extra_artists, bbox_inches='tight')
 
         if verbose:
```

