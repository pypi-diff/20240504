# Comparing `tmp/mobspy-2.3.4.tar.gz` & `tmp/mobspy-2.3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mobspy-2.3.4.tar", last modified: Thu Apr  4 13:21:16 2024, max compression
+gzip compressed data, was "mobspy-2.3.5.tar", last modified: Thu Apr 11 13:12:08 2024, max compression
```

## Comparing `mobspy-2.3.4.tar` & `mobspy-2.3.5.tar`

### file list

```diff
@@ -1,459 +1,422 @@
-drwxr-xr-x   0 fabriciocravo   (501) staff       (20)        0 2024-04-04 13:21:16.769390 mobspy-2.3.4/
-drwxr-xr-x   0 fabriciocravo   (501) staff       (20)        0 2024-04-04 13:21:15.790243 mobspy-2.3.4/.github/
-drwxr-xr-x   0 fabriciocravo   (501) staff       (20)        0 2024-04-04 13:21:15.845417 mobspy-2.3.4/.github/workflows/
--rw-r--r--   0 fabriciocravo   (501) staff       (20)     1201 2023-06-15 12:59:57.000000 mobspy-2.3.4/.github/workflows/python-app.yml
--rw-r--r--   0 fabriciocravo   (501) staff       (20)      395 2024-03-29 08:28:41.000000 mobspy-2.3.4/.gitignore
--rw-r--r--   0 fabriciocravo   (501) staff       (20)     1034 2024-02-26 16:22:21.000000 mobspy-2.3.4/.readthedocs.yaml
--rw-r--r--   0 fabriciocravo   (501) staff       (20)     1068 2023-06-15 12:59:57.000000 mobspy-2.3.4/LICENSE
--rw-r--r--   0 fabriciocravo   (501) staff       (20)     7577 2024-04-04 13:21:16.768786 mobspy-2.3.4/PKG-INFO
--rw-r--r--   0 fabriciocravo   (501) staff       (20)     6331 2024-03-08 01:34:03.000000 mobspy-2.3.4/README.md
-drwxr-xr-x   0 fabriciocravo   (501) staff       (20)        0 2024-04-04 13:21:15.872189 mobspy-2.3.4/docs/
--rw-r--r--   0 fabriciocravo   (501) staff       (20)      634 2024-01-28 20:38:15.000000 mobspy-2.3.4/docs/Makefile
-drwxr-xr-x   0 fabriciocravo   (501) staff       (20)        0 2024-04-04 13:21:15.906259 mobspy-2.3.4/docs/Notebooks/
--rw-r--r--   0 fabriciocravo   (501) staff       (20)   127718 2024-01-28 20:38:15.000000 mobspy-2.3.4/docs/Notebooks/01_Basic_Intro.ipynb
--rw-r--r--   0 fabriciocravo   (501) staff       (20)     6534 2024-01-28 20:38:15.000000 mobspy-2.3.4/docs/Notebooks/02_Reaction_Inheritance.ipynb
--rw-r--r--   0 fabriciocravo   (501) staff       (20)     8067 2024-01-28 20:38:15.000000 mobspy-2.3.4/docs/Notebooks/03_Characteristics.ipynb
--rw-r--r--   0 fabriciocravo   (501) staff       (20)     2210 2024-01-28 20:38:15.000000 mobspy-2.3.4/docs/Notebooks/04_Characteristic_restriction.ipynb
--rw-r--r--   0 fabriciocravo   (501) staff       (20)     5563 2024-01-28 20:38:15.000000 mobspy-2.3.4/docs/Notebooks/05_For_Loops.ipynb
--rw-r--r--   0 fabriciocravo   (501) staff       (20)     6167 2024-01-28 20:38:15.000000 mobspy-2.3.4/docs/Notebooks/06_Order_Matters.ipynb
--rw-r--r--   0 fabriciocravo   (501) staff       (20)    12448 2024-01-28 20:38:15.000000 mobspy-2.3.4/docs/Notebooks/07_Initial_Condition.ipynb
--rw-r--r--   0 fabriciocravo   (501) staff       (20)     5154 2024-01-28 20:38:15.000000 mobspy-2.3.4/docs/Notebooks/08_Units.ipynb
--rw-r--r--   0 fabriciocravo   (501) staff       (20)   106408 2024-01-28 20:38:15.000000 mobspy-2.3.4/docs/Notebooks/09_Result_Data.ipynb
--rw-r--r--   0 fabriciocravo   (501) staff       (20)    25996 2024-01-28 20:38:15.000000 mobspy-2.3.4/docs/Notebooks/10_Reaction_Rates.ipynb
--rw-r--r--   0 fabriciocravo   (501) staff       (20)     3942 2024-01-28 20:38:15.000000 mobspy-2.3.4/docs/Notebooks/11_Looping_Through_Species.ipynb
--rw-r--r--   0 fabriciocravo   (501) staff       (20)     4426 2024-01-28 20:38:15.000000 mobspy-2.3.4/docs/Notebooks/12_Born_Species.ipynb
--rw-r--r--   0 fabriciocravo   (501) staff       (20)    80668 2024-01-28 20:38:15.000000 mobspy-2.3.4/docs/Notebooks/13_Events.ipynb
--rw-r--r--   0 fabriciocravo   (501) staff       (20)    48456 2024-01-28 20:38:15.000000 mobspy-2.3.4/docs/Notebooks/14_Concatenating_Simulations.ipynb
-drwxr-xr-x   0 fabriciocravo   (501) staff       (20)        0 2024-04-04 13:21:15.908132 mobspy-2.3.4/docs/_autosummary/
--rw-r--r--   0 fabriciocravo   (501) staff       (20)       67 2024-01-28 20:38:15.000000 mobspy-2.3.4/docs/_autosummary/mobspy.rst
-drwxr-xr-x   0 fabriciocravo   (501) staff       (20)        0 2024-04-04 13:21:15.792731 mobspy-2.3.4/docs/_build/
-drwxr-xr-x   0 fabriciocravo   (501) staff       (20)        0 2024-04-04 13:21:15.946236 mobspy-2.3.4/docs/_build/doctrees/
-drwxr-xr-x   0 fabriciocravo   (501) staff       (20)        0 2024-04-04 13:21:15.972801 mobspy-2.3.4/docs/_build/doctrees/Notebooks/
--rw-r--r--   0 fabriciocravo   (501) staff       (20)    95114 2024-01-28 20:38:15.000000 mobspy-2.3.4/docs/_build/doctrees/Notebooks/01_Basic_Intro.doctree
--rw-r--r--   0 fabriciocravo   (501) staff       (20)    23601 2024-01-28 20:38:15.000000 mobspy-2.3.4/docs/_build/doctrees/Notebooks/02_Reaction_Inheritance.doctree
--rw-r--r--   0 fabriciocravo   (501) staff       (20)    30820 2024-01-28 20:38:15.000000 mobspy-2.3.4/docs/_build/doctrees/Notebooks/03_Characteristics.doctree
--rw-r--r--   0 fabriciocravo   (501) staff       (20)     7466 2024-01-28 20:38:15.000000 mobspy-2.3.4/docs/_build/doctrees/Notebooks/04_Characteristic_restriction.doctree
--rw-r--r--   0 fabriciocravo   (501) staff       (20)    24161 2024-01-28 20:38:15.000000 mobspy-2.3.4/docs/_build/doctrees/Notebooks/05_For_Loops.doctree
--rw-r--r--   0 fabriciocravo   (501) staff       (20)    21599 2024-01-28 20:38:15.000000 mobspy-2.3.4/docs/_build/doctrees/Notebooks/06_Order_Matters.doctree
--rw-r--r--   0 fabriciocravo   (501) staff       (20)    50076 2024-01-28 20:38:15.000000 mobspy-2.3.4/docs/_build/doctrees/Notebooks/07_Initial_Condition.doctree
--rw-r--r--   0 fabriciocravo   (501) staff       (20)    18699 2024-01-28 20:38:15.000000 mobspy-2.3.4/docs/_build/doctrees/Notebooks/08_Units.doctree
--rw-r--r--   0 fabriciocravo   (501) staff       (20)    41471 2024-01-28 20:38:15.000000 mobspy-2.3.4/docs/_build/doctrees/Notebooks/09_Result_Data.doctree
--rw-r--r--   0 fabriciocravo   (501) staff       (20)    28500 2024-01-28 20:38:15.000000 mobspy-2.3.4/docs/_build/doctrees/Notebooks/10_Reaction_Rates.doctree
--rw-r--r--   0 fabriciocravo   (501) staff       (20)    15272 2024-01-28 20:38:15.000000 mobspy-2.3.4/docs/_build/doctrees/Notebooks/11_Looping_Through_Species.doctree
--rw-r--r--   0 fabriciocravo   (501) staff       (20)    17080 2024-01-28 20:38:15.000000 mobspy-2.3.4/docs/_build/doctrees/Notebooks/12_Born_Species.doctree
--rw-r--r--   0 fabriciocravo   (501) staff       (20)    39545 2024-01-28 20:38:15.000000 mobspy-2.3.4/docs/_build/doctrees/Notebooks/13_Events.doctree
--rw-r--r--   0 fabriciocravo   (501) staff       (20)    15325 2024-01-28 20:38:15.000000 mobspy-2.3.4/docs/_build/doctrees/Notebooks/14_Concatenating_Simulations.doctree
-drwxr-xr-x   0 fabriciocravo   (501) staff       (20)        0 2024-04-04 13:21:15.974013 mobspy-2.3.4/docs/_build/doctrees/_autosummary/
--rw-r--r--   0 fabriciocravo   (501) staff       (20)     2971 2024-01-28 20:38:15.000000 mobspy-2.3.4/docs/_build/doctrees/_autosummary/mobspy.doctree
--rw-r--r--   0 fabriciocravo   (501) staff       (20)     4285 2024-01-28 20:38:15.000000 mobspy-2.3.4/docs/_build/doctrees/api.doctree
--rw-r--r--   0 fabriciocravo   (501) staff       (20)  1736636 2024-01-28 20:38:15.000000 mobspy-2.3.4/docs/_build/doctrees/environment.pickle
--rw-r--r--   0 fabriciocravo   (501) staff       (20)     2754 2024-01-28 20:38:15.000000 mobspy-2.3.4/docs/_build/doctrees/for_local_use.doctree
--rw-r--r--   0 fabriciocravo   (501) staff       (20)     4048 2024-01-28 20:38:15.000000 mobspy-2.3.4/docs/_build/doctrees/index.doctree
--rw-r--r--   0 fabriciocravo   (501) staff       (20)    26568 2024-01-28 20:38:15.000000 mobspy-2.3.4/docs/_build/doctrees/mobspy.data_handler.doctree
--rw-r--r--   0 fabriciocravo   (501) staff       (20)    67412 2024-01-28 20:38:15.000000 mobspy-2.3.4/docs/_build/doctrees/mobspy.doctree
--rw-r--r--   0 fabriciocravo   (501) staff       (20)   490595 2024-01-28 20:38:15.000000 mobspy-2.3.4/docs/_build/doctrees/mobspy.modules.doctree
--rw-r--r--   0 fabriciocravo   (501) staff       (20)    16088 2024-01-28 20:38:15.000000 mobspy-2.3.4/docs/_build/doctrees/mobspy.parameter_scripts.doctree
--rw-r--r--   0 fabriciocravo   (501) staff       (20)     8486 2024-01-28 20:38:15.000000 mobspy-2.3.4/docs/_build/doctrees/mobspy.parameters.doctree
--rw-r--r--   0 fabriciocravo   (501) staff       (20)     8077 2024-01-28 20:38:15.000000 mobspy-2.3.4/docs/_build/doctrees/mobspy.plot_params.doctree
--rw-r--r--   0 fabriciocravo   (501) staff       (20)    86993 2024-01-28 20:38:15.000000 mobspy-2.3.4/docs/_build/doctrees/mobspy.plot_scripts.doctree
--rw-r--r--   0 fabriciocravo   (501) staff       (20)    33712 2024-01-28 20:38:15.000000 mobspy-2.3.4/docs/_build/doctrees/mobspy.sbml_simulator.doctree
--rw-r--r--   0 fabriciocravo   (501) staff       (20)     9059 2024-01-28 20:38:15.000000 mobspy-2.3.4/docs/_build/doctrees/mobspy.simulation_logging.doctree
--rw-r--r--   0 fabriciocravo   (501) staff       (20)     2767 2024-01-28 20:38:15.000000 mobspy-2.3.4/docs/_build/doctrees/modules.doctree
-drwxr-xr-x   0 fabriciocravo   (501) staff       (20)        0 2024-04-04 13:21:16.000626 mobspy-2.3.4/docs/_build/doctrees/nbsphinx/
-drwxr-xr-x   0 fabriciocravo   (501) staff       (20)        0 2024-04-04 13:21:16.030773 mobspy-2.3.4/docs/_build/doctrees/nbsphinx/Notebooks/
--rw-r--r--   0 fabriciocravo   (501) staff       (20)   127718 2024-01-28 20:38:15.000000 mobspy-2.3.4/docs/_build/doctrees/nbsphinx/Notebooks/01_Basic_Intro.ipynb
--rw-r--r--   0 fabriciocravo   (501) staff       (20)     6534 2024-01-28 20:38:15.000000 mobspy-2.3.4/docs/_build/doctrees/nbsphinx/Notebooks/02_Reaction_Inheritance.ipynb
--rw-r--r--   0 fabriciocravo   (501) staff       (20)     8067 2024-01-28 20:38:15.000000 mobspy-2.3.4/docs/_build/doctrees/nbsphinx/Notebooks/03_Characteristics.ipynb
--rw-r--r--   0 fabriciocravo   (501) staff       (20)     2210 2024-01-28 20:38:15.000000 mobspy-2.3.4/docs/_build/doctrees/nbsphinx/Notebooks/04_Characteristic_restriction.ipynb
--rw-r--r--   0 fabriciocravo   (501) staff       (20)     5563 2024-01-28 20:38:15.000000 mobspy-2.3.4/docs/_build/doctrees/nbsphinx/Notebooks/05_For_Loops.ipynb
--rw-r--r--   0 fabriciocravo   (501) staff       (20)     6167 2024-01-28 20:38:15.000000 mobspy-2.3.4/docs/_build/doctrees/nbsphinx/Notebooks/06_Order_Matters.ipynb
--rw-r--r--   0 fabriciocravo   (501) staff       (20)    12448 2024-01-28 20:38:15.000000 mobspy-2.3.4/docs/_build/doctrees/nbsphinx/Notebooks/07_Initial_Condition.ipynb
--rw-r--r--   0 fabriciocravo   (501) staff       (20)     5154 2024-01-28 20:38:15.000000 mobspy-2.3.4/docs/_build/doctrees/nbsphinx/Notebooks/08_Units.ipynb
--rw-r--r--   0 fabriciocravo   (501) staff       (20)   106408 2024-01-28 20:38:15.000000 mobspy-2.3.4/docs/_build/doctrees/nbsphinx/Notebooks/09_Result_Data.ipynb
--rw-r--r--   0 fabriciocravo   (501) staff       (20)    25996 2024-01-28 20:38:15.000000 mobspy-2.3.4/docs/_build/doctrees/nbsphinx/Notebooks/10_Reaction_Rates.ipynb
--rw-r--r--   0 fabriciocravo   (501) staff       (20)     3942 2024-01-28 20:38:15.000000 mobspy-2.3.4/docs/_build/doctrees/nbsphinx/Notebooks/11_Looping_Through_Species.ipynb
--rw-r--r--   0 fabriciocravo   (501) staff       (20)     4426 2024-01-28 20:38:15.000000 mobspy-2.3.4/docs/_build/doctrees/nbsphinx/Notebooks/12_Born_Species.ipynb
--rw-r--r--   0 fabriciocravo   (501) staff       (20)    80668 2024-01-28 20:38:15.000000 mobspy-2.3.4/docs/_build/doctrees/nbsphinx/Notebooks/13_Events.ipynb
--rw-r--r--   0 fabriciocravo   (501) staff       (20)    48456 2024-01-28 20:38:15.000000 mobspy-2.3.4/docs/_build/doctrees/nbsphinx/Notebooks/14_Concatenating_Simulations.ipynb
--rw-r--r--   0 fabriciocravo   (501) staff       (20)    25979 2024-01-28 20:38:15.000000 mobspy-2.3.4/docs/_build/doctrees/nbsphinx/Notebooks_01_Basic_Intro_13_1.png
--rw-r--r--   0 fabriciocravo   (501) staff       (20)    10466 2024-01-28 20:38:15.000000 mobspy-2.3.4/docs/_build/doctrees/nbsphinx/Notebooks_01_Basic_Intro_18_0.png
--rw-r--r--   0 fabriciocravo   (501) staff       (20)    21874 2024-01-28 20:38:15.000000 mobspy-2.3.4/docs/_build/doctrees/nbsphinx/Notebooks_01_Basic_Intro_21_1.png
--rw-r--r--   0 fabriciocravo   (501) staff       (20)    17557 2024-01-28 20:38:15.000000 mobspy-2.3.4/docs/_build/doctrees/nbsphinx/Notebooks_01_Basic_Intro_3_1.png
--rw-r--r--   0 fabriciocravo   (501) staff       (20)     8683 2024-01-28 20:38:15.000000 mobspy-2.3.4/docs/_build/doctrees/nbsphinx/Notebooks_09_Result_Data_1_1.png
--rw-r--r--   0 fabriciocravo   (501) staff       (20)    30221 2024-01-28 20:38:15.000000 mobspy-2.3.4/docs/_build/doctrees/nbsphinx/Notebooks_09_Result_Data_3_0.png
--rw-r--r--   0 fabriciocravo   (501) staff       (20)    23598 2024-01-28 20:38:15.000000 mobspy-2.3.4/docs/_build/doctrees/nbsphinx/Notebooks_09_Result_Data_5_0.png
--rw-r--r--   0 fabriciocravo   (501) staff       (20)     9452 2024-01-28 20:38:15.000000 mobspy-2.3.4/docs/_build/doctrees/nbsphinx/Notebooks_09_Result_Data_9_1.png
--rw-r--r--   0 fabriciocravo   (501) staff       (20)    12468 2024-01-28 20:38:15.000000 mobspy-2.3.4/docs/_build/doctrees/nbsphinx/Notebooks_10_Reaction_Rates_11_1.png
--rw-r--r--   0 fabriciocravo   (501) staff       (20)    14066 2024-01-28 20:38:15.000000 mobspy-2.3.4/docs/_build/doctrees/nbsphinx/Notebooks_13_Events_11_2.png
--rw-r--r--   0 fabriciocravo   (501) staff       (20)    13308 2024-01-28 20:38:15.000000 mobspy-2.3.4/docs/_build/doctrees/nbsphinx/Notebooks_13_Events_1_2.png
--rw-r--r--   0 fabriciocravo   (501) staff       (20)    15379 2024-01-28 20:38:15.000000 mobspy-2.3.4/docs/_build/doctrees/nbsphinx/Notebooks_13_Events_4_3.png
--rw-r--r--   0 fabriciocravo   (501) staff       (20)     9027 2024-01-28 20:38:15.000000 mobspy-2.3.4/docs/_build/doctrees/nbsphinx/Notebooks_13_Events_8_1.png
--rw-r--r--   0 fabriciocravo   (501) staff       (20)    11337 2024-01-28 20:38:15.000000 mobspy-2.3.4/docs/_build/doctrees/nbsphinx/Notebooks_14_Concatenating_Simulations_1_1.png
--rw-r--r--   0 fabriciocravo   (501) staff       (20)    11111 2024-01-28 20:38:15.000000 mobspy-2.3.4/docs/_build/doctrees/nbsphinx/Notebooks_14_Concatenating_Simulations_3_1.png
--rw-r--r--   0 fabriciocravo   (501) staff       (20)    10008 2024-01-28 20:38:15.000000 mobspy-2.3.4/docs/_build/doctrees/nbsphinx/Notebooks_14_Concatenating_Simulations_5_1.png
--rw-r--r--   0 fabriciocravo   (501) staff       (20)     2407 2024-01-28 20:38:15.000000 mobspy-2.3.4/docs/_build/doctrees/setup.doctree
--rw-r--r--   0 fabriciocravo   (501) staff       (20)     2439 2024-01-28 20:38:15.000000 mobspy-2.3.4/docs/_build/doctrees/test_script.doctree
-drwxr-xr-x   0 fabriciocravo   (501) staff       (20)        0 2024-04-04 13:21:16.088392 mobspy-2.3.4/docs/_build/html/
--rw-r--r--   0 fabriciocravo   (501) staff       (20)      230 2024-01-28 20:38:15.000000 mobspy-2.3.4/docs/_build/html/.buildinfo
-drwxr-xr-x   0 fabriciocravo   (501) staff       (20)        0 2024-04-04 13:21:16.184648 mobspy-2.3.4/docs/_build/html/Notebooks/
--rw-r--r--   0 fabriciocravo   (501) staff       (20)    41132 2024-01-28 20:38:15.000000 mobspy-2.3.4/docs/_build/html/Notebooks/01_Basic_Intro.html
--rw-r--r--   0 fabriciocravo   (501) staff       (20)   127718 2024-01-28 20:38:15.000000 mobspy-2.3.4/docs/_build/html/Notebooks/01_Basic_Intro.ipynb
--rw-r--r--   0 fabriciocravo   (501) staff       (20)    16265 2024-01-28 20:38:15.000000 mobspy-2.3.4/docs/_build/html/Notebooks/02_Reaction_Inheritance.html
--rw-r--r--   0 fabriciocravo   (501) staff       (20)     6534 2024-01-28 20:38:15.000000 mobspy-2.3.4/docs/_build/html/Notebooks/02_Reaction_Inheritance.ipynb
--rw-r--r--   0 fabriciocravo   (501) staff       (20)    17425 2024-01-28 20:38:15.000000 mobspy-2.3.4/docs/_build/html/Notebooks/03_Characteristics.html
--rw-r--r--   0 fabriciocravo   (501) staff       (20)     8067 2024-01-28 20:38:15.000000 mobspy-2.3.4/docs/_build/html/Notebooks/03_Characteristics.ipynb
--rw-r--r--   0 fabriciocravo   (501) staff       (20)    10225 2024-01-28 20:38:15.000000 mobspy-2.3.4/docs/_build/html/Notebooks/04_Characteristic_restriction.html
--rw-r--r--   0 fabriciocravo   (501) staff       (20)     2210 2024-01-28 20:38:15.000000 mobspy-2.3.4/docs/_build/html/Notebooks/04_Characteristic_restriction.ipynb
--rw-r--r--   0 fabriciocravo   (501) staff       (20)    15743 2024-01-28 20:38:15.000000 mobspy-2.3.4/docs/_build/html/Notebooks/05_For_Loops.html
--rw-r--r--   0 fabriciocravo   (501) staff       (20)     5563 2024-01-28 20:38:15.000000 mobspy-2.3.4/docs/_build/html/Notebooks/05_For_Loops.ipynb
--rw-r--r--   0 fabriciocravo   (501) staff       (20)    14878 2024-01-28 20:38:15.000000 mobspy-2.3.4/docs/_build/html/Notebooks/06_Order_Matters.html
--rw-r--r--   0 fabriciocravo   (501) staff       (20)     6167 2024-01-28 20:38:15.000000 mobspy-2.3.4/docs/_build/html/Notebooks/06_Order_Matters.ipynb
--rw-r--r--   0 fabriciocravo   (501) staff       (20)    23518 2024-01-28 20:38:15.000000 mobspy-2.3.4/docs/_build/html/Notebooks/07_Initial_Condition.html
--rw-r--r--   0 fabriciocravo   (501) staff       (20)    12448 2024-01-28 20:38:15.000000 mobspy-2.3.4/docs/_build/html/Notebooks/07_Initial_Condition.ipynb
--rw-r--r--   0 fabriciocravo   (501) staff       (20)    15642 2024-01-28 20:38:15.000000 mobspy-2.3.4/docs/_build/html/Notebooks/08_Units.html
--rw-r--r--   0 fabriciocravo   (501) staff       (20)     5154 2024-01-28 20:38:15.000000 mobspy-2.3.4/docs/_build/html/Notebooks/08_Units.ipynb
--rw-r--r--   0 fabriciocravo   (501) staff       (20)    23686 2024-01-28 20:38:15.000000 mobspy-2.3.4/docs/_build/html/Notebooks/09_Result_Data.html
--rw-r--r--   0 fabriciocravo   (501) staff       (20)   106408 2024-01-28 20:38:15.000000 mobspy-2.3.4/docs/_build/html/Notebooks/09_Result_Data.ipynb
--rw-r--r--   0 fabriciocravo   (501) staff       (20)    23178 2024-01-28 20:38:15.000000 mobspy-2.3.4/docs/_build/html/Notebooks/10_Reaction_Rates.html
--rw-r--r--   0 fabriciocravo   (501) staff       (20)    25996 2024-01-28 20:38:15.000000 mobspy-2.3.4/docs/_build/html/Notebooks/10_Reaction_Rates.ipynb
--rw-r--r--   0 fabriciocravo   (501) staff       (20)    14337 2024-01-28 20:38:15.000000 mobspy-2.3.4/docs/_build/html/Notebooks/11_Looping_Through_Species.html
--rw-r--r--   0 fabriciocravo   (501) staff       (20)     3942 2024-01-28 20:38:15.000000 mobspy-2.3.4/docs/_build/html/Notebooks/11_Looping_Through_Species.ipynb
--rw-r--r--   0 fabriciocravo   (501) staff       (20)    14032 2024-01-28 20:38:15.000000 mobspy-2.3.4/docs/_build/html/Notebooks/12_Born_Species.html
--rw-r--r--   0 fabriciocravo   (501) staff       (20)     4426 2024-01-28 20:38:15.000000 mobspy-2.3.4/docs/_build/html/Notebooks/12_Born_Species.ipynb
--rw-r--r--   0 fabriciocravo   (501) staff       (20)    28370 2024-01-28 20:38:15.000000 mobspy-2.3.4/docs/_build/html/Notebooks/13_Events.html
--rw-r--r--   0 fabriciocravo   (501) staff       (20)    80668 2024-01-28 20:38:15.000000 mobspy-2.3.4/docs/_build/html/Notebooks/13_Events.ipynb
--rw-r--r--   0 fabriciocravo   (501) staff       (20)    18015 2024-01-28 20:38:15.000000 mobspy-2.3.4/docs/_build/html/Notebooks/14_Concatenating_Simulations.html
--rw-r--r--   0 fabriciocravo   (501) staff       (20)    48456 2024-01-28 20:38:15.000000 mobspy-2.3.4/docs/_build/html/Notebooks/14_Concatenating_Simulations.ipynb
-drwxr-xr-x   0 fabriciocravo   (501) staff       (20)        0 2024-04-04 13:21:16.188414 mobspy-2.3.4/docs/_build/html/_autosummary/
--rw-r--r--   0 fabriciocravo   (501) staff       (20)     7201 2024-01-28 20:38:15.000000 mobspy-2.3.4/docs/_build/html/_autosummary/mobspy.html
-drwxr-xr-x   0 fabriciocravo   (501) staff       (20)        0 2024-04-04 13:21:16.231515 mobspy-2.3.4/docs/_build/html/_images/
--rw-r--r--   0 fabriciocravo   (501) staff       (20)    25979 2024-01-28 20:38:15.000000 mobspy-2.3.4/docs/_build/html/_images/Notebooks_01_Basic_Intro_13_1.png
--rw-r--r--   0 fabriciocravo   (501) staff       (20)    10466 2024-01-28 20:38:15.000000 mobspy-2.3.4/docs/_build/html/_images/Notebooks_01_Basic_Intro_18_0.png
--rw-r--r--   0 fabriciocravo   (501) staff       (20)    21874 2024-01-28 20:38:15.000000 mobspy-2.3.4/docs/_build/html/_images/Notebooks_01_Basic_Intro_21_1.png
--rw-r--r--   0 fabriciocravo   (501) staff       (20)    17557 2024-01-28 20:38:15.000000 mobspy-2.3.4/docs/_build/html/_images/Notebooks_01_Basic_Intro_3_1.png
--rw-r--r--   0 fabriciocravo   (501) staff       (20)     8683 2024-01-28 20:38:15.000000 mobspy-2.3.4/docs/_build/html/_images/Notebooks_09_Result_Data_1_1.png
--rw-r--r--   0 fabriciocravo   (501) staff       (20)    30221 2024-01-28 20:38:15.000000 mobspy-2.3.4/docs/_build/html/_images/Notebooks_09_Result_Data_3_0.png
--rw-r--r--   0 fabriciocravo   (501) staff       (20)    23598 2024-01-28 20:38:15.000000 mobspy-2.3.4/docs/_build/html/_images/Notebooks_09_Result_Data_5_0.png
--rw-r--r--   0 fabriciocravo   (501) staff       (20)     9452 2024-01-28 20:38:15.000000 mobspy-2.3.4/docs/_build/html/_images/Notebooks_09_Result_Data_9_1.png
--rw-r--r--   0 fabriciocravo   (501) staff       (20)    12468 2024-01-28 20:38:15.000000 mobspy-2.3.4/docs/_build/html/_images/Notebooks_10_Reaction_Rates_11_1.png
--rw-r--r--   0 fabriciocravo   (501) staff       (20)    14066 2024-01-28 20:38:15.000000 mobspy-2.3.4/docs/_build/html/_images/Notebooks_13_Events_11_2.png
--rw-r--r--   0 fabriciocravo   (501) staff       (20)    13308 2024-01-28 20:38:15.000000 mobspy-2.3.4/docs/_build/html/_images/Notebooks_13_Events_1_2.png
--rw-r--r--   0 fabriciocravo   (501) staff       (20)    15379 2024-01-28 20:38:15.000000 mobspy-2.3.4/docs/_build/html/_images/Notebooks_13_Events_4_3.png
--rw-r--r--   0 fabriciocravo   (501) staff       (20)     9027 2024-01-28 20:38:15.000000 mobspy-2.3.4/docs/_build/html/_images/Notebooks_13_Events_8_1.png
--rw-r--r--   0 fabriciocravo   (501) staff       (20)    11337 2024-01-28 20:38:15.000000 mobspy-2.3.4/docs/_build/html/_images/Notebooks_14_Concatenating_Simulations_1_1.png
--rw-r--r--   0 fabriciocravo   (501) staff       (20)    11111 2024-01-28 20:38:15.000000 mobspy-2.3.4/docs/_build/html/_images/Notebooks_14_Concatenating_Simulations_3_1.png
--rw-r--r--   0 fabriciocravo   (501) staff       (20)    10008 2024-01-28 20:38:15.000000 mobspy-2.3.4/docs/_build/html/_images/Notebooks_14_Concatenating_Simulations_5_1.png
-drwxr-xr-x   0 fabriciocravo   (501) staff       (20)        0 2024-04-04 13:21:16.255656 mobspy-2.3.4/docs/_build/html/_sources/
-drwxr-xr-x   0 fabriciocravo   (501) staff       (20)        0 2024-04-04 13:21:16.285221 mobspy-2.3.4/docs/_build/html/_sources/Notebooks/
--rw-r--r--   0 fabriciocravo   (501) staff       (20)   127718 2024-01-28 20:38:15.000000 mobspy-2.3.4/docs/_build/html/_sources/Notebooks/01_Basic_Intro.ipynb.txt
--rw-r--r--   0 fabriciocravo   (501) staff       (20)     6534 2024-01-28 20:38:15.000000 mobspy-2.3.4/docs/_build/html/_sources/Notebooks/02_Reaction_Inheritance.ipynb.txt
--rw-r--r--   0 fabriciocravo   (501) staff       (20)     8067 2024-01-28 20:38:15.000000 mobspy-2.3.4/docs/_build/html/_sources/Notebooks/03_Characteristics.ipynb.txt
--rw-r--r--   0 fabriciocravo   (501) staff       (20)     2210 2024-01-28 20:38:15.000000 mobspy-2.3.4/docs/_build/html/_sources/Notebooks/04_Characteristic_restriction.ipynb.txt
--rw-r--r--   0 fabriciocravo   (501) staff       (20)     5563 2024-01-28 20:38:15.000000 mobspy-2.3.4/docs/_build/html/_sources/Notebooks/05_For_Loops.ipynb.txt
--rw-r--r--   0 fabriciocravo   (501) staff       (20)     6167 2024-01-28 20:38:15.000000 mobspy-2.3.4/docs/_build/html/_sources/Notebooks/06_Order_Matters.ipynb.txt
--rw-r--r--   0 fabriciocravo   (501) staff       (20)    12448 2024-01-28 20:38:15.000000 mobspy-2.3.4/docs/_build/html/_sources/Notebooks/07_Initial_Condition.ipynb.txt
--rw-r--r--   0 fabriciocravo   (501) staff       (20)     5154 2024-01-28 20:38:15.000000 mobspy-2.3.4/docs/_build/html/_sources/Notebooks/08_Units.ipynb.txt
--rw-r--r--   0 fabriciocravo   (501) staff       (20)   106408 2024-01-28 20:38:15.000000 mobspy-2.3.4/docs/_build/html/_sources/Notebooks/09_Result_Data.ipynb.txt
--rw-r--r--   0 fabriciocravo   (501) staff       (20)    25996 2024-01-28 20:38:15.000000 mobspy-2.3.4/docs/_build/html/_sources/Notebooks/10_Reaction_Rates.ipynb.txt
--rw-r--r--   0 fabriciocravo   (501) staff       (20)     3942 2024-01-28 20:38:15.000000 mobspy-2.3.4/docs/_build/html/_sources/Notebooks/11_Looping_Through_Species.ipynb.txt
--rw-r--r--   0 fabriciocravo   (501) staff       (20)     4426 2024-01-28 20:38:15.000000 mobspy-2.3.4/docs/_build/html/_sources/Notebooks/12_Born_Species.ipynb.txt
--rw-r--r--   0 fabriciocravo   (501) staff       (20)    80668 2024-01-28 20:38:15.000000 mobspy-2.3.4/docs/_build/html/_sources/Notebooks/13_Events.ipynb.txt
--rw-r--r--   0 fabriciocravo   (501) staff       (20)    48456 2024-01-28 20:38:15.000000 mobspy-2.3.4/docs/_build/html/_sources/Notebooks/14_Concatenating_Simulations.ipynb.txt
-drwxr-xr-x   0 fabriciocravo   (501) staff       (20)        0 2024-04-04 13:21:16.286832 mobspy-2.3.4/docs/_build/html/_sources/_autosummary/
--rw-r--r--   0 fabriciocravo   (501) staff       (20)       67 2024-01-28 20:38:15.000000 mobspy-2.3.4/docs/_build/html/_sources/_autosummary/mobspy.rst.txt
--rw-r--r--   0 fabriciocravo   (501) staff       (20)      123 2024-01-28 20:38:15.000000 mobspy-2.3.4/docs/_build/html/_sources/api.rst.txt
--rw-r--r--   0 fabriciocravo   (501) staff       (20)      131 2024-01-28 20:38:15.000000 mobspy-2.3.4/docs/_build/html/_sources/for_local_use.rst.txt
--rw-r--r--   0 fabriciocravo   (501) staff       (20)      839 2024-01-28 20:38:15.000000 mobspy-2.3.4/docs/_build/html/_sources/index.rst.txt
--rw-r--r--   0 fabriciocravo   (501) staff       (20)      626 2024-01-28 20:38:15.000000 mobspy-2.3.4/docs/_build/html/_sources/mobspy.data_handler.rst.txt
--rw-r--r--   0 fabriciocravo   (501) staff       (20)     3107 2024-01-28 20:38:15.000000 mobspy-2.3.4/docs/_build/html/_sources/mobspy.modules.rst.txt
--rw-r--r--   0 fabriciocravo   (501) staff       (20)      655 2024-01-28 20:38:15.000000 mobspy-2.3.4/docs/_build/html/_sources/mobspy.parameter_scripts.rst.txt
--rw-r--r--   0 fabriciocravo   (501) staff       (20)      571 2024-01-28 20:38:15.000000 mobspy-2.3.4/docs/_build/html/_sources/mobspy.parameters.rst.txt
--rw-r--r--   0 fabriciocravo   (501) staff       (20)      620 2024-01-28 20:38:15.000000 mobspy-2.3.4/docs/_build/html/_sources/mobspy.plot_params.rst.txt
--rw-r--r--   0 fabriciocravo   (501) staff       (20)     1029 2024-01-28 20:38:15.000000 mobspy-2.3.4/docs/_build/html/_sources/mobspy.plot_scripts.rst.txt
--rw-r--r--   0 fabriciocravo   (501) staff       (20)      549 2024-01-28 20:38:15.000000 mobspy-2.3.4/docs/_build/html/_sources/mobspy.rst.txt
--rw-r--r--   0 fabriciocravo   (501) staff       (20)      742 2024-01-28 20:38:15.000000 mobspy-2.3.4/docs/_build/html/_sources/mobspy.sbml_simulator.rst.txt
--rw-r--r--   0 fabriciocravo   (501) staff       (20)      427 2024-01-28 20:38:15.000000 mobspy-2.3.4/docs/_build/html/_sources/mobspy.simulation_logging.rst.txt
--rw-r--r--   0 fabriciocravo   (501) staff       (20)       96 2024-01-28 20:38:15.000000 mobspy-2.3.4/docs/_build/html/_sources/modules.rst.txt
--rw-r--r--   0 fabriciocravo   (501) staff       (20)      103 2024-01-28 20:38:15.000000 mobspy-2.3.4/docs/_build/html/_sources/setup.rst.txt
--rw-r--r--   0 fabriciocravo   (501) staff       (20)      123 2024-01-28 20:38:15.000000 mobspy-2.3.4/docs/_build/html/_sources/test_script.rst.txt
-drwxr-xr-x   0 fabriciocravo   (501) staff       (20)        0 2024-04-04 13:21:16.321189 mobspy-2.3.4/docs/_build/html/_static/
--rw-r--r--   0 fabriciocravo   (501) staff       (20)     4289 2024-01-28 20:38:15.000000 mobspy-2.3.4/docs/_build/html/_static/_sphinx_javascript_frameworks_compat.js
--rw-r--r--   0 fabriciocravo   (501) staff       (20)    15094 2024-01-28 20:38:15.000000 mobspy-2.3.4/docs/_build/html/_static/basic.css
-drwxr-xr-x   0 fabriciocravo   (501) staff       (20)        0 2024-04-04 13:21:16.324273 mobspy-2.3.4/docs/_build/html/_static/css/
--rw-r--r--   0 fabriciocravo   (501) staff       (20)     3229 2024-01-28 20:38:15.000000 mobspy-2.3.4/docs/_build/html/_static/css/badge_only.css
-drwxr-xr-x   0 fabriciocravo   (501) staff       (20)        0 2024-04-04 13:21:16.404025 mobspy-2.3.4/docs/_build/html/_static/css/fonts/
--rw-r--r--   0 fabriciocravo   (501) staff       (20)    87624 2024-01-28 20:38:15.000000 mobspy-2.3.4/docs/_build/html/_static/css/fonts/Roboto-Slab-Bold.woff
--rw-r--r--   0 fabriciocravo   (501) staff       (20)    67312 2024-01-28 20:38:15.000000 mobspy-2.3.4/docs/_build/html/_static/css/fonts/Roboto-Slab-Bold.woff2
--rw-r--r--   0 fabriciocravo   (501) staff       (20)    86288 2024-01-28 20:38:15.000000 mobspy-2.3.4/docs/_build/html/_static/css/fonts/Roboto-Slab-Regular.woff
--rw-r--r--   0 fabriciocravo   (501) staff       (20)    66444 2024-01-28 20:38:15.000000 mobspy-2.3.4/docs/_build/html/_static/css/fonts/Roboto-Slab-Regular.woff2
--rw-r--r--   0 fabriciocravo   (501) staff       (20)   165742 2024-01-28 20:38:15.000000 mobspy-2.3.4/docs/_build/html/_static/css/fonts/fontawesome-webfont.eot
--rw-r--r--   0 fabriciocravo   (501) staff       (20)   444379 2024-01-28 20:38:15.000000 mobspy-2.3.4/docs/_build/html/_static/css/fonts/fontawesome-webfont.svg
--rw-r--r--   0 fabriciocravo   (501) staff       (20)   165548 2024-01-28 20:38:15.000000 mobspy-2.3.4/docs/_build/html/_static/css/fonts/fontawesome-webfont.ttf
--rw-r--r--   0 fabriciocravo   (501) staff       (20)    98024 2024-01-28 20:38:15.000000 mobspy-2.3.4/docs/_build/html/_static/css/fonts/fontawesome-webfont.woff
--rw-r--r--   0 fabriciocravo   (501) staff       (20)    77160 2024-01-28 20:38:15.000000 mobspy-2.3.4/docs/_build/html/_static/css/fonts/fontawesome-webfont.woff2
--rw-r--r--   0 fabriciocravo   (501) staff       (20)   323344 2024-01-28 20:38:15.000000 mobspy-2.3.4/docs/_build/html/_static/css/fonts/lato-bold-italic.woff
--rw-r--r--   0 fabriciocravo   (501) staff       (20)   193308 2024-01-28 20:38:15.000000 mobspy-2.3.4/docs/_build/html/_static/css/fonts/lato-bold-italic.woff2
--rw-r--r--   0 fabriciocravo   (501) staff       (20)   309728 2024-01-28 20:38:15.000000 mobspy-2.3.4/docs/_build/html/_static/css/fonts/lato-bold.woff
--rw-r--r--   0 fabriciocravo   (501) staff       (20)   184912 2024-01-28 20:38:15.000000 mobspy-2.3.4/docs/_build/html/_static/css/fonts/lato-bold.woff2
--rw-r--r--   0 fabriciocravo   (501) staff       (20)   328412 2024-01-28 20:38:15.000000 mobspy-2.3.4/docs/_build/html/_static/css/fonts/lato-normal-italic.woff
--rw-r--r--   0 fabriciocravo   (501) staff       (20)   195704 2024-01-28 20:38:15.000000 mobspy-2.3.4/docs/_build/html/_static/css/fonts/lato-normal-italic.woff2
--rw-r--r--   0 fabriciocravo   (501) staff       (20)   309192 2024-01-28 20:38:15.000000 mobspy-2.3.4/docs/_build/html/_static/css/fonts/lato-normal.woff
--rw-r--r--   0 fabriciocravo   (501) staff       (20)   182708 2024-01-28 20:38:15.000000 mobspy-2.3.4/docs/_build/html/_static/css/fonts/lato-normal.woff2
--rw-r--r--   0 fabriciocravo   (501) staff       (20)   135314 2024-01-28 20:38:15.000000 mobspy-2.3.4/docs/_build/html/_static/css/theme.css
--rw-r--r--   0 fabriciocravo   (501) staff       (20)     4472 2024-01-28 20:38:15.000000 mobspy-2.3.4/docs/_build/html/_static/doctools.js
--rw-r--r--   0 fabriciocravo   (501) staff       (20)      326 2024-01-28 20:38:15.000000 mobspy-2.3.4/docs/_build/html/_static/documentation_options.js
--rw-r--r--   0 fabriciocravo   (501) staff       (20)      286 2024-01-28 20:38:15.000000 mobspy-2.3.4/docs/_build/html/_static/file.png
--rw-r--r--   0 fabriciocravo   (501) staff       (20)    89501 2024-01-28 20:38:15.000000 mobspy-2.3.4/docs/_build/html/_static/jquery.js
-drwxr-xr-x   0 fabriciocravo   (501) staff       (20)        0 2024-04-04 13:21:16.415338 mobspy-2.3.4/docs/_build/html/_static/js/
--rw-r--r--   0 fabriciocravo   (501) staff       (20)      934 2024-01-28 20:38:15.000000 mobspy-2.3.4/docs/_build/html/_static/js/badge_only.js
--rw-r--r--   0 fabriciocravo   (501) staff       (20)     4370 2024-01-28 20:38:15.000000 mobspy-2.3.4/docs/_build/html/_static/js/html5shiv-printshiv.min.js
--rw-r--r--   0 fabriciocravo   (501) staff       (20)     2734 2024-01-28 20:38:15.000000 mobspy-2.3.4/docs/_build/html/_static/js/html5shiv.min.js
--rw-r--r--   0 fabriciocravo   (501) staff       (20)     5023 2024-01-28 20:38:15.000000 mobspy-2.3.4/docs/_build/html/_static/js/theme.js
--rw-r--r--   0 fabriciocravo   (501) staff       (20)     4758 2024-01-28 20:38:15.000000 mobspy-2.3.4/docs/_build/html/_static/language_data.js
--rw-r--r--   0 fabriciocravo   (501) staff       (20)       90 2024-01-28 20:38:15.000000 mobspy-2.3.4/docs/_build/html/_static/minus.png
--rw-r--r--   0 fabriciocravo   (501) staff       (20)     4467 2024-01-28 20:38:15.000000 mobspy-2.3.4/docs/_build/html/_static/nbsphinx-broken-thumbnail.svg
--rw-r--r--   0 fabriciocravo   (501) staff       (20)     6861 2024-01-28 20:38:15.000000 mobspy-2.3.4/docs/_build/html/_static/nbsphinx-code-cells.css
--rw-r--r--   0 fabriciocravo   (501) staff       (20)      584 2024-01-28 20:38:15.000000 mobspy-2.3.4/docs/_build/html/_static/nbsphinx-gallery.css
--rw-r--r--   0 fabriciocravo   (501) staff       (20)     2871 2024-01-28 20:38:15.000000 mobspy-2.3.4/docs/_build/html/_static/nbsphinx-no-thumbnail.svg
--rw-r--r--   0 fabriciocravo   (501) staff       (20)       90 2024-01-28 20:38:15.000000 mobspy-2.3.4/docs/_build/html/_static/plus.png
--rw-r--r--   0 fabriciocravo   (501) staff       (20)     4902 2024-01-28 20:38:15.000000 mobspy-2.3.4/docs/_build/html/_static/pygments.css
--rw-r--r--   0 fabriciocravo   (501) staff       (20)    18732 2024-01-28 20:38:15.000000 mobspy-2.3.4/docs/_build/html/_static/searchtools.js
--rw-r--r--   0 fabriciocravo   (501) staff       (20)     5123 2024-01-28 20:38:15.000000 mobspy-2.3.4/docs/_build/html/_static/sphinx_highlight.js
--rw-r--r--   0 fabriciocravo   (501) staff       (20)     7627 2024-01-28 20:38:15.000000 mobspy-2.3.4/docs/_build/html/api.html
--rw-r--r--   0 fabriciocravo   (501) staff       (20)     6551 2024-01-28 20:38:15.000000 mobspy-2.3.4/docs/_build/html/for_local_use.html
--rw-r--r--   0 fabriciocravo   (501) staff       (20)    67727 2024-01-28 20:38:15.000000 mobspy-2.3.4/docs/_build/html/genindex.html
--rw-r--r--   0 fabriciocravo   (501) staff       (20)    10018 2024-01-28 20:38:15.000000 mobspy-2.3.4/docs/_build/html/index.html
--rw-r--r--   0 fabriciocravo   (501) staff       (20)    14863 2024-01-28 20:38:15.000000 mobspy-2.3.4/docs/_build/html/mobspy.data_handler.html
--rw-r--r--   0 fabriciocravo   (501) staff       (20)    91437 2024-01-28 20:38:15.000000 mobspy-2.3.4/docs/_build/html/mobspy.html
--rw-r--r--   0 fabriciocravo   (501) staff       (20)   178543 2024-01-28 20:38:15.000000 mobspy-2.3.4/docs/_build/html/mobspy.modules.html
--rw-r--r--   0 fabriciocravo   (501) staff       (20)    11761 2024-01-28 20:38:15.000000 mobspy-2.3.4/docs/_build/html/mobspy.parameter_scripts.html
--rw-r--r--   0 fabriciocravo   (501) staff       (20)     8867 2024-01-28 20:38:15.000000 mobspy-2.3.4/docs/_build/html/mobspy.parameters.html
--rw-r--r--   0 fabriciocravo   (501) staff       (20)     8736 2024-01-28 20:38:15.000000 mobspy-2.3.4/docs/_build/html/mobspy.plot_params.html
--rw-r--r--   0 fabriciocravo   (501) staff       (20)    36208 2024-01-28 20:38:15.000000 mobspy-2.3.4/docs/_build/html/mobspy.plot_scripts.html
--rw-r--r--   0 fabriciocravo   (501) staff       (20)    16526 2024-01-28 20:38:15.000000 mobspy-2.3.4/docs/_build/html/mobspy.sbml_simulator.html
--rw-r--r--   0 fabriciocravo   (501) staff       (20)     9250 2024-01-28 20:38:15.000000 mobspy-2.3.4/docs/_build/html/mobspy.simulation_logging.html
--rw-r--r--   0 fabriciocravo   (501) staff       (20)    23199 2024-01-28 20:38:15.000000 mobspy-2.3.4/docs/_build/html/modules.html
--rw-r--r--   0 fabriciocravo   (501) staff       (20)     8450 2024-01-28 20:38:15.000000 mobspy-2.3.4/docs/_build/html/objects.inv
--rw-r--r--   0 fabriciocravo   (501) staff       (20)    17062 2024-01-28 20:38:15.000000 mobspy-2.3.4/docs/_build/html/py-modindex.html
--rw-r--r--   0 fabriciocravo   (501) staff       (20)     6595 2024-01-28 20:38:15.000000 mobspy-2.3.4/docs/_build/html/search.html
--rw-r--r--   0 fabriciocravo   (501) staff       (20)    96699 2024-01-28 20:38:15.000000 mobspy-2.3.4/docs/_build/html/searchindex.js
--rw-r--r--   0 fabriciocravo   (501) staff       (20)     6464 2024-01-28 20:38:15.000000 mobspy-2.3.4/docs/_build/html/setup.html
--rw-r--r--   0 fabriciocravo   (501) staff       (20)     6500 2024-01-28 20:38:15.000000 mobspy-2.3.4/docs/_build/html/test_script.html
--rw-r--r--   0 fabriciocravo   (501) staff       (20)      123 2024-01-28 20:38:15.000000 mobspy-2.3.4/docs/api.rst
--rw-r--r--   0 fabriciocravo   (501) staff       (20)     1220 2024-01-28 20:38:15.000000 mobspy-2.3.4/docs/conf.py
--rw-r--r--   0 fabriciocravo   (501) staff       (20)      131 2024-01-28 20:38:15.000000 mobspy-2.3.4/docs/for_local_use.rst
--rw-r--r--   0 fabriciocravo   (501) staff       (20)      839 2024-01-28 20:38:15.000000 mobspy-2.3.4/docs/index.rst
--rw-r--r--   0 fabriciocravo   (501) staff       (20)      800 2024-01-28 20:38:15.000000 mobspy-2.3.4/docs/make.bat
--rw-r--r--   0 fabriciocravo   (501) staff       (20)      626 2024-01-28 20:38:15.000000 mobspy-2.3.4/docs/mobspy.data_handler.rst
--rw-r--r--   0 fabriciocravo   (501) staff       (20)     3107 2024-01-28 20:38:15.000000 mobspy-2.3.4/docs/mobspy.modules.rst
--rw-r--r--   0 fabriciocravo   (501) staff       (20)      655 2024-01-28 20:38:15.000000 mobspy-2.3.4/docs/mobspy.parameter_scripts.rst
--rw-r--r--   0 fabriciocravo   (501) staff       (20)      571 2024-01-28 20:38:15.000000 mobspy-2.3.4/docs/mobspy.parameters.rst
--rw-r--r--   0 fabriciocravo   (501) staff       (20)      620 2024-01-28 20:38:15.000000 mobspy-2.3.4/docs/mobspy.plot_params.rst
--rw-r--r--   0 fabriciocravo   (501) staff       (20)     1029 2024-01-28 20:38:15.000000 mobspy-2.3.4/docs/mobspy.plot_scripts.rst
--rw-r--r--   0 fabriciocravo   (501) staff       (20)      549 2024-01-28 20:38:15.000000 mobspy-2.3.4/docs/mobspy.rst
--rw-r--r--   0 fabriciocravo   (501) staff       (20)      742 2024-01-28 20:38:15.000000 mobspy-2.3.4/docs/mobspy.sbml_simulator.rst
--rw-r--r--   0 fabriciocravo   (501) staff       (20)      427 2024-01-28 20:38:15.000000 mobspy-2.3.4/docs/mobspy.simulation_logging.rst
--rw-r--r--   0 fabriciocravo   (501) staff       (20)       96 2024-01-28 20:38:15.000000 mobspy-2.3.4/docs/modules.rst
--rw-r--r--   0 fabriciocravo   (501) staff       (20)      103 2024-01-28 20:38:15.000000 mobspy-2.3.4/docs/setup.rst
--rw-r--r--   0 fabriciocravo   (501) staff       (20)      123 2024-01-28 20:38:15.000000 mobspy-2.3.4/docs/test_script.rst
-drwxr-xr-x   0 fabriciocravo   (501) staff       (20)        0 2024-04-04 13:21:15.796998 mobspy-2.3.4/example_models/
-drwxr-xr-x   0 fabriciocravo   (501) staff       (20)        0 2024-04-04 13:21:16.454845 mobspy-2.3.4/example_models/Tutorial Notebooks/
--rw-r--r--   0 fabriciocravo   (501) staff       (20)   101374 2024-02-28 22:33:14.000000 mobspy-2.3.4/example_models/Tutorial Notebooks/01_Basic_Intro.ipynb
--rw-r--r--   0 fabriciocravo   (501) staff       (20)     6432 2023-11-22 11:36:42.000000 mobspy-2.3.4/example_models/Tutorial Notebooks/02_Reaction_Inheritance.ipynb
--rw-r--r--   0 fabriciocravo   (501) staff       (20)     7971 2023-11-22 11:38:40.000000 mobspy-2.3.4/example_models/Tutorial Notebooks/03_Characteristics.ipynb
--rw-r--r--   0 fabriciocravo   (501) staff       (20)     2210 2023-04-10 17:13:33.000000 mobspy-2.3.4/example_models/Tutorial Notebooks/04_Characteristic_restriction.ipynb
--rw-r--r--   0 fabriciocravo   (501) staff       (20)     5458 2023-11-22 12:06:45.000000 mobspy-2.3.4/example_models/Tutorial Notebooks/05_For_Loops.ipynb
--rw-r--r--   0 fabriciocravo   (501) staff       (20)     6167 2023-04-10 19:38:34.000000 mobspy-2.3.4/example_models/Tutorial Notebooks/06_Order_Matters.ipynb
--rw-r--r--   0 fabriciocravo   (501) staff       (20)     9479 2023-11-22 12:08:40.000000 mobspy-2.3.4/example_models/Tutorial Notebooks/07_Initial_Condition.ipynb
--rw-r--r--   0 fabriciocravo   (501) staff       (20)     5154 2023-04-19 15:35:09.000000 mobspy-2.3.4/example_models/Tutorial Notebooks/08_Units.ipynb
--rw-r--r--   0 fabriciocravo   (501) staff       (20)     7347 2023-11-22 22:08:58.000000 mobspy-2.3.4/example_models/Tutorial Notebooks/09_Result_Data.ipynb
--rw-r--r--   0 fabriciocravo   (501) staff       (20)    26061 2023-11-22 12:57:35.000000 mobspy-2.3.4/example_models/Tutorial Notebooks/10_Reaction_Rates.ipynb
--rw-r--r--   0 fabriciocravo   (501) staff       (20)     4029 2023-11-22 12:58:00.000000 mobspy-2.3.4/example_models/Tutorial Notebooks/11_Looping_Through_Species.ipynb
--rw-r--r--   0 fabriciocravo   (501) staff       (20)     4498 2023-11-22 13:00:12.000000 mobspy-2.3.4/example_models/Tutorial Notebooks/12_Born_Species.ipynb
--rw-r--r--   0 fabriciocravo   (501) staff       (20)    49256 2023-11-22 13:00:32.000000 mobspy-2.3.4/example_models/Tutorial Notebooks/13_Events.ipynb
--rw-r--r--   0 fabriciocravo   (501) staff       (20)    48456 2023-04-21 15:54:19.000000 mobspy-2.3.4/example_models/Tutorial Notebooks/14_Concatenating_Simulations.ipynb
-drwxr-xr-x   0 fabriciocravo   (501) staff       (20)        0 2024-04-04 13:21:16.463551 mobspy-2.3.4/example_models/Tutorial Notebooks/images/
--rw-r--r--   0 fabriciocravo   (501) staff       (20)    12324 2023-04-19 14:32:18.000000 mobspy-2.3.4/example_models/Tutorial Notebooks/images/Matching_Meta.png
--rw-r--r--   0 fabriciocravo   (501) staff       (20)   141303 2023-04-09 17:03:35.000000 mobspy-2.3.4/example_models/Tutorial Notebooks/images/vectorial_space.png
-drwxr-xr-x   0 fabriciocravo   (501) staff       (20)        0 2024-04-04 13:21:16.492289 mobspy-2.3.4/example_models/application_models/
--rw-r--r--   0 fabriciocravo   (501) staff       (20)      572 2024-01-28 20:43:25.000000 mobspy-2.3.4/example_models/application_models/AB_2CD.py
--rw-r--r--   0 fabriciocravo   (501) staff       (20)     1448 2024-01-28 20:44:42.000000 mobspy-2.3.4/example_models/application_models/AND_gate.py
--rw-r--r--   0 fabriciocravo   (501) staff       (20)     2357 2024-01-28 20:43:25.000000 mobspy-2.3.4/example_models/application_models/CRISPR_Oscillator.py
--rw-r--r--   0 fabriciocravo   (501) staff       (20)     1421 2024-01-28 20:47:50.000000 mobspy-2.3.4/example_models/application_models/For_The_Trees.py
--rw-r--r--   0 fabriciocravo   (501) staff       (20)     1291 2024-01-28 20:48:26.000000 mobspy-2.3.4/example_models/application_models/NOR_gate.py
--rw-r--r--   0 fabriciocravo   (501) staff       (20)     1237 2024-01-28 20:47:24.000000 mobspy-2.3.4/example_models/application_models/donor_receptor.py
--rw-r--r--   0 fabriciocravo   (501) staff       (20)     1371 2024-01-28 20:48:41.000000 mobspy-2.3.4/example_models/application_models/oscillator.py
--rw-r--r--   0 fabriciocravo   (501) staff       (20)      994 2023-07-07 11:50:03.000000 mobspy-2.3.4/example_models/application_models/positive_phage_feedback_loop.py
--rw-r--r--   0 fabriciocravo   (501) staff       (20)     2917 2024-01-28 20:49:35.000000 mobspy-2.3.4/example_models/application_models/random_walk.py
--rw-r--r--   0 fabriciocravo   (501) staff       (20)      637 2023-07-05 11:46:34.000000 mobspy-2.3.4/example_models/application_models/simple_infection.py
--rw-r--r--   0 fabriciocravo   (501) staff       (20)      564 2024-01-28 20:50:18.000000 mobspy-2.3.4/example_models/application_models/simple_repressor.py
--rw-r--r--   0 fabriciocravo   (501) staff       (20)      828 2023-07-05 12:49:47.000000 mobspy-2.3.4/example_models/application_models/simple_rule_based_and_gate.py
--rw-r--r--   0 fabriciocravo   (501) staff       (20)      880 2024-03-29 08:24:18.000000 mobspy-2.3.4/for_local_use.py
-drwxr-xr-x   0 fabriciocravo   (501) staff       (20)        0 2024-04-04 13:21:16.494039 mobspy-2.3.4/images/
--rw-r--r--   0 fabriciocravo   (501) staff       (20)    18566 2023-06-15 12:59:57.000000 mobspy-2.3.4/images/img.png
-drwxr-xr-x   0 fabriciocravo   (501) staff       (20)        0 2024-04-04 13:21:16.500558 mobspy-2.3.4/mobspy/
--rw-r--r--   0 fabriciocravo   (501) staff       (20)       95 2023-06-15 12:59:57.000000 mobspy-2.3.4/mobspy/__init__.py
-drwxr-xr-x   0 fabriciocravo   (501) staff       (20)        0 2024-04-04 13:21:16.515558 mobspy-2.3.4/mobspy/__pycache__/
--rw-r--r--   0 fabriciocravo   (501) staff       (20)      236 2024-01-28 20:38:15.000000 mobspy-2.3.4/mobspy/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0 fabriciocravo   (501) staff       (20)      152 2024-01-28 20:38:15.000000 mobspy-2.3.4/mobspy/__pycache__/_version.cpython-310.pyc
--rw-r--r--   0 fabriciocravo   (501) staff       (20)    24852 2024-01-28 20:38:15.000000 mobspy-2.3.4/mobspy/__pycache__/simulation.cpython-310.pyc
--rw-r--r--   0 fabriciocravo   (501) staff       (20)       22 2024-04-04 13:18:53.000000 mobspy-2.3.4/mobspy/_version.py
-drwxr-xr-x   0 fabriciocravo   (501) staff       (20)        0 2024-04-04 13:21:16.520320 mobspy-2.3.4/mobspy/data_handler/
--rw-r--r--   0 fabriciocravo   (501) staff       (20)        0 2023-06-15 12:59:57.000000 mobspy-2.3.4/mobspy/data_handler/__init__.py
-drwxr-xr-x   0 fabriciocravo   (501) staff       (20)        0 2024-04-04 13:21:16.526293 mobspy-2.3.4/mobspy/data_handler/__pycache__/
--rw-r--r--   0 fabriciocravo   (501) staff       (20)      144 2024-01-28 20:38:15.000000 mobspy-2.3.4/mobspy/data_handler/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0 fabriciocravo   (501) staff       (20)     2558 2024-01-28 20:38:15.000000 mobspy-2.3.4/mobspy/data_handler/__pycache__/process_result_data.cpython-310.pyc
--rw-r--r--   0 fabriciocravo   (501) staff       (20)     6701 2024-01-28 20:38:15.000000 mobspy-2.3.4/mobspy/data_handler/__pycache__/time_series_object.cpython-310.pyc
--rw-r--r--   0 fabriciocravo   (501) staff       (20)     5329 2024-02-28 23:26:14.000000 mobspy-2.3.4/mobspy/data_handler/process_result_data.py
--rw-r--r--   0 fabriciocravo   (501) staff       (20)     8060 2024-02-22 02:35:14.000000 mobspy-2.3.4/mobspy/data_handler/time_series_object.py
-drwxr-xr-x   0 fabriciocravo   (501) staff       (20)        0 2024-04-04 13:21:16.562476 mobspy-2.3.4/mobspy/modules/
--rw-r--r--   0 fabriciocravo   (501) staff       (20)        0 2023-06-15 12:59:57.000000 mobspy-2.3.4/mobspy/modules/__init__.py
-drwxr-xr-x   0 fabriciocravo   (501) staff       (20)        0 2024-04-04 13:21:16.598108 mobspy-2.3.4/mobspy/modules/__pycache__/
--rw-r--r--   0 fabriciocravo   (501) staff       (20)      139 2024-01-28 20:38:15.000000 mobspy-2.3.4/mobspy/modules/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0 fabriciocravo   (501) staff       (20)     5212 2024-01-28 20:38:15.000000 mobspy-2.3.4/mobspy/modules/__pycache__/class_of_meta_specie_named_any.cpython-310.pyc
--rw-r--r--   0 fabriciocravo   (501) staff       (20)     3246 2024-01-28 20:38:15.000000 mobspy-2.3.4/mobspy/modules/__pycache__/event_functions.cpython-310.pyc
--rw-r--r--   0 fabriciocravo   (501) staff       (20)     7912 2024-01-28 20:38:15.000000 mobspy-2.3.4/mobspy/modules/__pycache__/function_rate_code.cpython-310.pyc
--rw-r--r--   0 fabriciocravo   (501) staff       (20)    12108 2024-01-28 20:38:15.000000 mobspy-2.3.4/mobspy/modules/__pycache__/logic_operator_objects.cpython-310.pyc
--rw-r--r--   0 fabriciocravo   (501) staff       (20)    52292 2024-01-28 20:38:15.000000 mobspy-2.3.4/mobspy/modules/__pycache__/meta_class.cpython-310.pyc
--rw-r--r--   0 fabriciocravo   (501) staff       (20)     4479 2024-01-28 20:38:15.000000 mobspy-2.3.4/mobspy/modules/__pycache__/meta_class_utils.cpython-310.pyc
--rw-r--r--   0 fabriciocravo   (501) staff       (20)    19989 2024-01-28 20:38:15.000000 mobspy-2.3.4/mobspy/modules/__pycache__/mobspy_expressions.cpython-310.pyc
--rw-r--r--   0 fabriciocravo   (501) staff       (20)     2317 2024-01-28 20:38:15.000000 mobspy-2.3.4/mobspy/modules/__pycache__/mobspy_parameters.cpython-310.pyc
--rw-r--r--   0 fabriciocravo   (501) staff       (20)    12697 2024-01-28 20:38:15.000000 mobspy-2.3.4/mobspy/modules/__pycache__/order_operators.cpython-310.pyc
--rw-r--r--   0 fabriciocravo   (501) staff       (20)    12942 2024-01-28 20:38:15.000000 mobspy-2.3.4/mobspy/modules/__pycache__/reaction_construction_nb.cpython-310.pyc
--rw-r--r--   0 fabriciocravo   (501) staff       (20)    13600 2024-01-28 20:38:15.000000 mobspy-2.3.4/mobspy/modules/__pycache__/reaction_construction_nb_parallel.cpython-310.pyc
--rw-r--r--   0 fabriciocravo   (501) staff       (20)     3250 2024-01-28 20:38:15.000000 mobspy-2.3.4/mobspy/modules/__pycache__/set_counts_module.cpython-310.pyc
--rw-r--r--   0 fabriciocravo   (501) staff       (20)     3390 2024-01-28 20:38:15.000000 mobspy-2.3.4/mobspy/modules/__pycache__/species_string_generator.cpython-310.pyc
--rw-r--r--   0 fabriciocravo   (501) staff       (20)     5299 2024-01-28 20:38:15.000000 mobspy-2.3.4/mobspy/modules/__pycache__/unit_handler.cpython-310.pyc
--rw-r--r--   0 fabriciocravo   (501) staff       (20)      455 2024-01-28 20:38:15.000000 mobspy-2.3.4/mobspy/modules/__pycache__/user_functions.cpython-310.pyc
--rw-r--r--   0 fabriciocravo   (501) staff       (20)     6281 2024-03-20 17:33:27.000000 mobspy-2.3.4/mobspy/modules/assignments_implementation.py
--rw-r--r--   0 fabriciocravo   (501) staff       (20)     5146 2024-02-25 21:08:54.000000 mobspy-2.3.4/mobspy/modules/class_of_meta_specie_named_any.py
--rw-r--r--   0 fabriciocravo   (501) staff       (20)     1827 2024-02-25 21:10:55.000000 mobspy-2.3.4/mobspy/modules/context_related_scripts.py
--rw-r--r--   0 fabriciocravo   (501) staff       (20)     5110 2023-06-25 17:16:47.000000 mobspy-2.3.4/mobspy/modules/event_functions.py
--rw-r--r--   0 fabriciocravo   (501) staff       (20)    12554 2024-02-29 01:47:29.000000 mobspy-2.3.4/mobspy/modules/function_rate_code.py
--rw-r--r--   0 fabriciocravo   (501) staff       (20)    13014 2024-02-26 15:53:24.000000 mobspy-2.3.4/mobspy/modules/logic_operator_objects.py
--rw-r--r--   0 fabriciocravo   (501) staff       (20)    71462 2024-03-20 17:33:27.000000 mobspy-2.3.4/mobspy/modules/meta_class.py
--rw-r--r--   0 fabriciocravo   (501) staff       (20)     5240 2023-12-21 15:41:16.000000 mobspy-2.3.4/mobspy/modules/meta_class_utils.py
--rw-r--r--   0 fabriciocravo   (501) staff       (20)    36116 2024-03-19 17:20:49.000000 mobspy-2.3.4/mobspy/modules/mobspy_expressions.py
--rw-r--r--   0 fabriciocravo   (501) staff       (20)     5042 2024-02-26 16:20:28.000000 mobspy-2.3.4/mobspy/modules/mobspy_parameters.py
--rw-r--r--   0 fabriciocravo   (501) staff       (20)    15158 2023-06-15 12:59:57.000000 mobspy-2.3.4/mobspy/modules/order_operators.py
--rw-r--r--   0 fabriciocravo   (501) staff       (20)    17445 2024-02-29 01:46:20.000000 mobspy-2.3.4/mobspy/modules/reaction_construction_nb.py
--rw-r--r--   0 fabriciocravo   (501) staff       (20)    18457 2023-06-15 12:59:57.000000 mobspy-2.3.4/mobspy/modules/reaction_construction_nb_parallel.py
--rw-r--r--   0 fabriciocravo   (501) staff       (20)     4363 2024-02-25 00:46:32.000000 mobspy-2.3.4/mobspy/modules/set_counts_module.py
--rw-r--r--   0 fabriciocravo   (501) staff       (20)     4143 2023-08-03 14:16:13.000000 mobspy-2.3.4/mobspy/modules/species_string_generator.py
--rw-r--r--   0 fabriciocravo   (501) staff       (20)     7435 2023-12-14 12:58:51.000000 mobspy-2.3.4/mobspy/modules/unit_handler.py
--rw-r--r--   0 fabriciocravo   (501) staff       (20)      443 2024-02-26 16:20:28.000000 mobspy-2.3.4/mobspy/modules/user_functions.py
-drwxr-xr-x   0 fabriciocravo   (501) staff       (20)        0 2024-04-04 13:21:16.604072 mobspy-2.3.4/mobspy/parameter_estimation_data_loader/
--rw-r--r--   0 fabriciocravo   (501) staff       (20)        0 2024-02-28 22:21:33.000000 mobspy-2.3.4/mobspy/parameter_estimation_data_loader/__init__.py
--rw-r--r--   0 fabriciocravo   (501) staff       (20)      912 2024-01-31 10:55:41.000000 mobspy-2.3.4/mobspy/parameter_estimation_data_loader/data_loader.py
--rw-r--r--   0 fabriciocravo   (501) staff       (20)     7595 2024-03-20 19:27:19.000000 mobspy-2.3.4/mobspy/parameter_estimation_data_loader/parameter_estimation_scripts.py
-drwxr-xr-x   0 fabriciocravo   (501) staff       (20)        0 2024-04-04 13:21:16.608944 mobspy-2.3.4/mobspy/parameter_scripts/
--rw-r--r--   0 fabriciocravo   (501) staff       (20)        0 2023-06-15 12:59:57.000000 mobspy-2.3.4/mobspy/parameter_scripts/__init__.py
-drwxr-xr-x   0 fabriciocravo   (501) staff       (20)        0 2024-04-04 13:21:16.615301 mobspy-2.3.4/mobspy/parameter_scripts/__pycache__/
--rw-r--r--   0 fabriciocravo   (501) staff       (20)      149 2024-01-28 20:38:15.000000 mobspy-2.3.4/mobspy/parameter_scripts/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0 fabriciocravo   (501) staff       (20)     3070 2024-01-28 20:38:15.000000 mobspy-2.3.4/mobspy/parameter_scripts/__pycache__/parameter_reader.cpython-310.pyc
--rw-r--r--   0 fabriciocravo   (501) staff       (20)     1563 2024-01-28 20:38:15.000000 mobspy-2.3.4/mobspy/parameter_scripts/__pycache__/parametric_sweeps.cpython-310.pyc
--rw-r--r--   0 fabriciocravo   (501) staff       (20)     8189 2024-03-08 01:01:48.000000 mobspy-2.3.4/mobspy/parameter_scripts/parameter_reader.py
--rw-r--r--   0 fabriciocravo   (501) staff       (20)     1957 2024-02-01 12:50:35.000000 mobspy-2.3.4/mobspy/parameter_scripts/parametric_sweeps.py
-drwxr-xr-x   0 fabriciocravo   (501) staff       (20)        0 2024-04-04 13:21:16.620877 mobspy-2.3.4/mobspy/parameters/
--rw-r--r--   0 fabriciocravo   (501) staff       (20)     1463 2023-06-15 12:59:57.000000 mobspy-2.3.4/mobspy/parameters/README.md
--rw-r--r--   0 fabriciocravo   (501) staff       (20)        0 2023-06-15 12:59:57.000000 mobspy-2.3.4/mobspy/parameters/__init__.py
-drwxr-xr-x   0 fabriciocravo   (501) staff       (20)        0 2024-04-04 13:21:16.626919 mobspy-2.3.4/mobspy/parameters/__pycache__/
--rw-r--r--   0 fabriciocravo   (501) staff       (20)      142 2024-01-28 20:38:15.000000 mobspy-2.3.4/mobspy/parameters/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0 fabriciocravo   (501) staff       (20)     1151 2024-01-28 20:38:15.000000 mobspy-2.3.4/mobspy/parameters/__pycache__/default_reader.cpython-310.pyc
--rw-r--r--   0 fabriciocravo   (501) staff       (20)     1319 2024-01-28 20:38:15.000000 mobspy-2.3.4/mobspy/parameters/__pycache__/example_reader.cpython-310.pyc
--rw-r--r--   0 fabriciocravo   (501) staff       (20)     1188 2024-01-30 18:15:37.000000 mobspy-2.3.4/mobspy/parameters/default_reader.py
--rw-r--r--   0 fabriciocravo   (501) staff       (20)     1285 2024-01-30 17:59:16.000000 mobspy-2.3.4/mobspy/parameters/example_reader.py
-drwxr-xr-x   0 fabriciocravo   (501) staff       (20)        0 2024-04-04 13:21:16.632041 mobspy-2.3.4/mobspy/plot_params/
--rw-r--r--   0 fabriciocravo   (501) staff       (20)        0 2023-06-15 12:59:57.000000 mobspy-2.3.4/mobspy/plot_params/__init__.py
-drwxr-xr-x   0 fabriciocravo   (501) staff       (20)        0 2024-04-04 13:21:16.638002 mobspy-2.3.4/mobspy/plot_params/__pycache__/
--rw-r--r--   0 fabriciocravo   (501) staff       (20)      143 2024-01-28 20:38:15.000000 mobspy-2.3.4/mobspy/plot_params/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0 fabriciocravo   (501) staff       (20)      351 2024-01-28 20:38:15.000000 mobspy-2.3.4/mobspy/plot_params/__pycache__/default_plot_reader.cpython-310.pyc
--rw-r--r--   0 fabriciocravo   (501) staff       (20)     1390 2024-01-28 20:38:15.000000 mobspy-2.3.4/mobspy/plot_params/__pycache__/example_plot_reader.cpython-310.pyc
--rw-r--r--   0 fabriciocravo   (501) staff       (20)      184 2023-06-15 12:59:57.000000 mobspy-2.3.4/mobspy/plot_params/default_plot_reader.py
--rw-r--r--   0 fabriciocravo   (501) staff       (20)     1573 2024-03-29 08:28:41.000000 mobspy-2.3.4/mobspy/plot_params/example_plot_reader.py
-drwxr-xr-x   0 fabriciocravo   (501) staff       (20)        0 2024-04-04 13:21:16.646095 mobspy-2.3.4/mobspy/plot_scripts/
--rw-r--r--   0 fabriciocravo   (501) staff       (20)        0 2024-03-28 14:29:54.000000 mobspy-2.3.4/mobspy/plot_scripts/__init__.py
--rw-r--r--   0 fabriciocravo   (501) staff       (20)     9268 2024-03-29 08:13:46.000000 mobspy-2.3.4/mobspy/plot_scripts/default_plots.py
--rw-r--r--   0 fabriciocravo   (501) staff       (20)    16874 2024-03-29 08:23:04.000000 mobspy-2.3.4/mobspy/plot_scripts/hierarchical_plot.py
--rw-r--r--   0 fabriciocravo   (501) staff       (20)     2482 2024-03-28 14:29:54.000000 mobspy-2.3.4/mobspy/plot_scripts/process_plot_data.py
--rw-r--r--   0 fabriciocravo   (501) staff       (20)     3885 2024-03-28 14:34:48.000000 mobspy-2.3.4/mobspy/plot_scripts/statistics_calculations.py
-drwxr-xr-x   0 fabriciocravo   (501) staff       (20)        0 2024-04-04 13:21:16.652504 mobspy-2.3.4/mobspy/sbml_simulator/
--rw-r--r--   0 fabriciocravo   (501) staff       (20)     8702 2024-03-20 17:46:34.000000 mobspy-2.3.4/mobspy/sbml_simulator/SBMLWriter.py
--rw-r--r--   0 fabriciocravo   (501) staff       (20)        0 2023-06-15 12:59:57.000000 mobspy-2.3.4/mobspy/sbml_simulator/__init__.py
-drwxr-xr-x   0 fabriciocravo   (501) staff       (20)        0 2024-04-04 13:21:16.659315 mobspy-2.3.4/mobspy/sbml_simulator/__pycache__/
--rw-r--r--   0 fabriciocravo   (501) staff       (20)     5705 2024-01-28 20:38:15.000000 mobspy-2.3.4/mobspy/sbml_simulator/__pycache__/SBMLWriter.cpython-310.pyc
--rw-r--r--   0 fabriciocravo   (501) staff       (20)      146 2024-01-28 20:38:15.000000 mobspy-2.3.4/mobspy/sbml_simulator/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0 fabriciocravo   (501) staff       (20)     1040 2024-01-28 20:38:15.000000 mobspy-2.3.4/mobspy/sbml_simulator/__pycache__/builder.cpython-310.pyc
--rw-r--r--   0 fabriciocravo   (501) staff       (20)     8808 2024-01-28 20:38:15.000000 mobspy-2.3.4/mobspy/sbml_simulator/__pycache__/run.cpython-310.pyc
--rw-r--r--   0 fabriciocravo   (501) staff       (20)     1029 2024-03-20 17:44:19.000000 mobspy-2.3.4/mobspy/sbml_simulator/builder.py
--rw-r--r--   0 fabriciocravo   (501) staff       (20)    11972 2024-03-20 17:43:06.000000 mobspy-2.3.4/mobspy/sbml_simulator/run.py
--rw-r--r--   0 fabriciocravo   (501) staff       (20)    39340 2024-03-29 08:12:30.000000 mobspy-2.3.4/mobspy/simulation.py
-drwxr-xr-x   0 fabriciocravo   (501) staff       (20)        0 2024-04-04 13:21:16.661401 mobspy-2.3.4/mobspy/simulation_logging/
--rw-r--r--   0 fabriciocravo   (501) staff       (20)        0 2023-06-15 12:59:57.000000 mobspy-2.3.4/mobspy/simulation_logging/__init__.py
-drwxr-xr-x   0 fabriciocravo   (501) staff       (20)        0 2024-04-04 13:21:16.667389 mobspy-2.3.4/mobspy/simulation_logging/__pycache__/
--rw-r--r--   0 fabriciocravo   (501) staff       (20)      150 2024-01-28 20:38:15.000000 mobspy-2.3.4/mobspy/simulation_logging/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0 fabriciocravo   (501) staff       (20)     1212 2024-01-28 20:38:15.000000 mobspy-2.3.4/mobspy/simulation_logging/__pycache__/log_scripts.cpython-310.pyc
--rw-r--r--   0 fabriciocravo   (501) staff       (20)      986 2024-01-28 20:25:20.000000 mobspy-2.3.4/mobspy/simulation_logging/log_scripts.py
-drwxr-xr-x   0 fabriciocravo   (501) staff       (20)        0 2024-04-04 13:21:16.509383 mobspy-2.3.4/mobspy.egg-info/
--rw-r--r--   0 fabriciocravo   (501) staff       (20)     7577 2024-04-04 13:21:14.000000 mobspy-2.3.4/mobspy.egg-info/PKG-INFO
--rw-r--r--   0 fabriciocravo   (501) staff       (20)    18477 2024-04-04 13:21:15.000000 mobspy-2.3.4/mobspy.egg-info/SOURCES.txt
--rw-r--r--   0 fabriciocravo   (501) staff       (20)        1 2024-04-04 13:21:14.000000 mobspy-2.3.4/mobspy.egg-info/dependency_links.txt
--rw-r--r--   0 fabriciocravo   (501) staff       (20)       76 2024-04-04 13:21:14.000000 mobspy-2.3.4/mobspy.egg-info/requires.txt
--rw-r--r--   0 fabriciocravo   (501) staff       (20)        7 2024-04-04 13:21:14.000000 mobspy-2.3.4/mobspy.egg-info/top_level.txt
--rw-r--r--   0 fabriciocravo   (501) staff       (20)       77 2023-06-15 12:59:57.000000 mobspy-2.3.4/requirements.txt
--rw-r--r--   0 fabriciocravo   (501) staff       (20)       38 2024-04-04 13:21:16.769705 mobspy-2.3.4/setup.cfg
--rw-r--r--   0 fabriciocravo   (501) staff       (20)      767 2023-06-15 12:59:57.000000 mobspy-2.3.4/setup.py
-drwxr-xr-x   0 fabriciocravo   (501) staff       (20)        0 2024-04-04 13:21:16.674873 mobspy-2.3.4/test_plot_images/
--rw-r--r--   0 fabriciocravo   (501) staff       (20)    11307 2024-04-04 13:14:42.000000 mobspy-2.3.4/test_plot_images/constant_tree.png
--rw-r--r--   0 fabriciocravo   (501) staff       (20)    45198 2024-04-04 13:14:42.000000 mobspy-2.3.4/test_plot_images/deterministic_tree.png
--rw-r--r--   0 fabriciocravo   (501) staff       (20)    57082 2024-04-04 13:14:42.000000 mobspy-2.3.4/test_plot_images/stochastic_tree.png
--rw-r--r--   0 fabriciocravo   (501) staff       (20)    39648 2024-03-08 01:16:27.000000 mobspy-2.3.4/test_script.py
-drwxr-xr-x   0 fabriciocravo   (501) staff       (20)        0 2024-04-04 13:21:16.767231 mobspy-2.3.4/test_tools/
--rw-r--r--   0 fabriciocravo   (501) staff       (20)      170 2023-06-15 12:59:57.000000 mobspy-2.3.4/test_tools/model_1.txt
--rw-r--r--   0 fabriciocravo   (501) staff       (20)      241 2023-06-26 11:54:08.000000 mobspy-2.3.4/test_tools/model_10.txt
--rw-r--r--   0 fabriciocravo   (501) staff       (20)      299 2023-06-15 12:59:57.000000 mobspy-2.3.4/test_tools/model_11.txt
--rw-r--r--   0 fabriciocravo   (501) staff       (20)      393 2023-06-15 12:59:57.000000 mobspy-2.3.4/test_tools/model_12.txt
--rw-r--r--   0 fabriciocravo   (501) staff       (20)      490 2023-06-15 12:59:57.000000 mobspy-2.3.4/test_tools/model_13.txt
--rw-r--r--   0 fabriciocravo   (501) staff       (20)      487 2023-06-15 12:59:57.000000 mobspy-2.3.4/test_tools/model_14.txt
--rw-r--r--   0 fabriciocravo   (501) staff       (20)      550 2023-06-15 12:59:57.000000 mobspy-2.3.4/test_tools/model_15.txt
--rw-r--r--   0 fabriciocravo   (501) staff       (20)      286 2023-06-15 12:59:57.000000 mobspy-2.3.4/test_tools/model_16.txt
--rw-r--r--   0 fabriciocravo   (501) staff       (20)      273 2023-06-15 12:59:57.000000 mobspy-2.3.4/test_tools/model_17.txt
--rw-r--r--   0 fabriciocravo   (501) staff       (20)      118 2023-06-15 12:59:57.000000 mobspy-2.3.4/test_tools/model_18.txt
--rw-r--r--   0 fabriciocravo   (501) staff       (20)      970 2023-06-15 12:59:57.000000 mobspy-2.3.4/test_tools/model_19.txt
--rw-r--r--   0 fabriciocravo   (501) staff       (20)      396 2023-06-15 12:59:57.000000 mobspy-2.3.4/test_tools/model_2.txt
--rw-r--r--   0 fabriciocravo   (501) staff       (20)      326 2023-06-15 12:59:57.000000 mobspy-2.3.4/test_tools/model_20.txt
--rw-r--r--   0 fabriciocravo   (501) staff       (20)     1453 2023-06-15 12:59:57.000000 mobspy-2.3.4/test_tools/model_21.txt
--rw-r--r--   0 fabriciocravo   (501) staff       (20)      471 2023-07-03 11:25:39.000000 mobspy-2.3.4/test_tools/model_22.txt
--rw-r--r--   0 fabriciocravo   (501) staff       (20)      186 2023-06-15 12:59:57.000000 mobspy-2.3.4/test_tools/model_23.txt
--rw-r--r--   0 fabriciocravo   (501) staff       (20)      605 2023-06-15 12:59:57.000000 mobspy-2.3.4/test_tools/model_24.txt
--rw-r--r--   0 fabriciocravo   (501) staff       (20)       81 2023-06-15 12:59:57.000000 mobspy-2.3.4/test_tools/model_25.txt
--rw-r--r--   0 fabriciocravo   (501) staff       (20)      518 2023-07-03 11:30:10.000000 mobspy-2.3.4/test_tools/model_26.txt
--rw-r--r--   0 fabriciocravo   (501) staff       (20)      145 2023-06-15 12:59:57.000000 mobspy-2.3.4/test_tools/model_27.txt
--rw-r--r--   0 fabriciocravo   (501) staff       (20)      400 2023-06-15 12:59:57.000000 mobspy-2.3.4/test_tools/model_28.txt
--rw-r--r--   0 fabriciocravo   (501) staff       (20)      395 2023-06-15 12:59:57.000000 mobspy-2.3.4/test_tools/model_29.txt
--rw-r--r--   0 fabriciocravo   (501) staff       (20)     3154 2023-06-15 12:59:57.000000 mobspy-2.3.4/test_tools/model_3.txt
--rw-r--r--   0 fabriciocravo   (501) staff       (20)      468 2023-06-15 12:59:57.000000 mobspy-2.3.4/test_tools/model_30.txt
--rw-r--r--   0 fabriciocravo   (501) staff       (20)    55662 2023-06-15 12:59:57.000000 mobspy-2.3.4/test_tools/model_31.txt
--rw-r--r--   0 fabriciocravo   (501) staff       (20)      129 2023-06-15 12:59:57.000000 mobspy-2.3.4/test_tools/model_32.txt
--rw-r--r--   0 fabriciocravo   (501) staff       (20)      831 2023-07-03 15:00:26.000000 mobspy-2.3.4/test_tools/model_33.txt
--rw-r--r--   0 fabriciocravo   (501) staff       (20)      123 2023-07-03 23:04:22.000000 mobspy-2.3.4/test_tools/model_34.txt
--rw-r--r--   0 fabriciocravo   (501) staff       (20)       61 2023-07-30 20:48:11.000000 mobspy-2.3.4/test_tools/model_35.txt
--rw-r--r--   0 fabriciocravo   (501) staff       (20)      175 2023-08-01 18:04:20.000000 mobspy-2.3.4/test_tools/model_36.txt
--rw-r--r--   0 fabriciocravo   (501) staff       (20)      391 2023-08-03 14:43:06.000000 mobspy-2.3.4/test_tools/model_37.txt
--rw-r--r--   0 fabriciocravo   (501) staff       (20)     1427 2023-08-19 22:03:11.000000 mobspy-2.3.4/test_tools/model_38.txt
--rw-r--r--   0 fabriciocravo   (501) staff       (20)     2853 2023-08-19 22:23:06.000000 mobspy-2.3.4/test_tools/model_39.txt
--rw-r--r--   0 fabriciocravo   (501) staff       (20)      727 2023-06-15 12:59:57.000000 mobspy-2.3.4/test_tools/model_4.txt
--rw-r--r--   0 fabriciocravo   (501) staff       (20)     2210 2023-11-15 12:57:45.000000 mobspy-2.3.4/test_tools/model_40.txt
--rw-r--r--   0 fabriciocravo   (501) staff       (20)     1412 2023-11-15 12:57:45.000000 mobspy-2.3.4/test_tools/model_41.txt
--rw-r--r--   0 fabriciocravo   (501) staff       (20)      178 2023-11-15 12:57:45.000000 mobspy-2.3.4/test_tools/model_42.txt
--rw-r--r--   0 fabriciocravo   (501) staff       (20)      419 2023-11-17 12:18:00.000000 mobspy-2.3.4/test_tools/model_43.txt
--rw-r--r--   0 fabriciocravo   (501) staff       (20)      197 2024-01-31 16:54:44.000000 mobspy-2.3.4/test_tools/model_44.txt
--rw-r--r--   0 fabriciocravo   (501) staff       (20)     8874 2024-02-22 02:44:14.000000 mobspy-2.3.4/test_tools/model_45.txt
--rw-r--r--   0 fabriciocravo   (501) staff       (20)      317 2024-02-24 00:21:58.000000 mobspy-2.3.4/test_tools/model_46.txt
--rw-r--r--   0 fabriciocravo   (501) staff       (20)      243 2024-02-24 13:50:27.000000 mobspy-2.3.4/test_tools/model_47.txt
--rw-r--r--   0 fabriciocravo   (501) staff       (20)      559 2023-06-15 12:59:57.000000 mobspy-2.3.4/test_tools/model_5.txt
--rw-r--r--   0 fabriciocravo   (501) staff       (20)      389 2023-07-03 10:56:19.000000 mobspy-2.3.4/test_tools/model_6.txt
--rw-r--r--   0 fabriciocravo   (501) staff       (20)     1362 2023-07-03 11:02:54.000000 mobspy-2.3.4/test_tools/model_7.txt
--rw-r--r--   0 fabriciocravo   (501) staff       (20)      433 2023-06-15 12:59:57.000000 mobspy-2.3.4/test_tools/model_8.txt
--rw-r--r--   0 fabriciocravo   (501) staff       (20)      736 2023-06-15 12:59:57.000000 mobspy-2.3.4/test_tools/model_9.txt
--rw-r--r--   0 fabriciocravo   (501) staff       (20)       60 2023-06-15 12:59:57.000000 mobspy-2.3.4/useful_parameters.json
+drwxr-xr-x   0 fabriciocravo   (501) staff       (20)        0 2024-04-11 13:12:08.131281 mobspy-2.3.5/
+drwxr-xr-x   0 fabriciocravo   (501) staff       (20)        0 2024-04-11 13:12:07.392538 mobspy-2.3.5/.github/
+drwxr-xr-x   0 fabriciocravo   (501) staff       (20)        0 2024-04-11 13:12:07.424298 mobspy-2.3.5/.github/workflows/
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)     1201 2023-06-15 12:59:57.000000 mobspy-2.3.5/.github/workflows/python-app.yml
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)      415 2024-04-09 17:41:00.000000 mobspy-2.3.5/.gitignore
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)     1034 2024-02-26 16:22:21.000000 mobspy-2.3.5/.readthedocs.yaml
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)     1068 2023-06-15 12:59:57.000000 mobspy-2.3.5/LICENSE
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)     7577 2024-04-11 13:12:08.130890 mobspy-2.3.5/PKG-INFO
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)     6331 2024-03-08 01:34:03.000000 mobspy-2.3.5/README.md
+drwxr-xr-x   0 fabriciocravo   (501) staff       (20)        0 2024-04-11 13:12:07.453972 mobspy-2.3.5/docs/
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)      634 2024-01-28 20:38:15.000000 mobspy-2.3.5/docs/Makefile
+drwxr-xr-x   0 fabriciocravo   (501) staff       (20)        0 2024-04-11 13:12:07.484504 mobspy-2.3.5/docs/Notebooks/
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)   127718 2024-01-28 20:38:15.000000 mobspy-2.3.5/docs/Notebooks/01_Basic_Intro.ipynb
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)     6534 2024-01-28 20:38:15.000000 mobspy-2.3.5/docs/Notebooks/02_Reaction_Inheritance.ipynb
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)     8067 2024-01-28 20:38:15.000000 mobspy-2.3.5/docs/Notebooks/03_Characteristics.ipynb
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)     2210 2024-01-28 20:38:15.000000 mobspy-2.3.5/docs/Notebooks/04_Characteristic_restriction.ipynb
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)     5563 2024-01-28 20:38:15.000000 mobspy-2.3.5/docs/Notebooks/05_For_Loops.ipynb
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)     6167 2024-01-28 20:38:15.000000 mobspy-2.3.5/docs/Notebooks/06_Order_Matters.ipynb
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)    12448 2024-01-28 20:38:15.000000 mobspy-2.3.5/docs/Notebooks/07_Initial_Condition.ipynb
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)     5154 2024-01-28 20:38:15.000000 mobspy-2.3.5/docs/Notebooks/08_Units.ipynb
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)   106408 2024-01-28 20:38:15.000000 mobspy-2.3.5/docs/Notebooks/09_Result_Data.ipynb
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)    25996 2024-01-28 20:38:15.000000 mobspy-2.3.5/docs/Notebooks/10_Reaction_Rates.ipynb
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)     3942 2024-01-28 20:38:15.000000 mobspy-2.3.5/docs/Notebooks/11_Looping_Through_Species.ipynb
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)     4426 2024-01-28 20:38:15.000000 mobspy-2.3.5/docs/Notebooks/12_Born_Species.ipynb
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)    80668 2024-01-28 20:38:15.000000 mobspy-2.3.5/docs/Notebooks/13_Events.ipynb
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)    48456 2024-01-28 20:38:15.000000 mobspy-2.3.5/docs/Notebooks/14_Concatenating_Simulations.ipynb
+drwxr-xr-x   0 fabriciocravo   (501) staff       (20)        0 2024-04-11 13:12:07.486076 mobspy-2.3.5/docs/_autosummary/
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)       67 2024-01-28 20:38:15.000000 mobspy-2.3.5/docs/_autosummary/mobspy.rst
+drwxr-xr-x   0 fabriciocravo   (501) staff       (20)        0 2024-04-11 13:12:07.394725 mobspy-2.3.5/docs/_build/
+drwxr-xr-x   0 fabriciocravo   (501) staff       (20)        0 2024-04-11 13:12:07.530839 mobspy-2.3.5/docs/_build/doctrees/
+drwxr-xr-x   0 fabriciocravo   (501) staff       (20)        0 2024-04-11 13:12:07.563975 mobspy-2.3.5/docs/_build/doctrees/Notebooks/
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)    95114 2024-01-28 20:38:15.000000 mobspy-2.3.5/docs/_build/doctrees/Notebooks/01_Basic_Intro.doctree
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)    23601 2024-01-28 20:38:15.000000 mobspy-2.3.5/docs/_build/doctrees/Notebooks/02_Reaction_Inheritance.doctree
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)    30820 2024-01-28 20:38:15.000000 mobspy-2.3.5/docs/_build/doctrees/Notebooks/03_Characteristics.doctree
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)     7466 2024-01-28 20:38:15.000000 mobspy-2.3.5/docs/_build/doctrees/Notebooks/04_Characteristic_restriction.doctree
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)    24161 2024-01-28 20:38:15.000000 mobspy-2.3.5/docs/_build/doctrees/Notebooks/05_For_Loops.doctree
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)    21599 2024-01-28 20:38:15.000000 mobspy-2.3.5/docs/_build/doctrees/Notebooks/06_Order_Matters.doctree
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)    50076 2024-01-28 20:38:15.000000 mobspy-2.3.5/docs/_build/doctrees/Notebooks/07_Initial_Condition.doctree
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)    18699 2024-01-28 20:38:15.000000 mobspy-2.3.5/docs/_build/doctrees/Notebooks/08_Units.doctree
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)    41471 2024-01-28 20:38:15.000000 mobspy-2.3.5/docs/_build/doctrees/Notebooks/09_Result_Data.doctree
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)    28500 2024-01-28 20:38:15.000000 mobspy-2.3.5/docs/_build/doctrees/Notebooks/10_Reaction_Rates.doctree
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)    15272 2024-01-28 20:38:15.000000 mobspy-2.3.5/docs/_build/doctrees/Notebooks/11_Looping_Through_Species.doctree
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)    17080 2024-01-28 20:38:15.000000 mobspy-2.3.5/docs/_build/doctrees/Notebooks/12_Born_Species.doctree
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)    39545 2024-01-28 20:38:15.000000 mobspy-2.3.5/docs/_build/doctrees/Notebooks/13_Events.doctree
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)    15325 2024-01-28 20:38:15.000000 mobspy-2.3.5/docs/_build/doctrees/Notebooks/14_Concatenating_Simulations.doctree
+drwxr-xr-x   0 fabriciocravo   (501) staff       (20)        0 2024-04-11 13:12:07.566372 mobspy-2.3.5/docs/_build/doctrees/_autosummary/
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)     2971 2024-01-28 20:38:15.000000 mobspy-2.3.5/docs/_build/doctrees/_autosummary/mobspy.doctree
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)     4285 2024-01-28 20:38:15.000000 mobspy-2.3.5/docs/_build/doctrees/api.doctree
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)  1736636 2024-01-28 20:38:15.000000 mobspy-2.3.5/docs/_build/doctrees/environment.pickle
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)     2754 2024-01-28 20:38:15.000000 mobspy-2.3.5/docs/_build/doctrees/for_local_use.doctree
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)     4048 2024-01-28 20:38:15.000000 mobspy-2.3.5/docs/_build/doctrees/index.doctree
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)    26568 2024-01-28 20:38:15.000000 mobspy-2.3.5/docs/_build/doctrees/mobspy.data_handler.doctree
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)    67412 2024-01-28 20:38:15.000000 mobspy-2.3.5/docs/_build/doctrees/mobspy.doctree
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)   490595 2024-01-28 20:38:15.000000 mobspy-2.3.5/docs/_build/doctrees/mobspy.modules.doctree
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)    16088 2024-01-28 20:38:15.000000 mobspy-2.3.5/docs/_build/doctrees/mobspy.parameter_scripts.doctree
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)     8486 2024-01-28 20:38:15.000000 mobspy-2.3.5/docs/_build/doctrees/mobspy.parameters.doctree
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)     8077 2024-01-28 20:38:15.000000 mobspy-2.3.5/docs/_build/doctrees/mobspy.plot_params.doctree
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)    86993 2024-01-28 20:38:15.000000 mobspy-2.3.5/docs/_build/doctrees/mobspy.plot_scripts.doctree
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)    33712 2024-01-28 20:38:15.000000 mobspy-2.3.5/docs/_build/doctrees/mobspy.sbml_simulator.doctree
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)     9059 2024-01-28 20:38:15.000000 mobspy-2.3.5/docs/_build/doctrees/mobspy.simulation_logging.doctree
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)     2767 2024-01-28 20:38:15.000000 mobspy-2.3.5/docs/_build/doctrees/modules.doctree
+drwxr-xr-x   0 fabriciocravo   (501) staff       (20)        0 2024-04-11 13:12:07.590401 mobspy-2.3.5/docs/_build/doctrees/nbsphinx/
+drwxr-xr-x   0 fabriciocravo   (501) staff       (20)        0 2024-04-11 13:12:07.614155 mobspy-2.3.5/docs/_build/doctrees/nbsphinx/Notebooks/
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)   127718 2024-01-28 20:38:15.000000 mobspy-2.3.5/docs/_build/doctrees/nbsphinx/Notebooks/01_Basic_Intro.ipynb
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)     6534 2024-01-28 20:38:15.000000 mobspy-2.3.5/docs/_build/doctrees/nbsphinx/Notebooks/02_Reaction_Inheritance.ipynb
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)     8067 2024-01-28 20:38:15.000000 mobspy-2.3.5/docs/_build/doctrees/nbsphinx/Notebooks/03_Characteristics.ipynb
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)     2210 2024-01-28 20:38:15.000000 mobspy-2.3.5/docs/_build/doctrees/nbsphinx/Notebooks/04_Characteristic_restriction.ipynb
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)     5563 2024-01-28 20:38:15.000000 mobspy-2.3.5/docs/_build/doctrees/nbsphinx/Notebooks/05_For_Loops.ipynb
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)     6167 2024-01-28 20:38:15.000000 mobspy-2.3.5/docs/_build/doctrees/nbsphinx/Notebooks/06_Order_Matters.ipynb
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)    12448 2024-01-28 20:38:15.000000 mobspy-2.3.5/docs/_build/doctrees/nbsphinx/Notebooks/07_Initial_Condition.ipynb
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)     5154 2024-01-28 20:38:15.000000 mobspy-2.3.5/docs/_build/doctrees/nbsphinx/Notebooks/08_Units.ipynb
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)   106408 2024-01-28 20:38:15.000000 mobspy-2.3.5/docs/_build/doctrees/nbsphinx/Notebooks/09_Result_Data.ipynb
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)    25996 2024-01-28 20:38:15.000000 mobspy-2.3.5/docs/_build/doctrees/nbsphinx/Notebooks/10_Reaction_Rates.ipynb
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)     3942 2024-01-28 20:38:15.000000 mobspy-2.3.5/docs/_build/doctrees/nbsphinx/Notebooks/11_Looping_Through_Species.ipynb
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)     4426 2024-01-28 20:38:15.000000 mobspy-2.3.5/docs/_build/doctrees/nbsphinx/Notebooks/12_Born_Species.ipynb
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)    80668 2024-01-28 20:38:15.000000 mobspy-2.3.5/docs/_build/doctrees/nbsphinx/Notebooks/13_Events.ipynb
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)    48456 2024-01-28 20:38:15.000000 mobspy-2.3.5/docs/_build/doctrees/nbsphinx/Notebooks/14_Concatenating_Simulations.ipynb
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)    25979 2024-01-28 20:38:15.000000 mobspy-2.3.5/docs/_build/doctrees/nbsphinx/Notebooks_01_Basic_Intro_13_1.png
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)    10466 2024-01-28 20:38:15.000000 mobspy-2.3.5/docs/_build/doctrees/nbsphinx/Notebooks_01_Basic_Intro_18_0.png
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)    21874 2024-01-28 20:38:15.000000 mobspy-2.3.5/docs/_build/doctrees/nbsphinx/Notebooks_01_Basic_Intro_21_1.png
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)    17557 2024-01-28 20:38:15.000000 mobspy-2.3.5/docs/_build/doctrees/nbsphinx/Notebooks_01_Basic_Intro_3_1.png
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)     8683 2024-01-28 20:38:15.000000 mobspy-2.3.5/docs/_build/doctrees/nbsphinx/Notebooks_09_Result_Data_1_1.png
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)    30221 2024-01-28 20:38:15.000000 mobspy-2.3.5/docs/_build/doctrees/nbsphinx/Notebooks_09_Result_Data_3_0.png
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)    23598 2024-01-28 20:38:15.000000 mobspy-2.3.5/docs/_build/doctrees/nbsphinx/Notebooks_09_Result_Data_5_0.png
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)     9452 2024-01-28 20:38:15.000000 mobspy-2.3.5/docs/_build/doctrees/nbsphinx/Notebooks_09_Result_Data_9_1.png
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)    12468 2024-01-28 20:38:15.000000 mobspy-2.3.5/docs/_build/doctrees/nbsphinx/Notebooks_10_Reaction_Rates_11_1.png
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)    14066 2024-01-28 20:38:15.000000 mobspy-2.3.5/docs/_build/doctrees/nbsphinx/Notebooks_13_Events_11_2.png
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)    13308 2024-01-28 20:38:15.000000 mobspy-2.3.5/docs/_build/doctrees/nbsphinx/Notebooks_13_Events_1_2.png
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)    15379 2024-01-28 20:38:15.000000 mobspy-2.3.5/docs/_build/doctrees/nbsphinx/Notebooks_13_Events_4_3.png
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)     9027 2024-01-28 20:38:15.000000 mobspy-2.3.5/docs/_build/doctrees/nbsphinx/Notebooks_13_Events_8_1.png
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)    11337 2024-01-28 20:38:15.000000 mobspy-2.3.5/docs/_build/doctrees/nbsphinx/Notebooks_14_Concatenating_Simulations_1_1.png
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)    11111 2024-01-28 20:38:15.000000 mobspy-2.3.5/docs/_build/doctrees/nbsphinx/Notebooks_14_Concatenating_Simulations_3_1.png
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)    10008 2024-01-28 20:38:15.000000 mobspy-2.3.5/docs/_build/doctrees/nbsphinx/Notebooks_14_Concatenating_Simulations_5_1.png
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)     2407 2024-01-28 20:38:15.000000 mobspy-2.3.5/docs/_build/doctrees/setup.doctree
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)     2439 2024-01-28 20:38:15.000000 mobspy-2.3.5/docs/_build/doctrees/test_script.doctree
+drwxr-xr-x   0 fabriciocravo   (501) staff       (20)        0 2024-04-11 13:12:07.667021 mobspy-2.3.5/docs/_build/html/
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)      230 2024-01-28 20:38:15.000000 mobspy-2.3.5/docs/_build/html/.buildinfo
+drwxr-xr-x   0 fabriciocravo   (501) staff       (20)        0 2024-04-11 13:12:07.738802 mobspy-2.3.5/docs/_build/html/Notebooks/
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)    41132 2024-01-28 20:38:15.000000 mobspy-2.3.5/docs/_build/html/Notebooks/01_Basic_Intro.html
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)   127718 2024-01-28 20:38:15.000000 mobspy-2.3.5/docs/_build/html/Notebooks/01_Basic_Intro.ipynb
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)    16265 2024-01-28 20:38:15.000000 mobspy-2.3.5/docs/_build/html/Notebooks/02_Reaction_Inheritance.html
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)     6534 2024-01-28 20:38:15.000000 mobspy-2.3.5/docs/_build/html/Notebooks/02_Reaction_Inheritance.ipynb
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)    17425 2024-01-28 20:38:15.000000 mobspy-2.3.5/docs/_build/html/Notebooks/03_Characteristics.html
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)     8067 2024-01-28 20:38:15.000000 mobspy-2.3.5/docs/_build/html/Notebooks/03_Characteristics.ipynb
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)    10225 2024-01-28 20:38:15.000000 mobspy-2.3.5/docs/_build/html/Notebooks/04_Characteristic_restriction.html
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)     2210 2024-01-28 20:38:15.000000 mobspy-2.3.5/docs/_build/html/Notebooks/04_Characteristic_restriction.ipynb
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)    15743 2024-01-28 20:38:15.000000 mobspy-2.3.5/docs/_build/html/Notebooks/05_For_Loops.html
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)     5563 2024-01-28 20:38:15.000000 mobspy-2.3.5/docs/_build/html/Notebooks/05_For_Loops.ipynb
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)    14878 2024-01-28 20:38:15.000000 mobspy-2.3.5/docs/_build/html/Notebooks/06_Order_Matters.html
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)     6167 2024-01-28 20:38:15.000000 mobspy-2.3.5/docs/_build/html/Notebooks/06_Order_Matters.ipynb
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)    23518 2024-01-28 20:38:15.000000 mobspy-2.3.5/docs/_build/html/Notebooks/07_Initial_Condition.html
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)    12448 2024-01-28 20:38:15.000000 mobspy-2.3.5/docs/_build/html/Notebooks/07_Initial_Condition.ipynb
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)    15642 2024-01-28 20:38:15.000000 mobspy-2.3.5/docs/_build/html/Notebooks/08_Units.html
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)     5154 2024-01-28 20:38:15.000000 mobspy-2.3.5/docs/_build/html/Notebooks/08_Units.ipynb
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)    23686 2024-01-28 20:38:15.000000 mobspy-2.3.5/docs/_build/html/Notebooks/09_Result_Data.html
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)   106408 2024-01-28 20:38:15.000000 mobspy-2.3.5/docs/_build/html/Notebooks/09_Result_Data.ipynb
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)    23178 2024-01-28 20:38:15.000000 mobspy-2.3.5/docs/_build/html/Notebooks/10_Reaction_Rates.html
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)    25996 2024-01-28 20:38:15.000000 mobspy-2.3.5/docs/_build/html/Notebooks/10_Reaction_Rates.ipynb
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)    14337 2024-01-28 20:38:15.000000 mobspy-2.3.5/docs/_build/html/Notebooks/11_Looping_Through_Species.html
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)     3942 2024-01-28 20:38:15.000000 mobspy-2.3.5/docs/_build/html/Notebooks/11_Looping_Through_Species.ipynb
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)    14032 2024-01-28 20:38:15.000000 mobspy-2.3.5/docs/_build/html/Notebooks/12_Born_Species.html
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)     4426 2024-01-28 20:38:15.000000 mobspy-2.3.5/docs/_build/html/Notebooks/12_Born_Species.ipynb
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)    28370 2024-01-28 20:38:15.000000 mobspy-2.3.5/docs/_build/html/Notebooks/13_Events.html
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)    80668 2024-01-28 20:38:15.000000 mobspy-2.3.5/docs/_build/html/Notebooks/13_Events.ipynb
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)    18015 2024-01-28 20:38:15.000000 mobspy-2.3.5/docs/_build/html/Notebooks/14_Concatenating_Simulations.html
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)    48456 2024-01-28 20:38:15.000000 mobspy-2.3.5/docs/_build/html/Notebooks/14_Concatenating_Simulations.ipynb
+drwxr-xr-x   0 fabriciocravo   (501) staff       (20)        0 2024-04-11 13:12:07.741157 mobspy-2.3.5/docs/_build/html/_autosummary/
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)     7201 2024-01-28 20:38:15.000000 mobspy-2.3.5/docs/_build/html/_autosummary/mobspy.html
+drwxr-xr-x   0 fabriciocravo   (501) staff       (20)        0 2024-04-11 13:12:07.770201 mobspy-2.3.5/docs/_build/html/_images/
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)    25979 2024-01-28 20:38:15.000000 mobspy-2.3.5/docs/_build/html/_images/Notebooks_01_Basic_Intro_13_1.png
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)    10466 2024-01-28 20:38:15.000000 mobspy-2.3.5/docs/_build/html/_images/Notebooks_01_Basic_Intro_18_0.png
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)    21874 2024-01-28 20:38:15.000000 mobspy-2.3.5/docs/_build/html/_images/Notebooks_01_Basic_Intro_21_1.png
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)    17557 2024-01-28 20:38:15.000000 mobspy-2.3.5/docs/_build/html/_images/Notebooks_01_Basic_Intro_3_1.png
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)     8683 2024-01-28 20:38:15.000000 mobspy-2.3.5/docs/_build/html/_images/Notebooks_09_Result_Data_1_1.png
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)    30221 2024-01-28 20:38:15.000000 mobspy-2.3.5/docs/_build/html/_images/Notebooks_09_Result_Data_3_0.png
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)    23598 2024-01-28 20:38:15.000000 mobspy-2.3.5/docs/_build/html/_images/Notebooks_09_Result_Data_5_0.png
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)     9452 2024-01-28 20:38:15.000000 mobspy-2.3.5/docs/_build/html/_images/Notebooks_09_Result_Data_9_1.png
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)    12468 2024-01-28 20:38:15.000000 mobspy-2.3.5/docs/_build/html/_images/Notebooks_10_Reaction_Rates_11_1.png
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)    14066 2024-01-28 20:38:15.000000 mobspy-2.3.5/docs/_build/html/_images/Notebooks_13_Events_11_2.png
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)    13308 2024-01-28 20:38:15.000000 mobspy-2.3.5/docs/_build/html/_images/Notebooks_13_Events_1_2.png
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)    15379 2024-01-28 20:38:15.000000 mobspy-2.3.5/docs/_build/html/_images/Notebooks_13_Events_4_3.png
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)     9027 2024-01-28 20:38:15.000000 mobspy-2.3.5/docs/_build/html/_images/Notebooks_13_Events_8_1.png
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)    11337 2024-01-28 20:38:15.000000 mobspy-2.3.5/docs/_build/html/_images/Notebooks_14_Concatenating_Simulations_1_1.png
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)    11111 2024-01-28 20:38:15.000000 mobspy-2.3.5/docs/_build/html/_images/Notebooks_14_Concatenating_Simulations_3_1.png
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)    10008 2024-01-28 20:38:15.000000 mobspy-2.3.5/docs/_build/html/_images/Notebooks_14_Concatenating_Simulations_5_1.png
+drwxr-xr-x   0 fabriciocravo   (501) staff       (20)        0 2024-04-11 13:12:07.787827 mobspy-2.3.5/docs/_build/html/_sources/
+drwxr-xr-x   0 fabriciocravo   (501) staff       (20)        0 2024-04-11 13:12:07.812627 mobspy-2.3.5/docs/_build/html/_sources/Notebooks/
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)   127718 2024-01-28 20:38:15.000000 mobspy-2.3.5/docs/_build/html/_sources/Notebooks/01_Basic_Intro.ipynb.txt
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)     6534 2024-01-28 20:38:15.000000 mobspy-2.3.5/docs/_build/html/_sources/Notebooks/02_Reaction_Inheritance.ipynb.txt
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)     8067 2024-01-28 20:38:15.000000 mobspy-2.3.5/docs/_build/html/_sources/Notebooks/03_Characteristics.ipynb.txt
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)     2210 2024-01-28 20:38:15.000000 mobspy-2.3.5/docs/_build/html/_sources/Notebooks/04_Characteristic_restriction.ipynb.txt
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)     5563 2024-01-28 20:38:15.000000 mobspy-2.3.5/docs/_build/html/_sources/Notebooks/05_For_Loops.ipynb.txt
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)     6167 2024-01-28 20:38:15.000000 mobspy-2.3.5/docs/_build/html/_sources/Notebooks/06_Order_Matters.ipynb.txt
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)    12448 2024-01-28 20:38:15.000000 mobspy-2.3.5/docs/_build/html/_sources/Notebooks/07_Initial_Condition.ipynb.txt
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)     5154 2024-01-28 20:38:15.000000 mobspy-2.3.5/docs/_build/html/_sources/Notebooks/08_Units.ipynb.txt
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)   106408 2024-01-28 20:38:15.000000 mobspy-2.3.5/docs/_build/html/_sources/Notebooks/09_Result_Data.ipynb.txt
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)    25996 2024-01-28 20:38:15.000000 mobspy-2.3.5/docs/_build/html/_sources/Notebooks/10_Reaction_Rates.ipynb.txt
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)     3942 2024-01-28 20:38:15.000000 mobspy-2.3.5/docs/_build/html/_sources/Notebooks/11_Looping_Through_Species.ipynb.txt
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)     4426 2024-01-28 20:38:15.000000 mobspy-2.3.5/docs/_build/html/_sources/Notebooks/12_Born_Species.ipynb.txt
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)    80668 2024-01-28 20:38:15.000000 mobspy-2.3.5/docs/_build/html/_sources/Notebooks/13_Events.ipynb.txt
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)    48456 2024-01-28 20:38:15.000000 mobspy-2.3.5/docs/_build/html/_sources/Notebooks/14_Concatenating_Simulations.ipynb.txt
+drwxr-xr-x   0 fabriciocravo   (501) staff       (20)        0 2024-04-11 13:12:07.814677 mobspy-2.3.5/docs/_build/html/_sources/_autosummary/
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)       67 2024-01-28 20:38:15.000000 mobspy-2.3.5/docs/_build/html/_sources/_autosummary/mobspy.rst.txt
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)      123 2024-01-28 20:38:15.000000 mobspy-2.3.5/docs/_build/html/_sources/api.rst.txt
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)      131 2024-01-28 20:38:15.000000 mobspy-2.3.5/docs/_build/html/_sources/for_local_use.rst.txt
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)      839 2024-01-28 20:38:15.000000 mobspy-2.3.5/docs/_build/html/_sources/index.rst.txt
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)      626 2024-01-28 20:38:15.000000 mobspy-2.3.5/docs/_build/html/_sources/mobspy.data_handler.rst.txt
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)     3107 2024-01-28 20:38:15.000000 mobspy-2.3.5/docs/_build/html/_sources/mobspy.modules.rst.txt
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)      655 2024-01-28 20:38:15.000000 mobspy-2.3.5/docs/_build/html/_sources/mobspy.parameter_scripts.rst.txt
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)      571 2024-01-28 20:38:15.000000 mobspy-2.3.5/docs/_build/html/_sources/mobspy.parameters.rst.txt
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)      620 2024-01-28 20:38:15.000000 mobspy-2.3.5/docs/_build/html/_sources/mobspy.plot_params.rst.txt
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)     1029 2024-01-28 20:38:15.000000 mobspy-2.3.5/docs/_build/html/_sources/mobspy.plot_scripts.rst.txt
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)      549 2024-01-28 20:38:15.000000 mobspy-2.3.5/docs/_build/html/_sources/mobspy.rst.txt
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)      742 2024-01-28 20:38:15.000000 mobspy-2.3.5/docs/_build/html/_sources/mobspy.sbml_simulator.rst.txt
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)      427 2024-01-28 20:38:15.000000 mobspy-2.3.5/docs/_build/html/_sources/mobspy.simulation_logging.rst.txt
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)       96 2024-01-28 20:38:15.000000 mobspy-2.3.5/docs/_build/html/_sources/modules.rst.txt
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)      103 2024-01-28 20:38:15.000000 mobspy-2.3.5/docs/_build/html/_sources/setup.rst.txt
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)      123 2024-01-28 20:38:15.000000 mobspy-2.3.5/docs/_build/html/_sources/test_script.rst.txt
+drwxr-xr-x   0 fabriciocravo   (501) staff       (20)        0 2024-04-11 13:12:07.835543 mobspy-2.3.5/docs/_build/html/_static/
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)     4289 2024-01-28 20:38:15.000000 mobspy-2.3.5/docs/_build/html/_static/_sphinx_javascript_frameworks_compat.js
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)    15094 2024-01-28 20:38:15.000000 mobspy-2.3.5/docs/_build/html/_static/basic.css
+drwxr-xr-x   0 fabriciocravo   (501) staff       (20)        0 2024-04-11 13:12:07.838330 mobspy-2.3.5/docs/_build/html/_static/css/
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)     3229 2024-01-28 20:38:15.000000 mobspy-2.3.5/docs/_build/html/_static/css/badge_only.css
+drwxr-xr-x   0 fabriciocravo   (501) staff       (20)        0 2024-04-11 13:12:07.908631 mobspy-2.3.5/docs/_build/html/_static/css/fonts/
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)    87624 2024-01-28 20:38:15.000000 mobspy-2.3.5/docs/_build/html/_static/css/fonts/Roboto-Slab-Bold.woff
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)    67312 2024-01-28 20:38:15.000000 mobspy-2.3.5/docs/_build/html/_static/css/fonts/Roboto-Slab-Bold.woff2
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)    86288 2024-01-28 20:38:15.000000 mobspy-2.3.5/docs/_build/html/_static/css/fonts/Roboto-Slab-Regular.woff
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)    66444 2024-01-28 20:38:15.000000 mobspy-2.3.5/docs/_build/html/_static/css/fonts/Roboto-Slab-Regular.woff2
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)   165742 2024-01-28 20:38:15.000000 mobspy-2.3.5/docs/_build/html/_static/css/fonts/fontawesome-webfont.eot
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)   444379 2024-01-28 20:38:15.000000 mobspy-2.3.5/docs/_build/html/_static/css/fonts/fontawesome-webfont.svg
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)   165548 2024-01-28 20:38:15.000000 mobspy-2.3.5/docs/_build/html/_static/css/fonts/fontawesome-webfont.ttf
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)    98024 2024-01-28 20:38:15.000000 mobspy-2.3.5/docs/_build/html/_static/css/fonts/fontawesome-webfont.woff
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)    77160 2024-01-28 20:38:15.000000 mobspy-2.3.5/docs/_build/html/_static/css/fonts/fontawesome-webfont.woff2
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)   323344 2024-01-28 20:38:15.000000 mobspy-2.3.5/docs/_build/html/_static/css/fonts/lato-bold-italic.woff
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)   193308 2024-01-28 20:38:15.000000 mobspy-2.3.5/docs/_build/html/_static/css/fonts/lato-bold-italic.woff2
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)   309728 2024-01-28 20:38:15.000000 mobspy-2.3.5/docs/_build/html/_static/css/fonts/lato-bold.woff
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)   184912 2024-01-28 20:38:15.000000 mobspy-2.3.5/docs/_build/html/_static/css/fonts/lato-bold.woff2
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)   328412 2024-01-28 20:38:15.000000 mobspy-2.3.5/docs/_build/html/_static/css/fonts/lato-normal-italic.woff
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)   195704 2024-01-28 20:38:15.000000 mobspy-2.3.5/docs/_build/html/_static/css/fonts/lato-normal-italic.woff2
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)   309192 2024-01-28 20:38:15.000000 mobspy-2.3.5/docs/_build/html/_static/css/fonts/lato-normal.woff
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)   182708 2024-01-28 20:38:15.000000 mobspy-2.3.5/docs/_build/html/_static/css/fonts/lato-normal.woff2
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)   135314 2024-01-28 20:38:15.000000 mobspy-2.3.5/docs/_build/html/_static/css/theme.css
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)     4472 2024-01-28 20:38:15.000000 mobspy-2.3.5/docs/_build/html/_static/doctools.js
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)      326 2024-01-28 20:38:15.000000 mobspy-2.3.5/docs/_build/html/_static/documentation_options.js
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)      286 2024-01-28 20:38:15.000000 mobspy-2.3.5/docs/_build/html/_static/file.png
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)    89501 2024-01-28 20:38:15.000000 mobspy-2.3.5/docs/_build/html/_static/jquery.js
+drwxr-xr-x   0 fabriciocravo   (501) staff       (20)        0 2024-04-11 13:12:07.916797 mobspy-2.3.5/docs/_build/html/_static/js/
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)      934 2024-01-28 20:38:15.000000 mobspy-2.3.5/docs/_build/html/_static/js/badge_only.js
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)     4370 2024-01-28 20:38:15.000000 mobspy-2.3.5/docs/_build/html/_static/js/html5shiv-printshiv.min.js
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)     2734 2024-01-28 20:38:15.000000 mobspy-2.3.5/docs/_build/html/_static/js/html5shiv.min.js
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)     5023 2024-01-28 20:38:15.000000 mobspy-2.3.5/docs/_build/html/_static/js/theme.js
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)     4758 2024-01-28 20:38:15.000000 mobspy-2.3.5/docs/_build/html/_static/language_data.js
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)       90 2024-01-28 20:38:15.000000 mobspy-2.3.5/docs/_build/html/_static/minus.png
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)     4467 2024-01-28 20:38:15.000000 mobspy-2.3.5/docs/_build/html/_static/nbsphinx-broken-thumbnail.svg
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)     6861 2024-01-28 20:38:15.000000 mobspy-2.3.5/docs/_build/html/_static/nbsphinx-code-cells.css
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)      584 2024-01-28 20:38:15.000000 mobspy-2.3.5/docs/_build/html/_static/nbsphinx-gallery.css
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)     2871 2024-01-28 20:38:15.000000 mobspy-2.3.5/docs/_build/html/_static/nbsphinx-no-thumbnail.svg
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)       90 2024-01-28 20:38:15.000000 mobspy-2.3.5/docs/_build/html/_static/plus.png
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)     4902 2024-01-28 20:38:15.000000 mobspy-2.3.5/docs/_build/html/_static/pygments.css
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)    18732 2024-01-28 20:38:15.000000 mobspy-2.3.5/docs/_build/html/_static/searchtools.js
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)     5123 2024-01-28 20:38:15.000000 mobspy-2.3.5/docs/_build/html/_static/sphinx_highlight.js
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)     7627 2024-01-28 20:38:15.000000 mobspy-2.3.5/docs/_build/html/api.html
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)     6551 2024-01-28 20:38:15.000000 mobspy-2.3.5/docs/_build/html/for_local_use.html
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)    67727 2024-01-28 20:38:15.000000 mobspy-2.3.5/docs/_build/html/genindex.html
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)    10018 2024-01-28 20:38:15.000000 mobspy-2.3.5/docs/_build/html/index.html
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)    14863 2024-01-28 20:38:15.000000 mobspy-2.3.5/docs/_build/html/mobspy.data_handler.html
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)    91437 2024-01-28 20:38:15.000000 mobspy-2.3.5/docs/_build/html/mobspy.html
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)   178543 2024-01-28 20:38:15.000000 mobspy-2.3.5/docs/_build/html/mobspy.modules.html
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)    11761 2024-01-28 20:38:15.000000 mobspy-2.3.5/docs/_build/html/mobspy.parameter_scripts.html
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)     8867 2024-01-28 20:38:15.000000 mobspy-2.3.5/docs/_build/html/mobspy.parameters.html
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)     8736 2024-01-28 20:38:15.000000 mobspy-2.3.5/docs/_build/html/mobspy.plot_params.html
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)    36208 2024-01-28 20:38:15.000000 mobspy-2.3.5/docs/_build/html/mobspy.plot_scripts.html
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)    16526 2024-01-28 20:38:15.000000 mobspy-2.3.5/docs/_build/html/mobspy.sbml_simulator.html
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)     9250 2024-01-28 20:38:15.000000 mobspy-2.3.5/docs/_build/html/mobspy.simulation_logging.html
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)    23199 2024-01-28 20:38:15.000000 mobspy-2.3.5/docs/_build/html/modules.html
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)     8450 2024-01-28 20:38:15.000000 mobspy-2.3.5/docs/_build/html/objects.inv
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)    17062 2024-01-28 20:38:15.000000 mobspy-2.3.5/docs/_build/html/py-modindex.html
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)     6595 2024-01-28 20:38:15.000000 mobspy-2.3.5/docs/_build/html/search.html
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)    96699 2024-01-28 20:38:15.000000 mobspy-2.3.5/docs/_build/html/searchindex.js
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)     6464 2024-01-28 20:38:15.000000 mobspy-2.3.5/docs/_build/html/setup.html
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)     6500 2024-01-28 20:38:15.000000 mobspy-2.3.5/docs/_build/html/test_script.html
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)      123 2024-01-28 20:38:15.000000 mobspy-2.3.5/docs/api.rst
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)     1220 2024-01-28 20:38:15.000000 mobspy-2.3.5/docs/conf.py
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)      131 2024-01-28 20:38:15.000000 mobspy-2.3.5/docs/for_local_use.rst
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)      839 2024-01-28 20:38:15.000000 mobspy-2.3.5/docs/index.rst
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)      800 2024-01-28 20:38:15.000000 mobspy-2.3.5/docs/make.bat
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)      626 2024-01-28 20:38:15.000000 mobspy-2.3.5/docs/mobspy.data_handler.rst
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)     3107 2024-01-28 20:38:15.000000 mobspy-2.3.5/docs/mobspy.modules.rst
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)      655 2024-01-28 20:38:15.000000 mobspy-2.3.5/docs/mobspy.parameter_scripts.rst
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)      571 2024-01-28 20:38:15.000000 mobspy-2.3.5/docs/mobspy.parameters.rst
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)      620 2024-01-28 20:38:15.000000 mobspy-2.3.5/docs/mobspy.plot_params.rst
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)     1029 2024-01-28 20:38:15.000000 mobspy-2.3.5/docs/mobspy.plot_scripts.rst
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)      549 2024-01-28 20:38:15.000000 mobspy-2.3.5/docs/mobspy.rst
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)      742 2024-01-28 20:38:15.000000 mobspy-2.3.5/docs/mobspy.sbml_simulator.rst
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)      427 2024-01-28 20:38:15.000000 mobspy-2.3.5/docs/mobspy.simulation_logging.rst
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)       96 2024-01-28 20:38:15.000000 mobspy-2.3.5/docs/modules.rst
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)      103 2024-01-28 20:38:15.000000 mobspy-2.3.5/docs/setup.rst
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)      123 2024-01-28 20:38:15.000000 mobspy-2.3.5/docs/test_script.rst
+drwxr-xr-x   0 fabriciocravo   (501) staff       (20)        0 2024-04-11 13:12:07.399217 mobspy-2.3.5/example_models/
+drwxr-xr-x   0 fabriciocravo   (501) staff       (20)        0 2024-04-11 13:12:07.938299 mobspy-2.3.5/example_models/Tutorial Notebooks/
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)   101374 2024-02-28 22:33:14.000000 mobspy-2.3.5/example_models/Tutorial Notebooks/01_Basic_Intro.ipynb
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)     6432 2023-11-22 11:36:42.000000 mobspy-2.3.5/example_models/Tutorial Notebooks/02_Reaction_Inheritance.ipynb
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)     7971 2023-11-22 11:38:40.000000 mobspy-2.3.5/example_models/Tutorial Notebooks/03_Characteristics.ipynb
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)     2210 2023-04-10 17:13:33.000000 mobspy-2.3.5/example_models/Tutorial Notebooks/04_Characteristic_restriction.ipynb
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)     5458 2023-11-22 12:06:45.000000 mobspy-2.3.5/example_models/Tutorial Notebooks/05_For_Loops.ipynb
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)     6167 2023-04-10 19:38:34.000000 mobspy-2.3.5/example_models/Tutorial Notebooks/06_Order_Matters.ipynb
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)     9479 2023-11-22 12:08:40.000000 mobspy-2.3.5/example_models/Tutorial Notebooks/07_Initial_Condition.ipynb
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)     5154 2023-04-19 15:35:09.000000 mobspy-2.3.5/example_models/Tutorial Notebooks/08_Units.ipynb
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)     7347 2023-11-22 22:08:58.000000 mobspy-2.3.5/example_models/Tutorial Notebooks/09_Result_Data.ipynb
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)    26061 2023-11-22 12:57:35.000000 mobspy-2.3.5/example_models/Tutorial Notebooks/10_Reaction_Rates.ipynb
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)     4029 2023-11-22 12:58:00.000000 mobspy-2.3.5/example_models/Tutorial Notebooks/11_Looping_Through_Species.ipynb
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)     4498 2023-11-22 13:00:12.000000 mobspy-2.3.5/example_models/Tutorial Notebooks/12_Born_Species.ipynb
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)    49256 2023-11-22 13:00:32.000000 mobspy-2.3.5/example_models/Tutorial Notebooks/13_Events.ipynb
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)    48456 2023-04-21 15:54:19.000000 mobspy-2.3.5/example_models/Tutorial Notebooks/14_Concatenating_Simulations.ipynb
+drwxr-xr-x   0 fabriciocravo   (501) staff       (20)        0 2024-04-11 13:12:07.941480 mobspy-2.3.5/example_models/Tutorial Notebooks/images/
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)    12324 2023-04-19 14:32:18.000000 mobspy-2.3.5/example_models/Tutorial Notebooks/images/Matching_Meta.png
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)   141303 2023-04-09 17:03:35.000000 mobspy-2.3.5/example_models/Tutorial Notebooks/images/vectorial_space.png
+drwxr-xr-x   0 fabriciocravo   (501) staff       (20)        0 2024-04-11 13:12:07.956690 mobspy-2.3.5/example_models/application_models/
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)      572 2024-01-28 20:43:25.000000 mobspy-2.3.5/example_models/application_models/AB_2CD.py
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)     1448 2024-01-28 20:44:42.000000 mobspy-2.3.5/example_models/application_models/AND_gate.py
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)     2357 2024-01-28 20:43:25.000000 mobspy-2.3.5/example_models/application_models/CRISPR_Oscillator.py
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)     1421 2024-01-28 20:47:50.000000 mobspy-2.3.5/example_models/application_models/For_The_Trees.py
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)     1291 2024-01-28 20:48:26.000000 mobspy-2.3.5/example_models/application_models/NOR_gate.py
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)     1237 2024-01-28 20:47:24.000000 mobspy-2.3.5/example_models/application_models/donor_receptor.py
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)     1371 2024-01-28 20:48:41.000000 mobspy-2.3.5/example_models/application_models/oscillator.py
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)      994 2023-07-07 11:50:03.000000 mobspy-2.3.5/example_models/application_models/positive_phage_feedback_loop.py
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)     2917 2024-01-28 20:49:35.000000 mobspy-2.3.5/example_models/application_models/random_walk.py
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)      637 2023-07-05 11:46:34.000000 mobspy-2.3.5/example_models/application_models/simple_infection.py
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)      564 2024-01-28 20:50:18.000000 mobspy-2.3.5/example_models/application_models/simple_repressor.py
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)      828 2023-07-05 12:49:47.000000 mobspy-2.3.5/example_models/application_models/simple_rule_based_and_gate.py
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)      701 2024-04-09 18:34:07.000000 mobspy-2.3.5/for_local_use.py
+drwxr-xr-x   0 fabriciocravo   (501) staff       (20)        0 2024-04-11 13:12:07.958004 mobspy-2.3.5/images/
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)    18566 2023-06-15 12:59:57.000000 mobspy-2.3.5/images/img.png
+drwxr-xr-x   0 fabriciocravo   (501) staff       (20)        0 2024-04-11 13:12:07.961876 mobspy-2.3.5/mobspy/
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)       95 2023-06-15 12:59:57.000000 mobspy-2.3.5/mobspy/__init__.py
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)       22 2024-04-11 13:11:28.000000 mobspy-2.3.5/mobspy/_version.py
+drwxr-xr-x   0 fabriciocravo   (501) staff       (20)        0 2024-04-11 13:12:07.967218 mobspy-2.3.5/mobspy/data_handler/
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)        0 2023-06-15 12:59:57.000000 mobspy-2.3.5/mobspy/data_handler/__init__.py
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)     5329 2024-02-28 23:26:14.000000 mobspy-2.3.5/mobspy/data_handler/process_result_data.py
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)     8060 2024-02-22 02:35:14.000000 mobspy-2.3.5/mobspy/data_handler/time_series_object.py
+drwxr-xr-x   0 fabriciocravo   (501) staff       (20)        0 2024-04-11 13:12:08.003402 mobspy-2.3.5/mobspy/modules/
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)        0 2023-06-15 12:59:57.000000 mobspy-2.3.5/mobspy/modules/__init__.py
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)     6281 2024-03-20 17:33:27.000000 mobspy-2.3.5/mobspy/modules/assignments_implementation.py
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)     5146 2024-02-25 21:08:54.000000 mobspy-2.3.5/mobspy/modules/class_of_meta_specie_named_any.py
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)     1827 2024-02-25 21:10:55.000000 mobspy-2.3.5/mobspy/modules/context_related_scripts.py
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)     5110 2023-06-25 17:16:47.000000 mobspy-2.3.5/mobspy/modules/event_functions.py
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)    12554 2024-02-29 01:47:29.000000 mobspy-2.3.5/mobspy/modules/function_rate_code.py
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)    13014 2024-02-26 15:53:24.000000 mobspy-2.3.5/mobspy/modules/logic_operator_objects.py
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)    71462 2024-03-20 17:33:27.000000 mobspy-2.3.5/mobspy/modules/meta_class.py
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)     5240 2023-12-21 15:41:16.000000 mobspy-2.3.5/mobspy/modules/meta_class_utils.py
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)    36116 2024-03-19 17:20:49.000000 mobspy-2.3.5/mobspy/modules/mobspy_expressions.py
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)     5042 2024-02-26 16:20:28.000000 mobspy-2.3.5/mobspy/modules/mobspy_parameters.py
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)    15158 2023-06-15 12:59:57.000000 mobspy-2.3.5/mobspy/modules/order_operators.py
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)    17445 2024-02-29 01:46:20.000000 mobspy-2.3.5/mobspy/modules/reaction_construction_nb.py
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)    18457 2023-06-15 12:59:57.000000 mobspy-2.3.5/mobspy/modules/reaction_construction_nb_parallel.py
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)     4363 2024-02-25 00:46:32.000000 mobspy-2.3.5/mobspy/modules/set_counts_module.py
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)     4143 2023-08-03 14:16:13.000000 mobspy-2.3.5/mobspy/modules/species_string_generator.py
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)     7435 2023-12-14 12:58:51.000000 mobspy-2.3.5/mobspy/modules/unit_handler.py
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)      443 2024-02-26 16:20:28.000000 mobspy-2.3.5/mobspy/modules/user_functions.py
+drwxr-xr-x   0 fabriciocravo   (501) staff       (20)        0 2024-04-11 13:12:08.007526 mobspy-2.3.5/mobspy/parameter_estimation_data_loader/
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)        0 2024-02-28 22:21:33.000000 mobspy-2.3.5/mobspy/parameter_estimation_data_loader/__init__.py
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)      912 2024-01-31 10:55:41.000000 mobspy-2.3.5/mobspy/parameter_estimation_data_loader/data_loader.py
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)     7714 2024-04-09 18:34:07.000000 mobspy-2.3.5/mobspy/parameter_estimation_data_loader/parameter_estimation_scripts.py
+drwxr-xr-x   0 fabriciocravo   (501) staff       (20)        0 2024-04-11 13:12:08.013214 mobspy-2.3.5/mobspy/parameter_scripts/
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)        0 2023-06-15 12:59:57.000000 mobspy-2.3.5/mobspy/parameter_scripts/__init__.py
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)     8189 2024-03-08 01:01:48.000000 mobspy-2.3.5/mobspy/parameter_scripts/parameter_reader.py
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)     1957 2024-02-01 12:50:35.000000 mobspy-2.3.5/mobspy/parameter_scripts/parametric_sweeps.py
+drwxr-xr-x   0 fabriciocravo   (501) staff       (20)        0 2024-04-11 13:12:08.017506 mobspy-2.3.5/mobspy/parameters/
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)     1463 2023-06-15 12:59:57.000000 mobspy-2.3.5/mobspy/parameters/README.md
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)        0 2023-06-15 12:59:57.000000 mobspy-2.3.5/mobspy/parameters/__init__.py
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)     1188 2024-01-30 18:15:37.000000 mobspy-2.3.5/mobspy/parameters/default_reader.py
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)     1285 2024-01-30 17:59:16.000000 mobspy-2.3.5/mobspy/parameters/example_reader.py
+drwxr-xr-x   0 fabriciocravo   (501) staff       (20)        0 2024-04-11 13:12:08.019789 mobspy-2.3.5/mobspy/patch_scripts/
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)        0 2024-04-09 18:34:07.000000 mobspy-2.3.5/mobspy/patch_scripts/__init__.py
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)    71177 2024-04-11 13:10:09.000000 mobspy-2.3.5/mobspy/patch_scripts/basico_task_parametrization.py
+drwxr-xr-x   0 fabriciocravo   (501) staff       (20)        0 2024-04-11 13:12:08.026275 mobspy-2.3.5/mobspy/plot_params/
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)        0 2023-06-15 12:59:57.000000 mobspy-2.3.5/mobspy/plot_params/__init__.py
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)      184 2023-06-15 12:59:57.000000 mobspy-2.3.5/mobspy/plot_params/default_plot_reader.py
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)     1573 2024-03-29 08:28:41.000000 mobspy-2.3.5/mobspy/plot_params/example_plot_reader.py
+drwxr-xr-x   0 fabriciocravo   (501) staff       (20)        0 2024-04-11 13:12:08.034688 mobspy-2.3.5/mobspy/plot_scripts/
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)        0 2024-03-28 14:29:54.000000 mobspy-2.3.5/mobspy/plot_scripts/__init__.py
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)     9268 2024-03-29 08:13:46.000000 mobspy-2.3.5/mobspy/plot_scripts/default_plots.py
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)    16874 2024-03-29 08:23:04.000000 mobspy-2.3.5/mobspy/plot_scripts/hierarchical_plot.py
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)     2482 2024-03-28 14:29:54.000000 mobspy-2.3.5/mobspy/plot_scripts/process_plot_data.py
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)     3885 2024-03-28 14:34:48.000000 mobspy-2.3.5/mobspy/plot_scripts/statistics_calculations.py
+drwxr-xr-x   0 fabriciocravo   (501) staff       (20)        0 2024-04-11 13:12:08.038848 mobspy-2.3.5/mobspy/sbml_simulator/
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)     8702 2024-03-20 17:46:34.000000 mobspy-2.3.5/mobspy/sbml_simulator/SBMLWriter.py
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)        0 2023-06-15 12:59:57.000000 mobspy-2.3.5/mobspy/sbml_simulator/__init__.py
+drwxr-xr-x   0 fabriciocravo   (501) staff       (20)        0 2024-04-11 13:12:08.045448 mobspy-2.3.5/mobspy/sbml_simulator/__pycache__/
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)     5705 2024-04-09 18:33:16.000000 mobspy-2.3.5/mobspy/sbml_simulator/__pycache__/SBMLWriter.cpython-310.pyc
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)      146 2024-04-09 18:33:16.000000 mobspy-2.3.5/mobspy/sbml_simulator/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)     1040 2024-04-09 18:33:16.000000 mobspy-2.3.5/mobspy/sbml_simulator/__pycache__/builder.cpython-310.pyc
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)     8808 2024-04-09 18:33:16.000000 mobspy-2.3.5/mobspy/sbml_simulator/__pycache__/run.cpython-310.pyc
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)     1029 2024-03-20 17:44:19.000000 mobspy-2.3.5/mobspy/sbml_simulator/builder.py
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)    11972 2024-03-20 17:43:06.000000 mobspy-2.3.5/mobspy/sbml_simulator/run.py
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)    39340 2024-03-29 08:12:30.000000 mobspy-2.3.5/mobspy/simulation.py
+drwxr-xr-x   0 fabriciocravo   (501) staff       (20)        0 2024-04-11 13:12:08.047504 mobspy-2.3.5/mobspy/simulation_logging/
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)        0 2023-06-15 12:59:57.000000 mobspy-2.3.5/mobspy/simulation_logging/__init__.py
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)      986 2024-01-28 20:25:20.000000 mobspy-2.3.5/mobspy/simulation_logging/log_scripts.py
+drwxr-xr-x   0 fabriciocravo   (501) staff       (20)        0 2024-04-11 13:12:07.964919 mobspy-2.3.5/mobspy.egg-info/
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)     7577 2024-04-11 13:12:06.000000 mobspy-2.3.5/mobspy.egg-info/PKG-INFO
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)    16540 2024-04-11 13:12:07.000000 mobspy-2.3.5/mobspy.egg-info/SOURCES.txt
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)        1 2024-04-11 13:12:06.000000 mobspy-2.3.5/mobspy.egg-info/dependency_links.txt
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)       76 2024-04-11 13:12:06.000000 mobspy-2.3.5/mobspy.egg-info/requires.txt
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)        7 2024-04-11 13:12:06.000000 mobspy-2.3.5/mobspy.egg-info/top_level.txt
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)       77 2023-06-15 12:59:57.000000 mobspy-2.3.5/requirements.txt
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)       38 2024-04-11 13:12:08.131441 mobspy-2.3.5/setup.cfg
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)      767 2023-06-15 12:59:57.000000 mobspy-2.3.5/setup.py
+drwxr-xr-x   0 fabriciocravo   (501) staff       (20)        0 2024-04-11 13:12:08.055565 mobspy-2.3.5/test_plot_images/
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)    11307 2024-04-09 18:24:31.000000 mobspy-2.3.5/test_plot_images/constant_tree.png
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)    47838 2024-04-09 18:34:07.000000 mobspy-2.3.5/test_plot_images/deterministic_tree.png
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)    57791 2024-04-09 18:34:07.000000 mobspy-2.3.5/test_plot_images/stochastic_tree.png
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)    39648 2024-03-08 01:16:27.000000 mobspy-2.3.5/test_script.py
+drwxr-xr-x   0 fabriciocravo   (501) staff       (20)        0 2024-04-11 13:12:08.129655 mobspy-2.3.5/test_tools/
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)      170 2023-06-15 12:59:57.000000 mobspy-2.3.5/test_tools/model_1.txt
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)      241 2023-06-26 11:54:08.000000 mobspy-2.3.5/test_tools/model_10.txt
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)      299 2023-06-15 12:59:57.000000 mobspy-2.3.5/test_tools/model_11.txt
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)      393 2023-06-15 12:59:57.000000 mobspy-2.3.5/test_tools/model_12.txt
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)      490 2023-06-15 12:59:57.000000 mobspy-2.3.5/test_tools/model_13.txt
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)      487 2023-06-15 12:59:57.000000 mobspy-2.3.5/test_tools/model_14.txt
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)      550 2023-06-15 12:59:57.000000 mobspy-2.3.5/test_tools/model_15.txt
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)      286 2023-06-15 12:59:57.000000 mobspy-2.3.5/test_tools/model_16.txt
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)      273 2023-06-15 12:59:57.000000 mobspy-2.3.5/test_tools/model_17.txt
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)      118 2023-06-15 12:59:57.000000 mobspy-2.3.5/test_tools/model_18.txt
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)      970 2023-06-15 12:59:57.000000 mobspy-2.3.5/test_tools/model_19.txt
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)      396 2023-06-15 12:59:57.000000 mobspy-2.3.5/test_tools/model_2.txt
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)      326 2023-06-15 12:59:57.000000 mobspy-2.3.5/test_tools/model_20.txt
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)     1453 2023-06-15 12:59:57.000000 mobspy-2.3.5/test_tools/model_21.txt
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)      471 2023-07-03 11:25:39.000000 mobspy-2.3.5/test_tools/model_22.txt
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)      186 2023-06-15 12:59:57.000000 mobspy-2.3.5/test_tools/model_23.txt
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)      605 2023-06-15 12:59:57.000000 mobspy-2.3.5/test_tools/model_24.txt
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)       81 2023-06-15 12:59:57.000000 mobspy-2.3.5/test_tools/model_25.txt
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)      518 2023-07-03 11:30:10.000000 mobspy-2.3.5/test_tools/model_26.txt
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)      145 2023-06-15 12:59:57.000000 mobspy-2.3.5/test_tools/model_27.txt
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)      400 2023-06-15 12:59:57.000000 mobspy-2.3.5/test_tools/model_28.txt
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)      395 2023-06-15 12:59:57.000000 mobspy-2.3.5/test_tools/model_29.txt
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)     3154 2023-06-15 12:59:57.000000 mobspy-2.3.5/test_tools/model_3.txt
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)      468 2023-06-15 12:59:57.000000 mobspy-2.3.5/test_tools/model_30.txt
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)    55662 2023-06-15 12:59:57.000000 mobspy-2.3.5/test_tools/model_31.txt
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)      129 2023-06-15 12:59:57.000000 mobspy-2.3.5/test_tools/model_32.txt
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)      831 2023-07-03 15:00:26.000000 mobspy-2.3.5/test_tools/model_33.txt
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)      123 2023-07-03 23:04:22.000000 mobspy-2.3.5/test_tools/model_34.txt
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)       61 2023-07-30 20:48:11.000000 mobspy-2.3.5/test_tools/model_35.txt
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)      175 2023-08-01 18:04:20.000000 mobspy-2.3.5/test_tools/model_36.txt
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)      391 2023-08-03 14:43:06.000000 mobspy-2.3.5/test_tools/model_37.txt
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)     1427 2023-08-19 22:03:11.000000 mobspy-2.3.5/test_tools/model_38.txt
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)     2853 2023-08-19 22:23:06.000000 mobspy-2.3.5/test_tools/model_39.txt
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)      727 2023-06-15 12:59:57.000000 mobspy-2.3.5/test_tools/model_4.txt
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)     2210 2023-11-15 12:57:45.000000 mobspy-2.3.5/test_tools/model_40.txt
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)     1412 2023-11-15 12:57:45.000000 mobspy-2.3.5/test_tools/model_41.txt
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)      178 2023-11-15 12:57:45.000000 mobspy-2.3.5/test_tools/model_42.txt
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)      419 2023-11-17 12:18:00.000000 mobspy-2.3.5/test_tools/model_43.txt
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)      197 2024-01-31 16:54:44.000000 mobspy-2.3.5/test_tools/model_44.txt
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)     8874 2024-02-22 02:44:14.000000 mobspy-2.3.5/test_tools/model_45.txt
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)      317 2024-02-24 00:21:58.000000 mobspy-2.3.5/test_tools/model_46.txt
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)      243 2024-02-24 13:50:27.000000 mobspy-2.3.5/test_tools/model_47.txt
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)      559 2023-06-15 12:59:57.000000 mobspy-2.3.5/test_tools/model_5.txt
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)      389 2023-07-03 10:56:19.000000 mobspy-2.3.5/test_tools/model_6.txt
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)     1362 2023-07-03 11:02:54.000000 mobspy-2.3.5/test_tools/model_7.txt
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)      433 2023-06-15 12:59:57.000000 mobspy-2.3.5/test_tools/model_8.txt
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)      736 2023-06-15 12:59:57.000000 mobspy-2.3.5/test_tools/model_9.txt
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)       60 2023-06-15 12:59:57.000000 mobspy-2.3.5/useful_parameters.json
```

### Comparing `mobspy-2.3.4/.github/workflows/python-app.yml` & `mobspy-2.3.5/.github/workflows/python-app.yml`

 * *Files identical despite different names*

### Comparing `mobspy-2.3.4/.readthedocs.yaml` & `mobspy-2.3.5/.readthedocs.yaml`

 * *Files identical despite different names*

### Comparing `mobspy-2.3.4/LICENSE` & `mobspy-2.3.5/LICENSE`

 * *Files identical despite different names*

### Comparing `mobspy-2.3.4/PKG-INFO` & `mobspy-2.3.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mobspy
-Version: 2.3.4
+Version: 2.3.5
 Summary: A Query-Based Language for Chemical Reaction Networks
 Home-page: https://github.com/ROBACON/mobspy
 License: UNKNOWN
 Description: ![Alt text](/images/img.png "MobsPy")
         
         # MobsPy
