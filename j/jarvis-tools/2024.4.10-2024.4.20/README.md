# Comparing `tmp/jarvis-tools-2024.4.10.tar.gz` & `tmp/jarvis_tools-2024.4.20.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jarvis-tools-2024.4.10.tar", last modified: Sun Apr 14 14:32:21 2024, max compression
+gzip compressed data, was "jarvis_tools-2024.4.20.tar", last modified: Sat May  4 16:07:18 2024, max compression
```

## Comparing `jarvis-tools-2024.4.10.tar` & `jarvis_tools-2024.4.20.tar`

### file list

```diff
@@ -1,282 +1,283 @@
-drwxr-xr-x   0 knc6     (54782) 642div   (36677)        0 2024-04-14 14:32:21.740308 jarvis-tools-2024.4.10/
--rw-r--r--   0 knc6     (54782) 642div   (36677)     1878 2024-03-31 13:46:30.000000 jarvis-tools-2024.4.10/LICENSE.rst
--rw-r--r--   0 knc6     (54782) 642div   (36677)     3442 2024-04-14 14:32:21.740308 jarvis-tools-2024.4.10/PKG-INFO
--rw-r--r--   0 knc6     (54782) 642div   (36677)    14481 2024-03-31 13:46:30.000000 jarvis-tools-2024.4.10/README.rst
-drwxr-xr-x   0 knc6     (54782) 642div   (36677)        0 2024-04-14 14:32:18.588327 jarvis-tools-2024.4.10/jarvis/
--rw-r--r--   0 knc6     (54782) 642div   (36677)      245 2024-04-14 13:11:23.000000 jarvis-tools-2024.4.10/jarvis/__init__.py
-drwxr-xr-x   0 knc6     (54782) 642div   (36677)        0 2024-04-14 14:32:18.592327 jarvis-tools-2024.4.10/jarvis/ai/
--rw-r--r--   0 knc6     (54782) 642div   (36677)       35 2024-03-31 13:46:30.000000 jarvis-tools-2024.4.10/jarvis/ai/__init__.py
-drwxr-xr-x   0 knc6     (54782) 642div   (36677)        0 2024-04-14 14:32:18.704326 jarvis-tools-2024.4.10/jarvis/ai/descriptors/
--rw-r--r--   0 knc6     (54782) 642div   (36677)       48 2024-03-31 13:46:30.000000 jarvis-tools-2024.4.10/jarvis/ai/descriptors/__init__.py
--rw-r--r--   0 knc6     (54782) 642div   (36677)    48400 2024-03-31 13:46:30.000000 jarvis-tools-2024.4.10/jarvis/ai/descriptors/cfid.py
--rw-r--r--   0 knc6     (54782) 642div   (36677)     1370 2024-03-31 13:46:30.000000 jarvis-tools-2024.4.10/jarvis/ai/descriptors/coulomb.py
--rw-r--r--   0 knc6     (54782) 642div   (36677)      511 2024-03-31 13:46:30.000000 jarvis-tools-2024.4.10/jarvis/ai/descriptors/elemental.py
-drwxr-xr-x   0 knc6     (54782) 642div   (36677)        0 2024-04-14 14:32:18.716326 jarvis-tools-2024.4.10/jarvis/ai/gcn/
--rw-r--r--   0 knc6     (54782) 642div   (36677)       47 2024-03-31 13:46:30.000000 jarvis-tools-2024.4.10/jarvis/ai/gcn/__init__.py
-drwxr-xr-x   0 knc6     (54782) 642div   (36677)        0 2024-04-14 14:32:18.780326 jarvis-tools-2024.4.10/jarvis/ai/pkgs/
--rw-r--r--   0 knc6     (54782) 642div   (36677)       35 2024-03-31 13:46:30.000000 jarvis-tools-2024.4.10/jarvis/ai/pkgs/__init__.py
-drwxr-xr-x   0 knc6     (54782) 642div   (36677)        0 2024-04-14 14:32:18.840325 jarvis-tools-2024.4.10/jarvis/ai/pkgs/lgbm/
--rw-r--r--   0 knc6     (54782) 642div   (36677)       28 2024-03-31 13:46:30.000000 jarvis-tools-2024.4.10/jarvis/ai/pkgs/lgbm/__init__.py
--rw-r--r--   0 knc6     (54782) 642div   (36677)     1148 2024-03-31 13:46:30.000000 jarvis-tools-2024.4.10/jarvis/ai/pkgs/lgbm/classification.py
--rw-r--r--   0 knc6     (54782) 642div   (36677)     9541 2024-03-31 13:46:30.000000 jarvis-tools-2024.4.10/jarvis/ai/pkgs/lgbm/regression.py
-drwxr-xr-x   0 knc6     (54782) 642div   (36677)        0 2024-04-14 14:32:18.932325 jarvis-tools-2024.4.10/jarvis/ai/pkgs/sklearn/
--rw-r--r--   0 knc6     (54782) 642div   (36677)       44 2024-03-31 13:46:30.000000 jarvis-tools-2024.4.10/jarvis/ai/pkgs/sklearn/__init__.py
--rw-r--r--   0 knc6     (54782) 642div   (36677)     5144 2024-03-31 13:46:30.000000 jarvis-tools-2024.4.10/jarvis/ai/pkgs/sklearn/classification.py
--rw-r--r--   0 knc6     (54782) 642div   (36677)    11368 2024-03-31 13:46:30.000000 jarvis-tools-2024.4.10/jarvis/ai/pkgs/sklearn/hyper_params.py
--rw-r--r--   0 knc6     (54782) 642div   (36677)     2969 2024-03-31 13:46:30.000000 jarvis-tools-2024.4.10/jarvis/ai/pkgs/sklearn/regression.py
--rw-r--r--   0 knc6     (54782) 642div   (36677)     3585 2024-03-31 13:46:30.000000 jarvis-tools-2024.4.10/jarvis/ai/pkgs/utils.py
-drwxr-xr-x   0 knc6     (54782) 642div   (36677)        0 2024-04-14 14:32:19.000324 jarvis-tools-2024.4.10/jarvis/ai/uncertainty/
--rw-r--r--   0 knc6     (54782) 642div   (36677)       34 2024-03-31 13:46:30.000000 jarvis-tools-2024.4.10/jarvis/ai/uncertainty/__init__.py
--rw-r--r--   0 knc6     (54782) 642div   (36677)     5573 2024-03-31 13:46:30.000000 jarvis-tools-2024.4.10/jarvis/ai/uncertainty/gaussian_process_uncertainty.py
--rw-r--r--   0 knc6     (54782) 642div   (36677)     7534 2024-03-31 13:46:30.000000 jarvis-tools-2024.4.10/jarvis/ai/uncertainty/lgbm_quantile_uncertainty.py
-drwxr-xr-x   0 knc6     (54782) 642div   (36677)        0 2024-04-14 14:32:19.024324 jarvis-tools-2024.4.10/jarvis/analysis/
--rw-r--r--   0 knc6     (54782) 642div   (36677)       35 2024-03-31 13:46:30.000000 jarvis-tools-2024.4.10/jarvis/analysis/__init__.py
-drwxr-xr-x   0 knc6     (54782) 642div   (36677)        0 2024-04-14 14:32:19.052324 jarvis-tools-2024.4.10/jarvis/analysis/darkmatter/
--rw-r--r--   0 knc6     (54782) 642div   (36677)       51 2024-03-31 13:46:30.000000 jarvis-tools-2024.4.10/jarvis/analysis/darkmatter/__init__.py
--rw-r--r--   0 knc6     (54782) 642div   (36677)      786 2024-03-31 13:46:30.000000 jarvis-tools-2024.4.10/jarvis/analysis/darkmatter/metrics.py
-drwxr-xr-x   0 knc6     (54782) 642div   (36677)        0 2024-04-14 14:32:19.148323 jarvis-tools-2024.4.10/jarvis/analysis/defects/
--rw-r--r--   0 knc6     (54782) 642div   (36677)       47 2024-03-31 13:46:30.000000 jarvis-tools-2024.4.10/jarvis/analysis/defects/__init__.py
--rw-r--r--   0 knc6     (54782) 642div   (36677)     2328 2024-03-31 13:46:30.000000 jarvis-tools-2024.4.10/jarvis/analysis/defects/substitutions.py
--rw-r--r--   0 knc6     (54782) 642div   (36677)     9305 2024-03-31 13:46:30.000000 jarvis-tools-2024.4.10/jarvis/analysis/defects/surface.py
--rw-r--r--   0 knc6     (54782) 642div   (36677)     5048 2024-03-31 13:46:30.000000 jarvis-tools-2024.4.10/jarvis/analysis/defects/vacancy.py
-drwxr-xr-x   0 knc6     (54782) 642div   (36677)        0 2024-04-14 14:32:19.180323 jarvis-tools-2024.4.10/jarvis/analysis/diffraction/
--rw-r--r--   0 knc6     (54782) 642div   (36677)       49 2024-03-31 13:46:30.000000 jarvis-tools-2024.4.10/jarvis/analysis/diffraction/__init__.py
--rw-r--r--   0 knc6     (54782) 642div   (36677)     6825 2024-03-31 13:46:30.000000 jarvis-tools-2024.4.10/jarvis/analysis/diffraction/atomic_scattering_params.json
--rw-r--r--   0 knc6     (54782) 642div   (36677)     7327 2024-03-31 13:46:30.000000 jarvis-tools-2024.4.10/jarvis/analysis/diffraction/xrd.py
-drwxr-xr-x   0 knc6     (54782) 642div   (36677)        0 2024-04-14 14:32:19.200323 jarvis-tools-2024.4.10/jarvis/analysis/elastic/
--rw-r--r--   0 knc6     (54782) 642div   (36677)       43 2024-03-31 13:46:30.000000 jarvis-tools-2024.4.10/jarvis/analysis/elastic/__init__.py
--rw-r--r--   0 knc6     (54782) 642div   (36677)     6602 2024-03-31 13:46:30.000000 jarvis-tools-2024.4.10/jarvis/analysis/elastic/tensor.py
-drwxr-xr-x   0 knc6     (54782) 642div   (36677)        0 2024-04-14 14:32:19.260323 jarvis-tools-2024.4.10/jarvis/analysis/interface/
--rw-r--r--   0 knc6     (54782) 642div   (36677)       53 2024-03-31 13:46:30.000000 jarvis-tools-2024.4.10/jarvis/analysis/interface/__init__.py
--rw-r--r--   0 knc6     (54782) 642div   (36677)    14764 2024-03-31 13:46:30.000000 jarvis-tools-2024.4.10/jarvis/analysis/interface/zur.py
-drwxr-xr-x   0 knc6     (54782) 642div   (36677)        0 2024-04-14 14:32:19.296323 jarvis-tools-2024.4.10/jarvis/analysis/magnetism/
--rw-r--r--   0 knc6     (54782) 642div   (36677)       46 2024-03-31 13:46:30.000000 jarvis-tools-2024.4.10/jarvis/analysis/magnetism/__init__.py
--rw-r--r--   0 knc6     (54782) 642div   (36677)     8101 2024-03-31 13:46:30.000000 jarvis-tools-2024.4.10/jarvis/analysis/magnetism/magmom_setup.py
-drwxr-xr-x   0 knc6     (54782) 642div   (36677)        0 2024-04-14 14:32:19.332322 jarvis-tools-2024.4.10/jarvis/analysis/periodic/
--rw-r--r--   0 knc6     (54782) 642div   (36677)       49 2024-03-31 13:46:30.000000 jarvis-tools-2024.4.10/jarvis/analysis/periodic/__init__.py
--rw-r--r--   0 knc6     (54782) 642div   (36677)     5907 2024-03-31 13:46:30.000000 jarvis-tools-2024.4.10/jarvis/analysis/periodic/ptable.py
-drwxr-xr-x   0 knc6     (54782) 642div   (36677)        0 2024-04-14 14:32:19.424322 jarvis-tools-2024.4.10/jarvis/analysis/phonon/
--rw-r--r--   0 knc6     (54782) 642div   (36677)       49 2024-03-31 13:46:30.000000 jarvis-tools-2024.4.10/jarvis/analysis/phonon/__init__.py
--rw-r--r--   0 knc6     (54782) 642div   (36677)     3934 2024-03-31 13:46:30.000000 jarvis-tools-2024.4.10/jarvis/analysis/phonon/dos.py
--rw-r--r--   0 knc6     (54782) 642div   (36677)     1189 2024-03-31 13:46:30.000000 jarvis-tools-2024.4.10/jarvis/analysis/phonon/force_constants.py
--rw-r--r--   0 knc6     (54782) 642div   (36677)     6473 2024-03-31 13:46:30.000000 jarvis-tools-2024.4.10/jarvis/analysis/phonon/ir.py
-drwxr-xr-x   0 knc6     (54782) 642div   (36677)        0 2024-04-14 14:32:19.496321 jarvis-tools-2024.4.10/jarvis/analysis/solarefficiency/
--rw-r--r--   0 knc6     (54782) 642div   (36677)       59 2024-03-31 13:46:30.000000 jarvis-tools-2024.4.10/jarvis/analysis/solarefficiency/__init__.py
--rw-r--r--   0 knc6     (54782) 642div   (36677)    35436 2024-03-31 13:46:30.000000 jarvis-tools-2024.4.10/jarvis/analysis/solarefficiency/am1.5G.dat
--rw-r--r--   0 knc6     (54782) 642div   (36677)    14217 2024-03-31 13:46:30.000000 jarvis-tools-2024.4.10/jarvis/analysis/solarefficiency/solar.py
-drwxr-xr-x   0 knc6     (54782) 642div   (36677)        0 2024-04-14 14:32:19.544321 jarvis-tools-2024.4.10/jarvis/analysis/stem/
--rw-r--r--   0 knc6     (54782) 642div   (36677)       38 2024-03-31 13:46:30.000000 jarvis-tools-2024.4.10/jarvis/analysis/stem/__init__.py
--rw-r--r--   0 knc6     (54782) 642div   (36677)     7315 2024-03-31 13:46:30.000000 jarvis-tools-2024.4.10/jarvis/analysis/stem/convolution_apprx.py
-drwxr-xr-x   0 knc6     (54782) 642div   (36677)        0 2024-04-14 14:32:19.564321 jarvis-tools-2024.4.10/jarvis/analysis/stm/
--rw-r--r--   0 knc6     (54782) 642div   (36677)       67 2024-03-31 13:46:30.000000 jarvis-tools-2024.4.10/jarvis/analysis/stm/__init__.py
--rw-r--r--   0 knc6     (54782) 642div   (36677)    10094 2024-03-31 13:46:30.000000 jarvis-tools-2024.4.10/jarvis/analysis/stm/tersoff_hamann.py
-drwxr-xr-x   0 knc6     (54782) 642div   (36677)        0 2024-04-14 14:32:19.588321 jarvis-tools-2024.4.10/jarvis/analysis/structure/
--rw-r--r--   0 knc6     (54782) 642div   (36677)       46 2024-03-31 13:46:30.000000 jarvis-tools-2024.4.10/jarvis/analysis/structure/__init__.py
--rw-r--r--   0 knc6     (54782) 642div   (36677)    21798 2024-03-31 13:46:30.000000 jarvis-tools-2024.4.10/jarvis/analysis/structure/neighbors.py
--rw-r--r--   0 knc6     (54782) 642div   (36677)    25663 2024-03-31 13:46:30.000000 jarvis-tools-2024.4.10/jarvis/analysis/structure/spacegroup.py
-drwxr-xr-x   0 knc6     (54782) 642div   (36677)        0 2024-04-14 14:32:19.696320 jarvis-tools-2024.4.10/jarvis/analysis/thermodynamics/
--rw-r--r--   0 knc6     (54782) 642div   (36677)       42 2024-03-31 13:46:30.000000 jarvis-tools-2024.4.10/jarvis/analysis/thermodynamics/__init__.py
--rw-r--r--   0 knc6     (54782) 642div   (36677)    14613 2024-03-31 13:46:30.000000 jarvis-tools-2024.4.10/jarvis/analysis/thermodynamics/energetics.py
--rw-r--r--   0 knc6     (54782) 642div   (36677)     4527 2024-03-31 13:46:30.000000 jarvis-tools-2024.4.10/jarvis/analysis/thermodynamics/unary.json
--rw-r--r--   0 knc6     (54782) 642div   (36677)     4781 2024-03-31 13:46:30.000000 jarvis-tools-2024.4.10/jarvis/analysis/thermodynamics/unary_qe_tb.json
-drwxr-xr-x   0 knc6     (54782) 642div   (36677)        0 2024-04-14 14:32:19.716320 jarvis-tools-2024.4.10/jarvis/analysis/topological/
--rw-r--r--   0 knc6     (54782) 642div   (36677)       50 2024-03-31 13:46:30.000000 jarvis-tools-2024.4.10/jarvis/analysis/topological/__init__.py
--rw-r--r--   0 knc6     (54782) 642div   (36677)    11892 2024-03-31 13:46:30.000000 jarvis-tools-2024.4.10/jarvis/analysis/topological/spillage.py
-drwxr-xr-x   0 knc6     (54782) 642div   (36677)        0 2024-04-14 14:32:19.856319 jarvis-tools-2024.4.10/jarvis/core/
--rw-r--r--   0 knc6     (54782) 642div   (36677)  1421253 2024-03-31 13:46:30.000000 jarvis-tools-2024.4.10/jarvis/core/Elements.json
--rw-r--r--   0 knc6     (54782) 642div   (36677)       49 2024-03-31 13:46:30.000000 jarvis-tools-2024.4.10/jarvis/core/__init__.py
--rw-r--r--   0 knc6     (54782) 642div   (36677)    28393 2024-03-31 13:46:30.000000 jarvis-tools-2024.4.10/jarvis/core/atom_init.json
--rw-r--r--   0 knc6     (54782) 642div   (36677)    74159 2024-04-14 12:46:57.000000 jarvis-tools-2024.4.10/jarvis/core/atoms.py
--rw-r--r--   0 knc6     (54782) 642div   (36677)     4313 2024-03-31 13:46:30.000000 jarvis-tools-2024.4.10/jarvis/core/circuits.py
--rw-r--r--   0 knc6     (54782) 642div   (36677)     5258 2024-03-31 13:46:30.000000 jarvis-tools-2024.4.10/jarvis/core/composition.py
--rw-r--r--   0 knc6     (54782) 642div   (36677)  1162701 2024-03-31 13:46:30.000000 jarvis-tools-2024.4.10/jarvis/core/element_charge.json
--rw-r--r--   0 knc6     (54782) 642div   (36677)    22713 2024-04-14 12:39:39.000000 jarvis-tools-2024.4.10/jarvis/core/graphs.py
--rw-r--r--   0 knc6     (54782) 642div   (36677)    10693 2024-03-31 13:46:30.000000 jarvis-tools-2024.4.10/jarvis/core/image.py
--rw-r--r--   0 knc6     (54782) 642div   (36677)    37783 2024-03-31 13:46:30.000000 jarvis-tools-2024.4.10/jarvis/core/kpoints.py
--rw-r--r--   0 knc6     (54782) 642div   (36677)    17427 2024-03-31 13:46:30.000000 jarvis-tools-2024.4.10/jarvis/core/lattice.py
--rw-r--r--   0 knc6     (54782) 642div   (36677)    47766 2024-03-31 13:46:30.000000 jarvis-tools-2024.4.10/jarvis/core/magpie.json
--rw-r--r--   0 knc6     (54782) 642div   (36677)    12121 2024-03-31 13:46:30.000000 jarvis-tools-2024.4.10/jarvis/core/specie.py
--rw-r--r--   0 knc6     (54782) 642div   (36677)     2891 2024-03-31 13:46:30.000000 jarvis-tools-2024.4.10/jarvis/core/spectrum.py
--rw-r--r--   0 knc6     (54782) 642div   (36677)     8933 2024-03-31 13:46:30.000000 jarvis-tools-2024.4.10/jarvis/core/utils.py
-drwxr-xr-x   0 knc6     (54782) 642div   (36677)        0 2024-04-14 14:32:19.968319 jarvis-tools-2024.4.10/jarvis/db/
--rw-r--r--   0 knc6     (54782) 642div   (36677)       53 2024-03-31 13:46:30.000000 jarvis-tools-2024.4.10/jarvis/db/__init__.py
--rw-r--r--   0 knc6     (54782) 642div   (36677)    26622 2024-03-31 13:46:30.000000 jarvis-tools-2024.4.10/jarvis/db/figshare.py
--rw-r--r--   0 knc6     (54782) 642div   (36677)      378 2024-03-31 13:46:30.000000 jarvis-tools-2024.4.10/jarvis/db/jsonutils.py
--rw-r--r--   0 knc6     (54782) 642div   (36677)     7761 2024-03-31 13:46:30.000000 jarvis-tools-2024.4.10/jarvis/db/lammps_to_xml.py
--rw-r--r--   0 knc6     (54782) 642div   (36677)    10649 2024-03-31 13:46:30.000000 jarvis-tools-2024.4.10/jarvis/db/qe_to_xml.py
--rw-r--r--   0 knc6     (54782) 642div   (36677)    17359 2024-03-31 16:17:56.000000 jarvis-tools-2024.4.10/jarvis/db/restapi.py
--rw-r--r--   0 knc6     (54782) 642div   (36677)    75218 2024-03-31 13:46:30.000000 jarvis-tools-2024.4.10/jarvis/db/vasp_to_xml.py
--rw-r--r--   0 knc6     (54782) 642div   (36677)     9586 2024-03-31 13:46:30.000000 jarvis-tools-2024.4.10/jarvis/db/webpages.py
-drwxr-xr-x   0 knc6     (54782) 642div   (36677)        0 2024-04-14 14:32:19.992318 jarvis-tools-2024.4.10/jarvis/io/
--rw-r--r--   0 knc6     (54782) 642div   (36677)       76 2024-03-31 13:46:31.000000 jarvis-tools-2024.4.10/jarvis/io/__init__.py
-drwxr-xr-x   0 knc6     (54782) 642div   (36677)        0 2024-04-14 14:32:20.048318 jarvis-tools-2024.4.10/jarvis/io/boltztrap/
--rw-r--r--   0 knc6     (54782) 642div   (36677)       67 2024-03-31 13:46:31.000000 jarvis-tools-2024.4.10/jarvis/io/boltztrap/__init__.py
--rw-r--r--   0 knc6     (54782) 642div   (36677)     6511 2024-03-31 13:46:31.000000 jarvis-tools-2024.4.10/jarvis/io/boltztrap/inputs.py
--rw-r--r--   0 knc6     (54782) 642div   (36677)     6767 2024-03-31 13:46:31.000000 jarvis-tools-2024.4.10/jarvis/io/boltztrap/outputs.py
-drwxr-xr-x   0 knc6     (54782) 642div   (36677)        0 2024-04-14 14:32:20.100318 jarvis-tools-2024.4.10/jarvis/io/calphad/
--rw-r--r--   0 knc6     (54782) 642div   (36677)       61 2024-03-31 13:46:31.000000 jarvis-tools-2024.4.10/jarvis/io/calphad/__init__.py
--rw-r--r--   0 knc6     (54782) 642div   (36677)     4228 2024-03-31 13:46:31.000000 jarvis-tools-2024.4.10/jarvis/io/calphad/write_decorated_poscar.py
-drwxr-xr-x   0 knc6     (54782) 642div   (36677)        0 2024-04-14 14:32:20.156318 jarvis-tools-2024.4.10/jarvis/io/lammps/
--rw-r--r--   0 knc6     (54782) 642div   (36677)       52 2024-03-31 13:46:31.000000 jarvis-tools-2024.4.10/jarvis/io/lammps/__init__.py
--rw-r--r--   0 knc6     (54782) 642div   (36677)    14615 2024-03-31 15:24:29.000000 jarvis-tools-2024.4.10/jarvis/io/lammps/inputs.py
--rw-r--r--   0 knc6     (54782) 642div   (36677)    20760 2024-03-31 15:15:06.000000 jarvis-tools-2024.4.10/jarvis/io/lammps/outputs.py
-drwxr-xr-x   0 knc6     (54782) 642div   (36677)        0 2024-04-14 14:32:20.240317 jarvis-tools-2024.4.10/jarvis/io/nexus/
--rw-r--r--   0 knc6     (54782) 642div   (36677)       47 2024-03-31 13:46:31.000000 jarvis-tools-2024.4.10/jarvis/io/nexus/__init__.py
--rw-r--r--   0 knc6     (54782) 642div   (36677)     4519 2024-03-31 13:46:31.000000 jarvis-tools-2024.4.10/jarvis/io/nexus/inputs.py
--rw-r--r--   0 knc6     (54782) 642div   (36677)       36 2024-03-31 13:46:31.000000 jarvis-tools-2024.4.10/jarvis/io/nexus/outputs.py
-drwxr-xr-x   0 knc6     (54782) 642div   (36677)        0 2024-04-14 14:32:20.280317 jarvis-tools-2024.4.10/jarvis/io/pennylane/
--rw-r--r--   0 knc6     (54782) 642div   (36677)       61 2024-03-31 13:46:31.000000 jarvis-tools-2024.4.10/jarvis/io/pennylane/__init__.py
--rw-r--r--   0 knc6     (54782) 642div   (36677)     2196 2024-03-31 13:46:31.000000 jarvis-tools-2024.4.10/jarvis/io/pennylane/inputs.py
-drwxr-xr-x   0 knc6     (54782) 642div   (36677)        0 2024-04-14 14:32:20.344316 jarvis-tools-2024.4.10/jarvis/io/phonopy/
--rw-r--r--   0 knc6     (54782) 642div   (36677)       43 2024-03-31 13:46:31.000000 jarvis-tools-2024.4.10/jarvis/io/phonopy/__init__.py
--rw-r--r--   0 knc6     (54782) 642div   (36677)     4501 2024-03-31 13:46:31.000000 jarvis-tools-2024.4.10/jarvis/io/phonopy/fcmat2hr.py
--rw-r--r--   0 knc6     (54782) 642div   (36677)     6844 2024-03-31 13:46:31.000000 jarvis-tools-2024.4.10/jarvis/io/phonopy/inputs.py
--rw-r--r--   0 knc6     (54782) 642div   (36677)     5696 2024-03-31 13:46:31.000000 jarvis-tools-2024.4.10/jarvis/io/phonopy/outputs.py
-drwxr-xr-x   0 knc6     (54782) 642div   (36677)        0 2024-04-14 14:32:20.372316 jarvis-tools-2024.4.10/jarvis/io/prismatic/
--rw-r--r--   0 knc6     (54782) 642div   (36677)       50 2024-03-31 13:46:31.000000 jarvis-tools-2024.4.10/jarvis/io/prismatic/__init__.py
--rw-r--r--   0 knc6     (54782) 642div   (36677)      674 2024-03-31 13:46:31.000000 jarvis-tools-2024.4.10/jarvis/io/prismatic/inputs.py
-drwxr-xr-x   0 knc6     (54782) 642div   (36677)        0 2024-04-14 14:32:20.428316 jarvis-tools-2024.4.10/jarvis/io/qe/
--rw-r--r--   0 knc6     (54782) 642div   (36677)       57 2024-03-31 13:46:31.000000 jarvis-tools-2024.4.10/jarvis/io/qe/__init__.py
--rw-r--r--   0 knc6     (54782) 642div   (36677)    15329 2024-03-31 13:46:58.000000 jarvis-tools-2024.4.10/jarvis/io/qe/inputs.py
--rwxr-xr-x   0 knc6     (54782) 642div   (36677)    29549 2024-03-31 13:46:31.000000 jarvis-tools-2024.4.10/jarvis/io/qe/outputs.py
-drwxr-xr-x   0 knc6     (54782) 642div   (36677)        0 2024-04-14 14:32:20.468316 jarvis-tools-2024.4.10/jarvis/io/qiskit/
--rw-r--r--   0 knc6     (54782) 642div   (36677)       56 2024-03-31 13:46:31.000000 jarvis-tools-2024.4.10/jarvis/io/qiskit/__init__.py
--rw-r--r--   0 knc6     (54782) 642div   (36677)    12104 2024-03-31 13:46:31.000000 jarvis-tools-2024.4.10/jarvis/io/qiskit/inputs.py
-drwxr-xr-x   0 knc6     (54782) 642div   (36677)        0 2024-04-14 14:32:20.508315 jarvis-tools-2024.4.10/jarvis/io/tequila/
--rw-r--r--   0 knc6     (54782) 642div   (36677)       60 2024-03-31 13:46:31.000000 jarvis-tools-2024.4.10/jarvis/io/tequila/__init__.py
--rw-r--r--   0 knc6     (54782) 642div   (36677)     2702 2024-03-31 13:46:31.000000 jarvis-tools-2024.4.10/jarvis/io/tequila/inputs.py
-drwxr-xr-x   0 knc6     (54782) 642div   (36677)        0 2024-04-14 14:32:20.536315 jarvis-tools-2024.4.10/jarvis/io/vasp/
--rw-r--r--   0 knc6     (54782) 642div   (36677)       56 2024-03-31 13:46:31.000000 jarvis-tools-2024.4.10/jarvis/io/vasp/__init__.py
--rw-r--r--   0 knc6     (54782) 642div   (36677)     1522 2024-03-31 13:46:31.000000 jarvis-tools-2024.4.10/jarvis/io/vasp/default_potcars.json
--rw-r--r--   0 knc6     (54782) 642div   (36677)    20248 2024-03-31 13:46:31.000000 jarvis-tools-2024.4.10/jarvis/io/vasp/inputs.py
--rw-r--r--   0 knc6     (54782) 642div   (36677)    82300 2024-03-31 13:46:31.000000 jarvis-tools-2024.4.10/jarvis/io/vasp/outputs.py
-drwxr-xr-x   0 knc6     (54782) 642div   (36677)        0 2024-04-14 14:32:20.568315 jarvis-tools-2024.4.10/jarvis/io/wannier/
--rw-r--r--   0 knc6     (54782) 642div   (36677)       61 2024-03-31 13:46:31.000000 jarvis-tools-2024.4.10/jarvis/io/wannier/__init__.py
--rw-r--r--   0 knc6     (54782) 642div   (36677)     4550 2024-03-31 13:46:31.000000 jarvis-tools-2024.4.10/jarvis/io/wannier/default_semicore.json
--rw-r--r--   0 knc6     (54782) 642div   (36677)     6929 2024-03-31 13:46:31.000000 jarvis-tools-2024.4.10/jarvis/io/wannier/inputs.py
--rw-r--r--   0 knc6     (54782) 642div   (36677)    34195 2024-03-31 13:46:31.000000 jarvis-tools-2024.4.10/jarvis/io/wannier/outputs.py
-drwxr-xr-x   0 knc6     (54782) 642div   (36677)        0 2024-04-14 14:32:20.620315 jarvis-tools-2024.4.10/jarvis/io/wanniertools/
--rw-r--r--   0 knc6     (54782) 642div   (36677)       60 2024-03-31 13:46:31.000000 jarvis-tools-2024.4.10/jarvis/io/wanniertools/__init__.py
--rw-r--r--   0 knc6     (54782) 642div   (36677)    10376 2024-03-31 13:46:31.000000 jarvis-tools-2024.4.10/jarvis/io/wanniertools/inputs.py
--rw-r--r--   0 knc6     (54782) 642div   (36677)     3818 2024-03-31 13:46:31.000000 jarvis-tools-2024.4.10/jarvis/io/wanniertools/outputs.py
-drwxr-xr-x   0 knc6     (54782) 642div   (36677)        0 2024-04-14 14:32:20.656315 jarvis-tools-2024.4.10/jarvis/io/wien2k/
--rw-r--r--   0 knc6     (54782) 642div   (36677)       55 2024-03-31 13:46:31.000000 jarvis-tools-2024.4.10/jarvis/io/wien2k/__init__.py
--rw-r--r--   0 knc6     (54782) 642div   (36677)     3238 2024-03-31 13:46:31.000000 jarvis-tools-2024.4.10/jarvis/io/wien2k/inputs.py
--rw-r--r--   0 knc6     (54782) 642div   (36677)     3353 2024-03-31 13:46:31.000000 jarvis-tools-2024.4.10/jarvis/io/wien2k/outputs.py
-drwxr-xr-x   0 knc6     (54782) 642div   (36677)        0 2024-04-14 14:32:20.688314 jarvis-tools-2024.4.10/jarvis/io/zeopp/
--rw-r--r--   0 knc6     (54782) 642div   (36677)       35 2024-03-31 13:46:31.000000 jarvis-tools-2024.4.10/jarvis/io/zeopp/__init__.py
--rw-r--r--   0 knc6     (54782) 642div   (36677)     2184 2024-03-31 13:46:31.000000 jarvis-tools-2024.4.10/jarvis/io/zeopp/inputs.py
-drwxr-xr-x   0 knc6     (54782) 642div   (36677)        0 2024-04-14 14:32:20.736314 jarvis-tools-2024.4.10/jarvis/tasks/
--rw-r--r--   0 knc6     (54782) 642div   (36677)       47 2024-03-31 13:46:31.000000 jarvis-tools-2024.4.10/jarvis/tasks/__init__.py
-drwxr-xr-x   0 knc6     (54782) 642div   (36677)        0 2024-04-14 14:32:20.748314 jarvis-tools-2024.4.10/jarvis/tasks/boltztrap/
--rw-r--r--   0 knc6     (54782) 642div   (36677)       56 2024-03-31 13:46:31.000000 jarvis-tools-2024.4.10/jarvis/tasks/boltztrap/__init__.py
--rw-r--r--   0 knc6     (54782) 642div   (36677)      608 2024-03-31 13:46:31.000000 jarvis-tools-2024.4.10/jarvis/tasks/boltztrap/run.py
-drwxr-xr-x   0 knc6     (54782) 642div   (36677)        0 2024-04-14 14:32:20.784314 jarvis-tools-2024.4.10/jarvis/tasks/lammps/
--rw-r--r--   0 knc6     (54782) 642div   (36677)       55 2024-03-31 13:46:31.000000 jarvis-tools-2024.4.10/jarvis/tasks/lammps/__init__.py
--rw-r--r--   0 knc6     (54782) 642div   (36677)    14071 2024-03-31 15:50:24.000000 jarvis-tools-2024.4.10/jarvis/tasks/lammps/lammps.py
-drwxr-xr-x   0 knc6     (54782) 642div   (36677)        0 2024-04-14 14:32:20.956313 jarvis-tools-2024.4.10/jarvis/tasks/lammps/templates/
--rw-r--r--   0 knc6     (54782) 642div   (36677)       47 2024-03-31 13:46:31.000000 jarvis-tools-2024.4.10/jarvis/tasks/lammps/templates/__init__.py
--rw-r--r--   0 knc6     (54782) 642div   (36677)     3463 2024-03-31 13:46:31.000000 jarvis-tools-2024.4.10/jarvis/tasks/lammps/templates/displace.mod
--rw-r--r--   0 knc6     (54782) 642div   (36677)     6416 2024-03-31 13:46:31.000000 jarvis-tools-2024.4.10/jarvis/tasks/lammps/templates/inelast.mod
--rw-r--r--   0 knc6     (54782) 642div   (36677)     6449 2024-03-31 13:46:31.000000 jarvis-tools-2024.4.10/jarvis/tasks/lammps/templates/inelast_min.mod
--rw-r--r--   0 knc6     (54782) 642div   (36677)     6418 2024-03-31 13:46:31.000000 jarvis-tools-2024.4.10/jarvis/tasks/lammps/templates/inelast_nobox.mod
--rw-r--r--   0 knc6     (54782) 642div   (36677)     6415 2024-03-31 13:46:31.000000 jarvis-tools-2024.4.10/jarvis/tasks/lammps/templates/inelastcomb.mod
--rw-r--r--   0 knc6     (54782) 642div   (36677)     6389 2024-03-31 13:46:31.000000 jarvis-tools-2024.4.10/jarvis/tasks/lammps/templates/inelastreax.mod
--rw-r--r--   0 knc6     (54782) 642div   (36677)     2653 2024-03-31 13:46:31.000000 jarvis-tools-2024.4.10/jarvis/tasks/lammps/templates/relax.mod
--rw-r--r--   0 knc6     (54782) 642div   (36677)      145 2024-03-31 13:46:31.000000 jarvis-tools-2024.4.10/jarvis/tasks/lammps/templates/run0.mod
--rw-r--r--   0 knc6     (54782) 642div   (36677)      917 2024-03-31 13:46:31.000000 jarvis-tools-2024.4.10/jarvis/tasks/lammps/templates/templates.py
-drwxr-xr-x   0 knc6     (54782) 642div   (36677)        0 2024-04-14 14:32:20.964313 jarvis-tools-2024.4.10/jarvis/tasks/nexus/
--rw-r--r--   0 knc6     (54782) 642div   (36677)       34 2024-03-31 13:46:31.000000 jarvis-tools-2024.4.10/jarvis/tasks/nexus/__init__.py
--rw-r--r--   0 knc6     (54782) 642div   (36677)     3243 2024-03-31 13:46:31.000000 jarvis-tools-2024.4.10/jarvis/tasks/nexus/qmc.py
-drwxr-xr-x   0 knc6     (54782) 642div   (36677)        0 2024-04-14 14:32:20.996313 jarvis-tools-2024.4.10/jarvis/tasks/phonopy/
--rw-r--r--   0 knc6     (54782) 642div   (36677)       54 2024-03-31 13:46:31.000000 jarvis-tools-2024.4.10/jarvis/tasks/phonopy/__init__.py
--rw-r--r--   0 knc6     (54782) 642div   (36677)      765 2024-03-31 13:46:31.000000 jarvis-tools-2024.4.10/jarvis/tasks/phonopy/run.py
-drwxr-xr-x   0 knc6     (54782) 642div   (36677)        0 2024-04-14 14:32:21.088312 jarvis-tools-2024.4.10/jarvis/tasks/qe/
--rw-r--r--   0 knc6     (54782) 642div   (36677)       29 2024-03-31 13:46:31.000000 jarvis-tools-2024.4.10/jarvis/tasks/qe/__init__.py
--rw-r--r--   0 knc6     (54782) 642div   (36677)    19582 2024-03-31 13:46:31.000000 jarvis-tools-2024.4.10/jarvis/tasks/qe/converg.py
--rw-r--r--   0 knc6     (54782) 642div   (36677)     3665 2024-03-31 13:46:31.000000 jarvis-tools-2024.4.10/jarvis/tasks/qe/master_super.py
--rw-r--r--   0 knc6     (54782) 642div   (36677)     4209 2024-03-31 13:46:31.000000 jarvis-tools-2024.4.10/jarvis/tasks/qe/qe.py
--rw-r--r--   0 knc6     (54782) 642div   (36677)    10626 2024-04-14 12:24:55.000000 jarvis-tools-2024.4.10/jarvis/tasks/qe/super.py
--rw-r--r--   0 knc6     (54782) 642div   (36677)     7387 2024-03-31 13:46:31.000000 jarvis-tools-2024.4.10/jarvis/tasks/qe/super_tetra.py
--rw-r--r--   0 knc6     (54782) 642div   (36677)     5873 2024-03-31 13:46:31.000000 jarvis-tools-2024.4.10/jarvis/tasks/queue_jobs.py
-drwxr-xr-x   0 knc6     (54782) 642div   (36677)        0 2024-04-14 14:32:21.108312 jarvis-tools-2024.4.10/jarvis/tasks/vasp/
--rw-r--r--   0 knc6     (54782) 642div   (36677)       61 2024-03-31 13:46:31.000000 jarvis-tools-2024.4.10/jarvis/tasks/vasp/__init__.py
--rw-r--r--   0 knc6     (54782) 642div   (36677)    66478 2024-03-31 13:46:31.000000 jarvis-tools-2024.4.10/jarvis/tasks/vasp/vasp.py
-drwxr-xr-x   0 knc6     (54782) 642div   (36677)        0 2024-04-14 14:32:21.132312 jarvis-tools-2024.4.10/jarvis/tests/
--rw-r--r--   0 knc6     (54782) 642div   (36677)       35 2024-03-31 13:46:31.000000 jarvis-tools-2024.4.10/jarvis/tests/__init__.py
-drwxr-xr-x   0 knc6     (54782) 642div   (36677)        0 2024-04-14 14:32:21.136312 jarvis-tools-2024.4.10/jarvis/tests/testfiles/
--rw-r--r--   0 knc6     (54782) 642div   (36677)        0 2024-03-31 13:46:31.000000 jarvis-tools-2024.4.10/jarvis/tests/testfiles/__init__.py
-drwxr-xr-x   0 knc6     (54782) 642div   (36677)        0 2024-04-14 14:32:21.160312 jarvis-tools-2024.4.10/jarvis/tests/testfiles/ai/
--rw-r--r--   0 knc6     (54782) 642div   (36677)        0 2024-03-31 13:46:31.000000 jarvis-tools-2024.4.10/jarvis/tests/testfiles/ai/__init__.py
--rw-r--r--   0 knc6     (54782) 642div   (36677)      950 2024-03-31 13:46:31.000000 jarvis-tools-2024.4.10/jarvis/tests/testfiles/ai/test_ai_uncertainty.py
--rw-r--r--   0 knc6     (54782) 642div   (36677)    67390 2024-03-31 13:46:31.000000 jarvis-tools-2024.4.10/jarvis/tests/testfiles/ai/test_desc.py
--rw-r--r--   0 knc6     (54782) 642div   (36677)     2206 2024-03-31 13:46:31.000000 jarvis-tools-2024.4.10/jarvis/tests/testfiles/ai/test_pkgs.py
-drwxr-xr-x   0 knc6     (54782) 642div   (36677)        0 2024-04-14 14:32:21.168312 jarvis-tools-2024.4.10/jarvis/tests/testfiles/analysis/
--rw-r--r--   0 knc6     (54782) 642div   (36677)        0 2024-03-31 13:46:31.000000 jarvis-tools-2024.4.10/jarvis/tests/testfiles/analysis/__init__.py
-drwxr-xr-x   0 knc6     (54782) 642div   (36677)        0 2024-04-14 14:32:21.172312 jarvis-tools-2024.4.10/jarvis/tests/testfiles/analysis/darkmatter/
--rw-r--r--   0 knc6     (54782) 642div   (36677)        0 2024-03-31 13:46:31.000000 jarvis-tools-2024.4.10/jarvis/tests/testfiles/analysis/darkmatter/__init__.py
--rw-r--r--   0 knc6     (54782) 642div   (36677)      464 2024-03-31 13:46:31.000000 jarvis-tools-2024.4.10/jarvis/tests/testfiles/analysis/darkmatter/test_metrics.py
-drwxr-xr-x   0 knc6     (54782) 642div   (36677)        0 2024-04-14 14:32:21.216311 jarvis-tools-2024.4.10/jarvis/tests/testfiles/analysis/defects/
--rw-r--r--   0 knc6     (54782) 642div   (36677)        0 2024-03-31 13:46:31.000000 jarvis-tools-2024.4.10/jarvis/tests/testfiles/analysis/defects/__init__.py
--rw-r--r--   0 knc6     (54782) 642div   (36677)      444 2024-03-31 13:46:31.000000 jarvis-tools-2024.4.10/jarvis/tests/testfiles/analysis/defects/test_subs.py
--rw-r--r--   0 knc6     (54782) 642div   (36677)     3252 2024-03-31 13:46:31.000000 jarvis-tools-2024.4.10/jarvis/tests/testfiles/analysis/defects/test_surface.py
--rw-r--r--   0 knc6     (54782) 642div   (36677)     1216 2024-03-31 13:46:31.000000 jarvis-tools-2024.4.10/jarvis/tests/testfiles/analysis/defects/test_vacancy.py
-drwxr-xr-x   0 knc6     (54782) 642div   (36677)        0 2024-04-14 14:32:21.236311 jarvis-tools-2024.4.10/jarvis/tests/testfiles/analysis/elastic/
--rw-r--r--   0 knc6     (54782) 642div   (36677)        0 2024-03-31 13:46:31.000000 jarvis-tools-2024.4.10/jarvis/tests/testfiles/analysis/elastic/__init__.py
--rw-r--r--   0 knc6     (54782) 642div   (36677)     2577 2024-03-31 13:46:31.000000 jarvis-tools-2024.4.10/jarvis/tests/testfiles/analysis/elastic/test_tensor.py
-drwxr-xr-x   0 knc6     (54782) 642div   (36677)        0 2024-04-14 14:32:21.264311 jarvis-tools-2024.4.10/jarvis/tests/testfiles/analysis/interface/
--rw-r--r--   0 knc6     (54782) 642div   (36677)        0 2024-03-31 13:46:31.000000 jarvis-tools-2024.4.10/jarvis/tests/testfiles/analysis/interface/__init__.py
--rw-r--r--   0 knc6     (54782) 642div   (36677)     8683 2024-03-31 13:46:31.000000 jarvis-tools-2024.4.10/jarvis/tests/testfiles/analysis/interface/test_zur.py
-drwxr-xr-x   0 knc6     (54782) 642div   (36677)        0 2024-04-14 14:32:21.296311 jarvis-tools-2024.4.10/jarvis/tests/testfiles/analysis/magnetism/
--rw-r--r--   0 knc6     (54782) 642div   (36677)        0 2024-03-31 13:46:31.000000 jarvis-tools-2024.4.10/jarvis/tests/testfiles/analysis/magnetism/__init__.py
--rw-r--r--   0 knc6     (54782) 642div   (36677)      589 2024-03-31 13:46:31.000000 jarvis-tools-2024.4.10/jarvis/tests/testfiles/analysis/magnetism/test_magnetism.py
-drwxr-xr-x   0 knc6     (54782) 642div   (36677)        0 2024-04-14 14:32:21.336311 jarvis-tools-2024.4.10/jarvis/tests/testfiles/analysis/phonon/
--rw-r--r--   0 knc6     (54782) 642div   (36677)        0 2024-03-31 13:46:31.000000 jarvis-tools-2024.4.10/jarvis/tests/testfiles/analysis/phonon/__init__.py
--rw-r--r--   0 knc6     (54782) 642div   (36677)     5121 2024-03-31 13:46:31.000000 jarvis-tools-2024.4.10/jarvis/tests/testfiles/analysis/phonon/test_dos.py
--rw-r--r--   0 knc6     (54782) 642div   (36677)      326 2024-03-31 13:46:31.000000 jarvis-tools-2024.4.10/jarvis/tests/testfiles/analysis/phonon/test_fc.py
--rw-r--r--   0 knc6     (54782) 642div   (36677)     1279 2024-03-31 13:46:31.000000 jarvis-tools-2024.4.10/jarvis/tests/testfiles/analysis/phonon/test_ir.py
-drwxr-xr-x   0 knc6     (54782) 642div   (36677)        0 2024-04-14 14:32:21.372310 jarvis-tools-2024.4.10/jarvis/tests/testfiles/analysis/solar/
--rw-r--r--   0 knc6     (54782) 642div   (36677)        0 2024-03-31 13:46:31.000000 jarvis-tools-2024.4.10/jarvis/tests/testfiles/analysis/solar/__init__.py
--rw-r--r--   0 knc6     (54782) 642div   (36677)     1399 2024-03-31 13:46:31.000000 jarvis-tools-2024.4.10/jarvis/tests/testfiles/analysis/solar/test_solar.py
-drwxr-xr-x   0 knc6     (54782) 642div   (36677)        0 2024-04-14 14:32:21.380310 jarvis-tools-2024.4.10/jarvis/tests/testfiles/analysis/stm/
--rw-r--r--   0 knc6     (54782) 642div   (36677)        0 2024-03-31 13:46:31.000000 jarvis-tools-2024.4.10/jarvis/tests/testfiles/analysis/stm/__init__.py
--rw-r--r--   0 knc6     (54782) 642div   (36677)     1672 2024-03-31 13:46:31.000000 jarvis-tools-2024.4.10/jarvis/tests/testfiles/analysis/stm/test_stm.py
-drwxr-xr-x   0 knc6     (54782) 642div   (36677)        0 2024-04-14 14:32:21.396310 jarvis-tools-2024.4.10/jarvis/tests/testfiles/analysis/structure/
--rw-r--r--   0 knc6     (54782) 642div   (36677)        0 2024-03-31 13:46:31.000000 jarvis-tools-2024.4.10/jarvis/tests/testfiles/analysis/structure/__init__.py
--rw-r--r--   0 knc6     (54782) 642div   (36677)      390 2024-03-31 13:46:31.000000 jarvis-tools-2024.4.10/jarvis/tests/testfiles/analysis/structure/test_energetics.py
--rw-r--r--   0 knc6     (54782) 642div   (36677)     1301 2024-03-31 13:46:31.000000 jarvis-tools-2024.4.10/jarvis/tests/testfiles/analysis/structure/test_neighbors.py
--rw-r--r--   0 knc6     (54782) 642div   (36677)     3585 2024-03-31 13:46:31.000000 jarvis-tools-2024.4.10/jarvis/tests/testfiles/analysis/structure/test_spacegroup.py
-drwxr-xr-x   0 knc6     (54782) 642div   (36677)        0 2024-04-14 14:32:21.408310 jarvis-tools-2024.4.10/jarvis/tests/testfiles/analysis/thermodynamics/
--rw-r--r--   0 knc6     (54782) 642div   (36677)        0 2024-03-31 13:46:31.000000 jarvis-tools-2024.4.10/jarvis/tests/testfiles/analysis/thermodynamics/__init__.py
--rw-r--r--   0 knc6     (54782) 642div   (36677)     1554 2024-03-31 13:46:31.000000 jarvis-tools-2024.4.10/jarvis/tests/testfiles/analysis/thermodynamics/test_energetics.py
-drwxr-xr-x   0 knc6     (54782) 642div   (36677)        0 2024-04-14 14:32:21.428310 jarvis-tools-2024.4.10/jarvis/tests/testfiles/analysis/topological/
--rw-r--r--   0 knc6     (54782) 642div   (36677)        0 2024-03-31 13:46:31.000000 jarvis-tools-2024.4.10/jarvis/tests/testfiles/analysis/topological/__init__.py
--rw-r--r--   0 knc6     (54782) 642div   (36677)      424 2024-03-31 13:46:31.000000 jarvis-tools-2024.4.10/jarvis/tests/testfiles/analysis/topological/test_spillage.py
-drwxr-xr-x   0 knc6     (54782) 642div   (36677)        0 2024-04-14 14:32:21.612309 jarvis-tools-2024.4.10/jarvis/tests/testfiles/core/
--rw-r--r--   0 knc6     (54782) 642div   (36677)        0 2024-03-31 13:46:32.000000 jarvis-tools-2024.4.10/jarvis/tests/testfiles/core/__init__.py
--rw-r--r--   0 knc6     (54782) 642div   (36677)     5666 2024-03-31 13:46:32.000000 jarvis-tools-2024.4.10/jarvis/tests/testfiles/core/p.py
--rw-r--r--   0 knc6     (54782) 642div   (36677)     6750 2024-04-14 12:36:23.000000 jarvis-tools-2024.4.10/jarvis/tests/testfiles/core/test_atoms.py
--rw-r--r--   0 knc6     (54782) 642div   (36677)      262 2024-03-31 13:46:32.000000 jarvis-tools-2024.4.10/jarvis/tests/testfiles/core/test_circuits.py
--rw-r--r--   0 knc6     (54782) 642div   (36677)      481 2024-03-31 13:46:32.000000 jarvis-tools-2024.4.10/jarvis/tests/testfiles/core/test_composition.py
--rw-r--r--   0 knc6     (54782) 642div   (36677)     2844 2024-03-31 13:46:32.000000 jarvis-tools-2024.4.10/jarvis/tests/testfiles/core/test_graph.py
--rw-r--r--   0 knc6     (54782) 642div   (36677)    11116 2024-03-31 13:46:32.000000 jarvis-tools-2024.4.10/jarvis/tests/testfiles/core/test_kpoints.py
--rw-r--r--   0 knc6     (54782) 642div   (36677)     1507 2024-03-31 13:46:32.000000 jarvis-tools-2024.4.10/jarvis/tests/testfiles/core/test_latice.py
--rw-r--r--   0 knc6     (54782) 642div   (36677)      339 2024-03-31 13:46:32.000000 jarvis-tools-2024.4.10/jarvis/tests/testfiles/core/test_pdb.py
--rw-r--r--   0 knc6     (54782) 642div   (36677)      551 2024-03-31 13:46:32.000000 jarvis-tools-2024.4.10/jarvis/tests/testfiles/core/test_specie.py
--rw-r--r--   0 knc6     (54782) 642div   (36677)      541 2024-03-31 13:46:32.000000 jarvis-tools-2024.4.10/jarvis/tests/testfiles/core/test_utils.py
-drwxr-xr-x   0 knc6     (54782) 642div   (36677)        0 2024-04-14 14:32:21.644309 jarvis-tools-2024.4.10/jarvis/tests/testfiles/db/
--rw-r--r--   0 knc6     (54782) 642div   (36677)        0 2024-03-31 13:46:32.000000 jarvis-tools-2024.4.10/jarvis/tests/testfiles/db/__init__.py
--rw-r--r--   0 knc6     (54782) 642div   (36677)     1496 2024-03-31 13:46:32.000000 jarvis-tools-2024.4.10/jarvis/tests/testfiles/db/test_figshare.py
--rw-r--r--   0 knc6     (54782) 642div   (36677)      154 2024-03-31 16:20:05.000000 jarvis-tools-2024.4.10/jarvis/tests/testfiles/db/test_restapi.py
-drwxr-xr-x   0 knc6     (54782) 642div   (36677)        0 2024-04-14 14:32:21.700308 jarvis-tools-2024.4.10/jarvis/tests/testfiles/tasks/
--rw-r--r--   0 knc6     (54782) 642div   (36677)        0 2024-03-31 13:46:33.000000 jarvis-tools-2024.4.10/jarvis/tests/testfiles/tasks/__init__.py
--rw-r--r--   0 knc6     (54782) 642div   (36677)      804 2024-03-31 13:46:33.000000 jarvis-tools-2024.4.10/jarvis/tests/testfiles/tasks/test_lammps.py
--rw-r--r--   0 knc6     (54782) 642div   (36677)      696 2024-03-31 13:46:33.000000 jarvis-tools-2024.4.10/jarvis/tests/testfiles/tasks/test_vasp.py
-drwxr-xr-x   0 knc6     (54782) 642div   (36677)        0 2024-04-14 14:32:21.728308 jarvis-tools-2024.4.10/jarvis_tools.egg-info/
--rw-r--r--   0 knc6     (54782) 642div   (36677)     3442 2024-04-14 14:32:17.000000 jarvis-tools-2024.4.10/jarvis_tools.egg-info/PKG-INFO
--rw-r--r--   0 knc6     (54782) 642div   (36677)     7607 2024-04-14 14:32:17.000000 jarvis-tools-2024.4.10/jarvis_tools.egg-info/SOURCES.txt
--rw-r--r--   0 knc6     (54782) 642div   (36677)        1 2024-04-14 14:32:17.000000 jarvis-tools-2024.4.10/jarvis_tools.egg-info/dependency_links.txt
--rw-r--r--   0 knc6     (54782) 642div   (36677)      265 2024-04-14 14:32:17.000000 jarvis-tools-2024.4.10/jarvis_tools.egg-info/requires.txt
--rw-r--r--   0 knc6     (54782) 642div   (36677)        7 2024-04-14 14:32:17.000000 jarvis-tools-2024.4.10/jarvis_tools.egg-info/top_level.txt
--rw-r--r--   0 knc6     (54782) 642div   (36677)      195 2024-04-14 14:32:21.744308 jarvis-tools-2024.4.10/setup.cfg
--rw-r--r--   0 knc6     (54782) 642div   (36677)     2649 2024-04-14 12:40:04.000000 jarvis-tools-2024.4.10/setup.py
+drwxr-xr-x   0 knc6     (54782) 642div   (36677)        0 2024-05-04 16:07:18.399181 jarvis_tools-2024.4.20/
+-rw-r--r--   0 knc6     (54782) 642div   (36677)     1878 2024-05-04 16:06:51.000000 jarvis_tools-2024.4.20/LICENSE.rst
+-rw-r--r--   0 knc6     (54782) 642div   (36677)     3442 2024-05-04 16:07:18.399181 jarvis_tools-2024.4.20/PKG-INFO
+-rw-r--r--   0 knc6     (54782) 642div   (36677)    14481 2024-05-04 16:06:51.000000 jarvis_tools-2024.4.20/README.rst
+drwxr-xr-x   0 knc6     (54782) 642div   (36677)        0 2024-05-04 16:07:17.747185 jarvis_tools-2024.4.20/jarvis/
+-rw-r--r--   0 knc6     (54782) 642div   (36677)      245 2024-05-04 16:07:08.000000 jarvis_tools-2024.4.20/jarvis/__init__.py
+drwxr-xr-x   0 knc6     (54782) 642div   (36677)        0 2024-05-04 16:07:17.751185 jarvis_tools-2024.4.20/jarvis/ai/
+-rw-r--r--   0 knc6     (54782) 642div   (36677)       35 2024-05-04 16:06:51.000000 jarvis_tools-2024.4.20/jarvis/ai/__init__.py
+drwxr-xr-x   0 knc6     (54782) 642div   (36677)        0 2024-05-04 16:07:17.763185 jarvis_tools-2024.4.20/jarvis/ai/descriptors/
+-rw-r--r--   0 knc6     (54782) 642div   (36677)       48 2024-05-04 16:06:51.000000 jarvis_tools-2024.4.20/jarvis/ai/descriptors/__init__.py
+-rw-r--r--   0 knc6     (54782) 642div   (36677)    48400 2024-05-04 16:06:51.000000 jarvis_tools-2024.4.20/jarvis/ai/descriptors/cfid.py
+-rw-r--r--   0 knc6     (54782) 642div   (36677)     1370 2024-05-04 16:06:51.000000 jarvis_tools-2024.4.20/jarvis/ai/descriptors/coulomb.py
+-rw-r--r--   0 knc6     (54782) 642div   (36677)      511 2024-05-04 16:06:51.000000 jarvis_tools-2024.4.20/jarvis/ai/descriptors/elemental.py
+drwxr-xr-x   0 knc6     (54782) 642div   (36677)        0 2024-05-04 16:07:17.767185 jarvis_tools-2024.4.20/jarvis/ai/gcn/
+-rw-r--r--   0 knc6     (54782) 642div   (36677)       47 2024-05-04 16:06:51.000000 jarvis_tools-2024.4.20/jarvis/ai/gcn/__init__.py
+drwxr-xr-x   0 knc6     (54782) 642div   (36677)        0 2024-05-04 16:07:17.775185 jarvis_tools-2024.4.20/jarvis/ai/pkgs/
+-rw-r--r--   0 knc6     (54782) 642div   (36677)       35 2024-05-04 16:06:51.000000 jarvis_tools-2024.4.20/jarvis/ai/pkgs/__init__.py
+drwxr-xr-x   0 knc6     (54782) 642div   (36677)        0 2024-05-04 16:07:17.783185 jarvis_tools-2024.4.20/jarvis/ai/pkgs/lgbm/
+-rw-r--r--   0 knc6     (54782) 642div   (36677)       28 2024-05-04 16:06:51.000000 jarvis_tools-2024.4.20/jarvis/ai/pkgs/lgbm/__init__.py
+-rw-r--r--   0 knc6     (54782) 642div   (36677)     1148 2024-05-04 16:06:51.000000 jarvis_tools-2024.4.20/jarvis/ai/pkgs/lgbm/classification.py
+-rw-r--r--   0 knc6     (54782) 642div   (36677)     9541 2024-05-04 16:06:51.000000 jarvis_tools-2024.4.20/jarvis/ai/pkgs/lgbm/regression.py
+drwxr-xr-x   0 knc6     (54782) 642div   (36677)        0 2024-05-04 16:07:17.795185 jarvis_tools-2024.4.20/jarvis/ai/pkgs/sklearn/
+-rw-r--r--   0 knc6     (54782) 642div   (36677)       44 2024-05-04 16:06:51.000000 jarvis_tools-2024.4.20/jarvis/ai/pkgs/sklearn/__init__.py
+-rw-r--r--   0 knc6     (54782) 642div   (36677)     5144 2024-05-04 16:06:51.000000 jarvis_tools-2024.4.20/jarvis/ai/pkgs/sklearn/classification.py
+-rw-r--r--   0 knc6     (54782) 642div   (36677)    11368 2024-05-04 16:06:51.000000 jarvis_tools-2024.4.20/jarvis/ai/pkgs/sklearn/hyper_params.py
+-rw-r--r--   0 knc6     (54782) 642div   (36677)     2969 2024-05-04 16:06:51.000000 jarvis_tools-2024.4.20/jarvis/ai/pkgs/sklearn/regression.py
+-rw-r--r--   0 knc6     (54782) 642div   (36677)     3585 2024-05-04 16:06:51.000000 jarvis_tools-2024.4.20/jarvis/ai/pkgs/utils.py
+drwxr-xr-x   0 knc6     (54782) 642div   (36677)        0 2024-05-04 16:07:17.803185 jarvis_tools-2024.4.20/jarvis/ai/uncertainty/
+-rw-r--r--   0 knc6     (54782) 642div   (36677)       34 2024-05-04 16:06:51.000000 jarvis_tools-2024.4.20/jarvis/ai/uncertainty/__init__.py
+-rw-r--r--   0 knc6     (54782) 642div   (36677)     5573 2024-05-04 16:06:51.000000 jarvis_tools-2024.4.20/jarvis/ai/uncertainty/gaussian_process_uncertainty.py
+-rw-r--r--   0 knc6     (54782) 642div   (36677)     7534 2024-05-04 16:06:51.000000 jarvis_tools-2024.4.20/jarvis/ai/uncertainty/lgbm_quantile_uncertainty.py
+drwxr-xr-x   0 knc6     (54782) 642div   (36677)        0 2024-05-04 16:07:17.807185 jarvis_tools-2024.4.20/jarvis/analysis/
+-rw-r--r--   0 knc6     (54782) 642div   (36677)       35 2024-05-04 16:06:51.000000 jarvis_tools-2024.4.20/jarvis/analysis/__init__.py
+drwxr-xr-x   0 knc6     (54782) 642div   (36677)        0 2024-05-04 16:07:17.811185 jarvis_tools-2024.4.20/jarvis/analysis/darkmatter/
+-rw-r--r--   0 knc6     (54782) 642div   (36677)       51 2024-05-04 16:06:51.000000 jarvis_tools-2024.4.20/jarvis/analysis/darkmatter/__init__.py
+-rw-r--r--   0 knc6     (54782) 642div   (36677)      786 2024-05-04 16:06:51.000000 jarvis_tools-2024.4.20/jarvis/analysis/darkmatter/metrics.py
+drwxr-xr-x   0 knc6     (54782) 642div   (36677)        0 2024-05-04 16:07:17.823185 jarvis_tools-2024.4.20/jarvis/analysis/defects/
+-rw-r--r--   0 knc6     (54782) 642div   (36677)       47 2024-05-04 16:06:51.000000 jarvis_tools-2024.4.20/jarvis/analysis/defects/__init__.py
+-rw-r--r--   0 knc6     (54782) 642div   (36677)     2328 2024-05-04 16:06:51.000000 jarvis_tools-2024.4.20/jarvis/analysis/defects/substitutions.py
+-rw-r--r--   0 knc6     (54782) 642div   (36677)    10069 2024-05-04 16:07:08.000000 jarvis_tools-2024.4.20/jarvis/analysis/defects/surface.py
+-rw-r--r--   0 knc6     (54782) 642div   (36677)     5048 2024-05-04 16:06:51.000000 jarvis_tools-2024.4.20/jarvis/analysis/defects/vacancy.py
+drwxr-xr-x   0 knc6     (54782) 642div   (36677)        0 2024-05-04 16:07:17.831184 jarvis_tools-2024.4.20/jarvis/analysis/diffraction/
+-rw-r--r--   0 knc6     (54782) 642div   (36677)       49 2024-05-04 16:06:51.000000 jarvis_tools-2024.4.20/jarvis/analysis/diffraction/__init__.py
+-rw-r--r--   0 knc6     (54782) 642div   (36677)     6825 2024-05-04 16:06:51.000000 jarvis_tools-2024.4.20/jarvis/analysis/diffraction/atomic_scattering_params.json
+-rw-r--r--   0 knc6     (54782) 642div   (36677)     7327 2024-05-04 16:06:51.000000 jarvis_tools-2024.4.20/jarvis/analysis/diffraction/xrd.py
+drwxr-xr-x   0 knc6     (54782) 642div   (36677)        0 2024-05-04 16:07:17.839185 jarvis_tools-2024.4.20/jarvis/analysis/elastic/
+-rw-r--r--   0 knc6     (54782) 642div   (36677)       43 2024-05-04 16:06:51.000000 jarvis_tools-2024.4.20/jarvis/analysis/elastic/__init__.py
+-rw-r--r--   0 knc6     (54782) 642div   (36677)     6602 2024-05-04 16:06:51.000000 jarvis_tools-2024.4.20/jarvis/analysis/elastic/tensor.py
+drwxr-xr-x   0 knc6     (54782) 642div   (36677)        0 2024-05-04 16:07:17.843185 jarvis_tools-2024.4.20/jarvis/analysis/interface/
+-rw-r--r--   0 knc6     (54782) 642div   (36677)       53 2024-05-04 16:06:51.000000 jarvis_tools-2024.4.20/jarvis/analysis/interface/__init__.py
+-rw-r--r--   0 knc6     (54782) 642div   (36677)    14764 2024-05-04 16:06:51.000000 jarvis_tools-2024.4.20/jarvis/analysis/interface/zur.py
+drwxr-xr-x   0 knc6     (54782) 642div   (36677)        0 2024-05-04 16:07:17.847185 jarvis_tools-2024.4.20/jarvis/analysis/magnetism/
+-rw-r--r--   0 knc6     (54782) 642div   (36677)       46 2024-05-04 16:06:51.000000 jarvis_tools-2024.4.20/jarvis/analysis/magnetism/__init__.py
+-rw-r--r--   0 knc6     (54782) 642div   (36677)     8101 2024-05-04 16:06:51.000000 jarvis_tools-2024.4.20/jarvis/analysis/magnetism/magmom_setup.py
+drwxr-xr-x   0 knc6     (54782) 642div   (36677)        0 2024-05-04 16:07:17.855184 jarvis_tools-2024.4.20/jarvis/analysis/periodic/
+-rw-r--r--   0 knc6     (54782) 642div   (36677)       49 2024-05-04 16:06:51.000000 jarvis_tools-2024.4.20/jarvis/analysis/periodic/__init__.py
+-rw-r--r--   0 knc6     (54782) 642div   (36677)     5907 2024-05-04 16:06:51.000000 jarvis_tools-2024.4.20/jarvis/analysis/periodic/ptable.py
+drwxr-xr-x   0 knc6     (54782) 642div   (36677)        0 2024-05-04 16:07:17.867184 jarvis_tools-2024.4.20/jarvis/analysis/phonon/
+-rw-r--r--   0 knc6     (54782) 642div   (36677)       49 2024-05-04 16:06:51.000000 jarvis_tools-2024.4.20/jarvis/analysis/phonon/__init__.py
+-rw-r--r--   0 knc6     (54782) 642div   (36677)     3934 2024-05-04 16:06:51.000000 jarvis_tools-2024.4.20/jarvis/analysis/phonon/dos.py
+-rw-r--r--   0 knc6     (54782) 642div   (36677)     1189 2024-05-04 16:06:51.000000 jarvis_tools-2024.4.20/jarvis/analysis/phonon/force_constants.py
+-rw-r--r--   0 knc6     (54782) 642div   (36677)     6473 2024-05-04 16:06:51.000000 jarvis_tools-2024.4.20/jarvis/analysis/phonon/ir.py
+drwxr-xr-x   0 knc6     (54782) 642div   (36677)        0 2024-05-04 16:07:17.875184 jarvis_tools-2024.4.20/jarvis/analysis/solarefficiency/
+-rw-r--r--   0 knc6     (54782) 642div   (36677)       59 2024-05-04 16:06:51.000000 jarvis_tools-2024.4.20/jarvis/analysis/solarefficiency/__init__.py
+-rw-r--r--   0 knc6     (54782) 642div   (36677)    35436 2024-05-04 16:06:51.000000 jarvis_tools-2024.4.20/jarvis/analysis/solarefficiency/am1.5G.dat
+-rw-r--r--   0 knc6     (54782) 642div   (36677)    14217 2024-05-04 16:06:51.000000 jarvis_tools-2024.4.20/jarvis/analysis/solarefficiency/solar.py
+drwxr-xr-x   0 knc6     (54782) 642div   (36677)        0 2024-05-04 16:07:17.879184 jarvis_tools-2024.4.20/jarvis/analysis/stem/
+-rw-r--r--   0 knc6     (54782) 642div   (36677)       38 2024-05-04 16:06:51.000000 jarvis_tools-2024.4.20/jarvis/analysis/stem/__init__.py
+-rw-r--r--   0 knc6     (54782) 642div   (36677)     7315 2024-05-04 16:06:51.000000 jarvis_tools-2024.4.20/jarvis/analysis/stem/convolution_apprx.py
+drwxr-xr-x   0 knc6     (54782) 642div   (36677)        0 2024-05-04 16:07:17.887184 jarvis_tools-2024.4.20/jarvis/analysis/stm/
+-rw-r--r--   0 knc6     (54782) 642div   (36677)       67 2024-05-04 16:06:51.000000 jarvis_tools-2024.4.20/jarvis/analysis/stm/__init__.py
+-rw-r--r--   0 knc6     (54782) 642div   (36677)    10094 2024-05-04 16:06:51.000000 jarvis_tools-2024.4.20/jarvis/analysis/stm/tersoff_hamann.py
+drwxr-xr-x   0 knc6     (54782) 642div   (36677)        0 2024-05-04 16:07:17.895184 jarvis_tools-2024.4.20/jarvis/analysis/structure/
+-rw-r--r--   0 knc6     (54782) 642div   (36677)       46 2024-05-04 16:06:51.000000 jarvis_tools-2024.4.20/jarvis/analysis/structure/__init__.py
+-rw-r--r--   0 knc6     (54782) 642div   (36677)    21798 2024-05-04 16:06:51.000000 jarvis_tools-2024.4.20/jarvis/analysis/structure/neighbors.py
+-rw-r--r--   0 knc6     (54782) 642div   (36677)    25663 2024-05-04 16:06:51.000000 jarvis_tools-2024.4.20/jarvis/analysis/structure/spacegroup.py
+drwxr-xr-x   0 knc6     (54782) 642div   (36677)        0 2024-05-04 16:07:17.911184 jarvis_tools-2024.4.20/jarvis/analysis/thermodynamics/
+-rw-r--r--   0 knc6     (54782) 642div   (36677)       42 2024-05-04 16:06:51.000000 jarvis_tools-2024.4.20/jarvis/analysis/thermodynamics/__init__.py
+-rw-r--r--   0 knc6     (54782) 642div   (36677)    14613 2024-05-04 16:06:51.000000 jarvis_tools-2024.4.20/jarvis/analysis/thermodynamics/energetics.py
+-rw-r--r--   0 knc6     (54782) 642div   (36677)     4527 2024-05-04 16:06:51.000000 jarvis_tools-2024.4.20/jarvis/analysis/thermodynamics/unary.json
+-rw-r--r--   0 knc6     (54782) 642div   (36677)     4781 2024-05-04 16:06:51.000000 jarvis_tools-2024.4.20/jarvis/analysis/thermodynamics/unary_qe_tb.json
+drwxr-xr-x   0 knc6     (54782) 642div   (36677)        0 2024-05-04 16:07:17.915184 jarvis_tools-2024.4.20/jarvis/analysis/topological/
+-rw-r--r--   0 knc6     (54782) 642div   (36677)       50 2024-05-04 16:06:51.000000 jarvis_tools-2024.4.20/jarvis/analysis/topological/__init__.py
+-rw-r--r--   0 knc6     (54782) 642div   (36677)    11892 2024-05-04 16:06:51.000000 jarvis_tools-2024.4.20/jarvis/analysis/topological/spillage.py
+drwxr-xr-x   0 knc6     (54782) 642div   (36677)        0 2024-05-04 16:07:17.991184 jarvis_tools-2024.4.20/jarvis/core/
+-rw-r--r--   0 knc6     (54782) 642div   (36677)  1421253 2024-05-04 16:06:51.000000 jarvis_tools-2024.4.20/jarvis/core/Elements.json
+-rw-r--r--   0 knc6     (54782) 642div   (36677)       49 2024-05-04 16:06:51.000000 jarvis_tools-2024.4.20/jarvis/core/__init__.py
+-rw-r--r--   0 knc6     (54782) 642div   (36677)    28393 2024-05-04 16:06:51.000000 jarvis_tools-2024.4.20/jarvis/core/atom_init.json
+-rw-r--r--   0 knc6     (54782) 642div   (36677)    81850 2024-05-04 16:07:08.000000 jarvis_tools-2024.4.20/jarvis/core/atoms.py
+-rw-r--r--   0 knc6     (54782) 642div   (36677)     4313 2024-05-04 16:06:51.000000 jarvis_tools-2024.4.20/jarvis/core/circuits.py
+-rw-r--r--   0 knc6     (54782) 642div   (36677)     6161 2024-05-04 16:07:08.000000 jarvis_tools-2024.4.20/jarvis/core/composition.py
+-rw-r--r--   0 knc6     (54782) 642div   (36677)  1162701 2024-05-04 16:06:51.000000 jarvis_tools-2024.4.20/jarvis/core/element_charge.json
+-rw-r--r--   0 knc6     (54782) 642div   (36677)    22713 2024-05-04 16:06:51.000000 jarvis_tools-2024.4.20/jarvis/core/graphs.py
+-rw-r--r--   0 knc6     (54782) 642div   (36677)    10693 2024-05-04 16:06:51.000000 jarvis_tools-2024.4.20/jarvis/core/image.py
+-rw-r--r--   0 knc6     (54782) 642div   (36677)    37783 2024-05-04 16:06:51.000000 jarvis_tools-2024.4.20/jarvis/core/kpoints.py
+-rw-r--r--   0 knc6     (54782) 642div   (36677)    17427 2024-05-04 16:06:51.000000 jarvis_tools-2024.4.20/jarvis/core/lattice.py
+-rw-r--r--   0 knc6     (54782) 642div   (36677)    47766 2024-05-04 16:06:51.000000 jarvis_tools-2024.4.20/jarvis/core/magpie.json
+-rw-r--r--   0 knc6     (54782) 642div   (36677)  3215996 2024-05-04 16:07:08.000000 jarvis_tools-2024.4.20/jarvis/core/mineral_name_prototype.json.zip
+-rw-r--r--   0 knc6     (54782) 642div   (36677)    12121 2024-05-04 16:06:51.000000 jarvis_tools-2024.4.20/jarvis/core/specie.py
+-rw-r--r--   0 knc6     (54782) 642div   (36677)     2891 2024-05-04 16:06:51.000000 jarvis_tools-2024.4.20/jarvis/core/spectrum.py
+-rw-r--r--   0 knc6     (54782) 642div   (36677)     8925 2024-05-04 16:07:08.000000 jarvis_tools-2024.4.20/jarvis/core/utils.py
+drwxr-xr-x   0 knc6     (54782) 642div   (36677)        0 2024-05-04 16:07:18.015184 jarvis_tools-2024.4.20/jarvis/db/
+-rw-r--r--   0 knc6     (54782) 642div   (36677)       53 2024-05-04 16:06:51.000000 jarvis_tools-2024.4.20/jarvis/db/__init__.py
+-rw-r--r--   0 knc6     (54782) 642div   (36677)    26622 2024-05-04 16:06:51.000000 jarvis_tools-2024.4.20/jarvis/db/figshare.py
+-rw-r--r--   0 knc6     (54782) 642div   (36677)      378 2024-05-04 16:06:51.000000 jarvis_tools-2024.4.20/jarvis/db/jsonutils.py
+-rw-r--r--   0 knc6     (54782) 642div   (36677)     7761 2024-05-04 16:06:51.000000 jarvis_tools-2024.4.20/jarvis/db/lammps_to_xml.py
+-rw-r--r--   0 knc6     (54782) 642div   (36677)    10649 2024-05-04 16:06:51.000000 jarvis_tools-2024.4.20/jarvis/db/qe_to_xml.py
+-rw-r--r--   0 knc6     (54782) 642div   (36677)    17359 2024-05-04 16:06:51.000000 jarvis_tools-2024.4.20/jarvis/db/restapi.py
+-rw-r--r--   0 knc6     (54782) 642div   (36677)    75218 2024-05-04 16:06:51.000000 jarvis_tools-2024.4.20/jarvis/db/vasp_to_xml.py
+-rw-r--r--   0 knc6     (54782) 642div   (36677)     9586 2024-05-04 16:06:51.000000 jarvis_tools-2024.4.20/jarvis/db/webpages.py
+drwxr-xr-x   0 knc6     (54782) 642div   (36677)        0 2024-05-04 16:07:18.019183 jarvis_tools-2024.4.20/jarvis/io/
+-rw-r--r--   0 knc6     (54782) 642div   (36677)       76 2024-05-04 16:06:51.000000 jarvis_tools-2024.4.20/jarvis/io/__init__.py
+drwxr-xr-x   0 knc6     (54782) 642div   (36677)        0 2024-05-04 16:07:18.027183 jarvis_tools-2024.4.20/jarvis/io/boltztrap/
+-rw-r--r--   0 knc6     (54782) 642div   (36677)       67 2024-05-04 16:06:51.000000 jarvis_tools-2024.4.20/jarvis/io/boltztrap/__init__.py
+-rw-r--r--   0 knc6     (54782) 642div   (36677)     6511 2024-05-04 16:06:51.000000 jarvis_tools-2024.4.20/jarvis/io/boltztrap/inputs.py
+-rw-r--r--   0 knc6     (54782) 642div   (36677)     6767 2024-05-04 16:06:51.000000 jarvis_tools-2024.4.20/jarvis/io/boltztrap/outputs.py
+drwxr-xr-x   0 knc6     (54782) 642div   (36677)        0 2024-05-04 16:07:18.031183 jarvis_tools-2024.4.20/jarvis/io/calphad/
+-rw-r--r--   0 knc6     (54782) 642div   (36677)       61 2024-05-04 16:06:51.000000 jarvis_tools-2024.4.20/jarvis/io/calphad/__init__.py
+-rw-r--r--   0 knc6     (54782) 642div   (36677)     4228 2024-05-04 16:06:51.000000 jarvis_tools-2024.4.20/jarvis/io/calphad/write_decorated_poscar.py
+drwxr-xr-x   0 knc6     (54782) 642div   (36677)        0 2024-05-04 16:07:18.043183 jarvis_tools-2024.4.20/jarvis/io/lammps/
+-rw-r--r--   0 knc6     (54782) 642div   (36677)       52 2024-05-04 16:06:51.000000 jarvis_tools-2024.4.20/jarvis/io/lammps/__init__.py
+-rw-r--r--   0 knc6     (54782) 642div   (36677)    14615 2024-05-04 16:06:51.000000 jarvis_tools-2024.4.20/jarvis/io/lammps/inputs.py
+-rw-r--r--   0 knc6     (54782) 642div   (36677)    20760 2024-05-04 16:06:51.000000 jarvis_tools-2024.4.20/jarvis/io/lammps/outputs.py
+drwxr-xr-x   0 knc6     (54782) 642div   (36677)        0 2024-05-04 16:07:18.051183 jarvis_tools-2024.4.20/jarvis/io/nexus/
+-rw-r--r--   0 knc6     (54782) 642div   (36677)       47 2024-05-04 16:06:51.000000 jarvis_tools-2024.4.20/jarvis/io/nexus/__init__.py
+-rw-r--r--   0 knc6     (54782) 642div   (36677)     4519 2024-05-04 16:06:51.000000 jarvis_tools-2024.4.20/jarvis/io/nexus/inputs.py
+-rw-r--r--   0 knc6     (54782) 642div   (36677)       36 2024-05-04 16:06:51.000000 jarvis_tools-2024.4.20/jarvis/io/nexus/outputs.py
+drwxr-xr-x   0 knc6     (54782) 642div   (36677)        0 2024-05-04 16:07:18.059183 jarvis_tools-2024.4.20/jarvis/io/pennylane/
+-rw-r--r--   0 knc6     (54782) 642div   (36677)       61 2024-05-04 16:06:51.000000 jarvis_tools-2024.4.20/jarvis/io/pennylane/__init__.py
+-rw-r--r--   0 knc6     (54782) 642div   (36677)     2196 2024-05-04 16:06:51.000000 jarvis_tools-2024.4.20/jarvis/io/pennylane/inputs.py
+drwxr-xr-x   0 knc6     (54782) 642div   (36677)        0 2024-05-04 16:07:18.071183 jarvis_tools-2024.4.20/jarvis/io/phonopy/
+-rw-r--r--   0 knc6     (54782) 642div   (36677)       43 2024-05-04 16:06:51.000000 jarvis_tools-2024.4.20/jarvis/io/phonopy/__init__.py
+-rw-r--r--   0 knc6     (54782) 642div   (36677)     4501 2024-05-04 16:06:51.000000 jarvis_tools-2024.4.20/jarvis/io/phonopy/fcmat2hr.py
+-rw-r--r--   0 knc6     (54782) 642div   (36677)     6844 2024-05-04 16:06:51.000000 jarvis_tools-2024.4.20/jarvis/io/phonopy/inputs.py
+-rw-r--r--   0 knc6     (54782) 642div   (36677)     5696 2024-05-04 16:06:51.000000 jarvis_tools-2024.4.20/jarvis/io/phonopy/outputs.py
+drwxr-xr-x   0 knc6     (54782) 642div   (36677)        0 2024-05-04 16:07:18.075183 jarvis_tools-2024.4.20/jarvis/io/prismatic/
+-rw-r--r--   0 knc6     (54782) 642div   (36677)       50 2024-05-04 16:06:51.000000 jarvis_tools-2024.4.20/jarvis/io/prismatic/__init__.py
+-rw-r--r--   0 knc6     (54782) 642div   (36677)      674 2024-05-04 16:06:51.000000 jarvis_tools-2024.4.20/jarvis/io/prismatic/inputs.py
+drwxr-xr-x   0 knc6     (54782) 642div   (36677)        0 2024-05-04 16:07:18.083183 jarvis_tools-2024.4.20/jarvis/io/qe/
+-rw-r--r--   0 knc6     (54782) 642div   (36677)       57 2024-05-04 16:06:51.000000 jarvis_tools-2024.4.20/jarvis/io/qe/__init__.py
+-rw-r--r--   0 knc6     (54782) 642div   (36677)    15329 2024-05-04 16:06:51.000000 jarvis_tools-2024.4.20/jarvis/io/qe/inputs.py
+-rwxr-xr-x   0 knc6     (54782) 642div   (36677)    29549 2024-05-04 16:06:51.000000 jarvis_tools-2024.4.20/jarvis/io/qe/outputs.py
+drwxr-xr-x   0 knc6     (54782) 642div   (36677)        0 2024-05-04 16:07:18.091183 jarvis_tools-2024.4.20/jarvis/io/qiskit/
+-rw-r--r--   0 knc6     (54782) 642div   (36677)       56 2024-05-04 16:06:51.000000 jarvis_tools-2024.4.20/jarvis/io/qiskit/__init__.py
+-rw-r--r--   0 knc6     (54782) 642div   (36677)    12104 2024-05-04 16:06:51.000000 jarvis_tools-2024.4.20/jarvis/io/qiskit/inputs.py
+drwxr-xr-x   0 knc6     (54782) 642div   (36677)        0 2024-05-04 16:07:18.099183 jarvis_tools-2024.4.20/jarvis/io/tequila/
+-rw-r--r--   0 knc6     (54782) 642div   (36677)       60 2024-05-04 16:06:51.000000 jarvis_tools-2024.4.20/jarvis/io/tequila/__init__.py
+-rw-r--r--   0 knc6     (54782) 642div   (36677)     2702 2024-05-04 16:06:51.000000 jarvis_tools-2024.4.20/jarvis/io/tequila/inputs.py
+drwxr-xr-x   0 knc6     (54782) 642div   (36677)        0 2024-05-04 16:07:18.111183 jarvis_tools-2024.4.20/jarvis/io/vasp/
+-rw-r--r--   0 knc6     (54782) 642div   (36677)       56 2024-05-04 16:06:51.000000 jarvis_tools-2024.4.20/jarvis/io/vasp/__init__.py
+-rw-r--r--   0 knc6     (54782) 642div   (36677)     1522 2024-05-04 16:06:51.000000 jarvis_tools-2024.4.20/jarvis/io/vasp/default_potcars.json
+-rw-r--r--   0 knc6     (54782) 642div   (36677)    20248 2024-05-04 16:06:51.000000 jarvis_tools-2024.4.20/jarvis/io/vasp/inputs.py
+-rw-r--r--   0 knc6     (54782) 642div   (36677)    84993 2024-05-04 16:07:08.000000 jarvis_tools-2024.4.20/jarvis/io/vasp/outputs.py
+drwxr-xr-x   0 knc6     (54782) 642div   (36677)        0 2024-05-04 16:07:18.119183 jarvis_tools-2024.4.20/jarvis/io/wannier/
+-rw-r--r--   0 knc6     (54782) 642div   (36677)       61 2024-05-04 16:06:52.000000 jarvis_tools-2024.4.20/jarvis/io/wannier/__init__.py
+-rw-r--r--   0 knc6     (54782) 642div   (36677)     4550 2024-05-04 16:06:52.000000 jarvis_tools-2024.4.20/jarvis/io/wannier/default_semicore.json
+-rw-r--r--   0 knc6     (54782) 642div   (36677)     6929 2024-05-04 16:06:52.000000 jarvis_tools-2024.4.20/jarvis/io/wannier/inputs.py
+-rw-r--r--   0 knc6     (54782) 642div   (36677)    34195 2024-05-04 16:06:52.000000 jarvis_tools-2024.4.20/jarvis/io/wannier/outputs.py
+drwxr-xr-x   0 knc6     (54782) 642div   (36677)        0 2024-05-04 16:07:18.127183 jarvis_tools-2024.4.20/jarvis/io/wanniertools/
+-rw-r--r--   0 knc6     (54782) 642div   (36677)       60 2024-05-04 16:06:52.000000 jarvis_tools-2024.4.20/jarvis/io/wanniertools/__init__.py
+-rw-r--r--   0 knc6     (54782) 642div   (36677)    10376 2024-05-04 16:06:52.000000 jarvis_tools-2024.4.20/jarvis/io/wanniertools/inputs.py
+-rw-r--r--   0 knc6     (54782) 642div   (36677)     3818 2024-05-04 16:06:52.000000 jarvis_tools-2024.4.20/jarvis/io/wanniertools/outputs.py
+drwxr-xr-x   0 knc6     (54782) 642div   (36677)        0 2024-05-04 16:07:18.135183 jarvis_tools-2024.4.20/jarvis/io/wien2k/
+-rw-r--r--   0 knc6     (54782) 642div   (36677)       55 2024-05-04 16:06:52.000000 jarvis_tools-2024.4.20/jarvis/io/wien2k/__init__.py
+-rw-r--r--   0 knc6     (54782) 642div   (36677)     3238 2024-05-04 16:06:52.000000 jarvis_tools-2024.4.20/jarvis/io/wien2k/inputs.py
+-rw-r--r--   0 knc6     (54782) 642div   (36677)     3353 2024-05-04 16:06:52.000000 jarvis_tools-2024.4.20/jarvis/io/wien2k/outputs.py
+drwxr-xr-x   0 knc6     (54782) 642div   (36677)        0 2024-05-04 16:07:18.143183 jarvis_tools-2024.4.20/jarvis/io/zeopp/
+-rw-r--r--   0 knc6     (54782) 642div   (36677)       35 2024-05-04 16:06:52.000000 jarvis_tools-2024.4.20/jarvis/io/zeopp/__init__.py
+-rw-r--r--   0 knc6     (54782) 642div   (36677)     2184 2024-05-04 16:06:52.000000 jarvis_tools-2024.4.20/jarvis/io/zeopp/inputs.py
+drwxr-xr-x   0 knc6     (54782) 642div   (36677)        0 2024-05-04 16:07:18.147183 jarvis_tools-2024.4.20/jarvis/tasks/
+-rw-r--r--   0 knc6     (54782) 642div   (36677)       47 2024-05-04 16:06:52.000000 jarvis_tools-2024.4.20/jarvis/tasks/__init__.py
+drwxr-xr-x   0 knc6     (54782) 642div   (36677)        0 2024-05-04 16:07:18.155183 jarvis_tools-2024.4.20/jarvis/tasks/boltztrap/
+-rw-r--r--   0 knc6     (54782) 642div   (36677)       56 2024-05-04 16:06:52.000000 jarvis_tools-2024.4.20/jarvis/tasks/boltztrap/__init__.py
+-rw-r--r--   0 knc6     (54782) 642div   (36677)      608 2024-05-04 16:06:52.000000 jarvis_tools-2024.4.20/jarvis/tasks/boltztrap/run.py
+drwxr-xr-x   0 knc6     (54782) 642div   (36677)        0 2024-05-04 16:07:18.163183 jarvis_tools-2024.4.20/jarvis/tasks/lammps/
+-rw-r--r--   0 knc6     (54782) 642div   (36677)       55 2024-05-04 16:06:52.000000 jarvis_tools-2024.4.20/jarvis/tasks/lammps/__init__.py
+-rw-r--r--   0 knc6     (54782) 642div   (36677)    14071 2024-05-04 16:06:52.000000 jarvis_tools-2024.4.20/jarvis/tasks/lammps/lammps.py
+drwxr-xr-x   0 knc6     (54782) 642div   (36677)        0 2024-05-04 16:07:18.191182 jarvis_tools-2024.4.20/jarvis/tasks/lammps/templates/
+-rw-r--r--   0 knc6     (54782) 642div   (36677)       47 2024-05-04 16:06:52.000000 jarvis_tools-2024.4.20/jarvis/tasks/lammps/templates/__init__.py
+-rw-r--r--   0 knc6     (54782) 642div   (36677)     3463 2024-05-04 16:06:52.000000 jarvis_tools-2024.4.20/jarvis/tasks/lammps/templates/displace.mod
+-rw-r--r--   0 knc6     (54782) 642div   (36677)     6416 2024-05-04 16:06:52.000000 jarvis_tools-2024.4.20/jarvis/tasks/lammps/templates/inelast.mod
+-rw-r--r--   0 knc6     (54782) 642div   (36677)     6449 2024-05-04 16:06:52.000000 jarvis_tools-2024.4.20/jarvis/tasks/lammps/templates/inelast_min.mod
+-rw-r--r--   0 knc6     (54782) 642div   (36677)     6418 2024-05-04 16:06:52.000000 jarvis_tools-2024.4.20/jarvis/tasks/lammps/templates/inelast_nobox.mod
+-rw-r--r--   0 knc6     (54782) 642div   (36677)     6415 2024-05-04 16:06:52.000000 jarvis_tools-2024.4.20/jarvis/tasks/lammps/templates/inelastcomb.mod
+-rw-r--r--   0 knc6     (54782) 642div   (36677)     6389 2024-05-04 16:06:52.000000 jarvis_tools-2024.4.20/jarvis/tasks/lammps/templates/inelastreax.mod
+-rw-r--r--   0 knc6     (54782) 642div   (36677)     2653 2024-05-04 16:06:52.000000 jarvis_tools-2024.4.20/jarvis/tasks/lammps/templates/relax.mod
+-rw-r--r--   0 knc6     (54782) 642div   (36677)      145 2024-05-04 16:06:52.000000 jarvis_tools-2024.4.20/jarvis/tasks/lammps/templates/run0.mod
+-rw-r--r--   0 knc6     (54782) 642div   (36677)      917 2024-05-04 16:06:52.000000 jarvis_tools-2024.4.20/jarvis/tasks/lammps/templates/templates.py
+drwxr-xr-x   0 knc6     (54782) 642div   (36677)        0 2024-05-04 16:07:18.199182 jarvis_tools-2024.4.20/jarvis/tasks/nexus/
+-rw-r--r--   0 knc6     (54782) 642div   (36677)       34 2024-05-04 16:06:52.000000 jarvis_tools-2024.4.20/jarvis/tasks/nexus/__init__.py
+-rw-r--r--   0 knc6     (54782) 642div   (36677)     3243 2024-05-04 16:06:52.000000 jarvis_tools-2024.4.20/jarvis/tasks/nexus/qmc.py
+drwxr-xr-x   0 knc6     (54782) 642div   (36677)        0 2024-05-04 16:07:18.203182 jarvis_tools-2024.4.20/jarvis/tasks/phonopy/
+-rw-r--r--   0 knc6     (54782) 642div   (36677)       54 2024-05-04 16:06:52.000000 jarvis_tools-2024.4.20/jarvis/tasks/phonopy/__init__.py
+-rw-r--r--   0 knc6     (54782) 642div   (36677)      765 2024-05-04 16:06:52.000000 jarvis_tools-2024.4.20/jarvis/tasks/phonopy/run.py
+drwxr-xr-x   0 knc6     (54782) 642div   (36677)        0 2024-05-04 16:07:18.223182 jarvis_tools-2024.4.20/jarvis/tasks/qe/
+-rw-r--r--   0 knc6     (54782) 642div   (36677)       29 2024-05-04 16:06:52.000000 jarvis_tools-2024.4.20/jarvis/tasks/qe/__init__.py
+-rw-r--r--   0 knc6     (54782) 642div   (36677)    19582 2024-05-04 16:06:52.000000 jarvis_tools-2024.4.20/jarvis/tasks/qe/converg.py
+-rw-r--r--   0 knc6     (54782) 642div   (36677)     3665 2024-05-04 16:06:52.000000 jarvis_tools-2024.4.20/jarvis/tasks/qe/master_super.py
+-rw-r--r--   0 knc6     (54782) 642div   (36677)     4209 2024-05-04 16:06:52.000000 jarvis_tools-2024.4.20/jarvis/tasks/qe/qe.py
+-rw-r--r--   0 knc6     (54782) 642div   (36677)    10626 2024-05-04 16:06:52.000000 jarvis_tools-2024.4.20/jarvis/tasks/qe/super.py
+-rw-r--r--   0 knc6     (54782) 642div   (36677)     7387 2024-05-04 16:06:52.000000 jarvis_tools-2024.4.20/jarvis/tasks/qe/super_tetra.py
+-rw-r--r--   0 knc6     (54782) 642div   (36677)     5873 2024-05-04 16:06:52.000000 jarvis_tools-2024.4.20/jarvis/tasks/queue_jobs.py
+drwxr-xr-x   0 knc6     (54782) 642div   (36677)        0 2024-05-04 16:07:18.227182 jarvis_tools-2024.4.20/jarvis/tasks/vasp/
+-rw-r--r--   0 knc6     (54782) 642div   (36677)       61 2024-05-04 16:06:52.000000 jarvis_tools-2024.4.20/jarvis/tasks/vasp/__init__.py
+-rw-r--r--   0 knc6     (54782) 642div   (36677)    66478 2024-05-04 16:06:52.000000 jarvis_tools-2024.4.20/jarvis/tasks/vasp/vasp.py
+drwxr-xr-x   0 knc6     (54782) 642div   (36677)        0 2024-05-04 16:07:18.231182 jarvis_tools-2024.4.20/jarvis/tests/
+-rw-r--r--   0 knc6     (54782) 642div   (36677)       35 2024-05-04 16:06:52.000000 jarvis_tools-2024.4.20/jarvis/tests/__init__.py
+drwxr-xr-x   0 knc6     (54782) 642div   (36677)        0 2024-05-04 16:07:18.235182 jarvis_tools-2024.4.20/jarvis/tests/testfiles/
+-rw-r--r--   0 knc6     (54782) 642div   (36677)        0 2024-05-04 16:06:52.000000 jarvis_tools-2024.4.20/jarvis/tests/testfiles/__init__.py
+drwxr-xr-x   0 knc6     (54782) 642div   (36677)        0 2024-05-04 16:07:18.243182 jarvis_tools-2024.4.20/jarvis/tests/testfiles/ai/
+-rw-r--r--   0 knc6     (54782) 642div   (36677)        0 2024-05-04 16:06:52.000000 jarvis_tools-2024.4.20/jarvis/tests/testfiles/ai/__init__.py
+-rw-r--r--   0 knc6     (54782) 642div   (36677)      950 2024-05-04 16:06:52.000000 jarvis_tools-2024.4.20/jarvis/tests/testfiles/ai/test_ai_uncertainty.py
+-rw-r--r--   0 knc6     (54782) 642div   (36677)    67390 2024-05-04 16:06:52.000000 jarvis_tools-2024.4.20/jarvis/tests/testfiles/ai/test_desc.py
+-rw-r--r--   0 knc6     (54782) 642div   (36677)     2206 2024-05-04 16:06:52.000000 jarvis_tools-2024.4.20/jarvis/tests/testfiles/ai/test_pkgs.py
+drwxr-xr-x   0 knc6     (54782) 642div   (36677)        0 2024-05-04 16:07:18.247182 jarvis_tools-2024.4.20/jarvis/tests/testfiles/analysis/
+-rw-r--r--   0 knc6     (54782) 642div   (36677)        0 2024-05-04 16:06:52.000000 jarvis_tools-2024.4.20/jarvis/tests/testfiles/analysis/__init__.py
+drwxr-xr-x   0 knc6     (54782) 642div   (36677)        0 2024-05-04 16:07:18.251182 jarvis_tools-2024.4.20/jarvis/tests/testfiles/analysis/darkmatter/
+-rw-r--r--   0 knc6     (54782) 642div   (36677)        0 2024-05-04 16:06:52.000000 jarvis_tools-2024.4.20/jarvis/tests/testfiles/analysis/darkmatter/__init__.py
+-rw-r--r--   0 knc6     (54782) 642div   (36677)      464 2024-05-04 16:06:52.000000 jarvis_tools-2024.4.20/jarvis/tests/testfiles/analysis/darkmatter/test_metrics.py
+drwxr-xr-x   0 knc6     (54782) 642div   (36677)        0 2024-05-04 16:07:18.263182 jarvis_tools-2024.4.20/jarvis/tests/testfiles/analysis/defects/
+-rw-r--r--   0 knc6     (54782) 642div   (36677)        0 2024-05-04 16:06:52.000000 jarvis_tools-2024.4.20/jarvis/tests/testfiles/analysis/defects/__init__.py
+-rw-r--r--   0 knc6     (54782) 642div   (36677)      444 2024-05-04 16:06:52.000000 jarvis_tools-2024.4.20/jarvis/tests/testfiles/analysis/defects/test_subs.py
+-rw-r--r--   0 knc6     (54782) 642div   (36677)     3252 2024-05-04 16:06:52.000000 jarvis_tools-2024.4.20/jarvis/tests/testfiles/analysis/defects/test_surface.py
+-rw-r--r--   0 knc6     (54782) 642div   (36677)     1216 2024-05-04 16:06:52.000000 jarvis_tools-2024.4.20/jarvis/tests/testfiles/analysis/defects/test_vacancy.py
+drwxr-xr-x   0 knc6     (54782) 642div   (36677)        0 2024-05-04 16:07:18.271182 jarvis_tools-2024.4.20/jarvis/tests/testfiles/analysis/elastic/
+-rw-r--r--   0 knc6     (54782) 642div   (36677)        0 2024-05-04 16:06:52.000000 jarvis_tools-2024.4.20/jarvis/tests/testfiles/analysis/elastic/__init__.py
+-rw-r--r--   0 knc6     (54782) 642div   (36677)     2577 2024-05-04 16:06:52.000000 jarvis_tools-2024.4.20/jarvis/tests/testfiles/analysis/elastic/test_tensor.py
+drwxr-xr-x   0 knc6     (54782) 642div   (36677)        0 2024-05-04 16:07:18.275182 jarvis_tools-2024.4.20/jarvis/tests/testfiles/analysis/interface/
+-rw-r--r--   0 knc6     (54782) 642div   (36677)        0 2024-05-04 16:06:52.000000 jarvis_tools-2024.4.20/jarvis/tests/testfiles/analysis/interface/__init__.py
+-rw-r--r--   0 knc6     (54782) 642div   (36677)     8683 2024-05-04 16:06:52.000000 jarvis_tools-2024.4.20/jarvis/tests/testfiles/analysis/interface/test_zur.py
+drwxr-xr-x   0 knc6     (54782) 642div   (36677)        0 2024-05-04 16:07:18.279182 jarvis_tools-2024.4.20/jarvis/tests/testfiles/analysis/magnetism/
+-rw-r--r--   0 knc6     (54782) 642div   (36677)        0 2024-05-04 16:06:52.000000 jarvis_tools-2024.4.20/jarvis/tests/testfiles/analysis/magnetism/__init__.py
+-rw-r--r--   0 knc6     (54782) 642div   (36677)      589 2024-05-04 16:06:52.000000 jarvis_tools-2024.4.20/jarvis/tests/testfiles/analysis/magnetism/test_magnetism.py
+drwxr-xr-x   0 knc6     (54782) 642div   (36677)        0 2024-05-04 16:07:18.291182 jarvis_tools-2024.4.20/jarvis/tests/testfiles/analysis/phonon/
+-rw-r--r--   0 knc6     (54782) 642div   (36677)        0 2024-05-04 16:06:52.000000 jarvis_tools-2024.4.20/jarvis/tests/testfiles/analysis/phonon/__init__.py
+-rw-r--r--   0 knc6     (54782) 642div   (36677)     5121 2024-05-04 16:06:52.000000 jarvis_tools-2024.4.20/jarvis/tests/testfiles/analysis/phonon/test_dos.py
+-rw-r--r--   0 knc6     (54782) 642div   (36677)      326 2024-05-04 16:06:52.000000 jarvis_tools-2024.4.20/jarvis/tests/testfiles/analysis/phonon/test_fc.py
+-rw-r--r--   0 knc6     (54782) 642div   (36677)     1279 2024-05-04 16:06:52.000000 jarvis_tools-2024.4.20/jarvis/tests/testfiles/analysis/phonon/test_ir.py
+drwxr-xr-x   0 knc6     (54782) 642div   (36677)        0 2024-05-04 16:07:18.299182 jarvis_tools-2024.4.20/jarvis/tests/testfiles/analysis/solar/
+-rw-r--r--   0 knc6     (54782) 642div   (36677)        0 2024-05-04 16:06:52.000000 jarvis_tools-2024.4.20/jarvis/tests/testfiles/analysis/solar/__init__.py
+-rw-r--r--   0 knc6     (54782) 642div   (36677)     1399 2024-05-04 16:06:52.000000 jarvis_tools-2024.4.20/jarvis/tests/testfiles/analysis/solar/test_solar.py
+drwxr-xr-x   0 knc6     (54782) 642div   (36677)        0 2024-05-04 16:07:18.303182 jarvis_tools-2024.4.20/jarvis/tests/testfiles/analysis/stm/
+-rw-r--r--   0 knc6     (54782) 642div   (36677)        0 2024-05-04 16:06:52.000000 jarvis_tools-2024.4.20/jarvis/tests/testfiles/analysis/stm/__init__.py
+-rw-r--r--   0 knc6     (54782) 642div   (36677)     1672 2024-05-04 16:06:52.000000 jarvis_tools-2024.4.20/jarvis/tests/testfiles/analysis/stm/test_stm.py
+drwxr-xr-x   0 knc6     (54782) 642div   (36677)        0 2024-05-04 16:07:18.315182 jarvis_tools-2024.4.20/jarvis/tests/testfiles/analysis/structure/
+-rw-r--r--   0 knc6     (54782) 642div   (36677)        0 2024-05-04 16:06:52.000000 jarvis_tools-2024.4.20/jarvis/tests/testfiles/analysis/structure/__init__.py
+-rw-r--r--   0 knc6     (54782) 642div   (36677)      390 2024-05-04 16:06:52.000000 jarvis_tools-2024.4.20/jarvis/tests/testfiles/analysis/structure/test_energetics.py
+-rw-r--r--   0 knc6     (54782) 642div   (36677)     1301 2024-05-04 16:06:52.000000 jarvis_tools-2024.4.20/jarvis/tests/testfiles/analysis/structure/test_neighbors.py
+-rw-r--r--   0 knc6     (54782) 642div   (36677)     3585 2024-05-04 16:06:52.000000 jarvis_tools-2024.4.20/jarvis/tests/testfiles/analysis/structure/test_spacegroup.py
+drwxr-xr-x   0 knc6     (54782) 642div   (36677)        0 2024-05-04 16:07:18.319182 jarvis_tools-2024.4.20/jarvis/tests/testfiles/analysis/thermodynamics/
+-rw-r--r--   0 knc6     (54782) 642div   (36677)        0 2024-05-04 16:06:52.000000 jarvis_tools-2024.4.20/jarvis/tests/testfiles/analysis/thermodynamics/__init__.py
+-rw-r--r--   0 knc6     (54782) 642div   (36677)     1554 2024-05-04 16:06:52.000000 jarvis_tools-2024.4.20/jarvis/tests/testfiles/analysis/thermodynamics/test_energetics.py
+drwxr-xr-x   0 knc6     (54782) 642div   (36677)        0 2024-05-04 16:07:18.327181 jarvis_tools-2024.4.20/jarvis/tests/testfiles/analysis/topological/
+-rw-r--r--   0 knc6     (54782) 642div   (36677)        0 2024-05-04 16:06:52.000000 jarvis_tools-2024.4.20/jarvis/tests/testfiles/analysis/topological/__init__.py
+-rw-r--r--   0 knc6     (54782) 642div   (36677)      424 2024-05-04 16:06:52.000000 jarvis_tools-2024.4.20/jarvis/tests/testfiles/analysis/topological/test_spillage.py
+drwxr-xr-x   0 knc6     (54782) 642div   (36677)        0 2024-05-04 16:07:18.359181 jarvis_tools-2024.4.20/jarvis/tests/testfiles/core/
+-rw-r--r--   0 knc6     (54782) 642div   (36677)        0 2024-05-04 16:06:53.000000 jarvis_tools-2024.4.20/jarvis/tests/testfiles/core/__init__.py
+-rw-r--r--   0 knc6     (54782) 642div   (36677)     5666 2024-05-04 16:06:53.000000 jarvis_tools-2024.4.20/jarvis/tests/testfiles/core/p.py
+-rw-r--r--   0 knc6     (54782) 642div   (36677)     6809 2024-05-04 16:07:08.000000 jarvis_tools-2024.4.20/jarvis/tests/testfiles/core/test_atoms.py
+-rw-r--r--   0 knc6     (54782) 642div   (36677)      262 2024-05-04 16:06:53.000000 jarvis_tools-2024.4.20/jarvis/tests/testfiles/core/test_circuits.py
+-rw-r--r--   0 knc6     (54782) 642div   (36677)      569 2024-05-04 16:07:08.000000 jarvis_tools-2024.4.20/jarvis/tests/testfiles/core/test_composition.py
+-rw-r--r--   0 knc6     (54782) 642div   (36677)     2844 2024-05-04 16:06:53.000000 jarvis_tools-2024.4.20/jarvis/tests/testfiles/core/test_graph.py
+-rw-r--r--   0 knc6     (54782) 642div   (36677)    11116 2024-05-04 16:06:53.000000 jarvis_tools-2024.4.20/jarvis/tests/testfiles/core/test_kpoints.py
+-rw-r--r--   0 knc6     (54782) 642div   (36677)     1507 2024-05-04 16:06:53.000000 jarvis_tools-2024.4.20/jarvis/tests/testfiles/core/test_latice.py
+-rw-r--r--   0 knc6     (54782) 642div   (36677)      339 2024-05-04 16:06:53.000000 jarvis_tools-2024.4.20/jarvis/tests/testfiles/core/test_pdb.py
+-rw-r--r--   0 knc6     (54782) 642div   (36677)      551 2024-05-04 16:06:53.000000 jarvis_tools-2024.4.20/jarvis/tests/testfiles/core/test_specie.py
+-rw-r--r--   0 knc6     (54782) 642div   (36677)      541 2024-05-04 16:06:53.000000 jarvis_tools-2024.4.20/jarvis/tests/testfiles/core/test_utils.py
+drwxr-xr-x   0 knc6     (54782) 642div   (36677)        0 2024-05-04 16:07:18.367181 jarvis_tools-2024.4.20/jarvis/tests/testfiles/db/
+-rw-r--r--   0 knc6     (54782) 642div   (36677)        0 2024-05-04 16:06:53.000000 jarvis_tools-2024.4.20/jarvis/tests/testfiles/db/__init__.py
+-rw-r--r--   0 knc6     (54782) 642div   (36677)     1496 2024-05-04 16:06:53.000000 jarvis_tools-2024.4.20/jarvis/tests/testfiles/db/test_figshare.py
+-rw-r--r--   0 knc6     (54782) 642div   (36677)      154 2024-05-04 16:06:53.000000 jarvis_tools-2024.4.20/jarvis/tests/testfiles/db/test_restapi.py
+drwxr-xr-x   0 knc6     (54782) 642div   (36677)        0 2024-05-04 16:07:18.375181 jarvis_tools-2024.4.20/jarvis/tests/testfiles/tasks/
+-rw-r--r--   0 knc6     (54782) 642div   (36677)        0 2024-05-04 16:06:54.000000 jarvis_tools-2024.4.20/jarvis/tests/testfiles/tasks/__init__.py
+-rw-r--r--   0 knc6     (54782) 642div   (36677)      804 2024-05-04 16:06:54.000000 jarvis_tools-2024.4.20/jarvis/tests/testfiles/tasks/test_lammps.py
+-rw-r--r--   0 knc6     (54782) 642div   (36677)      696 2024-05-04 16:06:54.000000 jarvis_tools-2024.4.20/jarvis/tests/testfiles/tasks/test_vasp.py
+drwxr-xr-x   0 knc6     (54782) 642div   (36677)        0 2024-05-04 16:07:18.391181 jarvis_tools-2024.4.20/jarvis_tools.egg-info/
+-rw-r--r--   0 knc6     (54782) 642div   (36677)     3442 2024-05-04 16:07:17.000000 jarvis_tools-2024.4.20/jarvis_tools.egg-info/PKG-INFO
+-rw-r--r--   0 knc6     (54782) 642div   (36677)     7651 2024-05-04 16:07:17.000000 jarvis_tools-2024.4.20/jarvis_tools.egg-info/SOURCES.txt
+-rw-r--r--   0 knc6     (54782) 642div   (36677)        1 2024-05-04 16:07:17.000000 jarvis_tools-2024.4.20/jarvis_tools.egg-info/dependency_links.txt
+-rw-r--r--   0 knc6     (54782) 642div   (36677)      265 2024-05-04 16:07:17.000000 jarvis_tools-2024.4.20/jarvis_tools.egg-info/requires.txt
+-rw-r--r--   0 knc6     (54782) 642div   (36677)        7 2024-05-04 16:07:17.000000 jarvis_tools-2024.4.20/jarvis_tools.egg-info/top_level.txt
+-rw-r--r--   0 knc6     (54782) 642div   (36677)      195 2024-05-04 16:07:18.403181 jarvis_tools-2024.4.20/setup.cfg
+-rw-r--r--   0 knc6     (54782) 642div   (36677)     2696 2024-05-04 16:07:08.000000 jarvis_tools-2024.4.20/setup.py
```

### Comparing `jarvis-tools-2024.4.10/LICENSE.rst` & `jarvis_tools-2024.4.20/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `jarvis-tools-2024.4.10/PKG-INFO` & `jarvis_tools-2024.4.20/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jarvis-tools
-Version: 2024.4.10
+Version: 2024.4.20
 Summary: jarvis-tools: an open-source software package for data-driven atomistic materials design. https://jarvis.nist.gov/
 Home-page: https://github.com/usnistgov/jarvis
 Author: Kamal Choudhary
 Author-email: kamal.choudhary@nist.gov
 License: NIST
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Development Status :: 4 - Beta
```

