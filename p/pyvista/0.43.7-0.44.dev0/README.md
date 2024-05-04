# Comparing `tmp/pyvista-0.43.7.tar.gz` & `tmp/pyvista-0.44.dev0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyvista-0.43.7.tar", last modified: Sat May  4 07:48:39 2024, max compression
+gzip compressed data, was "pyvista-0.44.dev0.tar", last modified: Tue Feb  6 10:39:19 2024, max compression
```

## Comparing `pyvista-0.43.7.tar` & `pyvista-0.44.dev0.tar`

### file list

```diff
@@ -1,184 +1,184 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 07:48:39.560978 pyvista-0.43.7/
--rw-r--r--   0 runner    (1001) docker     (127)     1932 2024-05-04 07:37:21.000000 pyvista-0.43.7/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1088 2024-05-04 07:37:21.000000 pyvista-0.43.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      158 2024-05-04 07:37:21.000000 pyvista-0.43.7/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    14665 2024-05-04 07:48:39.560978 pyvista-0.43.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    12681 2024-05-04 07:37:21.000000 pyvista-0.43.7/README.rst
--rw-r--r--   0 runner    (1001) docker     (127)     8460 2024-05-04 07:37:21.000000 pyvista-0.43.7/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 07:48:39.532978 pyvista-0.43.7/pyvista/
--rwxr-xr-x   0 runner    (1001) docker     (127)     2792 2024-05-04 07:37:21.000000 pyvista-0.43.7/pyvista/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9759 2024-05-04 07:37:21.000000 pyvista-0.43.7/pyvista/_plot.py
--rw-r--r--   0 runner    (1001) docker     (127)      400 2024-05-04 07:37:21.000000 pyvista-0.43.7/pyvista/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)      478 2024-05-04 07:37:21.000000 pyvista-0.43.7/pyvista/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 07:48:39.536978 pyvista-0.43.7/pyvista/core/
--rw-r--r--   0 runner    (1001) docker     (127)     1061 2024-05-04 07:37:21.000000 pyvista-0.43.7/pyvista/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1091 2024-05-04 07:37:21.000000 pyvista-0.43.7/pyvista/core/_typing_core.py
--rw-r--r--   0 runner    (1001) docker     (127)    11687 2024-05-04 07:37:21.000000 pyvista-0.43.7/pyvista/core/_vtk_core.py
--rw-r--r--   0 runner    (1001) docker     (127)    24269 2024-05-04 07:37:21.000000 pyvista-0.43.7/pyvista/core/cell.py
--rw-r--r--   0 runner    (1001) docker     (127)     4819 2024-05-04 07:37:21.000000 pyvista-0.43.7/pyvista/core/celltype.py
--rw-r--r--   0 runner    (1001) docker     (127)    42493 2024-05-04 07:37:21.000000 pyvista-0.43.7/pyvista/core/composite.py
--rw-r--r--   0 runner    (1001) docker     (127)    22250 2024-05-04 07:37:21.000000 pyvista-0.43.7/pyvista/core/dataobject.py
--rw-r--r--   0 runner    (1001) docker     (127)   107537 2024-05-04 07:37:21.000000 pyvista-0.43.7/pyvista/core/dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)    48777 2024-05-04 07:37:21.000000 pyvista-0.43.7/pyvista/core/datasetattributes.py
--rw-r--r--   0 runner    (1001) docker     (127)     3767 2024-05-04 07:37:21.000000 pyvista-0.43.7/pyvista/core/errors.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 07:48:39.536978 pyvista-0.43.7/pyvista/core/filters/
--rw-r--r--   0 runner    (1001) docker     (127)     2337 2024-05-04 07:37:21.000000 pyvista-0.43.7/pyvista/core/filters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6576 2024-05-04 07:37:21.000000 pyvista-0.43.7/pyvista/core/filters/composite.py
--rw-r--r--   0 runner    (1001) docker     (127)   244401 2024-05-04 07:37:21.000000 pyvista-0.43.7/pyvista/core/filters/data_set.py
--rw-r--r--   0 runner    (1001) docker     (127)    35703 2024-05-04 07:37:21.000000 pyvista-0.43.7/pyvista/core/filters/image_data.py
--rw-r--r--   0 runner    (1001) docker     (127)   134369 2024-05-04 07:37:21.000000 pyvista-0.43.7/pyvista/core/filters/poly_data.py
--rw-r--r--   0 runner    (1001) docker     (127)     5799 2024-05-04 07:37:21.000000 pyvista-0.43.7/pyvista/core/filters/rectilinear_grid.py
--rw-r--r--   0 runner    (1001) docker     (127)     7394 2024-05-04 07:37:21.000000 pyvista-0.43.7/pyvista/core/filters/structured_grid.py
--rw-r--r--   0 runner    (1001) docker     (127)     6169 2024-05-04 07:37:21.000000 pyvista-0.43.7/pyvista/core/filters/unstructured_grid.py
--rw-r--r--   0 runner    (1001) docker     (127)    28836 2024-05-04 07:37:21.000000 pyvista-0.43.7/pyvista/core/grid.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 07:48:39.536978 pyvista-0.43.7/pyvista/core/input_validation/
--rw-r--r--   0 runner    (1001) docker     (127)      920 2024-05-04 07:37:21.000000 pyvista-0.43.7/pyvista/core/input_validation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    34853 2024-05-04 07:37:21.000000 pyvista-0.43.7/pyvista/core/input_validation/check.py
--rw-r--r--   0 runner    (1001) docker     (127)    32556 2024-05-04 07:37:21.000000 pyvista-0.43.7/pyvista/core/input_validation/validate.py
--rw-r--r--   0 runner    (1001) docker     (127)    10679 2024-05-04 07:37:21.000000 pyvista-0.43.7/pyvista/core/objects.py
--rw-r--r--   0 runner    (1001) docker     (127)   108701 2024-05-04 07:37:21.000000 pyvista-0.43.7/pyvista/core/pointset.py
--rw-r--r--   0 runner    (1001) docker     (127)     4207 2024-05-04 07:37:21.000000 pyvista-0.43.7/pyvista/core/pyvista_ndarray.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 07:48:39.540978 pyvista-0.43.7/pyvista/core/utilities/
--rw-r--r--   0 runner    (1001) docker     (127)     3934 2024-05-04 07:37:21.000000 pyvista-0.43.7/pyvista/core/utilities/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    25162 2024-05-04 07:37:21.000000 pyvista-0.43.7/pyvista/core/utilities/arrays.py
--rw-r--r--   0 runner    (1001) docker     (127)     2966 2024-05-04 07:37:21.000000 pyvista-0.43.7/pyvista/core/utilities/cell_type_helper.py
--rw-r--r--   0 runner    (1001) docker     (127)     8951 2024-05-04 07:37:21.000000 pyvista-0.43.7/pyvista/core/utilities/cells.py
--rw-r--r--   0 runner    (1001) docker     (127)     4216 2024-05-04 07:37:21.000000 pyvista-0.43.7/pyvista/core/utilities/docs.py
--rw-r--r--   0 runner    (1001) docker     (127)    21838 2024-05-04 07:37:21.000000 pyvista-0.43.7/pyvista/core/utilities/features.py
--rw-r--r--   0 runner    (1001) docker     (127)    18705 2024-05-04 07:37:21.000000 pyvista-0.43.7/pyvista/core/utilities/fileio.py
--rw-r--r--   0 runner    (1001) docker     (127)    70180 2024-05-04 07:37:21.000000 pyvista-0.43.7/pyvista/core/utilities/geometric_objects.py
--rw-r--r--   0 runner    (1001) docker     (127)    25431 2024-05-04 07:37:21.000000 pyvista-0.43.7/pyvista/core/utilities/geometric_sources.py
--rw-r--r--   0 runner    (1001) docker     (127)     9080 2024-05-04 07:37:21.000000 pyvista-0.43.7/pyvista/core/utilities/helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)     8035 2024-05-04 07:37:21.000000 pyvista-0.43.7/pyvista/core/utilities/misc.py
--rw-r--r--   0 runner    (1001) docker     (127)     8635 2024-05-04 07:37:21.000000 pyvista-0.43.7/pyvista/core/utilities/observers.py
--rw-r--r--   0 runner    (1001) docker     (127)    41646 2024-05-04 07:37:21.000000 pyvista-0.43.7/pyvista/core/utilities/parametric_objects.py
--rw-r--r--   0 runner    (1001) docker     (127)    13653 2024-05-04 07:37:21.000000 pyvista-0.43.7/pyvista/core/utilities/points.py
--rw-r--r--   0 runner    (1001) docker     (127)    76127 2024-05-04 07:37:21.000000 pyvista-0.43.7/pyvista/core/utilities/reader.py
--rw-r--r--   0 runner    (1001) docker     (127)    10042 2024-05-04 07:37:21.000000 pyvista-0.43.7/pyvista/core/utilities/transformations.py
--rw-r--r--   0 runner    (1001) docker     (127)     1409 2024-05-04 07:37:21.000000 pyvista-0.43.7/pyvista/core/wrappers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 07:48:39.540978 pyvista-0.43.7/pyvista/demos/
--rw-r--r--   0 runner    (1001) docker     (127)      319 2024-05-04 07:37:21.000000 pyvista-0.43.7/pyvista/demos/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    15681 2024-05-04 07:37:21.000000 pyvista-0.43.7/pyvista/demos/demos.py
--rw-r--r--   0 runner    (1001) docker     (127)    10050 2024-05-04 07:37:21.000000 pyvista-0.43.7/pyvista/demos/logo.py
--rw-r--r--   0 runner    (1001) docker     (127)     1947 2024-05-04 07:37:21.000000 pyvista-0.43.7/pyvista/errors.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 07:48:39.544978 pyvista-0.43.7/pyvista/examples/
--rw-r--r--   0 runner    (1001) docker     (127)   463087 2024-05-04 07:37:21.000000 pyvista-0.43.7/pyvista/examples/2k_earth_daymap.jpg
--rwxr-xr-x   0 runner    (1001) docker     (127)      157 2024-05-04 07:37:21.000000 pyvista-0.43.7/pyvista/examples/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    74547 2024-05-04 07:37:21.000000 pyvista-0.43.7/pyvista/examples/airplane.ply
--rw-r--r--   0 runner    (1001) docker     (127)    17941 2024-05-04 07:37:21.000000 pyvista-0.43.7/pyvista/examples/ant.ply
--rw-r--r--   0 runner    (1001) docker     (127)    22540 2024-05-04 07:37:21.000000 pyvista-0.43.7/pyvista/examples/cells.py
--rw-r--r--   0 runner    (1001) docker     (127)   522284 2024-05-04 07:37:21.000000 pyvista-0.43.7/pyvista/examples/channels.vti
--rw-r--r--   0 runner    (1001) docker     (127)   152137 2024-05-04 07:37:21.000000 pyvista-0.43.7/pyvista/examples/downloads.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    12308 2024-05-04 07:37:21.000000 pyvista-0.43.7/pyvista/examples/examples.py
--rw-r--r--   0 runner    (1001) docker     (127)    37447 2024-05-04 07:37:21.000000 pyvista-0.43.7/pyvista/examples/globe.vtk
--rw-r--r--   0 runner    (1001) docker     (127)     3527 2024-05-04 07:37:21.000000 pyvista-0.43.7/pyvista/examples/gltf.py
--rw-r--r--   0 runner    (1001) docker     (127)     3091 2024-05-04 07:37:21.000000 pyvista-0.43.7/pyvista/examples/hexbeam.vtk
--rw-r--r--   0 runner    (1001) docker     (127)    20128 2024-05-04 07:37:21.000000 pyvista-0.43.7/pyvista/examples/nut.ply
--rw-r--r--   0 runner    (1001) docker     (127)    27183 2024-05-04 07:37:21.000000 pyvista-0.43.7/pyvista/examples/planets.py
--rw-r--r--   0 runner    (1001) docker     (127)   244663 2024-05-04 07:37:21.000000 pyvista-0.43.7/pyvista/examples/pyvista_logo.png
--rw-r--r--   0 runner    (1001) docker     (127)   228473 2024-05-04 07:37:21.000000 pyvista-0.43.7/pyvista/examples/rectilinear.vtk
--rw-r--r--   0 runner    (1001) docker     (127)    16237 2024-05-04 07:37:21.000000 pyvista-0.43.7/pyvista/examples/sphere.ply
--rw-r--r--   0 runner    (1001) docker     (127)    14094 2024-05-04 07:37:21.000000 pyvista-0.43.7/pyvista/examples/uniform.vtk
--rw-r--r--   0 runner    (1001) docker     (127)      963 2024-05-04 07:37:21.000000 pyvista-0.43.7/pyvista/examples/vrml.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 07:48:39.544978 pyvista-0.43.7/pyvista/ext/
--rw-r--r--   0 runner    (1001) docker     (127)       45 2024-05-04 07:37:21.000000 pyvista-0.43.7/pyvista/ext/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    16105 2024-05-04 07:37:21.000000 pyvista-0.43.7/pyvista/ext/coverage.py
--rw-r--r--   0 runner    (1001) docker     (127)    20382 2024-05-04 07:37:21.000000 pyvista-0.43.7/pyvista/ext/plot_directive.py
--rw-r--r--   0 runner    (1001) docker     (127)     4538 2024-05-04 07:37:21.000000 pyvista-0.43.7/pyvista/ext/viewer_directive.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 07:48:39.544978 pyvista-0.43.7/pyvista/jupyter/
--rw-r--r--   0 runner    (1001) docker     (127)     3792 2024-05-04 07:37:21.000000 pyvista-0.43.7/pyvista/jupyter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1200 2024-05-04 07:37:21.000000 pyvista-0.43.7/pyvista/jupyter/notebook.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 07:48:39.552978 pyvista-0.43.7/pyvista/plotting/
--rw-r--r--   0 runner    (1001) docker     (127)     3092 2024-05-04 07:37:21.000000 pyvista-0.43.7/pyvista/plotting/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9696 2024-05-04 07:37:21.000000 pyvista-0.43.7/pyvista/plotting/_plotting.py
--rw-r--r--   0 runner    (1001) docker     (127)    37838 2024-05-04 07:37:21.000000 pyvista-0.43.7/pyvista/plotting/_property.py
--rw-r--r--   0 runner    (1001) docker     (127)      939 2024-05-04 07:37:21.000000 pyvista-0.43.7/pyvista/plotting/_typing.py
--rw-r--r--   0 runner    (1001) docker     (127)     3186 2024-05-04 07:37:21.000000 pyvista-0.43.7/pyvista/plotting/_vtk.py
--rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-05-04 07:37:21.000000 pyvista-0.43.7/pyvista/plotting/_vtk_gl.py
--rw-r--r--   0 runner    (1001) docker     (127)    11762 2024-05-04 07:37:21.000000 pyvista-0.43.7/pyvista/plotting/actor.py
--rw-r--r--   0 runner    (1001) docker     (127)     4736 2024-05-04 07:37:21.000000 pyvista-0.43.7/pyvista/plotting/actor_properties.py
--rw-r--r--   0 runner    (1001) docker     (127)    18464 2024-05-04 07:37:21.000000 pyvista-0.43.7/pyvista/plotting/affine_widget.py
--rw-r--r--   0 runner    (1001) docker     (127)     3041 2024-05-04 07:37:21.000000 pyvista-0.43.7/pyvista/plotting/axes.py
--rw-r--r--   0 runner    (1001) docker     (127)    15715 2024-05-04 07:37:21.000000 pyvista-0.43.7/pyvista/plotting/axes_actor.py
--rw-r--r--   0 runner    (1001) docker     (127)     3019 2024-05-04 07:37:21.000000 pyvista-0.43.7/pyvista/plotting/background_renderer.py
--rw-r--r--   0 runner    (1001) docker     (127)    26651 2024-05-04 07:37:21.000000 pyvista-0.43.7/pyvista/plotting/camera.py
--rw-r--r--   0 runner    (1001) docker     (127)   152660 2024-05-04 07:37:21.000000 pyvista-0.43.7/pyvista/plotting/charts.py
--rw-r--r--   0 runner    (1001) docker     (127)    40899 2024-05-04 07:37:21.000000 pyvista-0.43.7/pyvista/plotting/colors.py
--rw-r--r--   0 runner    (1001) docker     (127)    29748 2024-05-04 07:37:21.000000 pyvista-0.43.7/pyvista/plotting/composite_mapper.py
--rw-r--r--   0 runner    (1001) docker     (127)    18685 2024-05-04 07:37:21.000000 pyvista-0.43.7/pyvista/plotting/cube_axes_actor.py
--rw-r--r--   0 runner    (1001) docker     (127)     1080 2024-05-04 07:37:21.000000 pyvista-0.43.7/pyvista/plotting/errors.py
--rw-r--r--   0 runner    (1001) docker     (127)     5435 2024-05-04 07:37:21.000000 pyvista-0.43.7/pyvista/plotting/helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)    41606 2024-05-04 07:37:21.000000 pyvista-0.43.7/pyvista/plotting/lights.py
--rw-r--r--   0 runner    (1001) docker     (127)    35796 2024-05-04 07:37:21.000000 pyvista-0.43.7/pyvista/plotting/lookup_table.py
--rw-r--r--   0 runner    (1001) docker     (127)    36048 2024-05-04 07:37:21.000000 pyvista-0.43.7/pyvista/plotting/mapper.py
--rw-r--r--   0 runner    (1001) docker     (127)     2015 2024-05-04 07:37:21.000000 pyvista-0.43.7/pyvista/plotting/opts.py
--rw-r--r--   0 runner    (1001) docker     (127)    71418 2024-05-04 07:37:21.000000 pyvista-0.43.7/pyvista/plotting/picking.py
--rw-r--r--   0 runner    (1001) docker     (127)   256359 2024-05-04 07:37:21.000000 pyvista-0.43.7/pyvista/plotting/plotter.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 07:48:39.552978 pyvista-0.43.7/pyvista/plotting/plotting/
--rw-r--r--   0 runner    (1001) docker     (127)      951 2024-05-04 07:37:21.000000 pyvista-0.43.7/pyvista/plotting/plotting/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9293 2024-05-04 07:37:21.000000 pyvista-0.43.7/pyvista/plotting/prop3d.py
--rw-r--r--   0 runner    (1001) docker     (127)    10528 2024-05-04 07:37:21.000000 pyvista-0.43.7/pyvista/plotting/render_passes.py
--rw-r--r--   0 runner    (1001) docker     (127)    47093 2024-05-04 07:37:21.000000 pyvista-0.43.7/pyvista/plotting/render_window_interactor.py
--rw-r--r--   0 runner    (1001) docker     (127)   125835 2024-05-04 07:37:21.000000 pyvista-0.43.7/pyvista/plotting/renderer.py
--rw-r--r--   0 runner    (1001) docker     (127)    24583 2024-05-04 07:37:21.000000 pyvista-0.43.7/pyvista/plotting/renderers.py
--rw-r--r--   0 runner    (1001) docker     (127)    20205 2024-05-04 07:37:21.000000 pyvista-0.43.7/pyvista/plotting/scalar_bars.py
--rw-r--r--   0 runner    (1001) docker     (127)    15802 2024-05-04 07:37:21.000000 pyvista-0.43.7/pyvista/plotting/text.py
--rw-r--r--   0 runner    (1001) docker     (127)    20730 2024-05-04 07:37:21.000000 pyvista-0.43.7/pyvista/plotting/texture.py
--rw-r--r--   0 runner    (1001) docker     (127)    96999 2024-05-04 07:37:21.000000 pyvista-0.43.7/pyvista/plotting/themes.py
--rw-r--r--   0 runner    (1001) docker     (127)    22809 2024-05-04 07:37:21.000000 pyvista-0.43.7/pyvista/plotting/tools.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 07:48:39.552978 pyvista-0.43.7/pyvista/plotting/utilities/
--rw-r--r--   0 runner    (1001) docker     (127)      756 2024-05-04 07:37:21.000000 pyvista-0.43.7/pyvista/plotting/utilities/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    17904 2024-05-04 07:37:21.000000 pyvista-0.43.7/pyvista/plotting/utilities/algorithms.py
--rw-r--r--   0 runner    (1001) docker     (127)     3409 2024-05-04 07:37:21.000000 pyvista-0.43.7/pyvista/plotting/utilities/cubemap.py
--rw-r--r--   0 runner    (1001) docker     (127)     1825 2024-05-04 07:37:21.000000 pyvista-0.43.7/pyvista/plotting/utilities/gl_checks.py
--rw-r--r--   0 runner    (1001) docker     (127)     7886 2024-05-04 07:37:21.000000 pyvista-0.43.7/pyvista/plotting/utilities/regression.py
--rw-r--r--   0 runner    (1001) docker     (127)     6822 2024-05-04 07:37:21.000000 pyvista-0.43.7/pyvista/plotting/utilities/sphinx_gallery.py
--rw-r--r--   0 runner    (1001) docker     (127)     1462 2024-05-04 07:37:21.000000 pyvista-0.43.7/pyvista/plotting/utilities/xvfb.py
--rw-r--r--   0 runner    (1001) docker     (127)     1725 2024-05-04 07:37:21.000000 pyvista-0.43.7/pyvista/plotting/volume.py
--rw-r--r--   0 runner    (1001) docker     (127)    12959 2024-05-04 07:37:21.000000 pyvista-0.43.7/pyvista/plotting/volume_property.py
--rw-r--r--   0 runner    (1001) docker     (127)    98543 2024-05-04 07:37:21.000000 pyvista-0.43.7/pyvista/plotting/widgets.py
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-04 07:37:21.000000 pyvista-0.43.7/pyvista/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)     6990 2024-05-04 07:37:21.000000 pyvista-0.43.7/pyvista/report.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 07:48:39.552978 pyvista-0.43.7/pyvista/trame/
--rw-r--r--   0 runner    (1001) docker     (127)      589 2024-05-04 07:37:21.000000 pyvista-0.43.7/pyvista/trame/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    15020 2024-05-04 07:37:21.000000 pyvista-0.43.7/pyvista/trame/jupyter.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 07:48:39.552978 pyvista-0.43.7/pyvista/trame/ui/
--rw-r--r--   0 runner    (1001) docker     (127)     3390 2024-05-04 07:37:21.000000 pyvista-0.43.7/pyvista/trame/ui/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7951 2024-05-04 07:37:21.000000 pyvista-0.43.7/pyvista/trame/ui/base_viewer.py
--rw-r--r--   0 runner    (1001) docker     (127)    12498 2024-05-04 07:37:21.000000 pyvista-0.43.7/pyvista/trame/ui/vuetify2.py
--rw-r--r--   0 runner    (1001) docker     (127)    12773 2024-05-04 07:37:21.000000 pyvista-0.43.7/pyvista/trame/ui/vuetify3.py
--rw-r--r--   0 runner    (1001) docker     (127)     9322 2024-05-04 07:37:21.000000 pyvista-0.43.7/pyvista/trame/views.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 07:48:39.556978 pyvista-0.43.7/pyvista/utilities/
--rw-r--r--   0 runner    (1001) docker     (127)     2177 2024-05-04 07:37:21.000000 pyvista-0.43.7/pyvista/utilities/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       65 2024-05-04 07:37:21.000000 pyvista-0.43.7/pyvista/utilities/algorithms.py
--rw-r--r--   0 runner    (1001) docker     (127)       65 2024-05-04 07:37:21.000000 pyvista-0.43.7/pyvista/utilities/arrays.py
--rw-r--r--   0 runner    (1001) docker     (127)       65 2024-05-04 07:37:21.000000 pyvista-0.43.7/pyvista/utilities/cell_type_helper.py
--rw-r--r--   0 runner    (1001) docker     (127)       65 2024-05-04 07:37:21.000000 pyvista-0.43.7/pyvista/utilities/cells.py
--rw-r--r--   0 runner    (1001) docker     (127)       65 2024-05-04 07:37:21.000000 pyvista-0.43.7/pyvista/utilities/common.py
--rw-r--r--   0 runner    (1001) docker     (127)       65 2024-05-04 07:37:21.000000 pyvista-0.43.7/pyvista/utilities/docs.py
--rw-r--r--   0 runner    (1001) docker     (127)       65 2024-05-04 07:37:21.000000 pyvista-0.43.7/pyvista/utilities/errors.py
--rw-r--r--   0 runner    (1001) docker     (127)       65 2024-05-04 07:37:21.000000 pyvista-0.43.7/pyvista/utilities/features.py
--rw-r--r--   0 runner    (1001) docker     (127)       65 2024-05-04 07:37:21.000000 pyvista-0.43.7/pyvista/utilities/fileio.py
--rw-r--r--   0 runner    (1001) docker     (127)       65 2024-05-04 07:37:21.000000 pyvista-0.43.7/pyvista/utilities/geometric_objects.py
--rw-r--r--   0 runner    (1001) docker     (127)       65 2024-05-04 07:37:21.000000 pyvista-0.43.7/pyvista/utilities/helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)       65 2024-05-04 07:37:21.000000 pyvista-0.43.7/pyvista/utilities/misc.py
--rw-r--r--   0 runner    (1001) docker     (127)       65 2024-05-04 07:37:21.000000 pyvista-0.43.7/pyvista/utilities/parametric_objects.py
--rw-r--r--   0 runner    (1001) docker     (127)       65 2024-05-04 07:37:21.000000 pyvista-0.43.7/pyvista/utilities/reader.py
--rw-r--r--   0 runner    (1001) docker     (127)       65 2024-05-04 07:37:21.000000 pyvista-0.43.7/pyvista/utilities/regression.py
--rw-r--r--   0 runner    (1001) docker     (127)       65 2024-05-04 07:37:21.000000 pyvista-0.43.7/pyvista/utilities/sphinx_gallery.py
--rw-r--r--   0 runner    (1001) docker     (127)       65 2024-05-04 07:37:21.000000 pyvista-0.43.7/pyvista/utilities/transformations.py
--rw-r--r--   0 runner    (1001) docker     (127)       65 2024-05-04 07:37:21.000000 pyvista-0.43.7/pyvista/utilities/wrappers.py
--rw-r--r--   0 runner    (1001) docker     (127)       65 2024-05-04 07:37:21.000000 pyvista-0.43.7/pyvista/utilities/xvfb.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 07:48:39.556978 pyvista-0.43.7/pyvista.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    14665 2024-05-04 07:48:39.000000 pyvista-0.43.7/pyvista.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4837 2024-05-04 07:48:39.000000 pyvista-0.43.7/pyvista.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-04 07:48:39.000000 pyvista-0.43.7/pyvista.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      305 2024-05-04 07:48:39.000000 pyvista-0.43.7/pyvista.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-04 07:48:39.000000 pyvista-0.43.7/pyvista.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-04 07:48:39.560978 pyvista-0.43.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       85 2024-05-04 07:37:21.000000 pyvista-0.43.7/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 07:48:39.556978 pyvista-0.43.7/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      600 2024-05-04 07:37:21.000000 pyvista-0.43.7/tests/test_init.py
--rw-r--r--   0 runner    (1001) docker     (127)     2071 2024-05-04 07:37:21.000000 pyvista-0.43.7/tests/test_meshio.py
--rw-r--r--   0 runner    (1001) docker     (127)      417 2024-05-04 07:37:21.000000 pyvista-0.43.7/tests/test_meta.py
--rw-r--r--   0 runner    (1001) docker     (127)     2810 2024-05-04 07:37:21.000000 pyvista-0.43.7/tests/test_tinypages.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-06 10:39:19.709519 pyvista-0.44.dev0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1932 2024-02-06 10:27:19.000000 pyvista-0.44.dev0/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1088 2024-02-06 10:27:19.000000 pyvista-0.44.dev0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      158 2024-02-06 10:27:19.000000 pyvista-0.44.dev0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    14668 2024-02-06 10:39:19.709519 pyvista-0.44.dev0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    12681 2024-02-06 10:27:19.000000 pyvista-0.44.dev0/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     8727 2024-02-06 10:27:20.000000 pyvista-0.44.dev0/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-06 10:39:19.681519 pyvista-0.44.dev0/pyvista/
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2792 2024-02-06 10:27:20.000000 pyvista-0.44.dev0/pyvista/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9759 2024-02-06 10:27:20.000000 pyvista-0.44.dev0/pyvista/_plot.py
+-rw-r--r--   0 runner    (1001) docker     (127)      405 2024-02-06 10:27:20.000000 pyvista-0.44.dev0/pyvista/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)      478 2024-02-06 10:27:20.000000 pyvista-0.44.dev0/pyvista/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-06 10:39:19.685519 pyvista-0.44.dev0/pyvista/core/
+-rw-r--r--   0 runner    (1001) docker     (127)     1061 2024-02-06 10:27:20.000000 pyvista-0.44.dev0/pyvista/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1091 2024-02-06 10:27:20.000000 pyvista-0.44.dev0/pyvista/core/_typing_core.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11725 2024-02-06 10:27:20.000000 pyvista-0.44.dev0/pyvista/core/_vtk_core.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25793 2024-02-06 10:27:20.000000 pyvista-0.44.dev0/pyvista/core/cell.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4819 2024-02-06 10:27:20.000000 pyvista-0.44.dev0/pyvista/core/celltype.py
+-rw-r--r--   0 runner    (1001) docker     (127)    42493 2024-02-06 10:27:20.000000 pyvista-0.44.dev0/pyvista/core/composite.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22250 2024-02-06 10:27:20.000000 pyvista-0.44.dev0/pyvista/core/dataobject.py
+-rw-r--r--   0 runner    (1001) docker     (127)   107653 2024-02-06 10:27:20.000000 pyvista-0.44.dev0/pyvista/core/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)    48878 2024-02-06 10:27:20.000000 pyvista-0.44.dev0/pyvista/core/datasetattributes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4104 2024-02-06 10:27:20.000000 pyvista-0.44.dev0/pyvista/core/errors.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-06 10:39:19.685519 pyvista-0.44.dev0/pyvista/core/filters/
+-rw-r--r--   0 runner    (1001) docker     (127)     2337 2024-02-06 10:27:20.000000 pyvista-0.44.dev0/pyvista/core/filters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6576 2024-02-06 10:27:20.000000 pyvista-0.44.dev0/pyvista/core/filters/composite.py
+-rw-r--r--   0 runner    (1001) docker     (127)   244404 2024-02-06 10:27:20.000000 pyvista-0.44.dev0/pyvista/core/filters/data_set.py
+-rw-r--r--   0 runner    (1001) docker     (127)    35703 2024-02-06 10:27:20.000000 pyvista-0.44.dev0/pyvista/core/filters/image_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)   133972 2024-02-06 10:27:20.000000 pyvista-0.44.dev0/pyvista/core/filters/poly_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5785 2024-02-06 10:27:20.000000 pyvista-0.44.dev0/pyvista/core/filters/rectilinear_grid.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7394 2024-02-06 10:27:20.000000 pyvista-0.44.dev0/pyvista/core/filters/structured_grid.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6169 2024-02-06 10:27:20.000000 pyvista-0.44.dev0/pyvista/core/filters/unstructured_grid.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28837 2024-02-06 10:27:20.000000 pyvista-0.44.dev0/pyvista/core/grid.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-06 10:39:19.685519 pyvista-0.44.dev0/pyvista/core/input_validation/
+-rw-r--r--   0 runner    (1001) docker     (127)      920 2024-02-06 10:27:20.000000 pyvista-0.44.dev0/pyvista/core/input_validation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    34853 2024-02-06 10:27:20.000000 pyvista-0.44.dev0/pyvista/core/input_validation/check.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32556 2024-02-06 10:27:20.000000 pyvista-0.44.dev0/pyvista/core/input_validation/validate.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10697 2024-02-06 10:27:20.000000 pyvista-0.44.dev0/pyvista/core/objects.py
+-rw-r--r--   0 runner    (1001) docker     (127)   111261 2024-02-06 10:27:20.000000 pyvista-0.44.dev0/pyvista/core/pointset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4207 2024-02-06 10:27:20.000000 pyvista-0.44.dev0/pyvista/core/pyvista_ndarray.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-06 10:39:19.689519 pyvista-0.44.dev0/pyvista/core/utilities/
+-rw-r--r--   0 runner    (1001) docker     (127)     3934 2024-02-06 10:27:20.000000 pyvista-0.44.dev0/pyvista/core/utilities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25162 2024-02-06 10:27:20.000000 pyvista-0.44.dev0/pyvista/core/utilities/arrays.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2966 2024-02-06 10:27:20.000000 pyvista-0.44.dev0/pyvista/core/utilities/cell_type_helper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8951 2024-02-06 10:27:20.000000 pyvista-0.44.dev0/pyvista/core/utilities/cells.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4216 2024-02-06 10:27:20.000000 pyvista-0.44.dev0/pyvista/core/utilities/docs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21838 2024-02-06 10:27:20.000000 pyvista-0.44.dev0/pyvista/core/utilities/features.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18705 2024-02-06 10:27:20.000000 pyvista-0.44.dev0/pyvista/core/utilities/fileio.py
+-rw-r--r--   0 runner    (1001) docker     (127)    69968 2024-02-06 10:27:20.000000 pyvista-0.44.dev0/pyvista/core/utilities/geometric_objects.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25405 2024-02-06 10:27:20.000000 pyvista-0.44.dev0/pyvista/core/utilities/geometric_sources.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9094 2024-02-06 10:27:20.000000 pyvista-0.44.dev0/pyvista/core/utilities/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8035 2024-02-06 10:27:20.000000 pyvista-0.44.dev0/pyvista/core/utilities/misc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8641 2024-02-06 10:27:20.000000 pyvista-0.44.dev0/pyvista/core/utilities/observers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    41646 2024-02-06 10:27:20.000000 pyvista-0.44.dev0/pyvista/core/utilities/parametric_objects.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13681 2024-02-06 10:27:20.000000 pyvista-0.44.dev0/pyvista/core/utilities/points.py
+-rw-r--r--   0 runner    (1001) docker     (127)    77177 2024-02-06 10:27:20.000000 pyvista-0.44.dev0/pyvista/core/utilities/reader.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10042 2024-02-06 10:27:20.000000 pyvista-0.44.dev0/pyvista/core/utilities/transformations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1409 2024-02-06 10:27:20.000000 pyvista-0.44.dev0/pyvista/core/wrappers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-06 10:39:19.689519 pyvista-0.44.dev0/pyvista/demos/
+-rw-r--r--   0 runner    (1001) docker     (127)      319 2024-02-06 10:27:20.000000 pyvista-0.44.dev0/pyvista/demos/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15681 2024-02-06 10:27:20.000000 pyvista-0.44.dev0/pyvista/demos/demos.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10050 2024-02-06 10:27:20.000000 pyvista-0.44.dev0/pyvista/demos/logo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1947 2024-02-06 10:27:20.000000 pyvista-0.44.dev0/pyvista/errors.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-06 10:39:19.693519 pyvista-0.44.dev0/pyvista/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)   463087 2024-02-06 10:27:20.000000 pyvista-0.44.dev0/pyvista/examples/2k_earth_daymap.jpg
+-rwxr-xr-x   0 runner    (1001) docker     (127)      157 2024-02-06 10:27:20.000000 pyvista-0.44.dev0/pyvista/examples/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    74547 2024-02-06 10:27:20.000000 pyvista-0.44.dev0/pyvista/examples/airplane.ply
+-rw-r--r--   0 runner    (1001) docker     (127)    17941 2024-02-06 10:27:20.000000 pyvista-0.44.dev0/pyvista/examples/ant.ply
+-rw-r--r--   0 runner    (1001) docker     (127)    22540 2024-02-06 10:27:20.000000 pyvista-0.44.dev0/pyvista/examples/cells.py
+-rw-r--r--   0 runner    (1001) docker     (127)   522284 2024-02-06 10:27:20.000000 pyvista-0.44.dev0/pyvista/examples/channels.vti
+-rw-r--r--   0 runner    (1001) docker     (127)   153215 2024-02-06 10:27:20.000000 pyvista-0.44.dev0/pyvista/examples/downloads.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    12308 2024-02-06 10:27:20.000000 pyvista-0.44.dev0/pyvista/examples/examples.py
+-rw-r--r--   0 runner    (1001) docker     (127)    37447 2024-02-06 10:27:20.000000 pyvista-0.44.dev0/pyvista/examples/globe.vtk
+-rw-r--r--   0 runner    (1001) docker     (127)     3527 2024-02-06 10:27:20.000000 pyvista-0.44.dev0/pyvista/examples/gltf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3091 2024-02-06 10:27:20.000000 pyvista-0.44.dev0/pyvista/examples/hexbeam.vtk
+-rw-r--r--   0 runner    (1001) docker     (127)    20128 2024-02-06 10:27:20.000000 pyvista-0.44.dev0/pyvista/examples/nut.ply
+-rw-r--r--   0 runner    (1001) docker     (127)    27183 2024-02-06 10:27:20.000000 pyvista-0.44.dev0/pyvista/examples/planets.py
+-rw-r--r--   0 runner    (1001) docker     (127)   244663 2024-02-06 10:27:20.000000 pyvista-0.44.dev0/pyvista/examples/pyvista_logo.png
+-rw-r--r--   0 runner    (1001) docker     (127)   228473 2024-02-06 10:27:20.000000 pyvista-0.44.dev0/pyvista/examples/rectilinear.vtk
+-rw-r--r--   0 runner    (1001) docker     (127)    16237 2024-02-06 10:27:20.000000 pyvista-0.44.dev0/pyvista/examples/sphere.ply
+-rw-r--r--   0 runner    (1001) docker     (127)    14094 2024-02-06 10:27:20.000000 pyvista-0.44.dev0/pyvista/examples/uniform.vtk
+-rw-r--r--   0 runner    (1001) docker     (127)      963 2024-02-06 10:27:20.000000 pyvista-0.44.dev0/pyvista/examples/vrml.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-06 10:39:19.693519 pyvista-0.44.dev0/pyvista/ext/
+-rw-r--r--   0 runner    (1001) docker     (127)       45 2024-02-06 10:27:20.000000 pyvista-0.44.dev0/pyvista/ext/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16105 2024-02-06 10:27:20.000000 pyvista-0.44.dev0/pyvista/ext/coverage.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20382 2024-02-06 10:27:20.000000 pyvista-0.44.dev0/pyvista/ext/plot_directive.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4538 2024-02-06 10:27:20.000000 pyvista-0.44.dev0/pyvista/ext/viewer_directive.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-06 10:39:19.693519 pyvista-0.44.dev0/pyvista/jupyter/
+-rw-r--r--   0 runner    (1001) docker     (127)     3792 2024-02-06 10:27:20.000000 pyvista-0.44.dev0/pyvista/jupyter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1200 2024-02-06 10:27:20.000000 pyvista-0.44.dev0/pyvista/jupyter/notebook.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-06 10:39:19.701519 pyvista-0.44.dev0/pyvista/plotting/
+-rw-r--r--   0 runner    (1001) docker     (127)     3092 2024-02-06 10:27:20.000000 pyvista-0.44.dev0/pyvista/plotting/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9696 2024-02-06 10:27:20.000000 pyvista-0.44.dev0/pyvista/plotting/_plotting.py
+-rw-r--r--   0 runner    (1001) docker     (127)    37838 2024-02-06 10:27:20.000000 pyvista-0.44.dev0/pyvista/plotting/_property.py
+-rw-r--r--   0 runner    (1001) docker     (127)      939 2024-02-06 10:27:20.000000 pyvista-0.44.dev0/pyvista/plotting/_typing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3186 2024-02-06 10:27:20.000000 pyvista-0.44.dev0/pyvista/plotting/_vtk.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-02-06 10:27:20.000000 pyvista-0.44.dev0/pyvista/plotting/_vtk_gl.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11719 2024-02-06 10:27:20.000000 pyvista-0.44.dev0/pyvista/plotting/actor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4736 2024-02-06 10:27:20.000000 pyvista-0.44.dev0/pyvista/plotting/actor_properties.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18464 2024-02-06 10:27:20.000000 pyvista-0.44.dev0/pyvista/plotting/affine_widget.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3041 2024-02-06 10:27:20.000000 pyvista-0.44.dev0/pyvista/plotting/axes.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15715 2024-02-06 10:27:20.000000 pyvista-0.44.dev0/pyvista/plotting/axes_actor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3019 2024-02-06 10:27:20.000000 pyvista-0.44.dev0/pyvista/plotting/background_renderer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26651 2024-02-06 10:27:20.000000 pyvista-0.44.dev0/pyvista/plotting/camera.py
+-rw-r--r--   0 runner    (1001) docker     (127)   152660 2024-02-06 10:27:20.000000 pyvista-0.44.dev0/pyvista/plotting/charts.py
+-rw-r--r--   0 runner    (1001) docker     (127)    40899 2024-02-06 10:27:20.000000 pyvista-0.44.dev0/pyvista/plotting/colors.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29748 2024-02-06 10:27:20.000000 pyvista-0.44.dev0/pyvista/plotting/composite_mapper.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18586 2024-02-06 10:27:20.000000 pyvista-0.44.dev0/pyvista/plotting/cube_axes_actor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1080 2024-02-06 10:27:20.000000 pyvista-0.44.dev0/pyvista/plotting/errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5491 2024-02-06 10:27:20.000000 pyvista-0.44.dev0/pyvista/plotting/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    41606 2024-02-06 10:27:20.000000 pyvista-0.44.dev0/pyvista/plotting/lights.py
+-rw-r--r--   0 runner    (1001) docker     (127)    35796 2024-02-06 10:27:20.000000 pyvista-0.44.dev0/pyvista/plotting/lookup_table.py
+-rw-r--r--   0 runner    (1001) docker     (127)    37663 2024-02-06 10:27:20.000000 pyvista-0.44.dev0/pyvista/plotting/mapper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2015 2024-02-06 10:27:20.000000 pyvista-0.44.dev0/pyvista/plotting/opts.py
+-rw-r--r--   0 runner    (1001) docker     (127)    71418 2024-02-06 10:27:20.000000 pyvista-0.44.dev0/pyvista/plotting/picking.py
+-rw-r--r--   0 runner    (1001) docker     (127)   256779 2024-02-06 10:27:20.000000 pyvista-0.44.dev0/pyvista/plotting/plotter.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-06 10:39:19.701519 pyvista-0.44.dev0/pyvista/plotting/plotting/
+-rw-r--r--   0 runner    (1001) docker     (127)      951 2024-02-06 10:27:20.000000 pyvista-0.44.dev0/pyvista/plotting/plotting/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9293 2024-02-06 10:27:20.000000 pyvista-0.44.dev0/pyvista/plotting/prop3d.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10528 2024-02-06 10:27:20.000000 pyvista-0.44.dev0/pyvista/plotting/render_passes.py
+-rw-r--r--   0 runner    (1001) docker     (127)    52729 2024-02-06 10:27:20.000000 pyvista-0.44.dev0/pyvista/plotting/render_window_interactor.py
+-rw-r--r--   0 runner    (1001) docker     (127)   126010 2024-02-06 10:27:20.000000 pyvista-0.44.dev0/pyvista/plotting/renderer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24583 2024-02-06 10:27:20.000000 pyvista-0.44.dev0/pyvista/plotting/renderers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20205 2024-02-06 10:27:20.000000 pyvista-0.44.dev0/pyvista/plotting/scalar_bars.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16656 2024-02-06 10:27:20.000000 pyvista-0.44.dev0/pyvista/plotting/text.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20730 2024-02-06 10:27:20.000000 pyvista-0.44.dev0/pyvista/plotting/texture.py
+-rw-r--r--   0 runner    (1001) docker     (127)    96996 2024-02-06 10:27:20.000000 pyvista-0.44.dev0/pyvista/plotting/themes.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22630 2024-02-06 10:27:20.000000 pyvista-0.44.dev0/pyvista/plotting/tools.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-06 10:39:19.701519 pyvista-0.44.dev0/pyvista/plotting/utilities/
+-rw-r--r--   0 runner    (1001) docker     (127)      756 2024-02-06 10:27:20.000000 pyvista-0.44.dev0/pyvista/plotting/utilities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17904 2024-02-06 10:27:20.000000 pyvista-0.44.dev0/pyvista/plotting/utilities/algorithms.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3409 2024-02-06 10:27:20.000000 pyvista-0.44.dev0/pyvista/plotting/utilities/cubemap.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1825 2024-02-06 10:27:20.000000 pyvista-0.44.dev0/pyvista/plotting/utilities/gl_checks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7886 2024-02-06 10:27:20.000000 pyvista-0.44.dev0/pyvista/plotting/utilities/regression.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6799 2024-02-06 10:27:20.000000 pyvista-0.44.dev0/pyvista/plotting/utilities/sphinx_gallery.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1462 2024-02-06 10:27:20.000000 pyvista-0.44.dev0/pyvista/plotting/utilities/xvfb.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1725 2024-02-06 10:27:20.000000 pyvista-0.44.dev0/pyvista/plotting/volume.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12959 2024-02-06 10:27:20.000000 pyvista-0.44.dev0/pyvista/plotting/volume_property.py
+-rw-r--r--   0 runner    (1001) docker     (127)    99745 2024-02-06 10:27:20.000000 pyvista-0.44.dev0/pyvista/plotting/widgets.py
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-02-06 10:27:20.000000 pyvista-0.44.dev0/pyvista/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)     6990 2024-02-06 10:27:20.000000 pyvista-0.44.dev0/pyvista/report.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-06 10:39:19.701519 pyvista-0.44.dev0/pyvista/trame/
+-rw-r--r--   0 runner    (1001) docker     (127)      589 2024-02-06 10:27:20.000000 pyvista-0.44.dev0/pyvista/trame/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15020 2024-02-06 10:27:20.000000 pyvista-0.44.dev0/pyvista/trame/jupyter.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-06 10:39:19.701519 pyvista-0.44.dev0/pyvista/trame/ui/
+-rw-r--r--   0 runner    (1001) docker     (127)     3390 2024-02-06 10:27:20.000000 pyvista-0.44.dev0/pyvista/trame/ui/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7951 2024-02-06 10:27:20.000000 pyvista-0.44.dev0/pyvista/trame/ui/base_viewer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12498 2024-02-06 10:27:20.000000 pyvista-0.44.dev0/pyvista/trame/ui/vuetify2.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12773 2024-02-06 10:27:20.000000 pyvista-0.44.dev0/pyvista/trame/ui/vuetify3.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9322 2024-02-06 10:27:20.000000 pyvista-0.44.dev0/pyvista/trame/views.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-06 10:39:19.705519 pyvista-0.44.dev0/pyvista/utilities/
+-rw-r--r--   0 runner    (1001) docker     (127)     2177 2024-02-06 10:27:20.000000 pyvista-0.44.dev0/pyvista/utilities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       65 2024-02-06 10:27:20.000000 pyvista-0.44.dev0/pyvista/utilities/algorithms.py
+-rw-r--r--   0 runner    (1001) docker     (127)       65 2024-02-06 10:27:20.000000 pyvista-0.44.dev0/pyvista/utilities/arrays.py
+-rw-r--r--   0 runner    (1001) docker     (127)       65 2024-02-06 10:27:20.000000 pyvista-0.44.dev0/pyvista/utilities/cell_type_helper.py
+-rw-r--r--   0 runner    (1001) docker     (127)       65 2024-02-06 10:27:20.000000 pyvista-0.44.dev0/pyvista/utilities/cells.py
+-rw-r--r--   0 runner    (1001) docker     (127)       65 2024-02-06 10:27:20.000000 pyvista-0.44.dev0/pyvista/utilities/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)       65 2024-02-06 10:27:20.000000 pyvista-0.44.dev0/pyvista/utilities/docs.py
+-rw-r--r--   0 runner    (1001) docker     (127)       65 2024-02-06 10:27:20.000000 pyvista-0.44.dev0/pyvista/utilities/errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)       65 2024-02-06 10:27:20.000000 pyvista-0.44.dev0/pyvista/utilities/features.py
+-rw-r--r--   0 runner    (1001) docker     (127)       65 2024-02-06 10:27:20.000000 pyvista-0.44.dev0/pyvista/utilities/fileio.py
+-rw-r--r--   0 runner    (1001) docker     (127)       65 2024-02-06 10:27:20.000000 pyvista-0.44.dev0/pyvista/utilities/geometric_objects.py
+-rw-r--r--   0 runner    (1001) docker     (127)       65 2024-02-06 10:27:20.000000 pyvista-0.44.dev0/pyvista/utilities/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)       65 2024-02-06 10:27:20.000000 pyvista-0.44.dev0/pyvista/utilities/misc.py
+-rw-r--r--   0 runner    (1001) docker     (127)       65 2024-02-06 10:27:20.000000 pyvista-0.44.dev0/pyvista/utilities/parametric_objects.py
+-rw-r--r--   0 runner    (1001) docker     (127)       65 2024-02-06 10:27:20.000000 pyvista-0.44.dev0/pyvista/utilities/reader.py
+-rw-r--r--   0 runner    (1001) docker     (127)       65 2024-02-06 10:27:20.000000 pyvista-0.44.dev0/pyvista/utilities/regression.py
+-rw-r--r--   0 runner    (1001) docker     (127)       65 2024-02-06 10:27:20.000000 pyvista-0.44.dev0/pyvista/utilities/sphinx_gallery.py
+-rw-r--r--   0 runner    (1001) docker     (127)       65 2024-02-06 10:27:20.000000 pyvista-0.44.dev0/pyvista/utilities/transformations.py
+-rw-r--r--   0 runner    (1001) docker     (127)       65 2024-02-06 10:27:20.000000 pyvista-0.44.dev0/pyvista/utilities/wrappers.py
+-rw-r--r--   0 runner    (1001) docker     (127)       65 2024-02-06 10:27:20.000000 pyvista-0.44.dev0/pyvista/utilities/xvfb.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-06 10:39:19.705519 pyvista-0.44.dev0/pyvista.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    14668 2024-02-06 10:39:19.000000 pyvista-0.44.dev0/pyvista.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4837 2024-02-06 10:39:19.000000 pyvista-0.44.dev0/pyvista.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-06 10:39:19.000000 pyvista-0.44.dev0/pyvista.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      305 2024-02-06 10:39:19.000000 pyvista-0.44.dev0/pyvista.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-02-06 10:39:19.000000 pyvista-0.44.dev0/pyvista.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-06 10:39:19.709519 pyvista-0.44.dev0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       85 2024-02-06 10:27:20.000000 pyvista-0.44.dev0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-06 10:39:19.705519 pyvista-0.44.dev0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      600 2024-02-06 10:27:20.000000 pyvista-0.44.dev0/tests/test_init.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2071 2024-02-06 10:27:20.000000 pyvista-0.44.dev0/tests/test_meshio.py
+-rw-r--r--   0 runner    (1001) docker     (127)      417 2024-02-06 10:27:20.000000 pyvista-0.44.dev0/tests/test_meta.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2810 2024-02-06 10:27:20.000000 pyvista-0.44.dev0/tests/test_tinypages.py
```

### Comparing `pyvista-0.43.7/AUTHORS.rst` & `pyvista-0.44.dev0/AUTHORS.rst`

 * *Files identical despite different names*

### Comparing `pyvista-0.43.7/LICENSE` & `pyvista-0.44.dev0/LICENSE`

 * *Files identical despite different names*

### Comparing `pyvista-0.43.7/PKG-INFO` & `pyvista-0.44.dev0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyvista
-Version: 0.43.7
+Version: 0.44.dev0
 Summary: Easier Pythonic interface to VTK
 Author-email: PyVista Developers <info@pyvista.org>
 License: MIT
 Project-URL: Documentation, https://docs.pyvista.org/
 Project-URL: Bug Tracker, https://github.com/pyvista/pyvista/issues
 Project-URL: Source Code, https://github.com/pyvista/pyvista
 Keywords: vtk,numpy,plotting,mesh
```

### Comparing `pyvista-0.43.7/README.rst` & `pyvista-0.44.dev0/README.rst`

 * *Files identical despite different names*

### Comparing `pyvista-0.43.7/pyproject.toml` & `pyvista-0.44.dev0/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -163,14 +163,16 @@
 
 [tool.numpydoc_validation]
 checks = [
     "all",  # all but the following:
     "GL01",  # Contradicts numpydoc examples
     "GL02",  # Permit a blank line after the end of our docstring
     "GL03",  # Considering enforcing
+    "GL06",  # Found unknown section
+    "GL07",  # "Sections are in the wrong order. Correct order is: {correct_sections}",
     "GL09",  # Deprecation warning should precede extended summary (check broken)
     "SA01",  # Not all docstrings need a see also
     "SA04",  # See also section does not need descriptions
     "SS05",  # Appears to be broken.
     "ES01",  # Not all docstrings need an extend summary.
     "EX01",  # Examples: Will eventually enforce
     "YD01",  # Yields: No plan to enforce
@@ -309,7 +311,15 @@
     # we already check black
     # "BLK100",
     # 'from module import *' used; unable to detect undefined names
     "F403",
 ]
 fixable = ["ALL"]
 unfixable = []
+extend-select = [
+    "C4",
+    "NPY",
+    "PGH004",
+]
+
+[tool.ruff.lint.flake8-comprehensions]
+allow-dict-calls-with-keyword-arguments = true
```

### Comparing `pyvista-0.43.7/pyvista/__init__.py` & `pyvista-0.44.dev0/pyvista/__init__.py`

 * *Files identical despite different names*

### Comparing `pyvista-0.43.7/pyvista/_plot.py` & `pyvista-0.44.dev0/pyvista/_plot.py`

 * *Files identical despite different names*

### Comparing `pyvista-0.43.7/pyvista/core/__init__.py` & `pyvista-0.44.dev0/pyvista/core/__init__.py`

 * *Files identical despite different names*

### Comparing `pyvista-0.43.7/pyvista/core/_typing_core.py` & `pyvista-0.44.dev0/pyvista/core/_typing_core.py`

 * *Files identical despite different names*

### Comparing `pyvista-0.43.7/pyvista/core/_vtk_core.py` & `pyvista-0.44.dev0/pyvista/core/_vtk_core.py`

 * *Files 1% similar despite different names*

```diff
@@ -201,14 +201,15 @@
     from vtkmodules.vtkCommonDataModel import VTK_TRIQUADRATIC_PYRAMID
 except ImportError:  # pragma: no cover
     pass
 
 from vtkmodules.vtkCommonExecutionModel import (
     vtkAlgorithm,
     vtkAlgorithmOutput,
+    vtkCompositeDataPipeline,
     vtkImageToStructuredGrid,
 )
 from vtkmodules.vtkCommonMath import vtkMatrix3x3, vtkMatrix4x4
 from vtkmodules.vtkCommonTransforms import vtkTransform
 from vtkmodules.vtkFiltersCore import (
     VTK_BEST_FITTING_PLANE,
     vtkAppendArcLength,
@@ -303,15 +304,15 @@
     vtkSubdivideTetra,
     vtkTrimmedExtrusionFilter,
 )
 from vtkmodules.vtkFiltersParallel import vtkIntegrateAttributes
 
 try:
     from vtkmodules.vtkFiltersParallelDIY2 import vtkRedistributeDataSetFilter
-except ImportError:  # pragma: no cover
+except ModuleNotFoundError:  # pragma: no cover
     # `vtkmodules.vtkFiltersParallelDIY2` is unavailable in some versions of `vtk` from conda-forge
     pass
 from vtkmodules.vtkFiltersPoints import vtkGaussianKernel, vtkPointInterpolator
 from vtkmodules.vtkFiltersSources import (
     vtkArcSource,
     vtkArrowSource,
     vtkConeSource,
```

### Comparing `pyvista-0.43.7/pyvista/core/cell.py` & `pyvista-0.44.dev0/pyvista/core/cell.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 """Contains the pyvista.Cell class."""
 from __future__ import annotations
 
-from typing import List, Optional, Tuple, Union, cast
+from typing import List, Optional, Sequence, Tuple, Union, cast
 
 import numpy as np
 
 import pyvista
 
 from . import _vtk_core as _vtk
 from ._typing_core import IntMatrix, IntVector, NumpyIntArray
 from .celltype import CellType
 from .dataset import DataObject
+from .errors import CellSizeError
 from .utilities.cells import ncells_from_cells, numpy_to_idarr
 
 
 def _get_vtk_id_type():
     """Return the numpy datatype responding to ``vtk.vtkIdTypeArray``."""
     VTK_ID_TYPE_SIZE = _vtk.vtkIdTypeArray().GetDataTypeSize()
     if VTK_ID_TYPE_SIZE == 4:
@@ -633,14 +634,25 @@
         if n_cells is None:
             if cells.ndim == 1:
                 n_cells = ncells_from_cells(cells)
             else:
                 n_cells = cells.shape[0]
 
         self.SetCells(n_cells, vtk_idarr)
+
+        # https://github.com/pyvista/pyvista/pull/5404
+        if self.cells.size != cells.size:
+            raise CellSizeError(
+                message=(
+                    f"Cell array size is invalid. Size ({cells.size}) does not"
+                    f" match expected size ({self.cells.size}). This is likely"
+                    " due to invalid connectivity array."
+                )
+            )
+
         self.__offsets = self.__connectivity = None
         return None
 
     @property
     def cells(self) -> np.ndarray:  # numpydoc ignore=RT01
         """Return a numpy array of the cells.
 
@@ -762,14 +774,33 @@
         cells = np.asarray(cells, dtype=pyvista.ID_TYPE)
         n_cells, cell_size = cells.shape
         offsets = cell_size * np.arange(n_cells + 1, dtype=pyvista.ID_TYPE)
         cellarr = cls()
         cellarr._set_data(offsets, cells, deep=deep)
         return cellarr
 
+    @classmethod
+    def from_irregular_cells(cls, cells: Sequence[IntVector]) -> pyvista.CellArray:
+        """Construct a ``CellArray`` from a (n_cells, cell_size) array of cell indices.
+
+        Parameters
+        ----------
+        cells : numpy.ndarray or list[list[int]]
+            Cell array of shape (n_cells, cell_size) where all cells have the same size `cell_size`.
+
+        Returns
+        -------
+        pyvista.CellArray
+            Constructed ``CellArray``.
+        """
+        offsets = np.cumsum([len(c) for c in cells])
+        offsets = np.concatenate([[0], offsets], dtype=pyvista.ID_TYPE)
+        connectivity = np.concatenate(cells, dtype=pyvista.ID_TYPE)
+        return cls.from_arrays(offsets, connectivity)
+
 
 # The following methods would be much nicer bound to CellArray,
 # but then they wouldn't be available on bare vtkCellArrays. In the future,
 # consider using vtkCellArray.override decorator, so they're all automatically
 # returned as CellArrays
 
 
@@ -788,7 +819,17 @@
     cells = _get_connectivity_array(cellarr)
     if len(cells) == 0:
         return cells
 
     offsets = _get_offset_array(cellarr)
     cell_size = offsets[1] - offsets[0]
     return cells.reshape(-1, cell_size)
+
+
+def _get_irregular_cells(cellarr: _vtk.vtkCellArray) -> Tuple[NumpyIntArray, ...]:
+    """Return a tuple of length n_cells of each cell's point indices."""
+    cells = _get_connectivity_array(cellarr)
+    if len(cells) == 0:
+        return ()
+
+    offsets = _get_offset_array(cellarr)
+    return tuple(np.split(cells, offsets[1:-1]))
```

### Comparing `pyvista-0.43.7/pyvista/core/celltype.py` & `pyvista-0.44.dev0/pyvista/core/celltype.py`

 * *Files identical despite different names*

### Comparing `pyvista-0.43.7/pyvista/core/composite.py` & `pyvista-0.44.dev0/pyvista/core/composite.py`

 * *Files identical despite different names*

### Comparing `pyvista-0.43.7/pyvista/core/dataobject.py` & `pyvista-0.44.dev0/pyvista/core/dataobject.py`

 * *Files identical despite different names*

### Comparing `pyvista-0.43.7/pyvista/core/dataset.py` & `pyvista-0.44.dev0/pyvista/core/dataset.py`

 * *Files 0% similar despite different names*

```diff
@@ -1495,15 +1495,17 @@
         --------
         Add point arrays to a mesh and list the available ``point_data``.
 
         >>> import pyvista as pv
         >>> import numpy as np
         >>> mesh = pv.Cube()
         >>> mesh.clear_data()
-        >>> mesh.point_data['my_array'] = np.random.random(mesh.n_points)
+        >>> mesh.point_data['my_array'] = np.random.default_rng().random(
+        ...     mesh.n_points
+        ... )
         >>> mesh.point_data['my_other_array'] = np.arange(mesh.n_points)
         >>> mesh.point_data
         pyvista DataSetAttributes
         Association     : POINT
         Active Scalars  : my_array
         Active Vectors  : None
         Active Texture  : None
@@ -1587,15 +1589,17 @@
         --------
         Add cell arrays to a mesh and list the available ``cell_data``.
 
         >>> import pyvista as pv
         >>> import numpy as np
         >>> mesh = pv.Cube()
         >>> mesh.clear_data()
-        >>> mesh.cell_data['my_array'] = np.random.random(mesh.n_cells)
+        >>> mesh.cell_data['my_array'] = np.random.default_rng().random(
+        ...     mesh.n_cells
+        ... )
         >>> mesh.cell_data['my_other_array'] = np.arange(mesh.n_cells)
         >>> mesh.cell_data
         pyvista DataSetAttributes
         Association     : CELL
         Active Scalars  : my_array
         Active Vectors  : None
         Active Texture  : None
@@ -2401,15 +2405,15 @@
         >>> distance = np.linalg.norm(relative_position, axis=1)
         >>> np.argmin(distance)
         338
 
         Find the nearest cells to several random points that
         are centered on the origin.
 
-        >>> points = 2 * np.random.random((5000, 3)) - 1
+        >>> points = 2 * np.random.default_rng().random((5000, 3)) - 1
         >>> indices = mesh.find_closest_cell(points)
         >>> indices.shape
         (5000,)
 
         For the closest cell, find the point inside the cell that is
         closest to the supplied point.  The rectangle is a unit square
         with 1 cell and 4 nodal points at the corners in the plane with
@@ -2508,15 +2512,15 @@
 
         >>> mesh.find_containing_cell([0.3, 0.3, 1.0])
         -1
 
         Find the cells that contain 1000 random points inside the mesh.
 
         >>> import numpy as np
-        >>> points = np.random.random((1000, 3))
+        >>> points = np.random.default_rng().random((1000, 3))
         >>> indices = mesh.find_containing_cell(points)
         >>> indices.shape
         (1000,)
 
         """
         point, singular = _coerce_pointslike_arg(point, copy=False)
```

### Comparing `pyvista-0.43.7/pyvista/core/datasetattributes.py` & `pyvista-0.44.dev0/pyvista/core/datasetattributes.py`

 * *Files 2% similar despite different names*

```diff
@@ -103,17 +103,17 @@
 
     Print the available arrays from dataset attributes.
 
     >>> import numpy as np
     >>> mesh = pv.Plane(i_resolution=1, j_resolution=1)
     >>> mesh.point_data.set_array(range(4), 'my-data')
     >>> mesh.point_data.set_array(range(5, 9), 'my-other-data')
-    >>> vectors0 = np.random.random((4, 3))
+    >>> vectors0 = np.random.default_rng().random((4, 3))
     >>> mesh.point_data.set_vectors(vectors0, 'vectors0')
-    >>> vectors1 = np.random.random((4, 3))
+    >>> vectors1 = np.random.default_rng().random((4, 3))
     >>> mesh.point_data.set_vectors(vectors1, 'vectors1')
     >>> mesh.point_data
     pyvista DataSetAttributes
     Association     : POINT
     Active Scalars  : None
     Active Vectors  : vectors1
     Active Texture  : TextureCoordinates
@@ -318,15 +318,15 @@
         Associate point data to a simple cube mesh and show that the
         active vectors in the point array are the most recently added
         array.
 
         >>> import pyvista as pv
         >>> import numpy as np
         >>> mesh = pv.Cube()
-        >>> vectors = np.random.random((mesh.n_points, 3))
+        >>> vectors = np.random.default_rng().random((mesh.n_points, 3))
         >>> mesh.point_data.set_vectors(vectors, 'my-vectors')
         >>> vectors_out = mesh.point_data.active_vectors
         >>> vectors_out.shape
         (8, 3)
 
         """
         self._raise_field_data_no_scalars_vectors()
@@ -667,15 +667,15 @@
         --------
         Add random vectors to a mesh as point data.
 
         >>> import pyvista as pv
         >>> import numpy as np
         >>> mesh = pv.Cube()
         >>> mesh.clear_data()
-        >>> vectors = np.random.random((mesh.n_points, 3))
+        >>> vectors = np.random.default_rng().random((mesh.n_points, 3))
         >>> mesh.point_data.set_vectors(vectors, 'my-vectors')
         >>> mesh.point_data
         pyvista DataSetAttributes
         Association     : POINT
         Active Scalars  : None
         Active Vectors  : my-vectors
         Active Texture  : None
@@ -1018,15 +1018,15 @@
 
         >>> import numpy as np
         >>> from pyvista import examples
         >>> mesh = examples.load_uniform()
         >>> n = len(mesh.point_data)
         >>> arrays = {
         ...     'foo': np.arange(mesh.n_points),
-        ...     'rand': np.random.random(mesh.n_points),
+        ...     'rand': np.random.default_rng().random(mesh.n_points),
         ... }
         >>> mesh.point_data.update(arrays)
         >>> mesh.point_data
         pyvista DataSetAttributes
         Association     : POINT
         Active Scalars  : Spatial Point Data
         Active Vectors  : None
@@ -1121,15 +1121,16 @@
 
         Examples
         --------
         >>> import pyvista as pv
         >>> import numpy as np
         >>> mesh = pv.Sphere()
         >>> mesh.point_data.set_vectors(
-        ...     np.random.random((mesh.n_points, 3)), 'my-vectors'
+        ...     np.random.default_rng().random((mesh.n_points, 3)),
+        ...     'my-vectors',
         ... )
         >>> mesh.point_data.active_vectors_name
         'my-vectors'
 
         """
         if self.GetVectors() is not None:
             return str(self.GetVectors().GetName())
```

### Comparing `pyvista-0.43.7/pyvista/core/errors.py` & `pyvista-0.44.dev0/pyvista/core/errors.py`

 * *Files 4% similar despite different names*

```diff
@@ -125,14 +125,29 @@
     """
 
     def __init__(self, message="Multiple data available."):
         """Call the base class constructor with the custom message."""
         super().__init__(message)
 
 
+class CellSizeError(ValueError):
+    """Exception when a cell array size is invalid.
+
+    Parameters
+    ----------
+    message : str
+        Error message.
+
+    """
+
+    def __init__(self, message="Cell array size is invalid."):
+        """Call the base class constructor with the custom message."""
+        super().__init__(message)
+
+
 class PyVistaPipelineError(RuntimeError):
     """Exception when a VTK pipeline runs into an issue.
 
     Parameters
     ----------
     message : str
         Error message.
```

### Comparing `pyvista-0.43.7/pyvista/core/filters/__init__.py` & `pyvista-0.44.dev0/pyvista/core/filters/__init__.py`

 * *Files identical despite different names*

### Comparing `pyvista-0.43.7/pyvista/core/filters/composite.py` & `pyvista-0.44.dev0/pyvista/core/filters/composite.py`

 * *Files identical despite different names*

### Comparing `pyvista-0.43.7/pyvista/core/filters/data_set.py` & `pyvista-0.44.dev0/pyvista/core/filters/data_set.py`

 * *Files 2% similar despite different names*

```diff
@@ -3739,20 +3739,20 @@
 
         Examples
         --------
         Interpolate the values of 5 points onto a sample plane.
 
         >>> import pyvista as pv
         >>> import numpy as np
-        >>> np.random.seed(7)
-        >>> point_cloud = np.random.random((5, 3))
+        >>> rng = np.random.default_rng(7)
+        >>> point_cloud = rng.random((5, 3))
         >>> point_cloud[:, 2] = 0
         >>> point_cloud -= point_cloud.mean(0)
         >>> pdata = pv.PolyData(point_cloud)
-        >>> pdata['values'] = np.random.random(5)
+        >>> pdata['values'] = rng.random(5)
         >>> plane = pv.Plane()
         >>> plane.clear_data()
         >>> plane = plane.interpolate(pdata, sharpness=3)
         >>> pl = pv.Plotter()
         >>> _ = pl.add_mesh(
         ...     pdata, render_points_as_spheres=True, point_size=50
         ... )
@@ -4339,20 +4339,20 @@
 
         Examples
         --------
         Sample over a plane that is interpolating a point cloud.
 
         >>> import pyvista as pv
         >>> import numpy as np
-        >>> np.random.seed(12)
-        >>> point_cloud = np.random.random((5, 3))
+        >>> rng = np.random.default_rng(12)
+        >>> point_cloud = rng.random((5, 3))
         >>> point_cloud[:, 2] = 0
         >>> point_cloud -= point_cloud.mean(0)
         >>> pdata = pv.PolyData(point_cloud)
-        >>> pdata['values'] = np.random.random(5)
+        >>> pdata['values'] = rng.random(5)
         >>> plane = pv.Plane()
         >>> plane.clear_data()
         >>> plane = plane.interpolate(pdata, sharpness=3.5)
         >>> sample = plane.sample_over_line((-0.5, -0.5, 0), (0.5, 0.5, 0))
         >>> pl = pv.Plotter()
         >>> _ = pl.add_mesh(
         ...     pdata, render_points_as_spheres=True, point_size=50
@@ -4494,20 +4494,20 @@
 
         Examples
         --------
         Sample over a plane that is interpolating a point cloud.
 
         >>> import pyvista as pv
         >>> import numpy as np
-        >>> np.random.seed(12)
-        >>> point_cloud = np.random.random((5, 3))
+        >>> rng = np.random.default_rng(12)
+        >>> point_cloud = rng.random((5, 3))
         >>> point_cloud[:, 2] = 0
         >>> point_cloud -= point_cloud.mean(0)
         >>> pdata = pv.PolyData(point_cloud)
-        >>> pdata['values'] = np.random.random(5)
+        >>> pdata['values'] = rng.random(5)
         >>> plane = pv.Plane()
         >>> plane.clear_data()
         >>> plane = plane.interpolate(pdata, sharpness=3.5)
         >>> sample = plane.sample_over_multiple_lines(
         ...     [[-0.5, -0.5, 0], [0.5, -0.5, 0], [0.5, 0.5, 0]]
         ... )
         >>> pl = pv.Plotter()
```

### Comparing `pyvista-0.43.7/pyvista/core/filters/image_data.py` & `pyvista-0.44.dev0/pyvista/core/filters/image_data.py`

 * *Files identical despite different names*

### Comparing `pyvista-0.43.7/pyvista/core/filters/poly_data.py` & `pyvista-0.44.dev0/pyvista/core/filters/poly_data.py`

 * *Files 0% similar despite different names*

```diff
@@ -519,15 +519,15 @@
         if is_polydata:
             # if either of the input datasets contained lines or strips, we
             # must use extract_geometry to ensure they get converted back
             # correctly. This incurrs a performance penalty, but is needed to
             # maintain data consistency.
             if isinstance(dataset, (list, tuple, pyvista.MultiBlock)):
                 dataset_has_lines_strips = any(
-                    [ds.n_lines or ds.n_strips or ds.n_verts for ds in dataset]
+                    ds.n_lines or ds.n_strips or ds.n_verts for ds in dataset
                 )
             else:
                 dataset_has_lines_strips = dataset.n_lines or dataset.n_strips or dataset.n_verts
 
             if self.n_lines or self.n_strips or self.n_verts or dataset_has_lines_strips:
                 merged = merged.extract_geometry()
             else:
@@ -2259,17 +2259,17 @@
         'Rays intersected at (0.499, 0.000, 0.000), (0.000, 0.497, 0.000), (0.000, 0.000, 0.500)'
 
         """
         if not self.is_all_triangles:
             raise NotAllTrianglesError("Input mesh for multi_ray_trace must be all triangles.")
 
         try:
-            import pyembree  # noqa
-            import rtree  # noqa
-            import trimesh  # noqa
+            import pyembree  # noqa: F401
+            import rtree  # noqa: F401
+            import trimesh  # noqa: F401
         except ImportError:
             raise ImportError(
                 "To use multi_ray_trace please install trimesh, rtree and pyembree with:\n"
                 "\tconda install trimesh rtree pyembree"
             )
 
         origins = np.asarray(origins)
@@ -2290,24 +2290,15 @@
 
             # compute ray points for all failed rays at once
             origins_retry = origins[retry_ray_indices, :]  # shape (n_retry, 3)
             directions_retry = directions[retry_ray_indices, :]
             unit_directions = directions_retry / np.linalg.norm(
                 directions_retry, axis=1, keepdims=True
             )
-
-            origin_to_centre_vector = (
-                (self.bounds[0] + self.bounds[1]) / 2 - origins_retry[0],
-                (self.bounds[2] + self.bounds[3]) / 2 - origins_retry[1],
-                (self.bounds[4] + self.bounds[5]) / 2 - origins_retry[2],
-            )
-            origin_to_centre_length = np.linalg.norm(origin_to_centre_vector)
-            second_points = origins_retry + unit_directions * (
-                self.length + origin_to_centre_length
-            )  # shape (n_retry, 3)
+            second_points = origins_retry + unit_directions * self.length  # shape (n_retry, 3)
 
             for id_r, origin, second_point in zip(retry_ray_indices, origins_retry, second_points):
                 locs, indices = self.ray_trace(origin, second_point, first_point=first_point)
                 if locs.any():
                     if first_point:
                         locs = locs.reshape([1, 3])
                     ray_lst.extend([id_r] * indices.size)
```

### Comparing `pyvista-0.43.7/pyvista/core/filters/rectilinear_grid.py` & `pyvista-0.44.dev0/pyvista/core/filters/rectilinear_grid.py`

 * *Files 2% similar despite different names*

```diff
@@ -104,16 +104,16 @@
                     f'`tetra_per_cell` should be either 5, 6, or 12, not {tetra_per_cell}'
                 )
 
             # Edge case causing a seg-fault where grid is flat in one dimension
             # See: https://gitlab.kitware.com/vtk/vtk/-/issues/18650
             if 1 in self.dimensions and tetra_per_cell == 12:  # type: ignore
                 raise RuntimeError(
-                    'Cannot split cells into 12 tetrahedrals when at least '
-                    f'one dimension is 1. Dimensions are {self.dimensions}.'  # type: ignore[attr-defined]
+                    'Cannot split cells into 12 tetrahedrals when at least '  # type: ignore
+                    f'one dimension is 1. Dimensions are {self.dimensions}.'
                 )
 
             alg.SetTetraPerCell(tetra_per_cell)
 
         alg.SetInputData(self)
         _update_alg(alg, progress_bar, 'Converting to tetrahedra')
         out = _get_output(alg)
```

### Comparing `pyvista-0.43.7/pyvista/core/filters/structured_grid.py` & `pyvista-0.44.dev0/pyvista/core/filters/structured_grid.py`

 * *Files identical despite different names*

### Comparing `pyvista-0.43.7/pyvista/core/filters/unstructured_grid.py` & `pyvista-0.44.dev0/pyvista/core/filters/unstructured_grid.py`

 * *Files identical despite different names*

### Comparing `pyvista-0.43.7/pyvista/core/grid.py` & `pyvista-0.44.dev0/pyvista/core/grid.py`

 * *Files 1% similar despite different names*

```diff
@@ -663,15 +663,15 @@
         nx, ny, nz = self.dimensions
         nx -= 1
         ny -= 1
         nz -= 1
         # get the points and convert to spacings
         dx, dy, dz = self.spacing
         # Now make the cell arrays
-        ox, oy, oz = np.array(self.origin) + self.extent[::2] * np.array([dx, dy, dz])
+        ox, oy, oz = np.array(self.origin) + np.array(self.extent[::2])  # type: ignore
         x = np.insert(np.cumsum(np.full(nx, dx)), 0, 0.0) + ox
         y = np.insert(np.cumsum(np.full(ny, dy)), 0, 0.0) + oy
         z = np.insert(np.cumsum(np.full(nz, dz)), 0, 0.0) + oz
         xx, yy, zz = np.meshgrid(x, y, z, indexing='ij')
         return np.c_[xx.ravel(order='F'), yy.ravel(order='F'), zz.ravel(order='F')]
 
     @points.setter
```

### Comparing `pyvista-0.43.7/pyvista/core/input_validation/__init__.py` & `pyvista-0.44.dev0/pyvista/core/input_validation/__init__.py`

 * *Files identical despite different names*

### Comparing `pyvista-0.43.7/pyvista/core/input_validation/check.py` & `pyvista-0.44.dev0/pyvista/core/input_validation/check.py`

 * *Files identical despite different names*

### Comparing `pyvista-0.43.7/pyvista/core/input_validation/validate.py` & `pyvista-0.44.dev0/pyvista/core/input_validation/validate.py`

 * *Files identical despite different names*

### Comparing `pyvista-0.43.7/pyvista/core/objects.py` & `pyvista-0.44.dev0/pyvista/core/objects.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,15 +21,15 @@
     Create by passing a 2D NumPy array of shape (``n_rows`` by ``n_columns``)
     or from a dictionary containing NumPy arrays.
 
     Examples
     --------
     >>> import pyvista as pv
     >>> import numpy as np
-    >>> arrays = np.random.rand(100, 3)
+    >>> arrays = np.random.default_rng().random((100, 3))
     >>> table = pv.Table(arrays)
 
     """
 
     def __init__(self, *args, **kwargs):
         """Initialize the table."""
         super().__init__(*args, **kwargs)
```

### Comparing `pyvista-0.43.7/pyvista/core/pointset.py` & `pyvista-0.44.dev0/pyvista/core/pointset.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """Sub-classes and wrappers for vtk.vtkPointSet."""
 import collections.abc
 from functools import wraps
 import numbers
 import os
 import pathlib
 from textwrap import dedent
-from typing import Optional, Tuple, Union, cast
+from typing import Optional, Sequence, Tuple, Union, cast
 import warnings
 
 import numpy as np
 
 import pyvista
 
 from . import _vtk_core as _vtk
@@ -20,15 +20,21 @@
     IntMatrix,
     IntVector,
     Matrix,
     NumpyIntArray,
     NumpyUINT8Array,
     Vector,
 )
-from .cell import CellArray, _get_connectivity_array, _get_offset_array, _get_regular_cells
+from .cell import (
+    CellArray,
+    _get_connectivity_array,
+    _get_irregular_cells,
+    _get_offset_array,
+    _get_regular_cells,
+)
 from .celltype import CellType
 from .dataset import DataSet
 from .errors import (
     PointSetCellOperationError,
     PointSetDimensionReductionError,
     PointSetNotSupported,
     PyVistaDeprecationWarning,
@@ -735,15 +741,15 @@
 
         Examples
         --------
         Create a point cloud polydata and return the vertex cells.
 
         >>> import pyvista as pv
         >>> import numpy as np
-        >>> points = np.random.random((5, 3))
+        >>> points = np.random.default_rng().random((5, 3))
         >>> pdata = pv.PolyData(points)
         >>> pdata.verts
         array([1, 0, 1, 1, 1, 2, 1, 3, 1, 4])
 
         Set vertex cells.  Note how the mesh plots both the surface
         mesh and the additional vertices in a single plot.
 
@@ -776,15 +782,15 @@
 
         Examples
         --------
         Return the lines from a spline.
 
         >>> import pyvista as pv
         >>> import numpy as np
-        >>> points = np.random.random((3, 3))
+        >>> points = np.random.default_rng().random((3, 3))
         >>> spline = pv.Spline(points, 10)
         >>> spline.lines
         array([10,  0,  1,  2,  3,  4,  5,  6,  7,  8,  9])
 
         """
         return _vtk.vtk_to_numpy(self.GetLines().GetData()).ravel()
 
@@ -923,29 +929,114 @@
             Whether to deep copy the faces array into vtkCellArray connectivity data.
 
         Returns
         -------
         pyvista.PolyData
             The newly constructed mesh.
 
+        See Also
+        --------
+        pyvista.PolyData.from_irregular_faces
+
         Examples
         --------
         Construct a tetrahedron from four triangles
 
         >>> import pyvista as pv
         >>> points = [[1.0, 1, 1], [-1, 1, -1], [1, -1, -1], [-1, -1, 1]]
         >>> faces = [[0, 1, 2], [1, 3, 2], [0, 2, 3], [0, 3, 1]]
         >>> tetra = pv.PolyData.from_regular_faces(points, faces)
+        >>> tetra.plot()
         """
         p = cls()
         p.points = points  # type: ignore
         p.faces = CellArray.from_regular_cells(faces, deep=deep)  # type: ignore
         return p
 
     @property
+    def irregular_faces(self) -> Tuple[NumpyIntArray, ...]:  # numpydoc ignore=RT01
+        """Return a tuple of face arrays.
+
+        Returns
+        -------
+        tuple[numpy.ndarray]
+            Tuple of length n_faces where each element is an array of point
+            indices for points in that face.
+
+        See Also
+        --------
+        pyvista.PolyData.faces
+        pyvista.PolyData.regular_faces
+
+        Examples
+        --------
+        Get the face arrays of the five faces of a pyramid.
+
+        >>> import pyvista as pv
+        >>> pyramid = pv.Pyramid().extract_surface()
+        >>> pyramid.irregular_faces
+        (array([0, 1, 2, 3]), array([0, 3, 4]), array([0, 4, 1]), array([3, 2, 4]), array([2, 1, 4]))
+
+        """
+        return _get_irregular_cells(self.GetPolys())
+
+    @irregular_faces.setter
+    def irregular_faces(self, faces: Sequence[IntVector]):  # numpydoc ignore=PR01
+        """Set the faces from a sequence of face arrays."""
+        self.faces = CellArray.from_irregular_cells(faces)
+
+    @classmethod
+    def from_irregular_faces(cls, points: Matrix, faces: Sequence[IntVector]):
+        """Alternate `pyvista.PolyData` convenience constructor from point and ragged face arrays.
+
+        Parameters
+        ----------
+        points : Matrix
+            A (n_points, 3) array of points.
+
+        faces : Sequence[IntVector]
+            A sequence of face vectors containing point indices.
+
+        Returns
+        -------
+        pyvista.PolyData
+            The newly constructed mesh.
+
+        See Also
+        --------
+        pyvista.PolyData.from_regular_faces
+
+        Examples
+        --------
+        Construct a pyramid from five points and five faces
+
+        >>> import pyvista as pv
+        >>> points = [
+        ...     (1, 1, 0),
+        ...     (-1, 1, 0),
+        ...     (-1, -1, 0),
+        ...     (1, -1, 0),
+        ...     (0, 0, 1.61),
+        ... ]
+        >>> faces = [
+        ...     (0, 1, 2, 3),
+        ...     (0, 3, 4),
+        ...     (0, 4, 1),
+        ...     (3, 2, 4),
+        ...     (2, 1, 4),
+        ... ]
+        >>> pyramid = pv.PolyData.from_irregular_faces(points, faces)
+        >>> pyramid.plot()
+        """
+        p = cls()
+        p.points = points  # type: ignore
+        p.faces = CellArray.from_irregular_cells(faces)  # type: ignore
+        return p
+
+    @property
     def strips(self) -> np.ndarray:  # numpydoc ignore=RT01
         """Return a pointer to the strips as a numpy array.
 
         Returns
         -------
         numpy.ndarray
             Array of strip indices.
```

### Comparing `pyvista-0.43.7/pyvista/core/pyvista_ndarray.py` & `pyvista-0.44.dev0/pyvista/core/pyvista_ndarray.py`

 * *Files identical despite different names*

### Comparing `pyvista-0.43.7/pyvista/core/utilities/__init__.py` & `pyvista-0.44.dev0/pyvista/core/utilities/__init__.py`

 * *Files identical despite different names*

### Comparing `pyvista-0.43.7/pyvista/core/utilities/arrays.py` & `pyvista-0.44.dev0/pyvista/core/utilities/arrays.py`

 * *Files identical despite different names*

### Comparing `pyvista-0.43.7/pyvista/core/utilities/cell_type_helper.py` & `pyvista-0.44.dev0/pyvista/core/utilities/cell_type_helper.py`

 * *Files identical despite different names*

### Comparing `pyvista-0.43.7/pyvista/core/utilities/cells.py` & `pyvista-0.44.dev0/pyvista/core/utilities/cells.py`

 * *Files identical despite different names*

### Comparing `pyvista-0.43.7/pyvista/core/utilities/docs.py` & `pyvista-0.44.dev0/pyvista/core/utilities/docs.py`

 * *Files identical despite different names*

### Comparing `pyvista-0.43.7/pyvista/core/utilities/features.py` & `pyvista-0.44.dev0/pyvista/core/utilities/features.py`

 * *Files identical despite different names*

### Comparing `pyvista-0.43.7/pyvista/core/utilities/fileio.py` & `pyvista-0.44.dev0/pyvista/core/utilities/fileio.py`

 * *Files identical despite different names*

### Comparing `pyvista-0.43.7/pyvista/core/utilities/geometric_objects.py` & `pyvista-0.44.dev0/pyvista/core/utilities/geometric_objects.py`

 * *Files 2% similar despite different names*

```diff
@@ -1637,15 +1637,15 @@
 
     arc.Update()
     angle = np.deg2rad(arc.GetAngle())
     arc = wrap(arc.GetOutput())
     # Compute distance of every point along circular arc
     center = np.array(center).ravel()
     radius = np.sqrt(np.sum((arc.points[0] - center) ** 2, axis=0))
-    angles = np.linspace(0.0, 1.0, arc.n_points) * angle
+    angles = np.arange(0.0, 1.0 + 1.0 / resolution, 1.0 / resolution) * angle
     arc['Distance'] = radius * angles
     return arc
 
 
 def CircularArcFromNormal(center, resolution=100, normal=None, polar=None, angle=None):
     """Create a circular arc defined by normal to the plane of the arc, and an angle.
 
@@ -1854,32 +1854,27 @@
     point_1 = points[1]
     point_2 = points[2]
 
     vec_01 = point_1 - point_0
     vec_02 = point_2 - point_0
     vec_12 = point_2 - point_1
 
-    mag_01 = np.linalg.norm(vec_01)
-    mag_02 = np.linalg.norm(vec_02)
-    mag_12 = np.linalg.norm(vec_12)
-
-    if np.isclose(mag_01, 0) or np.isclose(mag_02, 0) or np.isclose(mag_12, 0):
-        raise ValueError("Unable to build a rectangle with less than three different points")
-
-    scalar_pdct_01_02 = np.dot(vec_01, vec_02) / min(mag_01, mag_02) ** 2
-    scalar_pdct_01_12 = np.dot(vec_01, vec_12) / min(mag_01, mag_12) ** 2
-    scalar_pdct_02_12 = np.dot(vec_02, vec_12) / min(mag_02, mag_12) ** 2
+    scalar_pdct_01_02 = np.dot(vec_01, vec_02)
+    scalar_pdct_01_12 = np.dot(vec_01, vec_12)
+    scalar_pdct_02_12 = np.dot(vec_02, vec_12)
 
     null_scalar_products = [
         val
         for val in [scalar_pdct_01_02, scalar_pdct_01_12, scalar_pdct_02_12]
         if np.isclose(val, 0)
     ]
     if len(null_scalar_products) == 0:
         raise ValueError("The three points should defined orthogonal vectors")
+    if len(null_scalar_products) > 1:
+        raise ValueError("Unable to build a rectangle with less than three different points")
 
     points = np.array([point_0, point_1, point_2, point_0])
     if np.isclose(scalar_pdct_01_02, 0):
         points[3] = point_0 + vec_01 + vec_02
         cells = np.array([[4, 0, 1, 3, 2]])
     elif np.isclose(scalar_pdct_01_12, 0):
         points[3] = point_1 + vec_12 - vec_01
```

### Comparing `pyvista-0.43.7/pyvista/core/utilities/geometric_sources.py` & `pyvista-0.44.dev0/pyvista/core/utilities/geometric_sources.py`

 * *Files 0% similar despite different names*

```diff
@@ -51,15 +51,15 @@
     trans[:3, 0] = normx
     trans[:3, 1] = normy
     trans[:3, 2] = normz
     trans[3, 3] = 1
 
     surf.transform(trans)
     if not np.allclose(center, [0.0, 0.0, 0.0]):
-        surf.points += np.array(center, dtype=surf.points.dtype)
+        surf.points += np.array(center)
 
 
 @no_new_attr
 class ConeSource(_vtk.vtkConeSource):
     """Cone source algorithm class.
 
     Parameters
@@ -193,15 +193,15 @@
         ----------
         height : float
             Height of the cone.
         """
         self.SetHeight(height)
 
     @property
-    def radius(self) -> float:
+    def radius(self) -> bool:
         """Get base radius of the cone.
 
         Returns
         -------
         float
             Base radius of the cone.
         """
```

### Comparing `pyvista-0.43.7/pyvista/core/utilities/helpers.py` & `pyvista-0.44.dev0/pyvista/core/utilities/helpers.py`

 * *Files 1% similar despite different names*

```diff
@@ -44,15 +44,15 @@
 
     Examples
     --------
     Wrap a numpy array representing a random point cloud.
 
     >>> import numpy as np
     >>> import pyvista as pv
-    >>> points = np.random.random((10, 3))
+    >>> points = np.random.default_rng().random((10, 3))
     >>> cloud = pv.wrap(points)
     >>> cloud
     PolyData (...)
       N Cells:    10
       N Points:   10
       N Strips:   0
       X Bounds:   ...
```

### Comparing `pyvista-0.43.7/pyvista/core/utilities/misc.py` & `pyvista-0.44.dev0/pyvista/core/utilities/misc.py`

 * *Files identical despite different names*

### Comparing `pyvista-0.43.7/pyvista/core/utilities/observers.py` & `pyvista-0.44.dev0/pyvista/core/utilities/observers.py`

 * *Files 0% similar despite different names*

```diff
@@ -204,15 +204,15 @@
         Message to display in the progress bar.
 
     """
 
     def __init__(self, algorithm, message=""):
         """Initialize observer."""
         try:
-            from tqdm import tqdm  # noqa
+            from tqdm import tqdm  # noqa: F401
         except ImportError:
             raise ImportError("Please install `tqdm` to monitor algorithms.")
         self.event_type = _vtk.vtkCommand.ProgressEvent
         self.progress = 0.0
         self._last_progress = self.progress
         self.algorithm = algorithm
         self.message = message
```

### Comparing `pyvista-0.43.7/pyvista/core/utilities/parametric_objects.py` & `pyvista-0.44.dev0/pyvista/core/utilities/parametric_objects.py`

 * *Files identical despite different names*

### Comparing `pyvista-0.43.7/pyvista/core/utilities/points.py` & `pyvista-0.44.dev0/pyvista/core/utilities/points.py`

 * *Files 0% similar despite different names*

```diff
@@ -31,15 +31,15 @@
     vtk.vtkPoints
         The vtkPoints object.
 
     Examples
     --------
     >>> import pyvista as pv
     >>> import numpy as np
-    >>> points = np.random.random((10, 3))
+    >>> points = np.random.default_rng().random((10, 3))
     >>> vpoints = pv.vtk_points(points)
     >>> vpoints  # doctest:+SKIP
     (vtkmodules.vtkCommonCore.vtkPoints)0x7f0c2e26af40
 
     """
     points = np.asanyarray(points)
 
@@ -209,15 +209,15 @@
     --------
     Fit a plane to a random point cloud.
 
     >>> import pyvista as pv
     >>> import numpy as np
     >>>
     >>> # Create point cloud
-    >>> cloud = np.random.random((10, 3))
+    >>> cloud = np.random.default_rng().random((10, 3))
     >>> cloud[:, 2] *= 0.1
     >>>
     >>> # Fit plane
     >>> plane, center, normal = pv.fit_plane_to_points(
     ...     cloud, return_meta=True
     ... )
     >>>
```

### Comparing `pyvista-0.43.7/pyvista/core/utilities/reader.py` & `pyvista-0.44.dev0/pyvista/core/utilities/reader.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 import pathlib
 from typing import Any, Callable, List, Union
 from xml.etree import ElementTree
 
 import numpy as np
 
 import pyvista
+from pyvista.core import _vtk_core as _vtk
 
 from .fileio import _get_ext_force, _process_filename
 from .helpers import wrap
 from .misc import abstract_class
 
 HDF_HELP = 'https://kitware.github.io/vtk-examples/site/VTKFileFormats/#hdf-file-formats'
 
@@ -2402,15 +2403,15 @@
     >>> mesh.plot(rgba=True, zoom='tight', border=True, border_width=2)
 
     """
 
     _class_reader = _GIFReader
 
 
-class XdmfReader(BaseReader, PointCellDataSelection):
+class XdmfReader(BaseReader, PointCellDataSelection, TimeReader):
     """XdmfReader for .xdmf files.
 
     Notes
     -----
     We currently can't inspect the time values for this reader.
 
     Parameters
@@ -2443,16 +2444,44 @@
         int
             The number of grids to be read.
 
         """
         return self.reader.GetNumberOfGrids()
 
     def set_active_time_value(self, time_value):  # noqa: D102
+        if time_value not in self.time_values:
+            raise ValueError(
+                f"Not a valid time {time_value} from available time values: {self.time_values}"
+            )
+        self._active_time_value = time_value
         self.reader.UpdateTimeStep(time_value)
 
+    @property
+    def number_time_points(self):  # noqa: D102
+        return len(self.time_values)
+
+    def time_point_value(self, time_point):  # noqa: D102
+        return self.time_values[time_point]
+
+    @property
+    def time_values(self):  # noqa: D102
+        info = self.reader.GetOutputInformation(0)
+        return list(info.Get(_vtk.vtkCompositeDataPipeline.TIME_STEPS()))
+
+    @property
+    def active_time_value(self):  # noqa: D102
+        return self._active_time_value
+
+    def set_active_time_point(self, time_point):  # noqa: D102
+        self.set_active_time_value(self.time_values[time_point])
+
+    def _set_defaults_post(self):
+        self._active_time_value = self.time_values[0]
+        self.set_active_time_value(self._active_time_value)
+
 
 CLASS_READERS = {
     # Standard dataset readers:
     '.bmp': BMPReader,
     '.cas': FluentReader,
     '.case': EnSightReader,
     '.cgns': CGNSReader,
```

### Comparing `pyvista-0.43.7/pyvista/core/utilities/transformations.py` & `pyvista-0.44.dev0/pyvista/core/utilities/transformations.py`

 * *Files identical despite different names*

### Comparing `pyvista-0.43.7/pyvista/core/wrappers.py` & `pyvista-0.44.dev0/pyvista/core/wrappers.py`

 * *Files identical despite different names*

### Comparing `pyvista-0.43.7/pyvista/demos/demos.py` & `pyvista-0.44.dev0/pyvista/demos/demos.py`

 * *Files identical despite different names*

### Comparing `pyvista-0.43.7/pyvista/demos/logo.py` & `pyvista-0.44.dev0/pyvista/demos/logo.py`

 * *Files identical despite different names*

### Comparing `pyvista-0.43.7/pyvista/errors.py` & `pyvista-0.44.dev0/pyvista/errors.py`

 * *Files identical despite different names*

### Comparing `pyvista-0.43.7/pyvista/examples/2k_earth_daymap.jpg` & `pyvista-0.44.dev0/pyvista/examples/2k_earth_daymap.jpg`

 * *Files identical despite different names*

### Comparing `pyvista-0.43.7/pyvista/examples/airplane.ply` & `pyvista-0.44.dev0/pyvista/examples/airplane.ply`

 * *Files identical despite different names*

### Comparing `pyvista-0.43.7/pyvista/examples/ant.ply` & `pyvista-0.44.dev0/pyvista/examples/ant.ply`

 * *Files identical despite different names*

### Comparing `pyvista-0.43.7/pyvista/examples/cells.py` & `pyvista-0.44.dev0/pyvista/examples/cells.py`

 * *Files identical despite different names*

### Comparing `pyvista-0.43.7/pyvista/examples/channels.vti` & `pyvista-0.44.dev0/pyvista/examples/channels.vti`

 * *Files identical despite different names*

### Comparing `pyvista-0.43.7/pyvista/examples/downloads.py` & `pyvista-0.44.dev0/pyvista/examples/downloads.py`

 * *Files 0% similar despite different names*

```diff
@@ -6552,2958 +6552,3025 @@
 00019970: 7374 7265 6574 5f6d 6170 5f65 7861 6d70  street_map_examp
 00019980: 6c65 6020 666f 7220 6120 6675 6c6c 2065  le` for a full e
 00019990: 7861 6d70 6c65 2075 7369 6e67 2074 6869  xample using thi
 000199a0: 7320 6461 7461 7365 742e 0a0a 2020 2020  s dataset...    
 000199b0: 2222 220a 2020 2020 696d 706f 7274 2070  """.    import p
 000199c0: 6963 6b6c 650a 0a20 2020 2074 7279 3a0a  ickle..    try:.
 000199d0: 2020 2020 2020 2020 696d 706f 7274 206f          import o
-000199e0: 736d 6e78 2020 2320 6e6f 7161 0a20 2020  smnx  # noqa.   
-000199f0: 2065 7863 6570 7420 496d 706f 7274 4572   except ImportEr
-00019a00: 726f 723a 0a20 2020 2020 2020 2072 6169  ror:.        rai
-00019a10: 7365 2049 6d70 6f72 7445 7272 6f72 2827  se ImportError('
-00019a20: 496e 7374 616c 6c20 606f 736d 6e78 6020  Install `osmnx` 
-00019a30: 746f 2075 7365 2074 6869 7320 6578 616d  to use this exam
-00019a40: 706c 6527 290a 0a20 2020 2066 696c 656e  ple')..    filen
-00019a50: 616d 6520 3d20 646f 776e 6c6f 6164 5f66  ame = download_f
-00019a60: 696c 6528 276f 736d 6e78 5f67 7261 7068  ile('osmnx_graph
-00019a70: 2e70 2729 0a20 2020 2072 6574 7572 6e20  .p').    return 
-00019a80: 7069 636b 6c65 2e6c 6f61 6428 6f70 656e  pickle.load(open
-00019a90: 2866 696c 656e 616d 652c 2027 7262 2729  (filename, 'rb')
-00019aa0: 290a 0a0a 6465 6620 646f 776e 6c6f 6164  )...def download
-00019ab0: 5f63 6176 6974 7928 6c6f 6164 3d54 7275  _cavity(load=Tru
-00019ac0: 6529 3a20 2023 2070 7261 676d 613a 206e  e):  # pragma: n
-00019ad0: 6f20 636f 7665 720a 2020 2020 2222 2244  o cover.    """D
-00019ae0: 6f77 6e6c 6f61 6420 6361 7669 7479 204f  ownload cavity O
-00019af0: 7065 6e46 4f41 4d20 6578 616d 706c 652e  penFOAM example.
-00019b00: 0a0a 2020 2020 5265 7472 6965 7665 6420  ..    Retrieved 
-00019b10: 6672 6f6d 0a20 2020 2060 4b69 7477 6172  from.    `Kitwar
-00019b20: 6520 5654 4b20 4461 7461 203c 6874 7470  e VTK Data <http
-00019b30: 733a 2f2f 6461 7461 2e6b 6974 7761 7265  s://data.kitware
-00019b40: 2e63 6f6d 2f23 636f 6c6c 6563 7469 6f6e  .com/#collection
-00019b50: 2f35 3566 3137 6637 3538 6437 3737 6636  /55f17f758d777f6
-00019b60: 6464 6337 3839 3562 372f 666f 6c64 6572  ddc7895b7/folder
-00019b70: 2f35 6166 6439 3332 6538 6437 3737 6631  /5afd932e8d777f1
-00019b80: 3565 6265 3162 3138 333e 605f 2e0a 0a20  5ebe1b183>`_... 
-00019b90: 2020 2050 6172 616d 6574 6572 730a 2020     Parameters.  
-00019ba0: 2020 2d2d 2d2d 2d2d 2d2d 2d2d 0a20 2020    ----------.   
-00019bb0: 206c 6f61 6420 3a20 626f 6f6c 2c20 6465   load : bool, de
-00019bc0: 6661 756c 743a 2054 7275 650a 2020 2020  fault: True.    
-00019bd0: 2020 2020 4c6f 6164 2074 6865 2064 6174      Load the dat
-00019be0: 6173 6574 2061 6674 6572 2064 6f77 6e6c  aset after downl
-00019bf0: 6f61 6469 6e67 2069 7420 7768 656e 2060  oading it when `
-00019c00: 6054 7275 6560 602e 2020 5365 7420 7468  `True``.  Set th
-00019c10: 6973 0a20 2020 2020 2020 2074 6f20 6060  is.        to ``
-00019c20: 4661 6c73 6560 6020 616e 6420 6f6e 6c79  False`` and only
-00019c30: 2074 6865 2066 696c 656e 616d 6520 7769   the filename wi
-00019c40: 6c6c 2062 6520 7265 7475 726e 6564 2e0a  ll be returned..
-00019c50: 0a20 2020 2052 6574 7572 6e73 0a20 2020  .    Returns.   
-00019c60: 202d 2d2d 2d2d 2d2d 0a20 2020 2070 7976   -------.    pyv
-00019c70: 6973 7461 2e4d 756c 7469 426c 6f63 6b20  ista.MultiBlock 
-00019c80: 7c20 7374 720a 2020 2020 2020 2020 4461  | str.        Da
-00019c90: 7461 5365 7420 6f72 2066 696c 656e 616d  taSet or filenam
-00019ca0: 6520 6465 7065 6e64 696e 6720 6f6e 2060  e depending on `
-00019cb0: 606c 6f61 6460 602e 0a0a 2020 2020 4578  `load``...    Ex
-00019cc0: 616d 706c 6573 0a20 2020 202d 2d2d 2d2d  amples.    -----
-00019cd0: 2d2d 2d0a 2020 2020 3e3e 3e20 6672 6f6d  ---.    >>> from
-00019ce0: 2070 7976 6973 7461 2069 6d70 6f72 7420   pyvista import 
-00019cf0: 6578 616d 706c 6573 0a20 2020 203e 3e3e  examples.    >>>
-00019d00: 2064 6174 6173 6574 203d 2065 7861 6d70   dataset = examp
-00019d10: 6c65 732e 646f 776e 6c6f 6164 5f63 6176  les.download_cav
-00019d20: 6974 7928 2920 2023 2064 6f63 7465 7374  ity()  # doctest
-00019d30: 3a2b 534b 4950 0a0a 2020 2020 5365 6520  :+SKIP..    See 
-00019d40: 3a72 6566 3a60 6f70 656e 666f 616d 5f65  :ref:`openfoam_e
-00019d50: 7861 6d70 6c65 6020 666f 7220 6120 6675  xample` for a fu
-00019d60: 6c6c 2065 7861 6d70 6c65 2075 7369 6e67  ll example using
-00019d70: 2074 6869 7320 6461 7461 7365 742e 0a0a   this dataset...
-00019d80: 2020 2020 2222 220a 2020 2020 6669 6c65      """.    file
-00019d90: 6e61 6d65 203d 205f 646f 776e 6c6f 6164  name = _download
-00019da0: 5f61 7263 6869 7665 2827 4f70 656e 464f  _archive('OpenFO
-00019db0: 414d 2e7a 6970 272c 2074 6172 6765 745f  AM.zip', target_
-00019dc0: 6669 6c65 3d27 6361 7669 7479 2f63 6173  file='cavity/cas
-00019dd0: 652e 666f 616d 2729 0a20 2020 2069 6620  e.foam').    if 
-00019de0: 6e6f 7420 6c6f 6164 3a0a 2020 2020 2020  not load:.      
-00019df0: 2020 7265 7475 726e 2066 696c 656e 616d    return filenam
-00019e00: 650a 2020 2020 7265 7475 726e 2070 7976  e.    return pyv
-00019e10: 6973 7461 2e4f 7065 6e46 4f41 4d52 6561  ista.OpenFOAMRea
-00019e20: 6465 7228 6669 6c65 6e61 6d65 292e 7265  der(filename).re
-00019e30: 6164 2829 0a0a 0a64 6566 2064 6f77 6e6c  ad()...def downl
-00019e40: 6f61 645f 6f70 656e 666f 616d 5f74 7562  oad_openfoam_tub
-00019e50: 6573 286c 6f61 643d 5472 7565 293a 2020  es(load=True):  
-00019e60: 2320 7072 6167 6d61 3a20 6e6f 2063 6f76  # pragma: no cov
-00019e70: 6572 0a20 2020 2022 2222 446f 776e 6c6f  er.    """Downlo
-00019e80: 6164 2074 7562 6573 204f 7065 6e46 4f41  ad tubes OpenFOA
-00019e90: 4d20 6578 616d 706c 652e 0a0a 2020 2020  M example...    
-00019ea0: 4461 7461 2067 656e 6572 6174 6564 2066  Data generated f
-00019eb0: 726f 6d20 7075 626c 6963 2053 696d 5363  rom public SimSc
-00019ec0: 616c 6520 6578 616d 706c 6573 2061 7420  ale examples at 
-00019ed0: 6053 696d 5363 616c 6520 5072 6f6a 6563  `SimScale Projec
-00019ee0: 7420 4c69 6272 6172 7920 2d0a 2020 2020  t Library -.    
-00019ef0: 5475 7262 6f20 3c68 7474 7073 3a2f 2f77  Turbo <https://w
-00019f00: 7777 2e73 696d 7363 616c 652e 636f 6d2f  ww.simscale.com/
-00019f10: 7072 6f6a 6563 7473 2f61 7961 726e 6f7a  projects/ayarnoz
-00019f20: 2f74 7572 626f 2f3e 605f 2e0a 0a20 2020  /turbo/>`_...   
-00019f30: 204c 6963 656e 7369 6e67 2066 6f72 2074   Licensing for t
-00019f40: 6869 7320 6461 7461 7365 7420 6973 2067  his dataset is g
-00019f50: 7261 6e74 6564 2074 6f20 6672 6565 6c79  ranted to freely
-00019f60: 2061 6e64 2077 6974 686f 7574 2072 6573   and without res
-00019f70: 7472 6963 7469 6f6e 0a20 2020 2072 6570  triction.    rep
-00019f80: 726f 6475 6365 2c20 6469 7374 7269 6275  roduce, distribu
-00019f90: 7465 2c20 7075 626c 6973 6820 6163 636f  te, publish acco
-00019fa0: 7264 696e 6720 746f 2074 6865 2060 5369  rding to the `Si
-00019fb0: 6d53 6361 6c65 2054 6572 6d73 2061 6e64  mScale Terms and
-00019fc0: 0a20 2020 2043 6f6e 6469 7469 6f6e 7320  .    Conditions 
-00019fd0: 3c68 7474 7073 3a2f 2f77 7777 2e73 696d  <https://www.sim
-00019fe0: 7363 616c 652e 636f 6d2f 7465 726d 732d  scale.com/terms-
-00019ff0: 616e 642d 636f 6e64 6974 696f 6e73 2f3e  and-conditions/>
-0001a000: 605f 2e0a 0a20 2020 2050 6172 616d 6574  `_...    Paramet
-0001a010: 6572 730a 2020 2020 2d2d 2d2d 2d2d 2d2d  ers.    --------
-0001a020: 2d2d 0a20 2020 206c 6f61 6420 3a20 626f  --.    load : bo
-0001a030: 6f6c 2c20 6465 6661 756c 743a 2054 7275  ol, default: Tru
-0001a040: 650a 2020 2020 2020 2020 4c6f 6164 2074  e.        Load t
-0001a050: 6865 2064 6174 6173 6574 2061 6674 6572  he dataset after
-0001a060: 2064 6f77 6e6c 6f61 6469 6e67 2069 7420   downloading it 
-0001a070: 7768 656e 2060 6054 7275 6560 602e 2020  when ``True``.  
-0001a080: 5365 7420 7468 6973 0a20 2020 2020 2020  Set this.       
-0001a090: 2074 6f20 6060 4661 6c73 6560 6020 616e   to ``False`` an
-0001a0a0: 6420 6f6e 6c79 2074 6865 2066 696c 656e  d only the filen
-0001a0b0: 616d 6520 7769 6c6c 2062 6520 7265 7475  ame will be retu
-0001a0c0: 726e 6564 2e0a 0a20 2020 2052 6574 7572  rned...    Retur
-0001a0d0: 6e73 0a20 2020 202d 2d2d 2d2d 2d2d 0a20  ns.    -------. 
-0001a0e0: 2020 2070 7976 6973 7461 2e4d 756c 7469     pyvista.Multi
-0001a0f0: 426c 6f63 6b20 7c20 7374 720a 2020 2020  Block | str.    
-0001a100: 2020 2020 4461 7461 5365 7420 6f72 2066      DataSet or f
-0001a110: 696c 656e 616d 6520 6465 7065 6e64 696e  ilename dependin
-0001a120: 6720 6f6e 2060 606c 6f61 6460 602e 0a0a  g on ``load``...
-0001a130: 2020 2020 4578 616d 706c 6573 0a20 2020      Examples.   
-0001a140: 202d 2d2d 2d2d 2d2d 2d0a 2020 2020 506c   --------.    Pl
-0001a150: 6f74 2074 6865 206f 7574 6c69 6e65 206f  ot the outline o
-0001a160: 6620 7468 6520 6461 7461 7365 7420 616c  f the dataset al
-0001a170: 6f6e 6720 7769 7468 2061 2063 726f 7373  ong with a cross
-0001a180: 2073 6563 7469 6f6e 206f 6620 7468 6520   section of the 
-0001a190: 666c 6f77 2076 656c 6f63 6974 792e 0a0a  flow velocity...
-0001a1a0: 2020 2020 3e3e 3e20 696d 706f 7274 2070      >>> import p
-0001a1b0: 7976 6973 7461 2061 7320 7076 0a20 2020  yvista as pv.   
-0001a1c0: 203e 3e3e 2066 726f 6d20 7079 7669 7374   >>> from pyvist
-0001a1d0: 6120 696d 706f 7274 2065 7861 6d70 6c65  a import example
-0001a1e0: 730a 2020 2020 3e3e 3e20 6461 7461 7365  s.    >>> datase
-0001a1f0: 7420 3d20 6578 616d 706c 6573 2e64 6f77  t = examples.dow
-0001a200: 6e6c 6f61 645f 6f70 656e 666f 616d 5f74  nload_openfoam_t
-0001a210: 7562 6573 2829 0a20 2020 203e 3e3e 2061  ubes().    >>> a
-0001a220: 6972 203d 2064 6174 6173 6574 5b30 5d0a  ir = dataset[0].
-0001a230: 2020 2020 3e3e 3e20 795f 736c 6963 6520      >>> y_slice 
-0001a240: 3d20 6169 722e 736c 6963 6528 2779 2729  = air.slice('y')
-0001a250: 0a20 2020 203e 3e3e 2070 6c20 3d20 7076  .    >>> pl = pv
-0001a260: 2e50 6c6f 7474 6572 2829 0a20 2020 203e  .Plotter().    >
-0001a270: 3e3e 205f 203d 2070 6c2e 6164 645f 6d65  >> _ = pl.add_me
-0001a280: 7368 280a 2020 2020 2e2e 2e20 2020 2020  sh(.    ...     
-0001a290: 795f 736c 6963 652c 0a20 2020 202e 2e2e  y_slice,.    ...
-0001a2a0: 2020 2020 2073 6361 6c61 7273 3d27 5527       scalars='U'
-0001a2b0: 2c0a 2020 2020 2e2e 2e20 2020 2020 6c69  ,.    ...     li
-0001a2c0: 6768 7469 6e67 3d46 616c 7365 2c0a 2020  ghting=False,.  
-0001a2d0: 2020 2e2e 2e20 2020 2020 7363 616c 6172    ...     scalar
-0001a2e0: 5f62 6172 5f61 7267 733d 7b27 7469 746c  _bar_args={'titl
-0001a2f0: 6527 3a20 2746 6c6f 7720 5665 6c6f 6369  e': 'Flow Veloci
-0001a300: 7479 277d 2c0a 2020 2020 2e2e 2e20 290a  ty'},.    ... ).
-0001a310: 2020 2020 3e3e 3e20 5f20 3d20 706c 2e61      >>> _ = pl.a
-0001a320: 6464 5f6d 6573 6828 6169 722c 2063 6f6c  dd_mesh(air, col
-0001a330: 6f72 3d27 7727 2c20 6f70 6163 6974 793d  or='w', opacity=
-0001a340: 302e 3235 290a 2020 2020 3e3e 3e20 706c  0.25).    >>> pl
-0001a350: 2e65 6e61 626c 655f 616e 7469 5f61 6c69  .enable_anti_ali
-0001a360: 6173 696e 6728 290a 2020 2020 3e3e 3e20  asing().    >>> 
-0001a370: 706c 2e73 686f 7728 290a 0a20 2020 2053  pl.show()..    S
-0001a380: 6565 203a 7265 663a 606f 7065 6e66 6f61  ee :ref:`openfoa
-0001a390: 6d5f 7475 6265 735f 6578 616d 706c 6560  m_tubes_example`
-0001a3a0: 2066 6f72 2061 2066 756c 6c20 6578 616d   for a full exam
-0001a3b0: 706c 6520 7573 696e 6720 7468 6973 2064  ple using this d
-0001a3c0: 6174 6173 6574 2e0a 0a20 2020 2022 2222  ataset...    """
-0001a3d0: 0a20 2020 2066 696c 656e 616d 6520 3d20  .    filename = 
-0001a3e0: 5f64 6f77 6e6c 6f61 645f 6172 6368 6976  _download_archiv
-0001a3f0: 6528 0a20 2020 2020 2020 2027 6676 6d2f  e(.        'fvm/
-0001a400: 7475 7262 6f5f 696e 636f 6d70 7265 7373  turbo_incompress
-0001a410: 6962 6c65 2f54 7572 626f 2d49 6e63 6f6d  ible/Turbo-Incom
-0001a420: 7072 6573 7369 626c 655f 332d 5275 6e5f  pressible_3-Run_
-0001a430: 312d 534f 4c55 5449 4f4e 5f46 4945 4c44  1-SOLUTION_FIELD
-0001a440: 532e 7a69 7027 2c0a 2020 2020 2020 2020  S.zip',.        
-0001a450: 7461 7267 6574 5f66 696c 653d 2763 6173  target_file='cas
-0001a460: 652e 666f 616d 272c 0a20 2020 2029 0a20  e.foam',.    ). 
-0001a470: 2020 2069 6620 6e6f 7420 6c6f 6164 3a0a     if not load:.
-0001a480: 2020 2020 2020 2020 7265 7475 726e 2066          return f
-0001a490: 696c 656e 616d 650a 2020 2020 7265 6164  ilename.    read
-0001a4a0: 6572 203d 2070 7976 6973 7461 2e4f 7065  er = pyvista.Ope
-0001a4b0: 6e46 4f41 4d52 6561 6465 7228 6669 6c65  nFOAMReader(file
-0001a4c0: 6e61 6d65 290a 2020 2020 7265 6164 6572  name).    reader
-0001a4d0: 2e73 6574 5f61 6374 6976 655f 7469 6d65  .set_active_time
-0001a4e0: 5f76 616c 7565 2831 3030 3029 0a20 2020  _value(1000).   
-0001a4f0: 2072 6574 7572 6e20 7265 6164 6572 2e72   return reader.r
-0001a500: 6561 6428 290a 0a0a 6465 6620 646f 776e  ead()...def down
-0001a510: 6c6f 6164 5f6c 7563 7928 6c6f 6164 3d54  load_lucy(load=T
-0001a520: 7275 6529 3a20 2023 2070 7261 676d 613a  rue):  # pragma:
-0001a530: 206e 6f20 636f 7665 720a 2020 2020 2222   no cover.    ""
-0001a540: 2244 6f77 6e6c 6f61 6420 7468 6520 6c75  "Download the lu
-0001a550: 6379 2061 6e67 656c 206d 6573 682e 0a0a  cy angel mesh...
-0001a560: 2020 2020 4f72 6967 696e 616c 2064 6f77      Original dow
-0001a570: 6e6c 6f61 6465 6420 6672 6f6d 2074 6865  nloaded from the
-0001a580: 2060 5468 6520 5374 616e 666f 7264 2033   `The Stanford 3
-0001a590: 4420 5363 616e 6e69 6e67 2052 6570 6f73  D Scanning Repos
-0001a5a0: 6974 6f72 790a 2020 2020 3c68 7474 703a  itory.    <http:
-0001a5b0: 2f2f 6772 6170 6869 6373 2e73 7461 6e66  //graphics.stanf
-0001a5c0: 6f72 642e 6564 752f 6461 7461 2f33 4473  ord.edu/data/3Ds
-0001a5d0: 6361 6e72 6570 2f3e 605f 2061 6e64 2064  canrep/>`_ and d
-0001a5e0: 6563 696d 6174 6564 2074 6f0a 2020 2020  ecimated to.    
-0001a5f0: 6170 7072 6f78 696d 6174 656c 7920 3130  approximately 10
-0001a600: 306b 2074 7269 616e 676c 652e 0a0a 2020  0k triangle...  
-0001a610: 2020 5061 7261 6d65 7465 7273 0a20 2020    Parameters.   
-0001a620: 202d 2d2d 2d2d 2d2d 2d2d 2d0a 2020 2020   ----------.    
-0001a630: 6c6f 6164 203a 2062 6f6f 6c2c 2064 6566  load : bool, def
-0001a640: 6175 6c74 3a20 5472 7565 0a20 2020 2020  ault: True.     
-0001a650: 2020 204c 6f61 6420 7468 6520 6461 7461     Load the data
-0001a660: 7365 7420 6166 7465 7220 646f 776e 6c6f  set after downlo
-0001a670: 6164 696e 6720 6974 2077 6865 6e20 6060  ading it when ``
-0001a680: 5472 7565 6060 2e20 2053 6574 2074 6869  True``.  Set thi
-0001a690: 730a 2020 2020 2020 2020 746f 2060 6046  s.        to ``F
-0001a6a0: 616c 7365 6060 2061 6e64 206f 6e6c 7920  alse`` and only 
-0001a6b0: 7468 6520 6669 6c65 6e61 6d65 2077 696c  the filename wil
-0001a6c0: 6c20 6265 2072 6574 7572 6e65 642e 0a0a  l be returned...
-0001a6d0: 2020 2020 5265 7475 726e 730a 2020 2020      Returns.    
-0001a6e0: 2d2d 2d2d 2d2d 2d0a 2020 2020 7079 7669  -------.    pyvi
-0001a6f0: 7374 612e 506f 6c79 4461 7461 207c 2073  sta.PolyData | s
-0001a700: 7472 0a20 2020 2020 2020 2044 6174 6153  tr.        DataS
-0001a710: 6574 206f 7220 6669 6c65 6e61 6d65 2064  et or filename d
-0001a720: 6570 656e 6469 6e67 206f 6e20 6060 6c6f  epending on ``lo
-0001a730: 6164 6060 2e0a 0a20 2020 2045 7861 6d70  ad``...    Examp
-0001a740: 6c65 730a 2020 2020 2d2d 2d2d 2d2d 2d2d  les.    --------
-0001a750: 0a20 2020 2050 6c6f 7420 7468 6520 4c75  .    Plot the Lu
-0001a760: 6379 2041 6e67 656c 2064 6174 6173 6574  cy Angel dataset
-0001a770: 2077 6974 6820 6375 7374 6f6d 206c 6967   with custom lig
-0001a780: 6874 696e 672e 0a0a 2020 2020 3e3e 3e20  hting...    >>> 
-0001a790: 6672 6f6d 2070 7976 6973 7461 2069 6d70  from pyvista imp
-0001a7a0: 6f72 7420 6578 616d 706c 6573 0a20 2020  ort examples.   
-0001a7b0: 203e 3e3e 2069 6d70 6f72 7420 7079 7669   >>> import pyvi
-0001a7c0: 7374 6120 6173 2070 760a 2020 2020 3e3e  sta as pv.    >>
-0001a7d0: 3e20 6461 7461 7365 7420 3d20 6578 616d  > dataset = exam
-0001a7e0: 706c 6573 2e64 6f77 6e6c 6f61 645f 6c75  ples.download_lu
-0001a7f0: 6379 2829 0a0a 2020 2020 4372 6561 7465  cy()..    Create
-0001a800: 2061 206c 6967 6874 2061 7420 7468 6520   a light at the 
-0001a810: 2266 6c61 6d65 222e 0a0a 2020 2020 3e3e  "flame"...    >>
-0001a820: 3e20 666c 616d 655f 6c69 6768 7420 3d20  > flame_light = 
-0001a830: 7076 2e4c 6967 6874 280a 2020 2020 2e2e  pv.Light(.    ..
-0001a840: 2e20 2020 2020 636f 6c6f 723d 5b30 2e38  .     color=[0.8
-0001a850: 3836 2c20 302e 3334 352c 2030 2e31 3333  86, 0.345, 0.133
-0001a860: 5d2c 0a20 2020 202e 2e2e 2020 2020 2070  ],.    ...     p
-0001a870: 6f73 6974 696f 6e3d 5b35 3530 2c20 3134  osition=[550, 14
-0001a880: 302c 2039 3530 5d2c 0a20 2020 202e 2e2e  0, 950],.    ...
-0001a890: 2020 2020 2069 6e74 656e 7369 7479 3d31       intensity=1
-0001a8a0: 2e35 2c0a 2020 2020 2e2e 2e20 2020 2020  .5,.    ...     
-0001a8b0: 706f 7369 7469 6f6e 616c 3d54 7275 652c  positional=True,
-0001a8c0: 0a20 2020 202e 2e2e 2020 2020 2063 6f6e  .    ...     con
-0001a8d0: 655f 616e 676c 653d 3930 2c0a 2020 2020  e_angle=90,.    
-0001a8e0: 2e2e 2e20 2020 2020 6174 7465 6e75 6174  ...     attenuat
-0001a8f0: 696f 6e5f 7661 6c75 6573 3d28 302e 3030  ion_values=(0.00
-0001a900: 312c 2030 2e30 3035 2c20 3029 2c0a 2020  1, 0.005, 0),.  
-0001a910: 2020 2e2e 2e20 290a 0a20 2020 2043 7265    ... )..    Cre
-0001a920: 6174 6520 6120 7363 656e 6520 6c69 6768  ate a scene ligh
-0001a930: 742e 0a0a 2020 2020 3e3e 3e20 7363 656e  t...    >>> scen
-0001a940: 655f 6c69 6768 7420 3d20 7076 2e4c 6967  e_light = pv.Lig
-0001a950: 6874 2869 6e74 656e 7369 7479 3d30 2e32  ht(intensity=0.2
-0001a960: 290a 0a20 2020 203e 3e3e 2070 6c20 3d20  )..    >>> pl = 
-0001a970: 7076 2e50 6c6f 7474 6572 286c 6967 6874  pv.Plotter(light
-0001a980: 696e 673d 4e6f 6e65 290a 2020 2020 3e3e  ing=None).    >>
-0001a990: 3e20 5f20 3d20 706c 2e61 6464 5f6d 6573  > _ = pl.add_mes
-0001a9a0: 6828 6461 7461 7365 742c 2073 6d6f 6f74  h(dataset, smoot
-0001a9b0: 685f 7368 6164 696e 673d 5472 7565 290a  h_shading=True).
-0001a9c0: 2020 2020 3e3e 3e20 706c 2e61 6464 5f6c      >>> pl.add_l
-0001a9d0: 6967 6874 2866 6c61 6d65 5f6c 6967 6874  ight(flame_light
-0001a9e0: 290a 2020 2020 3e3e 3e20 706c 2e61 6464  ).    >>> pl.add
-0001a9f0: 5f6c 6967 6874 2873 6365 6e65 5f6c 6967  _light(scene_lig
-0001aa00: 6874 290a 2020 2020 3e3e 3e20 706c 2e62  ht).    >>> pl.b
-0001aa10: 6163 6b67 726f 756e 645f 636f 6c6f 7220  ackground_color 
-0001aa20: 3d20 276b 270a 2020 2020 3e3e 3e20 706c  = 'k'.    >>> pl
-0001aa30: 2e73 686f 7728 290a 0a20 2020 2053 6565  .show()..    See
-0001aa40: 203a 7265 663a 606a 7570 7974 6572 5f70   :ref:`jupyter_p
-0001aa50: 6c6f 7474 696e 6760 2066 6f72 2061 6e6f  lotting` for ano
-0001aa60: 7468 6572 2065 7861 6d70 6c65 2075 7369  ther example usi
-0001aa70: 6e67 2074 6869 7320 6461 7461 7365 742e  ng this dataset.
-0001aa80: 0a0a 2020 2020 2222 220a 2020 2020 7265  ..    """.    re
-0001aa90: 7475 726e 205f 646f 776e 6c6f 6164 5f61  turn _download_a
-0001aaa0: 6e64 5f72 6561 6428 276c 7563 792e 706c  nd_read('lucy.pl
-0001aab0: 7927 2c20 6c6f 6164 3d6c 6f61 6429 0a0a  y', load=load)..
-0001aac0: 0a64 6566 2064 6f77 6e6c 6f61 645f 7075  .def download_pu
-0001aad0: 6d70 5f62 7261 636b 6574 286c 6f61 643d  mp_bracket(load=
-0001aae0: 5472 7565 293a 2020 2320 7072 6167 6d61  True):  # pragma
-0001aaf0: 3a20 6e6f 2063 6f76 6572 0a20 2020 2022  : no cover.    "
-0001ab00: 2222 446f 776e 6c6f 6164 2074 6865 2070  ""Download the p
-0001ab10: 756d 7020 6272 6163 6b65 7420 6578 616d  ump bracket exam
-0001ab20: 706c 6520 6461 7461 7365 742e 0a0a 2020  ple dataset...  
-0001ab30: 2020 4461 7461 2067 656e 6572 6174 6564    Data generated
-0001ab40: 2066 726f 6d20 7075 626c 6963 2053 696d   from public Sim
-0001ab50: 5363 616c 6520 6578 616d 706c 6573 2061  Scale examples a
-0001ab60: 7420 6053 696d 5363 616c 6520 5072 6f6a  t `SimScale Proj
-0001ab70: 6563 7420 4c69 6272 6172 7920 2d0a 2020  ect Library -.  
-0001ab80: 2020 5475 7262 6f20 3c68 7474 7073 3a2f    Turbo <https:/
-0001ab90: 2f77 7777 2e73 696d 7363 616c 652e 636f  /www.simscale.co
-0001aba0: 6d2f 7072 6f6a 6563 7473 2f53 5452 2f62  m/projects/STR/b
-0001abb0: 7261 636b 6574 2f3e 605f 2e0a 0a20 2020  racket/>`_...   
-0001abc0: 204c 6963 656e 7369 6e67 2066 6f72 2074   Licensing for t
-0001abd0: 6869 7320 6461 7461 7365 7420 6973 2067  his dataset is g
-0001abe0: 7261 6e74 6564 2066 7265 656c 7920 616e  ranted freely an
-0001abf0: 6420 7769 7468 6f75 7420 7265 7374 7269  d without restri
-0001ac00: 6374 696f 6e20 746f 0a20 2020 2072 6570  ction to.    rep
-0001ac10: 726f 6475 6365 2c20 6469 7374 7269 6275  roduce, distribu
-0001ac20: 7465 2c20 616e 6420 7075 626c 6973 6820  te, and publish 
-0001ac30: 6163 636f 7264 696e 6720 746f 2074 6865  according to the
-0001ac40: 2060 5369 6d53 6361 6c65 2054 6572 6d73   `SimScale Terms
-0001ac50: 2061 6e64 0a20 2020 2043 6f6e 6469 7469   and.    Conditi
-0001ac60: 6f6e 7320 3c68 7474 7073 3a2f 2f77 7777  ons <https://www
-0001ac70: 2e73 696d 7363 616c 652e 636f 6d2f 7465  .simscale.com/te
-0001ac80: 726d 732d 616e 642d 636f 6e64 6974 696f  rms-and-conditio
-0001ac90: 6e73 2f3e 605f 2e0a 0a20 2020 2050 6172  ns/>`_...    Par
-0001aca0: 616d 6574 6572 730a 2020 2020 2d2d 2d2d  ameters.    ----
-0001acb0: 2d2d 2d2d 2d2d 0a20 2020 206c 6f61 6420  ------.    load 
-0001acc0: 3a20 626f 6f6c 2c20 6465 6661 756c 743a  : bool, default:
-0001acd0: 2054 7275 650a 2020 2020 2020 2020 4c6f   True.        Lo
-0001ace0: 6164 2074 6865 2064 6174 6173 6574 2061  ad the dataset a
-0001acf0: 6674 6572 2064 6f77 6e6c 6f61 6469 6e67  fter downloading
-0001ad00: 2069 7420 7768 656e 2060 6054 7275 6560   it when ``True`
-0001ad10: 602e 2020 5365 7420 7468 6973 0a20 2020  `.  Set this.   
-0001ad20: 2020 2020 2074 6f20 6060 4661 6c73 6560       to ``False`
-0001ad30: 6020 616e 6420 6f6e 6c79 2074 6865 2066  ` and only the f
-0001ad40: 696c 656e 616d 6520 7769 6c6c 2062 6520  ilename will be 
-0001ad50: 7265 7475 726e 6564 2e0a 0a20 2020 2052  returned...    R
-0001ad60: 6574 7572 6e73 0a20 2020 202d 2d2d 2d2d  eturns.    -----
-0001ad70: 2d2d 0a20 2020 2055 6e73 7472 7563 7475  --.    Unstructu
-0001ad80: 7265 6447 7269 6420 7c20 7374 720a 2020  redGrid | str.  
-0001ad90: 2020 2020 2020 4461 7461 5365 7420 6f72        DataSet or
-0001ada0: 2066 696c 656e 616d 6520 6465 7065 6e64   filename depend
-0001adb0: 696e 6720 6f6e 2060 606c 6f61 6460 602e  ing on ``load``.
-0001adc0: 0a0a 2020 2020 4578 616d 706c 6573 0a20  ..    Examples. 
-0001add0: 2020 202d 2d2d 2d2d 2d2d 2d0a 2020 2020     --------.    
-0001ade0: 4c6f 6164 2074 6865 2064 6174 6173 6574  Load the dataset
-0001adf0: 2e0a 0a20 2020 203e 3e3e 2069 6d70 6f72  ...    >>> impor
-0001ae00: 7420 7079 7669 7374 6120 6173 2070 760a  t pyvista as pv.
-0001ae10: 2020 2020 3e3e 3e20 6672 6f6d 2070 7976      >>> from pyv
-0001ae20: 6973 7461 2069 6d70 6f72 7420 6578 616d  ista import exam
-0001ae30: 706c 6573 0a20 2020 203e 3e3e 2064 6174  ples.    >>> dat
-0001ae40: 6173 6574 203d 2065 7861 6d70 6c65 732e  aset = examples.
-0001ae50: 646f 776e 6c6f 6164 5f70 756d 705f 6272  download_pump_br
-0001ae60: 6163 6b65 7428 290a 2020 2020 3e3e 3e20  acket().    >>> 
-0001ae70: 6461 7461 7365 740a 2020 2020 556e 7374  dataset.    Unst
-0001ae80: 7275 6374 7572 6564 4772 6964 2028 2e2e  ructuredGrid (..
-0001ae90: 2e29 0a20 2020 2020 204e 2043 656c 6c73  .).      N Cells
-0001aea0: 3a20 2020 2031 3234 3830 360a 2020 2020  :    124806.    
-0001aeb0: 2020 4e20 506f 696e 7473 3a20 2020 3235    N Points:   25
-0001aec0: 3034 3837 0a20 2020 2020 2058 2042 6f75  0487.      X Bou
-0001aed0: 6e64 733a 2020 202d 352e 3030 3065 2d30  nds:   -5.000e-0
-0001aee0: 312c 2035 2e30 3030 652d 3031 0a20 2020  1, 5.000e-01.   
-0001aef0: 2020 2059 2042 6f75 6e64 733a 2020 202d     Y Bounds:   -
-0001af00: 342e 3030 3065 2d30 312c 2030 2e30 3030  4.000e-01, 0.000
-0001af10: 652b 3030 0a20 2020 2020 205a 2042 6f75  e+00.      Z Bou
-0001af20: 6e64 733a 2020 202d 322e 3530 3065 2d30  nds:   -2.500e-0
-0001af30: 322c 2032 2e35 3030 652d 3032 0a20 2020  2, 2.500e-02.   
-0001af40: 2020 204e 2041 7272 6179 733a 2020 2031     N Arrays:   1
-0001af50: 300a 0a20 2020 2050 6c6f 7420 7468 6520  0..    Plot the 
-0001af60: 6469 7370 6c61 6365 6d65 6e74 206f 6620  displacement of 
-0001af70: 7468 6520 3474 6820 6d6f 6465 2073 6861  the 4th mode sha
-0001af80: 7065 2061 7320 7363 616c 6172 732e 0a0a  pe as scalars...
-0001af90: 2020 2020 3e3e 3e20 6370 6f73 203d 205b      >>> cpos = [
-0001afa0: 0a20 2020 202e 2e2e 2020 2020 2028 302e  .    ...     (0.
-0001afb0: 3734 342c 202d 302e 3530 322c 202d 302e  744, -0.502, -0.
-0001afc0: 3833 3029 2c0a 2020 2020 2e2e 2e20 2020  830),.    ...   
-0001afd0: 2020 2830 2e30 3532 302c 202d 302e 3136    (0.0520, -0.16
-0001afe0: 302c 2030 2e30 3734 3329 2c0a 2020 2020  0, 0.0743),.    
-0001aff0: 2e2e 2e20 2020 2020 282d 302e 3138 302c  ...     (-0.180,
-0001b000: 202d 302e 3935 382c 2030 2e32 3234 292c   -0.958, 0.224),
-0001b010: 0a20 2020 202e 2e2e 205d 0a20 2020 203e  .    ... ].    >
-0001b020: 3e3e 2064 6174 6173 6574 2e70 6c6f 7428  >> dataset.plot(
-0001b030: 0a20 2020 202e 2e2e 2020 2020 2073 6361  .    ...     sca
-0001b040: 6c61 7273 3d27 6469 7370 5f33 272c 0a20  lars='disp_3',. 
-0001b050: 2020 202e 2e2e 2020 2020 2063 706f 733d     ...     cpos=
-0001b060: 6370 6f73 2c0a 2020 2020 2e2e 2e20 2020  cpos,.    ...   
-0001b070: 2020 7368 6f77 5f73 6361 6c61 725f 6261    show_scalar_ba
-0001b080: 723d 4661 6c73 652c 0a20 2020 202e 2e2e  r=False,.    ...
-0001b090: 2020 2020 2061 6d62 6965 6e74 3d30 2e32       ambient=0.2
-0001b0a0: 2c0a 2020 2020 2e2e 2e20 2020 2020 616e  ,.    ...     an
-0001b0b0: 7469 5f61 6c69 6173 696e 673d 2766 7861  ti_aliasing='fxa
-0001b0c0: 6127 2c0a 2020 2020 2e2e 2e20 290a 0a20  a',.    ... ).. 
-0001b0d0: 2020 2053 6565 203a 7265 663a 6070 756d     See :ref:`pum
-0001b0e0: 705f 6272 6163 6b65 745f 6578 616d 706c  p_bracket_exampl
-0001b0f0: 6560 2066 6f72 2061 2066 756c 6c20 6578  e` for a full ex
-0001b100: 616d 706c 6520 7573 696e 6720 7468 6973  ample using this
-0001b110: 2064 6174 6173 6574 2e0a 0a20 2020 2022   dataset...    "
-0001b120: 2222 0a20 2020 2066 696c 656e 616d 6520  "".    filename 
-0001b130: 3d20 5f64 6f77 6e6c 6f61 645f 6172 6368  = _download_arch
-0001b140: 6976 6528 0a20 2020 2020 2020 2027 6665  ive(.        'fe
-0001b150: 612f 7075 6d70 5f62 7261 636b 6574 2f70  a/pump_bracket/p
-0001b160: 756d 705f 6272 6163 6b65 742e 7a69 7027  ump_bracket.zip'
-0001b170: 2c0a 2020 2020 2020 2020 2770 756d 705f  ,.        'pump_
-0001b180: 6272 6163 6b65 742e 7674 6b27 2c0a 2020  bracket.vtk',.  
-0001b190: 2020 290a 2020 2020 6966 206c 6f61 643a    ).    if load:
-0001b1a0: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
-0001b1b0: 7079 7669 7374 612e 7265 6164 2866 696c  pyvista.read(fil
-0001b1c0: 656e 616d 6529 0a20 2020 2072 6574 7572  ename).    retur
-0001b1d0: 6e20 6669 6c65 6e61 6d65 0a0a 0a64 6566  n filename...def
-0001b1e0: 2064 6f77 6e6c 6f61 645f 656c 6563 7472   download_electr
-0001b1f0: 6f6e 6963 735f 636f 6f6c 696e 6728 6c6f  onics_cooling(lo
-0001b200: 6164 3d54 7275 6529 3a20 2023 2070 7261  ad=True):  # pra
-0001b210: 676d 613a 206e 6f20 636f 7665 720a 2020  gma: no cover.  
-0001b220: 2020 2222 2244 6f77 6e6c 6f61 6420 7468    """Download th
-0001b230: 6520 656c 6563 7472 6f6e 6963 7320 636f  e electronics co
-0001b240: 6f6c 696e 6720 6578 616d 706c 6520 6461  oling example da
-0001b250: 7461 7365 7473 2e0a 0a20 2020 2044 6174  tasets...    Dat
-0001b260: 6120 6765 6e65 7261 7465 6420 6672 6f6d  a generated from
-0001b270: 2070 7562 6c69 6320 5369 6d53 6361 6c65   public SimScale
-0001b280: 2065 7861 6d70 6c65 7320 6174 2060 5369   examples at `Si
-0001b290: 6d53 6361 6c65 2050 726f 6a65 6374 204c  mScale Project L
-0001b2a0: 6962 7261 7279 202d 0a20 2020 2054 7572  ibrary -.    Tur
-0001b2b0: 626f 203c 6874 7470 733a 2f2f 7777 772e  bo <https://www.
-0001b2c0: 7369 6d73 6361 6c65 2e63 6f6d 2f70 726f  simscale.com/pro
-0001b2d0: 6a65 6374 732f 6179 6172 6e6f 7a2f 7475  jects/ayarnoz/tu
-0001b2e0: 7262 6f2f 3e60 5f2e 0a0a 2020 2020 4c69  rbo/>`_...    Li
-0001b2f0: 6365 6e73 696e 6720 666f 7220 7468 6973  censing for this
-0001b300: 2064 6174 6173 6574 2069 7320 6772 616e   dataset is gran
-0001b310: 7465 6420 746f 2066 7265 656c 7920 616e  ted to freely an
-0001b320: 6420 7769 7468 6f75 7420 7265 7374 7269  d without restri
-0001b330: 6374 696f 6e0a 2020 2020 7265 7072 6f64  ction.    reprod
-0001b340: 7563 652c 2064 6973 7472 6962 7574 652c  uce, distribute,
-0001b350: 2070 7562 6c69 7368 2061 6363 6f72 6469   publish accordi
-0001b360: 6e67 2074 6f20 7468 6520 6053 696d 5363  ng to the `SimSc
-0001b370: 616c 6520 5465 726d 7320 616e 640a 2020  ale Terms and.  
-0001b380: 2020 436f 6e64 6974 696f 6e73 203c 6874    Conditions <ht
-0001b390: 7470 733a 2f2f 7777 772e 7369 6d73 6361  tps://www.simsca
-0001b3a0: 6c65 2e63 6f6d 2f74 6572 6d73 2d61 6e64  le.com/terms-and
-0001b3b0: 2d63 6f6e 6469 7469 6f6e 732f 3e60 5f2e  -conditions/>`_.
-0001b3c0: 0a0a 2020 2020 5061 7261 6d65 7465 7273  ..    Parameters
-0001b3d0: 0a20 2020 202d 2d2d 2d2d 2d2d 2d2d 2d0a  .    ----------.
-0001b3e0: 2020 2020 6c6f 6164 203a 2062 6f6f 6c2c      load : bool,
-0001b3f0: 2064 6566 6175 6c74 3a20 5472 7565 0a20   default: True. 
-0001b400: 2020 2020 2020 204c 6f61 6420 7468 6520         Load the 
-0001b410: 6461 7461 7365 7420 6166 7465 7220 646f  dataset after do
-0001b420: 776e 6c6f 6164 696e 6720 6974 2077 6865  wnloading it whe
-0001b430: 6e20 6060 5472 7565 6060 2e20 2053 6574  n ``True``.  Set
-0001b440: 2074 6869 730a 2020 2020 2020 2020 746f   this.        to
-0001b450: 2060 6046 616c 7365 6060 2061 6e64 206f   ``False`` and o
-0001b460: 6e6c 7920 7468 6520 6669 6c65 6e61 6d65  nly the filename
-0001b470: 2077 696c 6c20 6265 2072 6574 7572 6e65   will be returne
-0001b480: 642e 0a0a 2020 2020 5265 7475 726e 730a  d...    Returns.
-0001b490: 2020 2020 2d2d 2d2d 2d2d 2d0a 2020 2020      -------.    
-0001b4a0: 7475 706c 655b 506f 6c79 4461 7461 2c20  tuple[PolyData, 
-0001b4b0: 556e 7374 7275 6374 7572 6564 4772 6964  UnstructuredGrid
-0001b4c0: 5d20 7c20 6c69 7374 5b73 7472 5d0a 2020  ] | list[str].  
-0001b4d0: 2020 2020 2020 4461 7461 5365 7473 206f        DataSets o
-0001b4e0: 7220 6669 6c65 6e61 6d65 7320 6465 7065  r filenames depe
-0001b4f0: 6e64 696e 6720 6f6e 2060 606c 6f61 6460  nding on ``load`
-0001b500: 602e 0a0a 2020 2020 4578 616d 706c 6573  `...    Examples
-0001b510: 0a20 2020 202d 2d2d 2d2d 2d2d 2d0a 2020  .    --------.  
-0001b520: 2020 4c6f 6164 2074 6865 2064 6174 6173    Load the datas
-0001b530: 6574 7320 616e 6420 706c 6f74 2074 6865  ets and plot the
-0001b540: 2061 6972 2076 656c 6f63 6974 7920 7468   air velocity th
-0001b550: 726f 7567 6820 7468 6520 656c 6563 7472  rough the electr
-0001b560: 6f6e 6963 732e 0a0a 2020 2020 3e3e 3e20  onics...    >>> 
-0001b570: 696d 706f 7274 2070 7976 6973 7461 2061  import pyvista a
-0001b580: 7320 7076 0a20 2020 203e 3e3e 2066 726f  s pv.    >>> fro
-0001b590: 6d20 7079 7669 7374 6120 696d 706f 7274  m pyvista import
-0001b5a0: 2065 7861 6d70 6c65 730a 2020 2020 3e3e   examples.    >>
-0001b5b0: 3e20 7374 7275 6374 7572 652c 2061 6972  > structure, air
-0001b5c0: 203d 2065 7861 6d70 6c65 732e 646f 776e   = examples.down
-0001b5d0: 6c6f 6164 5f65 6c65 6374 726f 6e69 6373  load_electronics
-0001b5e0: 5f63 6f6f 6c69 6e67 2829 0a20 2020 203e  _cooling().    >
-0001b5f0: 3e3e 2073 7472 7563 7475 7265 2c20 6169  >> structure, ai
-0001b600: 720a 2020 2020 2850 6f6c 7944 6174 6120  r.    (PolyData 
-0001b610: 282e 2e2e 290a 2020 2020 2020 4e20 4365  (...).      N Ce
-0001b620: 6c6c 733a 2020 2020 3334 3432 3730 0a20  lls:    344270. 
-0001b630: 2020 2020 204e 2050 6f69 6e74 733a 2020       N Points:  
-0001b640: 2031 3837 3939 320a 2020 2020 2020 4e20   187992.      N 
-0001b650: 5374 7269 7073 3a20 2020 300a 2020 2020  Strips:   0.    
-0001b660: 2020 5820 426f 756e 6473 3a20 2020 2d33    X Bounds:   -3
-0001b670: 2e30 3030 652d 3033 2c20 312e 3533 3065  .000e-03, 1.530e
-0001b680: 2d30 310a 2020 2020 2020 5920 426f 756e  -01.      Y Boun
-0001b690: 6473 3a20 2020 2d33 2e30 3030 652d 3033  ds:   -3.000e-03
-0001b6a0: 2c20 322e 3033 3065 2d30 310a 2020 2020  , 2.030e-01.    
-0001b6b0: 2020 5a20 426f 756e 6473 3a20 2020 2d39    Z Bounds:   -9
-0001b6c0: 2e30 3030 652d 3033 2c20 342e 3230 3065  .000e-03, 4.200e
-0001b6d0: 2d30 320a 2020 2020 2020 4e20 4172 7261  -02.      N Arra
-0001b6e0: 7973 3a20 2020 342c 2055 6e73 7472 7563  ys:   4, Unstruc
-0001b6f0: 7475 7265 6447 7269 6420 282e 2e2e 290a  turedGrid (...).
-0001b700: 2020 2020 2020 4e20 4365 6c6c 733a 2020        N Cells:  
-0001b710: 2020 3137 3439 3939 320a 2020 2020 2020    1749992.      
-0001b720: 4e20 506f 696e 7473 3a20 2020 3631 3031  N Points:   6101
-0001b730: 3736 0a20 2020 2020 2058 2042 6f75 6e64  76.      X Bound
-0001b740: 733a 2020 202d 312e 3338 3865 2d31 382c  s:   -1.388e-18,
-0001b750: 2031 2e35 3030 652d 3031 0a20 2020 2020   1.500e-01.     
-0001b760: 2059 2042 6f75 6e64 733a 2020 202d 332e   Y Bounds:   -3.
-0001b770: 3030 3065 2d30 332c 2032 2e30 3330 652d  000e-03, 2.030e-
-0001b780: 3031 0a20 2020 2020 205a 2042 6f75 6e64  01.      Z Bound
-0001b790: 733a 2020 202d 362e 3030 3065 2d30 332c  s:   -6.000e-03,
-0001b7a0: 2034 2e34 3030 652d 3032 0a20 2020 2020   4.400e-02.     
-0001b7b0: 204e 2041 7272 6179 733a 2020 2031 3029   N Arrays:   10)
-0001b7c0: 0a0a 2020 2020 3e3e 3e20 7a5f 736c 6963  ..    >>> z_slic
-0001b7d0: 6520 3d20 6169 722e 636c 6970 2827 7a27  e = air.clip('z'
-0001b7e0: 2c20 7661 6c75 653d 2d30 2e30 3035 290a  , value=-0.005).
-0001b7f0: 2020 2020 3e3e 3e20 706c 203d 2070 762e      >>> pl = pv.
-0001b800: 506c 6f74 7465 7228 290a 2020 2020 3e3e  Plotter().    >>
-0001b810: 3e20 706c 2e65 6e61 626c 655f 7373 616f  > pl.enable_ssao
-0001b820: 2872 6164 6975 733d 302e 3031 290a 2020  (radius=0.01).  
-0001b830: 2020 3e3e 3e20 5f20 3d20 706c 2e61 6464    >>> _ = pl.add
-0001b840: 5f6d 6573 6828 0a20 2020 202e 2e2e 2020  _mesh(.    ...  
-0001b850: 2020 207a 5f73 6c69 6365 2c0a 2020 2020     z_slice,.    
-0001b860: 2e2e 2e20 2020 2020 7363 616c 6172 733d  ...     scalars=
-0001b870: 2755 272c 0a20 2020 202e 2e2e 2020 2020  'U',.    ...    
-0001b880: 206c 6967 6874 696e 673d 4661 6c73 652c   lighting=False,
-0001b890: 0a20 2020 202e 2e2e 2020 2020 2073 6361  .    ...     sca
-0001b8a0: 6c61 725f 6261 725f 6172 6773 3d7b 2774  lar_bar_args={'t
-0001b8b0: 6974 6c65 273a 2027 5665 6c6f 6369 7479  itle': 'Velocity
-0001b8c0: 277d 2c0a 2020 2020 2e2e 2e20 290a 2020  '},.    ... ).  
-0001b8d0: 2020 3e3e 3e20 5f20 3d20 706c 2e61 6464    >>> _ = pl.add
-0001b8e0: 5f6d 6573 6828 0a20 2020 202e 2e2e 2020  _mesh(.    ...  
-0001b8f0: 2020 2073 7472 7563 7475 7265 2c0a 2020     structure,.  
-0001b900: 2020 2e2e 2e20 2020 2020 636f 6c6f 723d    ...     color=
-0001b910: 2777 272c 0a20 2020 202e 2e2e 2020 2020  'w',.    ...    
-0001b920: 2073 6d6f 6f74 685f 7368 6164 696e 673d   smooth_shading=
-0001b930: 5472 7565 2c0a 2020 2020 2e2e 2e20 2020  True,.    ...   
-0001b940: 2020 7370 6c69 745f 7368 6172 705f 6564    split_sharp_ed
-0001b950: 6765 733d 5472 7565 2c0a 2020 2020 2e2e  ges=True,.    ..
-0001b960: 2e20 290a 2020 2020 3e3e 3e20 706c 2e63  . ).    >>> pl.c
-0001b970: 616d 6572 615f 706f 7369 7469 6f6e 203d  amera_position =
-0001b980: 2027 7879 270a 2020 2020 3e3e 3e20 706c   'xy'.    >>> pl
-0001b990: 2e63 616d 6572 612e 726f 6c6c 203d 2039  .camera.roll = 9
-0001b9a0: 300a 2020 2020 3e3e 3e20 706c 2e65 6e61  0.    >>> pl.ena
-0001b9b0: 626c 655f 616e 7469 5f61 6c69 6173 696e  ble_anti_aliasin
-0001b9c0: 6728 2766 7861 6127 290a 2020 2020 3e3e  g('fxaa').    >>
-0001b9d0: 3e20 706c 2e73 686f 7728 290a 0a20 2020  > pl.show()..   
-0001b9e0: 2053 686f 7720 7468 6520 7479 7065 2061   Show the type a
-0001b9f0: 6e64 2062 6f75 6e64 7320 6f66 2074 6865  nd bounds of the
-0001ba00: 2064 6174 6173 6574 732e 0a0a 2020 2020   datasets...    
-0001ba10: 5365 6520 3a72 6566 3a60 6f70 656e 666f  See :ref:`openfo
-0001ba20: 616d 5f63 6f6f 6c69 6e67 5f65 7861 6d70  am_cooling_examp
-0001ba30: 6c65 6020 666f 7220 6120 6675 6c6c 2065  le` for a full e
-0001ba40: 7861 6d70 6c65 2075 7369 6e67 2074 6869  xample using thi
-0001ba50: 7320 6461 7461 7365 742e 0a0a 2020 2020  s dataset...    
-0001ba60: 2222 220a 2020 2020 666e 616d 6573 203d  """.    fnames =
-0001ba70: 205f 646f 776e 6c6f 6164 5f61 7263 6869   _download_archi
-0001ba80: 7665 2827 6676 6d2f 636f 6f6c 696e 675f  ve('fvm/cooling_
-0001ba90: 656c 6563 7472 6f6e 6963 732f 6461 7461  electronics/data
-0001baa0: 7365 7473 2e7a 6970 2729 0a20 2020 2069  sets.zip').    i
-0001bab0: 6620 6c6f 6164 3a0a 2020 2020 2020 2020  f load:.        
-0001bac0: 2320 7265 7475 726e 2074 6865 2073 7472  # return the str
-0001bad0: 7563 7475 7265 2064 6174 6173 6574 2066  ucture dataset f
-0001bae0: 6972 7374 0a20 2020 2020 2020 2069 6620  irst.        if 
-0001baf0: 666e 616d 6573 5b31 5d2e 656e 6473 7769  fnames[1].endswi
-0001bb00: 7468 2827 7374 7275 6374 7572 652e 7674  th('structure.vt
-0001bb10: 7027 293a 0a20 2020 2020 2020 2020 2020  p'):.           
-0001bb20: 2066 6e61 6d65 7320 3d20 666e 616d 6573   fnames = fnames
-0001bb30: 5b3a 3a2d 315d 0a20 2020 2020 2020 2072  [::-1].        r
-0001bb40: 6574 7572 6e20 7079 7669 7374 612e 7265  eturn pyvista.re
-0001bb50: 6164 2866 6e61 6d65 735b 305d 292c 2070  ad(fnames[0]), p
-0001bb60: 7976 6973 7461 2e72 6561 6428 666e 616d  yvista.read(fnam
-0001bb70: 6573 5b31 5d29 0a20 2020 2072 6574 7572  es[1]).    retur
-0001bb80: 6e20 666e 616d 6573 0a0a 0a64 6566 2064  n fnames...def d
-0001bb90: 6f77 6e6c 6f61 645f 6361 6e28 7061 7274  ownload_can(part
-0001bba0: 6961 6c3d 4661 6c73 652c 206c 6f61 643d  ial=False, load=
-0001bbb0: 5472 7565 293a 2020 2320 7072 6167 6d61  True):  # pragma
-0001bbc0: 3a20 6e6f 2063 6f76 6572 0a20 2020 2022  : no cover.    "
-0001bbd0: 2222 446f 776e 6c6f 6164 2074 6865 2063  ""Download the c
-0001bbe0: 616e 2064 6174 6173 6574 206d 6573 682e  an dataset mesh.
-0001bbf0: 0a0a 2020 2020 4669 6c65 206f 6274 6169  ..    File obtai
-0001bc00: 6e65 6420 6672 6f6d 2060 4b69 7477 6172  ned from `Kitwar
-0001bc10: 6520 3c68 7474 7073 3a2f 2f77 7777 2e6b  e <https://www.k
-0001bc20: 6974 7761 7265 2e63 6f6d 2f3e 605f 2e20  itware.com/>`_. 
-0001bc30: 5573 6564 0a20 2020 2066 6f72 2074 6573  Used.    for tes
-0001bc40: 7469 6e67 2068 6466 2066 696c 6573 2e0a  ting hdf files..
-0001bc50: 0a20 2020 2050 6172 616d 6574 6572 730a  .    Parameters.
-0001bc60: 2020 2020 2d2d 2d2d 2d2d 2d2d 2d2d 0a20      ----------. 
-0001bc70: 2020 2070 6172 7469 616c 203a 2062 6f6f     partial : boo
-0001bc80: 6c2c 2064 6566 6175 6c74 3a20 4661 6c73  l, default: Fals
-0001bc90: 650a 2020 2020 2020 2020 4c6f 6164 2070  e.        Load p
-0001bca0: 6172 7420 6f66 2074 6865 2064 6174 6173  art of the datas
-0001bcb0: 6574 2e0a 0a20 2020 206c 6f61 6420 3a20  et...    load : 
-0001bcc0: 626f 6f6c 2c20 6465 6661 756c 743a 2054  bool, default: T
-0001bcd0: 7275 650a 2020 2020 2020 2020 4c6f 6164  rue.        Load
-0001bce0: 2074 6865 2064 6174 6173 6574 2061 6674   the dataset aft
-0001bcf0: 6572 2064 6f77 6e6c 6f61 6469 6e67 2069  er downloading i
-0001bd00: 7420 7768 656e 2060 6054 7275 6560 602e  t when ``True``.
-0001bd10: 2020 5365 7420 7468 6973 0a20 2020 2020    Set this.     
-0001bd20: 2020 2074 6f20 6060 4661 6c73 6560 6020     to ``False`` 
-0001bd30: 616e 6420 6f6e 6c79 2074 6865 2066 696c  and only the fil
-0001bd40: 656e 616d 6520 7769 6c6c 2062 6520 7265  ename will be re
-0001bd50: 7475 726e 6564 2e0a 0a20 2020 2052 6574  turned...    Ret
-0001bd60: 7572 6e73 0a20 2020 202d 2d2d 2d2d 2d2d  urns.    -------
-0001bd70: 0a20 2020 2070 7976 6973 7461 2e50 6f6c  .    pyvista.Pol
-0001bd80: 7944 6174 612c 2073 7472 2c20 6f72 204c  yData, str, or L
-0001bd90: 6973 745b 7374 725d 0a20 2020 2020 2020  ist[str].       
-0001bda0: 2054 6865 2065 7861 6d70 6c65 2050 6172   The example Par
-0001bdb0: 6156 6965 7720 6361 6e20 4461 7461 5365  aView can DataSe
-0001bdc0: 7420 6f72 2066 696c 6520 7061 7468 2873  t or file path(s
-0001bdd0: 292e 0a0a 2020 2020 4578 616d 706c 6573  )...    Examples
-0001bde0: 0a20 2020 202d 2d2d 2d2d 2d2d 2d0a 2020  .    --------.  
-0001bdf0: 2020 506c 6f74 2074 6865 2063 616e 2064    Plot the can d
-0001be00: 6174 6173 6574 2e0a 0a20 2020 203e 3e3e  ataset...    >>>
-0001be10: 2066 726f 6d20 7079 7669 7374 6120 696d   from pyvista im
-0001be20: 706f 7274 2065 7861 6d70 6c65 730a 2020  port examples.  
-0001be30: 2020 3e3e 3e20 696d 706f 7274 2070 7976    >>> import pyv
-0001be40: 6973 7461 2061 7320 7076 0a20 2020 203e  ista as pv.    >
-0001be50: 3e3e 2064 6174 6173 6574 203d 2065 7861  >> dataset = exa
-0001be60: 6d70 6c65 732e 646f 776e 6c6f 6164 5f63  mples.download_c
-0001be70: 616e 2829 2020 2320 646f 6374 6573 743a  an()  # doctest:
-0001be80: 2b53 4b49 500a 2020 2020 3e3e 3e20 6461  +SKIP.    >>> da
-0001be90: 7461 7365 742e 706c 6f74 2873 6361 6c61  taset.plot(scala
-0001bea0: 7273 3d27 5645 4c27 2c20 736d 6f6f 7468  rs='VEL', smooth
-0001beb0: 5f73 6861 6469 6e67 3d54 7275 6529 2020  _shading=True)  
-0001bec0: 2320 646f 6374 6573 743a 2b53 4b49 500a  # doctest:+SKIP.
-0001bed0: 0a20 2020 2022 2222 0a20 2020 2069 6620  .    """.    if 
-0001bee0: 7079 7669 7374 612e 7674 6b5f 7665 7273  pyvista.vtk_vers
-0001bef0: 696f 6e5f 696e 666f 203e 2028 392c 2031  ion_info > (9, 1
-0001bf00: 293a 2020 2320 7072 6167 6d61 3a20 6e6f  ):  # pragma: no
-0001bf10: 2063 6f76 6572 0a20 2020 2020 2020 2072   cover.        r
-0001bf20: 6169 7365 2056 544b 5665 7273 696f 6e45  aise VTKVersionE
-0001bf30: 7272 6f72 280a 2020 2020 2020 2020 2020  rror(.          
-0001bf40: 2020 2754 6869 7320 6578 616d 706c 6520    'This example 
-0001bf50: 6669 6c65 2069 7320 6465 7072 6563 6174  file is deprecat
-0001bf60: 6564 2066 6f72 2056 544b 2076 392e 322e  ed for VTK v9.2.
-0001bf70: 3020 616e 6420 6e65 7765 722e 2027 0a20  0 and newer. '. 
-0001bf80: 2020 2020 2020 2020 2020 2027 5573 6520             'Use 
-0001bf90: 6064 6f77 6e6c 6f61 645f 6361 6e5f 6372  `download_can_cr
-0001bfa0: 7573 6865 645f 6864 6660 2069 6e73 7465  ushed_hdf` inste
-0001bfb0: 6164 2e27 0a20 2020 2020 2020 2029 0a0a  ad.'.        )..
-0001bfc0: 2020 2020 6361 6e5f 3020 3d20 5f64 6f77      can_0 = _dow
-0001bfd0: 6e6c 6f61 645f 616e 645f 7265 6164 2827  nload_and_read('
-0001bfe0: 6864 662f 6361 6e5f 302e 6864 6627 2c20  hdf/can_0.hdf', 
-0001bff0: 6c6f 6164 3d6c 6f61 6429 0a20 2020 2069  load=load).    i
-0001c000: 6620 7061 7274 6961 6c3a 0a20 2020 2020  f partial:.     
-0001c010: 2020 2072 6574 7572 6e20 6361 6e5f 300a     return can_0.
-0001c020: 0a20 2020 2063 616e 7320 3d20 5b0a 2020  .    cans = [.  
-0001c030: 2020 2020 2020 6361 6e5f 302c 0a20 2020        can_0,.   
-0001c040: 2020 2020 205f 646f 776e 6c6f 6164 5f61       _download_a
-0001c050: 6e64 5f72 6561 6428 2768 6466 2f63 616e  nd_read('hdf/can
-0001c060: 5f31 2e68 6466 272c 206c 6f61 643d 6c6f  _1.hdf', load=lo
-0001c070: 6164 292c 0a20 2020 2020 2020 205f 646f  ad),.        _do
-0001c080: 776e 6c6f 6164 5f61 6e64 5f72 6561 6428  wnload_and_read(
-0001c090: 2768 6466 2f63 616e 5f32 2e68 6466 272c  'hdf/can_2.hdf',
-0001c0a0: 206c 6f61 643d 6c6f 6164 292c 0a20 2020   load=load),.   
-0001c0b0: 205d 0a0a 2020 2020 6966 206c 6f61 643a   ]..    if load:
-0001c0c0: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
-0001c0d0: 7079 7669 7374 612e 6d65 7267 6528 6361  pyvista.merge(ca
-0001c0e0: 6e73 290a 2020 2020 7265 7475 726e 2063  ns).    return c
-0001c0f0: 616e 730a 0a0a 6465 6620 646f 776e 6c6f  ans...def downlo
-0001c100: 6164 5f63 616e 5f63 7275 7368 6564 5f68  ad_can_crushed_h
-0001c110: 6466 286c 6f61 643d 5472 7565 293a 2020  df(load=True):  
-0001c120: 2320 7072 6167 6d61 3a20 6e6f 2063 6f76  # pragma: no cov
-0001c130: 6572 0a20 2020 2022 2222 446f 776e 6c6f  er.    """Downlo
-0001c140: 6164 2074 6865 2063 7275 7368 6564 2063  ad the crushed c
-0001c150: 616e 2064 6174 6173 6574 2e0a 0a20 2020  an dataset...   
-0001c160: 2046 696c 6520 6f62 7461 696e 6564 2066   File obtained f
-0001c170: 726f 6d20 604b 6974 7761 7265 203c 6874  rom `Kitware <ht
-0001c180: 7470 733a 2f2f 7777 772e 6b69 7477 6172  tps://www.kitwar
-0001c190: 652e 636f 6d2f 3e60 5f2e 2055 7365 640a  e.com/>`_. Used.
-0001c1a0: 2020 2020 666f 7220 7465 7374 696e 6720      for testing 
-0001c1b0: 6864 6620 6669 6c65 732e 0a0a 2020 2020  hdf files...    
-0001c1c0: 4f72 6967 696e 616c 6c79 2062 7569 6c74  Originally built
-0001c1d0: 2075 7369 6e67 2056 544b 2076 392e 322e   using VTK v9.2.
-0001c1e0: 3072 6320 6672 6f6d 3a0a 0a20 2020 2060  0rc from:..    `
-0001c1f0: 6056 544b 2f62 7569 6c64 2f45 7874 6572  `VTK/build/Exter
-0001c200: 6e61 6c54 6573 7469 6e67 2f63 616e 2d76  nalTesting/can-v
-0001c210: 7475 2e68 6466 6060 0a0a 2020 2020 5061  tu.hdf``..    Pa
-0001c220: 7261 6d65 7465 7273 0a20 2020 202d 2d2d  rameters.    ---
-0001c230: 2d2d 2d2d 2d2d 2d0a 2020 2020 6c6f 6164  -------.    load
-0001c240: 203a 2062 6f6f 6c2c 2064 6566 6175 6c74   : bool, default
-0001c250: 3a20 5472 7565 0a20 2020 2020 2020 204c  : True.        L
-0001c260: 6f61 6420 7468 6520 6461 7461 7365 7420  oad the dataset 
-0001c270: 6166 7465 7220 646f 776e 6c6f 6164 696e  after downloadin
-0001c280: 6720 6974 2077 6865 6e20 6060 5472 7565  g it when ``True
-0001c290: 6060 2e20 2053 6574 2074 6869 730a 2020  ``.  Set this.  
-0001c2a0: 2020 2020 2020 746f 2060 6046 616c 7365        to ``False
-0001c2b0: 6060 2061 6e64 206f 6e6c 7920 7468 6520  `` and only the 
-0001c2c0: 6669 6c65 6e61 6d65 2077 696c 6c20 6265  filename will be
-0001c2d0: 2072 6574 7572 6e65 642e 0a0a 2020 2020   returned...    
-0001c2e0: 5265 7475 726e 730a 2020 2020 2d2d 2d2d  Returns.    ----
-0001c2f0: 2d2d 2d0a 2020 2020 7079 7669 7374 612e  ---.    pyvista.
-0001c300: 556e 7374 7275 6374 7572 6564 4772 6964  UnstructuredGrid
-0001c310: 207c 2073 7472 0a20 2020 2020 2020 2043   | str.        C
-0001c320: 7275 7368 6564 2063 616e 2064 6174 6173  rushed can datas
-0001c330: 6574 206f 7220 7061 7468 2064 6570 656e  et or path depen
-0001c340: 6469 6e67 206f 6e20 7468 6520 7661 6c75  ding on the valu
-0001c350: 6520 6f66 2060 606c 6f61 6460 602e 0a0a  e of ``load``...
-0001c360: 2020 2020 4578 616d 706c 6573 0a20 2020      Examples.   
-0001c370: 202d 2d2d 2d2d 2d2d 2d0a 2020 2020 506c   --------.    Pl
-0001c380: 6f74 2074 6865 2063 7275 7368 6564 2063  ot the crushed c
-0001c390: 616e 2064 6174 6173 6574 2e0a 0a20 2020  an dataset...   
-0001c3a0: 203e 3e3e 2066 726f 6d20 7079 7669 7374   >>> from pyvist
-0001c3b0: 6120 696d 706f 7274 2065 7861 6d70 6c65  a import example
-0001c3c0: 730a 2020 2020 3e3e 3e20 696d 706f 7274  s.    >>> import
-0001c3d0: 2070 7976 6973 7461 2061 7320 7076 0a20   pyvista as pv. 
-0001c3e0: 2020 203e 3e3e 2064 6174 6173 6574 203d     >>> dataset =
-0001c3f0: 2065 7861 6d70 6c65 732e 646f 776e 6c6f   examples.downlo
-0001c400: 6164 5f63 616e 5f63 7275 7368 6564 5f68  ad_can_crushed_h
-0001c410: 6466 2829 0a20 2020 203e 3e3e 2064 6174  df().    >>> dat
-0001c420: 6173 6574 2e70 6c6f 7428 736d 6f6f 7468  aset.plot(smooth
-0001c430: 5f73 6861 6469 6e67 3d54 7275 6529 0a0a  _shading=True)..
-0001c440: 2020 2020 2222 220a 2020 2020 7265 7475      """.    retu
-0001c450: 726e 205f 646f 776e 6c6f 6164 5f61 6e64  rn _download_and
-0001c460: 5f72 6561 6428 2768 6466 2f63 616e 2d76  _read('hdf/can-v
-0001c470: 7475 2e68 6466 272c 206c 6f61 643d 6c6f  tu.hdf', load=lo
-0001c480: 6164 290a 0a0a 6465 6620 646f 776e 6c6f  ad)...def downlo
-0001c490: 6164 5f63 676e 735f 7374 7275 6374 7572  ad_cgns_structur
-0001c4a0: 6564 286c 6f61 643d 5472 7565 293a 2020  ed(load=True):  
-0001c4b0: 2320 7072 6167 6d61 3a20 6e6f 2063 6f76  # pragma: no cov
-0001c4c0: 6572 0a20 2020 2022 2222 446f 776e 6c6f  er.    """Downlo
-0001c4d0: 6164 2074 6865 2073 7472 7563 7475 7265  ad the structure
-0001c4e0: 6420 4347 4e53 2064 6174 6173 6574 206d  d CGNS dataset m
-0001c4f0: 6573 682e 0a0a 2020 2020 4f72 6967 696e  esh...    Origin
-0001c500: 616c 6c79 2064 6f77 6e6c 6f61 6465 6420  ally downloaded 
-0001c510: 6672 6f6d 2060 4346 4420 4765 6e65 7261  from `CFD Genera
-0001c520: 6c20 4e6f 7461 7469 6f6e 2053 7973 7465  l Notation Syste
-0001c530: 6d20 4578 616d 706c 6520 4669 6c65 730a  m Example Files.
-0001c540: 2020 2020 3c68 7474 7073 3a2f 2f63 676e      <https://cgn
-0001c550: 732e 6769 7468 7562 2e69 6f2f 4347 4e53  s.github.io/CGNS
-0001c560: 4669 6c65 732e 6874 6d6c 3e60 5f0a 0a20  Files.html>`_.. 
-0001c570: 2020 2050 6172 616d 6574 6572 730a 2020     Parameters.  
-0001c580: 2020 2d2d 2d2d 2d2d 2d2d 2d2d 0a20 2020    ----------.   
-0001c590: 206c 6f61 6420 3a20 626f 6f6c 2c20 6465   load : bool, de
-0001c5a0: 6661 756c 743a 2054 7275 650a 2020 2020  fault: True.    
-0001c5b0: 2020 2020 4c6f 6164 2074 6865 2064 6174      Load the dat
-0001c5c0: 6173 6574 2061 6674 6572 2064 6f77 6e6c  aset after downl
-0001c5d0: 6f61 6469 6e67 2069 7420 7768 656e 2060  oading it when `
-0001c5e0: 6054 7275 6560 602e 2020 5365 7420 7468  `True``.  Set th
-0001c5f0: 6973 0a20 2020 2020 2020 2074 6f20 6060  is.        to ``
-0001c600: 4661 6c73 6560 6020 616e 6420 6f6e 6c79  False`` and only
-0001c610: 2074 6865 2066 696c 656e 616d 6520 7769   the filename wi
-0001c620: 6c6c 2062 6520 7265 7475 726e 6564 2e0a  ll be returned..
-0001c630: 0a20 2020 2052 6574 7572 6e73 0a20 2020  .    Returns.   
-0001c640: 202d 2d2d 2d2d 2d2d 0a20 2020 2070 7976   -------.    pyv
-0001c650: 6973 7461 2e4d 756c 7469 426c 6f63 6b20  ista.MultiBlock 
-0001c660: 7c20 7374 720a 2020 2020 2020 2020 5374  | str.        St
-0001c670: 7275 6374 7572 6564 2c20 3132 2062 6c6f  ructured, 12 blo
-0001c680: 636b 2c20 332d 4420 636f 6e73 7472 6963  ck, 3-D constric
-0001c690: 7469 6e67 2063 6861 6e6e 656c 2c20 7769  ting channel, wi
-0001c6a0: 7468 2065 7861 6d70 6c65 2075 7365 206f  th example use o
-0001c6b0: 660a 2020 2020 2020 2020 4661 6d69 6c79  f.        Family
-0001c6c0: 5f74 2066 6f72 2042 4373 2028 4144 4620  _t for BCs (ADF 
-0001c6d0: 7479 7065 292e 2049 6620 6060 6c6f 6164  type). If ``load
-0001c6e0: 6060 2069 7320 6060 4661 6c73 6560 602c  `` is ``False``,
-0001c6f0: 2074 6865 6e20 7468 6520 7061 7468 206f   then the path o
-0001c700: 6620 7468 650a 2020 2020 2020 2020 6578  f the.        ex
-0001c710: 616d 706c 6520 4347 4e53 2066 696c 6520  ample CGNS file 
-0001c720: 6973 2072 6574 7572 6e65 642e 0a0a 2020  is returned...  
-0001c730: 2020 4578 616d 706c 6573 0a20 2020 202d    Examples.    -
-0001c740: 2d2d 2d2d 2d2d 2d0a 2020 2020 506c 6f74  -------.    Plot
-0001c750: 2074 6865 2065 7861 6d70 6c65 2043 474e   the example CGN
-0001c760: 5320 6461 7461 7365 742e 0a0a 2020 2020  S dataset...    
-0001c770: 3e3e 3e20 6672 6f6d 2070 7976 6973 7461  >>> from pyvista
-0001c780: 2069 6d70 6f72 7420 6578 616d 706c 6573   import examples
-0001c790: 0a20 2020 203e 3e3e 2069 6d70 6f72 7420  .    >>> import 
-0001c7a0: 7079 7669 7374 6120 6173 2070 760a 2020  pyvista as pv.  
-0001c7b0: 2020 3e3e 3e20 6461 7461 7365 7420 3d20    >>> dataset = 
-0001c7c0: 6578 616d 706c 6573 2e64 6f77 6e6c 6f61  examples.downloa
-0001c7d0: 645f 6367 6e73 5f73 7472 7563 7475 7265  d_cgns_structure
-0001c7e0: 6428 290a 2020 2020 3e3e 3e20 6461 7461  d().    >>> data
-0001c7f0: 7365 745b 305d 2e70 6c6f 7428 7363 616c  set[0].plot(scal
-0001c800: 6172 733d 2744 656e 7369 7479 2729 0a0a  ars='Density')..
-0001c810: 2020 2020 2222 220a 2020 2020 6669 6c65      """.    file
-0001c820: 6e61 6d65 203d 2064 6f77 6e6c 6f61 645f  name = download_
-0001c830: 6669 6c65 2827 6367 6e73 2f73 716e 7a5f  file('cgns/sqnz_
-0001c840: 732e 6164 662e 6367 6e73 2729 0a20 2020  s.adf.cgns').   
-0001c850: 2069 6620 6e6f 7420 6c6f 6164 3a0a 2020   if not load:.  
-0001c860: 2020 2020 2020 7265 7475 726e 2066 696c        return fil
-0001c870: 656e 616d 650a 2020 2020 7265 7475 726e  ename.    return
-0001c880: 2070 7976 6973 7461 2e67 6574 5f72 6561   pyvista.get_rea
-0001c890: 6465 7228 6669 6c65 6e61 6d65 292e 7265  der(filename).re
-0001c8a0: 6164 2829 0a0a 0a64 6566 2064 6f77 6e6c  ad()...def downl
-0001c8b0: 6f61 645f 7465 6370 6c6f 745f 6173 6369  oad_tecplot_asci
-0001c8c0: 6928 6c6f 6164 3d54 7275 6529 3a20 2023  i(load=True):  #
-0001c8d0: 2070 7261 676d 613a 206e 6f20 636f 7665   pragma: no cove
-0001c8e0: 720a 2020 2020 2222 2244 6f77 6e6c 6f61  r.    """Downloa
-0001c8f0: 6420 7468 6520 7369 6e67 6c65 2062 6c6f  d the single blo
-0001c900: 636b 2041 5343 4949 2054 6563 706c 6f74  ck ASCII Tecplot
-0001c910: 2064 6174 6173 6574 2e0a 0a20 2020 204f   dataset...    O
-0001c920: 7269 6769 6e61 6c6c 7920 646f 776e 6c6f  riginally downlo
-0001c930: 6164 6564 2066 726f 6d20 5061 756c 2042  aded from Paul B
-0001c940: 6f75 726b 6527 730a 2020 2020 6053 616d  ourke's.    `Sam
-0001c950: 706c 6520 6669 6c65 203c 6874 7470 3a2f  ple file <http:/
-0001c960: 2f70 6175 6c62 6f75 726b 652e 6e65 742f  /paulbourke.net/
-0001c970: 6461 7461 666f 726d 6174 732f 7470 2f73  dataformats/tp/s
-0001c980: 616d 706c 652e 7470 3e60 5f0a 0a20 2020  ample.tp>`_..   
-0001c990: 2050 6172 616d 6574 6572 730a 2020 2020   Parameters.    
-0001c9a0: 2d2d 2d2d 2d2d 2d2d 2d2d 0a20 2020 206c  ----------.    l
-0001c9b0: 6f61 6420 3a20 626f 6f6c 2c20 6465 6661  oad : bool, defa
-0001c9c0: 756c 743a 2054 7275 650a 2020 2020 2020  ult: True.      
-0001c9d0: 2020 4c6f 6164 2074 6865 2064 6174 6173    Load the datas
-0001c9e0: 6574 2061 6674 6572 2064 6f77 6e6c 6f61  et after downloa
-0001c9f0: 6469 6e67 2069 7420 7768 656e 2060 6054  ding it when ``T
-0001ca00: 7275 6560 602e 2020 5365 7420 7468 6973  rue``.  Set this
-0001ca10: 0a20 2020 2020 2020 2074 6f20 6060 4661  .        to ``Fa
-0001ca20: 6c73 6560 6020 616e 6420 6f6e 6c79 2074  lse`` and only t
-0001ca30: 6865 2066 696c 656e 616d 6520 7769 6c6c  he filename will
-0001ca40: 2062 6520 7265 7475 726e 6564 2e0a 0a20   be returned... 
-0001ca50: 2020 2052 6574 7572 6e73 0a20 2020 202d     Returns.    -
-0001ca60: 2d2d 2d2d 2d2d 0a20 2020 2070 7976 6973  ------.    pyvis
-0001ca70: 7461 2e4d 756c 7469 426c 6f63 6b20 7c20  ta.MultiBlock | 
-0001ca80: 7374 720a 2020 2020 2020 2020 4d75 6c74  str.        Mult
-0001ca90: 6962 6c6f 636b 2066 6f72 6d61 7420 7769  iblock format wi
-0001caa0: 7468 206f 6e6c 7920 3120 6461 7461 2062  th only 1 data b
-0001cab0: 6c6f 636b 2c20 7369 6d70 6c65 2067 656f  lock, simple geo
-0001cac0: 6d65 7472 6963 2073 6861 7065 2e0a 2020  metric shape..  
-0001cad0: 2020 2020 2020 4966 2060 606c 6f61 6460        If ``load`
-0001cae0: 6020 6973 2060 6046 616c 7365 6060 2c20  ` is ``False``, 
-0001caf0: 7468 656e 2074 6865 2070 6174 6820 6f66  then the path of
-0001cb00: 2074 6865 2065 7861 6d70 6c65 2054 6563   the example Tec
-0001cb10: 706c 6f74 2066 696c 650a 2020 2020 2020  plot file.      
-0001cb20: 2020 6973 2072 6574 7572 6e65 642e 0a0a    is returned...
-0001cb30: 2020 2020 4578 616d 706c 6573 0a20 2020      Examples.   
-0001cb40: 202d 2d2d 2d2d 2d2d 2d0a 2020 2020 506c   --------.    Pl
-0001cb50: 6f74 2074 6865 2065 7861 6d70 6c65 2054  ot the example T
-0001cb60: 6563 706c 6f74 2064 6174 6173 6574 2e0a  ecplot dataset..
-0001cb70: 0a20 2020 203e 3e3e 2066 726f 6d20 7079  .    >>> from py
-0001cb80: 7669 7374 6120 696d 706f 7274 2065 7861  vista import exa
-0001cb90: 6d70 6c65 730a 2020 2020 3e3e 3e20 696d  mples.    >>> im
-0001cba0: 706f 7274 2070 7976 6973 7461 2061 7320  port pyvista as 
-0001cbb0: 7076 0a20 2020 203e 3e3e 2064 6174 6173  pv.    >>> datas
-0001cbc0: 6574 203d 2065 7861 6d70 6c65 732e 646f  et = examples.do
-0001cbd0: 776e 6c6f 6164 5f74 6563 706c 6f74 5f61  wnload_tecplot_a
-0001cbe0: 7363 6969 2829 0a20 2020 203e 3e3e 2064  scii().    >>> d
-0001cbf0: 6174 6173 6574 2e70 6c6f 7428 290a 0a20  ataset.plot().. 
-0001cc00: 2020 2022 2222 0a20 2020 2066 696c 656e     """.    filen
-0001cc10: 616d 6520 3d20 646f 776e 6c6f 6164 5f66  ame = download_f
-0001cc20: 696c 6528 2774 6563 706c 6f74 5f61 7363  ile('tecplot_asc
-0001cc30: 6969 2e64 6174 2729 0a20 2020 2069 6620  ii.dat').    if 
-0001cc40: 6e6f 7420 6c6f 6164 3a0a 2020 2020 2020  not load:.      
-0001cc50: 2020 7265 7475 726e 2066 696c 656e 616d    return filenam
-0001cc60: 650a 2020 2020 7265 7475 726e 2070 7976  e.    return pyv
-0001cc70: 6973 7461 2e67 6574 5f72 6561 6465 7228  ista.get_reader(
-0001cc80: 6669 6c65 6e61 6d65 292e 7265 6164 2829  filename).read()
-0001cc90: 0a0a 0a64 6566 2064 6f77 6e6c 6f61 645f  ...def download_
-0001cca0: 6367 6e73 5f6d 756c 7469 286c 6f61 643d  cgns_multi(load=
-0001ccb0: 5472 7565 293a 2020 2320 7072 6167 6d61  True):  # pragma
-0001ccc0: 3a20 6e6f 2063 6f76 6572 0a20 2020 2022  : no cover.    "
-0001ccd0: 2222 446f 776e 6c6f 6164 2061 206d 756c  ""Download a mul
-0001cce0: 7469 656c 656d 656e 7420 6169 7266 6f69  tielement airfoi
-0001ccf0: 6c20 7769 7468 2061 2063 656c 6c20 6365  l with a cell ce
-0001cd00: 6e74 6572 6564 2073 6f6c 7574 696f 6e2e  ntered solution.
-0001cd10: 0a0a 2020 2020 4f72 6967 696e 616c 6c79  ..    Originally
-0001cd20: 2064 6f77 6e6c 6f61 6465 6420 6672 6f6d   downloaded from
-0001cd30: 2060 4346 4420 4765 6e65 7261 6c20 4e6f   `CFD General No
-0001cd40: 7461 7469 6f6e 2053 7973 7465 6d20 4578  tation System Ex
-0001cd50: 616d 706c 6520 4669 6c65 730a 2020 2020  ample Files.    
-0001cd60: 3c68 7474 7073 3a2f 2f63 676e 732e 6769  <https://cgns.gi
-0001cd70: 7468 7562 2e69 6f2f 4347 4e53 4669 6c65  thub.io/CGNSFile
-0001cd80: 732e 6874 6d6c 3e60 5f0a 0a20 2020 2050  s.html>`_..    P
-0001cd90: 6172 616d 6574 6572 730a 2020 2020 2d2d  arameters.    --
-0001cda0: 2d2d 2d2d 2d2d 2d2d 0a20 2020 206c 6f61  --------.    loa
-0001cdb0: 6420 3a20 626f 6f6c 2c20 6465 6661 756c  d : bool, defaul
-0001cdc0: 743a 2054 7275 650a 2020 2020 2020 2020  t: True.        
-0001cdd0: 4c6f 6164 2074 6865 2064 6174 6173 6574  Load the dataset
-0001cde0: 2061 6674 6572 2064 6f77 6e6c 6f61 6469   after downloadi
-0001cdf0: 6e67 2069 7420 7768 656e 2060 6054 7275  ng it when ``Tru
-0001ce00: 6560 602e 2020 5365 7420 7468 6973 0a20  e``.  Set this. 
-0001ce10: 2020 2020 2020 2074 6f20 6060 4661 6c73         to ``Fals
-0001ce20: 6560 6020 616e 6420 6f6e 6c79 2074 6865  e`` and only the
-0001ce30: 2066 696c 656e 616d 6520 7769 6c6c 2062   filename will b
-0001ce40: 6520 7265 7475 726e 6564 2e0a 0a20 2020  e returned...   
-0001ce50: 2052 6574 7572 6e73 0a20 2020 202d 2d2d   Returns.    ---
-0001ce60: 2d2d 2d2d 0a20 2020 2070 7976 6973 7461  ----.    pyvista
-0001ce70: 2e4d 756c 7469 426c 6f63 6b20 7c20 7374  .MultiBlock | st
-0001ce80: 720a 2020 2020 2020 2020 5374 7275 6374  r.        Struct
-0001ce90: 7572 6564 2c20 3420 626c 6f63 6b73 2c20  ured, 4 blocks, 
-0001cea0: 3244 2028 3220 706c 616e 6573 2069 6e20  2D (2 planes in 
-0001ceb0: 7468 6972 6420 6469 6d65 6e73 696f 6e29  third dimension)
-0001cec0: 206d 756c 7469 656c 656d 656e 740a 2020   multielement.  
-0001ced0: 2020 2020 2020 6169 7266 6f69 6c2c 2077        airfoil, w
-0001cee0: 6974 6820 6365 6c6c 2063 656e 7465 7265  ith cell centere
-0001cef0: 6420 736f 6c75 7469 6f6e 2e20 4966 2060  d solution. If `
-0001cf00: 606c 6f61 6460 6020 6973 2060 6046 616c  `load`` is ``Fal
-0001cf10: 7365 6060 2c20 7468 656e 2074 6865 2070  se``, then the p
-0001cf20: 6174 6820 6f66 2074 6865 0a20 2020 2020  ath of the.     
-0001cf30: 2020 2065 7861 6d70 6c65 2043 474e 5320     example CGNS 
-0001cf40: 6669 6c65 2069 7320 7265 7475 726e 6564  file is returned
-0001cf50: 2e0a 0a20 2020 2045 7861 6d70 6c65 730a  ...    Examples.
-0001cf60: 2020 2020 2d2d 2d2d 2d2d 2d2d 0a20 2020      --------.   
-0001cf70: 2050 6c6f 7420 7468 6520 6169 7266 6f69   Plot the airfoi
-0001cf80: 6c20 6461 7461 7365 742e 204d 6572 6765  l dataset. Merge
-0001cf90: 2074 6865 206d 756c 7469 2d62 6c6f 636b   the multi-block
-0001cfa0: 2061 6e64 2074 6865 6e20 706c 6f74 2074   and then plot t
-0001cfb0: 6865 2061 6972 666f 696c 2773 0a20 2020  he airfoil's.   
-0001cfc0: 2060 6022 5669 7363 6f73 6974 7945 6464   ``"ViscosityEdd
-0001cfd0: 7922 6060 2e20 436f 6e76 6572 7420 7468  y"``. Convert th
-0001cfe0: 6520 6365 6c6c 2064 6174 6120 746f 2070  e cell data to p
-0001cff0: 6f69 6e74 2064 6174 6120 6173 2069 6e20  oint data as in 
-0001d000: 7468 6973 0a20 2020 2064 6174 6173 6574  this.    dataset
-0001d010: 2c20 7468 6520 736f 6c75 7469 6f6e 2069  , the solution i
-0001d020: 7320 7374 6f72 6564 2077 6974 6869 6e20  s stored within 
-0001d030: 7468 6520 6365 6c6c 732e 0a0a 2020 2020  the cells...    
-0001d040: 3e3e 3e20 6672 6f6d 2070 7976 6973 7461  >>> from pyvista
-0001d050: 2069 6d70 6f72 7420 6578 616d 706c 6573   import examples
-0001d060: 0a20 2020 203e 3e3e 2069 6d70 6f72 7420  .    >>> import 
-0001d070: 7079 7669 7374 6120 6173 2070 760a 2020  pyvista as pv.  
-0001d080: 2020 3e3e 3e20 6461 7461 7365 7420 3d20    >>> dataset = 
-0001d090: 6578 616d 706c 6573 2e64 6f77 6e6c 6f61  examples.downloa
-0001d0a0: 645f 6367 6e73 5f6d 756c 7469 2829 0a20  d_cgns_multi(). 
-0001d0b0: 2020 203e 3e3e 2075 6772 6964 203d 2064     >>> ugrid = d
-0001d0c0: 6174 6173 6574 2e63 6f6d 6269 6e65 2829  ataset.combine()
-0001d0d0: 0a20 2020 203e 3e3e 2075 6772 6964 203d  .    >>> ugrid =
-0001d0e0: 2075 6772 6964 203d 2075 6772 6964 2e63   ugrid = ugrid.c
-0001d0f0: 656c 6c5f 6461 7461 5f74 6f5f 706f 696e  ell_data_to_poin
-0001d100: 745f 6461 7461 2829 0a20 2020 203e 3e3e  t_data().    >>>
-0001d110: 2075 6772 6964 2e70 6c6f 7428 0a20 2020   ugrid.plot(.   
-0001d120: 202e 2e2e 2020 2020 2063 6d61 703d 2762   ...     cmap='b
-0001d130: 7772 272c 0a20 2020 202e 2e2e 2020 2020  wr',.    ...    
-0001d140: 2073 6361 6c61 7273 3d27 5669 7363 6f73   scalars='Viscos
-0001d150: 6974 7945 6464 7927 2c0a 2020 2020 2e2e  ityEddy',.    ..
-0001d160: 2e20 2020 2020 7a6f 6f6d 3d34 2c0a 2020  .     zoom=4,.  
-0001d170: 2020 2e2e 2e20 2020 2020 6370 6f73 3d27    ...     cpos='
-0001d180: 787a 272c 0a20 2020 202e 2e2e 2020 2020  xz',.    ...    
-0001d190: 2073 686f 775f 7363 616c 6172 5f62 6172   show_scalar_bar
-0001d1a0: 3d46 616c 7365 2c0a 2020 2020 2e2e 2e20  =False,.    ... 
-0001d1b0: 290a 0a20 2020 2022 2222 0a20 2020 2066  )..    """.    f
-0001d1c0: 696c 656e 616d 6520 3d20 646f 776e 6c6f  ilename = downlo
-0001d1d0: 6164 5f66 696c 6528 2763 676e 732f 6d75  ad_file('cgns/mu
-0001d1e0: 6c74 692e 6367 6e73 2729 0a20 2020 2069  lti.cgns').    i
-0001d1f0: 6620 6e6f 7420 6c6f 6164 3a0a 2020 2020  f not load:.    
-0001d200: 2020 2020 7265 7475 726e 2066 696c 656e      return filen
-0001d210: 616d 650a 2020 2020 7265 6164 6572 203d  ame.    reader =
-0001d220: 2070 7976 6973 7461 2e67 6574 5f72 6561   pyvista.get_rea
-0001d230: 6465 7228 6669 6c65 6e61 6d65 290a 0a20  der(filename).. 
-0001d240: 2020 2023 2064 6973 6162 6c65 2072 6561     # disable rea
-0001d250: 6469 6e67 2074 6865 2062 6f75 6e64 6172  ding the boundar
-0001d260: 7920 7061 7463 682e 2041 7320 6f66 2056  y patch. As of V
-0001d270: 544b 2039 2e31 2e30 2074 6869 7320 6765  TK 9.1.0 this ge
-0001d280: 6e65 7261 7465 730a 2020 2020 2320 6d65  nerates.    # me
-0001d290: 7373 6167 6573 206c 696b 6520 2253 6b69  ssages like "Ski
-0001d2a0: 7070 696e 6720 4243 5f74 206e 6f64 653a  pping BC_t node:
-0001d2b0: 2042 435f 7420 7479 7065 2027 4243 4661   BC_t type 'BCFa
-0001d2c0: 7266 6965 6c64 2720 6e6f 7420 7375 7070  rfield' not supp
-0001d2d0: 6f72 7465 640a 2020 2020 2320 7965 742e  orted.    # yet.
-0001d2e0: 220a 2020 2020 7265 6164 6572 2e6c 6f61  ".    reader.loa
-0001d2f0: 645f 626f 756e 6461 7279 5f70 6174 6368  d_boundary_patch
-0001d300: 203d 2046 616c 7365 0a20 2020 2072 6574   = False.    ret
-0001d310: 7572 6e20 7265 6164 6572 2e72 6561 6428  urn reader.read(
-0001d320: 290a 0a0a 6465 6620 646f 776e 6c6f 6164  )...def download
-0001d330: 5f64 6963 6f6d 5f73 7461 636b 286c 6f61  _dicom_stack(loa
-0001d340: 643a 2062 6f6f 6c20 3d20 5472 7565 2920  d: bool = True) 
-0001d350: 2d3e 2055 6e69 6f6e 5b70 7976 6973 7461  -> Union[pyvista
-0001d360: 2e49 6d61 6765 4461 7461 2c20 7374 725d  .ImageData, str]
-0001d370: 3a20 2023 2070 7261 676d 613a 206e 6f20  :  # pragma: no 
-0001d380: 636f 7665 720a 2020 2020 2222 2244 6f77  cover.    """Dow
-0001d390: 6e6c 6f61 6420 5443 4941 2044 4943 4f4d  nload TCIA DICOM
-0001d3a0: 2073 7461 636b 2076 6f6c 756d 652e 0a0a   stack volume...
-0001d3b0: 2020 2020 4f72 6967 696e 616c 2064 6f77      Original dow
-0001d3c0: 6e6c 6f61 6420 6672 6f6d 2074 6865 2060  nload from the `
-0001d3d0: 5468 6520 4361 6e63 6572 2049 6d61 6769  The Cancer Imagi
-0001d3e0: 6e67 2041 7263 6869 7665 2028 5443 4941  ng Archive (TCIA
-0001d3f0: 290a 2020 2020 3c68 7474 7073 3a2f 2f77  ).    <https://w
-0001d400: 7777 2e63 616e 6365 7269 6d61 6769 6e67  ww.cancerimaging
-0001d410: 6172 6368 6976 652e 6e65 742f 3e60 5f2e  archive.net/>`_.
-0001d420: 2054 6869 7320 6973 2070 6172 7420 6f66   This is part of
-0001d430: 2074 6865 0a20 2020 2043 6c69 6e69 6361   the.    Clinica
-0001d440: 6c20 5072 6f74 656f 6d69 6320 5475 6d6f  l Proteomic Tumo
-0001d450: 7220 416e 616c 7973 6973 2043 6f6e 736f  r Analysis Conso
-0001d460: 7274 6975 6d20 5361 7263 6f6d 6173 2028  rtium Sarcomas (
-0001d470: 4350 5441 432d 5341 5229 0a20 2020 2063  CPTAC-SAR).    c
-0001d480: 6f6c 6c65 6374 696f 6e2e 0a0a 2020 2020  ollection...    
-0001d490: 5061 7261 6d65 7465 7273 0a20 2020 202d  Parameters.    -
-0001d4a0: 2d2d 2d2d 2d2d 2d2d 2d0a 2020 2020 6c6f  ---------.    lo
-0001d4b0: 6164 203a 2062 6f6f 6c2c 2064 6566 6175  ad : bool, defau
-0001d4c0: 6c74 3a20 5472 7565 0a20 2020 2020 2020  lt: True.       
-0001d4d0: 204c 6f61 6420 7468 6520 6461 7461 7365   Load the datase
-0001d4e0: 7420 6166 7465 7220 646f 776e 6c6f 6164  t after download
-0001d4f0: 696e 6720 6974 2077 6865 6e20 6060 5472  ing it when ``Tr
-0001d500: 7565 6060 2e20 2053 6574 2074 6869 730a  ue``.  Set this.
-0001d510: 2020 2020 2020 2020 746f 2060 6046 616c          to ``Fal
-0001d520: 7365 6060 2061 6e64 206f 6e6c 7920 7468  se`` and only th
-0001d530: 6520 6669 6c65 6e61 6d65 2077 696c 6c20  e filename will 
-0001d540: 6265 2072 6574 7572 6e65 642e 0a0a 2020  be returned...  
-0001d550: 2020 5265 7475 726e 730a 2020 2020 2d2d    Returns.    --
-0001d560: 2d2d 2d2d 2d0a 2020 2020 7079 7669 7374  -----.    pyvist
-0001d570: 612e 496d 6167 6544 6174 6120 7c20 7374  a.ImageData | st
-0001d580: 720a 2020 2020 2020 2020 4461 7461 5365  r.        DataSe
-0001d590: 7420 6f72 2070 6174 6820 6465 7065 6e64  t or path depend
-0001d5a0: 696e 6720 6f6e 2060 606c 6f61 6460 602e  ing on ``load``.
-0001d5b0: 0a0a 2020 2020 5265 6665 7265 6e63 6573  ..    References
-0001d5c0: 0a20 2020 202d 2d2d 2d2d 2d2d 2d2d 2d0a  .    ----------.
-0001d5d0: 2020 2020 2a20 2a2a 4461 7461 2043 6974      * **Data Cit
-0001d5e0: 6174 696f 6e2a 2a0a 0a20 2020 2020 2020  ation**..       
-0001d5f0: 204e 6174 696f 6e61 6c20 4361 6e63 6572   National Cancer
-0001d600: 2049 6e73 7469 7475 7465 2043 6c69 6e69   Institute Clini
-0001d610: 6361 6c20 5072 6f74 656f 6d69 6320 5475  cal Proteomic Tu
-0001d620: 6d6f 7220 416e 616c 7973 6973 2043 6f6e  mor Analysis Con
-0001d630: 736f 7274 6975 6d0a 2020 2020 2020 2020  sortium.        
-0001d640: 2843 5054 4143 292e 2028 3230 3138 292e  (CPTAC). (2018).
-0001d650: 2020 5261 6469 6f6c 6f67 7920 4461 7461    Radiology Data
-0001d660: 2066 726f 6d20 7468 6520 436c 696e 6963   from the Clinic
-0001d670: 616c 2050 726f 7465 6f6d 6963 2054 756d  al Proteomic Tum
-0001d680: 6f72 0a20 2020 2020 2020 2041 6e61 6c79  or.        Analy
-0001d690: 7369 7320 436f 6e73 6f72 7469 756d 2053  sis Consortium S
-0001d6a0: 6172 636f 6d61 7320 5b43 5054 4143 2d53  arcomas [CPTAC-S
-0001d6b0: 4152 5d20 636f 6c6c 6563 7469 6f6e 205b  AR] collection [
-0001d6c0: 4461 7461 2073 6574 5d2e 2054 6865 0a20  Data set]. The. 
-0001d6d0: 2020 2020 2020 2043 616e 6365 7220 496d         Cancer Im
-0001d6e0: 6167 696e 6720 4172 6368 6976 652e 2020  aging Archive.  
-0001d6f0: 444f 493a 2031 302e 3739 3337 2f54 4349  DOI: 10.7937/TCI
-0001d700: 412e 3230 3139 2e39 6274 3233 7239 350a  A.2019.9bt23r95.
-0001d710: 0a20 2020 202a 202a 2a41 636b 6e6f 776c  .    * **Acknowl
-0001d720: 6564 6765 6d65 6e74 2a2a 0a0a 2020 2020  edgement**..    
-0001d730: 2020 2020 4461 7461 2075 7365 6420 696e      Data used in
-0001d740: 2074 6869 7320 7075 626c 6963 6174 696f   this publicatio
-0001d750: 6e20 7765 7265 2067 656e 6572 6174 6564  n were generated
-0001d760: 2062 7920 7468 6520 4e61 7469 6f6e 616c   by the National
-0001d770: 2043 616e 6365 7220 496e 7374 6974 7574   Cancer Institut
-0001d780: 6520 436c 696e 6963 616c 0a20 2020 2020  e Clinical.     
-0001d790: 2020 2050 726f 7465 6f6d 6963 2054 756d     Proteomic Tum
-0001d7a0: 6f72 2041 6e61 6c79 7369 7320 436f 6e73  or Analysis Cons
-0001d7b0: 6f72 7469 756d 2028 4350 5441 4329 2e0a  ortium (CPTAC)..
-0001d7c0: 0a20 2020 202a 202a 2a54 4349 4120 4369  .    * **TCIA Ci
-0001d7d0: 7461 7469 6f6e 2a2a 0a0a 2020 2020 2020  tation**..      
-0001d7e0: 2020 436c 6172 6b20 4b2c 2056 656e 6474    Clark K, Vendt
-0001d7f0: 2042 2c20 536d 6974 6820 4b2c 2046 7265   B, Smith K, Fre
-0001d800: 796d 616e 6e20 4a2c 204b 6972 6279 204a  ymann J, Kirby J
-0001d810: 2c20 4b6f 7070 656c 2050 2c20 4d6f 6f72  , Koppel P, Moor
-0001d820: 6520 532c 2050 6869 6c6c 6970 7320 532c  e S, Phillips S,
-0001d830: 0a20 2020 2020 2020 204d 6166 6669 7474  .        Maffitt
-0001d840: 2044 2c20 5072 696e 676c 6520 4d2c 2054   D, Pringle M, T
-0001d850: 6172 626f 7820 4c2c 2050 7269 6f72 2046  arbox L, Prior F
-0001d860: 2e20 5468 6520 4361 6e63 6572 2049 6d61  . The Cancer Ima
-0001d870: 6769 6e67 2041 7263 6869 7665 2028 5443  ging Archive (TC
-0001d880: 4941 293a 2020 2320 7072 6167 6d61 3a20  IA):  # pragma: 
-0001d890: 6e6f 2063 6f76 6572 0a20 2020 2020 2020  no cover.       
-0001d8a0: 204d 6169 6e74 6169 6e69 6e67 2061 6e64   Maintaining and
-0001d8b0: 204f 7065 7261 7469 6e67 2061 2050 7562   Operating a Pub
-0001d8c0: 6c69 6320 496e 666f 726d 6174 696f 6e20  lic Information 
-0001d8d0: 5265 706f 7369 746f 7279 2c20 4a6f 7572  Repository, Jour
-0001d8e0: 6e61 6c20 6f66 2044 6967 6974 616c 2049  nal of Digital I
-0001d8f0: 6d61 6769 6e67 2c0a 2020 2020 2020 2020  maging,.        
-0001d900: 566f 6c75 6d65 2032 362c 204e 756d 6265  Volume 26, Numbe
-0001d910: 7220 362c 2044 6563 656d 6265 722c 2032  r 6, December, 2
-0001d920: 3031 332c 2070 7020 3130 3435 2d31 3035  013, pp 1045-105
-0001d930: 372e 2064 6f69 3a20 3130 2e31 3030 372f  7. doi: 10.1007/
-0001d940: 7331 3032 3738 2d30 3133 2d39 3632 322d  s10278-013-9622-
-0001d950: 370a 0a20 2020 2045 7861 6d70 6c65 730a  7..    Examples.
-0001d960: 2020 2020 2d2d 2d2d 2d2d 2d2d 0a20 2020      --------.   
-0001d970: 203e 3e3e 2066 726f 6d20 7079 7669 7374   >>> from pyvist
-0001d980: 6120 696d 706f 7274 2065 7861 6d70 6c65  a import example
-0001d990: 730a 2020 2020 3e3e 3e20 6461 7461 7365  s.    >>> datase
-0001d9a0: 7420 3d20 6578 616d 706c 6573 2e64 6f77  t = examples.dow
-0001d9b0: 6e6c 6f61 645f 6469 636f 6d5f 7374 6163  nload_dicom_stac
-0001d9c0: 6b28 290a 2020 2020 3e3e 3e20 6461 7461  k().    >>> data
-0001d9d0: 7365 742e 706c 6f74 2876 6f6c 756d 653d  set.plot(volume=
-0001d9e0: 5472 7565 2c20 7a6f 6f6d 3d33 2c20 7368  True, zoom=3, sh
-0001d9f0: 6f77 5f73 6361 6c61 725f 6261 723d 4661  ow_scalar_bar=Fa
-0001da00: 6c73 6529 0a0a 2020 2020 2222 220a 2020  lse)..    """.  
-0001da10: 2020 666e 616d 6573 203d 205f 646f 776e    fnames = _down
-0001da20: 6c6f 6164 5f61 7263 6869 7665 2827 4449  load_archive('DI
-0001da30: 434f 4d5f 5374 6163 6b2f 6461 7461 2e7a  COM_Stack/data.z
-0001da40: 6970 2729 0a20 2020 2070 6174 6820 3d20  ip').    path = 
-0001da50: 6f73 2e70 6174 682e 6469 726e 616d 6528  os.path.dirname(
-0001da60: 666e 616d 6573 5b30 5d29 0a20 2020 2069  fnames[0]).    i
-0001da70: 6620 6c6f 6164 3a0a 2020 2020 2020 2020  f load:.        
-0001da80: 7265 6164 6572 203d 2044 4943 4f4d 5265  reader = DICOMRe
-0001da90: 6164 6572 2870 6174 6829 0a20 2020 2020  ader(path).     
-0001daa0: 2020 2072 6574 7572 6e20 7265 6164 6572     return reader
-0001dab0: 2e72 6561 6428 290a 2020 2020 7265 7475  .read().    retu
-0001dac0: 726e 2070 6174 680a 0a0a 6465 6620 646f  rn path...def do
-0001dad0: 776e 6c6f 6164 5f70 6172 6368 6564 5f63  wnload_parched_c
-0001dae0: 616e 616c 5f34 6b28 6c6f 6164 3d54 7275  anal_4k(load=Tru
-0001daf0: 6529 3a20 2023 2070 7261 676d 613a 206e  e):  # pragma: n
-0001db00: 6f20 636f 7665 720a 2020 2020 2222 2244  o cover.    """D
-0001db10: 6f77 6e6c 6f61 6420 7061 7263 6865 6420  ownload parched 
-0001db20: 6361 6e61 6c20 346b 2064 6174 6173 6574  canal 4k dataset
-0001db30: 2e0a 0a20 2020 2050 6172 616d 6574 6572  ...    Parameter
-0001db40: 730a 2020 2020 2d2d 2d2d 2d2d 2d2d 2d2d  s.    ----------
-0001db50: 0a20 2020 206c 6f61 6420 3a20 626f 6f6c  .    load : bool
-0001db60: 2c20 6465 6661 756c 743a 2054 7275 650a  , default: True.
-0001db70: 2020 2020 2020 2020 4c6f 6164 2074 6865          Load the
-0001db80: 2064 6174 6173 6574 2061 6674 6572 2064   dataset after d
-0001db90: 6f77 6e6c 6f61 6469 6e67 2069 7420 7768  ownloading it wh
-0001dba0: 656e 2060 6054 7275 6560 602e 2020 5365  en ``True``.  Se
-0001dbb0: 7420 7468 6973 0a20 2020 2020 2020 2074  t this.        t
-0001dbc0: 6f20 6060 4661 6c73 6560 6020 616e 6420  o ``False`` and 
-0001dbd0: 6f6e 6c79 2074 6865 2066 696c 656e 616d  only the filenam
-0001dbe0: 6520 7769 6c6c 2062 6520 7265 7475 726e  e will be return
-0001dbf0: 6564 2e0a 0a20 2020 2052 6574 7572 6e73  ed...    Returns
-0001dc00: 0a20 2020 202d 2d2d 2d2d 2d2d 0a20 2020  .    -------.   
-0001dc10: 2070 7976 6973 7461 2e54 6578 7475 7265   pyvista.Texture
-0001dc20: 207c 2073 7472 0a20 2020 2020 2020 2044   | str.        D
-0001dc30: 6174 6153 6574 206f 7220 6669 6c65 6e61  ataSet or filena
-0001dc40: 6d65 2064 6570 656e 6469 6e67 206f 6e20  me depending on 
-0001dc50: 6060 6c6f 6164 6060 2e0a 0a20 2020 2045  ``load``...    E
-0001dc60: 7861 6d70 6c65 730a 2020 2020 2d2d 2d2d  xamples.    ----
-0001dc70: 2d2d 2d2d 0a20 2020 203e 3e3e 2066 726f  ----.    >>> fro
-0001dc80: 6d20 7079 7669 7374 6120 696d 706f 7274  m pyvista import
-0001dc90: 2065 7861 6d70 6c65 730a 2020 2020 3e3e   examples.    >>
-0001dca0: 3e20 6461 7461 7365 7420 3d20 6578 616d  > dataset = exam
-0001dcb0: 706c 6573 2e64 6f77 6e6c 6f61 645f 7061  ples.download_pa
-0001dcc0: 7263 6865 645f 6361 6e61 6c5f 346b 2829  rched_canal_4k()
-0001dcd0: 0a20 2020 203e 3e3e 2064 6174 6173 6574  .    >>> dataset
-0001dce0: 2e70 6c6f 7428 6370 6f73 3d22 7879 2229  .plot(cpos="xy")
-0001dcf0: 0a0a 2020 2020 2222 220a 2020 2020 7265  ..    """.    re
-0001dd00: 7475 726e 205f 646f 776e 6c6f 6164 5f61  turn _download_a
-0001dd10: 6e64 5f72 6561 6428 2270 6172 6368 6564  nd_read("parched
-0001dd20: 5f63 616e 616c 5f34 6b2e 6864 7222 2c20  _canal_4k.hdr", 
-0001dd30: 7465 7874 7572 653d 5472 7565 2c20 6c6f  texture=True, lo
-0001dd40: 6164 3d6c 6f61 6429 0a0a 0a64 6566 2064  ad=load)...def d
-0001dd50: 6f77 6e6c 6f61 645f 6365 6c6c 735f 6e64  ownload_cells_nd
-0001dd60: 286c 6f61 643d 5472 7565 293a 2020 2320  (load=True):  # 
-0001dd70: 7072 6167 6d61 3a20 6e6f 2063 6f76 6572  pragma: no cover
-0001dd80: 0a20 2020 2022 2222 446f 776e 6c6f 6164  .    """Download
-0001dd90: 2065 7861 6d70 6c65 2041 5653 2055 4344   example AVS UCD
-0001dda0: 2064 6174 6173 6574 2e0a 0a20 2020 2050   dataset...    P
-0001ddb0: 6172 616d 6574 6572 730a 2020 2020 2d2d  arameters.    --
-0001ddc0: 2d2d 2d2d 2d2d 2d2d 0a20 2020 206c 6f61  --------.    loa
-0001ddd0: 6420 3a20 626f 6f6c 2c20 6465 6661 756c  d : bool, defaul
-0001dde0: 743a 2054 7275 650a 2020 2020 2020 2020  t: True.        
-0001ddf0: 4c6f 6164 2074 6865 2064 6174 6173 6574  Load the dataset
-0001de00: 2061 6674 6572 2064 6f77 6e6c 6f61 6469   after downloadi
-0001de10: 6e67 2069 7420 7768 656e 2060 6054 7275  ng it when ``Tru
-0001de20: 6560 602e 2020 5365 7420 7468 6973 0a20  e``.  Set this. 
-0001de30: 2020 2020 2020 2074 6f20 6060 4661 6c73         to ``Fals
-0001de40: 6560 6020 616e 6420 6f6e 6c79 2074 6865  e`` and only the
-0001de50: 2066 696c 656e 616d 6520 7769 6c6c 2062   filename will b
-0001de60: 6520 7265 7475 726e 6564 2e0a 0a20 2020  e returned...   
-0001de70: 2052 6574 7572 6e73 0a20 2020 202d 2d2d   Returns.    ---
-0001de80: 2d2d 2d2d 0a20 2020 2070 7976 6973 7461  ----.    pyvista
-0001de90: 2e55 6e73 7472 7563 7475 7265 6447 7269  .UnstructuredGri
-0001dea0: 6420 7c20 7374 720a 2020 2020 2020 2020  d | str.        
-0001deb0: 4461 7461 5365 7420 6f72 2066 696c 656e  DataSet or filen
-0001dec0: 616d 6520 6465 7065 6e64 696e 6720 6f6e  ame depending on
-0001ded0: 2060 606c 6f61 6460 602e 0a0a 2020 2020   ``load``...    
-0001dee0: 4578 616d 706c 6573 0a20 2020 202d 2d2d  Examples.    ---
-0001def0: 2d2d 2d2d 2d0a 2020 2020 3e3e 3e20 6672  -----.    >>> fr
-0001df00: 6f6d 2070 7976 6973 7461 2069 6d70 6f72  om pyvista impor
-0001df10: 7420 6578 616d 706c 6573 0a20 2020 203e  t examples.    >
-0001df20: 3e3e 2064 6174 6173 6574 203d 2065 7861  >> dataset = exa
-0001df30: 6d70 6c65 732e 646f 776e 6c6f 6164 5f63  mples.download_c
-0001df40: 656c 6c73 5f6e 6428 290a 2020 2020 3e3e  ells_nd().    >>
-0001df50: 3e20 6461 7461 7365 742e 706c 6f74 2863  > dataset.plot(c
-0001df60: 706f 733d 2278 7922 290a 0a20 2020 2022  pos="xy")..    "
-0001df70: 2222 0a20 2020 2072 6574 7572 6e20 5f64  "".    return _d
-0001df80: 6f77 6e6c 6f61 645f 616e 645f 7265 6164  ownload_and_read
-0001df90: 2822 6365 6c6c 736e 642e 6173 6369 692e  ("cellsnd.ascii.
-0001dfa0: 696e 7022 2c20 6c6f 6164 3d6c 6f61 6429  inp", load=load)
-0001dfb0: 0a0a 0a64 6566 2064 6f77 6e6c 6f61 645f  ...def download_
-0001dfc0: 6d6f 6f6e 6c61 6e64 696e 675f 696d 6167  moonlanding_imag
-0001dfd0: 6528 6c6f 6164 3d54 7275 6529 3a20 2023  e(load=True):  #
-0001dfe0: 2070 7261 676d 613a 206e 6f20 636f 7665   pragma: no cove
-0001dff0: 720a 2020 2020 2222 2244 6f77 6e6c 6f61  r.    """Downloa
-0001e000: 6420 7468 6520 4d6f 6f6e 206c 616e 6469  d the Moon landi
-0001e010: 6e67 2069 6d61 6765 2e0a 0a20 2020 2054  ng image...    T
-0001e020: 6869 7320 6973 2061 206e 6f69 7379 2069  his is a noisy i
-0001e030: 6d61 6765 206f 7269 6769 6e61 6c6c 7920  mage originally 
-0001e040: 6f62 7461 696e 6564 2066 726f 6d20 6053  obtained from `S
-0001e050: 6369 7079 204c 6563 7475 7265 204e 6f74  cipy Lecture Not
-0001e060: 6573 0a20 2020 203c 6874 7470 733a 2f2f  es.    <https://
-0001e070: 7363 6970 792d 6c65 6374 7572 6573 2e6f  scipy-lectures.o
-0001e080: 7267 2f69 6e64 6578 2e68 746d 6c3e 605f  rg/index.html>`_
-0001e090: 2061 6e64 2063 616e 2062 6520 7573 6564   and can be used
-0001e0a0: 2074 6f20 6465 6d6f 6e73 7472 6174 6520   to demonstrate 
-0001e0b0: 610a 2020 2020 6c6f 7720 7061 7373 2066  a.    low pass f
-0001e0c0: 696c 7465 722e 0a0a 2020 2020 5365 6520  ilter...    See 
-0001e0d0: 7468 6520 6073 6369 7079 2d6c 6563 7475  the `scipy-lectu
-0001e0e0: 7265 7320 6c69 6365 6e73 650a 2020 2020  res license.    
-0001e0f0: 3c68 7474 703a 2f2f 7363 6970 792d 6c65  <http://scipy-le
-0001e100: 6374 7572 6573 2e6f 7267 2f70 7265 6661  ctures.org/prefa
-0001e110: 6365 2e68 746d 6c23 6c69 6365 6e73 653e  ce.html#license>
-0001e120: 605f 2066 6f72 206d 6f72 6520 6465 7461  `_ for more deta
-0001e130: 696c 730a 2020 2020 7265 6761 7264 696e  ils.    regardin
-0001e140: 6720 7468 6973 2069 6d61 6765 2773 2075  g this image's u
-0001e150: 7365 2061 6e64 2064 6973 7472 6962 7574  se and distribut
-0001e160: 696f 6e2e 0a0a 2020 2020 5061 7261 6d65  ion...    Parame
-0001e170: 7465 7273 0a20 2020 202d 2d2d 2d2d 2d2d  ters.    -------
-0001e180: 2d2d 2d0a 2020 2020 6c6f 6164 203a 2062  ---.    load : b
-0001e190: 6f6f 6c2c 2064 6566 6175 6c74 3a20 5472  ool, default: Tr
-0001e1a0: 7565 0a20 2020 2020 2020 204c 6f61 6420  ue.        Load 
-0001e1b0: 7468 6520 6461 7461 7365 7420 6166 7465  the dataset afte
-0001e1c0: 7220 646f 776e 6c6f 6164 696e 6720 6974  r downloading it
-0001e1d0: 2077 6865 6e20 6060 5472 7565 6060 2e20   when ``True``. 
-0001e1e0: 2053 6574 2074 6869 730a 2020 2020 2020   Set this.      
-0001e1f0: 2020 746f 2060 6046 616c 7365 6060 2061    to ``False`` a
-0001e200: 6e64 206f 6e6c 7920 7468 6520 6669 6c65  nd only the file
-0001e210: 6e61 6d65 2077 696c 6c20 6265 2072 6574  name will be ret
-0001e220: 7572 6e65 642e 0a0a 2020 2020 5265 7475  urned...    Retu
-0001e230: 726e 730a 2020 2020 2d2d 2d2d 2d2d 2d0a  rns.    -------.
-0001e240: 2020 2020 7079 7669 7374 612e 496d 6167      pyvista.Imag
-0001e250: 6544 6174 6120 7c20 7374 720a 2020 2020  eData | str.    
-0001e260: 2020 2020 6060 4461 7461 5365 7460 6020      ``DataSet`` 
-0001e270: 6f72 2066 696c 656e 616d 6520 6465 7065  or filename depe
-0001e280: 6e64 696e 6720 6f6e 2060 606c 6f61 6460  nding on ``load`
-0001e290: 602e 0a0a 2020 2020 4578 616d 706c 6573  `...    Examples
-0001e2a0: 0a20 2020 202d 2d2d 2d2d 2d2d 2d0a 2020  .    --------.  
-0001e2b0: 2020 3e3e 3e20 6672 6f6d 2070 7976 6973    >>> from pyvis
-0001e2c0: 7461 2069 6d70 6f72 7420 6578 616d 706c  ta import exampl
-0001e2d0: 6573 0a20 2020 203e 3e3e 2064 6174 6173  es.    >>> datas
-0001e2e0: 6574 203d 2065 7861 6d70 6c65 732e 646f  et = examples.do
-0001e2f0: 776e 6c6f 6164 5f6d 6f6f 6e6c 616e 6469  wnload_moonlandi
-0001e300: 6e67 5f69 6d61 6765 2829 0a20 2020 203e  ng_image().    >
-0001e310: 3e3e 2064 6174 6173 6574 2e70 6c6f 7428  >> dataset.plot(
-0001e320: 0a20 2020 202e 2e2e 2020 2020 2063 706f  .    ...     cpo
-0001e330: 733d 2778 7927 2c0a 2020 2020 2e2e 2e20  s='xy',.    ... 
-0001e340: 2020 2020 636d 6170 3d27 6772 6179 272c      cmap='gray',
-0001e350: 0a20 2020 202e 2e2e 2020 2020 2062 6163  .    ...     bac
-0001e360: 6b67 726f 756e 643d 2777 272c 0a20 2020  kground='w',.   
-0001e370: 202e 2e2e 2020 2020 2073 686f 775f 7363   ...     show_sc
-0001e380: 616c 6172 5f62 6172 3d46 616c 7365 2c0a  alar_bar=False,.
-0001e390: 2020 2020 2e2e 2e20 290a 0a20 2020 2053      ... )..    S
-0001e3a0: 6565 203a 7265 663a 6069 6d61 6765 5f66  ee :ref:`image_f
-0001e3b0: 6674 5f65 7861 6d70 6c65 6020 666f 7220  ft_example` for 
-0001e3c0: 6120 6675 6c6c 2065 7861 6d70 6c65 2075  a full example u
-0001e3d0: 7369 6e67 2074 6869 7320 6461 7461 7365  sing this datase
-0001e3e0: 742e 0a0a 2020 2020 2222 220a 2020 2020  t...    """.    
-0001e3f0: 7265 7475 726e 205f 646f 776e 6c6f 6164  return _download
-0001e400: 5f61 6e64 5f72 6561 6428 276d 6f6f 6e6c  _and_read('moonl
-0001e410: 616e 6469 6e67 2e70 6e67 272c 206c 6f61  anding.png', loa
-0001e420: 643d 6c6f 6164 290a 0a0a 6465 6620 646f  d=load)...def do
-0001e430: 776e 6c6f 6164 5f61 6e67 756c 6172 5f73  wnload_angular_s
-0001e440: 6563 746f 7228 6c6f 6164 3d54 7275 6529  ector(load=True)
-0001e450: 3a20 2023 2070 7261 676d 613a 206e 6f20  :  # pragma: no 
-0001e460: 636f 7665 720a 2020 2020 2222 2244 6f77  cover.    """Dow
-0001e470: 6e6c 6f61 6420 7468 6520 616e 6775 6c61  nload the angula
-0001e480: 7220 7365 6374 6f72 2064 6174 6173 6574  r sector dataset
-0001e490: 2e0a 0a20 2020 2050 6172 616d 6574 6572  ...    Parameter
-0001e4a0: 730a 2020 2020 2d2d 2d2d 2d2d 2d2d 2d2d  s.    ----------
-0001e4b0: 0a20 2020 206c 6f61 6420 3a20 626f 6f6c  .    load : bool
-0001e4c0: 2c20 6465 6661 756c 743a 2054 7275 650a  , default: True.
-0001e4d0: 2020 2020 2020 2020 4c6f 6164 2074 6865          Load the
-0001e4e0: 2064 6174 6173 6574 2061 6674 6572 2064   dataset after d
-0001e4f0: 6f77 6e6c 6f61 6469 6e67 2069 7420 7768  ownloading it wh
-0001e500: 656e 2060 6054 7275 6560 602e 2020 5365  en ``True``.  Se
-0001e510: 7420 7468 6973 0a20 2020 2020 2020 2074  t this.        t
-0001e520: 6f20 6060 4661 6c73 6560 6020 616e 6420  o ``False`` and 
-0001e530: 6f6e 6c79 2074 6865 2066 696c 656e 616d  only the filenam
-0001e540: 6520 7769 6c6c 2062 6520 7265 7475 726e  e will be return
-0001e550: 6564 2e0a 0a20 2020 2052 6574 7572 6e73  ed...    Returns
-0001e560: 0a20 2020 202d 2d2d 2d2d 2d2d 0a20 2020  .    -------.   
-0001e570: 2070 7976 6973 7461 2e55 6e73 7472 7563   pyvista.Unstruc
-0001e580: 7475 7265 6447 7269 6420 7c20 7374 720a  turedGrid | str.
-0001e590: 2020 2020 2020 2020 4461 7461 5365 7420          DataSet 
-0001e5a0: 6f72 2066 696c 656e 616d 6520 6465 7065  or filename depe
-0001e5b0: 6e64 696e 6720 6f6e 2060 606c 6f61 6460  nding on ``load`
-0001e5c0: 602e 0a0a 2020 2020 4578 616d 706c 6573  `...    Examples
-0001e5d0: 0a20 2020 202d 2d2d 2d2d 2d2d 2d0a 2020  .    --------.  
-0001e5e0: 2020 3e3e 3e20 6672 6f6d 2070 7976 6973    >>> from pyvis
-0001e5f0: 7461 2069 6d70 6f72 7420 6578 616d 706c  ta import exampl
-0001e600: 6573 0a20 2020 203e 3e3e 2064 6174 6173  es.    >>> datas
-0001e610: 6574 203d 2065 7861 6d70 6c65 732e 646f  et = examples.do
-0001e620: 776e 6c6f 6164 5f61 6e67 756c 6172 5f73  wnload_angular_s
-0001e630: 6563 746f 7228 290a 2020 2020 3e3e 3e20  ector().    >>> 
-0001e640: 6461 7461 7365 742e 706c 6f74 2873 6361  dataset.plot(sca
-0001e650: 6c61 7273 3d27 506f 696e 7449 6427 290a  lars='PointId').
-0001e660: 0a20 2020 2022 2222 0a20 2020 2072 6574  .    """.    ret
-0001e670: 7572 6e20 5f64 6f77 6e6c 6f61 645f 616e  urn _download_an
-0001e680: 645f 7265 6164 2827 416e 6775 6c61 7253  d_read('AngularS
-0001e690: 6563 746f 722e 7674 6b27 2c20 6c6f 6164  ector.vtk', load
-0001e6a0: 3d6c 6f61 6429 0a0a 0a64 6566 2064 6f77  =load)...def dow
-0001e6b0: 6e6c 6f61 645f 6d6f 756e 745f 6461 6d61  nload_mount_dama
-0001e6c0: 7661 6e64 286c 6f61 643d 5472 7565 293a  vand(load=True):
-0001e6d0: 2020 2320 7072 6167 6d61 3a20 6e6f 2063    # pragma: no c
-0001e6e0: 6f76 6572 0a20 2020 2022 2222 446f 776e  over.    """Down
-0001e6f0: 6c6f 6164 2074 6865 204d 6f75 6e74 2044  load the Mount D
-0001e700: 616d 6176 616e 6420 6461 7461 7365 742e  amavand dataset.
-0001e710: 0a0a 2020 2020 5669 7375 616c 697a 6520  ..    Visualize 
-0001e720: 3344 206d 6f64 656c 7320 6f66 2044 616d  3D models of Dam
-0001e730: 6176 616e 6420 566f 6c63 616e 6f2c 2041  avand Volcano, A
-0001e740: 6c62 6f72 7a2c 2049 7261 6e2e 2054 6869  lborz, Iran. Thi
-0001e750: 7320 6973 2061 2032 4420 6d61 700a 2020  s is a 2D map.  
-0001e760: 2020 7769 7468 2074 6865 2061 6c74 6974    with the altit
-0001e770: 7564 6520 656d 6265 6464 6564 2061 7320  ude embedded as 
-0001e780: 6060 277a 2760 6020 6365 6c6c 2064 6174  ``'z'`` cell dat
-0001e790: 6120 7769 7468 696e 2074 6865 0a20 2020  a within the.   
-0001e7a0: 203a 636c 6173 733a 6070 7976 6973 7461   :class:`pyvista
-0001e7b0: 2e50 6f6c 7944 6174 6160 2e0a 0a20 2020  .PolyData`...   
-0001e7c0: 204f 7269 6769 6e61 6c6c 7920 706f 7374   Originally post
-0001e7d0: 6564 2061 7420 6062 616e 6573 756c 6c69  ed at `banesulli
-0001e7e0: 7661 6e2f 6461 6d61 7661 6e64 2d76 6f6c  van/damavand-vol
-0001e7f0: 6361 6e6f 0a20 2020 203c 6874 7470 733a  cano.    <https:
-0001e800: 2f2f 6769 7468 7562 2e63 6f6d 2f62 616e  //github.com/ban
-0001e810: 6573 756c 6c69 7661 6e2f 6461 6d61 7661  esullivan/damava
-0001e820: 6e64 2d76 6f6c 6361 6e6f 3e60 5f2e 0a0a  nd-volcano>`_...
-0001e830: 2020 2020 5061 7261 6d65 7465 7273 0a20      Parameters. 
-0001e840: 2020 202d 2d2d 2d2d 2d2d 2d2d 2d0a 2020     ----------.  
-0001e850: 2020 6c6f 6164 203a 2062 6f6f 6c2c 2064    load : bool, d
-0001e860: 6566 6175 6c74 3a20 5472 7565 0a20 2020  efault: True.   
-0001e870: 2020 2020 204c 6f61 6420 7468 6520 6461       Load the da
-0001e880: 7461 7365 7420 6166 7465 7220 646f 776e  taset after down
-0001e890: 6c6f 6164 696e 6720 6974 2077 6865 6e20  loading it when 
-0001e8a0: 6060 5472 7565 6060 2e20 2053 6574 2074  ``True``.  Set t
-0001e8b0: 6869 730a 2020 2020 2020 2020 746f 2060  his.        to `
-0001e8c0: 6046 616c 7365 6060 2061 6e64 206f 6e6c  `False`` and onl
-0001e8d0: 7920 7468 6520 6669 6c65 6e61 6d65 2077  y the filename w
-0001e8e0: 696c 6c20 6265 2072 6574 7572 6e65 642e  ill be returned.
-0001e8f0: 0a0a 2020 2020 5265 7475 726e 730a 2020  ..    Returns.  
-0001e900: 2020 2d2d 2d2d 2d2d 2d0a 2020 2020 7079    -------.    py
-0001e910: 7669 7374 612e 506f 6c79 4461 7461 207c  vista.PolyData |
-0001e920: 2073 7472 0a20 2020 2020 2020 2044 6174   str.        Dat
-0001e930: 6153 6574 206f 7220 6669 6c65 6e61 6d65  aSet or filename
-0001e940: 2064 6570 656e 6469 6e67 206f 6e20 6060   depending on ``
-0001e950: 6c6f 6164 6060 2e0a 0a20 2020 2045 7861  load``...    Exa
-0001e960: 6d70 6c65 730a 2020 2020 2d2d 2d2d 2d2d  mples.    ------
-0001e970: 2d2d 0a20 2020 2044 6f77 6e6c 6f61 6420  --.    Download 
-0001e980: 7468 6520 4461 6d61 7661 6e64 2064 6174  the Damavand dat
-0001e990: 6173 6574 2061 6e64 2070 6c6f 7420 6974  aset and plot it
-0001e9a0: 2061 6674 6572 2077 6172 7069 6e67 2069   after warping i
-0001e9b0: 7420 6279 2069 7473 2061 6c74 6974 7564  t by its altitud
-0001e9c0: 652e 0a0a 2020 2020 3e3e 3e20 6672 6f6d  e...    >>> from
-0001e9d0: 2070 7976 6973 7461 2069 6d70 6f72 7420   pyvista import 
-0001e9e0: 6578 616d 706c 6573 0a20 2020 203e 3e3e  examples.    >>>
-0001e9f0: 2064 6174 6173 6574 203d 2065 7861 6d70   dataset = examp
-0001ea00: 6c65 732e 646f 776e 6c6f 6164 5f6d 6f75  les.download_mou
-0001ea10: 6e74 5f64 616d 6176 616e 6428 290a 2020  nt_damavand().  
-0001ea20: 2020 3e3e 3e20 6461 7461 7365 7420 3d20    >>> dataset = 
-0001ea30: 6461 7461 7365 742e 6365 6c6c 5f64 6174  dataset.cell_dat
-0001ea40: 615f 746f 5f70 6f69 6e74 5f64 6174 6128  a_to_point_data(
-0001ea50: 290a 2020 2020 3e3e 3e20 6461 7461 7365  ).    >>> datase
-0001ea60: 7420 3d20 6461 7461 7365 742e 7761 7270  t = dataset.warp
-0001ea70: 5f62 795f 7363 616c 6172 2827 7a27 2c20  _by_scalar('z', 
-0001ea80: 6661 6374 6f72 3d32 290a 2020 2020 3e3e  factor=2).    >>
-0001ea90: 3e20 6461 7461 7365 742e 706c 6f74 2863  > dataset.plot(c
-0001eaa0: 6d61 703d 2767 6973 745f 6561 7274 6827  map='gist_earth'
-0001eab0: 2c20 7368 6f77 5f73 6361 6c61 725f 6261  , show_scalar_ba
-0001eac0: 723d 4661 6c73 6529 0a0a 2020 2020 2222  r=False)..    ""
-0001ead0: 220a 2020 2020 7265 7475 726e 205f 646f  ".    return _do
-0001eae0: 776e 6c6f 6164 5f61 6e64 5f72 6561 6428  wnload_and_read(
-0001eaf0: 2741 4f49 2e44 616d 6176 616e 642e 3332  'AOI.Damavand.32
-0001eb00: 3633 392e 7674 7027 2c20 6c6f 6164 3d6c  639.vtp', load=l
-0001eb10: 6f61 6429 0a0a 0a64 6566 2064 6f77 6e6c  oad)...def downl
-0001eb20: 6f61 645f 7061 7274 6963 6c65 735f 6c65  oad_particles_le
-0001eb30: 7468 6528 6c6f 6164 3d54 7275 6529 3a20  the(load=True): 
-0001eb40: 2023 2070 7261 676d 613a 206e 6f20 636f   # pragma: no co
-0001eb50: 7665 720a 2020 2020 2222 2244 6f77 6e6c  ver.    """Downl
-0001eb60: 6f61 6420 6120 7061 7274 6963 6c65 7320  oad a particles 
-0001eb70: 6461 7461 7365 7420 6765 6e65 7261 7465  dataset generate
-0001eb80: 6420 6279 2060 6c65 7468 6520 3c68 7474  d by `lethe <htt
-0001eb90: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
-0001eba0: 6c65 7468 652d 6366 642f 6c65 7468 653e  lethe-cfd/lethe>
-0001ebb0: 605f 202e 0a0a 2020 2020 5365 6520 6050  `_ ...    See `P
-0001ebc0: 7956 6973 7461 2064 6973 6375 7373 696f  yVista discussio
-0001ebd0: 6e73 2023 3139 3834 0a20 2020 203c 6874  ns #1984.    <ht
-0001ebe0: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
-0001ebf0: 2f70 7976 6973 7461 2f70 7976 6973 7461  /pyvista/pyvista
-0001ec00: 2f64 6973 6375 7373 696f 6e73 2f31 3938  /discussions/198
-0001ec10: 343e 605f 0a0a 2020 2020 5061 7261 6d65  4>`_..    Parame
-0001ec20: 7465 7273 0a20 2020 202d 2d2d 2d2d 2d2d  ters.    -------
-0001ec30: 2d2d 2d0a 2020 2020 6c6f 6164 203a 2062  ---.    load : b
-0001ec40: 6f6f 6c2c 2064 6566 6175 6c74 3a20 5472  ool, default: Tr
-0001ec50: 7565 0a20 2020 2020 2020 204c 6f61 6420  ue.        Load 
-0001ec60: 7468 6520 6461 7461 7365 7420 6166 7465  the dataset afte
-0001ec70: 7220 646f 776e 6c6f 6164 696e 6720 6974  r downloading it
-0001ec80: 2077 6865 6e20 6060 5472 7565 6060 2e20   when ``True``. 
-0001ec90: 2053 6574 2074 6869 730a 2020 2020 2020   Set this.      
-0001eca0: 2020 746f 2060 6046 616c 7365 6060 2061    to ``False`` a
-0001ecb0: 6e64 206f 6e6c 7920 7468 6520 6669 6c65  nd only the file
-0001ecc0: 6e61 6d65 2077 696c 6c20 6265 2072 6574  name will be ret
-0001ecd0: 7572 6e65 642e 0a0a 2020 2020 5265 7475  urned...    Retu
-0001ece0: 726e 730a 2020 2020 2d2d 2d2d 2d2d 2d0a  rns.    -------.
-0001ecf0: 2020 2020 7079 7669 7374 612e 556e 7374      pyvista.Unst
-0001ed00: 7275 6374 7572 6564 4772 6964 207c 2073  ructuredGrid | s
-0001ed10: 7472 0a20 2020 2020 2020 2044 6174 6153  tr.        DataS
-0001ed20: 6574 206f 7220 6669 6c65 6e61 6d65 2064  et or filename d
-0001ed30: 6570 656e 6469 6e67 206f 6e20 6060 6c6f  epending on ``lo
-0001ed40: 6164 6060 2e0a 0a20 2020 2045 7861 6d70  ad``...    Examp
-0001ed50: 6c65 730a 2020 2020 2d2d 2d2d 2d2d 2d2d  les.    --------
-0001ed60: 0a20 2020 2044 6f77 6e6c 6f61 6420 7468  .    Download th
-0001ed70: 6520 7061 7274 6963 6c65 7320 6461 7461  e particles data
-0001ed80: 7365 7420 616e 6420 706c 6f74 2069 7420  set and plot it 
-0001ed90: 6166 7465 7220 6765 6e65 7261 7469 6e67  after generating
-0001eda0: 2067 6c79 7068 732e 0a0a 2020 2020 3e3e   glyphs...    >>
-0001edb0: 3e20 6672 6f6d 2070 7976 6973 7461 2069  > from pyvista i
-0001edc0: 6d70 6f72 7420 6578 616d 706c 6573 0a20  mport examples. 
-0001edd0: 2020 203e 3e3e 2070 6172 7469 636c 6573     >>> particles
-0001ede0: 203d 2065 7861 6d70 6c65 732e 646f 776e   = examples.down
-0001edf0: 6c6f 6164 5f70 6172 7469 636c 6573 5f6c  load_particles_l
-0001ee00: 6574 6865 2829 0a20 2020 203e 3e3e 2070  ethe().    >>> p
-0001ee10: 6172 7469 636c 6573 2e70 6c6f 7428 0a20  articles.plot(. 
-0001ee20: 2020 202e 2e2e 2020 2020 2072 656e 6465     ...     rende
-0001ee30: 725f 706f 696e 7473 5f61 735f 7370 6865  r_points_as_sphe
-0001ee40: 7265 733d 5472 7565 2c0a 2020 2020 2e2e  res=True,.    ..
-0001ee50: 2e20 2020 2020 7374 796c 653d 2770 6f69  .     style='poi
-0001ee60: 6e74 7327 2c0a 2020 2020 2e2e 2e20 2020  nts',.    ...   
-0001ee70: 2020 7363 616c 6172 733d 2756 656c 6f63    scalars='Veloc
-0001ee80: 6974 7927 2c0a 2020 2020 2e2e 2e20 2020  ity',.    ...   
-0001ee90: 2020 6261 636b 6772 6f75 6e64 3d27 7727    background='w'
-0001eea0: 2c0a 2020 2020 2e2e 2e20 2020 2020 7363  ,.    ...     sc
-0001eeb0: 616c 6172 5f62 6172 5f61 7267 733d 7b27  alar_bar_args={'
-0001eec0: 636f 6c6f 7227 3a20 276b 277d 2c0a 2020  color': 'k'},.  
-0001eed0: 2020 2e2e 2e20 2020 2020 636d 6170 3d27    ...     cmap='
-0001eee0: 6277 7227 2c0a 2020 2020 2e2e 2e20 290a  bwr',.    ... ).
-0001eef0: 0a20 2020 2022 2222 0a20 2020 2072 6574  .    """.    ret
-0001ef00: 7572 6e20 5f64 6f77 6e6c 6f61 645f 616e  urn _download_an
-0001ef10: 645f 7265 6164 2827 6c65 7468 652f 7265  d_read('lethe/re
-0001ef20: 7375 6c74 5f70 6172 7469 636c 6573 2e32  sult_particles.2
-0001ef30: 3030 3030 2e30 3030 302e 7674 7527 2c20  0000.0000.vtu', 
-0001ef40: 6c6f 6164 3d6c 6f61 6429 0a0a 0a64 6566  load=load)...def
-0001ef50: 2064 6f77 6e6c 6f61 645f 6769 665f 7369   download_gif_si
-0001ef60: 6d70 6c65 286c 6f61 643d 5472 7565 293a  mple(load=True):
-0001ef70: 2020 2320 7072 6167 6d61 3a20 6e6f 2063    # pragma: no c
-0001ef80: 6f76 6572 0a20 2020 2022 2222 446f 776e  over.    """Down
-0001ef90: 6c6f 6164 2061 2073 696d 706c 6520 7468  load a simple th
-0001efa0: 7265 6520 6672 616d 6520 4749 462e 0a0a  ree frame GIF...
-0001efb0: 2020 2020 5061 7261 6d65 7465 7273 0a20      Parameters. 
-0001efc0: 2020 202d 2d2d 2d2d 2d2d 2d2d 2d0a 2020     ----------.  
-0001efd0: 2020 6c6f 6164 203a 2062 6f6f 6c2c 2064    load : bool, d
-0001efe0: 6566 6175 6c74 3a20 5472 7565 0a20 2020  efault: True.   
-0001eff0: 2020 2020 204c 6f61 6420 7468 6520 6461       Load the da
-0001f000: 7461 7365 7420 6166 7465 7220 646f 776e  taset after down
-0001f010: 6c6f 6164 696e 6720 6974 2077 6865 6e20  loading it when 
-0001f020: 6060 5472 7565 6060 2e20 2053 6574 2074  ``True``.  Set t
-0001f030: 6869 730a 2020 2020 2020 2020 746f 2060  his.        to `
-0001f040: 6046 616c 7365 6060 2061 6e64 206f 6e6c  `False`` and onl
-0001f050: 7920 7468 6520 6669 6c65 6e61 6d65 2077  y the filename w
-0001f060: 696c 6c20 6265 2072 6574 7572 6e65 642e  ill be returned.
-0001f070: 0a0a 2020 2020 5265 7475 726e 730a 2020  ..    Returns.  
-0001f080: 2020 2d2d 2d2d 2d2d 2d0a 2020 2020 7079    -------.    py
-0001f090: 7669 7374 612e 496d 6167 6544 6174 6120  vista.ImageData 
-0001f0a0: 7c20 7374 720a 2020 2020 2020 2020 4461  | str.        Da
-0001f0b0: 7461 5365 7420 6f72 2066 696c 656e 616d  taSet or filenam
-0001f0c0: 6520 6465 7065 6e64 696e 6720 6f6e 2060  e depending on `
-0001f0d0: 606c 6f61 6460 602e 0a0a 2020 2020 4578  `load``...    Ex
-0001f0e0: 616d 706c 6573 0a20 2020 202d 2d2d 2d2d  amples.    -----
-0001f0f0: 2d2d 2d0a 2020 2020 446f 776e 6c6f 6164  ---.    Download
-0001f100: 2061 6e64 2070 6c6f 7420 7468 6520 6669   and plot the fi
-0001f110: 7273 7420 6672 616d 6520 6f66 2061 2073  rst frame of a s
-0001f120: 696d 706c 6520 4749 462e 0a0a 2020 2020  imple GIF...    
-0001f130: 3e3e 3e20 6672 6f6d 2070 7976 6973 7461  >>> from pyvista
-0001f140: 2069 6d70 6f72 7420 6578 616d 706c 6573   import examples
-0001f150: 0a20 2020 203e 3e3e 2067 7269 6420 3d20  .    >>> grid = 
-0001f160: 6578 616d 706c 6573 2e64 6f77 6e6c 6f61  examples.downloa
-0001f170: 645f 6769 665f 7369 6d70 6c65 2829 0a20  d_gif_simple(). 
-0001f180: 2020 203e 3e3e 2067 7269 642e 706c 6f74     >>> grid.plot
-0001f190: 280a 2020 2020 2e2e 2e20 2020 2020 7363  (.    ...     sc
-0001f1a0: 616c 6172 733d 2766 7261 6d65 3027 2c0a  alars='frame0',.
-0001f1b0: 2020 2020 2e2e 2e20 2020 2020 7267 623d      ...     rgb=
-0001f1c0: 5472 7565 2c0a 2020 2020 2e2e 2e20 2020  True,.    ...   
-0001f1d0: 2020 6261 636b 6772 6f75 6e64 3d27 7727    background='w'
-0001f1e0: 2c0a 2020 2020 2e2e 2e20 2020 2020 7368  ,.    ...     sh
-0001f1f0: 6f77 5f73 6361 6c61 725f 6261 723d 4661  ow_scalar_bar=Fa
-0001f200: 6c73 652c 0a20 2020 202e 2e2e 2020 2020  lse,.    ...    
-0001f210: 2063 706f 733d 2778 7927 2c0a 2020 2020   cpos='xy',.    
-0001f220: 2e2e 2e20 290a 0a20 2020 2050 6c6f 7420  ... )..    Plot 
-0001f230: 7468 6520 7365 636f 6e64 2066 7261 6d65  the second frame
-0001f240: 2e0a 0a20 2020 203e 3e3e 2067 7269 642e  ...    >>> grid.
-0001f250: 706c 6f74 280a 2020 2020 2e2e 2e20 2020  plot(.    ...   
-0001f260: 2020 7363 616c 6172 733d 2766 7261 6d65    scalars='frame
-0001f270: 3127 2c0a 2020 2020 2e2e 2e20 2020 2020  1',.    ...     
-0001f280: 7267 623d 5472 7565 2c0a 2020 2020 2e2e  rgb=True,.    ..
-0001f290: 2e20 2020 2020 6261 636b 6772 6f75 6e64  .     background
-0001f2a0: 3d27 7727 2c0a 2020 2020 2e2e 2e20 2020  ='w',.    ...   
-0001f2b0: 2020 7368 6f77 5f73 6361 6c61 725f 6261    show_scalar_ba
-0001f2c0: 723d 4661 6c73 652c 0a20 2020 202e 2e2e  r=False,.    ...
-0001f2d0: 2020 2020 2063 706f 733d 2778 7927 2c0a       cpos='xy',.
-0001f2e0: 2020 2020 2e2e 2e20 290a 0a20 2020 2022      ... )..    "
-0001f2f0: 2222 0a20 2020 2072 6574 7572 6e20 5f64  "".    return _d
-0001f300: 6f77 6e6c 6f61 645f 616e 645f 7265 6164  ownload_and_read
-0001f310: 2827 6769 6673 2f73 616d 706c 652e 6769  ('gifs/sample.gi
-0001f320: 6627 2c20 6c6f 6164 3d6c 6f61 6429 0a0a  f', load=load)..
-0001f330: 0a64 6566 2064 6f77 6e6c 6f61 645f 636c  .def download_cl
-0001f340: 6f75 645f 6461 726b 5f6d 6174 7465 7228  oud_dark_matter(
-0001f350: 6c6f 6164 3d54 7275 6529 3a20 2023 2070  load=True):  # p
-0001f360: 7261 676d 613a 206e 6f20 636f 7665 720a  ragma: no cover.
-0001f370: 2020 2020 2222 2244 6f77 6e6c 6f61 6420      """Download 
-0001f380: 7061 7274 6963 6c65 7320 6672 6f6d 2061  particles from a
-0001f390: 2073 696d 756c 6174 6564 2064 6172 6b20   simulated dark 
-0001f3a0: 6d61 7474 6572 2068 616c 6f2e 0a0a 2020  matter halo...  
-0001f3b0: 2020 5468 6973 2064 6174 6173 6574 2063    This dataset c
-0001f3c0: 6f6e 7461 696e 7320 3332 2c33 3134 2070  ontains 32,314 p
-0001f3d0: 6172 7469 636c 6573 2e0a 0a20 2020 2050  articles...    P
-0001f3e0: 6172 616d 6574 6572 730a 2020 2020 2d2d  arameters.    --
-0001f3f0: 2d2d 2d2d 2d2d 2d2d 0a20 2020 206c 6f61  --------.    loa
-0001f400: 6420 3a20 626f 6f6c 2c20 6465 6661 756c  d : bool, defaul
-0001f410: 743a 2054 7275 650a 2020 2020 2020 2020  t: True.        
-0001f420: 4c6f 6164 2074 6865 2064 6174 6173 6574  Load the dataset
-0001f430: 2061 6674 6572 2064 6f77 6e6c 6f61 6469   after downloadi
-0001f440: 6e67 2069 7420 7768 656e 2060 6054 7275  ng it when ``Tru
-0001f450: 6560 602e 2020 5365 7420 7468 6973 0a20  e``.  Set this. 
-0001f460: 2020 2020 2020 2074 6f20 6060 4661 6c73         to ``Fals
-0001f470: 6560 6020 616e 6420 6f6e 6c79 2074 6865  e`` and only the
-0001f480: 2066 696c 656e 616d 6520 7769 6c6c 2062   filename will b
-0001f490: 6520 7265 7475 726e 6564 2e0a 0a20 2020  e returned...   
-0001f4a0: 2052 6574 7572 6e73 0a20 2020 202d 2d2d   Returns.    ---
-0001f4b0: 2d2d 2d2d 0a20 2020 2070 7976 6973 7461  ----.    pyvista
-0001f4c0: 2e50 6f69 6e74 5365 7420 7c20 7374 720a  .PointSet | str.
-0001f4d0: 2020 2020 2020 2020 4461 7461 5365 7420          DataSet 
-0001f4e0: 6f72 2066 696c 656e 616d 6520 6465 7065  or filename depe
-0001f4f0: 6e64 696e 6720 6f6e 2060 606c 6f61 6460  nding on ``load`
-0001f500: 602e 0a0a 2020 2020 4578 616d 706c 6573  `...    Examples
-0001f510: 0a20 2020 202d 2d2d 2d2d 2d2d 2d0a 2020  .    --------.  
-0001f520: 2020 446f 776e 6c6f 6164 2074 6865 2064    Download the d
-0001f530: 6172 6b20 6d61 7474 6572 2063 6c6f 7564  ark matter cloud
-0001f540: 2061 6e64 2064 6973 706c 6179 2069 7473   and display its
-0001f550: 2072 6570 7265 7365 6e74 6174 696f 6e2e   representation.
-0001f560: 0a0a 2020 2020 3e3e 3e20 696d 706f 7274  ..    >>> import
-0001f570: 206e 756d 7079 2061 7320 6e70 0a20 2020   numpy as np.   
-0001f580: 203e 3e3e 2066 726f 6d20 7079 7669 7374   >>> from pyvist
-0001f590: 6120 696d 706f 7274 2065 7861 6d70 6c65  a import example
-0001f5a0: 730a 2020 2020 3e3e 3e20 7063 203d 2065  s.    >>> pc = e
-0001f5b0: 7861 6d70 6c65 732e 646f 776e 6c6f 6164  xamples.download
-0001f5c0: 5f63 6c6f 7564 5f64 6172 6b5f 6d61 7474  _cloud_dark_matt
-0001f5d0: 6572 2829 0a20 2020 203e 3e3e 2070 630a  er().    >>> pc.
-0001f5e0: 2020 2020 506f 696e 7453 6574 2028 2e2e      PointSet (..
-0001f5f0: 2e29 0a20 2020 2020 204e 2043 656c 6c73  .).      N Cells
-0001f600: 3a20 2020 2030 0a20 2020 2020 204e 2050  :    0.      N P
-0001f610: 6f69 6e74 733a 2020 2033 3233 3134 0a20  oints:   32314. 
-0001f620: 2020 2020 2058 2042 6f75 6e64 733a 2020       X Bounds:  
-0001f630: 2037 2e34 3531 652b 3031 2c20 372e 3839   7.451e+01, 7.89
-0001f640: 3265 2b30 310a 2020 2020 2020 5920 426f  2e+01.      Y Bo
-0001f650: 756e 6473 3a20 2020 312e 3631 3665 2b30  unds:   1.616e+0
-0001f660: 312c 2032 2e32 3735 652b 3031 0a20 2020  1, 2.275e+01.   
-0001f670: 2020 205a 2042 6f75 6e64 733a 2020 2038     Z Bounds:   8
-0001f680: 2e39 3030 652b 3031 2c20 392e 3331 3965  .900e+01, 9.319e
-0001f690: 2b30 310a 2020 2020 2020 4e20 4172 7261  +01.      N Arra
-0001f6a0: 7973 3a20 2020 300a 0a20 2020 2050 6c6f  ys:   0..    Plo
-0001f6b0: 7420 7468 6520 706f 696e 7420 636c 6f75  t the point clou
-0001f6c0: 642e 2043 6f6c 6f72 2062 6173 6564 206f  d. Color based o
-0001f6d0: 6e20 7468 6520 6469 7374 616e 6365 2066  n the distance f
-0001f6e0: 726f 6d20 7468 6520 6365 6e74 6572 206f  rom the center o
-0001f6f0: 6620 7468 650a 2020 2020 636c 6f75 642e  f the.    cloud.
-0001f700: 0a0a 2020 2020 3e3e 3e20 7063 2e70 6c6f  ..    >>> pc.plo
-0001f710: 7428 0a20 2020 202e 2e2e 2020 2020 2073  t(.    ...     s
-0001f720: 6361 6c61 7273 3d6e 702e 6c69 6e61 6c67  calars=np.linalg
-0001f730: 2e6e 6f72 6d28 7063 2e70 6f69 6e74 7320  .norm(pc.points 
-0001f740: 2d20 7063 2e63 656e 7465 722c 2061 7869  - pc.center, axi
-0001f750: 733d 3129 2c0a 2020 2020 2e2e 2e20 2020  s=1),.    ...   
-0001f760: 2020 7374 796c 653d 2770 6f69 6e74 735f    style='points_
-0001f770: 6761 7573 7369 616e 272c 0a20 2020 202e  gaussian',.    .
-0001f780: 2e2e 2020 2020 206f 7061 6369 7479 3d30  ..     opacity=0
-0001f790: 2e35 2c0a 2020 2020 2e2e 2e20 2020 2020  .5,.    ...     
-0001f7a0: 706f 696e 745f 7369 7a65 3d31 2e35 2c0a  point_size=1.5,.
-0001f7b0: 2020 2020 2e2e 2e20 2020 2020 7368 6f77      ...     show
-0001f7c0: 5f73 6361 6c61 725f 6261 723d 4661 6c73  _scalar_bar=Fals
-0001f7d0: 652c 0a20 2020 202e 2e2e 2020 2020 207a  e,.    ...     z
-0001f7e0: 6f6f 6d3d 322c 0a20 2020 202e 2e2e 2029  oom=2,.    ... )
-0001f7f0: 0a0a 2020 2020 5365 6520 7468 6520 3a72  ..    See the :r
-0001f800: 6566 3a60 706c 6f74 7469 6e67 5f70 6f69  ef:`plotting_poi
-0001f810: 6e74 5f63 6c6f 7564 7360 2066 6f72 2061  nt_clouds` for a
-0001f820: 2066 756c 6c20 6578 616d 706c 6520 7573   full example us
-0001f830: 696e 6720 7468 6973 2064 6174 6173 6574  ing this dataset
-0001f840: 2e0a 0a20 2020 2022 2222 0a20 2020 2066  ...    """.    f
-0001f850: 696c 656e 616d 6520 3d20 646f 776e 6c6f  ilename = downlo
-0001f860: 6164 5f66 696c 6528 2770 6f69 6e74 2d63  ad_file('point-c
-0001f870: 6c6f 7564 732f 6669 6e64 7573 3233 2f68  louds/findus23/h
-0001f880: 616c 6f5f 6c6f 775f 7265 732e 6e70 7927  alo_low_res.npy'
-0001f890: 290a 0a20 2020 2069 6620 6c6f 6164 3a0a  )..    if load:.
-0001f8a0: 2020 2020 2020 2020 7265 7475 726e 2070          return p
-0001f8b0: 7976 6973 7461 2e50 6f69 6e74 5365 7428  yvista.PointSet(
-0001f8c0: 6e70 2e6c 6f61 6428 6669 6c65 6e61 6d65  np.load(filename
-0001f8d0: 2929 0a20 2020 2072 6574 7572 6e20 6669  )).    return fi
-0001f8e0: 6c65 6e61 6d65 0a0a 0a64 6566 2064 6f77  lename...def dow
-0001f8f0: 6e6c 6f61 645f 636c 6f75 645f 6461 726b  nload_cloud_dark
-0001f900: 5f6d 6174 7465 725f 6465 6e73 6528 6c6f  _matter_dense(lo
-0001f910: 6164 3d54 7275 6529 3a20 2023 2070 7261  ad=True):  # pra
-0001f920: 676d 613a 206e 6f20 636f 7665 720a 2020  gma: no cover.  
-0001f930: 2020 2222 2244 6f77 6e6c 6f61 6420 6120    """Download a 
-0001f940: 7061 7274 6963 6c65 7320 6672 6f6d 2061  particles from a
-0001f950: 2073 696d 756c 6174 6564 2064 6172 6b20   simulated dark 
-0001f960: 6d61 7474 6572 2068 616c 6f2e 0a0a 2020  matter halo...  
-0001f970: 2020 5468 6973 2064 6174 6173 6574 2063    This dataset c
-0001f980: 6f6e 7461 696e 7320 322c 3036 322c 3235  ontains 2,062,25
-0001f990: 3620 7061 7274 6963 6c65 732e 0a0a 2020  6 particles...  
-0001f9a0: 2020 5061 7261 6d65 7465 7273 0a20 2020    Parameters.   
-0001f9b0: 202d 2d2d 2d2d 2d2d 2d2d 2d0a 2020 2020   ----------.    
-0001f9c0: 6c6f 6164 203a 2062 6f6f 6c2c 2064 6566  load : bool, def
-0001f9d0: 6175 6c74 3a20 5472 7565 0a20 2020 2020  ault: True.     
-0001f9e0: 2020 204c 6f61 6420 7468 6520 6461 7461     Load the data
-0001f9f0: 7365 7420 6166 7465 7220 646f 776e 6c6f  set after downlo
-0001fa00: 6164 696e 6720 6974 2077 6865 6e20 6060  ading it when ``
-0001fa10: 5472 7565 6060 2e20 2053 6574 2074 6869  True``.  Set thi
-0001fa20: 730a 2020 2020 2020 2020 746f 2060 6046  s.        to ``F
-0001fa30: 616c 7365 6060 2061 6e64 206f 6e6c 7920  alse`` and only 
-0001fa40: 7468 6520 6669 6c65 6e61 6d65 2077 696c  the filename wil
-0001fa50: 6c20 6265 2072 6574 7572 6e65 642e 0a0a  l be returned...
-0001fa60: 2020 2020 5265 7475 726e 730a 2020 2020      Returns.    
-0001fa70: 2d2d 2d2d 2d2d 2d0a 2020 2020 7079 7669  -------.    pyvi
-0001fa80: 7374 612e 506f 696e 7453 6574 207c 2073  sta.PointSet | s
-0001fa90: 7472 0a20 2020 2020 2020 2044 6174 6153  tr.        DataS
-0001faa0: 6574 206f 7220 6669 6c65 6e61 6d65 2064  et or filename d
-0001fab0: 6570 656e 6469 6e67 206f 6e20 6060 6c6f  epending on ``lo
-0001fac0: 6164 6060 2e0a 0a20 2020 2045 7861 6d70  ad``...    Examp
-0001fad0: 6c65 730a 2020 2020 2d2d 2d2d 2d2d 2d2d  les.    --------
-0001fae0: 0a20 2020 2044 6f77 6e6c 6f61 6420 7468  .    Download th
-0001faf0: 6520 6461 726b 206d 6174 7465 7220 636c  e dark matter cl
-0001fb00: 6f75 6420 616e 6420 6469 7370 6c61 7920  oud and display 
-0001fb10: 6974 7320 7265 7072 6573 656e 7461 7469  its representati
-0001fb20: 6f6e 2e0a 0a20 2020 203e 3e3e 2069 6d70  on...    >>> imp
-0001fb30: 6f72 7420 6e75 6d70 7920 6173 206e 700a  ort numpy as np.
-0001fb40: 2020 2020 3e3e 3e20 6672 6f6d 2070 7976      >>> from pyv
-0001fb50: 6973 7461 2069 6d70 6f72 7420 6578 616d  ista import exam
-0001fb60: 706c 6573 0a20 2020 203e 3e3e 2070 6320  ples.    >>> pc 
-0001fb70: 3d20 6578 616d 706c 6573 2e64 6f77 6e6c  = examples.downl
-0001fb80: 6f61 645f 636c 6f75 645f 6461 726b 5f6d  oad_cloud_dark_m
-0001fb90: 6174 7465 725f 6465 6e73 6528 290a 2020  atter_dense().  
-0001fba0: 2020 3e3e 3e20 7063 0a20 2020 2050 6f69    >>> pc.    Poi
-0001fbb0: 6e74 5365 7420 282e 2e2e 290a 2020 2020  ntSet (...).    
-0001fbc0: 2020 4e20 4365 6c6c 733a 2020 2020 300a    N Cells:    0.
-0001fbd0: 2020 2020 2020 4e20 506f 696e 7473 3a20        N Points: 
-0001fbe0: 2020 3230 3632 3235 360a 2020 2020 2020    2062256.      
-0001fbf0: 5820 426f 756e 6473 3a20 2020 372e 3436  X Bounds:   7.46
-0001fc00: 3265 2b30 312c 2037 2e38 3633 652b 3031  2e+01, 7.863e+01
-0001fc10: 0a20 2020 2020 2059 2042 6f75 6e64 733a  .      Y Bounds:
-0001fc20: 2020 2031 2e36 3034 652b 3031 2c20 322e     1.604e+01, 2.
-0001fc30: 3234 3465 2b30 310a 2020 2020 2020 5a20  244e+01.      Z 
-0001fc40: 426f 756e 6473 3a20 2020 382e 3839 3365  Bounds:   8.893e
-0001fc50: 2b30 312c 2039 2e33 3337 652b 3031 0a20  +01, 9.337e+01. 
-0001fc60: 2020 2020 204e 2041 7272 6179 733a 2020       N Arrays:  
-0001fc70: 2030 0a0a 2020 2020 506c 6f74 2074 6865   0..    Plot the
-0001fc80: 2070 6f69 6e74 2063 6c6f 7564 2e20 436f   point cloud. Co
-0001fc90: 6c6f 7220 6261 7365 6420 6f6e 2074 6865  lor based on the
-0001fca0: 2064 6973 7461 6e63 6520 6672 6f6d 2074   distance from t
-0001fcb0: 6865 2063 656e 7465 7220 6f66 2074 6865  he center of the
-0001fcc0: 0a20 2020 2063 6c6f 7564 2e0a 0a20 2020  .    cloud...   
-0001fcd0: 203e 3e3e 2070 632e 706c 6f74 280a 2020   >>> pc.plot(.  
-0001fce0: 2020 2e2e 2e20 2020 2020 7363 616c 6172    ...     scalar
-0001fcf0: 733d 6e70 2e6c 696e 616c 672e 6e6f 726d  s=np.linalg.norm
-0001fd00: 2870 632e 706f 696e 7473 202d 2070 632e  (pc.points - pc.
-0001fd10: 6365 6e74 6572 2c20 6178 6973 3d31 292c  center, axis=1),
-0001fd20: 0a20 2020 202e 2e2e 2020 2020 2073 7479  .    ...     sty
-0001fd30: 6c65 3d27 706f 696e 7473 5f67 6175 7373  le='points_gauss
-0001fd40: 6961 6e27 2c0a 2020 2020 2e2e 2e20 2020  ian',.    ...   
-0001fd50: 2020 6f70 6163 6974 793d 302e 3033 302c    opacity=0.030,
-0001fd60: 0a20 2020 202e 2e2e 2020 2020 2070 6f69  .    ...     poi
-0001fd70: 6e74 5f73 697a 653d 322e 302c 0a20 2020  nt_size=2.0,.   
-0001fd80: 202e 2e2e 2020 2020 2073 686f 775f 7363   ...     show_sc
-0001fd90: 616c 6172 5f62 6172 3d46 616c 7365 2c0a  alar_bar=False,.
-0001fda0: 2020 2020 2e2e 2e20 2020 2020 7a6f 6f6d      ...     zoom
-0001fdb0: 3d32 2c0a 2020 2020 2e2e 2e20 290a 0a20  =2,.    ... ).. 
-0001fdc0: 2020 2053 6565 2074 6865 203a 7265 663a     See the :ref:
-0001fdd0: 6070 6c6f 7474 696e 675f 706f 696e 745f  `plotting_point_
-0001fde0: 636c 6f75 6473 6020 666f 7220 6d6f 7265  clouds` for more
-0001fdf0: 2064 6574 6169 6c73 206f 6e20 686f 7720   details on how 
-0001fe00: 746f 2070 6c6f 7420 706f 696e 740a 2020  to plot point.  
-0001fe10: 2020 636c 6f75 6473 2e0a 0a20 2020 2022    clouds...    "
-0001fe20: 2222 0a20 2020 2066 696c 656e 616d 6520  "".    filename 
-0001fe30: 3d20 646f 776e 6c6f 6164 5f66 696c 6528  = download_file(
-0001fe40: 2770 6f69 6e74 2d63 6c6f 7564 732f 6669  'point-clouds/fi
-0001fe50: 6e64 7573 3233 2f68 616c 6f5f 6869 6768  ndus23/halo_high
-0001fe60: 5f72 6573 2e6e 7079 2729 0a0a 2020 2020  _res.npy')..    
-0001fe70: 6966 206c 6f61 643a 0a20 2020 2020 2020  if load:.       
-0001fe80: 2072 6574 7572 6e20 7079 7669 7374 612e   return pyvista.
-0001fe90: 506f 696e 7453 6574 286e 702e 6c6f 6164  PointSet(np.load
-0001fea0: 2866 696c 656e 616d 6529 290a 2020 2020  (filename)).    
-0001feb0: 7265 7475 726e 2066 696c 656e 616d 650a  return filename.
-0001fec0: 0a0a 6465 6620 646f 776e 6c6f 6164 5f73  ..def download_s
-0001fed0: 7461 7273 5f63 6c6f 7564 5f68 7967 286c  tars_cloud_hyg(l
-0001fee0: 6f61 643d 5472 7565 293a 2020 2320 7072  oad=True):  # pr
-0001fef0: 6167 6d61 3a20 6e6f 2063 6f76 6572 0a20  agma: no cover. 
-0001ff00: 2020 2022 2222 446f 776e 6c6f 6164 2061     """Download a
-0001ff10: 2070 6f69 6e74 2063 6c6f 7564 206f 6620   point cloud of 
-0001ff20: 7374 6172 7320 6173 2063 6f6d 7075 7465  stars as compute
-0001ff30: 6420 6279 2074 6865 2048 5947 2044 6174  d by the HYG Dat
-0001ff40: 6162 6173 652e 0a0a 2020 2020 5365 6520  abase...    See 
-0001ff50: 6048 5947 2d44 6174 6162 6173 6520 3c68  `HYG-Database <h
-0001ff60: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
-0001ff70: 6d2f 6173 7472 6f6e 6578 7573 2f48 5947  m/astronexus/HYG
-0001ff80: 2d44 6174 6162 6173 653e 605f 2066 6f72  -Database>`_ for
-0001ff90: 206d 6f72 650a 2020 2020 6465 7461 696c   more.    detail
-0001ffa0: 732e 0a0a 2020 2020 5468 6973 2064 6174  s...    This dat
-0001ffb0: 6120 7365 7420 6973 206c 6963 656e 7365  a set is license
-0001ffc0: 6420 6279 2061 2043 7265 6174 6976 6520  d by a Creative 
-0001ffd0: 436f 6d6d 6f6e 7320 4174 7472 6962 7574  Commons Attribut
-0001ffe0: 696f 6e2d 5368 6172 6541 6c69 6b65 0a20  ion-ShareAlike. 
-0001fff0: 2020 206c 6963 656e 7365 2e20 466f 7220     license. For 
-00020000: 6d6f 7265 2064 6574 6169 6c73 2c20 7265  more details, re
-00020010: 6164 2074 6865 2060 4372 6561 7469 7665  ad the `Creative
-00020020: 2043 6f6d 6d6f 6e73 2070 6167 650a 2020   Commons page.  
-00020030: 2020 3c68 7474 7073 3a2f 2f63 7265 6174    <https://creat
-00020040: 6976 6563 6f6d 6d6f 6e73 2e6f 7267 2f6c  ivecommons.org/l
-00020050: 6963 656e 7365 732f 6279 2d73 612f 322e  icenses/by-sa/2.
-00020060: 352f 3e60 5f0a 0a20 2020 2053 6565 2074  5/>`_..    See t
-00020070: 6865 2060 5245 4144 4d45 2e6d 640a 2020  he `README.md.  
-00020080: 2020 3c68 7474 7073 3a2f 2f67 6974 6875    <https://githu
-00020090: 622e 636f 6d2f 7079 7669 7374 612f 7674  b.com/pyvista/vt
-000200a0: 6b2d 6461 7461 2f62 6c6f 622f 6d61 7374  k-data/blob/mast
-000200b0: 6572 2f44 6174 612f 706f 696e 742d 636c  er/Data/point-cl
-000200c0: 6f75 6473 2f68 7967 2d64 6174 6162 6173  ouds/hyg-databas
-000200d0: 652f 5245 4144 4d45 2e6d 643e 605f 0a20  e/README.md>`_. 
-000200e0: 2020 2066 6f72 206d 6f72 6520 6465 7461     for more deta
-000200f0: 696c 7320 666f 7220 686f 7720 7468 6520  ils for how the 
-00020100: 7374 6172 2063 6f6c 6f72 7320 7765 7265  star colors were
-00020110: 2063 6f6d 7075 7465 642e 0a0a 2020 2020   computed...    
-00020120: 4469 7374 616e 6365 7320 6172 6520 696e  Distances are in
-00020130: 2070 6172 7365 6373 2066 726f 6d20 4561   parsecs from Ea
-00020140: 7274 682e 0a0a 2020 2020 5061 7261 6d65  rth...    Parame
-00020150: 7465 7273 0a20 2020 202d 2d2d 2d2d 2d2d  ters.    -------
-00020160: 2d2d 2d0a 2020 2020 6c6f 6164 203a 2062  ---.    load : b
-00020170: 6f6f 6c2c 2064 6566 6175 6c74 3a20 5472  ool, default: Tr
-00020180: 7565 0a20 2020 2020 2020 204c 6f61 6420  ue.        Load 
-00020190: 7468 6520 6461 7461 7365 7420 6166 7465  the dataset afte
-000201a0: 7220 646f 776e 6c6f 6164 696e 6720 6974  r downloading it
-000201b0: 2077 6865 6e20 6060 5472 7565 6060 2e20   when ``True``. 
-000201c0: 2053 6574 2074 6869 730a 2020 2020 2020   Set this.      
-000201d0: 2020 746f 2060 6046 616c 7365 6060 2061    to ``False`` a
-000201e0: 6e64 206f 6e6c 7920 7468 6520 6669 6c65  nd only the file
-000201f0: 6e61 6d65 2077 696c 6c20 6265 2072 6574  name will be ret
-00020200: 7572 6e65 642e 0a0a 2020 2020 5265 7475  urned...    Retu
-00020210: 726e 730a 2020 2020 2d2d 2d2d 2d2d 2d0a  rns.    -------.
-00020220: 2020 2020 7079 7669 7374 612e 506f 6c79      pyvista.Poly
-00020230: 4461 7461 207c 2073 7472 0a20 2020 2020  Data | str.     
-00020240: 2020 2044 6174 6153 6574 206f 7220 6669     DataSet or fi
-00020250: 6c65 6e61 6d65 2064 6570 656e 6469 6e67  lename depending
-00020260: 206f 6e20 6060 6c6f 6164 6060 2e0a 0a20   on ``load``... 
-00020270: 2020 2045 7861 6d70 6c65 730a 2020 2020     Examples.    
-00020280: 2d2d 2d2d 2d2d 2d2d 0a20 2020 2044 6f77  --------.    Dow
-00020290: 6e6c 6f61 6420 616e 6420 706c 6f74 2061  nload and plot a
-000202a0: 2070 6f69 6e74 2063 6c6f 7564 206f 6620   point cloud of 
-000202b0: 7374 6172 7320 7769 7468 696e 2033 2c30  stars within 3,0
-000202c0: 3030 206c 6967 6874 2079 6561 7273 2e20  00 light years. 
-000202d0: 5374 6172 730a 2020 2020 6172 6520 636f  Stars.    are co
-000202e0: 6c6f 7265 6420 6163 636f 7264 696e 6720  lored according 
-000202f0: 746f 2074 6865 6972 2052 4742 4120 636f  to their RGBA co
-00020300: 6c6f 7273 2e0a 0a20 2020 203e 3e3e 2069  lors...    >>> i
-00020310: 6d70 6f72 7420 6e75 6d70 7920 6173 206e  mport numpy as n
-00020320: 700a 2020 2020 3e3e 3e20 6672 6f6d 2070  p.    >>> from p
-00020330: 7976 6973 7461 2069 6d70 6f72 7420 6578  yvista import ex
-00020340: 616d 706c 6573 0a20 2020 203e 3e3e 2073  amples.    >>> s
-00020350: 7461 7273 203d 2065 7861 6d70 6c65 732e  tars = examples.
-00020360: 646f 776e 6c6f 6164 5f73 7461 7273 5f63  download_stars_c
-00020370: 6c6f 7564 5f68 7967 2829 0a20 2020 203e  loud_hyg().    >
-00020380: 3e3e 2073 7461 7273 2e70 6c6f 7428 0a20  >> stars.plot(. 
-00020390: 2020 202e 2e2e 2020 2020 2073 7479 6c65     ...     style
-000203a0: 3d27 706f 696e 7473 5f67 6175 7373 6961  ='points_gaussia
-000203b0: 6e27 2c0a 2020 2020 2e2e 2e20 2020 2020  n',.    ...     
-000203c0: 6261 636b 6772 6f75 6e64 3d27 6b27 2c0a  background='k',.
-000203d0: 2020 2020 2e2e 2e20 2020 2020 706f 696e      ...     poin
-000203e0: 745f 7369 7a65 3d30 2e35 2c0a 2020 2020  t_size=0.5,.    
-000203f0: 2e2e 2e20 2020 2020 7363 616c 6172 733d  ...     scalars=
-00020400: 275f 7267 6261 272c 0a20 2020 202e 2e2e  '_rgba',.    ...
-00020410: 2020 2020 2072 656e 6465 725f 706f 696e       render_poin
-00020420: 7473 5f61 735f 7370 6865 7265 733d 4661  ts_as_spheres=Fa
-00020430: 6c73 652c 0a20 2020 202e 2e2e 2020 2020  lse,.    ...    
-00020440: 207a 6f6f 6d3d 332e 302c 0a20 2020 202e   zoom=3.0,.    .
-00020450: 2e2e 2029 0a0a 2020 2020 3e3e 3e20 7374  .. )..    >>> st
-00020460: 6172 730a 2020 2020 506f 6c79 4461 7461  ars.    PolyData
-00020470: 2028 2e2e 2e29 0a20 2020 2020 204e 2043   (...).      N C
-00020480: 656c 6c73 3a20 2020 2031 3037 3835 370a  ells:    107857.
-00020490: 2020 2020 2020 4e20 506f 696e 7473 3a20        N Points: 
-000204a0: 2020 3130 3738 3537 0a20 2020 2020 204e    107857.      N
-000204b0: 2053 7472 6970 733a 2020 2030 0a20 2020   Strips:   0.   
-000204c0: 2020 2058 2042 6f75 6e64 733a 2020 202d     X Bounds:   -
-000204d0: 392e 3735 3565 2b30 322c 2039 2e37 3734  9.755e+02, 9.774
-000204e0: 652b 3032 0a20 2020 2020 2059 2042 6f75  e+02.      Y Bou
-000204f0: 6e64 733a 2020 202d 392e 3632 3065 2b30  nds:   -9.620e+0
-00020500: 322c 2039 2e36 3632 652b 3032 0a20 2020  2, 9.662e+02.   
-00020510: 2020 205a 2042 6f75 6e64 733a 2020 202d     Z Bounds:   -
-00020520: 392e 3738 3865 2b30 322c 2039 2e37 3032  9.788e+02, 9.702
-00020530: 652b 3032 0a20 2020 2020 204e 2041 7272  e+02.      N Arr
-00020540: 6179 733a 2020 2033 0a0a 2020 2020 5365  ays:   3..    Se
-00020550: 6520 7468 6520 3a72 6566 3a60 706c 6f74  e the :ref:`plot
-00020560: 7469 6e67 5f70 6f69 6e74 5f63 6c6f 7564  ting_point_cloud
-00020570: 7360 2066 6f72 206d 6f72 6520 6465 7461  s` for more deta
-00020580: 696c 7320 6f6e 2068 6f77 2074 6f20 706c  ils on how to pl
-00020590: 6f74 2070 6f69 6e74 0a20 2020 2063 6c6f  ot point.    clo
-000205a0: 7564 732e 0a0a 2020 2020 2222 220a 2020  uds...    """.  
-000205b0: 2020 7265 7475 726e 205f 646f 776e 6c6f    return _downlo
-000205c0: 6164 5f61 6e64 5f72 6561 6428 2770 6f69  ad_and_read('poi
-000205d0: 6e74 2d63 6c6f 7564 732f 6879 672d 6461  nt-clouds/hyg-da
-000205e0: 7461 6261 7365 2f73 7461 7273 2e76 7470  tabase/stars.vtp
-000205f0: 272c 206c 6f61 643d 6c6f 6164 290a 0a0a  ', load=load)...
-00020600: 6465 6620 646f 776e 6c6f 6164 5f66 6561  def download_fea
-00020610: 5f62 7261 636b 6574 286c 6f61 643d 5472  _bracket(load=Tr
-00020620: 7565 293a 2020 2320 7072 6167 6d61 3a20  ue):  # pragma: 
-00020630: 6e6f 2063 6f76 6572 0a20 2020 2022 2222  no cover.    """
-00020640: 446f 776e 6c6f 6164 2074 6865 2066 696e  Download the fin
-00020650: 6974 6520 656c 656d 656e 7420 736f 6c75  ite element solu
-00020660: 7469 6f6e 206f 6620 6120 6272 6163 6b65  tion of a bracke
-00020670: 742e 0a0a 2020 2020 436f 6e74 6169 6e73  t...    Contains
-00020680: 2076 6f6e 2d6d 6973 6573 2065 7175 6976   von-mises equiv
-00020690: 616c 656e 7420 6365 6c6c 2073 7472 6573  alent cell stres
-000206a0: 7320 6173 7375 6d69 6e67 2061 2076 6572  s assuming a ver
-000206b0: 7469 6361 6c20 2879 2d61 7869 7329 206c  tical (y-axis) l
-000206c0: 6f61 642e 0a0a 2020 2020 5061 7261 6d65  oad...    Parame
-000206d0: 7465 7273 0a20 2020 202d 2d2d 2d2d 2d2d  ters.    -------
-000206e0: 2d2d 2d0a 2020 2020 6c6f 6164 203a 2062  ---.    load : b
-000206f0: 6f6f 6c2c 2064 6566 6175 6c74 3a20 5472  ool, default: Tr
-00020700: 7565 0a20 2020 2020 2020 204c 6f61 6420  ue.        Load 
-00020710: 7468 6520 6461 7461 7365 7420 6166 7465  the dataset afte
-00020720: 7220 646f 776e 6c6f 6164 696e 6720 6974  r downloading it
-00020730: 2077 6865 6e20 6060 5472 7565 6060 2e20   when ``True``. 
-00020740: 2053 6574 2074 6869 730a 2020 2020 2020   Set this.      
-00020750: 2020 746f 2060 6046 616c 7365 6060 2061    to ``False`` a
-00020760: 6e64 206f 6e6c 7920 7468 6520 6669 6c65  nd only the file
-00020770: 6e61 6d65 2077 696c 6c20 6265 2072 6574  name will be ret
-00020780: 7572 6e65 642e 0a0a 2020 2020 5265 7475  urned...    Retu
-00020790: 726e 730a 2020 2020 2d2d 2d2d 2d2d 2d0a  rns.    -------.
-000207a0: 2020 2020 7079 7669 7374 612e 556e 7374      pyvista.Unst
-000207b0: 7275 6374 7572 6564 4772 6964 207c 2073  ructuredGrid | s
-000207c0: 7472 0a20 2020 2020 2020 2044 6174 6153  tr.        DataS
-000207d0: 6574 206f 7220 6669 6c65 6e61 6d65 2064  et or filename d
-000207e0: 6570 656e 6469 6e67 206f 6e20 6060 6c6f  epending on ``lo
-000207f0: 6164 6060 2e0a 0a20 2020 2045 7861 6d70  ad``...    Examp
-00020800: 6c65 730a 2020 2020 2d2d 2d2d 2d2d 2d2d  les.    --------
-00020810: 0a20 2020 2044 6f77 6e6c 6f61 6420 616e  .    Download an
-00020820: 6420 706c 6f74 2065 7175 6976 616c 656e  d plot equivalen
-00020830: 7420 6365 6c6c 2073 7472 6573 732e 0a0a  t cell stress...
-00020840: 2020 2020 3e3e 3e20 6672 6f6d 2070 7976      >>> from pyv
-00020850: 6973 7461 2069 6d70 6f72 7420 6578 616d  ista import exam
-00020860: 706c 6573 0a20 2020 203e 3e3e 2067 7269  ples.    >>> gri
-00020870: 6420 3d20 6578 616d 706c 6573 2e64 6f77  d = examples.dow
-00020880: 6e6c 6f61 645f 6665 615f 6272 6163 6b65  nload_fea_bracke
-00020890: 7428 290a 2020 2020 3e3e 3e20 6772 6964  t().    >>> grid
-000208a0: 2e70 6c6f 7428 290a 0a20 2020 2050 6c6f  .plot()..    Plo
-000208b0: 7420 7468 6520 706f 696e 7420 7374 7265  t the point stre
-000208c0: 7373 2075 7369 6e67 2074 6865 2060 6027  ss using the ``'
-000208d0: 6a65 7427 6060 2063 6f6c 6f72 206d 6170  jet'`` color map
-000208e0: 2e20 436f 6e76 6572 7420 7468 6520 6365  . Convert the ce
-000208f0: 6c6c 2064 6174 610a 2020 2020 746f 2070  ll data.    to p
-00020900: 6f69 6e74 2064 6174 612e 0a0a 2020 2020  oint data...    
-00020910: 3e3e 3e20 6672 6f6d 2070 7976 6973 7461  >>> from pyvista
-00020920: 2069 6d70 6f72 7420 6578 616d 706c 6573   import examples
-00020930: 0a20 2020 203e 3e3e 2067 7269 6420 3d20  .    >>> grid = 
-00020940: 6578 616d 706c 6573 2e64 6f77 6e6c 6f61  examples.downloa
-00020950: 645f 6665 615f 6272 6163 6b65 7428 290a  d_fea_bracket().
-00020960: 2020 2020 3e3e 3e20 6772 6964 203d 2067      >>> grid = g
-00020970: 7269 642e 6365 6c6c 5f64 6174 615f 746f  rid.cell_data_to
-00020980: 5f70 6f69 6e74 5f64 6174 6128 290a 2020  _point_data().  
-00020990: 2020 3e3e 3e20 6772 6964 2e70 6c6f 7428    >>> grid.plot(
-000209a0: 736d 6f6f 7468 5f73 6861 6469 6e67 3d54  smooth_shading=T
-000209b0: 7275 652c 2073 706c 6974 5f73 6861 7270  rue, split_sharp
-000209c0: 5f65 6467 6573 3d54 7275 652c 2063 6d61  _edges=True, cma
-000209d0: 703d 276a 6574 2729 0a0a 2020 2020 2222  p='jet')..    ""
-000209e0: 220a 2020 2020 7265 7475 726e 205f 646f  ".    return _do
-000209f0: 776e 6c6f 6164 5f61 6e64 5f72 6561 6428  wnload_and_read(
-00020a00: 2766 6561 2f6b 6965 6665 722f 6461 7461  'fea/kiefer/data
-00020a10: 7365 742e 7674 7527 2c20 6c6f 6164 3d6c  set.vtu', load=l
-00020a20: 6f61 6429 0a0a 0a64 6566 2064 6f77 6e6c  oad)...def downl
-00020a30: 6f61 645f 6665 615f 6865 7274 7a69 616e  oad_fea_hertzian
-00020a40: 5f63 6f6e 7461 6374 5f63 796c 696e 6465  _contact_cylinde
-00020a50: 7228 6c6f 6164 3d54 7275 6529 3a20 2023  r(load=True):  #
-00020a60: 2070 7261 676d 613a 206e 6f20 636f 7665   pragma: no cove
-00020a70: 720a 2020 2020 2222 2244 6f77 6e6c 6f61  r.    """Downloa
-00020a80: 6420 6120 6865 7274 7a69 616e 2063 6f6e  d a hertzian con
-00020a90: 7461 6374 2066 696e 6974 6520 656c 656d  tact finite elem
-00020aa0: 656e 7420 736f 6c75 7469 6f6e 2e0a 0a20  ent solution... 
-00020ab0: 2020 2048 6572 747a 6961 6e20 636f 6e74     Hertzian cont
-00020ac0: 6163 7420 6973 2072 6566 6572 7265 6420  act is referred 
-00020ad0: 746f 2074 6865 2066 7269 6374 696f 6e6c  to the frictionl
-00020ae0: 6573 7320 636f 6e74 6163 7420 6265 7477  ess contact betw
-00020af0: 6565 6e20 7477 6f0a 2020 2020 626f 6469  een two.    bodi
-00020b00: 6573 2e20 5370 6865 7269 6361 6c20 636f  es. Spherical co
-00020b10: 6e74 6163 7420 6973 2061 2073 7065 6369  ntact is a speci
-00020b20: 616c 2063 6173 6520 6f66 2074 6865 2048  al case of the H
-00020b30: 6572 747a 2063 6f6e 7461 6374 2c20 7768  ertz contact, wh
-00020b40: 6963 6820 6973 0a20 2020 2062 6574 7765  ich is.    betwe
-00020b50: 656e 2074 776f 2073 7068 6572 6573 2c20  en two spheres, 
-00020b60: 6f72 2061 7320 696e 2074 6865 2063 6173  or as in the cas
-00020b70: 6520 6f66 2074 6869 7320 6461 7461 7365  e of this datase
-00020b80: 742c 2062 6574 7765 656e 2061 2073 7068  t, between a sph
-00020b90: 6572 650a 2020 2020 616e 6420 7468 6520  ere.    and the 
-00020ba0: 7375 7266 6163 6520 6f66 2061 2068 616c  surface of a hal
-00020bb0: 6620 7370 6163 6520 2866 6c61 7420 706c  f space (flat pl
-00020bc0: 616e 6529 2e0a 0a20 2020 2050 6172 616d  ane)...    Param
-00020bd0: 6574 6572 730a 2020 2020 2d2d 2d2d 2d2d  eters.    ------
-00020be0: 2d2d 2d2d 0a20 2020 206c 6f61 6420 3a20  ----.    load : 
-00020bf0: 626f 6f6c 2c20 6465 6661 756c 743a 2054  bool, default: T
-00020c00: 7275 650a 2020 2020 2020 2020 4c6f 6164  rue.        Load
-00020c10: 2074 6865 2064 6174 6173 6574 2061 6674   the dataset aft
-00020c20: 6572 2064 6f77 6e6c 6f61 6469 6e67 2069  er downloading i
-00020c30: 7420 7768 656e 2060 6054 7275 6560 602e  t when ``True``.
-00020c40: 2020 5365 7420 7468 6973 0a20 2020 2020    Set this.     
-00020c50: 2020 2074 6f20 6060 4661 6c73 6560 6020     to ``False`` 
-00020c60: 616e 6420 6f6e 6c79 2074 6865 2066 696c  and only the fil
-00020c70: 656e 616d 6520 7769 6c6c 2062 6520 7265  ename will be re
-00020c80: 7475 726e 6564 2e0a 0a20 2020 2052 6574  turned...    Ret
-00020c90: 7572 6e73 0a20 2020 202d 2d2d 2d2d 2d2d  urns.    -------
-00020ca0: 0a20 2020 2070 7976 6973 7461 2e55 6e73  .    pyvista.Uns
-00020cb0: 7472 7563 7475 7265 6447 7269 6420 7c20  tructuredGrid | 
-00020cc0: 7374 720a 2020 2020 2020 2020 4461 7461  str.        Data
-00020cd0: 5365 7420 6f72 2066 696c 656e 616d 6520  Set or filename 
-00020ce0: 6465 7065 6e64 696e 6720 6f6e 2060 606c  depending on ``l
-00020cf0: 6f61 6460 602e 0a0a 2020 2020 4578 616d  oad``...    Exam
-00020d00: 706c 6573 0a20 2020 202d 2d2d 2d2d 2d2d  ples.    -------
-00020d10: 2d0a 2020 2020 506c 6f74 2062 7920 7061  -.    Plot by pa
-00020d20: 7274 2049 442e 0a0a 2020 2020 3e3e 3e20  rt ID...    >>> 
-00020d30: 696d 706f 7274 206e 756d 7079 2061 7320  import numpy as 
-00020d40: 6e70 0a20 2020 203e 3e3e 2069 6d70 6f72  np.    >>> impor
-00020d50: 7420 7079 7669 7374 6120 6173 2070 760a  t pyvista as pv.
-00020d60: 2020 2020 3e3e 3e20 6672 6f6d 2070 7976      >>> from pyv
-00020d70: 6973 7461 2069 6d70 6f72 7420 6578 616d  ista import exam
-00020d80: 706c 6573 0a20 2020 203e 3e3e 2067 7269  ples.    >>> gri
-00020d90: 6420 3d20 6578 616d 706c 6573 2e64 6f77  d = examples.dow
-00020da0: 6e6c 6f61 645f 6665 615f 6865 7274 7a69  nload_fea_hertzi
-00020db0: 616e 5f63 6f6e 7461 6374 5f63 796c 696e  an_contact_cylin
-00020dc0: 6465 7228 290a 2020 2020 3e3e 3e20 6772  der().    >>> gr
-00020dd0: 6964 2e70 6c6f 7428 0a20 2020 202e 2e2e  id.plot(.    ...
-00020de0: 2020 2020 2073 6361 6c61 7273 3d27 5061       scalars='Pa
-00020df0: 7274 4944 272c 2063 6d61 703d 5b27 6772  rtID', cmap=['gr
-00020e00: 6565 6e27 2c20 2762 6c75 6527 5d2c 2073  een', 'blue'], s
-00020e10: 686f 775f 7363 616c 6172 5f62 6172 3d46  how_scalar_bar=F
-00020e20: 616c 7365 0a20 2020 202e 2e2e 2029 0a0a  alse.    ... )..
-00020e30: 2020 2020 506c 6f74 2074 6865 2061 6273      Plot the abs
-00020e40: 6f6c 7574 6520 7661 6c75 6520 6f66 2074  olute value of t
-00020e50: 6865 2063 6f6d 706f 6e65 6e74 2073 7472  he component str
-00020e60: 6573 7320 696e 2074 6865 205a 2064 6972  ess in the Z dir
-00020e70: 6563 7469 6f6e 2e0a 0a20 2020 203e 3e3e  ection...    >>>
-00020e80: 2070 6c20 3d20 7076 2e50 6c6f 7474 6572   pl = pv.Plotter
-00020e90: 2829 0a20 2020 203e 3e3e 207a 5f73 7472  ().    >>> z_str
-00020ea0: 6573 7320 3d20 6e70 2e61 6273 2867 7269  ess = np.abs(gri
-00020eb0: 645b 2753 7472 6573 7327 5d5b 3a2c 2032  d['Stress'][:, 2
-00020ec0: 5d29 0a20 2020 203e 3e3e 205f 203d 2070  ]).    >>> _ = p
-00020ed0: 6c2e 6164 645f 6d65 7368 280a 2020 2020  l.add_mesh(.    
-00020ee0: 2e2e 2e20 2020 2020 6772 6964 2c0a 2020  ...     grid,.  
-00020ef0: 2020 2e2e 2e20 2020 2020 7363 616c 6172    ...     scalar
-00020f00: 733d 7a5f 7374 7265 7373 2c0a 2020 2020  s=z_stress,.    
-00020f10: 2e2e 2e20 2020 2020 636c 696d 3d5b 302c  ...     clim=[0,
-00020f20: 2031 2e32 6539 5d2c 0a20 2020 202e 2e2e   1.2e9],.    ...
-00020f30: 2020 2020 2063 6d61 703d 276a 6574 272c       cmap='jet',
-00020f40: 0a20 2020 202e 2e2e 2020 2020 206c 6967  .    ...     lig
-00020f50: 6874 696e 673d 5472 7565 2c0a 2020 2020  hting=True,.    
-00020f60: 2e2e 2e20 2020 2020 7368 6f77 5f65 6467  ...     show_edg
-00020f70: 6573 3d46 616c 7365 2c0a 2020 2020 2e2e  es=False,.    ..
-00020f80: 2e20 2020 2020 616d 6269 656e 743d 302e  .     ambient=0.
-00020f90: 322c 0a20 2020 202e 2e2e 2029 0a20 2020  2,.    ... ).   
-00020fa0: 203e 3e3e 2070 6c2e 6361 6d65 7261 5f70   >>> pl.camera_p
-00020fb0: 6f73 6974 696f 6e20 3d20 2778 7a27 0a20  osition = 'xz'. 
-00020fc0: 2020 203e 3e3e 2070 6c2e 6361 6d65 7261     >>> pl.camera
-00020fd0: 2e7a 6f6f 6d28 312e 3429 0a20 2020 203e  .zoom(1.4).    >
-00020fe0: 3e3e 2070 6c2e 7368 6f77 2829 0a0a 2020  >> pl.show()..  
-00020ff0: 2020 2222 220a 2020 2020 6669 6c65 6e61    """.    filena
-00021000: 6d65 203d 205f 646f 776e 6c6f 6164 5f61  me = _download_a
-00021010: 7263 6869 7665 280a 2020 2020 2020 2020  rchive(.        
-00021020: 2766 6561 2f68 6572 747a 6961 6e5f 636f  'fea/hertzian_co
-00021030: 6e74 6163 745f 6379 6c69 6e64 6572 2f48  ntact_cylinder/H
-00021040: 6572 747a 6961 6e5f 6379 6c69 6e64 6572  ertzian_cylinder
-00021050: 5f6f 6e5f 706c 6174 652e 7a69 7027 2c0a  _on_plate.zip',.
-00021060: 2020 2020 2020 2020 7461 7267 6574 5f66          target_f
-00021070: 696c 653d 2762 6661 6339 6664 312d 6539  ile='bfac9fd1-e9
-00021080: 3832 2d34 3832 352d 3961 3935 2d39 6535  82-4825-9a95-9e5
-00021090: 6438 6335 6234 6433 655f 7265 7375 6c74  d8c5b4d3e_result
-000210a0: 5f31 2e70 7674 7527 2c0a 2020 2020 290a  _1.pvtu',.    ).
-000210b0: 2020 2020 6966 206c 6f61 643a 0a20 2020      if load:.   
-000210c0: 2020 2020 2072 6574 7572 6e20 7079 7669       return pyvi
-000210d0: 7374 612e 7265 6164 2866 696c 656e 616d  sta.read(filenam
-000210e0: 6529 0a20 2020 2072 6574 7572 6e20 6669  e).    return fi
-000210f0: 6c65 6e61 6d65 0a0a 0a64 6566 2064 6f77  lename...def dow
-00021100: 6e6c 6f61 645f 626c 6163 6b5f 7661 7365  nload_black_vase
-00021110: 286c 6f61 643d 5472 7565 293a 2020 2320  (load=True):  # 
-00021120: 7072 6167 6d61 3a20 6e6f 2063 6f76 6572  pragma: no cover
-00021130: 0a20 2020 2022 2222 446f 776e 6c6f 6164  .    """Download
-00021140: 2061 2062 6c61 636b 2076 6173 6520 7363   a black vase sc
-00021150: 616e 2063 7265 6174 6564 2062 7920 4976  an created by Iv
-00021160: 616e 204e 696b 6f6c 6f76 2e0a 0a20 2020  an Nikolov...   
-00021170: 2054 6865 2064 6174 6173 6574 2077 6173   The dataset was
-00021180: 2064 6f77 6e6c 6f61 6465 6420 6672 6f6d   downloaded from
-00021190: 2060 4747 472d 4265 6e63 686d 6172 6b53   `GGG-BenchmarkS
-000211a0: 664d 3a20 4461 7461 7365 7420 666f 7220  fM: Dataset for 
-000211b0: 4265 6e63 686d 6172 6b69 6e67 0a20 2020  Benchmarking.   
-000211c0: 2043 6c6f 7365 2d72 616e 6765 2053 664d   Close-range SfM
-000211d0: 2053 6f66 7477 6172 6520 5065 7266 6f72   Software Perfor
-000211e0: 6d61 6e63 6520 756e 6465 7220 5661 7279  mance under Vary
-000211f0: 696e 6720 4361 7074 7572 696e 6720 436f  ing Capturing Co
-00021200: 6e64 6974 696f 6e73 0a20 2020 203c 6874  nditions.    <ht
-00021210: 7470 733a 2f2f 6461 7461 2e6d 656e 6465  tps://data.mende
-00021220: 6c65 792e 636f 6d2f 6461 7461 7365 7473  ley.com/datasets
-00021230: 2f62 7a78 6b32 6e37 3873 392f 343e 605f  /bzxk2n78s9/4>`_
-00021240: 0a0a 2020 2020 4f72 6967 696e 616c 2064  ..    Original d
-00021250: 6174 6173 6574 7320 6172 6520 756e 6465  atasets are unde
-00021260: 7220 7468 6520 4343 2042 5920 342e 3020  r the CC BY 4.0 
-00021270: 6c69 6365 6e73 652e 0a0a 2020 2020 466f  license...    Fo
-00021280: 7220 6d6f 7265 2064 6574 6169 6c73 2c20  r more details, 
-00021290: 7365 6520 6049 7661 6e20 4e69 6b6f 6c6f  see `Ivan Nikolo
-000212a0: 7620 4461 7461 7365 7473 0a20 2020 203c  v Datasets.    <
-000212b0: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
-000212c0: 6f6d 2f70 7976 6973 7461 2f76 746b 2d64  om/pyvista/vtk-d
-000212d0: 6174 612f 7472 6565 2f6d 6173 7465 722f  ata/tree/master/
-000212e0: 4461 7461 2f69 7661 6e2d 6e69 6b6f 6c6f  Data/ivan-nikolo
-000212f0: 763e 605f 0a0a 2020 2020 5061 7261 6d65  v>`_..    Parame
-00021300: 7465 7273 0a20 2020 202d 2d2d 2d2d 2d2d  ters.    -------
-00021310: 2d2d 2d0a 2020 2020 6c6f 6164 203a 2062  ---.    load : b
-00021320: 6f6f 6c2c 2064 6566 6175 6c74 3a20 5472  ool, default: Tr
-00021330: 7565 0a20 2020 2020 2020 204c 6f61 6420  ue.        Load 
-00021340: 7468 6520 6461 7461 7365 7420 6166 7465  the dataset afte
-00021350: 7220 646f 776e 6c6f 6164 696e 6720 6974  r downloading it
-00021360: 2077 6865 6e20 6060 5472 7565 6060 2e20   when ``True``. 
-00021370: 2053 6574 2074 6869 730a 2020 2020 2020   Set this.      
-00021380: 2020 746f 2060 6046 616c 7365 6060 2061    to ``False`` a
-00021390: 6e64 206f 6e6c 7920 7468 6520 6669 6c65  nd only the file
-000213a0: 6e61 6d65 2077 696c 6c20 6265 2072 6574  name will be ret
-000213b0: 7572 6e65 642e 0a0a 2020 2020 5265 7475  urned...    Retu
-000213c0: 726e 730a 2020 2020 2d2d 2d2d 2d2d 2d0a  rns.    -------.
-000213d0: 2020 2020 7079 7669 7374 612e 506f 6c79      pyvista.Poly
-000213e0: 4461 7461 207c 2073 7472 0a20 2020 2020  Data | str.     
-000213f0: 2020 2044 6174 6153 6574 206f 7220 6669     DataSet or fi
-00021400: 6c65 6e61 6d65 2064 6570 656e 6469 6e67  lename depending
-00021410: 206f 6e20 6060 6c6f 6164 6060 2e0a 0a20   on ``load``... 
-00021420: 2020 2045 7861 6d70 6c65 730a 2020 2020     Examples.    
-00021430: 2d2d 2d2d 2d2d 2d2d 0a20 2020 2044 6f77  --------.    Dow
-00021440: 6e6c 6f61 6420 616e 6420 706c 6f74 2074  nload and plot t
-00021450: 6865 2064 6174 6173 6574 2e0a 0a20 2020  he dataset...   
-00021460: 203e 3e3e 2066 726f 6d20 7079 7669 7374   >>> from pyvist
-00021470: 6120 696d 706f 7274 2065 7861 6d70 6c65  a import example
-00021480: 730a 2020 2020 3e3e 3e20 6d65 7368 203d  s.    >>> mesh =
-00021490: 2065 7861 6d70 6c65 732e 646f 776e 6c6f   examples.downlo
-000214a0: 6164 5f62 6c61 636b 5f76 6173 6528 290a  ad_black_vase().
-000214b0: 2020 2020 3e3e 3e20 6d65 7368 2e70 6c6f      >>> mesh.plo
-000214c0: 7428 290a 0a20 2020 2052 6574 7572 6e20  t()..    Return 
-000214d0: 7468 6520 7374 6174 6973 7469 6373 206f  the statistics o
-000214e0: 6620 7468 6520 6461 7461 7365 742e 0a0a  f the dataset...
-000214f0: 2020 2020 3e3e 3e20 6d65 7368 0a20 2020      >>> mesh.   
-00021500: 2050 6f6c 7944 6174 6120 282e 2e2e 290a   PolyData (...).
-00021510: 2020 2020 2020 4e20 4365 6c6c 733a 2020        N Cells:  
-00021520: 2020 3331 3336 3635 320a 2020 2020 2020    3136652.      
-00021530: 4e20 506f 696e 7473 3a20 2020 3136 3131  N Points:   1611
-00021540: 3738 390a 2020 2020 2020 4e20 5374 7269  789.      N Stri
-00021550: 7073 3a20 2020 300a 2020 2020 2020 5820  ps:   0.      X 
-00021560: 426f 756e 6473 3a20 2020 2d31 2e30 3932  Bounds:   -1.092
-00021570: 652b 3032 2c20 312e 3533 3365 2b30 320a  e+02, 1.533e+02.
-00021580: 2020 2020 2020 5920 426f 756e 6473 3a20        Y Bounds: 
-00021590: 2020 2d31 2e32 3030 652b 3032 2c20 312e    -1.200e+02, 1.
-000215a0: 3431 3565 2b30 320a 2020 2020 2020 5a20  415e+02.      Z 
-000215b0: 426f 756e 6473 3a20 2020 312e 3636 3665  Bounds:   1.666e
-000215c0: 2b30 312c 2034 2e30 3737 652b 3032 0a20  +01, 4.077e+02. 
-000215d0: 2020 2020 204e 2041 7272 6179 733a 2020       N Arrays:  
-000215e0: 2030 0a0a 0a20 2020 2022 2222 0a20 2020   0...    """.   
-000215f0: 2066 696c 656e 616d 6520 3d20 5f64 6f77   filename = _dow
-00021600: 6e6c 6f61 645f 6172 6368 6976 6528 0a20  nload_archive(. 
-00021610: 2020 2020 2020 2027 6976 616e 2d6e 696b         'ivan-nik
-00021620: 6f6c 6f76 2f62 6c61 636b 5661 7365 2e7a  olov/blackVase.z
-00021630: 6970 272c 0a20 2020 2020 2020 2027 626c  ip',.        'bl
-00021640: 6163 6b56 6173 652e 7674 7027 2c0a 2020  ackVase.vtp',.  
-00021650: 2020 290a 2020 2020 6966 206c 6f61 643a    ).    if load:
-00021660: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
-00021670: 7079 7669 7374 612e 7265 6164 2866 696c  pyvista.read(fil
-00021680: 656e 616d 6529 0a20 2020 2072 6574 7572  ename).    retur
-00021690: 6e20 6669 6c65 6e61 6d65 0a0a 0a64 6566  n filename...def
-000216a0: 2064 6f77 6e6c 6f61 645f 6976 616e 5f61   download_ivan_a
-000216b0: 6e67 656c 286c 6f61 643d 5472 7565 293a  ngel(load=True):
-000216c0: 2020 2320 7072 6167 6d61 3a20 6e6f 2063    # pragma: no c
-000216d0: 6f76 6572 0a20 2020 2022 2222 446f 776e  over.    """Down
-000216e0: 6c6f 6164 2061 2073 6361 6e20 6f66 2061  load a scan of a
-000216f0: 6e20 616e 6765 6c20 7374 6174 7565 2063  n angel statue c
-00021700: 7265 6174 6564 2062 7920 4976 616e 204e  reated by Ivan N
-00021710: 696b 6f6c 6f76 2e0a 0a20 2020 2054 6865  ikolov...    The
-00021720: 2064 6174 6173 6574 2077 6173 2064 6f77   dataset was dow
-00021730: 6e6c 6f61 6465 6420 6672 6f6d 2060 4747  nloaded from `GG
-00021740: 472d 4265 6e63 686d 6172 6b53 664d 3a20  G-BenchmarkSfM: 
-00021750: 4461 7461 7365 7420 666f 7220 4265 6e63  Dataset for Benc
-00021760: 686d 6172 6b69 6e67 0a20 2020 2043 6c6f  hmarking.    Clo
-00021770: 7365 2d72 616e 6765 2053 664d 2053 6f66  se-range SfM Sof
-00021780: 7477 6172 6520 5065 7266 6f72 6d61 6e63  tware Performanc
-00021790: 6520 756e 6465 7220 5661 7279 696e 6720  e under Varying 
-000217a0: 4361 7074 7572 696e 6720 436f 6e64 6974  Capturing Condit
-000217b0: 696f 6e73 0a20 2020 203c 6874 7470 733a  ions.    <https:
-000217c0: 2f2f 6461 7461 2e6d 656e 6465 6c65 792e  //data.mendeley.
-000217d0: 636f 6d2f 6461 7461 7365 7473 2f62 7a78  com/datasets/bzx
-000217e0: 6b32 6e37 3873 392f 343e 605f 0a0a 2020  k2n78s9/4>`_..  
-000217f0: 2020 4f72 6967 696e 616c 2064 6174 6173    Original datas
-00021800: 6574 7320 6172 6520 756e 6465 7220 7468  ets are under th
-00021810: 6520 4343 2042 5920 342e 3020 6c69 6365  e CC BY 4.0 lice
-00021820: 6e73 652e 0a0a 2020 2020 466f 7220 6d6f  nse...    For mo
-00021830: 7265 2064 6574 6169 6c73 2c20 7365 6520  re details, see 
-00021840: 6049 7661 6e20 4e69 6b6f 6c6f 7620 4461  `Ivan Nikolov Da
-00021850: 7461 7365 7473 0a20 2020 203c 6874 7470  tasets.    <http
-00021860: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f70  s://github.com/p
-00021870: 7976 6973 7461 2f76 746b 2d64 6174 612f  yvista/vtk-data/
-00021880: 7472 6565 2f6d 6173 7465 722f 4461 7461  tree/master/Data
-00021890: 2f69 7661 6e2d 6e69 6b6f 6c6f 763e 605f  /ivan-nikolov>`_
-000218a0: 0a0a 2020 2020 5061 7261 6d65 7465 7273  ..    Parameters
-000218b0: 0a20 2020 202d 2d2d 2d2d 2d2d 2d2d 2d0a  .    ----------.
-000218c0: 2020 2020 6c6f 6164 203a 2062 6f6f 6c2c      load : bool,
-000218d0: 2064 6566 6175 6c74 3a20 5472 7565 0a20   default: True. 
-000218e0: 2020 2020 2020 204c 6f61 6420 7468 6520         Load the 
-000218f0: 6461 7461 7365 7420 6166 7465 7220 646f  dataset after do
-00021900: 776e 6c6f 6164 696e 6720 6974 2077 6865  wnloading it whe
-00021910: 6e20 6060 5472 7565 6060 2e20 2053 6574  n ``True``.  Set
-00021920: 2074 6869 730a 2020 2020 2020 2020 746f   this.        to
-00021930: 2060 6046 616c 7365 6060 2061 6e64 206f   ``False`` and o
-00021940: 6e6c 7920 7468 6520 6669 6c65 6e61 6d65  nly the filename
-00021950: 2077 696c 6c20 6265 2072 6574 7572 6e65   will be returne
-00021960: 642e 0a0a 2020 2020 5265 7475 726e 730a  d...    Returns.
-00021970: 2020 2020 2d2d 2d2d 2d2d 2d0a 2020 2020      -------.    
-00021980: 7079 7669 7374 612e 506f 6c79 4461 7461  pyvista.PolyData
-00021990: 207c 2073 7472 0a20 2020 2020 2020 2044   | str.        D
-000219a0: 6174 6153 6574 206f 7220 6669 6c65 6e61  ataSet or filena
-000219b0: 6d65 2064 6570 656e 6469 6e67 206f 6e20  me depending on 
-000219c0: 6060 6c6f 6164 6060 2e0a 0a20 2020 2045  ``load``...    E
-000219d0: 7861 6d70 6c65 730a 2020 2020 2d2d 2d2d  xamples.    ----
-000219e0: 2d2d 2d2d 0a20 2020 2044 6f77 6e6c 6f61  ----.    Downloa
-000219f0: 6420 616e 6420 706c 6f74 2074 6865 2064  d and plot the d
-00021a00: 6174 6173 6574 2e0a 0a20 2020 203e 3e3e  ataset...    >>>
-00021a10: 2066 726f 6d20 7079 7669 7374 6120 696d   from pyvista im
-00021a20: 706f 7274 2065 7861 6d70 6c65 730a 2020  port examples.  
-00021a30: 2020 3e3e 3e20 6d65 7368 203d 2065 7861    >>> mesh = exa
-00021a40: 6d70 6c65 732e 646f 776e 6c6f 6164 5f69  mples.download_i
-00021a50: 7661 6e5f 616e 6765 6c28 290a 2020 2020  van_angel().    
-00021a60: 3e3e 3e20 6370 6f73 203d 205b 0a20 2020  >>> cpos = [.   
-00021a70: 202e 2e2e 2020 2020 2028 2d34 3736 2e31   ...     (-476.1
-00021a80: 342c 202d 3339 332e 3733 2c20 3238 322e  4, -393.73, 282.
-00021a90: 3134 292c 0a20 2020 202e 2e2e 2020 2020  14),.    ...    
-00021aa0: 2028 2d31 352e 3030 2c20 3131 2e32 352c   (-15.00, 11.25,
-00021ab0: 2034 342e 3038 292c 0a20 2020 202e 2e2e   44.08),.    ...
-00021ac0: 2020 2020 2028 302e 3236 2c20 302e 3234       (0.26, 0.24
-00021ad0: 2c20 302e 3933 292c 0a20 2020 202e 2e2e  , 0.93),.    ...
-00021ae0: 205d 0a20 2020 203e 3e3e 206d 6573 682e   ].    >>> mesh.
-00021af0: 706c 6f74 2863 706f 733d 6370 6f73 290a  plot(cpos=cpos).
-00021b00: 0a20 2020 2052 6574 7572 6e20 7468 6520  .    Return the 
-00021b10: 7374 6174 6973 7469 6373 206f 6620 7468  statistics of th
-00021b20: 6520 6461 7461 7365 742e 0a0a 2020 2020  e dataset...    
-00021b30: 3e3e 3e20 6d65 7368 0a20 2020 2050 6f6c  >>> mesh.    Pol
-00021b40: 7944 6174 6120 282e 2e2e 290a 2020 2020  yData (...).    
-00021b50: 2020 4e20 4365 6c6c 733a 2020 2020 3335    N Cells:    35
-00021b60: 3830 3435 340a 2020 2020 2020 4e20 506f  80454.      N Po
-00021b70: 696e 7473 3a20 2020 3138 3131 3533 310a  ints:   1811531.
-00021b80: 2020 2020 2020 4e20 5374 7269 7073 3a20        N Strips: 
-00021b90: 2020 300a 2020 2020 2020 5820 426f 756e    0.      X Boun
-00021ba0: 6473 3a20 2020 2d31 2e31 3437 652b 3032  ds:   -1.147e+02
-00021bb0: 2c20 382e 3436 3865 2b30 310a 2020 2020  , 8.468e+01.    
-00021bc0: 2020 5920 426f 756e 6473 3a20 2020 2d36    Y Bounds:   -6
-00021bd0: 2e39 3936 652b 3031 2c20 392e 3234 3765  .996e+01, 9.247e
-00021be0: 2b30 310a 2020 2020 2020 5a20 426f 756e  +01.      Z Boun
-00021bf0: 6473 3a20 2020 2d31 2e31 3731 652b 3032  ds:   -1.171e+02
-00021c00: 2c20 322e 3035 3265 2b30 320a 2020 2020  , 2.052e+02.    
-00021c10: 2020 4e20 4172 7261 7973 3a20 2020 300a    N Arrays:   0.
-00021c20: 0a20 2020 2022 2222 0a20 2020 2066 696c  .    """.    fil
-00021c30: 656e 616d 6520 3d20 5f64 6f77 6e6c 6f61  ename = _downloa
-00021c40: 645f 6172 6368 6976 6528 0a20 2020 2020  d_archive(.     
-00021c50: 2020 2027 6976 616e 2d6e 696b 6f6c 6f76     'ivan-nikolov
-00021c60: 2f41 6e67 656c 2e7a 6970 272c 0a20 2020  /Angel.zip',.   
-00021c70: 2020 2020 2027 416e 6765 6c2e 7674 7027       'Angel.vtp'
-00021c80: 2c0a 2020 2020 290a 2020 2020 6966 206c  ,.    ).    if l
-00021c90: 6f61 643a 0a20 2020 2020 2020 2072 6574  oad:.        ret
-00021ca0: 7572 6e20 7079 7669 7374 612e 7265 6164  urn pyvista.read
-00021cb0: 2866 696c 656e 616d 6529 0a20 2020 2072  (filename).    r
-00021cc0: 6574 7572 6e20 6669 6c65 6e61 6d65 0a0a  eturn filename..
-00021cd0: 0a64 6566 2064 6f77 6e6c 6f61 645f 6269  .def download_bi
-00021ce0: 7264 5f62 6174 6828 6c6f 6164 3d54 7275  rd_bath(load=Tru
-00021cf0: 6529 3a20 2023 2070 7261 676d 613a 206e  e):  # pragma: n
-00021d00: 6f20 636f 7665 720a 2020 2020 2222 2244  o cover.    """D
-00021d10: 6f77 6e6c 6f61 6420 6120 7363 616e 206f  ownload a scan o
-00021d20: 6620 6120 6269 7264 2062 6174 6820 6372  f a bird bath cr
-00021d30: 6561 7465 6420 6279 2049 7661 6e20 4e69  eated by Ivan Ni
-00021d40: 6b6f 6c6f 762e 0a0a 2020 2020 5468 6520  kolov...    The 
-00021d50: 6461 7461 7365 7420 7761 7320 646f 776e  dataset was down
-00021d60: 6c6f 6164 6564 2066 726f 6d20 6047 4747  loaded from `GGG
-00021d70: 2d42 656e 6368 6d61 726b 5366 4d3a 2044  -BenchmarkSfM: D
-00021d80: 6174 6173 6574 2066 6f72 2042 656e 6368  ataset for Bench
-00021d90: 6d61 726b 696e 670a 2020 2020 436c 6f73  marking.    Clos
-00021da0: 652d 7261 6e67 6520 5366 4d20 536f 6674  e-range SfM Soft
-00021db0: 7761 7265 2050 6572 666f 726d 616e 6365  ware Performance
-00021dc0: 2075 6e64 6572 2056 6172 7969 6e67 2043   under Varying C
-00021dd0: 6170 7475 7269 6e67 2043 6f6e 6469 7469  apturing Conditi
-00021de0: 6f6e 730a 2020 2020 3c68 7474 7073 3a2f  ons.    <https:/
-00021df0: 2f64 6174 612e 6d65 6e64 656c 6579 2e63  /data.mendeley.c
-00021e00: 6f6d 2f64 6174 6173 6574 732f 627a 786b  om/datasets/bzxk
-00021e10: 326e 3738 7339 2f34 3e60 5f0a 0a20 2020  2n78s9/4>`_..   
-00021e20: 204f 7269 6769 6e61 6c20 6461 7461 7365   Original datase
-00021e30: 7473 2061 7265 2075 6e64 6572 2074 6865  ts are under the
-00021e40: 2043 4320 4259 2034 2e30 206c 6963 656e   CC BY 4.0 licen
-00021e50: 7365 2e0a 0a20 2020 2046 6f72 206d 6f72  se...    For mor
-00021e60: 6520 6465 7461 696c 732c 2073 6565 2060  e details, see `
-00021e70: 4976 616e 204e 696b 6f6c 6f76 2044 6174  Ivan Nikolov Dat
-00021e80: 6173 6574 730a 2020 2020 3c68 7474 7073  asets.    <https
-00021e90: 3a2f 2f67 6974 6875 622e 636f 6d2f 7079  ://github.com/py
-00021ea0: 7669 7374 612f 7674 6b2d 6461 7461 2f74  vista/vtk-data/t
-00021eb0: 7265 652f 6d61 7374 6572 2f44 6174 612f  ree/master/Data/
-00021ec0: 6976 616e 2d6e 696b 6f6c 6f76 3e60 5f0a  ivan-nikolov>`_.
-00021ed0: 0a20 2020 2050 6172 616d 6574 6572 730a  .    Parameters.
-00021ee0: 2020 2020 2d2d 2d2d 2d2d 2d2d 2d2d 0a20      ----------. 
-00021ef0: 2020 206c 6f61 6420 3a20 626f 6f6c 2c20     load : bool, 
-00021f00: 6465 6661 756c 743a 2054 7275 650a 2020  default: True.  
-00021f10: 2020 2020 2020 4c6f 6164 2074 6865 2064        Load the d
-00021f20: 6174 6173 6574 2061 6674 6572 2064 6f77  ataset after dow
-00021f30: 6e6c 6f61 6469 6e67 2069 7420 7768 656e  nloading it when
-00021f40: 2060 6054 7275 6560 602e 2020 5365 7420   ``True``.  Set 
-00021f50: 7468 6973 0a20 2020 2020 2020 2074 6f20  this.        to 
-00021f60: 6060 4661 6c73 6560 6020 616e 6420 6f6e  ``False`` and on
-00021f70: 6c79 2074 6865 2066 696c 656e 616d 6520  ly the filename 
-00021f80: 7769 6c6c 2062 6520 7265 7475 726e 6564  will be returned
-00021f90: 2e0a 0a20 2020 2052 6574 7572 6e73 0a20  ...    Returns. 
-00021fa0: 2020 202d 2d2d 2d2d 2d2d 0a20 2020 2070     -------.    p
-00021fb0: 7976 6973 7461 2e50 6f6c 7944 6174 6120  yvista.PolyData 
-00021fc0: 7c20 7374 720a 2020 2020 2020 2020 4461  | str.        Da
-00021fd0: 7461 5365 7420 6f72 2066 696c 656e 616d  taSet or filenam
-00021fe0: 6520 6465 7065 6e64 696e 6720 6f6e 2060  e depending on `
-00021ff0: 606c 6f61 6460 602e 0a0a 2020 2020 4578  `load``...    Ex
-00022000: 616d 706c 6573 0a20 2020 202d 2d2d 2d2d  amples.    -----
-00022010: 2d2d 2d0a 2020 2020 446f 776e 6c6f 6164  ---.    Download
-00022020: 2061 6e64 2070 6c6f 7420 7468 6520 6461   and plot the da
-00022030: 7461 7365 742e 0a0a 2020 2020 3e3e 3e20  taset...    >>> 
-00022040: 6672 6f6d 2070 7976 6973 7461 2069 6d70  from pyvista imp
-00022050: 6f72 7420 6578 616d 706c 6573 0a20 2020  ort examples.   
-00022060: 203e 3e3e 206d 6573 6820 3d20 6578 616d   >>> mesh = exam
-00022070: 706c 6573 2e64 6f77 6e6c 6f61 645f 6269  ples.download_bi
-00022080: 7264 5f62 6174 6828 290a 2020 2020 3e3e  rd_bath().    >>
-00022090: 3e20 6d65 7368 2e70 6c6f 7428 290a 0a20  > mesh.plot().. 
-000220a0: 2020 2052 6574 7572 6e20 7468 6520 7374     Return the st
-000220b0: 6174 6973 7469 6373 206f 6620 7468 6520  atistics of the 
-000220c0: 6461 7461 7365 742e 0a0a 2020 2020 3e3e  dataset...    >>
-000220d0: 3e20 6d65 7368 0a20 2020 2050 6f6c 7944  > mesh.    PolyD
-000220e0: 6174 6120 282e 2e2e 290a 2020 2020 2020  ata (...).      
-000220f0: 4e20 4365 6c6c 733a 2020 2020 3335 3037  N Cells:    3507
-00022100: 3933 350a 2020 2020 2020 4e20 506f 696e  935.      N Poin
-00022110: 7473 3a20 2020 3138 3331 3338 330a 2020  ts:   1831383.  
-00022120: 2020 2020 4e20 5374 7269 7073 3a20 2020      N Strips:   
-00022130: 300a 2020 2020 2020 5820 426f 756e 6473  0.      X Bounds
-00022140: 3a20 2020 2d31 2e36 3031 652b 3032 2c20  :   -1.601e+02, 
-00022150: 312e 3438 3365 2b30 320a 2020 2020 2020  1.483e+02.      
-00022160: 5920 426f 756e 6473 3a20 2020 2d31 2e35  Y Bounds:   -1.5
-00022170: 3231 652b 3032 2c20 312e 3534 3765 2b30  21e+02, 1.547e+0
-00022180: 320a 2020 2020 2020 5a20 426f 756e 6473  2.      Z Bounds
-00022190: 3a20 2020 2d34 2e32 3431 652b 3030 2c20  :   -4.241e+00, 
-000221a0: 312e 3430 3965 2b30 320a 2020 2020 2020  1.409e+02.      
-000221b0: 4e20 4172 7261 7973 3a20 2020 300a 0a20  N Arrays:   0.. 
-000221c0: 2020 2022 2222 0a20 2020 2066 696c 656e     """.    filen
-000221d0: 616d 6520 3d20 5f64 6f77 6e6c 6f61 645f  ame = _download_
-000221e0: 6172 6368 6976 6528 0a20 2020 2020 2020  archive(.       
-000221f0: 2027 6976 616e 2d6e 696b 6f6c 6f76 2f62   'ivan-nikolov/b
-00022200: 6972 6442 6174 682e 7a69 7027 2c0a 2020  irdBath.zip',.  
-00022210: 2020 2020 2020 2762 6972 6442 6174 682e        'birdBath.
-00022220: 7674 7027 2c0a 2020 2020 290a 2020 2020  vtp',.    ).    
-00022230: 6966 206c 6f61 643a 0a20 2020 2020 2020  if load:.       
-00022240: 2072 6574 7572 6e20 7079 7669 7374 612e   return pyvista.
-00022250: 7265 6164 2866 696c 656e 616d 6529 0a20  read(filename). 
-00022260: 2020 2072 6574 7572 6e20 6669 6c65 6e61     return filena
-00022270: 6d65 0a0a 0a64 6566 2064 6f77 6e6c 6f61  me...def downloa
-00022280: 645f 6f77 6c28 6c6f 6164 3d54 7275 6529  d_owl(load=True)
-00022290: 3a20 2023 2070 7261 676d 613a 206e 6f20  :  # pragma: no 
-000222a0: 636f 7665 720a 2020 2020 2222 2244 6f77  cover.    """Dow
-000222b0: 6e6c 6f61 6420 6120 7363 616e 206f 6620  nload a scan of 
-000222c0: 616e 206f 776c 2073 7461 7475 6520 6372  an owl statue cr
-000222d0: 6561 7465 6420 6279 2049 7661 6e20 4e69  eated by Ivan Ni
-000222e0: 6b6f 6c6f 762e 0a0a 2020 2020 5468 6520  kolov...    The 
-000222f0: 6461 7461 7365 7420 7761 7320 646f 776e  dataset was down
-00022300: 6c6f 6164 6564 2066 726f 6d20 6047 4747  loaded from `GGG
-00022310: 2d42 656e 6368 6d61 726b 5366 4d3a 2044  -BenchmarkSfM: D
-00022320: 6174 6173 6574 2066 6f72 2042 656e 6368  ataset for Bench
-00022330: 6d61 726b 696e 670a 2020 2020 436c 6f73  marking.    Clos
-00022340: 652d 7261 6e67 6520 5366 4d20 536f 6674  e-range SfM Soft
-00022350: 7761 7265 2050 6572 666f 726d 616e 6365  ware Performance
-00022360: 2075 6e64 6572 2056 6172 7969 6e67 2043   under Varying C
-00022370: 6170 7475 7269 6e67 2043 6f6e 6469 7469  apturing Conditi
-00022380: 6f6e 730a 2020 2020 3c68 7474 7073 3a2f  ons.    <https:/
-00022390: 2f64 6174 612e 6d65 6e64 656c 6579 2e63  /data.mendeley.c
-000223a0: 6f6d 2f64 6174 6173 6574 732f 627a 786b  om/datasets/bzxk
-000223b0: 326e 3738 7339 2f34 3e60 5f0a 0a20 2020  2n78s9/4>`_..   
-000223c0: 204f 7269 6769 6e61 6c20 6461 7461 7365   Original datase
-000223d0: 7473 2061 7265 2075 6e64 6572 2074 6865  ts are under the
-000223e0: 2043 4320 4259 2034 2e30 206c 6963 656e   CC BY 4.0 licen
-000223f0: 7365 2e0a 0a20 2020 2046 6f72 206d 6f72  se...    For mor
-00022400: 6520 6465 7461 696c 732c 2073 6565 2060  e details, see `
-00022410: 4976 616e 204e 696b 6f6c 6f76 2044 6174  Ivan Nikolov Dat
-00022420: 6173 6574 730a 2020 2020 3c68 7474 7073  asets.    <https
-00022430: 3a2f 2f67 6974 6875 622e 636f 6d2f 7079  ://github.com/py
-00022440: 7669 7374 612f 7674 6b2d 6461 7461 2f74  vista/vtk-data/t
-00022450: 7265 652f 6d61 7374 6572 2f44 6174 612f  ree/master/Data/
-00022460: 6976 616e 2d6e 696b 6f6c 6f76 3e60 5f0a  ivan-nikolov>`_.
-00022470: 0a20 2020 2050 6172 616d 6574 6572 730a  .    Parameters.
-00022480: 2020 2020 2d2d 2d2d 2d2d 2d2d 2d2d 0a20      ----------. 
-00022490: 2020 206c 6f61 6420 3a20 626f 6f6c 2c20     load : bool, 
-000224a0: 6465 6661 756c 743a 2054 7275 650a 2020  default: True.  
-000224b0: 2020 2020 2020 4c6f 6164 2074 6865 2064        Load the d
-000224c0: 6174 6173 6574 2061 6674 6572 2064 6f77  ataset after dow
-000224d0: 6e6c 6f61 6469 6e67 2069 7420 7768 656e  nloading it when
-000224e0: 2060 6054 7275 6560 602e 2020 5365 7420   ``True``.  Set 
-000224f0: 7468 6973 0a20 2020 2020 2020 2074 6f20  this.        to 
-00022500: 6060 4661 6c73 6560 6020 616e 6420 6f6e  ``False`` and on
-00022510: 6c79 2074 6865 2066 696c 656e 616d 6520  ly the filename 
-00022520: 7769 6c6c 2062 6520 7265 7475 726e 6564  will be returned
-00022530: 2e0a 0a20 2020 2052 6574 7572 6e73 0a20  ...    Returns. 
-00022540: 2020 202d 2d2d 2d2d 2d2d 0a20 2020 2070     -------.    p
-00022550: 7976 6973 7461 2e50 6f6c 7944 6174 6120  yvista.PolyData 
-00022560: 7c20 7374 720a 2020 2020 2020 2020 4461  | str.        Da
-00022570: 7461 5365 7420 6f72 2066 696c 656e 616d  taSet or filenam
-00022580: 6520 6465 7065 6e64 696e 6720 6f6e 2060  e depending on `
-00022590: 606c 6f61 6460 602e 0a0a 2020 2020 4578  `load``...    Ex
-000225a0: 616d 706c 6573 0a20 2020 202d 2d2d 2d2d  amples.    -----
-000225b0: 2d2d 2d0a 2020 2020 446f 776e 6c6f 6164  ---.    Download
-000225c0: 2061 6e64 2070 6c6f 7420 7468 6520 6461   and plot the da
-000225d0: 7461 7365 742e 0a0a 2020 2020 3e3e 3e20  taset...    >>> 
-000225e0: 6672 6f6d 2070 7976 6973 7461 2069 6d70  from pyvista imp
-000225f0: 6f72 7420 6578 616d 706c 6573 0a20 2020  ort examples.   
-00022600: 203e 3e3e 206d 6573 6820 3d20 6578 616d   >>> mesh = exam
-00022610: 706c 6573 2e64 6f77 6e6c 6f61 645f 6f77  ples.download_ow
-00022620: 6c28 290a 2020 2020 3e3e 3e20 6370 6f73  l().    >>> cpos
-00022630: 203d 205b 0a20 2020 202e 2e2e 2020 2020   = [.    ...    
-00022640: 2028 2d33 3135 2e31 382c 202d 3430 322e   (-315.18, -402.
-00022650: 3231 2c20 3233 302e 3731 292c 0a20 2020  21, 230.71),.   
-00022660: 202e 2e2e 2020 2020 2028 362e 3036 2c20   ...     (6.06, 
-00022670: 2d31 2e37 342c 2031 3031 2e34 3829 2c0a  -1.74, 101.48),.
-00022680: 2020 2020 2e2e 2e20 2020 2020 2830 2e31      ...     (0.1
-00022690: 3038 2c20 302e 3232 362c 2030 2e39 3638  08, 0.226, 0.968
-000226a0: 292c 0a20 2020 202e 2e2e 205d 0a20 2020  ),.    ... ].   
-000226b0: 203e 3e3e 206d 6573 682e 706c 6f74 2863   >>> mesh.plot(c
-000226c0: 706f 733d 6370 6f73 290a 0a20 2020 2052  pos=cpos)..    R
-000226d0: 6574 7572 6e20 7468 6520 7374 6174 6973  eturn the statis
-000226e0: 7469 6373 206f 6620 7468 6520 6461 7461  tics of the data
-000226f0: 7365 742e 0a0a 2020 2020 3e3e 3e20 6d65  set...    >>> me
-00022700: 7368 0a20 2020 2050 6f6c 7944 6174 6120  sh.    PolyData 
-00022710: 282e 2e2e 290a 2020 2020 2020 4e20 4365  (...).      N Ce
-00022720: 6c6c 733a 2020 2020 3234 3430 3730 370a  lls:    2440707.
-00022730: 2020 2020 2020 4e20 506f 696e 7473 3a20        N Points: 
-00022740: 2020 3132 3231 3735 360a 2020 2020 2020    1221756.      
-00022750: 4e20 5374 7269 7073 3a20 2020 300a 2020  N Strips:   0.  
-00022760: 2020 2020 5820 426f 756e 6473 3a20 2020      X Bounds:   
-00022770: 2d35 2e38 3334 652b 3031 2c20 372e 3034  -5.834e+01, 7.04
-00022780: 3765 2b30 310a 2020 2020 2020 5920 426f  7e+01.      Y Bo
-00022790: 756e 6473 3a20 2020 2d37 2e30 3036 652b  unds:   -7.006e+
-000227a0: 3031 2c20 362e 3635 3865 2b30 310a 2020  01, 6.658e+01.  
-000227b0: 2020 2020 5a20 426f 756e 6473 3a20 2020      Z Bounds:   
-000227c0: 312e 3637 3665 2b30 302c 2032 2e30 3133  1.676e+00, 2.013
-000227d0: 652b 3032 0a20 2020 2020 204e 2041 7272  e+02.      N Arr
-000227e0: 6179 733a 2020 2030 0a0a 2020 2020 2222  ays:   0..    ""
-000227f0: 220a 2020 2020 6669 6c65 6e61 6d65 203d  ".    filename =
-00022800: 205f 646f 776e 6c6f 6164 5f61 7263 6869   _download_archi
-00022810: 7665 280a 2020 2020 2020 2020 2769 7661  ve(.        'iva
-00022820: 6e2d 6e69 6b6f 6c6f 762f 6f77 6c2e 7a69  n-nikolov/owl.zi
-00022830: 7027 2c0a 2020 2020 2020 2020 276f 776c  p',.        'owl
-00022840: 2e76 7470 272c 0a20 2020 2029 0a20 2020  .vtp',.    ).   
-00022850: 2069 6620 6c6f 6164 3a0a 2020 2020 2020   if load:.      
-00022860: 2020 7265 7475 726e 2070 7976 6973 7461    return pyvista
-00022870: 2e72 6561 6428 6669 6c65 6e61 6d65 290a  .read(filename).
-00022880: 2020 2020 7265 7475 726e 2066 696c 656e      return filen
-00022890: 616d 650a 0a0a 6465 6620 646f 776e 6c6f  ame...def downlo
-000228a0: 6164 5f70 6c61 7374 6963 5f76 6173 6528  ad_plastic_vase(
-000228b0: 6c6f 6164 3d54 7275 6529 3a20 2023 2070  load=True):  # p
-000228c0: 7261 676d 613a 206e 6f20 636f 7665 720a  ragma: no cover.
-000228d0: 2020 2020 2222 2244 6f77 6e6c 6f61 6420      """Download 
-000228e0: 6120 7363 616e 206f 6620 6120 706c 6173  a scan of a plas
-000228f0: 7469 6320 7661 7365 2063 7265 6174 6564  tic vase created
-00022900: 2062 7920 4976 616e 204e 696b 6f6c 6f76   by Ivan Nikolov
-00022910: 2e0a 0a20 2020 2054 6865 2064 6174 6173  ...    The datas
-00022920: 6574 2077 6173 2064 6f77 6e6c 6f61 6465  et was downloade
-00022930: 6420 6672 6f6d 2060 4747 472d 4265 6e63  d from `GGG-Benc
-00022940: 686d 6172 6b53 664d 3a20 4461 7461 7365  hmarkSfM: Datase
-00022950: 7420 666f 7220 4265 6e63 686d 6172 6b69  t for Benchmarki
-00022960: 6e67 0a20 2020 2043 6c6f 7365 2d72 616e  ng.    Close-ran
-00022970: 6765 2053 664d 2053 6f66 7477 6172 6520  ge SfM Software 
-00022980: 5065 7266 6f72 6d61 6e63 6520 756e 6465  Performance unde
-00022990: 7220 5661 7279 696e 6720 4361 7074 7572  r Varying Captur
-000229a0: 696e 6720 436f 6e64 6974 696f 6e73 0a20  ing Conditions. 
-000229b0: 2020 203c 6874 7470 733a 2f2f 6461 7461     <https://data
-000229c0: 2e6d 656e 6465 6c65 792e 636f 6d2f 6461  .mendeley.com/da
-000229d0: 7461 7365 7473 2f62 7a78 6b32 6e37 3873  tasets/bzxk2n78s
-000229e0: 392f 343e 605f 0a0a 2020 2020 4f72 6967  9/4>`_..    Orig
-000229f0: 696e 616c 2064 6174 6173 6574 7320 6172  inal datasets ar
-00022a00: 6520 756e 6465 7220 7468 6520 4343 2042  e under the CC B
-00022a10: 5920 342e 3020 6c69 6365 6e73 652e 0a0a  Y 4.0 license...
-00022a20: 2020 2020 466f 7220 6d6f 7265 2064 6574      For more det
-00022a30: 6169 6c73 2c20 7365 6520 6049 7661 6e20  ails, see `Ivan 
-00022a40: 4e69 6b6f 6c6f 7620 4461 7461 7365 7473  Nikolov Datasets
-00022a50: 0a20 2020 203c 6874 7470 733a 2f2f 6769  .    <https://gi
-00022a60: 7468 7562 2e63 6f6d 2f70 7976 6973 7461  thub.com/pyvista
-00022a70: 2f76 746b 2d64 6174 612f 7472 6565 2f6d  /vtk-data/tree/m
-00022a80: 6173 7465 722f 4461 7461 2f69 7661 6e2d  aster/Data/ivan-
-00022a90: 6e69 6b6f 6c6f 763e 605f 0a0a 2020 2020  nikolov>`_..    
-00022aa0: 5061 7261 6d65 7465 7273 0a20 2020 202d  Parameters.    -
-00022ab0: 2d2d 2d2d 2d2d 2d2d 2d0a 2020 2020 6c6f  ---------.    lo
-00022ac0: 6164 203a 2062 6f6f 6c2c 2064 6566 6175  ad : bool, defau
-00022ad0: 6c74 3a20 5472 7565 0a20 2020 2020 2020  lt: True.       
-00022ae0: 204c 6f61 6420 7468 6520 6461 7461 7365   Load the datase
-00022af0: 7420 6166 7465 7220 646f 776e 6c6f 6164  t after download
-00022b00: 696e 6720 6974 2077 6865 6e20 6060 5472  ing it when ``Tr
-00022b10: 7565 6060 2e20 2053 6574 2074 6869 730a  ue``.  Set this.
-00022b20: 2020 2020 2020 2020 746f 2060 6046 616c          to ``Fal
-00022b30: 7365 6060 2061 6e64 206f 6e6c 7920 7468  se`` and only th
-00022b40: 6520 6669 6c65 6e61 6d65 2077 696c 6c20  e filename will 
-00022b50: 6265 2072 6574 7572 6e65 642e 0a0a 2020  be returned...  
-00022b60: 2020 5265 7475 726e 730a 2020 2020 2d2d    Returns.    --
-00022b70: 2d2d 2d2d 2d0a 2020 2020 7079 7669 7374  -----.    pyvist
-00022b80: 612e 506f 6c79 4461 7461 207c 2073 7472  a.PolyData | str
-00022b90: 0a20 2020 2020 2020 2044 6174 6153 6574  .        DataSet
-00022ba0: 206f 7220 6669 6c65 6e61 6d65 2064 6570   or filename dep
-00022bb0: 656e 6469 6e67 206f 6e20 6060 6c6f 6164  ending on ``load
-00022bc0: 6060 2e0a 0a20 2020 2045 7861 6d70 6c65  ``...    Example
-00022bd0: 730a 2020 2020 2d2d 2d2d 2d2d 2d2d 0a20  s.    --------. 
-00022be0: 2020 2044 6f77 6e6c 6f61 6420 616e 6420     Download and 
-00022bf0: 706c 6f74 2074 6865 2064 6174 6173 6574  plot the dataset
-00022c00: 2e0a 0a20 2020 203e 3e3e 2066 726f 6d20  ...    >>> from 
-00022c10: 7079 7669 7374 6120 696d 706f 7274 2065  pyvista import e
-00022c20: 7861 6d70 6c65 730a 2020 2020 3e3e 3e20  xamples.    >>> 
-00022c30: 6d65 7368 203d 2065 7861 6d70 6c65 732e  mesh = examples.
-00022c40: 646f 776e 6c6f 6164 5f70 6c61 7374 6963  download_plastic
-00022c50: 5f76 6173 6528 290a 2020 2020 3e3e 3e20  _vase().    >>> 
-00022c60: 6d65 7368 2e70 6c6f 7428 290a 0a20 2020  mesh.plot()..   
-00022c70: 2052 6574 7572 6e20 7468 6520 7374 6174   Return the stat
-00022c80: 6973 7469 6373 206f 6620 7468 6520 6461  istics of the da
-00022c90: 7461 7365 742e 0a0a 2020 2020 3e3e 3e20  taset...    >>> 
-00022ca0: 6d65 7368 0a20 2020 2050 6f6c 7944 6174  mesh.    PolyDat
-00022cb0: 6120 282e 2e2e 290a 2020 2020 2020 4e20  a (...).      N 
-00022cc0: 4365 6c6c 733a 2020 2020 3335 3730 3936  Cells:    357096
-00022cd0: 370a 2020 2020 2020 4e20 506f 696e 7473  7.      N Points
-00022ce0: 3a20 2020 3137 3936 3830 350a 2020 2020  :   1796805.    
-00022cf0: 2020 4e20 5374 7269 7073 3a20 2020 300a    N Strips:   0.
-00022d00: 2020 2020 2020 5820 426f 756e 6473 3a20        X Bounds: 
-00022d10: 2020 2d31 2e33 3634 652b 3032 2c20 312e    -1.364e+02, 1.
-00022d20: 3932 3965 2b30 320a 2020 2020 2020 5920  929e+02.      Y 
-00022d30: 426f 756e 6473 3a20 2020 2d31 2e36 3737  Bounds:   -1.677
-00022d40: 652b 3032 2c20 312e 3630 3365 2b30 320a  e+02, 1.603e+02.
-00022d50: 2020 2020 2020 5a20 426f 756e 6473 3a20        Z Bounds: 
-00022d60: 2020 312e 3230 3965 2b30 322c 2034 2e30    1.209e+02, 4.0
-00022d70: 3930 652b 3032 0a20 2020 2020 204e 2041  90e+02.      N A
-00022d80: 7272 6179 733a 2020 2030 0a0a 2020 2020  rrays:   0..    
-00022d90: 2222 220a 2020 2020 6669 6c65 6e61 6d65  """.    filename
-00022da0: 203d 205f 646f 776e 6c6f 6164 5f61 7263   = _download_arc
-00022db0: 6869 7665 280a 2020 2020 2020 2020 2769  hive(.        'i
-00022dc0: 7661 6e2d 6e69 6b6f 6c6f 762f 706c 6173  van-nikolov/plas
-00022dd0: 7469 6356 6173 652e 7a69 7027 2c0a 2020  ticVase.zip',.  
-00022de0: 2020 2020 2020 2770 6c61 7374 6963 5661        'plasticVa
-00022df0: 7365 2e76 7470 272c 0a20 2020 2029 0a20  se.vtp',.    ). 
-00022e00: 2020 2069 6620 6c6f 6164 3a0a 2020 2020     if load:.    
-00022e10: 2020 2020 7265 7475 726e 2070 7976 6973      return pyvis
-00022e20: 7461 2e72 6561 6428 6669 6c65 6e61 6d65  ta.read(filename
-00022e30: 290a 2020 2020 7265 7475 726e 2066 696c  ).    return fil
-00022e40: 656e 616d 650a 0a0a 6465 6620 646f 776e  ename...def down
-00022e50: 6c6f 6164 5f73 6561 5f76 6173 6528 6c6f  load_sea_vase(lo
-00022e60: 6164 3d54 7275 6529 3a20 2023 2070 7261  ad=True):  # pra
-00022e70: 676d 613a 206e 6f20 636f 7665 720a 2020  gma: no cover.  
-00022e80: 2020 2222 2244 6f77 6e6c 6f61 6420 6120    """Download a 
-00022e90: 7363 616e 206f 6620 6120 7365 6120 7661  scan of a sea va
-00022ea0: 7365 2063 7265 6174 6564 2062 7920 4976  se created by Iv
-00022eb0: 616e 204e 696b 6f6c 6f76 2e0a 0a20 2020  an Nikolov...   
-00022ec0: 2054 6865 2064 6174 6173 6574 2077 6173   The dataset was
-00022ed0: 2064 6f77 6e6c 6f61 6465 6420 6672 6f6d   downloaded from
-00022ee0: 2060 4747 472d 4265 6e63 686d 6172 6b53   `GGG-BenchmarkS
-00022ef0: 664d 3a20 4461 7461 7365 7420 666f 7220  fM: Dataset for 
-00022f00: 4265 6e63 686d 6172 6b69 6e67 0a20 2020  Benchmarking.   
-00022f10: 2043 6c6f 7365 2d72 616e 6765 2053 664d   Close-range SfM
-00022f20: 2053 6f66 7477 6172 6520 5065 7266 6f72   Software Perfor
-00022f30: 6d61 6e63 6520 756e 6465 7220 5661 7279  mance under Vary
-00022f40: 696e 6720 4361 7074 7572 696e 6720 436f  ing Capturing Co
-00022f50: 6e64 6974 696f 6e73 0a20 2020 203c 6874  nditions.    <ht
-00022f60: 7470 733a 2f2f 6461 7461 2e6d 656e 6465  tps://data.mende
-00022f70: 6c65 792e 636f 6d2f 6461 7461 7365 7473  ley.com/datasets
-00022f80: 2f62 7a78 6b32 6e37 3873 392f 343e 605f  /bzxk2n78s9/4>`_
-00022f90: 0a0a 2020 2020 4f72 6967 696e 616c 2064  ..    Original d
-00022fa0: 6174 6173 6574 7320 6172 6520 756e 6465  atasets are unde
-00022fb0: 7220 7468 6520 4343 2042 5920 342e 3020  r the CC BY 4.0 
-00022fc0: 6c69 6365 6e73 652e 0a0a 2020 2020 466f  license...    Fo
-00022fd0: 7220 6d6f 7265 2064 6574 6169 6c73 2c20  r more details, 
-00022fe0: 7365 6520 6049 7661 6e20 4e69 6b6f 6c6f  see `Ivan Nikolo
-00022ff0: 7620 4461 7461 7365 7473 0a20 2020 203c  v Datasets.    <
-00023000: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
-00023010: 6f6d 2f70 7976 6973 7461 2f76 746b 2d64  om/pyvista/vtk-d
-00023020: 6174 612f 7472 6565 2f6d 6173 7465 722f  ata/tree/master/
-00023030: 4461 7461 2f69 7661 6e2d 6e69 6b6f 6c6f  Data/ivan-nikolo
-00023040: 763e 605f 0a0a 2020 2020 5061 7261 6d65  v>`_..    Parame
-00023050: 7465 7273 0a20 2020 202d 2d2d 2d2d 2d2d  ters.    -------
-00023060: 2d2d 2d0a 2020 2020 6c6f 6164 203a 2062  ---.    load : b
-00023070: 6f6f 6c2c 2064 6566 6175 6c74 3a20 5472  ool, default: Tr
-00023080: 7565 0a20 2020 2020 2020 204c 6f61 6420  ue.        Load 
-00023090: 7468 6520 6461 7461 7365 7420 6166 7465  the dataset afte
-000230a0: 7220 646f 776e 6c6f 6164 696e 6720 6974  r downloading it
-000230b0: 2077 6865 6e20 6060 5472 7565 6060 2e20   when ``True``. 
-000230c0: 2053 6574 2074 6869 730a 2020 2020 2020   Set this.      
-000230d0: 2020 746f 2060 6046 616c 7365 6060 2061    to ``False`` a
-000230e0: 6e64 206f 6e6c 7920 7468 6520 6669 6c65  nd only the file
-000230f0: 6e61 6d65 2077 696c 6c20 6265 2072 6574  name will be ret
-00023100: 7572 6e65 642e 0a0a 2020 2020 5265 7475  urned...    Retu
-00023110: 726e 730a 2020 2020 2d2d 2d2d 2d2d 2d0a  rns.    -------.
-00023120: 2020 2020 7079 7669 7374 612e 506f 6c79      pyvista.Poly
-00023130: 4461 7461 207c 2073 7472 0a20 2020 2020  Data | str.     
-00023140: 2020 2044 6174 6153 6574 206f 7220 6669     DataSet or fi
-00023150: 6c65 6e61 6d65 2064 6570 656e 6469 6e67  lename depending
-00023160: 206f 6e20 6060 6c6f 6164 6060 2e0a 0a20   on ``load``... 
-00023170: 2020 2045 7861 6d70 6c65 730a 2020 2020     Examples.    
-00023180: 2d2d 2d2d 2d2d 2d2d 0a20 2020 2044 6f77  --------.    Dow
-00023190: 6e6c 6f61 6420 616e 6420 706c 6f74 2074  nload and plot t
-000231a0: 6865 2064 6174 6173 6574 2e0a 0a20 2020  he dataset...   
-000231b0: 203e 3e3e 2066 726f 6d20 7079 7669 7374   >>> from pyvist
-000231c0: 6120 696d 706f 7274 2065 7861 6d70 6c65  a import example
-000231d0: 730a 2020 2020 3e3e 3e20 6d65 7368 203d  s.    >>> mesh =
-000231e0: 2065 7861 6d70 6c65 732e 646f 776e 6c6f   examples.downlo
-000231f0: 6164 5f73 6561 5f76 6173 6528 290a 2020  ad_sea_vase().  
-00023200: 2020 3e3e 3e20 6d65 7368 2e70 6c6f 7428    >>> mesh.plot(
-00023210: 290a 0a20 2020 2052 6574 7572 6e20 7468  )..    Return th
-00023220: 6520 7374 6174 6973 7469 6373 206f 6620  e statistics of 
-00023230: 7468 6520 6461 7461 7365 742e 0a0a 2020  the dataset...  
-00023240: 2020 3e3e 3e20 6d65 7368 0a20 2020 2050    >>> mesh.    P
-00023250: 6f6c 7944 6174 6120 282e 2e2e 290a 2020  olyData (...).  
-00023260: 2020 2020 4e20 4365 6c6c 733a 2020 2020      N Cells:    
-00023270: 3335 3438 3437 330a 2020 2020 2020 4e20  3548473.      N 
-00023280: 506f 696e 7473 3a20 2020 3138 3130 3031  Points:   181001
-00023290: 320a 2020 2020 2020 4e20 5374 7269 7073  2.      N Strips
-000232a0: 3a20 2020 300a 2020 2020 2020 5820 426f  :   0.      X Bo
-000232b0: 756e 6473 3a20 2020 2d31 2e36 3636 652b  unds:   -1.666e+
-000232c0: 3032 2c20 312e 3436 3565 2b30 320a 2020  02, 1.465e+02.  
-000232d0: 2020 2020 5920 426f 756e 6473 3a20 2020      Y Bounds:   
-000232e0: 2d31 2e37 3432 652b 3032 2c20 312e 3338  -1.742e+02, 1.38
-000232f0: 3465 2b30 320a 2020 2020 2020 5a20 426f  4e+02.      Z Bo
-00023300: 756e 6473 3a20 2020 2d31 2e35 3030 652b  unds:   -1.500e+
-00023310: 3032 2c20 322e 3939 3265 2b30 320a 2020  02, 2.992e+02.  
-00023320: 2020 2020 4e20 4172 7261 7973 3a20 2020      N Arrays:   
-00023330: 300a 0a20 2020 2022 2222 0a20 2020 2066  0..    """.    f
-00023340: 696c 656e 616d 6520 3d20 5f64 6f77 6e6c  ilename = _downl
-00023350: 6f61 645f 6172 6368 6976 6528 0a20 2020  oad_archive(.   
-00023360: 2020 2020 2027 6976 616e 2d6e 696b 6f6c       'ivan-nikol
-00023370: 6f76 2f73 6561 5661 7365 2e7a 6970 272c  ov/seaVase.zip',
-00023380: 0a20 2020 2020 2020 2027 7365 6156 6173  .        'seaVas
-00023390: 652e 7674 7027 2c0a 2020 2020 290a 2020  e.vtp',.    ).  
-000233a0: 2020 6966 206c 6f61 643a 0a20 2020 2020    if load:.     
-000233b0: 2020 2072 6574 7572 6e20 7079 7669 7374     return pyvist
-000233c0: 612e 7265 6164 2866 696c 656e 616d 6529  a.read(filename)
-000233d0: 0a20 2020 2072 6574 7572 6e20 6669 6c65  .    return file
-000233e0: 6e61 6d65 0a0a 0a64 6566 2064 6f77 6e6c  name...def downl
-000233f0: 6f61 645f 6469 6b68 6f6c 6f6c 6f5f 6e69  oad_dikhololo_ni
-00023400: 6768 7428 293a 2020 2320 7072 6167 6d61  ght():  # pragma
-00023410: 3a20 6e6f 2063 6f76 6572 0a20 2020 2022  : no cover.    "
-00023420: 2222 446f 776e 6c6f 6164 2061 6e64 2072  ""Download and r
-00023430: 6561 6420 7468 6520 6469 6b68 6f6c 6f20  ead the dikholo 
-00023440: 6e69 6768 7420 6864 7220 7465 7874 7572  night hdr textur
-00023450: 6520 6578 616d 706c 652e 0a0a 2020 2020  e example...    
-00023460: 4669 6c65 7320 686f 7374 6564 2061 7420  Files hosted at 
-00023470: 6874 7470 733a 2f2f 706f 6c79 6861 7665  https://polyhave
-00023480: 6e2e 636f 6d2f 0a0a 2020 2020 5265 7475  n.com/..    Retu
-00023490: 726e 730a 2020 2020 2d2d 2d2d 2d2d 2d0a  rns.    -------.
-000234a0: 2020 2020 7079 7669 7374 612e 5465 7874      pyvista.Text
-000234b0: 7572 650a 2020 2020 2020 2020 4844 5220  ure.        HDR 
-000234c0: 5465 7874 7572 652e 0a0a 2020 2020 4578  Texture...    Ex
-000234d0: 616d 706c 6573 0a20 2020 202d 2d2d 2d2d  amples.    -----
-000234e0: 2d2d 2d0a 2020 2020 3e3e 3e20 696d 706f  ---.    >>> impo
-000234f0: 7274 2070 7976 6973 7461 2061 7320 7076  rt pyvista as pv
-00023500: 0a20 2020 203e 3e3e 2066 726f 6d20 7079  .    >>> from py
-00023510: 7669 7374 6120 696d 706f 7274 2065 7861  vista import exa
-00023520: 6d70 6c65 730a 2020 2020 3e3e 3e20 676c  mples.    >>> gl
-00023530: 7466 5f66 696c 6520 3d20 6578 616d 706c  tf_file = exampl
-00023540: 6573 2e67 6c74 662e 646f 776e 6c6f 6164  es.gltf.download
-00023550: 5f64 616d 6167 6564 5f68 656c 6d65 7428  _damaged_helmet(
-00023560: 290a 2020 2020 3e3e 3e20 7465 7874 7572  ).    >>> textur
-00023570: 6520 3d20 6578 616d 706c 6573 2e64 6f77  e = examples.dow
-00023580: 6e6c 6f61 645f 6469 6b68 6f6c 6f6c 6f5f  nload_dikhololo_
-00023590: 6e69 6768 7428 290a 2020 2020 3e3e 3e20  night().    >>> 
-000235a0: 706c 203d 2070 762e 506c 6f74 7465 7228  pl = pv.Plotter(
-000235b0: 290a 2020 2020 3e3e 3e20 706c 2e69 6d70  ).    >>> pl.imp
-000235c0: 6f72 745f 676c 7466 2867 6c74 665f 6669  ort_gltf(gltf_fi
-000235d0: 6c65 290a 2020 2020 3e3e 3e20 706c 2e73  le).    >>> pl.s
-000235e0: 6574 5f65 6e76 6972 6f6e 6d65 6e74 5f74  et_environment_t
-000235f0: 6578 7475 7265 2874 6578 7475 7265 290a  exture(texture).
-00023600: 2020 2020 3e3e 3e20 706c 2e73 686f 7728      >>> pl.show(
-00023610: 290a 0a20 2020 2022 2222 0a20 2020 2074  )..    """.    t
-00023620: 6578 7475 7265 203d 205f 646f 776e 6c6f  exture = _downlo
-00023630: 6164 5f61 6e64 5f72 6561 6428 2764 696b  ad_and_read('dik
-00023640: 686f 6c6f 6c6f 5f6e 6967 6874 5f34 6b2e  hololo_night_4k.
-00023650: 6864 7227 2c20 7465 7874 7572 653d 5472  hdr', texture=Tr
-00023660: 7565 290a 2020 2020 7465 7874 7572 652e  ue).    texture.
-00023670: 5365 7443 6f6c 6f72 4d6f 6465 546f 4469  SetColorModeToDi
-00023680: 7265 6374 5363 616c 6172 7328 290a 2020  rectScalars().  
-00023690: 2020 7465 7874 7572 652e 5365 744d 6970    texture.SetMip
-000236a0: 6d61 7028 5472 7565 290a 2020 2020 7465  map(True).    te
-000236b0: 7874 7572 652e 5365 7449 6e74 6572 706f  xture.SetInterpo
-000236c0: 6c61 7465 2854 7275 6529 0a20 2020 2072  late(True).    r
-000236d0: 6574 7572 6e20 7465 7874 7572 650a 0a0a  eturn texture...
-000236e0: 6465 6620 646f 776e 6c6f 6164 5f63 6164  def download_cad
-000236f0: 5f6d 6f64 656c 5f63 6173 6528 6c6f 6164  _model_case(load
-00023700: 3d54 7275 6529 3a20 2023 2070 7261 676d  =True):  # pragm
-00023710: 613a 206e 6f20 636f 7665 720a 2020 2020  a: no cover.    
-00023720: 2222 2244 6f77 6e6c 6f61 6420 6120 4341  """Download a CA
-00023730: 4420 6d6f 6465 6c20 6f66 2061 2052 6173  D model of a Ras
-00023740: 7062 6572 7279 2050 4920 3420 6361 7365  pberry PI 4 case
-00023750: 2e0a 0a20 2020 2054 6865 2064 6174 6173  ...    The datas
-00023760: 6574 2077 6173 2064 6f77 6e6c 6f61 6465  et was downloade
-00023770: 6420 6672 6f6d 2060 5468 696e 6769 7665  d from `Thingive
-00023780: 7273 650a 2020 2020 3c68 7474 7073 3a2f  rse.    <https:/
-00023790: 2f77 7777 2e74 6869 6e67 6976 6572 7365  /www.thingiverse
-000237a0: 2e63 6f6d 2f74 6869 6e67 3a34 3934 3737  .com/thing:49477
-000237b0: 3436 3e60 5f0a 0a20 2020 204f 7269 6769  46>`_..    Origi
-000237c0: 6e61 6c20 6461 7461 7365 7473 2061 7265  nal datasets are
-000237d0: 2075 6e64 6572 2074 6865 2060 4372 6561   under the `Crea
-000237e0: 7469 7665 2043 6f6d 6d6f 6e73 202d 2041  tive Commons - A
-000237f0: 7474 7269 6275 7469 6f6e 0a20 2020 203c  ttribution.    <
-00023800: 6874 7470 733a 2f2f 6372 6561 7469 7665  https://creative
-00023810: 636f 6d6d 6f6e 732e 6f72 672f 6c69 6365  commons.org/lice
-00023820: 6e73 6573 2f62 792f 342e 302f 3e60 5f20  nses/by/4.0/>`_ 
-00023830: 6c69 6365 6e73 652e 0a0a 2020 2020 5061  license...    Pa
-00023840: 7261 6d65 7465 7273 0a20 2020 202d 2d2d  rameters.    ---
-00023850: 2d2d 2d2d 2d2d 2d0a 2020 2020 6c6f 6164  -------.    load
-00023860: 203a 2062 6f6f 6c2c 2064 6566 6175 6c74   : bool, default
-00023870: 3a20 5472 7565 0a20 2020 2020 2020 204c  : True.        L
-00023880: 6f61 6420 7468 6520 6461 7461 7365 7420  oad the dataset 
-00023890: 6166 7465 7220 646f 776e 6c6f 6164 696e  after downloadin
-000238a0: 6720 6974 2077 6865 6e20 6060 5472 7565  g it when ``True
-000238b0: 6060 2e20 2053 6574 2074 6869 730a 2020  ``.  Set this.  
-000238c0: 2020 2020 2020 746f 2060 6046 616c 7365        to ``False
-000238d0: 6060 2061 6e64 206f 6e6c 7920 7468 6520  `` and only the 
-000238e0: 6669 6c65 6e61 6d65 2077 696c 6c20 6265  filename will be
-000238f0: 2072 6574 7572 6e65 642e 0a0a 2020 2020   returned...    
-00023900: 5265 7475 726e 730a 2020 2020 2d2d 2d2d  Returns.    ----
-00023910: 2d2d 2d0a 2020 2020 7079 7669 7374 612e  ---.    pyvista.
-00023920: 506f 6c79 4461 7461 207c 2073 7472 0a20  PolyData | str. 
-00023930: 2020 2020 2020 2044 6174 6153 6574 206f         DataSet o
-00023940: 7220 6669 6c65 6e61 6d65 2064 6570 656e  r filename depen
-00023950: 6469 6e67 206f 6e20 6060 6c6f 6164 6060  ding on ``load``
-00023960: 2e0a 0a20 2020 2045 7861 6d70 6c65 730a  ...    Examples.
-00023970: 2020 2020 2d2d 2d2d 2d2d 2d2d 0a20 2020      --------.   
-00023980: 2044 6f77 6e6c 6f61 6420 616e 6420 706c   Download and pl
-00023990: 6f74 2074 6865 2064 6174 6173 6574 2e0a  ot the dataset..
-000239a0: 0a20 2020 203e 3e3e 2066 726f 6d20 7079  .    >>> from py
-000239b0: 7669 7374 6120 696d 706f 7274 2065 7861  vista import exa
-000239c0: 6d70 6c65 730a 2020 2020 3e3e 3e20 6d65  mples.    >>> me
-000239d0: 7368 203d 2065 7861 6d70 6c65 732e 646f  sh = examples.do
-000239e0: 776e 6c6f 6164 5f63 6164 5f6d 6f64 656c  wnload_cad_model
-000239f0: 5f63 6173 6528 290a 2020 2020 3e3e 3e20  _case().    >>> 
-00023a00: 6d65 7368 2e70 6c6f 7428 290a 0a20 2020  mesh.plot()..   
-00023a10: 2052 6574 7572 6e20 7468 6520 7374 6174   Return the stat
-00023a20: 6973 7469 6373 206f 6620 7468 6520 6461  istics of the da
-00023a30: 7461 7365 742e 0a0a 2020 2020 3e3e 3e20  taset...    >>> 
-00023a40: 6d65 7368 0a20 2020 2050 6f6c 7944 6174  mesh.    PolyDat
-00023a50: 6120 282e 2e2e 290a 2020 2020 2020 4e20  a (...).      N 
-00023a60: 4365 6c6c 733a 2020 2020 3135 3434 360a  Cells:    15446.
-00023a70: 2020 2020 2020 4e20 506f 696e 7473 3a20        N Points: 
-00023a80: 2020 3736 3737 0a20 2020 2020 204e 2053    7677.      N S
-00023a90: 7472 6970 733a 2020 2030 0a20 2020 2020  trips:   0.     
-00023aa0: 2058 2042 6f75 6e64 733a 2020 202d 362e   X Bounds:   -6.
-00023ab0: 3436 3065 2d33 312c 2039 2e30 3030 652b  460e-31, 9.000e+
-00023ac0: 3031 0a20 2020 2020 2059 2042 6f75 6e64  01.      Y Bound
-00023ad0: 733a 2020 202d 332e 3533 3565 2d33 322c  s:   -3.535e-32,
-00023ae0: 2031 2e34 3830 652b 3032 0a20 2020 2020   1.480e+02.     
-00023af0: 205a 2042 6f75 6e64 733a 2020 2030 2e30   Z Bounds:   0.0
-00023b00: 3030 652b 3030 2c20 322e 3030 3065 2b30  00e+00, 2.000e+0
-00023b10: 310a 2020 2020 2020 4e20 4172 7261 7973  1.      N Arrays
-00023b20: 3a20 2020 320a 0a20 2020 2022 2222 0a20  :   2..    """. 
-00023b30: 2020 2072 6574 7572 6e20 5f64 6f77 6e6c     return _downl
-00023b40: 6f61 645f 616e 645f 7265 6164 2827 6361  oad_and_read('ca
-00023b50: 642f 3439 3437 3734 362f 5665 6e74 6564  d/4947746/Vented
-00023b60: 5f52 6561 725f 4361 7365 5f57 6974 685f  _Rear_Case_With_
-00023b70: 5069 5f53 7570 706f 7274 732e 7674 7027  Pi_Supports.vtp'
-00023b80: 2c20 6c6f 6164 3d6c 6f61 6429 0a0a 0a64  , load=load)...d
-00023b90: 6566 2064 6f77 6e6c 6f61 645f 6165 726f  ef download_aero
-00023ba0: 5f62 7261 636b 6574 286c 6f61 643d 5472  _bracket(load=Tr
-00023bb0: 7565 293a 2020 2320 7072 6167 6d61 3a20  ue):  # pragma: 
-00023bc0: 6e6f 2063 6f76 6572 0a20 2020 2022 2222  no cover.    """
-00023bd0: 446f 776e 6c6f 6164 2074 6865 2066 696e  Download the fin
-00023be0: 6974 6520 656c 656d 656e 7420 736f 6c75  ite element solu
-00023bf0: 7469 6f6e 206f 6620 616e 2061 6572 6f20  tion of an aero 
-00023c00: 6272 6163 6b65 742e 0a0a 2020 2020 4461  bracket...    Da
-00023c10: 7461 2067 656e 6572 6174 6564 2066 726f  ta generated fro
-00023c20: 6d20 7075 626c 6963 2053 696d 5363 616c  m public SimScal
-00023c30: 6520 6578 616d 706c 6573 2061 7420 6053  e examples at `S
-00023c40: 696d 5363 616c 6520 5072 6f6a 6563 7420  imScale Project 
-00023c50: 4c69 6272 6172 7920 2d0a 2020 2020 5475  Library -.    Tu
-00023c60: 7262 6f20 3c68 7474 7073 3a2f 2f77 7777  rbo <https://www
-00023c70: 2e73 696d 7363 616c 652e 636f 6d2f 7072  .simscale.com/pr
-00023c80: 6f6a 6563 7473 2f61 7961 726e 6f7a 2f74  ojects/ayarnoz/t
-00023c90: 7572 626f 2f3e 605f 2e0a 0a20 2020 204c  urbo/>`_...    L
-00023ca0: 6963 656e 7369 6e67 2066 6f72 2074 6869  icensing for thi
-00023cb0: 7320 6461 7461 7365 7420 6973 2067 7261  s dataset is gra
-00023cc0: 6e74 6564 2074 6f20 6672 6565 6c79 2061  nted to freely a
-00023cd0: 6e64 2077 6974 686f 7574 2072 6573 7472  nd without restr
-00023ce0: 6963 7469 6f6e 0a20 2020 2072 6570 726f  iction.    repro
-00023cf0: 6475 6365 2c20 6469 7374 7269 6275 7465  duce, distribute
-00023d00: 2c20 7075 626c 6973 6820 6163 636f 7264  , publish accord
-00023d10: 696e 6720 746f 2074 6865 2060 5369 6d53  ing to the `SimS
-00023d20: 6361 6c65 2054 6572 6d73 2061 6e64 0a20  cale Terms and. 
-00023d30: 2020 2043 6f6e 6469 7469 6f6e 7320 3c68     Conditions <h
-00023d40: 7474 7073 3a2f 2f77 7777 2e73 696d 7363  ttps://www.simsc
-00023d50: 616c 652e 636f 6d2f 7465 726d 732d 616e  ale.com/terms-an
-00023d60: 642d 636f 6e64 6974 696f 6e73 2f3e 605f  d-conditions/>`_
-00023d70: 2e0a 0a20 2020 2054 6869 7320 7072 6f6a  ...    This proj
-00023d80: 6563 7420 6465 6d6f 6e73 7472 6174 6573  ect demonstrates
-00023d90: 2074 6865 2073 7461 7469 6320 7374 7265   the static stre
-00023da0: 7373 2061 6e61 6c79 7369 7320 6f66 2074  ss analysis of t
-00023db0: 6872 6565 2061 6972 6372 6166 740a 2020  hree aircraft.  
-00023dc0: 2020 656e 6769 6e65 2062 6561 7269 6e67    engine bearing
-00023dd0: 2062 7261 636b 6574 206d 6f64 656c 7320   bracket models 
-00023de0: 636f 6e73 6964 6572 696e 6720 626f 7468  considering both
-00023df0: 206c 696e 6561 7220 616e 6420 6e6f 6e6c   linear and nonl
-00023e00: 696e 6561 720a 2020 2020 6d61 7465 7269  inear.    materi
-00023e10: 616c 2064 6566 696e 6974 696f 6e2e 2054  al definition. T
-00023e20: 6865 206d 6f64 656c 7320 6172 6520 7465  he models are te
-00023e30: 7374 6564 2077 6974 6820 686f 7269 7a6f  sted with horizo
-00023e40: 6e74 616c 2061 6e64 2076 6572 7469 6361  ntal and vertica
-00023e50: 6c0a 2020 2020 6c6f 6164 696e 6720 636f  l.    loading co
-00023e60: 6e64 6974 696f 6e73 2061 7320 7072 6f76  nditions as prov
-00023e70: 6964 6564 206f 6e20 7468 6520 6047 7261  ided on the `Gra
-00023e80: 6243 4144 202d 2041 6972 706c 616e 6520  bCAD - Airplane 
-00023e90: 4265 6172 696e 6720 4272 6163 6b65 740a  Bearing Bracket.
-00023ea0: 2020 2020 4368 616c 6c65 6e67 650a 2020      Challenge.  
-00023eb0: 2020 3c68 7474 7073 3a2f 2f67 7261 6263    <https://grabc
-00023ec0: 6164 2e63 6f6d 2f63 6861 6c6c 656e 6765  ad.com/challenge
-00023ed0: 732f 6169 7270 6c61 6e65 2d62 6561 7269  s/airplane-beari
-00023ee0: 6e67 2d62 7261 636b 6574 2d63 6861 6c6c  ng-bracket-chall
-00023ef0: 656e 6765 2f65 6e74 7269 6573 3e60 5f2e  enge/entries>`_.
-00023f00: 0a0a 2020 2020 5061 7261 6d65 7465 7273  ..    Parameters
-00023f10: 0a20 2020 202d 2d2d 2d2d 2d2d 2d2d 2d0a  .    ----------.
-00023f20: 2020 2020 6c6f 6164 203a 2062 6f6f 6c2c      load : bool,
-00023f30: 2064 6566 6175 6c74 3a20 5472 7565 0a20   default: True. 
-00023f40: 2020 2020 2020 204c 6f61 6420 7468 6520         Load the 
-00023f50: 6461 7461 7365 7420 6166 7465 7220 646f  dataset after do
-00023f60: 776e 6c6f 6164 696e 6720 6974 2077 6865  wnloading it whe
-00023f70: 6e20 6060 5472 7565 6060 2e20 2053 6574  n ``True``.  Set
-00023f80: 2074 6869 730a 2020 2020 2020 2020 746f   this.        to
-00023f90: 2060 6046 616c 7365 6060 2061 6e64 206f   ``False`` and o
-00023fa0: 6e6c 7920 7468 6520 6669 6c65 6e61 6d65  nly the filename
-00023fb0: 2077 696c 6c20 6265 2072 6574 7572 6e65   will be returne
-00023fc0: 642e 0a0a 2020 2020 5265 7475 726e 730a  d...    Returns.
-00023fd0: 2020 2020 2d2d 2d2d 2d2d 2d0a 2020 2020      -------.    
-00023fe0: 7079 7669 7374 612e 556e 7374 7275 6374  pyvista.Unstruct
-00023ff0: 7572 6564 4772 6964 207c 2073 7472 0a20  uredGrid | str. 
-00024000: 2020 2020 2020 2044 6174 6153 6574 206f         DataSet o
-00024010: 7220 6669 6c65 6e61 6d65 2064 6570 656e  r filename depen
-00024020: 6469 6e67 206f 6e20 6060 6c6f 6164 6060  ding on ``load``
-00024030: 2e0a 0a20 2020 2045 7861 6d70 6c65 730a  ...    Examples.
-00024040: 2020 2020 2d2d 2d2d 2d2d 2d2d 0a20 2020      --------.   
-00024050: 2044 6f77 6e6c 6f61 6420 7468 6520 6165   Download the ae
-00024060: 726f 2062 7261 636b 6574 2e0a 0a20 2020  ro bracket...   
-00024070: 203e 3e3e 2066 726f 6d20 7079 7669 7374   >>> from pyvist
-00024080: 6120 696d 706f 7274 2065 7861 6d70 6c65  a import example
-00024090: 730a 2020 2020 3e3e 3e20 6461 7461 7365  s.    >>> datase
-000240a0: 7420 3d20 6578 616d 706c 6573 2e64 6f77  t = examples.dow
-000240b0: 6e6c 6f61 645f 6165 726f 5f62 7261 636b  nload_aero_brack
-000240c0: 6574 2829 0a20 2020 203e 3e3e 2064 6174  et().    >>> dat
-000240d0: 6173 6574 0a20 2020 2055 6e73 7472 7563  aset.    Unstruc
-000240e0: 7475 7265 6447 7269 6420 282e 2e2e 290a  turedGrid (...).
-000240f0: 2020 2020 2020 4e20 4365 6c6c 733a 2020        N Cells:  
-00024100: 2020 3131 3732 3932 0a20 2020 2020 204e    117292.      N
-00024110: 2050 6f69 6e74 733a 2020 2031 3837 3033   Points:   18703
-00024120: 370a 2020 2020 2020 5820 426f 756e 6473  7.      X Bounds
-00024130: 3a20 2020 2d36 2e38 3538 652d 3033 2c20  :   -6.858e-03, 
-00024140: 312e 3131 3865 2d30 310a 2020 2020 2020  1.118e-01.      
-00024150: 5920 426f 756e 6473 3a20 2020 2d31 2e32  Y Bounds:   -1.2
-00024160: 3337 652d 3032 2c20 362e 3633 3465 2d30  37e-02, 6.634e-0
-00024170: 320a 2020 2020 2020 5a20 426f 756e 6473  2.      Z Bounds
-00024180: 3a20 2020 2d31 2e36 3338 652d 3032 2c20  :   -1.638e-02, 
-00024190: 312e 3633 3865 2d30 320a 2020 2020 2020  1.638e-02.      
-000241a0: 4e20 4172 7261 7973 3a20 2020 330a 0a20  N Arrays:   3.. 
-000241b0: 2020 2053 686f 7720 7468 6520 6176 6169     Show the avai
-000241c0: 6c61 626c 6520 706f 696e 7420 6461 7461  lable point data
-000241d0: 2061 7272 6179 732e 0a0a 2020 2020 3e3e   arrays...    >>
-000241e0: 3e20 6461 7461 7365 742e 706f 696e 745f  > dataset.point_
-000241f0: 6461 7461 0a20 2020 2070 7976 6973 7461  data.    pyvista
-00024200: 2044 6174 6153 6574 4174 7472 6962 7574   DataSetAttribut
-00024210: 6573 0a20 2020 2041 7373 6f63 6961 7469  es.    Associati
-00024220: 6f6e 2020 2020 203a 2050 4f49 4e54 0a20  on     : POINT. 
-00024230: 2020 2041 6374 6976 6520 5363 616c 6172     Active Scalar
-00024240: 7320 203a 204e 6f6e 650a 2020 2020 4163  s  : None.    Ac
-00024250: 7469 7665 2056 6563 746f 7273 2020 3a20  tive Vectors  : 
-00024260: 4e6f 6e65 0a20 2020 2041 6374 6976 6520  None.    Active 
-00024270: 5465 7874 7572 6520 203a 204e 6f6e 650a  Texture  : None.
-00024280: 2020 2020 4163 7469 7665 204e 6f72 6d61      Active Norma
-00024290: 6c73 2020 3a20 4e6f 6e65 0a20 2020 2043  ls  : None.    C
-000242a0: 6f6e 7461 696e 7320 6172 7261 7973 203a  ontains arrays :
-000242b0: 0a20 2020 2020 2020 2064 6973 706c 6163  .        displac
-000242c0: 656d 656e 7420 2020 2020 2020 2020 2020  ement           
-000242d0: 2066 6c6f 6174 3332 2020 2020 2831 3837   float32    (187
-000242e0: 3033 372c 2033 290a 2020 2020 2020 2020  037, 3).        
-000242f0: 746f 7461 6c20 6e6f 6e6c 696e 6561 7220  total nonlinear 
-00024300: 7374 7261 696e 2020 666c 6f61 7433 3220  strain  float32 
-00024310: 2020 2028 3138 3730 3337 2c20 3629 0a20     (187037, 6). 
-00024320: 2020 2020 2020 2076 6f6e 204d 6973 6573         von Mises
-00024330: 2073 7472 6573 7320 2020 2020 2020 2066   stress        f
-00024340: 6c6f 6174 3332 2020 2020 2831 3837 3033  loat32    (18703
-00024350: 372c 290a 0a20 2020 2050 6c6f 7420 7468  7,)..    Plot th
-00024360: 6520 766f 6e20 4d69 7365 7320 7374 7265  e von Mises stre
-00024370: 7373 2e0a 0a20 2020 203e 3e3e 2063 706f  ss...    >>> cpo
-00024380: 7320 3d20 5b0a 2020 2020 2e2e 2e20 2020  s = [.    ...   
-00024390: 2020 282d 302e 3035 3033 2c20 302e 3133    (-0.0503, 0.13
-000243a0: 322c 202d 302e 3137 3929 2c0a 2020 2020  2, -0.179),.    
-000243b0: 2e2e 2e20 2020 2020 2830 2e30 3530 352c  ...     (0.0505,
-000243c0: 2030 2e30 3138 352c 202d 302e 3030 3230   0.0185, -0.0020
-000243d0: 3129 2c0a 2020 2020 2e2e 2e20 2020 2020  1),.    ...     
-000243e0: 2830 2e32 3735 2c20 302e 3837 322c 2030  (0.275, 0.872, 0
-000243f0: 2e34 3035 292c 0a20 2020 202e 2e2e 205d  .405),.    ... ]
-00024400: 0a20 2020 203e 3e3e 2064 6174 6173 6574  .    >>> dataset
-00024410: 2e70 6c6f 7428 0a20 2020 202e 2e2e 2020  .plot(.    ...  
-00024420: 2020 2073 6d6f 6f74 685f 7368 6164 696e     smooth_shadin
-00024430: 673d 5472 7565 2c0a 2020 2020 2e2e 2e20  g=True,.    ... 
-00024440: 2020 2020 7370 6c69 745f 7368 6172 705f      split_sharp_
-00024450: 6564 6765 733d 5472 7565 2c0a 2020 2020  edges=True,.    
-00024460: 2e2e 2e20 2020 2020 7363 616c 6172 733d  ...     scalars=
-00024470: 2776 6f6e 204d 6973 6573 2073 7472 6573  'von Mises stres
-00024480: 7327 2c0a 2020 2020 2e2e 2e20 2020 2020  s',.    ...     
-00024490: 636d 6170 3d27 6277 7227 2c0a 2020 2020  cmap='bwr',.    
-000244a0: 2e2e 2e20 2020 2020 6370 6f73 3d63 706f  ...     cpos=cpo
-000244b0: 732c 0a20 2020 202e 2e2e 2020 2020 2061  s,.    ...     a
-000244c0: 6e74 695f 616c 6961 7369 6e67 3d27 6678  nti_aliasing='fx
-000244d0: 6161 272c 0a20 2020 202e 2e2e 2029 0a0a  aa',.    ... )..
-000244e0: 2020 2020 2222 220a 2020 2020 7265 7475      """.    retu
-000244f0: 726e 205f 646f 776e 6c6f 6164 5f61 6e64  rn _download_and
-00024500: 5f72 6561 6428 2766 6561 2f61 6572 6f5f  _read('fea/aero_
-00024510: 6272 6163 6b65 742f 6165 726f 5f62 7261  bracket/aero_bra
-00024520: 636b 6574 2e76 7475 272c 206c 6f61 643d  cket.vtu', load=
-00024530: 6c6f 6164 290a 0a0a 6465 6620 646f 776e  load)...def down
-00024540: 6c6f 6164 5f63 6f69 6c5f 6d61 676e 6574  load_coil_magnet
-00024550: 6963 5f66 6965 6c64 286c 6f61 643d 5472  ic_field(load=Tr
-00024560: 7565 293a 2020 2320 7072 6167 6d61 3a20  ue):  # pragma: 
-00024570: 6e6f 2063 6f76 6572 0a20 2020 2022 2222  no cover.    """
-00024580: 446f 776e 6c6f 6164 2074 6865 206d 6167  Download the mag
-00024590: 6e65 7469 6320 6669 656c 6420 6f66 2061  netic field of a
-000245a0: 2063 6f69 6c2e 0a0a 2020 2020 5468 6573   coil...    Thes
-000245b0: 6520 6578 616d 706c 6573 2077 6572 6520  e examples were 
-000245c0: 6765 6e65 7261 7465 6420 6672 6f6d 2074  generated from t
-000245d0: 6865 2066 6f6c 6c6f 7769 6e67 2060 7363  he following `sc
-000245e0: 7269 7074 0a20 2020 203c 6874 7470 733a  ript.    <https:
-000245f0: 2f2f 6769 7468 7562 2e63 6f6d 2f70 7976  //github.com/pyv
-00024600: 6973 7461 2f76 746b 2d64 6174 612f 7472  ista/vtk-data/tr
-00024610: 6565 2f6d 6173 7465 722f 4461 7461 2f6d  ee/master/Data/m
-00024620: 6167 7079 6c69 622f 3e60 5f2e 0a0a 2020  agpylib/>`_...  
-00024630: 2020 5061 7261 6d65 7465 7273 0a20 2020    Parameters.   
-00024640: 202d 2d2d 2d2d 2d2d 2d2d 2d0a 2020 2020   ----------.    
-00024650: 6c6f 6164 203a 2062 6f6f 6c2c 2064 6566  load : bool, def
-00024660: 6175 6c74 3a20 5472 7565 0a20 2020 2020  ault: True.     
-00024670: 2020 204c 6f61 6420 7468 6520 6461 7461     Load the data
-00024680: 7365 7420 6166 7465 7220 646f 776e 6c6f  set after downlo
-00024690: 6164 696e 6720 6974 2077 6865 6e20 6060  ading it when ``
-000246a0: 5472 7565 6060 2e20 2053 6574 2074 6869  True``.  Set thi
-000246b0: 730a 2020 2020 2020 2020 746f 2060 6046  s.        to ``F
-000246c0: 616c 7365 6060 2061 6e64 206f 6e6c 7920  alse`` and only 
-000246d0: 7468 6520 6669 6c65 6e61 6d65 2077 696c  the filename wil
-000246e0: 6c20 6265 2072 6574 7572 6e65 642e 0a0a  l be returned...
-000246f0: 2020 2020 5265 7475 726e 730a 2020 2020      Returns.    
-00024700: 2d2d 2d2d 2d2d 2d0a 2020 2020 7079 7669  -------.    pyvi
-00024710: 7374 612e 496d 6167 6544 6174 6120 6f72  sta.ImageData or
-00024720: 2073 7472 0a20 2020 2020 2020 2044 6174   str.        Dat
-00024730: 6153 6574 206f 7220 6669 6c65 6e61 6d65  aSet or filename
-00024740: 2064 6570 656e 6469 6e67 206f 6e20 6060   depending on ``
-00024750: 6c6f 6164 6060 2e0a 0a20 2020 2045 7861  load``...    Exa
-00024760: 6d70 6c65 730a 2020 2020 2d2d 2d2d 2d2d  mples.    ------
-00024770: 2d2d 0a20 2020 2044 6f77 6e6c 6f61 6420  --.    Download 
-00024780: 7468 6520 6d61 676e 6574 6963 2066 6965  the magnetic fie
-00024790: 6c64 2064 6174 6173 6574 2061 6e64 2067  ld dataset and g
-000247a0: 656e 6572 6174 6520 7374 7265 616d 6c69  enerate streamli
-000247b0: 6e65 7320 6672 6f6d 2074 6865 2066 6965  nes from the fie
-000247c0: 6c64 2e0a 0a20 2020 203e 3e3e 2069 6d70  ld...    >>> imp
-000247d0: 6f72 7420 7079 7669 7374 6120 6173 2070  ort pyvista as p
-000247e0: 760a 2020 2020 3e3e 3e20 6672 6f6d 2070  v.    >>> from p
-000247f0: 7976 6973 7461 2069 6d70 6f72 7420 6578  yvista import ex
-00024800: 616d 706c 6573 0a20 2020 203e 3e3e 2067  amples.    >>> g
-00024810: 7269 6420 3d20 6578 616d 706c 6573 2e64  rid = examples.d
-00024820: 6f77 6e6c 6f61 645f 636f 696c 5f6d 6167  ownload_coil_mag
-00024830: 6e65 7469 635f 6669 656c 6428 290a 2020  netic_field().  
-00024840: 2020 3e3e 3e20 7365 6564 203d 2070 762e    >>> seed = pv.
-00024850: 4469 7363 2869 6e6e 6572 3d31 2c20 6f75  Disc(inner=1, ou
-00024860: 7465 723d 352e 322c 2072 5f72 6573 3d33  ter=5.2, r_res=3
-00024870: 2c20 635f 7265 733d 3132 290a 2020 2020  , c_res=12).    
-00024880: 3e3e 3e20 7374 726c 203d 2067 7269 642e  >>> strl = grid.
-00024890: 7374 7265 616d 6c69 6e65 735f 6672 6f6d  streamlines_from
-000248a0: 5f73 6f75 7263 6528 0a20 2020 202e 2e2e  _source(.    ...
-000248b0: 2020 2020 2073 6565 642c 0a20 2020 202e       seed,.    .
-000248c0: 2e2e 2020 2020 2076 6563 746f 7273 3d27  ..     vectors='
-000248d0: 4227 2c0a 2020 2020 2e2e 2e20 2020 2020  B',.    ...     
-000248e0: 6d61 785f 7469 6d65 3d31 3830 2c0a 2020  max_time=180,.  
-000248f0: 2020 2e2e 2e20 2020 2020 696e 6974 6961    ...     initia
-00024900: 6c5f 7374 6570 5f6c 656e 6774 683d 302e  l_step_length=0.
-00024910: 312c 0a20 2020 202e 2e2e 2020 2020 2069  1,.    ...     i
-00024920: 6e74 6567 7261 7469 6f6e 5f64 6972 6563  ntegration_direc
-00024930: 7469 6f6e 3d27 626f 7468 272c 0a20 2020  tion='both',.   
-00024940: 202e 2e2e 2029 0a20 2020 203e 3e3e 2073   ... ).    >>> s
-00024950: 7472 6c2e 706c 6f74 280a 2020 2020 2e2e  trl.plot(.    ..
-00024960: 2e20 2020 2020 636d 6170 3d27 706c 6173  .     cmap='plas
-00024970: 6d61 272c 0a20 2020 202e 2e2e 2020 2020  ma',.    ...    
-00024980: 2072 656e 6465 725f 6c69 6e65 735f 6173   render_lines_as
-00024990: 5f74 7562 6573 3d54 7275 652c 0a20 2020  _tubes=True,.   
-000249a0: 202e 2e2e 2020 2020 206c 696e 655f 7769   ...     line_wi
-000249b0: 6474 683d 322c 0a20 2020 202e 2e2e 2020  dth=2,.    ...  
-000249c0: 2020 206c 6967 6874 696e 673d 4661 6c73     lighting=Fals
-000249d0: 652c 0a20 2020 202e 2e2e 2020 2020 207a  e,.    ...     z
-000249e0: 6f6f 6d3d 322c 0a20 2020 202e 2e2e 2029  oom=2,.    ... )
-000249f0: 0a0a 2020 2020 506c 6f74 2074 6865 206d  ..    Plot the m
-00024a00: 6167 6e65 7420 6669 656c 6420 7374 7265  agnet field stre
-00024a10: 6e67 7468 2069 6e20 7468 6520 5a20 6469  ngth in the Z di
-00024a20: 7265 6374 696f 6e2e 0a0a 2020 2020 3e3e  rection...    >>
-00024a30: 3e20 696d 706f 7274 206e 756d 7079 2061  > import numpy a
-00024a40: 7320 6e70 0a20 2020 203e 3e3e 2069 6d70  s np.    >>> imp
-00024a50: 6f72 7420 7079 7669 7374 6120 6173 2070  ort pyvista as p
-00024a60: 760a 2020 2020 3e3e 3e20 6672 6f6d 2070  v.    >>> from p
-00024a70: 7976 6973 7461 2069 6d70 6f72 7420 6578  yvista import ex
-00024a80: 616d 706c 6573 0a20 2020 203e 3e3e 2067  amples.    >>> g
-00024a90: 7269 6420 3d20 6578 616d 706c 6573 2e64  rid = examples.d
-00024aa0: 6f77 6e6c 6f61 645f 636f 696c 5f6d 6167  ownload_coil_mag
-00024ab0: 6e65 7469 635f 6669 656c 6428 290a 2020  netic_field().  
-00024ac0: 2020 3e3e 3e20 2320 6372 6561 7465 2063    >>> # create c
-00024ad0: 6f69 6c73 0a20 2020 203e 3e3e 2063 6f69  oils.    >>> coi
-00024ae0: 6c73 203d 205b 5d0a 2020 2020 3e3e 3e20  ls = [].    >>> 
-00024af0: 666f 7220 7a20 696e 206e 702e 6c69 6e73  for z in np.lins
-00024b00: 7061 6365 282d 382c 2038 2c20 3136 293a  pace(-8, 8, 16):
-00024b10: 0a20 2020 202e 2e2e 2020 2020 2063 6f69  .    ...     coi
-00024b20: 6c73 2e61 7070 656e 6428 0a20 2020 202e  ls.append(.    .
-00024b30: 2e2e 2020 2020 2020 2020 2070 762e 506f  ..         pv.Po
-00024b40: 6c79 676f 6e28 2830 2c20 302c 207a 292c  lygon((0, 0, z),
-00024b50: 2072 6164 6975 733d 352c 206e 5f73 6964   radius=5, n_sid
-00024b60: 6573 3d31 3030 2c20 6669 6c6c 3d46 616c  es=100, fill=Fal
-00024b70: 7365 290a 2020 2020 2e2e 2e20 2020 2020  se).    ...     
-00024b80: 290a 2020 2020 2e2e 2e0a 2020 2020 3e3e  ).    ....    >>
-00024b90: 3e20 636f 696c 7320 3d20 7076 2e4d 756c  > coils = pv.Mul
-00024ba0: 7469 426c 6f63 6b28 636f 696c 7329 0a20  tiBlock(coils). 
-00024bb0: 2020 203e 3e3e 2023 2070 6c6f 7420 7468     >>> # plot th
-00024bc0: 6520 6d61 676e 6574 2066 6965 6c64 2073  e magnet field s
-00024bd0: 7472 656e 6774 6820 696e 2074 6865 205a  trength in the Z
-00024be0: 2064 6972 6563 7469 6f6e 0a20 2020 203e   direction.    >
-00024bf0: 3e3e 2073 6361 6c61 7273 203d 206e 702e  >> scalars = np.
-00024c00: 6162 7328 6772 6964 5b27 4227 5d5b 3a2c  abs(grid['B'][:,
-00024c10: 2032 5d29 0a20 2020 203e 3e3e 2070 6c20   2]).    >>> pl 
-00024c20: 3d20 7076 2e50 6c6f 7474 6572 2829 0a20  = pv.Plotter(). 
-00024c30: 2020 203e 3e3e 205f 203d 2070 6c2e 6164     >>> _ = pl.ad
-00024c40: 645f 6d65 7368 280a 2020 2020 2e2e 2e20  d_mesh(.    ... 
-00024c50: 2020 2020 636f 696c 732c 2072 656e 6465      coils, rende
-00024c60: 725f 6c69 6e65 735f 6173 5f74 7562 6573  r_lines_as_tubes
-00024c70: 3d54 7275 652c 206c 696e 655f 7769 6474  =True, line_widt
-00024c80: 683d 352c 2063 6f6c 6f72 3d27 7727 0a20  h=5, color='w'. 
-00024c90: 2020 202e 2e2e 2029 0a20 2020 203e 3e3e     ... ).    >>>
-00024ca0: 2076 6f6c 203d 2070 6c2e 6164 645f 766f   vol = pl.add_vo
-00024cb0: 6c75 6d65 280a 2020 2020 2e2e 2e20 2020  lume(.    ...   
-00024cc0: 2020 6772 6964 2c0a 2020 2020 2e2e 2e20    grid,.    ... 
-00024cd0: 2020 2020 7363 616c 6172 733d 7363 616c      scalars=scal
-00024ce0: 6172 732c 0a20 2020 202e 2e2e 2020 2020  ars,.    ...    
-00024cf0: 2063 6d61 703d 2770 6c61 736d 6127 2c0a   cmap='plasma',.
-00024d00: 2020 2020 2e2e 2e20 2020 2020 7368 6f77      ...     show
-00024d10: 5f73 6361 6c61 725f 6261 723d 4661 6c73  _scalar_bar=Fals
-00024d20: 652c 0a20 2020 202e 2e2e 2020 2020 206c  e,.    ...     l
-00024d30: 6f67 5f73 6361 6c65 3d54 7275 652c 0a20  og_scale=True,. 
-00024d40: 2020 202e 2e2e 2020 2020 206f 7061 6369     ...     opaci
-00024d50: 7479 3d27 7369 676d 6f69 645f 3227 2c0a  ty='sigmoid_2',.
-00024d60: 2020 2020 2e2e 2e20 290a 2020 2020 3e3e      ... ).    >>
-00024d70: 3e20 766f 6c2e 7072 6f70 2e69 6e74 6572  > vol.prop.inter
-00024d80: 706f 6c61 7469 6f6e 5f74 7970 6520 3d20  polation_type = 
-00024d90: 276c 696e 6561 7227 0a20 2020 203e 3e3e  'linear'.    >>>
-00024da0: 205f 203d 2070 6c2e 6164 645f 766f 6c75   _ = pl.add_volu
-00024db0: 6d65 5f63 6c69 705f 706c 616e 6528 0a20  me_clip_plane(. 
-00024dc0: 2020 202e 2e2e 2020 2020 2076 6f6c 2c0a     ...     vol,.
-00024dd0: 2020 2020 2e2e 2e20 2020 2020 6e6f 726d      ...     norm
-00024de0: 616c 3d27 2d78 272c 0a20 2020 202e 2e2e  al='-x',.    ...
-00024df0: 2020 2020 206e 6f72 6d61 6c5f 726f 7461       normal_rota
-00024e00: 7469 6f6e 3d46 616c 7365 2c0a 2020 2020  tion=False,.    
-00024e10: 2e2e 2e20 2020 2020 696e 7465 7261 6374  ...     interact
-00024e20: 696f 6e5f 6576 656e 743d 2761 6c77 6179  ion_event='alway
-00024e30: 7327 2c0a 2020 2020 2e2e 2e20 2020 2020  s',.    ...     
-00024e40: 7769 6467 6574 5f63 6f6c 6f72 3d70 762e  widget_color=pv.
-00024e50: 436f 6c6f 7228 6f70 6163 6974 793d 302e  Color(opacity=0.
-00024e60: 3029 2c0a 2020 2020 2e2e 2e20 290a 2020  0),.    ... ).  
-00024e70: 2020 3e3e 3e20 706c 2e65 6e61 626c 655f    >>> pl.enable_
-00024e80: 616e 7469 5f61 6c69 6173 696e 6728 290a  anti_aliasing().
-00024e90: 2020 2020 3e3e 3e20 706c 2e63 616d 6572      >>> pl.camer
-00024ea0: 612e 7a6f 6f6d 2832 290a 2020 2020 3e3e  a.zoom(2).    >>
-00024eb0: 3e20 706c 2e73 686f 7728 290a 0a20 2020  > pl.show()..   
-00024ec0: 2053 6565 2074 6865 203a 7265 663a 606d   See the :ref:`m
-00024ed0: 6167 6e65 7469 635f 6669 656c 6473 5f65  agnetic_fields_e
-00024ee0: 7861 6d70 6c65 6020 666f 7220 6d6f 7265  xample` for more
-00024ef0: 2064 6574 6169 6c73 206f 6e20 686f 7720   details on how 
-00024f00: 746f 2070 6c6f 7420 7769 7468 0a20 2020  to plot with.   
-00024f10: 2074 6869 7320 6461 7461 7365 742e 0a0a   this dataset...
-00024f20: 2020 2020 2222 220a 2020 2020 7265 7475      """.    retu
-00024f30: 726e 205f 646f 776e 6c6f 6164 5f61 6e64  rn _download_and
-00024f40: 5f72 6561 6428 276d 6167 7079 6c69 622f  _read('magpylib/
-00024f50: 636f 696c 5f66 6965 6c64 2e76 7469 272c  coil_field.vti',
-00024f60: 206c 6f61 643d 6c6f 6164 290a 0a0a 6465   load=load)...de
-00024f70: 6620 646f 776e 6c6f 6164 5f6d 6573 6869  f download_meshi
-00024f80: 6f5f 7864 6d66 286c 6f61 643d 5472 7565  o_xdmf(load=True
-00024f90: 293a 2020 2320 7072 6167 6d61 3a20 6e6f  ):  # pragma: no
-00024fa0: 2063 6f76 6572 0a20 2020 2022 2222 446f   cover.    """Do
-00024fb0: 776e 6c6f 6164 2078 646d 6620 6669 6c65  wnload xdmf file
-00024fc0: 2063 7265 6174 6564 2062 7920 6d65 7368   created by mesh
-00024fd0: 696f 2e0a 0a20 2020 2054 6865 2064 6174  io...    The dat
-00024fe0: 6173 6574 2077 6173 2063 7265 6174 6564  aset was created
-00024ff0: 2062 7920 6060 7465 7374 5f74 696d 655f   by ``test_time_
-00025000: 7365 7269 6573 6060 2074 6573 7420 6675  series`` test fu
-00025010: 6e63 7469 6f6e 2069 6e20 6d65 7368 696f  nction in meshio
-00025020: 2e0a 0a20 2020 2050 6172 616d 6574 6572  ...    Parameter
-00025030: 730a 2020 2020 2d2d 2d2d 2d2d 2d2d 2d2d  s.    ----------
-00025040: 0a20 2020 206c 6f61 6420 3a20 626f 6f6c  .    load : bool
-00025050: 2c20 6465 6661 756c 743a 2054 7275 650a  , default: True.
-00025060: 2020 2020 2020 2020 4c6f 6164 2074 6865          Load the
-00025070: 2064 6174 6173 6574 2061 6674 6572 2064   dataset after d
-00025080: 6f77 6e6c 6f61 6469 6e67 2069 7420 7768  ownloading it wh
-00025090: 656e 2060 6054 7275 6560 602e 2020 5365  en ``True``.  Se
-000250a0: 7420 7468 6973 0a20 2020 2020 2020 2074  t this.        t
-000250b0: 6f20 6060 4661 6c73 6560 6020 616e 6420  o ``False`` and 
-000250c0: 6f6e 6c79 2074 6865 2066 696c 656e 616d  only the filenam
-000250d0: 6520 7769 6c6c 2062 6520 7265 7475 726e  e will be return
-000250e0: 6564 2e0a 0a20 2020 2052 6574 7572 6e73  ed...    Returns
-000250f0: 0a20 2020 202d 2d2d 2d2d 2d2d 0a20 2020  .    -------.   
-00025100: 2070 7976 6973 7461 2e55 6e73 7472 7563   pyvista.Unstruc
-00025110: 7475 7265 6447 7269 6420 6f72 2073 7472  turedGrid or str
-00025120: 0a20 2020 2020 2020 2044 6174 6153 6574  .        DataSet
-00025130: 206f 7220 6669 6c65 6e61 6d65 2064 6570   or filename dep
-00025140: 656e 6469 6e67 206f 6e20 6060 6c6f 6164  ending on ``load
-00025150: 6060 2e0a 0a20 2020 2045 7861 6d70 6c65  ``...    Example
-00025160: 730a 2020 2020 2d2d 2d2d 2d2d 2d2d 0a20  s.    --------. 
-00025170: 2020 203e 3e3e 2066 726f 6d20 7079 7669     >>> from pyvi
-00025180: 7374 6120 696d 706f 7274 2065 7861 6d70  sta import examp
-00025190: 6c65 730a 2020 2020 3e3e 3e20 6461 7461  les.    >>> data
-000251a0: 7365 7420 3d20 6578 616d 706c 6573 2e64  set = examples.d
-000251b0: 6f77 6e6c 6f61 645f 6d65 7368 696f 5f78  ownload_meshio_x
-000251c0: 646d 6628 290a 2020 2020 3e3e 3e20 6461  dmf().    >>> da
-000251d0: 7461 7365 742e 706c 6f74 2829 0a0a 2020  taset.plot()..  
-000251e0: 2020 2222 220a 2020 2020 5f20 3d20 646f    """.    _ = do
-000251f0: 776e 6c6f 6164 5f66 696c 6528 226d 6573  wnload_file("mes
-00025200: 6869 6f2f 6f75 742e 6835 2229 0a20 2020  hio/out.h5").   
-00025210: 2072 6574 7572 6e20 5f64 6f77 6e6c 6f61   return _downloa
-00025220: 645f 616e 645f 7265 6164 2822 6d65 7368  d_and_read("mesh
-00025230: 696f 2f6f 7574 2e78 646d 6622 2c20 6c6f  io/out.xdmf", lo
-00025240: 6164 3d6c 6f61 6429 0a                   ad=load).
+000199e0: 736d 6e78 2020 2320 6e6f 7161 3a20 4634  smnx  # noqa: F4
+000199f0: 3031 0a20 2020 2065 7863 6570 7420 496d  01.    except Im
+00019a00: 706f 7274 4572 726f 723a 0a20 2020 2020  portError:.     
+00019a10: 2020 2072 6169 7365 2049 6d70 6f72 7445     raise ImportE
+00019a20: 7272 6f72 2827 496e 7374 616c 6c20 606f  rror('Install `o
+00019a30: 736d 6e78 6020 746f 2075 7365 2074 6869  smnx` to use thi
+00019a40: 7320 6578 616d 706c 6527 290a 0a20 2020  s example')..   
+00019a50: 2066 696c 656e 616d 6520 3d20 646f 776e   filename = down
+00019a60: 6c6f 6164 5f66 696c 6528 276f 736d 6e78  load_file('osmnx
+00019a70: 5f67 7261 7068 2e70 2729 0a20 2020 2072  _graph.p').    r
+00019a80: 6574 7572 6e20 7069 636b 6c65 2e6c 6f61  eturn pickle.loa
+00019a90: 6428 6f70 656e 2866 696c 656e 616d 652c  d(open(filename,
+00019aa0: 2027 7262 2729 290a 0a0a 6465 6620 646f   'rb'))...def do
+00019ab0: 776e 6c6f 6164 5f63 6176 6974 7928 6c6f  wnload_cavity(lo
+00019ac0: 6164 3d54 7275 6529 3a20 2023 2070 7261  ad=True):  # pra
+00019ad0: 676d 613a 206e 6f20 636f 7665 720a 2020  gma: no cover.  
+00019ae0: 2020 2222 2244 6f77 6e6c 6f61 6420 6361    """Download ca
+00019af0: 7669 7479 204f 7065 6e46 4f41 4d20 6578  vity OpenFOAM ex
+00019b00: 616d 706c 652e 0a0a 2020 2020 5265 7472  ample...    Retr
+00019b10: 6965 7665 6420 6672 6f6d 0a20 2020 2060  ieved from.    `
+00019b20: 4b69 7477 6172 6520 5654 4b20 4461 7461  Kitware VTK Data
+00019b30: 203c 6874 7470 733a 2f2f 6461 7461 2e6b   <https://data.k
+00019b40: 6974 7761 7265 2e63 6f6d 2f23 636f 6c6c  itware.com/#coll
+00019b50: 6563 7469 6f6e 2f35 3566 3137 6637 3538  ection/55f17f758
+00019b60: 6437 3737 6636 6464 6337 3839 3562 372f  d777f6ddc7895b7/
+00019b70: 666f 6c64 6572 2f35 6166 6439 3332 6538  folder/5afd932e8
+00019b80: 6437 3737 6631 3565 6265 3162 3138 333e  d777f15ebe1b183>
+00019b90: 605f 2e0a 0a20 2020 2050 6172 616d 6574  `_...    Paramet
+00019ba0: 6572 730a 2020 2020 2d2d 2d2d 2d2d 2d2d  ers.    --------
+00019bb0: 2d2d 0a20 2020 206c 6f61 6420 3a20 626f  --.    load : bo
+00019bc0: 6f6c 2c20 6465 6661 756c 743a 2054 7275  ol, default: Tru
+00019bd0: 650a 2020 2020 2020 2020 4c6f 6164 2074  e.        Load t
+00019be0: 6865 2064 6174 6173 6574 2061 6674 6572  he dataset after
+00019bf0: 2064 6f77 6e6c 6f61 6469 6e67 2069 7420   downloading it 
+00019c00: 7768 656e 2060 6054 7275 6560 602e 2020  when ``True``.  
+00019c10: 5365 7420 7468 6973 0a20 2020 2020 2020  Set this.       
+00019c20: 2074 6f20 6060 4661 6c73 6560 6020 616e   to ``False`` an
+00019c30: 6420 6f6e 6c79 2074 6865 2066 696c 656e  d only the filen
+00019c40: 616d 6520 7769 6c6c 2062 6520 7265 7475  ame will be retu
+00019c50: 726e 6564 2e0a 0a20 2020 2052 6574 7572  rned...    Retur
+00019c60: 6e73 0a20 2020 202d 2d2d 2d2d 2d2d 0a20  ns.    -------. 
+00019c70: 2020 2070 7976 6973 7461 2e4d 756c 7469     pyvista.Multi
+00019c80: 426c 6f63 6b20 7c20 7374 720a 2020 2020  Block | str.    
+00019c90: 2020 2020 4461 7461 5365 7420 6f72 2066      DataSet or f
+00019ca0: 696c 656e 616d 6520 6465 7065 6e64 696e  ilename dependin
+00019cb0: 6720 6f6e 2060 606c 6f61 6460 602e 0a0a  g on ``load``...
+00019cc0: 2020 2020 4578 616d 706c 6573 0a20 2020      Examples.   
+00019cd0: 202d 2d2d 2d2d 2d2d 2d0a 2020 2020 3e3e   --------.    >>
+00019ce0: 3e20 6672 6f6d 2070 7976 6973 7461 2069  > from pyvista i
+00019cf0: 6d70 6f72 7420 6578 616d 706c 6573 0a20  mport examples. 
+00019d00: 2020 203e 3e3e 2064 6174 6173 6574 203d     >>> dataset =
+00019d10: 2065 7861 6d70 6c65 732e 646f 776e 6c6f   examples.downlo
+00019d20: 6164 5f63 6176 6974 7928 2920 2023 2064  ad_cavity()  # d
+00019d30: 6f63 7465 7374 3a2b 534b 4950 0a0a 2020  octest:+SKIP..  
+00019d40: 2020 5365 6520 3a72 6566 3a60 6f70 656e    See :ref:`open
+00019d50: 666f 616d 5f65 7861 6d70 6c65 6020 666f  foam_example` fo
+00019d60: 7220 6120 6675 6c6c 2065 7861 6d70 6c65  r a full example
+00019d70: 2075 7369 6e67 2074 6869 7320 6461 7461   using this data
+00019d80: 7365 742e 0a0a 2020 2020 2222 220a 2020  set...    """.  
+00019d90: 2020 6669 6c65 6e61 6d65 203d 205f 646f    filename = _do
+00019da0: 776e 6c6f 6164 5f61 7263 6869 7665 2827  wnload_archive('
+00019db0: 4f70 656e 464f 414d 2e7a 6970 272c 2074  OpenFOAM.zip', t
+00019dc0: 6172 6765 745f 6669 6c65 3d27 6361 7669  arget_file='cavi
+00019dd0: 7479 2f63 6173 652e 666f 616d 2729 0a20  ty/case.foam'). 
+00019de0: 2020 2069 6620 6e6f 7420 6c6f 6164 3a0a     if not load:.
+00019df0: 2020 2020 2020 2020 7265 7475 726e 2066          return f
+00019e00: 696c 656e 616d 650a 2020 2020 7265 7475  ilename.    retu
+00019e10: 726e 2070 7976 6973 7461 2e4f 7065 6e46  rn pyvista.OpenF
+00019e20: 4f41 4d52 6561 6465 7228 6669 6c65 6e61  OAMReader(filena
+00019e30: 6d65 292e 7265 6164 2829 0a0a 0a64 6566  me).read()...def
+00019e40: 2064 6f77 6e6c 6f61 645f 6f70 656e 666f   download_openfo
+00019e50: 616d 5f74 7562 6573 286c 6f61 643d 5472  am_tubes(load=Tr
+00019e60: 7565 293a 2020 2320 7072 6167 6d61 3a20  ue):  # pragma: 
+00019e70: 6e6f 2063 6f76 6572 0a20 2020 2022 2222  no cover.    """
+00019e80: 446f 776e 6c6f 6164 2074 7562 6573 204f  Download tubes O
+00019e90: 7065 6e46 4f41 4d20 6578 616d 706c 652e  penFOAM example.
+00019ea0: 0a0a 2020 2020 4461 7461 2067 656e 6572  ..    Data gener
+00019eb0: 6174 6564 2066 726f 6d20 7075 626c 6963  ated from public
+00019ec0: 2053 696d 5363 616c 6520 6578 616d 706c   SimScale exampl
+00019ed0: 6573 2061 7420 6053 696d 5363 616c 6520  es at `SimScale 
+00019ee0: 5072 6f6a 6563 7420 4c69 6272 6172 7920  Project Library 
+00019ef0: 2d0a 2020 2020 5475 7262 6f20 3c68 7474  -.    Turbo <htt
+00019f00: 7073 3a2f 2f77 7777 2e73 696d 7363 616c  ps://www.simscal
+00019f10: 652e 636f 6d2f 7072 6f6a 6563 7473 2f61  e.com/projects/a
+00019f20: 7961 726e 6f7a 2f74 7572 626f 2f3e 605f  yarnoz/turbo/>`_
+00019f30: 2e0a 0a20 2020 204c 6963 656e 7369 6e67  ...    Licensing
+00019f40: 2066 6f72 2074 6869 7320 6461 7461 7365   for this datase
+00019f50: 7420 6973 2067 7261 6e74 6564 2074 6f20  t is granted to 
+00019f60: 6672 6565 6c79 2061 6e64 2077 6974 686f  freely and witho
+00019f70: 7574 2072 6573 7472 6963 7469 6f6e 0a20  ut restriction. 
+00019f80: 2020 2072 6570 726f 6475 6365 2c20 6469     reproduce, di
+00019f90: 7374 7269 6275 7465 2c20 7075 626c 6973  stribute, publis
+00019fa0: 6820 6163 636f 7264 696e 6720 746f 2074  h according to t
+00019fb0: 6865 2060 5369 6d53 6361 6c65 2054 6572  he `SimScale Ter
+00019fc0: 6d73 2061 6e64 0a20 2020 2043 6f6e 6469  ms and.    Condi
+00019fd0: 7469 6f6e 7320 3c68 7474 7073 3a2f 2f77  tions <https://w
+00019fe0: 7777 2e73 696d 7363 616c 652e 636f 6d2f  ww.simscale.com/
+00019ff0: 7465 726d 732d 616e 642d 636f 6e64 6974  terms-and-condit
+0001a000: 696f 6e73 2f3e 605f 2e0a 0a20 2020 2050  ions/>`_...    P
+0001a010: 6172 616d 6574 6572 730a 2020 2020 2d2d  arameters.    --
+0001a020: 2d2d 2d2d 2d2d 2d2d 0a20 2020 206c 6f61  --------.    loa
+0001a030: 6420 3a20 626f 6f6c 2c20 6465 6661 756c  d : bool, defaul
+0001a040: 743a 2054 7275 650a 2020 2020 2020 2020  t: True.        
+0001a050: 4c6f 6164 2074 6865 2064 6174 6173 6574  Load the dataset
+0001a060: 2061 6674 6572 2064 6f77 6e6c 6f61 6469   after downloadi
+0001a070: 6e67 2069 7420 7768 656e 2060 6054 7275  ng it when ``Tru
+0001a080: 6560 602e 2020 5365 7420 7468 6973 0a20  e``.  Set this. 
+0001a090: 2020 2020 2020 2074 6f20 6060 4661 6c73         to ``Fals
+0001a0a0: 6560 6020 616e 6420 6f6e 6c79 2074 6865  e`` and only the
+0001a0b0: 2066 696c 656e 616d 6520 7769 6c6c 2062   filename will b
+0001a0c0: 6520 7265 7475 726e 6564 2e0a 0a20 2020  e returned...   
+0001a0d0: 2052 6574 7572 6e73 0a20 2020 202d 2d2d   Returns.    ---
+0001a0e0: 2d2d 2d2d 0a20 2020 2070 7976 6973 7461  ----.    pyvista
+0001a0f0: 2e4d 756c 7469 426c 6f63 6b20 7c20 7374  .MultiBlock | st
+0001a100: 720a 2020 2020 2020 2020 4461 7461 5365  r.        DataSe
+0001a110: 7420 6f72 2066 696c 656e 616d 6520 6465  t or filename de
+0001a120: 7065 6e64 696e 6720 6f6e 2060 606c 6f61  pending on ``loa
+0001a130: 6460 602e 0a0a 2020 2020 4578 616d 706c  d``...    Exampl
+0001a140: 6573 0a20 2020 202d 2d2d 2d2d 2d2d 2d0a  es.    --------.
+0001a150: 2020 2020 506c 6f74 2074 6865 206f 7574      Plot the out
+0001a160: 6c69 6e65 206f 6620 7468 6520 6461 7461  line of the data
+0001a170: 7365 7420 616c 6f6e 6720 7769 7468 2061  set along with a
+0001a180: 2063 726f 7373 2073 6563 7469 6f6e 206f   cross section o
+0001a190: 6620 7468 6520 666c 6f77 2076 656c 6f63  f the flow veloc
+0001a1a0: 6974 792e 0a0a 2020 2020 3e3e 3e20 696d  ity...    >>> im
+0001a1b0: 706f 7274 2070 7976 6973 7461 2061 7320  port pyvista as 
+0001a1c0: 7076 0a20 2020 203e 3e3e 2066 726f 6d20  pv.    >>> from 
+0001a1d0: 7079 7669 7374 6120 696d 706f 7274 2065  pyvista import e
+0001a1e0: 7861 6d70 6c65 730a 2020 2020 3e3e 3e20  xamples.    >>> 
+0001a1f0: 6461 7461 7365 7420 3d20 6578 616d 706c  dataset = exampl
+0001a200: 6573 2e64 6f77 6e6c 6f61 645f 6f70 656e  es.download_open
+0001a210: 666f 616d 5f74 7562 6573 2829 0a20 2020  foam_tubes().   
+0001a220: 203e 3e3e 2061 6972 203d 2064 6174 6173   >>> air = datas
+0001a230: 6574 5b30 5d0a 2020 2020 3e3e 3e20 795f  et[0].    >>> y_
+0001a240: 736c 6963 6520 3d20 6169 722e 736c 6963  slice = air.slic
+0001a250: 6528 2779 2729 0a20 2020 203e 3e3e 2070  e('y').    >>> p
+0001a260: 6c20 3d20 7076 2e50 6c6f 7474 6572 2829  l = pv.Plotter()
+0001a270: 0a20 2020 203e 3e3e 205f 203d 2070 6c2e  .    >>> _ = pl.
+0001a280: 6164 645f 6d65 7368 280a 2020 2020 2e2e  add_mesh(.    ..
+0001a290: 2e20 2020 2020 795f 736c 6963 652c 0a20  .     y_slice,. 
+0001a2a0: 2020 202e 2e2e 2020 2020 2073 6361 6c61     ...     scala
+0001a2b0: 7273 3d27 5527 2c0a 2020 2020 2e2e 2e20  rs='U',.    ... 
+0001a2c0: 2020 2020 6c69 6768 7469 6e67 3d46 616c      lighting=Fal
+0001a2d0: 7365 2c0a 2020 2020 2e2e 2e20 2020 2020  se,.    ...     
+0001a2e0: 7363 616c 6172 5f62 6172 5f61 7267 733d  scalar_bar_args=
+0001a2f0: 7b27 7469 746c 6527 3a20 2746 6c6f 7720  {'title': 'Flow 
+0001a300: 5665 6c6f 6369 7479 277d 2c0a 2020 2020  Velocity'},.    
+0001a310: 2e2e 2e20 290a 2020 2020 3e3e 3e20 5f20  ... ).    >>> _ 
+0001a320: 3d20 706c 2e61 6464 5f6d 6573 6828 6169  = pl.add_mesh(ai
+0001a330: 722c 2063 6f6c 6f72 3d27 7727 2c20 6f70  r, color='w', op
+0001a340: 6163 6974 793d 302e 3235 290a 2020 2020  acity=0.25).    
+0001a350: 3e3e 3e20 706c 2e65 6e61 626c 655f 616e  >>> pl.enable_an
+0001a360: 7469 5f61 6c69 6173 696e 6728 290a 2020  ti_aliasing().  
+0001a370: 2020 3e3e 3e20 706c 2e73 686f 7728 290a    >>> pl.show().
+0001a380: 0a20 2020 2053 6565 203a 7265 663a 606f  .    See :ref:`o
+0001a390: 7065 6e66 6f61 6d5f 7475 6265 735f 6578  penfoam_tubes_ex
+0001a3a0: 616d 706c 6560 2066 6f72 2061 2066 756c  ample` for a ful
+0001a3b0: 6c20 6578 616d 706c 6520 7573 696e 6720  l example using 
+0001a3c0: 7468 6973 2064 6174 6173 6574 2e0a 0a20  this dataset... 
+0001a3d0: 2020 2022 2222 0a20 2020 2066 696c 656e     """.    filen
+0001a3e0: 616d 6520 3d20 5f64 6f77 6e6c 6f61 645f  ame = _download_
+0001a3f0: 6172 6368 6976 6528 0a20 2020 2020 2020  archive(.       
+0001a400: 2027 6676 6d2f 7475 7262 6f5f 696e 636f   'fvm/turbo_inco
+0001a410: 6d70 7265 7373 6962 6c65 2f54 7572 626f  mpressible/Turbo
+0001a420: 2d49 6e63 6f6d 7072 6573 7369 626c 655f  -Incompressible_
+0001a430: 332d 5275 6e5f 312d 534f 4c55 5449 4f4e  3-Run_1-SOLUTION
+0001a440: 5f46 4945 4c44 532e 7a69 7027 2c0a 2020  _FIELDS.zip',.  
+0001a450: 2020 2020 2020 7461 7267 6574 5f66 696c        target_fil
+0001a460: 653d 2763 6173 652e 666f 616d 272c 0a20  e='case.foam',. 
+0001a470: 2020 2029 0a20 2020 2069 6620 6e6f 7420     ).    if not 
+0001a480: 6c6f 6164 3a0a 2020 2020 2020 2020 7265  load:.        re
+0001a490: 7475 726e 2066 696c 656e 616d 650a 2020  turn filename.  
+0001a4a0: 2020 7265 6164 6572 203d 2070 7976 6973    reader = pyvis
+0001a4b0: 7461 2e4f 7065 6e46 4f41 4d52 6561 6465  ta.OpenFOAMReade
+0001a4c0: 7228 6669 6c65 6e61 6d65 290a 2020 2020  r(filename).    
+0001a4d0: 7265 6164 6572 2e73 6574 5f61 6374 6976  reader.set_activ
+0001a4e0: 655f 7469 6d65 5f76 616c 7565 2831 3030  e_time_value(100
+0001a4f0: 3029 0a20 2020 2072 6574 7572 6e20 7265  0).    return re
+0001a500: 6164 6572 2e72 6561 6428 290a 0a0a 6465  ader.read()...de
+0001a510: 6620 646f 776e 6c6f 6164 5f6c 7563 7928  f download_lucy(
+0001a520: 6c6f 6164 3d54 7275 6529 3a20 2023 2070  load=True):  # p
+0001a530: 7261 676d 613a 206e 6f20 636f 7665 720a  ragma: no cover.
+0001a540: 2020 2020 2222 2244 6f77 6e6c 6f61 6420      """Download 
+0001a550: 7468 6520 6c75 6379 2061 6e67 656c 206d  the lucy angel m
+0001a560: 6573 682e 0a0a 2020 2020 4f72 6967 696e  esh...    Origin
+0001a570: 616c 2064 6f77 6e6c 6f61 6465 6420 6672  al downloaded fr
+0001a580: 6f6d 2074 6865 2060 5468 6520 5374 616e  om the `The Stan
+0001a590: 666f 7264 2033 4420 5363 616e 6e69 6e67  ford 3D Scanning
+0001a5a0: 2052 6570 6f73 6974 6f72 790a 2020 2020   Repository.    
+0001a5b0: 3c68 7474 703a 2f2f 6772 6170 6869 6373  <http://graphics
+0001a5c0: 2e73 7461 6e66 6f72 642e 6564 752f 6461  .stanford.edu/da
+0001a5d0: 7461 2f33 4473 6361 6e72 6570 2f3e 605f  ta/3Dscanrep/>`_
+0001a5e0: 2061 6e64 2064 6563 696d 6174 6564 2074   and decimated t
+0001a5f0: 6f0a 2020 2020 6170 7072 6f78 696d 6174  o.    approximat
+0001a600: 656c 7920 3130 306b 2074 7269 616e 676c  ely 100k triangl
+0001a610: 652e 0a0a 2020 2020 5061 7261 6d65 7465  e...    Paramete
+0001a620: 7273 0a20 2020 202d 2d2d 2d2d 2d2d 2d2d  rs.    ---------
+0001a630: 2d0a 2020 2020 6c6f 6164 203a 2062 6f6f  -.    load : boo
+0001a640: 6c2c 2064 6566 6175 6c74 3a20 5472 7565  l, default: True
+0001a650: 0a20 2020 2020 2020 204c 6f61 6420 7468  .        Load th
+0001a660: 6520 6461 7461 7365 7420 6166 7465 7220  e dataset after 
+0001a670: 646f 776e 6c6f 6164 696e 6720 6974 2077  downloading it w
+0001a680: 6865 6e20 6060 5472 7565 6060 2e20 2053  hen ``True``.  S
+0001a690: 6574 2074 6869 730a 2020 2020 2020 2020  et this.        
+0001a6a0: 746f 2060 6046 616c 7365 6060 2061 6e64  to ``False`` and
+0001a6b0: 206f 6e6c 7920 7468 6520 6669 6c65 6e61   only the filena
+0001a6c0: 6d65 2077 696c 6c20 6265 2072 6574 7572  me will be retur
+0001a6d0: 6e65 642e 0a0a 2020 2020 5265 7475 726e  ned...    Return
+0001a6e0: 730a 2020 2020 2d2d 2d2d 2d2d 2d0a 2020  s.    -------.  
+0001a6f0: 2020 7079 7669 7374 612e 506f 6c79 4461    pyvista.PolyDa
+0001a700: 7461 207c 2073 7472 0a20 2020 2020 2020  ta | str.       
+0001a710: 2044 6174 6153 6574 206f 7220 6669 6c65   DataSet or file
+0001a720: 6e61 6d65 2064 6570 656e 6469 6e67 206f  name depending o
+0001a730: 6e20 6060 6c6f 6164 6060 2e0a 0a20 2020  n ``load``...   
+0001a740: 2045 7861 6d70 6c65 730a 2020 2020 2d2d   Examples.    --
+0001a750: 2d2d 2d2d 2d2d 0a20 2020 2050 6c6f 7420  ------.    Plot 
+0001a760: 7468 6520 4c75 6379 2041 6e67 656c 2064  the Lucy Angel d
+0001a770: 6174 6173 6574 2077 6974 6820 6375 7374  ataset with cust
+0001a780: 6f6d 206c 6967 6874 696e 672e 0a0a 2020  om lighting...  
+0001a790: 2020 3e3e 3e20 6672 6f6d 2070 7976 6973    >>> from pyvis
+0001a7a0: 7461 2069 6d70 6f72 7420 6578 616d 706c  ta import exampl
+0001a7b0: 6573 0a20 2020 203e 3e3e 2069 6d70 6f72  es.    >>> impor
+0001a7c0: 7420 7079 7669 7374 6120 6173 2070 760a  t pyvista as pv.
+0001a7d0: 2020 2020 3e3e 3e20 6461 7461 7365 7420      >>> dataset 
+0001a7e0: 3d20 6578 616d 706c 6573 2e64 6f77 6e6c  = examples.downl
+0001a7f0: 6f61 645f 6c75 6379 2829 0a0a 2020 2020  oad_lucy()..    
+0001a800: 4372 6561 7465 2061 206c 6967 6874 2061  Create a light a
+0001a810: 7420 7468 6520 2266 6c61 6d65 222e 0a0a  t the "flame"...
+0001a820: 2020 2020 3e3e 3e20 666c 616d 655f 6c69      >>> flame_li
+0001a830: 6768 7420 3d20 7076 2e4c 6967 6874 280a  ght = pv.Light(.
+0001a840: 2020 2020 2e2e 2e20 2020 2020 636f 6c6f      ...     colo
+0001a850: 723d 5b30 2e38 3836 2c20 302e 3334 352c  r=[0.886, 0.345,
+0001a860: 2030 2e31 3333 5d2c 0a20 2020 202e 2e2e   0.133],.    ...
+0001a870: 2020 2020 2070 6f73 6974 696f 6e3d 5b35       position=[5
+0001a880: 3530 2c20 3134 302c 2039 3530 5d2c 0a20  50, 140, 950],. 
+0001a890: 2020 202e 2e2e 2020 2020 2069 6e74 656e     ...     inten
+0001a8a0: 7369 7479 3d31 2e35 2c0a 2020 2020 2e2e  sity=1.5,.    ..
+0001a8b0: 2e20 2020 2020 706f 7369 7469 6f6e 616c  .     positional
+0001a8c0: 3d54 7275 652c 0a20 2020 202e 2e2e 2020  =True,.    ...  
+0001a8d0: 2020 2063 6f6e 655f 616e 676c 653d 3930     cone_angle=90
+0001a8e0: 2c0a 2020 2020 2e2e 2e20 2020 2020 6174  ,.    ...     at
+0001a8f0: 7465 6e75 6174 696f 6e5f 7661 6c75 6573  tenuation_values
+0001a900: 3d28 302e 3030 312c 2030 2e30 3035 2c20  =(0.001, 0.005, 
+0001a910: 3029 2c0a 2020 2020 2e2e 2e20 290a 0a20  0),.    ... ).. 
+0001a920: 2020 2043 7265 6174 6520 6120 7363 656e     Create a scen
+0001a930: 6520 6c69 6768 742e 0a0a 2020 2020 3e3e  e light...    >>
+0001a940: 3e20 7363 656e 655f 6c69 6768 7420 3d20  > scene_light = 
+0001a950: 7076 2e4c 6967 6874 2869 6e74 656e 7369  pv.Light(intensi
+0001a960: 7479 3d30 2e32 290a 0a20 2020 203e 3e3e  ty=0.2)..    >>>
+0001a970: 2070 6c20 3d20 7076 2e50 6c6f 7474 6572   pl = pv.Plotter
+0001a980: 286c 6967 6874 696e 673d 4e6f 6e65 290a  (lighting=None).
+0001a990: 2020 2020 3e3e 3e20 5f20 3d20 706c 2e61      >>> _ = pl.a
+0001a9a0: 6464 5f6d 6573 6828 6461 7461 7365 742c  dd_mesh(dataset,
+0001a9b0: 2073 6d6f 6f74 685f 7368 6164 696e 673d   smooth_shading=
+0001a9c0: 5472 7565 290a 2020 2020 3e3e 3e20 706c  True).    >>> pl
+0001a9d0: 2e61 6464 5f6c 6967 6874 2866 6c61 6d65  .add_light(flame
+0001a9e0: 5f6c 6967 6874 290a 2020 2020 3e3e 3e20  _light).    >>> 
+0001a9f0: 706c 2e61 6464 5f6c 6967 6874 2873 6365  pl.add_light(sce
+0001aa00: 6e65 5f6c 6967 6874 290a 2020 2020 3e3e  ne_light).    >>
+0001aa10: 3e20 706c 2e62 6163 6b67 726f 756e 645f  > pl.background_
+0001aa20: 636f 6c6f 7220 3d20 276b 270a 2020 2020  color = 'k'.    
+0001aa30: 3e3e 3e20 706c 2e73 686f 7728 290a 0a20  >>> pl.show().. 
+0001aa40: 2020 2053 6565 203a 7265 663a 606a 7570     See :ref:`jup
+0001aa50: 7974 6572 5f70 6c6f 7474 696e 6760 2066  yter_plotting` f
+0001aa60: 6f72 2061 6e6f 7468 6572 2065 7861 6d70  or another examp
+0001aa70: 6c65 2075 7369 6e67 2074 6869 7320 6461  le using this da
+0001aa80: 7461 7365 742e 0a0a 2020 2020 2222 220a  taset...    """.
+0001aa90: 2020 2020 7265 7475 726e 205f 646f 776e      return _down
+0001aaa0: 6c6f 6164 5f61 6e64 5f72 6561 6428 276c  load_and_read('l
+0001aab0: 7563 792e 706c 7927 2c20 6c6f 6164 3d6c  ucy.ply', load=l
+0001aac0: 6f61 6429 0a0a 0a64 6566 2064 6f77 6e6c  oad)...def downl
+0001aad0: 6f61 645f 7075 6d70 5f62 7261 636b 6574  oad_pump_bracket
+0001aae0: 286c 6f61 643d 5472 7565 293a 2020 2320  (load=True):  # 
+0001aaf0: 7072 6167 6d61 3a20 6e6f 2063 6f76 6572  pragma: no cover
+0001ab00: 0a20 2020 2022 2222 446f 776e 6c6f 6164  .    """Download
+0001ab10: 2074 6865 2070 756d 7020 6272 6163 6b65   the pump bracke
+0001ab20: 7420 6578 616d 706c 6520 6461 7461 7365  t example datase
+0001ab30: 742e 0a0a 2020 2020 4461 7461 2067 656e  t...    Data gen
+0001ab40: 6572 6174 6564 2066 726f 6d20 7075 626c  erated from publ
+0001ab50: 6963 2053 696d 5363 616c 6520 6578 616d  ic SimScale exam
+0001ab60: 706c 6573 2061 7420 6053 696d 5363 616c  ples at `SimScal
+0001ab70: 6520 5072 6f6a 6563 7420 4c69 6272 6172  e Project Librar
+0001ab80: 7920 2d0a 2020 2020 5475 7262 6f20 3c68  y -.    Turbo <h
+0001ab90: 7474 7073 3a2f 2f77 7777 2e73 696d 7363  ttps://www.simsc
+0001aba0: 616c 652e 636f 6d2f 7072 6f6a 6563 7473  ale.com/projects
+0001abb0: 2f53 5452 2f62 7261 636b 6574 2f3e 605f  /STR/bracket/>`_
+0001abc0: 2e0a 0a20 2020 204c 6963 656e 7369 6e67  ...    Licensing
+0001abd0: 2066 6f72 2074 6869 7320 6461 7461 7365   for this datase
+0001abe0: 7420 6973 2067 7261 6e74 6564 2066 7265  t is granted fre
+0001abf0: 656c 7920 616e 6420 7769 7468 6f75 7420  ely and without 
+0001ac00: 7265 7374 7269 6374 696f 6e20 746f 0a20  restriction to. 
+0001ac10: 2020 2072 6570 726f 6475 6365 2c20 6469     reproduce, di
+0001ac20: 7374 7269 6275 7465 2c20 616e 6420 7075  stribute, and pu
+0001ac30: 626c 6973 6820 6163 636f 7264 696e 6720  blish according 
+0001ac40: 746f 2074 6865 2060 5369 6d53 6361 6c65  to the `SimScale
+0001ac50: 2054 6572 6d73 2061 6e64 0a20 2020 2043   Terms and.    C
+0001ac60: 6f6e 6469 7469 6f6e 7320 3c68 7474 7073  onditions <https
+0001ac70: 3a2f 2f77 7777 2e73 696d 7363 616c 652e  ://www.simscale.
+0001ac80: 636f 6d2f 7465 726d 732d 616e 642d 636f  com/terms-and-co
+0001ac90: 6e64 6974 696f 6e73 2f3e 605f 2e0a 0a20  nditions/>`_... 
+0001aca0: 2020 2050 6172 616d 6574 6572 730a 2020     Parameters.  
+0001acb0: 2020 2d2d 2d2d 2d2d 2d2d 2d2d 0a20 2020    ----------.   
+0001acc0: 206c 6f61 6420 3a20 626f 6f6c 2c20 6465   load : bool, de
+0001acd0: 6661 756c 743a 2054 7275 650a 2020 2020  fault: True.    
+0001ace0: 2020 2020 4c6f 6164 2074 6865 2064 6174      Load the dat
+0001acf0: 6173 6574 2061 6674 6572 2064 6f77 6e6c  aset after downl
+0001ad00: 6f61 6469 6e67 2069 7420 7768 656e 2060  oading it when `
+0001ad10: 6054 7275 6560 602e 2020 5365 7420 7468  `True``.  Set th
+0001ad20: 6973 0a20 2020 2020 2020 2074 6f20 6060  is.        to ``
+0001ad30: 4661 6c73 6560 6020 616e 6420 6f6e 6c79  False`` and only
+0001ad40: 2074 6865 2066 696c 656e 616d 6520 7769   the filename wi
+0001ad50: 6c6c 2062 6520 7265 7475 726e 6564 2e0a  ll be returned..
+0001ad60: 0a20 2020 2052 6574 7572 6e73 0a20 2020  .    Returns.   
+0001ad70: 202d 2d2d 2d2d 2d2d 0a20 2020 2055 6e73   -------.    Uns
+0001ad80: 7472 7563 7475 7265 6447 7269 6420 7c20  tructuredGrid | 
+0001ad90: 7374 720a 2020 2020 2020 2020 4461 7461  str.        Data
+0001ada0: 5365 7420 6f72 2066 696c 656e 616d 6520  Set or filename 
+0001adb0: 6465 7065 6e64 696e 6720 6f6e 2060 606c  depending on ``l
+0001adc0: 6f61 6460 602e 0a0a 2020 2020 4578 616d  oad``...    Exam
+0001add0: 706c 6573 0a20 2020 202d 2d2d 2d2d 2d2d  ples.    -------
+0001ade0: 2d0a 2020 2020 4c6f 6164 2074 6865 2064  -.    Load the d
+0001adf0: 6174 6173 6574 2e0a 0a20 2020 203e 3e3e  ataset...    >>>
+0001ae00: 2069 6d70 6f72 7420 7079 7669 7374 6120   import pyvista 
+0001ae10: 6173 2070 760a 2020 2020 3e3e 3e20 6672  as pv.    >>> fr
+0001ae20: 6f6d 2070 7976 6973 7461 2069 6d70 6f72  om pyvista impor
+0001ae30: 7420 6578 616d 706c 6573 0a20 2020 203e  t examples.    >
+0001ae40: 3e3e 2064 6174 6173 6574 203d 2065 7861  >> dataset = exa
+0001ae50: 6d70 6c65 732e 646f 776e 6c6f 6164 5f70  mples.download_p
+0001ae60: 756d 705f 6272 6163 6b65 7428 290a 2020  ump_bracket().  
+0001ae70: 2020 3e3e 3e20 6461 7461 7365 740a 2020    >>> dataset.  
+0001ae80: 2020 556e 7374 7275 6374 7572 6564 4772    UnstructuredGr
+0001ae90: 6964 2028 2e2e 2e29 0a20 2020 2020 204e  id (...).      N
+0001aea0: 2043 656c 6c73 3a20 2020 2031 3234 3830   Cells:    12480
+0001aeb0: 360a 2020 2020 2020 4e20 506f 696e 7473  6.      N Points
+0001aec0: 3a20 2020 3235 3034 3837 0a20 2020 2020  :   250487.     
+0001aed0: 2058 2042 6f75 6e64 733a 2020 202d 352e   X Bounds:   -5.
+0001aee0: 3030 3065 2d30 312c 2035 2e30 3030 652d  000e-01, 5.000e-
+0001aef0: 3031 0a20 2020 2020 2059 2042 6f75 6e64  01.      Y Bound
+0001af00: 733a 2020 202d 342e 3030 3065 2d30 312c  s:   -4.000e-01,
+0001af10: 2030 2e30 3030 652b 3030 0a20 2020 2020   0.000e+00.     
+0001af20: 205a 2042 6f75 6e64 733a 2020 202d 322e   Z Bounds:   -2.
+0001af30: 3530 3065 2d30 322c 2032 2e35 3030 652d  500e-02, 2.500e-
+0001af40: 3032 0a20 2020 2020 204e 2041 7272 6179  02.      N Array
+0001af50: 733a 2020 2031 300a 0a20 2020 2050 6c6f  s:   10..    Plo
+0001af60: 7420 7468 6520 6469 7370 6c61 6365 6d65  t the displaceme
+0001af70: 6e74 206f 6620 7468 6520 3474 6820 6d6f  nt of the 4th mo
+0001af80: 6465 2073 6861 7065 2061 7320 7363 616c  de shape as scal
+0001af90: 6172 732e 0a0a 2020 2020 3e3e 3e20 6370  ars...    >>> cp
+0001afa0: 6f73 203d 205b 0a20 2020 202e 2e2e 2020  os = [.    ...  
+0001afb0: 2020 2028 302e 3734 342c 202d 302e 3530     (0.744, -0.50
+0001afc0: 322c 202d 302e 3833 3029 2c0a 2020 2020  2, -0.830),.    
+0001afd0: 2e2e 2e20 2020 2020 2830 2e30 3532 302c  ...     (0.0520,
+0001afe0: 202d 302e 3136 302c 2030 2e30 3734 3329   -0.160, 0.0743)
+0001aff0: 2c0a 2020 2020 2e2e 2e20 2020 2020 282d  ,.    ...     (-
+0001b000: 302e 3138 302c 202d 302e 3935 382c 2030  0.180, -0.958, 0
+0001b010: 2e32 3234 292c 0a20 2020 202e 2e2e 205d  .224),.    ... ]
+0001b020: 0a20 2020 203e 3e3e 2064 6174 6173 6574  .    >>> dataset
+0001b030: 2e70 6c6f 7428 0a20 2020 202e 2e2e 2020  .plot(.    ...  
+0001b040: 2020 2073 6361 6c61 7273 3d27 6469 7370     scalars='disp
+0001b050: 5f33 272c 0a20 2020 202e 2e2e 2020 2020  _3',.    ...    
+0001b060: 2063 706f 733d 6370 6f73 2c0a 2020 2020   cpos=cpos,.    
+0001b070: 2e2e 2e20 2020 2020 7368 6f77 5f73 6361  ...     show_sca
+0001b080: 6c61 725f 6261 723d 4661 6c73 652c 0a20  lar_bar=False,. 
+0001b090: 2020 202e 2e2e 2020 2020 2061 6d62 6965     ...     ambie
+0001b0a0: 6e74 3d30 2e32 2c0a 2020 2020 2e2e 2e20  nt=0.2,.    ... 
+0001b0b0: 2020 2020 616e 7469 5f61 6c69 6173 696e      anti_aliasin
+0001b0c0: 673d 2766 7861 6127 2c0a 2020 2020 2e2e  g='fxaa',.    ..
+0001b0d0: 2e20 290a 0a20 2020 2053 6565 203a 7265  . )..    See :re
+0001b0e0: 663a 6070 756d 705f 6272 6163 6b65 745f  f:`pump_bracket_
+0001b0f0: 6578 616d 706c 6560 2066 6f72 2061 2066  example` for a f
+0001b100: 756c 6c20 6578 616d 706c 6520 7573 696e  ull example usin
+0001b110: 6720 7468 6973 2064 6174 6173 6574 2e0a  g this dataset..
+0001b120: 0a20 2020 2022 2222 0a20 2020 2066 696c  .    """.    fil
+0001b130: 656e 616d 6520 3d20 5f64 6f77 6e6c 6f61  ename = _downloa
+0001b140: 645f 6172 6368 6976 6528 0a20 2020 2020  d_archive(.     
+0001b150: 2020 2027 6665 612f 7075 6d70 5f62 7261     'fea/pump_bra
+0001b160: 636b 6574 2f70 756d 705f 6272 6163 6b65  cket/pump_bracke
+0001b170: 742e 7a69 7027 2c0a 2020 2020 2020 2020  t.zip',.        
+0001b180: 2770 756d 705f 6272 6163 6b65 742e 7674  'pump_bracket.vt
+0001b190: 6b27 2c0a 2020 2020 290a 2020 2020 6966  k',.    ).    if
+0001b1a0: 206c 6f61 643a 0a20 2020 2020 2020 2072   load:.        r
+0001b1b0: 6574 7572 6e20 7079 7669 7374 612e 7265  eturn pyvista.re
+0001b1c0: 6164 2866 696c 656e 616d 6529 0a20 2020  ad(filename).   
+0001b1d0: 2072 6574 7572 6e20 6669 6c65 6e61 6d65   return filename
+0001b1e0: 0a0a 0a64 6566 2064 6f77 6e6c 6f61 645f  ...def download_
+0001b1f0: 656c 6563 7472 6f6e 6963 735f 636f 6f6c  electronics_cool
+0001b200: 696e 6728 6c6f 6164 3d54 7275 6529 3a20  ing(load=True): 
+0001b210: 2023 2070 7261 676d 613a 206e 6f20 636f   # pragma: no co
+0001b220: 7665 720a 2020 2020 2222 2244 6f77 6e6c  ver.    """Downl
+0001b230: 6f61 6420 7468 6520 656c 6563 7472 6f6e  oad the electron
+0001b240: 6963 7320 636f 6f6c 696e 6720 6578 616d  ics cooling exam
+0001b250: 706c 6520 6461 7461 7365 7473 2e0a 0a20  ple datasets... 
+0001b260: 2020 2044 6174 6120 6765 6e65 7261 7465     Data generate
+0001b270: 6420 6672 6f6d 2070 7562 6c69 6320 5369  d from public Si
+0001b280: 6d53 6361 6c65 2065 7861 6d70 6c65 7320  mScale examples 
+0001b290: 6174 2060 5369 6d53 6361 6c65 2050 726f  at `SimScale Pro
+0001b2a0: 6a65 6374 204c 6962 7261 7279 202d 0a20  ject Library -. 
+0001b2b0: 2020 2054 7572 626f 203c 6874 7470 733a     Turbo <https:
+0001b2c0: 2f2f 7777 772e 7369 6d73 6361 6c65 2e63  //www.simscale.c
+0001b2d0: 6f6d 2f70 726f 6a65 6374 732f 6179 6172  om/projects/ayar
+0001b2e0: 6e6f 7a2f 7475 7262 6f2f 3e60 5f2e 0a0a  noz/turbo/>`_...
+0001b2f0: 2020 2020 4c69 6365 6e73 696e 6720 666f      Licensing fo
+0001b300: 7220 7468 6973 2064 6174 6173 6574 2069  r this dataset i
+0001b310: 7320 6772 616e 7465 6420 746f 2066 7265  s granted to fre
+0001b320: 656c 7920 616e 6420 7769 7468 6f75 7420  ely and without 
+0001b330: 7265 7374 7269 6374 696f 6e0a 2020 2020  restriction.    
+0001b340: 7265 7072 6f64 7563 652c 2064 6973 7472  reproduce, distr
+0001b350: 6962 7574 652c 2070 7562 6c69 7368 2061  ibute, publish a
+0001b360: 6363 6f72 6469 6e67 2074 6f20 7468 6520  ccording to the 
+0001b370: 6053 696d 5363 616c 6520 5465 726d 7320  `SimScale Terms 
+0001b380: 616e 640a 2020 2020 436f 6e64 6974 696f  and.    Conditio
+0001b390: 6e73 203c 6874 7470 733a 2f2f 7777 772e  ns <https://www.
+0001b3a0: 7369 6d73 6361 6c65 2e63 6f6d 2f74 6572  simscale.com/ter
+0001b3b0: 6d73 2d61 6e64 2d63 6f6e 6469 7469 6f6e  ms-and-condition
+0001b3c0: 732f 3e60 5f2e 0a0a 2020 2020 5061 7261  s/>`_...    Para
+0001b3d0: 6d65 7465 7273 0a20 2020 202d 2d2d 2d2d  meters.    -----
+0001b3e0: 2d2d 2d2d 2d0a 2020 2020 6c6f 6164 203a  -----.    load :
+0001b3f0: 2062 6f6f 6c2c 2064 6566 6175 6c74 3a20   bool, default: 
+0001b400: 5472 7565 0a20 2020 2020 2020 204c 6f61  True.        Loa
+0001b410: 6420 7468 6520 6461 7461 7365 7420 6166  d the dataset af
+0001b420: 7465 7220 646f 776e 6c6f 6164 696e 6720  ter downloading 
+0001b430: 6974 2077 6865 6e20 6060 5472 7565 6060  it when ``True``
+0001b440: 2e20 2053 6574 2074 6869 730a 2020 2020  .  Set this.    
+0001b450: 2020 2020 746f 2060 6046 616c 7365 6060      to ``False``
+0001b460: 2061 6e64 206f 6e6c 7920 7468 6520 6669   and only the fi
+0001b470: 6c65 6e61 6d65 2077 696c 6c20 6265 2072  lename will be r
+0001b480: 6574 7572 6e65 642e 0a0a 2020 2020 5265  eturned...    Re
+0001b490: 7475 726e 730a 2020 2020 2d2d 2d2d 2d2d  turns.    ------
+0001b4a0: 2d0a 2020 2020 7475 706c 655b 506f 6c79  -.    tuple[Poly
+0001b4b0: 4461 7461 2c20 556e 7374 7275 6374 7572  Data, Unstructur
+0001b4c0: 6564 4772 6964 5d20 7c20 6c69 7374 5b73  edGrid] | list[s
+0001b4d0: 7472 5d0a 2020 2020 2020 2020 4461 7461  tr].        Data
+0001b4e0: 5365 7473 206f 7220 6669 6c65 6e61 6d65  Sets or filename
+0001b4f0: 7320 6465 7065 6e64 696e 6720 6f6e 2060  s depending on `
+0001b500: 606c 6f61 6460 602e 0a0a 2020 2020 4578  `load``...    Ex
+0001b510: 616d 706c 6573 0a20 2020 202d 2d2d 2d2d  amples.    -----
+0001b520: 2d2d 2d0a 2020 2020 4c6f 6164 2074 6865  ---.    Load the
+0001b530: 2064 6174 6173 6574 7320 616e 6420 706c   datasets and pl
+0001b540: 6f74 2074 6865 2061 6972 2076 656c 6f63  ot the air veloc
+0001b550: 6974 7920 7468 726f 7567 6820 7468 6520  ity through the 
+0001b560: 656c 6563 7472 6f6e 6963 732e 0a0a 2020  electronics...  
+0001b570: 2020 3e3e 3e20 696d 706f 7274 2070 7976    >>> import pyv
+0001b580: 6973 7461 2061 7320 7076 0a20 2020 203e  ista as pv.    >
+0001b590: 3e3e 2066 726f 6d20 7079 7669 7374 6120  >> from pyvista 
+0001b5a0: 696d 706f 7274 2065 7861 6d70 6c65 730a  import examples.
+0001b5b0: 2020 2020 3e3e 3e20 7374 7275 6374 7572      >>> structur
+0001b5c0: 652c 2061 6972 203d 2065 7861 6d70 6c65  e, air = example
+0001b5d0: 732e 646f 776e 6c6f 6164 5f65 6c65 6374  s.download_elect
+0001b5e0: 726f 6e69 6373 5f63 6f6f 6c69 6e67 2829  ronics_cooling()
+0001b5f0: 0a20 2020 203e 3e3e 2073 7472 7563 7475  .    >>> structu
+0001b600: 7265 2c20 6169 720a 2020 2020 2850 6f6c  re, air.    (Pol
+0001b610: 7944 6174 6120 282e 2e2e 290a 2020 2020  yData (...).    
+0001b620: 2020 4e20 4365 6c6c 733a 2020 2020 3334    N Cells:    34
+0001b630: 3432 3730 0a20 2020 2020 204e 2050 6f69  4270.      N Poi
+0001b640: 6e74 733a 2020 2031 3837 3939 320a 2020  nts:   187992.  
+0001b650: 2020 2020 4e20 5374 7269 7073 3a20 2020      N Strips:   
+0001b660: 300a 2020 2020 2020 5820 426f 756e 6473  0.      X Bounds
+0001b670: 3a20 2020 2d33 2e30 3030 652d 3033 2c20  :   -3.000e-03, 
+0001b680: 312e 3533 3065 2d30 310a 2020 2020 2020  1.530e-01.      
+0001b690: 5920 426f 756e 6473 3a20 2020 2d33 2e30  Y Bounds:   -3.0
+0001b6a0: 3030 652d 3033 2c20 322e 3033 3065 2d30  00e-03, 2.030e-0
+0001b6b0: 310a 2020 2020 2020 5a20 426f 756e 6473  1.      Z Bounds
+0001b6c0: 3a20 2020 2d39 2e30 3030 652d 3033 2c20  :   -9.000e-03, 
+0001b6d0: 342e 3230 3065 2d30 320a 2020 2020 2020  4.200e-02.      
+0001b6e0: 4e20 4172 7261 7973 3a20 2020 342c 2055  N Arrays:   4, U
+0001b6f0: 6e73 7472 7563 7475 7265 6447 7269 6420  nstructuredGrid 
+0001b700: 282e 2e2e 290a 2020 2020 2020 4e20 4365  (...).      N Ce
+0001b710: 6c6c 733a 2020 2020 3137 3439 3939 320a  lls:    1749992.
+0001b720: 2020 2020 2020 4e20 506f 696e 7473 3a20        N Points: 
+0001b730: 2020 3631 3031 3736 0a20 2020 2020 2058    610176.      X
+0001b740: 2042 6f75 6e64 733a 2020 202d 312e 3338   Bounds:   -1.38
+0001b750: 3865 2d31 382c 2031 2e35 3030 652d 3031  8e-18, 1.500e-01
+0001b760: 0a20 2020 2020 2059 2042 6f75 6e64 733a  .      Y Bounds:
+0001b770: 2020 202d 332e 3030 3065 2d30 332c 2032     -3.000e-03, 2
+0001b780: 2e30 3330 652d 3031 0a20 2020 2020 205a  .030e-01.      Z
+0001b790: 2042 6f75 6e64 733a 2020 202d 362e 3030   Bounds:   -6.00
+0001b7a0: 3065 2d30 332c 2034 2e34 3030 652d 3032  0e-03, 4.400e-02
+0001b7b0: 0a20 2020 2020 204e 2041 7272 6179 733a  .      N Arrays:
+0001b7c0: 2020 2031 3029 0a0a 2020 2020 3e3e 3e20     10)..    >>> 
+0001b7d0: 7a5f 736c 6963 6520 3d20 6169 722e 636c  z_slice = air.cl
+0001b7e0: 6970 2827 7a27 2c20 7661 6c75 653d 2d30  ip('z', value=-0
+0001b7f0: 2e30 3035 290a 2020 2020 3e3e 3e20 706c  .005).    >>> pl
+0001b800: 203d 2070 762e 506c 6f74 7465 7228 290a   = pv.Plotter().
+0001b810: 2020 2020 3e3e 3e20 706c 2e65 6e61 626c      >>> pl.enabl
+0001b820: 655f 7373 616f 2872 6164 6975 733d 302e  e_ssao(radius=0.
+0001b830: 3031 290a 2020 2020 3e3e 3e20 5f20 3d20  01).    >>> _ = 
+0001b840: 706c 2e61 6464 5f6d 6573 6828 0a20 2020  pl.add_mesh(.   
+0001b850: 202e 2e2e 2020 2020 207a 5f73 6c69 6365   ...     z_slice
+0001b860: 2c0a 2020 2020 2e2e 2e20 2020 2020 7363  ,.    ...     sc
+0001b870: 616c 6172 733d 2755 272c 0a20 2020 202e  alars='U',.    .
+0001b880: 2e2e 2020 2020 206c 6967 6874 696e 673d  ..     lighting=
+0001b890: 4661 6c73 652c 0a20 2020 202e 2e2e 2020  False,.    ...  
+0001b8a0: 2020 2073 6361 6c61 725f 6261 725f 6172     scalar_bar_ar
+0001b8b0: 6773 3d7b 2774 6974 6c65 273a 2027 5665  gs={'title': 'Ve
+0001b8c0: 6c6f 6369 7479 277d 2c0a 2020 2020 2e2e  locity'},.    ..
+0001b8d0: 2e20 290a 2020 2020 3e3e 3e20 5f20 3d20  . ).    >>> _ = 
+0001b8e0: 706c 2e61 6464 5f6d 6573 6828 0a20 2020  pl.add_mesh(.   
+0001b8f0: 202e 2e2e 2020 2020 2073 7472 7563 7475   ...     structu
+0001b900: 7265 2c0a 2020 2020 2e2e 2e20 2020 2020  re,.    ...     
+0001b910: 636f 6c6f 723d 2777 272c 0a20 2020 202e  color='w',.    .
+0001b920: 2e2e 2020 2020 2073 6d6f 6f74 685f 7368  ..     smooth_sh
+0001b930: 6164 696e 673d 5472 7565 2c0a 2020 2020  ading=True,.    
+0001b940: 2e2e 2e20 2020 2020 7370 6c69 745f 7368  ...     split_sh
+0001b950: 6172 705f 6564 6765 733d 5472 7565 2c0a  arp_edges=True,.
+0001b960: 2020 2020 2e2e 2e20 290a 2020 2020 3e3e      ... ).    >>
+0001b970: 3e20 706c 2e63 616d 6572 615f 706f 7369  > pl.camera_posi
+0001b980: 7469 6f6e 203d 2027 7879 270a 2020 2020  tion = 'xy'.    
+0001b990: 3e3e 3e20 706c 2e63 616d 6572 612e 726f  >>> pl.camera.ro
+0001b9a0: 6c6c 203d 2039 300a 2020 2020 3e3e 3e20  ll = 90.    >>> 
+0001b9b0: 706c 2e65 6e61 626c 655f 616e 7469 5f61  pl.enable_anti_a
+0001b9c0: 6c69 6173 696e 6728 2766 7861 6127 290a  liasing('fxaa').
+0001b9d0: 2020 2020 3e3e 3e20 706c 2e73 686f 7728      >>> pl.show(
+0001b9e0: 290a 0a20 2020 2053 686f 7720 7468 6520  )..    Show the 
+0001b9f0: 7479 7065 2061 6e64 2062 6f75 6e64 7320  type and bounds 
+0001ba00: 6f66 2074 6865 2064 6174 6173 6574 732e  of the datasets.
+0001ba10: 0a0a 2020 2020 5365 6520 3a72 6566 3a60  ..    See :ref:`
+0001ba20: 6f70 656e 666f 616d 5f63 6f6f 6c69 6e67  openfoam_cooling
+0001ba30: 5f65 7861 6d70 6c65 6020 666f 7220 6120  _example` for a 
+0001ba40: 6675 6c6c 2065 7861 6d70 6c65 2075 7369  full example usi
+0001ba50: 6e67 2074 6869 7320 6461 7461 7365 742e  ng this dataset.
+0001ba60: 0a0a 2020 2020 2222 220a 2020 2020 666e  ..    """.    fn
+0001ba70: 616d 6573 203d 205f 646f 776e 6c6f 6164  ames = _download
+0001ba80: 5f61 7263 6869 7665 2827 6676 6d2f 636f  _archive('fvm/co
+0001ba90: 6f6c 696e 675f 656c 6563 7472 6f6e 6963  oling_electronic
+0001baa0: 732f 6461 7461 7365 7473 2e7a 6970 2729  s/datasets.zip')
+0001bab0: 0a20 2020 2069 6620 6c6f 6164 3a0a 2020  .    if load:.  
+0001bac0: 2020 2020 2020 2320 7265 7475 726e 2074        # return t
+0001bad0: 6865 2073 7472 7563 7475 7265 2064 6174  he structure dat
+0001bae0: 6173 6574 2066 6972 7374 0a20 2020 2020  aset first.     
+0001baf0: 2020 2069 6620 666e 616d 6573 5b31 5d2e     if fnames[1].
+0001bb00: 656e 6473 7769 7468 2827 7374 7275 6374  endswith('struct
+0001bb10: 7572 652e 7674 7027 293a 0a20 2020 2020  ure.vtp'):.     
+0001bb20: 2020 2020 2020 2066 6e61 6d65 7320 3d20         fnames = 
+0001bb30: 666e 616d 6573 5b3a 3a2d 315d 0a20 2020  fnames[::-1].   
+0001bb40: 2020 2020 2072 6574 7572 6e20 7079 7669       return pyvi
+0001bb50: 7374 612e 7265 6164 2866 6e61 6d65 735b  sta.read(fnames[
+0001bb60: 305d 292c 2070 7976 6973 7461 2e72 6561  0]), pyvista.rea
+0001bb70: 6428 666e 616d 6573 5b31 5d29 0a20 2020  d(fnames[1]).   
+0001bb80: 2072 6574 7572 6e20 666e 616d 6573 0a0a   return fnames..
+0001bb90: 0a64 6566 2064 6f77 6e6c 6f61 645f 6361  .def download_ca
+0001bba0: 6e28 7061 7274 6961 6c3d 4661 6c73 652c  n(partial=False,
+0001bbb0: 206c 6f61 643d 5472 7565 293a 2020 2320   load=True):  # 
+0001bbc0: 7072 6167 6d61 3a20 6e6f 2063 6f76 6572  pragma: no cover
+0001bbd0: 0a20 2020 2022 2222 446f 776e 6c6f 6164  .    """Download
+0001bbe0: 2074 6865 2063 616e 2064 6174 6173 6574   the can dataset
+0001bbf0: 206d 6573 682e 0a0a 2020 2020 4669 6c65   mesh...    File
+0001bc00: 206f 6274 6169 6e65 6420 6672 6f6d 2060   obtained from `
+0001bc10: 4b69 7477 6172 6520 3c68 7474 7073 3a2f  Kitware <https:/
+0001bc20: 2f77 7777 2e6b 6974 7761 7265 2e63 6f6d  /www.kitware.com
+0001bc30: 2f3e 605f 2e20 5573 6564 0a20 2020 2066  />`_. Used.    f
+0001bc40: 6f72 2074 6573 7469 6e67 2068 6466 2066  or testing hdf f
+0001bc50: 696c 6573 2e0a 0a20 2020 2050 6172 616d  iles...    Param
+0001bc60: 6574 6572 730a 2020 2020 2d2d 2d2d 2d2d  eters.    ------
+0001bc70: 2d2d 2d2d 0a20 2020 2070 6172 7469 616c  ----.    partial
+0001bc80: 203a 2062 6f6f 6c2c 2064 6566 6175 6c74   : bool, default
+0001bc90: 3a20 4661 6c73 650a 2020 2020 2020 2020  : False.        
+0001bca0: 4c6f 6164 2070 6172 7420 6f66 2074 6865  Load part of the
+0001bcb0: 2064 6174 6173 6574 2e0a 0a20 2020 206c   dataset...    l
+0001bcc0: 6f61 6420 3a20 626f 6f6c 2c20 6465 6661  oad : bool, defa
+0001bcd0: 756c 743a 2054 7275 650a 2020 2020 2020  ult: True.      
+0001bce0: 2020 4c6f 6164 2074 6865 2064 6174 6173    Load the datas
+0001bcf0: 6574 2061 6674 6572 2064 6f77 6e6c 6f61  et after downloa
+0001bd00: 6469 6e67 2069 7420 7768 656e 2060 6054  ding it when ``T
+0001bd10: 7275 6560 602e 2020 5365 7420 7468 6973  rue``.  Set this
+0001bd20: 0a20 2020 2020 2020 2074 6f20 6060 4661  .        to ``Fa
+0001bd30: 6c73 6560 6020 616e 6420 6f6e 6c79 2074  lse`` and only t
+0001bd40: 6865 2066 696c 656e 616d 6520 7769 6c6c  he filename will
+0001bd50: 2062 6520 7265 7475 726e 6564 2e0a 0a20   be returned... 
+0001bd60: 2020 2052 6574 7572 6e73 0a20 2020 202d     Returns.    -
+0001bd70: 2d2d 2d2d 2d2d 0a20 2020 2070 7976 6973  ------.    pyvis
+0001bd80: 7461 2e50 6f6c 7944 6174 612c 2073 7472  ta.PolyData, str
+0001bd90: 2c20 6f72 204c 6973 745b 7374 725d 0a20  , or List[str]. 
+0001bda0: 2020 2020 2020 2054 6865 2065 7861 6d70         The examp
+0001bdb0: 6c65 2050 6172 6156 6965 7720 6361 6e20  le ParaView can 
+0001bdc0: 4461 7461 5365 7420 6f72 2066 696c 6520  DataSet or file 
+0001bdd0: 7061 7468 2873 292e 0a0a 2020 2020 4578  path(s)...    Ex
+0001bde0: 616d 706c 6573 0a20 2020 202d 2d2d 2d2d  amples.    -----
+0001bdf0: 2d2d 2d0a 2020 2020 506c 6f74 2074 6865  ---.    Plot the
+0001be00: 2063 616e 2064 6174 6173 6574 2e0a 0a20   can dataset... 
+0001be10: 2020 203e 3e3e 2066 726f 6d20 7079 7669     >>> from pyvi
+0001be20: 7374 6120 696d 706f 7274 2065 7861 6d70  sta import examp
+0001be30: 6c65 730a 2020 2020 3e3e 3e20 696d 706f  les.    >>> impo
+0001be40: 7274 2070 7976 6973 7461 2061 7320 7076  rt pyvista as pv
+0001be50: 0a20 2020 203e 3e3e 2064 6174 6173 6574  .    >>> dataset
+0001be60: 203d 2065 7861 6d70 6c65 732e 646f 776e   = examples.down
+0001be70: 6c6f 6164 5f63 616e 2829 2020 2320 646f  load_can()  # do
+0001be80: 6374 6573 743a 2b53 4b49 500a 2020 2020  ctest:+SKIP.    
+0001be90: 3e3e 3e20 6461 7461 7365 742e 706c 6f74  >>> dataset.plot
+0001bea0: 2873 6361 6c61 7273 3d27 5645 4c27 2c20  (scalars='VEL', 
+0001beb0: 736d 6f6f 7468 5f73 6861 6469 6e67 3d54  smooth_shading=T
+0001bec0: 7275 6529 2020 2320 646f 6374 6573 743a  rue)  # doctest:
+0001bed0: 2b53 4b49 500a 0a20 2020 2022 2222 0a20  +SKIP..    """. 
+0001bee0: 2020 2069 6620 7079 7669 7374 612e 7674     if pyvista.vt
+0001bef0: 6b5f 7665 7273 696f 6e5f 696e 666f 203e  k_version_info >
+0001bf00: 2028 392c 2031 293a 2020 2320 7072 6167   (9, 1):  # prag
+0001bf10: 6d61 3a20 6e6f 2063 6f76 6572 0a20 2020  ma: no cover.   
+0001bf20: 2020 2020 2072 6169 7365 2056 544b 5665       raise VTKVe
+0001bf30: 7273 696f 6e45 7272 6f72 280a 2020 2020  rsionError(.    
+0001bf40: 2020 2020 2020 2020 2754 6869 7320 6578          'This ex
+0001bf50: 616d 706c 6520 6669 6c65 2069 7320 6465  ample file is de
+0001bf60: 7072 6563 6174 6564 2066 6f72 2056 544b  precated for VTK
+0001bf70: 2076 392e 322e 3020 616e 6420 6e65 7765   v9.2.0 and newe
+0001bf80: 722e 2027 0a20 2020 2020 2020 2020 2020  r. '.           
+0001bf90: 2027 5573 6520 6064 6f77 6e6c 6f61 645f   'Use `download_
+0001bfa0: 6361 6e5f 6372 7573 6865 645f 6864 6660  can_crushed_hdf`
+0001bfb0: 2069 6e73 7465 6164 2e27 0a20 2020 2020   instead.'.     
+0001bfc0: 2020 2029 0a0a 2020 2020 6361 6e5f 3020     )..    can_0 
+0001bfd0: 3d20 5f64 6f77 6e6c 6f61 645f 616e 645f  = _download_and_
+0001bfe0: 7265 6164 2827 6864 662f 6361 6e5f 302e  read('hdf/can_0.
+0001bff0: 6864 6627 2c20 6c6f 6164 3d6c 6f61 6429  hdf', load=load)
+0001c000: 0a20 2020 2069 6620 7061 7274 6961 6c3a  .    if partial:
+0001c010: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
+0001c020: 6361 6e5f 300a 0a20 2020 2063 616e 7320  can_0..    cans 
+0001c030: 3d20 5b0a 2020 2020 2020 2020 6361 6e5f  = [.        can_
+0001c040: 302c 0a20 2020 2020 2020 205f 646f 776e  0,.        _down
+0001c050: 6c6f 6164 5f61 6e64 5f72 6561 6428 2768  load_and_read('h
+0001c060: 6466 2f63 616e 5f31 2e68 6466 272c 206c  df/can_1.hdf', l
+0001c070: 6f61 643d 6c6f 6164 292c 0a20 2020 2020  oad=load),.     
+0001c080: 2020 205f 646f 776e 6c6f 6164 5f61 6e64     _download_and
+0001c090: 5f72 6561 6428 2768 6466 2f63 616e 5f32  _read('hdf/can_2
+0001c0a0: 2e68 6466 272c 206c 6f61 643d 6c6f 6164  .hdf', load=load
+0001c0b0: 292c 0a20 2020 205d 0a0a 2020 2020 6966  ),.    ]..    if
+0001c0c0: 206c 6f61 643a 0a20 2020 2020 2020 2072   load:.        r
+0001c0d0: 6574 7572 6e20 7079 7669 7374 612e 6d65  eturn pyvista.me
+0001c0e0: 7267 6528 6361 6e73 290a 2020 2020 7265  rge(cans).    re
+0001c0f0: 7475 726e 2063 616e 730a 0a0a 6465 6620  turn cans...def 
+0001c100: 646f 776e 6c6f 6164 5f63 616e 5f63 7275  download_can_cru
+0001c110: 7368 6564 5f68 6466 286c 6f61 643d 5472  shed_hdf(load=Tr
+0001c120: 7565 293a 2020 2320 7072 6167 6d61 3a20  ue):  # pragma: 
+0001c130: 6e6f 2063 6f76 6572 0a20 2020 2022 2222  no cover.    """
+0001c140: 446f 776e 6c6f 6164 2074 6865 2063 7275  Download the cru
+0001c150: 7368 6564 2063 616e 2064 6174 6173 6574  shed can dataset
+0001c160: 2e0a 0a20 2020 2046 696c 6520 6f62 7461  ...    File obta
+0001c170: 696e 6564 2066 726f 6d20 604b 6974 7761  ined from `Kitwa
+0001c180: 7265 203c 6874 7470 733a 2f2f 7777 772e  re <https://www.
+0001c190: 6b69 7477 6172 652e 636f 6d2f 3e60 5f2e  kitware.com/>`_.
+0001c1a0: 2055 7365 640a 2020 2020 666f 7220 7465   Used.    for te
+0001c1b0: 7374 696e 6720 6864 6620 6669 6c65 732e  sting hdf files.
+0001c1c0: 0a0a 2020 2020 4f72 6967 696e 616c 6c79  ..    Originally
+0001c1d0: 2062 7569 6c74 2075 7369 6e67 2056 544b   built using VTK
+0001c1e0: 2076 392e 322e 3072 6320 6672 6f6d 3a0a   v9.2.0rc from:.
+0001c1f0: 0a20 2020 2060 6056 544b 2f62 7569 6c64  .    ``VTK/build
+0001c200: 2f45 7874 6572 6e61 6c54 6573 7469 6e67  /ExternalTesting
+0001c210: 2f63 616e 2d76 7475 2e68 6466 6060 0a0a  /can-vtu.hdf``..
+0001c220: 2020 2020 5061 7261 6d65 7465 7273 0a20      Parameters. 
+0001c230: 2020 202d 2d2d 2d2d 2d2d 2d2d 2d0a 2020     ----------.  
+0001c240: 2020 6c6f 6164 203a 2062 6f6f 6c2c 2064    load : bool, d
+0001c250: 6566 6175 6c74 3a20 5472 7565 0a20 2020  efault: True.   
+0001c260: 2020 2020 204c 6f61 6420 7468 6520 6461       Load the da
+0001c270: 7461 7365 7420 6166 7465 7220 646f 776e  taset after down
+0001c280: 6c6f 6164 696e 6720 6974 2077 6865 6e20  loading it when 
+0001c290: 6060 5472 7565 6060 2e20 2053 6574 2074  ``True``.  Set t
+0001c2a0: 6869 730a 2020 2020 2020 2020 746f 2060  his.        to `
+0001c2b0: 6046 616c 7365 6060 2061 6e64 206f 6e6c  `False`` and onl
+0001c2c0: 7920 7468 6520 6669 6c65 6e61 6d65 2077  y the filename w
+0001c2d0: 696c 6c20 6265 2072 6574 7572 6e65 642e  ill be returned.
+0001c2e0: 0a0a 2020 2020 5265 7475 726e 730a 2020  ..    Returns.  
+0001c2f0: 2020 2d2d 2d2d 2d2d 2d0a 2020 2020 7079    -------.    py
+0001c300: 7669 7374 612e 556e 7374 7275 6374 7572  vista.Unstructur
+0001c310: 6564 4772 6964 207c 2073 7472 0a20 2020  edGrid | str.   
+0001c320: 2020 2020 2043 7275 7368 6564 2063 616e       Crushed can
+0001c330: 2064 6174 6173 6574 206f 7220 7061 7468   dataset or path
+0001c340: 2064 6570 656e 6469 6e67 206f 6e20 7468   depending on th
+0001c350: 6520 7661 6c75 6520 6f66 2060 606c 6f61  e value of ``loa
+0001c360: 6460 602e 0a0a 2020 2020 4578 616d 706c  d``...    Exampl
+0001c370: 6573 0a20 2020 202d 2d2d 2d2d 2d2d 2d0a  es.    --------.
+0001c380: 2020 2020 506c 6f74 2074 6865 2063 7275      Plot the cru
+0001c390: 7368 6564 2063 616e 2064 6174 6173 6574  shed can dataset
+0001c3a0: 2e0a 0a20 2020 203e 3e3e 2066 726f 6d20  ...    >>> from 
+0001c3b0: 7079 7669 7374 6120 696d 706f 7274 2065  pyvista import e
+0001c3c0: 7861 6d70 6c65 730a 2020 2020 3e3e 3e20  xamples.    >>> 
+0001c3d0: 696d 706f 7274 2070 7976 6973 7461 2061  import pyvista a
+0001c3e0: 7320 7076 0a20 2020 203e 3e3e 2064 6174  s pv.    >>> dat
+0001c3f0: 6173 6574 203d 2065 7861 6d70 6c65 732e  aset = examples.
+0001c400: 646f 776e 6c6f 6164 5f63 616e 5f63 7275  download_can_cru
+0001c410: 7368 6564 5f68 6466 2829 0a20 2020 203e  shed_hdf().    >
+0001c420: 3e3e 2064 6174 6173 6574 2e70 6c6f 7428  >> dataset.plot(
+0001c430: 736d 6f6f 7468 5f73 6861 6469 6e67 3d54  smooth_shading=T
+0001c440: 7275 6529 0a0a 2020 2020 2222 220a 2020  rue)..    """.  
+0001c450: 2020 7265 7475 726e 205f 646f 776e 6c6f    return _downlo
+0001c460: 6164 5f61 6e64 5f72 6561 6428 2768 6466  ad_and_read('hdf
+0001c470: 2f63 616e 2d76 7475 2e68 6466 272c 206c  /can-vtu.hdf', l
+0001c480: 6f61 643d 6c6f 6164 290a 0a0a 6465 6620  oad=load)...def 
+0001c490: 646f 776e 6c6f 6164 5f63 676e 735f 7374  download_cgns_st
+0001c4a0: 7275 6374 7572 6564 286c 6f61 643d 5472  ructured(load=Tr
+0001c4b0: 7565 293a 2020 2320 7072 6167 6d61 3a20  ue):  # pragma: 
+0001c4c0: 6e6f 2063 6f76 6572 0a20 2020 2022 2222  no cover.    """
+0001c4d0: 446f 776e 6c6f 6164 2074 6865 2073 7472  Download the str
+0001c4e0: 7563 7475 7265 6420 4347 4e53 2064 6174  uctured CGNS dat
+0001c4f0: 6173 6574 206d 6573 682e 0a0a 2020 2020  aset mesh...    
+0001c500: 4f72 6967 696e 616c 6c79 2064 6f77 6e6c  Originally downl
+0001c510: 6f61 6465 6420 6672 6f6d 2060 4346 4420  oaded from `CFD 
+0001c520: 4765 6e65 7261 6c20 4e6f 7461 7469 6f6e  General Notation
+0001c530: 2053 7973 7465 6d20 4578 616d 706c 6520   System Example 
+0001c540: 4669 6c65 730a 2020 2020 3c68 7474 7073  Files.    <https
+0001c550: 3a2f 2f63 676e 732e 6769 7468 7562 2e69  ://cgns.github.i
+0001c560: 6f2f 4347 4e53 4669 6c65 732e 6874 6d6c  o/CGNSFiles.html
+0001c570: 3e60 5f0a 0a20 2020 2050 6172 616d 6574  >`_..    Paramet
+0001c580: 6572 730a 2020 2020 2d2d 2d2d 2d2d 2d2d  ers.    --------
+0001c590: 2d2d 0a20 2020 206c 6f61 6420 3a20 626f  --.    load : bo
+0001c5a0: 6f6c 2c20 6465 6661 756c 743a 2054 7275  ol, default: Tru
+0001c5b0: 650a 2020 2020 2020 2020 4c6f 6164 2074  e.        Load t
+0001c5c0: 6865 2064 6174 6173 6574 2061 6674 6572  he dataset after
+0001c5d0: 2064 6f77 6e6c 6f61 6469 6e67 2069 7420   downloading it 
+0001c5e0: 7768 656e 2060 6054 7275 6560 602e 2020  when ``True``.  
+0001c5f0: 5365 7420 7468 6973 0a20 2020 2020 2020  Set this.       
+0001c600: 2074 6f20 6060 4661 6c73 6560 6020 616e   to ``False`` an
+0001c610: 6420 6f6e 6c79 2074 6865 2066 696c 656e  d only the filen
+0001c620: 616d 6520 7769 6c6c 2062 6520 7265 7475  ame will be retu
+0001c630: 726e 6564 2e0a 0a20 2020 2052 6574 7572  rned...    Retur
+0001c640: 6e73 0a20 2020 202d 2d2d 2d2d 2d2d 0a20  ns.    -------. 
+0001c650: 2020 2070 7976 6973 7461 2e4d 756c 7469     pyvista.Multi
+0001c660: 426c 6f63 6b20 7c20 7374 720a 2020 2020  Block | str.    
+0001c670: 2020 2020 5374 7275 6374 7572 6564 2c20      Structured, 
+0001c680: 3132 2062 6c6f 636b 2c20 332d 4420 636f  12 block, 3-D co
+0001c690: 6e73 7472 6963 7469 6e67 2063 6861 6e6e  nstricting chann
+0001c6a0: 656c 2c20 7769 7468 2065 7861 6d70 6c65  el, with example
+0001c6b0: 2075 7365 206f 660a 2020 2020 2020 2020   use of.        
+0001c6c0: 4661 6d69 6c79 5f74 2066 6f72 2042 4373  Family_t for BCs
+0001c6d0: 2028 4144 4620 7479 7065 292e 2049 6620   (ADF type). If 
+0001c6e0: 6060 6c6f 6164 6060 2069 7320 6060 4661  ``load`` is ``Fa
+0001c6f0: 6c73 6560 602c 2074 6865 6e20 7468 6520  lse``, then the 
+0001c700: 7061 7468 206f 6620 7468 650a 2020 2020  path of the.    
+0001c710: 2020 2020 6578 616d 706c 6520 4347 4e53      example CGNS
+0001c720: 2066 696c 6520 6973 2072 6574 7572 6e65   file is returne
+0001c730: 642e 0a0a 2020 2020 4578 616d 706c 6573  d...    Examples
+0001c740: 0a20 2020 202d 2d2d 2d2d 2d2d 2d0a 2020  .    --------.  
+0001c750: 2020 506c 6f74 2074 6865 2065 7861 6d70    Plot the examp
+0001c760: 6c65 2043 474e 5320 6461 7461 7365 742e  le CGNS dataset.
+0001c770: 0a0a 2020 2020 3e3e 3e20 6672 6f6d 2070  ..    >>> from p
+0001c780: 7976 6973 7461 2069 6d70 6f72 7420 6578  yvista import ex
+0001c790: 616d 706c 6573 0a20 2020 203e 3e3e 2069  amples.    >>> i
+0001c7a0: 6d70 6f72 7420 7079 7669 7374 6120 6173  mport pyvista as
+0001c7b0: 2070 760a 2020 2020 3e3e 3e20 6461 7461   pv.    >>> data
+0001c7c0: 7365 7420 3d20 6578 616d 706c 6573 2e64  set = examples.d
+0001c7d0: 6f77 6e6c 6f61 645f 6367 6e73 5f73 7472  ownload_cgns_str
+0001c7e0: 7563 7475 7265 6428 290a 2020 2020 3e3e  uctured().    >>
+0001c7f0: 3e20 6461 7461 7365 745b 305d 2e70 6c6f  > dataset[0].plo
+0001c800: 7428 7363 616c 6172 733d 2744 656e 7369  t(scalars='Densi
+0001c810: 7479 2729 0a0a 2020 2020 2222 220a 2020  ty')..    """.  
+0001c820: 2020 6669 6c65 6e61 6d65 203d 2064 6f77    filename = dow
+0001c830: 6e6c 6f61 645f 6669 6c65 2827 6367 6e73  nload_file('cgns
+0001c840: 2f73 716e 7a5f 732e 6164 662e 6367 6e73  /sqnz_s.adf.cgns
+0001c850: 2729 0a20 2020 2069 6620 6e6f 7420 6c6f  ').    if not lo
+0001c860: 6164 3a0a 2020 2020 2020 2020 7265 7475  ad:.        retu
+0001c870: 726e 2066 696c 656e 616d 650a 2020 2020  rn filename.    
+0001c880: 7265 7475 726e 2070 7976 6973 7461 2e67  return pyvista.g
+0001c890: 6574 5f72 6561 6465 7228 6669 6c65 6e61  et_reader(filena
+0001c8a0: 6d65 292e 7265 6164 2829 0a0a 0a64 6566  me).read()...def
+0001c8b0: 2064 6f77 6e6c 6f61 645f 7465 6370 6c6f   download_tecplo
+0001c8c0: 745f 6173 6369 6928 6c6f 6164 3d54 7275  t_ascii(load=Tru
+0001c8d0: 6529 3a20 2023 2070 7261 676d 613a 206e  e):  # pragma: n
+0001c8e0: 6f20 636f 7665 720a 2020 2020 2222 2244  o cover.    """D
+0001c8f0: 6f77 6e6c 6f61 6420 7468 6520 7369 6e67  ownload the sing
+0001c900: 6c65 2062 6c6f 636b 2041 5343 4949 2054  le block ASCII T
+0001c910: 6563 706c 6f74 2064 6174 6173 6574 2e0a  ecplot dataset..
+0001c920: 0a20 2020 204f 7269 6769 6e61 6c6c 7920  .    Originally 
+0001c930: 646f 776e 6c6f 6164 6564 2066 726f 6d20  downloaded from 
+0001c940: 5061 756c 2042 6f75 726b 6527 730a 2020  Paul Bourke's.  
+0001c950: 2020 6053 616d 706c 6520 6669 6c65 203c    `Sample file <
+0001c960: 6874 7470 3a2f 2f70 6175 6c62 6f75 726b  http://paulbourk
+0001c970: 652e 6e65 742f 6461 7461 666f 726d 6174  e.net/dataformat
+0001c980: 732f 7470 2f73 616d 706c 652e 7470 3e60  s/tp/sample.tp>`
+0001c990: 5f0a 0a20 2020 2050 6172 616d 6574 6572  _..    Parameter
+0001c9a0: 730a 2020 2020 2d2d 2d2d 2d2d 2d2d 2d2d  s.    ----------
+0001c9b0: 0a20 2020 206c 6f61 6420 3a20 626f 6f6c  .    load : bool
+0001c9c0: 2c20 6465 6661 756c 743a 2054 7275 650a  , default: True.
+0001c9d0: 2020 2020 2020 2020 4c6f 6164 2074 6865          Load the
+0001c9e0: 2064 6174 6173 6574 2061 6674 6572 2064   dataset after d
+0001c9f0: 6f77 6e6c 6f61 6469 6e67 2069 7420 7768  ownloading it wh
+0001ca00: 656e 2060 6054 7275 6560 602e 2020 5365  en ``True``.  Se
+0001ca10: 7420 7468 6973 0a20 2020 2020 2020 2074  t this.        t
+0001ca20: 6f20 6060 4661 6c73 6560 6020 616e 6420  o ``False`` and 
+0001ca30: 6f6e 6c79 2074 6865 2066 696c 656e 616d  only the filenam
+0001ca40: 6520 7769 6c6c 2062 6520 7265 7475 726e  e will be return
+0001ca50: 6564 2e0a 0a20 2020 2052 6574 7572 6e73  ed...    Returns
+0001ca60: 0a20 2020 202d 2d2d 2d2d 2d2d 0a20 2020  .    -------.   
+0001ca70: 2070 7976 6973 7461 2e4d 756c 7469 426c   pyvista.MultiBl
+0001ca80: 6f63 6b20 7c20 7374 720a 2020 2020 2020  ock | str.      
+0001ca90: 2020 4d75 6c74 6962 6c6f 636b 2066 6f72    Multiblock for
+0001caa0: 6d61 7420 7769 7468 206f 6e6c 7920 3120  mat with only 1 
+0001cab0: 6461 7461 2062 6c6f 636b 2c20 7369 6d70  data block, simp
+0001cac0: 6c65 2067 656f 6d65 7472 6963 2073 6861  le geometric sha
+0001cad0: 7065 2e0a 2020 2020 2020 2020 4966 2060  pe..        If `
+0001cae0: 606c 6f61 6460 6020 6973 2060 6046 616c  `load`` is ``Fal
+0001caf0: 7365 6060 2c20 7468 656e 2074 6865 2070  se``, then the p
+0001cb00: 6174 6820 6f66 2074 6865 2065 7861 6d70  ath of the examp
+0001cb10: 6c65 2054 6563 706c 6f74 2066 696c 650a  le Tecplot file.
+0001cb20: 2020 2020 2020 2020 6973 2072 6574 7572          is retur
+0001cb30: 6e65 642e 0a0a 2020 2020 4578 616d 706c  ned...    Exampl
+0001cb40: 6573 0a20 2020 202d 2d2d 2d2d 2d2d 2d0a  es.    --------.
+0001cb50: 2020 2020 506c 6f74 2074 6865 2065 7861      Plot the exa
+0001cb60: 6d70 6c65 2054 6563 706c 6f74 2064 6174  mple Tecplot dat
+0001cb70: 6173 6574 2e0a 0a20 2020 203e 3e3e 2066  aset...    >>> f
+0001cb80: 726f 6d20 7079 7669 7374 6120 696d 706f  rom pyvista impo
+0001cb90: 7274 2065 7861 6d70 6c65 730a 2020 2020  rt examples.    
+0001cba0: 3e3e 3e20 696d 706f 7274 2070 7976 6973  >>> import pyvis
+0001cbb0: 7461 2061 7320 7076 0a20 2020 203e 3e3e  ta as pv.    >>>
+0001cbc0: 2064 6174 6173 6574 203d 2065 7861 6d70   dataset = examp
+0001cbd0: 6c65 732e 646f 776e 6c6f 6164 5f74 6563  les.download_tec
+0001cbe0: 706c 6f74 5f61 7363 6969 2829 0a20 2020  plot_ascii().   
+0001cbf0: 203e 3e3e 2064 6174 6173 6574 2e70 6c6f   >>> dataset.plo
+0001cc00: 7428 290a 0a20 2020 2022 2222 0a20 2020  t()..    """.   
+0001cc10: 2066 696c 656e 616d 6520 3d20 646f 776e   filename = down
+0001cc20: 6c6f 6164 5f66 696c 6528 2774 6563 706c  load_file('tecpl
+0001cc30: 6f74 5f61 7363 6969 2e64 6174 2729 0a20  ot_ascii.dat'). 
+0001cc40: 2020 2069 6620 6e6f 7420 6c6f 6164 3a0a     if not load:.
+0001cc50: 2020 2020 2020 2020 7265 7475 726e 2066          return f
+0001cc60: 696c 656e 616d 650a 2020 2020 7265 7475  ilename.    retu
+0001cc70: 726e 2070 7976 6973 7461 2e67 6574 5f72  rn pyvista.get_r
+0001cc80: 6561 6465 7228 6669 6c65 6e61 6d65 292e  eader(filename).
+0001cc90: 7265 6164 2829 0a0a 0a64 6566 2064 6f77  read()...def dow
+0001cca0: 6e6c 6f61 645f 6367 6e73 5f6d 756c 7469  nload_cgns_multi
+0001ccb0: 286c 6f61 643d 5472 7565 293a 2020 2320  (load=True):  # 
+0001ccc0: 7072 6167 6d61 3a20 6e6f 2063 6f76 6572  pragma: no cover
+0001ccd0: 0a20 2020 2022 2222 446f 776e 6c6f 6164  .    """Download
+0001cce0: 2061 206d 756c 7469 656c 656d 656e 7420   a multielement 
+0001ccf0: 6169 7266 6f69 6c20 7769 7468 2061 2063  airfoil with a c
+0001cd00: 656c 6c20 6365 6e74 6572 6564 2073 6f6c  ell centered sol
+0001cd10: 7574 696f 6e2e 0a0a 2020 2020 4f72 6967  ution...    Orig
+0001cd20: 696e 616c 6c79 2064 6f77 6e6c 6f61 6465  inally downloade
+0001cd30: 6420 6672 6f6d 2060 4346 4420 4765 6e65  d from `CFD Gene
+0001cd40: 7261 6c20 4e6f 7461 7469 6f6e 2053 7973  ral Notation Sys
+0001cd50: 7465 6d20 4578 616d 706c 6520 4669 6c65  tem Example File
+0001cd60: 730a 2020 2020 3c68 7474 7073 3a2f 2f63  s.    <https://c
+0001cd70: 676e 732e 6769 7468 7562 2e69 6f2f 4347  gns.github.io/CG
+0001cd80: 4e53 4669 6c65 732e 6874 6d6c 3e60 5f0a  NSFiles.html>`_.
+0001cd90: 0a20 2020 2050 6172 616d 6574 6572 730a  .    Parameters.
+0001cda0: 2020 2020 2d2d 2d2d 2d2d 2d2d 2d2d 0a20      ----------. 
+0001cdb0: 2020 206c 6f61 6420 3a20 626f 6f6c 2c20     load : bool, 
+0001cdc0: 6465 6661 756c 743a 2054 7275 650a 2020  default: True.  
+0001cdd0: 2020 2020 2020 4c6f 6164 2074 6865 2064        Load the d
+0001cde0: 6174 6173 6574 2061 6674 6572 2064 6f77  ataset after dow
+0001cdf0: 6e6c 6f61 6469 6e67 2069 7420 7768 656e  nloading it when
+0001ce00: 2060 6054 7275 6560 602e 2020 5365 7420   ``True``.  Set 
+0001ce10: 7468 6973 0a20 2020 2020 2020 2074 6f20  this.        to 
+0001ce20: 6060 4661 6c73 6560 6020 616e 6420 6f6e  ``False`` and on
+0001ce30: 6c79 2074 6865 2066 696c 656e 616d 6520  ly the filename 
+0001ce40: 7769 6c6c 2062 6520 7265 7475 726e 6564  will be returned
+0001ce50: 2e0a 0a20 2020 2052 6574 7572 6e73 0a20  ...    Returns. 
+0001ce60: 2020 202d 2d2d 2d2d 2d2d 0a20 2020 2070     -------.    p
+0001ce70: 7976 6973 7461 2e4d 756c 7469 426c 6f63  yvista.MultiBloc
+0001ce80: 6b20 7c20 7374 720a 2020 2020 2020 2020  k | str.        
+0001ce90: 5374 7275 6374 7572 6564 2c20 3420 626c  Structured, 4 bl
+0001cea0: 6f63 6b73 2c20 3244 2028 3220 706c 616e  ocks, 2D (2 plan
+0001ceb0: 6573 2069 6e20 7468 6972 6420 6469 6d65  es in third dime
+0001cec0: 6e73 696f 6e29 206d 756c 7469 656c 656d  nsion) multielem
+0001ced0: 656e 740a 2020 2020 2020 2020 6169 7266  ent.        airf
+0001cee0: 6f69 6c2c 2077 6974 6820 6365 6c6c 2063  oil, with cell c
+0001cef0: 656e 7465 7265 6420 736f 6c75 7469 6f6e  entered solution
+0001cf00: 2e20 4966 2060 606c 6f61 6460 6020 6973  . If ``load`` is
+0001cf10: 2060 6046 616c 7365 6060 2c20 7468 656e   ``False``, then
+0001cf20: 2074 6865 2070 6174 6820 6f66 2074 6865   the path of the
+0001cf30: 0a20 2020 2020 2020 2065 7861 6d70 6c65  .        example
+0001cf40: 2043 474e 5320 6669 6c65 2069 7320 7265   CGNS file is re
+0001cf50: 7475 726e 6564 2e0a 0a20 2020 2045 7861  turned...    Exa
+0001cf60: 6d70 6c65 730a 2020 2020 2d2d 2d2d 2d2d  mples.    ------
+0001cf70: 2d2d 0a20 2020 2050 6c6f 7420 7468 6520  --.    Plot the 
+0001cf80: 6169 7266 6f69 6c20 6461 7461 7365 742e  airfoil dataset.
+0001cf90: 204d 6572 6765 2074 6865 206d 756c 7469   Merge the multi
+0001cfa0: 2d62 6c6f 636b 2061 6e64 2074 6865 6e20  -block and then 
+0001cfb0: 706c 6f74 2074 6865 2061 6972 666f 696c  plot the airfoil
+0001cfc0: 2773 0a20 2020 2060 6022 5669 7363 6f73  's.    ``"Viscos
+0001cfd0: 6974 7945 6464 7922 6060 2e20 436f 6e76  ityEddy"``. Conv
+0001cfe0: 6572 7420 7468 6520 6365 6c6c 2064 6174  ert the cell dat
+0001cff0: 6120 746f 2070 6f69 6e74 2064 6174 6120  a to point data 
+0001d000: 6173 2069 6e20 7468 6973 0a20 2020 2064  as in this.    d
+0001d010: 6174 6173 6574 2c20 7468 6520 736f 6c75  ataset, the solu
+0001d020: 7469 6f6e 2069 7320 7374 6f72 6564 2077  tion is stored w
+0001d030: 6974 6869 6e20 7468 6520 6365 6c6c 732e  ithin the cells.
+0001d040: 0a0a 2020 2020 3e3e 3e20 6672 6f6d 2070  ..    >>> from p
+0001d050: 7976 6973 7461 2069 6d70 6f72 7420 6578  yvista import ex
+0001d060: 616d 706c 6573 0a20 2020 203e 3e3e 2069  amples.    >>> i
+0001d070: 6d70 6f72 7420 7079 7669 7374 6120 6173  mport pyvista as
+0001d080: 2070 760a 2020 2020 3e3e 3e20 6461 7461   pv.    >>> data
+0001d090: 7365 7420 3d20 6578 616d 706c 6573 2e64  set = examples.d
+0001d0a0: 6f77 6e6c 6f61 645f 6367 6e73 5f6d 756c  ownload_cgns_mul
+0001d0b0: 7469 2829 0a20 2020 203e 3e3e 2075 6772  ti().    >>> ugr
+0001d0c0: 6964 203d 2064 6174 6173 6574 2e63 6f6d  id = dataset.com
+0001d0d0: 6269 6e65 2829 0a20 2020 203e 3e3e 2075  bine().    >>> u
+0001d0e0: 6772 6964 203d 2075 6772 6964 203d 2075  grid = ugrid = u
+0001d0f0: 6772 6964 2e63 656c 6c5f 6461 7461 5f74  grid.cell_data_t
+0001d100: 6f5f 706f 696e 745f 6461 7461 2829 0a20  o_point_data(). 
+0001d110: 2020 203e 3e3e 2075 6772 6964 2e70 6c6f     >>> ugrid.plo
+0001d120: 7428 0a20 2020 202e 2e2e 2020 2020 2063  t(.    ...     c
+0001d130: 6d61 703d 2762 7772 272c 0a20 2020 202e  map='bwr',.    .
+0001d140: 2e2e 2020 2020 2073 6361 6c61 7273 3d27  ..     scalars='
+0001d150: 5669 7363 6f73 6974 7945 6464 7927 2c0a  ViscosityEddy',.
+0001d160: 2020 2020 2e2e 2e20 2020 2020 7a6f 6f6d      ...     zoom
+0001d170: 3d34 2c0a 2020 2020 2e2e 2e20 2020 2020  =4,.    ...     
+0001d180: 6370 6f73 3d27 787a 272c 0a20 2020 202e  cpos='xz',.    .
+0001d190: 2e2e 2020 2020 2073 686f 775f 7363 616c  ..     show_scal
+0001d1a0: 6172 5f62 6172 3d46 616c 7365 2c0a 2020  ar_bar=False,.  
+0001d1b0: 2020 2e2e 2e20 290a 0a20 2020 2022 2222    ... )..    """
+0001d1c0: 0a20 2020 2066 696c 656e 616d 6520 3d20  .    filename = 
+0001d1d0: 646f 776e 6c6f 6164 5f66 696c 6528 2763  download_file('c
+0001d1e0: 676e 732f 6d75 6c74 692e 6367 6e73 2729  gns/multi.cgns')
+0001d1f0: 0a20 2020 2069 6620 6e6f 7420 6c6f 6164  .    if not load
+0001d200: 3a0a 2020 2020 2020 2020 7265 7475 726e  :.        return
+0001d210: 2066 696c 656e 616d 650a 2020 2020 7265   filename.    re
+0001d220: 6164 6572 203d 2070 7976 6973 7461 2e67  ader = pyvista.g
+0001d230: 6574 5f72 6561 6465 7228 6669 6c65 6e61  et_reader(filena
+0001d240: 6d65 290a 0a20 2020 2023 2064 6973 6162  me)..    # disab
+0001d250: 6c65 2072 6561 6469 6e67 2074 6865 2062  le reading the b
+0001d260: 6f75 6e64 6172 7920 7061 7463 682e 2041  oundary patch. A
+0001d270: 7320 6f66 2056 544b 2039 2e31 2e30 2074  s of VTK 9.1.0 t
+0001d280: 6869 7320 6765 6e65 7261 7465 730a 2020  his generates.  
+0001d290: 2020 2320 6d65 7373 6167 6573 206c 696b    # messages lik
+0001d2a0: 6520 2253 6b69 7070 696e 6720 4243 5f74  e "Skipping BC_t
+0001d2b0: 206e 6f64 653a 2042 435f 7420 7479 7065   node: BC_t type
+0001d2c0: 2027 4243 4661 7266 6965 6c64 2720 6e6f   'BCFarfield' no
+0001d2d0: 7420 7375 7070 6f72 7465 640a 2020 2020  t supported.    
+0001d2e0: 2320 7965 742e 220a 2020 2020 7265 6164  # yet.".    read
+0001d2f0: 6572 2e6c 6f61 645f 626f 756e 6461 7279  er.load_boundary
+0001d300: 5f70 6174 6368 203d 2046 616c 7365 0a20  _patch = False. 
+0001d310: 2020 2072 6574 7572 6e20 7265 6164 6572     return reader
+0001d320: 2e72 6561 6428 290a 0a0a 6465 6620 646f  .read()...def do
+0001d330: 776e 6c6f 6164 5f64 6963 6f6d 5f73 7461  wnload_dicom_sta
+0001d340: 636b 286c 6f61 643a 2062 6f6f 6c20 3d20  ck(load: bool = 
+0001d350: 5472 7565 2920 2d3e 2055 6e69 6f6e 5b70  True) -> Union[p
+0001d360: 7976 6973 7461 2e49 6d61 6765 4461 7461  yvista.ImageData
+0001d370: 2c20 7374 725d 3a20 2023 2070 7261 676d  , str]:  # pragm
+0001d380: 613a 206e 6f20 636f 7665 720a 2020 2020  a: no cover.    
+0001d390: 2222 2244 6f77 6e6c 6f61 6420 5443 4941  """Download TCIA
+0001d3a0: 2044 4943 4f4d 2073 7461 636b 2076 6f6c   DICOM stack vol
+0001d3b0: 756d 652e 0a0a 2020 2020 4f72 6967 696e  ume...    Origin
+0001d3c0: 616c 2064 6f77 6e6c 6f61 6420 6672 6f6d  al download from
+0001d3d0: 2074 6865 2060 5468 6520 4361 6e63 6572   the `The Cancer
+0001d3e0: 2049 6d61 6769 6e67 2041 7263 6869 7665   Imaging Archive
+0001d3f0: 2028 5443 4941 290a 2020 2020 3c68 7474   (TCIA).    <htt
+0001d400: 7073 3a2f 2f77 7777 2e63 616e 6365 7269  ps://www.canceri
+0001d410: 6d61 6769 6e67 6172 6368 6976 652e 6e65  magingarchive.ne
+0001d420: 742f 3e60 5f2e 2054 6869 7320 6973 2070  t/>`_. This is p
+0001d430: 6172 7420 6f66 2074 6865 0a20 2020 2043  art of the.    C
+0001d440: 6c69 6e69 6361 6c20 5072 6f74 656f 6d69  linical Proteomi
+0001d450: 6320 5475 6d6f 7220 416e 616c 7973 6973  c Tumor Analysis
+0001d460: 2043 6f6e 736f 7274 6975 6d20 5361 7263   Consortium Sarc
+0001d470: 6f6d 6173 2028 4350 5441 432d 5341 5229  omas (CPTAC-SAR)
+0001d480: 0a20 2020 2063 6f6c 6c65 6374 696f 6e2e  .    collection.
+0001d490: 0a0a 2020 2020 5061 7261 6d65 7465 7273  ..    Parameters
+0001d4a0: 0a20 2020 202d 2d2d 2d2d 2d2d 2d2d 2d0a  .    ----------.
+0001d4b0: 2020 2020 6c6f 6164 203a 2062 6f6f 6c2c      load : bool,
+0001d4c0: 2064 6566 6175 6c74 3a20 5472 7565 0a20   default: True. 
+0001d4d0: 2020 2020 2020 204c 6f61 6420 7468 6520         Load the 
+0001d4e0: 6461 7461 7365 7420 6166 7465 7220 646f  dataset after do
+0001d4f0: 776e 6c6f 6164 696e 6720 6974 2077 6865  wnloading it whe
+0001d500: 6e20 6060 5472 7565 6060 2e20 2053 6574  n ``True``.  Set
+0001d510: 2074 6869 730a 2020 2020 2020 2020 746f   this.        to
+0001d520: 2060 6046 616c 7365 6060 2061 6e64 206f   ``False`` and o
+0001d530: 6e6c 7920 7468 6520 6669 6c65 6e61 6d65  nly the filename
+0001d540: 2077 696c 6c20 6265 2072 6574 7572 6e65   will be returne
+0001d550: 642e 0a0a 2020 2020 5265 7475 726e 730a  d...    Returns.
+0001d560: 2020 2020 2d2d 2d2d 2d2d 2d0a 2020 2020      -------.    
+0001d570: 7079 7669 7374 612e 496d 6167 6544 6174  pyvista.ImageDat
+0001d580: 6120 7c20 7374 720a 2020 2020 2020 2020  a | str.        
+0001d590: 4461 7461 5365 7420 6f72 2070 6174 6820  DataSet or path 
+0001d5a0: 6465 7065 6e64 696e 6720 6f6e 2060 606c  depending on ``l
+0001d5b0: 6f61 6460 602e 0a0a 2020 2020 5265 6665  oad``...    Refe
+0001d5c0: 7265 6e63 6573 0a20 2020 202d 2d2d 2d2d  rences.    -----
+0001d5d0: 2d2d 2d2d 2d0a 2020 2020 2a20 2a2a 4461  -----.    * **Da
+0001d5e0: 7461 2043 6974 6174 696f 6e2a 2a0a 0a20  ta Citation**.. 
+0001d5f0: 2020 2020 2020 204e 6174 696f 6e61 6c20         National 
+0001d600: 4361 6e63 6572 2049 6e73 7469 7475 7465  Cancer Institute
+0001d610: 2043 6c69 6e69 6361 6c20 5072 6f74 656f   Clinical Proteo
+0001d620: 6d69 6320 5475 6d6f 7220 416e 616c 7973  mic Tumor Analys
+0001d630: 6973 2043 6f6e 736f 7274 6975 6d0a 2020  is Consortium.  
+0001d640: 2020 2020 2020 2843 5054 4143 292e 2028        (CPTAC). (
+0001d650: 3230 3138 292e 2020 5261 6469 6f6c 6f67  2018).  Radiolog
+0001d660: 7920 4461 7461 2066 726f 6d20 7468 6520  y Data from the 
+0001d670: 436c 696e 6963 616c 2050 726f 7465 6f6d  Clinical Proteom
+0001d680: 6963 2054 756d 6f72 0a20 2020 2020 2020  ic Tumor.       
+0001d690: 2041 6e61 6c79 7369 7320 436f 6e73 6f72   Analysis Consor
+0001d6a0: 7469 756d 2053 6172 636f 6d61 7320 5b43  tium Sarcomas [C
+0001d6b0: 5054 4143 2d53 4152 5d20 636f 6c6c 6563  PTAC-SAR] collec
+0001d6c0: 7469 6f6e 205b 4461 7461 2073 6574 5d2e  tion [Data set].
+0001d6d0: 2054 6865 0a20 2020 2020 2020 2043 616e   The.        Can
+0001d6e0: 6365 7220 496d 6167 696e 6720 4172 6368  cer Imaging Arch
+0001d6f0: 6976 652e 2020 444f 493a 2031 302e 3739  ive.  DOI: 10.79
+0001d700: 3337 2f54 4349 412e 3230 3139 2e39 6274  37/TCIA.2019.9bt
+0001d710: 3233 7239 350a 0a20 2020 202a 202a 2a41  23r95..    * **A
+0001d720: 636b 6e6f 776c 6564 6765 6d65 6e74 2a2a  cknowledgement**
+0001d730: 0a0a 2020 2020 2020 2020 4461 7461 2075  ..        Data u
+0001d740: 7365 6420 696e 2074 6869 7320 7075 626c  sed in this publ
+0001d750: 6963 6174 696f 6e20 7765 7265 2067 656e  ication were gen
+0001d760: 6572 6174 6564 2062 7920 7468 6520 4e61  erated by the Na
+0001d770: 7469 6f6e 616c 2043 616e 6365 7220 496e  tional Cancer In
+0001d780: 7374 6974 7574 6520 436c 696e 6963 616c  stitute Clinical
+0001d790: 0a20 2020 2020 2020 2050 726f 7465 6f6d  .        Proteom
+0001d7a0: 6963 2054 756d 6f72 2041 6e61 6c79 7369  ic Tumor Analysi
+0001d7b0: 7320 436f 6e73 6f72 7469 756d 2028 4350  s Consortium (CP
+0001d7c0: 5441 4329 2e0a 0a20 2020 202a 202a 2a54  TAC)...    * **T
+0001d7d0: 4349 4120 4369 7461 7469 6f6e 2a2a 0a0a  CIA Citation**..
+0001d7e0: 2020 2020 2020 2020 436c 6172 6b20 4b2c          Clark K,
+0001d7f0: 2056 656e 6474 2042 2c20 536d 6974 6820   Vendt B, Smith 
+0001d800: 4b2c 2046 7265 796d 616e 6e20 4a2c 204b  K, Freymann J, K
+0001d810: 6972 6279 204a 2c20 4b6f 7070 656c 2050  irby J, Koppel P
+0001d820: 2c20 4d6f 6f72 6520 532c 2050 6869 6c6c  , Moore S, Phill
+0001d830: 6970 7320 532c 0a20 2020 2020 2020 204d  ips S,.        M
+0001d840: 6166 6669 7474 2044 2c20 5072 696e 676c  affitt D, Pringl
+0001d850: 6520 4d2c 2054 6172 626f 7820 4c2c 2050  e M, Tarbox L, P
+0001d860: 7269 6f72 2046 2e20 5468 6520 4361 6e63  rior F. The Canc
+0001d870: 6572 2049 6d61 6769 6e67 2041 7263 6869  er Imaging Archi
+0001d880: 7665 2028 5443 4941 293a 2020 2320 7072  ve (TCIA):  # pr
+0001d890: 6167 6d61 3a20 6e6f 2063 6f76 6572 0a20  agma: no cover. 
+0001d8a0: 2020 2020 2020 204d 6169 6e74 6169 6e69         Maintaini
+0001d8b0: 6e67 2061 6e64 204f 7065 7261 7469 6e67  ng and Operating
+0001d8c0: 2061 2050 7562 6c69 6320 496e 666f 726d   a Public Inform
+0001d8d0: 6174 696f 6e20 5265 706f 7369 746f 7279  ation Repository
+0001d8e0: 2c20 4a6f 7572 6e61 6c20 6f66 2044 6967  , Journal of Dig
+0001d8f0: 6974 616c 2049 6d61 6769 6e67 2c0a 2020  ital Imaging,.  
+0001d900: 2020 2020 2020 566f 6c75 6d65 2032 362c        Volume 26,
+0001d910: 204e 756d 6265 7220 362c 2044 6563 656d   Number 6, Decem
+0001d920: 6265 722c 2032 3031 332c 2070 7020 3130  ber, 2013, pp 10
+0001d930: 3435 2d31 3035 372e 2064 6f69 3a20 3130  45-1057. doi: 10
+0001d940: 2e31 3030 372f 7331 3032 3738 2d30 3133  .1007/s10278-013
+0001d950: 2d39 3632 322d 370a 0a20 2020 2045 7861  -9622-7..    Exa
+0001d960: 6d70 6c65 730a 2020 2020 2d2d 2d2d 2d2d  mples.    ------
+0001d970: 2d2d 0a20 2020 203e 3e3e 2066 726f 6d20  --.    >>> from 
+0001d980: 7079 7669 7374 6120 696d 706f 7274 2065  pyvista import e
+0001d990: 7861 6d70 6c65 730a 2020 2020 3e3e 3e20  xamples.    >>> 
+0001d9a0: 6461 7461 7365 7420 3d20 6578 616d 706c  dataset = exampl
+0001d9b0: 6573 2e64 6f77 6e6c 6f61 645f 6469 636f  es.download_dico
+0001d9c0: 6d5f 7374 6163 6b28 290a 2020 2020 3e3e  m_stack().    >>
+0001d9d0: 3e20 6461 7461 7365 742e 706c 6f74 2876  > dataset.plot(v
+0001d9e0: 6f6c 756d 653d 5472 7565 2c20 7a6f 6f6d  olume=True, zoom
+0001d9f0: 3d33 2c20 7368 6f77 5f73 6361 6c61 725f  =3, show_scalar_
+0001da00: 6261 723d 4661 6c73 6529 0a0a 2020 2020  bar=False)..    
+0001da10: 2222 220a 2020 2020 666e 616d 6573 203d  """.    fnames =
+0001da20: 205f 646f 776e 6c6f 6164 5f61 7263 6869   _download_archi
+0001da30: 7665 2827 4449 434f 4d5f 5374 6163 6b2f  ve('DICOM_Stack/
+0001da40: 6461 7461 2e7a 6970 2729 0a20 2020 2070  data.zip').    p
+0001da50: 6174 6820 3d20 6f73 2e70 6174 682e 6469  ath = os.path.di
+0001da60: 726e 616d 6528 666e 616d 6573 5b30 5d29  rname(fnames[0])
+0001da70: 0a20 2020 2069 6620 6c6f 6164 3a0a 2020  .    if load:.  
+0001da80: 2020 2020 2020 7265 6164 6572 203d 2044        reader = D
+0001da90: 4943 4f4d 5265 6164 6572 2870 6174 6829  ICOMReader(path)
+0001daa0: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
+0001dab0: 7265 6164 6572 2e72 6561 6428 290a 2020  reader.read().  
+0001dac0: 2020 7265 7475 726e 2070 6174 680a 0a0a    return path...
+0001dad0: 6465 6620 646f 776e 6c6f 6164 5f70 6172  def download_par
+0001dae0: 6368 6564 5f63 616e 616c 5f34 6b28 6c6f  ched_canal_4k(lo
+0001daf0: 6164 3d54 7275 6529 3a20 2023 2070 7261  ad=True):  # pra
+0001db00: 676d 613a 206e 6f20 636f 7665 720a 2020  gma: no cover.  
+0001db10: 2020 2222 2244 6f77 6e6c 6f61 6420 7061    """Download pa
+0001db20: 7263 6865 6420 6361 6e61 6c20 346b 2064  rched canal 4k d
+0001db30: 6174 6173 6574 2e0a 0a20 2020 2050 6172  ataset...    Par
+0001db40: 616d 6574 6572 730a 2020 2020 2d2d 2d2d  ameters.    ----
+0001db50: 2d2d 2d2d 2d2d 0a20 2020 206c 6f61 6420  ------.    load 
+0001db60: 3a20 626f 6f6c 2c20 6465 6661 756c 743a  : bool, default:
+0001db70: 2054 7275 650a 2020 2020 2020 2020 4c6f   True.        Lo
+0001db80: 6164 2074 6865 2064 6174 6173 6574 2061  ad the dataset a
+0001db90: 6674 6572 2064 6f77 6e6c 6f61 6469 6e67  fter downloading
+0001dba0: 2069 7420 7768 656e 2060 6054 7275 6560   it when ``True`
+0001dbb0: 602e 2020 5365 7420 7468 6973 0a20 2020  `.  Set this.   
+0001dbc0: 2020 2020 2074 6f20 6060 4661 6c73 6560       to ``False`
+0001dbd0: 6020 616e 6420 6f6e 6c79 2074 6865 2066  ` and only the f
+0001dbe0: 696c 656e 616d 6520 7769 6c6c 2062 6520  ilename will be 
+0001dbf0: 7265 7475 726e 6564 2e0a 0a20 2020 2052  returned...    R
+0001dc00: 6574 7572 6e73 0a20 2020 202d 2d2d 2d2d  eturns.    -----
+0001dc10: 2d2d 0a20 2020 2070 7976 6973 7461 2e54  --.    pyvista.T
+0001dc20: 6578 7475 7265 207c 2073 7472 0a20 2020  exture | str.   
+0001dc30: 2020 2020 2044 6174 6153 6574 206f 7220       DataSet or 
+0001dc40: 6669 6c65 6e61 6d65 2064 6570 656e 6469  filename dependi
+0001dc50: 6e67 206f 6e20 6060 6c6f 6164 6060 2e0a  ng on ``load``..
+0001dc60: 0a20 2020 2045 7861 6d70 6c65 730a 2020  .    Examples.  
+0001dc70: 2020 2d2d 2d2d 2d2d 2d2d 0a20 2020 203e    --------.    >
+0001dc80: 3e3e 2066 726f 6d20 7079 7669 7374 6120  >> from pyvista 
+0001dc90: 696d 706f 7274 2065 7861 6d70 6c65 730a  import examples.
+0001dca0: 2020 2020 3e3e 3e20 6461 7461 7365 7420      >>> dataset 
+0001dcb0: 3d20 6578 616d 706c 6573 2e64 6f77 6e6c  = examples.downl
+0001dcc0: 6f61 645f 7061 7263 6865 645f 6361 6e61  oad_parched_cana
+0001dcd0: 6c5f 346b 2829 0a20 2020 203e 3e3e 2064  l_4k().    >>> d
+0001dce0: 6174 6173 6574 2e70 6c6f 7428 6370 6f73  ataset.plot(cpos
+0001dcf0: 3d22 7879 2229 0a0a 2020 2020 2222 220a  ="xy")..    """.
+0001dd00: 2020 2020 7265 7475 726e 205f 646f 776e      return _down
+0001dd10: 6c6f 6164 5f61 6e64 5f72 6561 6428 2270  load_and_read("p
+0001dd20: 6172 6368 6564 5f63 616e 616c 5f34 6b2e  arched_canal_4k.
+0001dd30: 6864 7222 2c20 7465 7874 7572 653d 5472  hdr", texture=Tr
+0001dd40: 7565 2c20 6c6f 6164 3d6c 6f61 6429 0a0a  ue, load=load)..
+0001dd50: 0a64 6566 2064 6f77 6e6c 6f61 645f 6365  .def download_ce
+0001dd60: 6c6c 735f 6e64 286c 6f61 643d 5472 7565  lls_nd(load=True
+0001dd70: 293a 2020 2320 7072 6167 6d61 3a20 6e6f  ):  # pragma: no
+0001dd80: 2063 6f76 6572 0a20 2020 2022 2222 446f   cover.    """Do
+0001dd90: 776e 6c6f 6164 2065 7861 6d70 6c65 2041  wnload example A
+0001dda0: 5653 2055 4344 2064 6174 6173 6574 2e0a  VS UCD dataset..
+0001ddb0: 0a20 2020 2050 6172 616d 6574 6572 730a  .    Parameters.
+0001ddc0: 2020 2020 2d2d 2d2d 2d2d 2d2d 2d2d 0a20      ----------. 
+0001ddd0: 2020 206c 6f61 6420 3a20 626f 6f6c 2c20     load : bool, 
+0001dde0: 6465 6661 756c 743a 2054 7275 650a 2020  default: True.  
+0001ddf0: 2020 2020 2020 4c6f 6164 2074 6865 2064        Load the d
+0001de00: 6174 6173 6574 2061 6674 6572 2064 6f77  ataset after dow
+0001de10: 6e6c 6f61 6469 6e67 2069 7420 7768 656e  nloading it when
+0001de20: 2060 6054 7275 6560 602e 2020 5365 7420   ``True``.  Set 
+0001de30: 7468 6973 0a20 2020 2020 2020 2074 6f20  this.        to 
+0001de40: 6060 4661 6c73 6560 6020 616e 6420 6f6e  ``False`` and on
+0001de50: 6c79 2074 6865 2066 696c 656e 616d 6520  ly the filename 
+0001de60: 7769 6c6c 2062 6520 7265 7475 726e 6564  will be returned
+0001de70: 2e0a 0a20 2020 2052 6574 7572 6e73 0a20  ...    Returns. 
+0001de80: 2020 202d 2d2d 2d2d 2d2d 0a20 2020 2070     -------.    p
+0001de90: 7976 6973 7461 2e55 6e73 7472 7563 7475  yvista.Unstructu
+0001dea0: 7265 6447 7269 6420 7c20 7374 720a 2020  redGrid | str.  
+0001deb0: 2020 2020 2020 4461 7461 5365 7420 6f72        DataSet or
+0001dec0: 2066 696c 656e 616d 6520 6465 7065 6e64   filename depend
+0001ded0: 696e 6720 6f6e 2060 606c 6f61 6460 602e  ing on ``load``.
+0001dee0: 0a0a 2020 2020 4578 616d 706c 6573 0a20  ..    Examples. 
+0001def0: 2020 202d 2d2d 2d2d 2d2d 2d0a 2020 2020     --------.    
+0001df00: 3e3e 3e20 6672 6f6d 2070 7976 6973 7461  >>> from pyvista
+0001df10: 2069 6d70 6f72 7420 6578 616d 706c 6573   import examples
+0001df20: 0a20 2020 203e 3e3e 2064 6174 6173 6574  .    >>> dataset
+0001df30: 203d 2065 7861 6d70 6c65 732e 646f 776e   = examples.down
+0001df40: 6c6f 6164 5f63 656c 6c73 5f6e 6428 290a  load_cells_nd().
+0001df50: 2020 2020 3e3e 3e20 6461 7461 7365 742e      >>> dataset.
+0001df60: 706c 6f74 2863 706f 733d 2278 7922 290a  plot(cpos="xy").
+0001df70: 0a20 2020 2022 2222 0a20 2020 2072 6574  .    """.    ret
+0001df80: 7572 6e20 5f64 6f77 6e6c 6f61 645f 616e  urn _download_an
+0001df90: 645f 7265 6164 2822 6365 6c6c 736e 642e  d_read("cellsnd.
+0001dfa0: 6173 6369 692e 696e 7022 2c20 6c6f 6164  ascii.inp", load
+0001dfb0: 3d6c 6f61 6429 0a0a 0a64 6566 2064 6f77  =load)...def dow
+0001dfc0: 6e6c 6f61 645f 6d6f 6f6e 6c61 6e64 696e  nload_moonlandin
+0001dfd0: 675f 696d 6167 6528 6c6f 6164 3d54 7275  g_image(load=Tru
+0001dfe0: 6529 3a20 2023 2070 7261 676d 613a 206e  e):  # pragma: n
+0001dff0: 6f20 636f 7665 720a 2020 2020 2222 2244  o cover.    """D
+0001e000: 6f77 6e6c 6f61 6420 7468 6520 4d6f 6f6e  ownload the Moon
+0001e010: 206c 616e 6469 6e67 2069 6d61 6765 2e0a   landing image..
+0001e020: 0a20 2020 2054 6869 7320 6973 2061 206e  .    This is a n
+0001e030: 6f69 7379 2069 6d61 6765 206f 7269 6769  oisy image origi
+0001e040: 6e61 6c6c 7920 6f62 7461 696e 6564 2066  nally obtained f
+0001e050: 726f 6d20 6053 6369 7079 204c 6563 7475  rom `Scipy Lectu
+0001e060: 7265 204e 6f74 6573 0a20 2020 203c 6874  re Notes.    <ht
+0001e070: 7470 733a 2f2f 7363 6970 792d 6c65 6374  tps://scipy-lect
+0001e080: 7572 6573 2e6f 7267 2f69 6e64 6578 2e68  ures.org/index.h
+0001e090: 746d 6c3e 605f 2061 6e64 2063 616e 2062  tml>`_ and can b
+0001e0a0: 6520 7573 6564 2074 6f20 6465 6d6f 6e73  e used to demons
+0001e0b0: 7472 6174 6520 610a 2020 2020 6c6f 7720  trate a.    low 
+0001e0c0: 7061 7373 2066 696c 7465 722e 0a0a 2020  pass filter...  
+0001e0d0: 2020 5365 6520 7468 6520 6073 6369 7079    See the `scipy
+0001e0e0: 2d6c 6563 7475 7265 7320 6c69 6365 6e73  -lectures licens
+0001e0f0: 650a 2020 2020 3c68 7474 703a 2f2f 7363  e.    <http://sc
+0001e100: 6970 792d 6c65 6374 7572 6573 2e6f 7267  ipy-lectures.org
+0001e110: 2f70 7265 6661 6365 2e68 746d 6c23 6c69  /preface.html#li
+0001e120: 6365 6e73 653e 605f 2066 6f72 206d 6f72  cense>`_ for mor
+0001e130: 6520 6465 7461 696c 730a 2020 2020 7265  e details.    re
+0001e140: 6761 7264 696e 6720 7468 6973 2069 6d61  garding this ima
+0001e150: 6765 2773 2075 7365 2061 6e64 2064 6973  ge's use and dis
+0001e160: 7472 6962 7574 696f 6e2e 0a0a 2020 2020  tribution...    
+0001e170: 5061 7261 6d65 7465 7273 0a20 2020 202d  Parameters.    -
+0001e180: 2d2d 2d2d 2d2d 2d2d 2d0a 2020 2020 6c6f  ---------.    lo
+0001e190: 6164 203a 2062 6f6f 6c2c 2064 6566 6175  ad : bool, defau
+0001e1a0: 6c74 3a20 5472 7565 0a20 2020 2020 2020  lt: True.       
+0001e1b0: 204c 6f61 6420 7468 6520 6461 7461 7365   Load the datase
+0001e1c0: 7420 6166 7465 7220 646f 776e 6c6f 6164  t after download
+0001e1d0: 696e 6720 6974 2077 6865 6e20 6060 5472  ing it when ``Tr
+0001e1e0: 7565 6060 2e20 2053 6574 2074 6869 730a  ue``.  Set this.
+0001e1f0: 2020 2020 2020 2020 746f 2060 6046 616c          to ``Fal
+0001e200: 7365 6060 2061 6e64 206f 6e6c 7920 7468  se`` and only th
+0001e210: 6520 6669 6c65 6e61 6d65 2077 696c 6c20  e filename will 
+0001e220: 6265 2072 6574 7572 6e65 642e 0a0a 2020  be returned...  
+0001e230: 2020 5265 7475 726e 730a 2020 2020 2d2d    Returns.    --
+0001e240: 2d2d 2d2d 2d0a 2020 2020 7079 7669 7374  -----.    pyvist
+0001e250: 612e 496d 6167 6544 6174 6120 7c20 7374  a.ImageData | st
+0001e260: 720a 2020 2020 2020 2020 6060 4461 7461  r.        ``Data
+0001e270: 5365 7460 6020 6f72 2066 696c 656e 616d  Set`` or filenam
+0001e280: 6520 6465 7065 6e64 696e 6720 6f6e 2060  e depending on `
+0001e290: 606c 6f61 6460 602e 0a0a 2020 2020 4578  `load``...    Ex
+0001e2a0: 616d 706c 6573 0a20 2020 202d 2d2d 2d2d  amples.    -----
+0001e2b0: 2d2d 2d0a 2020 2020 3e3e 3e20 6672 6f6d  ---.    >>> from
+0001e2c0: 2070 7976 6973 7461 2069 6d70 6f72 7420   pyvista import 
+0001e2d0: 6578 616d 706c 6573 0a20 2020 203e 3e3e  examples.    >>>
+0001e2e0: 2064 6174 6173 6574 203d 2065 7861 6d70   dataset = examp
+0001e2f0: 6c65 732e 646f 776e 6c6f 6164 5f6d 6f6f  les.download_moo
+0001e300: 6e6c 616e 6469 6e67 5f69 6d61 6765 2829  nlanding_image()
+0001e310: 0a20 2020 203e 3e3e 2064 6174 6173 6574  .    >>> dataset
+0001e320: 2e70 6c6f 7428 0a20 2020 202e 2e2e 2020  .plot(.    ...  
+0001e330: 2020 2063 706f 733d 2778 7927 2c0a 2020     cpos='xy',.  
+0001e340: 2020 2e2e 2e20 2020 2020 636d 6170 3d27    ...     cmap='
+0001e350: 6772 6179 272c 0a20 2020 202e 2e2e 2020  gray',.    ...  
+0001e360: 2020 2062 6163 6b67 726f 756e 643d 2777     background='w
+0001e370: 272c 0a20 2020 202e 2e2e 2020 2020 2073  ',.    ...     s
+0001e380: 686f 775f 7363 616c 6172 5f62 6172 3d46  how_scalar_bar=F
+0001e390: 616c 7365 2c0a 2020 2020 2e2e 2e20 290a  alse,.    ... ).
+0001e3a0: 0a20 2020 2053 6565 203a 7265 663a 6069  .    See :ref:`i
+0001e3b0: 6d61 6765 5f66 6674 5f65 7861 6d70 6c65  mage_fft_example
+0001e3c0: 6020 666f 7220 6120 6675 6c6c 2065 7861  ` for a full exa
+0001e3d0: 6d70 6c65 2075 7369 6e67 2074 6869 7320  mple using this 
+0001e3e0: 6461 7461 7365 742e 0a0a 2020 2020 2222  dataset...    ""
+0001e3f0: 220a 2020 2020 7265 7475 726e 205f 646f  ".    return _do
+0001e400: 776e 6c6f 6164 5f61 6e64 5f72 6561 6428  wnload_and_read(
+0001e410: 276d 6f6f 6e6c 616e 6469 6e67 2e70 6e67  'moonlanding.png
+0001e420: 272c 206c 6f61 643d 6c6f 6164 290a 0a0a  ', load=load)...
+0001e430: 6465 6620 646f 776e 6c6f 6164 5f61 6e67  def download_ang
+0001e440: 756c 6172 5f73 6563 746f 7228 6c6f 6164  ular_sector(load
+0001e450: 3d54 7275 6529 3a20 2023 2070 7261 676d  =True):  # pragm
+0001e460: 613a 206e 6f20 636f 7665 720a 2020 2020  a: no cover.    
+0001e470: 2222 2244 6f77 6e6c 6f61 6420 7468 6520  """Download the 
+0001e480: 616e 6775 6c61 7220 7365 6374 6f72 2064  angular sector d
+0001e490: 6174 6173 6574 2e0a 0a20 2020 2050 6172  ataset...    Par
+0001e4a0: 616d 6574 6572 730a 2020 2020 2d2d 2d2d  ameters.    ----
+0001e4b0: 2d2d 2d2d 2d2d 0a20 2020 206c 6f61 6420  ------.    load 
+0001e4c0: 3a20 626f 6f6c 2c20 6465 6661 756c 743a  : bool, default:
+0001e4d0: 2054 7275 650a 2020 2020 2020 2020 4c6f   True.        Lo
+0001e4e0: 6164 2074 6865 2064 6174 6173 6574 2061  ad the dataset a
+0001e4f0: 6674 6572 2064 6f77 6e6c 6f61 6469 6e67  fter downloading
+0001e500: 2069 7420 7768 656e 2060 6054 7275 6560   it when ``True`
+0001e510: 602e 2020 5365 7420 7468 6973 0a20 2020  `.  Set this.   
+0001e520: 2020 2020 2074 6f20 6060 4661 6c73 6560       to ``False`
+0001e530: 6020 616e 6420 6f6e 6c79 2074 6865 2066  ` and only the f
+0001e540: 696c 656e 616d 6520 7769 6c6c 2062 6520  ilename will be 
+0001e550: 7265 7475 726e 6564 2e0a 0a20 2020 2052  returned...    R
+0001e560: 6574 7572 6e73 0a20 2020 202d 2d2d 2d2d  eturns.    -----
+0001e570: 2d2d 0a20 2020 2070 7976 6973 7461 2e55  --.    pyvista.U
+0001e580: 6e73 7472 7563 7475 7265 6447 7269 6420  nstructuredGrid 
+0001e590: 7c20 7374 720a 2020 2020 2020 2020 4461  | str.        Da
+0001e5a0: 7461 5365 7420 6f72 2066 696c 656e 616d  taSet or filenam
+0001e5b0: 6520 6465 7065 6e64 696e 6720 6f6e 2060  e depending on `
+0001e5c0: 606c 6f61 6460 602e 0a0a 2020 2020 4578  `load``...    Ex
+0001e5d0: 616d 706c 6573 0a20 2020 202d 2d2d 2d2d  amples.    -----
+0001e5e0: 2d2d 2d0a 2020 2020 3e3e 3e20 6672 6f6d  ---.    >>> from
+0001e5f0: 2070 7976 6973 7461 2069 6d70 6f72 7420   pyvista import 
+0001e600: 6578 616d 706c 6573 0a20 2020 203e 3e3e  examples.    >>>
+0001e610: 2064 6174 6173 6574 203d 2065 7861 6d70   dataset = examp
+0001e620: 6c65 732e 646f 776e 6c6f 6164 5f61 6e67  les.download_ang
+0001e630: 756c 6172 5f73 6563 746f 7228 290a 2020  ular_sector().  
+0001e640: 2020 3e3e 3e20 6461 7461 7365 742e 706c    >>> dataset.pl
+0001e650: 6f74 2873 6361 6c61 7273 3d27 506f 696e  ot(scalars='Poin
+0001e660: 7449 6427 290a 0a20 2020 2022 2222 0a20  tId')..    """. 
+0001e670: 2020 2072 6574 7572 6e20 5f64 6f77 6e6c     return _downl
+0001e680: 6f61 645f 616e 645f 7265 6164 2827 416e  oad_and_read('An
+0001e690: 6775 6c61 7253 6563 746f 722e 7674 6b27  gularSector.vtk'
+0001e6a0: 2c20 6c6f 6164 3d6c 6f61 6429 0a0a 0a64  , load=load)...d
+0001e6b0: 6566 2064 6f77 6e6c 6f61 645f 6d6f 756e  ef download_moun
+0001e6c0: 745f 6461 6d61 7661 6e64 286c 6f61 643d  t_damavand(load=
+0001e6d0: 5472 7565 293a 2020 2320 7072 6167 6d61  True):  # pragma
+0001e6e0: 3a20 6e6f 2063 6f76 6572 0a20 2020 2022  : no cover.    "
+0001e6f0: 2222 446f 776e 6c6f 6164 2074 6865 204d  ""Download the M
+0001e700: 6f75 6e74 2044 616d 6176 616e 6420 6461  ount Damavand da
+0001e710: 7461 7365 742e 0a0a 2020 2020 5669 7375  taset...    Visu
+0001e720: 616c 697a 6520 3344 206d 6f64 656c 7320  alize 3D models 
+0001e730: 6f66 2044 616d 6176 616e 6420 566f 6c63  of Damavand Volc
+0001e740: 616e 6f2c 2041 6c62 6f72 7a2c 2049 7261  ano, Alborz, Ira
+0001e750: 6e2e 2054 6869 7320 6973 2061 2032 4420  n. This is a 2D 
+0001e760: 6d61 700a 2020 2020 7769 7468 2074 6865  map.    with the
+0001e770: 2061 6c74 6974 7564 6520 656d 6265 6464   altitude embedd
+0001e780: 6564 2061 7320 6060 277a 2760 6020 6365  ed as ``'z'`` ce
+0001e790: 6c6c 2064 6174 6120 7769 7468 696e 2074  ll data within t
+0001e7a0: 6865 0a20 2020 203a 636c 6173 733a 6070  he.    :class:`p
+0001e7b0: 7976 6973 7461 2e50 6f6c 7944 6174 6160  yvista.PolyData`
+0001e7c0: 2e0a 0a20 2020 204f 7269 6769 6e61 6c6c  ...    Originall
+0001e7d0: 7920 706f 7374 6564 2061 7420 6062 616e  y posted at `ban
+0001e7e0: 6573 756c 6c69 7661 6e2f 6461 6d61 7661  esullivan/damava
+0001e7f0: 6e64 2d76 6f6c 6361 6e6f 0a20 2020 203c  nd-volcano.    <
+0001e800: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
+0001e810: 6f6d 2f62 616e 6573 756c 6c69 7661 6e2f  om/banesullivan/
+0001e820: 6461 6d61 7661 6e64 2d76 6f6c 6361 6e6f  damavand-volcano
+0001e830: 3e60 5f2e 0a0a 2020 2020 5061 7261 6d65  >`_...    Parame
+0001e840: 7465 7273 0a20 2020 202d 2d2d 2d2d 2d2d  ters.    -------
+0001e850: 2d2d 2d0a 2020 2020 6c6f 6164 203a 2062  ---.    load : b
+0001e860: 6f6f 6c2c 2064 6566 6175 6c74 3a20 5472  ool, default: Tr
+0001e870: 7565 0a20 2020 2020 2020 204c 6f61 6420  ue.        Load 
+0001e880: 7468 6520 6461 7461 7365 7420 6166 7465  the dataset afte
+0001e890: 7220 646f 776e 6c6f 6164 696e 6720 6974  r downloading it
+0001e8a0: 2077 6865 6e20 6060 5472 7565 6060 2e20   when ``True``. 
+0001e8b0: 2053 6574 2074 6869 730a 2020 2020 2020   Set this.      
+0001e8c0: 2020 746f 2060 6046 616c 7365 6060 2061    to ``False`` a
+0001e8d0: 6e64 206f 6e6c 7920 7468 6520 6669 6c65  nd only the file
+0001e8e0: 6e61 6d65 2077 696c 6c20 6265 2072 6574  name will be ret
+0001e8f0: 7572 6e65 642e 0a0a 2020 2020 5265 7475  urned...    Retu
+0001e900: 726e 730a 2020 2020 2d2d 2d2d 2d2d 2d0a  rns.    -------.
+0001e910: 2020 2020 7079 7669 7374 612e 506f 6c79      pyvista.Poly
+0001e920: 4461 7461 207c 2073 7472 0a20 2020 2020  Data | str.     
+0001e930: 2020 2044 6174 6153 6574 206f 7220 6669     DataSet or fi
+0001e940: 6c65 6e61 6d65 2064 6570 656e 6469 6e67  lename depending
+0001e950: 206f 6e20 6060 6c6f 6164 6060 2e0a 0a20   on ``load``... 
+0001e960: 2020 2045 7861 6d70 6c65 730a 2020 2020     Examples.    
+0001e970: 2d2d 2d2d 2d2d 2d2d 0a20 2020 2044 6f77  --------.    Dow
+0001e980: 6e6c 6f61 6420 7468 6520 4461 6d61 7661  nload the Damava
+0001e990: 6e64 2064 6174 6173 6574 2061 6e64 2070  nd dataset and p
+0001e9a0: 6c6f 7420 6974 2061 6674 6572 2077 6172  lot it after war
+0001e9b0: 7069 6e67 2069 7420 6279 2069 7473 2061  ping it by its a
+0001e9c0: 6c74 6974 7564 652e 0a0a 2020 2020 3e3e  ltitude...    >>
+0001e9d0: 3e20 6672 6f6d 2070 7976 6973 7461 2069  > from pyvista i
+0001e9e0: 6d70 6f72 7420 6578 616d 706c 6573 0a20  mport examples. 
+0001e9f0: 2020 203e 3e3e 2064 6174 6173 6574 203d     >>> dataset =
+0001ea00: 2065 7861 6d70 6c65 732e 646f 776e 6c6f   examples.downlo
+0001ea10: 6164 5f6d 6f75 6e74 5f64 616d 6176 616e  ad_mount_damavan
+0001ea20: 6428 290a 2020 2020 3e3e 3e20 6461 7461  d().    >>> data
+0001ea30: 7365 7420 3d20 6461 7461 7365 742e 6365  set = dataset.ce
+0001ea40: 6c6c 5f64 6174 615f 746f 5f70 6f69 6e74  ll_data_to_point
+0001ea50: 5f64 6174 6128 290a 2020 2020 3e3e 3e20  _data().    >>> 
+0001ea60: 6461 7461 7365 7420 3d20 6461 7461 7365  dataset = datase
+0001ea70: 742e 7761 7270 5f62 795f 7363 616c 6172  t.warp_by_scalar
+0001ea80: 2827 7a27 2c20 6661 6374 6f72 3d32 290a  ('z', factor=2).
+0001ea90: 2020 2020 3e3e 3e20 6461 7461 7365 742e      >>> dataset.
+0001eaa0: 706c 6f74 2863 6d61 703d 2767 6973 745f  plot(cmap='gist_
+0001eab0: 6561 7274 6827 2c20 7368 6f77 5f73 6361  earth', show_sca
+0001eac0: 6c61 725f 6261 723d 4661 6c73 6529 0a0a  lar_bar=False)..
+0001ead0: 2020 2020 2222 220a 2020 2020 7265 7475      """.    retu
+0001eae0: 726e 205f 646f 776e 6c6f 6164 5f61 6e64  rn _download_and
+0001eaf0: 5f72 6561 6428 2741 4f49 2e44 616d 6176  _read('AOI.Damav
+0001eb00: 616e 642e 3332 3633 392e 7674 7027 2c20  and.32639.vtp', 
+0001eb10: 6c6f 6164 3d6c 6f61 6429 0a0a 0a64 6566  load=load)...def
+0001eb20: 2064 6f77 6e6c 6f61 645f 7061 7274 6963   download_partic
+0001eb30: 6c65 735f 6c65 7468 6528 6c6f 6164 3d54  les_lethe(load=T
+0001eb40: 7275 6529 3a20 2023 2070 7261 676d 613a  rue):  # pragma:
+0001eb50: 206e 6f20 636f 7665 720a 2020 2020 2222   no cover.    ""
+0001eb60: 2244 6f77 6e6c 6f61 6420 6120 7061 7274  "Download a part
+0001eb70: 6963 6c65 7320 6461 7461 7365 7420 6765  icles dataset ge
+0001eb80: 6e65 7261 7465 6420 6279 2060 6c65 7468  nerated by `leth
+0001eb90: 6520 3c68 7474 7073 3a2f 2f67 6974 6875  e <https://githu
+0001eba0: 622e 636f 6d2f 6c65 7468 652d 6366 642f  b.com/lethe-cfd/
+0001ebb0: 6c65 7468 653e 605f 202e 0a0a 2020 2020  lethe>`_ ...    
+0001ebc0: 5365 6520 6050 7956 6973 7461 2064 6973  See `PyVista dis
+0001ebd0: 6375 7373 696f 6e73 2023 3139 3834 0a20  cussions #1984. 
+0001ebe0: 2020 203c 6874 7470 733a 2f2f 6769 7468     <https://gith
+0001ebf0: 7562 2e63 6f6d 2f70 7976 6973 7461 2f70  ub.com/pyvista/p
+0001ec00: 7976 6973 7461 2f64 6973 6375 7373 696f  yvista/discussio
+0001ec10: 6e73 2f31 3938 343e 605f 0a0a 2020 2020  ns/1984>`_..    
+0001ec20: 5061 7261 6d65 7465 7273 0a20 2020 202d  Parameters.    -
+0001ec30: 2d2d 2d2d 2d2d 2d2d 2d0a 2020 2020 6c6f  ---------.    lo
+0001ec40: 6164 203a 2062 6f6f 6c2c 2064 6566 6175  ad : bool, defau
+0001ec50: 6c74 3a20 5472 7565 0a20 2020 2020 2020  lt: True.       
+0001ec60: 204c 6f61 6420 7468 6520 6461 7461 7365   Load the datase
+0001ec70: 7420 6166 7465 7220 646f 776e 6c6f 6164  t after download
+0001ec80: 696e 6720 6974 2077 6865 6e20 6060 5472  ing it when ``Tr
+0001ec90: 7565 6060 2e20 2053 6574 2074 6869 730a  ue``.  Set this.
+0001eca0: 2020 2020 2020 2020 746f 2060 6046 616c          to ``Fal
+0001ecb0: 7365 6060 2061 6e64 206f 6e6c 7920 7468  se`` and only th
+0001ecc0: 6520 6669 6c65 6e61 6d65 2077 696c 6c20  e filename will 
+0001ecd0: 6265 2072 6574 7572 6e65 642e 0a0a 2020  be returned...  
+0001ece0: 2020 5265 7475 726e 730a 2020 2020 2d2d    Returns.    --
+0001ecf0: 2d2d 2d2d 2d0a 2020 2020 7079 7669 7374  -----.    pyvist
+0001ed00: 612e 556e 7374 7275 6374 7572 6564 4772  a.UnstructuredGr
+0001ed10: 6964 207c 2073 7472 0a20 2020 2020 2020  id | str.       
+0001ed20: 2044 6174 6153 6574 206f 7220 6669 6c65   DataSet or file
+0001ed30: 6e61 6d65 2064 6570 656e 6469 6e67 206f  name depending o
+0001ed40: 6e20 6060 6c6f 6164 6060 2e0a 0a20 2020  n ``load``...   
+0001ed50: 2045 7861 6d70 6c65 730a 2020 2020 2d2d   Examples.    --
+0001ed60: 2d2d 2d2d 2d2d 0a20 2020 2044 6f77 6e6c  ------.    Downl
+0001ed70: 6f61 6420 7468 6520 7061 7274 6963 6c65  oad the particle
+0001ed80: 7320 6461 7461 7365 7420 616e 6420 706c  s dataset and pl
+0001ed90: 6f74 2069 7420 6166 7465 7220 6765 6e65  ot it after gene
+0001eda0: 7261 7469 6e67 2067 6c79 7068 732e 0a0a  rating glyphs...
+0001edb0: 2020 2020 3e3e 3e20 6672 6f6d 2070 7976      >>> from pyv
+0001edc0: 6973 7461 2069 6d70 6f72 7420 6578 616d  ista import exam
+0001edd0: 706c 6573 0a20 2020 203e 3e3e 2070 6172  ples.    >>> par
+0001ede0: 7469 636c 6573 203d 2065 7861 6d70 6c65  ticles = example
+0001edf0: 732e 646f 776e 6c6f 6164 5f70 6172 7469  s.download_parti
+0001ee00: 636c 6573 5f6c 6574 6865 2829 0a20 2020  cles_lethe().   
+0001ee10: 203e 3e3e 2070 6172 7469 636c 6573 2e70   >>> particles.p
+0001ee20: 6c6f 7428 0a20 2020 202e 2e2e 2020 2020  lot(.    ...    
+0001ee30: 2072 656e 6465 725f 706f 696e 7473 5f61   render_points_a
+0001ee40: 735f 7370 6865 7265 733d 5472 7565 2c0a  s_spheres=True,.
+0001ee50: 2020 2020 2e2e 2e20 2020 2020 7374 796c      ...     styl
+0001ee60: 653d 2770 6f69 6e74 7327 2c0a 2020 2020  e='points',.    
+0001ee70: 2e2e 2e20 2020 2020 7363 616c 6172 733d  ...     scalars=
+0001ee80: 2756 656c 6f63 6974 7927 2c0a 2020 2020  'Velocity',.    
+0001ee90: 2e2e 2e20 2020 2020 6261 636b 6772 6f75  ...     backgrou
+0001eea0: 6e64 3d27 7727 2c0a 2020 2020 2e2e 2e20  nd='w',.    ... 
+0001eeb0: 2020 2020 7363 616c 6172 5f62 6172 5f61      scalar_bar_a
+0001eec0: 7267 733d 7b27 636f 6c6f 7227 3a20 276b  rgs={'color': 'k
+0001eed0: 277d 2c0a 2020 2020 2e2e 2e20 2020 2020  '},.    ...     
+0001eee0: 636d 6170 3d27 6277 7227 2c0a 2020 2020  cmap='bwr',.    
+0001eef0: 2e2e 2e20 290a 0a20 2020 2022 2222 0a20  ... )..    """. 
+0001ef00: 2020 2072 6574 7572 6e20 5f64 6f77 6e6c     return _downl
+0001ef10: 6f61 645f 616e 645f 7265 6164 2827 6c65  oad_and_read('le
+0001ef20: 7468 652f 7265 7375 6c74 5f70 6172 7469  the/result_parti
+0001ef30: 636c 6573 2e32 3030 3030 2e30 3030 302e  cles.20000.0000.
+0001ef40: 7674 7527 2c20 6c6f 6164 3d6c 6f61 6429  vtu', load=load)
+0001ef50: 0a0a 0a64 6566 2064 6f77 6e6c 6f61 645f  ...def download_
+0001ef60: 6769 665f 7369 6d70 6c65 286c 6f61 643d  gif_simple(load=
+0001ef70: 5472 7565 293a 2020 2320 7072 6167 6d61  True):  # pragma
+0001ef80: 3a20 6e6f 2063 6f76 6572 0a20 2020 2022  : no cover.    "
+0001ef90: 2222 446f 776e 6c6f 6164 2061 2073 696d  ""Download a sim
+0001efa0: 706c 6520 7468 7265 6520 6672 616d 6520  ple three frame 
+0001efb0: 4749 462e 0a0a 2020 2020 5061 7261 6d65  GIF...    Parame
+0001efc0: 7465 7273 0a20 2020 202d 2d2d 2d2d 2d2d  ters.    -------
+0001efd0: 2d2d 2d0a 2020 2020 6c6f 6164 203a 2062  ---.    load : b
+0001efe0: 6f6f 6c2c 2064 6566 6175 6c74 3a20 5472  ool, default: Tr
+0001eff0: 7565 0a20 2020 2020 2020 204c 6f61 6420  ue.        Load 
+0001f000: 7468 6520 6461 7461 7365 7420 6166 7465  the dataset afte
+0001f010: 7220 646f 776e 6c6f 6164 696e 6720 6974  r downloading it
+0001f020: 2077 6865 6e20 6060 5472 7565 6060 2e20   when ``True``. 
+0001f030: 2053 6574 2074 6869 730a 2020 2020 2020   Set this.      
+0001f040: 2020 746f 2060 6046 616c 7365 6060 2061    to ``False`` a
+0001f050: 6e64 206f 6e6c 7920 7468 6520 6669 6c65  nd only the file
+0001f060: 6e61 6d65 2077 696c 6c20 6265 2072 6574  name will be ret
+0001f070: 7572 6e65 642e 0a0a 2020 2020 5265 7475  urned...    Retu
+0001f080: 726e 730a 2020 2020 2d2d 2d2d 2d2d 2d0a  rns.    -------.
+0001f090: 2020 2020 7079 7669 7374 612e 496d 6167      pyvista.Imag
+0001f0a0: 6544 6174 6120 7c20 7374 720a 2020 2020  eData | str.    
+0001f0b0: 2020 2020 4461 7461 5365 7420 6f72 2066      DataSet or f
+0001f0c0: 696c 656e 616d 6520 6465 7065 6e64 696e  ilename dependin
+0001f0d0: 6720 6f6e 2060 606c 6f61 6460 602e 0a0a  g on ``load``...
+0001f0e0: 2020 2020 4578 616d 706c 6573 0a20 2020      Examples.   
+0001f0f0: 202d 2d2d 2d2d 2d2d 2d0a 2020 2020 446f   --------.    Do
+0001f100: 776e 6c6f 6164 2061 6e64 2070 6c6f 7420  wnload and plot 
+0001f110: 7468 6520 6669 7273 7420 6672 616d 6520  the first frame 
+0001f120: 6f66 2061 2073 696d 706c 6520 4749 462e  of a simple GIF.
+0001f130: 0a0a 2020 2020 3e3e 3e20 6672 6f6d 2070  ..    >>> from p
+0001f140: 7976 6973 7461 2069 6d70 6f72 7420 6578  yvista import ex
+0001f150: 616d 706c 6573 0a20 2020 203e 3e3e 2067  amples.    >>> g
+0001f160: 7269 6420 3d20 6578 616d 706c 6573 2e64  rid = examples.d
+0001f170: 6f77 6e6c 6f61 645f 6769 665f 7369 6d70  ownload_gif_simp
+0001f180: 6c65 2829 0a20 2020 203e 3e3e 2067 7269  le().    >>> gri
+0001f190: 642e 706c 6f74 280a 2020 2020 2e2e 2e20  d.plot(.    ... 
+0001f1a0: 2020 2020 7363 616c 6172 733d 2766 7261      scalars='fra
+0001f1b0: 6d65 3027 2c0a 2020 2020 2e2e 2e20 2020  me0',.    ...   
+0001f1c0: 2020 7267 623d 5472 7565 2c0a 2020 2020    rgb=True,.    
+0001f1d0: 2e2e 2e20 2020 2020 6261 636b 6772 6f75  ...     backgrou
+0001f1e0: 6e64 3d27 7727 2c0a 2020 2020 2e2e 2e20  nd='w',.    ... 
+0001f1f0: 2020 2020 7368 6f77 5f73 6361 6c61 725f      show_scalar_
+0001f200: 6261 723d 4661 6c73 652c 0a20 2020 202e  bar=False,.    .
+0001f210: 2e2e 2020 2020 2063 706f 733d 2778 7927  ..     cpos='xy'
+0001f220: 2c0a 2020 2020 2e2e 2e20 290a 0a20 2020  ,.    ... )..   
+0001f230: 2050 6c6f 7420 7468 6520 7365 636f 6e64   Plot the second
+0001f240: 2066 7261 6d65 2e0a 0a20 2020 203e 3e3e   frame...    >>>
+0001f250: 2067 7269 642e 706c 6f74 280a 2020 2020   grid.plot(.    
+0001f260: 2e2e 2e20 2020 2020 7363 616c 6172 733d  ...     scalars=
+0001f270: 2766 7261 6d65 3127 2c0a 2020 2020 2e2e  'frame1',.    ..
+0001f280: 2e20 2020 2020 7267 623d 5472 7565 2c0a  .     rgb=True,.
+0001f290: 2020 2020 2e2e 2e20 2020 2020 6261 636b      ...     back
+0001f2a0: 6772 6f75 6e64 3d27 7727 2c0a 2020 2020  ground='w',.    
+0001f2b0: 2e2e 2e20 2020 2020 7368 6f77 5f73 6361  ...     show_sca
+0001f2c0: 6c61 725f 6261 723d 4661 6c73 652c 0a20  lar_bar=False,. 
+0001f2d0: 2020 202e 2e2e 2020 2020 2063 706f 733d     ...     cpos=
+0001f2e0: 2778 7927 2c0a 2020 2020 2e2e 2e20 290a  'xy',.    ... ).
+0001f2f0: 0a20 2020 2022 2222 0a20 2020 2072 6574  .    """.    ret
+0001f300: 7572 6e20 5f64 6f77 6e6c 6f61 645f 616e  urn _download_an
+0001f310: 645f 7265 6164 2827 6769 6673 2f73 616d  d_read('gifs/sam
+0001f320: 706c 652e 6769 6627 2c20 6c6f 6164 3d6c  ple.gif', load=l
+0001f330: 6f61 6429 0a0a 0a64 6566 2064 6f77 6e6c  oad)...def downl
+0001f340: 6f61 645f 636c 6f75 645f 6461 726b 5f6d  oad_cloud_dark_m
+0001f350: 6174 7465 7228 6c6f 6164 3d54 7275 6529  atter(load=True)
+0001f360: 3a20 2023 2070 7261 676d 613a 206e 6f20  :  # pragma: no 
+0001f370: 636f 7665 720a 2020 2020 2222 2244 6f77  cover.    """Dow
+0001f380: 6e6c 6f61 6420 7061 7274 6963 6c65 7320  nload particles 
+0001f390: 6672 6f6d 2061 2073 696d 756c 6174 6564  from a simulated
+0001f3a0: 2064 6172 6b20 6d61 7474 6572 2068 616c   dark matter hal
+0001f3b0: 6f2e 0a0a 2020 2020 5468 6973 2064 6174  o...    This dat
+0001f3c0: 6173 6574 2063 6f6e 7461 696e 7320 3332  aset contains 32
+0001f3d0: 2c33 3134 2070 6172 7469 636c 6573 2e0a  ,314 particles..
+0001f3e0: 0a20 2020 2050 6172 616d 6574 6572 730a  .    Parameters.
+0001f3f0: 2020 2020 2d2d 2d2d 2d2d 2d2d 2d2d 0a20      ----------. 
+0001f400: 2020 206c 6f61 6420 3a20 626f 6f6c 2c20     load : bool, 
+0001f410: 6465 6661 756c 743a 2054 7275 650a 2020  default: True.  
+0001f420: 2020 2020 2020 4c6f 6164 2074 6865 2064        Load the d
+0001f430: 6174 6173 6574 2061 6674 6572 2064 6f77  ataset after dow
+0001f440: 6e6c 6f61 6469 6e67 2069 7420 7768 656e  nloading it when
+0001f450: 2060 6054 7275 6560 602e 2020 5365 7420   ``True``.  Set 
+0001f460: 7468 6973 0a20 2020 2020 2020 2074 6f20  this.        to 
+0001f470: 6060 4661 6c73 6560 6020 616e 6420 6f6e  ``False`` and on
+0001f480: 6c79 2074 6865 2066 696c 656e 616d 6520  ly the filename 
+0001f490: 7769 6c6c 2062 6520 7265 7475 726e 6564  will be returned
+0001f4a0: 2e0a 0a20 2020 2052 6574 7572 6e73 0a20  ...    Returns. 
+0001f4b0: 2020 202d 2d2d 2d2d 2d2d 0a20 2020 2070     -------.    p
+0001f4c0: 7976 6973 7461 2e50 6f69 6e74 5365 7420  yvista.PointSet 
+0001f4d0: 7c20 7374 720a 2020 2020 2020 2020 4461  | str.        Da
+0001f4e0: 7461 5365 7420 6f72 2066 696c 656e 616d  taSet or filenam
+0001f4f0: 6520 6465 7065 6e64 696e 6720 6f6e 2060  e depending on `
+0001f500: 606c 6f61 6460 602e 0a0a 2020 2020 4578  `load``...    Ex
+0001f510: 616d 706c 6573 0a20 2020 202d 2d2d 2d2d  amples.    -----
+0001f520: 2d2d 2d0a 2020 2020 446f 776e 6c6f 6164  ---.    Download
+0001f530: 2074 6865 2064 6172 6b20 6d61 7474 6572   the dark matter
+0001f540: 2063 6c6f 7564 2061 6e64 2064 6973 706c   cloud and displ
+0001f550: 6179 2069 7473 2072 6570 7265 7365 6e74  ay its represent
+0001f560: 6174 696f 6e2e 0a0a 2020 2020 3e3e 3e20  ation...    >>> 
+0001f570: 696d 706f 7274 206e 756d 7079 2061 7320  import numpy as 
+0001f580: 6e70 0a20 2020 203e 3e3e 2066 726f 6d20  np.    >>> from 
+0001f590: 7079 7669 7374 6120 696d 706f 7274 2065  pyvista import e
+0001f5a0: 7861 6d70 6c65 730a 2020 2020 3e3e 3e20  xamples.    >>> 
+0001f5b0: 7063 203d 2065 7861 6d70 6c65 732e 646f  pc = examples.do
+0001f5c0: 776e 6c6f 6164 5f63 6c6f 7564 5f64 6172  wnload_cloud_dar
+0001f5d0: 6b5f 6d61 7474 6572 2829 0a20 2020 203e  k_matter().    >
+0001f5e0: 3e3e 2070 630a 2020 2020 506f 696e 7453  >> pc.    PointS
+0001f5f0: 6574 2028 2e2e 2e29 0a20 2020 2020 204e  et (...).      N
+0001f600: 2043 656c 6c73 3a20 2020 2030 0a20 2020   Cells:    0.   
+0001f610: 2020 204e 2050 6f69 6e74 733a 2020 2033     N Points:   3
+0001f620: 3233 3134 0a20 2020 2020 2058 2042 6f75  2314.      X Bou
+0001f630: 6e64 733a 2020 2037 2e34 3531 652b 3031  nds:   7.451e+01
+0001f640: 2c20 372e 3839 3265 2b30 310a 2020 2020  , 7.892e+01.    
+0001f650: 2020 5920 426f 756e 6473 3a20 2020 312e    Y Bounds:   1.
+0001f660: 3631 3665 2b30 312c 2032 2e32 3735 652b  616e+01, 2.275e+
+0001f670: 3031 0a20 2020 2020 205a 2042 6f75 6e64  01.      Z Bound
+0001f680: 733a 2020 2038 2e39 3030 652b 3031 2c20  s:   8.900e+01, 
+0001f690: 392e 3331 3965 2b30 310a 2020 2020 2020  9.319e+01.      
+0001f6a0: 4e20 4172 7261 7973 3a20 2020 300a 0a20  N Arrays:   0.. 
+0001f6b0: 2020 2050 6c6f 7420 7468 6520 706f 696e     Plot the poin
+0001f6c0: 7420 636c 6f75 642e 2043 6f6c 6f72 2062  t cloud. Color b
+0001f6d0: 6173 6564 206f 6e20 7468 6520 6469 7374  ased on the dist
+0001f6e0: 616e 6365 2066 726f 6d20 7468 6520 6365  ance from the ce
+0001f6f0: 6e74 6572 206f 6620 7468 650a 2020 2020  nter of the.    
+0001f700: 636c 6f75 642e 0a0a 2020 2020 3e3e 3e20  cloud...    >>> 
+0001f710: 7063 2e70 6c6f 7428 0a20 2020 202e 2e2e  pc.plot(.    ...
+0001f720: 2020 2020 2073 6361 6c61 7273 3d6e 702e       scalars=np.
+0001f730: 6c69 6e61 6c67 2e6e 6f72 6d28 7063 2e70  linalg.norm(pc.p
+0001f740: 6f69 6e74 7320 2d20 7063 2e63 656e 7465  oints - pc.cente
+0001f750: 722c 2061 7869 733d 3129 2c0a 2020 2020  r, axis=1),.    
+0001f760: 2e2e 2e20 2020 2020 7374 796c 653d 2770  ...     style='p
+0001f770: 6f69 6e74 735f 6761 7573 7369 616e 272c  oints_gaussian',
+0001f780: 0a20 2020 202e 2e2e 2020 2020 206f 7061  .    ...     opa
+0001f790: 6369 7479 3d30 2e35 2c0a 2020 2020 2e2e  city=0.5,.    ..
+0001f7a0: 2e20 2020 2020 706f 696e 745f 7369 7a65  .     point_size
+0001f7b0: 3d31 2e35 2c0a 2020 2020 2e2e 2e20 2020  =1.5,.    ...   
+0001f7c0: 2020 7368 6f77 5f73 6361 6c61 725f 6261    show_scalar_ba
+0001f7d0: 723d 4661 6c73 652c 0a20 2020 202e 2e2e  r=False,.    ...
+0001f7e0: 2020 2020 207a 6f6f 6d3d 322c 0a20 2020       zoom=2,.   
+0001f7f0: 202e 2e2e 2029 0a0a 2020 2020 5365 6520   ... )..    See 
+0001f800: 7468 6520 3a72 6566 3a60 706c 6f74 7469  the :ref:`plotti
+0001f810: 6e67 5f70 6f69 6e74 5f63 6c6f 7564 7360  ng_point_clouds`
+0001f820: 2066 6f72 2061 2066 756c 6c20 6578 616d   for a full exam
+0001f830: 706c 6520 7573 696e 6720 7468 6973 2064  ple using this d
+0001f840: 6174 6173 6574 2e0a 0a20 2020 2022 2222  ataset...    """
+0001f850: 0a20 2020 2066 696c 656e 616d 6520 3d20  .    filename = 
+0001f860: 646f 776e 6c6f 6164 5f66 696c 6528 2770  download_file('p
+0001f870: 6f69 6e74 2d63 6c6f 7564 732f 6669 6e64  oint-clouds/find
+0001f880: 7573 3233 2f68 616c 6f5f 6c6f 775f 7265  us23/halo_low_re
+0001f890: 732e 6e70 7927 290a 0a20 2020 2069 6620  s.npy')..    if 
+0001f8a0: 6c6f 6164 3a0a 2020 2020 2020 2020 7265  load:.        re
+0001f8b0: 7475 726e 2070 7976 6973 7461 2e50 6f69  turn pyvista.Poi
+0001f8c0: 6e74 5365 7428 6e70 2e6c 6f61 6428 6669  ntSet(np.load(fi
+0001f8d0: 6c65 6e61 6d65 2929 0a20 2020 2072 6574  lename)).    ret
+0001f8e0: 7572 6e20 6669 6c65 6e61 6d65 0a0a 0a64  urn filename...d
+0001f8f0: 6566 2064 6f77 6e6c 6f61 645f 636c 6f75  ef download_clou
+0001f900: 645f 6461 726b 5f6d 6174 7465 725f 6465  d_dark_matter_de
+0001f910: 6e73 6528 6c6f 6164 3d54 7275 6529 3a20  nse(load=True): 
+0001f920: 2023 2070 7261 676d 613a 206e 6f20 636f   # pragma: no co
+0001f930: 7665 720a 2020 2020 2222 2244 6f77 6e6c  ver.    """Downl
+0001f940: 6f61 6420 6120 7061 7274 6963 6c65 7320  oad a particles 
+0001f950: 6672 6f6d 2061 2073 696d 756c 6174 6564  from a simulated
+0001f960: 2064 6172 6b20 6d61 7474 6572 2068 616c   dark matter hal
+0001f970: 6f2e 0a0a 2020 2020 5468 6973 2064 6174  o...    This dat
+0001f980: 6173 6574 2063 6f6e 7461 696e 7320 322c  aset contains 2,
+0001f990: 3036 322c 3235 3620 7061 7274 6963 6c65  062,256 particle
+0001f9a0: 732e 0a0a 2020 2020 5061 7261 6d65 7465  s...    Paramete
+0001f9b0: 7273 0a20 2020 202d 2d2d 2d2d 2d2d 2d2d  rs.    ---------
+0001f9c0: 2d0a 2020 2020 6c6f 6164 203a 2062 6f6f  -.    load : boo
+0001f9d0: 6c2c 2064 6566 6175 6c74 3a20 5472 7565  l, default: True
+0001f9e0: 0a20 2020 2020 2020 204c 6f61 6420 7468  .        Load th
+0001f9f0: 6520 6461 7461 7365 7420 6166 7465 7220  e dataset after 
+0001fa00: 646f 776e 6c6f 6164 696e 6720 6974 2077  downloading it w
+0001fa10: 6865 6e20 6060 5472 7565 6060 2e20 2053  hen ``True``.  S
+0001fa20: 6574 2074 6869 730a 2020 2020 2020 2020  et this.        
+0001fa30: 746f 2060 6046 616c 7365 6060 2061 6e64  to ``False`` and
+0001fa40: 206f 6e6c 7920 7468 6520 6669 6c65 6e61   only the filena
+0001fa50: 6d65 2077 696c 6c20 6265 2072 6574 7572  me will be retur
+0001fa60: 6e65 642e 0a0a 2020 2020 5265 7475 726e  ned...    Return
+0001fa70: 730a 2020 2020 2d2d 2d2d 2d2d 2d0a 2020  s.    -------.  
+0001fa80: 2020 7079 7669 7374 612e 506f 696e 7453    pyvista.PointS
+0001fa90: 6574 207c 2073 7472 0a20 2020 2020 2020  et | str.       
+0001faa0: 2044 6174 6153 6574 206f 7220 6669 6c65   DataSet or file
+0001fab0: 6e61 6d65 2064 6570 656e 6469 6e67 206f  name depending o
+0001fac0: 6e20 6060 6c6f 6164 6060 2e0a 0a20 2020  n ``load``...   
+0001fad0: 2045 7861 6d70 6c65 730a 2020 2020 2d2d   Examples.    --
+0001fae0: 2d2d 2d2d 2d2d 0a20 2020 2044 6f77 6e6c  ------.    Downl
+0001faf0: 6f61 6420 7468 6520 6461 726b 206d 6174  oad the dark mat
+0001fb00: 7465 7220 636c 6f75 6420 616e 6420 6469  ter cloud and di
+0001fb10: 7370 6c61 7920 6974 7320 7265 7072 6573  splay its repres
+0001fb20: 656e 7461 7469 6f6e 2e0a 0a20 2020 203e  entation...    >
+0001fb30: 3e3e 2069 6d70 6f72 7420 6e75 6d70 7920  >> import numpy 
+0001fb40: 6173 206e 700a 2020 2020 3e3e 3e20 6672  as np.    >>> fr
+0001fb50: 6f6d 2070 7976 6973 7461 2069 6d70 6f72  om pyvista impor
+0001fb60: 7420 6578 616d 706c 6573 0a20 2020 203e  t examples.    >
+0001fb70: 3e3e 2070 6320 3d20 6578 616d 706c 6573  >> pc = examples
+0001fb80: 2e64 6f77 6e6c 6f61 645f 636c 6f75 645f  .download_cloud_
+0001fb90: 6461 726b 5f6d 6174 7465 725f 6465 6e73  dark_matter_dens
+0001fba0: 6528 290a 2020 2020 3e3e 3e20 7063 0a20  e().    >>> pc. 
+0001fbb0: 2020 2050 6f69 6e74 5365 7420 282e 2e2e     PointSet (...
+0001fbc0: 290a 2020 2020 2020 4e20 4365 6c6c 733a  ).      N Cells:
+0001fbd0: 2020 2020 300a 2020 2020 2020 4e20 506f      0.      N Po
+0001fbe0: 696e 7473 3a20 2020 3230 3632 3235 360a  ints:   2062256.
+0001fbf0: 2020 2020 2020 5820 426f 756e 6473 3a20        X Bounds: 
+0001fc00: 2020 372e 3436 3265 2b30 312c 2037 2e38    7.462e+01, 7.8
+0001fc10: 3633 652b 3031 0a20 2020 2020 2059 2042  63e+01.      Y B
+0001fc20: 6f75 6e64 733a 2020 2031 2e36 3034 652b  ounds:   1.604e+
+0001fc30: 3031 2c20 322e 3234 3465 2b30 310a 2020  01, 2.244e+01.  
+0001fc40: 2020 2020 5a20 426f 756e 6473 3a20 2020      Z Bounds:   
+0001fc50: 382e 3839 3365 2b30 312c 2039 2e33 3337  8.893e+01, 9.337
+0001fc60: 652b 3031 0a20 2020 2020 204e 2041 7272  e+01.      N Arr
+0001fc70: 6179 733a 2020 2030 0a0a 2020 2020 506c  ays:   0..    Pl
+0001fc80: 6f74 2074 6865 2070 6f69 6e74 2063 6c6f  ot the point clo
+0001fc90: 7564 2e20 436f 6c6f 7220 6261 7365 6420  ud. Color based 
+0001fca0: 6f6e 2074 6865 2064 6973 7461 6e63 6520  on the distance 
+0001fcb0: 6672 6f6d 2074 6865 2063 656e 7465 7220  from the center 
+0001fcc0: 6f66 2074 6865 0a20 2020 2063 6c6f 7564  of the.    cloud
+0001fcd0: 2e0a 0a20 2020 203e 3e3e 2070 632e 706c  ...    >>> pc.pl
+0001fce0: 6f74 280a 2020 2020 2e2e 2e20 2020 2020  ot(.    ...     
+0001fcf0: 7363 616c 6172 733d 6e70 2e6c 696e 616c  scalars=np.linal
+0001fd00: 672e 6e6f 726d 2870 632e 706f 696e 7473  g.norm(pc.points
+0001fd10: 202d 2070 632e 6365 6e74 6572 2c20 6178   - pc.center, ax
+0001fd20: 6973 3d31 292c 0a20 2020 202e 2e2e 2020  is=1),.    ...  
+0001fd30: 2020 2073 7479 6c65 3d27 706f 696e 7473     style='points
+0001fd40: 5f67 6175 7373 6961 6e27 2c0a 2020 2020  _gaussian',.    
+0001fd50: 2e2e 2e20 2020 2020 6f70 6163 6974 793d  ...     opacity=
+0001fd60: 302e 3033 302c 0a20 2020 202e 2e2e 2020  0.030,.    ...  
+0001fd70: 2020 2070 6f69 6e74 5f73 697a 653d 322e     point_size=2.
+0001fd80: 302c 0a20 2020 202e 2e2e 2020 2020 2073  0,.    ...     s
+0001fd90: 686f 775f 7363 616c 6172 5f62 6172 3d46  how_scalar_bar=F
+0001fda0: 616c 7365 2c0a 2020 2020 2e2e 2e20 2020  alse,.    ...   
+0001fdb0: 2020 7a6f 6f6d 3d32 2c0a 2020 2020 2e2e    zoom=2,.    ..
+0001fdc0: 2e20 290a 0a20 2020 2053 6565 2074 6865  . )..    See the
+0001fdd0: 203a 7265 663a 6070 6c6f 7474 696e 675f   :ref:`plotting_
+0001fde0: 706f 696e 745f 636c 6f75 6473 6020 666f  point_clouds` fo
+0001fdf0: 7220 6d6f 7265 2064 6574 6169 6c73 206f  r more details o
+0001fe00: 6e20 686f 7720 746f 2070 6c6f 7420 706f  n how to plot po
+0001fe10: 696e 740a 2020 2020 636c 6f75 6473 2e0a  int.    clouds..
+0001fe20: 0a20 2020 2022 2222 0a20 2020 2066 696c  .    """.    fil
+0001fe30: 656e 616d 6520 3d20 646f 776e 6c6f 6164  ename = download
+0001fe40: 5f66 696c 6528 2770 6f69 6e74 2d63 6c6f  _file('point-clo
+0001fe50: 7564 732f 6669 6e64 7573 3233 2f68 616c  uds/findus23/hal
+0001fe60: 6f5f 6869 6768 5f72 6573 2e6e 7079 2729  o_high_res.npy')
+0001fe70: 0a0a 2020 2020 6966 206c 6f61 643a 0a20  ..    if load:. 
+0001fe80: 2020 2020 2020 2072 6574 7572 6e20 7079         return py
+0001fe90: 7669 7374 612e 506f 696e 7453 6574 286e  vista.PointSet(n
+0001fea0: 702e 6c6f 6164 2866 696c 656e 616d 6529  p.load(filename)
+0001feb0: 290a 2020 2020 7265 7475 726e 2066 696c  ).    return fil
+0001fec0: 656e 616d 650a 0a0a 6465 6620 646f 776e  ename...def down
+0001fed0: 6c6f 6164 5f73 7461 7273 5f63 6c6f 7564  load_stars_cloud
+0001fee0: 5f68 7967 286c 6f61 643d 5472 7565 293a  _hyg(load=True):
+0001fef0: 2020 2320 7072 6167 6d61 3a20 6e6f 2063    # pragma: no c
+0001ff00: 6f76 6572 0a20 2020 2022 2222 446f 776e  over.    """Down
+0001ff10: 6c6f 6164 2061 2070 6f69 6e74 2063 6c6f  load a point clo
+0001ff20: 7564 206f 6620 7374 6172 7320 6173 2063  ud of stars as c
+0001ff30: 6f6d 7075 7465 6420 6279 2074 6865 2048  omputed by the H
+0001ff40: 5947 2044 6174 6162 6173 652e 0a0a 2020  YG Database...  
+0001ff50: 2020 5365 6520 6048 5947 2d44 6174 6162    See `HYG-Datab
+0001ff60: 6173 6520 3c68 7474 7073 3a2f 2f67 6974  ase <https://git
+0001ff70: 6875 622e 636f 6d2f 6173 7472 6f6e 6578  hub.com/astronex
+0001ff80: 7573 2f48 5947 2d44 6174 6162 6173 653e  us/HYG-Database>
+0001ff90: 605f 2066 6f72 206d 6f72 650a 2020 2020  `_ for more.    
+0001ffa0: 6465 7461 696c 732e 0a0a 2020 2020 5468  details...    Th
+0001ffb0: 6973 2064 6174 6120 7365 7420 6973 206c  is data set is l
+0001ffc0: 6963 656e 7365 6420 6279 2061 2043 7265  icensed by a Cre
+0001ffd0: 6174 6976 6520 436f 6d6d 6f6e 7320 4174  ative Commons At
+0001ffe0: 7472 6962 7574 696f 6e2d 5368 6172 6541  tribution-ShareA
+0001fff0: 6c69 6b65 0a20 2020 206c 6963 656e 7365  like.    license
+00020000: 2e20 466f 7220 6d6f 7265 2064 6574 6169  . For more detai
+00020010: 6c73 2c20 7265 6164 2074 6865 2060 4372  ls, read the `Cr
+00020020: 6561 7469 7665 2043 6f6d 6d6f 6e73 2070  eative Commons p
+00020030: 6167 650a 2020 2020 3c68 7474 7073 3a2f  age.    <https:/
+00020040: 2f63 7265 6174 6976 6563 6f6d 6d6f 6e73  /creativecommons
+00020050: 2e6f 7267 2f6c 6963 656e 7365 732f 6279  .org/licenses/by
+00020060: 2d73 612f 322e 352f 3e60 5f0a 0a20 2020  -sa/2.5/>`_..   
+00020070: 2053 6565 2074 6865 2060 5245 4144 4d45   See the `README
+00020080: 2e6d 640a 2020 2020 3c68 7474 7073 3a2f  .md.    <https:/
+00020090: 2f67 6974 6875 622e 636f 6d2f 7079 7669  /github.com/pyvi
+000200a0: 7374 612f 7674 6b2d 6461 7461 2f62 6c6f  sta/vtk-data/blo
+000200b0: 622f 6d61 7374 6572 2f44 6174 612f 706f  b/master/Data/po
+000200c0: 696e 742d 636c 6f75 6473 2f68 7967 2d64  int-clouds/hyg-d
+000200d0: 6174 6162 6173 652f 5245 4144 4d45 2e6d  atabase/README.m
+000200e0: 643e 605f 0a20 2020 2066 6f72 206d 6f72  d>`_.    for mor
+000200f0: 6520 6465 7461 696c 7320 666f 7220 686f  e details for ho
+00020100: 7720 7468 6520 7374 6172 2063 6f6c 6f72  w the star color
+00020110: 7320 7765 7265 2063 6f6d 7075 7465 642e  s were computed.
+00020120: 0a0a 2020 2020 4469 7374 616e 6365 7320  ..    Distances 
+00020130: 6172 6520 696e 2070 6172 7365 6373 2066  are in parsecs f
+00020140: 726f 6d20 4561 7274 682e 0a0a 2020 2020  rom Earth...    
+00020150: 5061 7261 6d65 7465 7273 0a20 2020 202d  Parameters.    -
+00020160: 2d2d 2d2d 2d2d 2d2d 2d0a 2020 2020 6c6f  ---------.    lo
+00020170: 6164 203a 2062 6f6f 6c2c 2064 6566 6175  ad : bool, defau
+00020180: 6c74 3a20 5472 7565 0a20 2020 2020 2020  lt: True.       
+00020190: 204c 6f61 6420 7468 6520 6461 7461 7365   Load the datase
+000201a0: 7420 6166 7465 7220 646f 776e 6c6f 6164  t after download
+000201b0: 696e 6720 6974 2077 6865 6e20 6060 5472  ing it when ``Tr
+000201c0: 7565 6060 2e20 2053 6574 2074 6869 730a  ue``.  Set this.
+000201d0: 2020 2020 2020 2020 746f 2060 6046 616c          to ``Fal
+000201e0: 7365 6060 2061 6e64 206f 6e6c 7920 7468  se`` and only th
+000201f0: 6520 6669 6c65 6e61 6d65 2077 696c 6c20  e filename will 
+00020200: 6265 2072 6574 7572 6e65 642e 0a0a 2020  be returned...  
+00020210: 2020 5265 7475 726e 730a 2020 2020 2d2d    Returns.    --
+00020220: 2d2d 2d2d 2d0a 2020 2020 7079 7669 7374  -----.    pyvist
+00020230: 612e 506f 6c79 4461 7461 207c 2073 7472  a.PolyData | str
+00020240: 0a20 2020 2020 2020 2044 6174 6153 6574  .        DataSet
+00020250: 206f 7220 6669 6c65 6e61 6d65 2064 6570   or filename dep
+00020260: 656e 6469 6e67 206f 6e20 6060 6c6f 6164  ending on ``load
+00020270: 6060 2e0a 0a20 2020 2045 7861 6d70 6c65  ``...    Example
+00020280: 730a 2020 2020 2d2d 2d2d 2d2d 2d2d 0a20  s.    --------. 
+00020290: 2020 2044 6f77 6e6c 6f61 6420 616e 6420     Download and 
+000202a0: 706c 6f74 2061 2070 6f69 6e74 2063 6c6f  plot a point clo
+000202b0: 7564 206f 6620 7374 6172 7320 7769 7468  ud of stars with
+000202c0: 696e 2033 2c30 3030 206c 6967 6874 2079  in 3,000 light y
+000202d0: 6561 7273 2e20 5374 6172 730a 2020 2020  ears. Stars.    
+000202e0: 6172 6520 636f 6c6f 7265 6420 6163 636f  are colored acco
+000202f0: 7264 696e 6720 746f 2074 6865 6972 2052  rding to their R
+00020300: 4742 4120 636f 6c6f 7273 2e0a 0a20 2020  GBA colors...   
+00020310: 203e 3e3e 2069 6d70 6f72 7420 6e75 6d70   >>> import nump
+00020320: 7920 6173 206e 700a 2020 2020 3e3e 3e20  y as np.    >>> 
+00020330: 6672 6f6d 2070 7976 6973 7461 2069 6d70  from pyvista imp
+00020340: 6f72 7420 6578 616d 706c 6573 0a20 2020  ort examples.   
+00020350: 203e 3e3e 2073 7461 7273 203d 2065 7861   >>> stars = exa
+00020360: 6d70 6c65 732e 646f 776e 6c6f 6164 5f73  mples.download_s
+00020370: 7461 7273 5f63 6c6f 7564 5f68 7967 2829  tars_cloud_hyg()
+00020380: 0a20 2020 203e 3e3e 2073 7461 7273 2e70  .    >>> stars.p
+00020390: 6c6f 7428 0a20 2020 202e 2e2e 2020 2020  lot(.    ...    
+000203a0: 2073 7479 6c65 3d27 706f 696e 7473 5f67   style='points_g
+000203b0: 6175 7373 6961 6e27 2c0a 2020 2020 2e2e  aussian',.    ..
+000203c0: 2e20 2020 2020 6261 636b 6772 6f75 6e64  .     background
+000203d0: 3d27 6b27 2c0a 2020 2020 2e2e 2e20 2020  ='k',.    ...   
+000203e0: 2020 706f 696e 745f 7369 7a65 3d30 2e35    point_size=0.5
+000203f0: 2c0a 2020 2020 2e2e 2e20 2020 2020 7363  ,.    ...     sc
+00020400: 616c 6172 733d 275f 7267 6261 272c 0a20  alars='_rgba',. 
+00020410: 2020 202e 2e2e 2020 2020 2072 656e 6465     ...     rende
+00020420: 725f 706f 696e 7473 5f61 735f 7370 6865  r_points_as_sphe
+00020430: 7265 733d 4661 6c73 652c 0a20 2020 202e  res=False,.    .
+00020440: 2e2e 2020 2020 207a 6f6f 6d3d 332e 302c  ..     zoom=3.0,
+00020450: 0a20 2020 202e 2e2e 2029 0a0a 2020 2020  .    ... )..    
+00020460: 3e3e 3e20 7374 6172 730a 2020 2020 506f  >>> stars.    Po
+00020470: 6c79 4461 7461 2028 2e2e 2e29 0a20 2020  lyData (...).   
+00020480: 2020 204e 2043 656c 6c73 3a20 2020 2031     N Cells:    1
+00020490: 3037 3835 370a 2020 2020 2020 4e20 506f  07857.      N Po
+000204a0: 696e 7473 3a20 2020 3130 3738 3537 0a20  ints:   107857. 
+000204b0: 2020 2020 204e 2053 7472 6970 733a 2020       N Strips:  
+000204c0: 2030 0a20 2020 2020 2058 2042 6f75 6e64   0.      X Bound
+000204d0: 733a 2020 202d 392e 3735 3565 2b30 322c  s:   -9.755e+02,
+000204e0: 2039 2e37 3734 652b 3032 0a20 2020 2020   9.774e+02.     
+000204f0: 2059 2042 6f75 6e64 733a 2020 202d 392e   Y Bounds:   -9.
+00020500: 3632 3065 2b30 322c 2039 2e36 3632 652b  620e+02, 9.662e+
+00020510: 3032 0a20 2020 2020 205a 2042 6f75 6e64  02.      Z Bound
+00020520: 733a 2020 202d 392e 3738 3865 2b30 322c  s:   -9.788e+02,
+00020530: 2039 2e37 3032 652b 3032 0a20 2020 2020   9.702e+02.     
+00020540: 204e 2041 7272 6179 733a 2020 2033 0a0a   N Arrays:   3..
+00020550: 2020 2020 5365 6520 7468 6520 3a72 6566      See the :ref
+00020560: 3a60 706c 6f74 7469 6e67 5f70 6f69 6e74  :`plotting_point
+00020570: 5f63 6c6f 7564 7360 2066 6f72 206d 6f72  _clouds` for mor
+00020580: 6520 6465 7461 696c 7320 6f6e 2068 6f77  e details on how
+00020590: 2074 6f20 706c 6f74 2070 6f69 6e74 0a20   to plot point. 
+000205a0: 2020 2063 6c6f 7564 732e 0a0a 2020 2020     clouds...    
+000205b0: 2222 220a 2020 2020 7265 7475 726e 205f  """.    return _
+000205c0: 646f 776e 6c6f 6164 5f61 6e64 5f72 6561  download_and_rea
+000205d0: 6428 2770 6f69 6e74 2d63 6c6f 7564 732f  d('point-clouds/
+000205e0: 6879 672d 6461 7461 6261 7365 2f73 7461  hyg-database/sta
+000205f0: 7273 2e76 7470 272c 206c 6f61 643d 6c6f  rs.vtp', load=lo
+00020600: 6164 290a 0a0a 6465 6620 646f 776e 6c6f  ad)...def downlo
+00020610: 6164 5f66 6561 5f62 7261 636b 6574 286c  ad_fea_bracket(l
+00020620: 6f61 643d 5472 7565 293a 2020 2320 7072  oad=True):  # pr
+00020630: 6167 6d61 3a20 6e6f 2063 6f76 6572 0a20  agma: no cover. 
+00020640: 2020 2022 2222 446f 776e 6c6f 6164 2074     """Download t
+00020650: 6865 2066 696e 6974 6520 656c 656d 656e  he finite elemen
+00020660: 7420 736f 6c75 7469 6f6e 206f 6620 6120  t solution of a 
+00020670: 6272 6163 6b65 742e 0a0a 2020 2020 436f  bracket...    Co
+00020680: 6e74 6169 6e73 2076 6f6e 2d6d 6973 6573  ntains von-mises
+00020690: 2065 7175 6976 616c 656e 7420 6365 6c6c   equivalent cell
+000206a0: 2073 7472 6573 7320 6173 7375 6d69 6e67   stress assuming
+000206b0: 2061 2076 6572 7469 6361 6c20 2879 2d61   a vertical (y-a
+000206c0: 7869 7329 206c 6f61 642e 0a0a 2020 2020  xis) load...    
+000206d0: 5061 7261 6d65 7465 7273 0a20 2020 202d  Parameters.    -
+000206e0: 2d2d 2d2d 2d2d 2d2d 2d0a 2020 2020 6c6f  ---------.    lo
+000206f0: 6164 203a 2062 6f6f 6c2c 2064 6566 6175  ad : bool, defau
+00020700: 6c74 3a20 5472 7565 0a20 2020 2020 2020  lt: True.       
+00020710: 204c 6f61 6420 7468 6520 6461 7461 7365   Load the datase
+00020720: 7420 6166 7465 7220 646f 776e 6c6f 6164  t after download
+00020730: 696e 6720 6974 2077 6865 6e20 6060 5472  ing it when ``Tr
+00020740: 7565 6060 2e20 2053 6574 2074 6869 730a  ue``.  Set this.
+00020750: 2020 2020 2020 2020 746f 2060 6046 616c          to ``Fal
+00020760: 7365 6060 2061 6e64 206f 6e6c 7920 7468  se`` and only th
+00020770: 6520 6669 6c65 6e61 6d65 2077 696c 6c20  e filename will 
+00020780: 6265 2072 6574 7572 6e65 642e 0a0a 2020  be returned...  
+00020790: 2020 5265 7475 726e 730a 2020 2020 2d2d    Returns.    --
+000207a0: 2d2d 2d2d 2d0a 2020 2020 7079 7669 7374  -----.    pyvist
+000207b0: 612e 556e 7374 7275 6374 7572 6564 4772  a.UnstructuredGr
+000207c0: 6964 207c 2073 7472 0a20 2020 2020 2020  id | str.       
+000207d0: 2044 6174 6153 6574 206f 7220 6669 6c65   DataSet or file
+000207e0: 6e61 6d65 2064 6570 656e 6469 6e67 206f  name depending o
+000207f0: 6e20 6060 6c6f 6164 6060 2e0a 0a20 2020  n ``load``...   
+00020800: 2045 7861 6d70 6c65 730a 2020 2020 2d2d   Examples.    --
+00020810: 2d2d 2d2d 2d2d 0a20 2020 2044 6f77 6e6c  ------.    Downl
+00020820: 6f61 6420 616e 6420 706c 6f74 2065 7175  oad and plot equ
+00020830: 6976 616c 656e 7420 6365 6c6c 2073 7472  ivalent cell str
+00020840: 6573 732e 0a0a 2020 2020 3e3e 3e20 6672  ess...    >>> fr
+00020850: 6f6d 2070 7976 6973 7461 2069 6d70 6f72  om pyvista impor
+00020860: 7420 6578 616d 706c 6573 0a20 2020 203e  t examples.    >
+00020870: 3e3e 2067 7269 6420 3d20 6578 616d 706c  >> grid = exampl
+00020880: 6573 2e64 6f77 6e6c 6f61 645f 6665 615f  es.download_fea_
+00020890: 6272 6163 6b65 7428 290a 2020 2020 3e3e  bracket().    >>
+000208a0: 3e20 6772 6964 2e70 6c6f 7428 290a 0a20  > grid.plot().. 
+000208b0: 2020 2050 6c6f 7420 7468 6520 706f 696e     Plot the poin
+000208c0: 7420 7374 7265 7373 2075 7369 6e67 2074  t stress using t
+000208d0: 6865 2060 6027 6a65 7427 6060 2063 6f6c  he ``'jet'`` col
+000208e0: 6f72 206d 6170 2e20 436f 6e76 6572 7420  or map. Convert 
+000208f0: 7468 6520 6365 6c6c 2064 6174 610a 2020  the cell data.  
+00020900: 2020 746f 2070 6f69 6e74 2064 6174 612e    to point data.
+00020910: 0a0a 2020 2020 3e3e 3e20 6672 6f6d 2070  ..    >>> from p
+00020920: 7976 6973 7461 2069 6d70 6f72 7420 6578  yvista import ex
+00020930: 616d 706c 6573 0a20 2020 203e 3e3e 2067  amples.    >>> g
+00020940: 7269 6420 3d20 6578 616d 706c 6573 2e64  rid = examples.d
+00020950: 6f77 6e6c 6f61 645f 6665 615f 6272 6163  ownload_fea_brac
+00020960: 6b65 7428 290a 2020 2020 3e3e 3e20 6772  ket().    >>> gr
+00020970: 6964 203d 2067 7269 642e 6365 6c6c 5f64  id = grid.cell_d
+00020980: 6174 615f 746f 5f70 6f69 6e74 5f64 6174  ata_to_point_dat
+00020990: 6128 290a 2020 2020 3e3e 3e20 6772 6964  a().    >>> grid
+000209a0: 2e70 6c6f 7428 736d 6f6f 7468 5f73 6861  .plot(smooth_sha
+000209b0: 6469 6e67 3d54 7275 652c 2073 706c 6974  ding=True, split
+000209c0: 5f73 6861 7270 5f65 6467 6573 3d54 7275  _sharp_edges=Tru
+000209d0: 652c 2063 6d61 703d 276a 6574 2729 0a0a  e, cmap='jet')..
+000209e0: 2020 2020 2222 220a 2020 2020 7265 7475      """.    retu
+000209f0: 726e 205f 646f 776e 6c6f 6164 5f61 6e64  rn _download_and
+00020a00: 5f72 6561 6428 2766 6561 2f6b 6965 6665  _read('fea/kiefe
+00020a10: 722f 6461 7461 7365 742e 7674 7527 2c20  r/dataset.vtu', 
+00020a20: 6c6f 6164 3d6c 6f61 6429 0a0a 0a64 6566  load=load)...def
+00020a30: 2064 6f77 6e6c 6f61 645f 6665 615f 6865   download_fea_he
+00020a40: 7274 7a69 616e 5f63 6f6e 7461 6374 5f63  rtzian_contact_c
+00020a50: 796c 696e 6465 7228 6c6f 6164 3d54 7275  ylinder(load=Tru
+00020a60: 6529 3a20 2023 2070 7261 676d 613a 206e  e):  # pragma: n
+00020a70: 6f20 636f 7665 720a 2020 2020 2222 2244  o cover.    """D
+00020a80: 6f77 6e6c 6f61 6420 6120 6865 7274 7a69  ownload a hertzi
+00020a90: 616e 2063 6f6e 7461 6374 2066 696e 6974  an contact finit
+00020aa0: 6520 656c 656d 656e 7420 736f 6c75 7469  e element soluti
+00020ab0: 6f6e 2e0a 0a20 2020 2048 6572 747a 6961  on...    Hertzia
+00020ac0: 6e20 636f 6e74 6163 7420 6973 2072 6566  n contact is ref
+00020ad0: 6572 7265 6420 746f 2074 6865 2066 7269  erred to the fri
+00020ae0: 6374 696f 6e6c 6573 7320 636f 6e74 6163  ctionless contac
+00020af0: 7420 6265 7477 6565 6e20 7477 6f0a 2020  t between two.  
+00020b00: 2020 626f 6469 6573 2e20 5370 6865 7269    bodies. Spheri
+00020b10: 6361 6c20 636f 6e74 6163 7420 6973 2061  cal contact is a
+00020b20: 2073 7065 6369 616c 2063 6173 6520 6f66   special case of
+00020b30: 2074 6865 2048 6572 747a 2063 6f6e 7461   the Hertz conta
+00020b40: 6374 2c20 7768 6963 6820 6973 0a20 2020  ct, which is.   
+00020b50: 2062 6574 7765 656e 2074 776f 2073 7068   between two sph
+00020b60: 6572 6573 2c20 6f72 2061 7320 696e 2074  eres, or as in t
+00020b70: 6865 2063 6173 6520 6f66 2074 6869 7320  he case of this 
+00020b80: 6461 7461 7365 742c 2062 6574 7765 656e  dataset, between
+00020b90: 2061 2073 7068 6572 650a 2020 2020 616e   a sphere.    an
+00020ba0: 6420 7468 6520 7375 7266 6163 6520 6f66  d the surface of
+00020bb0: 2061 2068 616c 6620 7370 6163 6520 2866   a half space (f
+00020bc0: 6c61 7420 706c 616e 6529 2e0a 0a20 2020  lat plane)...   
+00020bd0: 2050 6172 616d 6574 6572 730a 2020 2020   Parameters.    
+00020be0: 2d2d 2d2d 2d2d 2d2d 2d2d 0a20 2020 206c  ----------.    l
+00020bf0: 6f61 6420 3a20 626f 6f6c 2c20 6465 6661  oad : bool, defa
+00020c00: 756c 743a 2054 7275 650a 2020 2020 2020  ult: True.      
+00020c10: 2020 4c6f 6164 2074 6865 2064 6174 6173    Load the datas
+00020c20: 6574 2061 6674 6572 2064 6f77 6e6c 6f61  et after downloa
+00020c30: 6469 6e67 2069 7420 7768 656e 2060 6054  ding it when ``T
+00020c40: 7275 6560 602e 2020 5365 7420 7468 6973  rue``.  Set this
+00020c50: 0a20 2020 2020 2020 2074 6f20 6060 4661  .        to ``Fa
+00020c60: 6c73 6560 6020 616e 6420 6f6e 6c79 2074  lse`` and only t
+00020c70: 6865 2066 696c 656e 616d 6520 7769 6c6c  he filename will
+00020c80: 2062 6520 7265 7475 726e 6564 2e0a 0a20   be returned... 
+00020c90: 2020 2052 6574 7572 6e73 0a20 2020 202d     Returns.    -
+00020ca0: 2d2d 2d2d 2d2d 0a20 2020 2070 7976 6973  ------.    pyvis
+00020cb0: 7461 2e55 6e73 7472 7563 7475 7265 6447  ta.UnstructuredG
+00020cc0: 7269 6420 7c20 7374 720a 2020 2020 2020  rid | str.      
+00020cd0: 2020 4461 7461 5365 7420 6f72 2066 696c    DataSet or fil
+00020ce0: 656e 616d 6520 6465 7065 6e64 696e 6720  ename depending 
+00020cf0: 6f6e 2060 606c 6f61 6460 602e 0a0a 2020  on ``load``...  
+00020d00: 2020 4578 616d 706c 6573 0a20 2020 202d    Examples.    -
+00020d10: 2d2d 2d2d 2d2d 2d0a 2020 2020 506c 6f74  -------.    Plot
+00020d20: 2062 7920 7061 7274 2049 442e 0a0a 2020   by part ID...  
+00020d30: 2020 3e3e 3e20 696d 706f 7274 206e 756d    >>> import num
+00020d40: 7079 2061 7320 6e70 0a20 2020 203e 3e3e  py as np.    >>>
+00020d50: 2069 6d70 6f72 7420 7079 7669 7374 6120   import pyvista 
+00020d60: 6173 2070 760a 2020 2020 3e3e 3e20 6672  as pv.    >>> fr
+00020d70: 6f6d 2070 7976 6973 7461 2069 6d70 6f72  om pyvista impor
+00020d80: 7420 6578 616d 706c 6573 0a20 2020 203e  t examples.    >
+00020d90: 3e3e 2067 7269 6420 3d20 6578 616d 706c  >> grid = exampl
+00020da0: 6573 2e64 6f77 6e6c 6f61 645f 6665 615f  es.download_fea_
+00020db0: 6865 7274 7a69 616e 5f63 6f6e 7461 6374  hertzian_contact
+00020dc0: 5f63 796c 696e 6465 7228 290a 2020 2020  _cylinder().    
+00020dd0: 3e3e 3e20 6772 6964 2e70 6c6f 7428 0a20  >>> grid.plot(. 
+00020de0: 2020 202e 2e2e 2020 2020 2073 6361 6c61     ...     scala
+00020df0: 7273 3d27 5061 7274 4944 272c 2063 6d61  rs='PartID', cma
+00020e00: 703d 5b27 6772 6565 6e27 2c20 2762 6c75  p=['green', 'blu
+00020e10: 6527 5d2c 2073 686f 775f 7363 616c 6172  e'], show_scalar
+00020e20: 5f62 6172 3d46 616c 7365 0a20 2020 202e  _bar=False.    .
+00020e30: 2e2e 2029 0a0a 2020 2020 506c 6f74 2074  .. )..    Plot t
+00020e40: 6865 2061 6273 6f6c 7574 6520 7661 6c75  he absolute valu
+00020e50: 6520 6f66 2074 6865 2063 6f6d 706f 6e65  e of the compone
+00020e60: 6e74 2073 7472 6573 7320 696e 2074 6865  nt stress in the
+00020e70: 205a 2064 6972 6563 7469 6f6e 2e0a 0a20   Z direction... 
+00020e80: 2020 203e 3e3e 2070 6c20 3d20 7076 2e50     >>> pl = pv.P
+00020e90: 6c6f 7474 6572 2829 0a20 2020 203e 3e3e  lotter().    >>>
+00020ea0: 207a 5f73 7472 6573 7320 3d20 6e70 2e61   z_stress = np.a
+00020eb0: 6273 2867 7269 645b 2753 7472 6573 7327  bs(grid['Stress'
+00020ec0: 5d5b 3a2c 2032 5d29 0a20 2020 203e 3e3e  ][:, 2]).    >>>
+00020ed0: 205f 203d 2070 6c2e 6164 645f 6d65 7368   _ = pl.add_mesh
+00020ee0: 280a 2020 2020 2e2e 2e20 2020 2020 6772  (.    ...     gr
+00020ef0: 6964 2c0a 2020 2020 2e2e 2e20 2020 2020  id,.    ...     
+00020f00: 7363 616c 6172 733d 7a5f 7374 7265 7373  scalars=z_stress
+00020f10: 2c0a 2020 2020 2e2e 2e20 2020 2020 636c  ,.    ...     cl
+00020f20: 696d 3d5b 302c 2031 2e32 6539 5d2c 0a20  im=[0, 1.2e9],. 
+00020f30: 2020 202e 2e2e 2020 2020 2063 6d61 703d     ...     cmap=
+00020f40: 276a 6574 272c 0a20 2020 202e 2e2e 2020  'jet',.    ...  
+00020f50: 2020 206c 6967 6874 696e 673d 5472 7565     lighting=True
+00020f60: 2c0a 2020 2020 2e2e 2e20 2020 2020 7368  ,.    ...     sh
+00020f70: 6f77 5f65 6467 6573 3d46 616c 7365 2c0a  ow_edges=False,.
+00020f80: 2020 2020 2e2e 2e20 2020 2020 616d 6269      ...     ambi
+00020f90: 656e 743d 302e 322c 0a20 2020 202e 2e2e  ent=0.2,.    ...
+00020fa0: 2029 0a20 2020 203e 3e3e 2070 6c2e 6361   ).    >>> pl.ca
+00020fb0: 6d65 7261 5f70 6f73 6974 696f 6e20 3d20  mera_position = 
+00020fc0: 2778 7a27 0a20 2020 203e 3e3e 2070 6c2e  'xz'.    >>> pl.
+00020fd0: 6361 6d65 7261 2e7a 6f6f 6d28 312e 3429  camera.zoom(1.4)
+00020fe0: 0a20 2020 203e 3e3e 2070 6c2e 7368 6f77  .    >>> pl.show
+00020ff0: 2829 0a0a 2020 2020 2222 220a 2020 2020  ()..    """.    
+00021000: 6669 6c65 6e61 6d65 203d 205f 646f 776e  filename = _down
+00021010: 6c6f 6164 5f61 7263 6869 7665 280a 2020  load_archive(.  
+00021020: 2020 2020 2020 2766 6561 2f68 6572 747a        'fea/hertz
+00021030: 6961 6e5f 636f 6e74 6163 745f 6379 6c69  ian_contact_cyli
+00021040: 6e64 6572 2f48 6572 747a 6961 6e5f 6379  nder/Hertzian_cy
+00021050: 6c69 6e64 6572 5f6f 6e5f 706c 6174 652e  linder_on_plate.
+00021060: 7a69 7027 2c0a 2020 2020 2020 2020 7461  zip',.        ta
+00021070: 7267 6574 5f66 696c 653d 2762 6661 6339  rget_file='bfac9
+00021080: 6664 312d 6539 3832 2d34 3832 352d 3961  fd1-e982-4825-9a
+00021090: 3935 2d39 6535 6438 6335 6234 6433 655f  95-9e5d8c5b4d3e_
+000210a0: 7265 7375 6c74 5f31 2e70 7674 7527 2c0a  result_1.pvtu',.
+000210b0: 2020 2020 290a 2020 2020 6966 206c 6f61      ).    if loa
+000210c0: 643a 0a20 2020 2020 2020 2072 6574 7572  d:.        retur
+000210d0: 6e20 7079 7669 7374 612e 7265 6164 2866  n pyvista.read(f
+000210e0: 696c 656e 616d 6529 0a20 2020 2072 6574  ilename).    ret
+000210f0: 7572 6e20 6669 6c65 6e61 6d65 0a0a 0a64  urn filename...d
+00021100: 6566 2064 6f77 6e6c 6f61 645f 626c 6163  ef download_blac
+00021110: 6b5f 7661 7365 286c 6f61 643d 5472 7565  k_vase(load=True
+00021120: 293a 2020 2320 7072 6167 6d61 3a20 6e6f  ):  # pragma: no
+00021130: 2063 6f76 6572 0a20 2020 2022 2222 446f   cover.    """Do
+00021140: 776e 6c6f 6164 2061 2062 6c61 636b 2076  wnload a black v
+00021150: 6173 6520 7363 616e 2063 7265 6174 6564  ase scan created
+00021160: 2062 7920 4976 616e 204e 696b 6f6c 6f76   by Ivan Nikolov
+00021170: 2e0a 0a20 2020 2054 6865 2064 6174 6173  ...    The datas
+00021180: 6574 2077 6173 2064 6f77 6e6c 6f61 6465  et was downloade
+00021190: 6420 6672 6f6d 2060 4747 472d 4265 6e63  d from `GGG-Benc
+000211a0: 686d 6172 6b53 664d 3a20 4461 7461 7365  hmarkSfM: Datase
+000211b0: 7420 666f 7220 4265 6e63 686d 6172 6b69  t for Benchmarki
+000211c0: 6e67 0a20 2020 2043 6c6f 7365 2d72 616e  ng.    Close-ran
+000211d0: 6765 2053 664d 2053 6f66 7477 6172 6520  ge SfM Software 
+000211e0: 5065 7266 6f72 6d61 6e63 6520 756e 6465  Performance unde
+000211f0: 7220 5661 7279 696e 6720 4361 7074 7572  r Varying Captur
+00021200: 696e 6720 436f 6e64 6974 696f 6e73 0a20  ing Conditions. 
+00021210: 2020 203c 6874 7470 733a 2f2f 6461 7461     <https://data
+00021220: 2e6d 656e 6465 6c65 792e 636f 6d2f 6461  .mendeley.com/da
+00021230: 7461 7365 7473 2f62 7a78 6b32 6e37 3873  tasets/bzxk2n78s
+00021240: 392f 343e 605f 0a0a 2020 2020 4f72 6967  9/4>`_..    Orig
+00021250: 696e 616c 2064 6174 6173 6574 7320 6172  inal datasets ar
+00021260: 6520 756e 6465 7220 7468 6520 4343 2042  e under the CC B
+00021270: 5920 342e 3020 6c69 6365 6e73 652e 0a0a  Y 4.0 license...
+00021280: 2020 2020 466f 7220 6d6f 7265 2064 6574      For more det
+00021290: 6169 6c73 2c20 7365 6520 6049 7661 6e20  ails, see `Ivan 
+000212a0: 4e69 6b6f 6c6f 7620 4461 7461 7365 7473  Nikolov Datasets
+000212b0: 0a20 2020 203c 6874 7470 733a 2f2f 6769  .    <https://gi
+000212c0: 7468 7562 2e63 6f6d 2f70 7976 6973 7461  thub.com/pyvista
+000212d0: 2f76 746b 2d64 6174 612f 7472 6565 2f6d  /vtk-data/tree/m
+000212e0: 6173 7465 722f 4461 7461 2f69 7661 6e2d  aster/Data/ivan-
+000212f0: 6e69 6b6f 6c6f 763e 605f 0a0a 2020 2020  nikolov>`_..    
+00021300: 5061 7261 6d65 7465 7273 0a20 2020 202d  Parameters.    -
+00021310: 2d2d 2d2d 2d2d 2d2d 2d0a 2020 2020 6c6f  ---------.    lo
+00021320: 6164 203a 2062 6f6f 6c2c 2064 6566 6175  ad : bool, defau
+00021330: 6c74 3a20 5472 7565 0a20 2020 2020 2020  lt: True.       
+00021340: 204c 6f61 6420 7468 6520 6461 7461 7365   Load the datase
+00021350: 7420 6166 7465 7220 646f 776e 6c6f 6164  t after download
+00021360: 696e 6720 6974 2077 6865 6e20 6060 5472  ing it when ``Tr
+00021370: 7565 6060 2e20 2053 6574 2074 6869 730a  ue``.  Set this.
+00021380: 2020 2020 2020 2020 746f 2060 6046 616c          to ``Fal
+00021390: 7365 6060 2061 6e64 206f 6e6c 7920 7468  se`` and only th
+000213a0: 6520 6669 6c65 6e61 6d65 2077 696c 6c20  e filename will 
+000213b0: 6265 2072 6574 7572 6e65 642e 0a0a 2020  be returned...  
+000213c0: 2020 5265 7475 726e 730a 2020 2020 2d2d    Returns.    --
+000213d0: 2d2d 2d2d 2d0a 2020 2020 7079 7669 7374  -----.    pyvist
+000213e0: 612e 506f 6c79 4461 7461 207c 2073 7472  a.PolyData | str
+000213f0: 0a20 2020 2020 2020 2044 6174 6153 6574  .        DataSet
+00021400: 206f 7220 6669 6c65 6e61 6d65 2064 6570   or filename dep
+00021410: 656e 6469 6e67 206f 6e20 6060 6c6f 6164  ending on ``load
+00021420: 6060 2e0a 0a20 2020 2045 7861 6d70 6c65  ``...    Example
+00021430: 730a 2020 2020 2d2d 2d2d 2d2d 2d2d 0a20  s.    --------. 
+00021440: 2020 2044 6f77 6e6c 6f61 6420 616e 6420     Download and 
+00021450: 706c 6f74 2074 6865 2064 6174 6173 6574  plot the dataset
+00021460: 2e0a 0a20 2020 203e 3e3e 2066 726f 6d20  ...    >>> from 
+00021470: 7079 7669 7374 6120 696d 706f 7274 2065  pyvista import e
+00021480: 7861 6d70 6c65 730a 2020 2020 3e3e 3e20  xamples.    >>> 
+00021490: 6d65 7368 203d 2065 7861 6d70 6c65 732e  mesh = examples.
+000214a0: 646f 776e 6c6f 6164 5f62 6c61 636b 5f76  download_black_v
+000214b0: 6173 6528 290a 2020 2020 3e3e 3e20 6d65  ase().    >>> me
+000214c0: 7368 2e70 6c6f 7428 290a 0a20 2020 2052  sh.plot()..    R
+000214d0: 6574 7572 6e20 7468 6520 7374 6174 6973  eturn the statis
+000214e0: 7469 6373 206f 6620 7468 6520 6461 7461  tics of the data
+000214f0: 7365 742e 0a0a 2020 2020 3e3e 3e20 6d65  set...    >>> me
+00021500: 7368 0a20 2020 2050 6f6c 7944 6174 6120  sh.    PolyData 
+00021510: 282e 2e2e 290a 2020 2020 2020 4e20 4365  (...).      N Ce
+00021520: 6c6c 733a 2020 2020 3331 3336 3635 320a  lls:    3136652.
+00021530: 2020 2020 2020 4e20 506f 696e 7473 3a20        N Points: 
+00021540: 2020 3136 3131 3738 390a 2020 2020 2020    1611789.      
+00021550: 4e20 5374 7269 7073 3a20 2020 300a 2020  N Strips:   0.  
+00021560: 2020 2020 5820 426f 756e 6473 3a20 2020      X Bounds:   
+00021570: 2d31 2e30 3932 652b 3032 2c20 312e 3533  -1.092e+02, 1.53
+00021580: 3365 2b30 320a 2020 2020 2020 5920 426f  3e+02.      Y Bo
+00021590: 756e 6473 3a20 2020 2d31 2e32 3030 652b  unds:   -1.200e+
+000215a0: 3032 2c20 312e 3431 3565 2b30 320a 2020  02, 1.415e+02.  
+000215b0: 2020 2020 5a20 426f 756e 6473 3a20 2020      Z Bounds:   
+000215c0: 312e 3636 3665 2b30 312c 2034 2e30 3737  1.666e+01, 4.077
+000215d0: 652b 3032 0a20 2020 2020 204e 2041 7272  e+02.      N Arr
+000215e0: 6179 733a 2020 2030 0a0a 0a20 2020 2022  ays:   0...    "
+000215f0: 2222 0a20 2020 2066 696c 656e 616d 6520  "".    filename 
+00021600: 3d20 5f64 6f77 6e6c 6f61 645f 6172 6368  = _download_arch
+00021610: 6976 6528 0a20 2020 2020 2020 2027 6976  ive(.        'iv
+00021620: 616e 2d6e 696b 6f6c 6f76 2f62 6c61 636b  an-nikolov/black
+00021630: 5661 7365 2e7a 6970 272c 0a20 2020 2020  Vase.zip',.     
+00021640: 2020 2027 626c 6163 6b56 6173 652e 7674     'blackVase.vt
+00021650: 7027 2c0a 2020 2020 290a 2020 2020 6966  p',.    ).    if
+00021660: 206c 6f61 643a 0a20 2020 2020 2020 2072   load:.        r
+00021670: 6574 7572 6e20 7079 7669 7374 612e 7265  eturn pyvista.re
+00021680: 6164 2866 696c 656e 616d 6529 0a20 2020  ad(filename).   
+00021690: 2072 6574 7572 6e20 6669 6c65 6e61 6d65   return filename
+000216a0: 0a0a 0a64 6566 2064 6f77 6e6c 6f61 645f  ...def download_
+000216b0: 6976 616e 5f61 6e67 656c 286c 6f61 643d  ivan_angel(load=
+000216c0: 5472 7565 293a 2020 2320 7072 6167 6d61  True):  # pragma
+000216d0: 3a20 6e6f 2063 6f76 6572 0a20 2020 2022  : no cover.    "
+000216e0: 2222 446f 776e 6c6f 6164 2061 2073 6361  ""Download a sca
+000216f0: 6e20 6f66 2061 6e20 616e 6765 6c20 7374  n of an angel st
+00021700: 6174 7565 2063 7265 6174 6564 2062 7920  atue created by 
+00021710: 4976 616e 204e 696b 6f6c 6f76 2e0a 0a20  Ivan Nikolov... 
+00021720: 2020 2054 6865 2064 6174 6173 6574 2077     The dataset w
+00021730: 6173 2064 6f77 6e6c 6f61 6465 6420 6672  as downloaded fr
+00021740: 6f6d 2060 4747 472d 4265 6e63 686d 6172  om `GGG-Benchmar
+00021750: 6b53 664d 3a20 4461 7461 7365 7420 666f  kSfM: Dataset fo
+00021760: 7220 4265 6e63 686d 6172 6b69 6e67 0a20  r Benchmarking. 
+00021770: 2020 2043 6c6f 7365 2d72 616e 6765 2053     Close-range S
+00021780: 664d 2053 6f66 7477 6172 6520 5065 7266  fM Software Perf
+00021790: 6f72 6d61 6e63 6520 756e 6465 7220 5661  ormance under Va
+000217a0: 7279 696e 6720 4361 7074 7572 696e 6720  rying Capturing 
+000217b0: 436f 6e64 6974 696f 6e73 0a20 2020 203c  Conditions.    <
+000217c0: 6874 7470 733a 2f2f 6461 7461 2e6d 656e  https://data.men
+000217d0: 6465 6c65 792e 636f 6d2f 6461 7461 7365  deley.com/datase
+000217e0: 7473 2f62 7a78 6b32 6e37 3873 392f 343e  ts/bzxk2n78s9/4>
+000217f0: 605f 0a0a 2020 2020 4f72 6967 696e 616c  `_..    Original
+00021800: 2064 6174 6173 6574 7320 6172 6520 756e   datasets are un
+00021810: 6465 7220 7468 6520 4343 2042 5920 342e  der the CC BY 4.
+00021820: 3020 6c69 6365 6e73 652e 0a0a 2020 2020  0 license...    
+00021830: 466f 7220 6d6f 7265 2064 6574 6169 6c73  For more details
+00021840: 2c20 7365 6520 6049 7661 6e20 4e69 6b6f  , see `Ivan Niko
+00021850: 6c6f 7620 4461 7461 7365 7473 0a20 2020  lov Datasets.   
+00021860: 203c 6874 7470 733a 2f2f 6769 7468 7562   <https://github
+00021870: 2e63 6f6d 2f70 7976 6973 7461 2f76 746b  .com/pyvista/vtk
+00021880: 2d64 6174 612f 7472 6565 2f6d 6173 7465  -data/tree/maste
+00021890: 722f 4461 7461 2f69 7661 6e2d 6e69 6b6f  r/Data/ivan-niko
+000218a0: 6c6f 763e 605f 0a0a 2020 2020 5061 7261  lov>`_..    Para
+000218b0: 6d65 7465 7273 0a20 2020 202d 2d2d 2d2d  meters.    -----
+000218c0: 2d2d 2d2d 2d0a 2020 2020 6c6f 6164 203a  -----.    load :
+000218d0: 2062 6f6f 6c2c 2064 6566 6175 6c74 3a20   bool, default: 
+000218e0: 5472 7565 0a20 2020 2020 2020 204c 6f61  True.        Loa
+000218f0: 6420 7468 6520 6461 7461 7365 7420 6166  d the dataset af
+00021900: 7465 7220 646f 776e 6c6f 6164 696e 6720  ter downloading 
+00021910: 6974 2077 6865 6e20 6060 5472 7565 6060  it when ``True``
+00021920: 2e20 2053 6574 2074 6869 730a 2020 2020  .  Set this.    
+00021930: 2020 2020 746f 2060 6046 616c 7365 6060      to ``False``
+00021940: 2061 6e64 206f 6e6c 7920 7468 6520 6669   and only the fi
+00021950: 6c65 6e61 6d65 2077 696c 6c20 6265 2072  lename will be r
+00021960: 6574 7572 6e65 642e 0a0a 2020 2020 5265  eturned...    Re
+00021970: 7475 726e 730a 2020 2020 2d2d 2d2d 2d2d  turns.    ------
+00021980: 2d0a 2020 2020 7079 7669 7374 612e 506f  -.    pyvista.Po
+00021990: 6c79 4461 7461 207c 2073 7472 0a20 2020  lyData | str.   
+000219a0: 2020 2020 2044 6174 6153 6574 206f 7220       DataSet or 
+000219b0: 6669 6c65 6e61 6d65 2064 6570 656e 6469  filename dependi
+000219c0: 6e67 206f 6e20 6060 6c6f 6164 6060 2e0a  ng on ``load``..
+000219d0: 0a20 2020 2045 7861 6d70 6c65 730a 2020  .    Examples.  
+000219e0: 2020 2d2d 2d2d 2d2d 2d2d 0a20 2020 2044    --------.    D
+000219f0: 6f77 6e6c 6f61 6420 616e 6420 706c 6f74  ownload and plot
+00021a00: 2074 6865 2064 6174 6173 6574 2e0a 0a20   the dataset... 
+00021a10: 2020 203e 3e3e 2066 726f 6d20 7079 7669     >>> from pyvi
+00021a20: 7374 6120 696d 706f 7274 2065 7861 6d70  sta import examp
+00021a30: 6c65 730a 2020 2020 3e3e 3e20 6d65 7368  les.    >>> mesh
+00021a40: 203d 2065 7861 6d70 6c65 732e 646f 776e   = examples.down
+00021a50: 6c6f 6164 5f69 7661 6e5f 616e 6765 6c28  load_ivan_angel(
+00021a60: 290a 2020 2020 3e3e 3e20 6370 6f73 203d  ).    >>> cpos =
+00021a70: 205b 0a20 2020 202e 2e2e 2020 2020 2028   [.    ...     (
+00021a80: 2d34 3736 2e31 342c 202d 3339 332e 3733  -476.14, -393.73
+00021a90: 2c20 3238 322e 3134 292c 0a20 2020 202e  , 282.14),.    .
+00021aa0: 2e2e 2020 2020 2028 2d31 352e 3030 2c20  ..     (-15.00, 
+00021ab0: 3131 2e32 352c 2034 342e 3038 292c 0a20  11.25, 44.08),. 
+00021ac0: 2020 202e 2e2e 2020 2020 2028 302e 3236     ...     (0.26
+00021ad0: 2c20 302e 3234 2c20 302e 3933 292c 0a20  , 0.24, 0.93),. 
+00021ae0: 2020 202e 2e2e 205d 0a20 2020 203e 3e3e     ... ].    >>>
+00021af0: 206d 6573 682e 706c 6f74 2863 706f 733d   mesh.plot(cpos=
+00021b00: 6370 6f73 290a 0a20 2020 2052 6574 7572  cpos)..    Retur
+00021b10: 6e20 7468 6520 7374 6174 6973 7469 6373  n the statistics
+00021b20: 206f 6620 7468 6520 6461 7461 7365 742e   of the dataset.
+00021b30: 0a0a 2020 2020 3e3e 3e20 6d65 7368 0a20  ..    >>> mesh. 
+00021b40: 2020 2050 6f6c 7944 6174 6120 282e 2e2e     PolyData (...
+00021b50: 290a 2020 2020 2020 4e20 4365 6c6c 733a  ).      N Cells:
+00021b60: 2020 2020 3335 3830 3435 340a 2020 2020      3580454.    
+00021b70: 2020 4e20 506f 696e 7473 3a20 2020 3138    N Points:   18
+00021b80: 3131 3533 310a 2020 2020 2020 4e20 5374  11531.      N St
+00021b90: 7269 7073 3a20 2020 300a 2020 2020 2020  rips:   0.      
+00021ba0: 5820 426f 756e 6473 3a20 2020 2d31 2e31  X Bounds:   -1.1
+00021bb0: 3437 652b 3032 2c20 382e 3436 3865 2b30  47e+02, 8.468e+0
+00021bc0: 310a 2020 2020 2020 5920 426f 756e 6473  1.      Y Bounds
+00021bd0: 3a20 2020 2d36 2e39 3936 652b 3031 2c20  :   -6.996e+01, 
+00021be0: 392e 3234 3765 2b30 310a 2020 2020 2020  9.247e+01.      
+00021bf0: 5a20 426f 756e 6473 3a20 2020 2d31 2e31  Z Bounds:   -1.1
+00021c00: 3731 652b 3032 2c20 322e 3035 3265 2b30  71e+02, 2.052e+0
+00021c10: 320a 2020 2020 2020 4e20 4172 7261 7973  2.      N Arrays
+00021c20: 3a20 2020 300a 0a20 2020 2022 2222 0a20  :   0..    """. 
+00021c30: 2020 2066 696c 656e 616d 6520 3d20 5f64     filename = _d
+00021c40: 6f77 6e6c 6f61 645f 6172 6368 6976 6528  ownload_archive(
+00021c50: 0a20 2020 2020 2020 2027 6976 616e 2d6e  .        'ivan-n
+00021c60: 696b 6f6c 6f76 2f41 6e67 656c 2e7a 6970  ikolov/Angel.zip
+00021c70: 272c 0a20 2020 2020 2020 2027 416e 6765  ',.        'Ange
+00021c80: 6c2e 7674 7027 2c0a 2020 2020 290a 2020  l.vtp',.    ).  
+00021c90: 2020 6966 206c 6f61 643a 0a20 2020 2020    if load:.     
+00021ca0: 2020 2072 6574 7572 6e20 7079 7669 7374     return pyvist
+00021cb0: 612e 7265 6164 2866 696c 656e 616d 6529  a.read(filename)
+00021cc0: 0a20 2020 2072 6574 7572 6e20 6669 6c65  .    return file
+00021cd0: 6e61 6d65 0a0a 0a64 6566 2064 6f77 6e6c  name...def downl
+00021ce0: 6f61 645f 6269 7264 5f62 6174 6828 6c6f  oad_bird_bath(lo
+00021cf0: 6164 3d54 7275 6529 3a20 2023 2070 7261  ad=True):  # pra
+00021d00: 676d 613a 206e 6f20 636f 7665 720a 2020  gma: no cover.  
+00021d10: 2020 2222 2244 6f77 6e6c 6f61 6420 6120    """Download a 
+00021d20: 7363 616e 206f 6620 6120 6269 7264 2062  scan of a bird b
+00021d30: 6174 6820 6372 6561 7465 6420 6279 2049  ath created by I
+00021d40: 7661 6e20 4e69 6b6f 6c6f 762e 0a0a 2020  van Nikolov...  
+00021d50: 2020 5468 6520 6461 7461 7365 7420 7761    The dataset wa
+00021d60: 7320 646f 776e 6c6f 6164 6564 2066 726f  s downloaded fro
+00021d70: 6d20 6047 4747 2d42 656e 6368 6d61 726b  m `GGG-Benchmark
+00021d80: 5366 4d3a 2044 6174 6173 6574 2066 6f72  SfM: Dataset for
+00021d90: 2042 656e 6368 6d61 726b 696e 670a 2020   Benchmarking.  
+00021da0: 2020 436c 6f73 652d 7261 6e67 6520 5366    Close-range Sf
+00021db0: 4d20 536f 6674 7761 7265 2050 6572 666f  M Software Perfo
+00021dc0: 726d 616e 6365 2075 6e64 6572 2056 6172  rmance under Var
+00021dd0: 7969 6e67 2043 6170 7475 7269 6e67 2043  ying Capturing C
+00021de0: 6f6e 6469 7469 6f6e 730a 2020 2020 3c68  onditions.    <h
+00021df0: 7474 7073 3a2f 2f64 6174 612e 6d65 6e64  ttps://data.mend
+00021e00: 656c 6579 2e63 6f6d 2f64 6174 6173 6574  eley.com/dataset
+00021e10: 732f 627a 786b 326e 3738 7339 2f34 3e60  s/bzxk2n78s9/4>`
+00021e20: 5f0a 0a20 2020 204f 7269 6769 6e61 6c20  _..    Original 
+00021e30: 6461 7461 7365 7473 2061 7265 2075 6e64  datasets are und
+00021e40: 6572 2074 6865 2043 4320 4259 2034 2e30  er the CC BY 4.0
+00021e50: 206c 6963 656e 7365 2e0a 0a20 2020 2046   license...    F
+00021e60: 6f72 206d 6f72 6520 6465 7461 696c 732c  or more details,
+00021e70: 2073 6565 2060 4976 616e 204e 696b 6f6c   see `Ivan Nikol
+00021e80: 6f76 2044 6174 6173 6574 730a 2020 2020  ov Datasets.    
+00021e90: 3c68 7474 7073 3a2f 2f67 6974 6875 622e  <https://github.
+00021ea0: 636f 6d2f 7079 7669 7374 612f 7674 6b2d  com/pyvista/vtk-
+00021eb0: 6461 7461 2f74 7265 652f 6d61 7374 6572  data/tree/master
+00021ec0: 2f44 6174 612f 6976 616e 2d6e 696b 6f6c  /Data/ivan-nikol
+00021ed0: 6f76 3e60 5f0a 0a20 2020 2050 6172 616d  ov>`_..    Param
+00021ee0: 6574 6572 730a 2020 2020 2d2d 2d2d 2d2d  eters.    ------
+00021ef0: 2d2d 2d2d 0a20 2020 206c 6f61 6420 3a20  ----.    load : 
+00021f00: 626f 6f6c 2c20 6465 6661 756c 743a 2054  bool, default: T
+00021f10: 7275 650a 2020 2020 2020 2020 4c6f 6164  rue.        Load
+00021f20: 2074 6865 2064 6174 6173 6574 2061 6674   the dataset aft
+00021f30: 6572 2064 6f77 6e6c 6f61 6469 6e67 2069  er downloading i
+00021f40: 7420 7768 656e 2060 6054 7275 6560 602e  t when ``True``.
+00021f50: 2020 5365 7420 7468 6973 0a20 2020 2020    Set this.     
+00021f60: 2020 2074 6f20 6060 4661 6c73 6560 6020     to ``False`` 
+00021f70: 616e 6420 6f6e 6c79 2074 6865 2066 696c  and only the fil
+00021f80: 656e 616d 6520 7769 6c6c 2062 6520 7265  ename will be re
+00021f90: 7475 726e 6564 2e0a 0a20 2020 2052 6574  turned...    Ret
+00021fa0: 7572 6e73 0a20 2020 202d 2d2d 2d2d 2d2d  urns.    -------
+00021fb0: 0a20 2020 2070 7976 6973 7461 2e50 6f6c  .    pyvista.Pol
+00021fc0: 7944 6174 6120 7c20 7374 720a 2020 2020  yData | str.    
+00021fd0: 2020 2020 4461 7461 5365 7420 6f72 2066      DataSet or f
+00021fe0: 696c 656e 616d 6520 6465 7065 6e64 696e  ilename dependin
+00021ff0: 6720 6f6e 2060 606c 6f61 6460 602e 0a0a  g on ``load``...
+00022000: 2020 2020 4578 616d 706c 6573 0a20 2020      Examples.   
+00022010: 202d 2d2d 2d2d 2d2d 2d0a 2020 2020 446f   --------.    Do
+00022020: 776e 6c6f 6164 2061 6e64 2070 6c6f 7420  wnload and plot 
+00022030: 7468 6520 6461 7461 7365 742e 0a0a 2020  the dataset...  
+00022040: 2020 3e3e 3e20 6672 6f6d 2070 7976 6973    >>> from pyvis
+00022050: 7461 2069 6d70 6f72 7420 6578 616d 706c  ta import exampl
+00022060: 6573 0a20 2020 203e 3e3e 206d 6573 6820  es.    >>> mesh 
+00022070: 3d20 6578 616d 706c 6573 2e64 6f77 6e6c  = examples.downl
+00022080: 6f61 645f 6269 7264 5f62 6174 6828 290a  oad_bird_bath().
+00022090: 2020 2020 3e3e 3e20 6d65 7368 2e70 6c6f      >>> mesh.plo
+000220a0: 7428 290a 0a20 2020 2052 6574 7572 6e20  t()..    Return 
+000220b0: 7468 6520 7374 6174 6973 7469 6373 206f  the statistics o
+000220c0: 6620 7468 6520 6461 7461 7365 742e 0a0a  f the dataset...
+000220d0: 2020 2020 3e3e 3e20 6d65 7368 0a20 2020      >>> mesh.   
+000220e0: 2050 6f6c 7944 6174 6120 282e 2e2e 290a   PolyData (...).
+000220f0: 2020 2020 2020 4e20 4365 6c6c 733a 2020        N Cells:  
+00022100: 2020 3335 3037 3933 350a 2020 2020 2020    3507935.      
+00022110: 4e20 506f 696e 7473 3a20 2020 3138 3331  N Points:   1831
+00022120: 3338 330a 2020 2020 2020 4e20 5374 7269  383.      N Stri
+00022130: 7073 3a20 2020 300a 2020 2020 2020 5820  ps:   0.      X 
+00022140: 426f 756e 6473 3a20 2020 2d31 2e36 3031  Bounds:   -1.601
+00022150: 652b 3032 2c20 312e 3438 3365 2b30 320a  e+02, 1.483e+02.
+00022160: 2020 2020 2020 5920 426f 756e 6473 3a20        Y Bounds: 
+00022170: 2020 2d31 2e35 3231 652b 3032 2c20 312e    -1.521e+02, 1.
+00022180: 3534 3765 2b30 320a 2020 2020 2020 5a20  547e+02.      Z 
+00022190: 426f 756e 6473 3a20 2020 2d34 2e32 3431  Bounds:   -4.241
+000221a0: 652b 3030 2c20 312e 3430 3965 2b30 320a  e+00, 1.409e+02.
+000221b0: 2020 2020 2020 4e20 4172 7261 7973 3a20        N Arrays: 
+000221c0: 2020 300a 0a20 2020 2022 2222 0a20 2020    0..    """.   
+000221d0: 2066 696c 656e 616d 6520 3d20 5f64 6f77   filename = _dow
+000221e0: 6e6c 6f61 645f 6172 6368 6976 6528 0a20  nload_archive(. 
+000221f0: 2020 2020 2020 2027 6976 616e 2d6e 696b         'ivan-nik
+00022200: 6f6c 6f76 2f62 6972 6442 6174 682e 7a69  olov/birdBath.zi
+00022210: 7027 2c0a 2020 2020 2020 2020 2762 6972  p',.        'bir
+00022220: 6442 6174 682e 7674 7027 2c0a 2020 2020  dBath.vtp',.    
+00022230: 290a 2020 2020 6966 206c 6f61 643a 0a20  ).    if load:. 
+00022240: 2020 2020 2020 2072 6574 7572 6e20 7079         return py
+00022250: 7669 7374 612e 7265 6164 2866 696c 656e  vista.read(filen
+00022260: 616d 6529 0a20 2020 2072 6574 7572 6e20  ame).    return 
+00022270: 6669 6c65 6e61 6d65 0a0a 0a64 6566 2064  filename...def d
+00022280: 6f77 6e6c 6f61 645f 6f77 6c28 6c6f 6164  ownload_owl(load
+00022290: 3d54 7275 6529 3a20 2023 2070 7261 676d  =True):  # pragm
+000222a0: 613a 206e 6f20 636f 7665 720a 2020 2020  a: no cover.    
+000222b0: 2222 2244 6f77 6e6c 6f61 6420 6120 7363  """Download a sc
+000222c0: 616e 206f 6620 616e 206f 776c 2073 7461  an of an owl sta
+000222d0: 7475 6520 6372 6561 7465 6420 6279 2049  tue created by I
+000222e0: 7661 6e20 4e69 6b6f 6c6f 762e 0a0a 2020  van Nikolov...  
+000222f0: 2020 5468 6520 6461 7461 7365 7420 7761    The dataset wa
+00022300: 7320 646f 776e 6c6f 6164 6564 2066 726f  s downloaded fro
+00022310: 6d20 6047 4747 2d42 656e 6368 6d61 726b  m `GGG-Benchmark
+00022320: 5366 4d3a 2044 6174 6173 6574 2066 6f72  SfM: Dataset for
+00022330: 2042 656e 6368 6d61 726b 696e 670a 2020   Benchmarking.  
+00022340: 2020 436c 6f73 652d 7261 6e67 6520 5366    Close-range Sf
+00022350: 4d20 536f 6674 7761 7265 2050 6572 666f  M Software Perfo
+00022360: 726d 616e 6365 2075 6e64 6572 2056 6172  rmance under Var
+00022370: 7969 6e67 2043 6170 7475 7269 6e67 2043  ying Capturing C
+00022380: 6f6e 6469 7469 6f6e 730a 2020 2020 3c68  onditions.    <h
+00022390: 7474 7073 3a2f 2f64 6174 612e 6d65 6e64  ttps://data.mend
+000223a0: 656c 6579 2e63 6f6d 2f64 6174 6173 6574  eley.com/dataset
+000223b0: 732f 627a 786b 326e 3738 7339 2f34 3e60  s/bzxk2n78s9/4>`
+000223c0: 5f0a 0a20 2020 204f 7269 6769 6e61 6c20  _..    Original 
+000223d0: 6461 7461 7365 7473 2061 7265 2075 6e64  datasets are und
+000223e0: 6572 2074 6865 2043 4320 4259 2034 2e30  er the CC BY 4.0
+000223f0: 206c 6963 656e 7365 2e0a 0a20 2020 2046   license...    F
+00022400: 6f72 206d 6f72 6520 6465 7461 696c 732c  or more details,
+00022410: 2073 6565 2060 4976 616e 204e 696b 6f6c   see `Ivan Nikol
+00022420: 6f76 2044 6174 6173 6574 730a 2020 2020  ov Datasets.    
+00022430: 3c68 7474 7073 3a2f 2f67 6974 6875 622e  <https://github.
+00022440: 636f 6d2f 7079 7669 7374 612f 7674 6b2d  com/pyvista/vtk-
+00022450: 6461 7461 2f74 7265 652f 6d61 7374 6572  data/tree/master
+00022460: 2f44 6174 612f 6976 616e 2d6e 696b 6f6c  /Data/ivan-nikol
+00022470: 6f76 3e60 5f0a 0a20 2020 2050 6172 616d  ov>`_..    Param
+00022480: 6574 6572 730a 2020 2020 2d2d 2d2d 2d2d  eters.    ------
+00022490: 2d2d 2d2d 0a20 2020 206c 6f61 6420 3a20  ----.    load : 
+000224a0: 626f 6f6c 2c20 6465 6661 756c 743a 2054  bool, default: T
+000224b0: 7275 650a 2020 2020 2020 2020 4c6f 6164  rue.        Load
+000224c0: 2074 6865 2064 6174 6173 6574 2061 6674   the dataset aft
+000224d0: 6572 2064 6f77 6e6c 6f61 6469 6e67 2069  er downloading i
+000224e0: 7420 7768 656e 2060 6054 7275 6560 602e  t when ``True``.
+000224f0: 2020 5365 7420 7468 6973 0a20 2020 2020    Set this.     
+00022500: 2020 2074 6f20 6060 4661 6c73 6560 6020     to ``False`` 
+00022510: 616e 6420 6f6e 6c79 2074 6865 2066 696c  and only the fil
+00022520: 656e 616d 6520 7769 6c6c 2062 6520 7265  ename will be re
+00022530: 7475 726e 6564 2e0a 0a20 2020 2052 6574  turned...    Ret
+00022540: 7572 6e73 0a20 2020 202d 2d2d 2d2d 2d2d  urns.    -------
+00022550: 0a20 2020 2070 7976 6973 7461 2e50 6f6c  .    pyvista.Pol
+00022560: 7944 6174 6120 7c20 7374 720a 2020 2020  yData | str.    
+00022570: 2020 2020 4461 7461 5365 7420 6f72 2066      DataSet or f
+00022580: 696c 656e 616d 6520 6465 7065 6e64 696e  ilename dependin
+00022590: 6720 6f6e 2060 606c 6f61 6460 602e 0a0a  g on ``load``...
+000225a0: 2020 2020 4578 616d 706c 6573 0a20 2020      Examples.   
+000225b0: 202d 2d2d 2d2d 2d2d 2d0a 2020 2020 446f   --------.    Do
+000225c0: 776e 6c6f 6164 2061 6e64 2070 6c6f 7420  wnload and plot 
+000225d0: 7468 6520 6461 7461 7365 742e 0a0a 2020  the dataset...  
+000225e0: 2020 3e3e 3e20 6672 6f6d 2070 7976 6973    >>> from pyvis
+000225f0: 7461 2069 6d70 6f72 7420 6578 616d 706c  ta import exampl
+00022600: 6573 0a20 2020 203e 3e3e 206d 6573 6820  es.    >>> mesh 
+00022610: 3d20 6578 616d 706c 6573 2e64 6f77 6e6c  = examples.downl
+00022620: 6f61 645f 6f77 6c28 290a 2020 2020 3e3e  oad_owl().    >>
+00022630: 3e20 6370 6f73 203d 205b 0a20 2020 202e  > cpos = [.    .
+00022640: 2e2e 2020 2020 2028 2d33 3135 2e31 382c  ..     (-315.18,
+00022650: 202d 3430 322e 3231 2c20 3233 302e 3731   -402.21, 230.71
+00022660: 292c 0a20 2020 202e 2e2e 2020 2020 2028  ),.    ...     (
+00022670: 362e 3036 2c20 2d31 2e37 342c 2031 3031  6.06, -1.74, 101
+00022680: 2e34 3829 2c0a 2020 2020 2e2e 2e20 2020  .48),.    ...   
+00022690: 2020 2830 2e31 3038 2c20 302e 3232 362c    (0.108, 0.226,
+000226a0: 2030 2e39 3638 292c 0a20 2020 202e 2e2e   0.968),.    ...
+000226b0: 205d 0a20 2020 203e 3e3e 206d 6573 682e   ].    >>> mesh.
+000226c0: 706c 6f74 2863 706f 733d 6370 6f73 290a  plot(cpos=cpos).
+000226d0: 0a20 2020 2052 6574 7572 6e20 7468 6520  .    Return the 
+000226e0: 7374 6174 6973 7469 6373 206f 6620 7468  statistics of th
+000226f0: 6520 6461 7461 7365 742e 0a0a 2020 2020  e dataset...    
+00022700: 3e3e 3e20 6d65 7368 0a20 2020 2050 6f6c  >>> mesh.    Pol
+00022710: 7944 6174 6120 282e 2e2e 290a 2020 2020  yData (...).    
+00022720: 2020 4e20 4365 6c6c 733a 2020 2020 3234    N Cells:    24
+00022730: 3430 3730 370a 2020 2020 2020 4e20 506f  40707.      N Po
+00022740: 696e 7473 3a20 2020 3132 3231 3735 360a  ints:   1221756.
+00022750: 2020 2020 2020 4e20 5374 7269 7073 3a20        N Strips: 
+00022760: 2020 300a 2020 2020 2020 5820 426f 756e    0.      X Boun
+00022770: 6473 3a20 2020 2d35 2e38 3334 652b 3031  ds:   -5.834e+01
+00022780: 2c20 372e 3034 3765 2b30 310a 2020 2020  , 7.047e+01.    
+00022790: 2020 5920 426f 756e 6473 3a20 2020 2d37    Y Bounds:   -7
+000227a0: 2e30 3036 652b 3031 2c20 362e 3635 3865  .006e+01, 6.658e
+000227b0: 2b30 310a 2020 2020 2020 5a20 426f 756e  +01.      Z Boun
+000227c0: 6473 3a20 2020 312e 3637 3665 2b30 302c  ds:   1.676e+00,
+000227d0: 2032 2e30 3133 652b 3032 0a20 2020 2020   2.013e+02.     
+000227e0: 204e 2041 7272 6179 733a 2020 2030 0a0a   N Arrays:   0..
+000227f0: 2020 2020 2222 220a 2020 2020 6669 6c65      """.    file
+00022800: 6e61 6d65 203d 205f 646f 776e 6c6f 6164  name = _download
+00022810: 5f61 7263 6869 7665 280a 2020 2020 2020  _archive(.      
+00022820: 2020 2769 7661 6e2d 6e69 6b6f 6c6f 762f    'ivan-nikolov/
+00022830: 6f77 6c2e 7a69 7027 2c0a 2020 2020 2020  owl.zip',.      
+00022840: 2020 276f 776c 2e76 7470 272c 0a20 2020    'owl.vtp',.   
+00022850: 2029 0a20 2020 2069 6620 6c6f 6164 3a0a   ).    if load:.
+00022860: 2020 2020 2020 2020 7265 7475 726e 2070          return p
+00022870: 7976 6973 7461 2e72 6561 6428 6669 6c65  yvista.read(file
+00022880: 6e61 6d65 290a 2020 2020 7265 7475 726e  name).    return
+00022890: 2066 696c 656e 616d 650a 0a0a 6465 6620   filename...def 
+000228a0: 646f 776e 6c6f 6164 5f70 6c61 7374 6963  download_plastic
+000228b0: 5f76 6173 6528 6c6f 6164 3d54 7275 6529  _vase(load=True)
+000228c0: 3a20 2023 2070 7261 676d 613a 206e 6f20  :  # pragma: no 
+000228d0: 636f 7665 720a 2020 2020 2222 2244 6f77  cover.    """Dow
+000228e0: 6e6c 6f61 6420 6120 7363 616e 206f 6620  nload a scan of 
+000228f0: 6120 706c 6173 7469 6320 7661 7365 2063  a plastic vase c
+00022900: 7265 6174 6564 2062 7920 4976 616e 204e  reated by Ivan N
+00022910: 696b 6f6c 6f76 2e0a 0a20 2020 2054 6865  ikolov...    The
+00022920: 2064 6174 6173 6574 2077 6173 2064 6f77   dataset was dow
+00022930: 6e6c 6f61 6465 6420 6672 6f6d 2060 4747  nloaded from `GG
+00022940: 472d 4265 6e63 686d 6172 6b53 664d 3a20  G-BenchmarkSfM: 
+00022950: 4461 7461 7365 7420 666f 7220 4265 6e63  Dataset for Benc
+00022960: 686d 6172 6b69 6e67 0a20 2020 2043 6c6f  hmarking.    Clo
+00022970: 7365 2d72 616e 6765 2053 664d 2053 6f66  se-range SfM Sof
+00022980: 7477 6172 6520 5065 7266 6f72 6d61 6e63  tware Performanc
+00022990: 6520 756e 6465 7220 5661 7279 696e 6720  e under Varying 
+000229a0: 4361 7074 7572 696e 6720 436f 6e64 6974  Capturing Condit
+000229b0: 696f 6e73 0a20 2020 203c 6874 7470 733a  ions.    <https:
+000229c0: 2f2f 6461 7461 2e6d 656e 6465 6c65 792e  //data.mendeley.
+000229d0: 636f 6d2f 6461 7461 7365 7473 2f62 7a78  com/datasets/bzx
+000229e0: 6b32 6e37 3873 392f 343e 605f 0a0a 2020  k2n78s9/4>`_..  
+000229f0: 2020 4f72 6967 696e 616c 2064 6174 6173    Original datas
+00022a00: 6574 7320 6172 6520 756e 6465 7220 7468  ets are under th
+00022a10: 6520 4343 2042 5920 342e 3020 6c69 6365  e CC BY 4.0 lice
+00022a20: 6e73 652e 0a0a 2020 2020 466f 7220 6d6f  nse...    For mo
+00022a30: 7265 2064 6574 6169 6c73 2c20 7365 6520  re details, see 
+00022a40: 6049 7661 6e20 4e69 6b6f 6c6f 7620 4461  `Ivan Nikolov Da
+00022a50: 7461 7365 7473 0a20 2020 203c 6874 7470  tasets.    <http
+00022a60: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f70  s://github.com/p
+00022a70: 7976 6973 7461 2f76 746b 2d64 6174 612f  yvista/vtk-data/
+00022a80: 7472 6565 2f6d 6173 7465 722f 4461 7461  tree/master/Data
+00022a90: 2f69 7661 6e2d 6e69 6b6f 6c6f 763e 605f  /ivan-nikolov>`_
+00022aa0: 0a0a 2020 2020 5061 7261 6d65 7465 7273  ..    Parameters
+00022ab0: 0a20 2020 202d 2d2d 2d2d 2d2d 2d2d 2d0a  .    ----------.
+00022ac0: 2020 2020 6c6f 6164 203a 2062 6f6f 6c2c      load : bool,
+00022ad0: 2064 6566 6175 6c74 3a20 5472 7565 0a20   default: True. 
+00022ae0: 2020 2020 2020 204c 6f61 6420 7468 6520         Load the 
+00022af0: 6461 7461 7365 7420 6166 7465 7220 646f  dataset after do
+00022b00: 776e 6c6f 6164 696e 6720 6974 2077 6865  wnloading it whe
+00022b10: 6e20 6060 5472 7565 6060 2e20 2053 6574  n ``True``.  Set
+00022b20: 2074 6869 730a 2020 2020 2020 2020 746f   this.        to
+00022b30: 2060 6046 616c 7365 6060 2061 6e64 206f   ``False`` and o
+00022b40: 6e6c 7920 7468 6520 6669 6c65 6e61 6d65  nly the filename
+00022b50: 2077 696c 6c20 6265 2072 6574 7572 6e65   will be returne
+00022b60: 642e 0a0a 2020 2020 5265 7475 726e 730a  d...    Returns.
+00022b70: 2020 2020 2d2d 2d2d 2d2d 2d0a 2020 2020      -------.    
+00022b80: 7079 7669 7374 612e 506f 6c79 4461 7461  pyvista.PolyData
+00022b90: 207c 2073 7472 0a20 2020 2020 2020 2044   | str.        D
+00022ba0: 6174 6153 6574 206f 7220 6669 6c65 6e61  ataSet or filena
+00022bb0: 6d65 2064 6570 656e 6469 6e67 206f 6e20  me depending on 
+00022bc0: 6060 6c6f 6164 6060 2e0a 0a20 2020 2045  ``load``...    E
+00022bd0: 7861 6d70 6c65 730a 2020 2020 2d2d 2d2d  xamples.    ----
+00022be0: 2d2d 2d2d 0a20 2020 2044 6f77 6e6c 6f61  ----.    Downloa
+00022bf0: 6420 616e 6420 706c 6f74 2074 6865 2064  d and plot the d
+00022c00: 6174 6173 6574 2e0a 0a20 2020 203e 3e3e  ataset...    >>>
+00022c10: 2066 726f 6d20 7079 7669 7374 6120 696d   from pyvista im
+00022c20: 706f 7274 2065 7861 6d70 6c65 730a 2020  port examples.  
+00022c30: 2020 3e3e 3e20 6d65 7368 203d 2065 7861    >>> mesh = exa
+00022c40: 6d70 6c65 732e 646f 776e 6c6f 6164 5f70  mples.download_p
+00022c50: 6c61 7374 6963 5f76 6173 6528 290a 2020  lastic_vase().  
+00022c60: 2020 3e3e 3e20 6d65 7368 2e70 6c6f 7428    >>> mesh.plot(
+00022c70: 290a 0a20 2020 2052 6574 7572 6e20 7468  )..    Return th
+00022c80: 6520 7374 6174 6973 7469 6373 206f 6620  e statistics of 
+00022c90: 7468 6520 6461 7461 7365 742e 0a0a 2020  the dataset...  
+00022ca0: 2020 3e3e 3e20 6d65 7368 0a20 2020 2050    >>> mesh.    P
+00022cb0: 6f6c 7944 6174 6120 282e 2e2e 290a 2020  olyData (...).  
+00022cc0: 2020 2020 4e20 4365 6c6c 733a 2020 2020      N Cells:    
+00022cd0: 3335 3730 3936 370a 2020 2020 2020 4e20  3570967.      N 
+00022ce0: 506f 696e 7473 3a20 2020 3137 3936 3830  Points:   179680
+00022cf0: 350a 2020 2020 2020 4e20 5374 7269 7073  5.      N Strips
+00022d00: 3a20 2020 300a 2020 2020 2020 5820 426f  :   0.      X Bo
+00022d10: 756e 6473 3a20 2020 2d31 2e33 3634 652b  unds:   -1.364e+
+00022d20: 3032 2c20 312e 3932 3965 2b30 320a 2020  02, 1.929e+02.  
+00022d30: 2020 2020 5920 426f 756e 6473 3a20 2020      Y Bounds:   
+00022d40: 2d31 2e36 3737 652b 3032 2c20 312e 3630  -1.677e+02, 1.60
+00022d50: 3365 2b30 320a 2020 2020 2020 5a20 426f  3e+02.      Z Bo
+00022d60: 756e 6473 3a20 2020 312e 3230 3965 2b30  unds:   1.209e+0
+00022d70: 322c 2034 2e30 3930 652b 3032 0a20 2020  2, 4.090e+02.   
+00022d80: 2020 204e 2041 7272 6179 733a 2020 2030     N Arrays:   0
+00022d90: 0a0a 2020 2020 2222 220a 2020 2020 6669  ..    """.    fi
+00022da0: 6c65 6e61 6d65 203d 205f 646f 776e 6c6f  lename = _downlo
+00022db0: 6164 5f61 7263 6869 7665 280a 2020 2020  ad_archive(.    
+00022dc0: 2020 2020 2769 7661 6e2d 6e69 6b6f 6c6f      'ivan-nikolo
+00022dd0: 762f 706c 6173 7469 6356 6173 652e 7a69  v/plasticVase.zi
+00022de0: 7027 2c0a 2020 2020 2020 2020 2770 6c61  p',.        'pla
+00022df0: 7374 6963 5661 7365 2e76 7470 272c 0a20  sticVase.vtp',. 
+00022e00: 2020 2029 0a20 2020 2069 6620 6c6f 6164     ).    if load
+00022e10: 3a0a 2020 2020 2020 2020 7265 7475 726e  :.        return
+00022e20: 2070 7976 6973 7461 2e72 6561 6428 6669   pyvista.read(fi
+00022e30: 6c65 6e61 6d65 290a 2020 2020 7265 7475  lename).    retu
+00022e40: 726e 2066 696c 656e 616d 650a 0a0a 6465  rn filename...de
+00022e50: 6620 646f 776e 6c6f 6164 5f73 6561 5f76  f download_sea_v
+00022e60: 6173 6528 6c6f 6164 3d54 7275 6529 3a20  ase(load=True): 
+00022e70: 2023 2070 7261 676d 613a 206e 6f20 636f   # pragma: no co
+00022e80: 7665 720a 2020 2020 2222 2244 6f77 6e6c  ver.    """Downl
+00022e90: 6f61 6420 6120 7363 616e 206f 6620 6120  oad a scan of a 
+00022ea0: 7365 6120 7661 7365 2063 7265 6174 6564  sea vase created
+00022eb0: 2062 7920 4976 616e 204e 696b 6f6c 6f76   by Ivan Nikolov
+00022ec0: 2e0a 0a20 2020 2054 6865 2064 6174 6173  ...    The datas
+00022ed0: 6574 2077 6173 2064 6f77 6e6c 6f61 6465  et was downloade
+00022ee0: 6420 6672 6f6d 2060 4747 472d 4265 6e63  d from `GGG-Benc
+00022ef0: 686d 6172 6b53 664d 3a20 4461 7461 7365  hmarkSfM: Datase
+00022f00: 7420 666f 7220 4265 6e63 686d 6172 6b69  t for Benchmarki
+00022f10: 6e67 0a20 2020 2043 6c6f 7365 2d72 616e  ng.    Close-ran
+00022f20: 6765 2053 664d 2053 6f66 7477 6172 6520  ge SfM Software 
+00022f30: 5065 7266 6f72 6d61 6e63 6520 756e 6465  Performance unde
+00022f40: 7220 5661 7279 696e 6720 4361 7074 7572  r Varying Captur
+00022f50: 696e 6720 436f 6e64 6974 696f 6e73 0a20  ing Conditions. 
+00022f60: 2020 203c 6874 7470 733a 2f2f 6461 7461     <https://data
+00022f70: 2e6d 656e 6465 6c65 792e 636f 6d2f 6461  .mendeley.com/da
+00022f80: 7461 7365 7473 2f62 7a78 6b32 6e37 3873  tasets/bzxk2n78s
+00022f90: 392f 343e 605f 0a0a 2020 2020 4f72 6967  9/4>`_..    Orig
+00022fa0: 696e 616c 2064 6174 6173 6574 7320 6172  inal datasets ar
+00022fb0: 6520 756e 6465 7220 7468 6520 4343 2042  e under the CC B
+00022fc0: 5920 342e 3020 6c69 6365 6e73 652e 0a0a  Y 4.0 license...
+00022fd0: 2020 2020 466f 7220 6d6f 7265 2064 6574      For more det
+00022fe0: 6169 6c73 2c20 7365 6520 6049 7661 6e20  ails, see `Ivan 
+00022ff0: 4e69 6b6f 6c6f 7620 4461 7461 7365 7473  Nikolov Datasets
+00023000: 0a20 2020 203c 6874 7470 733a 2f2f 6769  .    <https://gi
+00023010: 7468 7562 2e63 6f6d 2f70 7976 6973 7461  thub.com/pyvista
+00023020: 2f76 746b 2d64 6174 612f 7472 6565 2f6d  /vtk-data/tree/m
+00023030: 6173 7465 722f 4461 7461 2f69 7661 6e2d  aster/Data/ivan-
+00023040: 6e69 6b6f 6c6f 763e 605f 0a0a 2020 2020  nikolov>`_..    
+00023050: 5061 7261 6d65 7465 7273 0a20 2020 202d  Parameters.    -
+00023060: 2d2d 2d2d 2d2d 2d2d 2d0a 2020 2020 6c6f  ---------.    lo
+00023070: 6164 203a 2062 6f6f 6c2c 2064 6566 6175  ad : bool, defau
+00023080: 6c74 3a20 5472 7565 0a20 2020 2020 2020  lt: True.       
+00023090: 204c 6f61 6420 7468 6520 6461 7461 7365   Load the datase
+000230a0: 7420 6166 7465 7220 646f 776e 6c6f 6164  t after download
+000230b0: 696e 6720 6974 2077 6865 6e20 6060 5472  ing it when ``Tr
+000230c0: 7565 6060 2e20 2053 6574 2074 6869 730a  ue``.  Set this.
+000230d0: 2020 2020 2020 2020 746f 2060 6046 616c          to ``Fal
+000230e0: 7365 6060 2061 6e64 206f 6e6c 7920 7468  se`` and only th
+000230f0: 6520 6669 6c65 6e61 6d65 2077 696c 6c20  e filename will 
+00023100: 6265 2072 6574 7572 6e65 642e 0a0a 2020  be returned...  
+00023110: 2020 5265 7475 726e 730a 2020 2020 2d2d    Returns.    --
+00023120: 2d2d 2d2d 2d0a 2020 2020 7079 7669 7374  -----.    pyvist
+00023130: 612e 506f 6c79 4461 7461 207c 2073 7472  a.PolyData | str
+00023140: 0a20 2020 2020 2020 2044 6174 6153 6574  .        DataSet
+00023150: 206f 7220 6669 6c65 6e61 6d65 2064 6570   or filename dep
+00023160: 656e 6469 6e67 206f 6e20 6060 6c6f 6164  ending on ``load
+00023170: 6060 2e0a 0a20 2020 2045 7861 6d70 6c65  ``...    Example
+00023180: 730a 2020 2020 2d2d 2d2d 2d2d 2d2d 0a20  s.    --------. 
+00023190: 2020 2044 6f77 6e6c 6f61 6420 616e 6420     Download and 
+000231a0: 706c 6f74 2074 6865 2064 6174 6173 6574  plot the dataset
+000231b0: 2e0a 0a20 2020 203e 3e3e 2066 726f 6d20  ...    >>> from 
+000231c0: 7079 7669 7374 6120 696d 706f 7274 2065  pyvista import e
+000231d0: 7861 6d70 6c65 730a 2020 2020 3e3e 3e20  xamples.    >>> 
+000231e0: 6d65 7368 203d 2065 7861 6d70 6c65 732e  mesh = examples.
+000231f0: 646f 776e 6c6f 6164 5f73 6561 5f76 6173  download_sea_vas
+00023200: 6528 290a 2020 2020 3e3e 3e20 6d65 7368  e().    >>> mesh
+00023210: 2e70 6c6f 7428 290a 0a20 2020 2052 6574  .plot()..    Ret
+00023220: 7572 6e20 7468 6520 7374 6174 6973 7469  urn the statisti
+00023230: 6373 206f 6620 7468 6520 6461 7461 7365  cs of the datase
+00023240: 742e 0a0a 2020 2020 3e3e 3e20 6d65 7368  t...    >>> mesh
+00023250: 0a20 2020 2050 6f6c 7944 6174 6120 282e  .    PolyData (.
+00023260: 2e2e 290a 2020 2020 2020 4e20 4365 6c6c  ..).      N Cell
+00023270: 733a 2020 2020 3335 3438 3437 330a 2020  s:    3548473.  
+00023280: 2020 2020 4e20 506f 696e 7473 3a20 2020      N Points:   
+00023290: 3138 3130 3031 320a 2020 2020 2020 4e20  1810012.      N 
+000232a0: 5374 7269 7073 3a20 2020 300a 2020 2020  Strips:   0.    
+000232b0: 2020 5820 426f 756e 6473 3a20 2020 2d31    X Bounds:   -1
+000232c0: 2e36 3636 652b 3032 2c20 312e 3436 3565  .666e+02, 1.465e
+000232d0: 2b30 320a 2020 2020 2020 5920 426f 756e  +02.      Y Boun
+000232e0: 6473 3a20 2020 2d31 2e37 3432 652b 3032  ds:   -1.742e+02
+000232f0: 2c20 312e 3338 3465 2b30 320a 2020 2020  , 1.384e+02.    
+00023300: 2020 5a20 426f 756e 6473 3a20 2020 2d31    Z Bounds:   -1
+00023310: 2e35 3030 652b 3032 2c20 322e 3939 3265  .500e+02, 2.992e
+00023320: 2b30 320a 2020 2020 2020 4e20 4172 7261  +02.      N Arra
+00023330: 7973 3a20 2020 300a 0a20 2020 2022 2222  ys:   0..    """
+00023340: 0a20 2020 2066 696c 656e 616d 6520 3d20  .    filename = 
+00023350: 5f64 6f77 6e6c 6f61 645f 6172 6368 6976  _download_archiv
+00023360: 6528 0a20 2020 2020 2020 2027 6976 616e  e(.        'ivan
+00023370: 2d6e 696b 6f6c 6f76 2f73 6561 5661 7365  -nikolov/seaVase
+00023380: 2e7a 6970 272c 0a20 2020 2020 2020 2027  .zip',.        '
+00023390: 7365 6156 6173 652e 7674 7027 2c0a 2020  seaVase.vtp',.  
+000233a0: 2020 290a 2020 2020 6966 206c 6f61 643a    ).    if load:
+000233b0: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
+000233c0: 7079 7669 7374 612e 7265 6164 2866 696c  pyvista.read(fil
+000233d0: 656e 616d 6529 0a20 2020 2072 6574 7572  ename).    retur
+000233e0: 6e20 6669 6c65 6e61 6d65 0a0a 0a64 6566  n filename...def
+000233f0: 2064 6f77 6e6c 6f61 645f 6469 6b68 6f6c   download_dikhol
+00023400: 6f6c 6f5f 6e69 6768 7428 293a 2020 2320  olo_night():  # 
+00023410: 7072 6167 6d61 3a20 6e6f 2063 6f76 6572  pragma: no cover
+00023420: 0a20 2020 2022 2222 446f 776e 6c6f 6164  .    """Download
+00023430: 2061 6e64 2072 6561 6420 7468 6520 6469   and read the di
+00023440: 6b68 6f6c 6f20 6e69 6768 7420 6864 7220  kholo night hdr 
+00023450: 7465 7874 7572 6520 6578 616d 706c 652e  texture example.
+00023460: 0a0a 2020 2020 4669 6c65 7320 686f 7374  ..    Files host
+00023470: 6564 2061 7420 6874 7470 733a 2f2f 706f  ed at https://po
+00023480: 6c79 6861 7665 6e2e 636f 6d2f 0a0a 2020  lyhaven.com/..  
+00023490: 2020 5265 7475 726e 730a 2020 2020 2d2d    Returns.    --
+000234a0: 2d2d 2d2d 2d0a 2020 2020 7079 7669 7374  -----.    pyvist
+000234b0: 612e 5465 7874 7572 650a 2020 2020 2020  a.Texture.      
+000234c0: 2020 4844 5220 5465 7874 7572 652e 0a0a    HDR Texture...
+000234d0: 2020 2020 4578 616d 706c 6573 0a20 2020      Examples.   
+000234e0: 202d 2d2d 2d2d 2d2d 2d0a 2020 2020 3e3e   --------.    >>
+000234f0: 3e20 696d 706f 7274 2070 7976 6973 7461  > import pyvista
+00023500: 2061 7320 7076 0a20 2020 203e 3e3e 2066   as pv.    >>> f
+00023510: 726f 6d20 7079 7669 7374 6120 696d 706f  rom pyvista impo
+00023520: 7274 2065 7861 6d70 6c65 730a 2020 2020  rt examples.    
+00023530: 3e3e 3e20 676c 7466 5f66 696c 6520 3d20  >>> gltf_file = 
+00023540: 6578 616d 706c 6573 2e67 6c74 662e 646f  examples.gltf.do
+00023550: 776e 6c6f 6164 5f64 616d 6167 6564 5f68  wnload_damaged_h
+00023560: 656c 6d65 7428 290a 2020 2020 3e3e 3e20  elmet().    >>> 
+00023570: 7465 7874 7572 6520 3d20 6578 616d 706c  texture = exampl
+00023580: 6573 2e64 6f77 6e6c 6f61 645f 6469 6b68  es.download_dikh
+00023590: 6f6c 6f6c 6f5f 6e69 6768 7428 290a 2020  ololo_night().  
+000235a0: 2020 3e3e 3e20 706c 203d 2070 762e 506c    >>> pl = pv.Pl
+000235b0: 6f74 7465 7228 290a 2020 2020 3e3e 3e20  otter().    >>> 
+000235c0: 706c 2e69 6d70 6f72 745f 676c 7466 2867  pl.import_gltf(g
+000235d0: 6c74 665f 6669 6c65 290a 2020 2020 3e3e  ltf_file).    >>
+000235e0: 3e20 706c 2e73 6574 5f65 6e76 6972 6f6e  > pl.set_environ
+000235f0: 6d65 6e74 5f74 6578 7475 7265 2874 6578  ment_texture(tex
+00023600: 7475 7265 290a 2020 2020 3e3e 3e20 706c  ture).    >>> pl
+00023610: 2e73 686f 7728 290a 0a20 2020 2022 2222  .show()..    """
+00023620: 0a20 2020 2074 6578 7475 7265 203d 205f  .    texture = _
+00023630: 646f 776e 6c6f 6164 5f61 6e64 5f72 6561  download_and_rea
+00023640: 6428 2764 696b 686f 6c6f 6c6f 5f6e 6967  d('dikhololo_nig
+00023650: 6874 5f34 6b2e 6864 7227 2c20 7465 7874  ht_4k.hdr', text
+00023660: 7572 653d 5472 7565 290a 2020 2020 7465  ure=True).    te
+00023670: 7874 7572 652e 5365 7443 6f6c 6f72 4d6f  xture.SetColorMo
+00023680: 6465 546f 4469 7265 6374 5363 616c 6172  deToDirectScalar
+00023690: 7328 290a 2020 2020 7465 7874 7572 652e  s().    texture.
+000236a0: 5365 744d 6970 6d61 7028 5472 7565 290a  SetMipmap(True).
+000236b0: 2020 2020 7465 7874 7572 652e 5365 7449      texture.SetI
+000236c0: 6e74 6572 706f 6c61 7465 2854 7275 6529  nterpolate(True)
+000236d0: 0a20 2020 2072 6574 7572 6e20 7465 7874  .    return text
+000236e0: 7572 650a 0a0a 6465 6620 646f 776e 6c6f  ure...def downlo
+000236f0: 6164 5f63 6164 5f6d 6f64 656c 5f63 6173  ad_cad_model_cas
+00023700: 6528 6c6f 6164 3d54 7275 6529 3a20 2023  e(load=True):  #
+00023710: 2070 7261 676d 613a 206e 6f20 636f 7665   pragma: no cove
+00023720: 720a 2020 2020 2222 2244 6f77 6e6c 6f61  r.    """Downloa
+00023730: 6420 6120 4341 4420 6d6f 6465 6c20 6f66  d a CAD model of
+00023740: 2061 2052 6173 7062 6572 7279 2050 4920   a Raspberry PI 
+00023750: 3420 6361 7365 2e0a 0a20 2020 2054 6865  4 case...    The
+00023760: 2064 6174 6173 6574 2077 6173 2064 6f77   dataset was dow
+00023770: 6e6c 6f61 6465 6420 6672 6f6d 2060 5468  nloaded from `Th
+00023780: 696e 6769 7665 7273 650a 2020 2020 3c68  ingiverse.    <h
+00023790: 7474 7073 3a2f 2f77 7777 2e74 6869 6e67  ttps://www.thing
+000237a0: 6976 6572 7365 2e63 6f6d 2f74 6869 6e67  iverse.com/thing
+000237b0: 3a34 3934 3737 3436 3e60 5f0a 0a20 2020  :4947746>`_..   
+000237c0: 204f 7269 6769 6e61 6c20 6461 7461 7365   Original datase
+000237d0: 7473 2061 7265 2075 6e64 6572 2074 6865  ts are under the
+000237e0: 2060 4372 6561 7469 7665 2043 6f6d 6d6f   `Creative Commo
+000237f0: 6e73 202d 2041 7474 7269 6275 7469 6f6e  ns - Attribution
+00023800: 0a20 2020 203c 6874 7470 733a 2f2f 6372  .    <https://cr
+00023810: 6561 7469 7665 636f 6d6d 6f6e 732e 6f72  eativecommons.or
+00023820: 672f 6c69 6365 6e73 6573 2f62 792f 342e  g/licenses/by/4.
+00023830: 302f 3e60 5f20 6c69 6365 6e73 652e 0a0a  0/>`_ license...
+00023840: 2020 2020 5061 7261 6d65 7465 7273 0a20      Parameters. 
+00023850: 2020 202d 2d2d 2d2d 2d2d 2d2d 2d0a 2020     ----------.  
+00023860: 2020 6c6f 6164 203a 2062 6f6f 6c2c 2064    load : bool, d
+00023870: 6566 6175 6c74 3a20 5472 7565 0a20 2020  efault: True.   
+00023880: 2020 2020 204c 6f61 6420 7468 6520 6461       Load the da
+00023890: 7461 7365 7420 6166 7465 7220 646f 776e  taset after down
+000238a0: 6c6f 6164 696e 6720 6974 2077 6865 6e20  loading it when 
+000238b0: 6060 5472 7565 6060 2e20 2053 6574 2074  ``True``.  Set t
+000238c0: 6869 730a 2020 2020 2020 2020 746f 2060  his.        to `
+000238d0: 6046 616c 7365 6060 2061 6e64 206f 6e6c  `False`` and onl
+000238e0: 7920 7468 6520 6669 6c65 6e61 6d65 2077  y the filename w
+000238f0: 696c 6c20 6265 2072 6574 7572 6e65 642e  ill be returned.
+00023900: 0a0a 2020 2020 5265 7475 726e 730a 2020  ..    Returns.  
+00023910: 2020 2d2d 2d2d 2d2d 2d0a 2020 2020 7079    -------.    py
+00023920: 7669 7374 612e 506f 6c79 4461 7461 207c  vista.PolyData |
+00023930: 2073 7472 0a20 2020 2020 2020 2044 6174   str.        Dat
+00023940: 6153 6574 206f 7220 6669 6c65 6e61 6d65  aSet or filename
+00023950: 2064 6570 656e 6469 6e67 206f 6e20 6060   depending on ``
+00023960: 6c6f 6164 6060 2e0a 0a20 2020 2045 7861  load``...    Exa
+00023970: 6d70 6c65 730a 2020 2020 2d2d 2d2d 2d2d  mples.    ------
+00023980: 2d2d 0a20 2020 2044 6f77 6e6c 6f61 6420  --.    Download 
+00023990: 616e 6420 706c 6f74 2074 6865 2064 6174  and plot the dat
+000239a0: 6173 6574 2e0a 0a20 2020 203e 3e3e 2066  aset...    >>> f
+000239b0: 726f 6d20 7079 7669 7374 6120 696d 706f  rom pyvista impo
+000239c0: 7274 2065 7861 6d70 6c65 730a 2020 2020  rt examples.    
+000239d0: 3e3e 3e20 6d65 7368 203d 2065 7861 6d70  >>> mesh = examp
+000239e0: 6c65 732e 646f 776e 6c6f 6164 5f63 6164  les.download_cad
+000239f0: 5f6d 6f64 656c 5f63 6173 6528 290a 2020  _model_case().  
+00023a00: 2020 3e3e 3e20 6d65 7368 2e70 6c6f 7428    >>> mesh.plot(
+00023a10: 290a 0a20 2020 2052 6574 7572 6e20 7468  )..    Return th
+00023a20: 6520 7374 6174 6973 7469 6373 206f 6620  e statistics of 
+00023a30: 7468 6520 6461 7461 7365 742e 0a0a 2020  the dataset...  
+00023a40: 2020 3e3e 3e20 6d65 7368 0a20 2020 2050    >>> mesh.    P
+00023a50: 6f6c 7944 6174 6120 282e 2e2e 290a 2020  olyData (...).  
+00023a60: 2020 2020 4e20 4365 6c6c 733a 2020 2020      N Cells:    
+00023a70: 3135 3434 360a 2020 2020 2020 4e20 506f  15446.      N Po
+00023a80: 696e 7473 3a20 2020 3736 3737 0a20 2020  ints:   7677.   
+00023a90: 2020 204e 2053 7472 6970 733a 2020 2030     N Strips:   0
+00023aa0: 0a20 2020 2020 2058 2042 6f75 6e64 733a  .      X Bounds:
+00023ab0: 2020 202d 362e 3436 3065 2d33 312c 2039     -6.460e-31, 9
+00023ac0: 2e30 3030 652b 3031 0a20 2020 2020 2059  .000e+01.      Y
+00023ad0: 2042 6f75 6e64 733a 2020 202d 332e 3533   Bounds:   -3.53
+00023ae0: 3565 2d33 322c 2031 2e34 3830 652b 3032  5e-32, 1.480e+02
+00023af0: 0a20 2020 2020 205a 2042 6f75 6e64 733a  .      Z Bounds:
+00023b00: 2020 2030 2e30 3030 652b 3030 2c20 322e     0.000e+00, 2.
+00023b10: 3030 3065 2b30 310a 2020 2020 2020 4e20  000e+01.      N 
+00023b20: 4172 7261 7973 3a20 2020 320a 0a20 2020  Arrays:   2..   
+00023b30: 2022 2222 0a20 2020 2072 6574 7572 6e20   """.    return 
+00023b40: 5f64 6f77 6e6c 6f61 645f 616e 645f 7265  _download_and_re
+00023b50: 6164 2827 6361 642f 3439 3437 3734 362f  ad('cad/4947746/
+00023b60: 5665 6e74 6564 5f52 6561 725f 4361 7365  Vented_Rear_Case
+00023b70: 5f57 6974 685f 5069 5f53 7570 706f 7274  _With_Pi_Support
+00023b80: 732e 7674 7027 2c20 6c6f 6164 3d6c 6f61  s.vtp', load=loa
+00023b90: 6429 0a0a 0a64 6566 2064 6f77 6e6c 6f61  d)...def downloa
+00023ba0: 645f 6165 726f 5f62 7261 636b 6574 286c  d_aero_bracket(l
+00023bb0: 6f61 643d 5472 7565 293a 2020 2320 7072  oad=True):  # pr
+00023bc0: 6167 6d61 3a20 6e6f 2063 6f76 6572 0a20  agma: no cover. 
+00023bd0: 2020 2022 2222 446f 776e 6c6f 6164 2074     """Download t
+00023be0: 6865 2066 696e 6974 6520 656c 656d 656e  he finite elemen
+00023bf0: 7420 736f 6c75 7469 6f6e 206f 6620 616e  t solution of an
+00023c00: 2061 6572 6f20 6272 6163 6b65 742e 0a0a   aero bracket...
+00023c10: 2020 2020 4461 7461 2067 656e 6572 6174      Data generat
+00023c20: 6564 2066 726f 6d20 7075 626c 6963 2053  ed from public S
+00023c30: 696d 5363 616c 6520 6578 616d 706c 6573  imScale examples
+00023c40: 2061 7420 6053 696d 5363 616c 6520 5072   at `SimScale Pr
+00023c50: 6f6a 6563 7420 4c69 6272 6172 7920 2d0a  oject Library -.
+00023c60: 2020 2020 5475 7262 6f20 3c68 7474 7073      Turbo <https
+00023c70: 3a2f 2f77 7777 2e73 696d 7363 616c 652e  ://www.simscale.
+00023c80: 636f 6d2f 7072 6f6a 6563 7473 2f61 7961  com/projects/aya
+00023c90: 726e 6f7a 2f74 7572 626f 2f3e 605f 2e0a  rnoz/turbo/>`_..
+00023ca0: 0a20 2020 204c 6963 656e 7369 6e67 2066  .    Licensing f
+00023cb0: 6f72 2074 6869 7320 6461 7461 7365 7420  or this dataset 
+00023cc0: 6973 2067 7261 6e74 6564 2074 6f20 6672  is granted to fr
+00023cd0: 6565 6c79 2061 6e64 2077 6974 686f 7574  eely and without
+00023ce0: 2072 6573 7472 6963 7469 6f6e 0a20 2020   restriction.   
+00023cf0: 2072 6570 726f 6475 6365 2c20 6469 7374   reproduce, dist
+00023d00: 7269 6275 7465 2c20 7075 626c 6973 6820  ribute, publish 
+00023d10: 6163 636f 7264 696e 6720 746f 2074 6865  according to the
+00023d20: 2060 5369 6d53 6361 6c65 2054 6572 6d73   `SimScale Terms
+00023d30: 2061 6e64 0a20 2020 2043 6f6e 6469 7469   and.    Conditi
+00023d40: 6f6e 7320 3c68 7474 7073 3a2f 2f77 7777  ons <https://www
+00023d50: 2e73 696d 7363 616c 652e 636f 6d2f 7465  .simscale.com/te
+00023d60: 726d 732d 616e 642d 636f 6e64 6974 696f  rms-and-conditio
+00023d70: 6e73 2f3e 605f 2e0a 0a20 2020 2054 6869  ns/>`_...    Thi
+00023d80: 7320 7072 6f6a 6563 7420 6465 6d6f 6e73  s project demons
+00023d90: 7472 6174 6573 2074 6865 2073 7461 7469  trates the stati
+00023da0: 6320 7374 7265 7373 2061 6e61 6c79 7369  c stress analysi
+00023db0: 7320 6f66 2074 6872 6565 2061 6972 6372  s of three aircr
+00023dc0: 6166 740a 2020 2020 656e 6769 6e65 2062  aft.    engine b
+00023dd0: 6561 7269 6e67 2062 7261 636b 6574 206d  earing bracket m
+00023de0: 6f64 656c 7320 636f 6e73 6964 6572 696e  odels considerin
+00023df0: 6720 626f 7468 206c 696e 6561 7220 616e  g both linear an
+00023e00: 6420 6e6f 6e6c 696e 6561 720a 2020 2020  d nonlinear.    
+00023e10: 6d61 7465 7269 616c 2064 6566 696e 6974  material definit
+00023e20: 696f 6e2e 2054 6865 206d 6f64 656c 7320  ion. The models 
+00023e30: 6172 6520 7465 7374 6564 2077 6974 6820  are tested with 
+00023e40: 686f 7269 7a6f 6e74 616c 2061 6e64 2076  horizontal and v
+00023e50: 6572 7469 6361 6c0a 2020 2020 6c6f 6164  ertical.    load
+00023e60: 696e 6720 636f 6e64 6974 696f 6e73 2061  ing conditions a
+00023e70: 7320 7072 6f76 6964 6564 206f 6e20 7468  s provided on th
+00023e80: 6520 6047 7261 6243 4144 202d 2041 6972  e `GrabCAD - Air
+00023e90: 706c 616e 6520 4265 6172 696e 6720 4272  plane Bearing Br
+00023ea0: 6163 6b65 740a 2020 2020 4368 616c 6c65  acket.    Challe
+00023eb0: 6e67 650a 2020 2020 3c68 7474 7073 3a2f  nge.    <https:/
+00023ec0: 2f67 7261 6263 6164 2e63 6f6d 2f63 6861  /grabcad.com/cha
+00023ed0: 6c6c 656e 6765 732f 6169 7270 6c61 6e65  llenges/airplane
+00023ee0: 2d62 6561 7269 6e67 2d62 7261 636b 6574  -bearing-bracket
+00023ef0: 2d63 6861 6c6c 656e 6765 2f65 6e74 7269  -challenge/entri
+00023f00: 6573 3e60 5f2e 0a0a 2020 2020 5061 7261  es>`_...    Para
+00023f10: 6d65 7465 7273 0a20 2020 202d 2d2d 2d2d  meters.    -----
+00023f20: 2d2d 2d2d 2d0a 2020 2020 6c6f 6164 203a  -----.    load :
+00023f30: 2062 6f6f 6c2c 2064 6566 6175 6c74 3a20   bool, default: 
+00023f40: 5472 7565 0a20 2020 2020 2020 204c 6f61  True.        Loa
+00023f50: 6420 7468 6520 6461 7461 7365 7420 6166  d the dataset af
+00023f60: 7465 7220 646f 776e 6c6f 6164 696e 6720  ter downloading 
+00023f70: 6974 2077 6865 6e20 6060 5472 7565 6060  it when ``True``
+00023f80: 2e20 2053 6574 2074 6869 730a 2020 2020  .  Set this.    
+00023f90: 2020 2020 746f 2060 6046 616c 7365 6060      to ``False``
+00023fa0: 2061 6e64 206f 6e6c 7920 7468 6520 6669   and only the fi
+00023fb0: 6c65 6e61 6d65 2077 696c 6c20 6265 2072  lename will be r
+00023fc0: 6574 7572 6e65 642e 0a0a 2020 2020 5265  eturned...    Re
+00023fd0: 7475 726e 730a 2020 2020 2d2d 2d2d 2d2d  turns.    ------
+00023fe0: 2d0a 2020 2020 7079 7669 7374 612e 556e  -.    pyvista.Un
+00023ff0: 7374 7275 6374 7572 6564 4772 6964 207c  structuredGrid |
+00024000: 2073 7472 0a20 2020 2020 2020 2044 6174   str.        Dat
+00024010: 6153 6574 206f 7220 6669 6c65 6e61 6d65  aSet or filename
+00024020: 2064 6570 656e 6469 6e67 206f 6e20 6060   depending on ``
+00024030: 6c6f 6164 6060 2e0a 0a20 2020 2045 7861  load``...    Exa
+00024040: 6d70 6c65 730a 2020 2020 2d2d 2d2d 2d2d  mples.    ------
+00024050: 2d2d 0a20 2020 2044 6f77 6e6c 6f61 6420  --.    Download 
+00024060: 7468 6520 6165 726f 2062 7261 636b 6574  the aero bracket
+00024070: 2e0a 0a20 2020 203e 3e3e 2066 726f 6d20  ...    >>> from 
+00024080: 7079 7669 7374 6120 696d 706f 7274 2065  pyvista import e
+00024090: 7861 6d70 6c65 730a 2020 2020 3e3e 3e20  xamples.    >>> 
+000240a0: 6461 7461 7365 7420 3d20 6578 616d 706c  dataset = exampl
+000240b0: 6573 2e64 6f77 6e6c 6f61 645f 6165 726f  es.download_aero
+000240c0: 5f62 7261 636b 6574 2829 0a20 2020 203e  _bracket().    >
+000240d0: 3e3e 2064 6174 6173 6574 0a20 2020 2055  >> dataset.    U
+000240e0: 6e73 7472 7563 7475 7265 6447 7269 6420  nstructuredGrid 
+000240f0: 282e 2e2e 290a 2020 2020 2020 4e20 4365  (...).      N Ce
+00024100: 6c6c 733a 2020 2020 3131 3732 3932 0a20  lls:    117292. 
+00024110: 2020 2020 204e 2050 6f69 6e74 733a 2020       N Points:  
+00024120: 2031 3837 3033 370a 2020 2020 2020 5820   187037.      X 
+00024130: 426f 756e 6473 3a20 2020 2d36 2e38 3538  Bounds:   -6.858
+00024140: 652d 3033 2c20 312e 3131 3865 2d30 310a  e-03, 1.118e-01.
+00024150: 2020 2020 2020 5920 426f 756e 6473 3a20        Y Bounds: 
+00024160: 2020 2d31 2e32 3337 652d 3032 2c20 362e    -1.237e-02, 6.
+00024170: 3633 3465 2d30 320a 2020 2020 2020 5a20  634e-02.      Z 
+00024180: 426f 756e 6473 3a20 2020 2d31 2e36 3338  Bounds:   -1.638
+00024190: 652d 3032 2c20 312e 3633 3865 2d30 320a  e-02, 1.638e-02.
+000241a0: 2020 2020 2020 4e20 4172 7261 7973 3a20        N Arrays: 
+000241b0: 2020 330a 0a20 2020 2053 686f 7720 7468    3..    Show th
+000241c0: 6520 6176 6169 6c61 626c 6520 706f 696e  e available poin
+000241d0: 7420 6461 7461 2061 7272 6179 732e 0a0a  t data arrays...
+000241e0: 2020 2020 3e3e 3e20 6461 7461 7365 742e      >>> dataset.
+000241f0: 706f 696e 745f 6461 7461 0a20 2020 2070  point_data.    p
+00024200: 7976 6973 7461 2044 6174 6153 6574 4174  yvista DataSetAt
+00024210: 7472 6962 7574 6573 0a20 2020 2041 7373  tributes.    Ass
+00024220: 6f63 6961 7469 6f6e 2020 2020 203a 2050  ociation     : P
+00024230: 4f49 4e54 0a20 2020 2041 6374 6976 6520  OINT.    Active 
+00024240: 5363 616c 6172 7320 203a 204e 6f6e 650a  Scalars  : None.
+00024250: 2020 2020 4163 7469 7665 2056 6563 746f      Active Vecto
+00024260: 7273 2020 3a20 4e6f 6e65 0a20 2020 2041  rs  : None.    A
+00024270: 6374 6976 6520 5465 7874 7572 6520 203a  ctive Texture  :
+00024280: 204e 6f6e 650a 2020 2020 4163 7469 7665   None.    Active
+00024290: 204e 6f72 6d61 6c73 2020 3a20 4e6f 6e65   Normals  : None
+000242a0: 0a20 2020 2043 6f6e 7461 696e 7320 6172  .    Contains ar
+000242b0: 7261 7973 203a 0a20 2020 2020 2020 2064  rays :.        d
+000242c0: 6973 706c 6163 656d 656e 7420 2020 2020  isplacement     
+000242d0: 2020 2020 2020 2066 6c6f 6174 3332 2020         float32  
+000242e0: 2020 2831 3837 3033 372c 2033 290a 2020    (187037, 3).  
+000242f0: 2020 2020 2020 746f 7461 6c20 6e6f 6e6c        total nonl
+00024300: 696e 6561 7220 7374 7261 696e 2020 666c  inear strain  fl
+00024310: 6f61 7433 3220 2020 2028 3138 3730 3337  oat32    (187037
+00024320: 2c20 3629 0a20 2020 2020 2020 2076 6f6e  , 6).        von
+00024330: 204d 6973 6573 2073 7472 6573 7320 2020   Mises stress   
+00024340: 2020 2020 2066 6c6f 6174 3332 2020 2020       float32    
+00024350: 2831 3837 3033 372c 290a 0a20 2020 2050  (187037,)..    P
+00024360: 6c6f 7420 7468 6520 766f 6e20 4d69 7365  lot the von Mise
+00024370: 7320 7374 7265 7373 2e0a 0a20 2020 203e  s stress...    >
+00024380: 3e3e 2063 706f 7320 3d20 5b0a 2020 2020  >> cpos = [.    
+00024390: 2e2e 2e20 2020 2020 282d 302e 3035 3033  ...     (-0.0503
+000243a0: 2c20 302e 3133 322c 202d 302e 3137 3929  , 0.132, -0.179)
+000243b0: 2c0a 2020 2020 2e2e 2e20 2020 2020 2830  ,.    ...     (0
+000243c0: 2e30 3530 352c 2030 2e30 3138 352c 202d  .0505, 0.0185, -
+000243d0: 302e 3030 3230 3129 2c0a 2020 2020 2e2e  0.00201),.    ..
+000243e0: 2e20 2020 2020 2830 2e32 3735 2c20 302e  .     (0.275, 0.
+000243f0: 3837 322c 2030 2e34 3035 292c 0a20 2020  872, 0.405),.   
+00024400: 202e 2e2e 205d 0a20 2020 203e 3e3e 2064   ... ].    >>> d
+00024410: 6174 6173 6574 2e70 6c6f 7428 0a20 2020  ataset.plot(.   
+00024420: 202e 2e2e 2020 2020 2073 6d6f 6f74 685f   ...     smooth_
+00024430: 7368 6164 696e 673d 5472 7565 2c0a 2020  shading=True,.  
+00024440: 2020 2e2e 2e20 2020 2020 7370 6c69 745f    ...     split_
+00024450: 7368 6172 705f 6564 6765 733d 5472 7565  sharp_edges=True
+00024460: 2c0a 2020 2020 2e2e 2e20 2020 2020 7363  ,.    ...     sc
+00024470: 616c 6172 733d 2776 6f6e 204d 6973 6573  alars='von Mises
+00024480: 2073 7472 6573 7327 2c0a 2020 2020 2e2e   stress',.    ..
+00024490: 2e20 2020 2020 636d 6170 3d27 6277 7227  .     cmap='bwr'
+000244a0: 2c0a 2020 2020 2e2e 2e20 2020 2020 6370  ,.    ...     cp
+000244b0: 6f73 3d63 706f 732c 0a20 2020 202e 2e2e  os=cpos,.    ...
+000244c0: 2020 2020 2061 6e74 695f 616c 6961 7369       anti_aliasi
+000244d0: 6e67 3d27 6678 6161 272c 0a20 2020 202e  ng='fxaa',.    .
+000244e0: 2e2e 2029 0a0a 2020 2020 2222 220a 2020  .. )..    """.  
+000244f0: 2020 7265 7475 726e 205f 646f 776e 6c6f    return _downlo
+00024500: 6164 5f61 6e64 5f72 6561 6428 2766 6561  ad_and_read('fea
+00024510: 2f61 6572 6f5f 6272 6163 6b65 742f 6165  /aero_bracket/ae
+00024520: 726f 5f62 7261 636b 6574 2e76 7475 272c  ro_bracket.vtu',
+00024530: 206c 6f61 643d 6c6f 6164 290a 0a0a 6465   load=load)...de
+00024540: 6620 646f 776e 6c6f 6164 5f63 6f69 6c5f  f download_coil_
+00024550: 6d61 676e 6574 6963 5f66 6965 6c64 286c  magnetic_field(l
+00024560: 6f61 643d 5472 7565 293a 2020 2320 7072  oad=True):  # pr
+00024570: 6167 6d61 3a20 6e6f 2063 6f76 6572 0a20  agma: no cover. 
+00024580: 2020 2022 2222 446f 776e 6c6f 6164 2074     """Download t
+00024590: 6865 206d 6167 6e65 7469 6320 6669 656c  he magnetic fiel
+000245a0: 6420 6f66 2061 2063 6f69 6c2e 0a0a 2020  d of a coil...  
+000245b0: 2020 5468 6573 6520 6578 616d 706c 6573    These examples
+000245c0: 2077 6572 6520 6765 6e65 7261 7465 6420   were generated 
+000245d0: 6672 6f6d 2074 6865 2066 6f6c 6c6f 7769  from the followi
+000245e0: 6e67 2060 7363 7269 7074 0a20 2020 203c  ng `script.    <
+000245f0: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
+00024600: 6f6d 2f70 7976 6973 7461 2f76 746b 2d64  om/pyvista/vtk-d
+00024610: 6174 612f 7472 6565 2f6d 6173 7465 722f  ata/tree/master/
+00024620: 4461 7461 2f6d 6167 7079 6c69 622f 3e60  Data/magpylib/>`
+00024630: 5f2e 0a0a 2020 2020 5061 7261 6d65 7465  _...    Paramete
+00024640: 7273 0a20 2020 202d 2d2d 2d2d 2d2d 2d2d  rs.    ---------
+00024650: 2d0a 2020 2020 6c6f 6164 203a 2062 6f6f  -.    load : boo
+00024660: 6c2c 2064 6566 6175 6c74 3a20 5472 7565  l, default: True
+00024670: 0a20 2020 2020 2020 204c 6f61 6420 7468  .        Load th
+00024680: 6520 6461 7461 7365 7420 6166 7465 7220  e dataset after 
+00024690: 646f 776e 6c6f 6164 696e 6720 6974 2077  downloading it w
+000246a0: 6865 6e20 6060 5472 7565 6060 2e20 2053  hen ``True``.  S
+000246b0: 6574 2074 6869 730a 2020 2020 2020 2020  et this.        
+000246c0: 746f 2060 6046 616c 7365 6060 2061 6e64  to ``False`` and
+000246d0: 206f 6e6c 7920 7468 6520 6669 6c65 6e61   only the filena
+000246e0: 6d65 2077 696c 6c20 6265 2072 6574 7572  me will be retur
+000246f0: 6e65 642e 0a0a 2020 2020 5265 7475 726e  ned...    Return
+00024700: 730a 2020 2020 2d2d 2d2d 2d2d 2d0a 2020  s.    -------.  
+00024710: 2020 7079 7669 7374 612e 496d 6167 6544    pyvista.ImageD
+00024720: 6174 6120 6f72 2073 7472 0a20 2020 2020  ata or str.     
+00024730: 2020 2044 6174 6153 6574 206f 7220 6669     DataSet or fi
+00024740: 6c65 6e61 6d65 2064 6570 656e 6469 6e67  lename depending
+00024750: 206f 6e20 6060 6c6f 6164 6060 2e0a 0a20   on ``load``... 
+00024760: 2020 2045 7861 6d70 6c65 730a 2020 2020     Examples.    
+00024770: 2d2d 2d2d 2d2d 2d2d 0a20 2020 2044 6f77  --------.    Dow
+00024780: 6e6c 6f61 6420 7468 6520 6d61 676e 6574  nload the magnet
+00024790: 6963 2066 6965 6c64 2064 6174 6173 6574  ic field dataset
+000247a0: 2061 6e64 2067 656e 6572 6174 6520 7374   and generate st
+000247b0: 7265 616d 6c69 6e65 7320 6672 6f6d 2074  reamlines from t
+000247c0: 6865 2066 6965 6c64 2e0a 0a20 2020 203e  he field...    >
+000247d0: 3e3e 2069 6d70 6f72 7420 7079 7669 7374  >> import pyvist
+000247e0: 6120 6173 2070 760a 2020 2020 3e3e 3e20  a as pv.    >>> 
+000247f0: 6672 6f6d 2070 7976 6973 7461 2069 6d70  from pyvista imp
+00024800: 6f72 7420 6578 616d 706c 6573 0a20 2020  ort examples.   
+00024810: 203e 3e3e 2067 7269 6420 3d20 6578 616d   >>> grid = exam
+00024820: 706c 6573 2e64 6f77 6e6c 6f61 645f 636f  ples.download_co
+00024830: 696c 5f6d 6167 6e65 7469 635f 6669 656c  il_magnetic_fiel
+00024840: 6428 290a 2020 2020 3e3e 3e20 7365 6564  d().    >>> seed
+00024850: 203d 2070 762e 4469 7363 2869 6e6e 6572   = pv.Disc(inner
+00024860: 3d31 2c20 6f75 7465 723d 352e 322c 2072  =1, outer=5.2, r
+00024870: 5f72 6573 3d33 2c20 635f 7265 733d 3132  _res=3, c_res=12
+00024880: 290a 2020 2020 3e3e 3e20 7374 726c 203d  ).    >>> strl =
+00024890: 2067 7269 642e 7374 7265 616d 6c69 6e65   grid.streamline
+000248a0: 735f 6672 6f6d 5f73 6f75 7263 6528 0a20  s_from_source(. 
+000248b0: 2020 202e 2e2e 2020 2020 2073 6565 642c     ...     seed,
+000248c0: 0a20 2020 202e 2e2e 2020 2020 2076 6563  .    ...     vec
+000248d0: 746f 7273 3d27 4227 2c0a 2020 2020 2e2e  tors='B',.    ..
+000248e0: 2e20 2020 2020 6d61 785f 7469 6d65 3d31  .     max_time=1
+000248f0: 3830 2c0a 2020 2020 2e2e 2e20 2020 2020  80,.    ...     
+00024900: 696e 6974 6961 6c5f 7374 6570 5f6c 656e  initial_step_len
+00024910: 6774 683d 302e 312c 0a20 2020 202e 2e2e  gth=0.1,.    ...
+00024920: 2020 2020 2069 6e74 6567 7261 7469 6f6e       integration
+00024930: 5f64 6972 6563 7469 6f6e 3d27 626f 7468  _direction='both
+00024940: 272c 0a20 2020 202e 2e2e 2029 0a20 2020  ',.    ... ).   
+00024950: 203e 3e3e 2073 7472 6c2e 706c 6f74 280a   >>> strl.plot(.
+00024960: 2020 2020 2e2e 2e20 2020 2020 636d 6170      ...     cmap
+00024970: 3d27 706c 6173 6d61 272c 0a20 2020 202e  ='plasma',.    .
+00024980: 2e2e 2020 2020 2072 656e 6465 725f 6c69  ..     render_li
+00024990: 6e65 735f 6173 5f74 7562 6573 3d54 7275  nes_as_tubes=Tru
+000249a0: 652c 0a20 2020 202e 2e2e 2020 2020 206c  e,.    ...     l
+000249b0: 696e 655f 7769 6474 683d 322c 0a20 2020  ine_width=2,.   
+000249c0: 202e 2e2e 2020 2020 206c 6967 6874 696e   ...     lightin
+000249d0: 673d 4661 6c73 652c 0a20 2020 202e 2e2e  g=False,.    ...
+000249e0: 2020 2020 207a 6f6f 6d3d 322c 0a20 2020       zoom=2,.   
+000249f0: 202e 2e2e 2029 0a0a 2020 2020 506c 6f74   ... )..    Plot
+00024a00: 2074 6865 206d 6167 6e65 7420 6669 656c   the magnet fiel
+00024a10: 6420 7374 7265 6e67 7468 2069 6e20 7468  d strength in th
+00024a20: 6520 5a20 6469 7265 6374 696f 6e2e 0a0a  e Z direction...
+00024a30: 2020 2020 3e3e 3e20 696d 706f 7274 206e      >>> import n
+00024a40: 756d 7079 2061 7320 6e70 0a20 2020 203e  umpy as np.    >
+00024a50: 3e3e 2069 6d70 6f72 7420 7079 7669 7374  >> import pyvist
+00024a60: 6120 6173 2070 760a 2020 2020 3e3e 3e20  a as pv.    >>> 
+00024a70: 6672 6f6d 2070 7976 6973 7461 2069 6d70  from pyvista imp
+00024a80: 6f72 7420 6578 616d 706c 6573 0a20 2020  ort examples.   
+00024a90: 203e 3e3e 2067 7269 6420 3d20 6578 616d   >>> grid = exam
+00024aa0: 706c 6573 2e64 6f77 6e6c 6f61 645f 636f  ples.download_co
+00024ab0: 696c 5f6d 6167 6e65 7469 635f 6669 656c  il_magnetic_fiel
+00024ac0: 6428 290a 2020 2020 3e3e 3e20 2320 6372  d().    >>> # cr
+00024ad0: 6561 7465 2063 6f69 6c73 0a20 2020 203e  eate coils.    >
+00024ae0: 3e3e 2063 6f69 6c73 203d 205b 5d0a 2020  >> coils = [].  
+00024af0: 2020 3e3e 3e20 666f 7220 7a20 696e 206e    >>> for z in n
+00024b00: 702e 6c69 6e73 7061 6365 282d 382c 2038  p.linspace(-8, 8
+00024b10: 2c20 3136 293a 0a20 2020 202e 2e2e 2020  , 16):.    ...  
+00024b20: 2020 2063 6f69 6c73 2e61 7070 656e 6428     coils.append(
+00024b30: 0a20 2020 202e 2e2e 2020 2020 2020 2020  .    ...        
+00024b40: 2070 762e 506f 6c79 676f 6e28 2830 2c20   pv.Polygon((0, 
+00024b50: 302c 207a 292c 2072 6164 6975 733d 352c  0, z), radius=5,
+00024b60: 206e 5f73 6964 6573 3d31 3030 2c20 6669   n_sides=100, fi
+00024b70: 6c6c 3d46 616c 7365 290a 2020 2020 2e2e  ll=False).    ..
+00024b80: 2e20 2020 2020 290a 2020 2020 2e2e 2e0a  .     ).    ....
+00024b90: 2020 2020 3e3e 3e20 636f 696c 7320 3d20      >>> coils = 
+00024ba0: 7076 2e4d 756c 7469 426c 6f63 6b28 636f  pv.MultiBlock(co
+00024bb0: 696c 7329 0a20 2020 203e 3e3e 2023 2070  ils).    >>> # p
+00024bc0: 6c6f 7420 7468 6520 6d61 676e 6574 2066  lot the magnet f
+00024bd0: 6965 6c64 2073 7472 656e 6774 6820 696e  ield strength in
+00024be0: 2074 6865 205a 2064 6972 6563 7469 6f6e   the Z direction
+00024bf0: 0a20 2020 203e 3e3e 2073 6361 6c61 7273  .    >>> scalars
+00024c00: 203d 206e 702e 6162 7328 6772 6964 5b27   = np.abs(grid['
+00024c10: 4227 5d5b 3a2c 2032 5d29 0a20 2020 203e  B'][:, 2]).    >
+00024c20: 3e3e 2070 6c20 3d20 7076 2e50 6c6f 7474  >> pl = pv.Plott
+00024c30: 6572 2829 0a20 2020 203e 3e3e 205f 203d  er().    >>> _ =
+00024c40: 2070 6c2e 6164 645f 6d65 7368 280a 2020   pl.add_mesh(.  
+00024c50: 2020 2e2e 2e20 2020 2020 636f 696c 732c    ...     coils,
+00024c60: 2072 656e 6465 725f 6c69 6e65 735f 6173   render_lines_as
+00024c70: 5f74 7562 6573 3d54 7275 652c 206c 696e  _tubes=True, lin
+00024c80: 655f 7769 6474 683d 352c 2063 6f6c 6f72  e_width=5, color
+00024c90: 3d27 7727 0a20 2020 202e 2e2e 2029 0a20  ='w'.    ... ). 
+00024ca0: 2020 203e 3e3e 2076 6f6c 203d 2070 6c2e     >>> vol = pl.
+00024cb0: 6164 645f 766f 6c75 6d65 280a 2020 2020  add_volume(.    
+00024cc0: 2e2e 2e20 2020 2020 6772 6964 2c0a 2020  ...     grid,.  
+00024cd0: 2020 2e2e 2e20 2020 2020 7363 616c 6172    ...     scalar
+00024ce0: 733d 7363 616c 6172 732c 0a20 2020 202e  s=scalars,.    .
+00024cf0: 2e2e 2020 2020 2063 6d61 703d 2770 6c61  ..     cmap='pla
+00024d00: 736d 6127 2c0a 2020 2020 2e2e 2e20 2020  sma',.    ...   
+00024d10: 2020 7368 6f77 5f73 6361 6c61 725f 6261    show_scalar_ba
+00024d20: 723d 4661 6c73 652c 0a20 2020 202e 2e2e  r=False,.    ...
+00024d30: 2020 2020 206c 6f67 5f73 6361 6c65 3d54       log_scale=T
+00024d40: 7275 652c 0a20 2020 202e 2e2e 2020 2020  rue,.    ...    
+00024d50: 206f 7061 6369 7479 3d27 7369 676d 6f69   opacity='sigmoi
+00024d60: 645f 3227 2c0a 2020 2020 2e2e 2e20 290a  d_2',.    ... ).
+00024d70: 2020 2020 3e3e 3e20 766f 6c2e 7072 6f70      >>> vol.prop
+00024d80: 2e69 6e74 6572 706f 6c61 7469 6f6e 5f74  .interpolation_t
+00024d90: 7970 6520 3d20 276c 696e 6561 7227 0a20  ype = 'linear'. 
+00024da0: 2020 203e 3e3e 205f 203d 2070 6c2e 6164     >>> _ = pl.ad
+00024db0: 645f 766f 6c75 6d65 5f63 6c69 705f 706c  d_volume_clip_pl
+00024dc0: 616e 6528 0a20 2020 202e 2e2e 2020 2020  ane(.    ...    
+00024dd0: 2076 6f6c 2c0a 2020 2020 2e2e 2e20 2020   vol,.    ...   
+00024de0: 2020 6e6f 726d 616c 3d27 2d78 272c 0a20    normal='-x',. 
+00024df0: 2020 202e 2e2e 2020 2020 206e 6f72 6d61     ...     norma
+00024e00: 6c5f 726f 7461 7469 6f6e 3d46 616c 7365  l_rotation=False
+00024e10: 2c0a 2020 2020 2e2e 2e20 2020 2020 696e  ,.    ...     in
+00024e20: 7465 7261 6374 696f 6e5f 6576 656e 743d  teraction_event=
+00024e30: 2761 6c77 6179 7327 2c0a 2020 2020 2e2e  'always',.    ..
+00024e40: 2e20 2020 2020 7769 6467 6574 5f63 6f6c  .     widget_col
+00024e50: 6f72 3d70 762e 436f 6c6f 7228 6f70 6163  or=pv.Color(opac
+00024e60: 6974 793d 302e 3029 2c0a 2020 2020 2e2e  ity=0.0),.    ..
+00024e70: 2e20 290a 2020 2020 3e3e 3e20 706c 2e65  . ).    >>> pl.e
+00024e80: 6e61 626c 655f 616e 7469 5f61 6c69 6173  nable_anti_alias
+00024e90: 696e 6728 290a 2020 2020 3e3e 3e20 706c  ing().    >>> pl
+00024ea0: 2e63 616d 6572 612e 7a6f 6f6d 2832 290a  .camera.zoom(2).
+00024eb0: 2020 2020 3e3e 3e20 706c 2e73 686f 7728      >>> pl.show(
+00024ec0: 290a 0a20 2020 2053 6565 2074 6865 203a  )..    See the :
+00024ed0: 7265 663a 606d 6167 6e65 7469 635f 6669  ref:`magnetic_fi
+00024ee0: 656c 6473 5f65 7861 6d70 6c65 6020 666f  elds_example` fo
+00024ef0: 7220 6d6f 7265 2064 6574 6169 6c73 206f  r more details o
+00024f00: 6e20 686f 7720 746f 2070 6c6f 7420 7769  n how to plot wi
+00024f10: 7468 0a20 2020 2074 6869 7320 6461 7461  th.    this data
+00024f20: 7365 742e 0a0a 2020 2020 2222 220a 2020  set...    """.  
+00024f30: 2020 7265 7475 726e 205f 646f 776e 6c6f    return _downlo
+00024f40: 6164 5f61 6e64 5f72 6561 6428 276d 6167  ad_and_read('mag
+00024f50: 7079 6c69 622f 636f 696c 5f66 6965 6c64  pylib/coil_field
+00024f60: 2e76 7469 272c 206c 6f61 643d 6c6f 6164  .vti', load=load
+00024f70: 290a 0a0a 6465 6620 646f 776e 6c6f 6164  )...def download
+00024f80: 5f6d 6573 6869 6f5f 7864 6d66 286c 6f61  _meshio_xdmf(loa
+00024f90: 643d 5472 7565 293a 2020 2320 7072 6167  d=True):  # prag
+00024fa0: 6d61 3a20 6e6f 2063 6f76 6572 0a20 2020  ma: no cover.   
+00024fb0: 2022 2222 446f 776e 6c6f 6164 2078 646d   """Download xdm
+00024fc0: 6620 6669 6c65 2063 7265 6174 6564 2062  f file created b
+00024fd0: 7920 6d65 7368 696f 2e0a 0a20 2020 2054  y meshio...    T
+00024fe0: 6865 2064 6174 6173 6574 2077 6173 2063  he dataset was c
+00024ff0: 7265 6174 6564 2062 7920 6060 7465 7374  reated by ``test
+00025000: 5f74 696d 655f 7365 7269 6573 6060 2074  _time_series`` t
+00025010: 6573 7420 6675 6e63 7469 6f6e 2069 6e20  est function in 
+00025020: 6d65 7368 696f 2e0a 0a20 2020 2050 6172  meshio...    Par
+00025030: 616d 6574 6572 730a 2020 2020 2d2d 2d2d  ameters.    ----
+00025040: 2d2d 2d2d 2d2d 0a20 2020 206c 6f61 6420  ------.    load 
+00025050: 3a20 626f 6f6c 2c20 6465 6661 756c 743a  : bool, default:
+00025060: 2054 7275 650a 2020 2020 2020 2020 4c6f   True.        Lo
+00025070: 6164 2074 6865 2064 6174 6173 6574 2061  ad the dataset a
+00025080: 6674 6572 2064 6f77 6e6c 6f61 6469 6e67  fter downloading
+00025090: 2069 7420 7768 656e 2060 6054 7275 6560   it when ``True`
+000250a0: 602e 2020 5365 7420 7468 6973 0a20 2020  `.  Set this.   
+000250b0: 2020 2020 2074 6f20 6060 4661 6c73 6560       to ``False`
+000250c0: 6020 616e 6420 6f6e 6c79 2074 6865 2066  ` and only the f
+000250d0: 696c 656e 616d 6520 7769 6c6c 2062 6520  ilename will be 
+000250e0: 7265 7475 726e 6564 2e0a 0a20 2020 2052  returned...    R
+000250f0: 6574 7572 6e73 0a20 2020 202d 2d2d 2d2d  eturns.    -----
+00025100: 2d2d 0a20 2020 2070 7976 6973 7461 2e55  --.    pyvista.U
+00025110: 6e73 7472 7563 7475 7265 6447 7269 6420  nstructuredGrid 
+00025120: 6f72 2073 7472 0a20 2020 2020 2020 2044  or str.        D
+00025130: 6174 6153 6574 206f 7220 6669 6c65 6e61  ataSet or filena
+00025140: 6d65 2064 6570 656e 6469 6e67 206f 6e20  me depending on 
+00025150: 6060 6c6f 6164 6060 2e0a 0a20 2020 2045  ``load``...    E
+00025160: 7861 6d70 6c65 730a 2020 2020 2d2d 2d2d  xamples.    ----
+00025170: 2d2d 2d2d 0a20 2020 203e 3e3e 2066 726f  ----.    >>> fro
+00025180: 6d20 7079 7669 7374 6120 696d 706f 7274  m pyvista import
+00025190: 2065 7861 6d70 6c65 730a 2020 2020 3e3e   examples.    >>
+000251a0: 3e20 6461 7461 7365 7420 3d20 6578 616d  > dataset = exam
+000251b0: 706c 6573 2e64 6f77 6e6c 6f61 645f 6d65  ples.download_me
+000251c0: 7368 696f 5f78 646d 6628 290a 2020 2020  shio_xdmf().    
+000251d0: 3e3e 3e20 6461 7461 7365 742e 706c 6f74  >>> dataset.plot
+000251e0: 2829 0a0a 2020 2020 2222 220a 2020 2020  ()..    """.    
+000251f0: 5f20 3d20 646f 776e 6c6f 6164 5f66 696c  _ = download_fil
+00025200: 6528 226d 6573 6869 6f2f 6f75 742e 6835  e("meshio/out.h5
+00025210: 2229 0a20 2020 2072 6574 7572 6e20 5f64  ").    return _d
+00025220: 6f77 6e6c 6f61 645f 616e 645f 7265 6164  ownload_and_read
+00025230: 2822 6d65 7368 696f 2f6f 7574 2e78 646d  ("meshio/out.xdm
+00025240: 6622 2c20 6c6f 6164 3d6c 6f61 6429 0a0a  f", load=load)..
+00025250: 0a64 6566 2064 6f77 6e6c 6f61 645f 7669  .def download_vi
+00025260: 6374 6f72 6961 6e5f 676f 626c 6574 5f66  ctorian_goblet_f
+00025270: 6163 655f 696c 6c75 7369 6f6e 286c 6f61  ace_illusion(loa
+00025280: 643d 5472 7565 293a 2020 2320 7072 6167  d=True):  # prag
+00025290: 6d61 3a20 6e6f 2063 6f76 6572 0a20 2020  ma: no cover.   
+000252a0: 2022 2222 446f 776e 6c6f 6164 2056 6963   """Download Vic
+000252b0: 746f 7269 616e 2047 6f62 6c65 7420 6661  torian Goblet fa
+000252c0: 6365 2069 6c6c 7573 696f 6e2e 0a0a 2020  ce illusion...  
+000252d0: 2020 5468 6973 2069 7320 6120 7265 706c    This is a repl
+000252e0: 6963 6120 6f66 2061 2056 6963 746f 7269  ica of a Victori
+000252f0: 616e 2067 6f62 6c65 7420 7769 7468 2061  an goblet with a
+00025300: 6e20 6578 7465 726e 616c 2070 726f 6669  n external profi
+00025310: 6c65 0a20 2020 2077 6869 6368 2072 6573  le.    which res
+00025320: 656d 626c 6573 2074 6861 7420 6f66 2061  embles that of a
+00025330: 2066 6163 652e 0a0a 2020 2020 5061 7261   face...    Para
+00025340: 6d65 7465 7273 0a20 2020 202d 2d2d 2d2d  meters.    -----
+00025350: 2d2d 2d2d 2d0a 2020 2020 6c6f 6164 203a  -----.    load :
+00025360: 2062 6f6f 6c2c 2064 6566 6175 6c74 3a20   bool, default: 
+00025370: 5472 7565 0a20 2020 2020 2020 204c 6f61  True.        Loa
+00025380: 6420 7468 6520 6461 7461 7365 7420 6166  d the dataset af
+00025390: 7465 7220 646f 776e 6c6f 6164 696e 6720  ter downloading 
+000253a0: 6974 2077 6865 6e20 6060 5472 7565 6060  it when ``True``
+000253b0: 2e20 2053 6574 2074 6869 730a 2020 2020  .  Set this.    
+000253c0: 2020 2020 746f 2060 6046 616c 7365 6060      to ``False``
+000253d0: 2061 6e64 206f 6e6c 7920 7468 6520 6669   and only the fi
+000253e0: 6c65 6e61 6d65 2077 696c 6c20 6265 2072  lename will be r
+000253f0: 6574 7572 6e65 642e 0a0a 2020 2020 5265  eturned...    Re
+00025400: 7475 726e 730a 2020 2020 2d2d 2d2d 2d2d  turns.    ------
+00025410: 2d0a 2020 2020 7079 7669 7374 612e 556e  -.    pyvista.Un
+00025420: 7374 7275 6374 7572 6564 4772 6964 206f  structuredGrid o
+00025430: 7220 7374 720a 2020 2020 2020 2020 4461  r str.        Da
+00025440: 7461 5365 7420 6f72 2066 696c 656e 616d  taSet or filenam
+00025450: 6520 6465 7065 6e64 696e 6720 6f6e 2060  e depending on `
+00025460: 606c 6f61 6460 602e 0a0a 2020 2020 4578  `load``...    Ex
+00025470: 616d 706c 6573 0a20 2020 202d 2d2d 2d2d  amples.    -----
+00025480: 2d2d 2d0a 2020 2020 3e3e 3e20 6672 6f6d  ---.    >>> from
+00025490: 2070 7976 6973 7461 2069 6d70 6f72 7420   pyvista import 
+000254a0: 6578 616d 706c 6573 0a20 2020 203e 3e3e  examples.    >>>
+000254b0: 2069 6d70 6f72 7420 7079 7669 7374 6120   import pyvista 
+000254c0: 6173 2070 760a 2020 2020 3e3e 3e20 6d65  as pv.    >>> me
+000254d0: 7368 203d 2065 7861 6d70 6c65 732e 646f  sh = examples.do
+000254e0: 776e 6c6f 6164 5f76 6963 746f 7269 616e  wnload_victorian
+000254f0: 5f67 6f62 6c65 745f 6661 6365 5f69 6c6c  _goblet_face_ill
+00025500: 7573 696f 6e28 290a 2020 2020 3e3e 3e20  usion().    >>> 
+00025510: 706c 6f74 7465 7220 3d20 7076 2e50 6c6f  plotter = pv.Plo
+00025520: 7474 6572 286c 6967 6874 696e 673d 276e  tter(lighting='n
+00025530: 6f6e 6527 290a 2020 2020 3e3e 3e20 5f20  one').    >>> _ 
+00025540: 3d20 706c 6f74 7465 722e 6164 645f 6d65  = plotter.add_me
+00025550: 7368 280a 2020 2020 2e2e 2e20 2020 2020  sh(.    ...     
+00025560: 6d65 7368 2c20 6564 6765 5f63 6f6c 6f72  mesh, edge_color
+00025570: 3d27 6772 6179 272c 2063 6f6c 6f72 3d27  ='gray', color='
+00025580: 7768 6974 6527 2c20 7368 6f77 5f65 6467  white', show_edg
+00025590: 6573 3d54 7275 650a 2020 2020 2e2e 2e20  es=True.    ... 
+000255a0: 290a 2020 2020 3e3e 3e20 5f20 3d20 706c  ).    >>> _ = pl
+000255b0: 6f74 7465 722e 6164 645f 666c 6f6f 7228  otter.add_floor(
+000255c0: 272d 7827 2c20 636f 6c6f 723d 2262 6c61  '-x', color="bla
+000255d0: 636b 2229 0a20 2020 203e 3e3e 2070 6c6f  ck").    >>> plo
+000255e0: 7474 6572 2e65 6e61 626c 655f 7061 7261  tter.enable_para
+000255f0: 6c6c 656c 5f70 726f 6a65 6374 696f 6e28  llel_projection(
+00025600: 290a 2020 2020 3e3e 3e20 706c 6f74 7465  ).    >>> plotte
+00025610: 722e 7368 6f77 2863 706f 733d 2279 7a22  r.show(cpos="yz"
+00025620: 290a 0a20 2020 2022 2222 0a20 2020 2072  )..    """.    r
+00025630: 6574 7572 6e20 5f64 6f77 6e6c 6f61 645f  eturn _download_
+00025640: 616e 645f 7265 6164 2827 5669 6374 6f72  and_read('Victor
+00025650: 6961 6e5f 476f 626c 6574 5f66 6163 655f  ian_Goblet_face_
+00025660: 696c 6c75 7369 6f6e 2f56 6173 652e 7374  illusion/Vase.st
+00025670: 6c27 2c20 6c6f 6164 3d6c 6f61 6429 0a    l', load=load).
```

### Comparing `pyvista-0.43.7/pyvista/examples/examples.py` & `pyvista-0.44.dev0/pyvista/examples/examples.py`

 * *Files identical despite different names*

### Comparing `pyvista-0.43.7/pyvista/examples/globe.vtk` & `pyvista-0.44.dev0/pyvista/examples/globe.vtk`

 * *Files identical despite different names*

### Comparing `pyvista-0.43.7/pyvista/examples/gltf.py` & `pyvista-0.44.dev0/pyvista/examples/gltf.py`

 * *Files identical despite different names*

### Comparing `pyvista-0.43.7/pyvista/examples/hexbeam.vtk` & `pyvista-0.44.dev0/pyvista/examples/hexbeam.vtk`

 * *Files identical despite different names*

### Comparing `pyvista-0.43.7/pyvista/examples/nut.ply` & `pyvista-0.44.dev0/pyvista/examples/nut.ply`

 * *Files identical despite different names*

### Comparing `pyvista-0.43.7/pyvista/examples/planets.py` & `pyvista-0.44.dev0/pyvista/examples/planets.py`

 * *Files identical despite different names*

### Comparing `pyvista-0.43.7/pyvista/examples/pyvista_logo.png` & `pyvista-0.44.dev0/pyvista/examples/pyvista_logo.png`

 * *Files identical despite different names*

### Comparing `pyvista-0.43.7/pyvista/examples/rectilinear.vtk` & `pyvista-0.44.dev0/pyvista/examples/rectilinear.vtk`

 * *Files identical despite different names*

### Comparing `pyvista-0.43.7/pyvista/examples/sphere.ply` & `pyvista-0.44.dev0/pyvista/examples/sphere.ply`

 * *Files identical despite different names*

### Comparing `pyvista-0.43.7/pyvista/examples/uniform.vtk` & `pyvista-0.44.dev0/pyvista/examples/uniform.vtk`

 * *Files identical despite different names*

### Comparing `pyvista-0.43.7/pyvista/examples/vrml.py` & `pyvista-0.44.dev0/pyvista/examples/vrml.py`

 * *Files identical despite different names*

### Comparing `pyvista-0.43.7/pyvista/ext/coverage.py` & `pyvista-0.44.dev0/pyvista/ext/coverage.py`

 * *Files identical despite different names*

### Comparing `pyvista-0.43.7/pyvista/ext/plot_directive.py` & `pyvista-0.44.dev0/pyvista/ext/plot_directive.py`

 * *Files identical despite different names*

### Comparing `pyvista-0.43.7/pyvista/ext/viewer_directive.py` & `pyvista-0.44.dev0/pyvista/ext/viewer_directive.py`

 * *Files identical despite different names*

### Comparing `pyvista-0.43.7/pyvista/jupyter/__init__.py` & `pyvista-0.44.dev0/pyvista/jupyter/__init__.py`

 * *Files identical despite different names*

### Comparing `pyvista-0.43.7/pyvista/jupyter/notebook.py` & `pyvista-0.44.dev0/pyvista/jupyter/notebook.py`

 * *Files identical despite different names*

### Comparing `pyvista-0.43.7/pyvista/plotting/__init__.py` & `pyvista-0.44.dev0/pyvista/plotting/__init__.py`

 * *Files identical despite different names*

### Comparing `pyvista-0.43.7/pyvista/plotting/_plotting.py` & `pyvista-0.44.dev0/pyvista/plotting/_plotting.py`

 * *Files identical despite different names*

### Comparing `pyvista-0.43.7/pyvista/plotting/_property.py` & `pyvista-0.44.dev0/pyvista/plotting/_property.py`

 * *Files identical despite different names*

### Comparing `pyvista-0.43.7/pyvista/plotting/_typing.py` & `pyvista-0.44.dev0/pyvista/plotting/_typing.py`

 * *Files identical despite different names*

### Comparing `pyvista-0.43.7/pyvista/plotting/_vtk.py` & `pyvista-0.44.dev0/pyvista/plotting/_vtk.py`

 * *Files identical despite different names*

### Comparing `pyvista-0.43.7/pyvista/plotting/_vtk_gl.py` & `pyvista-0.44.dev0/pyvista/plotting/_vtk_gl.py`

 * *Files identical despite different names*

### Comparing `pyvista-0.43.7/pyvista/plotting/actor.py` & `pyvista-0.44.dev0/pyvista/plotting/actor.py`

 * *Files 0% similar despite different names*

```diff
@@ -81,16 +81,14 @@
     def __init__(self, mapper=None, prop=None, name=None):
         """Initialize actor."""
         super().__init__()
         if mapper is not None:
             self.mapper = mapper
         if prop is None:
             self.prop = Property()
-        else:
-            self.prop = prop
         self._name = name
 
     @property
     def name(self) -> str:  # numpydoc ignore=RT01
         """Get or set the unique name identifier used by PyVista."""
         if self._name is None:
             self._name = f'{type(self).__name__}({self.memory_address})'
```

### Comparing `pyvista-0.43.7/pyvista/plotting/actor_properties.py` & `pyvista-0.44.dev0/pyvista/plotting/actor_properties.py`

 * *Files identical despite different names*

### Comparing `pyvista-0.43.7/pyvista/plotting/affine_widget.py` & `pyvista-0.44.dev0/pyvista/plotting/affine_widget.py`

 * *Files identical despite different names*

### Comparing `pyvista-0.43.7/pyvista/plotting/axes.py` & `pyvista-0.44.dev0/pyvista/plotting/axes.py`

 * *Files identical despite different names*

### Comparing `pyvista-0.43.7/pyvista/plotting/axes_actor.py` & `pyvista-0.44.dev0/pyvista/plotting/axes_actor.py`

 * *Files identical despite different names*

### Comparing `pyvista-0.43.7/pyvista/plotting/background_renderer.py` & `pyvista-0.44.dev0/pyvista/plotting/background_renderer.py`

 * *Files identical despite different names*

### Comparing `pyvista-0.43.7/pyvista/plotting/camera.py` & `pyvista-0.44.dev0/pyvista/plotting/camera.py`

 * *Files identical despite different names*

### Comparing `pyvista-0.43.7/pyvista/plotting/charts.py` & `pyvista-0.44.dev0/pyvista/plotting/charts.py`

 * *Files identical despite different names*

### Comparing `pyvista-0.43.7/pyvista/plotting/colors.py` & `pyvista-0.44.dev0/pyvista/plotting/colors.py`

 * *Files identical despite different names*

### Comparing `pyvista-0.43.7/pyvista/plotting/composite_mapper.py` & `pyvista-0.44.dev0/pyvista/plotting/composite_mapper.py`

 * *Files identical despite different names*

### Comparing `pyvista-0.43.7/pyvista/plotting/cube_axes_actor.py` & `pyvista-0.44.dev0/pyvista/plotting/cube_axes_actor.py`

 * *Files 1% similar despite different names*

```diff
@@ -251,35 +251,32 @@
     def x_axis_range(self) -> Tuple[float, float]:  # numpydoc ignore=RT01
         """Return or set the X axis range."""
         return self.GetXAxisRange()
 
     @x_axis_range.setter
     def x_axis_range(self, value: Tuple[float, float]):  # numpydoc ignore=GL08
         self.SetXAxisRange(value)
-        self._update_x_labels()
 
     @property
     def y_axis_range(self) -> Tuple[float, float]:  # numpydoc ignore=RT01
         """Return or set the Y axis range."""
         return self.GetYAxisRange()
 
     @y_axis_range.setter
     def y_axis_range(self, value: Tuple[float, float]):  # numpydoc ignore=GL08
         self.SetYAxisRange(value)
-        self._update_y_labels()
 
     @property
     def z_axis_range(self) -> Tuple[float, float]:  # numpydoc ignore=RT01
         """Return or set the Z axis range."""
         return self.GetZAxisRange()
 
     @z_axis_range.setter
     def z_axis_range(self, value: Tuple[float, float]):  # numpydoc ignore=GL08
         self.SetZAxisRange(value)
-        self._update_z_labels()
 
     @property
     def label_offset(self) -> float:  # numpydoc ignore=RT01
         """Return or set the distance between labels and the axis."""
         return self.GetLabelOffset()
 
     @label_offset.setter
@@ -498,43 +495,43 @@
 
     def _update_x_labels(self):
         """Regenerate X axis labels."""
         if self.x_axis_visibility:
             self.SetXTitle(self._x_title)
             if self._x_label_visibility:
                 self.SetAxisLabels(
-                    0, make_axis_labels(*self.x_axis_range, self.n_xlabels, self.x_label_format)
+                    0, make_axis_labels(*self.bounds[0:2], self.n_xlabels, self.x_label_format)
                 )
             else:
                 self.SetAxisLabels(0, self._empty_str)
         else:
             self.SetXTitle('')
             self.SetAxisLabels(0, self._empty_str)
 
     def _update_y_labels(self):
         """Regenerate Y axis labels."""
         if self.y_axis_visibility:
             self.SetYTitle(self._y_title)
             if self._y_label_visibility:
                 self.SetAxisLabels(
-                    1, make_axis_labels(*self.y_axis_range, self.n_ylabels, self.y_label_format)
+                    1, make_axis_labels(*self.bounds[2:4], self.n_ylabels, self.y_label_format)
                 )
             else:
                 self.SetAxisLabels(1, self._empty_str)
         else:
             self.SetYTitle('')
             self.SetAxisLabels(1, self._empty_str)
 
     def _update_z_labels(self):
         """Regenerate Z axis labels."""
         if self.z_axis_visibility:
             self.SetZTitle(self._z_title)
             if self._z_label_visibility:
                 self.SetAxisLabels(
-                    2, make_axis_labels(*self.z_axis_range, self.n_zlabels, self.z_label_format)
+                    2, make_axis_labels(*self.bounds[4:6], self.n_zlabels, self.z_label_format)
                 )
             else:
                 self.SetAxisLabels(2, self._empty_str)
         else:
             self.SetZTitle('')
             self.SetAxisLabels(2, self._empty_str)
```

### Comparing `pyvista-0.43.7/pyvista/plotting/errors.py` & `pyvista-0.44.dev0/pyvista/plotting/errors.py`

 * *Files identical despite different names*

### Comparing `pyvista-0.43.7/pyvista/plotting/helpers.py` & `pyvista-0.44.dev0/pyvista/plotting/helpers.py`

 * *Files 6% similar despite different names*

```diff
@@ -34,24 +34,24 @@
 
     Examples
     --------
     Plot a single random arrow.
 
     >>> import numpy as np
     >>> import pyvista as pv
-    >>> cent = np.random.random(3)
-    >>> direction = np.random.random(3)
+    >>> cent = np.random.default_rng().random(3)
+    >>> direction = np.random.default_rng().random(3)
     >>> pv.plot_arrows(cent, direction)
 
     Plot 100 random arrows.
 
     >>> import numpy as np
     >>> import pyvista as pv
-    >>> cent = np.random.random((100, 3))
-    >>> direction = np.random.random((100, 3))
+    >>> cent = np.random.default_rng().random((100, 3))
+    >>> direction = np.random.default_rng().random((100, 3))
     >>> pv.plot_arrows(cent, direction)
 
     """
     return pyvista.plot([cent, direction], **kwargs)
 
 
 def plot_compare_four(
```

### Comparing `pyvista-0.43.7/pyvista/plotting/lights.py` & `pyvista-0.44.dev0/pyvista/plotting/lights.py`

 * *Files identical despite different names*

### Comparing `pyvista-0.43.7/pyvista/plotting/lookup_table.py` & `pyvista-0.44.dev0/pyvista/plotting/lookup_table.py`

 * *Files identical despite different names*

### Comparing `pyvista-0.43.7/pyvista/plotting/mapper.py` & `pyvista-0.44.dev0/pyvista/plotting/mapper.py`

 * *Files 2% similar despite different names*

```diff
@@ -853,14 +853,63 @@
         """
         return self.GetScaleFactor()
 
     @scale_factor.setter
     def scale_factor(self, value: float):  # numpydoc ignore=GL08
         return self.SetScaleFactor(value)
 
+    @property
+    def scale_array(self) -> str:  # numpydoc ignore=RT01
+        """Set or return the name of the array used to scale the splats.
+
+        Scalars used to scale the gaussian points. Accepts a string
+        name of an array that is present on the mesh.
+
+        Notes
+        -----
+        Setting this automatically sets ``scale_factor = 1.0``.
+
+        Examples
+        --------
+        Plot spheres using `style='points_gaussian'` style and scale them by
+        radius.
+
+        >>> import numpy as np
+        >>> import pyvista as pv
+        >>> n_spheres = 1_000
+        >>> pos = np.random.random((n_spheres, 3))
+        >>> rad = np.random.random(n_spheres) * 0.01
+        >>> pdata = pv.PolyData(pos)
+        >>> pdata['radius'] = rad
+        >>> pl = pv.Plotter()
+        >>> actor = pl.add_mesh(
+        ...     pdata,
+        ...     style='points_gaussian',
+        ...     emissive=False,
+        ...     render_points_as_spheres=True,
+        ... )
+        >>> actor.mapper.scale_array = 'radius'
+        >>> pl.show()
+        """
+        return self.GetScaleArray()
+
+    @scale_array.setter
+    def scale_array(self, name: str):  # numpydoc ignore=GL08
+        if not self.dataset:  # pragma: no cover
+            raise RuntimeError('Missing dataset.')
+        if name not in self.dataset.point_data:
+            available_arrays = ", ".join(self.dataset.point_data.keys())
+            raise KeyError(
+                f'Point array "{name}" does not exist. '
+                f'Available point arrays are: {available_arrays}'
+            )
+
+        self.scale_factor = 1.0
+        return self.SetScaleArray(name)
+
     def use_circular_splat(self, opacity: float = 1.0):
         """Set the fragment shader code to create a circular splat.
 
         Parameters
         ----------
         opacity : float, default: 1.0
             Desired opacity between 0 and 1.
@@ -878,15 +927,14 @@
             "} else {\n"
             f"  float scale = ({opacity} - dist);\n"
             "  ambientColor *= scale;\n"
             "  diffuseColor *= scale;\n"
             "}\n"
         )
         # maintain consistency with the default style
-        self.emissive = True
         self.scale_factor *= 1.5
 
     def use_default_splat(self):
         """Clear the fragment shader and use the default splat."""
         self.SetSplatShaderCode(None)
         self.scale_factor /= 1.5
```

### Comparing `pyvista-0.43.7/pyvista/plotting/opts.py` & `pyvista-0.44.dev0/pyvista/plotting/opts.py`

 * *Files identical despite different names*

### Comparing `pyvista-0.43.7/pyvista/plotting/picking.py` & `pyvista-0.44.dev0/pyvista/plotting/picking.py`

 * *Files identical despite different names*

### Comparing `pyvista-0.43.7/pyvista/plotting/plotter.py` & `pyvista-0.44.dev0/pyvista/plotting/plotter.py`

 * *Files 1% similar despite different names*

```diff
@@ -61,15 +61,15 @@
 from .render_window_interactor import RenderWindowInteractor
 from .renderer import Camera, Renderer
 from .renderers import Renderers
 from .scalar_bars import ScalarBars
 from .text import CornerAnnotation, Text, TextProperty
 from .texture import numpy_to_texture
 from .themes import Theme
-from .tools import normalize, opacity_transfer_function, parse_font_family  # noqa
+from .tools import normalize, opacity_transfer_function, parse_font_family  # noqa: F401
 from .utilities.algorithms import (
     active_scalars_algorithm,
     algorithm_to_mesh_handler,
     decimation_algorithm,
     extract_surface_algorithm,
     pointset_to_polydata_algorithm,
     set_algorithm_input,
@@ -634,15 +634,15 @@
 
         Examples
         --------
         Output a simple point cloud represented as balls.
 
         >>> import numpy as np
         >>> import pyvista as pv
-        >>> point_cloud = np.random.random((100, 3))
+        >>> point_cloud = np.random.default_rng().random((100, 3))
         >>> pdata = pv.PolyData(point_cloud)
         >>> pdata['orig_sphere'] = np.arange(100)
         >>> sphere = pv.Sphere(radius=0.02)
         >>> pc = pdata.glyph(scale=False, geom=sphere, orient=False)
         >>> pl = pv.Plotter()
         >>> _ = pl.add_mesh(
         ...     pc,
@@ -2007,15 +2007,15 @@
 
     @pickable_actors.setter
     def pickable_actors(self, actors=None):  # numpydoc ignore=GL08
         actors = [] if actors is None else actors
         if isinstance(actors, _vtk.vtkActor):
             actors = [actors]
 
-        if not all([isinstance(actor, _vtk.vtkActor) for actor in actors]):
+        if not all(isinstance(actor, _vtk.vtkActor) for actor in actors):
             raise TypeError(
                 f'Expected a vtkActor instance or a list of vtkActors, got '
                 f'{[type(actor) for actor in actors]} instead.'
             )
 
         for renderer in self.renderers:
             for actor in renderer.actors.values():
@@ -2150,14 +2150,19 @@
         self.iren.enable_rubber_band_style()
 
     @wraps(RenderWindowInteractor.enable_rubber_band_2d_style)
     def enable_rubber_band_2d_style(self):  # numpydoc ignore=PR01,RT01
         """Wrap RenderWindowInteractor.enable_rubber_band_2d_style."""
         self.iren.enable_rubber_band_2d_style()
 
+    @wraps(RenderWindowInteractor.enable_2d_style)
+    def enable_2d_style(self):  # numpydoc ignore=PR01,RT01
+        """Wrap RenderWindowInteractor.enable_2d_style."""
+        self.iren.enable_2d_style()
+
     def enable_stereo_render(self):
         """Enable anaglyph stereo rendering.
 
         Disable this with :func:`disable_stereo_render
         <Plotter.disable_stereo_render>`
 
         Examples
@@ -2696,15 +2701,15 @@
         self.mapper = CompositePolyDataMapper(
             dataset,
             theme=self._theme,
             color_missing_with_nan=color_missing_with_nan,
             interpolate_before_map=interpolate_before_map,
         )
 
-        actor, _ = self.add_actor(self.mapper, render=False)
+        actor, _ = self.add_actor(self.mapper)
 
         prop = Property(
             self._theme,
             interpolation=interpolation,
             metallic=metallic,
             roughness=roughness,
             point_size=point_size,
@@ -3295,14 +3300,27 @@
         ...     style='points_gaussian',
         ...     opacity=0.5,
         ...     point_size=10,
         ...     render_points_as_spheres=False,
         ...     show_scalar_bar=False,
         ... )
 
+        Plot spheres using `points_gaussian` style and scale them by radius.
+
+        >>> N_SPHERES = 1_000_000
+        >>> pos = np.random.random((N_SPHERES, 3))
+        >>> rad = np.random.random(N_SPHERES) * 0.01
+        >>> pdata = pv.PolyData(pos)
+        >>> pdata['radius'] = rad
+        >>> pdata.plot(
+        ...     style='points_gaussian',
+        ...     emissive=False,
+        ...     render_points_as_spheres=True,
+        ... )
+
         """
         if style == 'points_gaussian':
             self.mapper = PointGaussianMapper(theme=self.theme, emissive=emissive)
         else:
             self.mapper = DataSetMapper(theme=self.theme)
 
         if render_lines_as_tubes and show_edges:
@@ -3473,20 +3491,14 @@
 
             # Set the active scalars name here. If the name already exists in
             # the input mesh, it may not be set as the active scalars within
             # the mapper. This should be refactored by 0.36.0
             field = get_array_association(mesh, original_scalar_name, preference=preference)
             self.mapper.scalar_map_mode = field.name
 
-            # set preference for downstream use with actual
-            if field == FieldAssociation.POINT:
-                preference = 'point'
-            elif field == FieldAssociation.CELL:
-                preference = 'cell'
-
             if algo is not None:
                 # Ensures that the right scalars are set as active on
                 # each pipeline request
                 algo = active_scalars_algorithm(algo, original_scalar_name, preference=preference)
                 mesh, algo = algorithm_to_mesh_handler(algo)
             else:
                 # Otherwise, make sure the mesh object's scalars are set
@@ -5495,21 +5507,23 @@
             label_mapper.SetStyleToFilled()
         else:
             label_mapper.SetStyleToOutline()
         label_mapper.SetBackgroundColor(Color(shape_color).float_rgb)
         label_mapper.SetBackgroundOpacity(shape_opacity)
         label_mapper.SetMargin(margin)
 
-        textprop = hier.GetTextProperty()
-        textprop.SetItalic(italic)
-        textprop.SetBold(bold)
-        textprop.SetFontSize(font_size)
-        textprop.SetFontFamily(parse_font_family(font_family))
-        textprop.SetColor(Color(text_color, default_color=self._theme.font.color).float_rgb)
-        textprop.SetShadow(shadow)
+        text_property = pyvista.TextProperty(
+            italic=italic,
+            bold=bold,
+            font_size=font_size,
+            font_family=font_family,
+            color=text_color,
+            shadow=shadow,
+        )
+        hier.SetTextProperty(text_property)
 
         self.remove_actor(f'{name}-points', reset_camera=False)
         self.remove_actor(f'{name}-labels', reset_camera=False)
 
         # add points
         if show_points:
             self.add_mesh(
@@ -5602,24 +5616,24 @@
 
         Examples
         --------
         Add a numpy array of points to a mesh.
 
         >>> import numpy as np
         >>> import pyvista as pv
-        >>> points = np.random.random((10, 3))
+        >>> points = np.random.default_rng().random((10, 3))
         >>> pl = pv.Plotter()
         >>> actor = pl.add_points(
         ...     points, render_points_as_spheres=True, point_size=100.0
         ... )
         >>> pl.show()
 
         Plot using the ``'points_gaussian'`` style
 
-        >>> points = np.random.random((10, 3))
+        >>> points = np.random.default_rng().random((10, 3))
         >>> pl = pv.Plotter()
         >>> actor = pl.add_points(points, style='points_gaussian')
         >>> pl.show()
 
         """
         if style not in ['points', 'points_gaussian']:
             raise ValueError(
@@ -5653,16 +5667,16 @@
 
         Examples
         --------
         Plot a random field of vectors and save a screenshot of it.
 
         >>> import numpy as np
         >>> import pyvista as pv
-        >>> cent = np.random.random((10, 3))
-        >>> direction = np.random.random((10, 3))
+        >>> cent = np.random.default_rng().random((10, 3))
+        >>> direction = np.random.default_rng().random((10, 3))
         >>> plotter = pv.Plotter()
         >>> _ = plotter.add_arrows(cent, direction, mag=2)
         >>> plotter.show()
 
         """
         if cent.shape != direction.shape:  # pragma: no cover
             raise ValueError('center and direction arrays must have the same shape')
```

### Comparing `pyvista-0.43.7/pyvista/plotting/plotting/__init__.py` & `pyvista-0.44.dev0/pyvista/plotting/plotting/__init__.py`

 * *Files identical despite different names*

### Comparing `pyvista-0.43.7/pyvista/plotting/prop3d.py` & `pyvista-0.44.dev0/pyvista/plotting/prop3d.py`

 * *Files identical despite different names*

### Comparing `pyvista-0.43.7/pyvista/plotting/render_passes.py` & `pyvista-0.44.dev0/pyvista/plotting/render_passes.py`

 * *Files identical despite different names*

### Comparing `pyvista-0.43.7/pyvista/plotting/render_window_interactor.py` & `pyvista-0.44.dev0/pyvista/plotting/render_window_interactor.py`

 * *Files 9% similar despite different names*

```diff
@@ -543,14 +543,115 @@
         >>> plotter.show()  # doctest:+SKIP
 
         """
         self._style = 'TrackballCamera'
         self._style_class = None
         self.update_style()
 
+    def enable_2d_style(self):
+        """Set the interactive style to 2D.
+
+        For a 3-button mouse, the left button pans, the
+        right button dollys, the middle button spins, and the wheel
+        dollys.
+        ctrl + left button spins, shift + left button dollys,
+        ctrl + middle button pans, shift + middle button dollys,
+        ctrl + right button rotates in 3D, and shift + right button
+        dollys.
+
+        Recommended to use with
+        :func:`pyvista.Plotter.enable_parallel_projection`.
+
+        Examples
+        --------
+        Create a simple scene with a plotter that has the
+        ParaView-like 2D style:
+
+        >>> import pyvista as pv
+        >>> plotter = pv.Plotter()
+        >>> _ = plotter.add_mesh(pv.Cube(center=(1, 0, 0)))
+        >>> _ = plotter.add_mesh(pv.Cube(center=(0, 1, 0)))
+        >>> plotter.show_axes()
+        >>> plotter.enable_parallel_projection()
+        >>> plotter.enable_2d_style()
+        >>> plotter.show()  # doctest:+SKIP
+        """
+        self._style = 'TrackballCamera'
+        self._style_class = None
+        self.update_style()
+
+        def _left_button_press_callback(_obj, event):  # pragma: no cover
+            """Left button press behavior."""
+            if self.interactor.GetControlKey():
+                self._style_class.StartSpin()
+            elif self.interactor.GetShiftKey():
+                self._style_class.StartDolly()
+            else:
+                self._style_class.StartPan()
+            self._style_class.OnLeftButtonDown()
+
+        def _left_button_release_callback(_obj, event):  # pragma: no cover
+            """Turn off all left button behavior."""
+            self._style_class.EndSpin()
+            self._style_class.EndPan()
+            self._style_class.EndDolly()
+            self._style_class.OnLeftButtonUp()
+
+        def _middle_button_press_callback(_obj, event):  # pragma: no cover
+            """Middle button press behavior."""
+            if self.interactor.GetControlKey():
+                self._style_class.StartPan()
+            elif self.interactor.GetShiftKey():
+                self._style_class.StartDolly()
+            else:
+                self._style_class.StartSpin()
+            self._style_class.OnMiddleButtonDown()
+
+        def _middle_button_release_callback(_obj, event):  # pragma: no cover
+            """Turn off all middle button behavior."""
+            self._style_class.EndSpin()
+            self._style_class.EndPan()
+            self._style_class.EndDolly()
+            self._style_class.OnMiddleButtonUp()
+
+        def _right_button_press_callback(_obj, event):  # pragma: no cover
+            """Right button press behavior."""
+            if self.interactor.GetControlKey():
+                self._style_class.StartRotate()
+            elif self.interactor.GetShiftKey():
+                # https://github.com/pyvista/pyvista/pull/5336#discussion_r1426060132
+                self._style_class.StartDolly()  # ParaView does a different type of zooming
+            else:
+                self._style_class.StartDolly()
+            self._style_class.OnRightButtonDown()
+
+        def _right_button_release_callback(_obj, event):  # pragma: no cover
+            """Turn off all right button behavior."""
+            self._style_class.EndRotate()
+            self._style_class.EndDolly()
+            self._style_class.OnRightButtonUp()
+
+        callback = partial(try_callback, _left_button_press_callback)
+        self._style_class.add_observer('LeftButtonPressEvent', callback)
+
+        callback = partial(try_callback, _left_button_release_callback)
+        self._style_class.add_observer('LeftButtonReleaseEvent', callback)
+
+        callback = partial(try_callback, _middle_button_press_callback)
+        self._style_class.add_observer('MiddleButtonPressEvent', callback)
+
+        callback = partial(try_callback, _middle_button_release_callback)
+        self._style_class.add_observer('MiddleButtonReleaseEvent', callback)
+
+        callback = partial(try_callback, _right_button_press_callback)
+        self._style_class.add_observer('RightButtonPressEvent', callback)
+
+        callback = partial(try_callback, _right_button_release_callback)
+        self._style_class.add_observer('RightButtonReleaseEvent', callback)
+
     def enable_trackball_actor_style(self):
         """Set the interactive style to Trackball Actor.
 
         This allows to rotate actors around the scene. The controls
         are similar to the default Trackball Camera style, but
         movements transform specific objects under the mouse cursor.
 
@@ -882,14 +983,30 @@
     def _simulate_keypress(self, key):  # pragma:
         """Simulate a keypress."""
         if len(key) > 1:
             raise ValueError('Only accepts a single key')
         self.interactor.SetKeyCode(key)
         self.interactor.CharEvent()
 
+    def _control_key_press(self):
+        """Simulate a control keypress."""
+        self.interactor.SetControlKey(1)
+
+    def _control_key_release(self):
+        """Simulate a control keypress."""
+        self.interactor.SetControlKey(0)
+
+    def _shift_key_press(self):
+        """Simulate a shift keypress."""
+        self.interactor.SetShiftKey(1)
+
+    def _shift_key_release(self):
+        """Simulate a shift keypress."""
+        self.interactor.SetShiftKey(0)
+
     def _mouse_left_button_press(
         self, x=None, y=None
     ):  # pragma: no cover # numpydoc ignore=PR01,RT01
         """Simulate a left mouse button press.
 
         If ``x`` and ``y`` are entered then simulates a movement to
         that position.
@@ -908,14 +1025,40 @@
         self.interactor.LeftButtonReleaseEvent()
 
     def _mouse_left_button_click(self, x=None, y=None, count=1):
         for _ in range(count):
             self._mouse_left_button_press(x, y)
             self._mouse_left_button_release()
 
+    def _mouse_middle_button_press(
+        self, x=None, y=None
+    ):  # pragma: no cover # numpydoc ignore=PR01,RT01
+        """Simulate a middle mouse button press.
+
+        If ``x`` and ``y`` are entered then simulates a movement to
+        that position.
+
+        """
+        if x is not None and y is not None:
+            self._mouse_move(x, y)
+        self.interactor.MiddleButtonPressEvent()
+
+    def _mouse_middle_button_release(
+        self, x=None, y=None
+    ):  # pragma: no cover # numpydoc ignore=PR01,RT01
+        """Simulate a middle mouse button release."""
+        if x is not None and y is not None:
+            self._mouse_move(x, y)
+        self.interactor.MiddleButtonReleaseEvent()
+
+    def _mouse_middle_button_click(self, x=None, y=None, count=1):
+        for _ in range(count):
+            self._mouse_middle_button_press(x, y)
+            self._mouse_middle_button_release()
+
     def _mouse_right_button_press(
         self, x=None, y=None
     ):  # pragma: no cover # numpydoc ignore=PR01,RT01
         """Simulate a right mouse button press.
 
         If ``x`` and ``y`` are entered then simulates a movement to
         that position.
@@ -936,15 +1079,15 @@
     def _mouse_right_button_click(self, x=None, y=None, count=1):
         for _ in range(count):
             self._mouse_right_button_press(x, y)
             self._mouse_right_button_release()
 
     def _mouse_move(self, x, y):  # pragma:
         """Simulate moving the mouse to ``(x, y)`` screen coordinates."""
-        self.interactor.SetEventInformation(x, y)
+        self.interactor.SetEventPosition(x, y)
         self.interactor.MouseMoveEvent()
 
     def get_event_position(self):
         """Get the event position.
 
         Returns
         -------
@@ -1238,15 +1381,15 @@
         self._timer_event = None
 
 
 def _style_factory(klass):
     """Create a subclass with capturing ability, return it."""
     # We have to use a custom subclass for this because the default ones
     # swallow the release events
-    # http://vtk.1045678.n5.nabble.com/Mouse-button-release-event-is-still-broken-in-VTK-6-0-0-td5724762.html  # noqa
+    # http://vtk.1045678.n5.nabble.com/Mouse-button-release-event-is-still-broken-in-VTK-6-0-0-td5724762.html
 
     def _make_class(klass):
         """Make the class."""
         try:
             from vtkmodules import vtkInteractionStyle
         except ImportError:  # pragma: no cover
             import vtk as vtkInteractionStyle
```

### Comparing `pyvista-0.43.7/pyvista/plotting/renderer.py` & `pyvista-0.44.dev0/pyvista/plotting/renderer.py`

 * *Files 2% similar despite different names*

```diff
@@ -282,15 +282,15 @@
         self._render_passes = RenderPasses(self)
         self.cube_axes_actor = None
 
         # This is a private variable to keep track of how many colorbars exist
         # This allows us to keep adding colorbars without overlapping
         self._scalar_bar_slots = set(range(MAX_N_COLOR_BARS))
         self._scalar_bar_slot_lookup = {}
-        self.__charts = None
+        self._charts = None
 
         self._border_actor = None
         if border:
             self.add_border(border_color, border_width)
 
         self.set_color_cycler(self._theme.color_cycler)
 
@@ -352,23 +352,14 @@
     def next_color(self):  # numpydoc ignore=RT01
         """Return next color from this renderer's color cycler."""
         if self._color_cycle is None:
             return self._theme.color
         return next(self._color_cycle)['color']
 
     @property
-    def _charts(self):
-        """Return the charts collection."""
-        # lazy instantiation here to avoid creating the charts object unless needed.
-        if self.__charts is None:
-            self.__charts = Charts(self)
-            self.AddObserver("StartEvent", partial(try_callback, self._before_render_event))
-        return self.__charts
-
-    @property
     def camera_position(self):  # numpydoc ignore=RT01
         """Return or set the camera position of active render window.
 
         Returns
         -------
         pyvista.CameraPosition
             Camera position.
@@ -400,15 +391,15 @@
                 raise InvalidCameraError
             self.view_vector(camera_location)
         else:
             # check if a valid camera position
             if not isinstance(camera_location, CameraPosition):
                 if not len(camera_location) == 3:
                     raise InvalidCameraError
-                elif any([len(item) != 3 for item in camera_location]):
+                elif any(len(item) != 3 for item in camera_location):
                     raise InvalidCameraError
 
             # everything is set explicitly
             self.camera.position = scale_point(self.camera, camera_location[0], invert=False)
             self.camera.focal_point = scale_point(self.camera, camera_location[1], invert=False)
             self.camera.up = camera_location[2]
 
@@ -689,31 +680,33 @@
         """
         if _vtk.vtkRenderingContextOpenGL2 is None:  # pragma: no cover
             from pyvista.core.errors import VTKVersionError
 
             raise VTKVersionError(
                 "VTK is missing vtkRenderingContextOpenGL2. Try installing VTK v9.1.0 or newer."
             )
+        # lazy instantiation here to avoid creating the charts object unless needed.
+        if self._charts is None:
+            self._charts = Charts(self)
+            self.AddObserver("StartEvent", partial(try_callback, self._before_render_event))
         self._charts.add_chart(chart, *charts)
 
     @property
     def has_charts(self):  # numpydoc ignore=RT01
         """Return whether this renderer has charts."""
-        return self.__charts is not None
+        return self._charts is not None and len(self._charts) > 0
 
     @wraps(Charts.set_interaction)
     def set_chart_interaction(self, interactive, toggle=False):  # numpydoc ignore=PR01,RT01
         """Wrap ``Charts.set_interaction``."""
-        # Make sure we don't create the __charts object if this renderer has no charts yet.
         return self._charts.set_interaction(interactive, toggle) if self.has_charts else []
 
     @wraps(Charts.get_charts_by_pos)
     def _get_charts_by_pos(self, pos):
         """Wrap ``Charts.get_charts_by_pos``."""
-        # Make sure we don't create the __charts object if this renderer has no charts yet.
         return self._charts.get_charts_by_pos(pos) if self.has_charts else []
 
     def remove_chart(self, chart_or_index):
         """Remove a chart from this renderer.
 
         Parameters
         ----------
@@ -748,15 +741,14 @@
         Finally, remove the left chart by reference.
 
         >>> pl, chart_left, chart_right = plotter_with_charts()
         >>> pl.remove_chart(chart_left)
         >>> pl.show()
 
         """
-        # Make sure we don't create the __charts object if this renderer has no charts yet.
         if self.has_charts:
             self._charts.remove_chart(chart_or_index)
 
     @property
     def actors(self):  # numpydoc ignore=RT01
         """Return a dictionary of actors assigned to this renderer."""
         return self._actors
@@ -1620,20 +1612,20 @@
 
         # Note: font_size does nothing as a property, use SetScreenSize instead
         # Here, we normalize relative to 12 to give the user an illusion of
         # just changing the font size relative to a font size of 12. 10 is used
         # here since it's the default "screen size".
         cube_axes_actor.SetScreenSize(font_size / 12 * 10.0)
 
-        if all_edges:
-            self.add_bounding_box(color=color, corner_factor=corner_factor)
-
         self.add_actor(cube_axes_actor, reset_camera=False, pickable=False, render=render)
         self.cube_axes_actor = cube_axes_actor
 
+        if all_edges:
+            self.add_bounding_box(color=color, corner_factor=corner_factor)
+
         self.Modified()
         return cube_axes_actor
 
     def show_grid(self, **kwargs):
         """Show grid lines and bounds axes labels.
 
         A wrapped implementation of :func:`show_bounds()
@@ -2087,15 +2079,15 @@
                 except KeyError:
                     pass
             self.Modified()
 
     def clear(self):
         """Remove all actors and properties."""
         self.clear_actors()
-        if self.__charts is not None:
+        if self._charts is not None:
             self._charts.deep_clean()
         self.remove_all_lights()
         self.RemoveAllViewProps()
         self.Modified()
 
         self._scalar_bar_slots = set(range(MAX_N_COLOR_BARS))
         self._scalar_bar_slot_lookup = {}
@@ -2204,14 +2196,18 @@
 
     def enable_parallel_projection(self):
         """Enable parallel projection.
 
         The camera will have a parallel projection. Parallel projection is
         often useful when viewing images or 2D datasets.
 
+        See Also
+        --------
+        pyvista.Plotter.enable_2d_style
+
         Examples
         --------
         >>> import pyvista as pv
         >>> from pyvista import demos
         >>> pl = pv.demos.orientation_plotter()
         >>> pl.enable_parallel_projection()
         >>> pl.show()
@@ -3169,16 +3165,16 @@
 
         if self._empty_str is not None:
             self._empty_str.SetReferenceCount(0)
             self._empty_str = None
 
     def on_plotter_render(self):
         """Notify renderer components of explicit plotter render call."""
-        if self.__charts is not None:
-            for chart in self.__charts:
+        if self._charts is not None:
+            for chart in self._charts:
                 # Notify Charts that plotter.render() is called
                 chart._render_event(plotter_render=True)
 
     def deep_clean(self, render=False):
         """Clean the renderer of the memory.
 
         Parameters
@@ -3194,17 +3190,17 @@
         if hasattr(self, 'edl_pass'):
             del self.edl_pass
         if hasattr(self, '_box_object'):
             self.remove_bounding_box(render=render)
         if hasattr(self, '_shadow_pass') and self._shadow_pass is not None:
             self.disable_shadows()
         try:
-            if self.__charts is not None:
-                self.__charts.deep_clean()
-                self.__charts = None
+            if self._charts is not None:
+                self._charts.deep_clean()
+                self._charts = None
         except AttributeError:  # pragma: no cover
             pass
 
         self._render_passes.deep_clean()
         self.remove_floors(render=render)
         self.remove_legend(render=render)
         self.RemoveAllViewProps()
@@ -3284,14 +3280,15 @@
         labels=None,
         bcolor=(0.5, 0.5, 0.5),
         border=False,
         size=(0.2, 0.2),
         name=None,
         loc='upper right',
         face='triangle',
+        font_family=None,
     ):
         """Add a legend to render window.
 
         Entries must be a list containing one string and color entry for each
         item.
 
         Parameters
@@ -3351,14 +3348,19 @@
             * Rectangle: ``"r"`` or ``'rectangle'``
             * Custom: :class:`pyvista.PolyData`
 
             Passing ``None`` removes the legend face.  A custom face can be
             created using :class:`pyvista.PolyData`.  This will be rendered
             from the XY plane.
 
+        font_family : str, optional
+            Font family.  Must be either ``'courier'``, ``'times'``,
+            or ``'arial'``. Defaults to :attr:`pyvista.global_theme.font.family
+            <pyvista.plotting.themes._Font.family>`.
+
         Returns
         -------
         vtk.vtkLegendBoxActor
             Actor for the legend.
 
         Examples
         --------
@@ -3429,14 +3431,20 @@
             self._legend.SetUseBackground(False)
         else:
             self._legend.SetUseBackground(True)
             self._legend.SetBackgroundColor(Color(bcolor).float_rgb)
 
         self._legend.SetBorder(border)
 
+        if font_family is None:
+            font_family = self._theme.font.family
+
+        font_family = parse_font_family(font_family)
+        self._legend.GetEntryTextProperty().SetFontFamily(font_family)
+
         self.add_actor(self._legend, reset_camera=False, name=name, pickable=False)
         return self._legend
 
     def remove_legend(self, render=True):
         """Remove the legend actor.
 
         Parameters
```

### Comparing `pyvista-0.43.7/pyvista/plotting/renderers.py` & `pyvista-0.44.dev0/pyvista/plotting/renderers.py`

 * *Files identical despite different names*

### Comparing `pyvista-0.43.7/pyvista/plotting/scalar_bars.py` & `pyvista-0.44.dev0/pyvista/plotting/scalar_bars.py`

 * *Files identical despite different names*

### Comparing `pyvista-0.43.7/pyvista/plotting/text.py` & `pyvista-0.44.dev0/pyvista/plotting/text.py`

 * *Files 3% similar despite different names*

```diff
@@ -254,14 +254,20 @@
         Text's horizontal justification.
         Should be either "left", "center" or "right".
 
     justification_vertical : str, optional
         Text's vertical justification.
         Should be either "bottom", "center" or "top".
 
+    italic : bool, default: False
+        Italicises title and bar labels.
+
+    bold : bool, default: True
+        Bolds title and bar labels.
+
     Examples
     --------
     Create a text's property.
 
     >>> from pyvista import TextProperty
     >>> prop = TextProperty()
     >>> prop.opacity = 0.5
@@ -287,14 +293,16 @@
         font_family=None,
         orientation=None,
         font_size=None,
         font_file=None,
         shadow=False,
         justification_horizontal=None,
         justification_vertical=None,
+        italic=False,
+        bold=False,
     ):
         """Initialize text's property."""
         super().__init__()
         if theme is None:
             # copy global theme to ensure local property theme is fixed
             # after creation.
             self._theme.load_theme(pyvista.global_theme)
@@ -310,14 +318,16 @@
             self.set_font_file(font_file)
         if shadow:
             self.enable_shadow()
         if justification_horizontal is not None:
             self.justification_horizontal = justification_horizontal
         if justification_vertical is not None:
             self.justification_vertical = justification_vertical
+        self.italic = italic
+        self.bold = bold
 
     @property
     def color(self) -> Color:
         """Color of text's property.
 
         Returns
         -------
@@ -554,7 +564,39 @@
         elif justification.lower() == 'top':
             self.SetVerticalJustificationToTop()
         else:
             raise ValueError(
                 f'Invalid {justification} for justification_vertical. '
                 'Should be either "bottom", "center" or "top".'
             )
+
+    @property
+    def italic(self) -> bool:
+        """Italic of text's property.
+
+        Returns
+        -------
+        bool
+            If text is italic.
+
+        """
+        return self.GetItalic()
+
+    @italic.setter
+    def italic(self, italic: bool):  # numpydoc ignore=GL08
+        self.SetItalic(italic)
+
+    @property
+    def bold(self) -> bool:
+        """Bold of text's property.
+
+        Returns
+        -------
+        bool
+            If text is bold.
+
+        """
+        return self.GetBold()
+
+    @bold.setter
+    def bold(self, bold: bool):  # numpydoc ignore=GL08
+        self.SetBold(bold)
```

### Comparing `pyvista-0.43.7/pyvista/plotting/texture.py` & `pyvista-0.44.dev0/pyvista/plotting/texture.py`

 * *Files identical despite different names*

### Comparing `pyvista-0.43.7/pyvista/plotting/themes.py` & `pyvista-0.44.dev0/pyvista/plotting/themes.py`

 * *Files 0% similar despite different names*

```diff
@@ -139,15 +139,15 @@
 # Mostly from https://stackoverflow.com/questions/56579348/how-can-i-force-subclasses-to-have-slots
 class _ForceSlots(type):
     """Metaclass to force classes and subclasses to have __slots__."""
 
     @classmethod
     def __prepare__(metaclass, name, bases, **kwargs):
         super_prepared = super().__prepare__(metaclass, name, bases, **kwargs)
-        super_prepared['__slots__'] = tuple()
+        super_prepared['__slots__'] = ()
         return super_prepared
 
 
 class _ThemeConfig(metaclass=_ForceSlots):
     """Provide common methods for theme configuration classes."""
 
     __slots__: List[str] = []
@@ -3035,16 +3035,16 @@
         """Return or set the logo file.
 
         .. note::
 
             :func:`pyvista.Plotter.add_logo_widget` will default to
             PyVista's logo if this is unset.
 
-        Example
-        -------
+        Examples
+        --------
         Set the logo file to a custom logo.
 
         >>> import pyvista as pv
         >>> from pyvista import examples
         >>> logo_file = examples.download_file('vtk.png')
         >>> pv.global_theme.logo_file = logo_file
```

### Comparing `pyvista-0.43.7/pyvista/plotting/tools.py` & `pyvista-0.44.dev0/pyvista/plotting/tools.py`

 * *Files 1% similar despite different names*

```diff
@@ -272,15 +272,14 @@
     x_face_color='red',
     y_face_color='green',
     z_face_color='blue',
     color_box=False,
     label_color=None,
     labels_off=False,
     opacity=0.5,
-    show_text_edges=False,
 ):
     """Create a Box axes orientation widget with labels.
 
     Parameters
     ----------
     line_width : float, optional
         The width of the marker lines.
@@ -329,17 +328,14 @@
 
     labels_off : bool, optional
         Enable or disable the text labels for the axes.
 
     opacity : float, optional
         Opacity in the range of ``[0, 1]`` of the orientation box.
 
-    show_text_edges : bool, optional
-        Enable or disable drawing the vector text edges.
-
     Returns
     -------
     vtk.vtkAnnotatedCubeActor
         Annotated cube actor.
 
     Examples
     --------
@@ -380,27 +376,26 @@
     if ylabel is not None:
         axes_actor.SetYPlusFaceText(f"+{ylabel}")
         axes_actor.SetYMinusFaceText(f"-{ylabel}")
     if zlabel is not None:
         axes_actor.SetZPlusFaceText(f"+{zlabel}")
         axes_actor.SetZMinusFaceText(f"-{zlabel}")
     axes_actor.SetFaceTextVisibility(not labels_off)
-    axes_actor.SetTextEdgesVisibility(show_text_edges)
-    # https://github.com/pyvista/pyvista/pull/5382
+    axes_actor.SetTextEdgesVisibility(False)
     # axes_actor.GetTextEdgesProperty().SetColor(edge_color.float_rgb)
-    axes_actor.GetTextEdgesProperty().SetLineWidth(line_width)
+    # axes_actor.GetTextEdgesProperty().SetLineWidth(line_width)
     axes_actor.GetXPlusFaceProperty().SetColor(x_color.float_rgb)
     axes_actor.GetXMinusFaceProperty().SetColor(x_color.float_rgb)
     axes_actor.GetYPlusFaceProperty().SetColor(y_color.float_rgb)
     axes_actor.GetYMinusFaceProperty().SetColor(y_color.float_rgb)
     axes_actor.GetZPlusFaceProperty().SetColor(z_color.float_rgb)
     axes_actor.GetZMinusFaceProperty().SetColor(z_color.float_rgb)
 
     axes_actor.GetCubeProperty().SetOpacity(opacity)
-    axes_actor.GetCubeProperty().SetEdgeColor(edge_color.float_rgb)
+    # axes_actor.GetCubeProperty().SetEdgeColor(edge_color.float_rgb)
     axes_actor.GetCubeProperty().SetEdgeVisibility(True)
     axes_actor.GetCubeProperty().BackfaceCullingOn()
     if opacity < 1.0:
         # Hide the text edges
         axes_actor.GetTextEdgesProperty().SetOpacity(0)
 
     if color_box:
```

### Comparing `pyvista-0.43.7/pyvista/plotting/utilities/__init__.py` & `pyvista-0.44.dev0/pyvista/plotting/utilities/__init__.py`

 * *Files identical despite different names*

### Comparing `pyvista-0.43.7/pyvista/plotting/utilities/algorithms.py` & `pyvista-0.44.dev0/pyvista/plotting/utilities/algorithms.py`

 * *Files identical despite different names*

### Comparing `pyvista-0.43.7/pyvista/plotting/utilities/cubemap.py` & `pyvista-0.44.dev0/pyvista/plotting/utilities/cubemap.py`

 * *Files identical despite different names*

### Comparing `pyvista-0.43.7/pyvista/plotting/utilities/gl_checks.py` & `pyvista-0.44.dev0/pyvista/plotting/utilities/gl_checks.py`

 * *Files identical despite different names*

### Comparing `pyvista-0.43.7/pyvista/plotting/utilities/regression.py` & `pyvista-0.44.dev0/pyvista/plotting/utilities/regression.py`

 * *Files identical despite different names*

### Comparing `pyvista-0.43.7/pyvista/plotting/utilities/sphinx_gallery.py` & `pyvista-0.44.dev0/pyvista/plotting/utilities/sphinx_gallery.py`

 * *Files 4% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 
     .. _sphinx-gallery/sphinx-gallery/494: https://github.com/sphinx-gallery/sphinx-gallery/pull/494
     """
     return Scraper()
 
 
 def html_rst(
-    figure_list, sources_dir, fig_titles='', srcsetpaths=None
+    figure_list, sources_dir, srcsetpaths=None
 ):  # pragma: no cover  # numpydoc ignore=PR01,RT01
     """Generate reST for viewer with exported scene."""
     from sphinx_gallery.scrapers import _get_srcset_st, figure_rst
 
     if srcsetpaths is None:
         # this should never happen, but figure_rst is public, so
         # this has to be a kwarg...
@@ -98,15 +98,15 @@
 
         """
         from sphinx_gallery.scrapers import figure_rst
 
         if not pyvista.BUILDING_GALLERY:
             raise RuntimeError(BUILDING_GALLERY_ERROR_MSG)
 
-        image_names = list()
+        image_names = []
         image_path_iterator = block_vars["image_path_iterator"]
         figures = pyvista.plotting.plotter._ALL_PLOTTERS
         for plotter in figures.values():
             _process_events_before_scraping(plotter)
             fname = next(image_path_iterator)
             if hasattr(plotter, "_gif_filename"):
                 # move gif to fname
@@ -151,15 +151,15 @@
 
         Called by sphinx-gallery.
 
         """
         if not pyvista.BUILDING_GALLERY:
             raise RuntimeError(BUILDING_GALLERY_ERROR_MSG)
 
-        image_names = list()
+        image_names = []
         image_path_iterator = block_vars["image_path_iterator"]
         figures = pyvista.plotting.plotter._ALL_PLOTTERS
         # read global option  if it exists
         force_static = block_vars['example_globals'].get(
             "PYVISTA_GALLERY_FORCE_STATIC_IN_DOCUMENT", False
         )
         # override with block specific value if it exists
```

### Comparing `pyvista-0.43.7/pyvista/plotting/utilities/xvfb.py` & `pyvista-0.44.dev0/pyvista/plotting/utilities/xvfb.py`

 * *Files identical despite different names*

### Comparing `pyvista-0.43.7/pyvista/plotting/volume.py` & `pyvista-0.44.dev0/pyvista/plotting/volume.py`

 * *Files identical despite different names*

### Comparing `pyvista-0.43.7/pyvista/plotting/volume_property.py` & `pyvista-0.44.dev0/pyvista/plotting/volume_property.py`

 * *Files identical despite different names*

### Comparing `pyvista-0.43.7/pyvista/plotting/widgets.py` & `pyvista-0.44.dev0/pyvista/plotting/widgets.py`

 * *Files 2% similar despite different names*

```diff
@@ -389,14 +389,15 @@
         outline_translation=False,
         origin_translation=True,
         implicit=True,
         pass_widget=False,
         test_callback=True,
         normal_rotation=True,
         interaction_event='end',
+        outline_opacity=None,
     ):
         """Add a plane widget to the scene.
 
         This is useless without a callback function. You can pass a
         callable function that takes two arguments, the normal and
         origin of the plane in that order output from this widget, and
         performs a task with that plane.
@@ -464,14 +465,20 @@
             The VTK interaction event to use for triggering the
             callback. Accepts either the strings ``'start'``, ``'end'``,
             ``'always'`` or a ``vtk.vtkCommand.EventIds``.
 
             .. versionchanged:: 0.38.0
                Now accepts either strings and ``vtk.vtkCommand.EventIds``.
 
+        outline_opacity : bool or float, optional
+            Set the visible of outline. Only valid when using
+            an implicit plane. Either a bool or float.
+
+            .. versionadded:: 0.44.0
+
         Returns
         -------
         vtk.vtkImplicitPlaneWidget or vtk.vtkPlaneWidget
             Plane widget.
 
         Examples
         --------
@@ -547,14 +554,17 @@
             plane_widget.SetPlaceFactor(factor)
             plane_widget.PlaceWidget(bounds)
             plane_widget.SetOrigin(origin)
 
             if not normal_rotation:
                 plane_widget.GetNormalProperty().SetOpacity(0)
 
+            if outline_opacity is not None:
+                plane_widget.GetOutlineProperty().SetOpacity(float(outline_opacity))
+
         else:
             # Position of the small plane
             source = _vtk.vtkPlaneSource()
             source.SetNormal(normal)
             source.SetCenter(origin)
             source.SetPoint1(
                 origin[0] + (bounds[1] - bounds[0]) * 0.01,
@@ -633,14 +643,15 @@
         origin_translation=True,
         outline_translation=False,
         implicit=True,
         normal_rotation=True,
         crinkle=False,
         interaction_event='end',
         origin=None,
+        outline_opacity=None,
         **kwargs,
     ):
         """Clip a mesh using a plane widget.
 
         Add a mesh to the scene with a plane widget that is used to clip
         the mesh interactively.
 
@@ -704,14 +715,20 @@
 
             .. versionchanged:: 0.38.0
                Now accepts either strings or ``vtk.vtkCommand.EventIds``.
 
         origin : tuple(float), optional
             The starting coordinate of the center of the plane.
 
+        outline_opacity : bool or float, optional
+            Set the visible of outline. Only valid when using
+            an implicit plane. Either a bool or float.
+
+            .. versionadded:: 0.44.0
+
         **kwargs : dict, optional
             All additional keyword arguments are passed to
             :func:`Plotter.add_mesh` to control how the mesh is
             displayed.
 
         Returns
         -------
@@ -786,14 +803,15 @@
             assign_to_axis=assign_to_axis,
             origin_translation=origin_translation,
             outline_translation=outline_translation,
             implicit=implicit,
             origin=origin,
             normal_rotation=normal_rotation,
             interaction_event=interaction_event,
+            outline_opacity=outline_opacity,
         )
 
         if crinkle:
             return self.add_mesh(crinkler, **kwargs)
         return self.add_mesh(clipper, **kwargs)
 
     def add_volume_clip_plane(
@@ -807,14 +825,15 @@
         tubing=False,
         origin_translation=True,
         outline_translation=False,
         implicit=True,
         normal_rotation=True,
         interaction_event='end',
         origin=None,
+        outline_opacity=None,
         **kwargs,
     ):
         """Clip a volume using a plane widget.
 
         Parameters
         ----------
         volume : pyvista.plotting.volume.Volume or pyvista.ImageData or pyvista.RectilinearGrid
@@ -865,14 +884,20 @@
 
         interaction_event : vtk.vtkCommand.EventIds, optional
             The VTK interaction event to use for triggering the callback.
 
         origin : tuple(float), optional
             The starting coordinate of the center of the plane.
 
+        outline_opacity : bool or float, optional
+            Set the visible of outline. Only valid when using
+            an implicit plane. Either a bool or float.
+
+            .. versionadded:: 0.44.0
+
         **kwargs : dict, optional
             All additional keyword arguments are passed to
             :func:`Plotter.add_volume` to control how the volume is
             displayed. Only applicable if ``volume`` is either a
             :class:`pyvista.ImageData` and :class:`pyvista.RectilinearGrid`.
 
         Returns
@@ -909,14 +934,15 @@
             assign_to_axis=assign_to_axis,
             origin_translation=origin_translation,
             outline_translation=outline_translation,
             implicit=implicit,
             origin=origin,
             normal_rotation=normal_rotation,
             interaction_event=interaction_event,
+            outline_opacity=outline_opacity,
         )
         widget.GetPlane(plane)
         volume.mapper.AddClippingPlane(plane)
         self.plane_widgets.append(widget)
 
         return widget
 
@@ -930,14 +956,15 @@
         tubing=False,
         origin_translation=True,
         outline_translation=False,
         implicit=True,
         normal_rotation=True,
         interaction_event=_vtk.vtkCommand.EndInteractionEvent,
         origin=None,
+        outline_opacity=None,
         **kwargs,
     ):
         """Slice a mesh using a plane widget.
 
         Add a mesh to the scene with a plane widget that is used to slice
         the mesh interactively.
 
@@ -989,14 +1016,20 @@
 
         interaction_event : vtk.vtkCommand.EventIds, optional
             The VTK interaction event to use for triggering the callback.
 
         origin : tuple(float), optional
             The starting coordinate of the center of the plane.
 
+        outline_opacity : bool or float, optional
+            Set the visible of outline. Only valid when using
+            an implicit plane. Either a bool or float.
+
+            .. versionadded:: 0.44.0
+
         **kwargs : dict, optional
             All additional keyword arguments are passed to
             :func:`Plotter.add_mesh` to control how the mesh is
             displayed.
 
         Returns
         -------
@@ -1054,14 +1087,15 @@
             assign_to_axis=assign_to_axis,
             origin_translation=origin_translation,
             outline_translation=outline_translation,
             implicit=implicit,
             origin=origin,
             normal_rotation=normal_rotation,
             interaction_event=interaction_event,
+            outline_opacity=outline_opacity,
         )
 
         return self.add_mesh(alg, **kwargs)
 
     def add_mesh_slice_orthogonal(
         self,
         mesh,
@@ -2343,15 +2377,15 @@
                     args = [point]
                 if pass_widget:
                     args.append(widget)
                 try_callback(callback, *args)
             return
 
         if indices is None:
-            indices = [x for x in range(num)]
+            indices = list(range(num))
 
         for i in range(num):
             if center.ndim > 1:
                 loc = center[i]
             else:
                 loc = center
             sphere_widget = _vtk.vtkSphereWidget()
```

### Comparing `pyvista-0.43.7/pyvista/report.py` & `pyvista-0.44.dev0/pyvista/report.py`

 * *Files identical despite different names*

### Comparing `pyvista-0.43.7/pyvista/trame/__init__.py` & `pyvista-0.44.dev0/pyvista/trame/__init__.py`

 * *Files identical despite different names*

### Comparing `pyvista-0.43.7/pyvista/trame/jupyter.py` & `pyvista-0.44.dev0/pyvista/trame/jupyter.py`

 * *Files identical despite different names*

### Comparing `pyvista-0.43.7/pyvista/trame/ui/__init__.py` & `pyvista-0.44.dev0/pyvista/trame/ui/__init__.py`

 * *Files identical despite different names*

### Comparing `pyvista-0.43.7/pyvista/trame/ui/base_viewer.py` & `pyvista-0.44.dev0/pyvista/trame/ui/base_viewer.py`

 * *Files identical despite different names*

### Comparing `pyvista-0.43.7/pyvista/trame/ui/vuetify2.py` & `pyvista-0.44.dev0/pyvista/trame/ui/vuetify2.py`

 * *Files identical despite different names*

### Comparing `pyvista-0.43.7/pyvista/trame/ui/vuetify3.py` & `pyvista-0.44.dev0/pyvista/trame/ui/vuetify3.py`

 * *Files identical despite different names*

### Comparing `pyvista-0.43.7/pyvista/trame/views.py` & `pyvista-0.44.dev0/pyvista/trame/views.py`

 * *Files identical despite different names*

### Comparing `pyvista-0.43.7/pyvista/utilities/__init__.py` & `pyvista-0.44.dev0/pyvista/utilities/__init__.py`

 * *Files identical despite different names*

### Comparing `pyvista-0.43.7/pyvista.egg-info/PKG-INFO` & `pyvista-0.44.dev0/pyvista.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyvista
-Version: 0.43.7
+Version: 0.44.dev0
 Summary: Easier Pythonic interface to VTK
 Author-email: PyVista Developers <info@pyvista.org>
 License: MIT
 Project-URL: Documentation, https://docs.pyvista.org/
 Project-URL: Bug Tracker, https://github.com/pyvista/pyvista/issues
 Project-URL: Source Code, https://github.com/pyvista/pyvista
 Keywords: vtk,numpy,plotting,mesh
```

### Comparing `pyvista-0.43.7/pyvista.egg-info/SOURCES.txt` & `pyvista-0.44.dev0/pyvista.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyvista-0.43.7/tests/test_init.py` & `pyvista-0.44.dev0/tests/test_init.py`

 * *Files identical despite different names*

### Comparing `pyvista-0.43.7/tests/test_meshio.py` & `pyvista-0.44.dev0/tests/test_meshio.py`

 * *Files identical despite different names*

### Comparing `pyvista-0.43.7/tests/test_tinypages.py` & `pyvista-0.44.dev0/tests/test_tinypages.py`

 * *Files identical despite different names*