```

### Comparing `mobspy-2.3.4/README.md` & `mobspy-2.3.5/README.md`

 * *Files identical despite different names*

### Comparing `mobspy-2.3.4/docs/Makefile` & `mobspy-2.3.5/docs/Makefile`

 * *Files identical despite different names*

### Comparing `mobspy-2.3.4/docs/Notebooks/01_Basic_Intro.ipynb` & `mobspy-2.3.5/docs/Notebooks/01_Basic_Intro.ipynb`

 * *Files identical despite different names*

### Comparing `mobspy-2.3.4/docs/Notebooks/02_Reaction_Inheritance.ipynb` & `mobspy-2.3.5/docs/Notebooks/02_Reaction_Inheritance.ipynb`

 * *Files identical despite different names*

### Comparing `mobspy-2.3.4/docs/Notebooks/03_Characteristics.ipynb` & `mobspy-2.3.5/docs/Notebooks/03_Characteristics.ipynb`

 * *Files identical despite different names*

### Comparing `mobspy-2.3.4/docs/Notebooks/04_Characteristic_restriction.ipynb` & `mobspy-2.3.5/docs/Notebooks/04_Characteristic_restriction.ipynb`

 * *Files identical despite different names*

### Comparing `mobspy-2.3.4/docs/Notebooks/05_For_Loops.ipynb` & `mobspy-2.3.5/docs/Notebooks/05_For_Loops.ipynb`

 * *Files identical despite different names*

### Comparing `mobspy-2.3.4/docs/Notebooks/06_Order_Matters.ipynb` & `mobspy-2.3.5/docs/Notebooks/06_Order_Matters.ipynb`

 * *Files identical despite different names*

### Comparing `mobspy-2.3.4/docs/Notebooks/07_Initial_Condition.ipynb` & `mobspy-2.3.5/docs/Notebooks/07_Initial_Condition.ipynb`

 * *Files identical despite different names*

### Comparing `mobspy-2.3.4/docs/Notebooks/08_Units.ipynb` & `mobspy-2.3.5/docs/Notebooks/08_Units.ipynb`

 * *Files identical despite different names*

### Comparing `mobspy-2.3.4/docs/Notebooks/09_Result_Data.ipynb` & `mobspy-2.3.5/docs/Notebooks/09_Result_Data.ipynb`

 * *Files identical despite different names*

### Comparing `mobspy-2.3.4/docs/Notebooks/10_Reaction_Rates.ipynb` & `mobspy-2.3.5/docs/Notebooks/10_Reaction_Rates.ipynb`

 * *Files identical despite different names*

### Comparing `mobspy-2.3.4/docs/Notebooks/11_Looping_Through_Species.ipynb` & `mobspy-2.3.5/docs/Notebooks/11_Looping_Through_Species.ipynb`

 * *Files identical despite different names*

### Comparing `mobspy-2.3.4/docs/Notebooks/12_Born_Species.ipynb` & `mobspy-2.3.5/docs/Notebooks/12_Born_Species.ipynb`

 * *Files identical despite different names*

### Comparing `mobspy-2.3.4/docs/Notebooks/13_Events.ipynb` & `mobspy-2.3.5/docs/Notebooks/13_Events.ipynb`

 * *Files identical despite different names*

### Comparing `mobspy-2.3.4/docs/Notebooks/14_Concatenating_Simulations.ipynb` & `mobspy-2.3.5/docs/Notebooks/14_Concatenating_Simulations.ipynb`

 * *Files identical despite different names*

### Comparing `mobspy-2.3.4/docs/_build/doctrees/Notebooks/01_Basic_Intro.doctree` & `mobspy-2.3.5/docs/_build/doctrees/Notebooks/01_Basic_Intro.doctree`

 * *Files identical despite different names*

### Comparing `mobspy-2.3.4/docs/_build/doctrees/Notebooks/02_Reaction_Inheritance.doctree` & `mobspy-2.3.5/docs/_build/doctrees/Notebooks/02_Reaction_Inheritance.doctree`

 * *Files identical despite different names*

### Comparing `mobspy-2.3.4/docs/_build/doctrees/Notebooks/03_Characteristics.doctree` & `mobspy-2.3.5/docs/_build/doctrees/Notebooks/03_Characteristics.doctree`

 * *Files identical despite different names*

### Comparing `mobspy-2.3.4/docs/_build/doctrees/Notebooks/04_Characteristic_restriction.doctree` & `mobspy-2.3.5/docs/_build/doctrees/Notebooks/04_Characteristic_restriction.doctree`

 * *Files identical despite different names*

### Comparing `mobspy-2.3.4/docs/_build/doctrees/Notebooks/05_For_Loops.doctree` & `mobspy-2.3.5/docs/_build/doctrees/Notebooks/05_For_Loops.doctree`

 * *Files identical despite different names*

### Comparing `mobspy-2.3.4/docs/_build/doctrees/Notebooks/06_Order_Matters.doctree` & `mobspy-2.3.5/docs/_build/doctrees/Notebooks/06_Order_Matters.doctree`

 * *Files identical despite different names*

### Comparing `mobspy-2.3.4/docs/_build/doctrees/Notebooks/07_Initial_Condition.doctree` & `mobspy-2.3.5/docs/_build/doctrees/Notebooks/07_Initial_Condition.doctree`

 * *Files identical despite different names*

### Comparing `mobspy-2.3.4/docs/_build/doctrees/Notebooks/08_Units.doctree` & `mobspy-2.3.5/docs/_build/doctrees/Notebooks/08_Units.doctree`

 * *Files identical despite different names*

### Comparing `mobspy-2.3.4/docs/_build/doctrees/Notebooks/09_Result_Data.doctree` & `mobspy-2.3.5/docs/_build/doctrees/Notebooks/09_Result_Data.doctree`

 * *Files identical despite different names*

### Comparing `mobspy-2.3.4/docs/_build/doctrees/Notebooks/10_Reaction_Rates.doctree` & `mobspy-2.3.5/docs/_build/doctrees/Notebooks/10_Reaction_Rates.doctree`

 * *Files identical despite different names*

### Comparing `mobspy-2.3.4/docs/_build/doctrees/Notebooks/11_Looping_Through_Species.doctree` & `mobspy-2.3.5/docs/_build/doctrees/Notebooks/11_Looping_Through_Species.doctree`

 * *Files identical despite different names*

### Comparing `mobspy-2.3.4/docs/_build/doctrees/Notebooks/12_Born_Species.doctree` & `mobspy-2.3.5/docs/_build/doctrees/Notebooks/12_Born_Species.doctree`

 * *Files identical despite different names*

### Comparing `mobspy-2.3.4/docs/_build/doctrees/Notebooks/13_Events.doctree` & `mobspy-2.3.5/docs/_build/doctrees/Notebooks/13_Events.doctree`

 * *Files identical despite different names*

### Comparing `mobspy-2.3.4/docs/_build/doctrees/Notebooks/14_Concatenating_Simulations.doctree` & `mobspy-2.3.5/docs/_build/doctrees/Notebooks/14_Concatenating_Simulations.doctree`

 * *Files identical despite different names*

### Comparing `mobspy-2.3.4/docs/_build/doctrees/_autosummary/mobspy.doctree` & `mobspy-2.3.5/docs/_build/doctrees/_autosummary/mobspy.doctree`

 * *Files identical despite different names*

### Comparing `mobspy-2.3.4/docs/_build/doctrees/api.doctree` & `mobspy-2.3.5/docs/_build/doctrees/api.doctree`

 * *Files identical despite different names*

### Comparing `mobspy-2.3.4/docs/_build/doctrees/environment.pickle` & `mobspy-2.3.5/docs/_build/doctrees/environment.pickle`

 * *Files identical despite different names*

### Comparing `mobspy-2.3.4/docs/_build/doctrees/for_local_use.doctree` & `mobspy-2.3.5/docs/_build/doctrees/for_local_use.doctree`

 * *Files identical despite different names*

### Comparing `mobspy-2.3.4/docs/_build/doctrees/index.doctree` & `mobspy-2.3.5/docs/_build/doctrees/index.doctree`

 * *Files identical despite different names*

### Comparing `mobspy-2.3.4/docs/_build/doctrees/mobspy.data_handler.doctree` & `mobspy-2.3.5/docs/_build/doctrees/mobspy.data_handler.doctree`

 * *Files identical despite different names*

### Comparing `mobspy-2.3.4/docs/_build/doctrees/mobspy.doctree` & `mobspy-2.3.5/docs/_build/doctrees/mobspy.doctree`

 * *Files identical despite different names*

### Comparing `mobspy-2.3.4/docs/_build/doctrees/mobspy.modules.doctree` & `mobspy-2.3.5/docs/_build/doctrees/mobspy.modules.doctree`

 * *Files identical despite different names*

### Comparing `mobspy-2.3.4/docs/_build/doctrees/mobspy.parameter_scripts.doctree` & `mobspy-2.3.5/docs/_build/doctrees/mobspy.parameter_scripts.doctree`

 * *Files identical despite different names*

### Comparing `mobspy-2.3.4/docs/_build/doctrees/mobspy.parameters.doctree` & `mobspy-2.3.5/docs/_build/doctrees/mobspy.parameters.doctree`

 * *Files identical despite different names*

### Comparing `mobspy-2.3.4/docs/_build/doctrees/mobspy.plot_params.doctree` & `mobspy-2.3.5/docs/_build/doctrees/mobspy.plot_params.doctree`

 * *Files identical despite different names*

### Comparing `mobspy-2.3.4/docs/_build/doctrees/mobspy.plot_scripts.doctree` & `mobspy-2.3.5/docs/_build/doctrees/mobspy.plot_scripts.doctree`

 * *Files identical despite different names*

### Comparing `mobspy-2.3.4/docs/_build/doctrees/mobspy.sbml_simulator.doctree` & `mobspy-2.3.5/docs/_build/doctrees/mobspy.sbml_simulator.doctree`

 * *Files identical despite different names*

### Comparing `mobspy-2.3.4/docs/_build/doctrees/mobspy.simulation_logging.doctree` & `mobspy-2.3.5/docs/_build/doctrees/mobspy.simulation_logging.doctree`

 * *Files identical despite different names*

### Comparing `mobspy-2.3.4/docs/_build/doctrees/modules.doctree` & `mobspy-2.3.5/docs/_build/doctrees/modules.doctree`

 * *Files identical despite different names*

### Comparing `mobspy-2.3.4/docs/_build/doctrees/nbsphinx/Notebooks/01_Basic_Intro.ipynb` & `mobspy-2.3.5/docs/_build/doctrees/nbsphinx/Notebooks/01_Basic_Intro.ipynb`

 * *Files identical despite different names*

### Comparing `mobspy-2.3.4/docs/_build/doctrees/nbsphinx/Notebooks/02_Reaction_Inheritance.ipynb` & `mobspy-2.3.5/docs/_build/doctrees/nbsphinx/Notebooks/02_Reaction_Inheritance.ipynb`

 * *Files identical despite different names*

### Comparing `mobspy-2.3.4/docs/_build/doctrees/nbsphinx/Notebooks/03_Characteristics.ipynb` & `mobspy-2.3.5/docs/_build/doctrees/nbsphinx/Notebooks/03_Characteristics.ipynb`

 * *Files identical despite different names*

### Comparing `mobspy-2.3.4/docs/_build/doctrees/nbsphinx/Notebooks/04_Characteristic_restriction.ipynb` & `mobspy-2.3.5/docs/_build/doctrees/nbsphinx/Notebooks/04_Characteristic_restriction.ipynb`

 * *Files identical despite different names*

### Comparing `mobspy-2.3.4/docs/_build/doctrees/nbsphinx/Notebooks/05_For_Loops.ipynb` & `mobspy-2.3.5/docs/_build/doctrees/nbsphinx/Notebooks/05_For_Loops.ipynb`

 * *Files identical despite different names*

### Comparing `mobspy-2.3.4/docs/_build/doctrees/nbsphinx/Notebooks/06_Order_Matters.ipynb` & `mobspy-2.3.5/docs/_build/doctrees/nbsphinx/Notebooks/06_Order_Matters.ipynb`

 * *Files identical despite different names*

### Comparing `mobspy-2.3.4/docs/_build/doctrees/nbsphinx/Notebooks/07_Initial_Condition.ipynb` & `mobspy-2.3.5/docs/_build/doctrees/nbsphinx/Notebooks/07_Initial_Condition.ipynb`

 * *Files identical despite different names*

### Comparing `mobspy-2.3.4/docs/_build/doctrees/nbsphinx/Notebooks/08_Units.ipynb` & `mobspy-2.3.5/docs/_build/doctrees/nbsphinx/Notebooks/08_Units.ipynb`

 * *Files identical despite different names*

### Comparing `mobspy-2.3.4/docs/_build/doctrees/nbsphinx/Notebooks/09_Result_Data.ipynb` & `mobspy-2.3.5/docs/_build/doctrees/nbsphinx/Notebooks/09_Result_Data.ipynb`

 * *Files identical despite different names*

### Comparing `mobspy-2.3.4/docs/_build/doctrees/nbsphinx/Notebooks/10_Reaction_Rates.ipynb` & `mobspy-2.3.5/docs/_build/doctrees/nbsphinx/Notebooks/10_Reaction_Rates.ipynb`

 * *Files identical despite different names*

### Comparing `mobspy-2.3.4/docs/_build/doctrees/nbsphinx/Notebooks/11_Looping_Through_Species.ipynb` & `mobspy-2.3.5/docs/_build/doctrees/nbsphinx/Notebooks/11_Looping_Through_Species.ipynb`

 * *Files identical despite different names*

### Comparing `mobspy-2.3.4/docs/_build/doctrees/nbsphinx/Notebooks/12_Born_Species.ipynb` & `mobspy-2.3.5/docs/_build/doctrees/nbsphinx/Notebooks/12_Born_Species.ipynb`

 * *Files identical despite different names*

### Comparing `mobspy-2.3.4/docs/_build/doctrees/nbsphinx/Notebooks/13_Events.ipynb` & `mobspy-2.3.5/docs/_build/doctrees/nbsphinx/Notebooks/13_Events.ipynb`

 * *Files identical despite different names*

### Comparing `mobspy-2.3.4/docs/_build/doctrees/nbsphinx/Notebooks/14_Concatenating_Simulations.ipynb` & `mobspy-2.3.5/docs/_build/doctrees/nbsphinx/Notebooks/14_Concatenating_Simulations.ipynb`

 * *Files identical despite different names*

### Comparing `mobspy-2.3.4/docs/_build/doctrees/nbsphinx/Notebooks_01_Basic_Intro_13_1.png` & `mobspy-2.3.5/docs/_build/doctrees/nbsphinx/Notebooks_01_Basic_Intro_13_1.png`

 * *Files identical despite different names*

### Comparing `mobspy-2.3.4/docs/_build/doctrees/nbsphinx/Notebooks_01_Basic_Intro_18_0.png` & `mobspy-2.3.5/docs/_build/doctrees/nbsphinx/Notebooks_01_Basic_Intro_18_0.png`

 * *Files identical despite different names*

### Comparing `mobspy-2.3.4/docs/_build/doctrees/nbsphinx/Notebooks_01_Basic_Intro_21_1.png` & `mobspy-2.3.5/docs/_build/doctrees/nbsphinx/Notebooks_01_Basic_Intro_21_1.png`

 * *Files identical despite different names*

### Comparing `mobspy-2.3.4/docs/_build/doctrees/nbsphinx/Notebooks_01_Basic_Intro_3_1.png` & `mobspy-2.3.5/docs/_build/doctrees/nbsphinx/Notebooks_01_Basic_Intro_3_1.png`

 * *Files identical despite different names*

### Comparing `mobspy-2.3.4/docs/_build/doctrees/nbsphinx/Notebooks_09_Result_Data_1_1.png` & `mobspy-2.3.5/docs/_build/doctrees/nbsphinx/Notebooks_09_Result_Data_1_1.png`

 * *Files identical despite different names*

### Comparing `mobspy-2.3.4/docs/_build/doctrees/nbsphinx/Notebooks_09_Result_Data_3_0.png` & `mobspy-2.3.5/docs/_build/doctrees/nbsphinx/Notebooks_09_Result_Data_3_0.png`

 * *Files identical despite different names*

### Comparing `mobspy-2.3.4/docs/_build/doctrees/nbsphinx/Notebooks_09_Result_Data_5_0.png` & `mobspy-2.3.5/docs/_build/doctrees/nbsphinx/Notebooks_09_Result_Data_5_0.png`

 * *Files identical despite different names*

### Comparing `mobspy-2.3.4/docs/_build/doctrees/nbsphinx/Notebooks_09_Result_Data_9_1.png` & `mobspy-2.3.5/docs/_build/doctrees/nbsphinx/Notebooks_09_Result_Data_9_1.png`

 * *Files identical despite different names*

### Comparing `mobspy-2.3.4/docs/_build/doctrees/nbsphinx/Notebooks_10_Reaction_Rates_11_1.png` & `mobspy-2.3.5/docs/_build/doctrees/nbsphinx/Notebooks_10_Reaction_Rates_11_1.png`

 * *Files identical despite different names*

### Comparing `mobspy-2.3.4/docs/_build/doctrees/nbsphinx/Notebooks_13_Events_11_2.png` & `mobspy-2.3.5/docs/_build/doctrees/nbsphinx/Notebooks_13_Events_11_2.png`

 * *Files identical despite different names*

### Comparing `mobspy-2.3.4/docs/_build/doctrees/nbsphinx/Notebooks_13_Events_1_2.png` & `mobspy-2.3.5/docs/_build/doctrees/nbsphinx/Notebooks_13_Events_1_2.png`

 * *Files identical despite different names*

### Comparing `mobspy-2.3.4/docs/_build/doctrees/nbsphinx/Notebooks_13_Events_4_3.png` & `mobspy-2.3.5/docs/_build/doctrees/nbsphinx/Notebooks_13_Events_4_3.png`

 * *Files identical despite different names*

### Comparing `mobspy-2.3.4/docs/_build/doctrees/nbsphinx/Notebooks_13_Events_8_1.png` & `mobspy-2.3.5/docs/_build/doctrees/nbsphinx/Notebooks_13_Events_8_1.png`

 * *Files identical despite different names*

### Comparing `mobspy-2.3.4/docs/_build/doctrees/nbsphinx/Notebooks_14_Concatenating_Simulations_1_1.png` & `mobspy-2.3.5/docs/_build/doctrees/nbsphinx/Notebooks_14_Concatenating_Simulations_1_1.png`

 * *Files identical despite different names*

### Comparing `mobspy-2.3.4/docs/_build/doctrees/nbsphinx/Notebooks_14_Concatenating_Simulations_3_1.png` & `mobspy-2.3.5/docs/_build/doctrees/nbsphinx/Notebooks_14_Concatenating_Simulations_3_1.png`

 * *Files identical despite different names*

### Comparing `mobspy-2.3.4/docs/_build/doctrees/nbsphinx/Notebooks_14_Concatenating_Simulations_5_1.png` & `mobspy-2.3.5/docs/_build/doctrees/nbsphinx/Notebooks_14_Concatenating_Simulations_5_1.png`

 * *Files identical despite different names*

### Comparing `mobspy-2.3.4/docs/_build/doctrees/setup.doctree` & `mobspy-2.3.5/docs/_build/doctrees/setup.doctree`

 * *Files identical despite different names*

### Comparing `mobspy-2.3.4/docs/_build/doctrees/test_script.doctree` & `mobspy-2.3.5/docs/_build/doctrees/test_script.doctree`

 * *Files identical despite different names*

### Comparing `mobspy-2.3.4/docs/_build/html/Notebooks/01_Basic_Intro.html` & `mobspy-2.3.5/docs/_build/html/Notebooks/01_Basic_Intro.html`

 * *Files identical despite different names*

### Comparing `mobspy-2.3.4/docs/_build/html/Notebooks/01_Basic_Intro.ipynb` & `mobspy-2.3.5/docs/_build/html/Notebooks/01_Basic_Intro.ipynb`

 * *Files identical despite different names*

### Comparing `mobspy-2.3.4/docs/_build/html/Notebooks/02_Reaction_Inheritance.html` & `mobspy-2.3.5/docs/_build/html/Notebooks/02_Reaction_Inheritance.html`

 * *Files identical despite different names*

### Comparing `mobspy-2.3.4/docs/_build/html/Notebooks/02_Reaction_Inheritance.ipynb` & `mobspy-2.3.5/docs/_build/html/Notebooks/02_Reaction_Inheritance.ipynb`

 * *Files identical despite different names*

### Comparing `mobspy-2.3.4/docs/_build/html/Notebooks/03_Characteristics.html` & `mobspy-2.3.5/docs/_build/html/Notebooks/03_Characteristics.html`

 * *Files identical despite different names*

### Comparing `mobspy-2.3.4/docs/_build/html/Notebooks/03_Characteristics.ipynb` & `mobspy-2.3.5/docs/_build/html/Notebooks/03_Characteristics.ipynb`

 * *Files identical despite different names*

### Comparing `mobspy-2.3.4/docs/_build/html/Notebooks/04_Characteristic_restriction.html` & `mobspy-2.3.5/docs/_build/html/Notebooks/04_Characteristic_restriction.html`

 * *Files identical despite different names*

### Comparing `mobspy-2.3.4/docs/_build/html/Notebooks/04_Characteristic_restriction.ipynb` & `mobspy-2.3.5/docs/_build/html/Notebooks/04_Characteristic_restriction.ipynb`

 * *Files identical despite different names*

### Comparing `mobspy-2.3.4/docs/_build/html/Notebooks/05_For_Loops.html` & `mobspy-2.3.5/docs/_build/html/Notebooks/05_For_Loops.html`

 * *Files identical despite different names*

### Comparing `mobspy-2.3.4/docs/_build/html/Notebooks/05_For_Loops.ipynb` & `mobspy-2.3.5/docs/_build/html/Notebooks/05_For_Loops.ipynb`

 * *Files identical despite different names*

### Comparing `mobspy-2.3.4/docs/_build/html/Notebooks/06_Order_Matters.html` & `mobspy-2.3.5/docs/_build/html/Notebooks/06_Order_Matters.html`

 * *Files identical despite different names*

### Comparing `mobspy-2.3.4/docs/_build/html/Notebooks/06_Order_Matters.ipynb` & `mobspy-2.3.5/docs/_build/html/Notebooks/06_Order_Matters.ipynb`

 * *Files identical despite different names*

### Comparing `mobspy-2.3.4/docs/_build/html/Notebooks/07_Initial_Condition.html` & `mobspy-2.3.5/docs/_build/html/Notebooks/07_Initial_Condition.html`

 * *Files identical despite different names*

### Comparing `mobspy-2.3.4/docs/_build/html/Notebooks/07_Initial_Condition.ipynb` & `mobspy-2.3.5/docs/_build/html/Notebooks/07_Initial_Condition.ipynb`

 * *Files identical despite different names*

### Comparing `mobspy-2.3.4/docs/_build/html/Notebooks/08_Units.html` & `mobspy-2.3.5/docs/_build/html/Notebooks/08_Units.html`

 * *Files identical despite different names*

### Comparing `mobspy-2.3.4/docs/_build/html/Notebooks/08_Units.ipynb` & `mobspy-2.3.5/docs/_build/html/Notebooks/08_Units.ipynb`

 * *Files identical despite different names*

### Comparing `mobspy-2.3.4/docs/_build/html/Notebooks/09_Result_Data.html` & `mobspy-2.3.5/docs/_build/html/Notebooks/09_Result_Data.html`

 * *Files identical despite different names*

### Comparing `mobspy-2.3.4/docs/_build/html/Notebooks/09_Result_Data.ipynb` & `mobspy-2.3.5/docs/_build/html/Notebooks/09_Result_Data.ipynb`

 * *Files identical despite different names*

### Comparing `mobspy-2.3.4/docs/_build/html/Notebooks/10_Reaction_Rates.html` & `mobspy-2.3.5/docs/_build/html/Notebooks/10_Reaction_Rates.html`

 * *Files identical despite different names*

### Comparing `mobspy-2.3.4/docs/_build/html/Notebooks/10_Reaction_Rates.ipynb` & `mobspy-2.3.5/docs/_build/html/Notebooks/10_Reaction_Rates.ipynb`

 * *Files identical despite different names*

### Comparing `mobspy-2.3.4/docs/_build/html/Notebooks/11_Looping_Through_Species.html` & `mobspy-2.3.5/docs/_build/html/Notebooks/11_Looping_Through_Species.html`

 * *Files identical despite different names*

### Comparing `mobspy-2.3.4/docs/_build/html/Notebooks/11_Looping_Through_Species.ipynb` & `mobspy-2.3.5/docs/_build/html/Notebooks/11_Looping_Through_Species.ipynb`

 * *Files identical despite different names*

### Comparing `mobspy-2.3.4/docs/_build/html/Notebooks/12_Born_Species.html` & `mobspy-2.3.5/docs/_build/html/Notebooks/12_Born_Species.html`

 * *Files identical despite different names*

### Comparing `mobspy-2.3.4/docs/_build/html/Notebooks/12_Born_Species.ipynb` & `mobspy-2.3.5/docs/_build/html/Notebooks/12_Born_Species.ipynb`

 * *Files identical despite different names*

### Comparing `mobspy-2.3.4/docs/_build/html/Notebooks/13_Events.html` & `mobspy-2.3.5/docs/_build/html/Notebooks/13_Events.html`

 * *Files identical despite different names*

### Comparing `mobspy-2.3.4/docs/_build/html/Notebooks/13_Events.ipynb` & `mobspy-2.3.5/docs/_build/html/Notebooks/13_Events.ipynb`

 * *Files identical despite different names*

### Comparing `mobspy-2.3.4/docs/_build/html/Notebooks/14_Concatenating_Simulations.html` & `mobspy-2.3.5/docs/_build/html/Notebooks/14_Concatenating_Simulations.html`

 * *Files identical despite different names*

### Comparing `mobspy-2.3.4/docs/_build/html/Notebooks/14_Concatenating_Simulations.ipynb` & `mobspy-2.3.5/docs/_build/html/Notebooks/14_Concatenating_Simulations.ipynb`

 * *Files identical despite different names*

### Comparing `mobspy-2.3.4/docs/_build/html/_autosummary/mobspy.html` & `mobspy-2.3.5/docs/_build/html/_autosummary/mobspy.html`

 * *Files identical despite different names*

### Comparing `mobspy-2.3.4/docs/_build/html/_images/Notebooks_01_Basic_Intro_13_1.png` & `mobspy-2.3.5/docs/_build/html/_images/Notebooks_01_Basic_Intro_13_1.png`

 * *Files identical despite different names*

### Comparing `mobspy-2.3.4/docs/_build/html/_images/Notebooks_01_Basic_Intro_18_0.png` & `mobspy-2.3.5/docs/_build/html/_images/Notebooks_01_Basic_Intro_18_0.png`

 * *Files identical despite different names*

### Comparing `mobspy-2.3.4/docs/_build/html/_images/Notebooks_01_Basic_Intro_21_1.png` & `mobspy-2.3.5/docs/_build/html/_images/Notebooks_01_Basic_Intro_21_1.png`

 * *Files identical despite different names*

### Comparing `mobspy-2.3.4/docs/_build/html/_images/Notebooks_01_Basic_Intro_3_1.png` & `mobspy-2.3.5/docs/_build/html/_images/Notebooks_01_Basic_Intro_3_1.png`

 * *Files identical despite different names*

### Comparing `mobspy-2.3.4/docs/_build/html/_images/Notebooks_09_Result_Data_1_1.png` & `mobspy-2.3.5/docs/_build/html/_images/Notebooks_09_Result_Data_1_1.png`

 * *Files identical despite different names*

### Comparing `mobspy-2.3.4/docs/_build/html/_images/Notebooks_09_Result_Data_3_0.png` & `mobspy-2.3.5/docs/_build/html/_images/Notebooks_09_Result_Data_3_0.png`

 * *Files identical despite different names*

### Comparing `mobspy-2.3.4/docs/_build/html/_images/Notebooks_09_Result_Data_5_0.png` & `mobspy-2.3.5/docs/_build/html/_images/Notebooks_09_Result_Data_5_0.png`

 * *Files identical despite different names*

### Comparing `mobspy-2.3.4/docs/_build/html/_images/Notebooks_09_Result_Data_9_1.png` & `mobspy-2.3.5/docs/_build/html/_images/Notebooks_09_Result_Data_9_1.png`

 * *Files identical despite different names*

### Comparing `mobspy-2.3.4/docs/_build/html/_images/Notebooks_10_Reaction_Rates_11_1.png` & `mobspy-2.3.5/docs/_build/html/_images/Notebooks_10_Reaction_Rates_11_1.png`

 * *Files identical despite different names*

### Comparing `mobspy-2.3.4/docs/_build/html/_images/Notebooks_13_Events_11_2.png` & `mobspy-2.3.5/docs/_build/html/_images/Notebooks_13_Events_11_2.png`

 * *Files identical despite different names*

### Comparing `mobspy-2.3.4/docs/_build/html/_images/Notebooks_13_Events_1_2.png` & `mobspy-2.3.5/docs/_build/html/_images/Notebooks_13_Events_1_2.png`

 * *Files identical despite different names*

### Comparing `mobspy-2.3.4/docs/_build/html/_images/Notebooks_13_Events_4_3.png` & `mobspy-2.3.5/docs/_build/html/_images/Notebooks_13_Events_4_3.png`

 * *Files identical despite different names*

### Comparing `mobspy-2.3.4/docs/_build/html/_images/Notebooks_13_Events_8_1.png` & `mobspy-2.3.5/docs/_build/html/_images/Notebooks_13_Events_8_1.png`

 * *Files identical despite different names*

### Comparing `mobspy-2.3.4/docs/_build/html/_images/Notebooks_14_Concatenating_Simulations_1_1.png` & `mobspy-2.3.5/docs/_build/html/_images/Notebooks_14_Concatenating_Simulations_1_1.png`

 * *Files identical despite different names*

### Comparing `mobspy-2.3.4/docs/_build/html/_images/Notebooks_14_Concatenating_Simulations_3_1.png` & `mobspy-2.3.5/docs/_build/html/_images/Notebooks_14_Concatenating_Simulations_3_1.png`

 * *Files identical despite different names*

### Comparing `mobspy-2.3.4/docs/_build/html/_images/Notebooks_14_Concatenating_Simulations_5_1.png` & `mobspy-2.3.5/docs/_build/html/_images/Notebooks_14_Concatenating_Simulations_5_1.png`

 * *Files identical despite different names*

### Comparing `mobspy-2.3.4/docs/_build/html/_sources/Notebooks/01_Basic_Intro.ipynb.txt` & `mobspy-2.3.5/docs/_build/html/_sources/Notebooks/01_Basic_Intro.ipynb.txt`

 * *Files identical despite different names*

### Comparing `mobspy-2.3.4/docs/_build/html/_sources/Notebooks/02_Reaction_Inheritance.ipynb.txt` & `mobspy-2.3.5/docs/_build/html/_sources/Notebooks/02_Reaction_Inheritance.ipynb.txt`

 * *Files identical despite different names*

### Comparing `mobspy-2.3.4/docs/_build/html/_sources/Notebooks/03_Characteristics.ipynb.txt` & `mobspy-2.3.5/docs/_build/html/_sources/Notebooks/03_Characteristics.ipynb.txt`

 * *Files identical despite different names*

### Comparing `mobspy-2.3.4/docs/_build/html/_sources/Notebooks/04_Characteristic_restriction.ipynb.txt` & `mobspy-2.3.5/docs/_build/html/_sources/Notebooks/04_Characteristic_restriction.ipynb.txt`

 * *Files identical despite different names*

### Comparing `mobspy-2.3.4/docs/_build/html/_sources/Notebooks/05_For_Loops.ipynb.txt` & `mobspy-2.3.5/docs/_build/html/_sources/Notebooks/05_For_Loops.ipynb.txt`

 * *Files identical despite different names*

### Comparing `mobspy-2.3.4/docs/_build/html/_sources/Notebooks/06_Order_Matters.ipynb.txt` & `mobspy-2.3.5/docs/_build/html/_sources/Notebooks/06_Order_Matters.ipynb.txt`

 * *Files identical despite different names*

### Comparing `mobspy-2.3.4/docs/_build/html/_sources/Notebooks/07_Initial_Condition.ipynb.txt` & `mobspy-2.3.5/docs/_build/html/_sources/Notebooks/07_Initial_Condition.ipynb.txt`

 * *Files identical despite different names*

### Comparing `mobspy-2.3.4/docs/_build/html/_sources/Notebooks/08_Units.ipynb.txt` & `mobspy-2.3.5/docs/_build/html/_sources/Notebooks/08_Units.ipynb.txt`

 * *Files identical despite different names*

### Comparing `mobspy-2.3.4/docs/_build/html/_sources/Notebooks/09_Result_Data.ipynb.txt` & `mobspy-2.3.5/docs/_build/html/_sources/Notebooks/09_Result_Data.ipynb.txt`

 * *Files identical despite different names*

### Comparing `mobspy-2.3.4/docs/_build/html/_sources/Notebooks/10_Reaction_Rates.ipynb.txt` & `mobspy-2.3.5/docs/_build/html/_sources/Notebooks/10_Reaction_Rates.ipynb.txt`

 * *Files identical despite different names*

### Comparing `mobspy-2.3.4/docs/_build/html/_sources/Notebooks/11_Looping_Through_Species.ipynb.txt` & `mobspy-2.3.5/docs/_build/html/_sources/Notebooks/11_Looping_Through_Species.ipynb.txt`

 * *Files identical despite different names*

### Comparing `mobspy-2.3.4/docs/_build/html/_sources/Notebooks/12_Born_Species.ipynb.txt` & `mobspy-2.3.5/docs/_build/html/_sources/Notebooks/12_Born_Species.ipynb.txt`

 * *Files identical despite different names*

### Comparing `mobspy-2.3.4/docs/_build/html/_sources/Notebooks/13_Events.ipynb.txt` & `mobspy-2.3.5/docs/_build/html/_sources/Notebooks/13_Events.ipynb.txt`

 * *Files identical despite different names*

### Comparing `mobspy-2.3.4/docs/_build/html/_sources/Notebooks/14_Concatenating_Simulations.ipynb.txt` & `mobspy-2.3.5/docs/_build/html/_sources/Notebooks/14_Concatenating_Simulations.ipynb.txt`

 * *Files identical despite different names*

### Comparing `mobspy-2.3.4/docs/_build/html/_sources/index.rst.txt` & `mobspy-2.3.5/docs/_build/html/_sources/index.rst.txt`

 * *Files identical despite different names*

### Comparing `mobspy-2.3.4/docs/_build/html/_sources/mobspy.data_handler.rst.txt` & `mobspy-2.3.5/docs/_build/html/_sources/mobspy.data_handler.rst.txt`

 * *Files identical despite different names*

### Comparing `mobspy-2.3.4/docs/_build/html/_sources/mobspy.modules.rst.txt` & `mobspy-2.3.5/docs/_build/html/_sources/mobspy.modules.rst.txt`

 * *Files identical despite different names*

### Comparing `mobspy-2.3.4/docs/_build/html/_sources/mobspy.parameter_scripts.rst.txt` & `mobspy-2.3.5/docs/_build/html/_sources/mobspy.parameter_scripts.rst.txt`

 * *Files identical despite different names*

### Comparing `mobspy-2.3.4/docs/_build/html/_sources/mobspy.parameters.rst.txt` & `mobspy-2.3.5/docs/_build/html/_sources/mobspy.parameters.rst.txt`

 * *Files identical despite different names*

### Comparing `mobspy-2.3.4/docs/_build/html/_sources/mobspy.plot_params.rst.txt` & `mobspy-2.3.5/docs/_build/html/_sources/mobspy.plot_params.rst.txt`

 * *Files identical despite different names*

### Comparing `mobspy-2.3.4/docs/_build/html/_sources/mobspy.plot_scripts.rst.txt` & `mobspy-2.3.5/docs/_build/html/_sources/mobspy.plot_scripts.rst.txt`

 * *Files identical despite different names*

### Comparing `mobspy-2.3.4/docs/_build/html/_sources/mobspy.rst.txt` & `mobspy-2.3.5/docs/_build/html/_sources/mobspy.rst.txt`

 * *Files identical despite different names*

### Comparing `mobspy-2.3.4/docs/_build/html/_sources/mobspy.sbml_simulator.rst.txt` & `mobspy-2.3.5/docs/_build/html/_sources/mobspy.sbml_simulator.rst.txt`

 * *Files identical despite different names*

### Comparing `mobspy-2.3.4/docs/_build/html/_static/_sphinx_javascript_frameworks_compat.js` & `mobspy-2.3.5/docs/_build/html/_static/_sphinx_javascript_frameworks_compat.js`

 * *Files identical despite different names*

### Comparing `mobspy-2.3.4/docs/_build/html/_static/basic.css` & `mobspy-2.3.5/docs/_build/html/_static/basic.css`

 * *Files identical despite different names*

### Comparing `mobspy-2.3.4/docs/_build/html/_static/css/badge_only.css` & `mobspy-2.3.5/docs/_build/html/_static/css/badge_only.css`

 * *Files identical despite different names*

### Comparing `mobspy-2.3.4/docs/_build/html/_static/css/fonts/Roboto-Slab-Bold.woff` & `mobspy-2.3.5/docs/_build/html/_static/css/fonts/Roboto-Slab-Bold.woff`

 * *Files identical despite different names*

### Comparing `mobspy-2.3.4/docs/_build/html/_static/css/fonts/Roboto-Slab-Bold.woff2` & `mobspy-2.3.5/docs/_build/html/_static/css/fonts/Roboto-Slab-Bold.woff2`

 * *Files identical despite different names*

### Comparing `mobspy-2.3.4/docs/_build/html/_static/css/fonts/Roboto-Slab-Regular.woff` & `mobspy-2.3.5/docs/_build/html/_static/css/fonts/Roboto-Slab-Regular.woff`

 * *Files identical despite different names*

### Comparing `mobspy-2.3.4/docs/_build/html/_static/css/fonts/Roboto-Slab-Regular.woff2` & `mobspy-2.3.5/docs/_build/html/_static/css/fonts/Roboto-Slab-Regular.woff2`

 * *Files identical despite different names*

### Comparing `mobspy-2.3.4/docs/_build/html/_static/css/fonts/fontawesome-webfont.eot` & `mobspy-2.3.5/docs/_build/html/_static/css/fonts/fontawesome-webfont.eot`

 * *Files identical despite different names*

### Comparing `mobspy-2.3.4/docs/_build/html/_static/css/fonts/fontawesome-webfont.svg` & `mobspy-2.3.5/docs/_build/html/_static/css/fonts/fontawesome-webfont.svg`

 * *Files identical despite different names*

### Comparing `mobspy-2.3.4/docs/_build/html/_static/css/fonts/fontawesome-webfont.ttf` & `mobspy-2.3.5/docs/_build/html/_static/css/fonts/fontawesome-webfont.ttf`

 * *Files identical despite different names*

### Comparing `mobspy-2.3.4/docs/_build/html/_static/css/fonts/fontawesome-webfont.woff` & `mobspy-2.3.5/docs/_build/html/_static/css/fonts/fontawesome-webfont.woff`

 * *Files identical despite different names*

### Comparing `mobspy-2.3.4/docs/_build/html/_static/css/fonts/fontawesome-webfont.woff2` & `mobspy-2.3.5/docs/_build/html/_static/css/fonts/fontawesome-webfont.woff2`

 * *Files identical despite different names*

### Comparing `mobspy-2.3.4/docs/_build/html/_static/css/fonts/lato-bold-italic.woff` & `mobspy-2.3.5/docs/_build/html/_static/css/fonts/lato-bold-italic.woff`

 * *Files identical despite different names*

### Comparing `mobspy-2.3.4/docs/_build/html/_static/css/fonts/lato-bold-italic.woff2` & `mobspy-2.3.5/docs/_build/html/_static/css/fonts/lato-bold-italic.woff2`

 * *Files identical despite different names*

### Comparing `mobspy-2.3.4/docs/_build/html/_static/css/fonts/lato-bold.woff` & `mobspy-2.3.5/docs/_build/html/_static/css/fonts/lato-bold.woff`

 * *Files identical despite different names*

### Comparing `mobspy-2.3.4/docs/_build/html/_static/css/fonts/lato-bold.woff2` & `mobspy-2.3.5/docs/_build/html/_static/css/fonts/lato-bold.woff2`

 * *Files identical despite different names*

### Comparing `mobspy-2.3.4/docs/_build/html/_static/css/fonts/lato-normal-italic.woff` & `mobspy-2.3.5/docs/_build/html/_static/css/fonts/lato-normal-italic.woff`

 * *Files identical despite different names*

### Comparing `mobspy-2.3.4/docs/_build/html/_static/css/fonts/lato-normal-italic.woff2` & `mobspy-2.3.5/docs/_build/html/_static/css/fonts/lato-normal-italic.woff2`

 * *Files identical despite different names*

### Comparing `mobspy-2.3.4/docs/_build/html/_static/css/fonts/lato-normal.woff` & `mobspy-2.3.5/docs/_build/html/_static/css/fonts/lato-normal.woff`

 * *Files identical despite different names*

### Comparing `mobspy-2.3.4/docs/_build/html/_static/css/fonts/lato-normal.woff2` & `mobspy-2.3.5/docs/_build/html/_static/css/fonts/lato-normal.woff2`

 * *Files identical despite different names*

### Comparing `mobspy-2.3.4/docs/_build/html/_static/css/theme.css` & `mobspy-2.3.5/docs/_build/html/_static/css/theme.css`

 * *Files identical despite different names*

### Comparing `mobspy-2.3.4/docs/_build/html/_static/doctools.js` & `mobspy-2.3.5/docs/_build/html/_static/doctools.js`

 * *Files identical despite different names*

### Comparing `mobspy-2.3.4/docs/_build/html/_static/jquery.js` & `mobspy-2.3.5/docs/_build/html/_static/jquery.js`

 * *Files identical despite different names*

### Comparing `mobspy-2.3.4/docs/_build/html/_static/js/badge_only.js` & `mobspy-2.3.5/docs/_build/html/_static/js/badge_only.js`

 * *Files identical despite different names*

### Comparing `mobspy-2.3.4/docs/_build/html/_static/js/html5shiv-printshiv.min.js` & `mobspy-2.3.5/docs/_build/html/_static/js/html5shiv-printshiv.min.js`

 * *Files identical despite different names*

### Comparing `mobspy-2.3.4/docs/_build/html/_static/js/html5shiv.min.js` & `mobspy-2.3.5/docs/_build/html/_static/js/html5shiv.min.js`

 * *Files identical despite different names*

### Comparing `mobspy-2.3.4/docs/_build/html/_static/js/theme.js` & `mobspy-2.3.5/docs/_build/html/_static/js/theme.js`

 * *Files identical despite different names*

### Comparing `mobspy-2.3.4/docs/_build/html/_static/language_data.js` & `mobspy-2.3.5/docs/_build/html/_static/language_data.js`

 * *Files identical despite different names*

### Comparing `mobspy-2.3.4/docs/_build/html/_static/nbsphinx-broken-thumbnail.svg` & `mobspy-2.3.5/docs/_build/html/_static/nbsphinx-broken-thumbnail.svg`

 * *Files identical despite different names*

### Comparing `mobspy-2.3.4/docs/_build/html/_static/nbsphinx-code-cells.css` & `mobspy-2.3.5/docs/_build/html/_static/nbsphinx-code-cells.css`

 * *Files identical despite different names*

### Comparing `mobspy-2.3.4/docs/_build/html/_static/nbsphinx-gallery.css` & `mobspy-2.3.5/docs/_build/html/_static/nbsphinx-gallery.css`

 * *Files identical despite different names*

### Comparing `mobspy-2.3.4/docs/_build/html/_static/nbsphinx-no-thumbnail.svg` & `mobspy-2.3.5/docs/_build/html/_static/nbsphinx-no-thumbnail.svg`

 * *Files identical despite different names*

### Comparing `mobspy-2.3.4/docs/_build/html/_static/pygments.css` & `mobspy-2.3.5/docs/_build/html/_static/pygments.css`

 * *Files identical despite different names*

### Comparing `mobspy-2.3.4/docs/_build/html/_static/searchtools.js` & `mobspy-2.3.5/docs/_build/html/_static/searchtools.js`

 * *Files identical despite different names*

### Comparing `mobspy-2.3.4/docs/_build/html/_static/sphinx_highlight.js` & `mobspy-2.3.5/docs/_build/html/_static/sphinx_highlight.js`

 * *Files identical despite different names*

### Comparing `mobspy-2.3.4/docs/_build/html/api.html` & `mobspy-2.3.5/docs/_build/html/api.html`

 * *Files identical despite different names*

### Comparing `mobspy-2.3.4/docs/_build/html/for_local_use.html` & `mobspy-2.3.5/docs/_build/html/for_local_use.html`

 * *Files identical despite different names*

### Comparing `mobspy-2.3.4/docs/_build/html/genindex.html` & `mobspy-2.3.5/docs/_build/html/genindex.html`

 * *Files identical despite different names*

### Comparing `mobspy-2.3.4/docs/_build/html/index.html` & `mobspy-2.3.5/docs/_build/html/index.html`

 * *Files identical despite different names*

### Comparing `mobspy-2.3.4/docs/_build/html/mobspy.data_handler.html` & `mobspy-2.3.5/docs/_build/html/mobspy.data_handler.html`

 * *Files identical despite different names*

### Comparing `mobspy-2.3.4/docs/_build/html/mobspy.html` & `mobspy-2.3.5/docs/_build/html/mobspy.html`

 * *Files identical despite different names*

### Comparing `mobspy-2.3.4/docs/_build/html/mobspy.modules.html` & `mobspy-2.3.5/docs/_build/html/mobspy.modules.html`

 * *Files identical despite different names*

### Comparing `mobspy-2.3.4/docs/_build/html/mobspy.parameter_scripts.html` & `mobspy-2.3.5/docs/_build/html/mobspy.parameter_scripts.html`

 * *Files identical despite different names*

### Comparing `mobspy-2.3.4/docs/_build/html/mobspy.parameters.html` & `mobspy-2.3.5/docs/_build/html/mobspy.parameters.html`

 * *Files identical despite different names*

### Comparing `mobspy-2.3.4/docs/_build/html/mobspy.plot_params.html` & `mobspy-2.3.5/docs/_build/html/mobspy.plot_params.html`

 * *Files identical despite different names*

### Comparing `mobspy-2.3.4/docs/_build/html/mobspy.plot_scripts.html` & `mobspy-2.3.5/docs/_build/html/mobspy.plot_scripts.html`

 * *Files identical despite different names*

### Comparing `mobspy-2.3.4/docs/_build/html/mobspy.sbml_simulator.html` & `mobspy-2.3.5/docs/_build/html/mobspy.sbml_simulator.html`

 * *Files identical despite different names*

### Comparing `mobspy-2.3.4/docs/_build/html/mobspy.simulation_logging.html` & `mobspy-2.3.5/docs/_build/html/mobspy.simulation_logging.html`

 * *Files identical despite different names*

### Comparing `mobspy-2.3.4/docs/_build/html/modules.html` & `mobspy-2.3.5/docs/_build/html/modules.html`

 * *Files identical despite different names*

### Comparing `mobspy-2.3.4/docs/_build/html/objects.inv` & `mobspy-2.3.5/docs/_build/html/objects.inv`

 * *Files identical despite different names*

### Comparing `mobspy-2.3.4/docs/_build/html/py-modindex.html` & `mobspy-2.3.5/docs/_build/html/py-modindex.html`

 * *Files identical despite different names*

### Comparing `mobspy-2.3.4/docs/_build/html/search.html` & `mobspy-2.3.5/docs/_build/html/search.html`

 * *Files identical despite different names*

### Comparing `mobspy-2.3.4/docs/_build/html/searchindex.js` & `mobspy-2.3.5/docs/_build/html/searchindex.js`

 * *Files identical despite different names*

### Comparing `mobspy-2.3.4/docs/_build/html/setup.html` & `mobspy-2.3.5/docs/_build/html/setup.html`

 * *Files identical despite different names*

### Comparing `mobspy-2.3.4/docs/_build/html/test_script.html` & `mobspy-2.3.5/docs/_build/html/test_script.html`

 * *Files identical despite different names*

### Comparing `mobspy-2.3.4/docs/conf.py` & `mobspy-2.3.5/docs/conf.py`

 * *Files identical despite different names*

### Comparing `mobspy-2.3.4/docs/index.rst` & `mobspy-2.3.5/docs/index.rst`

 * *Files identical despite different names*

### Comparing `mobspy-2.3.4/docs/make.bat` & `mobspy-2.3.5/docs/make.bat`

 * *Files identical despite different names*

### Comparing `mobspy-2.3.4/docs/mobspy.data_handler.rst` & `mobspy-2.3.5/docs/mobspy.data_handler.rst`

 * *Files identical despite different names*

### Comparing `mobspy-2.3.4/docs/mobspy.modules.rst` & `mobspy-2.3.5/docs/mobspy.modules.rst`

 * *Files identical despite different names*

### Comparing `mobspy-2.3.4/docs/mobspy.parameter_scripts.rst` & `mobspy-2.3.5/docs/mobspy.parameter_scripts.rst`

 * *Files identical despite different names*

### Comparing `mobspy-2.3.4/docs/mobspy.parameters.rst` & `mobspy-2.3.5/docs/mobspy.parameters.rst`

 * *Files identical despite different names*

### Comparing `mobspy-2.3.4/docs/mobspy.plot_params.rst` & `mobspy-2.3.5/docs/mobspy.plot_params.rst`

 * *Files identical despite different names*

### Comparing `mobspy-2.3.4/docs/mobspy.plot_scripts.rst` & `mobspy-2.3.5/docs/mobspy.plot_scripts.rst`

 * *Files identical despite different names*

### Comparing `mobspy-2.3.4/docs/mobspy.rst` & `mobspy-2.3.5/docs/mobspy.rst`

 * *Files identical despite different names*

### Comparing `mobspy-2.3.4/docs/mobspy.sbml_simulator.rst` & `mobspy-2.3.5/docs/mobspy.sbml_simulator.rst`

 * *Files identical despite different names*

### Comparing `mobspy-2.3.4/example_models/Tutorial Notebooks/01_Basic_Intro.ipynb` & `mobspy-2.3.5/example_models/Tutorial Notebooks/01_Basic_Intro.ipynb`

 * *Files identical despite different names*

### Comparing `mobspy-2.3.4/example_models/Tutorial Notebooks/02_Reaction_Inheritance.ipynb` & `mobspy-2.3.5/example_models/Tutorial Notebooks/02_Reaction_Inheritance.ipynb`

 * *Files identical despite different names*

### Comparing `mobspy-2.3.4/example_models/Tutorial Notebooks/03_Characteristics.ipynb` & `mobspy-2.3.5/example_models/Tutorial Notebooks/03_Characteristics.ipynb`

 * *Files identical despite different names*

### Comparing `mobspy-2.3.4/example_models/Tutorial Notebooks/04_Characteristic_restriction.ipynb` & `mobspy-2.3.5/example_models/Tutorial Notebooks/04_Characteristic_restriction.ipynb`

 * *Files identical despite different names*

### Comparing `mobspy-2.3.4/example_models/Tutorial Notebooks/05_For_Loops.ipynb` & `mobspy-2.3.5/example_models/Tutorial Notebooks/05_For_Loops.ipynb`

 * *Files identical despite different names*

### Comparing `mobspy-2.3.4/example_models/Tutorial Notebooks/06_Order_Matters.ipynb` & `mobspy-2.3.5/example_models/Tutorial Notebooks/06_Order_Matters.ipynb`

 * *Files identical despite different names*

### Comparing `mobspy-2.3.4/example_models/Tutorial Notebooks/07_Initial_Condition.ipynb` & `mobspy-2.3.5/example_models/Tutorial Notebooks/07_Initial_Condition.ipynb`

 * *Files identical despite different names*

### Comparing `mobspy-2.3.4/example_models/Tutorial Notebooks/08_Units.ipynb` & `mobspy-2.3.5/example_models/Tutorial Notebooks/08_Units.ipynb`

 * *Files identical despite different names*

### Comparing `mobspy-2.3.4/example_models/Tutorial Notebooks/09_Result_Data.ipynb` & `mobspy-2.3.5/example_models/Tutorial Notebooks/09_Result_Data.ipynb`

 * *Files identical despite different names*

### Comparing `mobspy-2.3.4/example_models/Tutorial Notebooks/10_Reaction_Rates.ipynb` & `mobspy-2.3.5/example_models/Tutorial Notebooks/10_Reaction_Rates.ipynb`

 * *Files identical despite different names*

### Comparing `mobspy-2.3.4/example_models/Tutorial Notebooks/11_Looping_Through_Species.ipynb` & `mobspy-2.3.5/example_models/Tutorial Notebooks/11_Looping_Through_Species.ipynb`

 * *Files identical despite different names*

### Comparing `mobspy-2.3.4/example_models/Tutorial Notebooks/12_Born_Species.ipynb` & `mobspy-2.3.5/example_models/Tutorial Notebooks/12_Born_Species.ipynb`

 * *Files identical despite different names*

### Comparing `mobspy-2.3.4/example_models/Tutorial Notebooks/13_Events.ipynb` & `mobspy-2.3.5/example_models/Tutorial Notebooks/13_Events.ipynb`

 * *Files identical despite different names*

### Comparing `mobspy-2.3.4/example_models/Tutorial Notebooks/14_Concatenating_Simulations.ipynb` & `mobspy-2.3.5/example_models/Tutorial Notebooks/14_Concatenating_Simulations.ipynb`

 * *Files identical despite different names*

### Comparing `mobspy-2.3.4/example_models/Tutorial Notebooks/images/Matching_Meta.png` & `mobspy-2.3.5/example_models/Tutorial Notebooks/images/Matching_Meta.png`

 * *Files identical despite different names*

### Comparing `mobspy-2.3.4/example_models/Tutorial Notebooks/images/vectorial_space.png` & `mobspy-2.3.5/example_models/Tutorial Notebooks/images/vectorial_space.png`

 * *Files identical despite different names*

### Comparing `mobspy-2.3.4/example_models/application_models/AB_2CD.py` & `mobspy-2.3.5/example_models/application_models/AB_2CD.py`

 * *Files identical despite different names*

### Comparing `mobspy-2.3.4/example_models/application_models/AND_gate.py` & `mobspy-2.3.5/example_models/application_models/AND_gate.py`

 * *Files identical despite different names*

### Comparing `mobspy-2.3.4/example_models/application_models/CRISPR_Oscillator.py` & `mobspy-2.3.5/example_models/application_models/CRISPR_Oscillator.py`

 * *Files identical despite different names*

### Comparing `mobspy-2.3.4/example_models/application_models/For_The_Trees.py` & `mobspy-2.3.5/example_models/application_models/For_The_Trees.py`

 * *Files identical despite different names*

### Comparing `mobspy-2.3.4/example_models/application_models/NOR_gate.py` & `mobspy-2.3.5/example_models/application_models/NOR_gate.py`

 * *Files identical despite different names*

### Comparing `mobspy-2.3.4/example_models/application_models/donor_receptor.py` & `mobspy-2.3.5/example_models/application_models/donor_receptor.py`

 * *Files identical despite different names*

### Comparing `mobspy-2.3.4/example_models/application_models/oscillator.py` & `mobspy-2.3.5/example_models/application_models/oscillator.py`

 * *Files identical despite different names*

### Comparing `mobspy-2.3.4/example_models/application_models/positive_phage_feedback_loop.py` & `mobspy-2.3.5/example_models/application_models/positive_phage_feedback_loop.py`

 * *Files identical despite different names*

### Comparing `mobspy-2.3.4/example_models/application_models/random_walk.py` & `mobspy-2.3.5/example_models/application_models/random_walk.py`

 * *Files identical despite different names*

### Comparing `mobspy-2.3.4/example_models/application_models/simple_infection.py` & `mobspy-2.3.5/example_models/application_models/simple_infection.py`

 * *Files identical despite different names*

### Comparing `mobspy-2.3.4/example_models/application_models/simple_repressor.py` & `mobspy-2.3.5/example_models/application_models/simple_repressor.py`

 * *Files identical despite different names*

### Comparing `mobspy-2.3.4/example_models/application_models/simple_rule_based_and_gate.py` & `mobspy-2.3.5/example_models/application_models/simple_rule_based_and_gate.py`

 * *Files identical despite different names*

### Comparing `mobspy-2.3.4/images/img.png` & `mobspy-2.3.5/images/img.png`

 * *Files identical despite different names*

### Comparing `mobspy-2.3.4/mobspy/data_handler/process_result_data.py` & `mobspy-2.3.5/mobspy/data_handler/process_result_data.py`

 * *Files identical despite different names*

### Comparing `mobspy-2.3.4/mobspy/data_handler/time_series_object.py` & `mobspy-2.3.5/mobspy/data_handler/time_series_object.py`

 * *Files identical despite different names*

### Comparing `mobspy-2.3.4/mobspy/modules/assignments_implementation.py` & `mobspy-2.3.5/mobspy/modules/assignments_implementation.py`

 * *Files identical despite different names*

### Comparing `mobspy-2.3.4/mobspy/modules/class_of_meta_specie_named_any.py` & `mobspy-2.3.5/mobspy/modules/class_of_meta_specie_named_any.py`

 * *Files identical despite different names*

### Comparing `mobspy-2.3.4/mobspy/modules/context_related_scripts.py` & `mobspy-2.3.5/mobspy/modules/context_related_scripts.py`

 * *Files identical despite different names*

### Comparing `mobspy-2.3.4/mobspy/modules/event_functions.py` & `mobspy-2.3.5/mobspy/modules/event_functions.py`

 * *Files identical despite different names*

### Comparing `mobspy-2.3.4/mobspy/modules/function_rate_code.py` & `mobspy-2.3.5/mobspy/modules/function_rate_code.py`

 * *Files identical despite different names*

### Comparing `mobspy-2.3.4/mobspy/modules/logic_operator_objects.py` & `mobspy-2.3.5/mobspy/modules/logic_operator_objects.py`

 * *Files identical despite different names*

### Comparing `mobspy-2.3.4/mobspy/modules/meta_class.py` & `mobspy-2.3.5/mobspy/modules/meta_class.py`

 * *Files identical despite different names*

### Comparing `mobspy-2.3.4/mobspy/modules/meta_class_utils.py` & `mobspy-2.3.5/mobspy/modules/meta_class_utils.py`

 * *Files identical despite different names*

### Comparing `mobspy-2.3.4/mobspy/modules/mobspy_expressions.py` & `mobspy-2.3.5/mobspy/modules/mobspy_expressions.py`

 * *Files identical despite different names*

### Comparing `mobspy-2.3.4/mobspy/modules/mobspy_parameters.py` & `mobspy-2.3.5/mobspy/modules/mobspy_parameters.py`

 * *Files identical despite different names*

### Comparing `mobspy-2.3.4/mobspy/modules/order_operators.py` & `mobspy-2.3.5/mobspy/modules/order_operators.py`

 * *Files identical despite different names*

### Comparing `mobspy-2.3.4/mobspy/modules/reaction_construction_nb.py` & `mobspy-2.3.5/mobspy/modules/reaction_construction_nb.py`

 * *Files identical despite different names*

### Comparing `mobspy-2.3.4/mobspy/modules/reaction_construction_nb_parallel.py` & `mobspy-2.3.5/mobspy/modules/reaction_construction_nb_parallel.py`

 * *Files identical despite different names*

### Comparing `mobspy-2.3.4/mobspy/modules/set_counts_module.py` & `mobspy-2.3.5/mobspy/modules/set_counts_module.py`

 * *Files identical despite different names*

### Comparing `mobspy-2.3.4/mobspy/modules/species_string_generator.py` & `mobspy-2.3.5/mobspy/modules/species_string_generator.py`

 * *Files identical despite different names*

### Comparing `mobspy-2.3.4/mobspy/modules/unit_handler.py` & `mobspy-2.3.5/mobspy/modules/unit_handler.py`

 * *Files identical despite different names*

### Comparing `mobspy-2.3.4/mobspy/parameter_estimation_data_loader/data_loader.py` & `mobspy-2.3.5/mobspy/parameter_estimation_data_loader/data_loader.py`

 * *Files identical despite different names*

### Comparing `mobspy-2.3.4/mobspy/parameter_estimation_data_loader/parameter_estimation_scripts.py` & `mobspy-2.3.5/mobspy/parameter_estimation_data_loader/parameter_estimation_scripts.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import mobspy.simulation_logging.log_scripts as simlog
 import basico