### Comparing `jarvis-tools-2024.4.10/README.rst` & `jarvis_tools-2024.4.20/README.rst`

 * *Files identical despite different names*

### Comparing `jarvis-tools-2024.4.10/jarvis/ai/descriptors/cfid.py` & `jarvis_tools-2024.4.20/jarvis/ai/descriptors/cfid.py`

 * *Files identical despite different names*

### Comparing `jarvis-tools-2024.4.10/jarvis/ai/descriptors/coulomb.py` & `jarvis_tools-2024.4.20/jarvis/ai/descriptors/coulomb.py`

 * *Files identical despite different names*

### Comparing `jarvis-tools-2024.4.10/jarvis/ai/pkgs/lgbm/classification.py` & `jarvis_tools-2024.4.20/jarvis/ai/pkgs/lgbm/classification.py`

 * *Files identical despite different names*

### Comparing `jarvis-tools-2024.4.10/jarvis/ai/pkgs/lgbm/regression.py` & `jarvis_tools-2024.4.20/jarvis/ai/pkgs/lgbm/regression.py`

 * *Files identical despite different names*

### Comparing `jarvis-tools-2024.4.10/jarvis/ai/pkgs/sklearn/classification.py` & `jarvis_tools-2024.4.20/jarvis/ai/pkgs/sklearn/classification.py`

 * *Files identical despite different names*

