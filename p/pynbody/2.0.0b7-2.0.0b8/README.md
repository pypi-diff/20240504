# Comparing `tmp/pynbody-2.0.0b7.tar.gz` & `tmp/pynbody-2.0.0b8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pynbody-2.0.0b7.tar", last modified: Wed Apr 17 19:05:56 2024, max compression
+gzip compressed data, was "pynbody-2.0.0b8.tar", last modified: Sat May  4 10:19:01 2024, max compression
```

## Comparing `pynbody-2.0.0b7.tar` & `pynbody-2.0.0b8.tar`

### file list

```diff
@@ -1,237 +1,218 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 19:05:56.389626 pynbody-2.0.0b7/
--rw-r--r--   0 runner    (1001) docker     (127)      171 2024-04-17 19:05:47.000000 pynbody-2.0.0b7/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     3306 2024-04-17 19:05:56.389626 pynbody-2.0.0b7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2514 2024-04-17 19:05:47.000000 pynbody-2.0.0b7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 19:05:56.357626 pynbody-2.0.0b7/docs/
--rw-r--r--   0 runner    (1001) docker     (127)     4597 2024-04-17 19:05:47.000000 pynbody-2.0.0b7/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)      268 2024-04-17 19:05:47.000000 pynbody-2.0.0b7/docs/acknowledge.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1322 2024-04-17 19:05:47.000000 pynbody-2.0.0b7/docs/bibliography.rst
--rw-r--r--   0 runner    (1001) docker     (127)     8294 2024-04-17 19:05:47.000000 pynbody-2.0.0b7/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)     3902 2024-04-17 19:05:47.000000 pynbody-2.0.0b7/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)     6720 2024-04-17 19:05:47.000000 pynbody-2.0.0b7/docs/installation.rst
--rw-r--r--   0 runner    (1001) docker     (127)     3475 2024-04-17 19:05:47.000000 pynbody-2.0.0b7/docs/loaders.rst
--rw-r--r--   0 runner    (1001) docker     (127)     6682 2024-04-17 19:05:47.000000 pynbody-2.0.0b7/docs/pitfalls.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 19:05:56.357626 pynbody-2.0.0b7/docs/reference/
--rw-r--r--   0 runner    (1001) docker     (127)      690 2024-04-17 19:05:47.000000 pynbody-2.0.0b7/docs/reference/analysis.rst
--rw-r--r--   0 runner    (1001) docker     (127)      262 2024-04-17 19:05:47.000000 pynbody-2.0.0b7/docs/reference/convenience.rst
--rw-r--r--   0 runner    (1001) docker     (127)     3537 2024-04-17 19:05:47.000000 pynbody-2.0.0b7/docs/reference/derived.rst
--rw-r--r--   0 runner    (1001) docker     (127)      355 2024-04-17 19:05:47.000000 pynbody-2.0.0b7/docs/reference/essentials.rst
--rw-r--r--   0 runner    (1001) docker     (127)      564 2024-04-17 19:05:47.000000 pynbody-2.0.0b7/docs/reference/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)      392 2024-04-17 19:05:47.000000 pynbody-2.0.0b7/docs/reference/plot.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 19:05:56.357626 pynbody-2.0.0b7/docs/sphinxext/
--rw-r--r--   0 runner    (1001) docker     (127)    15622 2024-04-17 19:05:47.000000 pynbody-2.0.0b7/docs/sphinxext/apigen.py
--rw-r--r--   0 runner    (1001) docker     (127)    14810 2024-04-17 19:05:47.000000 pynbody-2.0.0b7/docs/sphinxext/docscrape.py
--rw-r--r--   0 runner    (1001) docker     (127)     4237 2024-04-17 19:05:47.000000 pynbody-2.0.0b7/docs/sphinxext/docscrape_sphinx.py
--rw-r--r--   0 runner    (1001) docker     (127)    13715 2024-04-17 19:05:47.000000 pynbody-2.0.0b7/docs/sphinxext/inheritance_diagram.py
--rw-r--r--   0 runner    (1001) docker     (127)     4144 2024-04-17 19:05:47.000000 pynbody-2.0.0b7/docs/sphinxext/ipython_console_highlighting.py
--rw-r--r--   0 runner    (1001) docker     (127)    27658 2024-04-17 19:05:47.000000 pynbody-2.0.0b7/docs/sphinxext/ipython_directive.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 19:05:56.361626 pynbody-2.0.0b7/docs/tutorials/
--rw-r--r--   0 runner    (1001) docker     (127)     5012 2024-04-17 19:05:47.000000 pynbody-2.0.0b7/docs/tutorials/bridge.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1494 2024-04-17 19:05:47.000000 pynbody-2.0.0b7/docs/tutorials/configuration.rst
--rw-r--r--   0 runner    (1001) docker     (127)    17051 2024-04-17 19:05:47.000000 pynbody-2.0.0b7/docs/tutorials/data_access.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 19:05:56.361626 pynbody-2.0.0b7/docs/tutorials/example_code/
--rw-r--r--   0 runner    (1001) docker     (127)      465 2024-04-17 19:05:47.000000 pynbody-2.0.0b7/docs/tutorials/example_code/density_integrated.py
--rw-r--r--   0 runner    (1001) docker     (127)     1037 2024-04-17 19:05:47.000000 pynbody-2.0.0b7/docs/tutorials/example_code/density_profile.py
--rw-r--r--   0 runner    (1001) docker     (127)      429 2024-04-17 19:05:47.000000 pynbody-2.0.0b7/docs/tutorials/example_code/density_slice.py
--rw-r--r--   0 runner    (1001) docker     (127)     2337 2024-04-17 19:05:47.000000 pynbody-2.0.0b7/docs/tutorials/example_code/do_data.py
--rw-r--r--   0 runner    (1001) docker     (127)     2015 2024-04-17 19:05:47.000000 pynbody-2.0.0b7/docs/tutorials/example_code/do_images.py
--rw-r--r--   0 runner    (1001) docker     (127)     2055 2024-04-17 19:05:47.000000 pynbody-2.0.0b7/docs/tutorials/example_code/do_pictures.py
--rw-r--r--   0 runner    (1001) docker     (127)      958 2024-04-17 19:05:47.000000 pynbody-2.0.0b7/docs/tutorials/example_code/do_plots.py
--rw-r--r--   0 runner    (1001) docker     (127)     1443 2024-04-17 19:05:47.000000 pynbody-2.0.0b7/docs/tutorials/example_code/do_preamble.py
--rw-r--r--   0 runner    (1001) docker     (127)     1046 2024-04-17 19:05:47.000000 pynbody-2.0.0b7/docs/tutorials/example_code/rcs.py
--rw-r--r--   0 runner    (1001) docker     (127)      956 2024-04-17 19:05:47.000000 pynbody-2.0.0b7/docs/tutorials/example_code/rotcurve.py
--rw-r--r--   0 runner    (1001) docker     (127)      388 2024-04-17 19:05:47.000000 pynbody-2.0.0b7/docs/tutorials/example_code/star_render.py
--rw-r--r--   0 runner    (1001) docker     (127)      464 2024-04-17 19:05:47.000000 pynbody-2.0.0b7/docs/tutorials/example_code/temperature_slice.py
--rw-r--r--   0 runner    (1001) docker     (127)     1015 2024-04-17 19:05:47.000000 pynbody-2.0.0b7/docs/tutorials/example_code/velocity_vectors.py
--rw-r--r--   0 runner    (1001) docker     (127)     5015 2024-04-17 19:05:47.000000 pynbody-2.0.0b7/docs/tutorials/filters.rst
--rw-r--r--   0 runner    (1001) docker     (127)    12047 2024-04-17 19:05:47.000000 pynbody-2.0.0b7/docs/tutorials/halos.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2958 2024-04-17 19:05:47.000000 pynbody-2.0.0b7/docs/tutorials/hmf.rst
--rw-r--r--   0 runner    (1001) docker     (127)     8744 2024-04-17 19:05:47.000000 pynbody-2.0.0b7/docs/tutorials/performance.rst
--rw-r--r--   0 runner    (1001) docker     (127)     3319 2024-04-17 19:05:47.000000 pynbody-2.0.0b7/docs/tutorials/pictures.rst
--rw-r--r--   0 runner    (1001) docker     (127)     7271 2024-04-17 19:05:47.000000 pynbody-2.0.0b7/docs/tutorials/profile.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2141 2024-04-17 19:05:47.000000 pynbody-2.0.0b7/docs/tutorials/rotation_curve.rst
--rw-r--r--   0 runner    (1001) docker     (127)    11148 2024-04-17 19:05:47.000000 pynbody-2.0.0b7/docs/tutorials/snapshot_manipulation.rst
--rw-r--r--   0 runner    (1001) docker     (127)     5432 2024-04-17 19:05:47.000000 pynbody-2.0.0b7/docs/tutorials/threads.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1688 2024-04-17 19:05:47.000000 pynbody-2.0.0b7/docs/tutorials/tutorials.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 19:05:56.365626 pynbody-2.0.0b7/pynbody/
--rw-r--r--   0 runner    (1001) docker     (127)     1900 2024-04-17 19:05:47.000000 pynbody-2.0.0b7/pynbody/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 19:05:56.369626 pynbody-2.0.0b7/pynbody/analysis/
--rw-r--r--   0 runner    (1001) docker     (127)     4654 2024-04-17 19:05:47.000000 pynbody-2.0.0b7/pynbody/analysis/CAMB_WMAP7
--rw-r--r--   0 runner    (1001) docker     (127)      248 2024-04-17 19:05:47.000000 pynbody-2.0.0b7/pynbody/analysis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4358 2024-04-17 19:05:47.000000 pynbody-2.0.0b7/pynbody/analysis/_com.pyx
--rw-r--r--   0 runner    (1001) docker     (127)     4177 2024-04-17 19:05:47.000000 pynbody-2.0.0b7/pynbody/analysis/_interpolate3d.pyx
--rw-r--r--   0 runner    (1001) docker     (127)     4132 2024-04-17 19:05:47.000000 pynbody-2.0.0b7/pynbody/analysis/angmom.py
--rw-r--r--   0 runner    (1001) docker     (127)     9838 2024-04-17 19:05:47.000000 pynbody-2.0.0b7/pynbody/analysis/cambtemplate.ini
--rw-r--r--   0 runner    (1001) docker     (127)   103822 2024-04-17 19:05:47.000000 pynbody-2.0.0b7/pynbody/analysis/cmdlum.npz
--rw-r--r--   0 runner    (1001) docker     (127)     9878 2024-04-17 19:05:47.000000 pynbody-2.0.0b7/pynbody/analysis/cosmology.py
--rw-r--r--   0 runner    (1001) docker     (127)     7155 2024-04-17 19:05:47.000000 pynbody-2.0.0b7/pynbody/analysis/decomp.py
--rw-r--r--   0 runner    (1001) docker     (127)     3264 2024-04-17 19:05:47.000000 pynbody-2.0.0b7/pynbody/analysis/gravity.py
--rw-r--r--   0 runner    (1001) docker     (127)   872484 2024-04-17 19:05:47.000000 pynbody-2.0.0b7/pynbody/analysis/h1.hdf5
--rw-r--r--   0 runner    (1001) docker     (127)    16152 2024-04-17 19:05:47.000000 pynbody-2.0.0b7/pynbody/analysis/halo.py
--rw-r--r--   0 runner    (1001) docker     (127)     2851 2024-04-17 19:05:47.000000 pynbody-2.0.0b7/pynbody/analysis/hifrac.py
--rw-r--r--   0 runner    (1001) docker     (127)    28256 2024-04-17 19:05:47.000000 pynbody-2.0.0b7/pynbody/analysis/hmf.py
--rw-r--r--   0 runner    (1001) docker     (127)     2170 2024-04-17 19:05:47.000000 pynbody-2.0.0b7/pynbody/analysis/interpolate.py
--rw-r--r--   0 runner    (1001) docker     (127)     2014 2024-04-17 19:05:47.000000 pynbody-2.0.0b7/pynbody/analysis/ionfrac.py
--rw-r--r--   0 runner    (1001) docker     (127)    96846 2024-04-17 19:05:47.000000 pynbody-2.0.0b7/pynbody/analysis/ionfracs.npz
--rw-r--r--   0 runner    (1001) docker     (127)     6426 2024-04-17 19:05:47.000000 pynbody-2.0.0b7/pynbody/analysis/luminosity.py
--rw-r--r--   0 runner    (1001) docker     (127)    11390 2024-04-17 19:05:47.000000 pynbody-2.0.0b7/pynbody/analysis/pkdgrav_cosmo.py
--rw-r--r--   0 runner    (1001) docker     (127)    35128 2024-04-17 19:05:47.000000 pynbody-2.0.0b7/pynbody/analysis/profile.py
--rw-r--r--   0 runner    (1001) docker     (127)    14254 2024-04-17 19:05:47.000000 pynbody-2.0.0b7/pynbody/analysis/ramses_util.py
--rw-r--r--   0 runner    (1001) docker     (127)     9404 2024-04-17 19:05:47.000000 pynbody-2.0.0b7/pynbody/analysis/theoretical_profiles.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 19:05:56.369626 pynbody-2.0.0b7/pynbody/array/
--rw-r--r--   0 runner    (1001) docker     (127)    29451 2024-04-17 19:05:47.000000 pynbody-2.0.0b7/pynbody/array/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8958 2024-04-17 19:05:47.000000 pynbody-2.0.0b7/pynbody/array/shared.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 19:05:56.369626 pynbody-2.0.0b7/pynbody/bc_modules/
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-17 19:05:47.000000 pynbody-2.0.0b7/pynbody/bc_modules/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3385 2024-04-17 19:05:47.000000 pynbody-2.0.0b7/pynbody/bc_modules/capsulethunk.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 19:05:56.369626 pynbody-2.0.0b7/pynbody/bridge/
--rw-r--r--   0 runner    (1001) docker     (127)    13047 2024-04-17 19:05:47.000000 pynbody-2.0.0b7/pynbody/bridge/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2038 2024-04-17 19:05:47.000000 pynbody-2.0.0b7/pynbody/bridge/_bridge.pyx
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 19:05:56.369626 pynbody-2.0.0b7/pynbody/chunk/
--rw-r--r--   0 runner    (1001) docker     (127)    15750 2024-04-17 19:05:47.000000 pynbody-2.0.0b7/pynbody/chunk/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      793 2024-04-17 19:05:47.000000 pynbody-2.0.0b7/pynbody/chunk/scan.pyx
--rw-r--r--   0 runner    (1001) docker     (127)     3723 2024-04-17 19:05:47.000000 pynbody-2.0.0b7/pynbody/configuration.py
--rw-r--r--   0 runner    (1001) docker     (127)    11104 2024-04-17 19:05:47.000000 pynbody-2.0.0b7/pynbody/default_config.ini
--rw-r--r--   0 runner    (1001) docker     (127)     1736 2024-04-17 19:05:47.000000 pynbody-2.0.0b7/pynbody/dependencytracker.py
--rw-r--r--   0 runner    (1001) docker     (127)     9069 2024-04-17 19:05:47.000000 pynbody-2.0.0b7/pynbody/derived.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 19:05:56.369626 pynbody-2.0.0b7/pynbody/extern/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 19:05:47.000000 pynbody-2.0.0b7/pynbody/extern/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12161 2024-04-17 19:05:47.000000 pynbody-2.0.0b7/pynbody/extern/_cython_fortran_utils.pyx
--rw-r--r--   0 runner    (1001) docker     (127)       85 2024-04-17 19:05:47.000000 pynbody-2.0.0b7/pynbody/extern/cython_fortran_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     2974 2024-04-17 19:05:47.000000 pynbody-2.0.0b7/pynbody/family.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 19:05:56.373626 pynbody-2.0.0b7/pynbody/filt/
--rw-r--r--   0 runner    (1001) docker     (127)    15081 2024-04-17 19:05:47.000000 pynbody-2.0.0b7/pynbody/filt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3611 2024-04-17 19:05:47.000000 pynbody-2.0.0b7/pynbody/filt/geometry_selection.pyx
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 19:05:56.373626 pynbody-2.0.0b7/pynbody/gravity/
--rw-r--r--   0 runner    (1001) docker     (127)       19 2024-04-17 19:05:47.000000 pynbody-2.0.0b7/pynbody/gravity/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2186 2024-04-17 19:05:47.000000 pynbody-2.0.0b7/pynbody/gravity/_gravity.pyx
--rw-r--r--   0 runner    (1001) docker     (127)     5075 2024-04-17 19:05:47.000000 pynbody-2.0.0b7/pynbody/gravity/calc.py
--rw-r--r--   0 runner    (1001) docker     (127)    10115 2024-04-17 19:05:47.000000 pynbody-2.0.0b7/pynbody/gravity/config.h
--rw-r--r--   0 runner    (1001) docker     (127)     5263 2024-04-17 19:05:47.000000 pynbody-2.0.0b7/pynbody/gravity/grav.c
--rw-r--r--   0 runner    (1001) docker     (127)     4769 2024-04-17 19:05:47.000000 pynbody-2.0.0b7/pynbody/gravity/ilc.h
--rw-r--r--   0 runner    (1001) docker     (127)     3765 2024-04-17 19:05:47.000000 pynbody-2.0.0b7/pynbody/gravity/ilp.h
--rw-r--r--   0 runner    (1001) docker     (127)    18464 2024-04-17 19:05:47.000000 pynbody-2.0.0b7/pynbody/gravity/kd.h
--rw-r--r--   0 runner    (1001) docker     (127)     5510 2024-04-17 19:05:47.000000 pynbody-2.0.0b7/pynbody/gravity/main.c
--rw-r--r--   0 runner    (1001) docker     (127)    70165 2024-04-17 19:05:47.000000 pynbody-2.0.0b7/pynbody/gravity/moments.c
--rw-r--r--   0 runner    (1001) docker     (127)     5380 2024-04-17 19:05:47.000000 pynbody-2.0.0b7/pynbody/gravity/moments.h
--rw-r--r--   0 runner    (1001) docker     (127)    22930 2024-04-17 19:05:47.000000 pynbody-2.0.0b7/pynbody/gravity/serialtree.c
--rw-r--r--   0 runner    (1001) docker     (127)     1595 2024-04-17 19:05:47.000000 pynbody-2.0.0b7/pynbody/gravity/tree.py
--rw-r--r--   0 runner    (1001) docker     (127)     8007 2024-04-17 19:05:47.000000 pynbody-2.0.0b7/pynbody/gravity/walk.c
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 19:05:56.377626 pynbody-2.0.0b7/pynbody/halo/
--rw-r--r--   0 runner    (1001) docker     (127)    14818 2024-04-17 19:05:47.000000 pynbody-2.0.0b7/pynbody/halo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    16546 2024-04-17 19:05:47.000000 pynbody-2.0.0b7/pynbody/halo/adaptahop.py
--rw-r--r--   0 runner    (1001) docker     (127)    18094 2024-04-17 19:05:47.000000 pynbody-2.0.0b7/pynbody/halo/ahf.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 19:05:56.377626 pynbody-2.0.0b7/pynbody/halo/details/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 19:05:47.000000 pynbody-2.0.0b7/pynbody/halo/details/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3443 2024-04-17 19:05:47.000000 pynbody-2.0.0b7/pynbody/halo/details/iord_mapping.py
--rw-r--r--   0 runner    (1001) docker     (127)     8344 2024-04-17 19:05:47.000000 pynbody-2.0.0b7/pynbody/halo/details/number_mapping.py
--rw-r--r--   0 runner    (1001) docker     (127)     2300 2024-04-17 19:05:47.000000 pynbody-2.0.0b7/pynbody/halo/details/particle_indices.py
--rw-r--r--   0 runner    (1001) docker     (127)     9400 2024-04-17 19:05:47.000000 pynbody-2.0.0b7/pynbody/halo/hbtplus.py
--rw-r--r--   0 runner    (1001) docker     (127)     2517 2024-04-17 19:05:47.000000 pynbody-2.0.0b7/pynbody/halo/hop.py
--rw-r--r--   0 runner    (1001) docker     (127)     3382 2024-04-17 19:05:47.000000 pynbody-2.0.0b7/pynbody/halo/number_array.py
--rw-r--r--   0 runner    (1001) docker     (127)    16865 2024-04-17 19:05:47.000000 pynbody-2.0.0b7/pynbody/halo/rockstar.py
--rw-r--r--   0 runner    (1001) docker     (127)    15716 2024-04-17 19:05:47.000000 pynbody-2.0.0b7/pynbody/halo/subfind.py
--rw-r--r--   0 runner    (1001) docker     (127)    25211 2024-04-17 19:05:47.000000 pynbody-2.0.0b7/pynbody/halo/subfindhdf.py
--rw-r--r--   0 runner    (1001) docker     (127)     1499 2024-04-17 19:05:47.000000 pynbody-2.0.0b7/pynbody/halo/subhalo_catalogue.py
--rw-r--r--   0 runner    (1001) docker     (127)    10116 2024-04-17 19:05:47.000000 pynbody-2.0.0b7/pynbody/halo/velociraptor.py
--rw-r--r--   0 runner    (1001) docker     (127)     1665 2024-04-17 19:05:47.000000 pynbody-2.0.0b7/pynbody/iter_subclasses.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 19:05:56.377626 pynbody-2.0.0b7/pynbody/kdtree/
--rw-r--r--   0 runner    (1001) docker     (127)    19401 2024-04-17 19:05:47.000000 pynbody-2.0.0b7/pynbody/kdtree/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7036 2024-04-17 19:05:47.000000 pynbody-2.0.0b7/pynbody/kdtree/kd.cpp
--rw-r--r--   0 runner    (1001) docker     (127)    10541 2024-04-17 19:05:47.000000 pynbody-2.0.0b7/pynbody/kdtree/kd.h
--rw-r--r--   0 runner    (1001) docker     (127)    23690 2024-04-17 19:05:47.000000 pynbody-2.0.0b7/pynbody/kdtree/kdmain.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     6076 2024-04-17 19:05:47.000000 pynbody-2.0.0b7/pynbody/kdtree/pq.h
--rw-r--r--   0 runner    (1001) docker     (127)       79 2024-04-17 19:05:47.000000 pynbody-2.0.0b7/pynbody/kdtree/smooth.cpp
--rw-r--r--   0 runner    (1001) docker     (127)    28997 2024-04-17 19:05:47.000000 pynbody-2.0.0b7/pynbody/kdtree/smooth.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 19:05:56.377626 pynbody-2.0.0b7/pynbody/openmp/
--rw-r--r--   0 runner    (1001) docker     (127)      152 2024-04-17 19:05:47.000000 pynbody-2.0.0b7/pynbody/openmp/openmp_null.pyx
--rw-r--r--   0 runner    (1001) docker     (127)      347 2024-04-17 19:05:47.000000 pynbody-2.0.0b7/pynbody/openmp/openmp_real.pyx
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 19:05:56.377626 pynbody-2.0.0b7/pynbody/plot/
--rw-r--r--   0 runner    (1001) docker     (127)      530 2024-04-17 19:05:47.000000 pynbody-2.0.0b7/pynbody/plot/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3670 2024-04-17 19:05:47.000000 pynbody-2.0.0b7/pynbody/plot/gas.py
--rw-r--r--   0 runner    (1001) docker     (127)    19284 2024-04-17 19:05:47.000000 pynbody-2.0.0b7/pynbody/plot/generic.py
--rw-r--r--   0 runner    (1001) docker     (127)     1882 2024-04-17 19:05:47.000000 pynbody-2.0.0b7/pynbody/plot/metals.py
--rw-r--r--   0 runner    (1001) docker     (127)     6769 2024-04-17 19:05:47.000000 pynbody-2.0.0b7/pynbody/plot/profile.py
--rw-r--r--   0 runner    (1001) docker     (127)    17830 2024-04-17 19:05:47.000000 pynbody-2.0.0b7/pynbody/plot/sph.py
--rw-r--r--   0 runner    (1001) docker     (127)    41579 2024-04-17 19:05:47.000000 pynbody-2.0.0b7/pynbody/plot/stars.py
--rw-r--r--   0 runner    (1001) docker     (127)      121 2024-04-17 19:05:47.000000 pynbody-2.0.0b7/pynbody/plot/tollerud2008mw
--rw-r--r--   0 runner    (1001) docker     (127)     6364 2024-04-17 19:05:47.000000 pynbody-2.0.0b7/pynbody/plot/util.py
--rw-r--r--   0 runner    (1001) docker     (127)     2417 2024-04-17 19:05:47.000000 pynbody-2.0.0b7/pynbody/simdict.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 19:05:56.381626 pynbody-2.0.0b7/pynbody/snapshot/
--rw-r--r--   0 runner    (1001) docker     (127)     2631 2024-04-17 19:05:47.000000 pynbody-2.0.0b7/pynbody/snapshot/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2682 2024-04-17 19:05:47.000000 pynbody-2.0.0b7/pynbody/snapshot/ascii.py
--rw-r--r--   0 runner    (1001) docker     (127)     2578 2024-04-17 19:05:47.000000 pynbody-2.0.0b7/pynbody/snapshot/copy_on_access.py
--rw-r--r--   0 runner    (1001) docker     (127)    52738 2024-04-17 19:05:47.000000 pynbody-2.0.0b7/pynbody/snapshot/gadget.py
--rw-r--r--   0 runner    (1001) docker     (127)    41128 2024-04-17 19:05:47.000000 pynbody-2.0.0b7/pynbody/snapshot/gadgethdf.py
--rw-r--r--   0 runner    (1001) docker     (127)     8542 2024-04-17 19:05:47.000000 pynbody-2.0.0b7/pynbody/snapshot/grafic.py
--rw-r--r--   0 runner    (1001) docker     (127)     1903 2024-04-17 19:05:47.000000 pynbody-2.0.0b7/pynbody/snapshot/namemapper.py
--rw-r--r--   0 runner    (1001) docker     (127)     7619 2024-04-17 19:05:47.000000 pynbody-2.0.0b7/pynbody/snapshot/nchilada.py
--rw-r--r--   0 runner    (1001) docker     (127)    46971 2024-04-17 19:05:47.000000 pynbody-2.0.0b7/pynbody/snapshot/ramses.py
--rw-r--r--   0 runner    (1001) docker     (127)    68679 2024-04-17 19:05:47.000000 pynbody-2.0.0b7/pynbody/snapshot/simsnap.py
--rw-r--r--   0 runner    (1001) docker     (127)    15058 2024-04-17 19:05:47.000000 pynbody-2.0.0b7/pynbody/snapshot/subsnap.py
--rw-r--r--   0 runner    (1001) docker     (127)    10441 2024-04-17 19:05:47.000000 pynbody-2.0.0b7/pynbody/snapshot/swift.py
--rw-r--r--   0 runner    (1001) docker     (127)    63548 2024-04-17 19:05:47.000000 pynbody-2.0.0b7/pynbody/snapshot/tipsy.py
--rw-r--r--   0 runner    (1001) docker     (127)     3761 2024-04-17 19:05:47.000000 pynbody-2.0.0b7/pynbody/snapshot/util.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 19:05:56.381626 pynbody-2.0.0b7/pynbody/sph/
--rw-r--r--   0 runner    (1001) docker     (127)    31283 2024-04-17 19:05:47.000000 pynbody-2.0.0b7/pynbody/sph/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    18195 2024-04-17 19:05:47.000000 pynbody-2.0.0b7/pynbody/sph/_render.pyx
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 19:05:56.381626 pynbody-2.0.0b7/pynbody/test_utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 19:05:47.000000 pynbody-2.0.0b7/pynbody/test_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9906 2024-04-17 19:05:47.000000 pynbody-2.0.0b7/pynbody/test_utils/gadget4_subfind_reader.py
--rw-r--r--   0 runner    (1001) docker     (127)    18964 2024-04-17 19:05:47.000000 pynbody-2.0.0b7/pynbody/test_utils/pyread_gadget_hdf5.py
--rw-r--r--   0 runner    (1001) docker     (127)     5678 2024-04-17 19:05:47.000000 pynbody-2.0.0b7/pynbody/transformation.py
--rw-r--r--   0 runner    (1001) docker     (127)    24581 2024-04-17 19:05:47.000000 pynbody-2.0.0b7/pynbody/units.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 19:05:56.381626 pynbody-2.0.0b7/pynbody/util/
--rw-r--r--   0 runner    (1001) docker     (127)    19035 2024-04-17 19:05:47.000000 pynbody-2.0.0b7/pynbody/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10035 2024-04-17 19:05:47.000000 pynbody-2.0.0b7/pynbody/util/_util.pyx
--rw-r--r--   0 runner    (1001) docker     (127)     3296 2024-04-17 19:05:47.000000 pynbody-2.0.0b7/pynbody/util/hdf_vds.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 19:05:56.365626 pynbody-2.0.0b7/pynbody.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3306 2024-04-17 19:05:56.000000 pynbody-2.0.0b7/pynbody.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5712 2024-04-17 19:05:56.000000 pynbody-2.0.0b7/pynbody.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-17 19:05:56.000000 pynbody-2.0.0b7/pynbody.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      312 2024-04-17 19:05:56.000000 pynbody-2.0.0b7/pynbody.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)      254 2024-04-17 19:05:56.000000 pynbody-2.0.0b7/pynbody.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1183 2024-04-17 19:05:47.000000 pynbody-2.0.0b7/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-17 19:05:56.389626 pynbody-2.0.0b7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     8082 2024-04-17 19:05:47.000000 pynbody-2.0.0b7/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 19:05:56.389626 pynbody-2.0.0b7/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     8458 2024-04-17 19:05:47.000000 pynbody-2.0.0b7/tests/adaptahop_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    12103 2024-04-17 19:05:47.000000 pynbody-2.0.0b7/tests/ahf_halos_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     8377 2024-04-17 19:05:47.000000 pynbody-2.0.0b7/tests/array_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     4953 2024-04-17 19:05:47.000000 pynbody-2.0.0b7/tests/bridge_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     4735 2024-04-17 19:05:47.000000 pynbody-2.0.0b7/tests/copy_on_access_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     1377 2024-04-17 19:05:47.000000 pynbody-2.0.0b7/tests/cosmology_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     5658 2024-04-17 19:05:47.000000 pynbody-2.0.0b7/tests/derived_arrays_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     1296 2024-04-17 19:05:47.000000 pynbody-2.0.0b7/tests/family_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     6142 2024-04-17 19:05:47.000000 pynbody-2.0.0b7/tests/filter_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     7335 2024-04-17 19:05:47.000000 pynbody-2.0.0b7/tests/gadget_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     5398 2024-04-17 19:05:47.000000 pynbody-2.0.0b7/tests/gadgethdf_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     1775 2024-04-17 19:05:47.000000 pynbody-2.0.0b7/tests/grafic_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     2924 2024-04-17 19:05:47.000000 pynbody-2.0.0b7/tests/gravity_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    12875 2024-04-17 19:05:47.000000 pynbody-2.0.0b7/tests/halos_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     2666 2024-04-17 19:05:47.000000 pynbody-2.0.0b7/tests/halotools_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    13934 2024-04-17 19:05:47.000000 pynbody-2.0.0b7/tests/hbtplus_test.py
--rw-r--r--   0 runner    (1001) docker     (127)      711 2024-04-17 19:05:47.000000 pynbody-2.0.0b7/tests/hop_test.py
--rw-r--r--   0 runner    (1001) docker     (127)      137 2024-04-17 19:05:47.000000 pynbody-2.0.0b7/tests/import_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    10743 2024-04-17 19:05:47.000000 pynbody-2.0.0b7/tests/kdtree_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    11675 2024-04-17 19:05:47.000000 pynbody-2.0.0b7/tests/nchilada_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     1183 2024-04-17 19:05:47.000000 pynbody-2.0.0b7/tests/partial_tipsy_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     2350 2024-04-17 19:05:47.000000 pynbody-2.0.0b7/tests/performance_kdtree.py
--rw-r--r--   0 runner    (1001) docker     (127)     7722 2024-04-17 19:05:47.000000 pynbody-2.0.0b7/tests/ramses_new_ptcl_format_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    21515 2024-04-17 19:05:47.000000 pynbody-2.0.0b7/tests/ramses_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     3462 2024-04-17 19:05:47.000000 pynbody-2.0.0b7/tests/rockstar_test.py
--rw-r--r--   0 runner    (1001) docker     (127)      378 2024-04-17 19:05:47.000000 pynbody-2.0.0b7/tests/simsnap_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     6686 2024-04-17 19:05:47.000000 pynbody-2.0.0b7/tests/snapshot_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     5033 2024-04-17 19:05:47.000000 pynbody-2.0.0b7/tests/sph_image_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     1541 2024-04-17 19:05:47.000000 pynbody-2.0.0b7/tests/subarray_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     5669 2024-04-17 19:05:47.000000 pynbody-2.0.0b7/tests/subfind_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     5009 2024-04-17 19:05:47.000000 pynbody-2.0.0b7/tests/subfindhdf_gadget4_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     9396 2024-04-17 19:05:47.000000 pynbody-2.0.0b7/tests/subfindhdf_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     8163 2024-04-17 19:05:47.000000 pynbody-2.0.0b7/tests/swift_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     2773 2024-04-17 19:05:47.000000 pynbody-2.0.0b7/tests/test_profile.py
--rw-r--r--   0 runner    (1001) docker     (127)     4717 2024-04-17 19:05:47.000000 pynbody-2.0.0b7/tests/theoretical_profile.py
--rw-r--r--   0 runner    (1001) docker     (127)    19773 2024-04-17 19:05:47.000000 pynbody-2.0.0b7/tests/tipsy_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     3735 2024-04-17 19:05:47.000000 pynbody-2.0.0b7/tests/transformation_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     2988 2024-04-17 19:05:47.000000 pynbody-2.0.0b7/tests/units_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     6558 2024-04-17 19:05:47.000000 pynbody-2.0.0b7/tests/utils_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     4238 2024-04-17 19:05:47.000000 pynbody-2.0.0b7/tests/velociraptor_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 10:19:01.392221 pynbody-2.0.0b8/
+-rw-r--r--   0 runner    (1001) docker     (127)      171 2024-05-04 10:18:55.000000 pynbody-2.0.0b8/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     3306 2024-05-04 10:19:01.392221 pynbody-2.0.0b8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2514 2024-05-04 10:18:55.000000 pynbody-2.0.0b8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 10:19:01.364221 pynbody-2.0.0b8/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)     4597 2024-05-04 10:18:55.000000 pynbody-2.0.0b8/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 10:19:01.360221 pynbody-2.0.0b8/docs/_templates/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 10:19:01.364221 pynbody-2.0.0b8/docs/_templates/autosummary/
+-rw-r--r--   0 runner    (1001) docker     (127)      185 2024-05-04 10:18:55.000000 pynbody-2.0.0b8/docs/_templates/autosummary/class.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1103 2024-05-04 10:18:55.000000 pynbody-2.0.0b8/docs/_templates/autosummary/module.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      268 2024-05-04 10:18:55.000000 pynbody-2.0.0b8/docs/acknowledge.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1322 2024-05-04 10:18:55.000000 pynbody-2.0.0b8/docs/bibliography.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     9768 2024-05-04 10:18:55.000000 pynbody-2.0.0b8/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3652 2024-05-04 10:18:55.000000 pynbody-2.0.0b8/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     7397 2024-05-04 10:18:55.000000 pynbody-2.0.0b8/docs/installation.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3475 2024-05-04 10:18:55.000000 pynbody-2.0.0b8/docs/loaders.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     6911 2024-05-04 10:18:55.000000 pynbody-2.0.0b8/docs/pitfalls.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 10:19:01.364221 pynbody-2.0.0b8/docs/reference/
+-rw-r--r--   0 runner    (1001) docker     (127)      948 2024-05-04 10:18:55.000000 pynbody-2.0.0b8/docs/reference/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 10:19:01.364221 pynbody-2.0.0b8/docs/tutorials/
+-rw-r--r--   0 runner    (1001) docker     (127)    10514 2024-05-04 10:18:55.000000 pynbody-2.0.0b8/docs/tutorials/bridge.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1722 2024-05-04 10:18:55.000000 pynbody-2.0.0b8/docs/tutorials/configuration.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    19402 2024-05-04 10:18:55.000000 pynbody-2.0.0b8/docs/tutorials/data_access.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     5368 2024-05-04 10:18:55.000000 pynbody-2.0.0b8/docs/tutorials/derived.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 10:19:01.368221 pynbody-2.0.0b8/docs/tutorials/example_code/
+-rw-r--r--   0 runner    (1001) docker     (127)      465 2024-05-04 10:18:55.000000 pynbody-2.0.0b8/docs/tutorials/example_code/density_integrated.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1119 2024-05-04 10:18:55.000000 pynbody-2.0.0b8/docs/tutorials/example_code/density_profile.py
+-rw-r--r--   0 runner    (1001) docker     (127)      429 2024-05-04 10:18:55.000000 pynbody-2.0.0b8/docs/tutorials/example_code/density_slice.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2337 2024-05-04 10:18:55.000000 pynbody-2.0.0b8/docs/tutorials/example_code/do_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2015 2024-05-04 10:18:55.000000 pynbody-2.0.0b8/docs/tutorials/example_code/do_images.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2055 2024-05-04 10:18:55.000000 pynbody-2.0.0b8/docs/tutorials/example_code/do_pictures.py
+-rw-r--r--   0 runner    (1001) docker     (127)      958 2024-05-04 10:18:55.000000 pynbody-2.0.0b8/docs/tutorials/example_code/do_plots.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1443 2024-05-04 10:18:55.000000 pynbody-2.0.0b8/docs/tutorials/example_code/do_preamble.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1046 2024-05-04 10:18:55.000000 pynbody-2.0.0b8/docs/tutorials/example_code/rcs.py
+-rw-r--r--   0 runner    (1001) docker     (127)      956 2024-05-04 10:18:55.000000 pynbody-2.0.0b8/docs/tutorials/example_code/rotcurve.py
+-rw-r--r--   0 runner    (1001) docker     (127)      388 2024-05-04 10:18:55.000000 pynbody-2.0.0b8/docs/tutorials/example_code/star_render.py
+-rw-r--r--   0 runner    (1001) docker     (127)      464 2024-05-04 10:18:55.000000 pynbody-2.0.0b8/docs/tutorials/example_code/temperature_slice.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1022 2024-05-04 10:18:55.000000 pynbody-2.0.0b8/docs/tutorials/example_code/velocity_vectors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6782 2024-05-04 10:18:55.000000 pynbody-2.0.0b8/docs/tutorials/filters.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    11931 2024-05-04 10:18:55.000000 pynbody-2.0.0b8/docs/tutorials/halos.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     5431 2024-05-04 10:18:55.000000 pynbody-2.0.0b8/docs/tutorials/hmf.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     8744 2024-05-04 10:18:56.000000 pynbody-2.0.0b8/docs/tutorials/performance.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3319 2024-05-04 10:18:56.000000 pynbody-2.0.0b8/docs/tutorials/pictures.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    10348 2024-05-04 10:18:56.000000 pynbody-2.0.0b8/docs/tutorials/profile.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    13890 2024-05-04 10:18:56.000000 pynbody-2.0.0b8/docs/tutorials/quickstart.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     5432 2024-05-04 10:18:56.000000 pynbody-2.0.0b8/docs/tutorials/threads.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2570 2024-05-04 10:18:56.000000 pynbody-2.0.0b8/docs/tutorials/tutorials.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 10:19:01.368221 pynbody-2.0.0b8/pynbody/
+-rw-r--r--   0 runner    (1001) docker     (127)     1897 2024-05-04 10:18:56.000000 pynbody-2.0.0b8/pynbody/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 10:19:01.376221 pynbody-2.0.0b8/pynbody/analysis/
+-rw-r--r--   0 runner    (1001) docker     (127)    50000 2024-05-04 10:18:56.000000 pynbody-2.0.0b8/pynbody/analysis/CAMB_Planck18
+-rw-r--r--   0 runner    (1001) docker     (127)     4654 2024-05-04 10:18:56.000000 pynbody-2.0.0b8/pynbody/analysis/CAMB_WMAP7
+-rw-r--r--   0 runner    (1001) docker     (127)      806 2024-05-04 10:18:56.000000 pynbody-2.0.0b8/pynbody/analysis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2510 2024-05-04 10:18:56.000000 pynbody-2.0.0b8/pynbody/analysis/_com.pyx
+-rw-r--r--   0 runner    (1001) docker     (127)     4177 2024-05-04 10:18:56.000000 pynbody-2.0.0b8/pynbody/analysis/_interpolate3d.pyx
+-rw-r--r--   0 runner    (1001) docker     (127)     9240 2024-05-04 10:18:56.000000 pynbody-2.0.0b8/pynbody/analysis/angmom.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9838 2024-05-04 10:18:56.000000 pynbody-2.0.0b8/pynbody/analysis/cambtemplate.ini
+-rw-r--r--   0 runner    (1001) docker     (127)   103822 2024-05-04 10:18:56.000000 pynbody-2.0.0b8/pynbody/analysis/cmdlum.npz
+-rw-r--r--   0 runner    (1001) docker     (127)    12325 2024-05-04 10:18:56.000000 pynbody-2.0.0b8/pynbody/analysis/cosmology.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7344 2024-05-04 10:18:56.000000 pynbody-2.0.0b8/pynbody/analysis/decomp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3264 2024-05-04 10:18:56.000000 pynbody-2.0.0b8/pynbody/analysis/gravity.py
+-rw-r--r--   0 runner    (1001) docker     (127)   872484 2024-05-04 10:18:56.000000 pynbody-2.0.0b8/pynbody/analysis/h1.hdf5
+-rw-r--r--   0 runner    (1001) docker     (127)    20567 2024-05-04 10:18:56.000000 pynbody-2.0.0b8/pynbody/analysis/halo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2851 2024-05-04 10:18:56.000000 pynbody-2.0.0b8/pynbody/analysis/hifrac.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33570 2024-05-04 10:18:56.000000 pynbody-2.0.0b8/pynbody/analysis/hmf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2170 2024-05-04 10:18:56.000000 pynbody-2.0.0b8/pynbody/analysis/interpolate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2014 2024-05-04 10:18:56.000000 pynbody-2.0.0b8/pynbody/analysis/ionfrac.py
+-rw-r--r--   0 runner    (1001) docker     (127)    96846 2024-05-04 10:18:56.000000 pynbody-2.0.0b8/pynbody/analysis/ionfracs.npz
+-rw-r--r--   0 runner    (1001) docker     (127)     6426 2024-05-04 10:18:56.000000 pynbody-2.0.0b8/pynbody/analysis/luminosity.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11390 2024-05-04 10:18:56.000000 pynbody-2.0.0b8/pynbody/analysis/pkdgrav_cosmo.py
+-rw-r--r--   0 runner    (1001) docker     (127)    35128 2024-05-04 10:18:56.000000 pynbody-2.0.0b8/pynbody/analysis/profile.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14279 2024-05-04 10:18:56.000000 pynbody-2.0.0b8/pynbody/analysis/ramses_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9404 2024-05-04 10:18:56.000000 pynbody-2.0.0b8/pynbody/analysis/theoretical_profiles.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 10:19:01.376221 pynbody-2.0.0b8/pynbody/array/
+-rw-r--r--   0 runner    (1001) docker     (127)    35806 2024-05-04 10:18:56.000000 pynbody-2.0.0b8/pynbody/array/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8982 2024-05-04 10:18:56.000000 pynbody-2.0.0b8/pynbody/array/shared.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 10:19:01.376221 pynbody-2.0.0b8/pynbody/bridge/
+-rw-r--r--   0 runner    (1001) docker     (127)    20598 2024-05-04 10:18:56.000000 pynbody-2.0.0b8/pynbody/bridge/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2038 2024-05-04 10:18:56.000000 pynbody-2.0.0b8/pynbody/bridge/_bridge.pyx
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 10:19:01.376221 pynbody-2.0.0b8/pynbody/chunk/
+-rw-r--r--   0 runner    (1001) docker     (127)    14387 2024-05-04 10:18:56.000000 pynbody-2.0.0b8/pynbody/chunk/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1366 2024-05-04 10:18:56.000000 pynbody-2.0.0b8/pynbody/chunk/scan.pyx
+-rw-r--r--   0 runner    (1001) docker     (127)     4231 2024-05-04 10:18:56.000000 pynbody-2.0.0b8/pynbody/configuration.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12648 2024-05-04 10:18:56.000000 pynbody-2.0.0b8/pynbody/default_config.ini
+-rw-r--r--   0 runner    (1001) docker     (127)     3357 2024-05-04 10:18:56.000000 pynbody-2.0.0b8/pynbody/dependencytracker.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8967 2024-05-04 10:18:56.000000 pynbody-2.0.0b8/pynbody/derived.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 10:19:01.376221 pynbody-2.0.0b8/pynbody/extern/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-04 10:18:56.000000 pynbody-2.0.0b8/pynbody/extern/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12161 2024-05-04 10:18:56.000000 pynbody-2.0.0b8/pynbody/extern/_cython_fortran_utils.pyx
+-rw-r--r--   0 runner    (1001) docker     (127)       85 2024-05-04 10:18:56.000000 pynbody-2.0.0b8/pynbody/extern/cython_fortran_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4232 2024-05-04 10:18:56.000000 pynbody-2.0.0b8/pynbody/family.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 10:19:01.376221 pynbody-2.0.0b8/pynbody/filt/
+-rw-r--r--   0 runner    (1001) docker     (127)    20293 2024-05-04 10:18:56.000000 pynbody-2.0.0b8/pynbody/filt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3776 2024-05-04 10:18:56.000000 pynbody-2.0.0b8/pynbody/filt/geometry_selection.pyx
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 10:19:01.376221 pynbody-2.0.0b8/pynbody/gravity/
+-rw-r--r--   0 runner    (1001) docker     (127)       51 2024-05-04 10:18:56.000000 pynbody-2.0.0b8/pynbody/gravity/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2186 2024-05-04 10:18:56.000000 pynbody-2.0.0b8/pynbody/gravity/_gravity.pyx
+-rw-r--r--   0 runner    (1001) docker     (127)     7245 2024-05-04 10:18:56.000000 pynbody-2.0.0b8/pynbody/gravity/calc.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 10:19:01.376221 pynbody-2.0.0b8/pynbody/halo/
+-rw-r--r--   0 runner    (1001) docker     (127)    19880 2024-05-04 10:18:56.000000 pynbody-2.0.0b8/pynbody/halo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17451 2024-05-04 10:18:56.000000 pynbody-2.0.0b8/pynbody/halo/adaptahop.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19201 2024-05-04 10:18:56.000000 pynbody-2.0.0b8/pynbody/halo/ahf.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 10:19:01.380221 pynbody-2.0.0b8/pynbody/halo/details/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-04 10:18:56.000000 pynbody-2.0.0b8/pynbody/halo/details/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3443 2024-05-04 10:18:56.000000 pynbody-2.0.0b8/pynbody/halo/details/iord_mapping.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8344 2024-05-04 10:18:56.000000 pynbody-2.0.0b8/pynbody/halo/details/number_mapping.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2494 2024-05-04 10:18:56.000000 pynbody-2.0.0b8/pynbody/halo/details/particle_indices.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11555 2024-05-04 10:18:56.000000 pynbody-2.0.0b8/pynbody/halo/hbtplus.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3501 2024-05-04 10:18:56.000000 pynbody-2.0.0b8/pynbody/halo/hop.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3625 2024-05-04 10:18:56.000000 pynbody-2.0.0b8/pynbody/halo/number_array.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17216 2024-05-04 10:18:56.000000 pynbody-2.0.0b8/pynbody/halo/rockstar.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17250 2024-05-04 10:18:56.000000 pynbody-2.0.0b8/pynbody/halo/subfind.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25292 2024-05-04 10:18:56.000000 pynbody-2.0.0b8/pynbody/halo/subfindhdf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1610 2024-05-04 10:18:56.000000 pynbody-2.0.0b8/pynbody/halo/subhalo_catalogue.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10851 2024-05-04 10:18:56.000000 pynbody-2.0.0b8/pynbody/halo/velociraptor.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 10:19:01.380221 pynbody-2.0.0b8/pynbody/kdtree/
+-rw-r--r--   0 runner    (1001) docker     (127)    19401 2024-05-04 10:18:56.000000 pynbody-2.0.0b8/pynbody/kdtree/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7036 2024-05-04 10:18:56.000000 pynbody-2.0.0b8/pynbody/kdtree/kd.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)    10541 2024-05-04 10:18:56.000000 pynbody-2.0.0b8/pynbody/kdtree/kd.h
+-rw-r--r--   0 runner    (1001) docker     (127)    23690 2024-05-04 10:18:56.000000 pynbody-2.0.0b8/pynbody/kdtree/kdmain.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     6076 2024-05-04 10:18:56.000000 pynbody-2.0.0b8/pynbody/kdtree/pq.h
+-rw-r--r--   0 runner    (1001) docker     (127)       79 2024-05-04 10:18:56.000000 pynbody-2.0.0b8/pynbody/kdtree/smooth.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)    28997 2024-05-04 10:18:56.000000 pynbody-2.0.0b8/pynbody/kdtree/smooth.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 10:19:01.380221 pynbody-2.0.0b8/pynbody/openmp/
+-rw-r--r--   0 runner    (1001) docker     (127)      152 2024-05-04 10:18:56.000000 pynbody-2.0.0b8/pynbody/openmp/openmp_null.pyx
+-rw-r--r--   0 runner    (1001) docker     (127)      549 2024-05-04 10:18:56.000000 pynbody-2.0.0b8/pynbody/openmp/openmp_real.pyx
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 10:19:01.380221 pynbody-2.0.0b8/pynbody/plot/
+-rw-r--r--   0 runner    (1001) docker     (127)      530 2024-05-04 10:18:56.000000 pynbody-2.0.0b8/pynbody/plot/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3670 2024-05-04 10:18:56.000000 pynbody-2.0.0b8/pynbody/plot/gas.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19212 2024-05-04 10:18:56.000000 pynbody-2.0.0b8/pynbody/plot/generic.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1882 2024-05-04 10:18:56.000000 pynbody-2.0.0b8/pynbody/plot/metals.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6769 2024-05-04 10:18:56.000000 pynbody-2.0.0b8/pynbody/plot/profile.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4702 2024-05-04 10:18:56.000000 pynbody-2.0.0b8/pynbody/plot/quiverkey.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25811 2024-05-04 10:18:56.000000 pynbody-2.0.0b8/pynbody/plot/sph.py
+-rw-r--r--   0 runner    (1001) docker     (127)    44246 2024-05-04 10:18:56.000000 pynbody-2.0.0b8/pynbody/plot/stars.py
+-rw-r--r--   0 runner    (1001) docker     (127)      121 2024-05-04 10:18:56.000000 pynbody-2.0.0b8/pynbody/plot/tollerud2008mw
+-rw-r--r--   0 runner    (1001) docker     (127)     6364 2024-05-04 10:18:56.000000 pynbody-2.0.0b8/pynbody/plot/util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2417 2024-05-04 10:18:56.000000 pynbody-2.0.0b8/pynbody/simdict.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 10:19:01.384221 pynbody-2.0.0b8/pynbody/snapshot/
+-rw-r--r--   0 runner    (1001) docker     (127)     3157 2024-05-04 10:18:56.000000 pynbody-2.0.0b8/pynbody/snapshot/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3017 2024-05-04 10:18:56.000000 pynbody-2.0.0b8/pynbody/snapshot/ascii.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2962 2024-05-04 10:18:56.000000 pynbody-2.0.0b8/pynbody/snapshot/copy_on_access.py
+-rw-r--r--   0 runner    (1001) docker     (127)    52755 2024-05-04 10:18:56.000000 pynbody-2.0.0b8/pynbody/snapshot/gadget.py
+-rw-r--r--   0 runner    (1001) docker     (127)    41232 2024-05-04 10:18:56.000000 pynbody-2.0.0b8/pynbody/snapshot/gadgethdf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9161 2024-05-04 10:18:56.000000 pynbody-2.0.0b8/pynbody/snapshot/grafic.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2781 2024-05-04 10:18:56.000000 pynbody-2.0.0b8/pynbody/snapshot/namemapper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7164 2024-05-04 10:18:56.000000 pynbody-2.0.0b8/pynbody/snapshot/nchilada.py
+-rw-r--r--   0 runner    (1001) docker     (127)    47425 2024-05-04 10:18:56.000000 pynbody-2.0.0b8/pynbody/snapshot/ramses.py
+-rw-r--r--   0 runner    (1001) docker     (127)    71116 2024-05-04 10:18:56.000000 pynbody-2.0.0b8/pynbody/snapshot/simsnap.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15045 2024-05-04 10:18:56.000000 pynbody-2.0.0b8/pynbody/snapshot/subsnap.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10866 2024-05-04 10:18:56.000000 pynbody-2.0.0b8/pynbody/snapshot/swift.py
+-rw-r--r--   0 runner    (1001) docker     (127)    63498 2024-05-04 10:18:56.000000 pynbody-2.0.0b8/pynbody/snapshot/tipsy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4972 2024-05-04 10:18:56.000000 pynbody-2.0.0b8/pynbody/snapshot/util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 10:19:01.384221 pynbody-2.0.0b8/pynbody/sph/
+-rw-r--r--   0 runner    (1001) docker     (127)    31727 2024-05-04 10:18:56.000000 pynbody-2.0.0b8/pynbody/sph/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18653 2024-05-04 10:18:56.000000 pynbody-2.0.0b8/pynbody/sph/_render.pyx
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 10:19:01.384221 pynbody-2.0.0b8/pynbody/test_utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-04 10:18:56.000000 pynbody-2.0.0b8/pynbody/test_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9906 2024-05-04 10:18:56.000000 pynbody-2.0.0b8/pynbody/test_utils/gadget4_subfind_reader.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18964 2024-05-04 10:18:56.000000 pynbody-2.0.0b8/pynbody/test_utils/pyread_gadget_hdf5.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16592 2024-05-04 10:18:56.000000 pynbody-2.0.0b8/pynbody/transformation.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25347 2024-05-04 10:18:56.000000 pynbody-2.0.0b8/pynbody/units.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 10:19:01.384221 pynbody-2.0.0b8/pynbody/util/
+-rw-r--r--   0 runner    (1001) docker     (127)    19035 2024-05-04 10:18:56.000000 pynbody-2.0.0b8/pynbody/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10035 2024-05-04 10:18:56.000000 pynbody-2.0.0b8/pynbody/util/_util.pyx
+-rw-r--r--   0 runner    (1001) docker     (127)     3296 2024-05-04 10:18:56.000000 pynbody-2.0.0b8/pynbody/util/hdf_vds.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1830 2024-05-04 10:18:56.000000 pynbody-2.0.0b8/pynbody/util/iter_subclasses.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 10:19:01.368221 pynbody-2.0.0b8/pynbody.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3306 2024-05-04 10:19:01.000000 pynbody-2.0.0b8/pynbody.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5173 2024-05-04 10:19:01.000000 pynbody-2.0.0b8/pynbody.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-04 10:19:01.000000 pynbody-2.0.0b8/pynbody.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      441 2024-05-04 10:19:01.000000 pynbody-2.0.0b8/pynbody.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      235 2024-05-04 10:19:01.000000 pynbody-2.0.0b8/pynbody.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1289 2024-05-04 10:18:56.000000 pynbody-2.0.0b8/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-04 10:19:01.392221 pynbody-2.0.0b8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     8149 2024-05-04 10:18:56.000000 pynbody-2.0.0b8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 10:19:01.392221 pynbody-2.0.0b8/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     8487 2024-05-04 10:18:56.000000 pynbody-2.0.0b8/tests/adaptahop_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12467 2024-05-04 10:18:56.000000 pynbody-2.0.0b8/tests/ahf_halos_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9374 2024-05-04 10:18:56.000000 pynbody-2.0.0b8/tests/array_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7408 2024-05-04 10:18:56.000000 pynbody-2.0.0b8/tests/bridge_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4732 2024-05-04 10:18:56.000000 pynbody-2.0.0b8/tests/copy_on_access_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1377 2024-05-04 10:18:56.000000 pynbody-2.0.0b8/tests/cosmology_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6358 2024-05-04 10:18:56.000000 pynbody-2.0.0b8/tests/derived_arrays_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1296 2024-05-04 10:18:56.000000 pynbody-2.0.0b8/tests/family_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7081 2024-05-04 10:18:56.000000 pynbody-2.0.0b8/tests/filter_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7320 2024-05-04 10:18:56.000000 pynbody-2.0.0b8/tests/gadget_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5396 2024-05-04 10:18:56.000000 pynbody-2.0.0b8/tests/gadgethdf_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1773 2024-05-04 10:18:56.000000 pynbody-2.0.0b8/tests/grafic_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2919 2024-05-04 10:18:56.000000 pynbody-2.0.0b8/tests/gravity_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13591 2024-05-04 10:18:56.000000 pynbody-2.0.0b8/tests/halos_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3471 2024-05-04 10:18:56.000000 pynbody-2.0.0b8/tests/halotools_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14383 2024-05-04 10:18:56.000000 pynbody-2.0.0b8/tests/hbtplus_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2536 2024-05-04 10:18:56.000000 pynbody-2.0.0b8/tests/hmf_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1050 2024-05-04 10:18:56.000000 pynbody-2.0.0b8/tests/hop_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)      137 2024-05-04 10:18:56.000000 pynbody-2.0.0b8/tests/import_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10743 2024-05-04 10:18:56.000000 pynbody-2.0.0b8/tests/kdtree_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11675 2024-05-04 10:18:56.000000 pynbody-2.0.0b8/tests/nchilada_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1183 2024-05-04 10:18:56.000000 pynbody-2.0.0b8/tests/partial_tipsy_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2350 2024-05-04 10:18:56.000000 pynbody-2.0.0b8/tests/performance_kdtree.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7722 2024-05-04 10:18:56.000000 pynbody-2.0.0b8/tests/ramses_new_ptcl_format_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21598 2024-05-04 10:18:56.000000 pynbody-2.0.0b8/tests/ramses_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3549 2024-05-04 10:18:56.000000 pynbody-2.0.0b8/tests/rockstar_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)      378 2024-05-04 10:18:56.000000 pynbody-2.0.0b8/tests/simsnap_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7072 2024-05-04 10:18:56.000000 pynbody-2.0.0b8/tests/snapshot_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5151 2024-05-04 10:18:56.000000 pynbody-2.0.0b8/tests/sph_image_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1541 2024-05-04 10:18:56.000000 pynbody-2.0.0b8/tests/subarray_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6121 2024-05-04 10:18:56.000000 pynbody-2.0.0b8/tests/subfind_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5751 2024-05-04 10:18:56.000000 pynbody-2.0.0b8/tests/subfindhdf_gadget4_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9653 2024-05-04 10:18:56.000000 pynbody-2.0.0b8/tests/subfindhdf_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8681 2024-05-04 10:18:56.000000 pynbody-2.0.0b8/tests/swift_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2773 2024-05-04 10:18:56.000000 pynbody-2.0.0b8/tests/test_profile.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4717 2024-05-04 10:18:56.000000 pynbody-2.0.0b8/tests/theoretical_profile.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19416 2024-05-04 10:18:56.000000 pynbody-2.0.0b8/tests/tipsy_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5223 2024-05-04 10:18:56.000000 pynbody-2.0.0b8/tests/transformation_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3872 2024-05-04 10:18:56.000000 pynbody-2.0.0b8/tests/units_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6558 2024-05-04 10:18:56.000000 pynbody-2.0.0b8/tests/utils_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4536 2024-05-04 10:18:56.000000 pynbody-2.0.0b8/tests/velociraptor_test.py
```

### Comparing `pynbody-2.0.0b7/PKG-INFO` & `pynbody-2.0.0b8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pynbody
-Version: 2.0.0b7
+Version: 2.0.0b8
 Summary: Light-weight astronomical N-body/SPH analysis for python
 Home-page: https://github.com/pynbody/pynbody/releases
 Author: The pynbody team
 Author-email: pynbody@googlegroups.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
```

### Comparing `pynbody-2.0.0b7/README.md` & `pynbody-2.0.0b8/README.md`

 * *Files identical despite different names*

### Comparing `pynbody-2.0.0b7/docs/Makefile` & `pynbody-2.0.0b8/docs/Makefile`

 * *Files identical despite different names*

### Comparing `pynbody-2.0.0b7/docs/bibliography.rst` & `pynbody-2.0.0b8/docs/bibliography.rst`

 * *Files identical despite different names*

### Comparing `pynbody-2.0.0b7/docs/conf.py` & `pynbody-2.0.0b8/docs/conf.py`

 * *Files 11% similar despite different names*

```diff
@@ -9,14 +9,16 @@
 #
 # All configuration values have a default; values that are commented out
 # serve to show the default.
 
 import os
 import sys
 
+import numpy as np
+
 #import sphinx_bootstrap_theme
 
 # If extensions (or modules to document with autodoc) are in another directory,
 # add these directories to sys.path here. If the directory is relative to the
 # documentation root, use os.path.abspath to make it absolute, like shown here.
 sys.path.insert(0, os.path.abspath('.'))
 sys.path.insert(0, os.path.abspath('../pynbody'))
@@ -28,61 +30,76 @@
 #needs_sphinx = '1.0'
 
 # Add any Sphinx extension module names here, as strings. They can be extensions
 # coming with Sphinx (named 'sphinx.ext.*') or your custom ones.
 extensions = ['sphinx.ext.autodoc',
               'sphinx.ext.doctest',
               'sphinx.ext.todo',
+              'sphinx.ext.napoleon',
               'sphinx.ext.coverage',
-              'sphinx.ext.imgmath',
+              'sphinx.ext.mathjax',
               'sphinx.ext.ifconfig',
               'sphinx.ext.viewcode',
               'matplotlib.sphinxext.mathmpl',
               'matplotlib.sphinxext.plot_directive',
               'sphinx.ext.inheritance_diagram',
-              'numpydoc']
-
+              'sphinx_copybutton',
+              'numpydoc',
+              'nbsphinx'
+              ]
+
+nbsphinx_input_prompt = 'In [%s]:'
+nbsphinx_output_prompt = 'Out[%s]:'
+nbsphinx_execute = 'never' # the notebook is expensive to evaluate, so we need it pre-evaluated
 
+autosummary_generate = True
 
 ipython_warning_is_error = False
+ipython_savefig_dir = 'plots'
+
+# for .. plot:: directives
+plot_working_directory = '.'
+
+
+extensions+=['IPython.sphinxext.ipython_console_highlighting',
+             'IPython.sphinxext.ipython_directive']
 
-try:
-    import IPython.sphinxext.ipython_console_highlighting
-    extensions+=['IPython.sphinxext.ipython_console_highlighting',
-                 'IPython.sphinxext.ipython_directive']
-except ImportError:
-    extensions+=['ipython_console_highlighting','ipython_directive']
 
 # Add any paths that contain templates here, relative to this directory.
 templates_path = ['_templates']
 
 # The suffix of source filenames.
 source_suffix = '.rst'
 
 # The encoding of source files.
 #source_encoding = 'utf-8-sig'
 
 # The master toctree document.
 master_doc = 'index'
 
+globaltoc_collapse = True
+
 # General information about the project.
 project = 'pynbody'
-copyright = '2011-20, pynbody team'
+copyright = '2011-24, pynbody team'
 
 # The version info for the project you're documenting, acts as replacement for
 # |version| and |release|, also used in various other places throughout the
 # built documents.
 #
 # The short X.Y version.
 import pynbody
 
 version = ".".join(pynbody.__version__.split(".")[:2])
 # The full version, including alpha/beta/rc tags.
 release = pynbody.__version__
 
+# make sure plot module is imported for documenting
+import pynbody.plot
+
 # The language for content autogenerated by Sphinx. Refer to documentation
 # for a list of supported languages.
 #language = None
 
 # There are two options for replacing |today|: either, you set today to some
 # non-false value, then it is used:
 #today = ''
@@ -110,22 +127,28 @@
 # The name of the Pygments (syntax highlighting) style to use.
 pygments_style = 'sphinx'
 
 # A list of ignored prefixes for module index sorting.
 #modindex_common_prefix = []
 
 
+
 # -- Options for HTML output ---------------------------------------------------
 
 # The theme to use for HTML and HTML Help pages.  See the documentation for
 # a list of builtin themes.
-html_theme = 'alabaster'
+html_theme = 'sphinx_book_theme'
 
 # set up bootstrap
-html_theme_options = { 'logo': 'logo.svg', 'logo_name': False, 'sidebar_collapse': False}
+html_theme_options = {
+    "repository_url": "https://github.com/pynbody/pynbody",
+    "use_repository_button": True,
+                       }
+
+html_logo = "_static/logo.svg"
 
 """html_theme_path = sphinx_bootstrap_theme.get_html_theme_path()
 
 html_theme_options = {
     'bootswatch_theme': 'spacelab',
 
     'navbar_site_name': 'Sections',
@@ -167,15 +190,24 @@
 #html_last_updated_fmt = '%b %d, %Y'
 
 # If true, SmartyPants will be used to convert quotes and dashes to
 # typographically correct entities.
 #html_use_smartypants = True
 
 # Custom sidebar templates, maps document names to template names.
-#html_sidebars = {}
+# html_sidebars = {'**': ['logo.html', 'fulltoc.html', 'relations.html', 'searchbox.html']}
+
+# html_sidebars = {
+#     '**': [
+#         'about.html',
+#         'navigation.html',
+#         'relations.html',
+#         'searchbox.html',
+#     ]
+# }
 
 # Additional templates that should be rendered to pages, maps page names to
 # template names.
 #html_additional_pages = {}
 
 # If false, no module index is generated.
 #html_domain_indices = True
@@ -238,21 +270,44 @@
 
 # Additional stuff for the LaTeX preamble.
 #latex_preamble = ''
 
 # Documents to append as an appendix to all manuals.
 #latex_appendices = []
 
-# If false, no module index is generated.
 #latex_domain_indices = True
 
 
 # -- Options for manual page output --------------------------------------------
 
 # One entry per manual page. List of tuples
 # (source start file, name, description, authors, manual section).
 man_pages = [
     ('index', 'pynbody', 'pynbody Documentation',
      ['pynbody team'], 1)
 ]
 
-autodoc_member_order = 'bysource'
+#autodoc_member_order = 'alphabetical'
+#autoclass_content = 'both'
+
+copybutton_copy_empty_lines = False
+copybutton_selector =  "div.highlight > pre"
+copybutton_prompt_text = r">>> |\.\.\. |\$ |In \[\d*\]: | {2,5}\.{3,5}: | {5,8}: "
+copybutton_prompt_is_regexp = True
+copybutton_only_copy_prompt_lines = True
+
+def hide_numpy_methods(app, what, name, obj, skip, options):
+    if hasattr(obj, "__qualname__"):
+        qname = obj.__qualname__
+        if "SimArray" in qname:
+            method_name = qname.split(".")[-1]
+            if method_name in np.ndarray.__dict__:
+                print("Skipping ", qname)
+                return True
+def setup(app):
+    app.connect('autodoc-skip-member', hide_numpy_methods)
+
+import matplotlib
+
+matplotlib.rcParams['savefig.dpi'] = 200
+matplotlib.rcParams['savefig.bbox'] = 'tight'
+matplotlib.rcParams['savefig.pad_inches'] = 0.15
```

### Comparing `pynbody-2.0.0b7/docs/index.rst` & `pynbody-2.0.0b8/docs/index.rst`

 * *Files 17% similar despite different names*

```diff
@@ -1,104 +1,88 @@
 .. pynbody documentation master file, created by
    sphinx-quickstart on Mon Oct  3 11:57:24 2011.
    You can adapt this file completely to your liking, but it should at least
    contain the root ``toctree`` directive.
 
+.. warning::
 
-Pynbody Documentation
-===============================
+ You are looking at the documentation for pynbody v2, which is currently in beta.
+ To install pynbody v2 beta, use ``pip install --pre pynbody``.  Documentation for
+ v1 remains available at https://pynbody.github.io/pynbody/ .
 
 Welcome to the documentation for `pynbody
 <http://pynbody.github.io>`_ -- an analysis package for
 astrophysical N-body and Smooth Particle Hydrodynamics
-simulations, supporting Python 3.5+. (Old versions are
-available, prior to 1.0, that support Python 2.5, 2.6 and 2.7).
-
-We recommend you get started by reading about
-:ref:`pynbody-installation` and trying the :ref:`tutorials`. We are
-happy to provide further assistance via our
-`user group email list
-<https://groups.google.com/forum/?fromgroups#!forum/pynbody-users>`_.
-
-Where next?
------------
-
-Consult the :doc:`installation` documentation for instructions on how
-to get going. Then you might like to download some `test data
-<https://github.com/pynbody/pynbody/releases>`_ and try out the
-:ref:`first steps tutorial <snapshot_manipulation>` which gets straight
-to some of pynbody's analysis features. Or, if you prefer to learn
-a little more of how your data is organized, we also provide a :ref:`data
-access walkthrough <data-access>`.
-
-Our full documentation is organized into three sections:
-
-.. toctree::
-   :maxdepth: 1
-
-   Installation <installation>
-   Tutorials & walkthroughs <tutorials/tutorials>
-   Reference <reference/index>
-
-
-All of the information in the reference guide is also available
-through the interactive python help system. In ipython or Jupyter, this is as
-easy as putting a ``?`` at the end of a command:
-
-.. ipython::
-
-   In [1]: import pynbody
-
-   In [2]: pynbody.load?
+simulations, supporting Python 3 with minor version support
+adhering roughly to the `SPEC0 <https://scientific-python.org/specs/spec-0000/>`_ policy.
 
+Installation should be as simple as
 
+.. code-block:: bash
 
-.. _getting-help:
+   pip install pynbody
 
-Seeking Further Assistance
----------------------------
+but if you run into trouble, try the :doc:`installation` guide.
 
+Once installed, we recommend you get started by trying the :ref:`tutorials`.
 
-If the tutorials and reference documentation don't answer your question,
-any problem might be described in :doc:`pitfalls`.
+Support
+-------
 
-If you still find yourself stuck, don't hesitate to post a message to the
-`users group
-<https://groups.google.com/forum/?fromgroups#!forum/pynbody-users>`_.
-If you have a Google account you can join the groups
-easily, but if you don't have one please click on the ``About`` button
-of the group you are interested in and contact the owner.
-
-We have found that most development discussion takes place within our
-`github issue tracker <https://github.com/pynbody/pynbody/issues>`_ -- if you
-encounter a problem, feel free to create an issue there.
-We greatly value feedback from users, especially when things are not
-working correctly because this is the best way for us to correct
-bugs.  This includes any problems you encounter with documentation.
+Pynbody is a complex project maintained by a small team of scientists, and our dayjobs is doing science!
+We do our best to provide support, and we greatly appreciate feedback and bug reports. If you encounter any problems,
+please consider `opening an issue on github <https://github.com/pynbody/pynbody/issues/new/choose>`_ or posting to our
+`email list <https://groups.google.com/forum/?fromgroups#!forum/pynbody-users>`_. To help us help you, when asking for
+assistance please provide a simple, minimal python script that we can use to reproduce a bug, inaccuracy or situation.
+Preferably reproduce the bug using pynbody's own test data (as used by the tutorials,
+and downloadable at http://star.ucl.ac.uk/~app/testdata.tar.gz).
+If this impossible, provide us a pointer to another file that we can use to reproduce the problem.
 
 Please note that we adhere to a  `community code of conduct
 <https://github.com/pynbody/pynbody/blob/master/CODE_OF_CONDUCT.md>`_,
 which you should read and understand before posting to the users list or in a github issue.
 
-If you use the code regularly for your projects, please consider contributing
-your code back using a `pull request
+Open science relies on good will and reciprocity. Please strongly consider contributing any enhancements or fixes of
+your own back to the project using a `pull request
 <https://help.github.com/articles/using-pull-requests>`_.
 
+
+
 .. _acknowledging-pynbody:
 
 Acknowledging Pynbody in Scientific Publications
 ------------------------------------------------
 
-Pynbody development is an open-source, community effort. The only way
-to make it as robust as possible is to have a wide user-base and this
-is only possible by spreading the word. We ask that if you use pynbody
+Pynbody development is an open-source, community effort.We ask that if you use pynbody
 in preparing a scientific publication, you cite it via its
 `Astrophysics Source Code Library <http://ascl.net/1305.002>`_ entry
 using the following BibTex::
 
    @misc{pynbody,
      author = {{Pontzen}, A. and {Ro{\v s}kar}, R. and {Stinson}, G.~S. and {Woods},
         R. and {Reed}, D.~M. and {Coles}, J. and {Quinn}, T.~R.},
      title = "{pynbody: Astrophysics Simulation Analysis for Python}",
      note = {Astrophysics Source Code Library, ascl:1305.002},
      year = 2013
    }
+
+
+
+Where next?
+-----------
+
+Consult the :doc:`installation` documentation for instructions on how
+to get going. Then you might like to download some `test data
+<https://github.com/pynbody/pynbody/releases>`_ and try out the
+:ref:`quick-start tutorial <quickstart>` which gets straight
+to some of pynbody's analysis features. Or, if you prefer to learn
+a little more of how your data is organized, we also provide a :ref:`data
+access walkthrough <data-access>`.
+
+Our full documentation is organized into three sections:
+
+.. toctree::
+   :maxdepth: 3
+
+   Tutorials & walkthroughs <tutorials/tutorials>
+   Reference <reference/index>
+   Installation <installation>
```

### Comparing `pynbody-2.0.0b7/docs/loaders.rst` & `pynbody-2.0.0b8/docs/loaders.rst`

 * *Files identical despite different names*

### Comparing `pynbody-2.0.0b7/docs/pitfalls.rst` & `pynbody-2.0.0b8/docs/pitfalls.rst`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,19 @@
 .. pitfalls Common Pitfalls
 
 
 Common Pitfalls
 ===============
 
+I can't compile from source because of an error to do with OpenMP
+^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
+
+If you're on a mac, you need to use a non-default compiler. See
+:ref:`macos-compilers` for more details.
+
 .. _paramfiles_are_good:
 
 I get errors like "Unknown units" or "Not convertible" from analysis or plotting routines
 ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
 
 One of the great things about ``pynbody`` is that it takes care of units, but
 if it can't figure out what units to use, everything is assumed to be
@@ -33,15 +39,15 @@
  2. all the particles are clustered in the central pixel.
 
 To tackle both of these issues in turn:
 
  1. The image is *always* centred on ``(0,0,0)``, so you need to offset
  the simulation before you start. The most common way to do this
  is with the function :func:`pynbody.analysis.halo.center`; see
- :ref:`snapshot_manipulation` for an introduction.
+ :ref:`quickstart` for an introduction.
 
  2. The ``width`` keyword for the image function
  expects a floating point number in the current units of the
  snapshot. It also defaults to the number ``10``, which may be
  very large compared to your snapshot, depending on the units you
  have adopted. That means either you should *specify* a width which
  is more appropriate (i.e. your call might look like
```

### Comparing `pynbody-2.0.0b7/docs/tutorials/data_access.rst` & `pynbody-2.0.0b8/docs/tutorials/data_access.rst`

 * *Files 12% similar despite different names*

```diff
@@ -1,31 +1,32 @@
+.. Last checked by AP: 18 Mar 2024
+
 .. data_access tutorial
 
 .. _data-access:
 
-A walk through pynbody's low-level facilities
-=============================================
+A deeper walk through pynbody's data access facilities
+======================================================
 
 The following example shows how to load a file, determine various
-attributes, access some data and make use of unit information.
+attributes, access some data, make use of unit information, and understand
+how pynbody transforms data.
 
-If you're more interested in making pretty pictures and plots straight
-away, you may wish to read the :ref:`basic facilities tutorial
-<snapshot_manipulation>` first.
+A shorter tutorial that deals with the absolute basics and shows how to make
+some plots is offered by the :ref:`quick-start <quickstart>` guide.
 
 .. note::
 
  This tutorial assumes basic familiarity with python and is
  written as a series of ``ipython`` cells, like a ``Jupyter`` notebook.
  Before you start make sure ``pynbody`` is properly
  installed. See :ref:`pynbody-installation`
  for more information. You will also need the standard ``pynbody`` test
- files if you want to follow the tutorial.
- These files are available separately here:
- `testdata.tar.gz <https://github.com/pynbody/pynbody/releases>`_.
+ files if you want to follow the tutorial. See :ref:`obtaining_testdata`
+ for more information.
 
 After you have extracted the testdata folder (e.g. with ``tar -xzf
 testdata.tar.gz``), launch ``ipython`` or ``Jupyter``. At the prompt or in
 a cell, type ``import pynbody``. If all is installed correctly, this should silently
 succeed, and you are ready to use ``pynbody``.
 
 First steps
@@ -43,16 +44,15 @@
 
  In [2]: f = pynbody.load("testdata/gadget2/test_g2_snap")
 
 Here we've loaded a sample gadget file. Not much seems to have
 happened when you called :func:`pynbody.load`, but the variable ``f``
 is now your calling point for accessing data.
 
-In fact ``f`` is an object known as a ``SimSnap`` (see
-:class:`pynbody.snapshot.SimSnap`).
+In fact ``f`` is an object known as a :class:`~pynbody.snapshot.simsnap.SimSnap`.
 
 Behind the scenes, the function inspects the provided path and decides
 what file format it is. At the time of writing, supported file formats
 include tipsy, nchilada, gadget-1, gadget-2, gadget-HDF and
 ramses. For most purposes you should never need to know what type of
 file you are dealing with -- that's the whole point of the ``pynbody``
 framework.
@@ -74,45 +74,42 @@
 
 Let's start to inspect the file we've opened. The standard python operator ``len`` can be used to query the number
 of particles in the file:
 
 
 .. ipython::
 
- @doctest
  In [3]: len(f)
- Out[3]: 8192
 
 We can also find out about particles of a particular type or ``family``
 as it is known within pynbody. To find out which families are present
-in the file, use :func:`~pynbody.snapshot.SimSnap.families`:
+in the file, use :func:`~pynbody.snapshot.simsnap.SimSnap.families`:
 
 .. ipython::
 
  In [3]: f.families()
- Out[3]: [<Family gas>, <Family dm>, <Family star>]
 
 You can pick out just the particles belonging to a family by using the
 syntax ``f.family``. So, for example, we can see how many particles of
 each type are present:
 
 
 .. ipython::
 
- @doctest
- In [4]: len(f.dm)
- Out[4]: 4096
-
- @doctest
- In [5]: len(f.gas)
- Out[5]: 4039
-
- @doctest
- In [6]: len(f.star)
- Out[6]: 57
+     @doctest
+     In [4]: len(f.dm)
+     Out[4]: 4096
+
+     @doctest
+     In [5]: len(f.gas)
+     Out[5]: 4039
+
+     @doctest
+     In [6]: len(f.star)
+     Out[6]: 57
 
 Useful information about the file is stored in a python dictionary
 called ``properties``:
 
 .. ipython::
 
  In [4]: f.properties
@@ -134,26 +131,25 @@
 
 
 Retrieving data
 ---------------
 
 Like ``f.properties``, ``f`` itself also behaves like a python
 dictionary. The standard python method
-``f.``:func:`~pynbody.snapshot.SimSnap.keys` returns a list of arrays
+``f.``:func:`~pynbody.snapshot.simsnap.SimSnap.keys` returns a list of arrays
 that are currently in memory.
 
 .. ipython::
 
   In [7]: f.keys()
   Out[7]: ['eps']
 
 Right now it's empty! That's actually correct because data is only
-retrieved when you first access it. To find out what *could*` be loaded,
-use the ``pynbody``-specific method
-``f.``:func:`~pynbody.snapshot.SimSnap.loadable_keys`.
+retrieved when you first access it. To find out what *could* be loaded,
+use the ``pynbody``-specific method :func:`~pynbody.snapshot.simsnap.SimSnap.loadable_keys`:
 
 .. ipython::
 
   In [10]: f.loadable_keys()
   Out[10]: ['pos', 'vel', 'id', 'mass']
 
 This looks a bit more promising.
@@ -186,15 +182,15 @@
  :ref:`configurable <configuration>` should you wish to adopt
  different conventions.
 
 Some arrays are stored only for certain families. For example,
 densities are stored only for gas particles and are accessed as
 ``f.gas['rho']``.  To find out what arrays are available for the gas
 family, use
-``f.gas.``:func:`~pynbody.snapshot.SimSnap.loadable_keys`:
+``f.gas.``:func:`~pynbody.snapshot.simsnap.SimSnap.loadable_keys`:
 
 .. ipython::
 
  In [13]: f.gas.loadable_keys()
  Out[13]:
  ['nhp',
  'smooth',
@@ -280,24 +276,23 @@
 access it, only if the ``mass`` array has changed. Therefore you don't
 waste any time by using derived arrays. For more information see
 the reference documentation for :ref:`derived arrays <derived>`.
 
 Keeping on top of units
 -----------------------
 
-
 You might have noticed in the output from the above experiments that
 ``pynbody`` keeps track of unit information whenever it can.
 
 .. warning:: It's worth understanding exactly where pynbody gets this
- information from, in case anything goes wrong. In the case
- of ``Ramses``, and ``Gadget-HDF`` files the unit information is stored
- within your snapshot, and pynbody takes advantage of this. For
- old-style ``Gadget`` snapshots, the default cosmological gadget setup is
- assumed. For ``nchilada`` and ``tipsy``, an nchilada or gasoline
+ information from, in case anything goes wrong. Many simulation data
+ formats now store units (e.g. gadget, arepo or swift's HDF5 output, or
+ ramses output folders). In such
+ cases, pynbody will use the specified units.
+ For ``nchilada`` and ``tipsy``, a ChaNGa or gasoline
  ``.param`` file is sought in the directory from which you are loading
  the snapshot and its immediate parent. You can also create a text file
  with the same name as your snapshot but the extension ``.units`` to override
  the units at load time. For example, such a file can contain ::
 
    pos: kpc a
    vel: km s^-1
@@ -396,16 +391,16 @@
        [ 1473.32873535,  4711.41308594,  2117.31494141]], dtype=float32, 'km**2 s**-2')
 
 
  In [57]: np.sqrt(((f['vel']**2).sum(axis=1)*f['mass'])).units
  Out[57]:
 
 You can even associate arrays with the loaded
-:class:`~pynbody.snapshot.SimSnap` unit system even when you create
-them *outside* the :class:`~pynbody.snapshot.SimSnap`. This is useful
+:class:`~pynbody.snapshot.simsnap.SimSnap` unit system even when you create
+them *outside* the :class:`~pynbody.snapshot.simsnap.SimSnap`. This is useful
 for keeping things tidy with your unit conversions if you are
 calculating quantities that don't apply to all of the particles. For
 instance:
 
 .. ipython::
 
  In [6]: array = pynbody.array.SimArray(np.random.rand(10)) # make the newly-formed numpy array a pynbody array
@@ -417,24 +412,24 @@
  In [9]: array
 
  In [9]: array.in_units('kpc')
 
 Note that the units were correctly converted into physical units in
 the last step.
 
-For more information see the reference documentation for
-:class:`pynbody.units`.
+.. seealso::
+  For more information see the reference documentation for :class:`pynbody.units`.
 
 .. _subsnaps:
 
 Subsnaps
 --------
 
 An important concept within ``pynbody`` is that of a subsnap. These are
-objects that look just like a :class:`~pynbody.snapshot.SimSnap` but actually only point
+objects that look just like a :class:`~pynbody.snapshot.simsnap.SimSnap` but actually only point
 at a subset of the particles within a ``parent``. Subsnaps are always
 instances of the :class:`~pynbody.snapshot.SubSnap` class.
 
 You've already seen some examples of subsnaps, actually. When you
 accessed ``f.gas`` or ``f.dm``, you're given back a subsnap pointing
 at only those particles. However, subsnaps can be used in a much more
 general way. For example, you can use python's normal array slicing
@@ -530,19 +525,92 @@
 
 .. ipython::
 
  In [71]: from pynbody.filt import *
 
  In [72]: f_sphere = f[Sphere('10 kpc')]
 
+.. seealso::
+  For more information see :ref:`filters_tutorial`, and for a list of filters, see :py:mod:`pynbody.filt`.
 
-For a list of filters, see  :py:mod:`pynbody.filt`.
 
+.. _centering:
 
-Where next?
------------
+Centering
+---------
+
+Several built-in functions (e.g. those that plot images and make
+profiles) in ``pynbody`` like your data to be centered on a point of
+interest.  The most straight-forward way to center your snapshot on a
+halo is as follows:
+
+.. ipython :: python
+
+ f = pynbody.load("testdata/gasoline_ahf/g15784.lr.01024.gz");
+ h = f.halos();
+ pynbody.analysis.center(h[0])
+
+We passed ``h[0]`` to the function
+:func:`~pynbody.analysis.center` to center the *entire* snapshot
+on the largest halo. The default centring uses the *shrinking sphere* method,
+which normally gives a really stable and precise centre for galaxies, halos
+or any other astronomical object
+(see the documentation for :func:`~pynbody.analysis.center` for
+more details).
+
+Suppose we now want to center only the contents of halo 5, leaving the
+rest of the simulation untouched. This is no problem. Let's check
+where a particle in halo 5 is, then shift it and try again. You'll
+notice halo 1 doesn't move at all.
+
+.. ipython ::
+
+ In [4]: h[1]['pos'][0]
+
+ In [4]: h[5]['pos'][0]
+
+ In [4]: h5 = h[5]
+
+ In [4]: my_h5_transform = pynbody.analysis.center(h5, move_all=False)
+
+ In [4]: h[1]['pos'][0] # should be unchanged
+
+ In [4]: h5['pos'][0] # should be changed
+
+Note however that the data inside ``h5`` (or any halo) just *points*
+to a subset of the data in the full simulation. So you now have an
+inconsistent state where part of the simulation has been translated
+and the rest of it is where it started out. For that reason, functions
+that transform data return a ``Tranformation`` object that conveniently
+allows you to undo the operation:
+
+.. ipython ::
+
+ In [5]: my_h5_transform.revert()
+
+ In [5]: print(h5['pos'][0]) # back to where it started
+
+ In [5]: print(h[1]['pos'][0]) # still hasn't changed, of course
+
+
+In fact, there's a more pythonic and compact way to do this. Suppose
+you want to process ``h[5]`` in some way, but be sure that the
+centering is unaffected after you are done. This is the thing to do:
+
+.. ipython ::
+
+ In [6]: with pynbody.analysis.center(h[5]):
+    ...:     print("Position when inside with block: ", h[5]['pos'][0])
+    ...: print("Position when outside with block: ", h[5]['pos'][0])
+
+
+Inside the ``with`` code block, ``h[5]`` is centered. The moment the block
+exits, the transformation is undone -- even if the block exits with an
+exception.
+
+.. seealso::
+
+ For more information about centering, see the documentation for
+ :func:`~pynbody.analysis.halo.center`.
 
-This concludes the tutorial for basic use of ``pynbody``. Further
-:ref:`tutorials <tutorials>` for specific tasks are available. We are
-happy to provide further assistance via our
-`user group email list
-<https://groups.google.com/forum/?fromgroups#!forum/pynbody-users>`_.
+ For more information about transformations in general, see the documentation for the
+ :mod:`~pynbody.transformation` module.
```

### Comparing `pynbody-2.0.0b7/docs/tutorials/example_code/density_profile.py` & `pynbody-2.0.0b8/docs/tutorials/example_code/density_profile.py`

 * *Files 19% similar despite different names*

```diff
@@ -5,31 +5,33 @@
 # load the snapshot and set to physical units
 s = pynbody.load('testdata/gasoline_ahf/g15784.lr.01024.gz')
 
 # load the halos
 h = s.halos()
 
 # center on the largest halo and align the disk
-pynbody.analysis.angmom.faceon(h[1])
+pynbody.analysis.angmom.faceon(h[0])
 
 # convert all units to something reasonable (kpc, Msol etc)
 s.physical_units()
 
 # create a profile object for the stars (by default this is a 2D profile)
-p = pynbody.analysis.profile.Profile(h[1].s, vmin =.01, max=50)
+p = pynbody.analysis.profile.Profile(h[0].s, vmin =.01, max=50)
 
 # make the figure and sub plots
 f, axs = plt.subplots(1,2,figsize=(14,6))
 
 # make the plot
 axs[0].plot(p['rbins'],p['density'], 'k')
 axs[0].semilogy()
 axs[0].set_xlabel('R [kpc]')
 axs[0].set_ylabel(r'$\Sigma_{\star}$ [M$_{\odot}$ kpc$^{-2}$]')
+axs[0].set_title("2D stellar density")
 
 # make a 3D density plot of the dark matter (note ndim=3 in the constructor below)
-p = pynbody.analysis.profile.Profile(h[1].d,min=.01,max=50,ndim=3)
+p = pynbody.analysis.profile.Profile(h[0].d,min=.01,max=50,ndim=3)
 
 axs[1].plot(p['rbins'],p['density'], 'k')
 axs[1].semilogy()
 axs[1].set_xlabel('R [kpc]')
 axs[1].set_ylabel(r'$\rho_{DM}$ [M$_{\odot}$ kpc$^{-3}$]')
+axs[1].set_title("3D dark matter density")
```

### Comparing `pynbody-2.0.0b7/docs/tutorials/example_code/do_data.py` & `pynbody-2.0.0b8/docs/tutorials/example_code/do_data.py`

 * *Files identical despite different names*

### Comparing `pynbody-2.0.0b7/docs/tutorials/example_code/do_images.py` & `pynbody-2.0.0b8/docs/tutorials/example_code/do_images.py`

 * *Files identical despite different names*

### Comparing `pynbody-2.0.0b7/docs/tutorials/example_code/do_pictures.py` & `pynbody-2.0.0b8/docs/tutorials/example_code/do_pictures.py`

 * *Files identical despite different names*

### Comparing `pynbody-2.0.0b7/docs/tutorials/example_code/do_plots.py` & `pynbody-2.0.0b8/docs/tutorials/example_code/do_plots.py`

 * *Files identical despite different names*

### Comparing `pynbody-2.0.0b7/docs/tutorials/example_code/do_preamble.py` & `pynbody-2.0.0b8/docs/tutorials/example_code/do_preamble.py`

 * *Files identical despite different names*

### Comparing `pynbody-2.0.0b7/docs/tutorials/example_code/rcs.py` & `pynbody-2.0.0b8/docs/tutorials/example_code/rcs.py`

 * *Files identical despite different names*

### Comparing `pynbody-2.0.0b7/docs/tutorials/example_code/rotcurve.py` & `pynbody-2.0.0b8/docs/tutorials/example_code/rotcurve.py`

 * *Files identical despite different names*

### Comparing `pynbody-2.0.0b7/docs/tutorials/example_code/velocity_vectors.py` & `pynbody-2.0.0b8/docs/tutorials/example_code/velocity_vectors.py`

 * *Files 22% similar despite different names*

```diff
@@ -20,9 +20,9 @@
 sph.velocity_image(h[1].g, vector_color="cyan", qty="temp",width=50,cmap="YlOrRd",
                    denoise=True,approximate_fast=False, subplot=axs[0], show_cbar = False)
 
 #you can also make a stream visualization instead of a quiver plot
 pynbody.analysis.angmom.faceon(h[1])
 s['pos'].convert_units('Mpc')
 sph.velocity_image(s.g, width='3 Mpc', cmap = "Greys_r", mode='stream', units='Msol kpc^-2',
-                   density = 2.0, vector_resolution=100, vmin=1e-1,subplot=axs[1],
+                   stream_density= 2.0, vector_resolution=100, vmin=1e-1, subplot=axs[1],
                    show_cbar=False, vector_color='black')
```

### Comparing `pynbody-2.0.0b7/docs/tutorials/halos.rst` & `pynbody-2.0.0b8/docs/tutorials/halos.rst`

 * *Files 19% similar despite different names*

```diff
@@ -2,372 +2,301 @@
 
 
 .. _halo_tutorial:
 
 Halos in Pynbody
 =======================
 
-Finding the groups of particles that represent galaxies is the key first
-step of simulation analysis.  There are several public group finders
-available today that find these groups of particles.
-``Pynbody`` includes interfaces to several commonly used group finders.
+.. versionchanged:: 2.0
 
-Groups that are virialized are called "halos",
-so groups are available in ``pynbody`` using the
-:class:`~pynbody.snapshot.SimSnap.halos` function on a
-simulation object (``SimSnap``).  When :class:`~pynbody.snapshot.SimSnap.halos`
-is called, ``pynbody`` creates
-a :class:`~pynbody.halo.HaloCatalogue` that consists of
-:class:`~pynbody.halo.Halo` objects.
-The ``Halo`` object holds information about the particle IDs and other properties
-about a given halo.  A :class:`~pynbody.halo.HaloCatalogue` is an
-object is a compilation of all the halos in a given snapshot.
+  Changes to the halo catalogue system, especially affecting AHF
 
-Some possible halo finders that pynbody recognises include:
+  If migrating from version 1.x, please see relevant warnings :ref:`in the reference documentation <v2_0_halo_changes>`.
 
- - `Amiga Halo Finder (AHF) <http://popia.ft.uam.es/AHF/Download.html>`_ (:class:`~pynbody.halo.ahf.AHFCatalogue`);
- -  `Rockstar <https://bitbucket.org/pbehroozi/rockstar-galaxies>`_ (:class:`~pynbody.halo.rockstar.RockstarCatalogue`);
- - SKID (:class:`~pynbody.halo.number_array.HaloNumberCatalogue` class);
- - SubFind (:class:`~pynbody.halo.subfind.SubfindCatalogue`).
 
-The :func:`~pynbody.snapshot.SimSnap.halos` function in
-:class:`~pynbody.snapshot.SimSnap`
-automatically determines whether halo data exists
-on disk already for ``pynbody`` to read, or if it should run a halo
-finder to create halo data.
+Finding the groups of particles that encompass galaxies is the key first
+step of simulation analysis. Generally speaking, groups of particles that are gravitationally bound
+are known as 'halos', while unbound collections of particles are known simply as 'groups'. Some literature
+also talks about 'subhalos', which are smaller groups of particles that are gravitationally bound within
+a larger halo. However, the nomenclature around groups, halos and subhalos is not consistent across the
+literature, and different halo finders may use different terminology. In *pynbody*, we use the term 'halo'
+to refer to *any* group of particles that has been identified by a finder and stored on disk. Thus, a
+*pynbody* :class:`~pynbody.halo.Halo` may represent a halo, a group, or a subhalo, depending on the
+context in which it was created.
 
-This tutorial will show you how to setup and configure pynbody to best use
-the group finder functionality built into pynbody. If you are not familiar with
-``Pynbody`` in general, it is recommended that you first have a look at
-the :ref:`snapshot_manipulation` tutorial.
+There are several public group / halo finders available. Pynbody presents a common interface to these
+to the maximum extent possible. For a list of supported halo finders, see :ref:`supported_halo_finders`.
 
-Configuration
--------------
-
-``Pynbody`` reads a number of different halo formats including the popular
-``subfind``. However, it is most comfortable with either AHF or (more
-experimentally) Rockstar and can in many cases actually run these codes
-for you if you haven't already generated halo catalogues for your simulation.
-
-Rockstar
-^^^^^^^^
+.. note::
 
-To install Rockstar, grab the code from Peter Behroozi's bitbucket
-repository, make it, and copy it into your ``$PATH``
-::
+    The principal development of ``pynbody`` took place in the UK, and the spelling of "catalogue" is British English.
+    However, since much code is written in American English, v2.0.0 introduced aliases such that all
+    classes can be accessed with the American spelling ``HaloCatalog``, ``AdaptaHOPCatalog`` etc.
 
-	> git clone https://bitbucket.org/pbehroozi/rockstar-galaxies.git
-	> cd rockstar-galaxies; make
-	> cp rockstar-galaxies ~/bin/
+To load a catalogue, call the :func:`~pynbody.snapshot.simsnap.SimSnap.halos` method on a loaded
+simulation snapshot. *Pynbody* scans the disk looking for files that follow the naming convention of known
+halo finders.
 
-AHF
-^^^
+For example, with the *pynbody* test data, we can load halo catalogues as follows:
 
-To install AHF, take the most recent version from Alexander Knebe's AHF
-page, uncompress it
-::
+.. ipython::
 
-	> wget http://popia.ft.uam.es/AHF/files/ahf-v1.0-084.tgz
-	> tar zxf ahf-v1.0-084.tgz; cd ahf-v1.0-084
+ In [1]: import pynbody
+    ...: import matplotlib.pylab as plt
 
-Edit Makefile.config appropriate for your code, make AHF,
-and copy it into your $PATH.
-::
+ In [2]: s = pynbody.load('testdata/gasoline_ahf/g15784.lr.01024.gz')
 
-	> make AHF
-	> cp AHF-v1.0-084 ~/bin/
+ In [3]: s.halos()
 
-Now ``pynbody`` will use one of these halo finders to create group files
-you can use to analyze your simulations.
 
-Configuration
-^^^^^^^^^^^^^
+In this case, we have loaded a simulation snapshot from the *Gasoline* code, for which an AHF halo catalogue
+is available. *Pynbody* has automatically detected the presence of the AHF catalogue and loaded it for us.
+Here is another example from the test data:
 
-As described in :ref:`configuration`, you can tell pynbody which group
-finder you prefer in your configuration file, ``~/.pynbodyrc``.  In the ``general``
-section, you can arrange the priority of halo finders to use as you like.
+.. ipython::
 
+ In [5]: s = pynbody.load('testdata/gadget4_subfind_HBT/snapshot_034.hdf5')
 
-Working with Halos and Catalogues
----------------------------------
+ In [6]: s.halos()
 
-We will use the AHF catalogue here since that is the one that is
-available for the sample output in the ``testdata`` bundle. The SubFind specific
-halo / subhalo structure is handled later.
 
-.. ipython::
+The *Gadget4* snapshot has a SubFind halo catalogue, which *pynbody* has loaded for us. However, in this
+particular case there is _also_ and HBT+ catalogue available. To load this, we can specify the halo finder
+priority either in the configuration file (see :ref:`configuration`) or at runtime.
 
- In [1]: import pynbody, matplotlib.pylab as plt
 
- In [2]: s = pynbody.load('testdata/gasoline_ahf/g15784.lr.01024.gz')
+Selecting a format
+------------------
 
- In [3]: s.physical_units()
+If you have more than one halo catalogue available, or if your halo catalogue is not in the default location,
+you need to provide additional information to the :func:`~pynbody.snapshot.simsnap.SimSnap.halos` method.
 
-We've got the snapshot loaded, now we ask ``pynbody`` to load any
-available halo catalogue:
+To specify a particular halo finder, use the ``priority`` keyword argument. For example, to load the HBT+
+catalogue for the *Gadget4* snapshot, we can do:
 
 .. ipython::
 
- In [3]: h = s.halos()
-
-``h`` is the halo catalogue.
-
-.. note:: If the halo finders have to run to find the groups, they may take
-   	some time.  AHF typically takes 5 minutes for a million particle
-	simulation while Rockstar takes 5-10 minutes running on a single
-	processor.
+ In [8]: s.halos(priority=['HBTPlusCatalogue'])
 
-We can easily retrieve some basic
-information, like the total number of halos in this catalogue:
+Notice that *pynbody* has now loaded the HBT+ catalogue instead of the SubFind catalogue.
 
-.. ipython::
-
- In [4]: len(h)
+.. note::
 
-To actually access a halo, use square bracket syntax. For example, the following
-returns the number of particles in halos 1 and 2
+  In the specific case of HBT+, halos are found within the parent groups of a SubFind catalogue. To see the
+  full hierarchy of structure in this snapshot requires using both catalogues together. More information
+  about this is given in :ref:`the reference documentation <hbt_plus_parent_groups>`.
 
-.. ipython::
+For a list of the available halo finders, see :ref:`supported_halo_finders`. You can either pass classes or
+strings naming them to the ``priority`` argument.
 
- In [5]: len(h[1]), len(h[2])
+As described in :ref:`configuration`, you can also tell pynbody which group finders you prefer in your configuration
+file. The ``priority`` argument is used to override this default preference at runtime.
 
-The catalogue has halos ordered by number of particles, so the first
-halo for this zoom simulation will be the one we would most likely be
-interested in. Halo IDs begin with 1 for many halo finders (including AHF,
-which is the sample file being used here).
+Specifying locations
+--------------------
 
-As may now be evident, "halos" are treated using the
-:class:`~pynbody.snapshot.SubSnap` class. The syntax for dealing
-with an individual halo therefore precisely mirrors the syntax for
-dealing with an entire simulation. For example, we can get the total mass
-in halo 1 and see the position of its first few particles as follows:
+If your halo catalogue is not in the default location, it probably will not be found automatically when you call
+the :meth:`pynbody.snapshot.simsnap.SimSnap.halos` method. You can therefore specify the path to the catalogue using the
+``filename`` keyword argument. This also functions as an alternative way to disambiguate between multiple
+halo catalogues. For example:
 
 .. ipython::
 
- In [10]: h[1]['mass'].sum().in_units('1e12 Msol')
+ In [10]: s.halos(filename='testdata/gadget4_subfind_HBT/034/SubSnap_034.0.hdf5')
+ Out[10]: <HBTPlusCatalogue, length 2349>
 
- In [8]: h[1]['pos'][:5]
+ In [11]: h = s.halos(filename='testdata/gadget4_subfind_HBT/fof_subhalo_tab_034.hdf5')
 
-A really common use-case is that one wants to center the simulation on
-a given halo and analyze some of its properties. Since halos are just
-:class:`~pynbody.snapshot.SubSnap` objects, this is easy to do:
+ In [12]: h
+ Out[12]: <SubFindHDFCatalogue, length 2517>
 
-.. ipython::
+.. note::
 
- In [1]: pynbody.analysis.halo.center(h[1])
+    Some halo finders produce multiple files, so the ``filename`` keyword argument
+    is necessarily interpreted slightly differently by some readers. As a general
+    guideline, if the halo finder output is of the form ``path/to/file.extension``,
+    ``path/to/file.another_extension`` etc, then the ``filename``argument should
+    be the path to the basename (i.e.``path/to/file``). For specific help, consult the reference
+    documentation for the specific halo finder's ``__init__``; a list of these is available in
+    :ref:`supported_halo_finders`.
 
- @savefig halo1_image.png width=5in
- In [2]: im = pynbody.plot.image(h[1].d, width = '500 kpc', cmap=plt.cm.Greys, units = 'Msol kpc^-2')
 
+Information about the catalogue
+-------------------------------
 
-Halo catalogue information
---------------------------
+We will continue to use the Gadget4/SubFind sample catalogue for the following examples, and we
+assigned this to the variable ``h`` above.
 
-Any additional information generated by the halo finder
-is available through the ``properties`` dictionary associated with halos. For
-example
+We can easily retrieve some basic information, like the total number of halos in this catalogue:
 
 .. ipython::
 
- In [5]: h[1].properties['children']
+ In [4]: len(h)
 
-returns a list of sub-halos of this halo. Here there are no sub-halos, so
-we've been returned an empty list. To see everything that is
-known about the halo one can use the standard python dictionary method ``keys``:
+To access the particle members of a halo, use square bracket syntax. For example, the following
+returns the number of particles in the first two halos, use
 
 .. ipython::
 
- In [6]: h[1].properties.keys()
-
-
-Dealing with big simulations and lots of halos
-----------------------------------------------
+ In [5]: len(h[0]), len(h[1])
+ Out[5]: (307386, 137037)
+.. note ::
 
-Sometimes, simulations are too large to fit in the memory of your analysis
-machine. On the other hand, pynbody never actually loads particle data until
-it's needed so it is possible to load a halo catalogue anyway.
+   Halo numbers to use are assigned by the halo finder, unless overriden by the user. Here, the first halo
+   is halo 0, but that need not have been the case.
 
-Consider the following example.
+As may now be evident, the syntax for dealing with particles within an individual halo precisely mirrors the
+syntax for dealing with an entire simulation. For example, we can get the total mass
+in the first halo and see the position of its first few particles as follows:
 
 .. ipython::
 
- In [2]: f = pynbody.load("testdata/gasoline_ahf/g15784.lr.01024")
+ In [10]: h[0]['mass'].sum().in_units('1e12 Msol')
 
- In [3]: h = f.halos()
+ In [11]: h[0]['pos'][:5]
 
- In [4]: h[2].properties['mass']/1e12 # another property calculated by AHF in Msol/h
+We might also be interested in the properties that a halo finder has calculated for each halo. For example,
+SubFind calculates various masses and names them ``GroupMass``. This is accessible in the following way:
 
- In [5]: len(h[2])
+.. ipython::
 
-At no point does this load data from the simulation file; it only accesses the
-halo catalogue. In fact, with some formats (including AHF, which is what's
-in our sample test data here), you can specify ``dummy=True`` to load only the
-properties dictionary:
+     In [12]: h[0].properties['GroupMass']
 
-.. ipython:: :okexcept:
+Here, the units are currently not very user-friendly. Just as with a simulation snapshot, we can convert
+the units in a halo catalogue to something more useful:
 
- In [3]: h = f.halos(dummy=True)
+.. ipython::
 
- In [4]: h[2].properties['mass'] # this is still OK
+     In [13]: h.physical_units()
 
- In [5]: len(h[2]) # this, of course, is unknown
+     In [14]: h[0].properties['GroupMass']
 
-.. note::
+Calling :meth:`~pynbody.halo.HaloCatalogue.physical_units` on a halo catalogue object will convert all
+properties, and additionally all particle data, to the default pynbody units or a different set of units
+if specified. The call signature is the same as for
+:meth:`SimSnap.physical_units <pynbody.snapshot.simsnap.SimSnap.physical_units>`.
 
- The remainder of this section requires the underlying snapshot loader
- to support partial loading, which is currently only the case for *tipsy*
- and *nchilada* formats. See :ref:`loaders`.
-
-Combined with pynbody's partial-loading system, one can go further and
-pull only a single halo into your computer's memory at once. The following
-example shows you how:
+For halo finders such as SubFind that support a hierarchical view of the structure, a ``subhalos`` attribute
+is provided:
 
 .. ipython::
 
- In [1]: h2data = h.load_copy(2)
+ In [6]: subhalos_of_0 = h[0].subhalos
 
- In [2]: len(h2data) # this is correct again
+ In [7]: subhalos_of_0
 
- In [3]: h2data['mass']
+The ``subhalos_of_0`` object behaves just like a regular catalogue, but it only contains the specified subhalos.
+So, for example, we can see the number of particles in the first subhalo, and its mass:
 
-As you can see from the last line, you can now access particle arrays
-but the key difference is that ``h2data`` as constructed above only loads the
-particles that are required. Conversely
-accessing arrays
-directly from ``h[2]`` actually loads the full simulation array into memory, even
-if only part of it is ever going to be used.
+.. ipython::
 
+ In [8]: len(subhalos_of_0[0]), subhalos_of_0[0].properties['SubhaloMass']
 
+.. note::
 
+    **SubFind-specific information**
 
-Write halo catalog (i.e. convert AHF outfiles to tipsy format)
---------------------------------------------------------------
+    SubFind distinguishes sharply between parent halos (known as FOF groups) and subhalos. Even the properties are
+    different. For example, the mass of a subhalo is stored in the ``SubhaloMass`` property, while the mass of a
+    parent halo is stored in the ``GroupMass`` property, as above.
 
-Tipsy is a particle viewer.  A tipsy format file can be useful for
-quick viewing in tipsy to check whether the AHF halo finder did
-anything sensible. Write the (ahf) halo catalog to disk. Former idl
-users might notice that this produces outfiles similar to 'Alyson's
-idl script'.
+    The subhalos are not even available from the parent halo catalogue itself, i.e. running through all the
+    halos in ``h`` will not give you the subhalos, in contrast to some other halo finders. If you want to be able to
+    run through all subhalos within the entire simulation, you can load the subhalo catalogue directly using
 
-The 3 written file types are:
+    .. code-block:: python
 
-1.   .gtp (tipsy file with halos as star particles);
-2.   .grp (ascii halo id of every snapshot particle, 0 if none);
-3.   .stat (ascii condensed version of AHF halos file).
+        all_subhalos = s.halos(subhalos=True)
 
-This halo file set emulates the halo finder SKID. Tipsy and skid can be found at
-`<http://www-hpcc.astro.washington.edu/tools/>`_.
 
+Accessing particle data
+-----------------------
 
-Working with SubFind Halos and Subhalos
----------------------------------------
+When accessing halos in the above way, the particle data is also available. The object returned by ``h[0]``, ``h[1]``
+etc is actually a :class:`~pynbody.halo.Halo` object, which is a subclass of :class:`~pynbody.snapshot.SubSnap`,
+which in turn is a subclass of :class:`~pynbody.snapshot.simsnap.SimSnap`.
 
-If using the Gadget3 SubFind HDF5 output (for example, OWLS / Eagle or Smaug sims)
-most of the examples from AHF above can be used, except for the subhalos structure.
-One major change is that the halo catalogue is a separate file to the snapshot.
+This means that you can access the particle data as though the halo were a simulation snapshot. For example, to get
+the particle masses of the first halo:
 
 .. ipython::
 
- In [1]: import pynbody, matplotlib.pylab as plt
-
- In [2]: s = pynbody.load('testdata/gadget3/data/snapshot_103/snap_103.hdf5')
-
- In [3]: s.physical_units()
+ In [11]: h[0]['mass']
 
-We've got the snapshot loaded and can access the particle data in any manner we
-like as usual but unlike AHF we can't load halos. Instead to get ``pynbody``
-to load the halo catalogue we have to access the subfind output directly:
+We can verify that this agrees with the halo-finder-calculated mass:
 
 .. ipython::
 
- In [3]: s = pynbody.load('testdata/gadget3/data/subhalos_103/subhalo_103')
-
- In [2]: s.physical_units()
-
- In [4]: h = s.halos()
+ In [12]: h[0]['mass'].sum()
 
-``h`` is the Friends-of-Friends (FOF) halo catalogue, upon which SubFind is based.
+ In [13]: h[0].properties['GroupMass']
 
-As with the AHF example we can easily retrieve some basic
-information, like the total number of halos in this catalogue:
+The same is true for positions, velocities, etc. For example, to get the positions of the first 5 particles in the
+first halo:
 
 .. ipython::
 
- In [5]: len(h), h.ngroups, h.nsubhalos
+ In [14]: h[0]['pos'][:5]
 
-Where the last value is the number of subhalos, see next section on these.
-To actually access a halo, use square bracket syntax as before.
-For example, the following returns the number of particles in halos 1 and 2
+The same syntax can be used to access the particle data of subhalos. For example, to get the velocities of the first
+5 particles in the first subhalo of the first halo:
 
 .. ipython::
 
- In [6]: len(h[1]), len(h[2])
+ In [15]: h[0].subhalos[0]['vel'][:5]
 
-The catalogue has FOF halos ordered by number of particles, so the first
-halo for this small box simulation will be the largest object.
-Halo IDs begin with 0 for SubFind / FOF unlike AHF.
 
-The "halos" are treated using the
-:class:`~pynbody.snapshot.gadgethdf.SubFindHDFSnap` class. The syntax for dealing
-with an individual halo is the same as AHF and the snapshot simulation.
-For example, we can get the total mass in the second FOF halo
-and see the position of its first few particles as follows:
 
-.. ipython::
-
- In [7]: h[1]['mass'].sum().in_units('1e12 Msol')
+Working with large numbers of halos
+-----------------------------------
 
- In [8]: h[1]['pos'][:5]
+Most halo finders will produce a large number of halos. Sometimes we are only interested in accessing a few, in
+which case the approaches above are sufficient. If, however, we access several in a row, *pynbody* may issue
+a warning unless one first calls :meth:`~pynbody.halo.HaloCatalogue.load_all` to load all the halo data into memory.
+This is because *pynbody* is loading the data for each halo as it is accessed,
+and while this is efficient for a small number of halos, it can be slow if done repeatedly.
 
-A really common use-case is that one wants to center the simulation on
-a given halo and analyze some of its properties:
+Once in memory, the data can be accessed without further warnings. For example, to calculate the velocity
+dispersion in each of a number of halos, we can do:
 
 .. ipython::
 
- In [9]: pynbody.analysis.halo.center(h[1], vel=False)
-
- @savefig halo1_image_subfind.png width=5in
- In [10]: im = pynbody.plot.image(h[1].d, width = '40 kpc', cmap=plt.cm.Greys, units = 'Msol kpc^-2')
+  In [15]: h.load_all()
 
+  In [16]: h[0]['vel'].std() # for one
 
-Subhalo catalogue information
------------------------------
+  In [17]: v_std = [halo_i['vel'].std() for halo_i in h[:100]] # for the first 100
 
-After the FOF group has been found, SubFind runs on this reduced particle list
-to determine gravitational bound substructures (or subhalos) within the larger FOF halo.
-To access the list of subhalos simply call:
+If we are interested in finder-calculated properties, there is an even faster way to access them without ever
+constructing individual halo particle data objects. For example, to get the masses of halos, we can do:
 
 .. ipython::
 
- In [11]: h[1].sub[:]
+ In [18]: h.get_properties_one_halo(0)['GroupMass'] # for one, without touching any particles
 
-to return a list of sub-halos of this halo. Then one can select subhalo particles as
-before (e.g. dark matter velocities):
-
-.. ipython::
+ In [19]: masses = h.get_properties_all_halos()['GroupMass'][:100] # for first 100, without touching any particles
 
- In [12]: h[1].sub[0].d['vel']
-
-for the main (i.e. first) subhalo of the second FOF halo. As with AHF additional halo
-catalogue values such as the centre of mass, or the velocity dispersion, can be accessed
-by the properties list for each halo / subhalo. Note that the subhalo properties list
-is far more extensive than the FOF halo:
+This is much faster than constructing individual halo objects, and is the recommended way to access finder-calculated
+properties when you are not interested in the particle data. We can now take a look at the velocity dispersion as
+a function of mass in this halo catalogue:
 
 .. ipython::
 
- In [13]: h[2].properties
-
- In [14]: h[2].properties['CenterOfMass']
+ @suppress
+ In [20]: plt.clf()
 
- In [15]: h[2].sub[4].properties
+ In [20]: plt.plot(masses, v_std, 'o')
 
- In [16]: h[2].sub[4].properties['CenterOfMass']
+ In [21]: plt.xlabel(r'Mass / $M_{\odot}$')
 
-To access the entire dataset of a given property (say all of the Stellar
-Velocity Dispersions) requires an embedded for loop over the HDF5 catalogue and
-appending to an array:
+ In [21]: plt.ylabel(r'rms velocity / $\mathrm{km/s}$')
 
-.. ipython::
+ @savefig masses_vs_vels.png width=5in
+ In [21]: plt.loglog()
 
- In [17]: SubStellarVelDisp = [[subhalo.properties['SubStellarVelDisp'] for subhalo in halo.sub] for halo in h]
+.. note::
 
- In [19]: SubStellarVelDisp[5]
+    Pynbody includes infrastructure for analysing large simulations and halo catalogues using parallel processing.
+    This is used
+    by its sister project, `tangos <https://pynbody.github.io/tangos/>`_, which offers a way to collate and analyse
+    halo data across different timesteps and simulations, generating rich interactive databases which can then be
+    queried and visualised in a variety of ways.
```

### Comparing `pynbody-2.0.0b7/docs/tutorials/performance.rst` & `pynbody-2.0.0b8/docs/tutorials/performance.rst`

 * *Files identical despite different names*

### Comparing `pynbody-2.0.0b7/docs/tutorials/pictures.rst` & `pynbody-2.0.0b8/docs/tutorials/pictures.rst`

 * *Files identical despite different names*

### Comparing `pynbody-2.0.0b7/docs/tutorials/threads.rst` & `pynbody-2.0.0b8/docs/tutorials/threads.rst`

 * *Files identical despite different names*

### Comparing `pynbody-2.0.0b7/docs/tutorials/tutorials.rst` & `pynbody-2.0.0b8/docs/tutorials/tutorials.rst`

 * *Files 27% similar despite different names*

```diff
@@ -1,62 +1,89 @@
+.. Last checked by AP: 18 Mar 2024
+
 .. pynbody tutorials main index
 
 .. _tutorials:
 
 Pynbody Tutorials
 =================
 
 Here you will find tutorials that illustrate the use of pynbody. The
 :ref:`walkthroughs` demonstrate pynbody functionality through an
 interactive session in the ipython shell that you can follow along
 using either one of the outputs from the bundled test-data or one of
 your own simulations. To complement the walkthroughs, we also provide
-a few `IPython notebooks
-<https://github.com/pynbody/pynbody/tree/master/examples/notebooks>`_. The
+a quick-start `Jupyter notebook
+<https://github.com/pynbody/pynbody/blob/master/examples/pynbody_demo.ipynb>`_. The
 :ref:`cookbook` tutorials are more goal-oriented: they provide a
 script that can be used with only minor modifications to immediately
 produce a result (i.e. make an image). They also include, however, a
 somewhat more involved discussion of more advanced options and common
 pitfalls. Finally, the :ref:`advanced_topics` section is meant to
 provide a more in-depth look at the inner-workings of the code.
 
+.. _obtaining_testdata:
+
+Obtaining test data
+-------------------
+
+Many of the tutorials below use the same dataset that pynbody is tested on. While they are easily adapted for your
+own data, you can also download and unpack the test data to replicate the examples exactly. To do this, perform the
+following steps:
+
+1. Download the testdata tarball from `here <http://star.ucl.ac.uk/~app/testdata.tar.gz>`_. This is approximately 2.0GB.
+   From a command line, you can do this with the command
+
+   .. code:: bash
+
+       $ wget http://star.ucl.ac.uk/~app/testdata.tar.gz
+
+2. Unpack the tarball in a directory of your choice. This will create a directory called ``testdata``.
+
+   .. code:: bash
+
+       $ tar -xzf testdata.tar.gz
+
+3. Launch python, ipython or jupyter from the directory where you unpacked the tarball. You can then follow the tutorials
+   below, using the ``testdata`` directory as the root of your data.
+
 .. _walkthroughs:
 
 Walkthroughs
 ------------
 
 .. toctree::
    :maxdepth: 1
 
-   A first look at your data with pynbody <snapshot_manipulation>
-   Basic data access <data_access>
-   Subviews and Filters <filters>
-   Tracing particles across different snapshots <bridge>
+   Quick-start <quickstart>
+   Reading snapshots <data_access>
+   Sub-views & filters <filters>
+   Halos & groups <halos>
+   Linking snapshots <bridge>
 
 .. _cookbook:
 
 Cookbook/Recipes
 ----------------
 
 .. toctree::
    :maxdepth: 1
 
    Profiles <profile>
-   Rotation curves <rotation_curve>
-   Making Pictures <pictures>
-   Group finding <halos>
-   Halo mass Function <hmf>
+   Images <images>
+   Halo mass function <hmf>
 
 
 .. _advanced_topics:
 
 Advanced topics
 ---------------
 
 These tutorials are likely to be of interest only in special cases.
 
 .. toctree::
    :maxdepth: 1
 
-   Performance issues <performance>
-   Configuring Pynbody <configuration>
-   Understanding threading <threads>
+   Performance <performance>
+   Derived quantities <derived>
+   Configuration <configuration>
+   Threading/multiprocessing <threads>
```

### Comparing `pynbody-2.0.0b7/pynbody/__init__.py` & `pynbody-2.0.0b8/pynbody/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -69,12 +69,12 @@
     def __repr__(self):
         return "<Unloaded plot module>"
 
 plot = PlotModuleProxy()
 
 from .snapshot import load, new
 
-derived_array = snapshot.simsnap.SimSnap.derived_quantity
+derived_array = snapshot.simsnap.SimSnap.derived_array
 
-__version__ = '2.0.0-beta.7'
+__version__ = '2.0.0-beta.8'
 
 __all__ = ['load', 'new', 'derived_array']
```

### Comparing `pynbody-2.0.0b7/pynbody/analysis/CAMB_WMAP7` & `pynbody-2.0.0b8/pynbody/analysis/CAMB_WMAP7`

 * *Files identical despite different names*

### Comparing `pynbody-2.0.0b7/pynbody/analysis/_com.pyx` & `pynbody-2.0.0b8/pynbody/analysis/_com.pyx`

 * *Files 24% similar despite different names*

```diff
@@ -1,23 +1,25 @@
 cimport cython
 cimport numpy as np
 
 import logging
+import math
 
 import numpy as np
 from cython.parallel import prange
 
 logger = logging.getLogger('pynbody.analysis._com')
 
 
 @cython.boundscheck(False)
 @cython.wraparound(False)
 def shrink_sphere_center(np.ndarray[np.float64_t, ndim=2] pos,
                          np.ndarray[np.float64_t, ndim=1] mass,
                          int min_particles,
+                         int particles_for_second_radius,
                          float shrink_factor,
                          float starting_rmax,
                          int num_threads,
                          int itermax=1000) :
 
     cdef int npart = len(pos)
     cdef int npart_all = len(pos)
@@ -30,15 +32,17 @@
     cdef float current_rmax = np.inf, current_rmax2
     cdef double cx, cy, cz
     cdef double offset_x, offset_y, offset_z
     cdef double pix, piy, piz, mi
 
     logger.info("Initial rough COM=%s",com_x)
 
-    while npart>min_particles :
+    second_radius = None
+
+    while True :
         offset_x=0; offset_y=0; offset_z=0;
         cx=com_x[0]; cy=com_x[1]; cz=com_x[2]
         current_rmax2 = current_rmax*current_rmax
         with nogil:
             npart = 0
             for i in prange(npart_all, schedule='static', num_threads=num_threads):
                 pix=pos[i,0]-cx; piy=pos[i,1]-cy; piz=pos[i,2]-cz
@@ -47,91 +51,24 @@
                     mi = mass[i]
                     offset_x+=pix*mi
                     offset_y+=piy*mi
                     offset_z+=piz*mi
                     tot_mass+=mi
                     npart+=1
 
-        if npart==0:
-            return com_x
-
-
-        # divide out total mass and shift
-        com[0]=cx+offset_x/tot_mass; com[1]=cy+offset_y/tot_mass; com[2]=cz+offset_z/tot_mass
-
-
-
-        # update for next cycle
-        com_x[:]= com
-        com[:]=0
-        tot_mass=0
-
-        iternum+=1
-        if iternum>1 :
-            current_rmax*=shrink_factor
-        else :
-            current_rmax = starting_rmax
+        if npart < particles_for_second_radius and second_radius is None:
+            second_radius = math.sqrt(current_rmax2)
 
-        if iternum>itermax:
-            raise RuntimeError, "shrink_sphere_center failed to converge after %d iterations"%itermax
 
-    return com_x
+        if npart<min_particles:
+            break
 
-@cython.boundscheck(False)
-@cython.wraparound(False)
-def move_sphere_center(np.ndarray[np.float64_t, ndim=2] pos,
-                       np.ndarray[np.float64_t, ndim=1] mass,
-                       int min_particles,
-                       float shrink_factor,
-                       float starting_rmax,
-                       int num_threads,
-		       float tol,
-                       int itermax=1000) :
-
-    cdef int npart = len(pos)
-    cdef int npart_all = len(pos)
-    cdef float r = 0
-    cdef float tot_mass=0
-    cdef np.ndarray[np.float64_t, ndim=1] com = np.zeros(3)
-    cdef np.ndarray[np.float64_t, ndim=1] com_x = pos.mean(axis=0)
-    cdef int i
-    cdef int iternum=0
-    cdef float current_rmax = np.inf
-    cdef double cx, cy, cz
-    cdef double nx, ny, nz
-    cdef double pix, piy, piz, mi
-
-    logger.info("Initial rough COM=%s",com_x)
-
-    ocen=np.zeros(3)
-    while np.sqrt(((com_x-ocen)**2).sum())<=tol: ocen+=1.0
-
-    while np.sqrt(((com_x-ocen)**2).sum())>tol :
-        nx=0; ny=0; nz=0;
-        cx=com_x[0]; cy=com_x[1]; cz=com_x[2]
-        ocen = com_x
-        with nogil:
-            npart = 0
-            for i in prange(npart_all, schedule='static', num_threads=num_threads):
-                pix=pos[i,0]-cx; piy=pos[i,1]-cy; piz=pos[i,2]-cz
-                r = pix*pix+piy*piy+piz*piz
-                if r<current_rmax :
-                    mi = mass[i]
-                    nx+=pix*mi
-                    ny+=piy*mi
-                    nz+=piz*mi
-                    tot_mass+=mi
-                    npart+=1
-
-        if npart==0:
-            return com_x
 
         # divide out total mass and shift
-        com[0]=cx+nx/tot_mass; com[1]=cy+ny/tot_mass; com[2]=cz+nz/tot_mass
-
+        com[0]=cx+offset_x/tot_mass; com[1]=cy+offset_y/tot_mass; com[2]=cz+offset_z/tot_mass
 
 
 
         # update for next cycle
         com_x[:]= com
         com[:]=0
         tot_mass=0
@@ -141,8 +78,8 @@
             current_rmax*=shrink_factor
         else :
             current_rmax = starting_rmax
 
         if iternum>itermax:
             raise RuntimeError, "shrink_sphere_center failed to converge after %d iterations"%itermax
 
-    return com_x
+    return com_x, current_rmax, second_radius
```

### Comparing `pynbody-2.0.0b7/pynbody/analysis/_interpolate3d.pyx` & `pynbody-2.0.0b8/pynbody/analysis/_interpolate3d.pyx`

 * *Files identical despite different names*

### Comparing `pynbody-2.0.0b7/pynbody/analysis/cambtemplate.ini` & `pynbody-2.0.0b8/pynbody/analysis/cambtemplate.ini`

 * *Files identical despite different names*

### Comparing `pynbody-2.0.0b7/pynbody/analysis/cmdlum.npz` & `pynbody-2.0.0b8/pynbody/analysis/cmdlum.npz`

 * *Files identical despite different names*

### Comparing `pynbody-2.0.0b7/pynbody/analysis/cosmology.py` & `pynbody-2.0.0b8/pynbody/analysis/cosmology.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,13 +1,9 @@
 """
-
-cosmology
-=========
-
-A set of functions for common cosmological calculations.
+Functions for common cosmological calculations.
 
 """
 
 import math
 
 import numpy as np
 import scipy
@@ -33,93 +29,93 @@
 def _da_dtau(a, h0, om_m, om_l):
     return a**2 * _a_dot(a, h0, om_m, om_l)
 
 def _da_dtau_recip(*args):
     return 1. / _da_dtau(*args)
 
 
-def hzoverh0(a, omegam0):
+def _hzoverh0(a, omegam0):
     """ returns: H(a) / H0  = [omegam/a**3 + (1-omegam)]**0.5 """
     return np.sqrt(omegam0 * np.power(a, -3) + (1. - omegam0))
 
 
 def _lingrowthintegrand(a, omegam0):
     """ (e.g. eq. 8 in lukic et al. 2008)   returns: da / [a*H(a)/H0]**3 """
-    return np.power((a * hzoverh0(a, omegam0)), -3)
+    return np.power((a * _hzoverh0(a, omegam0)), -3)
 
 
 def _lingrowthfac(red, omegam0, omegal0, return_norm=False):
     """
     returns: linear growth factor, b(a) normalized to 1 at z=0, good for flat lambda only
     a = 1/1+z
     b(a) = Delta(a) / Delta(a=1)   [ so that b(z=0) = 1 ]
     (and b(a) [Einstein de Sitter, omegam=1] = a)
 
     Delta(a) = 5 omegam / 2 H(a) / H(0) * integral[0:a] [da / [a H(a) H0]**3]
     equation  from  peebles 1980 (or e.g. eq. 8 in lukic et al. 2008) """
-# need to add w ~= , nonflat, -1 functionality
+
+    # need to add w ~= , nonflat, -1 functionality
 
     import scipy.integrate
 
     if (abs(omegam0 + omegal0 - 1.) > 1.e-4):
         raise RuntimeError("Linear growth factors can only be calculated for flat cosmologies")
 
     a = 1 / (1. + red)
 
     # 1st calc. for z=z
     lingrowth = scipy.integrate.quad(_lingrowthintegrand, 0., a, (omegam0))[0]
-    lingrowth *= 5. / 2. * omegam0 * hzoverh0(a, omegam0)
+    lingrowth *= 5. / 2. * omegam0 * _hzoverh0(a, omegam0)
 
     # then calc. for z=0 (for normalization)
     a0 = 1.
     lingrowtha0 = scipy.integrate.quad(
         _lingrowthintegrand, 0., a0, (omegam0))[0]
-    lingrowtha0 *= 5. / 2. * omegam0 * hzoverh0(a0, omegam0)
+    lingrowtha0 *= 5. / 2. * omegam0 * _hzoverh0(a0, omegam0)
 
     lingrowthfactor = lingrowth / lingrowtha0
     if return_norm:
         return lingrowthfactor, lingrowtha0
     else:
         return lingrowthfactor
 
 
 def linear_growth_factor(f, z=None):
-    """Calculate the linear growth factor b(a), normalized to 1
-    at z=0, for the cosmology of snapshot f.
+    """Calculate the linear growth factor b(a), normalized to 1 at z=0, for the cosmology of snapshot f.
 
-    The output is dimensionless. If a redshift z is
-    specified, it is used in place of the redshift in
+    The output is dimensionless. If a redshift z is specified, it is used in place of the redshift in
     output f.
     """
     if z is None:
         z = f.properties['z']
     omegam0 = f.properties['omegaM0']
     omegal0 = f.properties['omegaL0']
     return _lingrowthfac(z, omegam0, omegal0)
 
 
 def rate_linear_growth(f, z=None, unit='h Gyr^-1'):
-    """Calculate the linear growth rate b'(a), normalized
-    to 1 at z=0, for the cosmology of snapshot f.
+    """Calculate the linear growth rate b'(a), normalized to 1 at z=0, for the cosmology of snapshot f.
+
+    The output is in 'h Gyr^-1' by default, but other units can be specified. If a redshift z is specified,
+    it is used in place of the redshift in output f.
 
-    The output is in 'h Gyr^-1' by default. If a redshift z is specified,
-    it is used in place of the redshift in output f."""
+    """
 
     if z is None:
         z = f.properties['z']
     a = 1. / (1. + z)
     omegam0 = f.properties['omegaM0']
     omegal0 = f.properties['omegaL0']
 
     b, X = _lingrowthfac(z, omegam0, omegal0, return_norm=True)
     I = _lingrowthintegrand(a, omegam0)
 
     term1 = -(1.5 * omegam0 * a ** -3) * b / \
         math.sqrt(1. - omegam0 + omegam0 * a ** -3)
-    term2 = (2.5 * omegam0) * hzoverh0(a, omegam0) ** 2 * a * I / X
+    term2 = (2.5 * omegam0) * _hzoverh0(a, omegam0) ** 2 * a * I / X
 
     res = units.h * (term1 + term2) * 100. * units.Unit("km s^-1 Mpc^-1")
 
     return res.in_units(unit, **f.conversion_context())
 
 
 def _test_rate_linear_growth(f, z=None, unit='h Gyr^-1'):
@@ -140,31 +136,39 @@
     dt = age(f, z1, unit ** -1) - age(f, z0, unit ** -1)
 
     return db / dt
 
 
 def age(f, z=None, unit='Gyr'):
     """
-    Calculate the age of the universe in the snapshot f
-    by integrating the Friedmann equation.
+    Calculate the age of the universe in the snapshot f by integrating the Friedmann equation.
 
-    The output is given in the specified units. If a redshift
-    z is specified, it is used in place of the redshift in the
+    The output is given in the specified units. If a redshift z is specified, it is used in place of the redshift in the
     output f.
 
-    **Input**:
+    If a long array of redshifts is provided, interpolation is used to speed up the calculation. Specifically,
+    the number of interpolation points is controlled by the configuration parameter 'cosmo-interpolation-points'.
+
+    Parameters
+    ----------
 
-    *f*: SimSnap
+    f : SimSnap
+        The snapshot from which to obtain the cosmological parameters.
 
-    **Optional Keywords**:
+    z : float, list, or np.ndarray, optional
+        The redshift(s) at which to calculate the age of the universe. If None, the redshift of the snapshot is used.
 
-    *z (None)*: desired redshift. Can be a single number, a list, or a
-    np.ndarray.
+    unit : str, optional
+        The units in which to return the age of the universe. Default is 'Gyr'.
 
-    *unit ('Gyr')*: desired units for age output
+    Returns
+    -------
+
+    SimArray | float
+        The age of the universe at the specified redshift(s).
 
     """
     if z is None:
         z = f.properties['z']
 
     h0 = f.properties['h']
     omM = f.properties['omegaM0']
@@ -188,69 +192,92 @@
             results = np.array([get_age(_z) for _z in z])
         results = results.view(SimArray)
         results.units = unit
         return results
     else:
         return get_age(z)
 
-def tau(f, z=None):
+def tau(f, z=None, unit="Gyr"):
     """
-    Calculate the conformal time of the universe in the snapshot f
-    by integrating the Friedmann equation.
+    Calculate the conformal age of the universe in the snapshot f by integrating the conformal Friedmann equation.
 
-    The output is given in the specified units. If a redshift
-    z is specified, it is used in place of the redshift in the
+    The output is given in the specified units. If a redshift z is specified, it is used in place of the redshift in the
     output f.
 
-    **Input**:
+    Parameters
+    ----------
+
+    f : SimSnap
+        The snapshot from which to obtain the cosmological parameters.
 
-    *f*: SimSnap
+    z : float, list, or np.ndarray, optional
+        The redshift(s) at which to calculate the age of the universe. If None, the redshift of the snapshot is used.
+
+    unit : str, optional
+        The units in which to return the age of the universe. Default is 'Gyr'.
+
+    Returns
+    -------
+
+    SimArray | float
+        The conformal age of the universe at the specified redshift(s).
 
-    **Optional Keywords**:
 
-    *z (None)*: desired redshift. Can be a single number, a list, or a
-    np.ndarray.
     """
     if z is None:
         z = f.properties['z']
 
     h0 = f.properties['h']
     omM = f.properties['omegaM0']
     omL = f.properties['omegaL0']
 
+    conv = units.Unit("0.01 s Mpc km^-1").ratio(unit, **f.conversion_context())
+
     @np.vectorize
     def get_tau(z):
         aexp = 1.0 / (1.0 + z)
         return scipy.integrate.quad(
             _da_dtau_recip,
             1,
             aexp,
             args=(h0, omM, omL)
         )[0]
 
-    return get_tau(z)
+    results = (get_tau(z) * conv)
+
+    if isinstance(results, np.ndarray):
+        results = results.view(SimArray)
+        results.units = unit
+
+    return results
 
 
 @units.takes_arg_in_units((1, "Gyr"), context_arg=0)
 def redshift(f, time):
     """
-    Calculate the redshift given a snapshot and a time since Big Bang
-    in Gyr.
+    Calculate the redshift given a snapshot and a time since Big Bang in Gyr.
 
     Uses scipy.optimize.newton to do the root finding if number of
-    elements in the time array is less than 1000, otherwise uses a linear
+    elements in the time array is less than 1000; otherwise uses a linear
     interpolation.
 
 
-    **Input**:
+    Parameters
+    ----------
+
+    f : SimSnap
+        The snapshot from which to obtain the cosmological parameters.
 
-    *f*: SimSnap with cosmological parameters defined
+    time : float, list, or np.ndarray
+        The time(s) since the Big Bang at which to calculate the redshift.
 
-    *time*: time since the Big Bang in Gyr for which a redshift should
-     be returned. float, list, or np.ndarray
+    Returns
+    -------
+    float or np.ndarray
+        The redshift(s) corresponding to the input time(s).
 
     """
 
     from scipy.interpolate import interp1d
     from scipy.optimize import newton
 
     def func(x, sim, time):
@@ -265,30 +292,44 @@
         else:
             return np.array([newton(func, 1, args=(f, x)) for x in time])
     else:
         return newton(func, 1, args=(f, time))
 
 
 def rho_crit(f, z=None, unit=None):
-    """Calculate the critical density of the universe in
-    the snapshot f.
+    """Calculate the critical density of the universe in the snapshot f.
+
+    .. warning ::
+        You can get slightly confusing results if your simulation is in comoving units and you specify a different
+        redshift z. Specifically, the physical density for the redshift you specify is calulated, but expressed as
+        a comoving density *at the redshift of the snapshot*. This is intentional, but can be surprising.
+
+    Parameters
+    ----------
+
+    f : SimSnap
+        The snapshot from which to obtain the cosmological parameters.
+
+    z : float, optional
+        The redshift at which to calculate the critical density. If None, the redshift of the snapshot is used.
+
+    unit : str, optional
+        The units in which to return the critical density. If None, the returned density will be in the units of
+        f["mass"].units/f["pos"].units**3. If that unit cannot be calculated, the returned units are Msol kpc^-3
+        comoving.
+
+    Returns
+    -------
 
-    z specifies the redshift. If z is none, the redshift of the
-    provided snapshot is used.
+    float
+        The critical density of the universe at the specified redshift.
 
-    unit specifies the units of the returned density. If unit is None,
-    the returned density will be in the units of
-    f["mass"].units/f["pos"].units**3. If that unit cannot be calculated,
-    the returned units are Msol kpc^-3 comoving.
-
-    Note that you can get slightly confusing results if your
-    simulation is in comoving units and you specify a different
-    redshift z. Specifically, the physical density for the redshift
-    you specify is calulated, but expressed as a comoving density *at
-    the redshift of the snapshot*. This is intentional behaviour."""
+
+
+    """
 
     if z is None:
         z = f.properties['z']
 
     if unit is None:
         try:
             unit = f.dm["mass"].units / f.dm["pos"].units ** 3
@@ -310,26 +351,50 @@
 
     return rho_crit.ratio(unit, **f.conversion_context())
 
 
 def rho_M(f, z=None, unit=None):
     """Calculate the matter density of the universe in snapshot f.
 
-    unit and z are used if not None, as by rho_crit. See also the note in
-    rho_crit about confusion over comoving units in this case."""
+    .. warning ::
+        You can get slightly confusing results if your simulation is in comoving units and you specify a different
+        redshift z. Specifically, the physical density for the redshift you specify is calulated, but expressed as
+        a comoving density *at the redshift of the snapshot*. This is intentional, but can be surprising.
+
+    Parameters
+    ----------
+
+    f : SimSnap
+        The snapshot from which to obtain the cosmological parameters.
+
+    z : float, optional
+        The redshift at which to calculate the critical density. If None, the redshift of the snapshot is used.
+
+    unit : str, optional
+        The units in which to return the matter density. If None, the returned density will be in the units of
+        f["mass"].units/f["pos"].units**3. If that unit cannot be calculated, the returned units are Msol kpc^-3
+        comoving.
+
+    Returns
+    -------
+
+    float
+        The matter density of the universe at the specified redshift.
+
+    """
 
     if z is None:
         z = f.properties['z']
 
     return f.properties['omegaM0'] * rho_crit(f, 0, unit) * (1.0 + z) ** 3
 
 
 def H(f):
     """Calculate the Hubble parameter of the universe in snapshot f"""
-    return f.properties['h'] * hzoverh0(f.properties['a'], f.properties['omegaM0']) * units.Unit("100 km s^-1 Mpc^-1")
+    return f.properties['h'] * _hzoverh0(f.properties['a'], f.properties['omegaM0']) * units.Unit("100 km s^-1 Mpc^-1")
 
 
 def add_hubble(f):
     """Add the hubble flow to velocities in snapshot f"""
 
     f['vel'] += f['pos'] * H(f)
```

### Comparing `pynbody-2.0.0b7/pynbody/analysis/decomp.py` & `pynbody-2.0.0b8/pynbody/analysis/decomp.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,222 +1,215 @@
 """
-
-decomp
-======
-
-Tools for bulge/disk/halo decomposition
+Galactic bulge/disk/halo decomposition
 
 """
 
 import logging
 
 import numpy as np
 
-from .. import array, config, filt, util
+from .. import array, config, filt, transformation, util
 from . import angmom, profile
 
 logger = logging.getLogger('pynbody.analysis.decomp')
 
 
 def decomp(h, aligned=False, j_disk_min=0.8, j_disk_max=1.1, E_cut=None, j_circ_from_r=False,
-           cen=None, vcen=None, log_interp=False, angmom_size="3 kpc"):
-    """
-    Creates an array 'decomp' for star particles in the simulation, with an
-    integer specifying a kinematic decomposition. The possible values are:
+           log_interp=False, angmom_size="3 kpc"):
+    """Creates an array 'decomp' for star particles in the simulation, with an integer specifying components.
+
+    The possible values of the components are:
 
     1 -- thin disk
 
     2 -- halo
 
     3 -- bulge
 
     4 -- thick disk
 
     5 -- pseudo bulge
 
     This routine is based on an original IDL procedure by Chris Brook.
 
+    Arguments
+    ---------
 
-    **Parameters:**
-
-    *h* -- the halo to work on
+    h : SimSnap
+        The simulation snapshot to analyze
 
-    *j_disk_min* -- the minimum angular momentum as a proportion of
-                  the circular angular momentum which a particle must
-                  have to be part of the 'disk'
+    aligned : bool
+        If True, the simulation is assumed to be already aligned so that the disk is in the xy plane.
+        Otherwise, the simulation is recentered and aligned into the xy plane.
 
-    *j_disk_max* -- the maximum angular momentum as a proportion of
-                  the circular angular momentum which a particle can
-                  have to be part of the 'disk'
+    j_disk_min : float
+        The minimum angular momentum as a proportion of the circular angular momentum which a particle must have to be
+        part of the 'disk'.
 
-    *E_cut* -- the energy boundary between bulge and spheroid. If
-             None, this is taken to be the median energy of the stars.
+    j_disk_max : float
+        The maximum angular momentum as a proportion of the circular angular momentum which a particle can have to be
+        part of the 'disk'.
 
-    *aligned* -- if False, the simulation is recenterd and aligned so
-               the disk is in the xy plane as required for the rest of
-               the analysis.
+    E_cut : float
+        The energy boundary between bulge and spheroid. If None, this is taken to be the median energy of the stars.
 
-    *cen* -- if not None, specifies the center of the halo. Otherwise
-           it is found.  This has no effect if aligned=True
+    j_circ_from_r : bool
+        If True, the maximum angular momentum is determined as a function of radius, rather than as a function of
+        orbital energy. Default False (determine as function of energy).
 
-    *vcen* -- if not None, specifies the velocity center of the
-            halo. Otherwise it is found.  This has no effect if
-            aligned=True
-
-    *j_circ_from_r* -- if True, the maximum angular momentum is
-    determined as a function of radius, rather than as a function of
-    orbital energy. Default False (determine as function of energy).
-
-    *angmom_size* -- the size of the gas sphere used to determine the
-     plane of the disk
+    angmom_size : str
+        The size of the disk to use for calculating the angular momentum vector. Default is "3 kpc".
 
     """
 
     import scipy.interpolate as interp
     global config
 
     # Center, eliminate proper motion, rotate so that
     # gas disk is in X-Y plane
-    if not aligned:
-        angmom.faceon(h, cen=cen, vcen=vcen, disk_size=angmom_size)
+    if aligned:
+        tx = transformation.NullTransformation(h)
+    else:
+        tx = angmom.faceon(h, disk_size=angmom_size)
 
-    # Find KE, PE and TE
-    ke = h['ke']
-    pe = h['phi']
+    with tx:
 
-    h['phi'].convert_units(ke.units)  # put PE and TE into same unit system
+        # Find KE, PE and TE
+        ke = h['ke']
+        pe = h['phi']
 
-    te = ke + pe
-    h['te'] = te
-    te_star = h.star['te']
+        h['phi'].convert_units(ke.units)  # put PE and TE into same unit system
 
-    te_max = te_star.max()
+        te = ke + pe
+        h['te'] = te
+        te_star = h.star['te']
 
-    # Add an arbitrary offset to the PE to reflect the idea that
-    # the group is 'fully bound'.
-    te -= te_max
-    logger.info("te_max = %.2e" % te_max)
+        te_max = te_star.max()
 
-    h['te'] -= te_max
+        # Add an arbitrary offset to the PE to reflect the idea that
+        # the group is 'fully bound'.
+        te -= te_max
+        logger.info("te_max = %.2e" % te_max)
 
-    logger.info("Making disk rotation curve...")
+        h['te'] -= te_max
 
-    # Now make a rotation curve for the disk. We'll take everything
-    # inside a vertical height of eps*3
+        logger.info("Making disk rotation curve...")
 
-    d = h[filt.Disc('1 Mpc', h['eps'].min() * 3)]
+        # Now make a rotation curve for the disk. We'll take everything
+        # inside a vertical height of eps*3
 
-    try:
+        d = h[filt.Disc('1 Mpc', h['eps'].min() * 3)]
 
-        # attempt to load rotation curve off disk
-        r, v_c = np.loadtxt(h.ancestor.filename + ".rot." +
-                            str(h.properties["halo_number"]), skiprows=1, unpack=True)
+        try:
 
-        pro_d = profile.Profile(d, nbins=100, type='log')
-        r_me = pro_d["rbins"].in_units("kpc")
-        r_x = np.concatenate(([0], r, [r.max() * 2]))
-        v_c = np.concatenate(([v_c[0]], v_c, [v_c[-1]]))
-        v_c = interp.interp1d(r_x, v_c, bounds_error=False)(r_me)
+            # attempt to load rotation curve off disk
+            r, v_c = np.loadtxt(h.ancestor.filename + ".rot." +
+                                str(h.properties["halo_number"]), skiprows=1, unpack=True)
 
-        logger.info(" - found existing rotation curve on disk, using that")
+            pro_d = profile.Profile(d, nbins=100, type='log')
+            r_me = pro_d["rbins"].in_units("kpc")
+            r_x = np.concatenate(([0], r, [r.max() * 2]))
+            v_c = np.concatenate(([v_c[0]], v_c, [v_c[-1]]))
+            v_c = interp.interp1d(r_x, v_c, bounds_error=False)(r_me)
 
-        v_c = v_c.view(array.SimArray)
-        v_c.units = "km s^-1"
-        v_c.sim = d
+            logger.info(" - found existing rotation curve on disk, using that")
 
-        v_c.convert_units(h['vel'].units)
+            v_c = v_c.view(array.SimArray)
+            v_c.units = "km s^-1"
+            v_c.sim = d
 
-        pro_d._profiles['v_circ'] = v_c
-        pro_d.v_circ_loaded = True
+            v_c.convert_units(h['vel'].units)
 
-    except Exception:
-        pro_d = profile.Profile(d, nbins=100, type='log')  # .D()
-        # Nasty hack follows to force the full halo to be used in calculating the
-        # gravity (otherwise get incorrect rotation curves)
-        pro_d._profiles['v_circ'] = profile.v_circ(pro_d, h)
+            pro_d._profiles['v_circ'] = v_c
+            pro_d.v_circ_loaded = True
 
-    pro_phi = pro_d['phi']
-    #import pdb; pdb.set_trace()
-    # offset the potential as for the te array
-    pro_phi -= te_max
+        except Exception:
+            pro_d = profile.Profile(d, nbins=100, type='log')  # .D()
+            # Nasty hack follows to force the full halo to be used in calculating the
+            # gravity (otherwise get incorrect rotation curves)
+            pro_d._profiles['v_circ'] = profile.v_circ(pro_d, h)
 
-    # (will automatically be reflected in E_circ etc)
-    # calculating v_circ for j_circ and E_circ is slow
+        pro_phi = pro_d['phi']
+        #import pdb; pdb.set_trace()
+        # offset the potential as for the te array
+        pro_phi -= te_max
 
-    if j_circ_from_r:
-        pro_d.create_particle_array("j_circ", out_sim=h)
-        pro_d.create_particle_array("E_circ", out_sim=h)
-    else:
+        # (will automatically be reflected in E_circ etc)
+        # calculating v_circ for j_circ and E_circ is slow
 
-        if log_interp:
-            j_from_E = interp.interp1d(
-                np.log10(-pro_d['E_circ'].in_units(ke.units))[::-1], np.log10(pro_d['j_circ'])[::-1], bounds_error=False)
-            h['j_circ'] = 10 ** j_from_E(np.log10(-h['te']))
+        if j_circ_from_r:
+            pro_d.create_particle_array("j_circ", out_sim=h)
+            pro_d.create_particle_array("E_circ", out_sim=h)
         else:
-            #            j_from_E  = interp.interp1d(-pro_d['E_circ'][::-1], (pro_d['j_circ'])[::-1], bounds_error=False)
-            j_from_E = interp.interp1d(
-                pro_d['E_circ'].in_units(ke.units), pro_d['j_circ'], bounds_error=False)
-            h['j_circ'] = j_from_E(h['te'])
-
-        # The next line forces everything close-to-unbound into the
-        # spheroid, as per CB's original script ('get rid of weird
-        # outputs', it says).
-        h['j_circ'][np.where(h['te'] > pro_d['E_circ'].max())] = np.inf
-
-        # There are only a handful of particles falling into the following
-        # category:
-        h['j_circ'][np.where(h['te'] < pro_d['E_circ'].min())] = pro_d[
-            'j_circ'][0]
-
-    h['jz_by_jzcirc'] = h['j'][:, 2] / h['j_circ']
-    h_star = h.star
-
-    if 'decomp' not in h_star:
-        h_star._create_array('decomp', dtype=int)
-    disk = np.where(
-        (h_star['jz_by_jzcirc'] > j_disk_min) * (h_star['jz_by_jzcirc'] < j_disk_max))
-
-    h_star['decomp', disk[0]] = 1
-    # h_star = h_star[np.where(h_star['decomp']!=1)]
-
-    # Find disk/spheroid angular momentum cut-off to make spheroid
-    # rotational velocity exactly zero.
-
-    V = h_star['vcxy']
-    JzJcirc = h_star['jz_by_jzcirc']
-    te = h_star['te']
-
-    logger.info("Finding spheroid/disk angular momentum boundary...")
-
-    j_crit = util.bisect(0., 5.0,
-                         lambda c: np.mean(V[np.where(JzJcirc < c)]))
-
-    logger.info("j_crit = %.2e" % j_crit)
-
-    if j_crit > j_disk_min:
-        logger.warning(
-            "!! j_crit exceeds j_disk_min. This is usually a sign that something is going wrong (train-wreck galaxy?)")
-        logger.warning("!! j_crit will be reset to j_disk_min=%.2e" % j_disk_min)
-        j_crit = j_disk_min
-
-    sphere = np.where(h_star['jz_by_jzcirc'] < j_crit)
-
-    if E_cut is None:
-        E_cut = np.median(h_star['te'])
-
-    logger.info("E_cut = %.2e" % E_cut)
-
-    halo = np.where((te > E_cut) * (JzJcirc < j_crit))
-    bulge = np.where((te <= E_cut) * (JzJcirc < j_crit))
-    pbulge = np.where((te <= E_cut) * (JzJcirc > j_crit)
-                      * ((JzJcirc < j_disk_min) + (JzJcirc > j_disk_max)))
-    thick = np.where((te > E_cut) * (JzJcirc > j_crit)
-                     * ((JzJcirc < j_disk_min) + (JzJcirc > j_disk_max)))
-
-    # h_star['decomp', disk] = 1
-    h_star['decomp', halo] = 2
-    h_star['decomp', bulge] = 3
-    h_star['decomp', thick] = 4
-    h_star['decomp', pbulge] = 5
+
+            if log_interp:
+                j_from_E = interp.interp1d(
+                    np.log10(-pro_d['E_circ'].in_units(ke.units))[::-1], np.log10(pro_d['j_circ'])[::-1], bounds_error=False)
+                h['j_circ'] = 10 ** j_from_E(np.log10(-h['te']))
+            else:
+                #            j_from_E  = interp.interp1d(-pro_d['E_circ'][::-1], (pro_d['j_circ'])[::-1], bounds_error=False)
+                j_from_E = interp.interp1d(
+                    pro_d['E_circ'].in_units(ke.units), pro_d['j_circ'], bounds_error=False)
+                h['j_circ'] = j_from_E(h['te'])
+
+            # The next line forces everything close-to-unbound into the
+            # spheroid, as per CB's original script ('get rid of weird
+            # outputs', it says).
+            h['j_circ'][np.where(h['te'] > pro_d['E_circ'].max())] = np.inf
+
+            # There are only a handful of particles falling into the following
+            # category:
+            h['j_circ'][np.where(h['te'] < pro_d['E_circ'].min())] = pro_d[
+                'j_circ'][0]
+
+        h['jz_by_jzcirc'] = h['j'][:, 2] / h['j_circ']
+        h_star = h.star
+
+        if 'decomp' not in h_star:
+            h_star._create_array('decomp', dtype=int)
+        disk = np.where(
+            (h_star['jz_by_jzcirc'] > j_disk_min) * (h_star['jz_by_jzcirc'] < j_disk_max))
+
+        h_star['decomp', disk[0]] = 1
+        # h_star = h_star[np.where(h_star['decomp']!=1)]
+
+        # Find disk/spheroid angular momentum cut-off to make spheroid
+        # rotational velocity exactly zero.
+
+        V = h_star['vcxy']
+        JzJcirc = h_star['jz_by_jzcirc']
+        te = h_star['te']
+
+        logger.info("Finding spheroid/disk angular momentum boundary...")
+
+        j_crit = util.bisect(0., 5.0,
+                             lambda c: np.mean(V[np.where(JzJcirc < c)]))
+
+        logger.info("j_crit = %.2e" % j_crit)
+
+        if j_crit > j_disk_min:
+            logger.warning(
+                "!! j_crit exceeds j_disk_min. This is usually a sign that something is going wrong (train-wreck galaxy?)")
+            logger.warning("!! j_crit will be reset to j_disk_min=%.2e" % j_disk_min)
+            j_crit = j_disk_min
+
+        sphere = np.where(h_star['jz_by_jzcirc'] < j_crit)
+
+        if E_cut is None:
+            E_cut = np.median(h_star['te'])
+
+        logger.info("E_cut = %.2e" % E_cut)
+
+        halo = np.where((te > E_cut) * (JzJcirc < j_crit))
+        bulge = np.where((te <= E_cut) * (JzJcirc < j_crit))
+        pbulge = np.where((te <= E_cut) * (JzJcirc > j_crit)
+                          * ((JzJcirc < j_disk_min) + (JzJcirc > j_disk_max)))
+        thick = np.where((te > E_cut) * (JzJcirc > j_crit)
+                         * ((JzJcirc < j_disk_min) + (JzJcirc > j_disk_max)))
+
+        h_star['decomp', halo] = 2
+        h_star['decomp', bulge] = 3
+        h_star['decomp', thick] = 4
+        h_star['decomp', pbulge] = 5
 
     # Return profile object for informational purposes
     return pro_d
```

### Comparing `pynbody-2.0.0b7/pynbody/analysis/gravity.py` & `pynbody-2.0.0b8/pynbody/analysis/gravity.py`

 * *Files identical despite different names*

### Comparing `pynbody-2.0.0b7/pynbody/analysis/h1.hdf5` & `pynbody-2.0.0b8/pynbody/analysis/h1.hdf5`

 * *Files identical despite different names*

### Comparing `pynbody-2.0.0b7/pynbody/analysis/halo.py` & `pynbody-2.0.0b8/pynbody/analysis/halo.py`

 * *Files 19% similar despite different names*

```diff
@@ -4,84 +4,73 @@
 ====
 
 Functions for dealing with and manipulating halos in simulations.
 
 
 """
 
+import functools
 import logging
 import math
+import operator
+import warnings
 
 import numpy as np
 
 from .. import array, config, filt, transformation, units, util
 from . import _com, cosmology, profile
 
 logger = logging.getLogger('pynbody.analysis.halo')
 
 
-def center_of_mass(sim):
+def shrink_sphere_center(sim, r=None, shrink_factor=0.7, min_particles=100,
+                         num_threads = None, particles_for_velocity = 0,
+                         families_for_velocity = ['dm', 'star']):
     """
+    Return the center according to the shrinking-sphere method of Power et al (2003)
 
-    Return the centre of mass of the SimSnap
+    Most users will want to use the higher-level :func:`center` function, which actually performs the centering operation.
+    This function is a lower-level interface that calculates the center but does not move the particles.
 
-    """
-    mtot = sim["mass"].sum()
-    p = np.sum(sim["mass"] * sim["pos"].transpose(), axis=1) / mtot
-
-    # otherwise behaviour is numpy version dependent
-    p.units = sim["pos"].units
-
-    # only return position to be consistent with other functions in halo.py
-    return p
-
-
-def center_of_mass_velocity(sim):
-    """
-
-    Return the center of mass velocity of the SimSnap
-
-    """
-    mtot = sim["mass"].sum()
-    v = np.sum(sim["mass"] * sim["vel"].transpose(), axis=1) / mtot
-    # otherwise behaviour is numpy version dependent
-    v.units = sim["vel"].units
+    Parameters
+    ----------
 
-    return v
+    sim : SimSnap
+        The simulation snapshot to center
 
+    r : float | str, optional
+        Initial search radius. If None, a rough estimate is used.
 
-def shrink_sphere_center(sim, r=None, shrink_factor=0.7, min_particles=100, verbose=False, num_threads = None,**kwargs):
-    """
-
-    Return the center according to the shrinking-sphere method of
-    Power et al (2003)
-
+    shrink_factor : float, optional
+        The amount to shrink the search radius by on each iteration
 
-    **Input**:
+    min_particles : int, optional
+        Minimum number of particles within the search radius. When this number is reached, the search is complete.
 
-    *sim* : a simulation snapshot - this can be any subclass of SimSnap
+    num_threads : int, optional
+        Number of threads to use for the calculation. If None, the number of threads is taken from the configuration.
 
-    **Optional Keywords**:
+    particles_for_velocity : int, optional
+        If > min_particles, a velocity centre is calculated when the number of particles falls below this threshold,
+        and returned.
 
-    *r* (default=None): initial search radius. This can be a string
-     indicating the unit, i.e. "200 kpc", or an instance of
-     :func:`~pynbody.units.Unit`.
+    families_for_velocity : list, optional
+        The families to use for the velocity centering. Default is ['dm', 'star'], because gas particles may
+        be involved in violent outflows making them a risky choice for velocity centering.
 
-    *shrink_factor* (default=0.7): the amount to shrink the search
-     radius by on each iteration
+    Returns
+    -------
+    com : SimArray
+        The center of mass of the final sphere
 
-    *min_particles* (default=100): minimum number of particles within
-     the search radius. When this number is reached, the search is
-     complete.
-
-    *verbose* (default=False): if True, prints out the diagnostics at
-     each iteration. Useful to determine whether the centering is
-     zeroing in on the wrong part of the simulation.
+    vel : SimArray
+        The center of mass velocity of the final sphere. Only returned if particles_for_velocity > min_particles.
 
     """
+
     if num_threads is None:
         num_threads = config['number_of_threads']
 
     if r is None:
 
         # use rough estimate for a maximum radius
         # results will be insensitive to the exact value chosen
@@ -91,152 +80,191 @@
         if isinstance(r, str):
             r = units.Unit(r)
         r = r.in_units(sim['pos'].units, **sim.conversion_context())
 
     mass = np.asarray(sim['mass'], dtype='double')
     pos = np.asarray(sim['pos'], dtype='double')
 
-    if shrink_factor == 1.0:
-        tol = sim['eps'].in_units(sim['pos'].units, **sim.conversion_context()).min()*0.1
-        com = _com.shrink_sphere_center(pos, mass, min_particles, shrink_factor, r, num_threads)
-        com = _com.move_sphere_center(pos, mass, min_particles, shrink_factor, r, tol)
-    else:
-        com = _com.shrink_sphere_center(pos, mass, min_particles, shrink_factor, r, num_threads)
+    R = _com.shrink_sphere_center(pos, mass, min_particles, particles_for_velocity,
+                                  shrink_factor, r, num_threads)
+
+    com, final_radius, velocity_radius = R
 
+    logger.info("Radius for velocity measurement = %s", velocity_radius)
     logger.info("Final SSC=%s", com)
 
-    return array.SimArray(com, sim['pos'].units)
+    com_to_return = array.SimArray(com, sim['pos'].units)
+
+    if particles_for_velocity > min_particles:
+        fam_filter = functools.reduce(operator.or_, (filt.FamilyFilter(f) for f in families_for_velocity))
+        final_sphere = sim[filt.Sphere(velocity_radius, com) & fam_filter]
+        logger.info("Particles in sphere = %d", len(final_sphere))
+        if len(final_sphere) == 0:
+            warnings.warn("Final sphere is empty; cannot return a velocity. This probably implies something is "
+                          "wrong with the position centre too.", RuntimeWarning)
+            return com_to_return, np.array([0., 0., 0.])
+        else:
+            vel = final_sphere.mean_by_mass('vel')
+            logger.info("Final velocity=%s", vel)
+            return com_to_return, vel
+    else:
+        return com_to_return
+
 
 
 def virial_radius(sim, cen=None, overden=178, r_max=None, rho_def='matter'):
-    """Calculate the virial radius of the halo centered on the given
-    coordinates.
+    """Calculate the virial radius of the halo centered on the given coordinates.
 
     The default is here defined by the sphere centered on cen which contains a
     mean density of overden * rho_M_0 * (1+z)^3.
 
-    **Input**:
+    Parameters
+    ----------
+
+    sim : SimSnap
+        The simulation snapshot for which to calculate the virial radius.
 
-    *sim* : a simulation snapshot - this can be any subclass of SimSnap, especially a halo.
+    cen : array_like, optional
+        The center of the halo. If None, the halo is assumed to be already centered.
 
-    **Optional Keywords**:
+    overden : float, optional
+        The overdensity of the halo. Default is 178.
 
-    *cen* (default=None): Provides the halo center. If None, assumes that the snapshot is already centered.
+    r_max : float, optional
+        The maximum radius to search for the virial radius. If None, the maximum radius of any
+        particle in *sim* is used
 
-    *rmax (default=None): Maximum radius to start the search. If None, inferred from the halo particle positions.
+    rho_def : str, optional
+        The density definition to use.
+        Default is 'matter', which uses the matter density at the redshift of the simulation. Alternatively,
+        'critical' can be used for the critical density at this redshift.
 
-    *overden (default=178): Overdensity corresponding to the required halo boundary definition.
-    178 is the virial criterion for spherical collapse in an EdS Universe. Common possible values are 200, 500 etc
+    Returns
+    -------
 
-    *rho_def (default='matter'): Physical density used to define the overdensity. Default is the matter density at
-    the redshift of the simulation. An other choice is "critical" for the critical density at this redshift.
+    float
+        The virial radius of the halo in the position units of *sim*.
 
     """
 
     if r_max is None:
         r_max = (sim["x"].max() - sim["x"].min())
     else:
         if cen is not None:
             sim = sim[filt.Sphere(r_max, cen)]
         else:
             sim = sim[filt.Sphere(r_max)]
 
     r_min = 0.0
 
-    if cen is not None:
-        tx = transformation.inverse_translate(sim, cen)
-    else:
-        tx = transformation.null(sim)
-
     if rho_def == 'matter':
        ref_density = sim.properties["omegaM0"] * cosmology.rho_crit(sim, z=0) * (1.0 + sim.properties["z"]) ** 3
     elif rho_def == 'critical':
         ref_density = cosmology.rho_crit(sim, z=sim.properties["z"])
     else:
         raise ValueError(rho_def + "is not a valid definition for the reference density")
 
     target_rho = overden * ref_density
     logger.info("target_rho=%s", target_rho)
 
-    with tx:
+    if cen is not None:
+        transform = sim.translate(-np.asanyarray(cen))
+    else:
+        transform = transformation.NullTransformation(sim)
+
+    with transform:
         sim = sim[filt.Sphere(r_max)]
         with sim.immediate_mode:
             mass_ar = np.asarray(sim['mass'])
             r_ar = np.asarray(sim['r'])
 
-        """
-        #pure numpy implementation
-        rho = lambda r: np.dot(
-            mass_ar, r_ar < r) / (4. * math.pi * (r ** 3) / 3)
-
-        #numexpr alternative - not much faster because sum is not threaded
-        def rho(r) :
-            r_ar; mass_ar; # just to get these into the local namespace
-            return ne.evaluate("sum((r_ar<r)*mass_ar)")/(4.*math.pi*(r**3)/3)
-        """
         rho = lambda r: util.sum_if_lt(mass_ar,r_ar,r)/(4. * math.pi * (r ** 3) / 3)
         result = util.bisect(r_min, r_max, lambda r: target_rho -
                              rho(r), epsilon=0, eta=1.e-3 * target_rho, verbose=False)
 
     return result
 
 
-def potential_minimum(sim):
+def _potential_minimum(sim):
     i = sim["phi"].argmin()
     return sim["pos"][i].copy()
 
 
 def hybrid_center(sim, r='3 kpc', **kwargs):
-    """
+    """Determine the center of the halo by finding the shrink-sphere-center near the potential minimum
+
+    Most users will want to use the general :func:`center` function, which actually performs the centering operation.
+    This function is a lower-level interface that calculates the center but does not move the particles.
+
+    Parameters
+    ----------
+
+    sim : SimSnap
+        The simulation snapshot of which to find the center
+    r : float | str, optional
+        Radius from the potential minimum to search for the center. Default is 3 kpc.
+
+    Remaining parameters are passed onto :func:`shrink_sphere_center`.
+
+    Returns
+    -------
+
+    com : SimArray
+        The center of mass of the final sphere
+    vel : SimArray
+        The center of mass velocity of the final sphere. Only returned if particles_for_velocity > min_particles.
 
-    Determine the center of the halo by finding the shrink-sphere
-    -center inside the specified distance of the potential minimum
 
     """
 
     try:
-        cen_a = potential_minimum(sim)
+        cen_a = _potential_minimum(sim)
     except KeyError:
         cen_a = center_of_mass(sim)
     return shrink_sphere_center(sim[filt.Sphere(r, cen_a)], **kwargs)
 
 
-def index_center(sim, **kwargs):
-    """
 
-    Determine the center of mass based on specific particles.
+def vel_center(sim, cen_size="1 kpc", return_cen=False, move_all=True, **kwargs):
+    """Recenter the snapshot on the center of mass velocity inside a sphere of specified radius
 
-    Supply a list of indices using the ``ind`` keyword.
+    Attempts to use the star particles, falling back to gas or dark matter if necessary.
 
-    """
+    Parameters
+    ----------
 
-    try:
-        ind = kwargs['ind']
-        return center_of_mass(sim[ind])
-    except KeyError:
-        raise RuntimeError("Need to supply indices for centering")
+    sim : SimSnap
+        The simulation snapshot to center
 
+    cen_size : str or float, optional
+        The size of the sphere to use for the velocity centering. Default is 1 kpc.
 
-def vel_center(sim, mode=None, cen_size="1 kpc", retcen=False, move_all=True, **kwargs):
-    """Use stars from a sphere to calculate center of velocity. The size
-    of the sphere is given by the ``cen_size`` keyword and defaults to
-    1 kpc.
+    return_cen : bool, optional
+        If True, only return the velocity center without actually moving the snapshot. Default is False.
 
-    **Keyword arguments:**
+    move_all : bool, optional
+        If True (default), move the entire snapshot. Otherwise only move the particles in the halo passed in.
 
-    *mode*: reserved for future use; currently ignored
+    retcen : bool, optional
+        Deprecated alias for return_cen
 
-    *move_all*: if True (default), move the entire snapshot. Otherwise only move
-    the particles in the halo passed in.
+    Returns
+    -------
 
-    *retcen*: if True only return the velocity center without moving the
-     snapshot (default = False)
+    Transformation | SimArray
+        Normally, a transformation object that can be used to revert the transformation.
+        However, if return_cen is True, a SimArray containing the velocity center
+        coordinates is returned instead, and the snapshot is not transformed.
 
     """
 
+    if "retcen" in kwargs:
+        return_cen = kwargs.pop("retcen")
+        warnings.warn("The 'retcen' keyword is deprecated. Use 'return_cen' instead.", DeprecationWarning)
+
     logger.info("Finding halo velocity center...")
 
     if move_all:
         target = sim.ancestor
     else:
         target = sim
 
@@ -250,128 +278,205 @@
     if len(cen) < 5:
         # very weird snapshot, or mis-centering!
         raise ValueError("Insufficient particles around center to get velocity")
 
     vcen = (cen['vel'].transpose() * cen['mass']).sum(axis=1) / \
         cen['mass'].sum()
     vcen.units = cen['vel'].units
-    if config['verbose']:
-        logger.info("vcen=%s", vcen)
 
-    if retcen:
+    logger.info("vcen=%s", vcen)
+
+    if return_cen:
         return vcen
     else:
-        return transformation.v_translate(target, -vcen)
+        return target.offset_velocity(-vcen)
 
 
-def center(sim, mode=None, retcen=False, vel=True, cen_size="1 kpc", move_all=True, wrap=False, **kwargs):
-    """
+def center(sim, mode=None, return_cen=False, with_velocity=True, cen_size="1 kpc",
+           cen_num_particles=10000, move_all=True, wrap=False, **kwargs):
+    """Transform the ancestor snapshot so that the provided snapshot is centred
+
+    The centering scheme is determined by the ``mode`` keyword. As well as the
+    position, the velocity can also be centred.
+
+    The following centring modes are available:
+
+    *  *pot*: potential minimum
+
+    *  *com*: center of mass
 
-    Determine the center of mass of the given particles using the
-    specified mode, then recenter the particles (of the entire
-    ancestor snapshot) accordingly
+    *  *ssc*: shrink sphere center
 
-    Accepted values for *mode* are
+    *  *hyb*: for most halos, returns the same as ssc, but works faster by starting iteration near potential minimum
 
-      *pot*: potential minimum
+    Before the main centring routine is called, the snapshot is translated so that the
+    halo is already near the origin. The box is then wrapped so that halos on the edge
+    of the box are handled correctly.
 
-      *com*: center of mass
 
-      *ssc*: shrink sphere center
+    Parameters
+    ----------
 
-      *ind*: center on specific particles; supply the list of particles using the ``ind`` keyword.
+    sim : SimSnap
+        The simulation snapshot from which to derive a centre. The ancestor snapshot is
+        then transformed.
 
-      *hyb*: for sane halos, returns the same as ssc, but works faster by
-             starting iteration near potential minimum
+    mode : str or function, optional
+        The method to use to determine the centre. If None, the default is taken from the configuration.
+        Accepted values are discussed above. A function returning the centre, or a pair of
+        centres (position and velocity) can also be passed.
 
-    or a function returning the COM.
+    cen_size : str or float, optional
+        The size of the sphere to use for the velocity centering. Default is 1 kpc.
+        Note that this is only used if velocity centring is requested but the underlying
+        method does not return a velocity centre. For example, if using the 'ssc' method,
+        the cen_num_particles keyword should be used instead.
 
-    **Other keywords:**
+    cen_num_particles : int, optional
+        The number of particles to use for the velocity centering. Default is 5000.
+        This is passed to the 'ssc' method, which then finds the sphere with approximately
+        this number of particles in it for the velocity centering.
 
-    *retcen*: if True only return the center without centering the
-     snapshot (default = False)
+    with_velocity: bool, optional
+        If True, also center the velocity. Default is True.
 
-    *ind*: only used when *mode=ind* -- specifies the indices of
-     particles to be used for centering
+    return_cen: bool, optional
+        If True, only return the center without actually centering the snapshot.
+        Default is False.
+
+    move_all: bool, optional
+        If True (default), move the entire snapshot. Otherwise only move the particles
+        in the halo/subsnap passed into this function.
+
+    vel: bool, optional
+        Deprecated alias for with_velocity. Default is True.
+
+    retcen: bool, optional
+        If True, only return the center without centering the snapshot. Default is False.
+
+    Returns
+    -------
+    Transformation | SimArray
+        Normally, a transformation object that can be used to revert the transformation.
+        However, if return_cen is True, a SimArray containing the center
+        coordinates is returned instead, and the snapshot is not transformed.
 
-    *vel*: if True, translate velocities so that the velocity of the
-    central 1kpc (default) is zeroed. Other values can be passed with cen_size.
 
-    *move_all*: if True (default), move the entire snapshot. Otherwise only move
-    the particles in the halo passed in.
 
-    *wrap*: if True, pre-centre and wrap the simulation so that halos on the edge
-    of the box are handled correctly. Default False.
     """
 
+    if 'vel' in kwargs:
+        warnings.warn("The 'vel' keyword is deprecated. Use 'with_velocity' instead.", DeprecationWarning)
+        with_velocity = kwargs.pop('vel')
+
+    if 'retcen' in kwargs:
+        warnings.warn("The 'retcen' keyword is deprecated. Use 'return_cen' instead.", DeprecationWarning)
+        return_cen = kwargs.pop('retcen')
+
+
     global config
     if mode is None:
         mode = config['centering-scheme']
 
     try:
-        fn = {'pot': potential_minimum,
-              'com': center_of_mass,
-              'ssc': shrink_sphere_center,
-              'hyb': hybrid_center,
-              'ind': index_center}[mode]
+        fn = {'pot': _potential_minimum,
+              'com': lambda s : s.mean_by_mass('pos'),
+              'ssc': functools.partial(shrink_sphere_center, particles_for_velocity=cen_num_particles),
+              'hyb': hybrid_center}[mode]
     except KeyError:
         fn = mode
 
     if move_all:
         target = sim.ancestor
     else:
         target = sim
 
     if wrap:
         # centre on something within the halo and wrap
-        target = transformation.inverse_translate(target, sim['pos'][0])
-        target.sim.wrap()
-
-    if retcen:
-        return fn(sim, **kwargs)
+        initial_offset = -sim['pos'][0]
+        transform = target.translate(initial_offset)
+        target.wrap()
     else:
-        cen = fn(sim, **kwargs)
-        tx = transformation.inverse_translate(target, cen)
+        transform = transformation.NullTransformation(target)
+        initial_offset = np.array([0., 0., 0.])
+
+    try:
+        centre = fn(sim, **kwargs)
+        if len(centre) == 2:
+            # implies we have a velocity centre as well
+            centre, vel_centre = centre
+        else:
+            vel_centre = None
+
+        if return_cen:
+            transform.revert()
+            return centre - initial_offset
+
+        transform = transform.translate(-centre)
+
+        if with_velocity:
+            if vel_centre is None :
+                vel_centre = vel_center(sim, cen_size=cen_size, retcen=True)
+            logger.info("vel_centre=%s", vel_centre)
+            transform = transform.offset_velocity(-vel_centre)
 
-    if vel:
-        velc = vel_center(sim, cen_size=cen_size, retcen=True)
-        tx = transformation.inverse_v_translate(tx, velc)
+    except:
+        transform.revert()
+        raise
 
-    return tx
+    return transform
 
 def halo_shape(sim, N=100, rin=None, rout=None, bins='equal'):
     """
-    Returns radii in units of ``sim['pos']``, axis ratios b/a and c/a,
-    the alignment angle of axis a in radians, and the rotation matrix
-    for homeoidal shells over a range of N halo radii.
-
-    **Keyword arguments:**
-
-    *N* (100): The number of homeoidal shells to consider. Shells with
-    few particles will take longer to fit.
-
-    *rin* (None): The minimum radial bin in units of ``sim['pos']``.
-    Note that this applies to axis a, so particles within this radius
-    may still be included within homeoidal shells. By default this is
-    taken as rout/1000.
-
-    *rout* (None): The maximum radial bin in units of ``sim['pos']``.
-    By default this is taken as the largest radial value in the halo
-    particle distribution.
-
-    *bins* (equal): The spacing scheme for the homeoidal shell bins.
-    ``equal`` initialises radial bins with equal numbers of particles,
-    with the exception of the final bin which will accomodate remainders.
-    This number is not necessarily maintained during fitting.
-    ``log`` and ``lin`` initialise bins with logarithmic and linear
-    radial spacing.
+    Computes the shape of a halo as a function of radius by fitting homeoidal shells.
+
+    The halo must be pre-centred, e.g. using :func:`center`.
 
-    Halo must be in a centered frame.
     Caution is advised when assigning large number of bins and radial
     ranges with many particles, as the algorithm becomes very slow.
+
+    Parameters
+    ----------
+
+    N : int
+        The number of homeoidal shells to consider. Shells with few particles will take longer to fit.
+
+    rin : float
+        The minimum radial bin in units of sim['pos']. By default this is taken as rout/1000.
+        Note that this applies to axis a, so particles within this radius may still be included within
+        homeoidal shells.
+
+    rout : float
+        The maximum radial bin in units of sim['pos']. By default this is taken as the largest radial value
+        in the halo particle distribution.
+
+    bins : str
+        The spacing scheme for the homeoidal shell bins. 'equal' initialises radial bins with equal numbers
+        of particles, with the exception of the final bin which will accomodate remainders. This
+        number is not necessarily maintained during fitting. 'log' and 'lin' initialise bins
+        with logarithmic and linear radial spacing.
+
+    Returns
+    -------
+
+    rbin : SimArray
+        The radial bins used for the fitting.
+
+    ba : array
+        The axial ratio b/a as a function of radius.
+
+    ca : array
+        The axial ratio c/a as a function of radius.
+
+    angle : array
+        The angle of the a-direction with respect to the x-axis as a function of radius.
+
+    Es : array
+        The rotation matrices for each shell.
+
     """
 
     #-----------------------------FUNCTIONS-----------------------------
     # Define an ellipsoid shell with lengths a,b,c and orientation E:
     def Ellipsoid(r, a,b,c, E):
         x,y,z = np.dot(np.transpose(E),[r[:,0],r[:,1],r[:,2]])
         return (x/a)**2 + (y/b)**2 + (z/c)**2
```

### Comparing `pynbody-2.0.0b7/pynbody/analysis/hifrac.py` & `pynbody-2.0.0b8/pynbody/analysis/hifrac.py`

 * *Files identical despite different names*

### Comparing `pynbody-2.0.0b7/pynbody/analysis/hmf.py` & `pynbody-2.0.0b8/pynbody/analysis/hmf.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,318 +1,391 @@
 """
+Routines related to halo mass function and other cosmological calculations.
 
-halo mass function (hmf)
-========================
-
-Various halo mass function routines.
+.. warning ::
+    These routines were implemented in 2012 when there were no other python libraries that could do this.
+    Since then, cosmology-focussed libraries such as `hmf <https://hmf.readthedocs.io/en/latest/index.html>`_,
+    `Colossus <https://bdiemer.bitbucket.io/colossus/index.html>`_ and
+    `CCL <https://ccl.readthedocs.io/en/latest/>`_ have been developed.
+    For precision cosmology applications, we recommend using these libraries, since the routines here
+    have not been tested for precision applications (and are known to use approximations).
 
 """
 
+import copy
+import logging
+import math
 import os
+import warnings
 
 import numpy as np
+import scipy
+import scipy.interpolate
 
 import pynbody
 
-from .. import units, util
+from .. import configuration, units, util
 from . import cosmology
 
-try:
-    import scipy
-    import scipy.interpolate
-except ImportError:
-    pass
-
-import logging
-import math
-import subprocess
-import tempfile
-import warnings
-
 logger = logging.getLogger('pynbody.analysis.hmf')
 
 
 #######################################################################
 # Filters
 #######################################################################
 
 class FieldFilter:
-
-    def __init__(self):
-        raise RuntimeError("Cannot instantiate directly, use a subclass instead")
+    """Represents a filter acting on a field"""
 
     def M_to_R(self, M):
         """Return the mass scale (Msol h^-1) for a given length (Mpc h^-1 comoving)"""
         return (M / (self.gammaF * self.rho_bar)) ** 0.3333
 
     def R_to_M(self, R):
         """Return the length scale (Mpc h^-1 comoving) for a given spherical mass (Msol h^-1)"""
         return self.gammaF * self.rho_bar * R ** 3
 
     @staticmethod
     def Wk(kR):
-        raise RuntimeError("Not implemented")
+        """Return the Fourier-space filter function, as a function of kR where R is the scale of the filter"""
+        raise NotImplementedError("Not implemented")
 
 
 class TophatFilter(FieldFilter):
-
+    """A top-hat filter in real space"""
     def __init__(self, context):
         self.gammaF = 4 * math.pi / 3
         self.rho_bar = cosmology.rho_M(context, unit="Msol Mpc^-3 h^2 a^-3")
 
     @staticmethod
     def Wk(kR):
         return 3 * (np.sin(kR) - kR * np.cos(kR)) / (kR) ** 3
 
 
 class GaussianFilter(FieldFilter):
+    """A Gaussian filter"""
 
     def __init__(self, context):
         self.gammaF = (2 * math.pi) ** 1.5
         self.rho_bar = cosmology.rho_M(context, unit="Msol Mpc^-3 h^2 a^-3")
 
     @staticmethod
     def Wk(kR):
         return np.exp(-(kR) ** 2 / 2)
 
 
 class HarmonicStepFilter(FieldFilter):
+    """A step filter in harmonic space"""
 
     def __init__(self, context):
         self.gammaF = 6 * math.pi ** 2
         self.rho_bar = cosmology.rho_M(context, unit="Msol Mpc^-3 h^2 a^-3")
 
     @staticmethod
     def Wk(kR):
         return (kR < 1)
 
 #######################################################################
 # Power spectrum management / normalization
 #######################################################################
 
 
-class PowerSpectrumCAMB:
+class PowerSpectrum:
+    """A power spectrum object, which can be called to return the power spectrum at a given wavenumber."""
+
+    def __init__(self, context, filename=None, k=None, Pk=None, log_interpolation=True):
+        """Set up a power spectrum object.
+
+        Either a tabulated power spectrum or the filename of a tabulated power spectrum can be passed.
+        If neither is provided, a default power spectrum is used which assumes Planck 2018 values.
+
+        Parameters
+        ----------
+
+        context : SimSnap
+            The simulation snapshot from which to pull the cosmological context. This is used for
+            the linear growth factor and sigma8 normalization.
+
+        filename : str, optional
+            The name of a file containing the power spectrum.
+
+        k : array, optional
+            The wavenumbers of the power spectrum in comoving h/Mpc
 
-    def __init__(self, context, filename=None, log_interpolation=True):
-        if filename is None:
-            warnings.warn(
-                "Using the default power-spectrum spectrum which assumes ns=0.96 and WMAP7+H0+BAO transfer function.", RuntimeWarning)
-            filename = os.path.join(os.path.dirname(__file__), "CAMB_WMAP7")
+        Pk : array, optional
+            The power spectrum in Mpc^3 h^-3
 
-        k, Pk = np.loadtxt(filename, unpack=True)
+        log_interpolation : bool, optional
+            If True, interpolate in log space. This is generally more accurate for power spectra.
+
+        """
+
+        if k is None or Pk is None:
+            if filename is None:
+                warnings.warn(
+                    "Using the default power-spectrum spectrum which assumes Planck 2018 values: "
+                    "Omega_c h^2 = 0.120; Omega_b h^2 = 0.0224; h = 0.676; n_s = 0.9667. Sigma8 will be correctly scaled to the simulation value. ",
+                    RuntimeWarning)
+                filename = os.path.join(os.path.dirname(__file__), "CAMB_Planck18")
+            k, Pk = np.loadtxt(filename, unpack=True)
 
         self._orig_k_min = k.min()
         self._orig_k_max = k.max()
 
-        bot_k = 1.e-5
+        bot_k = 1.e-4
 
         if k[0] > bot_k:
             # extrapolate out
             n = math.log10(Pk[1] / Pk[0]) / math.log10(k[1] / k[0])
 
             Pkinterp = 10 ** (math.log10(Pk[0]) - math.log10(k[0] / bot_k) * n)
             k = np.hstack((bot_k, k))
             Pk = np.hstack((Pkinterp, Pk))
 
-        top_k = 1.e7
+        top_k = 1.e4
 
         if k[-1] < top_k:
             # extrapolate out
             n = math.log10(Pk[-1] / Pk[-2]) / math.log10(k[-1] / k[-2])
 
             Pkinterp = 10 ** (math.log10(Pk[-1]
                                          ) - math.log10(k[-1] / top_k) * n)
             k = np.hstack((k, top_k))
             Pk = np.hstack((Pk, Pkinterp))
 
         self.k = k.view(pynbody.array.SimArray)
         self.k.units = "Mpc^-1 h a^-1"
 
-        self.Pk = Pk.view(pynbody.array.SimArray)
-        self.Pk.units = "Mpc^3 h^-3"
+        self.Pk_z0_unnormalised = Pk.view(pynbody.array.SimArray)
+        self.Pk_z0_unnormalised.units = "Mpc^3 h^-3"
 
         self.k.sim = context
-        self.Pk.sim = context
+        self.Pk_z0_unnormalised.sim = context
 
         self._lingrowth = 1
 
         if context.properties['z'] != 0:
             self._lingrowth = cosmology.linear_growth_factor(context) ** 2
 
         self._default_filter = TophatFilter(context)
-        self.min_k = self.k.min()
-        self.max_k = self.k.max()
+        self.min_k = self.k.min()*1.000001
+        self.max_k = self.k.max()*0.999999
         self._norm = 1
 
         self._log_interp = log_interpolation
 
         self._init_interpolation()
 
         self.set_sigma8(context.properties['sigma8'])
 
     def _init_interpolation(self):
         if self._log_interp:
             self._interp = scipy.interpolate.interp1d(
-                np.log(self.k), np.log(self.Pk))
+                np.log(self.k), np.log(self.Pk_z0_unnormalised))
         else:
-            self._interp = scipy.interpolate.interp1d(np.log(self.k), self.Pk)
+            self._interp = scipy.interpolate.interp1d(np.log(self.k), self.Pk_z0_unnormalised)
 
     def set_sigma8(self, sigma8):
+        """Update the normalisation for a given sigma8 value at z=0"""
         current_sigma8_2 = self.get_sigma8() ** 2
         self._norm *= sigma8 ** 2 / current_sigma8_2
 
     def get_sigma8(self):
+        """Calculate the current sigma8 value at z=0"""
         current_sigma8 = math.sqrt(
             variance(8.0, self._default_filter, self, True) / self._lingrowth)
         return current_sigma8
 
     def __call__(self, k):
-        if np.any(k < self._orig_k_min):
-            warnings.warn(
-                "Power spectrum does not extend to low enough k; using power-law extrapolation (this is likely to be fine)", RuntimeWarning)
-        if np.any(k > self._orig_k_max):
-            warnings.warn(
-                "Power spectrum does not extend to high enough k; using power-law extrapolation. This is bad but your results are unlikely to be sensitive to it unless they relate directly to very small scales or you have run CAMB with inappropriate settings.", RuntimeWarning)
+        """Evaluate the power spectrum at the snapshot redshift"""
         if self._log_interp:
             return self._norm * self._lingrowth * np.exp(self._interp(np.log(k)))
         else:
             return self._norm * self._lingrowth * self._interp(np.log(k))
 
 
-class PowerSpectrumCAMBLive(PowerSpectrumCAMB):
+class PowerSpectrumCAMB(PowerSpectrum):
+    """A power spectrum object that calculates the power spectrum on the fly using CAMB.
+
+    This is slower than using a precomputed power spectrum, but is more flexible."""
 
     def __init__(self, context, use_context=True, camb_params={}, log_interpolation=True):
-        """Run CAMB to get out a power spectrum. The default parameters are in cambtemplate.ini.
-        Any of these can be modified by passing the appropriate kwarg."""
+        """Runs CAMB to calculate a power spectrum for the provided context.
+
+        Parameters
+        ----------
+        context : SimSnap
+            The simulation snapshot from which to pull the cosmological context.
+
+        use_context : bool, optional
+            If True, use the context to set the cosmological parameters in CAMB.
+            If False, use only the parameters in ``camb_params``.
+
+        camb_params : dict, optional
+            A dictionary of parameters to pass to CAMB's ``set_cosmology`` method. Note that the
+            scalar spectral index ``ns`` is not included in ``set_cosmology``; if provided here, it is
+            extracted and passed to ``InitPower.set_params``.
+
+        log_interpolation : bool, optional
+            If True, interpolate in log space. This is generally more accurate for power spectra.
+
+        """
 
-        from .. import config_parser
-        path_to_camb = config_parser.get('camb', 'path')
-        if path_to_camb == '/path/to/camb':
-            raise RuntimeError("You need to compile CAMB and set up the executable path in your pynbody configuration file.")
-
-        file_in = open(
-            os.path.join(os.path.dirname(__file__), "cambtemplate.ini"))
-        folder_out = tempfile.mkdtemp()
-        file_out = open(os.path.join(folder_out, "camb.ini"), "w")
+        try:
+            import camb
+        except ImportError:
+            warnings.warn("The camb module is not installed. Falling back to using a pre-computed power spectrum"
+                          "which may not be appropriate for your cosmology.")
+            super().__init__(context)
+            return
+
+        camb_params_obj = camb.CAMBparams()
+        camb_params = copy.copy(camb_params)
+
+        # default value for ns, in case use_context is false:
+        ns = configuration.config_parser.get('default-cosmology', 'ns')
 
         if use_context:
             h0 = context.properties['h']
-            omB0 = context.properties['omegaB0'] * h0 ** 2
-            omM0 = context.properties['omegaM0'] * h0 ** 2
-            omC0 = omM0 - omB0
+            omBh2 = context.properties['omegaB0'] * h0 ** 2
+            omMh2 = context.properties['omegaM0'] * h0 ** 2
+            if omBh2 == 0.0 and 'ombh2' not in camb_params_obj:
+                warnings.warn("OmegaB0 is zero, presumably because this is a DMO run. For the power spectrum, setting ombh2 to 0.0224 (Planck 2018)."
+                              "To override, set 'omegaB0' in the simulation parameters, or 'ombh2' in the camb_params argument.")
+                omBh2 = 0.0224
+            OmCh2 = omMh2 - omBh2
+
+            if 'H0' not in camb_params:
+                camb_params['H0'] = h0 * 100
+            if 'ombh2' not in camb_params:
+                camb_params['ombh2'] = omBh2
+            if 'omch2' not in camb_params:
+                camb_params['omch2'] = OmCh2
+
             ns = context.properties['ns']
-            running = context.properties['running']
-            camb_params.update({'ombh2': omB0, 'omch2': omC0, 'hubble': h0 *
-                                100, 'scalar_nrun(1)': running, 'scalar_spectral_index(1)': ns})
-
-        for line in file_in:
-            if "=" in line and "#" not in line:
-                name, val = line.split("=")
-                name = name.strip()
-                if name in camb_params:
-                    val = camb_params[name]
-                print(name, "=", val, file=file_out)
-            else:
-                print(line.strip(), file=file_out)
-
-        file_out.close()
-
-        logger.info("Running %s on %s" %
-                    (path_to_camb, os.path.join(folder_out, "camb.ini")))
-        subprocess.check_output("cd %s; %s camb.ini" %
-                                (folder_out, path_to_camb), shell=True)
 
-        PowerSpectrumCAMB.__init__(self, context, os.path.join(
-            folder_out, "test_matterpower.dat"), log_interpolation=log_interpolation)
+        if 'ns' in camb_params:
+            ns = camb_params.pop('ns')
+
+        camb_params_obj.set_cosmology(**camb_params)
+
+        camb_params_obj.InitPower.set_params(ns=ns)
+
+        camb_params_obj.WantTransfer = True
+
+        # always get the matter power spectrum at z=0; growth factor will be scaled later if needed
+        camb_params_obj.set_matter_power(redshifts=[0.0], kmax=1e2, k_per_logint=0,
+                                     silent=True, nonlinear=False)
+        results = camb.get_results(camb_params_obj)
+
+        k, z, Pk = results.get_matter_power_spectrum(minkh=1.e-4, maxkh=1e2, npoints=1000)
 
+        # filename = os.path.join(os.path.dirname(__file__), "CAMB_Planck18")
+        # np.savetxt(filename, np.array([k, Pk[0]]).T)
 
-class BiasedPowerSpectrum(PowerSpectrumCAMB):
+        assert len(z)==1
+        assert z[0] == 0.0
+
+        super().__init__(context, k=k, Pk=Pk[0], log_interpolation=log_interpolation)
+
+
+
+class BiasedPowerSpectrum(PowerSpectrum):
+    """A power spectrum object with linear bias"""
 
     def __init__(self, bias, pspec):
         """Set up a biased power spectrum.
 
-        **args**
-          bias: either a number for a fixed bias, or a function taking
-                the wavenumber k in Mpc/h and returning the bias
+        Parameters
+        ----------
+        bias : float  or function
+            Either a constant linear bias factor, or a function of wavenumber that returns the bias at that wavenumber.
 
-          pspec: the underlying power spectrum
+        pspec : PowerSpectrum
+            The power spectrum object to wrap with a bias
         """
 
         if not hasattr(bias, '__call__'):
             bias = lambda x: bias
 
         self._bias = bias
         self._pspec = pspec
         self._norm = 1.0
         self.min_k = pspec.min_k
         self.max_k = pspec.max_k
         self.k = pspec.k
-        self.Pk = pspec.Pk * self._bias(self.k) ** 2
+        self.Pk_z0_unnormalised = pspec.Pk_z0_unnormalised * self._bias(self.k) ** 2
 
     def __call__(self, k):
         return self._norm * self._pspec(k) * self._bias(k) ** 2
 
 
 #######################################################################
 # Variance calculation
 #######################################################################
 
-def variance(M, f_filter=TophatFilter, powspec=PowerSpectrumCAMB, arg_is_R=False):
-    if hasattr(M, '__len__'):
+def variance(M_or_R, f_filter=TophatFilter, powspec=PowerSpectrum, arg_is_R=False):
+    """Calculate the variance of the density field smoothed on a mass scale M, or optionally a length scale R.
+
+    Parameters
+    ----------
+    M_or_R : float or array
+        The mass scale in Msol/h or the radius of the filter in Mpc/h comoving. If an array, the
+        variance is calculated for each element of the array.
+
+    f_filter : FieldFilter, optional
+        The filter to use. Default is a top-hat filter.
+
+    powspec : PowerSpectrum, optional
+        The power spectrum object to use. Default is a Planck 2018 power spectrum at z=0.
+
+    arg_is_R : bool, optional
+        If True, interpret the input as a length scale R rather than a mass scale M.
+
+    Returns
+    -------
+    float or array
+        The variance of the density field smoothed on the given scale(s).
+
+    """
+    if hasattr(M_or_R, '__len__'):
         ax = pynbody.array.SimArray(
-            [variance(Mi, f_filter, powspec, arg_is_R) for Mi in M])
+            [variance(Mi, f_filter, powspec, arg_is_R) for Mi in M_or_R])
         # hopefully dimensionless
-        ax.units = powspec.Pk.units * powspec.k.units ** 3
+        ax.units = powspec.Pk_z0_unnormalised.units * powspec.k.units ** 3
         return ax
 
     if arg_is_R:
-        R = M
+        R = M_or_R
     else:
-        R = f_filter.M_to_R(M)
+        R = f_filter.M_to_R(M_or_R)
 
     integrand = lambda k: k ** 2 * powspec(k) * f_filter.Wk(k * R) ** 2
     integrand_ln_k = lambda k: np.exp(k) * integrand(np.exp(k))
-    v = scipy.integrate.romberg(integrand_ln_k, math.log(powspec.min_k), math.log(
-        1. / R) + 3, divmax=10, rtol=1.e-4) / (2 * math.pi ** 2)
+    v =  scipy.integrate.quad(integrand_ln_k, math.log(powspec.min_k), math.log(
+        1. / R) + 3, epsrel=1.e-6)[0] / (2 * math.pi ** 2)
 
     return v
 
 
-def estimate_neffm(M, f_filter=TophatFilter, powspec=PowerSpectrumCAMB, arg_is_R=False):
-    # this routine is opaque and inefficient
-    dlnm = 0.01  # just needs to be small
-
-# if hasattr(M,'__len__') : ## why is this needed?
-#        ax =  pynbody.array.SimArray([estimate_neffm(Mi, f_filter, powspec) for Mi in M])
-# ax.units = powspec.Pk.units/ powspec.Pk.units * powspec.k.units**3 / powspec.k.units**3  # hopefully dimensionless
-#        return ax
-
-    M2 = np.exp(np.log(M) + dlnm)
-    sig = np.sqrt(variance(M, f_filter, powspec))
-    sig2 = np.sqrt(variance(M2, f_filter, powspec))
-    #  neff = 6 dlnsigmainv / dlnm, eq. 13 reed et al. 2007
-    neff = 6. * (np.log(sig / sig2)) / dlnm - 3.
-
-    return neff
-
-
 def get_neffm(mass, sigma):
-            #  neff = 6 dlnsigmainv / dlnm - 3, eq. 13 reed et al. 2007
+    """Calculate the effective spectral index of the power spectrum at a given mass scale."""
     dlnm = np.diff(np.log(mass))
     dlnsigmainv = np.diff(np.log(1. / sigma))
     neff = 6. * dlnsigmainv / dlnm - 3.
     return neff
 
 
 @units.takes_arg_in_units((0, "Mpc h^-1"))
-def correlation(r, powspec=PowerSpectrumCAMB):
+def correlation(r, powspec=PowerSpectrum):
+    """Calculate the correlation function of the density field at a specified radius."""
 
     if hasattr(r, '__len__'):
         ax = pynbody.array.SimArray([correlation(ri,  powspec) for ri in r])
-        ax.units = powspec.Pk.units * powspec.k.units ** 3
+        ax.units = powspec.Pk_z0_unnormalised.units * powspec.k.units ** 3
         return ax
 
     # Because sin kr becomes so highly oscilliatory, normal
     # quadrature is slow/inaccurate for this problem. The following
     # is the best way I could come up with to overcome that.
     #
     # For small kr, sin kr/kr is represented as a Taylor expansion and
@@ -404,44 +477,46 @@
 
     return tot
 
 
 def correlation_func(context, log_r_min=-3, log_r_max=2, delta_log_r=0.2,
                      pspec=PowerSpectrumCAMB):
     """
-
     Calculate the linear density field correlation function.
 
-    **Args**:
+    Parameters
+    ----------
 
-    *context* (SimSnap): The snapshot from which to pull the
-        cosmological context (includes sigma8 normalization and growth
-        function integrations, but does not currently affect transfer
-        function)
+    context : SimSnap
+        The snapshot from which to pull the cosmological context
 
-    **Kwargs:**
+    log_r_min : float, optional
+        log10 of the minimum separation (Mpc h^-1) to consider
 
-      *log_r_min:* log10 of the minimum separation (Mpc h^-1) to
-       consider
+    log_r_max : float, optional
+        log10 of the maximum separation (Mpc h^-1) to consider
 
-      *log_r_max:* log10 of the maximum separation (Mpc h^-1) to
-       consider
+    delta_log_r : float, optional
+        The value spacing in dex
 
-      *delta_log_r:* The value spacing in dex
+    pspec : PowerSpectrum, optional
+        The power spectrum class to use, or if an instance is provided, the power spectrum to use.
+        The default is to use PowerSpectrumCAMB which will attempt to calculate a power spectrum
+        from the simulation context; if it fails, it will fall back to using Planck2018 power spectrum
+        and issue a warning.
 
-      *pspec:* A power spectrum object; default is a WMAP7 cosmology
-        calculated by CAMB.
+    Returns
+    -------
 
-    **Returns:**
+    r : array
+        The separation values in Mpc h^-1
 
-      *r:* Array of the r values (Mpc h^-1) for which the correlation
-         function was evaluated.
+    Xi : array
+        The correlation function at each separation
 
-      *Xi:* Array of the dimensionless correlation for each
-       separation.
 
     """
 
     if isinstance(pspec, type):
         pspec = pspec(context)
 
     r = (10.0 ** np.arange(log_r_min, log_r_max + delta_log_r / 2,
@@ -457,62 +532,62 @@
     return r, Xi_r
 
 #######################################################################
 # Default kernels for halo mass function
 #######################################################################
 
 
-def f_press_schechter(nu):
+def _f_press_schechter(nu):
     """
 
     The Press-Schechter kernel used by halo_mass_function
 
     """
 
     f = math.sqrt(2. / math.pi) * nu * np.exp(-nu * nu / 2.)
     return f
 
 
-def f_sheth_tormen(nu, Anorm=0.3222, a=0.707, p=0.3):
+def _f_sheth_tormen(nu, Anorm=0.3222, a=0.707, p=0.3):
     """
     Sheth & Tormen (1999) fit (see also Sheth Mo & Tormen 2001)
     """
     #  Anorm: normalization, set so all mass is in halos (integral [f nu dn]=1)
     #  a: affects mainly the number of massive halo,
     #  a=0.75 is favored by Sheth & Tormen (2002)
 
     f = Anorm * math.sqrt(2. * a / math.pi) * \
         (1. + np.power((1. / a / nu / nu), p))
     f *= nu * np.exp(-a * nu * nu / 2.)
     return f
 
 
-def f_jenkins(nu, deltac=1.68647):
+def _f_jenkins(nu, deltac=1.68647):
     # Jenkins et al (2001) fit   ##  valid for  -1.2 << ln(1/sigma) << 1.05
     sigma = deltac / nu
     lnsigmainv = np.log(1. / sigma)
     if ((np.any(lnsigmainv < -1.2)) or (np.any(lnsigmainv > 1.05))):
         logger.warning(
             "Jenkins mass function is outsie of valid mass range.  Continuing calculations anyway.")
     f = 0.315 * np.exp(-np.power((np.fabs(lnsigmainv + 0.61)), 3.8))
     return f
 
 
-def f_warren(nu, deltac=1.68647):
+def _f_warren(nu, deltac=1.68647):
     #  Warren et al. 2006  -- valid for (10**10 - 10**15 Msun/h)
     sigma = deltac / nu
     A = 0.7234
     a = 1.625
     b = 0.2538
     c = 1.1982
     f = A * (np.power(sigma, -a) + b) * np.exp(-c / sigma ** 2)
     return f
 
 
-def f_reed_no_z(nu, deltac=1.68647):  # universal form
+def _f_reed_no_z(nu, deltac=1.68647):  # universal form
     # Reed et al. (2007) fit, eqn. 9 -- with no redshift depedence (simple
     # universal form)
     """ modified S-T fit  by the G1 gaussian term and c"""
     sigma = deltac / nu
     # normalization that all mass is in halos not strictly conserved here
     Anorm = 0.3222
     a = 0.707  # affects mostly the number of massive halos
@@ -524,15 +599,15 @@
     G1 = np.exp(-np.power((lnsigmainv - 0.4), 2) / (2. * 0.6 * 0.6))
     f = Anorm * np.sqrt(2. * a / np.pi) * \
         (1. + np.power((1. / a / nu / nu), p) + 0.2 * G1)
     f *= nu * np.exp(-c * a * nu * nu / 2.)
     return f
 
 
-def f_reed_z_evo(nu, neff, deltac=1.68647):  # non-universal form
+def _f_reed_z_evo(nu, neff, deltac=1.68647):  # non-universal form
     # Reed et al. (2007) fit, eqn. 11 -- with redshift depedence for accuracy
     # at z >~ z_reion
     """ modified S-T fit  by the n_eff dependence and the G1 and G2 gaussian terms and c
     where   P(k) proportional to k_halo**(n_eff)  and
     k_halo = Mhalo / r_halo_precollapse.
     eqn 13 of Reed et al 2007   estimtes neff = 6 d ln(1/sigma(M))/ d ln M  - 3 """
     sigma = deltac / nu
@@ -550,125 +625,128 @@
                                            np.power((1. / a / nu / nu), p) + 0.6 * G1 + 0.4 * G2)
     f *= nu * \
         np.exp(-c * a * nu * nu / 2. - 0.03 / (neff + 3)
                ** 2 * np.power(nu, 0.6))
     return f
 
 
-def f_bhattacharya(nu, red, deltac=1.68647):
+def _f_bhattacharya(nu, red, deltac=1.68647):
     # Bhattacharya et al. 2010  -- 6x10**11 - 310**15 Msun/h  z=0-2
     sigma = deltac / nu
     A = 0.333 / pow((1. + red), 0.11)
     a = 0.788 / pow((1. + red), 0.01)
     p = 0.807 / pow((1. + red), 0.0)
     q = 1.795 / pow((1. + red), 0.0)
     f = A * np.sqrt(2. / np.pi) * (1. + np.power((1. / a / nu / nu), p))
     f *= np.power(nu * math.sqrt(a), q) * np.exp(-a * nu * nu / 2.)
     return f
 
-
-#######################################################################
-# Bias functions
-#######################################################################
-
-def cole_kaiser_bias(nu, delta_c):
+def _cole_kaiser_bias(nu, delta_c):
     """
 
     The Cole-Kaiser (1989) bias function. Also in Mo & White 1996.
 
     """
     return 1 + (nu ** 2 - 1) / delta_c
 
 
-def sheth_tormen_bias(nu, delta_c,
-                      a=0.707, b=0.5, c=0.6):
+def _sheth_tormen_bias(nu, delta_c,
+                       a=0.707, b=0.5, c=0.6):
     """
 
     The Sheth-Tormen (1999) bias function [eq 8]
 
     """
 
     root_a = math.sqrt(a)
 
     return 1. + (root_a * a * nu ** 2 + root_a * b * (a * nu ** 2) ** (1. - c)
                  - (a * nu ** 2) ** c / ((a * nu ** 2) ** c + b * (1 - c) * (1 - c / 2))) \
         / (root_a * delta_c)
 
-#######################################################################
-# The most useful function: halo_mass_function
-#######################################################################
 
 
 def halo_mass_function(context,
                        log_M_min=8.0, log_M_max=15.0, delta_log_M=0.1,
                        kern="ST",
-                       pspec=PowerSpectrumCAMB,
-                       delta_crit=1.686,
-                       no_h=False):
+                       pspec=PowerSpectrum,
+                       delta_crit=1.686):
     """
+    Returns the halo mass function, dN/d log_{10} M in units of Mpc^-3 h^3.
 
-    Returns the halo mass function, dN/d log_{10} M in units of Mpc^-3
-    h^3.
+    See :ref:`hmf_tutorial` for an example and more information.
 
-    **Args:**
 
-    *context (SimSnap):* The snapshot from which to pull the
-    cosmological context (includes sigma8 normalization and growth
-    function integrations, but does not currently affect transfer
-    function)
+    Parameters
+    ----------
 
-    **Kwargs:**
+    context : SimSnap
+        The snapshot from which to pull the cosmological context. Sigma8 normalization and growth function
+        redshift dependence is always taken into account. If `camb <https://camb.readthedocs.io/en/latest/>`_ is
+        installed, an appropriate power spectrum is calculated for other cosmological parameters (e.g. baryon
+        density, Hubble constant) from the simulation. Otherwise, a default Planck18 power spectrum is
+        used.
 
-    *log_M_min:* The minimum halo mass (Msol h^-1) to consider
+    log_M_min : float, optional
+        The minimum halo mass (Msol h^-1) to consider. Default is 8.
 
-    *log_M_max:* The maximum halo mass (Msol h^-1) to consider
+    log_M_max : float, optional
+        The maximum halo mass (Msol h^-1) to consider. Default is 15.
 
-    *delta_log_M:* The bin spacing of halo masses (see warning below)
+    delta_log_M : float, optional
+        The bin spacing of halo masses. Default is 0.1.
 
-    *kern:* The kernel function which dictates what type of mass
-    function to calculate; or a string ("PS" or "ST") for one
-    of the defaults
+    kern : str or function, optional
+        The kernel function which dictates what type of mass function to calculate. Default is "ST" (Sheth-Tormen).
+        Other options are "PS" (Press-Schechter), "J" (Jenkins), "W" (Warren), "REEDZ" (Reed et al 2007 with redshift
+        dependence), "REEDU" (Reed et al 2007 without redshift dependence), "B" (Bhattacharya).
 
-    *pspec:* A power spectrum object (which also defines the window
-    function); default is a WMAP7 cosmology calculated by
-    CAMB, and a top hat window
+    pspec : PowerSpectrumCAMB, optional
+        A power spectrum object (which also defines the window function), overriding the cosmological
+        parameters of the simulation.
 
-    *delta_crit:* The critical overdensity for collapse
+    delta_crit : float, optional
+        The critical overdensity for collapse. Default is 1.686.
 
-    **Returns:**
+    Returns
+    -------
 
-    *M:* The centre of the mass bins, in Msol h^-1
+    M : SimArray
+        The centre of the mass bins, in Msol h^-1.
 
-    *sigma:* The linear variance of the corresponding sphere
+    sigma : SimArray
+        The linear variance of the corresponding sphere.
 
-    *N:* The abundance of halos of that mass (Mpc^-3 h^3 comoving,
-    per decade of mass)
+    N : SimArray
+        The abundance of halos of that mass (Mpc^-3 h^3 comoving, per decade of mass).
 
-    Because numerical derivatives are involved, the value of
-    delta_log_M affects the accuracy. Numerical experiments suggest
-    that delta_log_M=0.1 gives more than enough accuracy, but you
-    should check for your own use case.
+    Notes
+    -----
 
+    Because numerical derivatives are involved, the value of ``delta_log_M`` affects the accuracy.
 
-    Recommended m.f. for friends-of-friends linking length 0.2 particle sep.:
-    z <~ 2 : bhattacharya
-    z >~ 5 : reed_universal (no redshift dependence)
-    : or reed_evolving (w/redshift dependence for additional accuracy)
+    The halo mass function code in pynbody was implemented in 2012 when there
+    were no other python libraries that could do this.
+    Since then, cosmology-focussed libraries such as `hmf <https://hmf.readthedocs.io/en/latest/index.html>`_,
+    and `CCL <https://halotools.readthedocs.io/en/latest/>`_ have been developed.
+    For precision cosmology applications, we recommend using these libraries.
+
+    The functionality here is retained for quick cross-checks of simulations.
 
     """
 
     if isinstance(kern, str):
-        kern = {'PS': f_press_schechter,
-                'ST': f_sheth_tormen,
-                'J': f_jenkins,
-                'W': f_warren,
-                'REEDZ': f_reed_z_evo,
+        kern = {'PS': _f_press_schechter,
+                'ST': _f_sheth_tormen,
+                'J': _f_jenkins,
+                'W': _f_warren,
+                'REEDZ': _f_reed_z_evo,
                 # Reed et al 2007 without redshift dependence
-                'REEDU': f_reed_no_z,
-                'B': f_bhattacharya}[kern]
+                'REEDU': _f_reed_no_z,
+                'B': _f_bhattacharya}[kern]
 
     rho_bar = cosmology.rho_M(context, unit="Msol Mpc^-3 h^2")
     red = context.properties['z']  # redshift is always set by simulation
 
     M = np.arange(log_M_min, log_M_max, delta_log_M)
     M_mid = np.arange(
         log_M_min + delta_log_M / 2, log_M_max - delta_log_M / 2, delta_log_M)
@@ -683,20 +761,19 @@
 
     nu_mid = (nu[1:] + nu[:-1]) / 2
 
     d_ln_nu_d_ln_M = np.diff(np.log10(nu)) / delta_log_M
 
     dM = np.diff(10 ** M)
 
-    if (kern == f_reed_z_evo):
-        ##    neff = estimate_neffm(M)
+    if (kern == _f_reed_z_evo):
         neff = get_neffm(10. ** M, sig ** 0.5)
         out = (rho_bar / (10 ** M_mid)) * kern(nu_mid, neff) * \
             d_ln_nu_d_ln_M * math.log(10.) * context.properties['a'] ** 3
-    elif (kern == f_bhattacharya):
+    elif (kern == _f_bhattacharya):
        # eq 7.46, Mo, van den Bosch and White
         out = (rho_bar / (10 ** M_mid)) * kern(nu_mid, red) * \
             d_ln_nu_d_ln_M * math.log(10.) * context.properties['a'] ** 3
     else:
         # eq 7.46, Mo, van den Bosch and White
         out = (rho_bar / (10 ** M_mid)) * kern(nu_mid) * \
             d_ln_nu_d_ln_M * math.log(10.) * context.properties['a'] ** 3
@@ -710,114 +787,143 @@
     # interpolate sigma for output checking purposes
     sig = (sig[1:] + sig[:-1]) / 2
 
     return M_mid, np.sqrt(sig), out
 
 
 @units.takes_arg_in_units((1, "Msol h^-1"), context_arg=0)
-def halo_bias(context, M, kern=cole_kaiser_bias, pspec=PowerSpectrumCAMB,
+def halo_bias(context, M, kern="CK", pspec=PowerSpectrumCAMB,
               delta_crit=1.686):
     """
-
     Return the halo bias for the given halo mass.
 
-    **Args:**
+    Parameters
+    ----------
 
-       *context (SimSnap):* The snapshot from which to pull the
-        cosmological context
+    context : SimSnap
+        The snapshot from which to pull the cosmological context
 
-       *M:* float, unit or string describing the halo mass. If a
-        float, units are Msol h^-1.
+    M : float
+        The halo mass in Msol h^-1
 
-    **Kwargs:**
+    kern : str or function, optional
+        The kernel function describing the halo bias. Default is "CK" (Cole-Kaiser).
+        Other options are "ST" (Sheth-Tormen). Alternatively a function can be provided.
 
-       *kern:* The kernel function describing the halo bias (default
-        Cole-Kaiser).
+    pspec : PowerSpectrum, optional
+        The power spectrum class to use, or if an instance is provided, the power spectrum to use.
+        Default is PowerSpectrumCAMB which will attempt to calculate a power spectrum from the simulation context;
+        if it fails, it will fall back to using Planck2018 power spectrum and issue a warning.
 
-       *pspec:* A power spectrum object (which also defines the window
-              function); default is a WMAP7 cosmology calculated by
-              CAMB, and a top hat window
+    delta_crit : float, optional
+        The critical overdensity for collapse. Default is 1.686.
 
-       *delta_crit:* The critical overdensity for collapse
+    Returns
+    -------
 
-    **Returns:**
-
-       The halo bias (single float)
+    float
+        The halo bias for the given halo mass.
 
     """
 
+    if isinstance(kern, str):
+        kern = {'CK': _cole_kaiser_bias,
+                'ST': _sheth_tormen_bias}[kern]
+
     if isinstance(pspec, type):
         pspec = pspec(context)
 
     sig = variance(M, pspec._default_filter, pspec)
     nu = delta_crit / np.sqrt(sig)
 
     return kern(nu, delta_crit)
 
 
-def simulation_halo_mass_function(snapshot,
+def simulation_halo_mass_function(snapshot_or_cat,
                                   log_M_min=8.0, log_M_max=15.0, delta_log_M=0.1,
-                                  masses=None, mass_def="halo_finder", calculate_err=True,
+                                  masses=None, mass_property=None, calculate_err=True,
                                   subsample_catalogue=None):
-    """
+    """Estimate a halo mass function from a simulation, via binning haloes in mass.
 
-    Construct the halo mass function from a halo catalogue by binning haloes in mass and counting them.
-    This allows direct plotting of the simulation HMF against the theory HMF.
+    Parameters
+    ----------
 
-    **Args:**
+    snapshot_or_cat : SimSnap or HaloCatalogue
+        The snapshot from which to calculate the halo mass function, or the halo catalogue itself.
+        If a snapshot is provided, ``.halos()`` is called to get the first available catalogue.
 
-       *snapshot (SimSnap):* The snapshot from which to calculate halo masses
+    log_M_min : float, optional
+        The minimum halo mass (Msol h^-1) to consider. Default is 8.
 
-    **Kwargs:**
+    log_M_max : float, optional
+        The maximum halo mass (Msol h^-1) to consider. Default is 15.
 
-        *log_M_min:* The minimum halo mass (Msol h^-1) to consider
+    delta_log_M : float, optional
+        The bin spacing of halo masses. Default is 0.1.
 
-        *log_M_max:* The maximum halo mass (Msol h^-1) to consider
+    masses : array, optional
+        Provide an array of halo masses in Msol h^-1. If None, this is calculated from the snapshot.
 
-        *delta_log_M:* The bin spacing of halo masses
+    mass_property : str, optional
+        The property name giving the mass of each halo. If None, sums the mass in particles in each halo
+        according to the particle data in the catalogue. Summing masses can be slow for large catalogues.
 
-        *masses: Provide array of halo masses in Msol h**-1. If none, this is calculated from the snapshot.
+    calculate_err : bool, optional
+        If True, estimates error bars according to Poisson statistics.
 
-        *mass_def: Definition of the mass of a halo. Possible extensions could be M200_crit, M200_matter, Mvir etc...
+    subsample_catalogue : int, optional
+        Subsample the halo catalogue by the specified factor. Not recommended except for debugging.
 
-        *err: If true, calculates error bars according to Poisson process.
+    Returns
+    -------
 
-        *subsample_catalogue: Sample the halo catalogue every int value. Mostly for speed and debugging issues.
-        WARNING: If your halo catalogue is ordered, this method does not take responsability in randomising the catalogue so
-        you might not recover the true HMF.
+    bin_centers : SimArray
+        The centre of the mass bins, in Msol h^-1.
 
-    **Returns:**
+    num_den : SimArray
+        The binned number density of haloes in this snapshot in comoving Mpc**-3 h**3 per decade of mass.
 
-       The binned number density of haloes in this snapshot in comoving Mpc**-3 h**3 per decade of mass
+    err : SimArray
+        The error on the number density, if ``calculate_err`` is True.
 
     """
 
+    if isinstance(snapshot_or_cat, pynbody.snapshot.SimSnap):
+        snapshot = snapshot_or_cat
+        halo_catalogue = snapshot.halos()
+    elif isinstance(snapshot_or_cat, pynbody.halo.HaloCatalogue):
+        halo_catalogue = snapshot_or_cat
+        snapshot = halo_catalogue.base
+    else:
+        raise TypeError("snapshot_or_cat must be a SimSnap or HaloCatalogue")
+
+
     #Check that the mass resolution is uniform, this method does not handle otherwise
     if len(set(snapshot.d['mass'])) > 1:
         warnings.warn( "The mass resolution of the snapshot is not uniform (e.g. zooms). This method"
                        "will not generate a correct HMF in this case.")
 
     nbins = int(1 + (log_M_max - log_M_min)/delta_log_M)
     bins = np.logspace(log_M_min, log_M_max, num=nbins, base=10)
     bin_centers = (bins[:-1] + bins[1:]) / 2
 
-    halo_catalogue = snapshot.halos()
     halo_catalogue.load_all()
 
     if subsample_catalogue is not None:
         halo_catalogue_underlying = halo_catalogue # keep alive for the lifetime of the function
         halo_catalogue = halo_catalogue[::subsample_catalogue]
 
     if masses is None:
-        warnings.warn("Halo finder masses not provided. Calculating them (might take a while...)")
-
-        if mass_def=="halo_finder":
+        if mass_property is None:
+            warnings.warn("Halo finder masses not provided. Calculating them (might take a while...)")
             masses = np.array([h['mass'].sum().in_units('1 h**-1 Msol') for h in halo_catalogue])
         else:
-            raise KeyError("Only halo finder mass is supported in this calculation for now")
+            masses = halo_catalogue.get_properties_all_halos(with_units=True)[mass_property]
+            if units.has_unit(masses):
+                masses = masses.in_units('1 h**-1 Msol')
 
     if np.amax(masses) > 10**log_M_max or np.amin(masses) < 10**log_M_min :
         warnings.warn("Your bin range does not encompass the full range of halo masses")
 
     # Calculate number of halos in each bin
     num_halos = np.histogram(masses, bins)[0]
 
@@ -830,20 +936,20 @@
 
     num_halos = num_halos  / normalisation
 
 
     # Make sure units are consistent
     bin_centers = bin_centers.view(pynbody.array.SimArray)
     bin_centers.units = "Msol h**-1"
-    bin_centers.context = snapshot
+    bin_centers.sim = snapshot
 
     num_halos = num_halos.view(pynbody.array.SimArray)
     num_halos.units = "a**-3 Mpc**-3 h**3"
-    num_halos.context = snapshot
+    num_halos.sim = snapshot
 
     if calculate_err:
         err = err.view(pynbody.array.SimArray)
         err.units = "a**-3 Mpc**-3 h**3"
-        err.context = snapshot
+        err.sim = snapshot
         return bin_centers, num_halos, err
     else:
         return bin_centers, num_halos
```

### Comparing `pynbody-2.0.0b7/pynbody/analysis/interpolate.py` & `pynbody-2.0.0b8/pynbody/analysis/interpolate.py`

 * *Files identical despite different names*

### Comparing `pynbody-2.0.0b7/pynbody/analysis/ionfrac.py` & `pynbody-2.0.0b8/pynbody/analysis/ionfrac.py`

 * *Files identical despite different names*

### Comparing `pynbody-2.0.0b7/pynbody/analysis/ionfracs.npz` & `pynbody-2.0.0b8/pynbody/analysis/ionfracs.npz`

 * *Files identical despite different names*

### Comparing `pynbody-2.0.0b7/pynbody/analysis/luminosity.py` & `pynbody-2.0.0b8/pynbody/analysis/luminosity.py`

 * *Files identical despite different names*

### Comparing `pynbody-2.0.0b7/pynbody/analysis/pkdgrav_cosmo.py` & `pynbody-2.0.0b8/pynbody/analysis/pkdgrav_cosmo.py`

 * *Files identical despite different names*

### Comparing `pynbody-2.0.0b7/pynbody/analysis/profile.py` & `pynbody-2.0.0b8/pynbody/analysis/profile.py`

 * *Files identical despite different names*

### Comparing `pynbody-2.0.0b7/pynbody/analysis/ramses_util.py` & `pynbody-2.0.0b8/pynbody/analysis/ramses_util.py`

 * *Files 1% similar despite different names*

```diff
@@ -402,14 +402,14 @@
 
         time_tot = age(top, z=0) * H0
         birth_date = (time_tot + times) / H0
     else:
         h0 = top.properties["h"]
         aexp_bins = np.geomspace(1e-3, 1, 10_000)
         z_bins = 1 / aexp_bins - 1
-        tau_bins = tau(top, z=z_bins) * h0
+        tau_bins = tau(top, z=z_bins, unit="0.01 s Mpc km^-1") * h0
         age_bins = age(top, z=z_bins)
         birth_date = np.interp(birth_raw, tau_bins, age_bins)
 
     top.s["tform"] = birth_date
     top.s['tform'].units = "Gyr"
     return sim.s["tform"]
```

### Comparing `pynbody-2.0.0b7/pynbody/analysis/theoretical_profiles.py` & `pynbody-2.0.0b8/pynbody/analysis/theoretical_profiles.py`

 * *Files identical despite different names*

### Comparing `pynbody-2.0.0b7/pynbody/array/__init__.py` & `pynbody-2.0.0b8/pynbody/array/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 """
-array
-=====
+Arrays for simulation data
+==========================
 
-Defines a shallow wrapper around numpy.ndarray for extra functionality like unit-tracking.
+The main class defined in this module is the `SimArray` class, which defines a shallow wrapper around ``numpy.ndarray``
+for extra functionality like unit-tracking.
 
 For most purposes, the differences between numpy.ndarray and
 array.SimArray are not important. However, when units are specified
 (by setting the ``units`` attribute), the behaviour is slightly
 different. In particular,
 
 * it becomes impossible to add or subtract arrays with incompatible dimensions
@@ -40,16 +41,16 @@
 can represent a rational number, in this case one third.
 
 >>> SimArray([1.,2], "Msol Mpc**-3")**0.333
 SimArray([ 1.,1.26])  # Lost track of units
 
 
 
-*Getting the array in specified units*
---------------------------------------
+Getting the array in specified units
+------------------------------------
 
 Given an array, you can convert it in-place into units of your
 own chosing:
 
 >>> x = SimArray([1,2], "Msol")
 >>> x.convert_units('kg')
 >>> print(x)
@@ -86,16 +87,16 @@
          [ 1620.68592366, -1824.15000686, -4545.69387564],
          ...,
          [ 2065.9264273 , -2185.92982874, -2187.79225915],
          [ 2047.60759667, -2129.6537339 , -2291.6758134 ],
          [ 2047.2214441 , -2133.87693163, -2291.59406997]], 'kpc')
 
 
-*Specifying rules for ufunc's*
-------------------------------
+Specifying rules for ufunc's
+-----------------------------
 
 In general, it's not possible to infer what the output units from a given
 ufunc should be. While numpy built-in ufuncs should be handled OK, other
 ufuncs will need their output units defined (otherwise a numpy.ndarray
 will be returned instead of our custom type.)
 
 To do this, decorate a function with SimArray.ufunc_rule(ufunc). The function
@@ -135,50 +136,54 @@
         elif a_units is not None :
             return a_units
         else :
             return b_units
 
 """
 
+from __future__ import annotations
+
 import fractions
 import functools
 import logging
-import os
-import random
-import time
 import weakref
+from typing import TYPE_CHECKING
 
 import numpy as np
 
-from .. import units as units
+from .. import units
+
+if TYPE_CHECKING:
+    from .. import family, snapshot
 
 _units = units
 
 logger = logging.getLogger('pynbody.array')
 
 
 
 
 
 class SimArray(np.ndarray):
-
-    """
-    Defines a shallow wrapper around numpy.ndarray for extra
-    functionality like unit-tracking.
-    """
+    """A shallow wrapper around numpy.ndarray for extra functionality like unit-tracking."""
 
     _ufunc_registry = {}
 
+    __slots__ = ['_units', '_sim', '_name', '_family']
+
     @property
     def ancestor(self):
         """Provides the basemost SimArray that an IndexedSimArray is based on."""
         return self
 
     @property
     def derived(self):
+        """True if this array has been derived by pynbody; False otherwise.
+
+        For more information on derived arrays, see :ref:`derived_arrays`."""
         if self.sim and self.name:
             return self.sim.is_derived_array(self.name, getattr(self, 'family', None))
         else:
             return False
 
     @derived.setter
     def derived(self, value):
@@ -195,16 +200,25 @@
 
     def __setstate__(self, args):
         self._units = args[0]
         self.sim = None
         self._name = None
         np.ndarray.__setstate__(self, args[1:])
 
-    def __new__(subtype, data, units=None, sim=None, **kwargs):
-        new = np.array(data, **kwargs).view(subtype)
+    def __init__(self, data, units = None, sim = None, **kwargs):
+        """Initialise a SimArray with the specified units and simulation context.
+
+        Other arguments are as for numpy.ndarray. If the data argument is a SimArray, the units and sim arguments are ignored."""
+
+        # The actual initialisation is done by __new__ (it's actually unclear to me now why that should be the case,
+        # but it's been like this for a long time and so changing it would need to be handled with care.)
+        pass
+
+    def __new__(cls, data, units=None, sim=None, **kwargs):
+        new = np.array(data, **kwargs).view(cls)
         if hasattr(data, 'units') and hasattr(data, 'sim') and units is None and sim is None:
             units = data.units
             sim = data.sim
 
         if hasattr(data, 'family'):
             new.family = data.family
 
@@ -242,14 +256,49 @@
             if hasattr(obj, 'family'):
                 self.family = obj.family
         else:
             self._units = None
             self._sim = lambda: None
             self._name = None
 
+    def __array_function__(self, func, types, args, kwargs):
+        ok_types = (SimArray, np.ndarray)
+        if not all(issubclass(t, ok_types) for t in types):
+            return NotImplemented
+
+        args_processed = []
+        for arg in args:
+            if isinstance(arg, SimArray):
+                args_processed.append(arg.view(np.ndarray))
+            else:
+                args_processed.append(arg)
+
+        kwargs_processed= {}
+        for k, v in kwargs.items():
+            if isinstance(v, SimArray):
+                kwargs_processed[k] = v.view(np.ndarray)
+            else:
+                kwargs_processed[k] = v
+
+        result = func(*args_processed, **kwargs_processed)
+
+        if func in SimArray._ufunc_registry:
+            result = result.view(SimArray)
+            if isinstance(result, SimArray): # may not be true if the result is a scalar
+                sim = None
+                for arg in args:
+                    if isinstance(arg, SimArray):
+                        sim = arg.sim
+                        break
+                result.units = SimArray._ufunc_registry[func](*args, **kwargs)
+                result.sim = sim
+
+        return result
+
+
     def __array_wrap__(self, array, context=None):
         if context is None:
             n_array = array.view(SimArray)
             return n_array
 
         try:
             ufunc = context[0]
@@ -267,15 +316,16 @@
         def x(fn):
             SimArray._ufunc_registry[for_ufunc] = fn
             return fn
 
         return x
 
     @property
-    def units(self):
+    def units(self) -> units.UnitBase:
+        """The units of the array, if known; otherwise :ref:`units.NoUnit`."""
         if hasattr(self.base, 'units'):
             return self.base.units
         else:
             if self._units is None:
                 return _units.no_unit
             else:
                 return self._units
@@ -290,22 +340,23 @@
         else:
             if hasattr(u, "_no_unit"):
                 self._units = None
             else:
                 self._units = u
 
     @property
-    def name(self):
+    def name(self) -> str | None:
+        """The name of the array in the simulation snapshot, if known."""
         if hasattr(self.base, 'name'):
             return self.base.name
         return self._name
 
     @property
-    def sim(self):
-
+    def sim(self) -> snapshot.SimSnap | None:
+        """The simulation snapshot that the array belongs to, if known."""
         if hasattr(self.base, 'sim'):
             base_sim = self.base.sim
         else:
             base_sim = self._sim()
 
         if self.family is not None and base_sim is not None:
             return base_sim[self.family]
@@ -320,15 +371,22 @@
         else:
             if s is not None:
                 self._sim = weakref.ref(s)
             else:
                 self._sim = lambda: None
 
     @property
-    def family(self):
+    def family(self) -> family.Family | None:
+        """Returns the pynbody family that the array belongs to, if any.
+
+        If ``family`` isn't None, an array ``a`` belongs to ``a.sim[family]`` rather than ``a.sim``.
+
+        This doesn't necessarily mean that it is a family-level array, however, since it could be a slice into
+        a simulation array.
+        """
         try:
             return self._family
         except AttributeError:
             return None
 
     @family.setter
     def family(self, fam):
@@ -388,14 +446,17 @@
             try:
                 self.units /= rhs.units
             except AttributeError:
                 pass
         return self
 
     def conversion_context(self):
+        """Return a dictionary of contextual information that may be required for unit conversion.
+
+        This is typically cosmological scalefactor and Hubble parameter."""
         if self.sim is not None:
             return self.sim.conversion_context()
         else:
             return {}
 
     def _generic_add(self, x, add_op=np.add):
         if hasattr(x, 'units') and not hasattr(self.units, "_no_unit") and not hasattr(x.units, "_no_unit"):
@@ -546,15 +607,16 @@
         if hasattr(x, 'units') and self.units is not None:
             x.units = self.units
         if hasattr(x, 'sim') and self.sim is not None:
             x.sim = self.sim
         return x
 
     def mean_by_mass(self, *args, **kwargs):
-        return self.sim.mean_by_mass(self.name)
+        """Removed in pynbody 2.0. Use :func:`pynbody.snapshot.simsnap.SimSnap.mean_by_mass` instead."""
+        raise RuntimeError("SimArray.mean_by_mass has been removed. Use SimSnap.mean_by_mass instead.")
 
     def max(self, *args, **kwargs):
         x = np.ndarray.max(self, *args, **kwargs)
         if hasattr(x, 'units') and self.units is not None:
             x.units = self.units
         if hasattr(x, 'sim') and self.sim is not None:
             x.sim = self.sim
@@ -589,60 +651,94 @@
         if hasattr(x, 'units') and self.units is not None:
             x.units = self.units ** 2
         if hasattr(x, 'sim') and self.sim is not None:
             x.sim = self.sim
         return x
 
     def set_units_like(self, new_unit):
-        """Set the units for this array by performing dimensional analysis
-        on the supplied unit and referring to the units of the original
-        file"""
+        """Set the units of this array using a guess the ``sim``'s units for a given dimensionality.
+
+        For example, if ``sim`` has units of ``Msol`` and ``kpc``, and ``new_unit`` is ``kg m^-3``, the
+        units of this array will be set to ``Msol kpc^-3``.
+
+        The underlying code uses dimensional analysis; of course, simulation codes are free to use inconsistent
+        units if they like, so in general this routine cannot be guaranteed to infer the correct units. Human
+        cross-checks are strongly advised.
+
+        Note that this does not convert the array to the new units, it only sets the units attribute. To convert,
+        use :func:`in_units`, :func:`convert_units` or :func:`in_original_units`.
+        """
 
         if self.sim is not None:
             self.units = self.sim.infer_original_units(new_unit)
         else:
             raise RuntimeError("No link to SimSnap")
 
     def set_default_units(self, quiet=False):
-        """Set the units for this array by performing dimensional analysis
-        on the default dimensions for the array."""
+        """Set the units for this array by guessing the ``sim``'s unit scheme and known dimensionality information.
+
+        For example, if ``sim`` has units of ``Msol`` and ``kpc`` and this array is the ``rho`` array, the
+        units of this array will be set to ``Msol kpc^-3``.
+
+        The underlying code uses dimensional analysis; of course, simulation codes are free to use inconsistent
+        units if they like, so in general this routine cannot be guaranteed to infer the correct units. Human
+        cross-checks are strongly advised.
+
+        Note that this does not convert the array to the new units, it only sets the units attribute. To convert,
+        use :func:`in_units`, :func:`convert_units` or :func:`in_original_units`.
+        """
 
         if self.sim is not None:
             try:
                 self.units = self.sim._default_units_for(self.name)
             except (KeyError, units.UnitsException):
                 if not quiet:
                     raise
         else:
             raise RuntimeError("No link to SimSnap")
 
     def in_original_units(self):
-        """Retun a copy of this array expressed in the units
-        specified in the parameter file."""
+        """Return a copy of this array expressed in the file's internal unit scheme.
+
+        For example, if ``sim`` has units of ``Msol`` and ``kpc`` and this array is the ``rho`` array, a copy of the
+        array in units of ``Msol kpc^-3`` will be returned, even if the current units are something else like
+        ``kg m^-3``.
+
+        The underlying code uses dimensional analysis; of course, simulation codes are free to use inconsistent
+        units if they like, so in general this routine cannot be guaranteed to infer the correct units. Human
+        cross-checks are strongly advised.
+        """
 
         return self.in_units(self.sim.infer_original_units(self.units))
 
     def in_units(self, new_unit, **context_overrides):
-        """Return a copy of this array expressed relative to an alternative
-        unit."""
+        """Return a copy of this array, expressed relative to an alternative unit ``new_unit``.
+
+        Additional keyword arguments are interpreted as context overrides for the unit conversion. For example, if the
+        array is a comoving distance and you want to convert it to a physical distance, you might call
+
+        >>> x.in_units('kpc', a=0.1)
+
+        to get the result assuming a scalefactor 0.1. If no context overrides are given, the context of the underlying
+        ``sim`` is adopted.
+        """
 
         context = self.conversion_context()
         context.update(context_overrides)
 
         if self.units is not None:
             r = self * self.units.ratio(new_unit,
                                         **context)
             r.units = new_unit
             return r
         else:
             raise ValueError("Units of array unknown")
 
     def convert_units(self, new_unit):
-        """Convert units of this array in-place. Note that if
-        this is a sub-view, the entire base array will be converted."""
+        """Convert units of this array in-place. If this is a sub-view, the entire base array will be converted."""
 
         if self.base is not None and hasattr(self.base, 'units'):
             self.base.convert_units(new_unit)
         else:
             ratio = self.units.ratio(new_unit,
                                      **(self.conversion_context()))
             logger.debug("Converting %s units from %s to %s; ratio = %.3e" %
@@ -689,18 +785,18 @@
 
 for f in np.ndarray.__lt__, np.ndarray.__le__, np.ndarray.__eq__, \
         np.ndarray.__ne__, np.ndarray.__gt__, np.ndarray.__ge__:
 
     # N.B. cannot use functools.partial because it doesn't implement the descriptor
     # protocol
     @functools.wraps(f, assigned=("__name__", "__doc__"))
-    def wrapper_function(self, other, comparison_op=f):
+    def _wrapper_function(self, other, comparison_op=f):
         return _unit_aware_comparison(self, other, comparison_op=comparison_op)
 
-    setattr(SimArray, f.__name__, wrapper_function)
+    setattr(SimArray, f.__name__, _wrapper_function)
 
 
 # Now add dirty bit setters to all the operations which are known
 # to modify the numpy array
 
 def _dirty_fn(w):
     def q(a, *y, **kw):
@@ -842,26 +938,42 @@
 @_u(np.less)
 @_u(np.less_equal)
 @_u(np.equal)
 @_u(np.not_equal)
 def _comparison_units(*a):
     return None
 
+@_u(np.linalg.norm)
+def _norm_units(a, *args, **kwargs):
+    return a.units
+
 
 class IndexedSimArray:
+    """A view into a SimArray that allows for indexing and slicing.
 
+    Unlike numpy arrays, IndexedSimArrays do not copy data when indexed. Instead, they provide a view into the original
+    data. This is used by pynbody to provide a view into a subset of a simulation snapshot without copying the data,
+    while making sure any changes to the data are reflected in the original snapshot.
+
+    For most purposes, an IndexedSimArray should behave exactly like a SimArray. However, advanced users may want to
+    understand more about performance implications and ways to optimize code. This can be found in the
+    :ref:`performance` section of the documentation.
+    """
     @property
     def derived(self):
         return self.base.derived
 
     @property
     def ancestor(self):
         return self.base.ancestor
 
-    def __init__(self, array, ptr):
+    def __init__(self, array: SimArray, ptr: slice | np.ndarray):
+        """Initialise an IndexedSimArray based on an underlying SimArray and a pointer into that array.
+
+        The pointer can be a slice or an array of indexes."""
         self.base = array
         self._ptr = ptr
 
     def __array__(self, dtype=None):
         return np.asanyarray(self.base[self._ptr], dtype=dtype)
 
     def _reexpress_index(self, index):
@@ -948,35 +1060,47 @@
 
 # The IndexedSimArray class is now supplemented by wrapping all the
 # standard numpy methods with a generated function which extracts an
 # array realization of the subview before calling the underlying
 # method.
 
 def _wrap_fn(w):
+    @functools.wraps(w)
     def q(s, *y,  **kw):
         return w(SimArray(s), *y, **kw)
 
     q.__name__ = w.__name__
     return q
 
 # functions we definitely want to wrap, even though there's an existing
 # implementation
 _override = "__eq__", "__ne__", "__gt__", "__ge__", "__lt__", "__le__"
 
 for x in set(np.ndarray.__dict__).union(SimArray.__dict__):
-    w = getattr(SimArray, x)
-    if 'array' not in x and ((not hasattr(IndexedSimArray, x)) or x in _override) and hasattr(w, '__call__') and x!="__buffer__":
-        setattr(IndexedSimArray, x, _wrap_fn(w))
+    _w = getattr(SimArray, x)
+    if 'array' not in x and ((not hasattr(IndexedSimArray, x)) or x in _override) and hasattr(_w, '__call__') and x!="__buffer__":
+        setattr(IndexedSimArray, x, _wrap_fn(_w))
 
 
-def _array_factory(dims, dtype, zeros, shared):
+def array_factory(dims: int | tuple, dtype: np.dtype, zeros: bool, shared: bool) -> SimArray:
     """Create an array of dimensions *dims* with the given numpy *dtype*.
-    If *zeros* is True, the returned array is guaranteed zeroed. If *shared*
-    is True, the returned array uses shared memory so can be efficiently
-    shared across processes."""
+
+    Parameters
+    ----------
+
+    dims : int or tuple
+        The dimensions of the array.
+    dtype : numpy.dtype
+        The data type of the array.
+    zeros : bool
+        If True, the array is guaranteed to be zeroed.
+    shared : bool
+        If True, the array uses shared memory and can be efficiently shared across processes.
+
+    """
     if not hasattr(dims, '__len__'):
         dims = (dims,)
 
     if shared:
         from . import shared
         ret_ar = shared.make_shared_array(dims, dtype, zeros)
```

### Comparing `pynbody-2.0.0b7/pynbody/array/shared.py` & `pynbody-2.0.0b8/pynbody/array/shared.py`

 * *Files 6% similar despite different names*

```diff
@@ -10,28 +10,27 @@
 
 import numpy as np
 import posix_ipc
 
 from ..configuration import config_parser
 from . import SimArray
 
-DELAY_BEFORE_CLOSING_SHARED_MEM = float(config_parser.get('shared-array', 'cleanup-delay'))
-
 _owned_shared_memory_names = []
 
 class SharedArrayNotFound(OSError):
     pass
 
 class SharedMemorySimArray(SimArray):
-    __slots__ = ['_shared_fname']
+    __slots__ = ['_shared_fname', '_shared_owner']
     _shared_fname: str
+    _shared_owner: bool
 
     def __del__(self):
         global _owned_shared_memory_names
-        if hasattr(self, '_shared_fname'):
+        if hasattr(self, '_shared_fname') and getattr(self, '_shared_owner', False):
             if self._shared_fname in _owned_shared_memory_names:
                 _owned_shared_memory_names.remove(self._shared_fname)
                 posix_ipc.unlink_shared_memory(self._shared_fname)
 
 def make_shared_array(dims, dtype, zeros=False, fname=None, create=True,
                       offset = None, strides = None) -> SharedMemorySimArray:
     """Create an array of dimensions *dims* with the given numpy *dtype*.
@@ -96,14 +95,15 @@
     mem.close_fd()
 
     if offset is None:
         offset = 0
 
     ret_ar = np.frombuffer(mapped_mem, dtype=dtype, count=size, offset=offset).reshape(dims).view(SharedMemorySimArray)
     ret_ar._shared_fname = fname
+    ret_ar._shared_owner = create
 
     if strides:
         ret_ar.strides = strides
 
     if zero_size:
         ret_ar = ret_ar[1:]
```

### Comparing `pynbody-2.0.0b7/pynbody/bridge/_bridge.pyx` & `pynbody-2.0.0b8/pynbody/bridge/_bridge.pyx`

 * *Files identical despite different names*

### Comparing `pynbody-2.0.0b7/pynbody/chunk/__init__.py` & `pynbody-2.0.0b8/pynbody/chunk/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,165 +1,85 @@
 """
-
-chunk
-=====
-
 Methods for describing parts of files to load.
 
 This module provides generalized logic for getting parts of sequential data off disk.
 It is for internal use. If you want to write a loader that supports partial loading,
 it will make it a lot easier.
 
 The steps for loading particle data are as follows
 
 1. Set up a description of the particles you have on disk. This is a dictionary
-mapping a family type to a slice, e.g.
+   mapping a family type to a slice, e.g.
 
-  on_disk = {pynbody.family.dm: slice(0,100), pynbody.family.gas: slice(100, 150)}
+   .. code-block:: python
 
-describes a file with 100 dark matter particles followed by 50 gas particles.
+      on_disk = {pynbody.family.dm: slice(0,100), pynbody.family.gas: slice(100, 150)}
 
+   describes a file with 100 dark matter particles followed by 50 gas particles.
 
-2. Create a LoadControl object as defined in this module.
+2. Create a :class:`LoadControl` object.
 
- load_control = pynbody.chunk.LoadControl(on_disk, chunk_size, take)
+   .. code-block:: python
 
-Here,
+      load_control = pynbody.chunk.LoadControl(on_disk, chunk_size, take)
 
- * on_disk is the dictionary you set up in the last step.
+   Here,
 
- * chunk_size is the maximum number of particles you are willing to load off
-  disk at once these will have to be stored in a temporary array, so you don't
-  want it to be too large; but also reading a small number of large chunks is
-  more efficient, so you don't want it to be too small. No careful experimentation
-  has been done with this, but chunk_sizes of around 10000 seem to work OK.
+   * on_disk is the dictionary you set up in the last step.
 
- * take describes what to load in. Currently this is either None (= load the whole file)
-   or a list of ids (= load the specified particles). However this may be expanded
-   in future to a more comprehensive syntax. The idea is your code will not have to
-   change when this happens, and will automatically support more advanced partial loading
-   specifications.
+   * chunk_size is the maximum number of particles you are willing to load off
+     disk at once these will have to be stored in a temporary array, so you don't
+     want it to be too large; but also reading a small number of large chunks is
+     more efficient, so you don't want it to be too small. No careful experimentation
+     has been done with this, but chunk_sizes of around 10000 seem to work OK.
 
-3. Load your particle data. The load_control object has an iterate method. This returns
-step-by-step instructions that take you through the file, specifying what to keep and what
-to throw away in a simple-to-use fashion. See the help for LoadControl.iterate for details
-on how to implement this final step.
+   * take describes what to load in. Currently this is either ``None`` (= load the whole file)
+     or a list of ids (= load the specified particles). However this may be expanded
+     in future to a more comprehensive syntax. The idea is your code will not have to
+     change when this happens, and will automatically support more advanced partial loading
+     specifications.
+
+3. Load your particle data. The :class:`LoadControl` object has an ``iterate`` method. This returns
+   step-by-step instructions that take you through the file, specifying what to keep and what
+   to throw away in a simple-to-use fashion. See the help for :func:`LoadControl.iterate` for details
+   on how to implement this final step.
 
 """
 
+from __future__ import annotations
 
 import copy
-import math
-import random
+from typing import TYPE_CHECKING, Callable, Iterable, Iterator
 
 import numpy as np
 
 from .. import util
 
-
-class Chunk:
-
-    def __init__(self, *args, **kwargs):
-        pass
-        start, stop, step = 0, None, 1
-        if len(args) == 1:
-            start, stop, step = 0, args[0], 1
-        if len(args) == 2:
-            start, stop, step = args[0], args[1], 1
-        if len(args) == 3:
-            start, stop, step = args
-        self.random = kwargs.get('random', None)
-        self.ids = kwargs.get('ids', None)
-
-        self.start = start
-        self.stop = stop
-        self.step = step
-
-        assert (self.step is not None
-                or self.random is not None
-                or self.ids is not None)
-
-    def init(self, max_stop):
-
-        assert max_stop >= 0
-
-        if self.stop is None:
-            self.stop = max_stop
-        else:
-            self.stop = min(max_stop, self.stop)
-
-        assert self.start >= 0
-        assert self.stop >= 0, '%ld' % self.stop
-        assert self.step > 0
-        assert self.start <= self.stop
-
-        if self.random is not None:
-            assert random > 0
-
-        if self.ids is not None:
-            assert np.amax(self.ids) < max_stop
-            if self.random is not None:
-                if self.random < 1:
-                    self.random = int(self.random * len(self.ids))
-                self.ids = random.sample(self.ids, self.random)
-                self.ids.sort()
-            self.len = len(self.ids)
-        else:
-            slice_len = int(math.ceil((self.stop - self.start) / self.step))
-            self.len = slice_len
-            if self.random is not None:
-                if self.random < 1:
-                    self.random = int(self.random * self.len)
-                self.random = min(self.random, slice_len)
-                self.ids = random.sample(
-                    range(self.start, self.stop, self.step), self.random)
-                self.ids.sort()
-                self.len = len(self.ids)
-
-    def __len__(self):
-        return self.len
-
-    def pdeltas(self, step=None):
-
-        assert step is None or self.contiguous()
-        if step is None:
-            step = self.step
-
-        if self.ids is None:
-            for i in range(self.start, self.stop, self.step):
-                yield self.step
-        else:
-            yield self.ids[0]
-            for i in range(len(self.ids) - 1):
-                yield self.ids[i + 1] - self.ids[i]
-
-    def contiguous(self):
-        return self.ids is None and self.step == 1
-
+if TYPE_CHECKING:
+    from .. import family
 
 class LoadControl:
+    """LoadControl provides the logic required for partial loading.
 
-    """LoadControl provides the logic required for partial loading."""
+    See the documentation for :mod:`pynbody.chunk` for more information."""
 
-    def __init__(self, family_slice, max_chunk, clauses):
+    def __init__(self, family_slice: dict[family.Family, slice], max_chunk: int, clauses: np.ndarray | None):
         """Initialize a LoadControl object.
 
         *Inputs:*
 
           *family_slice*: a dictionary of family slices describing the contiguous
             layout of families on disk
 
           *max_chunk*: the guaranteed maximum chunk of data to load in a single
             read operation. Larger values are likely more efficient, but also require
             bigger temporary buffers in your reader code.
 
-          *clauses*: a dictionary describing the type of partial loading to implement.
-            If this dictionary is empty, all data is loaded. Otherwise it can contain
-            'ids', a list of ids to load.
-
+          *clauses*: a description of the type of partial loading to implement. If None, all data is loaded.
+            Otherwise, currently the only supported option is a numpy array of particle ids to load.
          """
 
         self._disk_family_slice = family_slice
         self._generate_family_order()
 
         # generate simulation-level ID list
         if hasattr(clauses, "__len__"):
@@ -214,16 +134,18 @@
         for current_family in self._ordered_families:
 
             start = stop
             stop = stop + len(self._family_ids[current_family])
             self.mem_family_slice[current_family] = slice(start, stop)
 
     def _generate_null_chunks(self, max_chunk):
-        """Generate internal chunk map in the special case that we are loading
-        all data"""
+        """Generate internal chunk map in the special case that we are loading all data.
+
+        See also :func:`_generate_chunks` for the general case.
+        """
 
         self._family_chunks = {}
 
         for current_family in self._ordered_families:
             self._family_chunks[current_family] = []
             disk_sl = self._disk_family_slice[current_family]
             for i0 in range(0, disk_sl.stop - disk_sl.start, max_chunk):
@@ -231,16 +153,21 @@
                 buf_sl = slice(0, nread)
                 mem_sl = slice(i0, i0 + nread)
 
                 self._family_chunks[current_family].append(
                     (nread, buf_sl, mem_sl))
 
     def _generate_chunks(self, max_chunk):
-        """Generate internal chunk map, with maximum load chunk of specified number
-        of entries, and with chunks that do not cross family boundaries."""
+        """Generate internal chunk map
+
+        This must satisfy the requirements that:
+          * maximum chunk size does not exceed *max_chunk*
+          * chunks do not cross family boundaries
+
+        """
 
         if self._ids is None:
             self._generate_null_chunks(max_chunk)
             return
 
         self._family_chunks = {}
 
@@ -272,31 +199,37 @@
                 mem_ptr = mem_ptr + j - i
                 i = j
                 disk_ptr = disk_ptr_end
 
                 self._family_chunks[current_family].append(
                     (nread_disk, disk_mask, mem_slice))
 
-    def iterate_with_interrupts(self, families_on_disk, families_in_memory,
-                                disk_interrupt_points, disk_interrupt_fn, multiskip=False):
-        """Performs the same function as
-        :func:`~pynbody.chunk.LoadControl.iterate` but additionally
-        takes a list of exact file offsets *disk_interrupt_points* at
-        which to interrupt the loading process and call a
-        user-specified function *disk_interrupt_fn*.
-
-        **Input:** :
-          *disk_interrupt_points*: a list (or other iterable) of disk offsets
-            (must be in ascending order) at which to call the interrupt function
-          *disk_interrupt_fn*: a function which takes the file offset as an argument,
-            and is called precisely at the point that the disk interrupt point is reached
+    def iterate_with_interrupts(self, families_on_disk: list[family.Family], families_in_memory: list[family.Family],
+                                disk_interrupt_points: Iterable[int], disk_interrupt_fn: Callable,
+                                multiskip: bool = False):
+        """Yields instructions for loading an array with the specified families, breaking at specified file offsets
+
+        Performs the same function as :func:`iterate` but additionally takes a list of exact file offsets
+        *disk_interrupt_points* at which to interrupt the loading process and call a user-specified function
+        *disk_interrupt_fn*.
 
-          See func:`~pynbody.chunk.LoadControl.iterate` for other arguments.
+        Parameters
+        ----------
 
-          """
+        disk_interrupt_points: Iterable
+            List (or other iterable) of disk offsets at which to call the interrupt function, in ascending order
+
+        disk_interrupt_fn: Callable
+            Function which takes the file offset as an argument, and is called precisely at the point that the disk
+            interrupt point is reached
+
+
+        See :func:`iterate` for other parameters.
+
+        """
 
         fpos = 0
         i = 0
         next_dip = disk_interrupt_points[i]
         for nread_disk, disk_slice, mem_slice in self.iterate(families_on_disk, families_in_memory, multiskip):
             while next_dip and fpos + nread_disk > next_dip:
                 # an interrupt falls in the middle of our slice
@@ -361,38 +294,50 @@
                 # decomposition)
                 nread_disk, disk_slice, mem_slice = len_post, d_slice_post, m_slice_post
 
 
             yield nread_disk, disk_slice, mem_slice
             fpos += nread_disk
 
-    def iterate(self, families_on_disk, families_in_memory, multiskip=False):
-        """Provide an iterator which yields step-by-step instructions
-        for partial-loading an array with the specified families stored
-        on disk into a memory array containing the specified families.
+    def iterate(self, families_on_disk: list[family.Family], families_in_memory: list[family.Family],
+                multiskip: bool = False) -> Iterator[tuple[int, slice | None, slice | None]]:
+        """Yields step-by-step instructions for partial-loading an array with the specified families.
 
-        Each output consists of *readlen*, *file_index*, *memory_index*.
         A typical read loop should be as follows:
 
-        for readlen, buffer_index, memory_index in ctl.iterate(fams_on_disk, fams_in_mem) :
-          data = read_entries(count=readlen)
-          if memory_index is not None :
-            target_array[memory_index] = data[buffer_index]
+        .. code-block:: python
+
+            for readlen, buffer_index, memory_index in ctl.iterate(fams_on_disk, fams_in_mem) :
+              data = read_entries(count=readlen)
+              if memory_index is not None :
+                target_array[memory_index] = data[buffer_index]
 
         Obviously this can be optimized, for instance to skip through
         file data when memory_index is None rather than read and discard it.
 
-        **Input:** :
-
-          *families_on_disk*: list of families for which the array exists on disk
-          *families_in_memory*: list of families to target in memory
-          *multiskip*: if True, skip commands (i.e. entries with file_index=None)
-             can have readlen greater than the block length
+        Parameters
+        ----------
+        families_on_disk : list
+            List of families for which the array exists on disk
+        families_in_memory : list
+            List of families for which we want to read the array into memory
+        multiskip : bool
+            If True, skip commands (i.e. entries with buffer_index=None)
+            can have readlen greater than the block length
+
+        Yields
+        ------
+        readlen : int
+            Number of entries to read from disk
+        buffer_index : slice | None
+            Slice to read from the resulting buffer, or None if this particular read is to be ignored (skipped)
+        memory_index : slice | None
+            Slice to write into memory, or None if ``buffer_index`` is None
 
-          """
+        """
 
         mem_offset = 0
 
         skip_accumulation = 0
 
         for current_family in self._ordered_families:
             if skip_accumulation > 0:
```

### Comparing `pynbody-2.0.0b7/pynbody/configuration.py` & `pynbody-2.0.0b8/pynbody/configuration.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,7 +1,13 @@
+"""Read and expose configuration information for pynbody
+
+The configuration system in pynbody is described in the :ref:`configuration` tutorial.
+
+"""
+
 import logging
 import multiprocessing
 import os
 import warnings
 
 
 def _get_config_parser_with_defaults():
@@ -35,16 +41,15 @@
     config_parser.read(os.path.join(os.path.dirname(__file__), "config.ini"))
     config_parser.read(os.path.expanduser("~/.pynbodyrc"))
     config_parser.read("config.ini")
     _merge_defaults_for_problematic_keys(config_parser)
 
 def _get_basic_config_from_parser(config_parser):
 
-    config = {'verbose': config_parser.getboolean('general', 'verbose'),
-              'centering-scheme': config_parser.get('general', 'centering-scheme')}
+    config = {'centering-scheme': config_parser.get('general', 'centering-scheme')}
 
     config['snap-class-priority'] = list(map(str.strip,
                                         config_parser.get('general', 'snap-class-priority').split(",")))
     config['halo-class-priority'] = list(map(str.strip,
                                         config_parser.get('general', 'halo-class-priority').split(",")))
 
 
@@ -68,31 +73,40 @@
     if config['number_of_threads']<0:
         config['number_of_threads']=multiprocessing.cpu_count()
 
     config['gravity_calculation_mode'] = config_parser.get(
         'general', 'gravity_calculation_mode')
     config['disk-fit-function'] = config_parser.get('general', 'disk-fit-function')
 
+    config['image-default-resolution'] = int(config_parser.get('general', 'image-default-resolution'))
+
     return config
 
 def _setup_logger(config):
     logger = logging.getLogger('pynbody')
     logger.setLevel(logging.DEBUG)
     formatter = logging.Formatter('%(name)s : %(message)s')
     for existing_handler in list(logger.handlers):
         logger.removeHandler(existing_handler)
 
     ch = logging.StreamHandler()
     ch.setFormatter(formatter)
     logger.addHandler(ch)
 
-    if config['verbose']:
-        logger.setLevel(logging.INFO)
+    if config_parser.getboolean('general','verbose'):
+        set_logging_level(logging.INFO)
         logger.info("Verbose mode is on")
     else:
-        logger.setLevel(logging.WARNING)
+        set_logging_level(logging.WARNING)
+
+def set_logging_level(level = logging.INFO):
+    """Set the logging level for pynbody, in terms of the standard Python logging module levels.
+
+    Set to logging.INFO for more verbose output, or logging.WARNING for less."""
+    logger = logging.getLogger('pynbody')
+    logger.setLevel(level)
 
 
 config_parser = _get_config_parser_with_defaults()
 _add_overrides_to_config_parser(config_parser)
 config = _get_basic_config_from_parser(config_parser)
 logger = _setup_logger(config)
```

### Comparing `pynbody-2.0.0b7/pynbody/default_config.ini` & `pynbody-2.0.0b8/pynbody/default_config.ini`

 * *Files 22% similar despite different names*

```diff
@@ -2,81 +2,106 @@
 #
 # If you want to override options, either create a local copy called
 # config.ini in the directory where pynbody is installed, create a local
 # copy called .pynbodyrc in your home directory, or a local copy called
 # config.ini in the directory where you are running pynbody.
 
 [general]
-verbose: False
-snap-class-priority: RamsesSnap, GrafICSnap, NchiladaSnap, GadgetSnap, SwiftSnap, EagleLikeHDFSnap, GadgetHDFSnap, SubFindHDFSnap, TipsySnap, AsciiSnap
-halo-class-priority: HaloNumberCatalogue, AmigaGrpCatalogue, VelociraptorCatalogue, SubFindHDFHaloCatalogue, RockstarCatalogue, AHFCatalogue, SubfindCatalogue, NewAdaptaHOPCatalogue, AdaptaHOPCatalogue, HOPCatalogue, Gadget4SubfindHDFCatalogue, ArepoSubfindHDFCatalogue, TNGSubfindHDFCatalogue
+# When you call pynbody.load, it will by default try interpreting them as formats in
+# the following order. You can override this ordering either as a configuration option, or
+# by passing load(..., priority = [...]) at runtime (see documentation for pynbody.snapshot.load).
+snap-class-priority: RamsesSnap, GrafICSnap, NchiladaSnap, GadgetSnap, SwiftSnap, EagleLikeHDFSnap, GadgetHDFSnap,
+    SubFindHDFSnap, TipsySnap, AsciiSnap
+
+# Similarly, when you call .halos() on a SimSnap, different readers are tried in succession,
+# and the first that is able to produce a halo catalogue is used. The order can be changed
+# here or by passing sim.halos(priority=[...]) at runtime (see documentation for SimSnap.halos).
+halo-class-priority: HaloNumberCatalogue, AmigaGrpCatalogue, VelociraptorCatalogue, SubFindHDFHaloCatalogue,
+    RockstarCatalogue, AHFCatalogue, SubfindCatalogue, NewAdaptaHOPCatalogue, AdaptaHOPCatalogue, HOPCatalogue,
+    Gadget4SubfindHDFCatalogue, ArepoSubfindHDFCatalogue, TNGSubfindHDFCatalogue
 
 centering-scheme: ssc
 
+# Some routines log information which will appear if verbose is set to True
+verbose: False
+
 threading: True
 number_of_threads: -1
 # -1 above indicates to detect the number of processors
 
 gravity_calculation_mode: direct
 
 disk-fit-function: expsech
 
 # number of points to use in cosmological function interpolations e.g. t->a transformations
 cosmo-interpolation-points: 1000
 
-# The following section defines the families in the format
+# The default resolution for images. This is the number of pixels along the longest axis.
+image-default-resolution: 1000
+
+[families]
+# This section defines the families in the format
 #    main_name: alias1, alias2, ...
 #
 # To add your own families, just add lines like this to
 # your own local copy.
 #
 # Note that the alias list can be blank, i.e. if you want
 # no aliases for particle family 'main_name', write:
 #   main_name:
 #
 
-[families]
 dm: d, dark
 star: stars, st, s
 gas: g
 neutrino: n, neu
 bh:
 debris:
 gas_tracer:
 dm_tracer:
 star_tracer:
 cloud_tracer:
 debris_tracer:
 cloud:
 
 [sph]
+# The number of particles to include in the SPH kernel:
 smooth-particles: 32
+
+# When building a KDTree, how many particles are in each leaf of the tree. This should have no
+# effect on results, just a minor impact on performance. Roughly half the number of smoothing
+# particles is probably optimal.
 tree-leafsize: 16
-Kernel: CubicSpline
 
-# Note that all smooths are now threaded according to number_of_threads
-# in [general] above. The algorithm is now exact.
+#
+Kernel: CubicSpline
 
 # This switches on threading for rendering images. There is unlikely to be
 # any reason you'd want to turn this off except for testing.
 threaded-image: True
 
 # This switches on an approximate rendering algorithm that
 # slightly degrades quality but radically speeds things up (especially
 # for projected images).
 approximate-fast-images: True
 
 
 [gadgethdf-type-mapping]
+# GadgetHDF stores six different particle types (numbered 0 to 5). This specifies how they map
+# onto pynbody particle types by default. To override, you can either make your own configuration
+# file (see above), or use special arguments when loading the HDF file (see reference documentation
+# for GadgetHDFSnap). Note that this mapping is also used for e.g. Arepo and Swift simulations which
+# follow a very similar format.
 gas: PartType0
 dm: PartType1, PartType2, PartType3
 star: PartType4
 bh: PartType5
 
 [gadgethdf-name-mapping]
+# Specifies how names in the HDF file map to pynbody names
 Coordinates: pos
 Velocity: vel
 Velocities: vel
 ParticleIDs: iord
 Masses: mass
 Mass: mass
 InternalEnergy: u
@@ -110,25 +135,31 @@
 Densities: rho
 InternalEnergies: u
 Pressures: p
 SmoothingLengths: smooth
 
 
 [default-cosmology]
-# from Planck+WP+highL+BAO, 1303.5076 Table 5
+# These parameters are assumed by default if a file doesn't provide the cosmological information.
+# From Planck 2018, https://arxiv.org/pdf/1807.06209, Table 2, last column; includes
+# BAO and CMB data.
 a: 1.0
-h: 0.6777
-ns: 0.96
+h: 0.6766
+ns: 0.9665
 running: 0.0
-omegaL0: 0.691
-omegaM0: 0.309
-omegaB0: 0.0482
-sigma8: 0.8288
+omegaM0: 0.3111
+omegaL0: 0.6889
+omegaB0: 0.0490
+# The above from omegaB0h^2 / h^2
+sigma8: 0.8102
 
 [default-array-dimensions]
+# If the unit system of a file is known, pynbody can use the following dimensional information
+# to infer the likely units. If specific unit information is available about a given array,
+# that will override any dimensions given here.
 pos: cm
 vel: cm s^-1
 eps: cm
 phi: cm^2 s^-2
 accg: cm s^-2
 mass: kg
 temp: K
@@ -147,33 +178,39 @@
 coolontime: s
 p: Pa
 u: km^2 s^-2
 uHot: km^2 s^-2
 massform: kg
 massHot: kg
 MassHot: kg
+
 # ramses RT stores radiation density in flux units:
 rad_0_rho: cm^-2 s^-1
 rad_0_flux: cm^-2 s^-1
 
 [tipsy]
+# In the tipsy binary format, arrays are stored on disk without explicit information about their
+# type. This specifies which binary files to be interpreted as integers as opposed to floating
+# point.
 binary-int-arrays: iord, igasorder, grp
 
 [gadget-type-mapping]
+# For non-HDF (i.e. old-style) gadget files, specifies the mapping from the gadget particle
+# type (0->5) to pynbody families
 gas: 0
 dm: 1,5
 star: 2,3,4
 
 [gadget-name-mapping]
+# Maps non-HDF (i.e. old-style) gadget block names to pynbody families
 HSML: smooth
 ID: iord
 
 [gadget-1-blocks]
-# The default block order for Gadget-1 files.
-# Not all blocks need be present
+# The default block order for Gadget-1 files. Not all blocks need be present
 blocks=HEAD,POS,VEL,ID,MASS,U,NH,NHE,HSML,SFR
 
 [nchilada-name-mapping]
 # this maps the nchilada XML names (not filenames) to pynbody names
 position: pos
 potential: phi
 smoothlength: smooth2
@@ -213,50 +250,65 @@
 # the last family in the list is also assigned to all other negative families
 type-mapping-negative: gas_tracer, dm_tracer, star_tracer, cloud_tracer, debris_tracer
 
 # family for the additional sink.csv file
 type-sink: bh
 
 # For the use of proper (if True) or conformal (if False) time when reading the age of star particles.
-# Should be turned to true the namelist flag use_proper_time is set to true
-# or for radiative transfer simulations.
-# By default, this will be guessed from the dataset.
+# Should be turned to True if the namelist flag use_proper_time is set to True
+# or for radiative transfer simulations. By default, this will be guessed from the dataset, so is not set here.
+
 # proper_time: False
 
-# The default particle blocks for RAMSES files
+# The default particle blocks for RAMSES files. Only used if the particle block names and type information are
+# not given in the header_....txt file inside the output_.... folder.
 particle-blocks=x,y,z,vx,vy,vz,mass,iord,level,tform,metal
 particle-format=f8,f8,f8,f8,f8,f8,f8,i4,i4,f8,f8
 
-# For RAMSES format up to November 2017:
+# For old-style RAMSES format (up to November 2017)
 # particle-distinguisher indicates the particle block which is non-zero for stars (0-based, so 9=age by default)
+# More recent RAMSES outputs have a specific field that explicitly distinguishes different particle types
+# so this is not used
 particle-distinguisher=9,f8
 
-# hydro-blocks in 3D. Anything ending in z will be removed for 2D snapshots.
+# Hydro blocks for old-style files; only used if the file_descriptor.txt file doesn't specify the
+# hydro blocks actually present in the file. The list here assumes 3D. Anything ending in z will
+# be removed for 2D snapshots.
 hydro-blocks=rho,vx,vy,vz,p,metal
 gravity-blocks=phi,accg_x,accg_y,accg_z
-# rt blocks where %d represents the waveband number
+
+# RT blocks where %d represents the waveband number. Even modern ramses files don't write out any
+# names for the RT blocks, although they do store the number of wavebands, so pynbody can generate
+# the right number of arrays
 rt-blocks=rad_%d_rho,rad_%d_flux_x,rad_%d_flux_y,rad_%d_flux_z
 
-# The following flag lets RamsesSnaps be read by multiple threads.
-# If parallel_read>=2, that is the number of workers used to read
-# a file. If parallel_read<=1, single threading is used.
+# Ramses files are read in parallel by the specified number of reader processes. Note that
+# the optimal number of readers probably depends on your disk performance rather than the number
+# of CPUs.
+#
+# If parallel_read<=1, ramses files are read on the main process.
 #
 parallel-read=8
 
 # specify the locations of RAMSES utilities -- obtain from
 # https://bitbucket.org/rteyssie/ramses
+# These utils were previously used to convert conformal times of star birth times into physical
+# times; however, now, that can be done internally and this is largely retained for historical
+# reasons.
 ramses_utils = $HOME/ramses/utils/
 
-# If true, use part2birth to convert from conformal to physical time
+# If True, use external part2birth utility (see above) to convert from conformal to physical time
+# Otherwise, use pynbody's internal routines. This is retained for historical reproducibility
+# but there is no reason to use it for new projects.
 use_part2birth_by_default = False
 
 [gadget-default-output]
-# Gadget files have no intrinsic set of fields, so this defines a
-# default set and an ordering too (in terms of the pynbody names,
-# not the gadget block names)
+# Very old gadget files have no block names to identify the fields that have been written to
+# disk.  This determines which blocks to expect in such a file, the families for which they
+# are defined, and the order in which they appear in the file.
 all = pos, vel
 gas = u, nh, nhe, smooth, sfr
 # Any arrays not mentioned in the field ordering below will be
 # tacked on the end of the file in an unspecified order
 field-ordering = pos, vel, iord, mass, u, nh, nhe, smooth, sfr
 
 [gadget-units]
@@ -266,173 +318,100 @@
 #
 # Cosmological dependencies (a and h) will be stripped out for non-
 # cosmological runs.
 vel: km s^-1 a^1/2
 pos: Mpc a h^-1
 mass: 1e10 Msol h^-1
 
-[tipsy-default-output]
-# Tipsy files come with a default set of fields which will be written
-# so this just specifies any extra arrays to be written out
+[camb]
+# To use CAMB live (e.g. to generate consistent power spectra automatically) you will need
+# to compile the default version of CAMB (ini-file driver) and set up the path to the
+# executable. Download CAMB here: http://camb.info
+path: /path/to/camb
+
+[SubfindHDF]
+
+FoF-ignore: SF, NSF, Stars
+Sub-ignore: GrNr, FirstSubOfHalo, SubParentHalo, SubMostBoundID, InertiaTensor, SF, NSF, NsubPerHalo, Stars
+
+
 
 [irreducible-units]
 # This defines the irreducible units, which cannot be expressed in
 # terms of anything more basic. We include in this cosmological
 # quantities 'a' and 'h' which are typically substituted for numerical
 # values at some point in the calculation.
 names: m, s, kg, K, a, h, aform, rad
 
 [named-units]
 # The next section defines the named units which are derived from the
 # above irreducible units. The file is processed sequentially so that
 # later entries can refer to previous named units.
 
-# Times
-yr: 3.1556926e7 s
+# Times - regard a year as the julian year 365.25 days, and a day as 86400 seconds, as per
+# https://www.iau.org/publications/proceedings_rules/
+yr: 31.5576e6 s
 kyr: 1000 yr
 Myr: 1000 kyr
 Gyr: 1000 Myr
 Hz: s^-1
 kHz: 1e3 Hz
 MHz: 1e6 Hz
 GHz: 1e9 Hz
 THz: 1e12 Hz
 
-# Distances
+# Distances; see
 angst: 1e-10 m
 cm: 0.01 m
 mm: 1e-3 m
 nm: 1e-9 m
 km: 1000 m
-au: 1.49598e11 m
-pc: 3.08568025e16 m
+au: 1.495978707e11 m
+pc: 3.0856775814913673e16 m
 kpc: 1000 pc
 Mpc: 1000 kpc
 Gpc: 1000 Mpc
 
 # Solid Angle
 sr: rad^2
 deg: 0.01745329251 rad
 arcmin: 0.01666666666 deg
 arcsec: 0.01666666666 arcmin
 
 # Masses
-Msol: 1.98892e30 kg
-# NB the above value is considerably out of date, and kept for now for backwards compatibility
-# a better value is 1.98842e30 kg (see https://iau-a3.gitlab.io/NSFA/NSFA_cbe.html#GMS2012)
-
+# see https://iau-a3.gitlab.io/NSFA/NSFA_cbe.html#GMS2012
+Msol: 1.98842e30 kg
 g: 1.0e-3 kg
-m_p: 1.67262158e-27 kg
-m_e: 9.10938188e-31 kg
+
+# proton/electron masses updated from https://physics.nist.gov/ in April 2024
+m_p: 1.67262192369e-27 kg
+m_e: 9.1093837015e-31 kg
 
 # Forces
 N: kg m s^-2
 dyn: g cm s^-2
 
 # Energies
 J: N m
 erg: 1.0e-7 J
-eV: 1.60217646e-19 J
+eV: 1.602176634e-19 J
 keV: 1000 eV
 MeV: 1000 keV
 
 # Pressures
 Pa: J m^-3
 
 # Redshift
 (1+z): a^-1
 
 # Helpful physical quantities
-k: 1.3806503e-23 J K^-1
+# updated from https://physics.nist.gov/ in April 2024
+k: 1.380649e-23 J K^-1
 c: 299792458 m s^-1
-G: 6.67300e-11 m^3 kg^-1 s^-2
-hP: 6.626068e-34 m^2 kg s^-1
+G: 6.67430e-11 m^3 kg^-1 s^-2
+hP: 6.62607015e-34 m^2 kg s^-1
 
 [units-latex]
 # Latex code for typesetting named units.
 Msol: M_{\odot}
 m_p: m_p
 m_e: m_e
-
-[AHFCatalogue]
-# settings for the AHF Catalogue reader
-
-AutoRun: False
-# automatically attempt to run AHF if no catalogue can be found
-# on disk
-
-Path: None
-# /path/to/AHF, or None to attempt to find it in your $PATH
-
-
-
-Config:	  [AHF]
-	  ic_filename = %(filename)s
-	  ic_filetype = %(typecode)d
-	  outfile_prefix = %(filename)s
-	  LgridDomain = 256
-	  LgridMax = %(gridmax)d
-	  NperDomCell = 5
-	  NperRefCell = 5
-	  VescTune = 1.5
-	  NminPerHalo = 50
-	  RhoVir = 0
-	  Dvir = 200
-	  MaxGatherRad = 10.0
-
-ConfigTipsy:	  [TIPSY]
-	  TIPSY_OMEGA0 = %(omega0)f
-	  TIPSY_LAMBDA0 = %(lambda0)f
-	  TIPSY_BOXSIZE = %(boxsize)e
-	  TIPSY_VUNIT = %(vunit)e
-	  TIPSY_MUNIT = %(munit)e
-	  TIPSY_EUNIT = %(eunit)e
-
-[RockstarCatalogue]
-# settings for the Rockstar Catalogue reader
-
-AutoRun: True
-# automatically attempt to run AHF if no catalogue can be found
-# on disk
-
-Path: None
-# /path/to/rockstar, or None to attempt to find it in your $PATH
-
-AutoGrp: False
-# set to true to automatically create a 'grp' array on load
-# The grp array
-
-AutoPid: False
-# set to true to automatically create a 'pid' array on load
-# the PID array is another way to get the particle IDs in the ancestor snapshot,
-# but the framework provides h[n].get_index_list(f) for halo catalogue h and
-# base snapshot f, so you probably don't need AutoPid
-
-
-Config:	  FILE_FORMAT = %(format)s
-	  PARTICLE_MASS = %(partmass)d
-	  SCALE_NOW = %(expfac)f
-	  h0 = %(hub)f
-	  Om = %(omega0)f
-	  Ol = %(lambda0)f
-	  TIPSY_LENGTH_CONVERSION = %(boxsize)e
-	  TIPSY_VELOCITY_CONVERSION = %(vunit)e
-	  TIPSY_MASS_CONVERSION = %(munit)e
-	  FORCE_RES = %(softening)e
-	  OUTPUT_FORMAT = BINARY
-
-[camb]
-# To use CAMB live (e.g. to generate consistent power spectra automatically) you will need
-# to compile the default version of CAMB (ini-file driver) and set up the path to the
-# executable. Download CAMB here: http://camb.info
-path: /path/to/camb
-
-[SubfindHDF]
-
-FoF-ignore: SF, NSF, Stars
-Sub-ignore: GrNr, FirstSubOfHalo, SubParentHalo, SubMostBoundID, InertiaTensor, SF, NSF, NsubPerHalo, Stars
-
-[shared-array]
-
-# delay in seconds between detecting a buffer is no longer needed and releasing the underlying memory
-# This delay is necessitated by implementation details (see pynbody.array.shared)
-cleanup-delay: 1e-2
```

### Comparing `pynbody-2.0.0b7/pynbody/derived.py` & `pynbody-2.0.0b8/pynbody/derived.py`

 * *Files 10% similar despite different names*

```diff
@@ -17,97 +17,97 @@
 from . import analysis, array, config, units
 from .dependencytracker import DependencyError
 from .snapshot import SimSnap
 
 logger = logging.getLogger('pynbody.derived')
 
 
-@SimSnap.derived_quantity
+@SimSnap.derived_array
 def r(self):
     """Radial position"""
     return ((self['pos'] ** 2).sum(axis=1)) ** (1, 2)
 
 
-@SimSnap.derived_quantity
+@SimSnap.derived_array
 def rxy(self):
     """Cylindrical radius in the x-y plane"""
     return ((self['pos'][:, 0:2] ** 2).sum(axis=1)) ** (1, 2)
 
 
-@SimSnap.derived_quantity
+@SimSnap.derived_array
 def vr(self):
     """Radial velocity"""
     return (self['pos'] * self['vel']).sum(axis=1) / self['r']
 
 
-@SimSnap.derived_quantity
+@SimSnap.derived_array
 def v2(self):
     """Squared velocity"""
     return (self['vel'] ** 2).sum(axis=1)
 
 
-@SimSnap.derived_quantity
+@SimSnap.derived_array
 def vt(self):
     """Tangential velocity"""
     return np.sqrt(self['v2'] - self['vr'] ** 2)
 
 
-@SimSnap.derived_quantity
+@SimSnap.derived_array
 def ke(self):
     """Specific kinetic energy"""
     return 0.5 * (self['vel'] ** 2).sum(axis=1)
 
 
-@SimSnap.derived_quantity
+@SimSnap.derived_array
 def te(self):
     """Specific total energy"""
     return self['ke'] + self['phi']
 
 
-@SimSnap.derived_quantity
+@SimSnap.derived_array
 def j(self):
     """Specific angular momentum"""
     angmom = np.cross(self['pos'], self['vel']).view(array.SimArray)
     angmom.units = self['pos'].units * self['vel'].units
     return angmom
 
 
-@SimSnap.derived_quantity
+@SimSnap.derived_array
 def j2(self):
     """Square of the specific angular momentum"""
     return (self['j'] ** 2).sum(axis=1)
 
 
-@SimSnap.derived_quantity
+@SimSnap.derived_array
 def jz(self):
     """z-component of the angular momentum"""
     return self['j'][:, 2]
 
 
-@SimSnap.derived_quantity
+@SimSnap.derived_array
 def vrxy(self):
     """Cylindrical radial velocity in the x-y plane"""
     return (self['pos'][:, 0:2] * self['vel'][:, 0:2]).sum(axis=1) / self['rxy']
 
 
-@SimSnap.derived_quantity
+@SimSnap.derived_array
 def vcxy(self):
     """Cylindrical tangential velocity in the x-y plane"""
     f = (self['x'] * self['vy'] - self['y'] * self['vx']) / self['rxy']
     f[np.where(f != f)] = 0
     return f
 
 
-@SimSnap.derived_quantity
+@SimSnap.derived_array
 def vphi(self):
     """Azimuthal velocity (synonym for vcxy)"""
     return self['vcxy']
 
 
-@SimSnap.derived_quantity
+@SimSnap.derived_array
 def vtheta(self):
     """Velocity projected to polar direction"""
     return (np.cos(self['az']) * np.cos(self['theta']) * self['vx'] +
             np.sin(self['az']) * np.cos(self['theta']) * self['vy'] -
             np.sin(self['theta']) * self['vz'])
 
 
@@ -147,40 +147,40 @@
     end = time.time()
 
     logger.info(f'{_op_dict[op]} done in {end - start:5.3g} s')
 
     return sm
 
 
-@SimSnap.derived_quantity
+@SimSnap.derived_array
 def v_mean(self):
     """SPH-smoothed mean velocity"""
     return _v_sph_operation(self, "mean")
 
-@SimSnap.derived_quantity
+@SimSnap.derived_array
 def v_disp(self):
     """SPH-smoothed velocity dispersion"""
     return _v_sph_operation(self, "disp")
 
-@SimSnap.derived_quantity
+@SimSnap.derived_array
 def v_curl(self):
     """SPH-smoothed curl of velocity"""
     return _v_sph_operation(self, "curl")
 
-@SimSnap.derived_quantity
+@SimSnap.derived_array
 def vorticity(self):
     """SPH-smoothed vorticity"""
     return _v_sph_operation(self, "curl")
 
-@SimSnap.derived_quantity
+@SimSnap.derived_array
 def v_div(self):
     """SPH-smoothed divergence of velocity"""
     return _v_sph_operation(self, "div")
 
-@SimSnap.derived_quantity
+@SimSnap.derived_array
 def age(self):
     """Stellar age determined from formation time and current snapshot time"""
     return self.properties['time'].in_units(self['tform'].units, **self.conversion_context()) - self['tform']
 
 bands_available = ['u', 'b', 'v', 'r', 'i', 'j', 'h', 'k', 'U', 'B', 'V', 'R', 'I',
                    'J', 'H', 'K']
 
@@ -189,51 +189,51 @@
         val.units = s['rho'].units/s['mass'].units
         return val
 
 for band in bands_available:
     X = lambda s, b=str(band): analysis.luminosity.calc_mags(s, band=b)
     X.__name__ = band + "_mag"
     X.__doc__ = band + " magnitude from analysis.luminosity.calc_mags"""
-    SimSnap.derived_quantity(X)
+    SimSnap.derived_array(X)
 
     lum_den = functools.partial(lum_den_template,band)
 
     lum_den.__name__ = band + "_lum_den"
     lum_den.__doc__ = "Luminosity density in astronomy-friendly units: 10^(-0.4 %s_mag) per unit volume. " \
                       "" \
                       "The magnitude is taken from analysis.luminosity.calc_mags."%band
-    SimSnap.derived_quantity(lum_den)
+    SimSnap.derived_array(lum_den)
 
 
-@SimSnap.derived_quantity
+@SimSnap.derived_array
 def theta(self):
     """Angle from the z axis, from [0:pi]"""
     return np.arccos(self['z'] / self['r'])
 
 
-@SimSnap.derived_quantity
+@SimSnap.derived_array
 def alt(self):
     """Angle from the horizon, from [-pi/2:pi/2]"""
     return np.pi / 2 - self['theta']
 
 
-@SimSnap.derived_quantity
+@SimSnap.derived_array
 def az(self):
     """Angle in the xy plane from the x axis, from [-pi:pi]"""
     return np.arctan2(self['y'], self['x'])
 
 
-@SimSnap.derived_quantity
+@SimSnap.derived_array
 def cs(self):
     """Sound speed"""
     return np.sqrt(5.0 / 3.0 * units.k * self['temp'] / self['mu'] / units.m_p)
 
 
 
-@SimSnap.derived_quantity
+@SimSnap.derived_array
 def mu(sim, t0=None, Y=0.245):
     """Mean molecular mass, i.e. the mean atomic mass per particle. Assumes primordial abundances."""
     try:
         x = _mu_from_electron_frac(sim, Y)
     except (KeyError, DependencyError):
         try:
             x = _mu_from_HI_HeI_HeII_HeIII(sim)
@@ -262,43 +262,43 @@
     return x
 
 def _mu_from_electron_frac(sim, Y):
     return 4./(4.-3.*Y+4*(1.-Y)*sim['ElectronAbundance'])
 
 
 
-@SimSnap.derived_quantity
+@SimSnap.derived_array
 def p(sim):
     """Pressure"""
     p = sim["u"] * sim["rho"] * (2. / 3)
     p.convert_units("Pa")
     return p
 
 
-@SimSnap.derived_quantity
+@SimSnap.derived_array
 def u(self):
     """Gas internal energy derived from temperature"""
     gamma = 5. / 3
     return self['temp'] * units.k / (self['mu'] * units.m_p * (gamma - 1))
 
 
-@SimSnap.derived_quantity
+@SimSnap.derived_array
 def temp(self):
     """Gas temperature derived from internal energy"""
     gamma = 5. / 3
     mu_est = np.ones(len(self))
     for i in range(5):
         temp = (self['u'] * units.m_p / units.k) * (mu_est * (gamma - 1))
         temp.sim = self # to allow use of conversion context, e.g. scalefactor
         temp.convert_units("K")
         mu_est = mu(self, temp)
     return temp
 
 
-@SimSnap.derived_quantity
+@SimSnap.derived_array
 def zeldovich_offset(self):
     """The position offset in the current snapshot according to
     the Zel'dovich approximation applied to the current velocities.
     (Only useful in the generation or analysis of initial conditions.)"""
     from . import analysis
     bdot_by_b = analysis.cosmology.rate_linear_growth(
         self, unit='km Mpc^-1 s^-1') / analysis.cosmology.linear_growth_factor(self)
@@ -306,27 +306,27 @@
     a = self.properties['a']
 
     offset = self['vel'] / (a * bdot_by_b)
     offset.units = self['vel'].units / units.Unit('km Mpc^-1 s^-1 a^-1')
     return offset
 
 
-@SimSnap.derived_quantity
+@SimSnap.derived_array
 def aform(self):
     """The expansion factor at the time specified by the tform array."""
 
     from . import analysis
     z = analysis.cosmology.redshift(self, self['tform'])
     a = 1. / (1. + z)
     return a
 
-@SimSnap.derived_quantity
+@SimSnap.derived_array
 def tform(self):
     """The time of the specified expansion factor in the aform"""
     from . import analysis
     t = analysis.cosmology.age(self, 1./self['aform'] - 1.)
     return t
 
-@SimSnap.derived_quantity
+@SimSnap.derived_array
 def iord_argsort(self):
     """Indices so that particles are ordered by increasing ids"""
     return np.argsort(self['iord'])
```

### Comparing `pynbody-2.0.0b7/pynbody/extern/_cython_fortran_utils.pyx` & `pynbody-2.0.0b8/pynbody/extern/_cython_fortran_utils.pyx`

 * *Files identical despite different names*

### Comparing `pynbody-2.0.0b7/pynbody/filt/__init__.py` & `pynbody-2.0.0b8/pynbody/filt/__init__.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,40 +1,47 @@
 """
+Filters are used to define subsets of simulations, especially (but not exclusively) spatial sub-regions.
 
-filt
-====
+The basic idea is that a :class:`Filter` object stores the abstract definition of the subset, and then it can be
+called with a simulation to return a boolean array indicating which particles are in the subset. The implementation
+of filters is designed to be as efficient as possible, and in many cases the selection is done in C with OpenMP
+parallelisation. Additionally, if a simulation has a :class:`pynbody.kdtree.KDTree` built (via
+:meth:`pynbody.snapshot.simsnap.SimSnap.build_tree`), then the selection can be done using the KDTree, which is considerably
+faster for very large simulations.
 
-Defines and implements 'filters' which allow abstract subsets
-of data to be specified.
-
-See the `filter tutorial
-<http://pynbody.github.io/pynbody/tutorials/filters.html>`_ for some
-sample usage.
+Filters can be combined using the logical operators `&`, `|` and `~` to create more complex selections.
 
+For a friendly introduction, see :doc:`/tutorials/filters`.
 """
-
+from __future__ import annotations
 
 import pickle
+from typing import TYPE_CHECKING
 
 import numpy as np
+from numpy.typing import ArrayLike
 
 from .. import family, units
 from . import geometry_selection
 
+if TYPE_CHECKING:
+    from .. import snapshot
 
 class Filter:
+    """Base class for all filters. Filters are callables that take simulations as input and return a boolean mask"""
 
-    def __init__(self):
-        self._descriptor = "filter"
-        pass
+    def where(self, sim: snapshot.SimSnap):
+        """Return the indices of particles that are in the filter.
 
-    def where(self, sim):
+        This is a convenience method that is equivalent to np.where(f(sim)) but may be more efficient for some filters.
+        """
         return np.where(self(sim))
 
-    def __call__(self, sim):
+    def __call__(self, sim: snapshot.SimSnap):
+        """Return a boolean mask indicating which particles are in the filter."""
         return np.ones(len(sim), dtype=bool)
 
     def __and__(self, f2):
         return And(self, f2)
 
     def __invert__(self):
         return Not(self)
@@ -96,49 +103,62 @@
         minpos = centroids.min()
         boxsize = (deltax + maxpos - minpos)
         ncells_from_geometry = np.round(boxsize / deltax) ** 3
         assert ncells == ncells_from_geometry, "Geometry of cells doesn't match expectations"
         return boxsize, deltax
 
 class FamilyFilter(Filter):
+    """A filter that selects particles based on their family."""
+
     def __init__(self, family_):
-        assert isinstance(family_, family.Family)
-        self._descriptor = family_.name
-        self.family = family_
+        self.family = family.get_family(family_, False)
 
     def __repr__(self):
         return "FamilyFilter("+self.family.name+")"
 
     def __call__(self, sim):
         slice_ = sim._get_family_slice(self.family)
         flags = np.zeros(len(sim), dtype=bool)
         flags[slice_] = True
         return flags
 
 class And(Filter):
+    """A filter that selects particles that are in both of two other filters.
+
+    You can construct this filter conveniently using the ``&`` operator, i.e.
+
+    >>> f = f1 & f2
+
+    returns a filter that selects particles that are in both ``f1`` and ``f2``.
+    """
 
     def __init__(self, f1, f2):
-        self._descriptor = f1._descriptor + "&" + f2._descriptor
         self.f1 = f1
         self.f2 = f2
 
     def __call__(self, sim):
         return self.f1(sim) * self.f2(sim)
 
     def __repr__(self):
         return "(" + repr(self.f1) + " & " + repr(self.f2) + ")"
 
     def cubic_cell_intersection(self, centroids):
         return self.f1.cubic_cell_intersection(centroids) & \
                self.f2.cubic_cell_intersection(centroids)
 
 class Or(Filter):
+    """A filter that selects particles that are in either of two other filters.
+
+    You can construct this filter conveniently using the ``|`` operator, i.e.
+
+    >>> f = f1 | f2
+
+    returns a filter that selects particles that are in either ``f1`` or ``f2``."""
 
     def __init__(self, f1, f2):
-        self._descriptor = f1._descriptor + "|" + f2._descriptor
         self.f1 = f1
         self.f2 = f2
 
     def __call__(self, sim):
         return self.f1(sim) + self.f2(sim)
 
     def __repr__(self):
@@ -146,45 +166,56 @@
 
     def cubic_cell_intersection(self, centroids):
         return self.f1.cubic_cell_intersection(centroids) | \
             self.f2.cubic_cell_intersection(centroids)
 
 
 class Not(Filter):
+    """A filter that selects particles that are not in another filter.
+
+    You can construct this filter conveniently using the ``~`` operator, i.e.
+
+    >>> f = ~f1
+
+    returns a filter that selects particles that are not in ``f1``.
+    """
 
     def __init__(self, f):
-        self._descriptor = "~" + f._descriptor
         self.f = f
 
     def __call__(self, sim):
         x = self.f(sim)
         return np.logical_not(x)
 
     def __repr__(self):
         return "~" + repr(self.f)
 
     def cubic_cell_intersection(self, centroids):
         return ~self.f1.cubic_cell_intersection(centroids)
 
 
 class Sphere(Filter):
-
     """
-    Return particles that are within `radius` of the point `cen`.
+    A filter that selects particles within `radius` of the point `cen`.
+    """
 
-    Inputs:
-    -------
+    def __init__(self, radius: float | str | units.UnitBase, cen: ArrayLike = (0, 0, 0)):
+        """Create a sphere filter.
 
-    *radius* : extent of the sphere. Can be a number or a string specifying the units.
+        Parameters
+        ----------
 
-    *cen* : center of the sphere. default = (0,0,0)
-    """
+        radius :
+            The radius of the sphere. If a string, it is interpreted as a unit string.
+
+        cen :
+            The centre of the sphere. If a :class:`pynbody.snapshot.simsnap.SimArray`, units can be provided and
+            will be correctly accounted for.
+        """
 
-    def __init__(self, radius, cen=(0, 0, 0)):
-        self._descriptor = "sphere"
         self.cen = np.asarray(cen)
         if self.cen.shape != (3,):
             raise ValueError("Centre must be length 3 array")
 
         if isinstance(radius, str):
             radius = units.Unit(radius)
 
@@ -231,25 +262,24 @@
         if units.is_unit(self.radius):
             return f"Sphere('{str(self.radius)}', {repr(self.cen)})"
         else:
             return f"Sphere({self.radius:.2e}, {repr(self.cen)})"
 
 
 class Cuboid(Filter):
+    """A filter that selects particles within a cuboid defined by two opposite corners."""
 
-    """Create a cube with specified edge coordinates. If any of the cube
-    coordinates `x1`, `y1`, `z1`, `x2`, `y2`, `z2` are not specified
-    they are determined as `y1=x1;` `z1=x1;` `x2=-x1;` `y2=-y1;`
-    `z2=-z1`.
-
-    """
-
-    def __init__(self, x1, y1=None, z1=None, x2=None, y2=None, z2=None):
-
-        self._descriptor = "cube"
+    def __init__(self, x1: float | str | units.UnitBase, y1: float | str | units.UnitBase = None,
+                 z1: float | str | units.UnitBase = None, x2: float | str | units.UnitBase = None,
+                 y2: float | str | units.UnitBase = None, z2: float | str | units.UnitBase = None):
+        """Create a cuboid filter.
+
+        If any of the cube coordinates ``x1``, ``y1``, ``z1``, ``x2``, ``y2``, ``z2`` are not specified they are
+        determined as ``y1=x1``; ``z1=x1``; ``x2=-x1``; ``y2=-y1``; ``z2=-z1``.
+        """
         x1, y1, z1, x2, y2, z2 = (
             units.Unit(x) if isinstance(x, str) else x for x in (x1, y1, z1, x2, y2, z2))
         if y1 is None:
             y1 = x1
         if z1 is None:
             z1 = x1
         if x2 is None:
@@ -319,22 +349,37 @@
         x1, y1, z1, x2, y2, z2 = ("'%s'" % str(x)
                                   if units.is_unit_like(x) else x
                                   for x in (self.x1, self.y1, self.z1, self.x2, self.y2, self.z2))
         return f"Cuboid({x1}, {y1}, {z1}, {x2}, {y2}, {z2})"
 
 
 class Disc(Filter):
+    """A filter that selects particles within a disc of specified extent and thickness."""
 
-    """
-    Return particles that are within a disc of extent `radius` and
-    thickness `height` centered on `cen`.
-    """
+    def __init__(self, radius: float | str | units.UnitBase, height: float | str | units.UnitBase,
+                 cen: ArrayLike = (0, 0, 0)):
+        """Create a disc filter.
+
+        In keeping with other parts of pynbody, the disc is defined in the x-y plane, with the z-axis being the
+        symmetry axis. This is useful in conjunction with automated disc alignment e.g.
+        :meth:`pynbody.analysis.angmom.sideon`.
 
-    def __init__(self, radius, height, cen=(0, 0, 0)):
-        self._descriptor = "disc"
+        Parameters
+        ----------
+
+        radius :
+            The radius of the disc (in the xy-plane). If a string, it is interpreted as a unit string.
+
+        height :
+            The thickness of the disc (in the z-direction). If a string, it is interpreted as a unit string.
+
+        cen :
+            The centre of the disc. If a :class:`pynbody.snapshot.simsnap.SimArray`, units can be provided and
+            will be correctly accounted for.
+        """
         self.cen = np.asarray(cen)
         if self.cen.shape != (3,):
             raise ValueError("Centre must be length 3 array")
 
         if isinstance(radius, str):
             radius = units.Unit(radius)
 
@@ -364,23 +409,31 @@
         radius, height = (
             ("'%s'" % str(x) if units.is_unit_like(x) else '%.2e' % x) for x in (radius, height))
 
         return f"Disc({radius}, {height}, {repr(self.cen)})"
 
 
 class BandPass(Filter):
+    """Selects particles in a bandpass of a named property"""
 
-    """
-    Return particles whose property `prop` is within `min` and `max`,
-    which can be specified as unit strings.
-    """
+    def __init__(self, prop: str, min: float | str | units.UnitBase, max: float | str | units.UnitBase):
+        """Create a bandpass filter.
+
+        Parameters
+        ----------
+
+        prop :
+            The name of the simulation array to filter on.
 
-    def __init__(self, prop, min, max):
-        self._descriptor = "bandpass_" + prop
+        min :
+            The minimum value of the property. If a string, it is interpreted as a unit string.
 
+        max :
+            The maximum value of the property. If a string, it is interpreted as a unit string.
+        """
         if isinstance(min, str):
             min = units.Unit(min)
 
         if isinstance(max, str):
             max = units.Unit(max)
 
         self._prop = prop
@@ -404,23 +457,29 @@
     def __repr__(self):
         min_, max_ = (("'%s'" % str(x) if units.is_unit_like(
             x) else '%.2e' % x) for x in (self._min, self._max))
         return f"BandPass('{self._prop}', {min_}, {max_})"
 
 
 class HighPass(Filter):
-
-    """
-    Return particles whose property `prop` exceeds `min`, which can be
-    specified as a unit string.
+    """Selects particles exceeding a specified threshold of a named property
     """
 
-    def __init__(self, prop, min):
-        self._descriptor = "highpass_" + prop
+    def __init__(self, prop: str, min: float | str | units.UnitBase):
+        """Create a high-pass filter.
+
+        Parameters
+        ----------
+
+        prop :
+            The name of the simulation array to filter on.
 
+        min :
+            The minimum value of the property. If a string, it is interpreted as a unit string.
+        """
         if isinstance(min, str):
             min = units.Unit(min)
 
         self._prop = prop
         self._min = min
 
     def __call__(self, sim):
@@ -438,21 +497,29 @@
         min = ("'%s'" % str(self._min) if units.is_unit_like(
             self._min) else '%.2e' % self._min)
         return f"HighPass('{self._prop}', {min})"
 
 
 class LowPass(Filter):
 
-    """Return particles whose property `prop` is less than `max`, which can be
-    specified as a unit string.
+    """Selects particles below a specified threshold of a named property
     """
 
-    def __init__(self, prop, max):
-        self._descriptor = "lowpass_" + prop
+    def __init__(self, prop: str, max: float | str | units.UnitBase):
+        """Create a low-pass filter.
 
+        Parameters
+        ----------
+
+        prop :
+            The name of the simulation array to filter on.
+
+        max :
+            The maximum value of the property. If a string, it is interpreted as a unit string.
+        """
         if isinstance(max, str):
             max = units.Unit(max)
 
         self._prop = prop
         self._max = max
 
     def __call__(self, sim):
@@ -468,28 +535,60 @@
 
     def __repr__(self):
         max = ("'%s'" % str(self._max) if isinstance(
             self._max, units.UnitBase) else '%.2e' % self._max)
         return f"LowPass('{self._prop}', {max})"
 
 
-def Annulus(r1, r2, cen=(0, 0, 0)):
-    """
-    Convenience function that returns a filter which selects particles
-    in between two spheres specified by radii `r1` and `r2` centered
-    on `cen`.
-    """
+class Annulus(And):
+    """A filter that selects particles in between two spheres specified by radii `r1` and `r2` centered on `cen`."""
 
-    x = Sphere(max(r1, r2), cen) & ~Sphere(min(r1, r2), cen)
-    x._descriptor = "annulus"
-    return x
+    def __init__(self, r1: float | str | units.UnitBase, r2: float | str | units.UnitBase, cen: ArrayLike = (0, 0, 0)):
+        """Create an annulus filter.
 
+        Parameters
+        ----------
 
-def SolarNeighborhood(r1=units.Unit("5 kpc"), r2=units.Unit("10 kpc"), height=units.Unit("2 kpc"), cen=(0, 0, 0)):
-    """
-    Convenience function that returns a filter which selects particles
-    in a disc between radii `r1` and `r2` and thickness `height`.
+        r1 :
+            The inner radius of the annulus. If a string, it is interpreted as a unit string.
+
+        r2 :
+            The outer radius of the annulus. If a string, it is interpreted as a unit string.
+
+        cen :
+            The centre of the annulus. If a :class:`pynbody.snapshot.simsnap.SimArray`, units can be provided and
+            will be correctly accounted for.
+        """
+        super().__init__(~Sphere(r1, cen), Sphere(r2, cen))
+
+
+class SolarNeighborhood(And):
+    """A filter that selects particles in a disc between 2d radii `r1` and `r2` and thickness `height`.
+
+    As for :class:`Disc`, the galaxy disc is defined in the x-y plane, with the z-axis being the symmetry axis.
+
+    Default parameters are provided that are approximately the solar neighborhood (coarsely selected).
     """
 
-    x = Disc(max(r1, r2), height, cen) & ~Disc(min(r1, r2), height, cen)
-    x._descriptor = "Solar Neighborhood"
-    return x
+    def __init__(self, r1: float | str | units.UnitBase = units.Unit("5 kpc"),
+                 r2: float | str | units.UnitBase = units.Unit("10 kpc"),
+                 height: float | str | units.UnitBase = units.Unit("2 kpc"),
+                 cen: ArrayLike = (0, 0, 0)):
+        """Create a solar neighborhood filter.
+
+        Parameters
+        ----------
+
+        r1 :
+            The inner radius of the disc. If a string, it is interpreted as a unit string.
+
+        r2 :
+            The outer radius of the disc. If a string, it is interpreted as a unit string.
+
+        height :
+            The thickness of the disc. If a string, it is interpreted as a unit string.
+
+        cen :
+            The centre of the disc. If a :class:`pynbody.snapshot.simsnap.SimArray`, units can be provided and
+            will be correctly accounted for.
+        """
+        super().__init__(~Disc(r1, height, cen), Disc(r2, height, cen))
```

### Comparing `pynbody-2.0.0b7/pynbody/filt/geometry_selection.pyx` & `pynbody-2.0.0b8/pynbody/filt/geometry_selection.pyx`

 * *Files 12% similar despite different names*

```diff
@@ -46,14 +46,18 @@
     cdef long N=len(pos_ar)
     cdef fused_float cx,cy,cz,x,y,z,r2
     cdef fused_float r_max_2
     cdef np.ndarray[np.uint8_t, ndim=1] output = np.empty(len(pos_ar),dtype=np.uint8)
 
     cdef char* output_data = <char*> np.PyArray_DATA(output)
 
+    if len(pos_ar) == 0:
+        # The check for C-contiguous 3-col fails when len is zero, but there is nothing to do anyway, so just return
+        return output
+
     if (np.PyArray_NDIM(pos_ar)!=2 or np.PyArray_DIMS(pos_ar)[1]!=3 or
             np.PyArray_STRIDES(pos_ar)[0] != sizeof(fused_float)*3 or
             np.PyArray_STRIDES(pos_ar)[1] != sizeof(fused_float)):
         raise ValueError("Input array must be C-contiguous and have 3 columns")
 
     cdef fused_float* pos_ar_data = <fused_float*> np.PyArray_DATA(pos_ar)
```

### Comparing `pynbody-2.0.0b7/pynbody/gravity/_gravity.pyx` & `pynbody-2.0.0b8/pynbody/gravity/_gravity.pyx`

 * *Files identical despite different names*

### Comparing `pynbody-2.0.0b7/pynbody/halo/__init__.py` & `pynbody-2.0.0b8/pynbody/halo/__init__.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,38 +1,85 @@
 """
+Support for halo and group catalogues.
 
-halo
-====
-
-Implements halo catalogue functions. If you have a supported halo
-catalogue on disk or a halo finder installed and correctly configured,
-you can access a halo catalogue through f.halos() where f is a
-SimSnap.
-
-See the `halo tutorial
-<http://pynbody.github.io/pynbody/tutorials/halos.html>`_ for some
-examples.
-
-Halo catalogues act like a dictionary, mapping from a _halo number_ to a
-Halo object. The halo number is typically determined by the halo finder, and
-is often (but not always) the same as the _halo index_ which is the zero-based
+Halo catalogues act like a dictionary, mapping from halo numbers to a Halo objects. The halo *number* is typically
+determined by the halo finder, and is often (but not always) the same as the halo *index* which is the zero-based
 offset within the catalogue.
+
+If you have a supported halo catalogue on disk or a halo finder installed and correctly configured, you can access a
+halo catalogue through ``f.halos()`` where ``f`` is a SimSnap.
+
+See the :ref:`halo catalogue tutorial <halo_tutorial>` for introductory information and guidance.
+
+
+.. _v2_0_halo_changes:
+
+.. versionchanged:: 2.0
+
+  Backwards-incompatible changes to the halo catalogue system
+
+  For version 2.0, the halo catalogue loading system was substantially rewritten. The new system is more robust and
+  more consistent across different halo finders. However, this means that some defaults have changed, most significantly
+  in the AHF halo numbering. Backward-compatibility can be achieved by passing ``halo_numbers='v1'`` to the
+  :class:`~pynbody.halo.ahf.AHFCatalogue` constructor. For more information, read the documentation for that class.
+
+  Furthermore, older versions of pynbody (i.e. v1.x) could be configured to create a halo catalogue if one was not
+  found, using AHF. This is no longer the case, as creating a halo catalogue requires choosing a halo finder and its
+  parameters carefully for the task in hand and it was not possible to provide a one-size-fits-all solution.
+
+  Finally, options to write ``.stat`` files and ``.grp`` files have been removed. However it is still possible to
+  generate a ``.grp`` file by  calling :meth:`~HaloCatalogue.get_group_array` and writing out the resulting
+  array of integers using a tool like ``numpy.savetxt``.
+
+  By paring back the less-used functionality of the halo catalogue system, the remaining functionality is more
+  consistent, robust, and extensible to new halo finders.
+
+
+.. _supported_halo_finders:
+
+Supported halo-finder formats
+-----------------------------
+
+The currently-supported formats are:
+
+- Adaptahop (:class:`~pynbody.halo.adaptahop.AdaptaHOPCatalogue`);
+- AHF (:class:`~pynbody.halo.ahf.AHFCatalogue`);
+- HBT+ (:class:`~pynbody.halo.hbtplus.HBTPlusCatalogue`);
+- HOP (:class:`~pynbody.halo.hop.HOPCatalogue`);
+- Rockstar (:class:`~pynbody.halo.rockstar.RockstarCatalogue`);
+- Subfind (old format :class:`~pynbody.halo.subfind.SubfindCatalogue`, or various HDF5 variants
+  as :class:`~pynbody.halo.subfindhdf.SubfindHDFCatalogue`);
+- VELOCIraptor (:class:`~pynbody.halo.velociraptor.VelociraptorCatalogue`).
+
+In addition, generic halo finders which output a list of halo numbers for each particle are supported via
+:class:`~pynbody.halo.number_array.HaloNumberCatalogue`.
+
+
+
+.. note::
+
+    The principal development of ``pynbody`` took place in the UK, and the spelling of "catalogue" is British English.
+    However, since much code is written in American English, v2.0.0 introduced aliases such that all
+    classes can be accessed with the American spelling ``HaloCatalog``, ``AdaptaHOPCatalog`` etc.
+
+
 """
 from __future__ import annotations
 
 import copy
 import logging
 import warnings
 import weakref
 from typing import TYPE_CHECKING, Iterable
 
 import numpy as np
 from numpy.typing import NDArray
 
-from .. import iter_subclasses, snapshot, units, util
+from .. import array, snapshot, units, util
+from ..util import iter_subclasses
 from .details.iord_mapping import make_iord_to_offset_mapper
 from .details.number_mapping import MonotonicHaloNumberMapper, create_halo_number_mapper
 from .details.particle_indices import HaloParticleIndices
 
 if TYPE_CHECKING:
     from .subhalo_catalogue import SubhaloCatalogue
 
@@ -46,15 +93,18 @@
     def physical_units(self, *args, **kwargs):
         pass
 
 
 class Halo(snapshot.subsnap.IndexedSubSnap):
 
     """
-    Generic class representing a halo.
+    Represents a single halo from a halo catalogue.
+
+    Note that pynbody refers to groups, halos and subhalos interchangably, with the term "halo" being used to cover
+    all of these.
     """
 
     def __init__(self, halo_number, properties, halo_catalogue, *args, **kwa):
         super().__init__(*args, **kwa)
         self._halo_catalogue = halo_catalogue
         self._halo_number = halo_number
         self._descriptor = "halo_" + str(halo_number)
@@ -64,51 +114,24 @@
 
         # Inherit autoconversion from parent
         self._autoconvert_properties()
 
     @property
     @util.deprecated("The sub property has been renamed to subhalos")
     def sub(self):
+        """Deprecated alias for :property:`subhalos`."""
         return self.subhalos
 
     @property
     def subhalos(self) -> SubhaloCatalogue:
+        """A HaloCatalogue object containing only the subhalos of this halo."""
         return self._halo_catalogue._get_subhalo_catalogue(self._halo_number)
 
-    def physical_units(self, distance='kpc', velocity='km s^-1', mass='Msol', persistent=True, convert_parent=True):
-        """
-        Converts all array's units to be consistent with the
-        distance, velocity, mass basis units specified.
-
-        Base units can be specified using keywords.
-
-        **Optional Keywords**:
-
-           *distance*: string (default = 'kpc')
-
-           *velocity*: string (default = 'km s^-1')
-
-           *mass*: string (default = 'Msol')
-
-           *persistent*: boolean (default = True); apply units change to future lazy-loaded arrays if True
-
-           *convert_parent*: boolean (default = None); if True, propagate units change to parent snapshot. See note below.
 
-        **Note**:
-
-            When convert_parent is True, the unit conversion is propagated to
-            the parent halo catalogue and the halo properties *are not
-            converted*. The halo catalogue is in charge of calling
-            physical_units with convert_parent=False for all halo objects
-            (including this one).
-
-            When convert_parent is False, the properties are converted
-            immediately.
-
-        """
+    def physical_units(self, distance='kpc', velocity='km s^-1', mass='Msol', persistent=True, convert_parent=True):
         if convert_parent:
             self._halo_catalogue.physical_units(
                 distance=distance,
                 velocity=velocity,
                 mass=mass,
                 persistent=persistent
             )
@@ -118,56 +141,76 @@
 
 
 class HaloCatalogue(snapshot.util.ContainerWithPhysicalUnitsOption,
                     iter_subclasses.IterableSubclasses):
 
     """Generic halo catalogue object.
 
-    To the user, this presents a simple interface where calling h[i] returns halo i.
+    To the user, this presents a simple interface where calling ``h[i]`` returns halo ``i``. Properties of halos
+    can be retrieved without loading the halo via :meth:`get_properties_one_halo` or :meth:`get_properties_all_halos`.
+
+    More information for users can be found in the :ref:`halo catalogue tutorial <halo_tutorial>`; see also the
+    :ref:`supported halo finders <supported_halo_finders>`.
 
-    By convention, i should use the halo finder's own indexing scheme, e.g. if the halo-finder is one-based then
-    h[1] should return the first halo.
+    Implementing a new format
+    ^^^^^^^^^^^^^^^^^^^^^^^^^
+
+    To support a new format, subclass :class:`HaloCatalogue` and implement the following methods:
+
+    * :meth:`__init__`
+    * :meth:`_can_load`
+    * :meth:`_get_all_particle_indices`
+    * :meth:`_get_particle_indices_one_halo` [only if it's possible to do this more efficiently than
+      :meth:`_get_all_particle_indices` for users accessing only a few halos]
+    * :meth:`get_properties_all_halos` [only if you have halo finder-provided properties to expose]
+    * :meth:`get_properties_one_halo` [only if you have halo finder-provided properties to expose, and it's efficient
+      to expose them one halo at a time; the default implementation will call get_properties_all_halos and extract]
+    * :meth:`get_group_array` [only if it's possible to do this more efficiently than the default implementation]
+
+    Nomenclature/conventions are worth being aware of if you are implementing a new format:
+
+    * The halo number is the user-exposed identifier for a halo. It is typically assigned by the halo finder, although
+      subclasses are free to assign their own (e.g. some have a `halo_number` option that can be passed to the
+      constructor to override the halo finder's numbering). The halo numbers are used to access individual halos via
+      the [] operator.
+    * The halo *index* is the zero-based offset within the catalogue, which may be different from the halo number.
+      Internally, *pynbody* converts between these using a :class:`details.number_mapping.HaloNumberMapper` object,
+      which is set up in the :meth:`__init__` method.
+    * Particle indices should be returned from methods like :meth:`_get_particle_indices_one_halo` as zero-relative
+      offsets within the snapshot, not particle IDs or 'iord's. Many halo finders output particle IDs which must
+      therefore be mapped. To aid this, call :meth:`_init_iord_to_fpos` in your :meth:`__init__` method, which creates
+      a mapper as :attr:`_iord_to_fpos`. See :mod:`details.iord_mapping` for more information.
 
-    To support a new format, subclass this and implement the following methods:
-      __init__, which must pass a HaloNumberMapper into the base constructor, to specify what halos are available
-      _get_all_particle_indices [essential]
-      _get_particle_indices_one_halo [optional, if it's possible to do this more efficiently than _get_all_particle_indices]
-      get_properties_one_halo [only if you have halo finder-provided properties to expose]
-      get_properties_all_halos [only if you have halo finder-provided properties to expose]
-      _get_halo [only if you want to add further customization to halos]
-      _get_num_halos [optional, if it's possible to do this more efficiently than calling _get_index_list_all_halos]
-      get_group_array [only if it's possible to do this more efficiently than the default implementation]
-      _get_subhalo_catalogue [optional, if this halo catalogue supports subhalos]; user-accessed via .subhalos on a Halo
-
-    Note that particle indices are zero-relative offsets within pynbody's representation of the snapshot. They are not
-    the same as particle IDs or 'iord's which are the particle IDs stored in the simulation file. To aid converting
-    between iords/IDs (which are used by many halo finder outputs) and pynbody's particle indices, call
-    _init_iord_to_fpos, which creates a mapper as _iord_to_fpos. See details/iord_mapping.py for more information.
     """
 
     def __init__(self, sim, number_mapper):
         self._base: weakref[snapshot.SimSnap] = weakref.ref(sim)
-        self.number_mapper: MonotonicHaloNumberMapper = number_mapper
+        self.number_mapper: HaloNumberMapper = number_mapper
         self._index_lists: HaloParticleIndices | None = None
         self._properties: dict | None = None
         self._cached_halos: dict[int, Halo] = {}
+        self._persistent_units = None
 
     def load_all(self):
         """Loads all halos, which is normally more efficient if a large fraction of them will be accessed."""
         if not self._index_lists:
             index_lists = self._get_all_particle_indices()
             properties = self.get_properties_all_halos(with_units=True)
             if isinstance(index_lists, tuple):
                 index_lists = HaloParticleIndices(*index_lists)
             self._index_lists = index_lists
             if len(properties)>0:
                 self._properties = properties
 
+            if self._persistent_units is not None:
+                self._cached_properties_to_physical_units(self._persistent_units)
+
     @util.deprecated("precalculate has been renamed to load_all")
     def precalculate(self):
+        """Deprecated alias for :meth:`load_all`"""
         self.load_all()
 
     def _get_num_halos(self):
         return len(self.number_mapper)
 
     def _get_all_particle_indices_cached(self):
         """Get the index information for all halos, using a cached version if available"""
@@ -181,27 +224,39 @@
         - particle_ids: particle IDs contained in halos, sorted by halo ID
         - boundaries: the indices in particle_ids where each halo starts and ends
         """
         raise NotImplementedError("This halo catalogue does not support loading all halos at once")
 
     def get_properties_one_halo(self, halo_number) -> dict:
         """Returns a dictionary of properties for a single halo, given a halo_number """
-        return {}
+
+        # Default implementation: extract from all halos. Subclasses may override this if they can load properties
+        # for a single halo more efficiently.
+        self._properties = self.get_properties_all_halos(with_units=True)
+        return self._get_properties_one_halo_using_cache_if_available(halo_number,
+                                                                      self.number_mapper.number_to_index(halo_number))
 
     def get_properties_all_halos(self, with_units=True) -> dict:
         """Returns a dictionary of properties for all halos.
 
         If with_units is True, the properties are returned as SimArrays with units if possible. Otherwise, numpy arrays
         are returned.
 
         Note that the returned properties are in contiguous arrays, and as a result may be in a different order to the
         halo numbers which are used to access individual halos. To map between halo numbers and properties, use the
         .number_mapper object; or access individual property dictionaries by halo number using get_properties_one_halo."""
         return {}
 
+    def _get_properties_one_halo_using_cache_if_available(self, halo_number, halo_index):
+        if self._properties is None:
+            return self.get_properties_one_halo(halo_number)
+        else:
+            return {k: units.get_item_with_unit(self._properties[k],halo_index)
+                    for k in self._properties}
+
     def _get_particle_indices_one_halo(self, halo_number) -> NDArray[int]:
         """Get the index list for a single halo, given a halo_number.
 
         A generic implementation is provided that fetches index lists for all halos and then extracts the one"""
         self.load_all()
         return self._index_lists.get_particle_index_list_for_halo(
             self.number_mapper.number_to_index(halo_number)
@@ -219,21 +274,14 @@
             # if not, the default implementation will populate _cached_index_lists
 
     def _get_halo_cached(self, halo_number) -> Halo:
         if halo_number not in self._cached_halos:
             self._cached_halos[halo_number] = self._get_halo(halo_number)
         return self._cached_halos[halo_number]
 
-    def _get_properties_one_halo_using_cache_if_available(self, halo_number, halo_index):
-        if self._properties is None:
-            return self.get_properties_one_halo(halo_number)
-        else:
-            return {k: units.get_item_with_unit(self._properties[k],halo_index)
-                    for k in self._properties}
-
     def _get_halo(self, halo_number) -> Halo:
         halo_index = self.number_mapper.number_to_index(halo_number)
         return Halo(halo_number,
                     self._get_properties_one_halo_using_cache_if_available(halo_number, halo_index),
                     self, self.base,
                     self._get_particle_indices_one_halo_using_list_if_available(halo_number, halo_index))
 
@@ -247,25 +295,33 @@
         return self._get_num_halos()
 
     def __iter__(self) -> Iterable[Halo]:
         self.load_all()
         for i in self.number_mapper:
             yield self[i]
 
+    def __repr__(self):
+        return f"<{type(self).__name__}, length {len(self)}>"
+
+    def keys(self):
+        """Return an iterable of all halo numbers in the catalogue."""
+        return self.number_mapper.all_numbers
+
     def __getitem__(self, item) -> Halo | SubhaloCatalogue:
         from .subhalo_catalogue import SubhaloCatalogue
         if isinstance(item, slice):
             return SubhaloCatalogue(self, np.arange(*item.indices(len(self))))
         elif hasattr(item, "__len__"):
             return SubhaloCatalogue(self, item)
         else:
             return self._get_halo_cached(item)
 
     @property
     def base(self) -> snapshot.SimSnap:
+        """The snapshot object that this halo catalogue is based on."""
         return self._base()
 
     def _init_iord_to_fpos(self):
         """Create a member array, _iord_to_fpos, that maps particle IDs to file positions.
 
         This is a convenience function for subclasses to use."""
         if not hasattr(self, "_iord_to_fpos"):
@@ -286,27 +342,43 @@
         from .subhalo_catalogue import SubhaloCatalogue
         props = self.get_properties_one_halo(parent_halo_number)
         if 'children' in props:
             return SubhaloCatalogue(self, props['children'])
         else:
             raise ValueError(f"This halo catalogue does not support subhalos")
 
+    @util.deprecated("This method is deprecated and will be removed in a future release. Use python `in` syntax instead.")
     def contains(self, halo_number: int) -> bool:
+        """Deprecated alias; instead of ``h.contains(number)`` use ``number in h``."""
+        return halo_number in self
+
+    def __contains__(self, halo_number) -> bool:
+        """Returns True if the halo catalogue contains the specified halo number."""
         return halo_number in self.number_mapper
 
-    def __contains__(self, haloid):
-        return self.contains(haloid)
+    def get_group_array(self, family=None, use_index=False):
+        """Return an array with an integer for each particle in the simulation, indicating the halo of that particle.
+
+        If there are multiple levels (i.e. subhalos), the number returned corresponds to the lowest level, i.e.
+        the smallest subhalo.
 
-    def get_group_array(self, family=None):
-        """Return an array with an integer for each particle in the simulation
-        indicating which halo that particle is associated with. If there are multiple
-        levels (i.e. subhalos), the number returned corresponds to the lowest level, i.e.
-        the smallest subhalo."""
+        Parameters
+        ----------
+
+        family : str, optional
+            If specified, return only the group array for the specified family.
+
+        use_index: bool, optional
+            If True, return the halo index rather than the halo number. (See the class documentation for the
+            distinction between halo numbers and indices.)
+
+        """
         self.load_all()
-        number_per_particle = self._index_lists.get_halo_number_per_particle(len(self.base), self.number_mapper)
+        number_per_particle = self._index_lists.get_halo_number_per_particle(len(self.base),
+                                                                             None if use_index else self.number_mapper)
         if family is not None:
             return number_per_particle[self.base._get_family_slice(family)]
         else:
             return number_per_particle
 
     def load_copy(self, halo_number):
         """Load a fresh SimSnap with only the particles in specified halo
@@ -314,54 +386,70 @@
         This relies on the underlying SimSnap being capable of partial loading."""
         from .. import load
         halo_index = self.number_mapper.number_to_index(halo_number)
         return load(self.base.filename,
                     take=self._get_particle_indices_one_halo_using_list_if_available(halo_number, halo_index))
 
     def physical_units(self, distance='kpc', velocity='km s^-1', mass='Msol', persistent=True, convert_parent=False):
-        """
-        Converts all array's units to be consistent with the
-        distance, velocity, mass basis units specified.
-
-        Base units can be specified using keywords.
-
-        **Optional Keywords**:
-
-           *distance*: string (default = 'kpc')
-
-           *velocity*: string (default = 'km s^-1')
-
-           *mass*: string (default = 'Msol')
-
-           *persistent*: boolean (default = True); apply units change to future lazy-loaded arrays if True
-
-           *convert_parent*: boolean (default = None); ignored for HaloCatalogue objects
-
-        """
         self.base.physical_units(distance=distance, velocity=velocity, mass=mass, persistent=persistent)
 
         # Convert all instantiated subhalos
         for halo in self._cached_halos.values():
             halo.physical_units(
                 distance,
                 velocity,
                 mass,
                 persistent=persistent,
                 convert_parent=False
             )
 
+        all_units = [units.Unit(x) for x in (distance, velocity, mass, 'a', 'h', 'K')]
+
+        if persistent:
+            self._persistent_units = all_units
+
+        self._cached_properties_to_physical_units(all_units)
+
+    def _cached_properties_to_physical_units(self, all_units):
+        if self._properties is not None:
+            for k in self._properties:
+                if isinstance(self._properties[k], array.SimArray) and units.has_unit(self._properties[k]):
+                    self.base._autoconvert_array_unit(self._properties[k], all_units)
+
+
     @classmethod
     def _can_load(cls, sim):
         return False
 
-
 from . import (
     adaptahop,
     ahf,
     hbtplus,
     hop,
     number_array,
     rockstar,
     subfind,
     subfindhdf,
     velociraptor,
 )
+
+
+def _fix_american_spelling(p):
+    """Map American to British spelling (used by SimSnap.halos to allow flexible spelling)"""
+    if isinstance(p, str) and p.endswith('Catalog'):
+        return p.replace('Catalog', 'Catalogue')
+    else:
+        return p
+def _alias_american_spelling():
+    """Create American spelling aliases for all HaloCatalogue subclasses."""
+    for c in HaloCatalogue.iter_subclasses():
+        american_name = c.__name__.replace("Catalogue", "Catalog")
+        # put american_name into the same module as c (not this module)
+
+        if c.__module__.startswith('pynbody.halo.'):
+            module = eval(c.__module__.replace('pynbody.halo.', ''))
+
+        setattr(module, american_name, c)
+
+    globals()['HaloCatalog'] = HaloCatalogue
+
+_alias_american_spelling()
```

### Comparing `pynbody-2.0.0b7/pynbody/halo/adaptahop.py` & `pynbody-2.0.0b8/pynbody/halo/adaptahop.py`

 * *Files 6% similar despite different names*

```diff
@@ -54,47 +54,69 @@
     'virial_temperature': unit_temperature,
     'nfw_rho0': unit_density,
     'density_profile': unit_density,
 }
 
 
 class BaseAdaptaHOPCatalogue(HaloCatalogue):
-    """A AdaptaHOP Catalogue. AdaptaHOP output files must be in
-    Halos/<simulation_number>/ directory or specified by fname"""
+    """Handles catalogues produced by AdaptaHOP."""
 
     _AdaptaHOP_fname = None
     _halos = None
     _headers = None
     _fname = ""
     _read_contamination = False
 
     _halo_attributes = tuple()
     _halo_attributes_contam = tuple()
     _header_attributes = tuple()
 
-    def __init__(self, sim, fname=None, read_contamination=None, longint=None):
+    def __init__(self, sim, filename=None, read_contamination=None, longint=None):
+        """Initialise a AdaptaHOP catalogue.
+
+        Parameters
+        ----------
+
+        sim : ~pynbody.snapshot.simsnap.SimSnap
+            The snapshot to which this catalogue is attached.
+
+        filename : str, optional
+            The filename of the AdaptaHOP catalogue (``path/to/tree_bricksXXX``). If not specified, the
+            code will attempt to find the catalogue in the simulation directory.
+
+        read_contamination : bool, optional
+            Whether to read information about contamination of each halo. If not specified, the code will attempt to
+            detect the format. Note that if specifying read_contamination, longint must also be specified.
+
+        longint : bool, optional
+            Whether to read 64-bit integers. If not specified, the code will attempt to detect the format. Note that if
+            specifying longint, read_contamination must also be specified.
+        """
         if FortranFile is None:
             raise RuntimeError(
                 "Support for AdaptaHOP requires the package `cython-fortran-file` to be installed."
             )
 
-        if fname is None:
-            for fname in AdaptaHOPCatalogue._enumerate_hop_tag_locations_from_sim(sim):
-                if os.path.exists(fname):
+        if filename is None:
+            for filename in AdaptaHOPCatalogue._enumerate_hop_tag_locations_from_sim(sim):
+                if os.path.exists(filename):
                     break
 
-            if not os.path.exists(fname):
+            if not os.path.exists(filename):
                 raise RuntimeError(
                     "Unable to find AdaptaHOP brick file in simulation directory"
                 )
 
-        self._fname = fname
+        self._fname = filename
+
+        if (read_contamination or longint) is not None and (read_contamination is None or longint is None):
+            raise ValueError("If specifying read_contamination or longint, both must be specified")
 
         if read_contamination is None or longint is None:
-            read_contamination, longint = self._detect_file_format(fname)
+            read_contamination, longint = self._detect_file_format(filename)
         self._read_contamination = read_contamination
         self._longint = longint
 
         if self._longint:
             self._length_type = np.int64
         else:
             self._length_type = np.int32
@@ -122,28 +144,29 @@
         # but then the parent class will use the position offsets as though they refer to the whole file
         dm_offset = self.base._get_family_slice('dm').start
         if dm_offset>0:
             self._iord_to_fpos = iord_mapping.IordOffsetModifier(self._iord_to_fpos, dm_offset)
 
         self._halos = {}
 
-        self._AdaptaHOP_fname = fname
+        self._AdaptaHOP_fname = filename
 
 
         logger.debug("AdaptaHOPCatalogue loaded")
 
-    def _detect_file_format(self, fname):
+    @classmethod
+    def _detect_file_format(cls, fname):
         """
         Detect if the file is in the old format or the new format.
         """
         with FortranFile(fname) as fpu:
-            longint_flag = self._detect_longint(fpu, (False, True))
+            longint_flag = cls._detect_longint(fpu, (False, True))
 
             # Now attempts reading the first halo data
-            attrs, attrs_contam = (self.convert_i8b(_, longint_flag) for _ in (self._halo_attributes, self._halo_attributes_contam))
+            attrs, attrs_contam = (cls.convert_i8b(_, longint_flag) for _ in (cls._halo_attributes, cls._halo_attributes_contam))
 
             if len(attrs_contam) == 0:
                 read_contamination = False
             else:
                 fpu.skip(3) # number + ids of parts + halo_ID
                 fpu.read_attrs(attrs)
                 try:
@@ -334,38 +357,35 @@
                 return longint_flag
             except (ValueError, OSError):
                 pass
 
         raise ValueError("Could not detect longint")
 
     @classmethod
-    def _can_load(cls, sim, arr_name="grp", *args, **kwa):
-        candidates = [
-            fname
-            for fname in cls._enumerate_hop_tag_locations_from_sim(sim)
-        ]
+    def _can_load(cls, sim, filename=None, arr_name="grp", *args, **kwa):
+        if cls is BaseAdaptaHOPCatalogue:
+            return False # Must load a specialisation
+
+        if filename is None:
+            candidates = [
+                fname
+                for fname in cls._enumerate_hop_tag_locations_from_sim(sim)
+            ]
+        else:
+            candidates = [filename]
         valid_candidates = [fname for fname in candidates if os.path.exists(fname)]
         if len(valid_candidates) == 0:
             return False
 
-        # Logic is as follows:
-        # - If `longint` is provided, try loading with it.
-        # - Otherwise, try loading with and without it
-        use_longint = kwa.pop("longint", None)
-        if use_longint is None:
-            longint_flags = [True, False]
-        else:
-            longint_flags = use_longint
         for fname in valid_candidates:
-            with FortranFile(fname) as fpu:
-                try:
-                    cls._detect_longint(fpu, longint_flags)
-                    return True
-                except ValueError:
-                    pass
+            try:
+                cls._detect_file_format(fname)
+                return True
+            except ValueError:
+                pass
         return False
 
     @staticmethod
     def _enumerate_hop_tag_locations_from_sim(sim):
         try:
             match = re.search("output_([0-9]{5})", sim.filename)
             if match is None:
```

### Comparing `pynbody-2.0.0b7/pynbody/halo/ahf.py` & `pynbody-2.0.0b8/pynbody/halo/ahf.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,15 @@
+"""AHF (Amiga Halo Finder) support"""
+
+from __future__ import annotations
+
 import glob
 import gzip
 import os.path
+import pathlib
 import re
 import warnings
 
 import numpy as np
 
 from .. import snapshot, util
 from . import HaloCatalogue, HaloParticleIndices, logger
@@ -12,88 +17,91 @@
     NonMonotonicHaloNumberMapper,
     SimpleHaloNumberMapper,
     create_halo_number_mapper,
 )
 
 
 class AHFCatalogue(HaloCatalogue):
-
     """
     Class to handle catalogues produced by Amiga Halo Finder (AHF).
     """
 
-    def __init__(self, sim, make_grp=None, get_all_parts=None, use_iord=None, ahf_basename=None,
+    def __init__(self, sim, filename=None, make_grp=None, get_all_parts=None, use_iord=None, ahf_basename=None,
                  dosort=None, only_stat=None, write_fpos=True, halo_numbers='file-order',
                  ignore_missing_substructure=True,
                  **kwargs):
         """Initialize an AHFCatalogue.
 
-        **kwargs** :
+        Parameters
+        ----------
 
-        *use_iord*: if True, the particle IDs in the Amiga catalogue
-                    are taken to refer to the iord array. If False,
-                    they are the particle offsets within the file. If
-                    None, the parameter defaults to True for
-                    GadgetSnap, False otherwise.
-
-        *ahf_basename*: specify the basename of the AHF halo catalog
-                        files - the code will append 'halos',
-                        'particles', and 'substructure' to this
-                        basename to load the catalog data.
-
-        *halo_numbers*: specify how to number the halos. Options are:
-                             'ahf' (default): use the halo numbers written in the AHF halos file,
-                                              or a zero-based indexing if none is present
-                             'file-order': zero-based indexing of the halos
-                             'v1': one-based indexing of the halos, compatible with pynbody v1.x
-                             'length-order': sort by the number of particles in each halo, with the
-                                             halo with most particles being halo 0
-                             'length-order-v1': as length-order, but indexing from halo 1,
-                                                compatible with dosort=True in pynbody v1
-
-        *ignore_missing_substructure*: if True (default), the code will not
-                            raise an exception if the substructure file is
-                            missing or corrupt. If False, it will raise an exception.
-
-        Deprecated kwargs:
-
-        *make_grp*: if True a 'grp' array is created in the underlying
-                    snapshot specifying the lowest level halo that any
-                    given particle belongs to. If it is False, no such
-                    array is created; if None, the behaviour is
-                    determined by the configuration system.
-
-        *get_all_parts*: if True, the particle file is loaded for all halos.
-                    Suggested to keep this None, as this is memory intensive.
-                    The default function is to load in this data as needed.
-
-        *dosort*: equivalent to halo_numbers='length-order'
-
-        *only_stat*: specify that you only wish to collect the halo
-                    properties stored in the AHF_halos file and not
-                    worry about particle information [deprecated, use
-                    get_dummy_halo instead]
+        *sim*: SimSnap
+          the simulation snapshot to which this catalogue refers
 
-        """
+        *filename*: str | pathlib.Path
+          specify a path to an AHF halo catalog. Note that AHF actually outputs multiple files; you can specify the
+          path to the ``AHF_halos`` or ``AHF_particles`` file and the code will infer the other filenames from this.
+          Alternatively you can specify the path up to the ``AHF_`` prefix and the code will similarly infer the full
+          set of filenames.
+
+        *halo_numbers*: str
+          specify how to number the halos. Options are:
+
+          * 'ahf' (default): use the halo numbers written in the AHF halos file if present, or a zero-based indexing
+          * 'file-order': zero-based indexing of the halos
+          * 'v1': one-based indexing of the halos, compatible with pynbody v1 default behaviour
+          * 'length-order': sort by the number of particles in each halo, with the halo with most particles being halo 0
+          * 'length-order-v1': as length-order, but indexing from halo 1, compatible with ``dosort=True`` in pynbody v1
+
+        *ignore_missing_substructure*: bool
+          If True (default), the code will not raise an exception if the substructure file is missing or corrupt. If
+          False, it will raise an exception.
+
+        *use_iord*: bool
+          if True, the particle IDs in the Amiga catalogue are taken to refer to the iord array. If False,
+          they are the particle offsets within the file. If None, the parameter defaults to True for GadgetSnap,
+          False otherwise.
+
+        *ahf_basename*: str
+          Deprecated way to specify the location of the catalogue
+
+        *make_grp*:
+          Deprecated. If True a 'grp' array is created in the underlying snapshot specifying the lowest level halo
+          that any given particle belongs to. If it is False, no such array is created; if None, the behaviour is
+          determined by the configuration system.
+
+        *get_all_parts*:
+          Deprecated; use the :meth:`load_all` method instead.
+
+        *dosort*:
+          Deprecated; equivalent to ``halo_numbers='length-order'``
+
+        *only_stat*:
+          Deprecated; this keyword is now ignored. To obtain halo information without loading the particles,
+          use the methods :meth:`get_properties_one_halo` or :meth:`get_properties_all_halos`.
 
+        """
 
         if use_iord is None:
             use_iord = isinstance(
                 sim.ancestor,
                 (snapshot.gadget.GadgetSnap, snapshot.gadgethdf.GadgetHDFSnap)
             )
 
         self._use_iord = use_iord
         self._only_stat = only_stat
         self._try_writing_fpos = write_fpos
 
         if only_stat:
             warnings.warn(DeprecationWarning("only_stat keyword is deprecated; instead, use the catalogue's get_dummy_halo method"))
 
-        if ahf_basename is not None:
+        if filename is not None:
+            self._ahfBasename = str(self._user_specified_filename_to_ahf_basename(filename))
+        elif ahf_basename is not None:
+            warnings.warn(DeprecationWarning("ahf_basename keyword is deprecated; use filename instead"))
             self._ahfBasename = ahf_basename
         else:
             self._ahfBasename = self._infer_ahf_basename(sim)
 
         self._determine_format_revision_from_filename()
 
         logger.info("AHFCatalogue loading halo properties")
@@ -336,33 +344,36 @@
 
         # get all the property names from the first, commented line
         # remove (#)
         fields = first_line.replace("#", "").split()
         keys = [re.sub(r'\([0-9]*\)', '', field)
                 for field in fields]
 
+        omit_first_column = False
+
         if self._is_new_format:
             # fix for column 0 being a non-column in some versions of the AHF
             # output
             if keys[0] == '':
+                omit_first_column = True
                 keys = keys[1:]
 
         self._halo_properties = {k: [] for k in keys}
 
         self._num_halos = len(lines)
 
         for line in lines:
             values = [
                 float(x) if any(_ in x for _ in (".", "e", "nan", "inf"))
                 else int(x)
                 for x in line.split()
             ]
             # XXX Unit issues!  AHF uses distances in Mpc/h, possibly masses as
             # well
-            if not self._is_new_format:
+            if omit_first_column:
                 values = values[1:]
 
             for key, value in zip(keys, values):
                 self._halo_properties[key].append(value)
 
         for key in keys:
             self._halo_properties[key] = np.array(self._halo_properties[key])
@@ -403,13 +414,29 @@
 
         if os.path.isdir(sim._filename):
             candidates = candidates.union(glob.glob(os.path.join(sim._filename, "*z*particles*")))
 
         return list(candidates)
 
     @classmethod
-    def _can_load(cls, sim, ahf_basename=None, **kwargs):
-        if ahf_basename:
-            return True
-        candidates = cls._list_candidate_ahf_basenames(sim)
-        number_ahf_file_candidates = len(candidates)
-        return number_ahf_file_candidates > 0
+    def _user_specified_filename_to_ahf_basename(cls, filename: str | pathlib.Path) -> pathlib.Path:
+        allowed_endings = ["AHF_halos", "AHF_particles", "AHF_", "AHF"]
+        filename = util.cutgz(filename)
+        for ending in allowed_endings:
+            if str(filename).endswith(ending):
+                return pathlib.Path(str(filename)[:-len(ending)]+"AHF_")
+        raise ValueError("Filename cannot be understood as an AHF catalogue basename. "
+                         "For information about how to specify an AHF filename, see the class documentation for "
+                         "AHFCatalogue.")
+
+    @classmethod
+    def _can_load(cls, sim, filename=None, **kwargs):
+        if filename is not None:
+            try:
+                cls._user_specified_filename_to_ahf_basename(filename)
+                return True
+            except ValueError:
+                return False
+        else:
+            candidates = cls._list_candidate_ahf_basenames(sim)
+            number_ahf_file_candidates = len(candidates)
+            return number_ahf_file_candidates > 0
```

### Comparing `pynbody-2.0.0b7/pynbody/halo/details/iord_mapping.py` & `pynbody-2.0.0b8/pynbody/halo/details/iord_mapping.py`

 * *Files identical despite different names*

### Comparing `pynbody-2.0.0b7/pynbody/halo/details/number_mapping.py` & `pynbody-2.0.0b8/pynbody/halo/details/number_mapping.py`

 * *Files identical despite different names*

### Comparing `pynbody-2.0.0b7/pynbody/halo/details/particle_indices.py` & `pynbody-2.0.0b8/pynbody/halo/details/particle_indices.py`

 * *Files 18% similar despite different names*

```diff
@@ -29,22 +29,27 @@
         i.e. the one whose index list starts at self.boundaries[obj_offset]"""
         ptcl_start, ptcl_end = self.particle_index_list_boundaries[obj_offset]
         return slice(ptcl_start, ptcl_end)
 
     def get_halo_number_per_particle(self, sim_length, number_mapper, fill_value=-1, dtype=int):
         """Return an array of halo numbers, one per particle.
 
-        Requires a HaloNumberMapper to map halo indices to halo numbers"""
+        Requires a HaloNumberMapper to map halo indices to halo numbers. If None is passed for the number_mapper,
+        the halo indices are returned instead."""
         lengths = np.diff(self.particle_index_list_boundaries, axis=1).ravel()
         ordering = np.argsort(-lengths, kind='stable')
 
         id_array = np.empty(sim_length, dtype=dtype)
         id_array.fill(fill_value)
 
-        halo_numbers = number_mapper.index_to_number(ordering)
+        if number_mapper is not None:
+            halo_numbers = number_mapper.index_to_number(ordering)
+        else:
+            halo_numbers = range(len(ordering))
+
         for halo_number, halo_index in zip(halo_numbers, ordering):
             indexing_slice = self._get_index_slice_for_halo(halo_index)
             id_array[self.particle_index_list[indexing_slice]] = halo_number
 
         return id_array
 
     def __len__(self):
```

### Comparing `pynbody-2.0.0b7/pynbody/halo/hbtplus.py` & `pynbody-2.0.0b8/pynbody/halo/hbtplus.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,46 +1,104 @@
+"""HBT+ halo catalogue support.
+
+.. _hbt_plus_parent_groups:
+
+HBT+ and parent groups
+----------------------
+
+HBT+ identifies halos, not the parent groups (using the SubFind terminology). As a result, it may be used alongside a
+parent group catalogue. The *pynbody* reader can present a unified interface to the combined hierarchy, presenting
+groups from the parent catalogue as the top-level objects, with the HBT+ halos as children of these groups, and
+HBT+ subhalos as children of the HBT+ halos.
+
+For example:
+
+.. ipython::
+
+  In [1]: import pynbody
+
+  In [2]: s = pynbody.load('testdata/gadget4_subfind_HBT/snapshot_034.hdf5')
+
+  In [3]: hbtplus_halos = s.halos(priority=["HBTPlusCatalogue"])
+
+  In [4]: subfind_groups = s.halos(priority=["Gadget4SubfindHDFCatalogue"])
+
+  In [5]: combined_catalogue = hbtplus_halos.with_groups_from(subfind_groups)
+
+  In [6]: combined_catalogue[0]
+  Out[6]: <SimSnap "testdata/gadget4_subfind_HBT/snapshot_034.hdf5:halo_0" len=307386>
+
+We can tell that this is actually a SubFind group by inspecting its properties:
+
+.. ipython::
+
+  In [7]: combined_catalogue[0].properties['GroupMass'] # <-- a SubFind property
+  Out[7]: Unit("7.80e+44 g h**-1")
+
+  In [8]: subfind_groups[0].properties['GroupMass'] # <-- the same property accessed directly from SubFind
+  Out[8]: Unit("7.80e+44 g h**-1")
+
+The ``subhalos`` attribute of each halo in the ``combined_catalogue`` will return the HBT+ subhalos that are children of
+the corresponding SubFind group:
+
+.. ipython::
+
+  In [14]: combined_catalogue[0].subhalos[0].properties['TrackId'] # <-- an HBT+ property
+  Out[14]: 54
+
+Naturally, not only the properties but the particle information is available in the combined catalogue.
+
+
+"""
 from __future__ import annotations
 
 import pathlib
 import re
 
 import h5py
 import numpy as np
 from numpy.typing import NDArray
 
 from . import HaloCatalogue, HaloParticleIndices
 from .details import number_mapping
 
 
 class HBTPlusCatalogue(HaloCatalogue):
-    def __init__(self, sim, halo_numbers=None, hbt_filename=None):
+    """A class to represent a HBT+ halo catalogue."""
+    def __init__(self, sim, halo_numbers=None, filename=None):
         """Initialize a HBTPlusCatalogue object.
 
         Parameters
         ----------
         sim : SimSnap
             The simulation snapshot to which this catalogue applies.
+
         halo_numbers : str, optional
             How to number the halos. If None (default), use a zero-based indexing.
-            If 'track', use the TrackId from the catalogue.
-            If 'length-order', order by Nbound (descending), similar to the AHF option of the same name
-        hbt_filename : str, optional
-            The filename of the HBTPlus catalogue. If None (default), attempt to find
-            the file automatically.
+
+            * If ``track``, use the TrackId from the catalogue.
+            * If ``length-order``, order by Nbound (descending), similar to the AHF option of the same name.
+
+        filename : str, optional
+            The filename of the HBTPlus catalogue. If the file is spanned across multiple outputs (e.g.
+            ``path/to/SubSnap_034.0.hdf5``, ``SubSnap_034.1.hdf5``, etc.), pass the filename of the first file or
+            the common prefix (``path/to/SubSnap_034``). If None (default), attempt to find the file automatically.
         """
-        if hbt_filename is None:
-            hbt_filename = self._infer_hbt_filename(sim)
+        if filename is None:
+            filename = self._infer_hbt_filename(sim)
+        else:
+            filename = self._map_user_filename_to_file_0(filename)
 
-        self._file = h5py.File(hbt_filename, 'r')
+        self._file = h5py.File(filename, 'r')
 
         num_halos = int(self._file["NumberOfSubhalosInAllFiles"][0])
         if int(self._file["NumberOfFiles"][0])>1:
             from ..util import hdf_vds
-            hbt_filename = str(hbt_filename)[:-7]
-            all_files = [f"{hbt_filename}.{num}.hdf5" for num in range(int(self._file["NumberOfFiles"][0]))]
+            filename = str(filename)[:-7]
+            all_files = [f"{filename}.{num}.hdf5" for num in range(int(self._file["NumberOfFiles"][0]))]
             maker = hdf_vds.HdfVdsMaker(all_files)
             self._file = maker.get_temporary_hdf_vfile()
 
         self._trackid_number_mapper = number_mapping.create_halo_number_mapper(self._file["Subhalos"]["TrackId"])
 
         if halo_numbers is None:
             number_mapper = number_mapping.SimpleHaloNumberMapper(0, num_halos)
@@ -125,24 +183,24 @@
             end = start + len(halo_parts)
             indices[start:end] = np.sort(self._iord_to_fpos.map_ignoring_order(halo_parts))
             boundaries[i] = (start,end)
             start = end
         return indices, boundaries
 
     def with_groups_from(self, other: HaloCatalogue) -> HaloCatalogue:
-        """HBT+ identifies halos, not the parent groups (using the SubFind terminology).
-
-        If you can load the original group catalogue from which HBT+ was run, this comines the two catalogues into one
-        single expression of the hierarchy, with the original group catalogue as the parent groups.
+        """Return a new catalogue that combines an HBT+ halo catalogue with a parent group catalogue.
 
         For example:
+
         >>> grps = hbt_cat.with_groups_from(subfind_cat)
         >>> grps[0] # -> returns subfind_cat[0]
         >>> grps[0].properties['children'] # -> returns relevant halo numbers in hbt_cat
         >>> grps[0].subhalos # -> returns HBT+ subhalos that are children of subfind_cat[0]
+
+        See also :ref:`hbt_plus_parent_groups`.
         """
         return HBTPlusCatalogueWithGroups(self, other)
 
     def get_properties_one_halo(self, halo_number) -> dict:
         index = self.number_mapper.number_to_index(halo_number)
         result = {}
         for k in self._file["Subhalos"].dtype.names:
@@ -161,29 +219,36 @@
 
     def _get_children_one_halo(self, index) -> NDArray[int]:
         return self._map_trackid_to_pynbody_number(self._file["NestedSubhalos"][index])
 
 
 
     @classmethod
-    def _can_load(cls, sim, halo_numbers=None, hbt_filename=None):
+    def _can_load(cls, sim, halo_numbers=None, filename=None):
+        if filename is not None:
+            filename = cls._map_user_filename_to_file_0(filename)
         try:
-            hbt_filename = hbt_filename or cls._infer_hbt_filename(sim)
+            hbt_filename = filename or cls._infer_hbt_filename(sim)
             if h5py.is_hdf5(hbt_filename):
                 with h5py.File(hbt_filename, 'r') as f:
                     if "NumberOfFiles" in f:
                         return True
         except OSError:
             pass
         return False
 
 
 
 
 class HBTPlusCatalogueWithGroups(HaloCatalogue):
+    """A class to represent a HBT+ halo catalogue with parent groups from another finder.
+
+    For more information about parent groups, see :ref:`hbt_plus_parent_groups`.
+    """
+
     def __init__(self, hbt_cat: HBTPlusCatalogue, group_cat: HaloCatalogue):
         if hbt_cat.base is not group_cat.base:
             raise ValueError("The two catalogues must have the same base simulation snapshot")
         if not isinstance(hbt_cat, HBTPlusCatalogue):
             raise ValueError("The first catalogue must be a HBTPlusCatalogue")
 
         self._hbt_cat = hbt_cat
```

### Comparing `pynbody-2.0.0b7/pynbody/halo/hop.py` & `pynbody-2.0.0b8/pynbody/halo/hop.py`

 * *Files 26% similar despite different names*

```diff
@@ -4,49 +4,79 @@
 
 import numpy as np
 
 from .number_array import HaloNumberCatalogue
 
 
 class HOPCatalogue(HaloNumberCatalogue):
-    """A HOP Catalogue as used by Ramses. HOP output files must be in simulation directory, in simulation/hop/ directory
-    or specified by fname"""
-    def __init__(self, sim, fname=None):
-        if fname is None:
-            for fname in HOPCatalogue._enumerate_hop_tag_locations_from_sim(sim):
-                if os.path.exists(fname):
+    """Represents a HOP Catalogue as used by Ramses."""
+
+    dtype = np.int32
+
+    def __init__(self, sim, filename=None):
+        """Create a new HOP catalogue object from the given simulation object.
+
+        Parameters
+        ----------
+
+        sim : :class:`pynbody.snapshot.SimSnap`
+            The simulation snapshot to which this catalogue applies.
+
+        filename : str, optional
+            The filename of the HOP catalogue. The filename should be either the ``grp*.tag`` file or the
+            ``hop*.hop`` file that HOP produces. If no filename is provided, the code will attempt to find a
+            suitable ``grp*.tag`` file in the Ramses output folder, in the folder in which the simulation is
+            located, or in a ``hop`` subfolder.
+
+        """
+
+        if filename is None:
+            for filename in HOPCatalogue._enumerate_hop_tag_locations_from_sim(sim):
+                if os.path.exists(filename):
                     break
 
-            if not os.path.exists(fname):
+            if not os.path.exists(filename):
                 raise RuntimeError("Unable to find HOP .tag file in simulation directory")
 
-        sim._create_array('hop_grp', dtype=np.int32)
+        sim._create_array('hop_grp', dtype=self.dtype)
         sim['hop_grp'] = -1
-        with open(fname, "rb") as f:
-            num_part, = struct.unpack('i', f.read(4))
-            if num_part == 8:
-                # fortran-formatted output
-                num_part, num_grps, _, _ = struct.unpack('iiii', f.read(16))
-            else:
-                # plain binary output
-                num_grps, = struct.unpack('i', f.read(4))
+        with open(filename, "rb") as f:
+            num_part = self._get_npart_from_file(f)
 
             if num_part != len(sim.dm):
                 raise RuntimeError("Mismatching number of particles between "
                                    "snapshot %s and HOP file %s. Check your pynbody configuration for any missing"
-                                   " particle fields or partial loading" % (sim.filename, fname))
+                                   " particle fields or partial loading" % (sim.filename, filename))
 
-            sim.dm['hop_grp'] = np.fromfile(f, np.int32, len(sim.dm))
+            sim.dm['hop_grp'] = np.fromfile(f, self.dtype, len(sim.dm))
         super().__init__(sim, array="hop_grp", ignore=-1)
 
     @classmethod
-    def _can_load(cls, sim, arr_name='grp'):
+    def _get_npart_from_file(cls, f):
+        num_part, = struct.unpack('i', f.read(4))
+        if num_part == 8:
+            # fortran-formatted output
+            num_part, num_grps, _, _ = struct.unpack('iiii', f.read(16))
+        else:
+            # plain binary output
+            num_grps, = struct.unpack('i', f.read(4))
+        return num_part
+
+    @classmethod
+    def _can_load(cls, sim, filename=None):
         # Hop output must be in output directory or in output_*/hop directory
-        exists = any([os.path.exists(fname) for fname in HOPCatalogue._enumerate_hop_tag_locations_from_sim(sim)])
-        return exists
+        if filename is not None:
+            if not os.path.exists(filename):
+                return False
+            with open(filename, "rb") as f:
+                num_part = cls._get_npart_from_file(f)
+            return num_part == len(sim.dm)
+        else:
+            exists = any([os.path.exists(fname) for fname in HOPCatalogue._enumerate_hop_tag_locations_from_sim(sim)])
+            return exists
 
     @staticmethod
     def _extract_hop_name_from_sim(sim):
         match = re.search("output_([0-9]*)", sim.filename)
         if match is None:
             raise OSError("Cannot guess the HOP catalogue filename for %s" % sim.filename)
         return "grp%s.tag" % match.group(1)
```

### Comparing `pynbody-2.0.0b7/pynbody/halo/number_array.py` & `pynbody-2.0.0b8/pynbody/halo/number_array.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+"""Support for generic halo catalogues based on an array of halo numbers for each particle."""
+
 import numpy as np
 
 from . import HaloCatalogue
 from .details.number_mapping import create_halo_number_mapper
 from .details.particle_indices import HaloParticleIndices
 
 
@@ -58,19 +60,25 @@
         if len(array) == 0:
             self._no_such_halo(halo_number)
         return array
 
     def _no_such_halo(self, i):
         raise KeyError(f"No such halo {i}")
 
-    def get_group_array(self, family=None):
+    def get_group_array(self, family=None, use_index=False):
         if family is not None:
-            return self.base[family][self._array]
+            result = self.base[family][self._array]
+        else:
+            result = self.base[self._array]
+
+        if use_index:
+            return self.number_mapper.number_to_index(result)
         else:
-            return self.base[self._array]
+            return result
+
 
     @classmethod
     def _can_load(cls, sim, arr_name='grp'):
         if (arr_name in sim.loadable_keys()) or (arr_name in list(sim.keys())) :
             return True
         else:
             return False
```

### Comparing `pynbody-2.0.0b7/pynbody/halo/rockstar.py` & `pynbody-2.0.0b8/pynbody/halo/rockstar.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+"""Support for the Rockstar halo finder"""
+
+from __future__ import annotations
+
 import glob
 import os.path
 import sys
 
 import numpy as np
 
 from .. import util
@@ -10,48 +14,43 @@
 
 
 class RockstarFormatRevisionError(RuntimeError):
     pass
 
 
 class RockstarCatalogue(HaloCatalogue):
-    def __init__(self, sim, dummy=False, pathname=None, format_revision=None,
-                 filenames=None, sort=False, **kwargs):
+    def __init__(self, sim, filename=None, format_revision=None):
         """Initialize a RockstarCatalogue.
 
-        **kwargs** :
-
-
-        *dummy*: if True, the particle file is not loaded, and all
-                 halos returned are just dummies (with the correct
-                 properties dictionary loaded). Use load_copy to get
-                 the actual data in this case.
+        Parameters
+        ----------
 
-        *sort*: if True, resort the halos into descending order of
-                particle number. Otherwise, leave in RockStar output order.
+        sim : :class:`pynbody.snapshot.simsnap.SimSnap`
+            The simulation snapshot to which this catalogue applies.
 
-        *filenames*: a list of filenames of each of the RockStar outputs.
-                     You probably want to use pathname instead, which specifies
-                     the path to the output folder.
-
-        *pathname*: the path of the output folder with the individual RockStar outputs
-
-        *format_revision*: Override the header's format revision information. Specify
-                    1, 2, 'caterpillar', 'galaxies' for Rockstar prior to 2014, post 2014,
-                    customized for the caterpillar project and for rockstar
-                    galaxies respectively
+        filename : str, optional
+            The path to the Rockstar outputs. This can either be the first binary file in the series (e.g.
+            ``path/to/halos_15.0.bin``) or the stem for the series (e.g. ``path/to/halos_15``). If not specified,
+            the code will attempt to find the Rockstar outputs in the same directory as the simulation snapshot.
+
+        format_revision : int, str, optional
+            Override the header's format revision information. Specify 1, 2, 'caterpillar', 'galaxies' for Rockstar
+            prior to 2014, post 2014, customized for the caterpillar project and for rockstar galaxies respectively.
+            If not specified, the code will attempt to detect the format revision automatically.
 
         """
 
-        if filenames is not None:
-            self._files = filenames
+        if filename is not None:
+            filestem = str(filename)
+            if filestem.endswith(".0.bin"):
+                filestem = filestem[:-6]
+            self._files = glob.glob(filestem + "*.bin") + glob.glob(filestem + "*.boundbin")
         else:
-            if pathname is None:
-                pathname = os.path.dirname(sim.filename)
-            self._files = glob.glob(os.path.join(pathname,'halos*.bin'))
+            pathname = os.path.dirname(sim.filename)
+            self._files = glob.glob(os.path.join(pathname, 'halos*.bin'))
             if len(self._files)==0 :
                 self._files = glob.glob(os.path.join(pathname, 'halos*.boundbin'))
             self._files.sort()
 
         if len(self._files)==0:
             raise OSError("Could not find any Rockstar output. Try specifying pathname='/path/to/rockstar/outputfolder'")
 
@@ -127,18 +126,26 @@
                     props[k] = np.concatenate((props[k], v))
                 else:
                     props[k] = v
 
         return props
 
     @classmethod
-    def _can_load(cls, sim, **kwargs):
-        return len(
-            glob.glob(os.path.join(os.path.dirname(sim.filename), 'halos*.bin'))
-        ) > 0
+    def _can_load(cls, sim, filename=None, format_revision=None):
+        if filename is None:
+            return len(
+                glob.glob(os.path.join(os.path.dirname(sim.filename), 'halos*.bin'))
+            ) > 0
+        else:
+            if str(filename).endswith(".0.bin") and os.path.exists(filename):
+                return True
+            if os.path.exists(str(filename)+".0.bin"):
+                return True
+            return False
+
 
 
 class _RockstarCatalogueOneCpu:
     """
     Low-level reader for single CPU output from Rockstar. Users should normally not use this class,
     rather using RockstarCatalogue which collates the multiple sub-files that Rockstar produces.
     """
```

### Comparing `pynbody-2.0.0b7/pynbody/halo/subfind.py` & `pynbody-2.0.0b8/pynbody/halo/subfind.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,80 +1,107 @@
+"""Support for the SubFind halo finder"""
+
+from __future__ import annotations
+
 import os.path
 import warnings
-import weakref
 
 import numpy as np
 
 from .. import units
 from ..array import SimArray
 from . import HaloCatalogue
 from .details import number_mapping, particle_indices
 from .subhalo_catalogue import SubhaloCatalogue
 
 
 class SubfindCatalogue(HaloCatalogue):
-    """Class to handle catalogues produced by the SubFind halo finder."""
+    """Handles catalogues produced by the SubFind halo finder (old versions that do not use HDF5 outputs)."""
 
-
-    def __init__(self, sim, subs=False, ordered=None, _inherit_data_from=None):
+    def __init__(self, sim, filename=None, subs=None, subhalos=False,  ordered=None, _inherit_data_from=None):
         """Initialise a SubFind catalogue
 
         By default, the FoF groups are imported, and subhalos are available via the 'subhalos' attribute of each
         halo object, e.g.
 
         >>> f = pynbody.load('path/to/snapshot')
         >>> h = f.halos()
         >>> h[1].subhalos[2] # returns the third subhalo of FoF group 1
 
-        However by setting subs=True, the FoF groups are ignored and the catalogue is of all subhalos.
+        However by setting ``subs=True``, the FoF groups are ignored and the catalogue is of all subhalos.
+
+        Parameters
+        ----------
+
+        sim : ~pynbody.snapshot.simsnap.SimSnap
+            The simulation snapshot to which this catalogue applies.
+
+        filename : str, optional
+            The path to the SubFind output(s). This is expected to be a folder named ``groups_XXX`` where XXX is the
+            snapshot number. The code extracts the snapshot number from the folder name and uses it to construct
+            the filename of the catalogue files, for example ``groups_XXX/subhalo_tab_XXX.0``. If no filename is
+            provided, the code will attempt to find a suitable catalogue starting from the simulation's directory.
+
+        subhalos : bool, optional
+            If False (default), catalogue represents the FoF groups and subhalos are available through the
+            :meth:`~pynbody.halo.Halo.subhalos` attribute of each group (see note above). If True, the catalogue
+            represents the subhalos directly and FoF groups are not available.
+
+        ordered : bool, optional
+            If True, the snapshot must have sequential iords. If False, the iords might be out-of-sequence, and
+            therefore reordering will take place. If None (default), the iords are examined to check whether
+            re-ordering is required or not. Note that re-ordering can be undesirable because it also destroys
+            subfind's order-by-binding-energy
+
+        _inherit_data_from : SubfindCatalogue, optional
+            For internal use only; allows subhalo catalogue to share data with its parent FOF catalogue
 
-        **kwargs** :
 
-        *subs*: if True, load the subhalos; otherwise, load FoF groups (default)
-        *ordered*: if True, the snapshot must have sequential iords. If False, the iords might be out-of-sequence, and
-                 therefore reordering will take place. If None (default), the iords are examined to check whether
-                 re-ordering is required or not. Note that re-ordering can be undesirable because it also destroys
-                 subfind's order-by-binding-energy
-        *_inherit_data_from*: for internal use only, allows subhalo catalogue to share data with its parent FOF catalogue
         """
 
-        self._subs=subs
+        if subs is not None:
+            warnings.warn("The 'subs' argument to SubfindCatalogue is deprecated; use 'subhalos' instead",
+                          DeprecationWarning)
+            subhalos = subs
+
+        self._subs=subhalos
 
         if ordered is not None:
             self._ordered = ordered
         else:
             self._ordered = bool((sim['iord']==np.arange(len(sim))).all())
 
         self._halos = {}
 
         self.dtype_int = sim['iord'].dtype
         self.dtype_flt = 'float32' #SUBFIND data is apparently always single precision???
-        self._subfind_dir = self._name_of_catalogue(sim)
+        self._subfind_dir = filename or self._name_of_catalogue(sim)
 
         self.header = self._read_header()
         self._tasks = self.header[4]
 
         if _inherit_data_from:
             self._inherit_data(_inherit_data_from)
         else:
             self._read_data(sim)
 
 
 
-        if subs:
+        if subhalos:
             if self.header[6]==0:
                 raise ValueError("This file does not contain subhalos")
             length = len(self._subhalodat['sub_off'])
         else:
             length = len(self._halodat['group_off'])
 
         super().__init__(sim, number_mapping.SimpleHaloNumberMapper(0, length))
 
-        if not subs:
-            self._subhalo_catalogue = SubfindCatalogue(sim, subs=True, ordered=self._ordered, _inherit_data_from=self)
+        if not subhalos:
+            self._subhalo_catalogue = SubfindCatalogue(sim, subhalos=True, filename=filename,
+                                                       ordered=self._ordered, _inherit_data_from=self)
 
     def _inherit_data(self, from_):
         inherit = ['_halodat', '_subhalodat', '_keys_halo', '_keys_subhalo']
         for k in inherit:
             setattr(self, k, getattr(from_, k))
 
     def _get_all_particle_indices(self):
@@ -297,19 +324,22 @@
         # alternative path if snapshot is single file
         else:
             snapnum = os.path.basename(sim.filename).split("_")[-1]
             parent_dir = os.path.dirname(sim.filename)
             return os.path.join(parent_dir,"groups_" + snapnum)
 
     @staticmethod
-    def _can_load(sim, **kwargs):
+    def _can_load(sim, filename=None, **kwargs):
+        if filename is not None:
+            if str(filename)[:-3].endswith("groups_"):
+                return True
         file = SubfindCatalogue._name_of_catalogue(sim)
         if os.path.exists(file):
             if os.path.exists(file):
                 if file.endswith(".hdf5"):
                     return False
-                elif os.listdir(file)[0].endswith(".hdf5"):
+                elif os.path.isdir(file) and os.listdir(file)[0].endswith(".hdf5"):
                     return False
                 else:
                     return True
         else:
             return False
```

### Comparing `pynbody-2.0.0b7/pynbody/halo/subfindhdf.py` & `pynbody-2.0.0b8/pynbody/halo/subfindhdf.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,99 +1,41 @@
+"""Support for the SubFind halo finder, in the HDF5 format used by Gadget3, 4 and Arepo."""
+
+from __future__ import annotations
+
 import os.path
 import warnings
 
+import h5py
 import numpy as np
 
 from .. import array, config_parser, snapshot, units
 from ..snapshot import gadgethdf
 from . import Halo, HaloCatalogue
+from .details import number_mapping, particle_indices
+from .subhalo_catalogue import SubhaloCatalogue
 
 
-class SubFindHDFSubhaloCatalogue(HaloCatalogue) :
-    """
-    Gadget's SubFind HDF Subhalo catalogue.
-
-    Initialized with the parent FOF group catalogue and created
-    automatically when an fof group is created
-    """
-
-    def __init__(self, group_id, group_catalogue) :
-        super().__init__(group_catalogue.base)
-
-        self._group_id = group_id
-        self._group_catalogue = group_catalogue
-        self.__calc_len()
-
-    def __calc_len(self):
-        next_group_id = self._group_id + 1
-        next_first_subhalo = self._group_catalogue.nsubhalos
-        while next_group_id < len(self._group_catalogue._fof_group_first_subhalo)-1:
-            if self._group_catalogue._fof_group_first_subhalo[self._group_id + 1]!=-1:
-                next_first_subhalo = self._group_catalogue._fof_group_first_subhalo[next_group_id]
-                break
-            next_group_id+=1
-
-
-        self._len = (next_first_subhalo - self._group_catalogue._fof_group_first_subhalo[self._group_id])
-
-    def __len__(self):
-        return self._len
-
-    def _get_halo(self, halo_number):
-        if self.base is None :
-            raise RuntimeError("Parent SimSnap has been deleted")
-
-        if halo_number > len(self)-1 :
-            raise ValueError("FOF group %d does not have subhalo %d" % (self._group_id, halo_number))
-
-        # need this to index the global offset and length arrays
-        absolute_id = self._group_catalogue._fof_group_first_subhalo[self._group_id] + halo_number
-
-        # now form the particle IDs needed for this subhalo
-        type_map = self.base._family_to_group_map
-
-        halo_lengths = self._group_catalogue._subfind_halo_lengths
-        halo_offsets = self._group_catalogue._subfind_halo_offsets
-
-        # create the particle lists
-        tot_len = 0
-        for g_ptypes in list(type_map.values()) :
-            for g_ptype in g_ptypes:
-                tot_len += halo_lengths[g_ptype][absolute_id]
-
-        plist = np.zeros(tot_len,dtype='int64')
-
-        npart = 0
-        for ptype in self.base._families_ordered():
-            # family slice in the SubFindHDFSnap
-            sl = self.base._family_slice[ptype]
-
-            for g_ptype in type_map[ptype]:
-                # add the particle indices to the particle list
-                offset = halo_offsets[g_ptype][absolute_id]
-                length = halo_lengths[g_ptype][absolute_id]
-                ind = np.arange(sl.start + offset, sl.start + offset + length)
-                plist[npart:npart+length] = ind
-                npart += length
+class SubFindHDFHaloCatalogue(HaloCatalogue) :
+    """Handles catalogues produced by the SubFind halo finder, in the HDF5 format used by Gadget3, 4 and Arepo.
 
-        return SubFindHDFSubHalo(halo_number, self._group_id, self._group_catalogue, self, self.base, plist)
+    Since the internal format differs quite substantially between these versions, child classes are provided for
+    Gadget 4, Arepo and TNG. The base class is able to handle the common elements of the format, and is also used
+    for Gadget 3 SubFind outputs.
 
+    See :class:`Gadget4SubfindHDFCatalogue`, :class:`ArepoSubfindHDFCatalogue` and :class:`TNGSubfindHDFCatalogue`.
 
-    @property
-    def base(self) :
-        return self._base()
-from .details import number_mapping, particle_indices
-from .subhalo_catalogue import SubhaloCatalogue
+    .. warning::
 
+        At present, the Gadget 4, Arepo and TNG subclasses of this class are not tested against multi-file
+        outputs. If you encounter issues with these, please report them to the pynbody developers.
 
-class SubFindHDFHaloCatalogue(HaloCatalogue) :
-    """Halo or group catalogue generated from subfind information stored inside a GadgetHDF snapshot
     """
 
-    # Names of various groups and attributes in the hdf file (which vary in different versions of SubFind?)
+    # Names of various groups and attributes in the hdf file (which vary in different versions of SubFind)
 
     _fof_name = 'FOF'
     _header_name = 'FOF'
     _subfind_name = 'SUBFIND'
     _subfind_grnr_name = 'GrNr'
     _subfind_first_gr_name = 'SUBFIND/FirstSubOfHalo'
 
@@ -102,59 +44,97 @@
 
     _grp_offset_name = 'Offset'
     _grp_len_name = 'Length'
 
     _sub_offset_name = 'SUB_Offset'
     _sub_len_name = 'SUB_Length'
 
-    def __init__(self, sim, subs=False, _inherit_data_from=None) :
-        """Initialise a Subfind catalogue.
+    def __init__(self, sim, filename=None, subs=None, subhalos=False, _inherit_data_from=None) :
+        """Initialise a SubFindHDF catalogue.
 
         By default, the FoF groups are imported, and subhalos are available via the 'subhalos' attribute of each
         halo object, e.g.
 
         >>> f = pynbody.load('path/to/snapshot.hdf5')
         >>> h = f.halos()
         >>> h[1].subhalos[2] # returns the third subhalo of FoF group 1
 
-        *sim*: The SimSnap
-        *subs*: If True, enumerate the subhalos instead of the groups. Otherwise, the jth subhalo of FOF group i
-        is still available, as halo_cat[i].subhalos[j].
-        *_inherit_data_from*: for internal use only, allows subhalo catalogue to share data with its parent FOF catalogue
+        However by setting ``subhalos=True``, the FoF groups are ignored and the catalogue is of all subhalos.
+
+        .. note::
+
+            Note that this constructor is common between :class:`SubFindHDFHaloCatalogue` and its subclasses
+            :class:`Gadget4SubfindHDFCatalogue`, :class:`ArepoSubfindHDFCatalogue` and
+            :class:`TNGSubfindHDFCatalogue`.
+
+            For Gadget 3 outputs, the SubFind data is stored internally to the snapshot itself. Therefore
+            passing a *filename* to the constructor for :class:`SubFindHDFHaloCatalogue` will result in an exception.
+            For Gadget 4, Arepo and TNG SubFind outputs, a filename can be passed that points to the
+            ``fof_subhalo_tab_XXX.hdf5`` file (see below).
+
+
+        Parameters
+        ----------
+
+        sim : ~pynbody.snapshot.simsnap.SimSnap
+            The simulation snapshot to which this catalogue applies.
+
+        filename : str, optional
+            The filename of the HDF5 file containing the SubFind catalogue. This is only used for Gadget 4, Arepo and
+            TNG subclasses and **must** be None when used with the Gadget 3 base class. See the note above.
+
+        subhalos : bool, optional
+            If False (default), catalogue represents the FoF groups and subhalos are available through the
+            :meth:`~pynbody.halo.Halo.subhalos` attribute of each group (see note above). If True, the catalogue
+            represents the subhalos directly and FoF groups are not available.
+
+        subs : bool, optional
+            Deprecated alias for ``subhalos``.
+
+        _inherit_data_from : SubfindCatalogue, optional
+            For internal use only; allows subhalo catalogue to share data with its parent FOF catalogue
         """
 
-        self._sub_mode = subs
-        self._hdf_files = self._get_catalogue_multifile(sim)
+        if subs is not None:
+            warnings.warn("The 'subs' argument to SubFindHDFHaloCatalogue is deprecated. Use 'subhalos' instead.",
+                          DeprecationWarning)
+            subhalos = subs
+
+        self._sub_mode = subhalos
+        self._hdf_files = self._get_catalogue_multifile(sim, user_provided_filename=filename)
 
         super().__init__(sim, number_mapping.SimpleHaloNumberMapper(0, self.__get_length()))
 
         if _inherit_data_from:
             self.__inherit_data(_inherit_data_from)
         else:
             self.__init_halo_offset_data()
             self.__init_subhalo_relationships()
             self.__init_halo_properties()
             self.__reshape_multidimensional_properties()
             self.__reassign_properties_from_sub_to_fof()
 
-        if not subs:
-            self._subhalo_catalogue = type(self)(sim, subs=True, _inherit_data_from=self)
+        if not subhalos:
+            self._subhalo_catalogue = type(self)(sim, subhalos=True, filename=filename, _inherit_data_from=self)
 
     def __inherit_data(self, parent):
         attrs_to_share = ["_fof_properties", "_sub_properties", "_fof_group_offsets", "_fof_group_lengths",
                          "_subfind_halo_offsets", "_subfind_halo_lengths",
                           "fof_ignore", "sub_ignore","_subfind_halo_parent_groups"]
         for attr in attrs_to_share:
             setattr(self, attr, getattr(parent, attr))
 
 
-    def _get_catalogue_multifile(self, sim):
+    def _get_catalogue_multifile(self, sim, user_provided_filename):
         """Some variants of Subfind put all the particle data in the catalogue files, in which case the catalogue
         HDF files are already present in the base simulation. In other cases, notably Gadget4/Arepo, this must be
         overridden to locate the actual HDF5 files for the catalogue"""
+        if user_provided_filename is not None:
+            raise ValueError("Filename must be None for loading a Gadget3-style SubFindHDFCatalogue")
+
         if not isinstance(sim, gadgethdf.SubFindHDFSnap):
             raise ValueError("SubFindHDFHaloCatalogue can only work with a SubFindHDFSnap simulation")
 
         return sim._hdf_files
 
     def __init_ignorable_keys(self):
         self.fof_ignore = list(map(str.strip,config_parser.get("SubfindHDF","FoF-ignore").split(",")))
@@ -435,68 +415,29 @@
         if not self._sub_mode:
             props = self.get_properties_one_halo(parent_halo_number)
             return SubhaloCatalogue(self._subhalo_catalogue, props['children'])
         else:
             return SubhaloCatalogue(self._subhalo_catalogue, [])
 
     @classmethod
-    def _can_load(cls, sim, subs=False):
+    def _can_load(cls, sim, **kwargs):
         if isinstance(sim, gadgethdf.SubFindHDFSnap):
             return True
         else:
             return False
 
-class SubFindFOFGroup(Halo) :
-    """
-    SubFind FOF group class
-    """
-
-    def __init__(self, group_id, *args) :
-        """Construct a special halo representing subfind's FOF group"""
-        super().__init__(group_id, *args)
-
-        self._subhalo_catalogue = SubFindHDFSubhaloCatalogue(group_id, self._halo_catalogue)
-
-        self._descriptor = "fof_group_"+str(group_id)
-
-        self.properties.update(self._halo_catalogue.get_halo_properties(group_id, subs=False))
+class Gadget4SubfindHDFCatalogue(SubFindHDFHaloCatalogue):
+    """Handles catalogues produced by the SubFind halo finder, in the HDF5 format used by Gadget 4
 
+    .. warning::
 
-    def __getattr__(self, name):
-        if name == 'sub':
-            return self._subhalo_catalogue
-        else :
-            return super().__getattr__(name)
+        At present, this is not tested against multi-file outputs. If you encounter issues with these, please report
+        them to the pynbody developers.
 
-class SubFindHDFSubHalo(Halo) :
     """
-    SubFind subhalo class
-    """
-
-    def __init__(self, halo_number, group_id, subfind_data_object, *args) :
-        """Construct a special halo representing subfind's subhalo
-
-        *halo_id*: The halo_id, where 0 is the first halo within the specified group
-        *group_id*: The group across the entire snapshot
-        *subfind_data_object*: The object which actually holds the HDF data
-
-        Other arguments get passed to the standard halo constructor
-        """
-        super().__init__(halo_number, *args)
-        self._group_id = group_id
-        self._descriptor = "fof_group_%d_subhalo_%d"%(group_id, halo_number)
-
-        # need this to index the global offset and length arrays
-        absolute_id = subfind_data_object._fof_group_first_subhalo[self._group_id] + halo_number
-
-        # load properties
-        self.properties.update(subfind_data_object.get_halo_properties(absolute_id, subs=True))
-
-
-class Gadget4SubfindHDFCatalogue(SubFindHDFHaloCatalogue):
 
     _fof_name = 'Group'
     _subfind_name = 'Subhalo'
     _header_name = 'Header'
     _subfind_grnr_name = 'SubhaloGroupNr'
     _subfind_first_gr_name = 'Group/GroupFirstSub'
 
@@ -505,20 +446,20 @@
 
     _grp_offset_name = 'GroupOffsetType'
     _grp_len_name = 'GroupLenType'
 
     _sub_offset_name = 'SubhaloOffsetType'
     _sub_len_name = 'SubhaloLenType'
 
-    def __init__(self, sim, **kwargs):
-        super().__init__(sim, **kwargs)
+    def __init__(self, sim, filename=None, **kwargs):
+        super().__init__(sim, filename, **kwargs)
         i = 0
         for prog_or_desc in "prog", "desc":
             try:
-                files = self._get_progenitor_or_descendant_multifile(sim, prog_or_desc)
+                files = self._get_progenitor_or_descendant_multifile(sim, prog_or_desc, filename)
             except FileNotFoundError:
                 continue
             props = self._get_properties_from_multifile(files, 'Subhalo')
             self._sub_properties.update(props)
 
     def _get_halodata_array(self, hdf_file, array_name, halo_or_group, particle_type):
         return hdf_file[halo_or_group][array_name][:,int(particle_type[-1])]
@@ -537,51 +478,72 @@
             return None
 
         return self.base.infer_original_units(dimensions)
 
 
 
     @classmethod
-    def _get_catalogue_multifile(cls, sim):
-        class Gadget4SubfindHdfMultiFileManager(gadgethdf.SubfindHdfMultiFileManager):
+    def _get_catalogue_multifile(cls, sim, user_provided_filename):
+        class Gadget4SubfindHdfMultiFileManager(gadgethdf._SubfindHdfMultiFileManager):
             _nfiles_groupname = cls._fof_name
             _nfiles_attrname = "NTask"
             _subgroup_name = None
 
-        return Gadget4SubfindHdfMultiFileManager(cls._catalogue_filename(sim))
+        return Gadget4SubfindHdfMultiFileManager(cls._catalogue_filename(sim, user_provided_filename))
 
     @classmethod
-    def _get_progenitor_or_descendant_multifile(cls, sim, prog_or_desc):
-        class Gadget4SubfindHdfProgenitorsMultiFileManager(gadgethdf.SubfindHdfMultiFileManager):
+    def _get_progenitor_or_descendant_multifile(cls, sim, prog_or_desc, user_provided_filename):
+        class Gadget4SubfindHdfProgenitorsMultiFileManager(gadgethdf._SubfindHdfMultiFileManager):
             _nfiles_groupname = "Header"
             _nfiles_attrname = "NumFiles"
             _subgroup_name = None
 
-        return Gadget4SubfindHdfProgenitorsMultiFileManager(cls._catalogue_filename(sim, "subhalo_"+prog_or_desc+"_"))
+        return Gadget4SubfindHdfProgenitorsMultiFileManager(cls._catalogue_filename(sim, user_provided_filename,
+                                                                                    "subhalo_"+prog_or_desc+"_"))
 
     @classmethod
-    def _catalogue_filename(cls, sim, namestem ="fof_subhalo_tab_"):
+    def _catalogue_filename(cls, sim, user_provided_filename=None, namestem ="fof_subhalo_tab_"):
+        if user_provided_filename is not None:
+            user_provided_filename = str(user_provided_filename)
+            if "fof_subhalo_tab_" not in user_provided_filename:
+                raise ValueError("Filename must contain 'fof_subhalo_tab_'")
+            return user_provided_filename.replace("fof_subhalo_tab_", namestem)
+
         snapnum = os.path.basename(sim.filename).split("_")[-1]
         parent_dir = os.path.dirname(os.path.abspath(sim.filename))
         return os.path.join(parent_dir, namestem + snapnum)
 
+
     @classmethod
-    def _can_load(cls, sim, **kwargs):
-        file = cls._catalogue_filename(sim)
-        if os.path.exists(file) and (file.endswith(".hdf5") or os.listdir(file)[0].endswith(".hdf5")) \
-                or os.path.exists(file+".0.hdf5"):
-            # very hard to figure out whether it's the right sort of hdf5 file without just going ahead and loading it
-            try:
-                cls(sim, **kwargs)
-                return True
-            except:
+    def _can_load(cls, sim, filename=None, **kwargs):
+        try:
+            file = cls._catalogue_filename(sim, user_provided_filename=filename)
+        except ValueError:
+            return False
+        if not h5py.is_hdf5(file):
+            file = file + ".0.hdf5"
+            if not h5py.is_hdf5(file):
                 return False
+        with h5py.File(file, 'r') as f:
+            if cls._header_name not in f:
+                return False
+            if cls._numsubs_name not in f[cls._header_name].attrs:
+                return False
+        return True
 
 
 class ArepoSubfindHDFCatalogue(Gadget4SubfindHDFCatalogue):
+    """Handles catalogues produced by the SubFind halo finder, in the HDF5 format used by Arepo
+
+    .. warning::
+
+        At present, this is not tested against multi-file outputs. If you encounter issues with these, please report
+        them to the pynbody developers.
+
+    """
     _numsubs_name = 'Nsubgroups_Total'
 
     _subfind_grnr_name = 'SubhaloGrNr'
 
 
     def _get_halodata_array(self, hdf_file, array_name, halo_or_group, particle_type):
         if array_name.endswith("OffsetType"):
@@ -589,22 +551,32 @@
             # this doesn't exist in arepo
             lens = super()._get_halodata_array(hdf_file, len_array_name, halo_or_group, particle_type)
             return np.concatenate(([0],np.cumsum(lens)[:-1]))
         else:
             return super()._get_halodata_array(hdf_file, array_name, halo_or_group, particle_type)
 
 class TNGSubfindHDFCatalogue(ArepoSubfindHDFCatalogue):
+    """Handles catalogues produced by the SubFind halo finder, in the HDF5 format used by Arepo (TNG variant)
+
+    .. warning::
+
+        At present, this is not tested against multi-file outputs. If you encounter issues with these, please report
+        them to the pynbody developers.
+
+    """
     @classmethod
-    def _catalogue_filename(cls, sim, namestem ="fof_subhalo_tab_"):
+    def _catalogue_filename(cls, sim, user_provided_filename, namestem ="fof_subhalo_tab_"):
+        if user_provided_filename is not None:
+            return super()._catalogue_filename(sim, user_provided_filename, namestem)
         snapnum = os.path.basename(sim.filename).split("_")[-1]
         parent_dir = os.path.dirname(os.path.dirname(os.path.abspath(sim.filename)))
         f = os.path.join(parent_dir, "groups_"+snapnum, namestem + snapnum)
         return f
 
     @classmethod
-    def _get_catalogue_multifile(cls, sim):
-        class TNGSubfindHdfMultiFileManager(gadgethdf.SubfindHdfMultiFileManager):
+    def _get_catalogue_multifile(cls, sim, user_provided_filename):
+        class TNGSubfindHdfMultiFileManager(gadgethdf._SubfindHdfMultiFileManager):
             _nfiles_groupname = "Header"
             _nfiles_attrname = "NumFiles"
             _subgroup_name = None
 
-        return TNGSubfindHdfMultiFileManager(cls._catalogue_filename(sim))
+        return TNGSubfindHdfMultiFileManager(cls._catalogue_filename(sim, user_provided_filename))
```

### Comparing `pynbody-2.0.0b7/pynbody/halo/subhalo_catalogue.py` & `pynbody-2.0.0b8/pynbody/halo/subhalo_catalogue.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+"""Support for subhalo catalogues, which are effectively views on a parent halo catalogue"""
+
 import weakref
 
 from numpy.typing import NDArray
 
 from . import HaloCatalogue
 from .details import number_mapping
 
@@ -20,15 +22,15 @@
         if hc is None:
             raise ValueError("The underlying halo catalogue has been deleted")
         return hc
 
     def load_all(self):
         self._full_halo_catalogue.load_all()
 
-    def get_group_array(self, family=None):
+    def get_group_array(self, family=None, use_index=False):
         raise RuntimeError("It is not possible to retrieve the group array of a subhalo catalogue")
 
     def physical_units(self, distance='kpc', velocity='km s^-1', mass='Msol', persistent=True, convert_parent=False):
         self._full_halo_catalogue.physical_units(distance, velocity, mass, persistent, convert_parent)
 
     def _get_halo(self, i):
         return self._full_halo_catalogue._get_halo(self._subhalo_numbers[i])
```

### Comparing `pynbody-2.0.0b7/pynbody/halo/velociraptor.py` & `pynbody-2.0.0b8/pynbody/halo/velociraptor.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+"""Support for the Velociraptor halo finder."""
+
 from __future__ import annotations
 
 import functools
 import warnings
 from pathlib import Path
 from typing import Optional
 
@@ -11,16 +13,15 @@
 
 from .. import array, units, util
 from . import HaloCatalogue, HaloParticleIndices
 from .details import number_mapping
 
 
 class VelociraptorCatalogue(HaloCatalogue):
-    """
-    Velociraptor catalogue -- tested only with swift at present
+    """Handles catalogues produced by the velociraptor halo finder.
     """
 
     @classmethod
     def _catalogue_path(cls, sim) -> Path | None:
 
 
         simpath = Path(sim.filename)
@@ -57,21 +58,35 @@
 
         for suffix in ['.catalog_groups.0', '.catalog_particles.0', '.properties.0']:
             if not (path.with_suffix(suffix).is_file()):
                 return False
 
         return True
 
-    def __init__(self, sim, vr_basename=None, include_unbound=False):
+    def __init__(self, sim, filename=None, include_unbound=False):
+        """Create a new velociraptor catalogue object
+
+        Parameters
+        ----------
+        sim : pynbody.SimSnap
+            The simulation snapshot
+        filename : str, optional
+            The filename of the velociraptor catalogue. If not specified, the code will try to guess the filename.
+            Here, the filename is considered to be the stem; e.g. if your velociraptor files are called
+            ``folder/output.properties.0`, ``folder/output.catalog_groups.0``, etc., you should specify
+            ``filename='folder/output'``.
+        include_unbound : bool, optional
+            Whether to include unbound particles in the particle list. Default is False.
+        """
 
         self._include_unbound = include_unbound
-        if vr_basename is None:
+        if filename is None:
             self._path = self._catalogue_path(sim)
         else:
-            self._path = Path(vr_basename)
+            self._path = Path(filename)
 
         if self._path is None:
             raise OSError("Could not find velociraptor catalogue. Try specifying vr_basename='path/to/output', where the velociraptor outputs are output.properties.0 etc")
         self._grps = h5py.File(str(self._path.with_suffix('.catalog_groups.0')), 'r')
         self._part_ids = h5py.File(str(self._path.with_suffix('.catalog_particles.0')), 'r')
         self._properties_hdf_file = h5py.File(str(self._path.with_suffix('.properties.0')), 'r')
```

### Comparing `pynbody-2.0.0b7/pynbody/iter_subclasses.py` & `pynbody-2.0.0b8/pynbody/util/iter_subclasses.py`

 * *Files 8% similar despite different names*

```diff
@@ -5,14 +5,17 @@
 
 class IterableSubclasses:
     """A mixin for classes where we need to be able to iterate over their subclasses, possibly in a
     user-specified order. This is used by HaloCatalogue and SimSnap to find a suitable loader for
     a given file. """
     @classmethod
     def iter_subclasses(cls) -> Iterable[type]:
+        """Iterate over all subclasses of this class, recursively.
+
+        This is used by HaloCatalogue and SimSnap to find a suitable loader for a given file."""
         for c in cls.__subclasses__():
             yield from c.iter_subclasses()
             yield c
 
     @classmethod
     def iter_subclasses_with_priority(cls, priority: Iterable[str | type]) -> Iterable[type]:
         """Iterate over all subclasses, starting with the given priorities
```

### Comparing `pynbody-2.0.0b7/pynbody/kdtree/__init__.py` & `pynbody-2.0.0b8/pynbody/kdtree/__init__.py`

 * *Files identical despite different names*

### Comparing `pynbody-2.0.0b7/pynbody/kdtree/kd.cpp` & `pynbody-2.0.0b8/pynbody/kdtree/kd.cpp`

 * *Files identical despite different names*

### Comparing `pynbody-2.0.0b7/pynbody/kdtree/kd.h` & `pynbody-2.0.0b8/pynbody/kdtree/kd.h`

 * *Files identical despite different names*

### Comparing `pynbody-2.0.0b7/pynbody/kdtree/kdmain.cpp` & `pynbody-2.0.0b8/pynbody/kdtree/kdmain.cpp`

 * *Files identical despite different names*

### Comparing `pynbody-2.0.0b7/pynbody/kdtree/pq.h` & `pynbody-2.0.0b8/pynbody/kdtree/pq.h`

 * *Files identical despite different names*

### Comparing `pynbody-2.0.0b7/pynbody/kdtree/smooth.h` & `pynbody-2.0.0b8/pynbody/kdtree/smooth.h`

 * *Files identical despite different names*

### Comparing `pynbody-2.0.0b7/pynbody/plot/__init__.py` & `pynbody-2.0.0b8/pynbody/plot/__init__.py`

 * *Files identical despite different names*

### Comparing `pynbody-2.0.0b7/pynbody/plot/gas.py` & `pynbody-2.0.0b8/pynbody/plot/gas.py`

 * *Files identical despite different names*

### Comparing `pynbody-2.0.0b7/pynbody/plot/generic.py` & `pynbody-2.0.0b8/pynbody/plot/generic.py`

 * *Files 0% similar despite different names*

```diff
@@ -540,17 +540,15 @@
 
     if colorbar:
         cb = plt.colorbar(cs, format="%.2e").set_label(r'' + cb_label)
 
     if legend:
         plt.legend(loc=2)
 
-    if (filename):
-        if config['verbose']:
-            print("Saving " + filename)
+    if filename:
         plt.savefig(filename)
 
 
 def fourier_map(sim, nbins=100, nmin=1000, nphi=100, mmin=1, mmax=7, rmax=10,
                 levels=[.01, .05, .1, .2], subplot=None, ret=False, **kwargs):
     """
```

### Comparing `pynbody-2.0.0b7/pynbody/plot/metals.py` & `pynbody-2.0.0b8/pynbody/plot/metals.py`

 * *Files identical despite different names*

### Comparing `pynbody-2.0.0b7/pynbody/plot/profile.py` & `pynbody-2.0.0b8/pynbody/plot/profile.py`

 * *Files identical despite different names*

### Comparing `pynbody-2.0.0b7/pynbody/plot/stars.py` & `pynbody-2.0.0b8/pynbody/plot/stars.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,47 +1,45 @@
 """
-
-stars
-=====
+Routines for plots related to stellar particles
 
 """
 
 import logging
 import warnings
 
 import matplotlib
 import matplotlib.pyplot as plt
 import numpy as np
 
 from .. import array, filt, units, units as _units
 from ..analysis import angmom, profile
 from ..sph import Kernel2D, render_spherical_image
-from .sph import image
+from . import sph as plot_sph
 
 logger = logging.getLogger('pynbody.plot.stars')
 
 
-def bytscl(arr, mini=0, maxi=10000):
+def _bytscl(arr, mini=0, maxi=10000):
 	X = (arr - mini) / (maxi - mini)
 	X[X > 1] = 1
 	X[X < 0] = 0
 	return X
 
 
-def nw_scale_rgb(r, g, b, scales=[4, 3.2, 3.4]):
+def _nw_scale_rgb(r, g, b, scales=[4, 3.2, 3.4]):
 	return r * scales[0], g * scales[1], b * scales[2]
 
 
-def nw_arcsinh_fit(r, g, b, nonlinearity=3):
+def _nw_arcsinh_fit(r, g, b, nonlinearity=3):
 	radius = r + g + b
 	val = np.arcsinh(radius * nonlinearity) / nonlinearity / radius
 	return r * val, g * val, b * val
 
 
-def combine(r, g, b, magnitude_range, brightest_mag=None, mollview=False):
+def _combine(r, g, b, magnitude_range, brightest_mag=None, mollview=False):
 	# flip sign so that brightest pixels have biggest value
 	r = -r
 	g = -g
 	b = -b
 
 	if brightest_mag is None:
 		brightest_mag = []
@@ -56,168 +54,202 @@
 			brightest_mag.append(ordered[-len(ordered) // 5000])
 
 		brightest_mag = max(brightest_mag)
 	else:
 		brightest_mag = -brightest_mag
 
 	rgbim = np.zeros((r.shape[0], r.shape[1], 3))
-	rgbim[:, :, 0] = bytscl(r, brightest_mag - magnitude_range, brightest_mag)
-	rgbim[:, :, 1] = bytscl(g, brightest_mag - magnitude_range, brightest_mag)
-	rgbim[:, :, 2] = bytscl(b, brightest_mag - magnitude_range, brightest_mag)
+	rgbim[:, :, 0] = _bytscl(r, brightest_mag - magnitude_range, brightest_mag)
+	rgbim[:, :, 1] = _bytscl(g, brightest_mag - magnitude_range, brightest_mag)
+	rgbim[:, :, 2] = _bytscl(b, brightest_mag - magnitude_range, brightest_mag)
 	return rgbim, -brightest_mag
 
-def convert_to_mag_arcsec2(image, mollview=False):
+def _convert_to_mag_arcsec2(image, mollview=False):
 	if not mollview:
 		assert image.units=="pc^-2"
 	pc2_to_sqarcsec = 2.3504430539466191e-09
 	return -2.5*np.log10(image*pc2_to_sqarcsec)
 
-def render(sim, filename=None,
+def contour_surface_brightness(sim, band='v', width=50, resolution=None, axes=None, label=True,
+								contour_kwargs=None, smooth_min=0.0):
+	"""Plot surface brightness contours in the given band.
+
+	For information about how surface brightnesses are calculated, see the documentation for
+	:mod:`pynbody.analysis.luminosity`.
+
+	Parameters
+	----------
+
+	sim : SimSnap
+		The simulation snapshot to plot.
+
+	band : str
+		The band to plot. Default is 'v'.
+
+	width : float | str, optional
+		The width of the image to produce
+
+	resolution : int, optional
+		The resolution of the image to produce. The default is determined by the configuration
+		option ``image-default-resolution``.
+
+	axes : matplotlib axes object, optional
+		If not None, the axes object to plot to
+
+	label : bool, optional
+		If True, the contours are labelled with the surface brightness in mag arcsec^-2
+
+	contour_kwargs : dict or None, optional
+		Keyword arguments to pass to the matplotlib contour plot function. For example, this
+		can be used to determine the contour levels.
+
+	smooth_min : float or str, optional
+		The minimum size of the smoothing kernel, either as a float or a unit string.
+		Setting this to a non-zero value makes smoother, clearer contours but loses fine detail.
+		Default is 0.0.
+
+	"""
+
+	return plot_sph.contour(sim, qty=band + '_lum_den', units="pc^-2", width=width,
+							resolution=resolution, axes=axes, label=label, smooth_min=smooth_min,
+							_transform = _convert_to_mag_arcsec2,
+							log=False, contour_kwargs=contour_kwargs)
+
+
+
+def render(sim,
 		   r_band='i', g_band='v', b_band='u',
+		   width=50,
 		   r_scale=0.5, g_scale=1.0, b_scale=1.0,
+		   with_dust=False,
 		   dynamic_range=2.0,
 		   mag_range=None,
-		   width=50,
-		   resolution=500,
-		   starsize=None,
-		   plot=True, axes=None, ret_im=False, clear=True,
-		   ret_range=False, with_dust=False, z_range=50.0):
+		   resolution=None,
+		   noplot=False, axes=None, return_image=False, clear=True,
+		   return_range=False):
 	'''
 	Make a 3-color image of stars.
 
-	The colors are based on magnitudes found using stellar Marigo
-	stellar population code.  If with_dust is True, a simple dust
-	screening is applied.
+	For information about how surface brightnesses are calculated, see the documentation for
+	:mod:`pynbody.analysis.luminosity`.
 
-	Returns: If ret_im=True, an NxNx3 array representing an RGB image
+	If ``with_dust`` is True, a simple dust screening is applied; see below for important notes
+	on the dust screening.
 
-	**Optional keyword arguments:**
+	Parameters
+	----------
 
-	   *filename*: string (default: None)
-		 Filename to be written to (if a filename is specified)
+	sim : SimSnap
+		The simulation snapshot to plot.
 
-	   *r_band*: string (default: 'i')
-		 Determines which Johnston filter will go into the image red channel
+	r_band, g_band, b_band : str
+		The filter bands to use for R, G and B image channels. Default is 'i', 'v', 'b'.
 
-	   *g_band*: string (default: 'v')
-		 Determines which Johnston filter will go into the image green channel
+	width : float | str, optional
+		The width of the image to produce, either as a float or a unit string.
 
-	   *b_band*: string (default: 'b')
-		 Determines which Johnston filter will go into the image blue channel
+	r_scale, g_scale, b_scale : float, optional
+		The scaling of the red, green and blue channels before they are combined.
 
-	   *r_scale*: float (default: 0.5)
-		 The scaling of the red channel before channels are combined
+	dynamic_range : float, optional
+		The number of dex in luminosity over which the image brightness ranges, if
+		``mag_range`` is not provided.
 
-	   *g_scale*: float (default: 1.0)
-		 The scaling of the green channel before channels are combined
+	with_dust : bool, optional
+		If True, the image is rendered with a simple dust screening model. See important notes below.
 
-	   *b_scale*: float (default: 1.0)
-		 The scaling of the blue channel before channels are combined
+	mag_range : tuple, optional
+		The brightest and faintest surface brightnesses in the final image, in
+		mag arcsec^-2.
 
-	   *width*: float in kpc (default:50)
-		 Sets the size of the image field in kpc
+	resolution : int, optional
+		The resolution of the image to produce. The default is determined by the configuration
+		option ``image-default-resolution``.
 
-	   *resolution*: integer (default: 500)
-	     Sets the number of pixels on the side of the image
+	noplot : bool, optional
+		If True, the image is not plotted; most useful alongside ``return_image``, if you want to save the
+		image to a file.
 
-	   *starsize*: float in kpc (default: None)
-		 If not None, sets the maximum size of stars in the image
+	axes : matplotlib.axes.Axes, optional
+		If not None, the axes object to plot to.
 
-	   *ret_im*: bool (default: False)
-		 if True, the NxNx3 image array is returned
+	return_image : bool, optional
+		If True, the image is returned as an array (N x N x 3) for the RGB channels. Default is False.
 
-	   *ret_range*: bool (default: False)
-		 if True, the range of the image in mag arcsec^-2 is returned.
+	return_range : bool, optional
+		If True, a tuple with the range of the image in mag arcsec^-2 is returned. Default is False.
 
-	   *plot*: bool (default: True)
-		 if True, the image is plotted
+	clear : bool, optional
+		If True, the current figure is cleared before plotting. Default is True.
 
-	   *axes*: matplotlib axes object (deault: None)
-		 if not None, the axes object to plot to
 
-	   *dynamic_range*: float (default: 2.0)
-		 The number of dex in luminosity over which the image brightness ranges
+	Returns
+	-------
 
-	   *mag_range*: float, float (default: None)
-		 If provided, the brightest and faintest surface brightnesses in the range,
-		 in mag arcsec^-2. Takes precedence over dynamic_range.
+	If ``return_image`` is True, an array (N x N x 3) representing the RGB image is returned.
 
-	   *with_dust*: bool, (default: False)
-		 If True, the image is rendered with a simple dust screening model
-		 based on Calzetti's law.
-
-	   *z_range*: float, (default: 50.0)
-		 If with_dust is True this parameter specifies the z range
-		 over which the column density will be calculated.
-		 The default value is 50 kpc.
+	If ``return_range`` is True, a tuple with the range of the image in mag arcsec^-2 is returned.
 
-	'''
+	Notes
+	-----
 
-	if isinstance(width, str) or issubclass(width.__class__, _units.UnitBase):
-		if isinstance(width, str):
-			width = _units.Unit(width)
-		width = width.in_units(sim['pos'].units, **sim.conversion_context())
+	The dust screening model is exceptionally simple and can only be used for indicative purposes.
+	For more accurate results, radiative transfer is essential and is provided by other packages
+	such as `skirt <https://skirt.ugent.be/root/_home.html>`_.
 
-	if starsize is not None:
-		smf = filt.HighPass('smooth', str(starsize) + ' kpc')
-		sim.s[smf]['smooth'] = array.SimArray(starsize, 'kpc', sim=sim)
+	The model assumes that the dust is proportional to the metal density. It estimates a V-band
+	extinction A_V using empirical data from Draine & Lee (1984, ApJ, 285, 89) and Savage and Mathis
+	(1979, ARA&A, 17, 73). This is then converted to extinction in the given bands using the
+	Calzetti law.
 
-	r = image(sim.s, qty=r_band + '_lum_den', width=width, log=False,
+	The model furthermore assumes that half the dust is in front of the stars and half behind, because
+	there is no radiative transfer to account for the actual distribution of dust in the 3d space.
+
+	'''
+
+	width = plot_sph._width_in_sim_units(sim, width)
+
+	r = plot_sph.image(sim.s, qty=r_band + '_lum_den', width=width, log=False,
 			  units="pc^-2", clear=False, noplot=True, resolution=resolution) * r_scale
-	g = image(sim.s, qty=g_band + '_lum_den', width=width, log=False,
+	g = plot_sph.image(sim.s, qty=g_band + '_lum_den', width=width, log=False,
 			  units="pc^-2", clear=False, noplot=True, resolution=resolution) * g_scale
-	b = image(sim.s, qty=b_band + '_lum_den', width=width, log=False,
+	b = plot_sph.image(sim.s, qty=b_band + '_lum_den', width=width, log=False,
 			  units="pc^-2", clear=False, noplot=True, resolution=resolution) * b_scale
 
 	# convert all channels to mag arcsec^-2
 
-	r=convert_to_mag_arcsec2(r)
-	g=convert_to_mag_arcsec2(g)
-	b=convert_to_mag_arcsec2(b)
+	r=_convert_to_mag_arcsec2(r)
+	g=_convert_to_mag_arcsec2(g)
+	b=_convert_to_mag_arcsec2(b)
 
 	if with_dust is True:
 		# render image with a simple dust absorption correction based on Calzetti's law using the gas content.
+
+		a_v = _dust_Av_image(sim, width, resolution)
+
 		try:
 			import extinction
 		except ImportError:
-			warnings.warn(
-				"Could not load extinction package. If you want to use this feature, "
+			raise ImportError("Could not load extinction package. If you want to use this feature, "
 				"plaese install the extinction package from here: http://extinction.readthedocs.io/en/latest/"
-				"or <via pip install extinction> or <conda install -c conda-forge extinction>", RuntimeWarning)
-			return
-
-		warm = filt.HighPass('temp',3e4)
-		cool = filt.LowPass('temp',3e4)
-		positive = filt.BandPass('z',-z_range,z_range) #LowPass('z',0)
-
-		column_den_warm = image(sim.g[positive][warm], qty='rho', width=width, log=False,
-			  units="kg cm^-2", clear=False, noplot=True,z_camera=z_range)
-		column_den_cool = image(sim.g[positive][cool], qty='rho', width=width, log=False,
-			  units="kg cm^-2", clear=False, noplot=True,z_camera=z_range)
-		mh = 1.67e-27 # units kg
-
-		cool_fac = 0.25 # fudge factor to make dust absorption not too strong
-		# get the column density of gas
-		col_den = np.divide(column_den_warm,mh)+np.divide(column_den_cool*cool_fac,mh)
-		# get absorption coefficient
-		a_v = 0.5*col_den*2e-21
+				"or <via pip install extinction> or <conda install -c conda-forge extinction>") from None
 
 		#get the central wavelength for the given band
 		wavelength_avail = {'u':3571,'b':4378,'v':5466,'r':6695,'i':8565,'j':12101,
 				   'h':16300,'k':21900,'U':3571,'B':4378,'V':5466,'R':6695,'I':8565,'J':12101,
 				   'H':16300,'K':21900} #in Angstrom
 		# effective wavelength taken from http://svo2.cab.inta-csic.es/svo/theory/fps3/index.php?mode=browse&gname=Generic&gname2=Johnson
 		# and from https://en.wikipedia.org/wiki/Photometric_system for h, k
 
 		lr,lg,lb = wavelength_avail[r_band],wavelength_avail[g_band],wavelength_avail[b_band] #in Angstrom
 		wave = np.array([lb, lg, lr])
 
-		ext_r = np.empty_like(r)
-		ext_g = np.empty_like(g)
-		ext_b = np.empty_like(b)
+		ext_r = np.empty(a_v.shape)
+		ext_g = np.empty(a_v.shape)
+		ext_b = np.empty(a_v.shape)
 
 		for i in range(len(a_v)):
 			for j in range(len(a_v[0])):
 				ext = extinction.calzetti00(wave.astype(np.float_), a_v[i][j].astype(np.float_), 3.1, unit='aa', out=None)
 				ext_r[i][j] = ext[2]
 				ext_g[i][j] = ext[1]
 				ext_b[i][j] = ext[0]
@@ -226,43 +258,76 @@
 		g = g+ext_g
 		b = b+ext_b
 
 	#r,g,b = nw_scale_rgb(r,g,b)
 	#r,g,b = nw_arcsinh_fit(r,g,b)
 
 	if mag_range is None:
-		rgbim, mag_max = combine(r, g, b, dynamic_range*2.5)
+		rgbim, mag_max = _combine(r, g, b, dynamic_range * 2.5)
 		mag_min = mag_max + 2.5*dynamic_range
 	else:
 		mag_max, mag_min = mag_range
-		rgbim, mag_max = combine(r, g, b, mag_min - mag_max, mag_max)
+		rgbim, mag_max = _combine(r, g, b, mag_min - mag_max, mag_max)
 
-	if plot:
+	if not noplot:
 		if clear:
 			plt.clf()
 		if axes is None:
 			axes = plt.gca()
 
 		if axes:
 			axes.imshow(
 				rgbim[::-1, :], extent=(-width / 2, width / 2, -width / 2, width / 2))
 			axes.set_xlabel('x [' + str(sim.s['x'].units) + ']')
 			axes.set_ylabel('y [' + str(sim.s['y'].units) + ']')
 			plt.draw()
 
-	if filename:
-		plt.savefig(filename)
-
-	if ret_im:
+	if return_image:
 		return rgbim
 
-	if ret_range:
+	if return_range:
 		return mag_max, mag_min
 
 
+
+def _dust_Av_image(sim, width, resolution):
+	"""Produce a map of the extinction Av for the given simulation, using the gas content.
+
+	Note that the dust model is very simple and naive! See comments inline.
+	"""
+
+	# Assume that only the gas with z>0 absorbs light (i.e. 'all light' is produced in the midplane)
+	gas = sim.g
+
+	# calculate the density of metals, and assume that dust is proportional to the metal density
+	rho_metals = gas['rho'] * gas['metals']
+	rho_metals.units = gas['rho'].units
+	column_den = plot_sph.image(gas, qty=rho_metals, width=width, log=False, restrict_depth=True,
+					            units="m_p cm^-2", clear=False, noplot=True, resolution=resolution)
+
+	# From Draine & Lee (1984, ApJ, 285, 89) in the V band (lambda^-1 ~= 2 micron^-1), the optical
+	# depth is 0.5 for an H column density of 10^21 cm^2. That scaling in turn is based on data in
+	# the review of Savage and Mathis (1979, ARA&A, 17, 73). Amazingly, this is the most up-to-date
+	# reference I could find on the subject. There is no mention of the metallicity dependence but
+	# one would assume dust columns should scale at least with metal columns (perhaps even more
+	# steeply with local metallicity). Given the wild approximations in all this, I assume a
+	# metallicity of 0.02 for gas in the Milky Way
+
+	tau_to_mag_extinction = 2.5 / np.log(10.)
+
+	a_v = tau_to_mag_extinction * 0.5 * column_den / 1e21 / 0.02
+
+	# Finally, we assume that half the dust is in front of the stars and half behind. This is
+	# yet another big assumption!
+
+	a_v/=2
+
+	return a_v
+
+
 def mollview(map=None,fig=None,plot=False,filenme=None,
 			 rot=None,coord=None,unit='',
 			 xsize=800,title='Mollweide view',nest=False,
 			 min=None,max=None,flip='astro',
 			 remove_dip=False,remove_mono=False,
 			 gal_cut=0,
 			 format='%g',format2='%g',
@@ -531,24 +596,24 @@
 	g = render_spherical_image(sim.s, qty=g_band + '_lum_den', nside=nside, distance=width, kernel=Kernel2D(),kstep=0.5, denoise=None, out_units="pc^-2", threaded=False)# * g_scale
 	g = mollview(g,return_projected_map=True,fig=f) * g_scale
 	f=plt.gcf()
 	b = render_spherical_image(sim.s, qty=b_band + '_lum_den', nside=nside, distance=width, kernel=Kernel2D(),kstep=0.5, denoise=None, out_units="pc^-2", threaded=False)# * b_scale
 	b = mollview(b,return_projected_map=True,fig=f) * b_scale
 	# convert all channels to mag arcsec^-2
 
-	r=convert_to_mag_arcsec2(r, mollview=True)
-	g=convert_to_mag_arcsec2(g, mollview=True)
-	b=convert_to_mag_arcsec2(b, mollview=True)
+	r=_convert_to_mag_arcsec2(r, mollview=True)
+	g=_convert_to_mag_arcsec2(g, mollview=True)
+	b=_convert_to_mag_arcsec2(b, mollview=True)
 
 	if mag_range is None:
-		rgbim, mag_max = combine(r, g, b, dynamic_range*2.5, mollview=True)
+		rgbim, mag_max = _combine(r, g, b, dynamic_range * 2.5, mollview=True)
 		mag_min = mag_max + 2.5*dynamic_range
 	else:
 		mag_max, mag_min = mag_range
-		rgbim, mag_max = combine(r, g, b, mag_min - mag_max, mag_max, mollview=True)
+		rgbim, mag_max = _combine(r, g, b, mag_min - mag_max, mag_max, mollview=True)
 
 	if plot:
 		if clear:
 			plt.clf()
 		if axes is None:
 			axes = plt.gca()
```

### Comparing `pynbody-2.0.0b7/pynbody/plot/util.py` & `pynbody-2.0.0b8/pynbody/plot/util.py`

 * *Files identical despite different names*

### Comparing `pynbody-2.0.0b7/pynbody/simdict.py` & `pynbody-2.0.0b8/pynbody/simdict.py`

 * *Files identical despite different names*

### Comparing `pynbody-2.0.0b7/pynbody/snapshot/__init__.py` & `pynbody-2.0.0b8/pynbody/snapshot/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,62 +1,74 @@
 """
-snapshot
-========
-
-This module implements the  :class:`~pynbody.snapshot.SimSnap` class which manages and stores snapshot data.
-It also implements the :class:`~pynbody.snapshot.SubSnap` class (and relatives) which
-represent different views of an existing :class:`~pynbody.snapshot.SimSnap`.
-
+Implements classes to load and manipulate snapshot data
 """
 
 import logging
 import pathlib
 
 from .. import config, family
 from . import util
 from .simsnap import SimSnap
 
 logger = logging.getLogger('pynbody.snapshot')
 
 
 def load(filename, *args, **kwargs) -> SimSnap:
-    """Loads a file using the appropriate class, returning a SimSnap
-    instance."""
+    """Loads a file using the appropriate class, returning a SimSnap instance.
+
+    This routine is the main entry point for loading snapshots. It will try to load the file using the appropriate
+    class, based on inspection by the candidate subclasses. If no class can load the file, an OSError is raised.
+
+    Arguments
+    ---------
+    filename : str
+        The filename to load
+
+    priority : optional, list[str | type]
+        A list of SimSnap subclasses to try, in order. The first class which is capable of loading the file
+        is used. If not specified, the ordering is as specified in the configuration files.
+
+    *args, **kwargs :
+        Other arguments and keyword arguments are passed to the class constructor that is used to load the file.
+
+    Returns
+    -------
+    SimSnap
+        The loaded snapshot
+
+    """
 
     filename = pathlib.Path(filename)
 
     priority = kwargs.pop('priority', config['snap-class-priority'])
 
     for c in SimSnap.iter_subclasses_with_priority(priority):
         if c._can_load(filename):
             logger.info("Loading using backend %s" % str(c))
             return c(filename, *args, **kwargs)
 
     raise OSError(
         "File %r: format not understood or does not exist" % filename)
 
-def new(n_particles=0, order=None, class_=SimSnap, **families):
+def new(n_particles = 0, order = None, class_ = SimSnap, **families) -> SimSnap:
     """Create a blank SimSnap, with the specified number of particles.
 
-    Position, velocity and mass arrays are created and filled
-    with zeros.
+    Position, velocity and mass arrays are created and filled with zeros.
 
     By default all particles are taken to be dark matter.
-    To specify otherwise, pass in keyword arguments specifying
-    the number of particles for each family, e.g.
 
-    f = new(dm=50, star=25, gas=25)
+    To specify otherwise, pass in keyword arguments specifying the number of particles for each family, e.g.
+
+    >>> f = new(dm=50, star=25, gas=25)
 
-    The order in which the different families appear in the snapshot
-    is unspecified unless you add an 'order' argument:
+    The order in which the different families appear in the snapshot is unspecified unless you add an 'order' argument:
 
-    f = new(dm=50, star=25, gas=25, order='star,gas,dm')
+    >>> f = new(dm=50, star=25, gas=25, order='star,gas,dm')
 
-    guarantees the stars, then gas, then dark matter particles appear
-    in sequence.
+    guarantees the stars, then gas, then dark matter particles appear in sequence.
     """
 
     if len(families) == 0:
         families = {'dm': n_particles}
 
     t_fam = []
     tot_particles = 0
```

### Comparing `pynbody-2.0.0b7/pynbody/snapshot/copy_on_access.py` & `pynbody-2.0.0b8/pynbody/snapshot/copy_on_access.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,22 +1,29 @@
+"""Implements classes to automatically copy data from another snapshot when needed.
+
+Most users will not need to use this module directly. It is used by `tangos <https://pynbody.github.io/tangos>`_
+to provide a transparent view of a snapshot that is actually stored in a different location.
+"""
+
 import copy
 
 from .simsnap import SimSnap
 
 
 class UnderlyingClassMixin:
+    """Mixin for a SimSnap that allows it to derive quantities associated with another class."""
     def __init__(self, underlying_class, *args, **kwargs):
         super().__init__(*args, **kwargs)
         self._underlying_class = underlying_class
 
     def _find_deriving_function(self, name):
         cl = self._underlying_class
-        if cl in self._derived_quantity_registry \
-                and name in self._derived_quantity_registry[cl]:
-            return self._derived_quantity_registry[cl][name]
+        if cl in self._derived_array_registry \
+                and name in self._derived_array_registry[cl]:
+            return self._derived_array_registry[cl][name]
         else:
             return super()._find_deriving_function(name)
 
 class CopyOnAccessSimSnap(UnderlyingClassMixin, SimSnap):
     """SimSnap that copies data from another SimSnap when that data is needed.
 
     To the user, data which is already loaded in the underlying snapshot presents merely as 'loadable'
```

### Comparing `pynbody-2.0.0b7/pynbody/snapshot/gadget.py` & `pynbody-2.0.0b8/pynbody/snapshot/gadget.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 """
+Implements reading old-style gadget binary files (format 1 and 2, but not HDF5).
+
+The gadget array names are mapped into pynbody array names according to the mappings given by the `config.ini`
+section `[gadget-name-mapping]`.
+
+Very old gadget-1 style files have a fixed block order, which is specified in the config.ini section
+`[gadget-1-blocks]`.
 
-gadget
-======
 
-Implements classes and functions for handling gadget files; you rarely
-need to access this module directly as it will be invoked
-automatically via pynbody.load.
 
 """
 
 
 import configparser
 import copy
 import errno
@@ -63,15 +65,15 @@
         return l
     elif fam is None:
         return list(np.arange(0, N_TYPE))
     else:
         return _type_map[fam]
 
 
-class GadgetBlock:
+class _GadgetBlock:
 
     """Class to describe each block.
     Each block has a start, a length, and a length-per-particle"""
 
     def __init__(self, start=0, length=0, partlen=0, dtype=np.float32, p_types=np.zeros(N_TYPE, bool)):
         # Start of block in file
         self.start = start
@@ -121,16 +123,16 @@
      time, redshift,  flag_sfr, flag_feedback,
      npartTotal[0], npartTotal[1], npartTotal[
      2], npartTotal[3], npartTotal[4], npartTotal[5],
      flag_cooling, num_files, BoxSize, Omega0, OmegaLambda, HubbleParam, flag_stellarage, flag_metals,
      NallHW[0], NallHW[1], NallHW[2], NallHW[3], NallHW[4], NallHW[5],
      flag_entropy_instead_u, flag_doubleprecision, flag_ic_info, lpt_scalingfactor, fill) = struct.unpack(fmt, data)
 
-    header = GadgetHeader(npart, mass, time, redshift,
-                          BoxSize, Omega0, OmegaLambda, HubbleParam, num_files)
+    header = _GadgetHeader(npart, mass, time, redshift,
+                           BoxSize, Omega0, OmegaLambda, HubbleParam, num_files)
     header.flag_sfr = flag_sfr
     header.flag_feedback = flag_feedback
     header.npartTotal = npartTotal
     header.flag_cooling = flag_cooling
     header.flag_stellarage = flag_stellarage
     header.flag_metals = flag_metals
     header.NallHW = NallHW
@@ -139,15 +141,15 @@
     header.flag_ic_info = flag_ic_info
     header.lpt_scalingfactor = lpt_scalingfactor
     header.endian = endian
 
     return header
 
 
-class GadgetHeader:
+class _GadgetHeader:
 
     """Describes the header of gadget class files; this is all our metadata, so we are going to store it inline"""
 
     def __init__(self, npart, mass, time, redshift, BoxSize, Omega0, OmegaLambda, HubbleParam, num_files=1):
         "Construct a header from values, instead of a datastring."""
         assert(len(mass) == 6)
         assert(len(npart) == 6)
@@ -246,15 +248,15 @@
                                                                   self.NallHW[4]), int(
                                                                       self.NallHW[
                                                                           5]),
             self.flag_entropy_instead_u, self.flag_doubleprecision, self.flag_ic_info, self.lpt_scalingfactor)
         return data
 
 
-class GadgetFile:
+class _GadgetFile:
 
     """Gadget file management class. Users should access gadget files through
     :class:`~pynbody.snapshot.gadget.GadgetSnap`."""
 
     def __init__(self, filename):
         self._filename = filename
         self.blocks = {}
@@ -269,15 +271,15 @@
                     'gadget-1-blocks', "blocks").split(",")
                 self.block_names = [q.upper().ljust(4) for q in self.block_names]
                 if sys.version_info[0] > 2:
                     self.block_names = [str.encode(x, 'utf-8') for x in self.block_names]
                 # This is a counter for the fallback
                 self.extra = 0
             while True:
-                block = GadgetBlock()
+                block = _GadgetBlock()
                 (name, block.length) = self.read_block_head(fd)
                 if block.length == 0:
                     break
                 # Do special things for the HEAD block
                 if name[0:4] == b"HEAD":
                     if block.length != 256:
                         raise OSError("Mis-sized HEAD block in " + filename)
@@ -357,15 +359,15 @@
                     warnings.warn("Encountered a gadget block %r which could not be interpreted - is it a strange length or data type (length=%d)?" %
                                 (name, block.length), RuntimeWarning)
                 else:
                     self.blocks[name[0:4]] = block
 
         # Make a mass block if one isn't found.
         if b'MASS' not in self.blocks:
-            block = GadgetBlock()
+            block = _GadgetBlock()
             block.length = 0
             block.start = 0
 
             # Mass should be the same type as POS (see issue #321)
             block.data_type = self.blocks[b'POS '].data_type
             block.partlen = np.dtype(block.data_type).itemsize
             self.blocks[b'MASS'] = block
@@ -573,15 +575,15 @@
         # Get last block
         lb = max(list(self.blocks.values()), key=lambda val: val.start)
 
         if np.issubdtype(dtype, np.floating):
             dtype = np.float32  # coerce to single precision
 
         # Make new block
-        block = GadgetBlock(length=blocksize, partlen=partlen, dtype=dtype)
+        block = _GadgetBlock(length=blocksize, partlen=partlen, dtype=dtype)
         block.start = lb.start + lb.length + 6 * \
             4  # For the block header, and footer of the previous block
         if p_types is None:
             block.p_types = np.ones(N_TYPE, bool)
         else:
             block.p_types = p_types
         self.blocks[name] = block
@@ -640,15 +642,15 @@
             fd.seek(48, 1)
             data = self.write_block_footer(b"HEAD", 256)
             fd.write(data)
         finally:
             fd.close()
 
 
-class GadgetWriteFile (GadgetFile):
+class _GadgetWriteFile(_GadgetFile):
 
     """Class for write-only snapshots, as when we are creating a new set of files from, eg, a TipsySnap.
         Should not be used directly. block_names is a list so we can specify an on-disc ordering."""
 
     def __init__(self, filename, npart, block_names, header, format2=True):
         self.header = header
         self._filename = filename
@@ -663,22 +665,22 @@
         footer_size = 4
         # First block is just past the header.
         cur_pos = 256 + header_size + footer_size
         for block in block_names:
             # Add block if present for some types
             if block.types.sum():
                 b_part = npart * block.types
-                b = GadgetBlock(
+                b = _GadgetBlock(
                     start=cur_pos + header_size, partlen=block.partlen,
                     length=block.partlen * b_part.sum(), dtype=block.dtype, p_types=block.types)
                 cur_pos += b.length + header_size + footer_size
                 self.blocks[_to_raw(block.name)] = b
 
 
-class WriteBlock:
+class _WriteBlock:
 
     """Internal structure for passing data around between file and snapshot"""
 
     def __init__(self, partlen=4, dtype=np.float32, types=np.zeros(N_TYPE, bool), name="    "):
 
         if np.issubdtype(dtype, np.floating):
             dtype = np.float32
@@ -689,17 +691,15 @@
         self.dtype = dtype
 
         self.types = types
         self.name = name
 
 
 class GadgetSnap(SimSnap):
-
-    """Main class for reading Gadget-2 snapshots. The constructor makes a map of the locations
-    of the blocks, which are then read by _load_array"""
+    """Class for reading Gadget-1 and Gadget-2 old-style (i.e. pre-HDF5) snapshots."""
 
     def __init__(self, filename: pathlib.Path, only_header=False, must_have_paramfile=False, ignore_cosmo=False):
 
         filename = str(filename)
 
         global config
         super().__init__()
@@ -714,27 +714,27 @@
             filename = filename + ".0"
             files = None
 
         if filename[-2:] == ".0":
             self._filename = filename[:-2]
         # Read the first file and use it to get an idea of how many files we
         # are expecting.
-        first_file = GadgetFile(filename)
+        first_file = _GadgetFile(filename)
         self._files.append(first_file)
         files_expected = self._files[0].header.num_files
         npart = np.array(self._files[0].header.npart)
 
         if files is None:
             # we want to load all files
             base_filename = filename[:-2]
             files = [base_filename + "." + str(i)
                      for i in range(files_expected)]
 
         for filename in files[1:]:
-            tmp_file = GadgetFile(filename)
+            tmp_file = _GadgetFile(filename)
             if not self.check_headers(tmp_file.header, self._files[0].header):
                 warnings.warn("file " + str(
                     i) + " is not part of this snapshot set!", RuntimeWarning)
                 continue
             self._files.append(tmp_file)
             npart = npart + tmp_file.header.npart
         # Set up things from the parent class
@@ -1004,15 +1004,15 @@
                     # Note that if we have more than one type per family, we cannot
                     # determine which type each individual particle is, so
                     # assume they are all the first.
                     npart[np.min(gadget_type(f))] = len(self[f][arr_name])
                 # Construct a header
                 # npart, mass, time, redshift, BoxSize,Omega0, OmegaLambda,
                 # HubbleParam, num_files=1
-                gheader = GadgetHeader(
+                gheader = _GadgetHeader(
                     npart, np.zeros(N_TYPE, float), self.properties[
                         "a"], self.properties["z"],
                     self.properties["boxsize"].in_units(self[
                                                         'pos'].units, **self.conversion_context()),
                     self.properties["omegaM0"], self.properties["omegaL0"], self.properties["h"], 1)
                 # Construct the block_names; each block_name needs partlen, data_type, and p_types,
                 # as well as a name. Blocks will hit the disc in the order they are in all_keys.
@@ -1035,19 +1035,19 @@
                             try:
                                 partlen = np.shape(self[
                                                    f][k])[1]  # *dtype.itemsize
                             except IndexError:
                                 partlen = 1  # dtype.itemsize
                         except KeyError:
                             pass
-                    bb = WriteBlock(partlen, dtype=dtype, types=types, name=_translate_array_name(
+                    bb = _WriteBlock(partlen, dtype=dtype, types=types, name=_translate_array_name(
                         k).upper().ljust(4)[0:4])
                     block_names.append(bb)
                 # Create an output file
-                out_file = GadgetWriteFile(
+                out_file = _GadgetWriteFile(
                     filename, npart, block_names, gheader)
                 # Write the header
                 out_file.write_header(gheader, filename)
                 # Write all the arrays
                 for x in all_keys:
                     g_name = _to_raw(
                         _translate_array_name(x).upper().ljust(4)[0:4])
@@ -1158,18 +1158,15 @@
                         s += f_parts[i]
 
 
 def _header_suggests_cosmological(gadget_header):
     return (gadget_header.HubbleParam != 0.) and (gadget_header.Omega0 != 0.) and (gadget_header.BoxSize != 0.)
 
 @GadgetSnap.decorator
-def do_units(sim):
-    # cosmo =
-    # (sim._hdf_files['Parameters']['NumericalParameters'].attrs['ComovingIntegrationOn'])!=0
-
+def _do_units(sim):
     vel_unit = config_parser.get('gadget-units', 'vel')
     dist_unit = config_parser.get('gadget-units', 'pos')
     mass_unit = config_parser.get('gadget-units', 'mass')
 
     vel_unit, dist_unit, mass_unit = (
         units.Unit(x) for x in (vel_unit, dist_unit, mass_unit))
 
@@ -1181,15 +1178,15 @@
         dist_unit = units.Unit("kpc") * dist_unit.in_units("kpc", a=1, h=1)
 
     sim._file_units_system = [units.Unit("K"), vel_unit, dist_unit, mass_unit]
     sim._override_units_system()
 
 
 @GadgetSnap.decorator
-def do_properties(sim):
+def _do_properties(sim):
     h = sim.header
 
     if not(sim._ignore_cosmo) and _header_suggests_cosmological(h):
         from .. import analysis
         sim.properties['omegaM0'] = h.Omega0
         # sim.properties['omegaB0'] = ... This one is non-trivial to calculate
         sim.properties['omegaL0'] = h.OmegaLambda
```

### Comparing `pynbody-2.0.0b7/pynbody/snapshot/gadgethdf.py` & `pynbody-2.0.0b8/pynbody/snapshot/gadgethdf.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,27 +1,21 @@
 """
+Implements reading HDF5 Gadget files, in various variants.
 
-gadgethdf
-=========
-
-
-Implementation of backend reader for GadgetHDF files by Andrew Pontzen.
-
-The gadget array names are mapped into pynbody array mes according
-to the mappings given by the config.ini section [gadgethdf-name-mapping].
+The gadget array names are mapped into pynbody array names according
+to the mappings given by the config.ini section ``[gadgethdf-name-mapping]``.
 
 The gadget particle groups are mapped into pynbody families according
-to the mappings specified by the config.ini section [gadgethdf-type-mapping].
+to the mappings specified by the config.ini section ``[gadgethdf-type-mapping]``.
 This can be many-to-one (many gadget particle types mapping into one
 pynbody family), but only datasets which are common to all gadget types
 will be available from pynbody.
 
-Spanned files are supported. To load a range of files snap.0, snap.1, ... snap.n,
-pass the filename 'snap'. If you pass snap.0, only that particular file will
-be loaded.
+Spanned files are supported. To load a range of files ``snap.0.hdf5``, ``snap.1.hdf5``, ... ``snap.n.hdf5``,
+pass the filename ``snap``. If you pass e.g. ``snap.2.hdf5``, only file 2 will be loaded.
 """
 
 import configparser
 import functools
 import itertools
 import logging
 import warnings
@@ -50,15 +44,15 @@
 for hdf_groups in _default_type_map.values():
     for hdf_group in hdf_groups:
         _all_hdf_particle_groups.append(hdf_group)
 
 
 
 
-class DummyHDFData:
+class _DummyHDFData:
 
     """A stupid class to allow emulation of mass arrays for particles
     whose mass is in the header"""
 
     def __init__(self, value, length, dtype):
         self.value = value
         self.length = length
@@ -69,15 +63,15 @@
     def __len__(self):
         return self.length
 
     def read_direct(self, target):
         target[:] = self.value
 
 
-class GadgetHdfMultiFileManager:
+class _GadgetHdfMultiFileManager:
     _nfiles_groupname = "Header"
     _nfiles_attrname = "NumFilesPerSnapshot"
     _size_from_hdf5_key = "ParticleIDs"
     _subgroup_name = None
 
     def __init__(self, filename, mode='r') :
         filename = str(filename)
@@ -151,31 +145,37 @@
     def reopen_in_mode(self, mode):
         if mode!=self._mode:
             self._open_files = {}
             self._mode = mode
 
 
 
-class SubfindHdfMultiFileManager(GadgetHdfMultiFileManager):
+class _SubfindHdfMultiFileManager(_GadgetHdfMultiFileManager):
     _nfiles_groupname = "FOF"
     _nfiles_attrname = "NTask"
     _subgroup_name = "FOF"
 
 
 class GadgetHDFSnap(SimSnap):
     """
-    Class that reads HDF Gadget data
+    Class that reads HDF Gadget snapshots.
     """
 
-    _multifile_manager_class = GadgetHdfMultiFileManager
+    _multifile_manager_class = _GadgetHdfMultiFileManager
     _readable_hdf5_test_key = "PartType?"
     _size_from_hdf5_key = "ParticleIDs"
     _namemapper_config_section = "gadgethdf-name-mapping"
 
-    def __init__(self, filename, ):
+    def __init__(self, filename):
+        """Initialise a Gadget HDF snapshot.
+
+        Spanned files are supported. To load a range of files ``snap.0.hdf5``, ``snap.1.hdf5``, ... ``snap.n.hdf5``,
+        pass the filename ``snap``. If you pass e.g. ``snap.2.hdf5``, only file 2 will be loaded.
+        """
+
         super().__init__()
 
         self._filename = filename
 
         self._init_hdf_filemanager(filename)
 
         self._translate_array_name = namemapper.AdaptiveNameMapper(self._namemapper_config_section)
@@ -358,16 +358,16 @@
         an apparent Mass array even if the mass is actually stored in the header"""
 
         if self._translate_array_name(hdf_name,reverse=True)=='mass':
             try:
                 pgid = int(particle_group.name[-1])
                 mtab = particle_group.parent['Header'].attrs['MassTable'][pgid]
                 if mtab > 0:
-                    return DummyHDFData(mtab, particle_group[self._size_from_hdf5_key].size,
-                                        self._mass_dtype)
+                    return _DummyHDFData(mtab, particle_group[self._size_from_hdf5_key].size,
+                                         self._mass_dtype)
             except (IndexError, KeyError):
                 pass
 
         ret = particle_group
         for tpart in hdf_name.split("/"):
             ret = ret[tpart]
         return ret
@@ -704,17 +704,17 @@
 
 ###################
 # SubFindHDF class
 ###################
 
 class SubFindHDFSnap(GadgetHDFSnap) :
     """
-    Class to read Gadget's SubFind HDF data
+    Reads the variant of Gadget HDF snapshots that include SubFind output inside the snapshot itself.
     """
-    _multifile_manager_class = SubfindHdfMultiFileManager
+    _multifile_manager_class = _SubfindHdfMultiFileManager
     _readable_hdf5_test_key = "FOF"
 
 
 class EagleLikeHDFSnap(GadgetHDFSnap):
     """Reads Eagle-like HDF snapshots (download at http://data.cosma.dur.ac.uk:8080/eagle-snapshots/)"""
     _readable_hdf5_test_key = "PartType1/SubGroupNumber"
 
@@ -734,108 +734,108 @@
                                      array="SubGroupNumber", ignore=np.max(self['SubGroupNumber']))
             cat._keep_subsnap_alive = parent_group # by default, HaloCatalogue only keeps a weakref (should this be changed?)
             return cat
         else:
             return halo.number_array.HaloNumberCatalogue(self, array="GroupNumber", ignore=np.max(self['GroupNumber']))
 
 ## Gadget has internal energy variable
-@GadgetHDFSnap.derived_quantity
-@SubFindHDFSnap.derived_quantity
+@GadgetHDFSnap.derived_array
+@SubFindHDFSnap.derived_array
 def u(self) :
     """Gas internal energy derived from snapshot variable or temperature"""
     try:
         u = self['InternalEnergy']
     except KeyError:
         gamma = 5./3
         u = self['temp']*units.k/(self['mu']*units.m_p*(gamma-1))
 
     return u
 
-@GadgetHDFSnap.derived_quantity
-@SubFindHDFSnap.derived_quantity
+@GadgetHDFSnap.derived_array
+@SubFindHDFSnap.derived_array
 def p(sim) :
     """Calculate the pressure for gas particles, including polytropic equation of state gas"""
 
     critpres = 2300. * units.K * units.m_p / units.cm**3 ## m_p K cm^-3
     critdens = 0.1 * units.m_p / units.cm**3 ## m_p cm^-3
     gammaeff = 4./3.
 
     oneos = sim.g['OnEquationOfState'] == 1.
 
     p = sim.g['rho'].in_units('m_p cm**-3') * sim.g['temp'].in_units('K')
     p[oneos] = critpres * (sim.g['rho'][oneos].in_units('m_p cm**-3')/critdens)**gammaeff
 
     return p
 
-@GadgetHDFSnap.derived_quantity
-@SubFindHDFSnap.derived_quantity
+@GadgetHDFSnap.derived_array
+@SubFindHDFSnap.derived_array
 def HII(sim) :
     """Number of HII ions per proton mass"""
 
     return sim.g["hydrogen"] - sim.g["HI"]
 
-@GadgetHDFSnap.derived_quantity
-@SubFindHDFSnap.derived_quantity
+@GadgetHDFSnap.derived_array
+@SubFindHDFSnap.derived_array
 def HeIII(sim) :
     """Number of HeIII ions per proton mass"""
 
     return sim.g["hetot"] - sim.g["HeII"] - sim.g["HeI"]
 
-@GadgetHDFSnap.derived_quantity
-@SubFindHDFSnap.derived_quantity
+@GadgetHDFSnap.derived_array
+@SubFindHDFSnap.derived_array
 def ne(sim) :
     """Number of electrons per proton mass, ignoring the contribution from He!"""
     ne = sim.g["HII"]  #+ sim["HeII"] + 2*sim["HeIII"]
     ne.units = units.m_p**-1
 
     return ne
 
-@GadgetHDFSnap.derived_quantity
-@SubFindHDFSnap.derived_quantity
+@GadgetHDFSnap.derived_array
+@SubFindHDFSnap.derived_array
 def rho_ne(sim) :
     """Electron number density per SPH particle, currently ignoring the contribution from He!"""
 
     return sim.g["ne"].in_units("m_p**-1") * sim.g["rho"].in_units("m_p cm**-3")
 
-@GadgetHDFSnap.derived_quantity
-@SubFindHDFSnap.derived_quantity
+@GadgetHDFSnap.derived_array
+@SubFindHDFSnap.derived_array
 def dm(sim) :
     """Dispersion measure per SPH particle currently ignoring n_e contribution from He """
 
     return sim.g["rho_ne"]
 
-@GadgetHDFSnap.derived_quantity
-@SubFindHDFSnap.derived_quantity
+@GadgetHDFSnap.derived_array
+@SubFindHDFSnap.derived_array
 def cosmodm(sim) :
     """Cosmological Dispersion measure per SPH particle includes (1+z) factor, currently ignoring n_e contribution from He """
 
     return sim.g["rho_ne"] * (1. + sim.g["redshift"])
-@GadgetHDFSnap.derived_quantity
-@SubFindHDFSnap.derived_quantity
+@GadgetHDFSnap.derived_array
+@SubFindHDFSnap.derived_array
 def redshift(sim) :
     """Redshift from LoS Velocity 'losvel' """
 
     return np.exp( sim['losvel'].in_units('c') ) - 1.
 
-@GadgetHDFSnap.derived_quantity
-@SubFindHDFSnap.derived_quantity
+@GadgetHDFSnap.derived_array
+@SubFindHDFSnap.derived_array
 def doppler_redshift(sim) :
     """Doppler Redshift from LoS Velocity 'losvel' using SR """
 
     return np.sqrt( (1. + sim['losvel'].in_units('c')) / (1. - sim['losvel'].in_units('c'))  ) - 1.
 
-@GadgetHDFSnap.derived_quantity
-@SubFindHDFSnap.derived_quantity
+@GadgetHDFSnap.derived_array
+@SubFindHDFSnap.derived_array
 def em(sim) :
     """Emission Measure (n_e^2) per particle to be integrated along LoS"""
 
     return sim.g["rho_ne"]*sim.g["rho_ne"]
 
-@GadgetHDFSnap.derived_quantity
-@SubFindHDFSnap.derived_quantity
+@GadgetHDFSnap.derived_array
+@SubFindHDFSnap.derived_array
 def halpha(sim) :
     """H alpha intensity (based on Emission Measure n_e^2) per particle to be integrated along LoS"""
 
     ## Rate at which recombining electrons and protons produce Halpha photons.
     ## Case B recombination assumed from Draine (2011)
     #alpha = 2.54e-13 * (sim.g['temp'].in_units('K') / 1e4)**(-0.8163-0.0208*np.log(sim.g['temp'].in_units('K') / 1e4))
     #alpha.units = units.cm**(3) * units.s**(-1)
@@ -846,147 +846,147 @@
     coeff = (6.6260755e-27) * (299792458. / 656.281e-9) / (4.*np.pi) ## units are erg sr^-1
     alpha = coeff * 7.864e-14 * (1e4 / sim.g['temp'].in_units('K'))
 
     alpha.units = units.erg * units.cm**(3) * units.s**(-1) * units.sr**(-1) ## It's intensity in erg cm^3 s^-1 sr^-1
 
     return alpha * sim["em"] # Flux erg cm^-3 s^-1 sr^-1
 
-@GadgetHDFSnap.derived_quantity
-@SubFindHDFSnap.derived_quantity
+@GadgetHDFSnap.derived_array
+@SubFindHDFSnap.derived_array
 def c_n_sq(sim) :
     """Turbulent amplitude C_N^2 for use in SM calculations (e.g. Eqn 20 of Macquart & Koay 2013 ApJ 776 2) """
 
     ## Spectrum of turbulence below the SPH resolution, assume Kolmogorov
     beta = 11./3.
     L_min = 0.1*units.Mpc
     c_n_sq = ((beta - 3.)/((2.)*(2.*np.pi)**(4.-beta)))*L_min**(3.-beta)*sim["em"]
     c_n_sq.units = units.m**(-20,3)
 
     return c_n_sq
 
-@GadgetHDFSnap.derived_quantity
-@SubFindHDFSnap.derived_quantity
+@GadgetHDFSnap.derived_array
+@SubFindHDFSnap.derived_array
 def hetot(self) :
     return self["He"]
 
-@GadgetHDFSnap.derived_quantity
-@SubFindHDFSnap.derived_quantity
+@GadgetHDFSnap.derived_array
+@SubFindHDFSnap.derived_array
 def hydrogen(self) :
     return self["H"]
 
 ## Need to use the ionisation fraction calculation here which gives ionisation fraction
 ## based on the gas temperature, density and redshift for a CLOUDY table
-@GadgetHDFSnap.derived_quantity
-@SubFindHDFSnap.derived_quantity
+@GadgetHDFSnap.derived_array
+@SubFindHDFSnap.derived_array
 def HI(sim) :
     """Fraction of Neutral Hydrogen HI use limited CLOUDY table"""
 
     import pynbody.analysis.hifrac
 
     return pynbody.analysis.hifrac.calculate(sim.g,ion='hi')
 
 ## Need to use the ionisation fraction calculation here which gives ionisation fraction
 ## based on the gas temperature, density and redshift for a CLOUDY table, then applying
 ## selfshielding for the dense, star forming gas on the equation of state
-@GadgetHDFSnap.derived_quantity
-@SubFindHDFSnap.derived_quantity
+@GadgetHDFSnap.derived_array
+@SubFindHDFSnap.derived_array
 def HIeos(sim) :
     """Fraction of Neutral Hydrogen HI use limited CLOUDY table, assuming dense EoS gas is selfshielded"""
 
     import pynbody.analysis.hifrac
 
     return pynbody.analysis.hifrac.calculate(sim.g,ion='hi', selfshield='eos')
 
 ## Need to use the ionisation fraction calculation here which gives ionisation fraction
 ## based on the gas temperature, density and redshift for a CLOUDY table, then applying
 ## selfshielding for the dense, star forming gas on the equation of state AND a further
 ## pressure based limit for
-@GadgetHDFSnap.derived_quantity
-@SubFindHDFSnap.derived_quantity
+@GadgetHDFSnap.derived_array
+@SubFindHDFSnap.derived_array
 def HID12(sim) :
     """Fraction of Neutral Hydrogen HI use limited CLOUDY table, using the Duffy +12a prescription for selfshielding"""
 
     import pynbody.analysis.hifrac
 
     return pynbody.analysis.hifrac.calculate(sim.g,ion='hi', selfshield='duffy12')
 
-@GadgetHDFSnap.derived_quantity
-@SubFindHDFSnap.derived_quantity
+@GadgetHDFSnap.derived_array
+@SubFindHDFSnap.derived_array
 def HeI(sim) :
     """Fraction of Helium HeI"""
 
     import pynbody.analysis.ionfrac
 
     return pynbody.analysis.ionfrac.calculate(sim.g,ion='hei')
 
-@GadgetHDFSnap.derived_quantity
-@SubFindHDFSnap.derived_quantity
+@GadgetHDFSnap.derived_array
+@SubFindHDFSnap.derived_array
 def HeII(sim) :
     """Fraction of Helium HeII"""
 
     import pynbody.analysis.ionfrac
 
     return pynbody.analysis.ionfrac.calculate(sim.g,ion='heii')
 
-@GadgetHDFSnap.derived_quantity
-@SubFindHDFSnap.derived_quantity
+@GadgetHDFSnap.derived_array
+@SubFindHDFSnap.derived_array
 def OI(sim) :
     """Fraction of Oxygen OI"""
 
     import pynbody.analysis.ionfrac
 
     return pynbody.analysis.ionfrac.calculate(sim.g,ion='oi')
 
-@GadgetHDFSnap.derived_quantity
-@SubFindHDFSnap.derived_quantity
+@GadgetHDFSnap.derived_array
+@SubFindHDFSnap.derived_array
 def OII(sim) :
     """Fraction of Oxygen OII"""
 
     import pynbody.analysis.ionfrac
 
     return pynbody.analysis.ionfrac.calculate(sim.g,ion='oii')
 
-@GadgetHDFSnap.derived_quantity
-@SubFindHDFSnap.derived_quantity
+@GadgetHDFSnap.derived_array
+@SubFindHDFSnap.derived_array
 def OVI(sim) :
     """Fraction of Oxygen OVI"""
 
     import pynbody.analysis.ionfrac
 
     return pynbody.analysis.ionfrac.calculate(sim.g,ion='ovi')
 
-@GadgetHDFSnap.derived_quantity
-@SubFindHDFSnap.derived_quantity
+@GadgetHDFSnap.derived_array
+@SubFindHDFSnap.derived_array
 def CIV(sim) :
     """Fraction of Carbon CIV"""
 
     import pynbody.analysis.ionfrac
 
     return pynbody.analysis.ionfrac.calculate(sim.g,ion='civ')
 
-@GadgetHDFSnap.derived_quantity
-@SubFindHDFSnap.derived_quantity
+@GadgetHDFSnap.derived_array
+@SubFindHDFSnap.derived_array
 def NV(sim) :
     """Fraction of Nitrogen NV"""
 
     import pynbody.analysis.ionfrac
 
     return pynbody.analysis.ionfrac.calculate(sim.g,ion='nv')
 
-@GadgetHDFSnap.derived_quantity
-@SubFindHDFSnap.derived_quantity
+@GadgetHDFSnap.derived_array
+@SubFindHDFSnap.derived_array
 def SIV(sim) :
     """Fraction of Silicon SiIV"""
 
     import pynbody.analysis.ionfrac
 
     return pynbody.analysis.ionfrac.calculate(sim.g,ion='siiv')
 
-@GadgetHDFSnap.derived_quantity
-@SubFindHDFSnap.derived_quantity
+@GadgetHDFSnap.derived_array
+@SubFindHDFSnap.derived_array
 def MGII(sim) :
     """Fraction of Magnesium MgII"""
 
     import pynbody.analysis.ionfrac
 
     return pynbody.analysis.ionfrac.calculate(sim.g,ion='mgii')
 
@@ -999,111 +999,111 @@
 XSOLNe=1.4144605E-3
 XSOLMg=5.907064E-4
 XSOLSi=6.825874E-4
 XSOLS=4.0898522E-4
 XSOLCa=6.4355E-5
 XSOLFe=1.1032152E-3
 
-@GadgetHDFSnap.derived_quantity
-@SubFindHDFSnap.derived_quantity
+@GadgetHDFSnap.derived_array
+@SubFindHDFSnap.derived_array
 def feh(self) :
     minfe = np.amin(self['Fe'][np.where(self['Fe'] > 0)])
     self['Fe'][np.where(self['Fe'] == 0)]=minfe
     return np.log10(self['Fe']/self['H']) - np.log10(XSOLFe/XSOLH)
 
-@GadgetHDFSnap.derived_quantity
-@SubFindHDFSnap.derived_quantity
+@GadgetHDFSnap.derived_array
+@SubFindHDFSnap.derived_array
 def sixh(self) :
     minsi = np.amin(self['Si'][np.where(self['Si'] > 0)])
     self['Si'][np.where(self['Si'] == 0)]=minsi
     return np.log10(self['Si']/self['Si']) - np.log10(XSOLSi/XSOLH)
 
-@GadgetHDFSnap.derived_quantity
-@SubFindHDFSnap.derived_quantity
+@GadgetHDFSnap.derived_array
+@SubFindHDFSnap.derived_array
 def sxh(self) :
     minsx = np.amin(self['S'][np.where(self['S'] > 0)])
     self['S'][np.where(self['S'] == 0)]=minsx
     return np.log10(self['S']/self['S']) - np.log10(XSOLS/XSOLH)
 
-@GadgetHDFSnap.derived_quantity
-@SubFindHDFSnap.derived_quantity
+@GadgetHDFSnap.derived_array
+@SubFindHDFSnap.derived_array
 def mgxh(self) :
     minmg = np.amin(self['Mg'][np.where(self['Mg'] > 0)])
     self['Mg'][np.where(self['Mg'] == 0)]=minmg
     return np.log10(self['Mg']/self['Mg']) - np.log10(XSOLMg/XSOLH)
 
-@GadgetHDFSnap.derived_quantity
-@SubFindHDFSnap.derived_quantity
+@GadgetHDFSnap.derived_array
+@SubFindHDFSnap.derived_array
 def oxh(self) :
     minox = np.amin(self['O'][np.where(self['O'] > 0)])
     self['O'][np.where(self['O'] == 0)]=minox
     return np.log10(self['O']/self['H']) - np.log10(XSOLO/XSOLH)
 
-@GadgetHDFSnap.derived_quantity
-@SubFindHDFSnap.derived_quantity
+@GadgetHDFSnap.derived_array
+@SubFindHDFSnap.derived_array
 def nexh(self) :
     minne = np.amin(self['Ne'][np.where(self['Ne'] > 0)])
     self['Ne'][np.where(self['Ne'] == 0)]=minne
     return np.log10(self['Ne']/self['Ne']) - np.log10(XSOLNe/XSOLH)
 
-@SubFindHDFSnap.derived_quantity
+@SubFindHDFSnap.derived_array
 def hexh(self) :
     minhe = np.amin(self['He'][np.where(self['He'] > 0)])
     self['He'][np.where(self['He'] == 0)]=minhe
     return np.log10(self['He']/self['He']) - np.log10(XSOLHe/XSOLH)
 
-@GadgetHDFSnap.derived_quantity
-@SubFindHDFSnap.derived_quantity
+@GadgetHDFSnap.derived_array
+@SubFindHDFSnap.derived_array
 def cxh(self) :
     mincx = np.amin(self['C'][np.where(self['C'] > 0)])
     self['C'][np.where(self['C'] == 0)]=mincx
     return np.log10(self['C']/self['H']) - np.log10(XSOLC/XSOLH)
 
-@GadgetHDFSnap.derived_quantity
-@SubFindHDFSnap.derived_quantity
+@GadgetHDFSnap.derived_array
+@SubFindHDFSnap.derived_array
 def caxh(self) :
     mincax = np.amin(self['Ca'][np.where(self['Ca'] > 0)])
     self['Ca'][np.where(self['Ca'] == 0)]=mincax
     return np.log10(self['Ca']/self['H']) - np.log10(XSOLCa/XSOLH)
 
-@GadgetHDFSnap.derived_quantity
-@SubFindHDFSnap.derived_quantity
+@GadgetHDFSnap.derived_array
+@SubFindHDFSnap.derived_array
 def nxh(self) :
     minnx = np.amin(self['N'][np.where(self['N'] > 0)])
     self['N'][np.where(self['N'] == 0)]=minnx
     return np.log10(self['N']/self['H']) - np.log10(XSOLH/XSOLH)
 
-@GadgetHDFSnap.derived_quantity
-@SubFindHDFSnap.derived_quantity
+@GadgetHDFSnap.derived_array
+@SubFindHDFSnap.derived_array
 def ofe(self) :
     minox = np.amin(self['O'][np.where(self['O'] > 0)])
     self['O'][np.where(self['O'] == 0)]=minox
     minfe = np.amin(self['Fe'][np.where(self['Fe'] > 0)])
     self['Fe'][np.where(self['Fe'] == 0)]=minfe
     return np.log10(self['O']/self['Fe']) - np.log10(XSOLO/XSOLFe)
 
-@GadgetHDFSnap.derived_quantity
-@SubFindHDFSnap.derived_quantity
+@GadgetHDFSnap.derived_array
+@SubFindHDFSnap.derived_array
 def mgfe(sim) :
     minmg = np.amin(sim['Mg'][np.where(sim['Mg'] > 0)])
     sim['Mg'][np.where(sim['Mg'] == 0)]=minmg
     minfe = np.amin(sim['Fe'][np.where(sim['Fe'] > 0)])
     sim['Fe'][np.where(sim['Fe'] == 0)]=minfe
     return np.log10(sim['Mg']/sim['Fe']) - np.log10(XSOLMg/XSOLFe)
 
-@GadgetHDFSnap.derived_quantity
-@SubFindHDFSnap.derived_quantity
+@GadgetHDFSnap.derived_array
+@SubFindHDFSnap.derived_array
 def nefe(sim) :
     minne = np.amin(sim['Ne'][np.where(sim['Ne'] > 0)])
     sim['Ne'][np.where(sim['Ne'] == 0)]=minne
     minfe = np.amin(sim['Fe'][np.where(sim['Fe'] > 0)])
     sim['Fe'][np.where(sim['Fe'] == 0)]=minfe
     return np.log10(sim['Ne']/sim['Fe']) - np.log10(XSOLNe/XSOLFe)
 
-@GadgetHDFSnap.derived_quantity
-@SubFindHDFSnap.derived_quantity
+@GadgetHDFSnap.derived_array
+@SubFindHDFSnap.derived_array
 def sife(sim) :
     minsi = np.amin(sim['Si'][np.where(sim['Si'] > 0)])
     sim['Si'][np.where(sim['Si'] == 0)]=minsi
     minfe = np.amin(sim['Fe'][np.where(sim['Fe'] > 0)])
     sim['Fe'][np.where(sim['Fe'] == 0)]=minfe
     return np.log10(sim['Si']/sim['Fe']) - np.log10(XSOLSi/XSOLFe)
```

### Comparing `pynbody-2.0.0b7/pynbody/snapshot/grafic.py` & `pynbody-2.0.0b8/pynbody/snapshot/grafic.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,13 +1,9 @@
 """
-
-grafic
-======
-
-Support for loading grafIC files
+Support for loading grafIC initial conditions files
 """
 
 import glob
 import os
 import warnings
 
 import numpy as np
@@ -16,15 +12,15 @@
 from ..extern.cython_fortran_utils import FortranFile
 from ..util import grid_gen
 from . import SimSnap
 
 _float_data_type = 'f'
 _int_data_type = 'l'
 
-genic_header = dict(
+_header = dict(
     keys=('nx', 'ny', 'nz', 'dx', 'lx', 'ly', 'lz', 'astart', 'omegam', 'omegal', 'h0'),
     dtype='i,i,i,f,f,f,f,f,f,f,f'
 )
 
 Tcmb = 2.72548
 
 
@@ -35,25 +31,40 @@
         yield q
 
 
 _max_buflen = 1024 ** 2
 
 
 class GrafICSnap(SimSnap):
+    """Class for loading grafIC initial conditions files"""
 
     @staticmethod
     def _can_load(f):
         return os.path.isdir(f) and os.path.exists(os.path.join(f, "ic_velcx"))
 
     def __init__(self, f, take=None, use_pos_file=True):
+        """Load a grafIC initial conditions file
+
+        Parameters
+        ----------
+
+        f : str
+            The directory containing the initial conditions files
+        take : np.ndarray, optional
+            The array of particles to load. If not specified, all particles are loaded.
+        use_pos_file : bool, optional
+            If True, use the displacement field stored in the ic_poscx file to displace particles.
+            If False, use the Zeldovich approximation to reconstruct displacements from velocity information in ic_velx
+            etc.
+        """
         super().__init__()
         with FortranFile(os.path.join(f, "ic_velcx")) as f_cx:
             self._header = {
                 k: v
-                for k, v in zip(genic_header['keys'], f_cx.read_vector(genic_header['dtype'])[0])}
+                for k, v in zip(_header['keys'], f_cx.read_vector(_header['dtype'])[0])}
         h = self._header
         self._dlen = int(h['nx'] * h['ny'])
         self.properties['a'] = float(h['astart'])
         self.properties['h'] = float(h['h0']) / 100.
         self.properties['omegaM0'] = float(h['omegam'])
         self.properties['omegaL0'] = float(h['omegal'])
 
@@ -184,15 +195,15 @@
 
         self._create_array('pvar',dtype=_float_data_type)
         self._read_grafic_file(filename, self['pvar'], _float_data_type)
 
     def _read_grafic_file(self, filename, target_buffer, data_type):
         with FortranFile(filename) as f:
             h = {k: v for k, v
-                 in zip(genic_header['keys'], f.read_vector(genic_header['dtype'])[0])}
+                 in zip(_header['keys'], f.read_vector(_header['dtype'])[0])}
 
             def dummy_interrupt(pos):
                 pass
 
             for readlen, buf_index, mem_index in \
                     self._load_control.iterate_with_interrupts(
                         family.dm, family.dm,
```

### Comparing `pynbody-2.0.0b7/pynbody/snapshot/nchilada.py` & `pynbody-2.0.0b8/pynbody/snapshot/nchilada.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,9 @@
 """
-
-nchilada
-========
-
-Implements classes and functions for handling nchilada files.  You rarely
-need to access this module directly as it will be invoked
-automatically via pynbody.load.
+Implements loading of nchilada files.
 
 """
 
 import os
 import struct
 import warnings
 import xml.dom.minidom
@@ -27,14 +21,15 @@
                              'float32', 'float64']))
 
 
 _max_buf = 1024 * 512
 
 
 class NchiladaSnap(SimSnap):
+    """Implements loading of nchilada files."""
 
     def _load_header(self, f):
         # Used to use xdrlib, but that is deprecated in Python 3.11
         # The following code just follows the old xdrlib implementation
         buf= f.read(28)
         pos= 0
         # Read int, walrus assignment updates pos
@@ -77,14 +72,26 @@
             self.properties['a'] = header_time
         self._load_control = chunk.LoadControl(
             disk_family_slice, _max_buf, take)
         self._family_slice = self._load_control.mem_family_slice
         self._num_particles = self._load_control.mem_num_particles
 
     def __init__(self, filename, **kwargs):
+        """Load a nchilada file.
+
+        Parameters
+        ----------
+
+        filename : str
+            The path to the nchilada output to load. Nchilada outputs are directories containing a description.xml
+            file and a number of binary files.
+        take : np.ndarray, optional
+            The array of particles to load. If not specified, all particles are loaded.
+        """
+
         super().__init__()
 
         must_have_paramfile = kwargs.get('must_have_paramfile', False)
         take = kwargs.get('take', None)
 
         self._dom_sim = xml.dom.minidom.parse(
             os.path.join(filename, "description.xml")).getElementsByTagName('simulation')[0]
@@ -179,29 +186,10 @@
             if ndim > 1:
                 b = b.reshape((readlen, ndim))
 
             if mem_index is not None:
                 r[mem_index] = b[buf_index]
         f.close()
 
-    """
-    def _write_array(self, array_name, fam=None) :
-        if fam is None :
-            fam = self.families()
-
-        for f in fam :
-            fname = self._loadable_keys_registry[fam][array_name]
-            # to do: sort out what happens when this doesn't exist
-            ar = self[fam][array_name]
-
-            _, nbod, ndim, dtype = self._load_header(f)
-            for readlen, buf_index, mem_index in self._load_control.iterate(fam, fam) :
-                b = np.fromfile(f, dtype=disk_dtype, count=readlen*ndim)
-                if ndim>1 : b = b.reshape((readlen, ndim))
-                if mem_index is not None :
-                    b[buf_index] = ar[mem_index]
-                    f.seek(-readlen*ndim*disk_dtype.itemsize,1)
-    """
-
-    @staticmethod
-    def _can_load(f):
+    @classmethod
+    def _can_load(cls, f):
         return os.path.isdir(f) and os.path.exists(os.path.join(f, "description.xml"))
```

### Comparing `pynbody-2.0.0b7/pynbody/snapshot/ramses.py` & `pynbody-2.0.0b8/pynbody/snapshot/ramses.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,13 @@
 """
+Implements classes and functions for handling RAMSES files.
 
-ramses
-======
-
-Implements classes and functions for handling RAMSES files. AMR cells
-are loaded as particles. You rarely need to access this module
-directly as it will be invoked automatically via pynbody.load.
-
-
-For a complete demo on how to use RAMSES outputs with pynbody, look at
-the `ipython notebook demo
-<http://nbviewer.ipython.org/github/pynbody/pynbody/blob/master/examples/notebooks/pynbody_demo-ramses.ipynb>`_
+Note that AMR cells are loaded as particles, although this works surprisingly well for most analysis purposes.
+In particular SPH image generation routines automatically switch on an appropriate de-noising scheme to provide
+effective interpolation between cells.
 
 """
 
 import csv
 import logging
 import os
 import re
@@ -360,64 +353,63 @@
 rt_blocks = [_.strip() for _ in config_parser.get('ramses', 'rt-blocks', raw=True).split(",")]
 
 particle_distinguisher = [_.strip() for _ in config_parser.get('ramses', 'particle-distinguisher').split(",")]
 positive_typemap = [family.get_family(str.strip(x)) for x in config_parser.get('ramses', 'type-mapping-positive').split(",")]
 
 negative_typemap = [family.get_family(str.strip(x)) for x in config_parser.get('ramses', 'type-mapping-negative').split(",")]
 
-def read_descriptor(fname):
+def _read_descriptor(fname):
+    """Read a RAMSES file descriptor and return a list of the variable names."""
     description = []
     name_mapping = namemapper.AdaptiveNameMapper('ramses-name-mapping')
     with open(fname) as fd:
         if fd.readline() != "# version:  1\n":
             raise OSError("Wrong file format")
         fd.readline()  # ivar, variable_name, variable_type
         for line in fd.readlines():
             i, name, dtype = (_.strip() for _ in line.split(","))
 
             description.append(name_mapping(name, reverse=True))
     return description
 
 
 class RamsesSnap(SimSnap):
+    """Implements loading of Ramses snapshots.
+
+    Note that AMR cells are loaded as particles, although this works surprisingly well for most analysis purposes.
+    In particular SPH image generation routines automatically switch on an appropriate de-noising scheme to provide
+    effective interpolation between cells.
+    """
     reader_pool = None
 
-    def __init__(
-        self,
-        dirname,
-        cpus=None,
-        maxlevel=None,
-        with_gas=True,
-        force_gas=False,
-        times_are_proper=None,
-    ):
+    def __init__(self, dirname, cpus=None, maxlevel=None, with_gas=True, force_gas=False, times_are_proper=None):
         """
         Initialize a RamsesSnap.
 
         Parameters
         ----------
         dirname : str
             Directory containing the RAMSES output
         cpus : list of int, optional
             A list of the CPU IDs to load. If not set, load all
             CPU's data.
         maxlevel : int, optional
             The maximum refinement level to load. If not set, the
             deepest level is loaded.
-        with_gas : bool
+        with_gas : bool, optional
             If False, never load any gas cells (particles only).
             Default is True
-        force_gas : bool
+        force_gas : bool, optional
             If True, load the AMR cells as "gas particles" even if
             they don't actually contain gas in the run. Default is
             False.
-        times_are_proper : bool
+        times_are_proper : bool, optional
             If True, the times in the output are assumed to be proper
             times. If False, they are assumed to be conformal. If
-            unset, assume proper for non-cosmological simulations
+            None (default), assume proper for non-cosmological simulations
             and conformal for cosmological ones.
         """
 
         global config
         super().__init__()
 
         self.__setup_parallel_reading()
@@ -488,15 +480,15 @@
     def _load_fluid_descriptors(self):
         types = ["hydro", "grav"]
         default_blocks = [hydro_blocks, grav_blocks]
         descriptors_fnames = [os.path.join(self._filename, f"{ftype}_file_descriptor.txt") for ftype in types]
 
         for desc_type, default_block, descriptor_fname in zip(types, default_blocks, descriptors_fnames):
             try:
-                block = read_descriptor(descriptor_fname)
+                block = _read_descriptor(descriptor_fname)
             except (FileNotFoundError, OSError):
                 block = default_block
 
             setattr(self, f"_{desc_type}_blocks", block)
 
     def _load_rt_infofile(self):
         self._rt_blocks = []
@@ -1058,15 +1050,16 @@
             from ..analysis import ramses_util
 
             # Replace the tform array by its usual meaning using the birth files
             ramses_util.get_tform(self, times_are_proper=self.times_are_proper)
 
 
     @property
-    def times_are_proper(self):
+    def times_are_proper(self) -> bool:
+        """Best guess for whether the times in the output (e.g. star formation times) are proper times"""
         if hasattr(self, "_is_using_proper_time"):
             # Already set, skipping
             pass
         elif config_parser.has_option("ramses", "proper_time"):
             self.times_are_proper = config_parser.getboolean(
                 "ramses", "proper_time"
             )
@@ -1213,15 +1206,15 @@
         tsid = _timestep_id(f)
         if tsid:
             return os.path.isdir(f) and os.path.exists(os.path.join(f, f"info_{tsid}.txt"))
         return False
 
 
 @RamsesSnap.decorator
-def translate_info(sim):
+def _translate_info(sim):
 
     if sim._info['H0']>1e-3:
         sim.properties['a'] = sim._info['aexp']
         sim.properties['omegaM0'] = sim._info['omega_m']
         sim.properties['omegaL0'] = sim._info['omega_l']
         sim.properties['h'] = sim._info['H0'] / 100.
 
@@ -1237,24 +1230,27 @@
         sim.properties['time'] = sim._info['time'] * t_unit
     else:
         sim.properties["time"] = age(sim, unit="Gyr") * units.Unit("Gyr")
 
     sim._file_units_system = [d_unit, t_unit, l_unit]
 
 
-@RamsesSnap.derived_quantity
+@RamsesSnap.derived_array
 def mass(sim):
+    """Gas mass estimated from cell size and density"""
     return sim['rho'] * sim['smooth'] ** 3
 
 
-@RamsesSnap.derived_quantity
+@RamsesSnap.derived_array
 def temp(sim):
-    """ Gas temperature derived from pressure and density """
+    """Gas temperature derived from pressure and density """
+
     # Has to be redefined and rederived here from Ramses native variables
     # to avoid running into circular dependencies with the traditional derived definition
     # Now uses the self-consistent molecular weight field from pynbody (issue 598)
+
     from ..derived import mu
     mu_est = array.SimArray(np.ones(len(sim)), units="1")
     for i in range(5):
         temp = ((sim['p'] / sim['rho']) * (mu_est * units.m_p / units.k)).in_units("K")
         mu_est = mu(sim, t0=temp)
     return temp
```

### Comparing `pynbody-2.0.0b7/pynbody/snapshot/simsnap.py` & `pynbody-2.0.0b8/pynbody/snapshot/simsnap.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,94 +1,64 @@
+"""Implementation of the key simulation snapshot class.
+
+In a sense this is the core of pynbody, as it is the class that manages data and is subclasses to provide
+IO for different simulation formats.
+
+For an introduction, see :doc:`/tutorials/data_access`."""
+
 from __future__ import annotations
 
 import copy
 import gc
 import hashlib
 import logging
 import pathlib
 import re
 import threading
 import traceback
 import typing
 import warnings
 import weakref
 from functools import reduce
+from typing import Iterator
 
 import numpy as np
 
 from .. import (
     array,
     dependencytracker,
     family,
     filt,
-    iter_subclasses,
     simdict,
+    transformation,
     units,
     util,
 )
 from ..units import has_units
+from ..util import iter_subclasses
 from .util import ContainerWithPhysicalUnitsOption
 
 if typing.TYPE_CHECKING:
-    from .. import halo
+    from .. import bridge, halo, subsnap, transformation
+
 
 logger = logging.getLogger('pynbody.snapshot.simsnap')
 
-class SimSnap(ContainerWithPhysicalUnitsOption, iter_subclasses.IterableSubclasses):
+class SimSnap(ContainerWithPhysicalUnitsOption, iter_subclasses.IterableSubclasses, transformation.Transformable):
 
     """The class for managing simulation snapshots.
 
-    For most purposes, SimSnaps should be initialized through
-    :func:`~pynbody.load` or :func:`~pynbody.new`.
-
-    For a basic tutorial explaining how to load a file as a SimSnap
-    see :doc:`tutorials/data_access`.
-
-    *Getting arrays or subsnaps*
-
-    Once a :class:`SimSnap` object ``f`` is instantiated, it can
-    be used in various ways. The most common operation is to
-    access something with the code ``f[x]``.  Depending on the
-    type of ``x``, various behaviours result:
-
-    - If ``x`` is a string, the array named by ``x`` is returned. If
-      no such array exists, the framework attempts to load or
-      derive an array of that name (in that order). If this is
-      unsuccessful, a `KeyError` is raised.
-
-    - If ``x`` is a python `slice` (e.g. ``f[5:100:3]``) or an array of
-      integers (e.g. ``f[[1,5,100,200]]``) a subsnap containing only the
-      mentioned particles is returned.
-
-      See :doc:`tutorials/data_access` for more information.
-
-    - If ``x`` is a numpy array of booleans, it is interpreted as a mask and
-      a subsnap containing only those particles for which x[i] is True.
-      This means that f[condition] is a shortcut for f[np.where(condition)].
-
-    - If ``x`` is a :class:`pynbody.filt.Filter` object, a subsnap
-      containing only the particles which pass the filter condition
-      is returned.
-
-      See :doc:`tutorials/data_access` for more information.
-
-    - If ``x`` is a :class:`pynbody.family.Family` object, a subsnap
-      containing only the particles in that family is returned. In practice
-      for most code it is more convenient to write e.g. ``f.dm`` in place of
-      the equivalent syntax f[pynbody.family.dm].
-
-    *Getting metadata*
+    For most purposes, SimSnaps should be initialized through :func:`~pynbody.snapshot.load`
+    or :func:`~pynbody.snapshot.new`.
 
-    The property `filename` gives the filename of a snapshot.
+    For an introduction to using this class, see :doc:`/tutorials/data_access`.
 
-    There is also a `properties` dictionary which
-    contains further metadata about the snapshot. See :ref:`subsnaps`.
     """
 
-    _derived_quantity_registry = {}
+    _derived_array_registry = {}
 
     _decorator_registry = {}
 
     _loadable_keys_registry = {}
     _persistent = ["kdtree", "_immediate_cache", "_kdtree_derived_smoothing"]
 
     # These 3D arrays get four views automatically created, one reflecting the
@@ -155,17 +125,17 @@
         # this should be implemented by subclasses that can load from disk
         return False
 
 
     def __init__(self):
         """Initialize an empty, zero-length SimSnap.
 
-        For most purposes SimSnaps should instead be initialized through
-       :func:`~pynbody.load` or :func:`~pynbody.new`.
-       """
+        For most purposes SimSnaps should instead be initialized through :func:`~pynbody.snapshot.load`
+        or :func:`~pynbody.snapshot.new`.
+        """
 
         super().__init__()
 
         self._arrays = {}
         self._num_particles = 0
         self._family_slice = {}
         self._family_arrays = {}
@@ -220,26 +190,27 @@
 
     ############################################
     # THE BASICS: SIMPLE INFORMATION
     ############################################
 
     @property
     def filename(self):
+        """The filename of the snapshot, if it was loaded from disk."""
         return self._filename
 
-    def __len__(self):
+    def __len__(self) -> int:
         return self._num_particles
 
     def __repr__(self):
         if self._filename != "":
             return "<SimSnap \"" + str(self._filename) + "\" len=" + str(len(self)) + ">"
         else:
             return "<SimSnap len=" + str(len(self)) + ">"
 
-    def families(self):
+    def families(self) -> list[family.Family]:
         """Return the particle families which have representitives in this SimSnap.
         The families are ordered by their appearance in the snapshot."""
         out = []
         start = {}
         for fam in family._registry:
             sl = self._get_family_slice(fam)
             if sl.start != sl.stop:
@@ -248,15 +219,15 @@
         out.sort(key=start.__getitem__)
         return out
 
     ############################################
     # THE BASICS: GETTING AND SETTING
     ############################################
 
-    def __getitem__(self, i):
+    def __getitem__(self, i) -> array.SimArray | subsnap.SubSnapBase :
         """Return either a specific array or a subview of this simulation. See
         the class documentation (:class:`SimSnap`) for more information."""
         from . import subsnap
 
         if isinstance(i, str):
             return self._get_array_with_lazy_actions(i)
         elif isinstance(i, slice):
@@ -496,167 +467,171 @@
                     pass
                 return
         object.__delattr__(self, name)
 
     ############################################
     # DICTIONARY EMULATION FUNCTIONS
     ############################################
-    def keys(self):
+    def keys(self) -> list[str]:
         """Return the directly accessible array names (in memory)"""
         return list(self._arrays.keys())
 
-    def has_key(self, name):
+    def has_key(self, name: str) -> bool:
         """Returns True if the array name is accessible (in memory)"""
         return name in self.keys()
 
-    def values(self):
+    def values(self) -> list[array.SimArray]:
         """Returns a list of the actual arrays in memory"""
         x = []
         for k in list(self.keys()):
             x.append(self[k])
         return x
 
-    def items(self):
+    def items(self) -> list[tuple[str, array.SimArray]]:
         """Returns a list of tuples describing the array
         names and their contents in memory"""
         x = []
         for k in list(self.keys()):
             x.append((k, self[k]))
         return x
 
-    def get(self, key, alternative=None):
+    def get(self, key, alternative=None) -> array.SimArray | None :
         """Standard python get method, returns self[key] if
         key in self else alternative"""
         try:
             return self[key]
         except KeyError:
             return alternative
 
-    def iterkeys(self):
+    def iterkeys(self) -> Iterator[str]:
+        """Iterator over the array names in memory"""
         yield from list(self.keys())
 
     __iter__ = iterkeys
 
-    def itervalues(self):
+    def itervalues(self) -> Iterator[array.SimArray]:
+        """Iterator over the arrays in memory"""
         for k in self:
             yield self[k]
 
-    def iteritems(self):
+    def iteritems(self) -> Iterator[tuple[str, array.SimArray]]:
+        """Iterator over the array names and their contents in memory"""
         for k in self:
             yield (k, self[k])
 
     ############################################
     # DICTIONARY-LIKE FUNCTIONS
     # (not in the normal interface for dictionaries,
     # but serving similar purposes)
     ############################################
 
-    def has_family_key(self, name):
+    def has_family_key(self, name: str) -> bool:
         """Returns True if the array name is accessible (in memory) for at least one family"""
         return name in self.family_keys()
 
-    def loadable_keys(self, fam=None):
+    def loadable_keys(self, fam=None) -> list[str]:
         """Returns a list of arrays which can be lazy-loaded from
         an auxiliary file."""
         return []
 
-    def derivable_keys(self):
+    def derivable_keys(self) -> list[str]:
         """Returns a list of arrays which can be lazy-evaluated."""
         res = []
         for cl in type(self).__mro__:
-            if cl in self._derived_quantity_registry:
-                res += list(self._derived_quantity_registry[cl].keys())
+            if cl in self._derived_array_registry:
+                res += list(self._derived_array_registry[cl].keys())
         return res
 
-    def all_keys(self):
+    def all_keys(self) -> list[str]:
         """Returns a list of all arrays that can be either lazy-evaluated
         or lazy loaded from an auxiliary file."""
         return self.derivable_keys() + self.loadable_keys()
 
-    def family_keys(self, fam=None):
+    def family_keys(self, fam=None) -> list[str]:
         """Return list of arrays which are not accessible from this
         view, but can be accessed from family-specific sub-views.
 
         If *fam* is not None, only those keys applying to the specific
         family will be returned (equivalent to self.fam.keys())."""
         if fam is not None:
             return [x for x in self._family_arrays if fam in self._family_arrays[x]]
         else:
             return list(self._family_arrays.keys())
 
     ############################################
     # ANCESTRY FUNCTIONS
     ############################################
 
-    def is_ancestor(self, other):
+    def is_ancestor(self, other) -> bool:
         """Returns true if other is a subview of self"""
 
         if other is self:
             return True
         elif hasattr(other, 'base'):
             return self.is_ancestor(other.base)
         else:
             return False
 
-    def is_descendant(self, other):
+    def is_descendant(self, other) -> bool:
         """Returns true if self is a subview of other"""
         return other.is_ancestor(self)
 
     @property
-    def ancestor(self):
+    def ancestor(self) -> SimSnap:
         """The original SimSnap from which this view is derived (potentially self)"""
         if hasattr(self, 'base'):
             return self.base.ancestor
         else:
             return self
 
-    def get_index_list(self, relative_to, of_particles=None):
-        """Get a list specifying the index of the particles in this view relative
-        to the ancestor *relative_to*, such that relative_to[get_index_list(relative_to)]==self."""
+    def get_index_list(self, relative_to, of_particles=None) -> np.ndarray:
+        """Get a list specifying the index of the particles in this view relative to the ancestor *relative_to*
+
+        The returned index list satisfies ``relative_to[get_index_list(relative_to)]==self``."""
 
         # Implementation for base snapshot
 
         if self is not relative_to:
             raise RuntimeError("Not a descendant of the specified simulation")
         if of_particles is None:
             of_particles = np.arange(len(self))
 
         return of_particles
 
     ############################################
     # SET-LIKE OPERATIONS FOR SUBSNAPS
     ############################################
-    def intersect(self, other, op=np.intersect1d):
+    def intersect(self, other, op=np.intersect1d) -> SimSnap:
         """Returns the set intersection of this simulation view with another view
         of the same simulation"""
 
         anc = self.ancestor
         if not anc.is_ancestor(other):
             raise RuntimeError("Parentage is not suitable")
 
         a = self.get_index_list(anc)
         b = other.get_index_list(anc)
         return anc[op(a, b)]
 
-    def union(self, other):
+    def union(self, other) -> SimSnap:
         """Returns the set union of this simulation view with another view
         of the same simulation"""
 
         return self.intersect(other, op=np.union1d)
 
-    def setdiff(self, other):
+    def setdiff(self, other) -> SimSnap:
         """Returns the set difference of this simulation view with another view
         of the same simulation"""
 
         return self.intersect(other, op=np.setdiff1d)
 
     ############################################
     # UNIT MANIPULATION
     ############################################
-    def conversion_context(self):
+    def conversion_context(self) -> dict[str, float]:
         """Return a dictionary containing a (scalefactor) and h
         (Hubble constant in canonical units) for this snapshot, ready for
         passing into unit conversion functions."""
         d = {}
         wanted = ['a', 'h']
         for x in wanted:
             if x in self.properties:
@@ -769,16 +744,19 @@
                             mass=self.infer_original_units('Msol'), persistent=False)
 
 
     def infer_original_units(self, dimensions):
         """Given a unit (or string) `dimensions`, returns a unit with the same
         physical dimensions which is in the unit schema of the current file."""
         dimensions = units.Unit(dimensions)
-        d = dimensions.dimensional_project(
-            self._file_units_system + ["a", "h"])
+        try:
+            d = dimensions.dimensional_project(
+                self._file_units_system + ["a", "h"])
+        except units.UnitsException:
+            return units.no_unit
         new_unit = reduce(lambda x, y: x * y, [
                           a ** b for a, b in zip(self._file_units_system, d)])
         return new_unit
 
     def _default_units_for(self, array_name):
         """Attempt to construct and return the units for the named array
         on disk, using what we know about the purpose of arrays (in config.ini)
@@ -788,62 +766,68 @@
         if u is not None:
             u = self.infer_original_units(u)
         return u
 
     def halos(self, *args, **kwargs) -> halo.HaloCatalogue:
         """Tries to instantiate a halo catalogue object for the given snapshot.
 
+        For introductory information about halo catalogues, see :ref:`halo_tutorial`, and the documentation for
+        :py:mod:`pynbody.halo`.
+
         Multiple catalogue classes are available in pynbody, and they are tried in turn until the first which
         accepted the request to load halos for this file.
 
         The order of catalogue class priority is either defined in the configuration file or can be passed
         as a 'priority' keyword argument, which should be a list of either class names or classes.
 
         For example
 
         >>> h = snap.halos(priority = ["HOPCatalogue", "AHFCatalogue", pynbody.halo.subfind.SubfindCatalogue])
 
         would try to load HOP halos, then AHF halos, then Subfind halos, before finally trying all other
         known halo classes in an arbitrary order.
 
-        Aarguments and keyword arguments other than `priority` are passed onto the individual halo loaders.
+        Arguments and keyword arguments other than `priority` are passed onto the individual halo loaders.
         If a given catalogue class does not accept the args/kwargs that you pass in, by definition it cannot
         be used; this can lead to 'silent' failures. To understand why a given class is not being instantiated
         by this method, the best option is to try _directly_ instantiating that class to reveal the error
-        explicitly."""
+        explicitly.
+        """
 
         from .. import config, halo
 
         priority = kwargs.pop('priority',
                               config['halo-class-priority'])
 
+        priority = [halo._fix_american_spelling(p) for p in priority]
+
         for c in halo.HaloCatalogue.iter_subclasses_with_priority(priority):
             try:
                 can_load = c._can_load(self, *args, **kwargs)
             except TypeError:
                 can_load = False
 
             if can_load:
                 return c(self, *args, **kwargs)
 
         raise RuntimeError("No halo catalogue found for %r" % str(self))
 
-    def bridge(self, other):
+    def bridge(self, other) -> bridge.AbstractBridge:
         """Tries to construct a bridge function between this SimSnap
         and another one.
 
         This function calls :func:`pynbody.bridge.bridge_factory`. For
         more information see :ref:`bridge-tutorial`, or the reference
         documentation for :py:mod:`pynbody.bridge`.
 
         """
         from .. import bridge
         return bridge.bridge_factory(self, other)
 
-    def load_copy(self):
+    def load_copy(self) -> SimSnap:
         """Tries to load a copy of this snapshot, using partial loading to select
         only a subset of particles corresponding to a given SubSnap"""
         from .. import load
         if getattr(self.ancestor,'partial_load',False):
             raise NotImplementedError("Cannot load a copy of data that was itself partial-loaded")
         return load(self.ancestor.filename, take=self.get_index_list(self.ancestor))
 
@@ -912,81 +896,45 @@
                         anc._autoconvert_array_unit(anc[f][v])
 
 
 
     ############################################
     # VECTOR TRANSFORMATIONS OF THE SNAPSHOT
     ############################################
-    def transform(self, matrix):
-        from .. import transformation
-        return transformation.transform(self, matrix)
-
-    def _transform(self, matrix):
-        """Transforms the snapshot according to the 3x3 matrix given."""
-
-        # NB though it might seem more efficient to access _arrays and
-        # _family_arrays directly, this would not work for SubSnaps.
-        snapshot_keys = self.keys()
-
-        for array_name in snapshot_keys:
-            ar = self[array_name]
-            if len(ar.shape) == 2 and ar.shape[1] == 3:
-                ar[:] = np.dot(matrix, ar.transpose()).transpose()
-
-        for fam in self.families():
-            family_keys = self[fam].keys()
-            family_keys_not_in_snapshot = set(family_keys) - set(snapshot_keys)
-            for array_name in family_keys_not_in_snapshot:
-                ar = self[fam][array_name]
-                if len(ar.shape) == 2 and ar.shape[1] == 3:
-                    ar[:] = np.dot(matrix, ar.transpose()).transpose()
-
-    def rotate_x(self, angle):
-        """Rotates the snapshot about the current x-axis by 'angle' degrees."""
-        angle *= np.pi / 180
-        return self.transform(np.array([[1,      0,             0],
-                                        [0, np.cos(angle), -np.sin(angle)],
-                                        [0, np.sin(angle),  np.cos(angle)]]))
-
-    def rotate_y(self, angle):
-        """Rotates the snapshot about the current y-axis by 'angle' degrees."""
-        angle *= np.pi / 180
-        return self.transform(np.array([[np.cos(angle),    0,   np.sin(angle)],
-                                        [0,                1,        0],
-                                        [-np.sin(angle),   0,   np.cos(angle)]]))
-
-    def rotate_z(self, angle):
-        """Rotates the snapshot about the current z-axis by 'angle' degrees."""
-        angle *= np.pi / 180
-        return self.transform(np.array([[np.cos(angle), -np.sin(angle), 0],
-                                        [np.sin(angle),  np.cos(angle), 0],
-                                        [0,             0,        1]]))
 
     def wrap(self, boxsize=None, convention='center'):
-        """Wraps the positions of the particles in the box to lie between
-        [-boxsize/2, boxsize/2].
+        """Wraps the positions of the particles in the box to lie in a chosen fundamental domain.
 
-        If no boxsize is specified, self.properties["boxsize"] is used."""
+        Parameters
+        ----------
+        boxsize : float | units.UnitBase, optional
+            The size of the box to wrap the particles in. If not specified, the boxsize is taken from the snapshot's
+            properties.
+
+        convention : str, optional
+            The convention to use for wrapping the particles. The default is 'center', which wraps the particles to lie
+            in the range [-boxsize/2, boxsize/2). Alternatively, 'upper' wraps the particles to lie in the range
+            [0, boxsize).
+        """
 
 
         if boxsize is None:
             boxsize = self.properties["boxsize"]
 
         if isinstance(boxsize, units.UnitBase):
-            boxsize = float(boxsize.ratio(self[
-                            "pos"].units, **self.conversion_context()))
+            boxsize = float(boxsize.ratio(self["pos"].units, **self.conversion_context()))
 
         if convention=='center':
             for coord in "x", "y", "z":
-                self[coord][np.where(self[coord] < -boxsize / 2)] += boxsize
+                self[coord][np.where(self[coord] <= -boxsize / 2)] += boxsize
                 self[coord][np.where(self[coord] > boxsize / 2)] -= boxsize
         elif convention=='upper':
             for coord in "x", "y", "z":
                 self[coord][np.where(self[coord] < 0)] += boxsize
-                self[coord][np.where(self[coord] > boxsize)] -= boxsize
+                self[coord][np.where(self[coord] >= boxsize)] -= boxsize
         else:
             raise ValueError("Unknown wrapping convention")
 
     ############################################
     # WRITING FUNCTIONS
     ############################################
     def write(self, fmt=None, filename=None, **kwargs):
@@ -1003,27 +951,34 @@
         else:
             fmt._write(self, filename, **kwargs)
 
     def write_array(self, array_name, fam=None, overwrite=False, **kwargs):
         """
         Write out the array with the specified name.
 
-        Some of the functionality is available via the
-        :func:`pynbody.array.SimArray.write` method, which calls the
-        present function with appropriate arguments.
+        Only a subset of SimSnap subclasses support this operation. If the subclass does not support it, an ``OSError``
+        will be raised.
+
+        .. seealso:: :meth:`pynbody.array.SimArray.write`
+
+        Parameters
+        ----------
+
+        array_name : str
+            the name of the array to write
 
-        **Input**
+        fam : str or list of str, optional
+            Write out only one family; or provide a list to write out a set of families.
 
-        *array_name* - the name of the array to write
+        overwrite : bool, optional
+            If True, overwrite the array on disk if it already exists. If False (default), an OSError will be raised
+            if the array already exists.
 
-        **Optional Keywords**
 
-        *fam* (None) - Write out only one family; or provide a list to
-         write out a set of families.
-         """
+        """
 
         # Determine whether this is a write or an update
         if fam is None:
             fam = self.families()
 
         # It's an update if we're not fully replacing the file on
         # disk, i.e. there exists a family f in self.families() but
@@ -1103,15 +1058,15 @@
         else:
             dims = (self._num_particles, ndim)
 
         if shared is None:
             shared = self._shared_arrays
 
         if source_array is None:
-            source_array = array._array_factory(dims, dtype, zeros, shared)
+            source_array = array.array_factory(dims, dtype, zeros, shared)
         else:
             assert isinstance(source_array, array.SimArray)
             assert source_array.shape == dims
 
         source_array._sim = weakref.ref(self)
         source_array._name = array_name
         source_array.family = None
@@ -1200,15 +1155,15 @@
         # if we get here, either the array cannot be promoted to simulation level, or that would
         # not be appropriate, so actually go ahead and create the family array
 
         if shared is None:
             shared = self._shared_arrays
 
         if source_array is None:
-            source_array = array._array_factory(dims, dtype, False, shared)
+            source_array = array.array_factory(dims, dtype, False, shared)
         else:
             assert isinstance(source_array, array.SimArray)
             assert source_array.shape == dims
         source_array._sim = weakref.ref(self)
         source_array._name = array_name
         source_array.family = family
 
@@ -1454,43 +1409,109 @@
 
         return self._arrays[name]
 
     ############################################
     # DERIVED ARRAY SYSTEM
     ############################################
     @classmethod
-    def derived_quantity(cl, fn):
-        if cl not in SimSnap._derived_quantity_registry:
-            SimSnap._derived_quantity_registry[cl] = {}
-        SimSnap._derived_quantity_registry[cl][fn.__name__] = fn
+    def derived_array(cls, fn):
+        """Function decorator to register a derivable quantity for all SimSnaps, or for a specific subclass.
+
+        Example usage:
+
+        >>> @pynbody.derived_array
+        ... def radius_squared(sim):
+        ...     return sim['x']**2 + sim['y']**2 + sim['z']**2
+
+        When a user tries to access the ``radius_squared`` array from any snapshot, the function will be called
+        and the result will be stored then returned. The function should take a single argument, the simulation object,
+        and return a numpy array or SimArray of the same length as the simulation.
+
+        The array will be automatically updated whenever arrays it relies upon for derivation are changed.
+
+        If instead of ``pynbody.derived_array``, a derived array associated with a specific subclass of
+        :class:`~pynbody.snapshot.SimSnap` is desired, one may use the following syntax:
+
+        >>> @MySimSnapSubclass.derived_array
+        ... def radius_squared(sim):
+        ...     return sim['x']**2 + sim['y']**2 + sim['z']**2
+
+        If the function has a docstring, it will be prepended with "Derived: " to indicate that it is a derived
+        quantity. If the derived array is being added for a specific subclass, a list of subclasses is also
+        included in the automatic modifications to the docstring.
+
+        For more information about derived quantities see :ref:`derived-quantities`.
+
+        .. versionchanged:: 2.0
+            The function name has been changed from ``derived_quantity`` to ``derived_array``. The old name is
+            still available but will be removed in a future version.
+        """
+        if cls not in SimSnap._derived_array_registry:
+            SimSnap._derived_array_registry[cls] = {}
+        SimSnap._derived_array_registry[cls][fn.__name__] = fn
         fn.__stable__ = False
+        cls._add_derived_to_doc(fn)
+
         return fn
 
     @classmethod
-    def stable_derived_quantity(cl, fn):
-        if cl not in SimSnap._derived_quantity_registry:
-            SimSnap._derived_quantity_registry[cl] = {}
-        SimSnap._derived_quantity_registry[cl][fn.__name__] = fn
-        fn.__stable__ = True
+    def _add_derived_to_doc(cls, fn):
+        if fn.__doc__ is None:
+            return
+        if cls is not SimSnap:
+            if fn.__doc__.startswith("Derived ["):
+                fn.__doc__ = f"Derived [{cls.__name__}, " + fn.__doc__[9:]
+            else:
+                fn.__doc__ = f"Derived [{cls.__name__}]: " + fn.__doc__
+        else:
+            if not fn.__doc__.startswith("Derived"):
+                fn.__doc__ = "Derived: " + fn.__doc__
+
+    @classmethod
+    def stable_derived_array(cls, fn):
+        """Function decorator to register a stable derivable quantity for all SimSnaps, or for a specific subclass.
 
+        A stable derived array is one that is not expected to change over the course of a simulation, and so is
+        only ever calculated once. Otherwise, it behaves just like a derived array; see
+        :func:`~pynbody.snapshot.simsnap.SimSnap.derived_array`.
+
+        If the function has a docstring, it will be prepended with "Derived: " to indicate that it is a derived
+        quantity. If the derived array is being added for a specific subclass, a list of subclasses is also
+        included in the automatic modifications to the docstring.
+
+        For more information about derived quantities see :ref:`derived-quantities`, and specifically the
+        subsection :ref:`stable-derived-quantities`.
+
+        .. versionchanged:: 2.0
+            The function name has been changed from ``stable_derived_quantity`` to ``stable_derived_array``. The old
+            name is still available but will be removed in a future version.
+        """
+
+        if cls not in SimSnap._derived_array_registry:
+            SimSnap._derived_array_registry[cls] = {}
+        SimSnap._derived_array_registry[cls][fn.__name__] = fn
+        fn.__stable__ = True
+        cls._add_derived_to_doc(fn)
         return fn
 
+
+
     def _find_deriving_function(self, name):
         for cl in type(self).__mro__:
-            if cl in self._derived_quantity_registry \
-                    and name in self._derived_quantity_registry[cl]:
-                return self._derived_quantity_registry[cl][name]
+            if cl in self._derived_array_registry \
+                    and name in self._derived_array_registry[cl]:
+                return self._derived_array_registry[cl][name]
         else:
             return None
 
     def _derive_array(self, name, fam=None):
         """Calculate and store, for this SnapShot, the derivable array 'name'.
         If *fam* is not None, derive only for the specified family.
 
-        This searches the registry of @X.derived_quantity functions
+        This searches the registry of @X.derived_array functions
         for all X in the inheritance path of the current class.
         """
         global config
 
         calculated = False
         fn = self._find_deriving_function(name)
         if fn:
@@ -1557,15 +1578,15 @@
                         if self.is_derived_array(d_ar, fam):
                             was_derived = True
                             del self[fam][d_ar]
                     if was_derived:
                         self._dirty(d_ar)
 
 
-    def is_derived_array(self, name, fam=None):
+    def is_derived_array(self, name, fam=None) -> bool:
         """Returns True if the array or family array of given name is
         auto-derived (and therefore read-only)."""
         fam = fam or self._unifamily
         if fam:
             return (name in self._family_derived_array_names[fam]) or name in self._derived_array_names
         elif name in list(self.keys()):
             return name in self._derived_array_names
@@ -1592,28 +1613,32 @@
 
         else:
             raise RuntimeError("Not a derived array")
 
     ############################################
     # CONVENIENCE FUNCTIONS
     ############################################
-    def mean_by_mass(self, name):
+    def mean_by_mass(self, name) -> float | units.UnitBase:
         """Calculate the mean by mass of the specified array."""
-        m = np.asanyarray(self["mass"])
-        ret = array.SimArray(
-            (self[name].transpose() * m).transpose().mean(axis=0) / m.mean(), self[name].units)
-
-        return ret
+        with self.immediate_mode:
+            mass = self['mass']
+            array = self[name]
+            mass_indexing = (slice(None), ) + (np.newaxis, ) * (len(array.shape) - 1)
+            return (mass[mass_indexing] * array).sum(axis=0) / mass.sum(axis=0)
 
     ############################################
     # SNAPSHOT DECORATION
     ############################################
 
     @classmethod
     def decorator(cl, fn):
+        """Register a decorator to be applied to all instances of a given class.
+
+        Decorators are called when a new instance of the class is created, and are passed the new instance as an
+        argument."""
         if cl not in SimSnap._decorator_registry:
             SimSnap._decorator_registry[cl] = []
         SimSnap._decorator_registry[cl].append(fn)
         return fn
 
     def _decorate(self):
         for cl in type(self).__mro__:
@@ -1621,15 +1646,15 @@
                 for fn in self._decorator_registry[cl]:
                     fn(self)
 
     ############################################
     # KD-Tree
     ############################################
 
-    def build_tree(self, num_threads=None, shared_mem=None):
+    def build_tree(self, num_threads=None, shared_mem=None) -> None:
         """Build a kdtree for SPH operations and for accelerating geometrical filters
 
         Parameters
         ----------
 
         num_threads : int, optional
             Number of threads to use for building and most operations on the tree.
@@ -1644,15 +1669,15 @@
             from ..configuration import config
             boxsize = self._get_boxsize_for_kdtree()
             self.kdtree = kdtree.KDTree(self['pos'], self['mass'],
                                         leafsize=config['sph']['tree-leafsize'],
                                         boxsize=boxsize, num_threads=num_threads,
                                         shared_mem=shared_mem)
 
-    def import_tree(self, serialized_tree, num_threads=None):
+    def import_tree(self, serialized_tree, num_threads=None) -> None:
         """Import a precomputed kdtree from a serialized form.
 
         Throws ValueError if the tree is not compatible with the snapshot (though
         does not protect against all possible incompatibilities, so use with care)."""
         from .. import kdtree
         self.kdtree = kdtree.KDTree.deserialize(self['pos'], self['mass'],
                                          serialized_tree,
@@ -1727,15 +1752,25 @@
                         new_snap[fam][k] = self_fam[k]
 
         new_snap.properties = copy.deepcopy(self.properties, memo)
         new_snap._file_units_system = copy.deepcopy(self._file_units_system, memo)
 
         return new_snap
 
-    def get_copy_on_access_simsnap(self):
+    def get_copy_on_access_simsnap(self) -> SimSnap:
         """Return a new SimSnap that copies data out of this one when accessed
 
         This provides a degree of isolation (e.g. modifications made to the arrays in the copy-on-access
         view are not reflected back into the original snapshot). It is intended for advanced use, e.g. by
         tangos."""
         from .copy_on_access import CopyOnAccessSimSnap
         return CopyOnAccessSimSnap(self)
+
+SimSnap.stable_derived_quantity = util.deprecated(SimSnap.stable_derived_array,
+                                              "stable_derived_quantity has been renamed to stable_derived_array")
+
+SimSnap.stable_derived_quantity.__doc__ = "Deprecated alias for :meth:`stable_derived_array`"
+
+SimSnap.derived_quantity = util.deprecated(SimSnap.derived_array,
+                                           "derived_quantity has been renamed to derived_array")
+
+SimSnap.derived_quantity.__doc__ = "Deprecated alias for :meth:`derived_array`"
```

### Comparing `pynbody-2.0.0b7/pynbody/snapshot/subsnap.py` & `pynbody-2.0.0b8/pynbody/snapshot/subsnap.py`

 * *Files 1% similar despite different names*

```diff
@@ -199,15 +199,15 @@
         if index_array is not None and iord_array is not None:
             raise ValueError(
                 "Cannot define a subsnap without both and index_array and iord_array.")
         if iord_array is not None:
             index_array = self._iord_to_index(iord_array)
 
         if isinstance(index_array, filt.Filter):
-            self._descriptor = index_array._descriptor
+            self._descriptor = "filtered"
             index_array = index_array.where(self._subsnap_base)[0]
 
         elif isinstance(index_array, tuple):
             if isinstance(index_array[0], np.ndarray):
                 index_array = index_array[0]
             else:
                 index_array = np.array(index_array)
```

### Comparing `pynbody-2.0.0b7/pynbody/snapshot/swift.py` & `pynbody-2.0.0b8/pynbody/snapshot/swift.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,18 +2,18 @@
 import pathlib
 import tempfile
 
 import h5py
 import numpy as np
 
 from .. import halo, units, util
-from .gadgethdf import GadgetHdfMultiFileManager, GadgetHDFSnap
+from .gadgethdf import GadgetHDFSnap, _GadgetHdfMultiFileManager
 
 
-class SwiftMultiFileManager(GadgetHdfMultiFileManager):
+class SwiftMultiFileManager(_GadgetHdfMultiFileManager):
 
     def __init__(self, filename: pathlib.Path, take_cells, take_region, mode='r'):
         self._take_cells = take_cells
 
         if take_cells is not None and take_region is not None:
             raise ValueError("Either take_cells or take_region must be specified, not both")
 
@@ -200,15 +200,16 @@
     def _get_units_from_hdf_attr(self, hdfattrs):
         this_unit = units.Unit("1")
         for k in hdfattrs.keys():
             if k.endswith('exponent'):
                 unitname = k.split(" ")[0]
                 exponent = util.fractions.Fraction.from_float(float(ExtractScalarWrapper(hdfattrs)[k])).limit_denominator()
 
-                this_unit *= self._hdf_unitvar.get(unitname, units.no_unit)**exponent
+                if exponent != 0:
+                    this_unit *= self._hdf_unitvar.get(unitname, units.no_unit)**exponent
 
         return this_unit
 
     def _init_unit_information(self):
         atr = ExtractScalarWrapper(self._hdf_files.get_unit_attrs())
         dist_unit = atr['Unit length in cgs (U_L)'] * units.cm
         mass_unit = atr['Unit mass in cgs (U_M)'] * units.g
@@ -216,22 +217,27 @@
         temp_unit = atr['Unit temperature in cgs (U_T)'] * units.K
         vel_unit = dist_unit / time_unit
 
         unitvar = {'U_V': vel_unit,
                    'U_L': dist_unit,
                    'U_M': mass_unit,
                    'U_t': time_unit,
-                   'U_T': temp_unit}
-
-        if self._is_cosmological():
-            dist_unit *= units.a
+                   'U_T': temp_unit,
+                   'a-scale': units.a,
+                   'h-scale': units.h}
 
 
         self._hdf_unitvar = unitvar
 
+        if self._is_cosmological():
+            # when using hdf-provided exponents, the scalefactor will automatically be included. However, if using
+            # infer_original_units, our best guess is that distances are comoving. So include the scalefactor
+            # in self._file_units_system but not in self._hdf_unitvar.
+            dist_unit = dist_unit * units.a
+
         self._file_units_system = [vel_unit, dist_unit, mass_unit, temp_unit]
 
     def halos(self, **kwargs):
         h = super().halos(**kwargs)
 
         if isinstance(h, halo.number_array.HaloNumberCatalogue):
             ignore = int(self._hdf_files.get_parameter_attrs()['FOF:group_id_default'])
```

### Comparing `pynbody-2.0.0b7/pynbody/snapshot/tipsy.py` & `pynbody-2.0.0b8/pynbody/snapshot/tipsy.py`

 * *Files 2% similar despite different names*

```diff
@@ -208,15 +208,15 @@
                             self_fam[name][mem_index] = buf[name][buf_index]
 
         f.close()
 
     def _update_loadable_keys(self):
         def is_readable_array(x):
             try:
-                with util.open_(x, 'r') as f:
+                with util.open_(x, 'rt') as f:
                     return int(f.readline()) == len(self)
             except ValueError:
                 # could be a binary file
                 with util.open_(x, 'rb') as f:
                     header = f.read(4)
                 if len(header) != 4:
                     return False
@@ -970,44 +970,44 @@
     Y_He = ((0.236 + 2.1 * metal) / 4.0) * (metal <= 0.1)
     Y_He += ((-0.446 * (metal - 0.1) / 0.9 + 0.446) / 4.0) * (metal > 0.1)
     Y_H = 1.0 - Y_He * 4. - metal
 
     return Y_H, Y_He
 
 
-@TipsySnap.derived_quantity
+@TipsySnap.derived_array
 def HII(sim):
     """Number of HII ions per proton mass"""
     Y_H, Y_He = _abundance_estimator(sim["metals"])
     try:
         return Y_H - sim["HI"] - 2 * sim["H2"]
     except KeyError:
         return Y_H - sim["HI"]
 
 
-@TipsySnap.derived_quantity
+@TipsySnap.derived_array
 def HeIII(sim):
     """Number of HeIII ions per proton mass"""
     Y_H, Y_He = _abundance_estimator(sim["metals"])
     return Y_He - sim["HeII"] - sim["HeI"]
 
 
-@TipsySnap.derived_quantity
+@TipsySnap.derived_array
 def ne(sim):
     """Number of electrons per proton mass"""
     return sim["HII"] + sim["HeII"] + 2 * sim["HeIII"]
 
 
-@TipsySnap.derived_quantity
+@TipsySnap.derived_array
 def hetot(self):
     """Helium mass fraction including correction based on metallicity"""
     return 0.236 + (2.1 * self['metals'])
 
 
-@TipsySnap.derived_quantity
+@TipsySnap.derived_array
 def hydrogen(self):
     """Hydrogen mass fraction including correction based on metallicity"""
     return 1.0 - self['metals'] - self['hetot']
 
 #from .tipsy import TipsySnap
 # Asplund et al (2009) ARA&A solar abundances (Table 1)
 # m_frac = 10.0^([X/H] - 12)*M_X/M_H*0.74
@@ -1026,120 +1026,120 @@
 XSOLC = 3.03e-3           # 2.39e-3
 XSOLN = 9.2e-4          # 7e-4
 XSOLNe = 1.66e-3          # 1.26e-3
 XSOLMg = 6.44e-4          # 7e-4
 XSOLSi = 7e-4          # 6.7e-4
 
 
-@TipsySnap.derived_quantity
+@TipsySnap.derived_array
 def feh(self):
     """Iron abundance [Fe/H] derived from tipsy array FeMassFrac, with solar
     values from Asplund et al 09"""
     minfe = np.amin(self['FeMassFrac'][np.where(self['FeMassFrac'] > 0)])
     self['FeMassFrac'][np.where(self['FeMassFrac'] == 0)] = minfe
     return np.log10(self['FeMassFrac'] / self['hydrogen']) - np.log10(XSOLFe / XSOLH)
 
 
-@TipsySnap.derived_quantity
+@TipsySnap.derived_array
 def oxh(self):
     """Oxygen abundance [O/H] derived from tipsy array FeMassFrac, with solar
     values from Asplund et al 09"""
     minox = np.amin(self['OxMassFrac'][np.where(self['OxMassFrac'] > 0)])
     self['OxMassFrac'][np.where(self['OxMassFrac'] == 0)] = minox
     return np.log10(self['OxMassFrac'] / self['hydrogen']) - np.log10(XSOLO / XSOLH)
 
 
-@TipsySnap.derived_quantity
+@TipsySnap.derived_array
 def ofe(self):
     """Oxygen-to-iron ratio [O/Fe] derived from tipsy arrays OxMassFrac and FeMassFrac
     with solar values from Asplund et al 09"""
     minox = np.amin(self['OxMassFrac'][np.where(self['OxMassFrac'] > 0)])
     self['OxMassFrac'][np.where(self['OxMassFrac'] == 0)] = minox
     minfe = np.amin(self['FeMassFrac'][np.where(self['FeMassFrac'] > 0)])
     self['FeMassFrac'][np.where(self['FeMassFrac'] == 0)] = minfe
     return np.log10(self['OxMassFrac'] / self['FeMassFrac']) - np.log10(XSOLO / XSOLFe)
 
 
-@TipsySnap.derived_quantity
+@TipsySnap.derived_array
 def mgfe(sim):
     """Magnesium-to-iron ratio [Mg/Fe] derived from tipsy arrays MgMassFrac and FeMassFrac
     with solar values from Asplund et al 09"""
     minmg = np.amin(sim['MgMassFrac'][np.where(sim['MgMassFrac'] > 0)])
     sim['MgMassFrac'][np.where(sim['MgMassFrac'] == 0)] = minmg
     minfe = np.amin(sim['FeMassFrac'][np.where(sim['FeMassFrac'] > 0)])
     sim['FeMassFrac'][np.where(sim['FeMassFrac'] == 0)] = minfe
     return np.log10(sim['MgMassFrac'] / sim['FeMassFrac']) - np.log10(XSOLMg / XSOLFe)
 
 
-@TipsySnap.derived_quantity
+@TipsySnap.derived_array
 def nefe(sim):
     """Neon-to-iron ratio [Ne/Fe] derived from tipsy arrays MgMassFrac and FeMassFrac
     with solar values from Asplund et al 09"""
     minne = np.amin(sim['NeMassFrac'][np.where(sim['NeMassFrac'] > 0)])
     sim['NeMassFrac'][np.where(sim['NeMassFrac'] == 0)] = minne
     minfe = np.amin(sim['FeMassFrac'][np.where(sim['FeMassFrac'] > 0)])
     sim['FeMassFrac'][np.where(sim['FeMassFrac'] == 0)] = minfe
     return np.log10(sim['NeMassFrac'] / sim['FeMassFrac']) - np.log10(XSOLNe / XSOLFe)
 
 
-@TipsySnap.derived_quantity
+@TipsySnap.derived_array
 def sife(sim):
     """Silicon-to-iron ratio [Si/Fe] derived from tipsy arrays MgMassFrac and FeMassFrac
     with solar values from Asplund et al 09"""
     minsi = np.amin(sim['SiMassFrac'][np.where(sim['SiMassFrac'] > 0)])
     sim['SiMassFrac'][np.where(sim['SiMassFrac'] == 0)] = minsi
     minfe = np.amin(sim['FeMassFrac'][np.where(sim['FeMassFrac'] > 0)])
     sim['FeMassFrac'][np.where(sim['FeMassFrac'] == 0)] = minfe
     return np.log10(sim['SiMassFrac'] / sim['FeMassFrac']) - np.log10(XSOLSi / XSOLFe)
 
 
-@TipsySnap.derived_quantity
+@TipsySnap.derived_array
 def c_s(self):
     """Ideal gas sound speed based on pressure and density"""
     #x = np.sqrt(5./3.*units.k*self['temp']*self['mu'])
     x = np.sqrt(5. / 3. * self['p'] / self['rho'])
     x.convert_units('km s^-1')
     return x
 
 
-@TipsySnap.derived_quantity
+@TipsySnap.derived_array
 def c_s_turb(self):
     """Turbulent sound speed (from Mac Low & Klessen 2004)"""
     x = np.sqrt(self['c_s'] ** 2 + 1. / 3 * self['v_disp'] ** 2)
     x.convert_units('km s^-1')
     return x
 
 
-@TipsySnap.derived_quantity
+@TipsySnap.derived_array
 def mjeans(self):
     """Classical Jeans mass"""
     x = np.pi ** (5. / 2.) * self['c_s'] ** 3 / \
         (6. * units.G ** (3, 2) * self['rho'] ** (1, 2))
     x.convert_units('Msol')
     return x
 
 
-@TipsySnap.derived_quantity
+@TipsySnap.derived_array
 def mjeans_turb(self):
     """Turbulent Jeans mass"""
     x = np.pi ** (5. / 2.) * self['c_s_turb'] ** 3 / \
         (6. * units.G ** (3, 2) * self['rho'] ** (1, 2))
     x.convert_units('Msol')
     return x
 
 
-@TipsySnap.derived_quantity
+@TipsySnap.derived_array
 def ljeans(self):
     """Jeans length"""
     x = self['c_s'] * np.sqrt(np.pi / (units.G * self['rho']))
     x.convert_units('kpc')
     return x
 
 
-@TipsySnap.derived_quantity
+@TipsySnap.derived_array
 def ljeans_turb(self):
     """Turbulent Jeans length"""
     x = self['c_s_turb'] * np.sqrt(np.pi / (units.G * self['rho']))
     x.convert_units('kpc')
     return x
```

### Comparing `pynbody-2.0.0b7/pynbody/sph/__init__.py` & `pynbody-2.0.0b8/pynbody/sph/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -53,15 +53,15 @@
     if not _kernel_suitable_for_denoise(kernel):
         return False
     elif isinstance(sim.ancestor,snapshot.ramses.RamsesSnap):
         return True
     else:
         return False
 
-@pynbody.snapshot.simsnap.SimSnap.stable_derived_quantity
+@pynbody.snapshot.simsnap.SimSnap.stable_derived_array
 def smooth(self):
     self.build_tree()
 
     logger.info('Smoothing with %d nearest neighbours' %
                 config['sph']['smooth-particles'])
 
     sm = array.SimArray(np.empty(len(self['pos']), dtype=self['pos'].dtype), self['pos'].units)
@@ -83,15 +83,15 @@
             smooth_ar = smooth(self)
         else:
             smooth_ar = self['smooth']
     else:
         self['smooth'] = smooth_ar = smooth(self)
     return smooth_ar
 
-@pynbody.snapshot.simsnap.SimSnap.stable_derived_quantity
+@pynbody.snapshot.simsnap.SimSnap.stable_derived_array
 def rho(self):
     self.build_tree()
 
 
     logger.info('Calculating SPH density')
     rho = array.SimArray(
         np.empty(len(self['pos'])), self['mass'].units / self['pos'].units ** 3,
@@ -387,19 +387,20 @@
 
 
 def render_image(snap, qty='rho', x2=100, nx=500, y2=None, ny=None, x1=None,
                  y1=None, z_plane=0.0, out_units=None, xy_units=None,
                  kernel=Kernel(),
                  z_camera=None,
                  smooth='smooth',
-                 smooth_in_pixels=False,
+                 smooth_min=0.0,
                  force_quiet=False,
                  approximate_fast=_approximate_image,
                  threaded=None,
-                 denoise=None):
+                 denoise=None,
+                 z_range=None):
     """
     Render an SPH image using a typical (mass/rho)-weighted 'scatter'
     scheme.
 
     **Keyword arguments:**
 
     *qty* ('rho'): The name of the array within the simulation to render
@@ -429,19 +430,21 @@
      assuming the kernel is suitable (i.e. is a projecting
      kernel). The camera is at the specified z coordinate looking
      towards -ve z, and each pixel represents a line-of-sight radially
      outwards from the camera. The width then specifies the width of
      the image in the z=0 plane. Particles too close to the camera are
      also excluded.
 
+     *z_range*: If set, only particles with z between z_range[0] and z_range[1] will be included
+
      *smooth*: The name of the array which contains the smoothing lengths
       (default 'smooth')
 
-     *smooth_in_pixels*: If True, the smoothing array contains the smoothing
-       length in image pixels, rather than in real distance units (default False)
+     *smooth_min*: The minimum smoothing length; if smoothing lengths fall below
+      this, they are artificially inflated to this value
 
      *approximate_fast*: if True, render high smoothing length particles at
        progressively lower resolution, resample and sum
 
      *denoise*: if True, divide through by an estimate of the discreteness noise.
        The returned image is then not strictly an SPH estimate, but this option
        can be useful to reduce noise especially when rendering AMR grids which
@@ -466,60 +469,65 @@
             _render_image, int(np.floor(np.log2(nx / 20))))
     else:
         base_renderer = _render_image
 
     if threaded is None:
         threaded = _get_threaded_image()
 
+    if isinstance(qty, str):
+        qty = snap[qty]
+
     if threaded:
         im = _threaded_render_image(base_renderer, snap, qty, x2, nx, y2, ny, x1, y1, z_plane,
                                     out_units, xy_units, kernel, z_camera, smooth,
-                                    smooth_in_pixels, True,
-                                    num_threads=threaded)
+                                    True,
+                                    num_threads=threaded, smooth_min = smooth_min, z_range=z_range)
     else:
         im = base_renderer(snap, qty, x2, nx, y2, ny, x1, y1, z_plane,
                            out_units, xy_units, kernel, z_camera, smooth,
-                           smooth_in_pixels, False)
+                           False, smooth_min = smooth_min, z_range=z_range)
 
     if denoise:
         # call self to render a 'flat field'
-        snap['__denoise_one'] = 1
-        im2 = render_image(snap, '__denoise_one', x2, nx, y2, ny, x1, y1, z_plane, None,
-                           xy_units, kernel, z_camera, smooth, smooth_in_pixels,
-                           force_quiet, approximate_fast, threaded, False)
-        del snap.ancestor['__denoise_one']
+        im2 = render_image(snap, np.ones(len(snap), dtype=qty.dtype), x2, nx, y2, ny, x1, y1, z_plane, None,
+                           xy_units, kernel, z_camera, smooth, smooth_min, True, approximate_fast, threaded, False,
+                           z_range=z_range)
         im2 = im / im2
         im2.units = im.units
         return im2
 
     else:
         return im
 
 
 def _render_image(snap, qty, x2, nx, y2, ny, x1,
                   y1, z_plane, out_units, xy_units, kernel, z_camera,
-                  smooth, smooth_in_pixels,  force_quiet,
-                  smooth_range=None, res_downgrade=None, snap_slice=None,
+                  smooth, force_quiet, smooth_min = 0.0,
+                  smooth_range=None, res_downgrade=None, snap_slice=None,z_range=None,
                   __threaded=False):
     """The single-threaded image rendering core function. External calls
     should be made to the render_image function."""
 
     global config
 
-    verbose = config["verbose"] and not force_quiet
-
     snap_proxy = {}
 
     # cache the arrays and take a slice of them if we've been asked to
-    for arname in 'x', 'y', 'z', 'pos', smooth, qty, 'rho', 'mass':
+    for arname in 'x', 'y', 'z', 'pos', smooth, 'rho', 'mass':
         snap_proxy[arname] = snap[arname]
         if snap_slice is not None:
             snap_proxy[arname] = snap_proxy[arname][snap_slice]
 
+    if snap_slice is not None:
+        qty = qty[snap_slice]
 
+    if units.has_units(qty):
+        qty_units = qty.units
+    else:
+        qty_units = 1.0
 
     in_time = time.time()
 
     if y2 is None:
         if ny is not None:
             y2 = x2 * float(ny) / nx
         else:
@@ -555,14 +563,21 @@
     if smooth_range is not None:
         smooth_lo = float(smooth_range[0])
         smooth_hi = float(smooth_range[1])
     else:
         smooth_lo = 0.0
         smooth_hi = 100000.0
 
+    if z_range is not None:
+        z_lo = float(z_range[0])
+        z_hi = float(z_range[1])
+    else:
+        z_lo = -np.inf
+        z_hi = np.inf
+
     nx = int(nx + .5)
     ny = int(ny + .5)
 
     result = np.zeros((ny, nx), dtype=np.float32)
 
     n_part = len(snap)
 
@@ -571,33 +586,38 @@
 
     x = snap_proxy['x'].in_units(xy_units)
     y = snap_proxy['y'].in_units(xy_units)
     z = snap_proxy['z'].in_units(xy_units)
 
     sm = snap_proxy[smooth]
 
-    if sm.units != x.units and not smooth_in_pixels:
+    if sm.units != x.units:
         sm = sm.in_units(x.units)
 
-    qty_s = qty
-    qty = snap_proxy[qty]
+    if isinstance(smooth_min, str):
+        smooth_min = units.Unit(smooth_min)
+
+    if units.is_unit(smooth_min):
+        smooth_min = smooth_min.ratio(x.units, **snap.conversion_context())
+
     mass = snap_proxy['mass']
     rho = snap_proxy['rho']
 
     if out_units is not None:
         # Calculate the ratio now so we don't waste time calculating
         # the image only to throw a UnitsException later
-        conv_ratio = (qty.units * mass.units / (rho.units * sm.units ** kernel.h_power)).ratio(out_units,
+
+        conv_ratio = (qty_units * mass.units / (rho.units * sm.units ** kernel.h_power)).ratio(out_units,
                                                                                                **snap.conversion_context())
 
     if z_camera is None:
         z_camera = 0.0
 
     result = _render.render_image(nx, ny, x, y, z, sm, x1, x2, y1, y2, z_camera, 0.0, qty, mass, rho,
-                                  smooth_lo, smooth_hi, kernel,
+                                  smooth_lo, smooth_hi, z_lo, z_hi, smooth_min, kernel,
                                   _calculate_wrapping_repeat_array(snap, x1, x2, xy_units),
                                   _calculate_wrapping_repeat_array(snap, y1, y2, xy_units))
 
     result = result.view(array.SimArray)
 
     # The weighting works such that there is a factor of (M_u/rho_u)h_u^3
     # where M-u, rho_u and h_u are mass, density and smoothing units
@@ -605,16 +625,15 @@
     # have been changed since load-time.
     if out_units is None:
         result *= (snap_proxy['mass'].units / (snap_proxy['rho'].units)).ratio(
             snap_proxy['x'].units ** 3, **snap_proxy['x'].conversion_context())
 
         # The following will be the units of outputs after the above conversion
         # is applied
-        result.units = snap_proxy[qty_s].units * \
-            snap_proxy['x'].units ** (3 - kernel.h_power)
+        result.units = qty_units * snap_proxy['x'].units ** (3 - kernel.h_power)
     else:
         result *= conv_ratio
         result.units = out_units
 
     result.sim = snap
     return result
 
@@ -913,16 +932,14 @@
 
     code+=file(os.path.join(os.path.dirname(__file__),'sph_spectra.c')).read()
 
     # before inlining, the views on the arrays must be standard np.ndarray
     # otherwise the normal numpy macros are not generated
     x,y,vz,temp,sm,qty, mass, rho = (q.view(np.ndarray) for q in (x,y,vz,temp,sm,qty, mass, rho))
 
-    if config['verbose']: print("Constructing SPH spectrum", file=sys.stderr)
-
     if config["tracktime"] :
         print("Beginning SPH render at %.2f s"%(time.time()-in_time), file=sys.stderr)
     #import pdb; pdb.set_trace()
     util.threadsafe_inline( code, ['tau', 'nvel', 'x', 'y', 'vz', 'temp', 'sm', 'v1', 'v2',
                    'nnucleons','qty', 'mass', 'rho'],verbose=2)
 
     if config["tracktime"] :
```

### Comparing `pynbody-2.0.0b7/pynbody/sph/_render.pyx` & `pynbody-2.0.0b8/pynbody/sph/_render.pyx`

 * *Files 1% similar despite different names*

```diff
@@ -129,14 +129,16 @@
                  np.ndarray[fused_input_type_2,ndim=1] sm,
                  fixed_input_type x1,fixed_input_type x2,fixed_input_type y1,
                  fixed_input_type y2,fixed_input_type z_camera, fixed_input_type z0,
                  np.ndarray[fused_input_type_3,ndim=1] qty,
                  np.ndarray[fused_input_type_4,ndim=1] mass,
                  np.ndarray[fused_input_type_5,ndim=1] rho,
                  fixed_input_type smooth_lo, fixed_input_type smooth_hi,
+                 fixed_input_type z_lo, fixed_input_type z_hi,
+                 fixed_input_type min_smooth,
                  kernel,
                  wrap_offsets_x=[0], wrap_offsets_y=[0]) :
 
     cdef fixed_input_type pixel_dx = (x2-x1)/nx
     cdef fixed_input_type pixel_dy = (y2-y1)/ny
     cdef fixed_input_type x_start = x1+pixel_dx/2
     cdef fixed_input_type y_start = y1+pixel_dy/2
@@ -182,14 +184,20 @@
         for wrap_offset_y in wrap_offsets_y :
             with nogil:
                 for i in range(n_part) :
                     # load particle details
                     x_i = x[i]+wrap_offset_x; y_i=y[i]+wrap_offset_y;
                     z_i=z[i]; sm_i = sm[i]; qty_i = qty[i]*mass[i]/rho[i]
 
+                    if z_i<z_lo or z_i>z_hi :
+                        continue
+
+                    if qty_i!=qty_i:
+                        continue
+
                     if z_camera!=0.0 :
                         # perspective image -
                         # update image bounds for the current z
                         if (z_i>z_camera and z_camera>0) or (z_i<z_camera and z_camera<0) :
                             # behind camera
                             continue
                         dz_i = z_camera-z_i
@@ -198,18 +206,22 @@
                         y1 = mid_y - per_z_dy*dz_i
                         y2 = mid_y + per_z_dy*dz_i
                         pixel_dx = (x2-x1)/nx
                         pixel_dy = (y2-y1)/ny
                         x_start = x1+pixel_dx/2
                         y_start = y1+pixel_dy/2
 
+                    # minimum smoothing can be specified to create a smoother image (esp useful for contour plots)
+                    if sm_i<min_smooth:
+                        sm_i = min_smooth
 
                     # check particle smoothing is within specified range
                     if sm_i<pixel_dx*smooth_lo or sm_i>pixel_dx*smooth_hi : continue
 
+
                     total_ptcls+=1
 
                     # check particle is within bounds
                     if not ((use_z*cmath.fabs(z_i-z0)<max_d_over_h*sm_i)
                             and x_i>x1-2*sm_i and x_i<x2+2*sm_i and y_i>y1-2*sm_i and y_i<y2+2*sm_i) :
                         continue
```

### Comparing `pynbody-2.0.0b7/pynbody/test_utils/gadget4_subfind_reader.py` & `pynbody-2.0.0b8/pynbody/test_utils/gadget4_subfind_reader.py`

 * *Files identical despite different names*

### Comparing `pynbody-2.0.0b7/pynbody/test_utils/pyread_gadget_hdf5.py` & `pynbody-2.0.0b8/pynbody/test_utils/pyread_gadget_hdf5.py`

 * *Files identical despite different names*

### Comparing `pynbody-2.0.0b7/pynbody/units.py` & `pynbody-2.0.0b8/pynbody/units.py`

 * *Files 3% similar despite different names*

```diff
@@ -446,21 +446,40 @@
 
         Prefactors are converted into exponent notation. Named units by default
         are represented by the string '\mathrm{unit_name}', although this can
         be overriden in the pynbody configuration files or by setting
         unit_name._latex."""
 
         if self._scale != 1:
-            x = ("%.2e" % self._scale).split('e')
-            s = x[0]
-            ex = x[1].lstrip('0+')
-            if len(ex) > 0 and ex[0] == '-':
-                ex = '-' + (ex[1:]).lstrip('0')
-            if ex != '':
-                s += r"\times 10^{" + ex + "}"
+            log10_scale = np.log10(abs(self._scale))
+
+            # if we can compactly express the scale without exponents, do so
+            force_no_exponent = str(self._scale).endswith(".0") and log10_scale < 4
+
+            if (log10_scale < 2.5 and log10_scale > -1.0) or force_no_exponent:
+                if log10_scale > 2.0:
+                    s = "%.1f" % self._scale
+                elif log10_scale > 1.0:
+                    s = "%.2f" % self._scale
+                elif log10_scale > 0.0:
+                    s = "%.3f" % self._scale
+                else:
+                    s = "%.4f" % self._scale
+
+                while "." in s and s.endswith("0") or s.endswith("."):
+                    s = s[:-1]
+            else:
+                x = ("%.2e" % self._scale).split('e')
+                s = x[0]
+                ex = x[1].lstrip('0+')
+                if len(ex) > 0 and ex[0] == '-':
+                    ex = '-' + (ex[1:]).lstrip('0')
+                if ex != '':
+                    s += r"\times 10^{" + ex + "}"
+
         else:
             s = ""
 
         for b, p in zip(self._bases, self._powers):
             if s != "":
                 s += r"\," + b.latex()
             else:
```

### Comparing `pynbody-2.0.0b7/pynbody/util/__init__.py` & `pynbody-2.0.0b8/pynbody/util/__init__.py`

 * *Files identical despite different names*

### Comparing `pynbody-2.0.0b7/pynbody/util/_util.pyx` & `pynbody-2.0.0b8/pynbody/util/_util.pyx`

 * *Files identical despite different names*

### Comparing `pynbody-2.0.0b7/pynbody/util/hdf_vds.py` & `pynbody-2.0.0b8/pynbody/util/hdf_vds.py`

 * *Files identical despite different names*

### Comparing `pynbody-2.0.0b7/pynbody.egg-info/PKG-INFO` & `pynbody-2.0.0b8/pynbody.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pynbody
-Version: 2.0.0b7
+Version: 2.0.0b8
 Summary: Light-weight astronomical N-body/SPH analysis for python
 Home-page: https://github.com/pynbody/pynbody/releases
 Author: The pynbody team
 Author-email: pynbody@googlegroups.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
```

### Comparing `pynbody-2.0.0b7/pynbody.egg-info/SOURCES.txt` & `pynbody-2.0.0b8/pynbody.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -6,37 +6,28 @@
 docs/acknowledge.rst
 docs/bibliography.rst
 docs/conf.py
 docs/index.rst
 docs/installation.rst
 docs/loaders.rst
 docs/pitfalls.rst
-docs/reference/analysis.rst
-docs/reference/convenience.rst
-docs/reference/derived.rst
-docs/reference/essentials.rst
+docs/_templates/autosummary/class.rst
+docs/_templates/autosummary/module.rst
 docs/reference/index.rst
-docs/reference/plot.rst
-docs/sphinxext/apigen.py
-docs/sphinxext/docscrape.py
-docs/sphinxext/docscrape_sphinx.py
-docs/sphinxext/inheritance_diagram.py
-docs/sphinxext/ipython_console_highlighting.py
-docs/sphinxext/ipython_directive.py
 docs/tutorials/bridge.rst
 docs/tutorials/configuration.rst
 docs/tutorials/data_access.rst
+docs/tutorials/derived.rst
 docs/tutorials/filters.rst
 docs/tutorials/halos.rst
 docs/tutorials/hmf.rst
 docs/tutorials/performance.rst
 docs/tutorials/pictures.rst
 docs/tutorials/profile.rst
-docs/tutorials/rotation_curve.rst
-docs/tutorials/snapshot_manipulation.rst
+docs/tutorials/quickstart.rst
 docs/tutorials/threads.rst
 docs/tutorials/tutorials.rst
 docs/tutorials/example_code/density_integrated.py
 docs/tutorials/example_code/density_profile.py
 docs/tutorials/example_code/density_slice.py
 docs/tutorials/example_code/do_data.py
 docs/tutorials/example_code/do_images.py
@@ -50,23 +41,23 @@
 docs/tutorials/example_code/velocity_vectors.py
 pynbody/__init__.py
 pynbody/configuration.py
 pynbody/default_config.ini
 pynbody/dependencytracker.py
 pynbody/derived.py
 pynbody/family.py
-pynbody/iter_subclasses.py
 pynbody/simdict.py
 pynbody/transformation.py
 pynbody/units.py
 pynbody.egg-info/PKG-INFO
 pynbody.egg-info/SOURCES.txt
 pynbody.egg-info/dependency_links.txt
 pynbody.egg-info/requires.txt
 pynbody.egg-info/top_level.txt
+pynbody/analysis/CAMB_Planck18
 pynbody/analysis/CAMB_WMAP7
 pynbody/analysis/__init__.py
 pynbody/analysis/_com.pyx
 pynbody/analysis/_interpolate3d.pyx
 pynbody/analysis/angmom.py
 pynbody/analysis/cambtemplate.ini
 pynbody/analysis/cmdlum.npz
@@ -83,39 +74,26 @@
 pynbody/analysis/luminosity.py
 pynbody/analysis/pkdgrav_cosmo.py
 pynbody/analysis/profile.py
 pynbody/analysis/ramses_util.py
 pynbody/analysis/theoretical_profiles.py
 pynbody/array/__init__.py
 pynbody/array/shared.py
-pynbody/bc_modules/__init__.py
-pynbody/bc_modules/capsulethunk.h
 pynbody/bridge/__init__.py
 pynbody/bridge/_bridge.pyx
 pynbody/chunk/__init__.py
 pynbody/chunk/scan.pyx
 pynbody/extern/__init__.py
 pynbody/extern/_cython_fortran_utils.pyx
 pynbody/extern/cython_fortran_utils.py
 pynbody/filt/__init__.py
 pynbody/filt/geometry_selection.pyx
 pynbody/gravity/__init__.py
 pynbody/gravity/_gravity.pyx
 pynbody/gravity/calc.py
-pynbody/gravity/config.h
-pynbody/gravity/grav.c
-pynbody/gravity/ilc.h
-pynbody/gravity/ilp.h
-pynbody/gravity/kd.h
-pynbody/gravity/main.c
-pynbody/gravity/moments.c
-pynbody/gravity/moments.h
-pynbody/gravity/serialtree.c
-pynbody/gravity/tree.py
-pynbody/gravity/walk.c
 pynbody/halo/__init__.py
 pynbody/halo/adaptahop.py
 pynbody/halo/ahf.py
 pynbody/halo/hbtplus.py
 pynbody/halo/hop.py
 pynbody/halo/number_array.py
 pynbody/halo/rockstar.py
@@ -137,14 +115,15 @@
 pynbody/openmp/openmp_null.pyx
 pynbody/openmp/openmp_real.pyx
 pynbody/plot/__init__.py
 pynbody/plot/gas.py
 pynbody/plot/generic.py
 pynbody/plot/metals.py
 pynbody/plot/profile.py
+pynbody/plot/quiverkey.py
 pynbody/plot/sph.py
 pynbody/plot/stars.py
 pynbody/plot/tollerud2008mw
 pynbody/plot/util.py
 pynbody/snapshot/__init__.py
 pynbody/snapshot/ascii.py
 pynbody/snapshot/copy_on_access.py
@@ -163,14 +142,15 @@
 pynbody/sph/_render.pyx
 pynbody/test_utils/__init__.py
 pynbody/test_utils/gadget4_subfind_reader.py
 pynbody/test_utils/pyread_gadget_hdf5.py
 pynbody/util/__init__.py
 pynbody/util/_util.pyx
 pynbody/util/hdf_vds.py
+pynbody/util/iter_subclasses.py
 tests/adaptahop_test.py
 tests/ahf_halos_test.py
 tests/array_test.py
 tests/bridge_test.py
 tests/copy_on_access_test.py
 tests/cosmology_test.py
 tests/derived_arrays_test.py
@@ -179,14 +159,15 @@
 tests/gadget_test.py
 tests/gadgethdf_test.py
 tests/grafic_test.py
 tests/gravity_test.py
 tests/halos_test.py
 tests/halotools_test.py
 tests/hbtplus_test.py
+tests/hmf_test.py
 tests/hop_test.py
 tests/import_test.py
 tests/kdtree_test.py
 tests/nchilada_test.py
 tests/partial_tipsy_test.py
 tests/performance_kdtree.py
 tests/ramses_new_ptcl_format_test.py
```

### Comparing `pynbody-2.0.0b7/pyproject.toml` & `pynbody-2.0.0b8/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -12,14 +12,16 @@
     'ignore:Namelist file either not found or unable to read.*assuming flat LCDM:UserWarning',
     'ignore:More hydro variables.*:RuntimeWarning',
     # ignore other common farily harmless scenarios:
     'ignore:Conjoining derived and non-derived arrays.*:RuntimeWarning',
     'ignore:invalid value encountered in multiply:RuntimeWarning',
     # ignore deprecation warnings triggered by h5py with python 3.12
     'ignore:datetime.datetime.utcfromtimestamp\(\) is deprecated:DeprecationWarning',
+    # ignore integration warnings which come up
+    'ignore:The occurrence of roundoff error:UserWarning'
   ]
 
 [tool.isort]
 profile = "black"
 combine_as_imports = true
 known_third_party = [
   "IPython",
```

### Comparing `pynbody-2.0.0b7/setup.py` & `pynbody-2.0.0b8/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -150,22 +150,26 @@
     'matplotlib>=3.0.0',
     'numpy>=1.21.6',
     'scipy>=1.0.0',
     'posix-ipc>=1.1.0'
 ]
 
 tests_require = [
-    'pytest','pandas'
+    'pytest','pandas','camb'
 ]
 
 docs_require = [
     'ipython>=3',
     'Sphinx>=7',
-    'sphinx-bootstrap-theme',
+    'sphinx-book-theme',
+    'sphinx-copybutton',
     'numpydoc',
+    'extinction',
+    'nbsphinx',
+    'camb'
 ],
 
 extras_require = {
     'tests': tests_require,
     'docs': docs_require,
 }
 
@@ -182,23 +186,23 @@
 setup(name = 'pynbody',
       author = 'The pynbody team',
       author_email = 'pynbody@googlegroups.com',
       version = get_version("pynbody/__init__.py"),
       description = 'Light-weight astronomical N-body/SPH analysis for python',
       url = 'https://github.com/pynbody/pynbody/releases',
       package_dir = {'pynbody/': ''},
-      packages = ['pynbody', 'pynbody/analysis', 'pynbody/bc_modules', 'pynbody/array',
+      packages = ['pynbody', 'pynbody/analysis', 'pynbody/array',
                   'pynbody/plot', 'pynbody/gravity', 'pynbody/chunk', 'pynbody/filt', 'pynbody/sph',
                   'pynbody/snapshot', 'pynbody/bridge', 'pynbody/halo', 'pynbody/halo/details',
                   'pynbody/extern', 'pynbody/kdtree', 'pynbody/test_utils', 'pynbody/util'],
       package_data={'pynbody': ['default_config.ini'],
                     'pynbody/analysis': ['cmdlum.npz',
                                          'h1.hdf5',
                                          'ionfracs.npz',
-                                         'CAMB_WMAP7',
+                                         'CAMB_WMAP7', 'CAMB_Planck18',
                                          'cambtemplate.ini'],
                     'pynbody/plot': ['tollerud2008mw']},
       ext_modules = ext_modules,
       classifiers = ["Development Status :: 4 - Beta",
                      "Intended Audience :: Developers",
                      "Intended Audience :: Science/Research",
                      "License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)",
```

### Comparing `pynbody-2.0.0b7/tests/adaptahop_test.py` & `pynbody-2.0.0b8/tests/adaptahop_test.py`

 * *Files 1% similar despite different names*

```diff
@@ -218,15 +218,15 @@
     ),
 )
 def test_longint_contamination_autodetection(f, fname, Halo_T, ans):
     # Note: we hack things a little bit here because
     # we just want to make sure the longint/contamination
     # flags are properly detected.
 
-    halos = Halo_T(f, fname=fname)
+    halos = Halo_T(f, filename=fname)
     assert halos._longint == ans["_longint"]
     assert halos._read_contamination == ans["_read_contamination"]
 
 def test_halo_iteration(halos):
     h = list(halos)
 
     assert len(h) == len(halos)
@@ -241,11 +241,11 @@
     f_with_tracers = pynbody.new(gas_tracer=100, dm=len(f.dm), star=len(f.star), gas=len(f.gas))
     f_with_tracers.dm['iord'] = f.dm['iord']
     f_with_tracers.properties.update(f.properties)
 
     halos = f.halos()
 
     halos2 = pynbody.halo.adaptahop.NewAdaptaHOPCatalogue(f_with_tracers,
-                                 fname = "testdata/new_adaptahop_output_00080/Halos/tree_bricks080")
+                                                          filename="testdata/new_adaptahop_output_00080/Halos/tree_bricks080")
 
     assert (halos2[1].dm['iord'] == halos[1].dm['iord']).all()
     assert (halos2[2].dm['iord'] == halos[2].dm['iord']).all()
```

### Comparing `pynbody-2.0.0b7/tests/ahf_halos_test.py` & `pynbody-2.0.0b8/tests/ahf_halos_test.py`

 * *Files 4% similar despite different names*

```diff
@@ -21,14 +21,22 @@
 
 
 def test_load_ahf_catalogue():
     f = pynbody.load("testdata/gasoline_ahf/g15784.lr.01024")
     h = pynbody.halo.ahf.AHFCatalogue(f)
     assert len(h)==1411
 
+def test_load_ahf_catalogue_via_filename():
+    f = pynbody.load("testdata/gasoline_ahf/g15784.lr.01024")
+    f._filename = '' # obfuscate the filename, so we can check loading via user-specified filename
+
+    h = f.halos(filename="testdata/gasoline_ahf/g15784.lr.01024.z0.000.AHF")
+    assert isinstance(h, pynbody.halo.ahf.AHFCatalogue)
+    assert len(h)==1411
+
 h0_sample_iords = [57, 27875, 54094, 82969, 112002, 140143, 173567, 205840, 264606,
            301694, 333383, 358730, 374767, 402300, 430180, 456015, 479885, 496606,
            519824, 539971, 555195, 575204, 596047, 617669, 652724, 1533992, 1544021,
            1554045, 1564080, 1574107, 1584130, 1594158, 1604204, 1614257, 1624308, 1634376,
            1644485, 1654580, 1664698, 1674831, 1685054, 1695252, 1705513, 1715722, 1725900,
            1736070, 1746235, 1756400, 1766584, 1776754, 1786886]
```

### Comparing `pynbody-2.0.0b7/tests/array_test.py` & `pynbody-2.0.0b8/tests/array_test.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,18 +1,20 @@
 import pynbody
-import pynbody.array
+import pynbody.array as pyn_array
 import pynbody.array.shared as shared
 
 SA = pynbody.array.SimArray
+import gc
 import os
 import signal
 import sys
 import time
 
 import numpy as np
+import numpy.testing as npt
 import pytest
 
 
 def test_pickle():
     import pickle
     x = SA([1, 2, 3, 4], units='kpc')
     assert str(x.units) == 'kpc'
@@ -111,20 +113,27 @@
     assert id(x) == x_id
 
 
 def test_unit_array_interaction():
     """Test for issue 113 and related"""
     x = pynbody.units.Unit('1 Mpc')
     y = SA(np.ones(10), 'kpc')
-    assert all(x + y == SA([1.001] * 10, 'Mpc'))
-    assert all(x - y == SA([0.999] * 10, 'Mpc'))
+    npt.assert_allclose(x + y, SA([1.001] * 10, 'Mpc'))
+    npt.assert_allclose(x - y, SA([0.999] * 10, 'Mpc'))
+
     assert (x + y).units == 'Mpc'
-    assert all(y + x == SA([1.001] * 10, 'Mpc'))
-    assert all(y - x == SA([-999.] * 10, 'kpc'))
 
+    npt.assert_allclose(y + x, SA([1.001] * 10, 'Mpc'))
+    npt.assert_allclose(y - x, SA([-999.] * 10, 'kpc'))
+
+def test_norm_units():
+    x = SA(np.ones((10, 3) ), "kpc")
+    result = np.linalg.norm(x, axis=1)
+    npt.assert_allclose(result, np.ones(10) * np.sqrt(3), rtol=1.e-5)
+    assert result.units == "kpc"
 
 def test_dimensionful_comparison():
     # check that dimensionful units compare correctly
     # see issue 130
     a1 = SA(np.ones(2), 'kpc')
     a2 = SA(np.ones(2) * 2, 'pc')
     assert (a2 < a1).all()
@@ -185,29 +194,25 @@
 
 
     np.testing.assert_allclose(sigvz, np.array([19.68325233, 29.49512482,  0.]), rtol=1e-6)
     np.testing.assert_allclose(sigvr, np.array([25.64306641, 26.01454544,  0.]), rtol=1e-6)
     np.testing.assert_allclose(sigvt, np.array([28.49997711, 18.84262276,  0.]), rtol=1e-6)
     np.testing.assert_allclose(rxy, np.array([1136892.125, 1606893.625, 1610494.75]), rtol=1e-6)
 
-
 def _test_and_alter_shared_value(array_info):
     array = pynbody.array.shared._shared_array_reconstruct(array_info)
     assert (array[:] == np.arange(3)[: , np.newaxis] * np.arange(5)[np.newaxis, :]).all()
     array[:] = np.arange(3)[:, np.newaxis]
 
 def test_shared_arrays():
-    import gc
-
-    import pynbody.array as pyn_array
 
     gc.collect() # this is to start with a clean slate, get rid of any shared arrays that might be hanging around
     baseline_num_shared_arrays = pyn_array.shared.get_num_shared_arrays_owned() # hopefully zero, but we can't guarantee that
 
-    ar = pyn_array._array_factory((3,5), dtype=np.float32, zeros=True, shared=True)
+    ar = pyn_array.array_factory((3, 5), dtype=np.float32, zeros=True, shared=True)
 
     assert ar.shape == (3,5)
     assert (ar == 0.0).all()
 
     ar[:] = np.arange(3)[: , np.newaxis] * np.arange(5)[np.newaxis, :]
 
     # now let's see if we can transfer it to another process:
@@ -219,22 +224,42 @@
     p.join()
 
     # check that the other process has successfully changed our value:
     assert (ar[:] ==  np.arange(3)[:, np.newaxis] ).all()
 
     assert pyn_array.shared.get_num_shared_arrays_owned() == 1 + baseline_num_shared_arrays
 
-    ar2 = pyn_array._array_factory((3,5), dtype=np.float32, zeros=True, shared=True)
+    ar2 = pyn_array.array_factory((3, 5), dtype=np.float32, zeros=True, shared=True)
     assert pyn_array.shared.get_num_shared_arrays_owned() == 2 + baseline_num_shared_arrays
 
     del ar, ar2
     gc.collect()
 
     assert pyn_array.shared.get_num_shared_arrays_owned() == baseline_num_shared_arrays
 
+def test_shared_array_ownership():
+    """Test that we can have two copies of a shared array in a process, but that only the 'owner' cleans up the memory"""
+
+    import pynbody.array as pyn_array
+
+    baseline_num_shared_arrays = pyn_array.shared.get_num_shared_arrays_owned()  # hopefully zero, but we can't guarantee that
+    ar = pyn_array.array_factory((10,), int, True, True)
+    assert pyn_array.shared.get_num_shared_arrays_owned() == 1 + baseline_num_shared_arrays
+
+    array_info = pyn_array.shared._shared_array_deconstruct(ar)
+    ar2 = pynbody.array.shared._shared_array_reconstruct(array_info)
+    del ar2
+
+    gc.collect()
+
+    # shouldn't have been deleted!
+    assert pyn_array.shared.get_num_shared_arrays_owned() == 1 + baseline_num_shared_arrays
+
+
+
 @pytest.fixture
 def clean_up_test_protection():
     import posix_ipc
     try:
         posix_ipc.unlink_shared_memory("pynbody-test-cleanup")
     except posix_ipc.ExistentialError:
         pass
```

### Comparing `pynbody-2.0.0b7/tests/copy_on_access_test.py` & `pynbody-2.0.0b8/tests/copy_on_access_test.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,15 +27,15 @@
         assert (f['blob'] == np.arange(10)).all()
 
 
 class ExampleSnap(pynbody.snapshot.simsnap.SimSnap):
     pass
 
 
-@ExampleSnap.derived_quantity
+@ExampleSnap.derived_array
 def foo(sim):
     return sim['blob']+5
 
 
 def test_copy_on_access_subsnap_emulating_class():
     f = pynbody.new(10, class_=ExampleSnap)
     f['blob'] = np.arange(10)
```

### Comparing `pynbody-2.0.0b7/tests/cosmology_test.py` & `pynbody-2.0.0b8/tests/cosmology_test.py`

 * *Files identical despite different names*

### Comparing `pynbody-2.0.0b7/tests/derived_arrays_test.py` & `pynbody-2.0.0b8/tests/derived_arrays_test.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import numpy as np
+import pytest
 
 import pynbody
 
 
 def setup_module():
     global f, h
     f = pynbody.new(dm=1000, star=500, gas=500, order='gas,dm,star')
@@ -101,22 +102,21 @@
         test_spherical_coordinates_arrays()
 
     # And another rotation
     with f.rotate_z(90):
         test_spherical_coordinates_arrays()
 
     # And translation + rotation
-    with pynbody.transformation.translate(f, pynbody.array.SimArray([-100, 140, 200], units='kpc')):
-        with f.rotate_x(173):
-            test_spherical_coordinates_arrays()
+    with f.translate(pynbody.array.SimArray([-100, 140, 200], units='kpc')).rotate_x(173):
+        test_spherical_coordinates_arrays()
 
 class ExampleSnap(pynbody.snapshot.SimSnap):
     pass
 
-@ExampleSnap.derived_quantity
+@ExampleSnap.derived_array
 def _test_quantity(sim):
     return sim['input']+2
 
 def test_derived_array_update():
     f = pynbody.new(10, class_=ExampleSnap)
     f['input'] = np.arange(0,10)
     assert (f['_test_quantity']==np.arange(2,12)).all()
@@ -142,7 +142,27 @@
     assert f.dm['_test_quantity'].derived
     assert not f.star['_test_quantity'].derived
 
     f['input']*=2
 
     assert (f.dm['_test_quantity']==np.arange(2,22,2)).all()
     assert (f.star['_test_quantity']==np.arange(-10,0)).all()
+
+
+def test_deprecated_derived_quantity():
+    with pytest.warns(DeprecationWarning):
+        @ExampleSnap.derived_quantity
+        def another_test_quantity(sim):
+            return sim['input'] + 2
+
+    with pytest.warns(DeprecationWarning):
+        @ExampleSnap.stable_derived_quantity
+        def another_test_quantity_stable(sim):
+            return sim['input'] + 4
+
+    f = pynbody.new(10, class_=ExampleSnap)
+    f['input'] = np.arange(0,10)
+    assert (f['another_test_quantity']==np.arange(2,12)).all()
+    assert (f['another_test_quantity_stable']==np.arange(4,14)).all()
+    f['input']+=2
+    assert (f['another_test_quantity']==np.arange(4,14)).all()
+    assert (f['another_test_quantity_stable']==np.arange(4,14)).all()
```

### Comparing `pynbody-2.0.0b7/tests/family_test.py` & `pynbody-2.0.0b8/tests/family_test.py`

 * *Files identical despite different names*

### Comparing `pynbody-2.0.0b7/tests/filter_test.py` & `pynbody-2.0.0b8/tests/filter_test.py`

 * *Files 16% similar despite different names*

```diff
@@ -41,14 +41,21 @@
     assert sp['x'].max() < 0.5
     assert sp['x'].min() > -0.5
     assert sp['r'].max() < 0.5
 
     sp_units = f[pynbody.filt.Sphere('500 pc')]
     assert len(sp_units.intersect(sp)) == len(sp)
 
+
+def test_empty_sphere():
+    snap = pynbody.new(0)
+    # This would fail due to the C code seeing an array it couldn't handle (due to zero length)
+    sp_empty = snap[pynbody.filt.Sphere(1.0)]
+    assert len(sp_empty) == 0
+
 def test_wrapping_sphere(wrapping_snap):
     f, min = wrapping_snap
     # put a sphere at the lower left corner of the box
     sp = f[pynbody.filt.Sphere(0.5, (min, min, min))]
 
     f['pos']-=np.array([min, min, min]) # put our sphere at the origin and re-wrap
     f.wrap()
@@ -152,14 +159,32 @@
     f_dm = f.dm
     f_dm_filter = f[pynbody.filt.FamilyFilter(pynbody.family.dm)]
     f_gas = f.gas
     f_gas_filter = f[pynbody.filt.FamilyFilter(pynbody.family.gas)]
     assert (f_dm.get_index_list(f) == f_dm_filter.get_index_list(f)).all()
     assert (f_gas.get_index_list(f) == f_gas_filter.get_index_list(f)).all()
 
+def test_annulus(snap):
+    a = snap[pynbody.filt.Annulus(0.5, 1.0)]
+    assert len(a)>100 and len(a)<200
+    assert (a.get_index_list(snap) == np.where(
+        (snap['r'] > 0.5) * (snap['r'] < 1.0))[0]).all()
+
+def test_disc(snap):
+    d = snap[pynbody.filt.Disc(0.8, 0.3)]
+    assert len(d)>50 and len(d)<100
+    assert (d.get_index_list(snap) == np.where(
+        (snap['rxy'] < 0.8) * (abs(snap['z']) < 0.3))[0]).all()
+
+def test_solar_neighbourhood(snap):
+    filt = pynbody.filt.SolarNeighborhood(0.5, 1.0, 0.3)
+    sn = snap[filt]
+    assert len(sn) > 50 and len(sn) < 100
+    assert (sn.get_index_list(snap) == np.where(
+        (snap['rxy'] > 0.5) * (snap['rxy'] < 1.0) * (abs(snap['z']) < 0.3))[0]).all()
 
 def test_hashing():
     X = {}
     X[pynbody.filt.Sphere('100 kpc')] = 5
 
     X[pynbody.filt.FamilyFilter(pynbody.family.gas)] = 10
     assert X.get(pynbody.filt.Sphere('100 kpc'), None) == 5
```

### Comparing `pynbody-2.0.0b7/tests/gadget_test.py` & `pynbody-2.0.0b8/tests/gadget_test.py`

 * *Files 2% similar despite different names*

```diff
@@ -208,10 +208,10 @@
     assert f_no_unit_override.filename == "testdata/gadget2/test_g2_snap.1"
     assert f_no_unit_override['pos'].units == "Mpc a h^-1"  # from default_config.ini
 
 
 def test_ignore_cosmology():
     f = pynbody.load("testdata/gadget2/test_g2_snap.1")
     f.physical_units()
-    np.testing.assert_allclose(f.properties['time'].in_units('Gyr'), 2.5769525238964737)
+    np.testing.assert_allclose(f.properties['time'].in_units('Gyr'), 2.57689526)
     f_no_cosmo = pynbody.load("testdata/gadget2/test_g2_snap.1", ignore_cosmo=True)
-    np.testing.assert_allclose(f_no_cosmo.properties['time'].in_units('Gyr'), 271.6149884391969)
+    np.testing.assert_allclose(f_no_cosmo.properties['time'].in_units('Gyr'), 271.608952)
```

### Comparing `pynbody-2.0.0b7/tests/gadgethdf_test.py` & `pynbody-2.0.0b8/tests/gadgethdf_test.py`

 * *Files 2% similar despite different names*

```diff
@@ -102,20 +102,20 @@
     assert snap._family_slice[pynbody.family.star] == slice(4174059, 4194304, None)
 
 
 def test_mass_in_header():
     f = pynbody.load("testdata/snap_028_z000p000.0.hdf5")
     f.physical_units()
     f['mass'] # load all masses
-    assert np.allclose(f.dm['mass'][0], 3981879.2046075417)
+    assert np.allclose(f.dm['mass'][0], 3982880.471745421)
 
     f = pynbody.load("testdata/snap_028_z000p000.0.hdf5")
     f.physical_units()
     # don't load all masses, allow it to be loaded for DM only
-    assert np.allclose(f.dm['mass'][0], 3981879.2046075417)
+    assert np.allclose(f.dm['mass'][0], 3982880.471745421)
 
 def test_gadgethdf_style_units():
     f = pynbody.load("testdata/gadget3/data/snapshot_103/snap_103.hdf5")
     npt.assert_allclose(f.st['InitialMass'].units.in_units("1.989e43 g h^-1"), 1.0,
                         rtol=1e-3)
 
 def test_arepo_style_units():
```

### Comparing `pynbody-2.0.0b7/tests/grafic_test.py` & `pynbody-2.0.0b8/tests/grafic_test.py`

 * *Files 1% similar despite different names*

```diff
@@ -28,15 +28,15 @@
           [ 8.94585317, 62.49853492, 62.46953045]])
 
 
 def test_iord():
     assert (f['iord'][::10]==[ 0, 40,  5, 45, 10, 35, 15]).all()
 
 def test_mass():
-    npt.assert_allclose(f['mass'], 2.15729774e+14)
+    npt.assert_allclose(f['mass'], 2.157418e+14)
 
 def test_deltab():
     npt.assert_allclose(f['deltab'][::10], [0.0058372 , -0.00301547, -0.00595138, -0.00416407, -0.01490865,
           -0.01760859, -0.00807793], atol=1e-8)
 
 def test_partial_loading():
     np.random.seed(1)  # so that results are reproducible
```

### Comparing `pynbody-2.0.0b7/tests/gravity_test.py` & `pynbody-2.0.0b8/tests/gravity_test.py`

 * *Files 12% similar despite different names*

```diff
@@ -7,31 +7,31 @@
 def test_gravity():
     f = pynbody.load("testdata/gasoline_ahf/g15784.lr.01024")
     h = f.halos()
     pynbody.analysis.angmom.faceon(h[0])
     pro = pynbody.analysis.profile.Profile(
         h[0], type='equaln', nbins=50, rmin='100 pc', rmax='50 kpc')
 
-    v_circ_correct = np.array([  57.19634349,  103.04331454,  132.12411594,  155.65275799,
-        175.52850379,  193.26102536,  209.52418648,  224.3799979 ,
-        237.98666437,  250.73544548,  262.7691209 ,  273.84754088,
-        283.90399116,  293.11826051,  301.35145207,  308.54834075,
-        314.80692238,  320.03311211,  324.21239628,  327.41041566,
-        329.65615964,  330.93911797,  331.26282888,  330.58067058,
-        328.98176969,  326.54392634,  323.59673278,  321.05292019,
-        318.70939336,  316.17958584,  312.99775752,  308.6537309 ,
-        303.85807775,  299.75311891,  296.75429822,  290.89777773,
-        283.85313613,  277.87270183,  271.31168303,  267.90725824,
-        263.91617477,  259.83215657,  256.09476119,  251.42881956,
-        247.00831007,  244.89573797,  240.35616032,  238.19548506,
-        233.91552211,  229.68799203])
+    v_circ_correct = np.array([ 57.19445406, 103.07628964, 132.11223368, 155.58932808,
+          175.48202525, 193.19929044, 209.50654738, 224.36527055,
+          237.93659247, 250.68636441, 262.72949256, 273.84865161,
+          283.90032809, 293.10420183, 301.32998659, 308.540641  ,
+          314.80948167, 320.0281338 , 324.2028914 , 327.40124838,
+          329.64625769, 330.92733193, 331.25336332, 330.57151552,
+          328.97485235, 326.54886075, 323.60357994, 321.03602331,
+          318.69193219, 316.16834582, 312.98912943, 308.66044926,
+          303.84896218, 299.75583821, 296.77125812, 290.91251525,
+          283.84275867, 277.87033036, 271.31481248, 267.90817792,
+          263.89271744, 259.83899922, 256.07340296, 251.42403094,
+          247.00347206, 244.89404984, 240.3383157 , 238.17681295,
+          233.90977942, 229.66882597])
 
     v_circ = pro['v_circ'].in_units('km s^-1')
 
-    npt.assert_allclose(v_circ, v_circ_correct,atol=1e-5)
+    npt.assert_allclose(v_circ, v_circ_correct, rtol=1e-2, atol=0)
 
 def test_gravity_float():
     f = pynbody.new(100)
     np.random.seed(0)
     coords = np.random.normal(size=(100,3))
     del f['pos']
     del f['mass']
```

### Comparing `pynbody-2.0.0b7/tests/halos_test.py` & `pynbody-2.0.0b8/tests/halos_test.py`

 * *Files 6% similar despite different names*

```diff
@@ -220,14 +220,19 @@
     assert h[2].properties['testproperty'] == 3.0
 
 def test_property_from_dummy():
     f = pynbody.new(dm=100)
     h = SimpleHaloCatalogue(f)
     assert h.get_dummy_halo(1).properties['testproperty'] == 1.5
 
+def test_halocat_keys():
+    f = pynbody.new(dm=100)
+    h = SimpleHaloCatalogue(f)
+    assert (h.keys() == np.arange(1,10)).all()
+
 def test_property_units():
     f = pynbody.new(dm=100)
     h = SimpleHaloCatalogue(f)
     assert "kpc" not in str(h[1].properties['testproperty_with_units'])
 
     h = SimpleHaloCatalogue(f)
     f.physical_units()
@@ -376,7 +381,24 @@
     # check we can pass a class instead of its name
     halos = f.halos(priority=[AdaptaHOPCatalogue])
     assert isinstance(halos, AdaptaHOPCatalogue)
 
     # check that classes not in the priority order are still scanned
     halos = f.halos(priority=["AHFCatalogue"])
     assert isinstance(halos, HOPCatalogue) or isinstance(halos, AdaptaHOPCatalogue)
+
+def test_load_halo_priority_americanised():
+    from pynbody.halo.adaptahop import AdaptaHOPCatalogue
+    from pynbody.halo.hop import HOPCatalogue
+    f = pynbody.load("testdata/output_00080")
+
+    # check that the priority ordering is respected
+    halos = f.halos(priority=['HOPCatalog'])
+    assert isinstance(halos, HOPCatalogue)
+
+    halos = f.halos(priority=["AdaptaHOPCatalog"])
+    assert isinstance(halos, AdaptaHOPCatalogue)
+
+def test_repr():
+    f = pynbody.load("testdata/output_00080")
+    halos = f.halos()
+    assert repr(halos) == "<AdaptaHOPCatalogue, length 170>"
```

### Comparing `pynbody-2.0.0b7/tests/halotools_test.py` & `pynbody-2.0.0b8/tests/halotools_test.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import glob
 import os
 import time
 
 import numpy as np
+import numpy.testing as npt
 import pytest
 
 import pynbody
 
 
 def setup_module():
     global f, h
@@ -19,25 +20,49 @@
     del f, h
 
 
 def test_center():
     global f, h
     with pynbody.analysis.halo.center(h[0]):
         np.testing.assert_allclose(
-            f['pos'][0], [-0.0137471,  -0.00208458, -0.04392379], atol=1e-4)
+            f['pos'][0], [-0.0137471,  -0.00208458, -0.04392379], rtol=1e-4)
+
+def test_center_wrapped_halo():
+    npart = 10000
+    f = pynbody.new(dm=npart)
+    np.random.seed(1337)
+    f['pos'] = np.random.normal(scale=0.1, size=f['pos'].shape)
+    f['vel'] = np.random.normal(scale=0.1, size=f['vel'].shape)
+    f['pos'][0] = [0.0, 0.0, 0.0] # this is the known centre!
+    f['vel'][0] = [0.0, 0.0, 0.0] # again, a known centre
+    f['vel'] += 5.0
+
+    f['mass'] = np.ones(npart)
+    f['x']+=0.95
+    f['y']+=0.5
+    f['z']-=0.94
+    f.properties['boxsize'] = 2.0
+    f.wrap()
+
+    with pynbody.analysis.halo.center(f) as t:
+        npt.assert_almost_equal(f['pos'][0], [0.0, 0.0, 0.0], decimal=1)
+        npt.assert_almost_equal(f['vel'][0], [0.0, 0.0, 0.0], decimal=1)
+
 
 
 def test_align():
     global f, h
-    with pynbody.analysis.angmom.faceon(h[0]):
-        np.testing.assert_allclose(f['pos'][:2], [[-0.010718, -0.001504, -0.044783],
-                                                  [-0.010026,  0.002441, -0.04465 ]], atol=1e-5)
+    with pynbody.analysis.angmom.faceon(h[0]) as t:
+        print(repr(t))
+        np.testing.assert_allclose(f['pos'][:2], [[-0.010711, -0.001491, -0.044785],
+                                                          [-0.010019,  0.002454, -0.04465 ]],
+                                   atol=1e-5)
 
-        np.testing.assert_allclose(f['vel'][:2], [[ 0.017203,  0.01848 , -0.019859],
-                                                  [ 0.051333,  0.027357, -0.010303]], atol=1e-5)
+        np.testing.assert_allclose(f['vel'][:2], [[ 0.019214,  0.024604, -0.020356],
+                                                          [ 0.053343,  0.033478, -0.010793]], atol=1e-5)
 
 
 def test_virialradius():
     global f, h
     with pynbody.analysis.halo.center(h[0]):
         start = time.time()
         vrad = pynbody.analysis.halo.virial_radius(f)
```

### Comparing `pynbody-2.0.0b7/tests/hbtplus_test.py` & `pynbody-2.0.0b8/tests/hbtplus_test.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import pathlib
 import warnings
 
 import numpy as np
 import numpy.testing as npt
 import pytest
 
 import pynbody
@@ -143,14 +144,25 @@
     }[snap_type]
     assert ( halos[100]['iord'] == h100_iords ).all()
 
 def test_load(snap):
     h = snap.halos(priority=["HBTPlusCatalogue", "Gadget4SubfindHDFCatalogue"])
     assert isinstance(h, pynbody.halo.hbtplus.HBTPlusCatalogue)
 
+def test_load_from_filename(snap):
+    filename: pathlib.Path = snap.filename
+    snap._filename = "" # clear filename so we can test loading from catalogue filename
+
+    for name in ['SubSnap_034', 'SubSnap_034.0']:
+        # work out the HBT+ catalogue filename
+        hbt_filename = filename.parent / "034" / name
+
+        h = snap.halos(filename=hbt_filename)
+        assert isinstance(h, pynbody.halo.hbtplus.HBTPlusCatalogue)
+
 @pytest.fixture
 def expected_properties(snap_type):
     return {
         'single-file': {0: {'Nbound': 41, 'TrackId': 0, 'Mbound': 0.0052275728,},
                         79: {'TrackId': 92, 'Mbound': 0.004462562},
                         5: {'ComovingAveragePosition': [24.523391, 28.355526, 25.766893]}},
         'multifile': {0: {'Nbound': 29,  'TrackId': 333},
```

### Comparing `pynbody-2.0.0b7/tests/hop_test.py` & `pynbody-2.0.0b8/tests/hop_test.py`

 * *Files 21% similar despite different names*

```diff
@@ -17,7 +17,18 @@
 def test_get_halo(halos):
     assert len(halos[0]) == 37927
     assert len(halos[1]) == 20870
     assert (halos[1].dm['iord'][::1000] == [950469, 178234, 570544, 602770, 983503, 185854, 189546, 183353,
                                            971918, 189890, 981389, 978381, 184919, 201405, 227622, 180288,
                                            194977, 195167, 187596, 192792, 590108]).all()
     assert len(halos) == 369
+
+def test_autoload_halos(f):
+    halos = f.halos(priority=["HOPCatalogue"])
+    assert isinstance(halos, HOPCatalogue)
+    assert len(halos[0]) == 37927
+
+def test_autoload_halos_by_filename(f):
+    halos = f.halos(filename="testdata/output_00080/grp00080.tag")
+
+    assert isinstance(halos, HOPCatalogue)
+    assert len(halos[0]) == 37927
```

### Comparing `pynbody-2.0.0b7/tests/kdtree_test.py` & `pynbody-2.0.0b8/tests/kdtree_test.py`

 * *Files identical despite different names*

### Comparing `pynbody-2.0.0b7/tests/nchilada_test.py` & `pynbody-2.0.0b8/tests/nchilada_test.py`

 * *Files identical despite different names*

### Comparing `pynbody-2.0.0b7/tests/partial_tipsy_test.py` & `pynbody-2.0.0b8/tests/partial_tipsy_test.py`

 * *Files identical despite different names*

### Comparing `pynbody-2.0.0b7/tests/performance_kdtree.py` & `pynbody-2.0.0b8/tests/performance_kdtree.py`

 * *Files identical despite different names*

### Comparing `pynbody-2.0.0b7/tests/ramses_new_ptcl_format_test.py` & `pynbody-2.0.0b8/tests/ramses_new_ptcl_format_test.py`

 * *Files identical despite different names*

### Comparing `pynbody-2.0.0b7/tests/ramses_test.py` & `pynbody-2.0.0b8/tests/ramses_test.py`

 * *Files 1% similar despite different names*

```diff
@@ -312,38 +312,37 @@
         tform = fcosmo.st["tform"]
         tform_raw = fcosmo.st["tform_raw"]
 
     np.testing.assert_allclose(tform, np.full(31990, -1))
     _test_tform_checker(tform_raw)
 
 def test_proper_time_loading():
-    expected_times = np.array([
-        2.50421602, 2.54981476, 2.64293759, 2.97459085, 2.47246567,
-        3.60575216, 2.19990045, 2.51812602, 2.28107602, 3.43433139,
-        2.46447623, 3.40593189, 2.37042486, 2.72302068, 3.05392067,
-        2.66978924, 2.94991936, 3.05711287, 2.46661848, 3.78098984,
-        3.9314067 , 2.22836996, 3.99929978, 3.63914358, 2.61559192,
-        2.67241162, 2.57897509, 4.02035096, 2.75958541, 2.69266309,
-        2.35971505, 4.34920931, 2.66643275, 3.354545  , 3.25341288,
-        3.01484682, 2.41245746, 2.63102207, 2.88776033, 2.54323499
-    ])
+    expected_times = np.array([2.50416037, 2.5497581 , 2.64287886, 2.97452475, 2.47241073,
+          3.60567204, 2.19985156, 2.51807006, 2.28102533, 3.43425507,
+          2.46442147, 3.4058562 , 2.37037218, 2.72296016, 3.05385281,
+          2.66972991, 2.9498538 , 3.05704494, 2.46656367, 3.78090582,
+          3.93131933, 2.22832044, 3.9992109 , 3.63906271, 2.61553379,
+          2.67235223, 2.57891777, 4.02026162, 2.75952408, 2.69260326,
+          2.35966261, 4.34911266, 2.66637349, 3.35447046, 3.25334058,
+          3.01477982, 2.41240385, 2.6309636 , 2.88769616, 2.54317847])
     for (load_opts, force) in (
         ({"times_are_proper": True}, False),
         ({}, True),
     ):
         f_pt = pynbody.load(
             "testdata/prop_time_output_00030",
             cpus=range(10, 20),
             **load_opts,
         )
         if force:
             f_pt.times_are_proper = True
 
         f_pt._load_particle_block('tform')
         f_pt._convert_tform()
+
         np.testing.assert_allclose(
             f_pt.s["tform"].in_units("Gyr"),
             expected_times,
             rtol=1e-5
         )
 
 
@@ -366,17 +365,18 @@
     ramses_file.g['mu']
     ramses_file.g['temp']
 
     assert(ramses_file.g['mu'].min() != ramses_file.g['mu'].max())   # Check that ionized and neutral mu are now generated
     np.testing.assert_allclose(ramses_file.g['mu'][:10], 0.590406 * np.ones(10), rtol=1e-5)
     np.testing.assert_allclose(ramses_file.g['mu'].max(), 1.225115, rtol=1e-5)
 
-    np.testing.assert_allclose(ramses_file.g['temp'][:10], [26006.212237, 28014.491234, 28014.45815 , 30537.462281,
-                                                          26950.323296, 29093.741241, 29197.270737, 31939.873103,
-                                                          26950.318628, 29197.316078])
+    np.testing.assert_allclose(ramses_file.g['temp'][:10], [26006.242067, 28014.523369, 28014.490285,
+                                                                   30537.49731 , 26950.35421 , 29093.774613,
+                                                                   29197.304228, 31939.90974 , 26950.349542,
+                                                                   29197.349569])
 
 
 def test_family_array(ramses_file):
     ramses_file.dm['mass']
     assert "mass" in ramses_file.family_keys()
     assert ramses_file.dm['mass'].sim == ramses_file.dm
 
@@ -403,15 +403,15 @@
     with pytest.raises(KeyError, match="No array.*"):
         f_dmo.st['metals'] # noqa
 
     # Now define a custom-derived metals array, which should enable us to access the array at all time
     # Previously to #689, this would still break the loading with the same ValueError
     # Now it loads the derived field without issues
     from pynbody.snapshot.ramses import RamsesSnap
-    @RamsesSnap.derived_quantity
+    @RamsesSnap.derived_array
     def metals(snap):
         return np.zeros(len(snap))
 
     f_dmo.st['metals'] # noqa
 
 
 def array_by_array_test_tipsy_converter(ramses_snap, tipsy_snap):
```

### Comparing `pynbody-2.0.0b7/tests/rockstar_test.py` & `pynbody-2.0.0b8/tests/rockstar_test.py`

 * *Files 5% similar despite different names*

```diff
@@ -42,16 +42,17 @@
     assert np.allclose(props['vel'], np.array([  77.035904, -119.406364,  -27.567175]))
 
 def test_load_rockstar(dummy_file):
     h = pynbody.halo.rockstar.RockstarCatalogue(dummy_file)
     assert len(h)==5851
     assert isinstance(h, pynbody.halo.rockstar.RockstarCatalogue)
 
-def test_autodetect_rockstar(dummy_file):
-    h = dummy_file.halos()
+def test_autodetect_rockstar_from_filename(dummy_file):
+    dummy_file._filename = ""
+    h = dummy_file.halos(filename="testdata/rockstar/halos_15.0.bin")
     assert isinstance(h, pynbody.halo.rockstar.RockstarCatalogue)
 
 def test_rockstar_properties(rockstar_halos):
     h_properties = rockstar_halos[4977].properties
     assert h_properties['num_p']==40
     npt.assert_allclose(h_properties['pos'], [43.892704, 0.197397, 40.751919], rtol=1e-6)
```

### Comparing `pynbody-2.0.0b7/tests/snapshot_test.py` & `pynbody-2.0.0b8/tests/snapshot_test.py`

 * *Files 15% similar despite different names*

```diff
@@ -172,15 +172,15 @@
     f['pos'].units = 'kpc'
     f2 = copy.deepcopy(f[[1, 2, 3, 4]])
     assert f2['pos'].units == 'kpc'
     # this tests for a bug where units were not correctly
     # copied in from IndexedSimArrays
 
 
-def test_mean_by_mass():
+def test_mean_by_mass_units():
     f['pos'].units = 'kpc'
     f['mass'].units = 'Msol'
 
     assert str(f.mean_by_mass('pos').units) == 'kpc'
 
 
 def test_name_awareness():
@@ -252,7 +252,19 @@
     # rho doesn't exist in f.loadable_keys(), only f.gas.loadable_keys():
     assert not f._array_name_implies_ND_slice('rho_x')
 
 def test_index_list():
     f = pynbody.load("testdata/gasoline_ahf/g15784.lr.01024")
     h = f.halos()
     index_list = h[1].get_index_list(f)
+
+def test_mean_by_mass_value():
+    f = pynbody.new(dm=2000)
+    f['mass'] = np.ones(2000)
+    f['mass'][:500] = 2
+
+    f['test_array'] = np.arange(2000)
+
+    f = f[np.arange(1000)] # test on a subsnap for generality
+
+    np.testing.assert_allclose(f.mean_by_mass('test_array'),
+                               (f['test_array'][:500]*2./3 + f['test_array'][500:1000]*1./3).mean())
```

### Comparing `pynbody-2.0.0b7/tests/sph_image_test.py` & `pynbody-2.0.0b8/tests/sph_image_test.py`

 * *Files 5% similar despite different names*

```diff
@@ -51,18 +51,18 @@
     yield np.load(test_folder / "test_stars_2d.npy")
 
 def test_images(compare2d, compare3d, compare_grid, compare2d_wendlandC2, compare3d_wendlandC2):
 
     global f
 
     im3d = pynbody.plot.sph.image(
-        f.gas, width=20.0, units="m_p cm^-3", noplot=True, approximate_fast=False)
+        f.gas, width=20.0, units="m_p cm^-3", noplot=True, approximate_fast=False, resolution=500)
 
     im2d = pynbody.plot.sph.image(
-        f.gas, width=20.0, units="m_p cm^-2", noplot=True, approximate_fast=False)
+        f.gas, width=20.0, units="m_p cm^-2", noplot=True, approximate_fast=False, resolution=500)
 
     im_grid = pynbody.sph.to_3d_grid(f.gas,nx=200,x2=20.0)[::50]
 
 
     np.save("result_im_2d.npy",im2d)
     np.save("result_im_3d.npy",im3d)
     np.save("result_im_grid.npy",im_grid)
@@ -70,17 +70,19 @@
 
     npt.assert_allclose(im2d,compare2d,rtol=1e-4)
     npt.assert_allclose(im3d,compare3d,rtol=1e-4)
     npt.assert_allclose(im_grid,compare_grid,rtol=1e-4)
 
     # Make images with a different kernel (Wendland C2)
     im3d_wendlandC2 = pynbody.plot.sph.image(
-        f.gas, width=20.0, units="m_p cm^-3", noplot=True, approximate_fast=False, kernel_type='wendlandC2')
+        f.gas, width=20.0, units="m_p cm^-3", noplot=True, approximate_fast=False, kernel_type='wendlandC2',
+        resolution=500)
     im2d_wendlandC2 = pynbody.plot.sph.image(
-        f.gas, width=20.0, units="m_p cm^-2", noplot=True, approximate_fast=False, kernel_type='wendlandC2')
+        f.gas, width=20.0, units="m_p cm^-2", noplot=True, approximate_fast=False, kernel_type='wendlandC2',
+        resolution=500)
 
 
     np.save("result_im_2d_wendlandC2.npy",im2d_wendlandC2)
     np.save("result_im_3d_wendlandC2.npy",im3d_wendlandC2)
 
     # Check that using a different kernel produces a different image
     npt.assert_raises(AssertionError,npt.assert_array_equal,im3d_wendlandC2,im3d)
@@ -95,17 +97,17 @@
                                         approximate_fast=False).in_units("m_p cm^-3")
     compare_rect = compare3d[125:-125]
     npt.assert_allclose(im_rect,compare_rect,rtol=1e-4)
 
 def test_approximate_images(compare2d, compare3d):
     global f
     im3d = pynbody.plot.sph.image(
-        f.gas, width=20.0, units="m_p cm^-3", noplot=True, approximate_fast=True)
+        f.gas, width=20.0, units="m_p cm^-3", noplot=True, approximate_fast=True, resolution=500)
     im2d = pynbody.plot.sph.image(
-        f.gas, width=20.0, units="m_p cm^-2", noplot=True, approximate_fast=True )
+        f.gas, width=20.0, units="m_p cm^-2", noplot=True, approximate_fast=True, resolution=500)
 
     np.save("result_approx_im_2d.npy", im2d)
     np.save("result_approx_im_3d.npy", im3d)
 
     # approximate interpolated images are only close in a mean sense
     assert abs(np.log10(im2d/compare2d)).mean()<0.03
     assert abs(np.log10(im3d/compare3d)).mean()<0.03
@@ -120,15 +122,15 @@
         # this should not:
         pynbody.plot.sph.image(f.gas, width=20.0, units="m_p cm^-2", noplot=True, approximate_fast=True, denoise=True)
 
 
 def test_render_stars(stars_2d):
     global f
     with pytest.warns(UserWarning, match=r"No log file found; reverting to guess-and-check"):
-        im = pynbody.plot.stars.render(f, width=10.0, resolution=100, ret_im=True, plot=False)
+        im = pynbody.plot.stars.render(f, width=10.0, resolution=100, return_image=True, noplot=True)
 
     np.save("result_stars_2d.npy", im[40:60])
 
     npt.assert_allclose(stars_2d,im[40:60],atol=0.01)
 
 
 @pynbody.derived_array
```

### Comparing `pynbody-2.0.0b7/tests/subarray_test.py` & `pynbody-2.0.0b8/tests/subarray_test.py`

 * *Files identical despite different names*

### Comparing `pynbody-2.0.0b7/tests/subfind_test.py` & `pynbody-2.0.0b8/tests/subfind_test.py`

 * *Files 13% similar despite different names*

```diff
@@ -10,28 +10,38 @@
     f = pynbody.load("testdata/subfind/snapshot_019")
     if request.param:
         f['iord'] = np.random.permutation(f['iord'])
     return f
 
 @pytest.fixture
 def halos(snap):
-    return pynbody.halo.subfind.SubfindCatalogue(snap, subs=True)
+    return pynbody.halo.subfind.SubfindCatalogue(snap, subhalos=True)
 
 @pytest.fixture
 def groups(snap):
-    return pynbody.halo.subfind.SubfindCatalogue(snap, subs=False)
+    return pynbody.halo.subfind.SubfindCatalogue(snap, subhalos=False)
 
 
 def test_lengths(halos, groups):
     assert len(groups)==2853
     assert len(halos)==3290
 
+def test_deprecated_subs_keyword(snap, halos):
+    with pytest.warns(DeprecationWarning):
+        new_halos = snap.halos(subs=True)
+        assert isinstance(new_halos, pynbody.halo.subfind.SubfindCatalogue)
+        assert len(new_halos) == len(halos)
+
 def test_autodetect_subfind(snap):
     assert isinstance(snap.halos(), pynbody.halo.subfind.SubfindCatalogue)
 
+def test_autodetect_subfind_from_filename(snap):
+    snap._filename = ""
+    assert isinstance(snap.halos(filename="testdata/subfind/groups_019"), pynbody.halo.subfind.SubfindCatalogue)
+
 def test_group_properties(groups):
     assert_allclose(float(groups[3].properties['mmean_200']), 1.22e14, rtol=1.e-2)
     assert_allclose(float(groups[3].properties['rtop_200']), 1.02, rtol=1.e-2)
 
 @pytest.mark.parametrize('with_units', [True, False])
 def test_all_group_properties(groups, with_units):
     properties = groups.get_properties_all_halos(with_units=with_units)
@@ -47,15 +57,15 @@
 
 def test_group_children(groups):
     assert np.all(groups[0].properties['children'] == np.arange(0, 39))
     assert np.all(groups[3].properties['children'] == np.arange(89,109))
     halo_nums_in_subs = [sh.properties['halo_number'] for sh in groups[3].subhalos]
     assert (halo_nums_in_subs == np.arange(89,109)).all()
 
-    halos = groups.base.halos(subs=True)
+    halos = groups.base.halos(subhalos=True)
     for sh_from_group, sh in zip(groups[3].subhalos, halos[89:109]):
         assert sh.properties['halo_number'] == sh_from_group.properties['halo_number']
         assert np.all(sh['iord'] == sh_from_group['iord'])
 
     # subs of subs also tested below in test_halo_children
     assert groups[1].subhalos[0].subhalos[0].properties['halo_number'] == 39
```

### Comparing `pynbody-2.0.0b7/tests/subfindhdf_gadget4_test.py` & `pynbody-2.0.0b8/tests/subfindhdf_gadget4_test.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,59 +1,75 @@
 import numpy as np
 import pytest
 
 import pynbody
 from pynbody.test_utils.gadget4_subfind_reader import Halos
 
+# tell pytest not to raise warnings across this module
+pytestmark = pytest.mark.filterwarnings("ignore:Masses are either stored")
+
 
 def setup_module():
     global snap, halos, subhalos, htest, snap_arepo, halos_arepo, subhalos_arepo, htest_arepo
     with pytest.warns(UserWarning, match="Masses are either stored in the header or have another dataset .*"):
         snap = pynbody.load('testdata/gadget4_subfind/snapshot_000.hdf5')
         snap_arepo = pynbody.load('testdata/arepo/cosmobox_015.hdf5')
 
     halos = pynbody.halo.subfindhdf.Gadget4SubfindHDFCatalogue(snap)
-    subhalos = pynbody.halo.subfindhdf.Gadget4SubfindHDFCatalogue(snap, subs=True)
+    subhalos = pynbody.halo.subfindhdf.Gadget4SubfindHDFCatalogue(snap, subhalos=True)
     htest = Halos('testdata/gadget4_subfind/', 0)
 
     halos_arepo = pynbody.halo.subfindhdf.ArepoSubfindHDFCatalogue(snap_arepo)
-    subhalos_arepo = pynbody.halo.subfindhdf.ArepoSubfindHDFCatalogue(snap_arepo, subs=True)
+    subhalos_arepo = pynbody.halo.subfindhdf.ArepoSubfindHDFCatalogue(snap_arepo, subhalos=True)
     htest_arepo = Halos('testdata/arepo/', 15)
 
 
 def teardown_module():
     global snap, halos, subhalos, htest, snap_arepo, halos_arepo, subhalos_arepo, htest_arepo
     del snap, halos, subhalos, htest, snap_arepo, halos_arepo, subhalos_arepo, htest_arepo
 
 
 def test_catalogue():
     _h_nogrp = snap.halos()
-    _subh_nogrp = snap.halos(subs=True)
+    _subh_nogrp = snap.halos(subhalos=True)
     _harepo_nogrp = snap_arepo.halos()
-    _subharepo_nogrp = snap_arepo.halos(subs=True)
+    _subharepo_nogrp = snap_arepo.halos(subhalos=True)
     for h in [halos, subhalos, _h_nogrp, _subh_nogrp, halos_arepo, subhalos_arepo, _harepo_nogrp, _subharepo_nogrp]:
         assert(isinstance(h, pynbody.halo.subfindhdf.Gadget4SubfindHDFCatalogue)), \
             "Should be a Gadget4SubfindHDFCatalogue catalogue but instead it is a " + str(type(h))
 
 def test_lengths():
     assert len(halos)==299
     assert len(subhalos)==343
     assert len(halos_arepo)==447
     assert len(subhalos_arepo)==475
 
+def test_catalogue_from_filename_gadget4():
+    snap = pynbody.load('testdata/gadget4_subfind/snapshot_000.hdf5')
+    snap._filename = ""
+
+    halos = snap.halos(filename='testdata/gadget4_subfind/fof_subhalo_tab_000.hdf5')
+    assert isinstance(halos, pynbody.halo.subfindhdf.Gadget4SubfindHDFCatalogue)
+
+def test_catalogue_from_filename_arepo():
+    snap = pynbody.load('testdata/arepo/cosmobox_015.hdf5')
+    snap._filename = ""
+
+    halos = snap.halos(filename='testdata/arepo/fof_subhalo_tab_015.hdf5')
+    assert isinstance(halos, pynbody.halo.subfindhdf.ArepoSubfindHDFCatalogue)
 
 @pytest.mark.parametrize('mode', ('gadget4', 'arepo'))
 @pytest.mark.parametrize('subhalos', (True, False))
 def test_halo_or_subhalo_properties(mode, subhalos):
 
     halos_str = 'subhalos' if subhalos else 'halos'
     if mode == 'gadget4':
-        comparison_catalogue, pynbody_catalogue = htest.load()[halos_str], snap.halos(subs=subhalos)
+        comparison_catalogue, pynbody_catalogue = htest.load()[halos_str], snap.halos(subhalos=subhalos)
     elif mode=='arepo':
-        comparison_catalogue, pynbody_catalogue = htest_arepo.load()[halos_str], snap_arepo.halos(subs=subhalos)
+        comparison_catalogue, pynbody_catalogue = htest_arepo.load()[halos_str], snap_arepo.halos(subhalos=subhalos)
     else:
         raise ValueError("Invalid mode")
 
     np.random.seed(1)
     hids = np.random.choice(range(len(pynbody_catalogue)), 20)
 
     for hid in hids:
```

### Comparing `pynbody-2.0.0b7/tests/subfindhdf_test.py` & `pynbody-2.0.0b8/tests/subfindhdf_test.py`

 * *Files 3% similar despite different names*

```diff
@@ -63,29 +63,36 @@
             for fam in [halo.g, halo.d, halo.s]:
                 assert (len(fam['iord']) ==
                         snap._hdf_files[0][snap._family_to_group_map[fam.families()[0]][0]]['Length'][i])
 
 def test_subhalos(snap):
     """Test that subhalos can be accessed from each parent FOF group, as well as directly through a subs object"""
     h = pynbody.halo.subfindhdf.SubFindHDFHaloCatalogue(snap)
-    subs = pynbody.halo.subfindhdf.SubFindHDFHaloCatalogue(snap, subs=True)
+    subs = pynbody.halo.subfindhdf.SubFindHDFHaloCatalogue(snap, subhalos=True)
     h.load_all()
 
     assert (h[0].subhalos[0]['iord'] == subs[0]['iord']).all()
     assert (h[1].subhalos[1]['iord'] == subs[7]['iord']).all()
 
     with pytest.warns(DeprecationWarning):
         assert (h[1].sub[1]['iord'] == subs[7]['iord']).all()
 
+def test_deprecated_subs_keyword(snap):
+    with pytest.warns(DeprecationWarning):
+        new_halos = snap.halos(subs=True)
+        assert isinstance(new_halos, pynbody.halo.subfindhdf.SubFindHDFHaloCatalogue)
+        assert len(new_halos) == 3294
+
 def test_finds_correct_halo(snap):
     h = snap.halos()
     assert isinstance(h, pynbody.halo.subfindhdf.SubFindHDFHaloCatalogue)
-    h = snap.halos(subs=True)
+    h = snap.halos(subhalos=True)
     assert isinstance(h, pynbody.halo.subfindhdf.SubFindHDFHaloCatalogue)
 
+
 def test_grp_array(snap):
     h = snap.halos()
     grp = h.get_group_array()
     for i in range(0,100,10):
         assert len(snap['iord'][grp==i]) == len(h[i])
         assert (h[i]['iord'] == snap['iord'][grp==i]).all()
 
@@ -100,15 +107,15 @@
                         8.880245794949587)
     npt.assert_allclose(h.get_dummy_halo(1).properties['Halo_M_Crit200'].in_units(file_mass_unit),
                         8.116568749712314)
 
 @pytest.mark.parametrize('subhalos', (True, False))
 @pytest.mark.parametrize('with_units', (True, False))
 def test_properties_all_halos(snap, subhalos, with_units):
-    h = snap.halos(subs=subhalos)
+    h = snap.halos(subhalos=subhalos)
     properties = h.get_properties_all_halos(with_units=with_units)
 
     filesub = 'testdata/gadget3/data/subhalos_103/subhalo_103'
     dir = 'subfind' if subhalos else 'fof'
     FoF_Mass = pyread_gadget_hdf5(filesub + '.0.hdf5', 10, 'Mass', sub_dir=dir, nopanda=True, silent=True)
     FoF_CoM = pyread_gadget_hdf5(filesub+'.0.hdf5', 10, 'CenterOfMass', sub_dir=dir, nopanda=True, silent=True)
 
@@ -188,8 +195,8 @@
 
 @pytest.mark.parametrize('load_all', (True, False))
 def test_halo_properties_physical_units(snap, load_all):
     h = snap.halos()
     if load_all:
         h.load_all()
     h.physical_units()
-    npt.assert_allclose(h[0].properties['CenterOfMass'], [1242.67381894, 1571.45917479, 2232.62036159])
+    npt.assert_allclose(h[0].properties['CenterOfMass'], [1242.674894, 1571.460534, 2232.622292])
```

### Comparing `pynbody-2.0.0b7/tests/swift_test.py` & `pynbody-2.0.0b8/tests/swift_test.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import numpy as np
+import numpy.testing as npt
 import pytest
 from pytest import raises
 
 import pynbody
 import pynbody.halo.velociraptor
 import pynbody.snapshot.swift
 
@@ -25,15 +26,15 @@
 def test_swift_arrays():
     f = pynbody.load("testdata/SWIFT/snap_0150.hdf5")
     assert np.allclose(f.dm['pos'].units.ratio("Mpc a", **f.conversion_context()), 1.0)
     assert np.allclose(f.dm['vel'].units.ratio("km s^-1", **f.conversion_context()), 1.0)
     # the reason the following isn't exactly 1.0 is because our solar mass is slightly different to swift's
     # (the pynbody value is outdated but it will need some work to think about how to fix this without
     # breaking backwards compatibility)
-    assert np.allclose(f.dm['mass'].units.ratio("1e10 Msol", **f.conversion_context()), 0.9997436)
+    assert np.allclose(f.dm['mass'].units.ratio("1e10 Msol", **f.conversion_context()), 1.0)
     assert np.allclose(f.dm['vel'][::50000], np.array([[-249.5395 ,   122.65865 , -144.79892 ],
                                              [  75.57313 ,  -51.598354 , 250.10258 ],
                                              [-139.62218 , -132.5298   , 479.02545 ],
                                              [ 147.22443 , -168.17662  ,-249.17387 ],
                                              [  27.643984,  161.06497  ,  21.430338],
                                              [  79.65777 ,   25.674492 , -45.813534]]))
     assert np.allclose(f.gas['pos'][::50000], np.array([[  2.54333146,   0.56501471,   3.08184457],
@@ -154,7 +155,17 @@
                      take_region = test_region)
 
     f_full = pynbody.load("testdata/SWIFT/snap_0150.hdf5")
 
     assert len(f) < len(f_full)
 
     assert np.all(f[test_region]['iord'] == f_full[test_region]['iord'])
+
+def test_swift_scalefactor_in_units():
+    f = pynbody.load("testdata/SWIFT/snap_0150.hdf5")
+
+    # naively, one would assume cm^2 s^-2, but actual units header says 1e10 a^2 cm^2 s^-2
+    # So this tests pynbody respects that. Note that we don't give the scalefactor context,
+    # so if scalefactor exponents are wrong, this will raise an exception
+    npt.assert_allclose((f.gas['u'].units).in_units("km^2 s^-2 a^-2"), 1.0)
+
+    npt.assert_allclose(f.gas['pos'].units.in_units("Mpc a"), 1.0)
```

### Comparing `pynbody-2.0.0b7/tests/test_profile.py` & `pynbody-2.0.0b8/tests/test_profile.py`

 * *Files identical despite different names*

### Comparing `pynbody-2.0.0b7/tests/theoretical_profile.py` & `pynbody-2.0.0b8/tests/theoretical_profile.py`

 * *Files identical despite different names*

### Comparing `pynbody-2.0.0b7/tests/tipsy_test.py` & `pynbody-2.0.0b8/tests/tipsy_test.py`

 * *Files 20% similar despite different names*

```diff
@@ -354,34 +354,34 @@
     f1['pos']
     assert f1['pos'].units != 'kpc'
 
 
 @pytest.mark.filterwarnings("ignore:No log file found; reverting to guess-and-check:UserWarning")
 def test_3d_interpolation(snap):
     # this is the result using scipy.interpolate.interp
-    ref3d = np.array([0.07527991,  0.06456315,  0.08380653,  0.15143689,  0.15568259,
-                      0.09593283,  0.15549068,  0.13407668,  0.15177078,  0.14166734,
-                      0.06554151,  0.13197516,  0.08851156,  0.06210035,  0.09224193,
-                      0.162001,  0.16017458,  0.06572785,  0.16384523,  0.1621215,
-                      0.15005151,  0.15224003,  0.1580059,  0.1606176,  0.16919882,
-                      0.15257504,  0.15542396,  0.15950106,  0.15208175,  0.06277352,
-                      0.16297019,  0.16536367,  0.15913841,  0.16852261,  0.16592073,
-                      0.16994837,  0.13997742,  0.16381589,  0.16592951,  0.16631843,
-                      0.12965855,  0.16823705,  0.16560094,  0.16819444,  0.15564206,
-                      0.15821792,  0.1596779,  0.15242394,  0.16538892,  0.16265422,
-                      0.1698232,  0.16823449,  0.16036913,  0.13258314,  0.16295899,
-                      0.16926536,  0.16349818,  0.07734309,  0.16657909,  0.16847497,
-                      0.16370438,  0.17016328,  0.16424645,  0.14292659,  0.17001509,
-                      0.16708861,  0.17015931,  0.06657929,  0.16794139,  0.16821759,
-                      0.16128866,  0.14454934,  0.16137588,  0.16934885,  0.17008926,
-                      0.16986069,  0.16963654,  0.14639736,  0.16590415,  0.16879675,
-                      0.16349512,  0.16999227,  0.17003994,  0.15351041,  0.16446416,
-                      0.14130995,  0.1636267,  0.17015097,  0.16989277,  0.16982946,
-                      0.17006758,  0.16906539,  0.16315827,  0.17021533,  0.16991691,
-                      0.17006688,  0.17006756,  0.16753875,  0.15553802,  0.15892623])
+    ref3d = np.array([0.07527991, 0.06456315, 0.08380653, 0.15143689, 0.15568259,
+       0.09593283, 0.15549068, 0.13407668, 0.15177078, 0.14166734,
+       0.06554151, 0.13197516, 0.08851156, 0.06210035, 0.09224193,
+       0.162001  , 0.16017458, 0.06572785, 0.16384523, 0.1621215 ,
+       0.15005151, 0.15224003, 0.1580059 , 0.1606176 , 0.16919882,
+       0.15257504, 0.15542396, 0.15950106, 0.15208175, 0.06277352,
+       0.16297019, 0.16536367, 0.15913841, 0.16852261, 0.16592073,
+       0.16994837, 0.13997742, 0.16381589, 0.16592951, 0.16631843,
+       0.12965855, 0.16823705, 0.16560094, 0.16819444, 0.15564206,
+       0.15821792, 0.1596779 , 0.15242394, 0.16538892, 0.16265422,
+       0.1698232 , 0.16823449, 0.16036913, 0.13258314, 0.16295899,
+       0.16926536, 0.16349818, 0.07734905, 0.16657909, 0.16847497,
+       0.16370438, 0.17016328, 0.16424645, 0.14292659, 0.17001509,
+       0.16708861, 0.17015931, 0.06657929, 0.16794139, 0.16821759,
+       0.16128866, 0.14454934, 0.16137588, 0.16934885, 0.17008926,
+       0.16986069, 0.16963654, 0.14639736, 0.16590415, 0.16879675,
+       0.16349512, 0.16999227, 0.17003994, 0.15351041, 0.16446416,
+       0.14130995, 0.1636267 , 0.17015097, 0.16989277, 0.16982946,
+       0.17006758, 0.16906539, 0.16315827, 0.17021533, 0.16991691,
+       0.17006688, 0.17006756, 0.16753875, 0.15553802, 0.15892623])
 
     arr = pynbody.analysis.ionfrac.calculate(snap, 'ovi')
     assert(np.allclose(arr[0:100], ref3d))
 
     ref2d = np.array([-8.43178697, -8.43437937, -8.43515772, -8.43554701, -8.43801415,
                       -8.44009401, -8.44048422, -
                       8.4410046, -8.44178542, -8.44204576,
```

### Comparing `pynbody-2.0.0b7/tests/utils_test.py` & `pynbody-2.0.0b8/tests/utils_test.py`

 * *Files identical despite different names*

### Comparing `pynbody-2.0.0b7/tests/velociraptor_test.py` & `pynbody-2.0.0b8/tests/velociraptor_test.py`

 * *Files 4% similar despite different names*

```diff
@@ -93,7 +93,14 @@
     assert np.allclose(all_properties['Lx'][0], -90787.3983020414)
     assert np.allclose(all_properties['Lx'][9], -73881.83861892551)
 
     if with_units:
         assert all_properties['Lx'].units == '1e13 kpc Msol km s**-1'
     else:
         assert not hasattr(all_properties['Lx'], 'units')
+
+def test_swift_velociraptor_select_catalogue_with_filename():
+    f = pynbody.load("testdata/SWIFT/snap_0150.hdf5")
+    h = f.halos(filename="testdata/SWIFT/catalogue_0150/output")
+    assert isinstance(h, pynbody.halo.velociraptor.VelociraptorCatalogue)
+    h.load_all()
+    assert len(h) == 209
```