+import mobspy.patch_scripts.basico_task_parametrization as basico_task_par
 from pandas import DataFrame
 
 
 def basiCO_parameter_estimation(simulation_object, parameters_to_estimate,
                                 experimental_data=None, bound=None,
                                 method='Evolution Strategy (SRES)', verbose=True,
                                 change_parameter_values=True):
@@ -107,17 +108,17 @@
             fit_dictionary = {'name': basico_parameter_name, 'lower': bound[par][0], 'upper': bound[par][1]}
         else:
             fit_dictionary = {'name': basico_parameter_name, 'lower': bound[0], 'upper': bound[1]}
         fit_list.append(fit_dictionary)
 
     if type(experimental_data) == list or type(experimental_data) == set or type(experimental_data) == tuple:
         for i, exp in enumerate(experimental_data):
-            basico.add_experiment('exp' + str(i), exp)
+            basico_task_par.add_experiment('exp' + str(i), exp, model=model)
     else:
-        basico.add_experiment('exp1', experimental_data)
+        basico_task_par.add_experiment('exp1', experimental_data, model=model)
 
     basico.set_fit_parameters(fit_list, model=model)
     basico_results = basico.run_parameter_estimation(model=model, method=method)
 
     # WHY IS EVERYTHING PANDAS IN BASICO??????????? - I don't get paid enough for this
     results = {}
     for key, sol in basico_results.to_dict()['sol'].items():