### Comparing `jarvis-tools-2024.4.10/jarvis/ai/pkgs/sklearn/hyper_params.py` & `jarvis_tools-2024.4.20/jarvis/ai/pkgs/sklearn/hyper_params.py`

 * *Files identical despite different names*

### Comparing `jarvis-tools-2024.4.10/jarvis/ai/pkgs/sklearn/regression.py` & `jarvis_tools-2024.4.20/jarvis/ai/pkgs/sklearn/regression.py`

 * *Files identical despite different names*

### Comparing `jarvis-tools-2024.4.10/jarvis/ai/pkgs/utils.py` & `jarvis_tools-2024.4.20/jarvis/ai/pkgs/utils.py`

 * *Files identical despite different names*

### Comparing `jarvis-tools-2024.4.10/jarvis/ai/uncertainty/gaussian_process_uncertainty.py` & `jarvis_tools-2024.4.20/jarvis/ai/uncertainty/gaussian_process_uncertainty.py`

 * *Files identical despite different names*

### Comparing `jarvis-tools-2024.4.10/jarvis/ai/uncertainty/lgbm_quantile_uncertainty.py` & `jarvis_tools-2024.4.20/jarvis/ai/uncertainty/lgbm_quantile_uncertainty.py`

 * *Files identical despite different names*