```

### Comparing `mobspy-2.3.4/mobspy/parameter_scripts/parameter_reader.py` & `mobspy-2.3.5/mobspy/parameter_scripts/parameter_reader.py`

 * *Files identical despite different names*

### Comparing `mobspy-2.3.4/mobspy/parameter_scripts/parametric_sweeps.py` & `mobspy-2.3.5/mobspy/parameter_scripts/parametric_sweeps.py`

 * *Files identical despite different names*

### Comparing `mobspy-2.3.4/mobspy/parameters/README.md` & `mobspy-2.3.5/mobspy/parameters/README.md`

 * *Files identical despite different names*

### Comparing `mobspy-2.3.4/mobspy/parameters/default_reader.py` & `mobspy-2.3.5/mobspy/parameters/default_reader.py`

 * *Files identical despite different names*

### Comparing `mobspy-2.3.4/mobspy/parameters/example_reader.py` & `mobspy-2.3.5/mobspy/parameters/example_reader.py`

 * *Files identical despite different names*

### Comparing `mobspy-2.3.4/mobspy/plot_params/example_plot_reader.py` & `mobspy-2.3.5/mobspy/plot_params/example_plot_reader.py`

 * *Files identical despite different names*

### Comparing `mobspy-2.3.4/mobspy/plot_scripts/default_plots.py` & `mobspy-2.3.5/mobspy/plot_scripts/default_plots.py`

 * *Files identical despite different names*

### Comparing `mobspy-2.3.4/mobspy/plot_scripts/hierarchical_plot.py` & `mobspy-2.3.5/mobspy/plot_scripts/hierarchical_plot.py`

 * *Files identical despite different names*

### Comparing `mobspy-2.3.4/mobspy/plot_scripts/process_plot_data.py` & `mobspy-2.3.5/mobspy/plot_scripts/process_plot_data.py`

 * *Files identical despite different names*

### Comparing `mobspy-2.3.4/mobspy/plot_scripts/statistics_calculations.py` & `mobspy-2.3.5/mobspy/plot_scripts/statistics_calculations.py`

 * *Files identical despite different names*

### Comparing `mobspy-2.3.4/mobspy/sbml_simulator/SBMLWriter.py` & `mobspy-2.3.5/mobspy/sbml_simulator/SBMLWriter.py`

 * *Files identical despite different names*

### Comparing `mobspy-2.3.4/mobspy/sbml_simulator/__pycache__/SBMLWriter.cpython-310.pyc` & `mobspy-2.3.5/mobspy/sbml_simulator/__pycache__/SBMLWriter.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `mobspy-2.3.4/mobspy/sbml_simulator/__pycache__/builder.cpython-310.pyc` & `mobspy-2.3.5/mobspy/sbml_simulator/__pycache__/builder.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `mobspy-2.3.4/mobspy/sbml_simulator/__pycache__/run.cpython-310.pyc` & `mobspy-2.3.5/mobspy/sbml_simulator/__pycache__/run.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `mobspy-2.3.4/mobspy/sbml_simulator/builder.py` & `mobspy-2.3.5/mobspy/sbml_simulator/builder.py`

 * *Files identical despite different names*