### Comparing `jarvis-tools-2024.4.10/jarvis/analysis/darkmatter/metrics.py` & `jarvis_tools-2024.4.20/jarvis/analysis/darkmatter/metrics.py`

 * *Files identical despite different names*

### Comparing `jarvis-tools-2024.4.10/jarvis/analysis/defects/substitutions.py` & `jarvis_tools-2024.4.20/jarvis/analysis/defects/substitutions.py`

 * *Files identical despite different names*

### Comparing `jarvis-tools-2024.4.10/jarvis/analysis/defects/surface.py` & `jarvis_tools-2024.4.20/jarvis/analysis/defects/surface.py`

 * *Files 2% similar despite different names*

```diff
@@ -31,18 +31,19 @@
     """Get surface object of arbitrary atoms object and miller index."""
 
     def __init__(
         self,
         atoms=None,
         indices=[0, 0, 1],
         layers=3,
-        thickness=25,
+        thickness=None,
         vacuum=18.0,
         tol=1e-10,
         from_conventional_structure=True,
+        use_thickness_c=True,
     ):
         """Initialize the class.
 
         Args:
              atoms: jarvis.core.Atoms object
 
              indices: Miller indices
@@ -63,14 +64,15 @@
             self.atoms = Spacegroup3D(atoms).conventional_standard_structure
         else:
             self.atoms = atoms
         self.tol = tol
         self.vacuum = vacuum
         self.layers = layers
         self.thickness = thickness
+        self.use_thickness_c = use_thickness_c
         # Note thickness overwrites layers
 
     def to_dict(self):
         """Convert to a dictionary."""
         d = OrderedDict()
         d["atoms"] = self.atoms.to_dict()
         d["indices"] = self.indices
@@ -143,15 +145,34 @@
         new_atoms = Atoms(
             lattice_mat=tmp_cell,
             coords=new_coords,
             elements=atoms.elements,
             cartesian=True,
         )
         if self.thickness is not None and (self.thickness) > 0:
-            self.layers = int(self.thickness / new_atoms.lattice.c) + 1
+            if not self.use_thickness_c:
+                new_lat = new_atoms.lattice_mat  # lat_lengths()
+                a1 = new_lat[0]
+                a2 = new_lat[1]
+                a3 = new_lat[2]
+                new_lat = np.array(
+                    [
+                        a1,
+                        a2,
+                        np.cross(a1, a2)
+                        * np.dot(a3, np.cross(a1, a2))
+                        / norm(np.cross(a1, a2)) ** 2,
+                    ]
+                )
+
+                a3 = new_lat[2]
+                self.layers = int(self.thickness / np.linalg.norm(a3)) + 1
+            else:
+                self.layers = int(self.thickness / new_atoms.lattice.c) + 1
+            # print("self.layers", self.layers)
             # dims=get_supercell_dims(new_atoms,enforce_c_size=self.thickness)
             # print ('dims=',dims,self.layers)
             # surf_atoms = new_atoms.make_supercell_matrix([1, 1, dims[2]])
             # print('self.layers',self.layers,self.thickness,new_atoms.lattice.c)
         surf_atoms = new_atoms.make_supercell_matrix([1, 1, self.layers])
         # print("supercell_cart_coords", surf_atoms.frac_coords)
```