### Comparing `mobspy-2.3.4/mobspy/sbml_simulator/run.py` & `mobspy-2.3.5/mobspy/sbml_simulator/run.py`

 * *Files identical despite different names*

### Comparing `mobspy-2.3.4/mobspy/simulation.py` & `mobspy-2.3.5/mobspy/simulation.py`

 * *Files identical despite different names*

### Comparing `mobspy-2.3.4/mobspy/simulation_logging/log_scripts.py` & `mobspy-2.3.5/mobspy/simulation_logging/log_scripts.py`

 * *Files identical despite different names*

### Comparing `mobspy-2.3.4/mobspy.egg-info/PKG-INFO` & `mobspy-2.3.5/mobspy.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mobspy
-Version: 2.3.4
+Version: 2.3.5
 Summary: A Query-Based Language for Chemical Reaction Networks
 Home-page: https://github.com/ROBACON/mobspy
 License: UNKNOWN
 Description: ![Alt text](/images/img.png "MobsPy")
         
         # MobsPy
```

### Comparing `mobspy-2.3.4/mobspy.egg-info/SOURCES.txt` & `mobspy-2.3.5/mobspy.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -270,23 +270,17 @@
 mobspy/_version.py
 mobspy/simulation.py
 mobspy.egg-info/PKG-INFO
 mobspy.egg-info/SOURCES.txt
 mobspy.egg-info/dependency_links.txt
 mobspy.egg-info/requires.txt
 mobspy.egg-info/top_level.txt
-mobspy/__pycache__/__init__.cpython-310.pyc
-mobspy/__pycache__/_version.cpython-310.pyc
-mobspy/__pycache__/simulation.cpython-310.pyc
 mobspy/data_handler/__init__.py
 mobspy/data_handler/process_result_data.py
 mobspy/data_handler/time_series_object.py
-mobspy/data_handler/__pycache__/__init__.cpython-310.pyc
-mobspy/data_handler/__pycache__/process_result_data.cpython-310.pyc
-mobspy/data_handler/__pycache__/time_series_object.cpython-310.pyc
 mobspy/modules/__init__.py
 mobspy/modules/assignments_implementation.py
 mobspy/modules/class_of_meta_specie_named_any.py
 mobspy/modules/context_related_scripts.py
 mobspy/modules/event_functions.py
 mobspy/modules/function_rate_code.py
 mobspy/modules/logic_operator_objects.py
@@ -297,52 +291,29 @@
 mobspy/modules/order_operators.py
 mobspy/modules/reaction_construction_nb.py
 mobspy/modules/reaction_construction_nb_parallel.py
 mobspy/modules/set_counts_module.py
 mobspy/modules/species_string_generator.py
 mobspy/modules/unit_handler.py
 mobspy/modules/user_functions.py
-mobspy/modules/__pycache__/__init__.cpython-310.pyc
-mobspy/modules/__pycache__/class_of_meta_specie_named_any.cpython-310.pyc
-mobspy/modules/__pycache__/event_functions.cpython-310.pyc
-mobspy/modules/__pycache__/function_rate_code.cpython-310.pyc
-mobspy/modules/__pycache__/logic_operator_objects.cpython-310.pyc
-mobspy/modules/__pycache__/meta_class.cpython-310.pyc
-mobspy/modules/__pycache__/meta_class_utils.cpython-310.pyc
-mobspy/modules/__pycache__/mobspy_expressions.cpython-310.pyc
-mobspy/modules/__pycache__/mobspy_parameters.cpython-310.pyc
-mobspy/modules/__pycache__/order_operators.cpython-310.pyc
-mobspy/modules/__pycache__/reaction_construction_nb.cpython-310.pyc
-mobspy/modules/__pycache__/reaction_construction_nb_parallel.cpython-310.pyc
-mobspy/modules/__pycache__/set_counts_module.cpython-310.pyc
-mobspy/modules/__pycache__/species_string_generator.cpython-310.pyc
-mobspy/modules/__pycache__/unit_handler.cpython-310.pyc
-mobspy/modules/__pycache__/user_functions.cpython-310.pyc
 mobspy/parameter_estimation_data_loader/__init__.py
 mobspy/parameter_estimation_data_loader/data_loader.py
 mobspy/parameter_estimation_data_loader/parameter_estimation_scripts.py
 mobspy/parameter_scripts/__init__.py
 mobspy/parameter_scripts/parameter_reader.py
 mobspy/parameter_scripts/parametric_sweeps.py