### Comparing `jarvis-tools-2024.4.10/jarvis/analysis/defects/vacancy.py` & `jarvis_tools-2024.4.20/jarvis/analysis/defects/vacancy.py`

 * *Files identical despite different names*

### Comparing `jarvis-tools-2024.4.10/jarvis/analysis/diffraction/atomic_scattering_params.json` & `jarvis_tools-2024.4.20/jarvis/analysis/diffraction/atomic_scattering_params.json`

 * *Files identical despite different names*

### Comparing `jarvis-tools-2024.4.10/jarvis/analysis/diffraction/xrd.py` & `jarvis_tools-2024.4.20/jarvis/analysis/diffraction/xrd.py`

 * *Files identical despite different names*

### Comparing `jarvis-tools-2024.4.10/jarvis/analysis/elastic/tensor.py` & `jarvis_tools-2024.4.20/jarvis/analysis/elastic/tensor.py`

 * *Files identical despite different names*

### Comparing `jarvis-tools-2024.4.10/jarvis/analysis/interface/zur.py` & `jarvis_tools-2024.4.20/jarvis/analysis/interface/zur.py`

 * *Files identical despite different names*

### Comparing `jarvis-tools-2024.4.10/jarvis/analysis/magnetism/magmom_setup.py` & `jarvis_tools-2024.4.20/jarvis/analysis/magnetism/magmom_setup.py`

 * *Files identical despite different names*

### Comparing `jarvis-tools-2024.4.10/jarvis/analysis/periodic/ptable.py` & `jarvis_tools-2024.4.20/jarvis/analysis/periodic/ptable.py`

 * *Files identical despite different names*

### Comparing `jarvis-tools-2024.4.10/jarvis/analysis/phonon/dos.py` & `jarvis_tools-2024.4.20/jarvis/analysis/phonon/dos.py`

 * *Files identical despite different names*

### Comparing `jarvis-tools-2024.4.10/jarvis/analysis/phonon/force_constants.py` & `jarvis_tools-2024.4.20/jarvis/analysis/phonon/force_constants.py`

 * *Files identical despite different names*

### Comparing `jarvis-tools-2024.4.10/jarvis/analysis/phonon/ir.py` & `jarvis_tools-2024.4.20/jarvis/analysis/phonon/ir.py`

 * *Files identical despite different names*

### Comparing `jarvis-tools-2024.4.10/jarvis/analysis/solarefficiency/am1.5G.dat` & `jarvis_tools-2024.4.20/jarvis/analysis/solarefficiency/am1.5G.dat`

 * *Files identical despite different names*

### Comparing `jarvis-tools-2024.4.10/jarvis/analysis/solarefficiency/solar.py` & `jarvis_tools-2024.4.20/jarvis/analysis/solarefficiency/solar.py`

 * *Files identical despite different names*

### Comparing `jarvis-tools-2024.4.10/jarvis/analysis/stem/convolution_apprx.py` & `jarvis_tools-2024.4.20/jarvis/analysis/stem/convolution_apprx.py`

 * *Files identical despite different names*

### Comparing `jarvis-tools-2024.4.10/jarvis/analysis/stm/tersoff_hamann.py` & `jarvis_tools-2024.4.20/jarvis/analysis/stm/tersoff_hamann.py`

 * *Files identical despite different names*

### Comparing `jarvis-tools-2024.4.10/jarvis/analysis/structure/neighbors.py` & `jarvis_tools-2024.4.20/jarvis/analysis/structure/neighbors.py`

 * *Files identical despite different names*

### Comparing `jarvis-tools-2024.4.10/jarvis/analysis/structure/spacegroup.py` & `jarvis_tools-2024.4.20/jarvis/analysis/structure/spacegroup.py`

 * *Files identical despite different names*

### Comparing `jarvis-tools-2024.4.10/jarvis/analysis/thermodynamics/energetics.py` & `jarvis_tools-2024.4.20/jarvis/analysis/thermodynamics/energetics.py`

 * *Files identical despite different names*

### Comparing `jarvis-tools-2024.4.10/jarvis/analysis/thermodynamics/unary.json` & `jarvis_tools-2024.4.20/jarvis/analysis/thermodynamics/unary.json`

 * *Files identical despite different names*

### Comparing `jarvis-tools-2024.4.10/jarvis/analysis/thermodynamics/unary_qe_tb.json` & `jarvis_tools-2024.4.20/jarvis/analysis/thermodynamics/unary_qe_tb.json`

 * *Files identical despite different names*

### Comparing `jarvis-tools-2024.4.10/jarvis/analysis/topological/spillage.py` & `jarvis_tools-2024.4.20/jarvis/analysis/topological/spillage.py`

 * *Files identical despite different names*

### Comparing `jarvis-tools-2024.4.10/jarvis/core/Elements.json` & `jarvis_tools-2024.4.20/jarvis/core/Elements.json`

 * *Files identical despite different names*

### Comparing `jarvis-tools-2024.4.10/jarvis/core/atom_init.json` & `jarvis_tools-2024.4.20/jarvis/core/atom_init.json`

 * *Files identical despite different names*

### Comparing `jarvis-tools-2024.4.10/jarvis/core/atoms.py` & `jarvis_tools-2024.4.20/jarvis/core/atoms.py`

 * *Files 3% similar despite different names*