-mobspy/parameter_scripts/__pycache__/__init__.cpython-310.pyc
-mobspy/parameter_scripts/__pycache__/parameter_reader.cpython-310.pyc
-mobspy/parameter_scripts/__pycache__/parametric_sweeps.cpython-310.pyc
 mobspy/parameters/README.md
 mobspy/parameters/__init__.py
 mobspy/parameters/default_reader.py
 mobspy/parameters/example_reader.py
-mobspy/parameters/__pycache__/__init__.cpython-310.pyc
-mobspy/parameters/__pycache__/default_reader.cpython-310.pyc
-mobspy/parameters/__pycache__/example_reader.cpython-310.pyc
+mobspy/patch_scripts/__init__.py
+mobspy/patch_scripts/basico_task_parametrization.py
 mobspy/plot_params/__init__.py
 mobspy/plot_params/default_plot_reader.py
 mobspy/plot_params/example_plot_reader.py
-mobspy/plot_params/__pycache__/__init__.cpython-310.pyc
-mobspy/plot_params/__pycache__/default_plot_reader.cpython-310.pyc
-mobspy/plot_params/__pycache__/example_plot_reader.cpython-310.pyc
 mobspy/plot_scripts/__init__.py
 mobspy/plot_scripts/default_plots.py
 mobspy/plot_scripts/hierarchical_plot.py
 mobspy/plot_scripts/process_plot_data.py
 mobspy/plot_scripts/statistics_calculations.py
 mobspy/sbml_simulator/SBMLWriter.py
 mobspy/sbml_simulator/__init__.py