```diff
@@ -16,18 +16,34 @@
 import os
 import math
 import tempfile
 import random
 import string
 import datetime
 from collections import defaultdict
+from sklearn.metrics import mean_absolute_error
+import zipfile
+import json
 
 amu_gm = 1.66054e-24
 ang_cm = 1e-8
 
+with zipfile.ZipFile(
+    str(
+        os.path.join(
+            os.path.dirname(__file__), "mineral_name_prototype.json.zip"
+        )
+    ),
+    "r",
+) as z:
+    # Open the specific JSON file within the zip
+    with z.open("mineral_name_prototype.json") as file:
+        # Load the JSON data from the file
+        mineral_json_file = json.load(file)
+
 
 class Atoms(object):
     """
     Generate Atoms python object.
 
     >>> box = [[2.715, 2.715, 0], [0, 2.715, 2.715], [2.715, 0, 2.715]]
     >>> coords = [[0, 0, 0], [0.25, 0.2, 0.25]]
@@ -645,18 +661,18 @@
                 # if site[2] == z_max:
                 up = up + Specie(element).Z
             if site[2] <= z_min + tol:
                 # if site[2] == z_min:
                 dn = dn + Specie(element).Z
         polar = False
         if up != dn:
-            print("Seems like a polar materials.")
+            # print("Seems like a polar materials.")
             polar = True
         if up == dn:
-            print("Non-polar")
+            # print("Non-polar")
             polar = False
         return polar
 
     def strain_atoms(self, strain):
         """Apply volumetric strain to atoms."""
         # strains=np.arange(0.80,1.2,0.02)
         s = np.eye(3) + np.array(strain) * np.eye(3)
@@ -1035,14 +1051,114 @@
     def density(self):
         """Get density in g/cm3 of the atoms object."""
         den = float(self.composition.weight * amu_gm) / (
             float(self.volume) * (ang_cm) ** 3
         )
         return den
 
+    def plot_atoms(
+        self=None,
+        colors=[],
+        sizes=[],
+        cutoff=1.9,
+        opacity=0.5,
+        bond_width=2,
+        filename=None,
+    ):
+        """Plot atoms using plotly."""
+        import plotly.graph_objects as go
+
+        fig = go.Figure()
+        if not colors:
+            colors = ["blue", "green", "red"]
+
+        unique_elements = self.uniq_species
+        if len(unique_elements) > len(colors):
+            raise ValueError("Provide more colors.")
+        color_map = {}
+        size_map = {}
+        for ii, i in enumerate(unique_elements):
+            color_map[i] = colors[ii]
+            size_map[i] = Specie(i).Z * 2
+        cart_coords = self.cart_coords
+        elements = self.elements
+        atoms_arr = []
+
+        for ii, i in enumerate(cart_coords):
+            atoms_arr.append(
+                [
+                    i[0],
+                    i[1],
+                    i[2],
+                    color_map[elements[ii]],
+                    size_map[elements[ii]],
+                ]
+            )
+        # atoms = [
+        #     (0, 0, 0, 'red'),   # Atom 1
+        #     (1, 1, 1, 'blue'),  # Atom 2
+        #     (2, 0, 1, 'green')  # Atom 3
+        # ]
+
+        # Create a scatter plot for the 3D points
+        trace1 = go.Scatter3d(
+            x=[atom[0] for atom in atoms_arr],
+            y=[atom[1] for atom in atoms_arr],
+            z=[atom[2] for atom in atoms_arr],
+            mode="markers",
+            marker=dict(
+                size=[atom[4] for atom in atoms_arr],  # Marker size
+                color=[atom[3] for atom in atoms_arr],  # Marker color
+                opacity=opacity,
+            ),
+        )
+        fig.add_trace(trace1)
+
+        # Update plot layout
+        fig.update_layout(
+            title="3D Atom Coordinates",
+            scene=dict(
+                xaxis_title="X Coordinates",
+                yaxis_title="Y Coordinates",
+                zaxis_title="Z Coordinates",
+            ),
+            margin=dict(l=0, r=0, b=0, t=0),  # Tight layout
+        )
+        if bond_width is not None:
+            nbs = self.get_all_neighbors(r=5)
+            bonds = []
+            for i in nbs:
+                for j in i:
+                    if j[2] <= cutoff:
+                        bonds.append([j[0], j[1]])
+            for bond in bonds:
+                # print(bond)
+                # Extract coordinates of the first and second atom in each bond
+                x_coords = [atoms_arr[bond[0]][0], atoms_arr[bond[1]][0]]
+                y_coords = [atoms_arr[bond[0]][1], atoms_arr[bond[1]][1]]
+                z_coords = [atoms_arr[bond[0]][2], atoms_arr[bond[1]][2]]
+
+                fig.add_trace(
+                    go.Scatter3d(
+                        x=x_coords,
+                        y=y_coords,
+                        z=z_coords,
+                        mode="lines",
+                        line=dict(color="grey", width=bond_width),
+                        marker=dict(
+                            size=0.1
+                        ),  # Small marker size to make lines prominent
+                    )
+                )
+        # Show the plot
+        if filename is not None:
+            fig.write_image(filename)
+        else:
+            fig.show()
+
     @property
     def atomic_numbers(self):
         """Get list of atomic numbers of atoms in the atoms object."""
         numbers = []
         for i in self.elements:
             numbers.append(Specie(i).Z)
         return numbers
@@ -1164,14 +1280,113 @@
         """Get packing fraction of the atoms object."""
         total_rad = 0
         for i in self.elements:
             total_rad = total_rad + Specie(i).atomic_rad ** 3
         pf = np.array([4 * np.pi * total_rad / (3 * self.volume)])
         return round(pf[0], 5)
 
+    def get_alignn_feats(
+        self,
+        model_name="jv_formation_energy_peratom_alignn",
+        max_neighbors=12,
+        neighbor_strategy="k-nearest",
+        use_canonize=True,
+        atom_features="cgcnn",
+        line_graph=True,
+        cutoff=8,
+        model="",
+    ):
+        """Get ALIGNN features."""
+
+        def get_val(model, g, lg):
+            activation = {}
+
+            def getActivation(name):
+                # the hook signature
+                def hook(model, input, output):
+                    activation[name] = output.detach()
+
+                return hook
+
+            h = model.readout.register_forward_hook(getActivation("readout"))
+            out = model([g, lg])
+            del out
+            h.remove()
+            return activation["readout"][0]
+
+        from alignn.graphs import Graph
+        from alignn.pretrained import get_figshare_model
+
+        g, lg = Graph.atom_dgl_multigraph(
+            self,
+            cutoff=cutoff,
+            atom_features=atom_features,
+            max_neighbors=max_neighbors,
+            neighbor_strategy=neighbor_strategy,
+            compute_line_graph=line_graph,
+            use_canonize=use_canonize,
+        )
+        if model == "":
+            model = get_figshare_model(
+                model_name="jv_formation_energy_peratom_alignn"
+            )
+        h = get_val(model, g, lg)
+        return h
+
+    def get_mineral_prototype_name(
+        self, prim=True, include_c_over_a=False, digits=3
+    ):
+        from jarvis.analysis.structure.spacegroup import Spacegroup3D
+
+        spg = Spacegroup3D(self)
+        number = spg.space_group_number
+        cnv_atoms = spg.conventional_standard_structure
+        n_conv = cnv_atoms.num_atoms
+        # hall_number=str(spg._dataset['hall_number'])
+        wyc = "".join(list((sorted(set(spg._dataset["wyckoffs"])))))
+        name = (
+            (self.composition.prototype_new)
+            + "_"
+            + str(number)
+            + "_"
+            + str(wyc)
+            + "_"
+            + str(n_conv)
+        )
+        # if include_com:
+        if include_c_over_a:
+            # print(cnv_atoms)
+            abc = cnv_atoms.lattice.abc
+            ca = round(abc[2] / abc[0], digits)
+            # com_positions = "_".join(map(str,self.get_center_of_mass()))
+            # round(np.sum(spg._dataset['std_positions']),round_digit)
+            name += "_" + str(ca)
+            # name+="_"+str(com_positions)
+        return name
+
+    def get_minaral_name(self, model=""):
+        """Get mineral prototype."""
+        mae = np.inf
+        feats = self.get_alignn_feats(model=model)
+        nm = self.get_mineral_prototype_name()
+        if nm in mineral_json_file:
+            for i in mineral_json_file[nm]:
+                maem = mean_absolute_error(i[1], feats)
+                if maem < mae:
+                    mae = maem
+                    name = i[0]
+        else:
+            for i, j in mineral_json_file.items():
+                for k in j:
+                    maem = mean_absolute_error(k[1], feats)
+                    if maem < mae:
+                        mae = maem
+                        name = k[0]
+        return name
+
     def lattice_points_in_supercell(self, supercell_matrix):
         """
         Adapted from Pymatgen.
 
         Returns the list of points on the original lattice contained in the
         supercell in fractional coordinates (with the supercell basis).
         e.g. [[2,0,0],[0,1,0],[0,0,1]] returns [[0,0,0],[0.5,0,0]]
@@ -1232,14 +1447,15 @@
         cutoff=4,
         take_n_bonds=2,
         include_spg=True,
     ):
         """Describe for NLP applications."""
         from jarvis.analysis.diffraction.xrd import XRD
 
+        min_name = self.get_minaral_name()
         if include_spg:
             from jarvis.analysis.structure.spacegroup import Spacegroup3D
 
             spg = Spacegroup3D(self)
         theta, d_hkls, intens = XRD().simulate(atoms=self)
         #     x = atoms.atomwise_angle_and_radial_distribution()
         #     bond_distances = {}
@@ -1260,14 +1476,15 @@
                 dist = dist[0:take_n_bonds]
             bond_distances[i] = ", ".join(map(str, dist))
         fracs = {}
         for i, j in (self.composition.atomic_fraction).items():
             fracs[i] = round(j, 3)
         info = {}
         chem_info = {
+            "mineral_name": min_name,
             "atomic_formula": self.composition.reduced_formula,
             "prototype": self.composition.prototype,
             "molecular_weight": round(self.composition.weight / 2, 2),
             "atomic_fraction": (fracs),
             "atomic_X": ", ".join(
                 map(str, [Specie(s).X for s in self.uniq_species])
             ),
@@ -1368,16 +1585,38 @@
             + "º with some of the top XRD peaks at "
             + struct_info["top_k_xrd_peaks"]
             + "º with "
             + "Wyckoff symbols "
             + struct_info["wyckoff"]
             + "."
         )
+        if min_name is not None:
+            line3 = (
+                chem_info["atomic_formula"]
+                + " is "
+                + min_name
+                + "-derived structured and"
+                + " crystallizes in the "
+                + struct_info["crystal_system"]
+                + " "
+                + str(struct_info["spg_symbol"])
+                + " spacegroup."
+            )
+        else:
+            line3 = (
+                chem_info["atomic_formula"]
+                + " crystallizes in the "
+                + struct_info["crystal_system"]
+                + " "
+                + str(struct_info["spg_symbol"])
+                + " spacegroup."
+            )
         info["desc_1"] = line1
         info["desc_2"] = line2
+        info["desc_3"] = line3
         return info
 
     def make_supercell_matrix(self, scaling_matrix):
         """
         Adapted from Pymatgen.
 
         Makes a supercell. Allowing to have sites outside the unit cell.
```

### Comparing `jarvis-tools-2024.4.10/jarvis/core/circuits.py` & `jarvis_tools-2024.4.20/jarvis/core/circuits.py`

 * *Files identical despite different names*

### Comparing `jarvis-tools-2024.4.10/jarvis/core/composition.py` & `jarvis_tools-2024.4.20/jarvis/core/composition.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Modules handling chemical composition."""
+
 # from math import gcd
 import string
 from jarvis.core.specie import Specie
 from collections import OrderedDict
 from collections import defaultdict
 from jarvis.core.utils import gcd
 import re
@@ -72,17 +73,44 @@
         """Get chemical prototypes such as A, AB etc."""
         proto = ""
         all_upper = string.ascii_uppercase
 
         reduced, repeat = self.reduce()
         N = 0
         for specie, count in reduced.items():
-            proto = proto + str(all_upper[N]) + str(round(count, 3))
-            N = N + 1
-        return proto.replace("1", "")
+            if count != 1:
+                proto = proto + str(all_upper[N]) + str(round(count, 3))
+                N = N + 1
+            else:
+                proto = proto + str(all_upper[N])
+                N = N + 1
+        return proto  # .replace("1", "")
+
+    @property
+    def prototype_new(self):
+        """Get chemical prototypes such as A, AB etc."""
+        proto = ""
+        all_upper = string.ascii_uppercase
+        # print('reduce',self.reduce())
+        reduced, repeat = self.reduce()
+        items = sorted(list(reduced.values()), reverse=True)
+        # print('items',items)
+        N = 0
+        for c in items:
+            if c == 1:
+                proto = proto + str(all_upper[N])
+                N = N + 1
+            else:
+                proto = proto + str(all_upper[N]) + str(round(c, 3))
+                N = N + 1
+
+        # for specie, count in reduced.items():
+        #    proto = proto + str(all_upper[N]) + str(round(count, 3))
+        #    N = N + 1
+        return proto  # .replace("1", "")
 
     def to_dict(self):
         """Return dictionary format."""
         return self._content
 
     @property
     def nspecies(self):
```

### Comparing `jarvis-tools-2024.4.10/jarvis/core/element_charge.json` & `jarvis_tools-2024.4.20/jarvis/core/element_charge.json`

 * *Files identical despite different names*

### Comparing `jarvis-tools-2024.4.10/jarvis/core/graphs.py` & `jarvis_tools-2024.4.20/jarvis/core/graphs.py`

 * *Files identical despite different names*

### Comparing `jarvis-tools-2024.4.10/jarvis/core/image.py` & `jarvis_tools-2024.4.20/jarvis/core/image.py`

 * *Files identical despite different names*

### Comparing `jarvis-tools-2024.4.10/jarvis/core/kpoints.py` & `jarvis_tools-2024.4.20/jarvis/core/kpoints.py`

 * *Files identical despite different names*

### Comparing `jarvis-tools-2024.4.10/jarvis/core/lattice.py` & `jarvis_tools-2024.4.20/jarvis/core/lattice.py`

 * *Files identical despite different names*

### Comparing `jarvis-tools-2024.4.10/jarvis/core/magpie.json` & `jarvis_tools-2024.4.20/jarvis/core/magpie.json`

 * *Files identical despite different names*

### Comparing `jarvis-tools-2024.4.10/jarvis/core/specie.py` & `jarvis_tools-2024.4.20/jarvis/core/specie.py`

 * *Files identical despite different names*

### Comparing `jarvis-tools-2024.4.10/jarvis/core/spectrum.py` & `jarvis_tools-2024.4.20/jarvis/core/spectrum.py`

 * *Files identical despite different names*

### Comparing `jarvis-tools-2024.4.10/jarvis/core/utils.py` & `jarvis_tools-2024.4.20/jarvis/core/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -245,24 +245,21 @@
     """Operate affine method."""
     affine_point = np.array([cart_coord[0], cart_coord[1], cart_coord[2], 1])
     return np.dot(np.array(affine_matrix), affine_point)[0:3]
 
 
 def gaussian(x, sigma):
     """Get Gaussian profile."""
-    return np.exp(-(x ** 2) / (2 * sigma ** 2))
+    return np.exp(-(x**2) / (2 * sigma**2))
 
 
 def lorentzian2(x, gamma):
     """Get Lorentziann profile."""
     return (
-        gamma
-        / 2
-        / (np.pi * (x ** 2 + (gamma / 2) ** 2))
-        / (2 / (np.pi * gamma))
+        gamma / 2 / (np.pi * (x**2 + (gamma / 2) ** 2)) / (2 / (np.pi * gamma))
     )
 
 
 def digitize_array(values=[], max_len=10):
     """Digitze an array."""
     has_float = False in [float(i).is_integer() for i in values]
     if has_float:
@@ -271,15 +268,22 @@
         min_val = min(arr)
         bins = np.arange(1, max_len + 1) * (max_val - min_val) / 10
         values = np.digitize(arr, bins)
     return values
 
 
 def bond_angle(
-    dist1, dist2, bondx1, bondx2, bondy1, bondy2, bondz1, bondz2,
+    dist1,
+    dist2,
+    bondx1,
+    bondx2,
+    bondy1,
+    bondy2,
+    bondz1,
+    bondz2,
 ):
     """Get an angle."""
     nm = dist1 * dist2
     rrx = bondx1 * bondx2
     rry = bondy1 * bondy2
     rrz = bondz1 * bondz2
     cos = (rrx + rry + rrz) / (nm)
@@ -320,15 +324,15 @@
         .squeeze()
     )
     return new_data.numpy()
 
 
 def cos_formula(a, b, c):
     """Get angle between three edges for oblique triangles."""
-    res = (a ** 2 + b ** 2 - c ** 2) / (2 * a * b)
+    res = (a**2 + b**2 - c**2) / (2 * a * b)
     res = -1.0 if res < -1.0 else res
     res = 1.0 if res > 1.0 else res
     return np.arccos(res)
 
 
 # def is_xml_valid(xsd="jarvisdft.xsd", xml="JVASP-1002.xml"):
 #   """Check if XML is valid."""
```

### Comparing `jarvis-tools-2024.4.10/jarvis/db/figshare.py` & `jarvis_tools-2024.4.20/jarvis/db/figshare.py`

 * *Files identical despite different names*

### Comparing `jarvis-tools-2024.4.10/jarvis/db/lammps_to_xml.py` & `jarvis_tools-2024.4.20/jarvis/db/lammps_to_xml.py`

 * *Files identical despite different names*

### Comparing `jarvis-tools-2024.4.10/jarvis/db/qe_to_xml.py` & `jarvis_tools-2024.4.20/jarvis/db/qe_to_xml.py`

 * *Files identical despite different names*

### Comparing `jarvis-tools-2024.4.10/jarvis/db/restapi.py` & `jarvis_tools-2024.4.20/jarvis/db/restapi.py`

 * *Files identical despite different names*

### Comparing `jarvis-tools-2024.4.10/jarvis/db/vasp_to_xml.py` & `jarvis_tools-2024.4.20/jarvis/db/vasp_to_xml.py`

 * *Files identical despite different names*

### Comparing `jarvis-tools-2024.4.10/jarvis/db/webpages.py` & `jarvis_tools-2024.4.20/jarvis/db/webpages.py`

 * *Files identical despite different names*

### Comparing `jarvis-tools-2024.4.10/jarvis/io/boltztrap/inputs.py` & `jarvis_tools-2024.4.20/jarvis/io/boltztrap/inputs.py`

 * *Files identical despite different names*

### Comparing `jarvis-tools-2024.4.10/jarvis/io/boltztrap/outputs.py` & `jarvis_tools-2024.4.20/jarvis/io/boltztrap/outputs.py`

 * *Files identical despite different names*

### Comparing `jarvis-tools-2024.4.10/jarvis/io/calphad/write_decorated_poscar.py` & `jarvis_tools-2024.4.20/jarvis/io/calphad/write_decorated_poscar.py`

 * *Files identical despite different names*

### Comparing `jarvis-tools-2024.4.10/jarvis/io/lammps/inputs.py` & `jarvis_tools-2024.4.20/jarvis/io/lammps/inputs.py`

 * *Files identical despite different names*

### Comparing `jarvis-tools-2024.4.10/jarvis/io/lammps/outputs.py` & `jarvis_tools-2024.4.20/jarvis/io/lammps/outputs.py`

 * *Files identical despite different names*

### Comparing `jarvis-tools-2024.4.10/jarvis/io/nexus/inputs.py` & `jarvis_tools-2024.4.20/jarvis/io/nexus/inputs.py`

 * *Files identical despite different names*

### Comparing `jarvis-tools-2024.4.10/jarvis/io/pennylane/inputs.py` & `jarvis_tools-2024.4.20/jarvis/io/pennylane/inputs.py`

 * *Files identical despite different names*

### Comparing `jarvis-tools-2024.4.10/jarvis/io/phonopy/fcmat2hr.py` & `jarvis_tools-2024.4.20/jarvis/io/phonopy/fcmat2hr.py`

 * *Files identical despite different names*

### Comparing `jarvis-tools-2024.4.10/jarvis/io/phonopy/inputs.py` & `jarvis_tools-2024.4.20/jarvis/io/phonopy/inputs.py`

 * *Files identical despite different names*

### Comparing `jarvis-tools-2024.4.10/jarvis/io/phonopy/outputs.py` & `jarvis_tools-2024.4.20/jarvis/io/phonopy/outputs.py`

 * *Files identical despite different names*

### Comparing `jarvis-tools-2024.4.10/jarvis/io/prismatic/inputs.py` & `jarvis_tools-2024.4.20/jarvis/io/prismatic/inputs.py`

 * *Files identical despite different names*

### Comparing `jarvis-tools-2024.4.10/jarvis/io/qe/inputs.py` & `jarvis_tools-2024.4.20/jarvis/io/qe/inputs.py`

 * *Files identical despite different names*

### Comparing `jarvis-tools-2024.4.10/jarvis/io/qe/outputs.py` & `jarvis_tools-2024.4.20/jarvis/io/qe/outputs.py`

 * *Files identical despite different names*

### Comparing `jarvis-tools-2024.4.10/jarvis/io/qiskit/inputs.py` & `jarvis_tools-2024.4.20/jarvis/io/qiskit/inputs.py`

 * *Files identical despite different names*

### Comparing `jarvis-tools-2024.4.10/jarvis/io/tequila/inputs.py` & `jarvis_tools-2024.4.20/jarvis/io/tequila/inputs.py`

 * *Files identical despite different names*

### Comparing `jarvis-tools-2024.4.10/jarvis/io/vasp/default_potcars.json` & `jarvis_tools-2024.4.20/jarvis/io/vasp/default_potcars.json`

 * *Files identical despite different names*

### Comparing `jarvis-tools-2024.4.10/jarvis/io/vasp/inputs.py` & `jarvis_tools-2024.4.20/jarvis/io/vasp/inputs.py`

 * *Files identical despite different names*

### Comparing `jarvis-tools-2024.4.10/jarvis/io/vasp/outputs.py` & `jarvis_tools-2024.4.20/jarvis/io/vasp/outputs.py`

 * *Files 1% similar despite different names*

```diff
@@ -195,15 +195,14 @@
                 chg_arr.append(chg)
         chg = np.array(chg_arr)
         # self.chg = chg
         return chg
 
     def chg_set(self, text, start, end, volume, ng):
         """Return CHGCAR sets."""
-
         lines_0 = text[start:end]
         # tmp = np.empty((ng))
         # p = np.fromstring('\n'.join(lines_0),  sep=' ')
         # for zz in range(tmp.shape[2]):
         # for yy in range(tmp.shape[1]):
         #    tmp[:,yy,zz] = np.fromstring(p,  sep=' ',count=tmp.shape[0])
         #    print(np.fromstring(p,  sep=' ',count=tmp.shape[0]))
@@ -227,15 +226,14 @@
         cbm=0,
         vbm=0,
         filename="Avg.png",
         use_ase=False,
         plot=True,
     ):
         """Calculate vacuum potential used in work-function calculation."""
-
         if use_ase:
             from ase.calculators.vasp import VaspChargeDensity
 
             locd = VaspChargeDensity(self.filename)
             cell = locd.atoms[0].cell
             latlens = np.linalg.norm(cell, axis=1)
             vol = np.linalg.det(cell)
@@ -510,14 +508,88 @@
         """Get Fermi energy."""
         efermi = []
         for i in self.data:
             if "E-fermi :" in i:
                 efermi.append(float(i.split()[2]))
         return efermi[-1]
 
+    def all_structures(self, elements=[]):
+        """Get all structure snapshots."""
+        force_pattern = "TOTAL-FORCE (eV/Angst)"
+        if not elements:
+            try:
+                atoms = Atoms.from_poscar(
+                    self.filename.replace("OUTCAR", "POSCAR")
+                ).elements
+            except Exception:
+                print("Check POSCAR exsist, or pass elements.")
+                pass
+        blocks = []
+        for ii, i in enumerate(self.data):
+            if "  free  energy   TOTEN  =" in i:
+                blocks.append(i)
+            if "  free  energy ML TOTEN  =" in i:
+                blocks.append(i)
+        nions = self.nions
+        atoms_array = []
+        energy_array = []
+        force_array = []
+        stress_array = []
+        for ii, i in enumerate(self.data):
+            if "in kB" in i:
+                stress = [
+                    float(j) for j in self.data[ii].split("in kB")[1].split()
+                ]
+                stress_array.append(stress)
+            if "VOLUME and BASIS-vectors are now :" in i:
+                tmp1 = [float(j) for j in self.data[ii + 5].split()]
+                tmp2 = [float(j) for j in self.data[ii + 6].split()]
+                tmp3 = [float(j) for j in self.data[ii + 7].split()]
+                lat_mat = [
+                    [tmp1[0], tmp1[1], tmp1[2]],
+                    [tmp2[0], tmp2[1], tmp2[2]],
+                    [tmp3[0], tmp3[1], tmp3[2]],
+                ]
+            if "  free  energy   TOTEN  =" in i:
+                energy = (
+                    self.data[ii]
+                    .split("  free  energy   TOTEN  =")[1]
+                    .split("eV")[0]
+                )
+                energy_array.append(energy)
+            if "  free  energy ML TOTEN  =" in i:
+                energy = (
+                    self.data[ii]
+                    .split("  free  energy   TOTEN  =")[1]
+                    .split("eV")[0]
+                )
+                energy_array.append(energy)
+
+            if force_pattern in i:
+                coords = []
+                forces = []
+                for j in range(nions):
+                    tmp = [float(k) for k in self.data[ii + 2 + j].split()]
+                    coords.append([tmp[0], tmp[1], tmp[2]])
+                    forces.append([tmp[3], tmp[4], tmp[5]])
+                    # print(tmp)
+                atoms = Atoms(
+                    lattice_mat=lat_mat,
+                    coords=coords,
+                    elements=elements,
+                    cartesian=True,
+                )
+
+                atoms_array.append(atoms)
+        if len(blocks) != len(atoms_array):
+            print(
+                "WARNING: check OUTCAR parser", len(blocks), len(atoms_array)
+            )
+        return atoms_array, energy_array, force_array, stress_array
+
     @property
     def all_band_energies(self):
         """Get all band energies."""
         last_efermi = None
         for i, ii in enumerate(self.data):
             if "E-fermi :" in ii:
                 last_efermi = i
@@ -2373,14 +2445,7 @@
     info["freqs"] = freqs
     info["activity"] = activity
     info["alpha"] = alpha
     info["beta2"] = beta2
     info["indices"] = indices
     info["intensity"] = intensity
     return info
-
-
-"""
-kp='/users/knc6/Software/Devs/jarvis/jarvis/examples/vasp/SiOptb88/MAIN-RELAX-bulk@mp_149/KPOINT'
-kpt=Kpoints(filename=kp)
-print (kpt)
-"""
```

### Comparing `jarvis-tools-2024.4.10/jarvis/io/wannier/default_semicore.json` & `jarvis_tools-2024.4.20/jarvis/io/wannier/default_semicore.json`

 * *Files identical despite different names*

### Comparing `jarvis-tools-2024.4.10/jarvis/io/wannier/inputs.py` & `jarvis_tools-2024.4.20/jarvis/io/wannier/inputs.py`

 * *Files identical despite different names*

### Comparing `jarvis-tools-2024.4.10/jarvis/io/wannier/outputs.py` & `jarvis_tools-2024.4.20/jarvis/io/wannier/outputs.py`

 * *Files identical despite different names*

### Comparing `jarvis-tools-2024.4.10/jarvis/io/wanniertools/inputs.py` & `jarvis_tools-2024.4.20/jarvis/io/wanniertools/inputs.py`

 * *Files identical despite different names*

### Comparing `jarvis-tools-2024.4.10/jarvis/io/wanniertools/outputs.py` & `jarvis_tools-2024.4.20/jarvis/io/wanniertools/outputs.py`

 * *Files identical despite different names*

### Comparing `jarvis-tools-2024.4.10/jarvis/io/wien2k/inputs.py` & `jarvis_tools-2024.4.20/jarvis/io/wien2k/inputs.py`

 * *Files identical despite different names*

### Comparing `jarvis-tools-2024.4.10/jarvis/io/wien2k/outputs.py` & `jarvis_tools-2024.4.20/jarvis/io/wien2k/outputs.py`

 * *Files identical despite different names*

### Comparing `jarvis-tools-2024.4.10/jarvis/io/zeopp/inputs.py` & `jarvis_tools-2024.4.20/jarvis/io/zeopp/inputs.py`

 * *Files identical despite different names*

### Comparing `jarvis-tools-2024.4.10/jarvis/tasks/boltztrap/run.py` & `jarvis_tools-2024.4.20/jarvis/tasks/boltztrap/run.py`

 * *Files identical despite different names*

### Comparing `jarvis-tools-2024.4.10/jarvis/tasks/lammps/lammps.py` & `jarvis_tools-2024.4.20/jarvis/tasks/lammps/lammps.py`

 * *Files identical despite different names*

### Comparing `jarvis-tools-2024.4.10/jarvis/tasks/lammps/templates/displace.mod` & `jarvis_tools-2024.4.20/jarvis/tasks/lammps/templates/displace.mod`

 * *Files identical despite different names*

### Comparing `jarvis-tools-2024.4.10/jarvis/tasks/lammps/templates/inelast.mod` & `jarvis_tools-2024.4.20/jarvis/tasks/lammps/templates/inelast.mod`

 * *Files identical despite different names*

### Comparing `jarvis-tools-2024.4.10/jarvis/tasks/lammps/templates/inelast_min.mod` & `jarvis_tools-2024.4.20/jarvis/tasks/lammps/templates/inelast_min.mod`

 * *Files identical despite different names*

### Comparing `jarvis-tools-2024.4.10/jarvis/tasks/lammps/templates/inelast_nobox.mod` & `jarvis_tools-2024.4.20/jarvis/tasks/lammps/templates/inelast_nobox.mod`

 * *Files identical despite different names*

### Comparing `jarvis-tools-2024.4.10/jarvis/tasks/lammps/templates/inelastcomb.mod` & `jarvis_tools-2024.4.20/jarvis/tasks/lammps/templates/inelastcomb.mod`

 * *Files identical despite different names*

### Comparing `jarvis-tools-2024.4.10/jarvis/tasks/lammps/templates/inelastreax.mod` & `jarvis_tools-2024.4.20/jarvis/tasks/lammps/templates/inelastreax.mod`

 * *Files identical despite different names*

### Comparing `jarvis-tools-2024.4.10/jarvis/tasks/lammps/templates/relax.mod` & `jarvis_tools-2024.4.20/jarvis/tasks/lammps/templates/relax.mod`

 * *Files identical despite different names*

### Comparing `jarvis-tools-2024.4.10/jarvis/tasks/lammps/templates/templates.py` & `jarvis_tools-2024.4.20/jarvis/tasks/lammps/templates/templates.py`

 * *Files identical despite different names*

### Comparing `jarvis-tools-2024.4.10/jarvis/tasks/nexus/qmc.py` & `jarvis_tools-2024.4.20/jarvis/tasks/nexus/qmc.py`

 * *Files identical despite different names*

### Comparing `jarvis-tools-2024.4.10/jarvis/tasks/phonopy/run.py` & `jarvis_tools-2024.4.20/jarvis/tasks/phonopy/run.py`

 * *Files identical despite different names*

### Comparing `jarvis-tools-2024.4.10/jarvis/tasks/qe/converg.py` & `jarvis_tools-2024.4.20/jarvis/tasks/qe/converg.py`

 * *Files identical despite different names*

### Comparing `jarvis-tools-2024.4.10/jarvis/tasks/qe/master_super.py` & `jarvis_tools-2024.4.20/jarvis/tasks/qe/master_super.py`

 * *Files identical despite different names*

### Comparing `jarvis-tools-2024.4.10/jarvis/tasks/qe/qe.py` & `jarvis_tools-2024.4.20/jarvis/tasks/qe/qe.py`

 * *Files identical despite different names*

### Comparing `jarvis-tools-2024.4.10/jarvis/tasks/qe/super.py` & `jarvis_tools-2024.4.20/jarvis/tasks/qe/super.py`

 * *Files identical despite different names*

### Comparing `jarvis-tools-2024.4.10/jarvis/tasks/qe/super_tetra.py` & `jarvis_tools-2024.4.20/jarvis/tasks/qe/super_tetra.py`

 * *Files identical despite different names*

### Comparing `jarvis-tools-2024.4.10/jarvis/tasks/queue_jobs.py` & `jarvis_tools-2024.4.20/jarvis/tasks/queue_jobs.py`

 * *Files identical despite different names*

### Comparing `jarvis-tools-2024.4.10/jarvis/tasks/vasp/vasp.py` & `jarvis_tools-2024.4.20/jarvis/tasks/vasp/vasp.py`

 * *Files identical despite different names*

### Comparing `jarvis-tools-2024.4.10/jarvis/tests/testfiles/ai/test_ai_uncertainty.py` & `jarvis_tools-2024.4.20/jarvis/tests/testfiles/ai/test_ai_uncertainty.py`

 * *Files identical despite different names*

### Comparing `jarvis-tools-2024.4.10/jarvis/tests/testfiles/ai/test_desc.py` & `jarvis_tools-2024.4.20/jarvis/tests/testfiles/ai/test_desc.py`

 * *Files identical despite different names*

### Comparing `jarvis-tools-2024.4.10/jarvis/tests/testfiles/ai/test_pkgs.py` & `jarvis_tools-2024.4.20/jarvis/tests/testfiles/ai/test_pkgs.py`

 * *Files identical despite different names*

### Comparing `jarvis-tools-2024.4.10/jarvis/tests/testfiles/analysis/defects/test_surface.py` & `jarvis_tools-2024.4.20/jarvis/tests/testfiles/analysis/defects/test_surface.py`

 * *Files identical despite different names*

### Comparing `jarvis-tools-2024.4.10/jarvis/tests/testfiles/analysis/defects/test_vacancy.py` & `jarvis_tools-2024.4.20/jarvis/tests/testfiles/analysis/defects/test_vacancy.py`

 * *Files identical despite different names*

### Comparing `jarvis-tools-2024.4.10/jarvis/tests/testfiles/analysis/elastic/test_tensor.py` & `jarvis_tools-2024.4.20/jarvis/tests/testfiles/analysis/elastic/test_tensor.py`

 * *Files identical despite different names*

### Comparing `jarvis-tools-2024.4.10/jarvis/tests/testfiles/analysis/interface/test_zur.py` & `jarvis_tools-2024.4.20/jarvis/tests/testfiles/analysis/interface/test_zur.py`

 * *Files identical despite different names*

### Comparing `jarvis-tools-2024.4.10/jarvis/tests/testfiles/analysis/magnetism/test_magnetism.py` & `jarvis_tools-2024.4.20/jarvis/tests/testfiles/analysis/magnetism/test_magnetism.py`

 * *Files identical despite different names*

### Comparing `jarvis-tools-2024.4.10/jarvis/tests/testfiles/analysis/phonon/test_dos.py` & `jarvis_tools-2024.4.20/jarvis/tests/testfiles/analysis/phonon/test_dos.py`

 * *Files identical despite different names*

### Comparing `jarvis-tools-2024.4.10/jarvis/tests/testfiles/analysis/phonon/test_ir.py` & `jarvis_tools-2024.4.20/jarvis/tests/testfiles/analysis/phonon/test_ir.py`

 * *Files identical despite different names*

### Comparing `jarvis-tools-2024.4.10/jarvis/tests/testfiles/analysis/solar/test_solar.py` & `jarvis_tools-2024.4.20/jarvis/tests/testfiles/analysis/solar/test_solar.py`

 * *Files identical despite different names*

### Comparing `jarvis-tools-2024.4.10/jarvis/tests/testfiles/analysis/stm/test_stm.py` & `jarvis_tools-2024.4.20/jarvis/tests/testfiles/analysis/stm/test_stm.py`

 * *Files identical despite different names*

### Comparing `jarvis-tools-2024.4.10/jarvis/tests/testfiles/analysis/structure/test_neighbors.py` & `jarvis_tools-2024.4.20/jarvis/tests/testfiles/analysis/structure/test_neighbors.py`

 * *Files identical despite different names*

### Comparing `jarvis-tools-2024.4.10/jarvis/tests/testfiles/analysis/structure/test_spacegroup.py` & `jarvis_tools-2024.4.20/jarvis/tests/testfiles/analysis/structure/test_spacegroup.py`

 * *Files identical despite different names*

### Comparing `jarvis-tools-2024.4.10/jarvis/tests/testfiles/analysis/thermodynamics/test_energetics.py` & `jarvis_tools-2024.4.20/jarvis/tests/testfiles/analysis/thermodynamics/test_energetics.py`

 * *Files identical despite different names*

### Comparing `jarvis-tools-2024.4.10/jarvis/tests/testfiles/core/p.py` & `jarvis_tools-2024.4.20/jarvis/tests/testfiles/core/p.py`

 * *Files identical despite different names*

### Comparing `jarvis-tools-2024.4.10/jarvis/tests/testfiles/core/test_atoms.py` & `jarvis_tools-2024.4.20/jarvis/tests/testfiles/core/test_atoms.py`

 * *Files 2% similar despite different names*

```diff
@@ -92,15 +92,14 @@
     f = open(cif_example, "r")
     lines = f.read()
     f.close()
     x = Atoms.from_cif(from_string=lines)
 
 
 def test_basic_atoms():
-
     Si = Atoms(
         lattice_mat=FIXTURES["lattice_mat"],
         coords=FIXTURES["coords"],
         elements=FIXTURES["elements"],
     )
     dim = get_supercell_dims(Si)
     build_xanes_poscar(atoms=Si, filename_with_prefix=True)
@@ -108,22 +107,23 @@
 
     opt = OptimadeAdaptor(Si)
     opt_info = opt.to_optimade()
     opt = OptimadeAdaptor()
     print(opt.from_optimade(opt_info))
 
     polar = Si.check_polar
+    # prot = Si.get_prototype_name()
     Si.props = ["a", "a"]
     vac_pad = VacuumPadding(Si)
     den_2d = round(vac_pad.get_effective_2d_slab().density, 2)
     den_0d = round(vac_pad.get_effective_molecule().density, 2)
     den_lll_red = round(Si.get_lll_reduced_structure().density, 2)
     strng = Si.get_string()
     scell_nat_old = Si.make_supercell_old([2, 2, 2]).num_atoms
-    descr = Si.describe()
+    # descr = Si.describe()
     scell_nat = Si.make_supercell([2, 2, 2]).num_atoms
     scell_nat2 = Si.make_supercell_matrix(
         [[2, 0, 0], [0, 2, 0], [0, 0, 2]]
     ).num_atoms
     # print("scell_nat,scell_nat2", scell_nat, scell_nat2)
     # print(Si.make_supercell([2, 2, 2]))
     # print()
@@ -262,8 +262,9 @@
     print(
         "Si2_supercell_without_two_atoms.num_atoms",
         Si2_supercell_without_two_atoms.num_atoms,
     )
     assert Si2_supercell_without_two_atoms.num_atoms == 14
 
 
+# test_basic_atoms()
 # test_remove_sites_by_indices()
```

### Comparing `jarvis-tools-2024.4.10/jarvis/tests/testfiles/core/test_graph.py` & `jarvis_tools-2024.4.20/jarvis/tests/testfiles/core/test_graph.py`

 * *Files identical despite different names*

### Comparing `jarvis-tools-2024.4.10/jarvis/tests/testfiles/core/test_kpoints.py` & `jarvis_tools-2024.4.20/jarvis/tests/testfiles/core/test_kpoints.py`

 * *Files identical despite different names*

### Comparing `jarvis-tools-2024.4.10/jarvis/tests/testfiles/core/test_latice.py` & `jarvis_tools-2024.4.20/jarvis/tests/testfiles/core/test_latice.py`

 * *Files identical despite different names*

### Comparing `jarvis-tools-2024.4.10/jarvis/tests/testfiles/core/test_specie.py` & `jarvis_tools-2024.4.20/jarvis/tests/testfiles/core/test_specie.py`

 * *Files identical despite different names*

### Comparing `jarvis-tools-2024.4.10/jarvis/tests/testfiles/core/test_utils.py` & `jarvis_tools-2024.4.20/jarvis/tests/testfiles/core/test_utils.py`

 * *Files identical despite different names*

### Comparing `jarvis-tools-2024.4.10/jarvis/tests/testfiles/db/test_figshare.py` & `jarvis_tools-2024.4.20/jarvis/tests/testfiles/db/test_figshare.py`

 * *Files identical despite different names*

### Comparing `jarvis-tools-2024.4.10/jarvis/tests/testfiles/tasks/test_lammps.py` & `jarvis_tools-2024.4.20/jarvis/tests/testfiles/tasks/test_lammps.py`

 * *Files identical despite different names*

### Comparing `jarvis-tools-2024.4.10/jarvis/tests/testfiles/tasks/test_vasp.py` & `jarvis_tools-2024.4.20/jarvis/tests/testfiles/tasks/test_vasp.py`

 * *Files identical despite different names*

### Comparing `jarvis-tools-2024.4.10/jarvis_tools.egg-info/PKG-INFO` & `jarvis_tools-2024.4.20/jarvis_tools.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jarvis-tools
-Version: 2024.4.10
+Version: 2024.4.20
 Summary: jarvis-tools: an open-source software package for data-driven atomistic materials design. https://jarvis.nist.gov/
 Home-page: https://github.com/usnistgov/jarvis
 Author: Kamal Choudhary
 Author-email: kamal.choudhary@nist.gov
 License: NIST
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Development Status :: 4 - Beta
```

### Comparing `jarvis-tools-2024.4.10/jarvis_tools.egg-info/SOURCES.txt` & `jarvis_tools-2024.4.20/jarvis_tools.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -67,14 +67,15 @@
 jarvis/core/composition.py
 jarvis/core/element_charge.json
 jarvis/core/graphs.py
 jarvis/core/image.py
 jarvis/core/kpoints.py
 jarvis/core/lattice.py
 jarvis/core/magpie.json
+jarvis/core/mineral_name_prototype.json.zip
 jarvis/core/specie.py
 jarvis/core/spectrum.py
 jarvis/core/utils.py
 jarvis/db/__init__.py
 jarvis/db/figshare.py
 jarvis/db/jsonutils.py
 jarvis/db/lammps_to_xml.py
```

### Comparing `jarvis-tools-2024.4.10/setup.py` & `jarvis_tools-2024.4.20/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 base_dir = os.path.dirname(__file__)
 # with open(os.path.join(base_dir, "README.rst")) as f:
 with open(os.path.join(base_dir, "README.md")) as f:
     long_d = f.read()
 
 setup(
     name="jarvis-tools",
-    version="2024.4.10",
+    version="2024.4.20",
     long_description=long_d,
     install_requires=[
         "numpy>=1.20.1",
         "scipy>=1.5.0",
         "matplotlib>=3.0.0",
         "spglib>=1.14.1",
         "joblib>=0.14.1",
@@ -30,14 +30,15 @@
     ],
     package_data={
         "jarvis.core": [
             "Elements.json",
             "magpie.json",
             "element_charge.json",
             "atom_init.json",
+            "mineral_name_prototype.json.zip",
         ],
         "jarvis.tasks.lammps.templates": [
             "displace.mod",
             "inelastcomb.mod",
             "inelast_min.mod",
             "inelast.mod",
             "inelast_nobox.mod",
```