@@ -350,16 +321,14 @@
 mobspy/sbml_simulator/run.py
 mobspy/sbml_simulator/__pycache__/SBMLWriter.cpython-310.pyc
 mobspy/sbml_simulator/__pycache__/__init__.cpython-310.pyc
 mobspy/sbml_simulator/__pycache__/builder.cpython-310.pyc
 mobspy/sbml_simulator/__pycache__/run.cpython-310.pyc
 mobspy/simulation_logging/__init__.py
 mobspy/simulation_logging/log_scripts.py
-mobspy/simulation_logging/__pycache__/__init__.cpython-310.pyc
-mobspy/simulation_logging/__pycache__/log_scripts.cpython-310.pyc
 test_plot_images/constant_tree.png
 test_plot_images/deterministic_tree.png
 test_plot_images/stochastic_tree.png
 test_tools/model_1.txt
 test_tools/model_10.txt
 test_tools/model_11.txt
 test_tools/model_12.txt
```

### Comparing `mobspy-2.3.4/setup.py` & `mobspy-2.3.5/setup.py`

 * *Files identical despite different names*

### Comparing `mobspy-2.3.4/test_plot_images/constant_tree.png` & `mobspy-2.3.5/test_plot_images/constant_tree.png`

 * *Files identical despite different names*

### Comparing `mobspy-2.3.4/test_script.py` & `mobspy-2.3.5/test_script.py`

 * *Files identical despite different names*

### Comparing `mobspy-2.3.4/test_tools/model_15.txt` & `mobspy-2.3.5/test_tools/model_15.txt`

 * *Files identical despite different names*

### Comparing `mobspy-2.3.4/test_tools/model_19.txt` & `mobspy-2.3.5/test_tools/model_19.txt`

 * *Files identical despite different names*

### Comparing `mobspy-2.3.4/test_tools/model_21.txt` & `mobspy-2.3.5/test_tools/model_21.txt`

 * *Files identical despite different names*

### Comparing `mobspy-2.3.4/test_tools/model_24.txt` & `mobspy-2.3.5/test_tools/model_24.txt`

 * *Files identical despite different names*

### Comparing `mobspy-2.3.4/test_tools/model_26.txt` & `mobspy-2.3.5/test_tools/model_26.txt`

 * *Files identical despite different names*

### Comparing `mobspy-2.3.4/test_tools/model_3.txt` & `mobspy-2.3.5/test_tools/model_3.txt`

 * *Files identical despite different names*

### Comparing `mobspy-2.3.4/test_tools/model_31.txt` & `mobspy-2.3.5/test_tools/model_31.txt`

 * *Files identical despite different names*

### Comparing `mobspy-2.3.4/test_tools/model_33.txt` & `mobspy-2.3.5/test_tools/model_33.txt`

 * *Files identical despite different names*

### Comparing `mobspy-2.3.4/test_tools/model_38.txt` & `mobspy-2.3.5/test_tools/model_38.txt`

 * *Files identical despite different names*

### Comparing `mobspy-2.3.4/test_tools/model_39.txt` & `mobspy-2.3.5/test_tools/model_39.txt`

 * *Files identical despite different names*

### Comparing `mobspy-2.3.4/test_tools/model_4.txt` & `mobspy-2.3.5/test_tools/model_4.txt`

 * *Files identical despite different names*

### Comparing `mobspy-2.3.4/test_tools/model_40.txt` & `mobspy-2.3.5/test_tools/model_40.txt`

 * *Files identical despite different names*

### Comparing `mobspy-2.3.4/test_tools/model_41.txt` & `mobspy-2.3.5/test_tools/model_41.txt`

 * *Files identical despite different names*

### Comparing `mobspy-2.3.4/test_tools/model_45.txt` & `mobspy-2.3.5/test_tools/model_45.txt`

 * *Files identical despite different names*

### Comparing `mobspy-2.3.4/test_tools/model_5.txt` & `mobspy-2.3.5/test_tools/model_5.txt`

 * *Files identical despite different names*

### Comparing `mobspy-2.3.4/test_tools/model_7.txt` & `mobspy-2.3.5/test_tools/model_7.txt`

 * *Files identical despite different names*

### Comparing `mobspy-2.3.4/test_tools/model_9.txt` & `mobspy-2.3.5/test_tools/model_9.txt`

 * *Files identical despite different names*

