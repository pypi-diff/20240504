# Comparing `tmp/phono3py-3.0.2.tar.gz` & `tmp/phono3py-3.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "phono3py-3.0.2.tar", last modified: Sun Apr 21 05:59:46 2024, max compression
+gzip compressed data, was "phono3py-3.0.3.tar", last modified: Sat May  4 07:43:29 2024, max compression
```

## Comparing `phono3py-3.0.2.tar` & `phono3py-3.0.3.tar`

### file list

```diff
@@ -1,262 +1,267 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 05:59:46.641300 phono3py-3.0.2/
--rw-r--r--   0 runner    (1001) docker     (127)     1470 2024-04-21 05:58:48.000000 phono3py-3.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      120 2024-04-21 05:58:48.000000 phono3py-3.0.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)      451 2024-04-21 05:59:46.641300 phono3py-3.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2446 2024-04-21 05:58:48.000000 phono3py-3.0.2/README.md
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-21 05:59:41.000000 phono3py-3.0.2/__nanoversion__.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 05:59:46.613300 phono3py-3.0.2/c/
--rw-r--r--   0 runner    (1001) docker     (127)    68786 2024-04-21 05:58:48.000000 phono3py-3.0.2/c/_phono3py.c
--rw-r--r--   0 runner    (1001) docker     (127)     8081 2024-04-21 05:58:48.000000 phono3py-3.0.2/c/_phononcalc.c
--rw-r--r--   0 runner    (1001) docker     (127)    15045 2024-04-21 05:58:48.000000 phono3py-3.0.2/c/bzgrid.c
--rw-r--r--   0 runner    (1001) docker     (127)     3674 2024-04-21 05:58:48.000000 phono3py-3.0.2/c/bzgrid.h
--rw-r--r--   0 runner    (1001) docker     (127)    12441 2024-04-21 05:58:48.000000 phono3py-3.0.2/c/collision_matrix.c
--rw-r--r--   0 runner    (1001) docker     (127)     2584 2024-04-21 05:58:48.000000 phono3py-3.0.2/c/collision_matrix.h
--rw-r--r--   0 runner    (1001) docker     (127)    29801 2024-04-21 05:58:48.000000 phono3py-3.0.2/c/dynmat.c
--rw-r--r--   0 runner    (1001) docker     (127)     5149 2024-04-21 05:58:48.000000 phono3py-3.0.2/c/dynmat.h
--rw-r--r--   0 runner    (1001) docker     (127)    23953 2024-04-21 05:58:48.000000 phono3py-3.0.2/c/fc3.c
--rw-r--r--   0 runner    (1001) docker     (127)     2805 2024-04-21 05:58:48.000000 phono3py-3.0.2/c/fc3.h
--rw-r--r--   0 runner    (1001) docker     (127)    15184 2024-04-21 05:58:48.000000 phono3py-3.0.2/c/grgrid.c
--rw-r--r--   0 runner    (1001) docker     (127)     3392 2024-04-21 05:58:48.000000 phono3py-3.0.2/c/grgrid.h
--rw-r--r--   0 runner    (1001) docker     (127)    11554 2024-04-21 05:58:48.000000 phono3py-3.0.2/c/gridsys.c
--rw-r--r--   0 runner    (1001) docker     (127)    13923 2024-04-21 05:58:48.000000 phono3py-3.0.2/c/gridsys.h
--rw-r--r--   0 runner    (1001) docker     (127)    16545 2024-04-21 05:58:48.000000 phono3py-3.0.2/c/imag_self_energy_with_g.c
--rw-r--r--   0 runner    (1001) docker     (127)     3183 2024-04-21 05:58:48.000000 phono3py-3.0.2/c/imag_self_energy_with_g.h
--rw-r--r--   0 runner    (1001) docker     (127)    12188 2024-04-21 05:58:48.000000 phono3py-3.0.2/c/interaction.c
--rw-r--r--   0 runner    (1001) docker     (127)     2951 2024-04-21 05:58:48.000000 phono3py-3.0.2/c/interaction.h
--rw-r--r--   0 runner    (1001) docker     (127)     9128 2024-04-21 05:58:48.000000 phono3py-3.0.2/c/isotope.c
--rw-r--r--   0 runner    (1001) docker     (127)     2588 2024-04-21 05:58:48.000000 phono3py-3.0.2/c/isotope.h
--rw-r--r--   0 runner    (1001) docker     (127)     8032 2024-04-21 05:58:48.000000 phono3py-3.0.2/c/lagrid.c
--rw-r--r--   0 runner    (1001) docker     (127)     3487 2024-04-21 05:58:48.000000 phono3py-3.0.2/c/lagrid.h
--rw-r--r--   0 runner    (1001) docker     (127)     9063 2024-04-21 05:58:48.000000 phono3py-3.0.2/c/lapack_wrapper.c
--rw-r--r--   0 runner    (1001) docker     (127)     2975 2024-04-21 05:58:48.000000 phono3py-3.0.2/c/lapack_wrapper.h
--rw-r--r--   0 runner    (1001) docker     (127)    14541 2024-04-21 05:58:48.000000 phono3py-3.0.2/c/niggli.c
--rw-r--r--   0 runner    (1001) docker     (127)     2109 2024-04-21 05:58:48.000000 phono3py-3.0.2/c/niggli.h
--rw-r--r--   0 runner    (1001) docker     (127)    32268 2024-04-21 05:58:48.000000 phono3py-3.0.2/c/phono3py.c
--rw-r--r--   0 runner    (1001) docker     (127)    14077 2024-04-21 05:58:48.000000 phono3py-3.0.2/c/phono3py.h
--rw-r--r--   0 runner    (1001) docker     (127)     1986 2024-04-21 05:58:48.000000 phono3py-3.0.2/c/phonoc_array.h
--rw-r--r--   0 runner    (1001) docker     (127)     1813 2024-04-21 05:58:48.000000 phono3py-3.0.2/c/phonoc_const.h
--rw-r--r--   0 runner    (1001) docker     (127)     2199 2024-04-21 05:58:48.000000 phono3py-3.0.2/c/phonoc_utils.c
--rw-r--r--   0 runner    (1001) docker     (127)     1935 2024-04-21 05:58:48.000000 phono3py-3.0.2/c/phonoc_utils.h
--rw-r--r--   0 runner    (1001) docker     (127)    20519 2024-04-21 05:58:48.000000 phono3py-3.0.2/c/phonon.c
--rw-r--r--   0 runner    (1001) docker     (127)     3324 2024-04-21 05:58:48.000000 phono3py-3.0.2/c/phonon.h
--rw-r--r--   0 runner    (1001) docker     (127)     3514 2024-04-21 05:58:48.000000 phono3py-3.0.2/c/phononcalc.c
--rw-r--r--   0 runner    (1001) docker     (127)     2661 2024-04-21 05:58:48.000000 phono3py-3.0.2/c/phononcalc.h
--rw-r--r--   0 runner    (1001) docker     (127)    11627 2024-04-21 05:58:48.000000 phono3py-3.0.2/c/pp_collision.c
--rw-r--r--   0 runner    (1001) docker     (127)     3036 2024-04-21 05:58:48.000000 phono3py-3.0.2/c/pp_collision.h
--rw-r--r--   0 runner    (1001) docker     (127)     9296 2024-04-21 05:58:48.000000 phono3py-3.0.2/c/real_self_energy.c
--rw-r--r--   0 runner    (1001) docker     (127)     2514 2024-04-21 05:58:48.000000 phono3py-3.0.2/c/real_self_energy.h
--rw-r--r--   0 runner    (1001) docker     (127)    16752 2024-04-21 05:58:48.000000 phono3py-3.0.2/c/real_to_reciprocal.c
--rw-r--r--   0 runner    (1001) docker     (127)     2362 2024-04-21 05:58:48.000000 phono3py-3.0.2/c/real_to_reciprocal.h
--rw-r--r--   0 runner    (1001) docker     (127)    12160 2024-04-21 05:58:48.000000 phono3py-3.0.2/c/reciprocal_to_normal.c
--rw-r--r--   0 runner    (1001) docker     (127)     2294 2024-04-21 05:58:48.000000 phono3py-3.0.2/c/reciprocal_to_normal.h
--rw-r--r--   0 runner    (1001) docker     (127)    14689 2024-04-21 05:58:48.000000 phono3py-3.0.2/c/snf3x3.c
--rw-r--r--   0 runner    (1001) docker     (127)      267 2024-04-21 05:58:48.000000 phono3py-3.0.2/c/snf3x3.h
--rw-r--r--   0 runner    (1001) docker     (127)    38926 2024-04-21 05:58:48.000000 phono3py-3.0.2/c/tetrahedron_method.c
--rw-r--r--   0 runner    (1001) docker     (127)     2295 2024-04-21 05:58:48.000000 phono3py-3.0.2/c/tetrahedron_method.h
--rw-r--r--   0 runner    (1001) docker     (127)     5933 2024-04-21 05:58:48.000000 phono3py-3.0.2/c/triplet.c
--rw-r--r--   0 runner    (1001) docker     (127)     4134 2024-04-21 05:58:48.000000 phono3py-3.0.2/c/triplet.h
--rw-r--r--   0 runner    (1001) docker     (127)    18558 2024-04-21 05:58:48.000000 phono3py-3.0.2/c/triplet_grid.c
--rw-r--r--   0 runner    (1001) docker     (127)     2464 2024-04-21 05:58:48.000000 phono3py-3.0.2/c/triplet_grid.h
--rw-r--r--   0 runner    (1001) docker     (127)    13656 2024-04-21 05:58:48.000000 phono3py-3.0.2/c/triplet_iw.c
--rw-r--r--   0 runner    (1001) docker     (127)     2871 2024-04-21 05:58:48.000000 phono3py-3.0.2/c/triplet_iw.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 05:59:46.589300 phono3py-3.0.2/example/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 05:59:46.613300 phono3py-3.0.2/example/AlN-LDA/
--rw-r--r--   0 runner    (1001) docker     (127)      357 2024-04-21 05:58:48.000000 phono3py-3.0.2/example/AlN-LDA/BORN
--rw-r--r--   0 runner    (1001) docker     (127)    86886 2024-04-21 05:58:48.000000 phono3py-3.0.2/example/AlN-LDA/FORCES_FC2
--rw-r--r--   0 runner    (1001) docker     (127)   862253 2024-04-21 05:58:48.000000 phono3py-3.0.2/example/AlN-LDA/FORCES_FC3.lzma
--rw-r--r--   0 runner    (1001) docker     (127)      487 2024-04-21 05:58:48.000000 phono3py-3.0.2/example/AlN-LDA/POSCAR-unitcell
--rw-r--r--   0 runner    (1001) docker     (127)     2399 2024-04-21 05:58:48.000000 phono3py-3.0.2/example/AlN-LDA/README.md
--rw-r--r--   0 runner    (1001) docker     (127)   143873 2024-04-21 05:58:48.000000 phono3py-3.0.2/example/AlN-LDA/phono3py_disp.yaml
--rw-r--r--   0 runner    (1001) docker     (127)   176702 2024-04-21 05:58:48.000000 phono3py-3.0.2/example/AlN-LDA/phono3py_disp_dimfc2.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 05:59:46.613300 phono3py-3.0.2/example/NaCl-alm/
--rw-r--r--   0 runner    (1001) docker     (127)     1429 2024-04-21 05:58:48.000000 phono3py-3.0.2/example/NaCl-alm/README.md
--rw-r--r--   0 runner    (1001) docker     (127)   303332 2024-04-21 05:58:48.000000 phono3py-3.0.2/example/NaCl-alm/phono3py_params_NaCl222.yaml.xz
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 05:59:46.617300 phono3py-3.0.2/example/Si-CRYSTAL/
--rw-r--r--   0 runner    (1001) docker     (127)     6225 2024-04-21 05:58:48.000000 phono3py-3.0.2/example/Si-CRYSTAL/FORCES_FC2
--rw-r--r--   0 runner    (1001) docker     (127)    52417 2024-04-21 05:58:48.000000 phono3py-3.0.2/example/Si-CRYSTAL/FORCES_FC3
--rw-r--r--   0 runner    (1001) docker     (127)     1213 2024-04-21 05:58:48.000000 phono3py-3.0.2/example/Si-CRYSTAL/README
--rw-r--r--   0 runner    (1001) docker     (127)      815 2024-04-21 05:58:48.000000 phono3py-3.0.2/example/Si-CRYSTAL/TEMPLATE
--rw-r--r--   0 runner    (1001) docker     (127)      815 2024-04-21 05:58:48.000000 phono3py-3.0.2/example/Si-CRYSTAL/TEMPLATE3
--rw-r--r--   0 runner    (1001) docker     (127)    50060 2024-04-21 05:58:48.000000 phono3py-3.0.2/example/Si-CRYSTAL/crystal.o
--rw-r--r--   0 runner    (1001) docker     (127)   801243 2024-04-21 05:58:48.000000 phono3py-3.0.2/example/Si-CRYSTAL/outputs.tar.gz
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 05:59:46.617300 phono3py-3.0.2/example/Si-LDA/
--rw-r--r--   0 runner    (1001) docker     (127)   357907 2024-04-21 05:58:48.000000 phono3py-3.0.2/example/Si-LDA/FORCES_FC3
--rw-r--r--   0 runner    (1001) docker     (127)      727 2024-04-21 05:58:48.000000 phono3py-3.0.2/example/Si-LDA/POSCAR-unitcell
--rw-r--r--   0 runner    (1001) docker     (127)     1293 2024-04-21 05:58:48.000000 phono3py-3.0.2/example/Si-LDA/README.md
--rw-r--r--   0 runner    (1001) docker     (127)    32796 2024-04-21 05:58:48.000000 phono3py-3.0.2/example/Si-LDA/phono3py_disp.yaml
--rw-r--r--   0 runner    (1001) docker     (127)   305364 2024-04-21 05:58:48.000000 phono3py-3.0.2/example/Si-LDA/vasprun_xmls.tar.lzma
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 05:59:46.621300 phono3py-3.0.2/example/Si-PBE/
--rw-r--r--   0 runner    (1001) docker     (127)   357907 2024-04-21 05:58:48.000000 phono3py-3.0.2/example/Si-PBE/FORCES_FC3
--rw-r--r--   0 runner    (1001) docker     (127)      727 2024-04-21 05:58:48.000000 phono3py-3.0.2/example/Si-PBE/POSCAR-unitcell
--rw-r--r--   0 runner    (1001) docker     (127)     1293 2024-04-21 05:58:48.000000 phono3py-3.0.2/example/Si-PBE/README.md
--rw-r--r--   0 runner    (1001) docker     (127)    32796 2024-04-21 05:58:48.000000 phono3py-3.0.2/example/Si-PBE/phono3py_disp.yaml
--rw-r--r--   0 runner    (1001) docker     (127)   314724 2024-04-21 05:58:48.000000 phono3py-3.0.2/example/Si-PBE/vasprun_xmls.tar.lzma
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 05:59:46.621300 phono3py-3.0.2/example/Si-PBEsol/
--rw-r--r--   0 runner    (1001) docker     (127)   357907 2024-04-21 05:58:48.000000 phono3py-3.0.2/example/Si-PBEsol/FORCES_FC3
--rw-r--r--   0 runner    (1001) docker     (127)      727 2024-04-21 05:58:48.000000 phono3py-3.0.2/example/Si-PBEsol/POSCAR-unitcell
--rw-r--r--   0 runner    (1001) docker     (127)     2844 2024-04-21 05:58:48.000000 phono3py-3.0.2/example/Si-PBEsol/README.md
--rw-r--r--   0 runner    (1001) docker     (127)    46793 2024-04-21 05:58:48.000000 phono3py-3.0.2/example/Si-PBEsol/Si-band-DOS.png
--rw-r--r--   0 runner    (1001) docker     (127)    28346 2024-04-21 05:58:48.000000 phono3py-3.0.2/example/Si-PBEsol/Si-kaccum.png
--rw-r--r--   0 runner    (1001) docker     (127)     1029 2024-04-21 05:58:48.000000 phono3py-3.0.2/example/Si-PBEsol/Si.py
--rw-r--r--   0 runner    (1001) docker     (127)    32796 2024-04-21 05:58:48.000000 phono3py-3.0.2/example/Si-PBEsol/phono3py_disp.yaml
--rw-r--r--   0 runner    (1001) docker     (127)    95766 2024-04-21 05:58:48.000000 phono3py-3.0.2/example/Si-PBEsol/phono3py_disp_dimfc2.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 05:59:46.589300 phono3py-3.0.2/example/Si-PBEsol/vasprun_xml_fc2/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 05:59:46.625300 phono3py-3.0.2/example/Si-PBEsol/vasprun_xml_fc2/disp-fc2-00001/
--rw-r--r--   0 runner    (1001) docker     (127)      267 2024-04-21 05:58:48.000000 phono3py-3.0.2/example/Si-PBEsol/vasprun_xml_fc2/disp-fc2-00001/INCAR
--rw-r--r--   0 runner    (1001) docker     (127)    31479 2024-04-21 05:58:48.000000 phono3py-3.0.2/example/Si-PBEsol/vasprun_xml_fc2/disp-fc2-00001/POSCAR
--rw-r--r--   0 runner    (1001) docker     (127)   291058 2024-04-21 05:58:48.000000 phono3py-3.0.2/example/Si-PBEsol/vasprun_xml_fc2/disp-fc2-00001/vasprun.xml
--rw-r--r--   0 runner    (1001) docker     (127)   300636 2024-04-21 05:58:48.000000 phono3py-3.0.2/example/Si-PBEsol/vasprun_xmls.tar.lzma
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 05:59:46.625300 phono3py-3.0.2/example/Si-QE/
--rw-r--r--   0 runner    (1001) docker     (127)   357907 2024-04-21 05:58:48.000000 phono3py-3.0.2/example/Si-QE/FORCES_FC3
--rw-r--r--   0 runner    (1001) docker     (127)     1039 2024-04-21 05:58:48.000000 phono3py-3.0.2/example/Si-QE/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1025 2024-04-21 05:58:48.000000 phono3py-3.0.2/example/Si-QE/Si.in
--rw-r--r--   0 runner    (1001) docker     (127)    32833 2024-04-21 05:58:48.000000 phono3py-3.0.2/example/Si-QE/phono3py_disp.yaml
--rw-r--r--   0 runner    (1001) docker     (127)   150928 2024-04-21 05:58:48.000000 phono3py-3.0.2/example/Si-QE/supercell_out.tar.lzma
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 05:59:46.625300 phono3py-3.0.2/example/Si-TURBOMOLE/
--rw-r--r--   0 runner    (1001) docker     (127)    10449 2024-04-21 05:58:48.000000 phono3py-3.0.2/example/Si-TURBOMOLE/FORCES_FC2
--rw-r--r--   0 runner    (1001) docker     (127)   357907 2024-04-21 05:58:48.000000 phono3py-3.0.2/example/Si-TURBOMOLE/FORCES_FC3
--rw-r--r--   0 runner    (1001) docker     (127)     1195 2024-04-21 05:58:48.000000 phono3py-3.0.2/example/Si-TURBOMOLE/README
--rw-r--r--   0 runner    (1001) docker     (127)      253 2024-04-21 05:58:48.000000 phono3py-3.0.2/example/Si-TURBOMOLE/control
--rw-r--r--   0 runner    (1001) docker     (127)      492 2024-04-21 05:58:48.000000 phono3py-3.0.2/example/Si-TURBOMOLE/coord
--rw-r--r--   0 runner    (1001) docker     (127)   278495 2024-04-21 05:58:48.000000 phono3py-3.0.2/example/Si-TURBOMOLE/outputs.tar.gz
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 05:59:46.629300 phono3py-3.0.2/example/Wigner_La2Zr2O7/
--rw-r--r--   0 runner    (1001) docker     (127)      598 2024-04-21 05:58:48.000000 phono3py-3.0.2/example/Wigner_La2Zr2O7/BORN
--rw-r--r--   0 runner    (1001) docker     (127)     1598 2024-04-21 05:58:48.000000 phono3py-3.0.2/example/Wigner_La2Zr2O7/POSCAR
--rw-r--r--   0 runner    (1001) docker     (127)      197 2024-04-21 05:58:48.000000 phono3py-3.0.2/example/Wigner_La2Zr2O7/command.sh
--rw-r--r--   0 runner    (1001) docker     (127)  1098761 2024-04-21 05:58:48.000000 phono3py-3.0.2/example/Wigner_La2Zr2O7/fc2.hdf5
--rw-r--r--   0 runner    (1001) docker     (127)   339529 2024-04-21 05:58:48.000000 phono3py-3.0.2/example/Wigner_La2Zr2O7/kappa-m191919.hdf5
--rw-r--r--   0 runner    (1001) docker     (127)   160648 2024-04-21 05:58:48.000000 phono3py-3.0.2/example/Wigner_La2Zr2O7/tc_La2Zr2O7.out.xz
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 05:59:46.629300 phono3py-3.0.2/example/zb-ZnTe-PBEsol/
--rw-r--r--   0 runner    (1001) docker     (127)      551 2024-04-21 05:58:48.000000 phono3py-3.0.2/example/zb-ZnTe-PBEsol/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     4658 2024-04-21 05:58:48.000000 phono3py-3.0.2/example/zb-ZnTe-PBEsol/launch_phono3py_ZnTe_PBEsol_222.py
--rw-r--r--   0 runner    (1001) docker     (127)   131412 2024-04-21 05:58:48.000000 phono3py-3.0.2/example/zb-ZnTe-PBEsol/phono3py_params_ZnTe.yaml.xz
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 05:59:46.593300 phono3py-3.0.2/phono3py/
--rw-r--r--   0 runner    (1001) docker     (127)     1930 2024-04-21 05:58:48.000000 phono3py-3.0.2/phono3py/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5536 2024-04-21 05:58:48.000000 phono3py-3.0.2/phono3py/api_isotope.py
--rw-r--r--   0 runner    (1001) docker     (127)    11563 2024-04-21 05:58:48.000000 phono3py-3.0.2/phono3py/api_jointdos.py
--rw-r--r--   0 runner    (1001) docker     (127)    87780 2024-04-21 05:58:48.000000 phono3py-3.0.2/phono3py/api_phono3py.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 05:59:46.593300 phono3py-3.0.2/phono3py/conductivity/
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-04-21 05:58:48.000000 phono3py-3.0.2/phono3py/conductivity/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    31851 2024-04-21 05:58:48.000000 phono3py-3.0.2/phono3py/conductivity/base.py
--rw-r--r--   0 runner    (1001) docker     (127)    71606 2024-04-21 05:58:48.000000 phono3py-3.0.2/phono3py/conductivity/direct_solution.py
--rw-r--r--   0 runner    (1001) docker     (127)     5829 2024-04-21 05:58:48.000000 phono3py-3.0.2/phono3py/conductivity/kubo.py
--rw-r--r--   0 runner    (1001) docker     (127)    41437 2024-04-21 05:58:48.000000 phono3py-3.0.2/phono3py/conductivity/rta.py
--rw-r--r--   0 runner    (1001) docker     (127)    44752 2024-04-21 05:58:48.000000 phono3py-3.0.2/phono3py/conductivity/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     8629 2024-04-21 05:58:48.000000 phono3py-3.0.2/phono3py/conductivity/wigner.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 05:59:46.597300 phono3py-3.0.2/phono3py/cui/
--rw-r--r--   0 runner    (1001) docker     (127)       47 2024-04-21 05:58:48.000000 phono3py-3.0.2/phono3py/cui/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    20611 2024-04-21 05:58:48.000000 phono3py-3.0.2/phono3py/cui/create_force_constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     4797 2024-04-21 05:58:48.000000 phono3py-3.0.2/phono3py/cui/create_supercells.py
--rw-r--r--   0 runner    (1001) docker     (127)    14312 2024-04-21 05:58:48.000000 phono3py-3.0.2/phono3py/cui/kaccum_script.py
--rw-r--r--   0 runner    (1001) docker     (127)    24757 2024-04-21 05:58:48.000000 phono3py-3.0.2/phono3py/cui/load.py
--rw-r--r--   0 runner    (1001) docker     (127)    24731 2024-04-21 05:58:48.000000 phono3py-3.0.2/phono3py/cui/phono3py_argparse.py
--rw-r--r--   0 runner    (1001) docker     (127)    51088 2024-04-21 05:58:48.000000 phono3py-3.0.2/phono3py/cui/phono3py_script.py
--rw-r--r--   0 runner    (1001) docker     (127)    37210 2024-04-21 05:58:48.000000 phono3py-3.0.2/phono3py/cui/settings.py
--rw-r--r--   0 runner    (1001) docker     (127)     9786 2024-04-21 05:58:48.000000 phono3py-3.0.2/phono3py/cui/show_log.py
--rw-r--r--   0 runner    (1001) docker     (127)     5804 2024-04-21 05:58:48.000000 phono3py-3.0.2/phono3py/cui/triplets_info.py
--rw-r--r--   0 runner    (1001) docker     (127)    58029 2024-04-21 05:58:48.000000 phono3py-3.0.2/phono3py/file_IO.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 05:59:46.597300 phono3py-3.0.2/phono3py/interface/
--rw-r--r--   0 runner    (1001) docker     (127)       50 2024-04-21 05:58:48.000000 phono3py-3.0.2/phono3py/interface/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2058 2024-04-21 05:58:48.000000 phono3py-3.0.2/phono3py/interface/alm.py
--rw-r--r--   0 runner    (1001) docker     (127)     4273 2024-04-21 05:58:48.000000 phono3py-3.0.2/phono3py/interface/calculator.py
--rw-r--r--   0 runner    (1001) docker     (127)     3736 2024-04-21 05:58:48.000000 phono3py-3.0.2/phono3py/interface/fc_calculator.py
--rw-r--r--   0 runner    (1001) docker     (127)    22585 2024-04-21 05:58:48.000000 phono3py-3.0.2/phono3py/interface/phono3py_yaml.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 05:59:46.597300 phono3py-3.0.2/phono3py/other/
--rw-r--r--   0 runner    (1001) docker     (127)       40 2024-04-21 05:58:48.000000 phono3py-3.0.2/phono3py/other/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    14016 2024-04-21 05:58:48.000000 phono3py-3.0.2/phono3py/other/isotope.py
--rw-r--r--   0 runner    (1001) docker     (127)     9015 2024-04-21 05:58:48.000000 phono3py-3.0.2/phono3py/other/kaccum.py
--rw-r--r--   0 runner    (1001) docker     (127)     6998 2024-04-21 05:58:48.000000 phono3py-3.0.2/phono3py/other/tetrahedron_method.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 05:59:46.601300 phono3py-3.0.2/phono3py/phonon/
--rw-r--r--   0 runner    (1001) docker     (127)       55 2024-04-21 05:58:48.000000 phono3py-3.0.2/phono3py/phonon/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3290 2024-04-21 05:58:48.000000 phono3py-3.0.2/phono3py/phonon/func.py
--rw-r--r--   0 runner    (1001) docker     (127)    42765 2024-04-21 05:58:48.000000 phono3py-3.0.2/phono3py/phonon/grid.py
--rw-r--r--   0 runner    (1001) docker     (127)     7529 2024-04-21 05:58:48.000000 phono3py-3.0.2/phono3py/phonon/group_velocity_matrix.py
--rw-r--r--   0 runner    (1001) docker     (127)     2956 2024-04-21 05:58:48.000000 phono3py-3.0.2/phono3py/phonon/heat_capacity_matrix.py
--rw-r--r--   0 runner    (1001) docker     (127)     6688 2024-04-21 05:58:48.000000 phono3py-3.0.2/phono3py/phonon/solver.py
--rw-r--r--   0 runner    (1001) docker     (127)     9059 2024-04-21 05:58:48.000000 phono3py-3.0.2/phono3py/phonon/velocity_operator.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 05:59:46.601300 phono3py-3.0.2/phono3py/phonon3/
--rw-r--r--   0 runner    (1001) docker     (127)       42 2024-04-21 05:58:48.000000 phono3py-3.0.2/phono3py/phonon3/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11853 2024-04-21 05:58:48.000000 phono3py-3.0.2/phono3py/phonon3/collision_matrix.py
--rw-r--r--   0 runner    (1001) docker     (127)     3841 2024-04-21 05:58:48.000000 phono3py-3.0.2/phono3py/phonon3/dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)    14165 2024-04-21 05:58:48.000000 phono3py-3.0.2/phono3py/phonon3/displacement_fc3.py
--rw-r--r--   0 runner    (1001) docker     (127)    30148 2024-04-21 05:58:48.000000 phono3py-3.0.2/phono3py/phonon3/fc3.py
--rw-r--r--   0 runner    (1001) docker     (127)    18092 2024-04-21 05:58:48.000000 phono3py-3.0.2/phono3py/phonon3/gruneisen.py
--rw-r--r--   0 runner    (1001) docker     (127)    38050 2024-04-21 05:58:48.000000 phono3py-3.0.2/phono3py/phonon3/imag_self_energy.py
--rw-r--r--   0 runner    (1001) docker     (127)    37969 2024-04-21 05:58:48.000000 phono3py-3.0.2/phono3py/phonon3/interaction.py
--rw-r--r--   0 runner    (1001) docker     (127)    15753 2024-04-21 05:58:48.000000 phono3py-3.0.2/phono3py/phonon3/joint_dos.py
--rw-r--r--   0 runner    (1001) docker     (127)    25948 2024-04-21 05:58:48.000000 phono3py-3.0.2/phono3py/phonon3/real_self_energy.py
--rw-r--r--   0 runner    (1001) docker     (127)     4709 2024-04-21 05:58:48.000000 phono3py-3.0.2/phono3py/phonon3/real_to_reciprocal.py
--rw-r--r--   0 runner    (1001) docker     (127)     4239 2024-04-21 05:58:48.000000 phono3py-3.0.2/phono3py/phonon3/reciprocal_to_normal.py
--rw-r--r--   0 runner    (1001) docker     (127)    13786 2024-04-21 05:58:48.000000 phono3py-3.0.2/phono3py/phonon3/spectral_function.py
--rw-r--r--   0 runner    (1001) docker     (127)    14879 2024-04-21 05:58:48.000000 phono3py-3.0.2/phono3py/phonon3/triplets.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 05:59:46.601300 phono3py-3.0.2/phono3py/sscha/
--rw-r--r--   0 runner    (1001) docker     (127)       26 2024-04-21 05:58:48.000000 phono3py-3.0.2/phono3py/sscha/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    19518 2024-04-21 05:58:48.000000 phono3py-3.0.2/phono3py/sscha/sscha.py
--rw-r--r--   0 runner    (1001) docker     (127)     1637 2024-04-21 05:58:48.000000 phono3py-3.0.2/phono3py/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 05:59:46.641300 phono3py-3.0.2/phono3py.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      451 2024-04-21 05:59:46.000000 phono3py-3.0.2/phono3py.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     6255 2024-04-21 05:59:46.000000 phono3py-3.0.2/phono3py.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-21 05:59:46.000000 phono3py-3.0.2/phono3py.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       92 2024-04-21 05:59:46.000000 phono3py-3.0.2/phono3py.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-21 05:59:46.000000 phono3py-3.0.2/phono3py.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      298 2024-04-21 05:58:48.000000 phono3py-3.0.2/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 05:59:46.633300 phono3py-3.0.2/scripts/
--rwxr-xr-x   0 runner    (1001) docker     (127)     1831 2024-04-21 05:58:48.000000 phono3py-3.0.2/scripts/phono3py
--rwxr-xr-x   0 runner    (1001) docker     (127)     3845 2024-04-21 05:58:48.000000 phono3py-3.0.2/scripts/phono3py-coleigplot
--rwxr-xr-x   0 runner    (1001) docker     (127)     1688 2024-04-21 05:58:48.000000 phono3py-3.0.2/scripts/phono3py-kaccum
--rwxr-xr-x   0 runner    (1001) docker     (127)     9488 2024-04-21 05:58:48.000000 phono3py-3.0.2/scripts/phono3py-kdeplot
--rwxr-xr-x   0 runner    (1001) docker     (127)     1797 2024-04-21 05:58:48.000000 phono3py-3.0.2/scripts/phono3py-load
--rw-r--r--   0 runner    (1001) docker     (127)      120 2024-04-21 05:59:46.641300 phono3py-3.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)    10421 2024-04-21 05:58:48.000000 phono3py-3.0.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 05:59:46.637300 phono3py-3.0.2/test/
--rw-r--r--   0 runner    (1001) docker     (127)     1236 2024-04-21 05:58:48.000000 phono3py-3.0.2/test/AgNO2_cell.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      133 2024-04-21 05:58:48.000000 phono3py-3.0.2/test/BORN_NaCl
--rw-r--r--   0 runner    (1001) docker     (127)   357907 2024-04-21 05:58:48.000000 phono3py-3.0.2/test/FORCES_FC3_si_pbesol
--rw-r--r--   0 runner    (1001) docker     (127)     6282 2024-04-21 05:58:48.000000 phono3py-3.0.2/test/FORCE_SETS_NaCl
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 05:59:46.637300 phono3py-3.0.2/test/api/
--rw-r--r--   0 runner    (1001) docker     (127)     1125 2024-04-21 05:58:48.000000 phono3py-3.0.2/test/api/test_api_phono3py.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 05:59:46.637300 phono3py-3.0.2/test/conductivity/
--rw-r--r--   0 runner    (1001) docker     (127)       39 2024-04-21 05:58:48.000000 phono3py-3.0.2/test/conductivity/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2696 2024-04-21 05:58:48.000000 phono3py-3.0.2/test/conductivity/test_kappa_LBTE.py
--rw-r--r--   0 runner    (1001) docker     (127)     1943 2024-04-21 05:58:48.000000 phono3py-3.0.2/test/conductivity/test_kappa_LBTE_Wigner.py
--rw-r--r--   0 runner    (1001) docker     (127)    12437 2024-04-21 05:58:48.000000 phono3py-3.0.2/test/conductivity/test_kappa_RTA.py
--rw-r--r--   0 runner    (1001) docker     (127)    12309 2024-04-21 05:58:48.000000 phono3py-3.0.2/test/conductivity/test_kappa_RTA_Wigner.py
--rw-r--r--   0 runner    (1001) docker     (127)    12947 2024-04-21 05:58:48.000000 phono3py-3.0.2/test/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 05:59:46.637300 phono3py-3.0.2/test/cui/
--rw-r--r--   0 runner    (1001) docker     (127)    62552 2024-04-21 05:58:48.000000 phono3py-3.0.2/test/cui/phono3py_params-qe-Si222.yaml.xz
--rw-r--r--   0 runner    (1001) docker     (127)     4847 2024-04-21 05:58:48.000000 phono3py-3.0.2/test/cui/test_phono3py_load_script.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 05:59:46.637300 phono3py-3.0.2/test/file_IO/
--rw-r--r--   0 runner    (1001) docker     (127)     2310 2024-04-21 05:58:48.000000 phono3py-3.0.2/test/file_IO/test_file_IO.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 05:59:46.637300 phono3py-3.0.2/test/interface/
--rw-r--r--   0 runner    (1001) docker     (127)     4558 2024-04-21 05:58:48.000000 phono3py-3.0.2/test/interface/test_phono3py_yaml.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 05:59:46.641300 phono3py-3.0.2/test/other/
--rw-r--r--   0 runner    (1001) docker     (127)       37 2024-04-21 05:58:48.000000 phono3py-3.0.2/test/other/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3871 2024-04-21 05:58:48.000000 phono3py-3.0.2/test/other/test_isotope.py
--rw-r--r--   0 runner    (1001) docker     (127)    14548 2024-04-21 05:58:48.000000 phono3py-3.0.2/test/other/test_kaccum.py
--rw-r--r--   0 runner    (1001) docker     (127)   177468 2024-04-21 05:58:48.000000 phono3py-3.0.2/test/phono3py_params-Si111-rd.yaml.xz
--rw-r--r--   0 runner    (1001) docker     (127)   943848 2024-04-21 05:58:48.000000 phono3py-3.0.2/test/phono3py_params_AlN332.yaml.xz
--rw-r--r--   0 runner    (1001) docker     (127)    26352 2024-04-21 05:58:48.000000 phono3py-3.0.2/test/phono3py_params_NaCl111.yaml
--rw-r--r--   0 runner    (1001) docker     (127)    69120 2024-04-21 05:58:48.000000 phono3py-3.0.2/test/phono3py_params_NaCl222.yaml.xz
--rw-r--r--   0 runner    (1001) docker     (127)    30693 2024-04-21 05:58:48.000000 phono3py-3.0.2/test/phono3py_params_Si-111-222.yaml
--rw-r--r--   0 runner    (1001) docker     (127)    18216 2024-04-21 05:58:48.000000 phono3py-3.0.2/test/phono3py_params_Si111.yaml
--rw-r--r--   0 runner    (1001) docker     (127)    32800 2024-04-21 05:58:48.000000 phono3py-3.0.2/test/phono3py_si_pbesol.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 05:59:46.641300 phono3py-3.0.2/test/phonon/
--rw-r--r--   0 runner    (1001) docker     (127)       50 2024-04-21 05:58:48.000000 phono3py-3.0.2/test/phonon/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    51828 2024-04-21 05:58:48.000000 phono3py-3.0.2/test/phonon/test_grid.py
--rw-r--r--   0 runner    (1001) docker     (127)    19747 2024-04-21 05:58:48.000000 phono3py-3.0.2/test/phonon/test_velocity_operator.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 05:59:46.641300 phono3py-3.0.2/test/phonon3/
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-04-21 05:58:48.000000 phono3py-3.0.2/test/phonon3/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4142 2024-04-21 05:58:48.000000 phono3py-3.0.2/test/phonon3/test_displacements.py
--rw-r--r--   0 runner    (1001) docker     (127)    11450 2024-04-21 05:58:48.000000 phono3py-3.0.2/test/phonon3/test_fc3.py
--rw-r--r--   0 runner    (1001) docker     (127)    47987 2024-04-21 05:58:48.000000 phono3py-3.0.2/test/phonon3/test_imag_self_energy.py
--rw-r--r--   0 runner    (1001) docker     (127)    11113 2024-04-21 05:58:48.000000 phono3py-3.0.2/test/phonon3/test_interaction.py
--rw-r--r--   0 runner    (1001) docker     (127)    11546 2024-04-21 05:58:48.000000 phono3py-3.0.2/test/phonon3/test_joint_dos.py
--rw-r--r--   0 runner    (1001) docker     (127)    19498 2024-04-21 05:58:48.000000 phono3py-3.0.2/test/phonon3/test_real_self_energy.py
--rw-r--r--   0 runner    (1001) docker     (127)    19561 2024-04-21 05:58:48.000000 phono3py-3.0.2/test/phonon3/test_spectral_function.py
--rw-r--r--   0 runner    (1001) docker     (127)    41126 2024-04-21 05:58:48.000000 phono3py-3.0.2/test/phonon3/test_triplets.py
--rw-r--r--   0 runner    (1001) docker     (127)    12203 2024-04-21 05:58:48.000000 phono3py-3.0.2/test/phonopy_disp_NaCl.yaml
--rw-r--r--   0 runner    (1001) docker     (127)   286407 2024-04-21 05:58:48.000000 phono3py-3.0.2/test/phonopy_params-Si111-iterha.yaml.gz
--rw-r--r--   0 runner    (1001) docker     (127)     5587 2024-04-21 05:58:48.000000 phono3py-3.0.2/test/phonopy_params_Si.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 05:59:46.641300 phono3py-3.0.2/test/sscha/
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-04-21 05:58:48.000000 phono3py-3.0.2/test/sscha/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8801 2024-04-21 05:58:48.000000 phono3py-3.0.2/test/sscha/test_sscha.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 07:43:29.205348 phono3py-3.0.3/
+-rw-r--r--   0 runner    (1001) docker     (127)     1470 2024-05-04 07:42:36.000000 phono3py-3.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      120 2024-05-04 07:42:36.000000 phono3py-3.0.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)      451 2024-05-04 07:43:29.205348 phono3py-3.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2446 2024-05-04 07:42:36.000000 phono3py-3.0.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-04 07:43:24.000000 phono3py-3.0.3/__nanoversion__.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 07:43:29.169347 phono3py-3.0.3/c/
+-rw-r--r--   0 runner    (1001) docker     (127)    68786 2024-05-04 07:42:36.000000 phono3py-3.0.3/c/_phono3py.c
+-rw-r--r--   0 runner    (1001) docker     (127)     8081 2024-05-04 07:42:36.000000 phono3py-3.0.3/c/_phononcalc.c
+-rw-r--r--   0 runner    (1001) docker     (127)    15045 2024-05-04 07:42:36.000000 phono3py-3.0.3/c/bzgrid.c
+-rw-r--r--   0 runner    (1001) docker     (127)     3674 2024-05-04 07:42:36.000000 phono3py-3.0.3/c/bzgrid.h
+-rw-r--r--   0 runner    (1001) docker     (127)    12441 2024-05-04 07:42:36.000000 phono3py-3.0.3/c/collision_matrix.c
+-rw-r--r--   0 runner    (1001) docker     (127)     2584 2024-05-04 07:42:36.000000 phono3py-3.0.3/c/collision_matrix.h
+-rw-r--r--   0 runner    (1001) docker     (127)    29801 2024-05-04 07:42:36.000000 phono3py-3.0.3/c/dynmat.c
+-rw-r--r--   0 runner    (1001) docker     (127)     5149 2024-05-04 07:42:36.000000 phono3py-3.0.3/c/dynmat.h
+-rw-r--r--   0 runner    (1001) docker     (127)    23953 2024-05-04 07:42:36.000000 phono3py-3.0.3/c/fc3.c
+-rw-r--r--   0 runner    (1001) docker     (127)     2805 2024-05-04 07:42:36.000000 phono3py-3.0.3/c/fc3.h
+-rw-r--r--   0 runner    (1001) docker     (127)    15184 2024-05-04 07:42:36.000000 phono3py-3.0.3/c/grgrid.c
+-rw-r--r--   0 runner    (1001) docker     (127)     3392 2024-05-04 07:42:36.000000 phono3py-3.0.3/c/grgrid.h
+-rw-r--r--   0 runner    (1001) docker     (127)    11554 2024-05-04 07:42:36.000000 phono3py-3.0.3/c/gridsys.c
+-rw-r--r--   0 runner    (1001) docker     (127)    13923 2024-05-04 07:42:36.000000 phono3py-3.0.3/c/gridsys.h
+-rw-r--r--   0 runner    (1001) docker     (127)    16545 2024-05-04 07:42:36.000000 phono3py-3.0.3/c/imag_self_energy_with_g.c
+-rw-r--r--   0 runner    (1001) docker     (127)     3183 2024-05-04 07:42:36.000000 phono3py-3.0.3/c/imag_self_energy_with_g.h
+-rw-r--r--   0 runner    (1001) docker     (127)    12188 2024-05-04 07:42:36.000000 phono3py-3.0.3/c/interaction.c
+-rw-r--r--   0 runner    (1001) docker     (127)     2951 2024-05-04 07:42:36.000000 phono3py-3.0.3/c/interaction.h
+-rw-r--r--   0 runner    (1001) docker     (127)     9128 2024-05-04 07:42:36.000000 phono3py-3.0.3/c/isotope.c
+-rw-r--r--   0 runner    (1001) docker     (127)     2588 2024-05-04 07:42:36.000000 phono3py-3.0.3/c/isotope.h
+-rw-r--r--   0 runner    (1001) docker     (127)     8032 2024-05-04 07:42:36.000000 phono3py-3.0.3/c/lagrid.c
+-rw-r--r--   0 runner    (1001) docker     (127)     3487 2024-05-04 07:42:36.000000 phono3py-3.0.3/c/lagrid.h
+-rw-r--r--   0 runner    (1001) docker     (127)     9063 2024-05-04 07:42:36.000000 phono3py-3.0.3/c/lapack_wrapper.c
+-rw-r--r--   0 runner    (1001) docker     (127)     2975 2024-05-04 07:42:36.000000 phono3py-3.0.3/c/lapack_wrapper.h
+-rw-r--r--   0 runner    (1001) docker     (127)    14541 2024-05-04 07:42:36.000000 phono3py-3.0.3/c/niggli.c
+-rw-r--r--   0 runner    (1001) docker     (127)     2109 2024-05-04 07:42:36.000000 phono3py-3.0.3/c/niggli.h
+-rw-r--r--   0 runner    (1001) docker     (127)    32268 2024-05-04 07:42:36.000000 phono3py-3.0.3/c/phono3py.c
+-rw-r--r--   0 runner    (1001) docker     (127)    14077 2024-05-04 07:42:36.000000 phono3py-3.0.3/c/phono3py.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1986 2024-05-04 07:42:36.000000 phono3py-3.0.3/c/phonoc_array.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1813 2024-05-04 07:42:36.000000 phono3py-3.0.3/c/phonoc_const.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2199 2024-05-04 07:42:36.000000 phono3py-3.0.3/c/phonoc_utils.c
+-rw-r--r--   0 runner    (1001) docker     (127)     1935 2024-05-04 07:42:36.000000 phono3py-3.0.3/c/phonoc_utils.h
+-rw-r--r--   0 runner    (1001) docker     (127)    20519 2024-05-04 07:42:36.000000 phono3py-3.0.3/c/phonon.c
+-rw-r--r--   0 runner    (1001) docker     (127)     3324 2024-05-04 07:42:36.000000 phono3py-3.0.3/c/phonon.h
+-rw-r--r--   0 runner    (1001) docker     (127)     3514 2024-05-04 07:42:36.000000 phono3py-3.0.3/c/phononcalc.c
+-rw-r--r--   0 runner    (1001) docker     (127)     2661 2024-05-04 07:42:36.000000 phono3py-3.0.3/c/phononcalc.h
+-rw-r--r--   0 runner    (1001) docker     (127)    11627 2024-05-04 07:42:36.000000 phono3py-3.0.3/c/pp_collision.c
+-rw-r--r--   0 runner    (1001) docker     (127)     3036 2024-05-04 07:42:36.000000 phono3py-3.0.3/c/pp_collision.h
+-rw-r--r--   0 runner    (1001) docker     (127)     9296 2024-05-04 07:42:36.000000 phono3py-3.0.3/c/real_self_energy.c
+-rw-r--r--   0 runner    (1001) docker     (127)     2514 2024-05-04 07:42:36.000000 phono3py-3.0.3/c/real_self_energy.h
+-rw-r--r--   0 runner    (1001) docker     (127)    16752 2024-05-04 07:42:36.000000 phono3py-3.0.3/c/real_to_reciprocal.c
+-rw-r--r--   0 runner    (1001) docker     (127)     2362 2024-05-04 07:42:36.000000 phono3py-3.0.3/c/real_to_reciprocal.h
+-rw-r--r--   0 runner    (1001) docker     (127)    12160 2024-05-04 07:42:36.000000 phono3py-3.0.3/c/reciprocal_to_normal.c
+-rw-r--r--   0 runner    (1001) docker     (127)     2294 2024-05-04 07:42:36.000000 phono3py-3.0.3/c/reciprocal_to_normal.h
+-rw-r--r--   0 runner    (1001) docker     (127)    14689 2024-05-04 07:42:36.000000 phono3py-3.0.3/c/snf3x3.c
+-rw-r--r--   0 runner    (1001) docker     (127)      267 2024-05-04 07:42:36.000000 phono3py-3.0.3/c/snf3x3.h
+-rw-r--r--   0 runner    (1001) docker     (127)    38926 2024-05-04 07:42:36.000000 phono3py-3.0.3/c/tetrahedron_method.c
+-rw-r--r--   0 runner    (1001) docker     (127)     2295 2024-05-04 07:42:36.000000 phono3py-3.0.3/c/tetrahedron_method.h
+-rw-r--r--   0 runner    (1001) docker     (127)     5933 2024-05-04 07:42:36.000000 phono3py-3.0.3/c/triplet.c
+-rw-r--r--   0 runner    (1001) docker     (127)     4134 2024-05-04 07:42:36.000000 phono3py-3.0.3/c/triplet.h
+-rw-r--r--   0 runner    (1001) docker     (127)    18558 2024-05-04 07:42:36.000000 phono3py-3.0.3/c/triplet_grid.c
+-rw-r--r--   0 runner    (1001) docker     (127)     2464 2024-05-04 07:42:36.000000 phono3py-3.0.3/c/triplet_grid.h
+-rw-r--r--   0 runner    (1001) docker     (127)    13656 2024-05-04 07:42:36.000000 phono3py-3.0.3/c/triplet_iw.c
+-rw-r--r--   0 runner    (1001) docker     (127)     2871 2024-05-04 07:42:36.000000 phono3py-3.0.3/c/triplet_iw.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 07:43:29.141347 phono3py-3.0.3/example/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 07:43:29.173347 phono3py-3.0.3/example/AlN-LDA/
+-rw-r--r--   0 runner    (1001) docker     (127)      357 2024-05-04 07:42:36.000000 phono3py-3.0.3/example/AlN-LDA/BORN
+-rw-r--r--   0 runner    (1001) docker     (127)    86886 2024-05-04 07:42:36.000000 phono3py-3.0.3/example/AlN-LDA/FORCES_FC2
+-rw-r--r--   0 runner    (1001) docker     (127)   862253 2024-05-04 07:42:36.000000 phono3py-3.0.3/example/AlN-LDA/FORCES_FC3.lzma
+-rw-r--r--   0 runner    (1001) docker     (127)      487 2024-05-04 07:42:36.000000 phono3py-3.0.3/example/AlN-LDA/POSCAR-unitcell
+-rw-r--r--   0 runner    (1001) docker     (127)     2399 2024-05-04 07:42:36.000000 phono3py-3.0.3/example/AlN-LDA/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)   143873 2024-05-04 07:42:36.000000 phono3py-3.0.3/example/AlN-LDA/phono3py_disp.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)   176702 2024-05-04 07:42:36.000000 phono3py-3.0.3/example/AlN-LDA/phono3py_disp_dimfc2.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 07:43:29.173347 phono3py-3.0.3/example/NaCl-alm/
+-rw-r--r--   0 runner    (1001) docker     (127)     1429 2024-05-04 07:42:36.000000 phono3py-3.0.3/example/NaCl-alm/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)   303332 2024-05-04 07:42:36.000000 phono3py-3.0.3/example/NaCl-alm/phono3py_params_NaCl222.yaml.xz
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 07:43:29.173347 phono3py-3.0.3/example/Si-CRYSTAL/
+-rw-r--r--   0 runner    (1001) docker     (127)     6225 2024-05-04 07:42:36.000000 phono3py-3.0.3/example/Si-CRYSTAL/FORCES_FC2
+-rw-r--r--   0 runner    (1001) docker     (127)    52417 2024-05-04 07:42:36.000000 phono3py-3.0.3/example/Si-CRYSTAL/FORCES_FC3
+-rw-r--r--   0 runner    (1001) docker     (127)     1213 2024-05-04 07:42:36.000000 phono3py-3.0.3/example/Si-CRYSTAL/README
+-rw-r--r--   0 runner    (1001) docker     (127)      815 2024-05-04 07:42:36.000000 phono3py-3.0.3/example/Si-CRYSTAL/TEMPLATE
+-rw-r--r--   0 runner    (1001) docker     (127)      815 2024-05-04 07:42:36.000000 phono3py-3.0.3/example/Si-CRYSTAL/TEMPLATE3
+-rw-r--r--   0 runner    (1001) docker     (127)    50060 2024-05-04 07:42:36.000000 phono3py-3.0.3/example/Si-CRYSTAL/crystal.o
+-rw-r--r--   0 runner    (1001) docker     (127)   801243 2024-05-04 07:42:36.000000 phono3py-3.0.3/example/Si-CRYSTAL/outputs.tar.gz
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 07:43:29.177348 phono3py-3.0.3/example/Si-LDA/
+-rw-r--r--   0 runner    (1001) docker     (127)   357907 2024-05-04 07:42:36.000000 phono3py-3.0.3/example/Si-LDA/FORCES_FC3
+-rw-r--r--   0 runner    (1001) docker     (127)      727 2024-05-04 07:42:36.000000 phono3py-3.0.3/example/Si-LDA/POSCAR-unitcell
+-rw-r--r--   0 runner    (1001) docker     (127)     1293 2024-05-04 07:42:36.000000 phono3py-3.0.3/example/Si-LDA/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)    32796 2024-05-04 07:42:36.000000 phono3py-3.0.3/example/Si-LDA/phono3py_disp.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)   305364 2024-05-04 07:42:36.000000 phono3py-3.0.3/example/Si-LDA/vasprun_xmls.tar.lzma
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 07:43:29.181347 phono3py-3.0.3/example/Si-PBE/
+-rw-r--r--   0 runner    (1001) docker     (127)   357907 2024-05-04 07:42:36.000000 phono3py-3.0.3/example/Si-PBE/FORCES_FC3
+-rw-r--r--   0 runner    (1001) docker     (127)      727 2024-05-04 07:42:36.000000 phono3py-3.0.3/example/Si-PBE/POSCAR-unitcell
+-rw-r--r--   0 runner    (1001) docker     (127)     1293 2024-05-04 07:42:36.000000 phono3py-3.0.3/example/Si-PBE/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)    32796 2024-05-04 07:42:36.000000 phono3py-3.0.3/example/Si-PBE/phono3py_disp.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)   314724 2024-05-04 07:42:36.000000 phono3py-3.0.3/example/Si-PBE/vasprun_xmls.tar.lzma
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 07:43:29.181347 phono3py-3.0.3/example/Si-PBEsol/
+-rw-r--r--   0 runner    (1001) docker     (127)   357907 2024-05-04 07:42:36.000000 phono3py-3.0.3/example/Si-PBEsol/FORCES_FC3
+-rw-r--r--   0 runner    (1001) docker     (127)      727 2024-05-04 07:42:36.000000 phono3py-3.0.3/example/Si-PBEsol/POSCAR-unitcell
+-rw-r--r--   0 runner    (1001) docker     (127)     2844 2024-05-04 07:42:36.000000 phono3py-3.0.3/example/Si-PBEsol/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)    46793 2024-05-04 07:42:36.000000 phono3py-3.0.3/example/Si-PBEsol/Si-band-DOS.png
+-rw-r--r--   0 runner    (1001) docker     (127)    28346 2024-05-04 07:42:36.000000 phono3py-3.0.3/example/Si-PBEsol/Si-kaccum.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1029 2024-05-04 07:42:36.000000 phono3py-3.0.3/example/Si-PBEsol/Si.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32796 2024-05-04 07:42:36.000000 phono3py-3.0.3/example/Si-PBEsol/phono3py_disp.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)    95766 2024-05-04 07:42:36.000000 phono3py-3.0.3/example/Si-PBEsol/phono3py_disp_dimfc2.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 07:43:29.141347 phono3py-3.0.3/example/Si-PBEsol/vasprun_xml_fc2/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 07:43:29.185347 phono3py-3.0.3/example/Si-PBEsol/vasprun_xml_fc2/disp-fc2-00001/
+-rw-r--r--   0 runner    (1001) docker     (127)      267 2024-05-04 07:42:36.000000 phono3py-3.0.3/example/Si-PBEsol/vasprun_xml_fc2/disp-fc2-00001/INCAR
+-rw-r--r--   0 runner    (1001) docker     (127)    31479 2024-05-04 07:42:36.000000 phono3py-3.0.3/example/Si-PBEsol/vasprun_xml_fc2/disp-fc2-00001/POSCAR
+-rw-r--r--   0 runner    (1001) docker     (127)   291058 2024-05-04 07:42:36.000000 phono3py-3.0.3/example/Si-PBEsol/vasprun_xml_fc2/disp-fc2-00001/vasprun.xml
+-rw-r--r--   0 runner    (1001) docker     (127)   300636 2024-05-04 07:42:36.000000 phono3py-3.0.3/example/Si-PBEsol/vasprun_xmls.tar.lzma
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 07:43:29.185347 phono3py-3.0.3/example/Si-QE/
+-rw-r--r--   0 runner    (1001) docker     (127)   357907 2024-05-04 07:42:36.000000 phono3py-3.0.3/example/Si-QE/FORCES_FC3
+-rw-r--r--   0 runner    (1001) docker     (127)     1039 2024-05-04 07:42:36.000000 phono3py-3.0.3/example/Si-QE/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1025 2024-05-04 07:42:36.000000 phono3py-3.0.3/example/Si-QE/Si.in
+-rw-r--r--   0 runner    (1001) docker     (127)    32833 2024-05-04 07:42:36.000000 phono3py-3.0.3/example/Si-QE/phono3py_disp.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)   150928 2024-05-04 07:42:36.000000 phono3py-3.0.3/example/Si-QE/supercell_out.tar.lzma
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 07:43:29.189348 phono3py-3.0.3/example/Si-TURBOMOLE/
+-rw-r--r--   0 runner    (1001) docker     (127)    10449 2024-05-04 07:42:36.000000 phono3py-3.0.3/example/Si-TURBOMOLE/FORCES_FC2
+-rw-r--r--   0 runner    (1001) docker     (127)   357907 2024-05-04 07:42:36.000000 phono3py-3.0.3/example/Si-TURBOMOLE/FORCES_FC3
+-rw-r--r--   0 runner    (1001) docker     (127)     1195 2024-05-04 07:42:36.000000 phono3py-3.0.3/example/Si-TURBOMOLE/README
+-rw-r--r--   0 runner    (1001) docker     (127)      253 2024-05-04 07:42:36.000000 phono3py-3.0.3/example/Si-TURBOMOLE/control
+-rw-r--r--   0 runner    (1001) docker     (127)      492 2024-05-04 07:42:36.000000 phono3py-3.0.3/example/Si-TURBOMOLE/coord
+-rw-r--r--   0 runner    (1001) docker     (127)   278495 2024-05-04 07:42:36.000000 phono3py-3.0.3/example/Si-TURBOMOLE/outputs.tar.gz
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 07:43:29.189348 phono3py-3.0.3/example/Wigner_La2Zr2O7/
+-rw-r--r--   0 runner    (1001) docker     (127)      598 2024-05-04 07:42:36.000000 phono3py-3.0.3/example/Wigner_La2Zr2O7/BORN
+-rw-r--r--   0 runner    (1001) docker     (127)     1598 2024-05-04 07:42:36.000000 phono3py-3.0.3/example/Wigner_La2Zr2O7/POSCAR
+-rw-r--r--   0 runner    (1001) docker     (127)      197 2024-05-04 07:42:36.000000 phono3py-3.0.3/example/Wigner_La2Zr2O7/command.sh
+-rw-r--r--   0 runner    (1001) docker     (127)  1098761 2024-05-04 07:42:36.000000 phono3py-3.0.3/example/Wigner_La2Zr2O7/fc2.hdf5
+-rw-r--r--   0 runner    (1001) docker     (127)   339529 2024-05-04 07:42:36.000000 phono3py-3.0.3/example/Wigner_La2Zr2O7/kappa-m191919.hdf5
+-rw-r--r--   0 runner    (1001) docker     (127)   160648 2024-05-04 07:42:36.000000 phono3py-3.0.3/example/Wigner_La2Zr2O7/tc_La2Zr2O7.out.xz
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 07:43:29.193348 phono3py-3.0.3/example/zb-ZnTe-PBEsol/
+-rw-r--r--   0 runner    (1001) docker     (127)      551 2024-05-04 07:42:36.000000 phono3py-3.0.3/example/zb-ZnTe-PBEsol/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     4658 2024-05-04 07:42:36.000000 phono3py-3.0.3/example/zb-ZnTe-PBEsol/launch_phono3py_ZnTe_PBEsol_222.py
+-rw-r--r--   0 runner    (1001) docker     (127)   131412 2024-05-04 07:42:36.000000 phono3py-3.0.3/example/zb-ZnTe-PBEsol/phono3py_params_ZnTe.yaml.xz
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 07:43:29.149347 phono3py-3.0.3/phono3py/
+-rw-r--r--   0 runner    (1001) docker     (127)     1930 2024-05-04 07:42:36.000000 phono3py-3.0.3/phono3py/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5536 2024-05-04 07:42:36.000000 phono3py-3.0.3/phono3py/api_isotope.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11563 2024-05-04 07:42:36.000000 phono3py-3.0.3/phono3py/api_jointdos.py
+-rw-r--r--   0 runner    (1001) docker     (127)    93292 2024-05-04 07:42:36.000000 phono3py-3.0.3/phono3py/api_phono3py.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 07:43:29.149347 phono3py-3.0.3/phono3py/conductivity/
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-05-04 07:42:36.000000 phono3py-3.0.3/phono3py/conductivity/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31851 2024-05-04 07:42:36.000000 phono3py-3.0.3/phono3py/conductivity/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)    71606 2024-05-04 07:42:36.000000 phono3py-3.0.3/phono3py/conductivity/direct_solution.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5829 2024-05-04 07:42:36.000000 phono3py-3.0.3/phono3py/conductivity/kubo.py
+-rw-r--r--   0 runner    (1001) docker     (127)    41437 2024-05-04 07:42:36.000000 phono3py-3.0.3/phono3py/conductivity/rta.py
+-rw-r--r--   0 runner    (1001) docker     (127)    44752 2024-05-04 07:42:36.000000 phono3py-3.0.3/phono3py/conductivity/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8629 2024-05-04 07:42:36.000000 phono3py-3.0.3/phono3py/conductivity/wigner.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 07:43:29.153347 phono3py-3.0.3/phono3py/cui/
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-05-04 07:42:36.000000 phono3py-3.0.3/phono3py/cui/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20611 2024-05-04 07:42:36.000000 phono3py-3.0.3/phono3py/cui/create_force_constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14183 2024-05-04 07:42:36.000000 phono3py-3.0.3/phono3py/cui/create_force_sets.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4798 2024-05-04 07:42:36.000000 phono3py-3.0.3/phono3py/cui/create_supercells.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14312 2024-05-04 07:42:36.000000 phono3py-3.0.3/phono3py/cui/kaccum_script.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24835 2024-05-04 07:42:36.000000 phono3py-3.0.3/phono3py/cui/load.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24961 2024-05-04 07:42:36.000000 phono3py-3.0.3/phono3py/cui/phono3py_argparse.py
+-rw-r--r--   0 runner    (1001) docker     (127)    42636 2024-05-04 07:42:36.000000 phono3py-3.0.3/phono3py/cui/phono3py_script.py
+-rw-r--r--   0 runner    (1001) docker     (127)    37210 2024-05-04 07:42:36.000000 phono3py-3.0.3/phono3py/cui/settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9786 2024-05-04 07:42:36.000000 phono3py-3.0.3/phono3py/cui/show_log.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5804 2024-05-04 07:42:36.000000 phono3py-3.0.3/phono3py/cui/triplets_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)    58029 2024-05-04 07:42:36.000000 phono3py-3.0.3/phono3py/file_IO.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 07:43:29.153347 phono3py-3.0.3/phono3py/interface/
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-05-04 07:42:36.000000 phono3py-3.0.3/phono3py/interface/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2058 2024-05-04 07:42:36.000000 phono3py-3.0.3/phono3py/interface/alm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4273 2024-05-04 07:42:36.000000 phono3py-3.0.3/phono3py/interface/calculator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3736 2024-05-04 07:42:36.000000 phono3py-3.0.3/phono3py/interface/fc_calculator.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22947 2024-05-04 07:42:36.000000 phono3py-3.0.3/phono3py/interface/phono3py_yaml.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 07:43:29.153347 phono3py-3.0.3/phono3py/other/
+-rw-r--r--   0 runner    (1001) docker     (127)       40 2024-05-04 07:42:36.000000 phono3py-3.0.3/phono3py/other/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14016 2024-05-04 07:42:36.000000 phono3py-3.0.3/phono3py/other/isotope.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9015 2024-05-04 07:42:36.000000 phono3py-3.0.3/phono3py/other/kaccum.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6998 2024-05-04 07:42:36.000000 phono3py-3.0.3/phono3py/other/tetrahedron_method.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 07:43:29.153347 phono3py-3.0.3/phono3py/phonon/
+-rw-r--r--   0 runner    (1001) docker     (127)       55 2024-05-04 07:42:36.000000 phono3py-3.0.3/phono3py/phonon/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3290 2024-05-04 07:42:36.000000 phono3py-3.0.3/phono3py/phonon/func.py
+-rw-r--r--   0 runner    (1001) docker     (127)    42765 2024-05-04 07:42:36.000000 phono3py-3.0.3/phono3py/phonon/grid.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7529 2024-05-04 07:42:36.000000 phono3py-3.0.3/phono3py/phonon/group_velocity_matrix.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2956 2024-05-04 07:42:36.000000 phono3py-3.0.3/phono3py/phonon/heat_capacity_matrix.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6688 2024-05-04 07:42:36.000000 phono3py-3.0.3/phono3py/phonon/solver.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9059 2024-05-04 07:42:36.000000 phono3py-3.0.3/phono3py/phonon/velocity_operator.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 07:43:29.157347 phono3py-3.0.3/phono3py/phonon3/
+-rw-r--r--   0 runner    (1001) docker     (127)       42 2024-05-04 07:42:36.000000 phono3py-3.0.3/phono3py/phonon3/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11853 2024-05-04 07:42:36.000000 phono3py-3.0.3/phono3py/phonon3/collision_matrix.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3841 2024-05-04 07:42:36.000000 phono3py-3.0.3/phono3py/phonon3/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14165 2024-05-04 07:42:36.000000 phono3py-3.0.3/phono3py/phonon3/displacement_fc3.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30148 2024-05-04 07:42:36.000000 phono3py-3.0.3/phono3py/phonon3/fc3.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18092 2024-05-04 07:42:36.000000 phono3py-3.0.3/phono3py/phonon3/gruneisen.py
+-rw-r--r--   0 runner    (1001) docker     (127)    38050 2024-05-04 07:42:36.000000 phono3py-3.0.3/phono3py/phonon3/imag_self_energy.py
+-rw-r--r--   0 runner    (1001) docker     (127)    37969 2024-05-04 07:42:36.000000 phono3py-3.0.3/phono3py/phonon3/interaction.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15753 2024-05-04 07:42:36.000000 phono3py-3.0.3/phono3py/phonon3/joint_dos.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25948 2024-05-04 07:42:36.000000 phono3py-3.0.3/phono3py/phonon3/real_self_energy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4709 2024-05-04 07:42:36.000000 phono3py-3.0.3/phono3py/phonon3/real_to_reciprocal.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4239 2024-05-04 07:42:36.000000 phono3py-3.0.3/phono3py/phonon3/reciprocal_to_normal.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13786 2024-05-04 07:42:36.000000 phono3py-3.0.3/phono3py/phonon3/spectral_function.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14879 2024-05-04 07:42:36.000000 phono3py-3.0.3/phono3py/phonon3/triplets.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 07:43:29.157347 phono3py-3.0.3/phono3py/sscha/
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-05-04 07:42:36.000000 phono3py-3.0.3/phono3py/sscha/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19518 2024-05-04 07:42:36.000000 phono3py-3.0.3/phono3py/sscha/sscha.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1637 2024-05-04 07:42:36.000000 phono3py-3.0.3/phono3py/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 07:43:29.205348 phono3py-3.0.3/phono3py.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      451 2024-05-04 07:43:29.000000 phono3py-3.0.3/phono3py.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6429 2024-05-04 07:43:29.000000 phono3py-3.0.3/phono3py.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-04 07:43:29.000000 phono3py-3.0.3/phono3py.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       92 2024-05-04 07:43:29.000000 phono3py-3.0.3/phono3py.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-04 07:43:29.000000 phono3py-3.0.3/phono3py.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      298 2024-05-04 07:42:36.000000 phono3py-3.0.3/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 07:43:29.193348 phono3py-3.0.3/scripts/
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1831 2024-05-04 07:42:36.000000 phono3py-3.0.3/scripts/phono3py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3845 2024-05-04 07:42:36.000000 phono3py-3.0.3/scripts/phono3py-coleigplot
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1688 2024-05-04 07:42:36.000000 phono3py-3.0.3/scripts/phono3py-kaccum
+-rwxr-xr-x   0 runner    (1001) docker     (127)     9488 2024-05-04 07:42:36.000000 phono3py-3.0.3/scripts/phono3py-kdeplot
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1797 2024-05-04 07:42:36.000000 phono3py-3.0.3/scripts/phono3py-load
+-rw-r--r--   0 runner    (1001) docker     (127)      120 2024-05-04 07:43:29.209348 phono3py-3.0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)    10421 2024-05-04 07:42:36.000000 phono3py-3.0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 07:43:29.201348 phono3py-3.0.3/test/
+-rw-r--r--   0 runner    (1001) docker     (127)     1236 2024-05-04 07:42:36.000000 phono3py-3.0.3/test/AgNO2_cell.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      133 2024-05-04 07:42:36.000000 phono3py-3.0.3/test/BORN_NaCl
+-rw-r--r--   0 runner    (1001) docker     (127)   357907 2024-05-04 07:42:36.000000 phono3py-3.0.3/test/FORCES_FC3_si_pbesol
+-rw-r--r--   0 runner    (1001) docker     (127)     6282 2024-05-04 07:42:36.000000 phono3py-3.0.3/test/FORCE_SETS_NaCl
+-rw-r--r--   0 runner    (1001) docker     (127)   200548 2024-05-04 07:42:36.000000 phono3py-3.0.3/test/Si-111-222-fd.tar.xz
+-rw-r--r--   0 runner    (1001) docker     (127)   375392 2024-05-04 07:42:36.000000 phono3py-3.0.3/test/Si-111-222-rd.tar.xz
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 07:43:29.201348 phono3py-3.0.3/test/api/
+-rw-r--r--   0 runner    (1001) docker     (127)     5812 2024-05-04 07:42:36.000000 phono3py-3.0.3/test/api/test_api_phono3py.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 07:43:29.201348 phono3py-3.0.3/test/conductivity/
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-05-04 07:42:36.000000 phono3py-3.0.3/test/conductivity/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2696 2024-05-04 07:42:36.000000 phono3py-3.0.3/test/conductivity/test_kappa_LBTE.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1943 2024-05-04 07:42:36.000000 phono3py-3.0.3/test/conductivity/test_kappa_LBTE_Wigner.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12437 2024-05-04 07:42:36.000000 phono3py-3.0.3/test/conductivity/test_kappa_RTA.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12309 2024-05-04 07:42:36.000000 phono3py-3.0.3/test/conductivity/test_kappa_RTA_Wigner.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15956 2024-05-04 07:42:36.000000 phono3py-3.0.3/test/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 07:43:29.201348 phono3py-3.0.3/test/cui/
+-rw-r--r--   0 runner    (1001) docker     (127)    62552 2024-05-04 07:42:36.000000 phono3py-3.0.3/test/cui/phono3py_params-qe-Si222.yaml.xz
+-rw-r--r--   0 runner    (1001) docker     (127)     4847 2024-05-04 07:42:36.000000 phono3py-3.0.3/test/cui/test_phono3py_load_script.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 07:43:29.201348 phono3py-3.0.3/test/file_IO/
+-rw-r--r--   0 runner    (1001) docker     (127)     2310 2024-05-04 07:42:36.000000 phono3py-3.0.3/test/file_IO/test_file_IO.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 07:43:29.201348 phono3py-3.0.3/test/interface/
+-rw-r--r--   0 runner    (1001) docker     (127)     4558 2024-05-04 07:42:36.000000 phono3py-3.0.3/test/interface/test_phono3py_yaml.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 07:43:29.205348 phono3py-3.0.3/test/other/
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-05-04 07:42:36.000000 phono3py-3.0.3/test/other/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3871 2024-05-04 07:42:36.000000 phono3py-3.0.3/test/other/test_isotope.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14548 2024-05-04 07:42:36.000000 phono3py-3.0.3/test/other/test_kaccum.py
+-rw-r--r--   0 runner    (1001) docker     (127)   177468 2024-05-04 07:42:36.000000 phono3py-3.0.3/test/phono3py_params-Si111-rd.yaml.xz
+-rw-r--r--   0 runner    (1001) docker     (127)   943848 2024-05-04 07:42:36.000000 phono3py-3.0.3/test/phono3py_params_AlN332.yaml.xz
+-rw-r--r--   0 runner    (1001) docker     (127)    26352 2024-05-04 07:42:36.000000 phono3py-3.0.3/test/phono3py_params_NaCl111.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)    69120 2024-05-04 07:42:36.000000 phono3py-3.0.3/test/phono3py_params_NaCl222.yaml.xz
+-rw-r--r--   0 runner    (1001) docker     (127)     3176 2024-05-04 07:42:36.000000 phono3py-3.0.3/test/phono3py_params_Si-111-222-fd.yaml.xz
+-rw-r--r--   0 runner    (1001) docker     (127)    11664 2024-05-04 07:42:36.000000 phono3py-3.0.3/test/phono3py_params_Si-111-222-rd.yaml.xz
+-rw-r--r--   0 runner    (1001) docker     (127)    30693 2024-05-04 07:42:36.000000 phono3py-3.0.3/test/phono3py_params_Si-111-222.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)    18216 2024-05-04 07:42:36.000000 phono3py-3.0.3/test/phono3py_params_Si111.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)    32800 2024-05-04 07:42:36.000000 phono3py-3.0.3/test/phono3py_si_pbesol.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 07:43:29.205348 phono3py-3.0.3/test/phonon/
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-05-04 07:42:36.000000 phono3py-3.0.3/test/phonon/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    51828 2024-05-04 07:42:36.000000 phono3py-3.0.3/test/phonon/test_grid.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19747 2024-05-04 07:42:36.000000 phono3py-3.0.3/test/phonon/test_velocity_operator.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 07:43:29.205348 phono3py-3.0.3/test/phonon3/
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-05-04 07:42:36.000000 phono3py-3.0.3/test/phonon3/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4142 2024-05-04 07:42:36.000000 phono3py-3.0.3/test/phonon3/test_displacements.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11450 2024-05-04 07:42:36.000000 phono3py-3.0.3/test/phonon3/test_fc3.py
+-rw-r--r--   0 runner    (1001) docker     (127)    47987 2024-05-04 07:42:36.000000 phono3py-3.0.3/test/phonon3/test_imag_self_energy.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11113 2024-05-04 07:42:36.000000 phono3py-3.0.3/test/phonon3/test_interaction.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11546 2024-05-04 07:42:36.000000 phono3py-3.0.3/test/phonon3/test_joint_dos.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19498 2024-05-04 07:42:36.000000 phono3py-3.0.3/test/phonon3/test_real_self_energy.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19561 2024-05-04 07:42:36.000000 phono3py-3.0.3/test/phonon3/test_spectral_function.py
+-rw-r--r--   0 runner    (1001) docker     (127)    41126 2024-05-04 07:42:36.000000 phono3py-3.0.3/test/phonon3/test_triplets.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12203 2024-05-04 07:42:36.000000 phono3py-3.0.3/test/phonopy_disp_NaCl.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)   286407 2024-05-04 07:42:36.000000 phono3py-3.0.3/test/phonopy_params-Si111-iterha.yaml.gz
+-rw-r--r--   0 runner    (1001) docker     (127)     5587 2024-05-04 07:42:36.000000 phono3py-3.0.3/test/phonopy_params_Si.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 07:43:29.205348 phono3py-3.0.3/test/sscha/
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-04 07:42:36.000000 phono3py-3.0.3/test/sscha/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8801 2024-05-04 07:42:36.000000 phono3py-3.0.3/test/sscha/test_sscha.py
```

### Comparing `phono3py-3.0.2/LICENSE` & `phono3py-3.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `phono3py-3.0.2/README.md` & `phono3py-3.0.3/README.md`

 * *Files identical despite different names*

### Comparing `phono3py-3.0.2/c/_phono3py.c` & `phono3py-3.0.3/c/_phono3py.c`

 * *Files identical despite different names*

### Comparing `phono3py-3.0.2/c/_phononcalc.c` & `phono3py-3.0.3/c/_phononcalc.c`

 * *Files identical despite different names*

### Comparing `phono3py-3.0.2/c/bzgrid.c` & `phono3py-3.0.3/c/bzgrid.c`

 * *Files identical despite different names*

### Comparing `phono3py-3.0.2/c/bzgrid.h` & `phono3py-3.0.3/c/bzgrid.h`

 * *Files identical despite different names*

### Comparing `phono3py-3.0.2/c/collision_matrix.c` & `phono3py-3.0.3/c/collision_matrix.c`

 * *Files identical despite different names*

### Comparing `phono3py-3.0.2/c/collision_matrix.h` & `phono3py-3.0.3/c/collision_matrix.h`

 * *Files identical despite different names*

### Comparing `phono3py-3.0.2/c/dynmat.c` & `phono3py-3.0.3/c/dynmat.c`

 * *Files identical despite different names*

### Comparing `phono3py-3.0.2/c/dynmat.h` & `phono3py-3.0.3/c/dynmat.h`

 * *Files identical despite different names*

### Comparing `phono3py-3.0.2/c/fc3.c` & `phono3py-3.0.3/c/fc3.c`

 * *Files identical despite different names*

### Comparing `phono3py-3.0.2/c/fc3.h` & `phono3py-3.0.3/c/fc3.h`

 * *Files identical despite different names*

### Comparing `phono3py-3.0.2/c/grgrid.c` & `phono3py-3.0.3/c/grgrid.c`

 * *Files identical despite different names*

### Comparing `phono3py-3.0.2/c/grgrid.h` & `phono3py-3.0.3/c/grgrid.h`

 * *Files identical despite different names*

### Comparing `phono3py-3.0.2/c/gridsys.c` & `phono3py-3.0.3/c/gridsys.c`

 * *Files identical despite different names*

### Comparing `phono3py-3.0.2/c/gridsys.h` & `phono3py-3.0.3/c/gridsys.h`

 * *Files identical despite different names*

### Comparing `phono3py-3.0.2/c/imag_self_energy_with_g.c` & `phono3py-3.0.3/c/imag_self_energy_with_g.c`

 * *Files identical despite different names*

### Comparing `phono3py-3.0.2/c/imag_self_energy_with_g.h` & `phono3py-3.0.3/c/imag_self_energy_with_g.h`

 * *Files identical despite different names*

### Comparing `phono3py-3.0.2/c/interaction.c` & `phono3py-3.0.3/c/interaction.c`

 * *Files identical despite different names*

### Comparing `phono3py-3.0.2/c/interaction.h` & `phono3py-3.0.3/c/interaction.h`

 * *Files identical despite different names*

### Comparing `phono3py-3.0.2/c/isotope.c` & `phono3py-3.0.3/c/isotope.c`

 * *Files identical despite different names*

### Comparing `phono3py-3.0.2/c/isotope.h` & `phono3py-3.0.3/c/isotope.h`

 * *Files identical despite different names*

### Comparing `phono3py-3.0.2/c/lagrid.c` & `phono3py-3.0.3/c/lagrid.c`

 * *Files identical despite different names*

### Comparing `phono3py-3.0.2/c/lagrid.h` & `phono3py-3.0.3/c/lagrid.h`

 * *Files identical despite different names*

### Comparing `phono3py-3.0.2/c/lapack_wrapper.c` & `phono3py-3.0.3/c/lapack_wrapper.c`

 * *Files identical despite different names*

### Comparing `phono3py-3.0.2/c/lapack_wrapper.h` & `phono3py-3.0.3/c/lapack_wrapper.h`

 * *Files identical despite different names*

### Comparing `phono3py-3.0.2/c/niggli.c` & `phono3py-3.0.3/c/niggli.c`

 * *Files identical despite different names*

### Comparing `phono3py-3.0.2/c/niggli.h` & `phono3py-3.0.3/c/niggli.h`

 * *Files identical despite different names*

### Comparing `phono3py-3.0.2/c/phono3py.c` & `phono3py-3.0.3/c/phono3py.c`

 * *Files identical despite different names*

### Comparing `phono3py-3.0.2/c/phono3py.h` & `phono3py-3.0.3/c/phono3py.h`

 * *Files identical despite different names*

### Comparing `phono3py-3.0.2/c/phonoc_array.h` & `phono3py-3.0.3/c/phonoc_array.h`

 * *Files identical despite different names*

### Comparing `phono3py-3.0.2/c/phonoc_const.h` & `phono3py-3.0.3/c/phonoc_const.h`

 * *Files identical despite different names*

### Comparing `phono3py-3.0.2/c/phonoc_utils.c` & `phono3py-3.0.3/c/phonoc_utils.c`

 * *Files identical despite different names*

### Comparing `phono3py-3.0.2/c/phonoc_utils.h` & `phono3py-3.0.3/c/phonoc_utils.h`

 * *Files identical despite different names*

### Comparing `phono3py-3.0.2/c/phonon.c` & `phono3py-3.0.3/c/phonon.c`

 * *Files identical despite different names*

### Comparing `phono3py-3.0.2/c/phonon.h` & `phono3py-3.0.3/c/phonon.h`

 * *Files identical despite different names*

### Comparing `phono3py-3.0.2/c/phononcalc.c` & `phono3py-3.0.3/c/phononcalc.c`

 * *Files identical despite different names*

### Comparing `phono3py-3.0.2/c/phononcalc.h` & `phono3py-3.0.3/c/phononcalc.h`

 * *Files identical despite different names*

### Comparing `phono3py-3.0.2/c/pp_collision.c` & `phono3py-3.0.3/c/pp_collision.c`

 * *Files identical despite different names*

### Comparing `phono3py-3.0.2/c/pp_collision.h` & `phono3py-3.0.3/c/pp_collision.h`

 * *Files identical despite different names*

### Comparing `phono3py-3.0.2/c/real_self_energy.c` & `phono3py-3.0.3/c/real_self_energy.c`

 * *Files identical despite different names*

### Comparing `phono3py-3.0.2/c/real_self_energy.h` & `phono3py-3.0.3/c/real_self_energy.h`

 * *Files identical despite different names*

### Comparing `phono3py-3.0.2/c/real_to_reciprocal.c` & `phono3py-3.0.3/c/real_to_reciprocal.c`

 * *Files identical despite different names*

### Comparing `phono3py-3.0.2/c/real_to_reciprocal.h` & `phono3py-3.0.3/c/real_to_reciprocal.h`

 * *Files identical despite different names*

### Comparing `phono3py-3.0.2/c/reciprocal_to_normal.c` & `phono3py-3.0.3/c/reciprocal_to_normal.c`

 * *Files identical despite different names*

### Comparing `phono3py-3.0.2/c/reciprocal_to_normal.h` & `phono3py-3.0.3/c/reciprocal_to_normal.h`

 * *Files identical despite different names*

### Comparing `phono3py-3.0.2/c/snf3x3.c` & `phono3py-3.0.3/c/snf3x3.c`

 * *Files identical despite different names*

### Comparing `phono3py-3.0.2/c/tetrahedron_method.c` & `phono3py-3.0.3/c/tetrahedron_method.c`

 * *Files identical despite different names*

### Comparing `phono3py-3.0.2/c/tetrahedron_method.h` & `phono3py-3.0.3/c/tetrahedron_method.h`

 * *Files identical despite different names*

### Comparing `phono3py-3.0.2/c/triplet.c` & `phono3py-3.0.3/c/triplet.c`

 * *Files identical despite different names*

### Comparing `phono3py-3.0.2/c/triplet.h` & `phono3py-3.0.3/c/triplet.h`

 * *Files identical despite different names*

### Comparing `phono3py-3.0.2/c/triplet_grid.c` & `phono3py-3.0.3/c/triplet_grid.c`

 * *Files identical despite different names*

### Comparing `phono3py-3.0.2/c/triplet_grid.h` & `phono3py-3.0.3/c/triplet_grid.h`

 * *Files identical despite different names*

### Comparing `phono3py-3.0.2/c/triplet_iw.c` & `phono3py-3.0.3/c/triplet_iw.c`

 * *Files identical despite different names*

### Comparing `phono3py-3.0.2/c/triplet_iw.h` & `phono3py-3.0.3/c/triplet_iw.h`

 * *Files identical despite different names*

### Comparing `phono3py-3.0.2/example/AlN-LDA/FORCES_FC2` & `phono3py-3.0.3/example/AlN-LDA/FORCES_FC2`

 * *Files identical despite different names*

### Comparing `phono3py-3.0.2/example/AlN-LDA/FORCES_FC3.lzma` & `phono3py-3.0.3/example/AlN-LDA/FORCES_FC3.lzma`

 * *Files identical despite different names*

### Comparing `phono3py-3.0.2/example/AlN-LDA/README.md` & `phono3py-3.0.3/example/AlN-LDA/README.md`

 * *Files identical despite different names*

### Comparing `phono3py-3.0.2/example/AlN-LDA/phono3py_disp.yaml` & `phono3py-3.0.3/example/AlN-LDA/phono3py_disp.yaml`

 * *Files identical despite different names*

### Comparing `phono3py-3.0.2/example/AlN-LDA/phono3py_disp_dimfc2.yaml` & `phono3py-3.0.3/example/AlN-LDA/phono3py_disp_dimfc2.yaml`

 * *Files identical despite different names*

### Comparing `phono3py-3.0.2/example/NaCl-alm/README.md` & `phono3py-3.0.3/example/NaCl-alm/README.md`

 * *Files identical despite different names*

### Comparing `phono3py-3.0.2/example/NaCl-alm/phono3py_params_NaCl222.yaml.xz` & `phono3py-3.0.3/example/NaCl-alm/phono3py_params_NaCl222.yaml.xz`

 * *Files identical despite different names*

### Comparing `phono3py-3.0.2/example/Si-CRYSTAL/FORCES_FC2` & `phono3py-3.0.3/example/Si-CRYSTAL/FORCES_FC2`

 * *Files identical despite different names*

### Comparing `phono3py-3.0.2/example/Si-CRYSTAL/FORCES_FC3` & `phono3py-3.0.3/example/Si-CRYSTAL/FORCES_FC3`

 * *Files identical despite different names*

### Comparing `phono3py-3.0.2/example/Si-CRYSTAL/README` & `phono3py-3.0.3/example/Si-CRYSTAL/README`

 * *Files identical despite different names*

### Comparing `phono3py-3.0.2/example/Si-CRYSTAL/TEMPLATE` & `phono3py-3.0.3/example/Si-CRYSTAL/TEMPLATE`

 * *Files identical despite different names*

### Comparing `phono3py-3.0.2/example/Si-CRYSTAL/TEMPLATE3` & `phono3py-3.0.3/example/Si-CRYSTAL/TEMPLATE3`

 * *Files identical despite different names*

### Comparing `phono3py-3.0.2/example/Si-CRYSTAL/crystal.o` & `phono3py-3.0.3/example/Si-CRYSTAL/crystal.o`

 * *Files identical despite different names*

### Comparing `phono3py-3.0.2/example/Si-CRYSTAL/outputs.tar.gz` & `phono3py-3.0.3/example/Si-CRYSTAL/outputs.tar.gz`

 * *Files identical despite different names*

### Comparing `phono3py-3.0.2/example/Si-LDA/FORCES_FC3` & `phono3py-3.0.3/example/Si-LDA/FORCES_FC3`

 * *Files identical despite different names*

### Comparing `phono3py-3.0.2/example/Si-LDA/POSCAR-unitcell` & `phono3py-3.0.3/example/Si-LDA/POSCAR-unitcell`

 * *Files identical despite different names*

### Comparing `phono3py-3.0.2/example/Si-LDA/README.md` & `phono3py-3.0.3/example/Si-LDA/README.md`

 * *Files identical despite different names*

### Comparing `phono3py-3.0.2/example/Si-LDA/phono3py_disp.yaml` & `phono3py-3.0.3/example/Si-LDA/phono3py_disp.yaml`

 * *Files identical despite different names*

### Comparing `phono3py-3.0.2/example/Si-LDA/vasprun_xmls.tar.lzma` & `phono3py-3.0.3/example/Si-LDA/vasprun_xmls.tar.lzma`

 * *Files identical despite different names*

### Comparing `phono3py-3.0.2/example/Si-PBE/FORCES_FC3` & `phono3py-3.0.3/example/Si-PBE/FORCES_FC3`

 * *Files identical despite different names*

### Comparing `phono3py-3.0.2/example/Si-PBE/POSCAR-unitcell` & `phono3py-3.0.3/example/Si-PBE/POSCAR-unitcell`

 * *Files identical despite different names*

### Comparing `phono3py-3.0.2/example/Si-PBE/README.md` & `phono3py-3.0.3/example/Si-PBE/README.md`

 * *Files identical despite different names*

### Comparing `phono3py-3.0.2/example/Si-PBE/phono3py_disp.yaml` & `phono3py-3.0.3/example/Si-PBE/phono3py_disp.yaml`

 * *Files identical despite different names*

### Comparing `phono3py-3.0.2/example/Si-PBE/vasprun_xmls.tar.lzma` & `phono3py-3.0.3/example/Si-PBE/vasprun_xmls.tar.lzma`

 * *Files identical despite different names*

### Comparing `phono3py-3.0.2/example/Si-PBEsol/FORCES_FC3` & `phono3py-3.0.3/example/Si-PBEsol/FORCES_FC3`

 * *Files identical despite different names*

### Comparing `phono3py-3.0.2/example/Si-PBEsol/POSCAR-unitcell` & `phono3py-3.0.3/example/Si-PBEsol/POSCAR-unitcell`

 * *Files identical despite different names*

### Comparing `phono3py-3.0.2/example/Si-PBEsol/README.md` & `phono3py-3.0.3/example/Si-PBEsol/README.md`

 * *Files identical despite different names*

### Comparing `phono3py-3.0.2/example/Si-PBEsol/Si-band-DOS.png` & `phono3py-3.0.3/example/Si-PBEsol/Si-band-DOS.png`

 * *Files identical despite different names*

### Comparing `phono3py-3.0.2/example/Si-PBEsol/Si-kaccum.png` & `phono3py-3.0.3/example/Si-PBEsol/Si-kaccum.png`

 * *Files identical despite different names*

### Comparing `phono3py-3.0.2/example/Si-PBEsol/Si.py` & `phono3py-3.0.3/example/Si-PBEsol/Si.py`

 * *Files identical despite different names*

### Comparing `phono3py-3.0.2/example/Si-PBEsol/phono3py_disp.yaml` & `phono3py-3.0.3/example/Si-PBEsol/phono3py_disp.yaml`

 * *Files identical despite different names*

### Comparing `phono3py-3.0.2/example/Si-PBEsol/phono3py_disp_dimfc2.yaml` & `phono3py-3.0.3/example/Si-PBEsol/phono3py_disp_dimfc2.yaml`

 * *Files identical despite different names*

### Comparing `phono3py-3.0.2/example/Si-PBEsol/vasprun_xml_fc2/disp-fc2-00001/POSCAR` & `phono3py-3.0.3/example/Si-PBEsol/vasprun_xml_fc2/disp-fc2-00001/POSCAR`

 * *Files identical despite different names*

### Comparing `phono3py-3.0.2/example/Si-PBEsol/vasprun_xml_fc2/disp-fc2-00001/vasprun.xml` & `phono3py-3.0.3/example/Si-PBEsol/vasprun_xml_fc2/disp-fc2-00001/vasprun.xml`

 * *Files identical despite different names*

### Comparing `phono3py-3.0.2/example/Si-PBEsol/vasprun_xmls.tar.lzma` & `phono3py-3.0.3/example/Si-PBEsol/vasprun_xmls.tar.lzma`

 * *Files identical despite different names*

### Comparing `phono3py-3.0.2/example/Si-QE/FORCES_FC3` & `phono3py-3.0.3/example/Si-QE/FORCES_FC3`

 * *Files identical despite different names*

### Comparing `phono3py-3.0.2/example/Si-QE/README.md` & `phono3py-3.0.3/example/Si-QE/README.md`

 * *Files identical despite different names*

### Comparing `phono3py-3.0.2/example/Si-QE/Si.in` & `phono3py-3.0.3/example/Si-QE/Si.in`

 * *Files identical despite different names*

### Comparing `phono3py-3.0.2/example/Si-QE/phono3py_disp.yaml` & `phono3py-3.0.3/example/Si-QE/phono3py_disp.yaml`

 * *Files identical despite different names*

### Comparing `phono3py-3.0.2/example/Si-QE/supercell_out.tar.lzma` & `phono3py-3.0.3/example/Si-QE/supercell_out.tar.lzma`

 * *Files identical despite different names*

### Comparing `phono3py-3.0.2/example/Si-TURBOMOLE/FORCES_FC2` & `phono3py-3.0.3/example/Si-TURBOMOLE/FORCES_FC2`

 * *Files identical despite different names*

### Comparing `phono3py-3.0.2/example/Si-TURBOMOLE/FORCES_FC3` & `phono3py-3.0.3/example/Si-TURBOMOLE/FORCES_FC3`

 * *Files identical despite different names*

### Comparing `phono3py-3.0.2/example/Si-TURBOMOLE/README` & `phono3py-3.0.3/example/Si-TURBOMOLE/README`

 * *Files identical despite different names*

### Comparing `phono3py-3.0.2/example/Si-TURBOMOLE/outputs.tar.gz` & `phono3py-3.0.3/example/Si-TURBOMOLE/outputs.tar.gz`

 * *Files identical despite different names*

### Comparing `phono3py-3.0.2/example/Wigner_La2Zr2O7/BORN` & `phono3py-3.0.3/example/Wigner_La2Zr2O7/BORN`

 * *Files identical despite different names*

### Comparing `phono3py-3.0.2/example/Wigner_La2Zr2O7/POSCAR` & `phono3py-3.0.3/example/Wigner_La2Zr2O7/POSCAR`

 * *Files identical despite different names*

### Comparing `phono3py-3.0.2/example/Wigner_La2Zr2O7/fc2.hdf5` & `phono3py-3.0.3/example/Wigner_La2Zr2O7/fc2.hdf5`

 * *Files identical despite different names*

### Comparing `phono3py-3.0.2/example/Wigner_La2Zr2O7/kappa-m191919.hdf5` & `phono3py-3.0.3/example/Wigner_La2Zr2O7/kappa-m191919.hdf5`

 * *Files identical despite different names*

### Comparing `phono3py-3.0.2/example/Wigner_La2Zr2O7/tc_La2Zr2O7.out.xz` & `phono3py-3.0.3/example/Wigner_La2Zr2O7/tc_La2Zr2O7.out.xz`

 * *Files identical despite different names*

### Comparing `phono3py-3.0.2/example/zb-ZnTe-PBEsol/README.md` & `phono3py-3.0.3/example/zb-ZnTe-PBEsol/README.md`

 * *Files identical despite different names*

### Comparing `phono3py-3.0.2/example/zb-ZnTe-PBEsol/launch_phono3py_ZnTe_PBEsol_222.py` & `phono3py-3.0.3/example/zb-ZnTe-PBEsol/launch_phono3py_ZnTe_PBEsol_222.py`

 * *Files identical despite different names*

### Comparing `phono3py-3.0.2/example/zb-ZnTe-PBEsol/phono3py_params_ZnTe.yaml.xz` & `phono3py-3.0.3/example/zb-ZnTe-PBEsol/phono3py_params_ZnTe.yaml.xz`

 * *Files identical despite different names*

### Comparing `phono3py-3.0.2/phono3py/__init__.py` & `phono3py-3.0.3/phono3py/__init__.py`

 * *Files identical despite different names*

### Comparing `phono3py-3.0.2/phono3py/api_isotope.py` & `phono3py-3.0.3/phono3py/api_isotope.py`

 * *Files identical despite different names*

### Comparing `phono3py-3.0.2/phono3py/api_jointdos.py` & `phono3py-3.0.3/phono3py/api_jointdos.py`

 * *Files identical despite different names*

### Comparing `phono3py-3.0.2/phono3py/api_phono3py.py` & `phono3py-3.0.3/phono3py/api_phono3py.py`

 * *Files 6% similar despite different names*

```diff
@@ -94,5394 +94,5738 @@
 000005d0: 204f 5220 4f54 4845 5257 4953 4529 2041   OR OTHERWISE) A
 000005e0: 5249 5349 4e47 2049 4e0a 2320 414e 5920  RISING IN.# ANY 
 000005f0: 5741 5920 4f55 5420 4f46 2054 4845 2055  WAY OUT OF THE U
 00000600: 5345 204f 4620 5448 4953 2053 4f46 5457  SE OF THIS SOFTW
 00000610: 4152 452c 2045 5645 4e20 4946 2041 4456  ARE, EVEN IF ADV
 00000620: 4953 4544 204f 4620 5448 450a 2320 504f  ISED OF THE.# PO
 00000630: 5353 4942 494c 4954 5920 4f46 2053 5543  SSIBILITY OF SUC
-00000640: 4820 4441 4d41 4745 2e0a 0a66 726f 6d20  H DAMAGE...from 
-00000650: 636f 6c6c 6563 7469 6f6e 732e 6162 6320  collections.abc 
-00000660: 696d 706f 7274 2053 6571 7565 6e63 650a  import Sequence.
-00000670: 6672 6f6d 2074 7970 696e 6720 696d 706f  from typing impo
-00000680: 7274 204f 7074 696f 6e61 6c2c 2055 6e69  rt Optional, Uni
-00000690: 6f6e 0a0a 696d 706f 7274 206e 756d 7079  on..import numpy
-000006a0: 2061 7320 6e70 0a66 726f 6d20 7068 6f6e   as np.from phon
-000006b0: 6f70 792e 6578 6365 7074 696f 6e20 696d  opy.exception im
-000006c0: 706f 7274 2046 6f72 6365 4361 6c63 756c  port ForceCalcul
-000006d0: 6174 6f72 5265 7175 6972 6564 4572 726f  atorRequiredErro
-000006e0: 720a 6672 6f6d 2070 686f 6e6f 7079 2e68  r.from phonopy.h
-000006f0: 6172 6d6f 6e69 632e 6469 7370 6c61 6365  armonic.displace
-00000700: 6d65 6e74 2069 6d70 6f72 7420 280a 2020  ment import (.  
-00000710: 2020 6469 7265 6374 696f 6e73 5f74 6f5f    directions_to_
-00000720: 6469 7370 6c61 6365 6d65 6e74 5f64 6174  displacement_dat
-00000730: 6173 6574 2c0a 2020 2020 6765 745f 6c65  aset,.    get_le
-00000740: 6173 745f 6469 7370 6c61 6365 6d65 6e74  ast_displacement
-00000750: 732c 0a29 0a66 726f 6d20 7068 6f6e 6f70  s,.).from phonop
-00000760: 792e 6861 726d 6f6e 6963 2e66 6f72 6365  y.harmonic.force
-00000770: 5f63 6f6e 7374 616e 7473 2069 6d70 6f72  _constants impor
-00000780: 7420 6765 745f 6663 3220 6173 2067 6574  t get_fc2 as get
-00000790: 5f70 686f 6e6f 7079 5f66 6332 0a66 726f  _phonopy_fc2.fro
-000007a0: 6d20 7068 6f6e 6f70 792e 6861 726d 6f6e  m phonopy.harmon
-000007b0: 6963 2e66 6f72 6365 5f63 6f6e 7374 616e  ic.force_constan
-000007c0: 7473 2069 6d70 6f72 7420 280a 2020 2020  ts import (.    
-000007d0: 7365 745f 7065 726d 7574 6174 696f 6e5f  set_permutation_
-000007e0: 7379 6d6d 6574 7279 2c0a 2020 2020 7365  symmetry,.    se
-000007f0: 745f 7472 616e 736c 6174 696f 6e61 6c5f  t_translational_
-00000800: 696e 7661 7269 616e 6365 2c0a 2020 2020  invariance,.    
-00000810: 7379 6d6d 6574 7269 7a65 5f63 6f6d 7061  symmetrize_compa
-00000820: 6374 5f66 6f72 6365 5f63 6f6e 7374 616e  ct_force_constan
-00000830: 7473 2c0a 2020 2020 7379 6d6d 6574 7269  ts,.    symmetri
-00000840: 7a65 5f66 6f72 6365 5f63 6f6e 7374 616e  ze_force_constan
-00000850: 7473 2c0a 290a 6672 6f6d 2070 686f 6e6f  ts,.).from phono
-00000860: 7079 2e69 6e74 6572 6661 6365 2e66 635f  py.interface.fc_
-00000870: 6361 6c63 756c 6174 6f72 2069 6d70 6f72  calculator impor
-00000880: 7420 6765 745f 6663 320a 6672 6f6d 2070  t get_fc2.from p
-00000890: 686f 6e6f 7079 2e73 7472 7563 7475 7265  honopy.structure
-000008a0: 2e61 746f 6d73 2069 6d70 6f72 7420 5068  .atoms import Ph
-000008b0: 6f6e 6f70 7941 746f 6d73 0a66 726f 6d20  onopyAtoms.from 
-000008c0: 7068 6f6e 6f70 792e 7374 7275 6374 7572  phonopy.structur
-000008d0: 652e 6365 6c6c 7320 696d 706f 7274 2028  e.cells import (
-000008e0: 0a20 2020 2050 7269 6d69 7469 7665 2c0a  .    Primitive,.
-000008f0: 2020 2020 5375 7065 7263 656c 6c2c 0a20      Supercell,. 
-00000900: 2020 2067 6574 5f70 7269 6d69 7469 7665     get_primitive
-00000910: 2c0a 2020 2020 6765 745f 7072 696d 6974  ,.    get_primit
-00000920: 6976 655f 6d61 7472 6978 2c0a 2020 2020  ive_matrix,.    
-00000930: 6765 745f 7375 7065 7263 656c 6c2c 0a20  get_supercell,. 
-00000940: 2020 2067 7565 7373 5f70 7269 6d69 7469     guess_primiti
-00000950: 7665 5f6d 6174 7269 782c 0a20 2020 2073  ve_matrix,.    s
-00000960: 6861 7065 5f73 7570 6572 6365 6c6c 5f6d  hape_supercell_m
-00000970: 6174 7269 782c 0a29 0a66 726f 6d20 7068  atrix,.).from ph
-00000980: 6f6e 6f70 792e 7374 7275 6374 7572 652e  onopy.structure.
-00000990: 6461 7461 7365 7420 696d 706f 7274 2067  dataset import g
-000009a0: 6574 5f64 6973 706c 6163 656d 656e 7473  et_displacements
-000009b0: 5f61 6e64 5f66 6f72 6365 730a 6672 6f6d  _and_forces.from
-000009c0: 2070 686f 6e6f 7079 2e73 7472 7563 7475   phonopy.structu
-000009d0: 7265 2e73 796d 6d65 7472 7920 696d 706f  re.symmetry impo
-000009e0: 7274 2053 796d 6d65 7472 790a 6672 6f6d  rt Symmetry.from
-000009f0: 2070 686f 6e6f 7079 2e75 6e69 7473 2069   phonopy.units i
-00000a00: 6d70 6f72 7420 5661 7370 546f 5448 7a0a  mport VaspToTHz.
-00000a10: 0a66 726f 6d20 7068 6f6e 6f33 7079 2e63  .from phono3py.c
-00000a20: 6f6e 6475 6374 6976 6974 792e 6469 7265  onductivity.dire
-00000a30: 6374 5f73 6f6c 7574 696f 6e20 696d 706f  ct_solution impo
-00000a40: 7274 2067 6574 5f74 6865 726d 616c 5f63  rt get_thermal_c
-00000a50: 6f6e 6475 6374 6976 6974 795f 4c42 5445  onductivity_LBTE
-00000a60: 0a66 726f 6d20 7068 6f6e 6f33 7079 2e63  .from phono3py.c
-00000a70: 6f6e 6475 6374 6976 6974 792e 7274 6120  onductivity.rta 
-00000a80: 696d 706f 7274 2067 6574 5f74 6865 726d  import get_therm
-00000a90: 616c 5f63 6f6e 6475 6374 6976 6974 795f  al_conductivity_
-00000aa0: 5254 410a 6672 6f6d 2070 686f 6e6f 3370  RTA.from phono3p
-00000ab0: 792e 696e 7465 7266 6163 652e 6663 5f63  y.interface.fc_c
-00000ac0: 616c 6375 6c61 746f 7220 696d 706f 7274  alculator import
-00000ad0: 2067 6574 5f66 6333 0a66 726f 6d20 7068   get_fc3.from ph
-00000ae0: 6f6e 6f33 7079 2e69 6e74 6572 6661 6365  ono3py.interface
-00000af0: 2e70 686f 6e6f 3370 795f 7961 6d6c 2069  .phono3py_yaml i
-00000b00: 6d70 6f72 7420 5068 6f6e 6f33 7079 5961  mport Phono3pyYa
-00000b10: 6d6c 0a66 726f 6d20 7068 6f6e 6f33 7079  ml.from phono3py
-00000b20: 2e70 686f 6e6f 6e33 2e64 6174 6173 6574  .phonon3.dataset
-00000b30: 2069 6d70 6f72 7420 6765 745f 6469 7370   import get_disp
-00000b40: 6c61 6365 6d65 6e74 735f 616e 645f 666f  lacements_and_fo
-00000b50: 7263 6573 5f66 6333 0a66 726f 6d20 7068  rces_fc3.from ph
-00000b60: 6f6e 6f33 7079 2e70 686f 6e6f 6e33 2e64  ono3py.phonon3.d
-00000b70: 6973 706c 6163 656d 656e 745f 6663 3320  isplacement_fc3 
-00000b80: 696d 706f 7274 2028 0a20 2020 2064 6972  import (.    dir
-00000b90: 6563 7469 6f6e 5f74 6f5f 6469 7370 6c61  ection_to_displa
-00000ba0: 6365 6d65 6e74 2c0a 2020 2020 6765 745f  cement,.    get_
-00000bb0: 7468 6972 645f 6f72 6465 725f 6469 7370  third_order_disp
-00000bc0: 6c61 6365 6d65 6e74 732c 0a29 0a66 726f  lacements,.).fro
-00000bd0: 6d20 7068 6f6e 6f33 7079 2e70 686f 6e6f  m phono3py.phono
-00000be0: 6e33 2e66 6333 2069 6d70 6f72 7420 6375  n3.fc3 import cu
-00000bf0: 746f 6666 5f66 6333 5f62 795f 7a65 726f  toff_fc3_by_zero
-00000c00: 0a66 726f 6d20 7068 6f6e 6f33 7079 2e70  .from phono3py.p
-00000c10: 686f 6e6f 6e33 2e66 6333 2069 6d70 6f72  honon3.fc3 impor
-00000c20: 7420 6765 745f 6663 3320 6173 2067 6574  t get_fc3 as get
-00000c30: 5f70 686f 6e6f 3370 795f 6663 330a 6672  _phono3py_fc3.fr
-00000c40: 6f6d 2070 686f 6e6f 3370 792e 7068 6f6e  om phono3py.phon
-00000c50: 6f6e 332e 6663 3320 696d 706f 7274 2028  on3.fc3 import (
-00000c60: 0a20 2020 2073 6574 5f70 6572 6d75 7461  .    set_permuta
-00000c70: 7469 6f6e 5f73 796d 6d65 7472 795f 636f  tion_symmetry_co
-00000c80: 6d70 6163 745f 6663 332c 0a20 2020 2073  mpact_fc3,.    s
-00000c90: 6574 5f70 6572 6d75 7461 7469 6f6e 5f73  et_permutation_s
-00000ca0: 796d 6d65 7472 795f 6663 332c 0a20 2020  ymmetry_fc3,.   
-00000cb0: 2073 6574 5f74 7261 6e73 6c61 7469 6f6e   set_translation
-00000cc0: 616c 5f69 6e76 6172 6961 6e63 655f 636f  al_invariance_co
-00000cd0: 6d70 6163 745f 6663 332c 0a20 2020 2073  mpact_fc3,.    s
-00000ce0: 6574 5f74 7261 6e73 6c61 7469 6f6e 616c  et_translational
-00000cf0: 5f69 6e76 6172 6961 6e63 655f 6663 332c  _invariance_fc3,
-00000d00: 0a29 0a66 726f 6d20 7068 6f6e 6f33 7079  .).from phono3py
-00000d10: 2e70 686f 6e6f 6e33 2e69 6d61 675f 7365  .phonon3.imag_se
-00000d20: 6c66 5f65 6e65 7267 7920 696d 706f 7274  lf_energy import
-00000d30: 2028 0a20 2020 2067 6574 5f69 6d61 675f   (.    get_imag_
-00000d40: 7365 6c66 5f65 6e65 7267 792c 0a20 2020  self_energy,.   
-00000d50: 2077 7269 7465 5f69 6d61 675f 7365 6c66   write_imag_self
-00000d60: 5f65 6e65 7267 792c 0a29 0a66 726f 6d20  _energy,.).from 
-00000d70: 7068 6f6e 6f33 7079 2e70 686f 6e6f 6e33  phono3py.phonon3
-00000d80: 2e69 6e74 6572 6163 7469 6f6e 2069 6d70  .interaction imp
-00000d90: 6f72 7420 496e 7465 7261 6374 696f 6e0a  ort Interaction.
-00000da0: 6672 6f6d 2070 686f 6e6f 3370 792e 7068  from phono3py.ph
-00000db0: 6f6e 6f6e 332e 7265 616c 5f73 656c 665f  onon3.real_self_
-00000dc0: 656e 6572 6779 2069 6d70 6f72 7420 280a  energy import (.
-00000dd0: 2020 2020 6765 745f 7265 616c 5f73 656c      get_real_sel
-00000de0: 665f 656e 6572 6779 2c0a 2020 2020 7772  f_energy,.    wr
-00000df0: 6974 655f 7265 616c 5f73 656c 665f 656e  ite_real_self_en
-00000e00: 6572 6779 2c0a 290a 6672 6f6d 2070 686f  ergy,.).from pho
-00000e10: 6e6f 3370 792e 7068 6f6e 6f6e 332e 7370  no3py.phonon3.sp
-00000e20: 6563 7472 616c 5f66 756e 6374 696f 6e20  ectral_function 
-00000e30: 696d 706f 7274 2072 756e 5f73 7065 6374  import run_spect
-00000e40: 7261 6c5f 6675 6e63 7469 6f6e 0a66 726f  ral_function.fro
-00000e50: 6d20 7068 6f6e 6f33 7079 2e70 686f 6e6f  m phono3py.phono
-00000e60: 6e2e 6772 6964 2069 6d70 6f72 7420 425a  n.grid import BZ
-00000e70: 4772 6964 0a66 726f 6d20 7068 6f6e 6f33  Grid.from phono3
-00000e80: 7079 2e76 6572 7369 6f6e 2069 6d70 6f72  py.version impor
-00000e90: 7420 5f5f 7665 7273 696f 6e5f 5f0a 0a0a  t __version__...
-00000ea0: 636c 6173 7320 5068 6f6e 6f33 7079 3a0a  class Phono3py:.
-00000eb0: 2020 2020 2222 2250 686f 6e6f 3370 7920      """Phono3py 
-00000ec0: 6d61 696e 2063 6c61 7373 2e0a 0a20 2020  main class...   
-00000ed0: 2041 7474 7269 6275 7465 730a 2020 2020   Attributes.    
-00000ee0: 2d2d 2d2d 2d2d 2d2d 2d2d 0a20 2020 2076  ----------.    v
-00000ef0: 6572 7369 6f6e 0a20 2020 2063 616c 6375  ersion.    calcu
-00000f00: 6c61 746f 720a 2020 2020 6663 3320 3a20  lator.    fc3 : 
-00000f10: 6765 7474 6572 2061 6e64 2073 6574 7465  getter and sette
-00000f20: 720a 2020 2020 6663 3220 3a20 6765 7474  r.    fc2 : gett
-00000f30: 6572 2061 6e64 2073 6574 7465 720a 2020  er and setter.  
-00000f40: 2020 666f 7263 655f 636f 6e73 7461 6e74    force_constant
-00000f50: 730a 2020 2020 7369 676d 6120 3a20 6765  s.    sigma : ge
-00000f60: 7474 6572 2061 6e64 2073 6574 7465 720a  tter and setter.
-00000f70: 2020 2020 7369 676d 615f 6375 746f 6666      sigma_cutoff
-00000f80: 203a 2067 6574 7465 7220 616e 6420 7365   : getter and se
-00000f90: 7474 6572 0a20 2020 206e 6163 5f70 6172  tter.    nac_par
-00000fa0: 616d 7320 3a20 6765 7474 6572 2061 6e64  ams : getter and
-00000fb0: 2073 6574 7465 720a 2020 2020 6479 6e61   setter.    dyna
-00000fc0: 6d69 6361 6c5f 6d61 7472 6978 0a20 2020  mical_matrix.   
-00000fd0: 2070 7269 6d69 7469 7665 0a20 2020 2075   primitive.    u
-00000fe0: 6e69 7463 656c 6c0a 2020 2020 7375 7065  nitcell.    supe
-00000ff0: 7263 656c 6c0a 2020 2020 7068 6f6e 6f6e  rcell.    phonon
-00001000: 5f73 7570 6572 6365 6c6c 0a20 2020 2070  _supercell.    p
-00001010: 686f 6e6f 6e5f 7072 696d 6974 6976 650a  honon_primitive.
-00001020: 2020 2020 7379 6d6d 6574 7279 0a20 2020      symmetry.   
-00001030: 2070 7269 6d69 7469 7665 5f73 796d 6d65   primitive_symme
-00001040: 7472 790a 2020 2020 7068 6f6e 6f6e 5f73  try.    phonon_s
-00001050: 7570 6572 6365 6c6c 5f73 796d 6d65 7472  upercell_symmetr
-00001060: 790a 2020 2020 7375 7065 7263 656c 6c5f  y.    supercell_
-00001070: 6d61 7472 6978 0a20 2020 2070 686f 6e6f  matrix.    phono
-00001080: 6e5f 7375 7065 7263 656c 6c5f 6d61 7472  n_supercell_matr
-00001090: 6978 0a20 2020 2070 7269 6d69 7469 7665  ix.    primitive
-000010a0: 5f6d 6174 7269 780a 2020 2020 756e 6974  _matrix.    unit
-000010b0: 5f63 6f6e 7665 7273 696f 6e5f 6661 6374  _conversion_fact
-000010c0: 6f72 0a20 2020 2064 6174 6173 6574 203a  or.    dataset :
-000010d0: 2067 6574 7465 7220 616e 6420 7365 7474   getter and sett
-000010e0: 6572 0a20 2020 2070 686f 6e6f 6e5f 6461  er.    phonon_da
-000010f0: 7461 7365 7420 3a20 6765 7474 6572 2061  taset : getter a
-00001100: 6e64 2073 6574 7465 720a 2020 2020 6261  nd setter.    ba
-00001110: 6e64 5f69 6e64 6963 6573 203a 2067 6574  nd_indices : get
-00001120: 7465 7220 616e 6420 7365 7474 6572 0a20  ter and setter. 
-00001130: 2020 2070 686f 6e6f 6e5f 7375 7065 7263     phonon_superc
-00001140: 656c 6c73 5f77 6974 685f 6469 7370 6c61  ells_with_displa
-00001150: 6365 6d65 6e74 730a 2020 2020 7375 7065  cements.    supe
-00001160: 7263 656c 6c73 5f77 6974 685f 6469 7370  rcells_with_disp
-00001170: 6c61 6365 6d65 6e74 730a 2020 2020 6d65  lacements.    me
-00001180: 7368 5f6e 756d 6265 7273 203a 2067 6574  sh_numbers : get
-00001190: 7465 7220 616e 6420 7365 7474 6572 0a20  ter and setter. 
-000011a0: 2020 2074 6865 726d 616c 5f63 6f6e 6475     thermal_condu
-000011b0: 6374 6976 6974 790a 2020 2020 6469 7370  ctivity.    disp
-000011c0: 6c61 6365 6d65 6e74 7320 3a20 6765 7474  lacements : gett
-000011d0: 6572 2061 6e64 2073 6574 7465 720a 2020  er and setter.  
-000011e0: 2020 666f 7263 6573 203a 2067 6574 7465    forces : gette
-000011f0: 7220 616e 6420 7365 7474 6572 0a20 2020  r and setter.   
-00001200: 2070 686f 6e6f 6e5f 6469 7370 6c61 6365   phonon_displace
-00001210: 6d65 6e74 7320 3a20 6765 7474 6572 2061  ments : getter a
-00001220: 6e64 2073 6574 7465 720a 2020 2020 7068  nd setter.    ph
-00001230: 6f6e 6f6e 5f66 6f72 6365 7320 3a20 6765  onon_forces : ge
-00001240: 7474 6572 2061 6e64 2073 6574 7465 720a  tter and setter.
-00001250: 2020 2020 7068 7068 5f69 6e74 6572 6163      phph_interac
-00001260: 7469 6f6e 0a0a 2020 2020 2222 220a 0a20  tion..    """.. 
-00001270: 2020 2064 6566 205f 5f69 6e69 745f 5f28     def __init__(
-00001280: 0a20 2020 2020 2020 2073 656c 662c 0a20  .        self,. 
-00001290: 2020 2020 2020 2075 6e69 7463 656c 6c3a         unitcell:
-000012a0: 2050 686f 6e6f 7079 4174 6f6d 732c 0a20   PhonopyAtoms,. 
-000012b0: 2020 2020 2020 2073 7570 6572 6365 6c6c         supercell
-000012c0: 5f6d 6174 7269 783d 4e6f 6e65 2c0a 2020  _matrix=None,.  
-000012d0: 2020 2020 2020 7072 696d 6974 6976 655f        primitive_
-000012e0: 6d61 7472 6978 3d4e 6f6e 652c 0a20 2020  matrix=None,.   
-000012f0: 2020 2020 2070 686f 6e6f 6e5f 7375 7065       phonon_supe
-00001300: 7263 656c 6c5f 6d61 7472 6978 3d4e 6f6e  rcell_matrix=Non
-00001310: 652c 0a20 2020 2020 2020 2063 7574 6f66  e,.        cutof
-00001320: 665f 6672 6571 7565 6e63 793d 3165 2d34  f_frequency=1e-4
-00001330: 2c0a 2020 2020 2020 2020 6672 6571 7565  ,.        freque
-00001340: 6e63 795f 6661 6374 6f72 5f74 6f5f 5448  ncy_factor_to_TH
-00001350: 7a3d 5661 7370 546f 5448 7a2c 0a20 2020  z=VaspToTHz,.   
-00001360: 2020 2020 2069 735f 7379 6d6d 6574 7279       is_symmetry
-00001370: 3d54 7275 652c 0a20 2020 2020 2020 2069  =True,.        i
-00001380: 735f 6d65 7368 5f73 796d 6d65 7472 793d  s_mesh_symmetry=
-00001390: 5472 7565 2c0a 2020 2020 2020 2020 7573  True,.        us
-000013a0: 655f 6772 673d 4661 6c73 652c 0a20 2020  e_grg=False,.   
-000013b0: 2020 2020 2053 4e46 5f63 6f6f 7264 696e       SNF_coordin
-000013c0: 6174 6573 3d22 7265 6369 7072 6f63 616c  ates="reciprocal
-000013d0: 222c 0a20 2020 2020 2020 206d 616b 655f  ",.        make_
-000013e0: 7230 5f61 7665 7261 6765 3a20 626f 6f6c  r0_average: bool
-000013f0: 203d 2054 7275 652c 0a20 2020 2020 2020   = True,.       
-00001400: 2073 796d 7072 6563 3d31 652d 352c 0a20   symprec=1e-5,. 
-00001410: 2020 2020 2020 2063 616c 6375 6c61 746f         calculato
-00001420: 723a 204f 7074 696f 6e61 6c5b 7374 725d  r: Optional[str]
-00001430: 203d 204e 6f6e 652c 0a20 2020 2020 2020   = None,.       
-00001440: 206c 6f67 5f6c 6576 656c 3d30 2c0a 2020   log_level=0,.  
-00001450: 2020 293a 0a20 2020 2020 2020 2022 2222    ):.        """
-00001460: 496e 6974 206d 6574 686f 642e 0a0a 2020  Init method...  
-00001470: 2020 2020 2020 5061 7261 6d65 7465 7273        Parameters
-00001480: 0a20 2020 2020 2020 202d 2d2d 2d2d 2d2d  .        -------
-00001490: 2d2d 2d0a 2020 2020 2020 2020 756e 6974  ---.        unit
-000014a0: 6365 6c6c 203a 2050 686f 6e6f 7079 4174  cell : PhonopyAt
-000014b0: 6f6d 732c 206f 7074 696f 6e61 6c0a 2020  oms, optional.  
-000014c0: 2020 2020 2020 2020 2020 496e 7075 7420            Input 
-000014d0: 756e 6974 2063 656c 6c2e 0a20 2020 2020  unit cell..     
-000014e0: 2020 2073 7570 6572 6365 6c6c 5f6d 6174     supercell_mat
-000014f0: 7269 7820 3a20 6172 7261 795f 6c69 6b65  rix : array_like
-00001500: 2c20 6f70 7469 6f6e 616c 0a20 2020 2020  , optional.     
-00001510: 2020 2020 2020 2053 7570 6572 6365 6c6c         Supercell
-00001520: 206d 6174 7269 7820 6d75 6c74 6970 6c69   matrix multipli
-00001530: 6564 2074 6f20 696e 7075 7420 6365 6c6c  ed to input cell
-00001540: 2062 6173 6973 2076 6563 746f 7273 2e20   basis vectors. 
-00001550: 7368 6170 653d 2833 2c20 290a 2020 2020  shape=(3, ).    
-00001560: 2020 2020 2020 2020 6f72 2028 332c 2033          or (3, 3
-00001570: 292c 2077 6865 7265 2074 6865 2066 6f72  ), where the for
-00001580: 6d65 7220 6973 2063 6f6e 7369 6465 7265  mer is considere
-00001590: 6420 6120 6469 6167 6f6e 616c 206d 6174  d a diagonal mat
-000015a0: 7269 782e 2054 6865 0a20 2020 2020 2020  rix. The.       
-000015b0: 2020 2020 2065 6c65 6d65 6e74 7320 6861       elements ha
-000015c0: 7665 2074 6f20 6265 2067 6976 656e 2062  ve to be given b
-000015d0: 7920 696e 7465 6765 7273 2e20 416c 7468  y integers. Alth
-000015e0: 6f75 6768 2074 6865 2064 6566 6175 6c74  ough the default
-000015f0: 2069 7320 4e6f 6e65 2c0a 2020 2020 2020   is None,.      
-00001600: 2020 2020 2020 7768 6963 6820 7265 7375        which resu
-00001610: 6c74 7320 696e 2069 6465 6e74 6974 7920  lts in identity 
-00001620: 6d61 7472 6978 2c20 6974 2069 7320 7265  matrix, it is re
-00001630: 636f 6d6d 656e 6465 6420 746f 2067 6976  commended to giv
-00001640: 650a 2020 2020 2020 2020 2020 2020 6073  e.            `s
-00001650: 7570 6572 6365 6c6c 5f6d 6174 7269 7860  upercell_matrix`
-00001660: 2065 7870 6c69 6369 746c 792e 0a20 2020   explicitly..   
-00001670: 2020 2020 2070 7269 6d69 7469 7665 5f6d       primitive_m
-00001680: 6174 7269 7820 3a20 6172 7261 795f 6c69  atrix : array_li
-00001690: 6b65 206f 7220 7374 722c 206f 7074 696f  ke or str, optio
-000016a0: 6e61 6c0a 2020 2020 2020 2020 2020 2020  nal.            
-000016b0: 5072 696d 6974 6976 6520 6d61 7472 6978  Primitive matrix
-000016c0: 206d 756c 7469 706c 6965 6420 746f 2069   multiplied to i
-000016d0: 6e70 7574 2063 656c 6c20 6261 7369 7320  nput cell basis 
-000016e0: 7665 6374 6f72 732e 2044 6566 6175 6c74  vectors. Default
-000016f0: 2069 730a 2020 2020 2020 2020 2020 2020   is.            
-00001700: 7468 6520 6964 656e 7469 7479 206d 6174  the identity mat
-00001710: 7269 782e 2057 6865 6e20 6769 7665 6e20  rix. When given 
-00001720: 6173 2061 7272 6179 5f6c 696b 652c 2073  as array_like, s
-00001730: 6861 7065 3d28 332c 2033 292c 0a20 2020  hape=(3, 3),.   
-00001740: 2020 2020 2020 2020 2064 7479 7065 3d66           dtype=f
-00001750: 6c6f 6174 2e20 5768 656e 2027 4627 2c20  loat. When 'F', 
-00001760: 2749 272c 2027 4127 2c20 2743 272c 206f  'I', 'A', 'C', o
-00001770: 7220 2752 2720 6973 2067 6976 656e 2069  r 'R' is given i
-00001780: 6e73 7465 6164 206f 6620 610a 2020 2020  nstead of a.    
-00001790: 2020 2020 2020 2020 3378 3320 6d61 7472          3x3 matr
-000017a0: 6978 2c20 7468 6520 7072 696d 6974 6976  ix, the primitiv
-000017b0: 6520 6d61 7472 6978 2064 6566 696e 6564  e matrix defined
-000017c0: 2061 740a 2020 2020 2020 2020 2020 2020   at.            
-000017d0: 6874 7470 733a 2f2f 7370 676c 6962 2e67  https://spglib.g
-000017e0: 6974 6875 622e 696f 2f73 7067 6c69 622f  ithub.io/spglib/
-000017f0: 6465 6669 6e69 7469 6f6e 2e68 746d 6c20  definition.html 
-00001800: 6973 2075 7365 642e 2057 6865 6e20 2761  is used. When 'a
-00001810: 7574 6f27 0a20 2020 2020 2020 2020 2020  uto'.           
-00001820: 2069 7320 6769 7665 6e2c 2074 6865 2063   is given, the c
-00001830: 656e 7472 696e 6720 7479 7065 2028 2746  entring type ('F
-00001840: 272c 2027 4927 2c20 2741 272c 2027 4327  ', 'I', 'A', 'C'
-00001850: 2c20 2752 272c 206f 7220 7072 696d 6974  , 'R', or primit
-00001860: 6976 650a 2020 2020 2020 2020 2020 2020  ive.            
-00001870: 2750 2729 2069 7320 6175 746f 6d61 7469  'P') is automati
-00001880: 6361 6c6c 7920 6368 6f73 656e 2e0a 2020  cally chosen..  
-00001890: 2020 2020 2020 7068 6f6e 6f6e 5f73 7570        phonon_sup
-000018a0: 6572 6365 6c6c 5f6d 6174 7269 7820 3a20  ercell_matrix : 
-000018b0: 6172 7261 795f 6c69 6b65 2c20 6f70 7469  array_like, opti
-000018c0: 6f6e 616c 0a20 2020 2020 2020 2020 2020  onal.           
-000018d0: 2053 7570 6572 6365 6c6c 206d 6174 7269   Supercell matri
-000018e0: 7820 7573 6564 2066 6f72 2066 6332 2e20  x used for fc2. 
-000018f0: 496e 2070 686f 6e6f 3370 792c 2073 7570  In phono3py, sup
-00001900: 6572 6365 6c6c 206d 6174 7269 7820 666f  ercell matrix fo
-00001910: 7220 6663 330a 2020 2020 2020 2020 2020  r fc3.          
-00001920: 2020 616e 6420 6663 3220 6361 6e20 6265    and fc2 can be
-00001930: 2064 6966 6665 7265 6e74 2074 6f20 7375   different to su
-00001940: 7070 6f72 7420 6c6f 6e67 6572 2072 616e  pport longer ran
-00001950: 6765 2069 6e74 6572 6163 7469 6f6e 206f  ge interaction o
-00001960: 6620 6663 320a 2020 2020 2020 2020 2020  f fc2.          
-00001970: 2020 7468 616e 2074 6861 7420 6f66 2066    than that of f
-00001980: 6333 2e20 556e 6c65 7373 2073 6574 7469  c3. Unless setti
-00001990: 6e67 2074 6869 732c 2073 7570 6572 6365  ng this, superce
-000019a0: 6c6c 5f6d 6174 7269 7820 6973 2075 7365  ll_matrix is use
-000019b0: 642e 0a20 2020 2020 2020 2020 2020 2054  d..            T
-000019c0: 6869 7320 6973 206f 6e6c 7920 7661 6c69  his is only vali
-000019d0: 6465 2077 6865 6e20 756e 6974 6365 6c6c  de when unitcell
-000019e0: 206f 7220 756e 6974 6365 6c6c 5f66 696c   or unitcell_fil
-000019f0: 656e 616d 6520 6973 2067 6976 656e 2e0a  ename is given..
-00001a00: 2020 2020 2020 2020 2020 2020 4465 6661              Defa
-00001a10: 756c 7420 6973 204e 6f6e 652e 0a20 2020  ult is None..   
-00001a20: 2020 2020 2063 7574 6f66 665f 6672 6571       cutoff_freq
-00001a30: 7565 6e63 7920 3a20 666c 6f61 742c 206f  uency : float, o
-00001a40: 7074 696f 6e61 6c0a 2020 2020 2020 2020  ptional.        
-00001a50: 2020 2020 5068 6f6e 6f6e 2066 7265 7175      Phonon frequ
-00001a60: 656e 6379 2062 656c 6f77 2074 6869 7320  ency below this 
-00001a70: 7661 6c75 6520 6973 2069 676e 6f72 6564  value is ignored
-00001a80: 2077 6865 6e20 7468 6520 6375 746f 6666   when the cutoff
-00001a90: 2069 730a 2020 2020 2020 2020 2020 2020   is.            
-00001aa0: 6e65 6564 6564 2066 6f72 2074 6865 2063  needed for the c
-00001ab0: 6f6d 7075 7461 7469 6f6e 2e20 4465 6661  omputation. Defa
-00001ac0: 756c 7420 6973 2031 652d 342e 0a20 2020  ult is 1e-4..   
-00001ad0: 2020 2020 2066 7265 7175 656e 6379 5f66       frequency_f
-00001ae0: 6163 746f 725f 746f 5f54 487a 203a 2066  actor_to_THz : f
-00001af0: 6c6f 6174 2c20 6f70 7469 6f6e 616c 0a20  loat, optional. 
-00001b00: 2020 2020 2020 2020 2020 2050 686f 6e6f             Phono
-00001b10: 6e20 6672 6571 7565 6e63 7920 756e 6974  n frequency unit
-00001b20: 2063 6f6e 7665 7273 696f 6e20 6661 6374   conversion fact
-00001b30: 6f72 2e20 556e 6c65 7373 2073 7065 6369  or. Unless speci
-00001b40: 6669 6564 2c20 6465 6661 756c 740a 2020  fied, default.  
-00001b50: 2020 2020 2020 2020 2020 756e 6974 2063            unit c
-00001b60: 6f6e 7665 7273 696f 6e20 6661 6374 6f72  onversion factor
-00001b70: 2066 6f72 2065 6163 6820 6361 6c63 756c   for each calcul
-00001b80: 6174 6f72 2069 7320 7573 6564 2e0a 2020  ator is used..  
-00001b90: 2020 2020 2020 6973 5f73 796d 6d65 7472        is_symmetr
-00001ba0: 7920 3a20 626f 6f6c 2c20 6f70 7469 6f6e  y : bool, option
-00001bb0: 616c 0a20 2020 2020 2020 2020 2020 2055  al.            U
-00001bc0: 7365 2063 7279 7374 616c 2073 796d 6d65  se crystal symme
-00001bd0: 7472 7920 696e 206d 6f73 7420 6361 6c63  try in most calc
-00001be0: 756c 6174 696f 6e73 2077 6865 6e20 5472  ulations when Tr
-00001bf0: 7565 2e20 4465 6661 756c 7420 6973 0a20  ue. Default is. 
-00001c00: 2020 2020 2020 2020 2020 2054 7275 652e             True.
-00001c10: 0a20 2020 2020 2020 2069 735f 6d65 7368  .        is_mesh
-00001c20: 5f73 796d 6d65 7472 7920 3a20 626f 6f6c  _symmetry : bool
-00001c30: 2c20 6f70 7469 6f6e 616c 0a20 2020 2020  , optional.     
-00001c40: 2020 2020 2020 2055 7365 2063 7279 7374         Use cryst
-00001c50: 616c 2073 796d 6d65 7472 7920 696e 2072  al symmetry in r
-00001c60: 6563 6970 726f 6361 6c20 7370 6163 6520  eciprocal space 
-00001c70: 6772 6964 2068 616e 646c 696e 6720 7768  grid handling wh
-00001c80: 656e 2054 7275 652e 0a20 2020 2020 2020  en True..       
-00001c90: 2020 2020 2044 6566 6175 6c74 2069 7320       Default is 
-00001ca0: 5472 7565 2e0a 2020 2020 2020 2020 7573  True..        us
-00001cb0: 655f 6772 6720 3a20 626f 6f6c 2c20 6f70  e_grg : bool, op
-00001cc0: 7469 6f6e 616c 0a20 2020 2020 2020 2020  tional.         
-00001cd0: 2020 2055 7365 2067 656e 6572 616c 697a     Use generaliz
-00001ce0: 6564 2072 6567 756c 6172 2067 7269 6420  ed regular grid 
-00001cf0: 7768 656e 2054 7275 652e 2044 6566 6175  when True. Defau
-00001d00: 6c74 2069 7320 4661 6c73 652e 0a20 2020  lt is False..   
-00001d10: 2020 2020 2053 4e46 5f63 6f6f 7264 696e       SNF_coordin
-00001d20: 6174 6573 203a 2073 7472 2c20 6f70 7469  ates : str, opti
-00001d30: 6f6e 616c 0a20 2020 2020 2020 2020 2020  onal.           
-00001d40: 2060 7265 6369 7072 6f63 616c 6020 6f72   `reciprocal` or
-00001d50: 2060 6469 7265 6374 602e 2053 7061 6365   `direct`. Space
-00001d60: 206f 6620 636f 6f72 6469 6e61 7465 7320   of coordinates 
-00001d70: 746f 2067 656e 6572 6174 6520 6772 6964  to generate grid
-00001d80: 0a20 2020 2020 2020 2020 2020 2067 656e  .            gen
-00001d90: 6572 6174 696e 6720 6d61 7472 6978 2065  erating matrix e
-00001da0: 6974 6865 7220 696e 2064 6972 6563 7420  ither in direct 
-00001db0: 6f72 2072 6563 6970 726f 6361 6c20 7370  or reciprocal sp
-00001dc0: 6163 652e 2054 6865 2064 6566 6175 6c74  ace. The default
-00001dd0: 0a20 2020 2020 2020 2020 2020 2069 7320  .            is 
-00001de0: 6072 6563 6970 726f 6361 6c60 2e0a 2020  `reciprocal`..  
-00001df0: 2020 2020 2020 6d61 6b65 5f72 305f 6176        make_r0_av
-00001e00: 6572 6167 6520 3a20 626f 6f6c 2c20 6f70  erage : bool, op
-00001e10: 7469 6f6e 616c 0a20 2020 2020 2020 2020  tional.         
-00001e20: 2020 2066 6333 2074 7261 6e73 666f 726d     fc3 transform
-00001e30: 6174 696f 6e20 6672 6f6d 2072 6561 6c20  ation from real 
-00001e40: 746f 2072 6563 6970 726f 6361 6c20 7370  to reciprocal sp
-00001e50: 6163 6520 6973 2064 6f6e 650a 2020 2020  ace is done.    
-00001e60: 2020 2020 2020 2020 6172 6f75 6e64 2074          around t
-00001e70: 6872 6565 2061 746f 6d73 2061 6e64 2061  hree atoms and a
-00001e80: 7665 7261 6765 6420 7768 656e 2054 7275  veraged when Tru
-00001e90: 652e 2044 6566 6175 6c74 2069 7320 4661  e. Default is Fa
-00001ea0: 6c73 652c 2069 2e65 2e2c 0a20 2020 2020  lse, i.e.,.     
-00001eb0: 2020 2020 2020 206f 6e6c 7920 6172 6f75         only arou
-00001ec0: 6e64 2074 6865 2066 6972 7374 2061 746f  nd the first ato
-00001ed0: 6d2e 2053 6574 7469 6e67 2046 616c 7365  m. Setting False
-00001ee0: 2069 7320 666f 7220 726f 7567 6820 636f   is for rough co
-00001ef0: 6d70 6174 6962 696c 6974 790a 2020 2020  mpatibility.    
-00001f00: 2020 2020 2020 2020 7769 7468 2076 322e          with v2.
-00001f10: 782e 2044 6566 6175 6c74 2069 7320 5472  x. Default is Tr
-00001f20: 7565 2e0a 2020 2020 2020 2020 7379 6d70  ue..        symp
-00001f30: 7265 6320 3a20 666c 6f61 742c 206f 7074  rec : float, opt
-00001f40: 696f 6e61 6c0a 2020 2020 2020 2020 2020  ional.          
-00001f50: 2020 546f 6c65 7261 6e63 6520 7573 6564    Tolerance used
-00001f60: 2074 6f20 6669 6e64 2063 7279 7374 616c   to find crystal
-00001f70: 2073 796d 6d65 7472 792e 2044 6566 6175   symmetry. Defau
-00001f80: 6c74 2069 7320 3165 2d35 2e0a 2020 2020  lt is 1e-5..    
-00001f90: 2020 2020 6361 6c63 756c 6174 6f72 203a      calculator :
-00001fa0: 2073 7472 2c20 6f70 7469 6f6e 616c 2e0a   str, optional..
-00001fb0: 2020 2020 2020 2020 2020 2020 4361 6c63              Calc
-00001fc0: 756c 6174 6f72 2075 7365 6420 666f 7220  ulator used for 
-00001fd0: 636f 6d70 7574 696e 6720 666f 7263 6573  computing forces
-00001fe0: 2e20 5468 6973 2069 7320 7573 6564 2074  . This is used t
-00001ff0: 6f20 7377 6974 6368 2074 6865 2073 6574  o switch the set
-00002000: 0a20 2020 2020 2020 2020 2020 206f 6620  .            of 
-00002010: 7068 7973 6963 616c 2075 6e69 7473 2e20  physical units. 
-00002020: 4465 6661 756c 7420 6973 204e 6f6e 652c  Default is None,
-00002030: 2077 6869 6368 2069 7320 6571 7569 7661   which is equiva
-00002040: 6c65 6e74 2074 6f20 2276 6173 7022 2e0a  lent to "vasp"..
-00002050: 2020 2020 2020 2020 6c6f 675f 6c65 7665          log_leve
-00002060: 6c20 3a20 696e 742c 206f 7074 696f 6e61  l : int, optiona
-00002070: 6c0a 2020 2020 2020 2020 2020 2020 5665  l.            Ve
-00002080: 7262 6f73 6974 7920 636f 6e74 726f 6c2e  rbosity control.
-00002090: 2044 6566 6175 6c74 2069 7320 302e 2054   Default is 0. T
-000020a0: 6869 7320 6361 6e20 6265 2030 2c20 312c  his can be 0, 1,
-000020b0: 206f 7220 322e 0a0a 2020 2020 2020 2020   or 2...        
-000020c0: 2222 220a 2020 2020 2020 2020 7365 6c66  """.        self
-000020d0: 2e5f 7379 6d70 7265 6320 3d20 7379 6d70  ._symprec = symp
-000020e0: 7265 630a 2020 2020 2020 2020 7365 6c66  rec.        self
-000020f0: 2e5f 6672 6571 7565 6e63 795f 6661 6374  ._frequency_fact
-00002100: 6f72 5f74 6f5f 5448 7a20 3d20 6672 6571  or_to_THz = freq
-00002110: 7565 6e63 795f 6661 6374 6f72 5f74 6f5f  uency_factor_to_
-00002120: 5448 7a0a 2020 2020 2020 2020 7365 6c66  THz.        self
-00002130: 2e5f 6973 5f73 796d 6d65 7472 7920 3d20  ._is_symmetry = 
-00002140: 6973 5f73 796d 6d65 7472 790a 2020 2020  is_symmetry.    
-00002150: 2020 2020 7365 6c66 2e5f 6973 5f6d 6573      self._is_mes
-00002160: 685f 7379 6d6d 6574 7279 203d 2069 735f  h_symmetry = is_
-00002170: 6d65 7368 5f73 796d 6d65 7472 790a 2020  mesh_symmetry.  
-00002180: 2020 2020 2020 7365 6c66 2e5f 7573 655f        self._use_
-00002190: 6772 6720 3d20 7573 655f 6772 670a 2020  grg = use_grg.  
-000021a0: 2020 2020 2020 7365 6c66 2e5f 534e 465f        self._SNF_
-000021b0: 636f 6f72 6469 6e61 7465 7320 3d20 534e  coordinates = SN
-000021c0: 465f 636f 6f72 6469 6e61 7465 730a 0a20  F_coordinates.. 
-000021d0: 2020 2020 2020 2073 656c 662e 5f6d 616b         self._mak
-000021e0: 655f 7230 5f61 7665 7261 6765 203d 206d  e_r0_average = m
-000021f0: 616b 655f 7230 5f61 7665 7261 6765 0a0a  ake_r0_average..
-00002200: 2020 2020 2020 2020 7365 6c66 2e5f 6375          self._cu
-00002210: 746f 6666 5f66 7265 7175 656e 6379 203d  toff_frequency =
-00002220: 2063 7574 6f66 665f 6672 6571 7565 6e63   cutoff_frequenc
-00002230: 790a 2020 2020 2020 2020 7365 6c66 2e5f  y.        self._
-00002240: 6361 6c63 756c 6174 6f72 3a20 4f70 7469  calculator: Opti
-00002250: 6f6e 616c 5b73 7472 5d20 3d20 6361 6c63  onal[str] = calc
-00002260: 756c 6174 6f72 0a20 2020 2020 2020 2073  ulator.        s
-00002270: 656c 662e 5f6c 6f67 5f6c 6576 656c 203d  elf._log_level =
-00002280: 206c 6f67 5f6c 6576 656c 0a0a 2020 2020   log_level..    
-00002290: 2020 2020 2320 4372 6561 7465 2073 7570      # Create sup
-000022a0: 6572 6365 6c6c 2061 6e64 2070 7269 6d69  ercell and primi
-000022b0: 7469 7665 2063 656c 6c0a 2020 2020 2020  tive cell.      
-000022c0: 2020 7365 6c66 2e5f 756e 6974 6365 6c6c    self._unitcell
-000022d0: 203d 2075 6e69 7463 656c 6c0a 2020 2020   = unitcell.    
-000022e0: 2020 2020 7365 6c66 2e5f 7375 7065 7263      self._superc
-000022f0: 656c 6c5f 6d61 7472 6978 203d 206e 702e  ell_matrix = np.
-00002300: 6172 7261 7928 0a20 2020 2020 2020 2020  array(.         
-00002310: 2020 2073 6861 7065 5f73 7570 6572 6365     shape_superce
-00002320: 6c6c 5f6d 6174 7269 7828 7375 7065 7263  ll_matrix(superc
-00002330: 656c 6c5f 6d61 7472 6978 292c 2064 7479  ell_matrix), dty
-00002340: 7065 3d22 696e 745f 222c 206f 7264 6572  pe="int_", order
-00002350: 3d22 4322 0a20 2020 2020 2020 2029 0a20  ="C".        ). 
-00002360: 2020 2020 2020 2070 6d61 7420 3d20 7365         pmat = se
-00002370: 6c66 2e5f 6465 7465 726d 696e 655f 7072  lf._determine_pr
-00002380: 696d 6974 6976 655f 6d61 7472 6978 2870  imitive_matrix(p
-00002390: 7269 6d69 7469 7665 5f6d 6174 7269 7829  rimitive_matrix)
-000023a0: 0a20 2020 2020 2020 2073 656c 662e 5f70  .        self._p
-000023b0: 7269 6d69 7469 7665 5f6d 6174 7269 7820  rimitive_matrix 
-000023c0: 3d20 706d 6174 0a20 2020 2020 2020 2073  = pmat.        s
-000023d0: 656c 662e 5f6e 6163 5f70 6172 616d 7320  elf._nac_params 
-000023e0: 3d20 4e6f 6e65 0a20 2020 2020 2020 2069  = None.        i
-000023f0: 6620 7068 6f6e 6f6e 5f73 7570 6572 6365  f phonon_superce
-00002400: 6c6c 5f6d 6174 7269 7820 6973 206e 6f74  ll_matrix is not
-00002410: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
-00002420: 2020 2073 656c 662e 5f70 686f 6e6f 6e5f     self._phonon_
-00002430: 7375 7065 7263 656c 6c5f 6d61 7472 6978  supercell_matrix
-00002440: 203d 206e 702e 6172 7261 7928 0a20 2020   = np.array(.   
-00002450: 2020 2020 2020 2020 2020 2020 2073 6861               sha
-00002460: 7065 5f73 7570 6572 6365 6c6c 5f6d 6174  pe_supercell_mat
-00002470: 7269 7828 7068 6f6e 6f6e 5f73 7570 6572  rix(phonon_super
-00002480: 6365 6c6c 5f6d 6174 7269 7829 2c20 6474  cell_matrix), dt
-00002490: 7970 653d 2269 6e74 5f22 2c20 6f72 6465  ype="int_", orde
-000024a0: 723d 2243 220a 2020 2020 2020 2020 2020  r="C".          
-000024b0: 2020 290a 2020 2020 2020 2020 656c 7365    ).        else
-000024c0: 3a0a 2020 2020 2020 2020 2020 2020 7365  :.            se
-000024d0: 6c66 2e5f 7068 6f6e 6f6e 5f73 7570 6572  lf._phonon_super
-000024e0: 6365 6c6c 5f6d 6174 7269 7820 3d20 4e6f  cell_matrix = No
-000024f0: 6e65 0a20 2020 2020 2020 2073 656c 662e  ne.        self.
-00002500: 5f73 7570 6572 6365 6c6c 203d 204e 6f6e  _supercell = Non
-00002510: 650a 2020 2020 2020 2020 7365 6c66 2e5f  e.        self._
-00002520: 7072 696d 6974 6976 6520 3d20 4e6f 6e65  primitive = None
-00002530: 0a20 2020 2020 2020 2073 656c 662e 5f70  .        self._p
-00002540: 686f 6e6f 6e5f 7375 7065 7263 656c 6c20  honon_supercell 
-00002550: 3d20 4e6f 6e65 0a20 2020 2020 2020 2073  = None.        s
-00002560: 656c 662e 5f70 686f 6e6f 6e5f 7072 696d  elf._phonon_prim
-00002570: 6974 6976 6520 3d20 4e6f 6e65 0a20 2020  itive = None.   
-00002580: 2020 2020 2073 656c 662e 5f62 7569 6c64       self._build
-00002590: 5f73 7570 6572 6365 6c6c 2829 0a20 2020  _supercell().   
-000025a0: 2020 2020 2073 656c 662e 5f62 7569 6c64       self._build
-000025b0: 5f70 7269 6d69 7469 7665 5f63 656c 6c28  _primitive_cell(
-000025c0: 290a 2020 2020 2020 2020 7365 6c66 2e5f  ).        self._
-000025d0: 6275 696c 645f 7068 6f6e 6f6e 5f73 7570  build_phonon_sup
-000025e0: 6572 6365 6c6c 2829 0a20 2020 2020 2020  ercell().       
-000025f0: 2073 656c 662e 5f62 7569 6c64 5f70 686f   self._build_pho
-00002600: 6e6f 6e5f 7072 696d 6974 6976 655f 6365  non_primitive_ce
-00002610: 6c6c 2829 0a0a 2020 2020 2020 2020 7365  ll()..        se
-00002620: 6c66 2e5f 7369 676d 6173 203d 205b 0a20  lf._sigmas = [. 
-00002630: 2020 2020 2020 2020 2020 204e 6f6e 652c             None,
-00002640: 0a20 2020 2020 2020 205d 0a20 2020 2020  .        ].     
-00002650: 2020 2073 656c 662e 5f73 6967 6d61 5f63     self._sigma_c
-00002660: 7574 6f66 6620 3d20 4e6f 6e65 0a0a 2020  utoff = None..  
-00002670: 2020 2020 2020 2320 4772 6964 0a20 2020        # Grid.   
-00002680: 2020 2020 2073 656c 662e 5f62 7a5f 6772       self._bz_gr
-00002690: 6964 203d 204e 6f6e 650a 0a20 2020 2020  id = None..     
-000026a0: 2020 2023 2053 6574 2073 7570 6572 6365     # Set superce
-000026b0: 6c6c 2c20 7072 696d 6974 6976 652c 2061  ll, primitive, a
-000026c0: 6e64 2070 686f 6e6f 6e20 7375 7065 7263  nd phonon superc
-000026d0: 656c 6c20 7379 6d6d 6574 7269 6573 0a20  ell symmetries. 
-000026e0: 2020 2020 2020 2073 656c 662e 5f73 796d         self._sym
-000026f0: 6d65 7472 7920 3d20 4e6f 6e65 0a20 2020  metry = None.   
-00002700: 2020 2020 2073 656c 662e 5f70 7269 6d69       self._primi
-00002710: 7469 7665 5f73 796d 6d65 7472 7920 3d20  tive_symmetry = 
-00002720: 4e6f 6e65 0a20 2020 2020 2020 2073 656c  None.        sel
-00002730: 662e 5f70 686f 6e6f 6e5f 7375 7065 7263  f._phonon_superc
-00002740: 656c 6c5f 7379 6d6d 6574 7279 203d 204e  ell_symmetry = N
-00002750: 6f6e 650a 2020 2020 2020 2020 7365 6c66  one.        self
-00002760: 2e5f 7365 6172 6368 5f73 796d 6d65 7472  ._search_symmetr
-00002770: 7928 290a 2020 2020 2020 2020 7365 6c66  y().        self
-00002780: 2e5f 7365 6172 6368 5f70 7269 6d69 7469  ._search_primiti
-00002790: 7665 5f73 796d 6d65 7472 7928 290a 2020  ve_symmetry().  
-000027a0: 2020 2020 2020 7365 6c66 2e5f 7365 6172        self._sear
-000027b0: 6368 5f70 686f 6e6f 6e5f 7375 7065 7263  ch_phonon_superc
-000027c0: 656c 6c5f 7379 6d6d 6574 7279 2829 0a0a  ell_symmetry()..
-000027d0: 2020 2020 2020 2020 2320 4469 7370 6c61          # Displa
-000027e0: 6365 6d65 6e74 7320 616e 6420 7375 7065  cements and supe
-000027f0: 7263 656c 6c73 0a20 2020 2020 2020 2073  rcells.        s
-00002800: 656c 662e 5f73 7570 6572 6365 6c6c 735f  elf._supercells_
-00002810: 7769 7468 5f64 6973 706c 6163 656d 656e  with_displacemen
-00002820: 7473 203d 204e 6f6e 650a 2020 2020 2020  ts = None.      
-00002830: 2020 7365 6c66 2e5f 6461 7461 7365 7420    self._dataset 
-00002840: 3d20 4e6f 6e65 0a20 2020 2020 2020 2073  = None.        s
-00002850: 656c 662e 5f70 686f 6e6f 6e5f 6461 7461  elf._phonon_data
-00002860: 7365 7420 3d20 4e6f 6e65 0a20 2020 2020  set = None.     
-00002870: 2020 2073 656c 662e 5f70 686f 6e6f 6e5f     self._phonon_
-00002880: 7375 7065 7263 656c 6c73 5f77 6974 685f  supercells_with_
-00002890: 6469 7370 6c61 6365 6d65 6e74 7320 3d20  displacements = 
-000028a0: 4e6f 6e65 0a0a 2020 2020 2020 2020 2320  None..        # 
-000028b0: 5468 6572 6d61 6c20 636f 6e64 7563 7469  Thermal conducti
-000028c0: 7669 7479 0a20 2020 2020 2020 2023 2063  vity.        # c
-000028d0: 6f6e 6475 6374 6976 6974 795f 5254 4120  onductivity_RTA 
-000028e0: 6f72 2063 6f6e 6475 6374 6976 6974 795f  or conductivity_
-000028f0: 4c42 5445 2063 6c61 7373 2069 6e73 7461  LBTE class insta
-00002900: 6e63 650a 2020 2020 2020 2020 7365 6c66  nce.        self
-00002910: 2e5f 7468 6572 6d61 6c5f 636f 6e64 7563  ._thermal_conduc
-00002920: 7469 7669 7479 203d 204e 6f6e 650a 0a20  tivity = None.. 
-00002930: 2020 2020 2020 2023 2049 6d61 6769 6e61         # Imagina
-00002940: 7279 2070 6172 7420 6f66 2073 656c 6620  ry part of self 
-00002950: 656e 6572 6779 2061 7420 6672 6571 7565  energy at freque
-00002960: 6e63 7920 706f 696e 7473 0a20 2020 2020  ncy points.     
-00002970: 2020 2073 656c 662e 5f67 616d 6d61 7320     self._gammas 
-00002980: 3d20 4e6f 6e65 0a20 2020 2020 2020 2073  = None.        s
-00002990: 656c 662e 5f73 6361 7474 6572 696e 675f  elf._scattering_
-000029a0: 6576 656e 745f 636c 6173 7320 3d20 4e6f  event_class = No
-000029b0: 6e65 0a0a 2020 2020 2020 2020 2320 4672  ne..        # Fr
-000029c0: 6571 7565 6e63 7920 7368 6966 7420 2872  equency shift (r
-000029d0: 6561 6c20 7061 7274 206f 6620 6275 6262  eal part of bubb
-000029e0: 6c65 2064 6961 6772 616d 290a 2020 2020  le diagram).    
-000029f0: 2020 2020 7365 6c66 2e5f 7265 616c 5f73      self._real_s
-00002a00: 656c 665f 656e 6572 6779 203d 204e 6f6e  elf_energy = Non
-00002a10: 650a 0a20 2020 2020 2020 2073 656c 662e  e..        self.
-00002a20: 5f67 7269 645f 706f 696e 7473 203d 204e  _grid_points = N
-00002a30: 6f6e 650a 2020 2020 2020 2020 7365 6c66  one.        self
-00002a40: 2e5f 6672 6571 7565 6e63 795f 706f 696e  ._frequency_poin
-00002a50: 7473 203d 204e 6f6e 650a 2020 2020 2020  ts = None.      
-00002a60: 2020 7365 6c66 2e5f 7465 6d70 6572 6174    self._temperat
-00002a70: 7572 6573 203d 204e 6f6e 650a 0a20 2020  ures = None..   
-00002a80: 2020 2020 2023 204f 7468 6572 2076 6172       # Other var
-00002a90: 6961 626c 6573 0a20 2020 2020 2020 2073  iables.        s
-00002aa0: 656c 662e 5f66 6332 203d 204e 6f6e 650a  elf._fc2 = None.
-00002ab0: 2020 2020 2020 2020 7365 6c66 2e5f 6663          self._fc
-00002ac0: 3320 3d20 4e6f 6e65 0a0a 2020 2020 2020  3 = None..      
-00002ad0: 2020 2320 5365 7475 7020 696e 7465 7261    # Setup intera
-00002ae0: 6374 696f 6e0a 2020 2020 2020 2020 7365  ction.        se
-00002af0: 6c66 2e5f 696e 7465 7261 6374 696f 6e20  lf._interaction 
-00002b00: 3d20 4e6f 6e65 0a20 2020 2020 2020 2073  = None.        s
-00002b10: 656c 662e 5f62 616e 645f 696e 6469 6365  elf._band_indice
-00002b20: 7320 3d20 4e6f 6e65 0a20 2020 2020 2020  s = None.       
-00002b30: 2073 656c 662e 5f62 616e 645f 696e 6469   self._band_indi
-00002b40: 6365 735f 666c 6174 7465 6e20 3d20 4e6f  ces_flatten = No
-00002b50: 6e65 0a20 2020 2020 2020 2073 656c 662e  ne.        self.
-00002b60: 5f73 6574 5f62 616e 645f 696e 6469 6365  _set_band_indice
-00002b70: 7328 290a 0a20 2020 2040 7072 6f70 6572  s()..    @proper
-00002b80: 7479 0a20 2020 2064 6566 2076 6572 7369  ty.    def versi
-00002b90: 6f6e 2873 656c 6629 3a0a 2020 2020 2020  on(self):.      
-00002ba0: 2020 2222 2252 6574 7572 6e20 7068 6f6e    """Return phon
-00002bb0: 6f33 7079 2072 656c 6561 7365 2076 6572  o3py release ver
-00002bc0: 7369 6f6e 206e 756d 6265 722e 0a0a 2020  sion number...  
-00002bd0: 2020 2020 2020 7374 720a 2020 2020 2020        str.      
-00002be0: 2020 2020 2020 5068 6f6e 6f33 7079 2072        Phono3py r
-00002bf0: 656c 6561 7365 2076 6572 7369 6f6e 206e  elease version n
-00002c00: 756d 6265 720a 0a20 2020 2020 2020 2022  umber..        "
-00002c10: 2222 0a20 2020 2020 2020 2072 6574 7572  "".        retur
-00002c20: 6e20 5f5f 7665 7273 696f 6e5f 5f0a 0a20  n __version__.. 
-00002c30: 2020 2040 7072 6f70 6572 7479 0a20 2020     @property.   
-00002c40: 2064 6566 2063 616c 6375 6c61 746f 7228   def calculator(
-00002c50: 7365 6c66 2920 2d3e 204f 7074 696f 6e61  self) -> Optiona
-00002c60: 6c5b 7374 725d 3a0a 2020 2020 2020 2020  l[str]:.        
-00002c70: 2222 2252 6574 7572 6e20 6361 6c63 756c  """Return calcul
-00002c80: 6174 6f72 2069 6e74 6572 6661 6365 206e  ator interface n
-00002c90: 616d 652e 0a0a 2020 2020 2020 2020 7374  ame...        st
-00002ca0: 720a 2020 2020 2020 2020 2020 2020 4361  r.            Ca
-00002cb0: 6c63 756c 6174 6f72 206e 616d 6520 7375  lculator name su
-00002cc0: 6368 2061 7320 2776 6173 7027 2c20 2771  ch as 'vasp', 'q
-00002cd0: 6527 2c20 6574 632e 0a0a 2020 2020 2020  e', etc...      
-00002ce0: 2020 2222 220a 2020 2020 2020 2020 7265    """.        re
-00002cf0: 7475 726e 2073 656c 662e 5f63 616c 6375  turn self._calcu
-00002d00: 6c61 746f 720a 0a20 2020 2040 7072 6f70  lator..    @prop
-00002d10: 6572 7479 0a20 2020 2064 6566 2066 6333  erty.    def fc3
-00002d20: 2873 656c 6629 3a0a 2020 2020 2020 2020  (self):.        
-00002d30: 2222 2253 6574 7465 7220 616e 6420 6765  """Setter and ge
-00002d40: 7474 6572 206f 6620 7468 6972 6420 6f72  tter of third or
-00002d50: 6465 7220 666f 7263 6520 636f 6e73 7461  der force consta
-00002d60: 6e74 7320 2866 6333 292e 0a0a 2020 2020  nts (fc3)...    
-00002d70: 2020 2020 6e64 6172 7261 790a 2020 2020      ndarray.    
-00002d80: 2020 2020 2020 2020 6663 3320 7368 6170          fc3 shap
-00002d90: 6520 6973 2065 6974 6865 7220 2873 7570  e is either (sup
-00002da0: 6572 6365 6c6c 2c20 7375 7065 6365 6c6c  ercell, supecell
-00002db0: 2c20 7375 7065 7263 656c 6c2c 2033 2c20  , supercell, 3, 
-00002dc0: 332c 2033 2920 6f72 0a20 2020 2020 2020  3, 3) or.       
-00002dd0: 2020 2020 2028 7072 696d 6974 6976 652c       (primitive,
-00002de0: 2073 7570 6572 6365 6c6c 2c20 7375 7065   supercell, supe
-00002df0: 6365 6c6c 2c20 332c 2033 2c20 3329 2c0a  cell, 3, 3, 3),.
-00002e00: 2020 2020 2020 2020 2020 2020 7768 6572              wher
-00002e10: 6520 2773 7570 6572 6365 6c6c 2720 616e  e 'supercell' an
-00002e20: 6420 2770 7269 6d69 7469 7665 2720 696e  d 'primitive' in
-00002e30: 6469 6361 7465 206e 756d 6265 7220 6f66  dicate number of
-00002e40: 2061 746f 6d73 2069 6e0a 2020 2020 2020   atoms in.      
-00002e50: 2020 2020 2020 7468 6573 6520 6365 6c6c        these cell
-00002e60: 732e 0a0a 2020 2020 2020 2020 2222 220a  s...        """.
-00002e70: 2020 2020 2020 2020 7265 7475 726e 2073          return s
-00002e80: 656c 662e 5f66 6333 0a0a 2020 2020 4066  elf._fc3..    @f
-00002e90: 6333 2e73 6574 7465 720a 2020 2020 6465  c3.setter.    de
-00002ea0: 6620 6663 3328 7365 6c66 2c20 6663 3329  f fc3(self, fc3)
-00002eb0: 3a0a 2020 2020 2020 2020 7365 6c66 2e5f  :.        self._
-00002ec0: 6663 3320 3d20 6663 330a 0a20 2020 2040  fc3 = fc3..    @
-00002ed0: 7072 6f70 6572 7479 0a20 2020 2064 6566  property.    def
-00002ee0: 2066 6332 2873 656c 6629 3a0a 2020 2020   fc2(self):.    
-00002ef0: 2020 2020 2222 2253 6574 7465 7220 616e      """Setter an
-00002f00: 6420 6765 7474 6572 206f 6620 7365 636f  d getter of seco
-00002f10: 6e64 206f 7264 6572 2066 6f72 6365 2063  nd order force c
-00002f20: 6f6e 7374 616e 7473 2028 6663 3229 2e0a  onstants (fc2)..
-00002f30: 0a20 2020 2020 2020 206e 6461 7272 6179  .        ndarray
-00002f40: 0a20 2020 2020 2020 2020 2020 2066 6332  .            fc2
-00002f50: 2073 6861 7065 2069 7320 6569 7468 6572   shape is either
-00002f60: 2028 7375 7065 7263 656c 6c2c 2073 7570   (supercell, sup
-00002f70: 6563 656c 6c2c 2033 2c20 3329 206f 720a  ecell, 3, 3) or.
-00002f80: 2020 2020 2020 2020 2020 2020 2870 7269              (pri
-00002f90: 6d69 7469 7665 2c20 7375 7065 6365 6c6c  mitive, supecell
-00002fa0: 2c20 332c 2033 292c 0a20 2020 2020 2020  , 3, 3),.       
-00002fb0: 2020 2020 2077 6865 7265 2027 7375 7065       where 'supe
-00002fc0: 7263 656c 6c27 2061 6e64 2027 7072 696d  rcell' and 'prim
-00002fd0: 6974 6976 6527 2069 6e64 6963 6174 6520  itive' indicate 
-00002fe0: 6e75 6d62 6572 206f 6620 6174 6f6d 7320  number of atoms 
-00002ff0: 696e 0a20 2020 2020 2020 2020 2020 2074  in.            t
-00003000: 6865 7365 2063 656c 6c73 2e0a 0a20 2020  hese cells...   
-00003010: 2020 2020 2022 2222 0a20 2020 2020 2020       """.       
-00003020: 2072 6574 7572 6e20 7365 6c66 2e5f 6663   return self._fc
-00003030: 320a 0a20 2020 2040 6663 322e 7365 7474  2..    @fc2.sett
-00003040: 6572 0a20 2020 2064 6566 2066 6332 2873  er.    def fc2(s
-00003050: 656c 662c 2066 6332 293a 0a20 2020 2020  elf, fc2):.     
-00003060: 2020 2073 656c 662e 5f66 6332 203d 2066     self._fc2 = f
-00003070: 6332 0a0a 2020 2020 4070 726f 7065 7274  c2..    @propert
-00003080: 790a 2020 2020 6465 6620 666f 7263 655f  y.    def force_
-00003090: 636f 6e73 7461 6e74 7328 7365 6c66 293a  constants(self):
-000030a0: 0a20 2020 2020 2020 2022 2222 5265 7475  .        """Retu
-000030b0: 726e 2066 6332 2e20 5468 6973 2069 7320  rn fc2. This is 
-000030c0: 7361 6d65 2061 7320 7468 6520 6765 7474  same as the gett
-000030d0: 6572 2061 7474 7269 6275 7465 2060 6663  er attribute `fc
-000030e0: 3260 2e22 2222 0a20 2020 2020 2020 2072  2`.""".        r
-000030f0: 6574 7572 6e20 7365 6c66 2e66 6332 0a0a  eturn self.fc2..
-00003100: 2020 2020 4070 726f 7065 7274 790a 2020      @property.  
-00003110: 2020 6465 6620 7369 676d 6173 2873 656c    def sigmas(sel
-00003120: 6629 3a0a 2020 2020 2020 2020 2222 2253  f):.        """S
-00003130: 6574 7465 7220 616e 6420 6765 7474 6572  etter and getter
-00003140: 206f 6620 736d 6561 7269 6e67 2077 6964   of smearing wid
-00003150: 7468 732e 0a0a 2020 2020 2020 2020 6c69  ths...        li
-00003160: 7374 0a20 2020 2020 2020 2020 2020 2054  st.            T
-00003170: 6865 2066 6c6f 6174 2076 616c 7565 7320  he float values 
-00003180: 6172 6520 6769 7665 6e20 6173 2074 6865  are given as the
-00003190: 2073 7461 6e64 6172 6420 6465 7669 6174   standard deviat
-000031a0: 696f 6e73 206f 6620 4761 7573 7369 616e  ions of Gaussian
-000031b0: 0a20 2020 2020 2020 2020 2020 2066 756e  .            fun
-000031c0: 6374 696f 6e2e 2049 6620 4e6f 6e65 2069  ction. If None i
-000031d0: 7320 6769 7665 6e20 6173 2061 6e20 656c  s given as an el
-000031e0: 656d 656e 7420 6f66 2074 6869 7320 6c69  ement of this li
-000031f0: 7374 2c20 6c69 6e65 6172 0a20 2020 2020  st, linear.     
-00003200: 2020 2020 2020 2074 6574 7261 6865 6472         tetrahedr
-00003210: 6f6e 206d 6574 686f 6420 6973 2075 7365  on method is use
-00003220: 6420 696e 7374 6561 6420 6f66 2073 6d65  d instead of sme
-00003230: 6172 696e 6720 6d65 7468 6f64 2e0a 0a20  aring method... 
-00003240: 2020 2020 2020 2022 2222 0a20 2020 2020         """.     
-00003250: 2020 2072 6574 7572 6e20 7365 6c66 2e5f     return self._
-00003260: 7369 676d 6173 0a0a 2020 2020 4073 6967  sigmas..    @sig
-00003270: 6d61 732e 7365 7474 6572 0a20 2020 2064  mas.setter.    d
-00003280: 6566 2073 6967 6d61 7328 7365 6c66 2c20  ef sigmas(self, 
-00003290: 7369 676d 6173 293a 0a20 2020 2020 2020  sigmas):.       
-000032a0: 2069 6620 7369 676d 6173 2069 7320 4e6f   if sigmas is No
-000032b0: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
-000032c0: 7365 6c66 2e5f 7369 676d 6173 203d 205b  self._sigmas = [
-000032d0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000032e0: 204e 6f6e 652c 0a20 2020 2020 2020 2020   None,.         
-000032f0: 2020 205d 0a20 2020 2020 2020 2065 6c69     ].        eli
-00003300: 6620 6973 696e 7374 616e 6365 2873 6967  f isinstance(sig
-00003310: 6d61 732c 2066 6c6f 6174 2920 6f72 2069  mas, float) or i
-00003320: 7369 6e73 7461 6e63 6528 7369 676d 6173  sinstance(sigmas
-00003330: 2c20 696e 7429 3a0a 2020 2020 2020 2020  , int):.        
-00003340: 2020 2020 7365 6c66 2e5f 7369 676d 6173      self._sigmas
-00003350: 203d 205b 0a20 2020 2020 2020 2020 2020   = [.           
-00003360: 2020 2020 2066 6c6f 6174 2873 6967 6d61       float(sigma
-00003370: 7329 2c0a 2020 2020 2020 2020 2020 2020  s),.            
-00003380: 5d0a 2020 2020 2020 2020 656c 7365 3a0a  ].        else:.
-00003390: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-000033a0: 2e5f 7369 676d 6173 203d 205b 5d0a 2020  ._sigmas = [].  
-000033b0: 2020 2020 2020 2020 2020 666f 7220 7320            for s 
-000033c0: 696e 2073 6967 6d61 733a 0a20 2020 2020  in sigmas:.     
-000033d0: 2020 2020 2020 2020 2020 2069 6620 6973             if is
-000033e0: 696e 7374 616e 6365 2873 2c20 666c 6f61  instance(s, floa
-000033f0: 7429 206f 7220 6973 696e 7374 616e 6365  t) or isinstance
-00003400: 2873 2c20 696e 7429 3a0a 2020 2020 2020  (s, int):.      
-00003410: 2020 2020 2020 2020 2020 2020 2020 7365                se
-00003420: 6c66 2e5f 7369 676d 6173 2e61 7070 656e  lf._sigmas.appen
-00003430: 6428 666c 6f61 7428 7329 290a 2020 2020  d(float(s)).    
-00003440: 2020 2020 2020 2020 2020 2020 656c 6966              elif
-00003450: 2073 2069 7320 4e6f 6e65 3a0a 2020 2020   s is None:.    
-00003460: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003470: 7365 6c66 2e5f 7369 676d 6173 2e61 7070  self._sigmas.app
-00003480: 656e 6428 4e6f 6e65 290a 0a20 2020 2040  end(None)..    @
-00003490: 7072 6f70 6572 7479 0a20 2020 2064 6566  property.    def
-000034a0: 2073 6967 6d61 5f63 7574 6f66 6628 7365   sigma_cutoff(se
-000034b0: 6c66 293a 0a20 2020 2020 2020 2022 2222  lf):.        """
-000034c0: 5365 7474 6572 2061 6e64 2067 6574 7465  Setter and gette
-000034d0: 7220 6f66 2053 6d65 6172 696e 6720 6375  r of Smearing cu
-000034e0: 746f 6666 2077 6964 7468 2e0a 0a20 2020  toff width...   
-000034f0: 2020 2020 2054 6869 7320 6973 2067 6976       This is giv
-00003500: 656e 2061 7320 6120 6d75 6c74 6970 6c65  en as a multiple
-00003510: 206f 6620 7468 6520 7374 616e 6461 7264   of the standard
-00003520: 2064 6576 6961 7469 6f6e 2e0a 0a20 2020   deviation...   
-00003530: 2020 2020 2066 6c6f 6174 0a20 2020 2020       float.     
-00003540: 2020 2020 2020 2046 6f72 2065 7861 6d70         For examp
-00003550: 6c65 2c20 6966 2074 6869 7320 7661 6c75  le, if this valu
-00003560: 6520 6973 2035 2c20 7468 6520 7461 696c  e is 5, the tail
-00003570: 206f 6620 7468 6520 4761 7573 7369 616e   of the Gaussian
-00003580: 2066 756e 6374 696f 6e0a 2020 2020 2020   function.      
-00003590: 2020 2020 2020 6973 2063 7574 2061 7420        is cut at 
-000035a0: 3520 7369 676d 612e 0a0a 2020 2020 2020  5 sigma...      
-000035b0: 2020 2222 220a 2020 2020 2020 2020 7265    """.        re
-000035c0: 7475 726e 2073 656c 662e 5f73 6967 6d61  turn self._sigma
-000035d0: 5f63 7574 6f66 660a 0a20 2020 2040 7369  _cutoff..    @si
-000035e0: 676d 615f 6375 746f 6666 2e73 6574 7465  gma_cutoff.sette
-000035f0: 720a 2020 2020 6465 6620 7369 676d 615f  r.    def sigma_
-00003600: 6375 746f 6666 2873 656c 662c 2073 6967  cutoff(self, sig
-00003610: 6d61 5f63 7574 6f66 6629 3a0a 2020 2020  ma_cutoff):.    
-00003620: 2020 2020 7365 6c66 2e5f 7369 676d 615f      self._sigma_
-00003630: 6375 746f 6666 203d 2073 6967 6d61 5f63  cutoff = sigma_c
-00003640: 7574 6f66 660a 0a20 2020 2040 7072 6f70  utoff..    @prop
-00003650: 6572 7479 0a20 2020 2064 6566 206e 6163  erty.    def nac
-00003660: 5f70 6172 616d 7328 7365 6c66 293a 0a20  _params(self):. 
-00003670: 2020 2020 2020 2022 2222 5365 7474 6572         """Setter
-00003680: 2061 6e64 2067 6574 7465 7220 6f66 2070   and getter of p
-00003690: 6172 616d 6574 6572 7320 666f 7220 6e6f  arameters for no
-000036a0: 6e2d 616e 616c 7974 6963 616c 2074 6572  n-analytical ter
-000036b0: 6d20 636f 7272 6563 7469 6f6e 2e0a 0a20  m correction... 
-000036c0: 2020 2020 2020 2064 6963 740a 2020 2020         dict.    
-000036d0: 2020 2020 2020 2020 5061 7261 6d65 7465          Paramete
-000036e0: 7273 2075 7365 6420 666f 7220 6e6f 6e2d  rs used for non-
-000036f0: 616e 616c 7974 6963 616c 2074 6572 6d20  analytical term 
-00003700: 636f 7272 6563 7469 6f6e 0a20 2020 2020  correction.     
-00003710: 2020 2020 2020 2027 626f 726e 273a 206e         'born': n
-00003720: 6461 7272 6179 0a20 2020 2020 2020 2020  darray.         
-00003730: 2020 2020 2020 2042 6f72 6e20 6566 6665         Born effe
-00003740: 6374 6976 6520 6368 6172 6765 730a 2020  ctive charges.  
-00003750: 2020 2020 2020 2020 2020 2020 2020 7368                sh
-00003760: 6170 653d 2870 7269 6d69 7469 7665 2063  ape=(primitive c
-00003770: 656c 6c20 6174 6f6d 732c 2033 2c20 3329  ell atoms, 3, 3)
-00003780: 2c20 6474 7970 653d 2764 6f75 626c 6527  , dtype='double'
-00003790: 2c20 6f72 6465 723d 2743 270a 2020 2020  , order='C'.    
-000037a0: 2020 2020 2020 2020 2766 6163 746f 7227          'factor'
-000037b0: 3a20 666c 6f61 740a 2020 2020 2020 2020  : float.        
-000037c0: 2020 2020 2020 2020 556e 6974 2063 6f6e          Unit con
-000037d0: 7665 7273 696f 6e20 6661 6374 6f72 0a20  version factor. 
-000037e0: 2020 2020 2020 2020 2020 2027 6469 656c             'diel
-000037f0: 6563 7472 6963 273a 206e 6461 7272 6179  ectric': ndarray
-00003800: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00003810: 2044 6965 6c65 6374 7269 6320 636f 6e73   Dielectric cons
-00003820: 7461 6e74 2074 656e 736f 720a 2020 2020  tant tensor.    
-00003830: 2020 2020 2020 2020 2020 2020 7368 6170              shap
-00003840: 653d 2833 2c20 3329 2c20 6474 7970 653d  e=(3, 3), dtype=
-00003850: 2764 6f75 626c 6527 2c20 6f72 6465 723d  'double', order=
-00003860: 2743 270a 0a20 2020 2020 2020 2022 2222  'C'..        """
-00003870: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
-00003880: 7365 6c66 2e5f 6e61 635f 7061 7261 6d73  self._nac_params
-00003890: 0a0a 2020 2020 406e 6163 5f70 6172 616d  ..    @nac_param
-000038a0: 732e 7365 7474 6572 0a20 2020 2064 6566  s.setter.    def
-000038b0: 206e 6163 5f70 6172 616d 7328 7365 6c66   nac_params(self
-000038c0: 2c20 6e61 635f 7061 7261 6d73 293a 0a20  , nac_params):. 
-000038d0: 2020 2020 2020 2073 656c 662e 5f6e 6163         self._nac
-000038e0: 5f70 6172 616d 7320 3d20 6e61 635f 7061  _params = nac_pa
-000038f0: 7261 6d73 0a20 2020 2020 2020 2069 6620  rams.        if 
-00003900: 7365 6c66 2e5f 696e 7465 7261 6374 696f  self._interactio
-00003910: 6e20 6973 206e 6f74 204e 6f6e 653a 0a20  n is not None:. 
-00003920: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-00003930: 5f69 6e69 745f 6479 6e61 6d69 6361 6c5f  _init_dynamical_
-00003940: 6d61 7472 6978 2829 0a0a 2020 2020 4070  matrix()..    @p
-00003950: 726f 7065 7274 790a 2020 2020 6465 6620  roperty.    def 
-00003960: 6479 6e61 6d69 6361 6c5f 6d61 7472 6978  dynamical_matrix
-00003970: 2873 656c 6629 3a0a 2020 2020 2020 2020  (self):.        
-00003980: 2222 2252 6574 7572 6e20 4479 6e61 6d69  """Return Dynami
-00003990: 6361 6c4d 6174 7269 7820 696e 7374 616e  calMatrix instan
-000039a0: 6365 2e0a 0a20 2020 2020 2020 2054 6869  ce...        Thi
-000039b0: 7320 6973 206e 6f74 2064 796e 616d 6963  s is not dynamic
-000039c0: 616c 206d 6174 7269 6365 7320 6275 7420  al matrices but 
-000039d0: 7468 6520 696e 7374 616e 6365 206f 6620  the instance of 
-000039e0: 4479 6e61 6d69 6361 6c4d 6174 7269 780a  DynamicalMatrix.
-000039f0: 2020 2020 2020 2020 636c 6173 732e 0a0a          class...
-00003a00: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
-00003a10: 2020 2020 6966 2073 656c 662e 5f69 6e74      if self._int
-00003a20: 6572 6163 7469 6f6e 2069 7320 4e6f 6e65  eraction is None
-00003a30: 3a0a 2020 2020 2020 2020 2020 2020 7265  :.            re
-00003a40: 7475 726e 204e 6f6e 650a 2020 2020 2020  turn None.      
-00003a50: 2020 656c 7365 3a0a 2020 2020 2020 2020    else:.        
-00003a60: 2020 2020 7265 7475 726e 2073 656c 662e      return self.
-00003a70: 5f69 6e74 6572 6163 7469 6f6e 2e64 796e  _interaction.dyn
-00003a80: 616d 6963 616c 5f6d 6174 7269 780a 0a20  amical_matrix.. 
-00003a90: 2020 2040 7072 6f70 6572 7479 0a20 2020     @property.   
-00003aa0: 2064 6566 2070 7269 6d69 7469 7665 2873   def primitive(s
-00003ab0: 656c 6629 202d 3e20 5072 696d 6974 6976  elf) -> Primitiv
-00003ac0: 653a 0a20 2020 2020 2020 2022 2222 5265  e:.        """Re
-00003ad0: 7475 726e 2070 7269 6d69 7469 7665 2063  turn primitive c
-00003ae0: 656c 6c2e 0a0a 2020 2020 2020 2020 5072  ell...        Pr
-00003af0: 696d 6974 6976 650a 2020 2020 2020 2020  imitive.        
-00003b00: 2020 2020 5072 696d 6974 6976 6520 6365      Primitive ce
-00003b10: 6c6c 2e0a 0a20 2020 2020 2020 2022 2222  ll...        """
-00003b20: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
-00003b30: 7365 6c66 2e5f 7072 696d 6974 6976 650a  self._primitive.
-00003b40: 0a20 2020 2040 7072 6f70 6572 7479 0a20  .    @property. 
-00003b50: 2020 2064 6566 2075 6e69 7463 656c 6c28     def unitcell(
-00003b60: 7365 6c66 2920 2d3e 2050 686f 6e6f 7079  self) -> Phonopy
-00003b70: 4174 6f6d 733a 0a20 2020 2020 2020 2022  Atoms:.        "
-00003b80: 2222 5265 7475 726e 2055 6e69 7420 6365  ""Return Unit ce
-00003b90: 6c6c 2e0a 0a20 2020 2020 2020 2050 686f  ll...        Pho
-00003ba0: 6e6f 7079 4174 6f6d 730a 2020 2020 2020  nopyAtoms.      
-00003bb0: 2020 2020 2020 556e 6974 2063 656c 6c2e        Unit cell.
-00003bc0: 0a0a 2020 2020 2020 2020 2222 220a 2020  ..        """.  
-00003bd0: 2020 2020 2020 7265 7475 726e 2073 656c        return sel
-00003be0: 662e 5f75 6e69 7463 656c 6c0a 0a20 2020  f._unitcell..   
-00003bf0: 2040 7072 6f70 6572 7479 0a20 2020 2064   @property.    d
-00003c00: 6566 2073 7570 6572 6365 6c6c 2873 656c  ef supercell(sel
-00003c10: 6629 202d 3e20 5375 7065 7263 656c 6c3a  f) -> Supercell:
-00003c20: 0a20 2020 2020 2020 2022 2222 5265 7475  .        """Retu
-00003c30: 726e 2073 7570 6572 6365 6c6c 2e0a 0a20  rn supercell... 
-00003c40: 2020 2020 2020 2053 7570 6572 6365 6c6c         Supercell
-00003c50: 0a20 2020 2020 2020 2020 2020 2053 7570  .            Sup
-00003c60: 6572 6365 6c6c 2e0a 0a20 2020 2020 2020  ercell...       
-00003c70: 2022 2222 0a20 2020 2020 2020 2072 6574   """.        ret
-00003c80: 7572 6e20 7365 6c66 2e5f 7375 7065 7263  urn self._superc
-00003c90: 656c 6c0a 0a20 2020 2040 7072 6f70 6572  ell..    @proper
-00003ca0: 7479 0a20 2020 2064 6566 2070 686f 6e6f  ty.    def phono
-00003cb0: 6e5f 7375 7065 7263 656c 6c28 7365 6c66  n_supercell(self
-00003cc0: 2920 2d3e 2053 7570 6572 6365 6c6c 3a0a  ) -> Supercell:.
-00003cd0: 2020 2020 2020 2020 2222 2252 6574 7572          """Retur
-00003ce0: 6e20 7375 7065 7263 656c 6c20 666f 7220  n supercell for 
-00003cf0: 6663 322e 0a0a 2020 2020 2020 2020 5375  fc2...        Su
-00003d00: 7065 7263 656c 6c0a 2020 2020 2020 2020  percell.        
-00003d10: 2020 2020 5375 7065 7263 656c 6c20 666f      Supercell fo
-00003d20: 7220 6663 322e 0a0a 2020 2020 2020 2020  r fc2...        
-00003d30: 2222 220a 2020 2020 2020 2020 7265 7475  """.        retu
-00003d40: 726e 2073 656c 662e 5f70 686f 6e6f 6e5f  rn self._phonon_
-00003d50: 7375 7065 7263 656c 6c0a 0a20 2020 2040  supercell..    @
-00003d60: 7072 6f70 6572 7479 0a20 2020 2064 6566  property.    def
-00003d70: 2070 686f 6e6f 6e5f 7072 696d 6974 6976   phonon_primitiv
-00003d80: 6528 7365 6c66 2920 2d3e 2050 7269 6d69  e(self) -> Primi
-00003d90: 7469 7665 3a0a 2020 2020 2020 2020 2222  tive:.        ""
-00003da0: 2252 6574 7572 6e20 7072 696d 6974 6976  "Return primitiv
-00003db0: 6520 6365 6c6c 2066 6f72 2066 6332 2e0a  e cell for fc2..
-00003dc0: 0a20 2020 2020 2020 2050 7269 6d69 7469  .        Primiti
-00003dd0: 7665 0a20 2020 2020 2020 2020 2020 2050  ve.            P
-00003de0: 7269 6d69 7469 7665 2063 656c 6c20 666f  rimitive cell fo
-00003df0: 7220 6663 322e 2054 6869 7320 7368 6f75  r fc2. This shou
-00003e00: 6c64 2062 6520 7468 6520 7361 6d65 2061  ld be the same a
-00003e10: 7320 7468 6520 7072 696d 6974 6976 650a  s the primitive.
-00003e20: 2020 2020 2020 2020 2020 2020 6365 6c6c              cell
-00003e30: 2066 6f72 2066 6333 2c20 6275 7420 7468   for fc3, but th
-00003e40: 6973 2069 7320 6372 6561 7465 6420 6672  is is created fr
-00003e50: 6f6d 2073 7570 6572 6365 6c6c 2066 6f72  om supercell for
-00003e60: 2066 6332 2061 6e64 0a20 2020 2020 2020   fc2 and.       
-00003e70: 2020 2020 2063 616e 2062 6520 6e6f 7420       can be not 
-00003e80: 6e75 6d65 7269 6361 6c6c 7920 7065 7266  numerically perf
-00003e90: 6563 746c 7920 6964 656e 7469 6361 6c2e  ectly identical.
-00003ea0: 0a0a 2020 2020 2020 2020 2222 220a 2020  ..        """.  
-00003eb0: 2020 2020 2020 7265 7475 726e 2073 656c        return sel
-00003ec0: 662e 5f70 686f 6e6f 6e5f 7072 696d 6974  f._phonon_primit
-00003ed0: 6976 650a 0a20 2020 2040 7072 6f70 6572  ive..    @proper
-00003ee0: 7479 0a20 2020 2064 6566 2073 796d 6d65  ty.    def symme
-00003ef0: 7472 7928 7365 6c66 2920 2d3e 2053 796d  try(self) -> Sym
-00003f00: 6d65 7472 793a 0a20 2020 2020 2020 2022  metry:.        "
-00003f10: 2222 5265 7475 726e 2073 796d 6d65 7472  ""Return symmetr
-00003f20: 7920 6f66 2073 7570 6572 6365 6c6c 2e0a  y of supercell..
-00003f30: 0a20 2020 2020 2020 2053 796d 6d65 7472  .        Symmetr
-00003f40: 790a 2020 2020 2020 2020 2020 2020 5379  y.            Sy
-00003f50: 6d6d 6574 7279 206f 6620 7375 7065 7263  mmetry of superc
-00003f60: 656c 6c0a 0a20 2020 2020 2020 2022 2222  ell..        """
-00003f70: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
-00003f80: 7365 6c66 2e5f 7379 6d6d 6574 7279 0a0a  self._symmetry..
-00003f90: 2020 2020 4070 726f 7065 7274 790a 2020      @property.  
-00003fa0: 2020 6465 6620 7072 696d 6974 6976 655f    def primitive_
-00003fb0: 7379 6d6d 6574 7279 2873 656c 6629 202d  symmetry(self) -
-00003fc0: 3e20 5379 6d6d 6574 7279 3a0a 2020 2020  > Symmetry:.    
-00003fd0: 2020 2020 2222 2252 6574 7572 6e20 7379      """Return sy
-00003fe0: 6d6d 6574 7279 206f 6620 7072 696d 6974  mmetry of primit
-00003ff0: 6976 6520 6365 6c6c 2e0a 0a20 2020 2020  ive cell...     
-00004000: 2020 2053 796d 6d65 7472 790a 2020 2020     Symmetry.    
+00000640: 4820 4441 4d41 4745 2e0a 0a69 6d70 6f72  H DAMAGE...impor
+00000650: 7420 636f 7079 0a66 726f 6d20 636f 6c6c  t copy.from coll
+00000660: 6563 7469 6f6e 732e 6162 6320 696d 706f  ections.abc impo
+00000670: 7274 2053 6571 7565 6e63 650a 6672 6f6d  rt Sequence.from
+00000680: 2074 7970 696e 6720 696d 706f 7274 204c   typing import L
+00000690: 6974 6572 616c 2c20 4f70 7469 6f6e 616c  iteral, Optional
+000006a0: 2c20 556e 696f 6e0a 0a69 6d70 6f72 7420  , Union..import 
+000006b0: 6e75 6d70 7920 6173 206e 700a 6672 6f6d  numpy as np.from
+000006c0: 2070 686f 6e6f 7079 2e65 7863 6570 7469   phonopy.excepti
+000006d0: 6f6e 2069 6d70 6f72 7420 466f 7263 6543  on import ForceC
+000006e0: 616c 6375 6c61 746f 7252 6571 7569 7265  alculatorRequire
+000006f0: 6445 7272 6f72 0a66 726f 6d20 7068 6f6e  dError.from phon
+00000700: 6f70 792e 6861 726d 6f6e 6963 2e64 6973  opy.harmonic.dis
+00000710: 706c 6163 656d 656e 7420 696d 706f 7274  placement import
+00000720: 2028 0a20 2020 2064 6972 6563 7469 6f6e   (.    direction
+00000730: 735f 746f 5f64 6973 706c 6163 656d 656e  s_to_displacemen
+00000740: 745f 6461 7461 7365 742c 0a20 2020 2067  t_dataset,.    g
+00000750: 6574 5f6c 6561 7374 5f64 6973 706c 6163  et_least_displac
+00000760: 656d 656e 7473 2c0a 290a 6672 6f6d 2070  ements,.).from p
+00000770: 686f 6e6f 7079 2e68 6172 6d6f 6e69 632e  honopy.harmonic.
+00000780: 666f 7263 655f 636f 6e73 7461 6e74 7320  force_constants 
+00000790: 696d 706f 7274 2067 6574 5f66 6332 2061  import get_fc2 a
+000007a0: 7320 6765 745f 7068 6f6e 6f70 795f 6663  s get_phonopy_fc
+000007b0: 320a 6672 6f6d 2070 686f 6e6f 7079 2e68  2.from phonopy.h
+000007c0: 6172 6d6f 6e69 632e 666f 7263 655f 636f  armonic.force_co
+000007d0: 6e73 7461 6e74 7320 696d 706f 7274 2028  nstants import (
+000007e0: 0a20 2020 2073 6574 5f70 6572 6d75 7461  .    set_permuta
+000007f0: 7469 6f6e 5f73 796d 6d65 7472 792c 0a20  tion_symmetry,. 
+00000800: 2020 2073 6574 5f74 7261 6e73 6c61 7469     set_translati
+00000810: 6f6e 616c 5f69 6e76 6172 6961 6e63 652c  onal_invariance,
+00000820: 0a20 2020 2073 796d 6d65 7472 697a 655f  .    symmetrize_
+00000830: 636f 6d70 6163 745f 666f 7263 655f 636f  compact_force_co
+00000840: 6e73 7461 6e74 732c 0a20 2020 2073 796d  nstants,.    sym
+00000850: 6d65 7472 697a 655f 666f 7263 655f 636f  metrize_force_co
+00000860: 6e73 7461 6e74 732c 0a29 0a66 726f 6d20  nstants,.).from 
+00000870: 7068 6f6e 6f70 792e 696e 7465 7266 6163  phonopy.interfac
+00000880: 652e 6663 5f63 616c 6375 6c61 746f 7220  e.fc_calculator 
+00000890: 696d 706f 7274 2067 6574 5f66 6332 0a66  import get_fc2.f
+000008a0: 726f 6d20 7068 6f6e 6f70 792e 7374 7275  rom phonopy.stru
+000008b0: 6374 7572 652e 6174 6f6d 7320 696d 706f  cture.atoms impo
+000008c0: 7274 2050 686f 6e6f 7079 4174 6f6d 730a  rt PhonopyAtoms.
+000008d0: 6672 6f6d 2070 686f 6e6f 7079 2e73 7472  from phonopy.str
+000008e0: 7563 7475 7265 2e63 656c 6c73 2069 6d70  ucture.cells imp
+000008f0: 6f72 7420 280a 2020 2020 5072 696d 6974  ort (.    Primit
+00000900: 6976 652c 0a20 2020 2053 7570 6572 6365  ive,.    Superce
+00000910: 6c6c 2c0a 2020 2020 6765 745f 7072 696d  ll,.    get_prim
+00000920: 6974 6976 652c 0a20 2020 2067 6574 5f70  itive,.    get_p
+00000930: 7269 6d69 7469 7665 5f6d 6174 7269 782c  rimitive_matrix,
+00000940: 0a20 2020 2067 6574 5f73 7570 6572 6365  .    get_superce
+00000950: 6c6c 2c0a 2020 2020 6775 6573 735f 7072  ll,.    guess_pr
+00000960: 696d 6974 6976 655f 6d61 7472 6978 2c0a  imitive_matrix,.
+00000970: 2020 2020 7368 6170 655f 7375 7065 7263      shape_superc
+00000980: 656c 6c5f 6d61 7472 6978 2c0a 290a 6672  ell_matrix,.).fr
+00000990: 6f6d 2070 686f 6e6f 7079 2e73 7472 7563  om phonopy.struc
+000009a0: 7475 7265 2e64 6174 6173 6574 2069 6d70  ture.dataset imp
+000009b0: 6f72 7420 6765 745f 6469 7370 6c61 6365  ort get_displace
+000009c0: 6d65 6e74 735f 616e 645f 666f 7263 6573  ments_and_forces
+000009d0: 0a66 726f 6d20 7068 6f6e 6f70 792e 7374  .from phonopy.st
+000009e0: 7275 6374 7572 652e 7379 6d6d 6574 7279  ructure.symmetry
+000009f0: 2069 6d70 6f72 7420 5379 6d6d 6574 7279   import Symmetry
+00000a00: 0a66 726f 6d20 7068 6f6e 6f70 792e 756e  .from phonopy.un
+00000a10: 6974 7320 696d 706f 7274 2056 6173 7054  its import VaspT
+00000a20: 6f54 487a 0a0a 6672 6f6d 2070 686f 6e6f  oTHz..from phono
+00000a30: 3370 792e 636f 6e64 7563 7469 7669 7479  3py.conductivity
+00000a40: 2e64 6972 6563 745f 736f 6c75 7469 6f6e  .direct_solution
+00000a50: 2069 6d70 6f72 7420 6765 745f 7468 6572   import get_ther
+00000a60: 6d61 6c5f 636f 6e64 7563 7469 7669 7479  mal_conductivity
+00000a70: 5f4c 4254 450a 6672 6f6d 2070 686f 6e6f  _LBTE.from phono
+00000a80: 3370 792e 636f 6e64 7563 7469 7669 7479  3py.conductivity
+00000a90: 2e72 7461 2069 6d70 6f72 7420 6765 745f  .rta import get_
+00000aa0: 7468 6572 6d61 6c5f 636f 6e64 7563 7469  thermal_conducti
+00000ab0: 7669 7479 5f52 5441 0a66 726f 6d20 7068  vity_RTA.from ph
+00000ac0: 6f6e 6f33 7079 2e69 6e74 6572 6661 6365  ono3py.interface
+00000ad0: 2e66 635f 6361 6c63 756c 6174 6f72 2069  .fc_calculator i
+00000ae0: 6d70 6f72 7420 6765 745f 6663 330a 6672  mport get_fc3.fr
+00000af0: 6f6d 2070 686f 6e6f 3370 792e 696e 7465  om phono3py.inte
+00000b00: 7266 6163 652e 7068 6f6e 6f33 7079 5f79  rface.phono3py_y
+00000b10: 616d 6c20 696d 706f 7274 2050 686f 6e6f  aml import Phono
+00000b20: 3370 7959 616d 6c0a 6672 6f6d 2070 686f  3pyYaml.from pho
+00000b30: 6e6f 3370 792e 7068 6f6e 6f6e 332e 6461  no3py.phonon3.da
+00000b40: 7461 7365 7420 696d 706f 7274 2067 6574  taset import get
+00000b50: 5f64 6973 706c 6163 656d 656e 7473 5f61  _displacements_a
+00000b60: 6e64 5f66 6f72 6365 735f 6663 330a 6672  nd_forces_fc3.fr
+00000b70: 6f6d 2070 686f 6e6f 3370 792e 7068 6f6e  om phono3py.phon
+00000b80: 6f6e 332e 6469 7370 6c61 6365 6d65 6e74  on3.displacement
+00000b90: 5f66 6333 2069 6d70 6f72 7420 280a 2020  _fc3 import (.  
+00000ba0: 2020 6469 7265 6374 696f 6e5f 746f 5f64    direction_to_d
+00000bb0: 6973 706c 6163 656d 656e 742c 0a20 2020  isplacement,.   
+00000bc0: 2067 6574 5f74 6869 7264 5f6f 7264 6572   get_third_order
+00000bd0: 5f64 6973 706c 6163 656d 656e 7473 2c0a  _displacements,.
+00000be0: 290a 6672 6f6d 2070 686f 6e6f 3370 792e  ).from phono3py.
+00000bf0: 7068 6f6e 6f6e 332e 6663 3320 696d 706f  phonon3.fc3 impo
+00000c00: 7274 2063 7574 6f66 665f 6663 335f 6279  rt cutoff_fc3_by
+00000c10: 5f7a 6572 6f0a 6672 6f6d 2070 686f 6e6f  _zero.from phono
+00000c20: 3370 792e 7068 6f6e 6f6e 332e 6663 3320  3py.phonon3.fc3 
+00000c30: 696d 706f 7274 2067 6574 5f66 6333 2061  import get_fc3 a
+00000c40: 7320 6765 745f 7068 6f6e 6f33 7079 5f66  s get_phono3py_f
+00000c50: 6333 0a66 726f 6d20 7068 6f6e 6f33 7079  c3.from phono3py
+00000c60: 2e70 686f 6e6f 6e33 2e66 6333 2069 6d70  .phonon3.fc3 imp
+00000c70: 6f72 7420 280a 2020 2020 7365 745f 7065  ort (.    set_pe
+00000c80: 726d 7574 6174 696f 6e5f 7379 6d6d 6574  rmutation_symmet
+00000c90: 7279 5f63 6f6d 7061 6374 5f66 6333 2c0a  ry_compact_fc3,.
+00000ca0: 2020 2020 7365 745f 7065 726d 7574 6174      set_permutat
+00000cb0: 696f 6e5f 7379 6d6d 6574 7279 5f66 6333  ion_symmetry_fc3
+00000cc0: 2c0a 2020 2020 7365 745f 7472 616e 736c  ,.    set_transl
+00000cd0: 6174 696f 6e61 6c5f 696e 7661 7269 616e  ational_invarian
+00000ce0: 6365 5f63 6f6d 7061 6374 5f66 6333 2c0a  ce_compact_fc3,.
+00000cf0: 2020 2020 7365 745f 7472 616e 736c 6174      set_translat
+00000d00: 696f 6e61 6c5f 696e 7661 7269 616e 6365  ional_invariance
+00000d10: 5f66 6333 2c0a 290a 6672 6f6d 2070 686f  _fc3,.).from pho
+00000d20: 6e6f 3370 792e 7068 6f6e 6f6e 332e 696d  no3py.phonon3.im
+00000d30: 6167 5f73 656c 665f 656e 6572 6779 2069  ag_self_energy i
+00000d40: 6d70 6f72 7420 280a 2020 2020 6765 745f  mport (.    get_
+00000d50: 696d 6167 5f73 656c 665f 656e 6572 6779  imag_self_energy
+00000d60: 2c0a 2020 2020 7772 6974 655f 696d 6167  ,.    write_imag
+00000d70: 5f73 656c 665f 656e 6572 6779 2c0a 290a  _self_energy,.).
+00000d80: 6672 6f6d 2070 686f 6e6f 3370 792e 7068  from phono3py.ph
+00000d90: 6f6e 6f6e 332e 696e 7465 7261 6374 696f  onon3.interactio
+00000da0: 6e20 696d 706f 7274 2049 6e74 6572 6163  n import Interac
+00000db0: 7469 6f6e 0a66 726f 6d20 7068 6f6e 6f33  tion.from phono3
+00000dc0: 7079 2e70 686f 6e6f 6e33 2e72 6561 6c5f  py.phonon3.real_
+00000dd0: 7365 6c66 5f65 6e65 7267 7920 696d 706f  self_energy impo
+00000de0: 7274 2028 0a20 2020 2067 6574 5f72 6561  rt (.    get_rea
+00000df0: 6c5f 7365 6c66 5f65 6e65 7267 792c 0a20  l_self_energy,. 
+00000e00: 2020 2077 7269 7465 5f72 6561 6c5f 7365     write_real_se
+00000e10: 6c66 5f65 6e65 7267 792c 0a29 0a66 726f  lf_energy,.).fro
+00000e20: 6d20 7068 6f6e 6f33 7079 2e70 686f 6e6f  m phono3py.phono
+00000e30: 6e33 2e73 7065 6374 7261 6c5f 6675 6e63  n3.spectral_func
+00000e40: 7469 6f6e 2069 6d70 6f72 7420 7275 6e5f  tion import run_
+00000e50: 7370 6563 7472 616c 5f66 756e 6374 696f  spectral_functio
+00000e60: 6e0a 6672 6f6d 2070 686f 6e6f 3370 792e  n.from phono3py.
+00000e70: 7068 6f6e 6f6e 2e67 7269 6420 696d 706f  phonon.grid impo
+00000e80: 7274 2042 5a47 7269 640a 6672 6f6d 2070  rt BZGrid.from p
+00000e90: 686f 6e6f 3370 792e 7665 7273 696f 6e20  hono3py.version 
+00000ea0: 696d 706f 7274 205f 5f76 6572 7369 6f6e  import __version
+00000eb0: 5f5f 0a0a 0a63 6c61 7373 2050 686f 6e6f  __...class Phono
+00000ec0: 3370 793a 0a20 2020 2022 2222 5068 6f6e  3py:.    """Phon
+00000ed0: 6f33 7079 206d 6169 6e20 636c 6173 732e  o3py main class.
+00000ee0: 0a0a 2020 2020 4174 7472 6962 7574 6573  ..    Attributes
+00000ef0: 0a20 2020 202d 2d2d 2d2d 2d2d 2d2d 2d0a  .    ----------.
+00000f00: 2020 2020 7665 7273 696f 6e0a 2020 2020      version.    
+00000f10: 6361 6c63 756c 6174 6f72 0a20 2020 2066  calculator.    f
+00000f20: 6333 203a 2067 6574 7465 7220 616e 6420  c3 : getter and 
+00000f30: 7365 7474 6572 0a20 2020 2066 6332 203a  setter.    fc2 :
+00000f40: 2067 6574 7465 7220 616e 6420 7365 7474   getter and sett
+00000f50: 6572 0a20 2020 2066 6f72 6365 5f63 6f6e  er.    force_con
+00000f60: 7374 616e 7473 0a20 2020 2073 6967 6d61  stants.    sigma
+00000f70: 203a 2067 6574 7465 7220 616e 6420 7365   : getter and se
+00000f80: 7474 6572 0a20 2020 2073 6967 6d61 5f63  tter.    sigma_c
+00000f90: 7574 6f66 6620 3a20 6765 7474 6572 2061  utoff : getter a
+00000fa0: 6e64 2073 6574 7465 720a 2020 2020 6e61  nd setter.    na
+00000fb0: 635f 7061 7261 6d73 203a 2067 6574 7465  c_params : gette
+00000fc0: 7220 616e 6420 7365 7474 6572 0a20 2020  r and setter.   
+00000fd0: 2064 796e 616d 6963 616c 5f6d 6174 7269   dynamical_matri
+00000fe0: 780a 2020 2020 7072 696d 6974 6976 650a  x.    primitive.
+00000ff0: 2020 2020 756e 6974 6365 6c6c 0a20 2020      unitcell.   
+00001000: 2073 7570 6572 6365 6c6c 0a20 2020 2070   supercell.    p
+00001010: 686f 6e6f 6e5f 7375 7065 7263 656c 6c0a  honon_supercell.
+00001020: 2020 2020 7068 6f6e 6f6e 5f70 7269 6d69      phonon_primi
+00001030: 7469 7665 0a20 2020 2073 796d 6d65 7472  tive.    symmetr
+00001040: 790a 2020 2020 7072 696d 6974 6976 655f  y.    primitive_
+00001050: 7379 6d6d 6574 7279 0a20 2020 2070 686f  symmetry.    pho
+00001060: 6e6f 6e5f 7375 7065 7263 656c 6c5f 7379  non_supercell_sy
+00001070: 6d6d 6574 7279 0a20 2020 2073 7570 6572  mmetry.    super
+00001080: 6365 6c6c 5f6d 6174 7269 780a 2020 2020  cell_matrix.    
+00001090: 7068 6f6e 6f6e 5f73 7570 6572 6365 6c6c  phonon_supercell
+000010a0: 5f6d 6174 7269 780a 2020 2020 7072 696d  _matrix.    prim
+000010b0: 6974 6976 655f 6d61 7472 6978 0a20 2020  itive_matrix.   
+000010c0: 2075 6e69 745f 636f 6e76 6572 7369 6f6e   unit_conversion
+000010d0: 5f66 6163 746f 720a 2020 2020 6461 7461  _factor.    data
+000010e0: 7365 7420 3a20 6765 7474 6572 2061 6e64  set : getter and
+000010f0: 2073 6574 7465 720a 2020 2020 7068 6f6e   setter.    phon
+00001100: 6f6e 5f64 6174 6173 6574 203a 2067 6574  on_dataset : get
+00001110: 7465 7220 616e 6420 7365 7474 6572 0a20  ter and setter. 
+00001120: 2020 2062 616e 645f 696e 6469 6365 7320     band_indices 
+00001130: 3a20 6765 7474 6572 2061 6e64 2073 6574  : getter and set
+00001140: 7465 720a 2020 2020 7068 6f6e 6f6e 5f73  ter.    phonon_s
+00001150: 7570 6572 6365 6c6c 735f 7769 7468 5f64  upercells_with_d
+00001160: 6973 706c 6163 656d 656e 7473 0a20 2020  isplacements.   
+00001170: 2073 7570 6572 6365 6c6c 735f 7769 7468   supercells_with
+00001180: 5f64 6973 706c 6163 656d 656e 7473 0a20  _displacements. 
+00001190: 2020 206d 6573 685f 6e75 6d62 6572 7320     mesh_numbers 
+000011a0: 3a20 6765 7474 6572 2061 6e64 2073 6574  : getter and set
+000011b0: 7465 720a 2020 2020 7468 6572 6d61 6c5f  ter.    thermal_
+000011c0: 636f 6e64 7563 7469 7669 7479 0a20 2020  conductivity.   
+000011d0: 2064 6973 706c 6163 656d 656e 7473 203a   displacements :
+000011e0: 2067 6574 7465 7220 616e 6420 7365 7474   getter and sett
+000011f0: 6572 0a20 2020 2066 6f72 6365 7320 3a20  er.    forces : 
+00001200: 6765 7474 6572 2061 6e64 2073 6574 7465  getter and sette
+00001210: 720a 2020 2020 7068 6f6e 6f6e 5f64 6973  r.    phonon_dis
+00001220: 706c 6163 656d 656e 7473 203a 2067 6574  placements : get
+00001230: 7465 7220 616e 6420 7365 7474 6572 0a20  ter and setter. 
+00001240: 2020 2070 686f 6e6f 6e5f 666f 7263 6573     phonon_forces
+00001250: 203a 2067 6574 7465 7220 616e 6420 7365   : getter and se
+00001260: 7474 6572 0a20 2020 2070 6870 685f 696e  tter.    phph_in
+00001270: 7465 7261 6374 696f 6e0a 0a20 2020 2022  teraction..    "
+00001280: 2222 0a0a 2020 2020 6465 6620 5f5f 696e  ""..    def __in
+00001290: 6974 5f5f 280a 2020 2020 2020 2020 7365  it__(.        se
+000012a0: 6c66 2c0a 2020 2020 2020 2020 756e 6974  lf,.        unit
+000012b0: 6365 6c6c 3a20 5068 6f6e 6f70 7941 746f  cell: PhonopyAto
+000012c0: 6d73 2c0a 2020 2020 2020 2020 7375 7065  ms,.        supe
+000012d0: 7263 656c 6c5f 6d61 7472 6978 3d4e 6f6e  rcell_matrix=Non
+000012e0: 652c 0a20 2020 2020 2020 2070 7269 6d69  e,.        primi
+000012f0: 7469 7665 5f6d 6174 7269 783d 4e6f 6e65  tive_matrix=None
+00001300: 2c0a 2020 2020 2020 2020 7068 6f6e 6f6e  ,.        phonon
+00001310: 5f73 7570 6572 6365 6c6c 5f6d 6174 7269  _supercell_matri
+00001320: 783d 4e6f 6e65 2c0a 2020 2020 2020 2020  x=None,.        
+00001330: 6375 746f 6666 5f66 7265 7175 656e 6379  cutoff_frequency
+00001340: 3d31 652d 342c 0a20 2020 2020 2020 2066  =1e-4,.        f
+00001350: 7265 7175 656e 6379 5f66 6163 746f 725f  requency_factor_
+00001360: 746f 5f54 487a 3d56 6173 7054 6f54 487a  to_THz=VaspToTHz
+00001370: 2c0a 2020 2020 2020 2020 6973 5f73 796d  ,.        is_sym
+00001380: 6d65 7472 793d 5472 7565 2c0a 2020 2020  metry=True,.    
+00001390: 2020 2020 6973 5f6d 6573 685f 7379 6d6d      is_mesh_symm
+000013a0: 6574 7279 3d54 7275 652c 0a20 2020 2020  etry=True,.     
+000013b0: 2020 2075 7365 5f67 7267 3d46 616c 7365     use_grg=False
+000013c0: 2c0a 2020 2020 2020 2020 534e 465f 636f  ,.        SNF_co
+000013d0: 6f72 6469 6e61 7465 733d 2272 6563 6970  ordinates="recip
+000013e0: 726f 6361 6c22 2c0a 2020 2020 2020 2020  rocal",.        
+000013f0: 6d61 6b65 5f72 305f 6176 6572 6167 653a  make_r0_average:
+00001400: 2062 6f6f 6c20 3d20 5472 7565 2c0a 2020   bool = True,.  
+00001410: 2020 2020 2020 7379 6d70 7265 633d 3165        symprec=1e
+00001420: 2d35 2c0a 2020 2020 2020 2020 6361 6c63  -5,.        calc
+00001430: 756c 6174 6f72 3a20 4f70 7469 6f6e 616c  ulator: Optional
+00001440: 5b73 7472 5d20 3d20 4e6f 6e65 2c0a 2020  [str] = None,.  
+00001450: 2020 2020 2020 6c6f 675f 6c65 7665 6c3d        log_level=
+00001460: 302c 0a20 2020 2029 3a0a 2020 2020 2020  0,.    ):.      
+00001470: 2020 2222 2249 6e69 7420 6d65 7468 6f64    """Init method
+00001480: 2e0a 0a20 2020 2020 2020 2050 6172 616d  ...        Param
+00001490: 6574 6572 730a 2020 2020 2020 2020 2d2d  eters.        --
+000014a0: 2d2d 2d2d 2d2d 2d2d 0a20 2020 2020 2020  --------.       
+000014b0: 2075 6e69 7463 656c 6c20 3a20 5068 6f6e   unitcell : Phon
+000014c0: 6f70 7941 746f 6d73 2c20 6f70 7469 6f6e  opyAtoms, option
+000014d0: 616c 0a20 2020 2020 2020 2020 2020 2049  al.            I
+000014e0: 6e70 7574 2075 6e69 7420 6365 6c6c 2e0a  nput unit cell..
+000014f0: 2020 2020 2020 2020 7375 7065 7263 656c          supercel
+00001500: 6c5f 6d61 7472 6978 203a 2061 7272 6179  l_matrix : array
+00001510: 5f6c 696b 652c 206f 7074 696f 6e61 6c0a  _like, optional.
+00001520: 2020 2020 2020 2020 2020 2020 5375 7065              Supe
+00001530: 7263 656c 6c20 6d61 7472 6978 206d 756c  rcell matrix mul
+00001540: 7469 706c 6965 6420 746f 2069 6e70 7574  tiplied to input
+00001550: 2063 656c 6c20 6261 7369 7320 7665 6374   cell basis vect
+00001560: 6f72 732e 2073 6861 7065 3d28 332c 2029  ors. shape=(3, )
+00001570: 0a20 2020 2020 2020 2020 2020 206f 7220  .            or 
+00001580: 2833 2c20 3329 2c20 7768 6572 6520 7468  (3, 3), where th
+00001590: 6520 666f 726d 6572 2069 7320 636f 6e73  e former is cons
+000015a0: 6964 6572 6564 2061 2064 6961 676f 6e61  idered a diagona
+000015b0: 6c20 6d61 7472 6978 2e20 5468 650a 2020  l matrix. The.  
+000015c0: 2020 2020 2020 2020 2020 656c 656d 656e            elemen
+000015d0: 7473 2068 6176 6520 746f 2062 6520 6769  ts have to be gi
+000015e0: 7665 6e20 6279 2069 6e74 6567 6572 732e  ven by integers.
+000015f0: 2041 6c74 686f 7567 6820 7468 6520 6465   Although the de
+00001600: 6661 756c 7420 6973 204e 6f6e 652c 0a20  fault is None,. 
+00001610: 2020 2020 2020 2020 2020 2077 6869 6368             which
+00001620: 2072 6573 756c 7473 2069 6e20 6964 656e   results in iden
+00001630: 7469 7479 206d 6174 7269 782c 2069 7420  tity matrix, it 
+00001640: 6973 2072 6563 6f6d 6d65 6e64 6564 2074  is recommended t
+00001650: 6f20 6769 7665 0a20 2020 2020 2020 2020  o give.         
+00001660: 2020 2060 7375 7065 7263 656c 6c5f 6d61     `supercell_ma
+00001670: 7472 6978 6020 6578 706c 6963 6974 6c79  trix` explicitly
+00001680: 2e0a 2020 2020 2020 2020 7072 696d 6974  ..        primit
+00001690: 6976 655f 6d61 7472 6978 203a 2061 7272  ive_matrix : arr
+000016a0: 6179 5f6c 696b 6520 6f72 2073 7472 2c20  ay_like or str, 
+000016b0: 6f70 7469 6f6e 616c 0a20 2020 2020 2020  optional.       
+000016c0: 2020 2020 2050 7269 6d69 7469 7665 206d       Primitive m
+000016d0: 6174 7269 7820 6d75 6c74 6970 6c69 6564  atrix multiplied
+000016e0: 2074 6f20 696e 7075 7420 6365 6c6c 2062   to input cell b
+000016f0: 6173 6973 2076 6563 746f 7273 2e20 4465  asis vectors. De
+00001700: 6661 756c 7420 6973 0a20 2020 2020 2020  fault is.       
+00001710: 2020 2020 2074 6865 2069 6465 6e74 6974       the identit
+00001720: 7920 6d61 7472 6978 2e20 5768 656e 2067  y matrix. When g
+00001730: 6976 656e 2061 7320 6172 7261 795f 6c69  iven as array_li
+00001740: 6b65 2c20 7368 6170 653d 2833 2c20 3329  ke, shape=(3, 3)
+00001750: 2c0a 2020 2020 2020 2020 2020 2020 6474  ,.            dt
+00001760: 7970 653d 666c 6f61 742e 2057 6865 6e20  ype=float. When 
+00001770: 2746 272c 2027 4927 2c20 2741 272c 2027  'F', 'I', 'A', '
+00001780: 4327 2c20 6f72 2027 5227 2069 7320 6769  C', or 'R' is gi
+00001790: 7665 6e20 696e 7374 6561 6420 6f66 2061  ven instead of a
+000017a0: 0a20 2020 2020 2020 2020 2020 2033 7833  .            3x3
+000017b0: 206d 6174 7269 782c 2074 6865 2070 7269   matrix, the pri
+000017c0: 6d69 7469 7665 206d 6174 7269 7820 6465  mitive matrix de
+000017d0: 6669 6e65 6420 6174 0a20 2020 2020 2020  fined at.       
+000017e0: 2020 2020 2068 7474 7073 3a2f 2f73 7067       https://spg
+000017f0: 6c69 622e 6769 7468 7562 2e69 6f2f 7370  lib.github.io/sp
+00001800: 676c 6962 2f64 6566 696e 6974 696f 6e2e  glib/definition.
+00001810: 6874 6d6c 2069 7320 7573 6564 2e20 5768  html is used. Wh
+00001820: 656e 2027 6175 746f 270a 2020 2020 2020  en 'auto'.      
+00001830: 2020 2020 2020 6973 2067 6976 656e 2c20        is given, 
+00001840: 7468 6520 6365 6e74 7269 6e67 2074 7970  the centring typ
+00001850: 6520 2827 4627 2c20 2749 272c 2027 4127  e ('F', 'I', 'A'
+00001860: 2c20 2743 272c 2027 5227 2c20 6f72 2070  , 'C', 'R', or p
+00001870: 7269 6d69 7469 7665 0a20 2020 2020 2020  rimitive.       
+00001880: 2020 2020 2027 5027 2920 6973 2061 7574       'P') is aut
+00001890: 6f6d 6174 6963 616c 6c79 2063 686f 7365  omatically chose
+000018a0: 6e2e 0a20 2020 2020 2020 2070 686f 6e6f  n..        phono
+000018b0: 6e5f 7375 7065 7263 656c 6c5f 6d61 7472  n_supercell_matr
+000018c0: 6978 203a 2061 7272 6179 5f6c 696b 652c  ix : array_like,
+000018d0: 206f 7074 696f 6e61 6c0a 2020 2020 2020   optional.      
+000018e0: 2020 2020 2020 5375 7065 7263 656c 6c20        Supercell 
+000018f0: 6d61 7472 6978 2075 7365 6420 666f 7220  matrix used for 
+00001900: 6663 322e 2049 6e20 7068 6f6e 6f33 7079  fc2. In phono3py
+00001910: 2c20 7375 7065 7263 656c 6c20 6d61 7472  , supercell matr
+00001920: 6978 2066 6f72 2066 6333 0a20 2020 2020  ix for fc3.     
+00001930: 2020 2020 2020 2061 6e64 2066 6332 2063         and fc2 c
+00001940: 616e 2062 6520 6469 6666 6572 656e 7420  an be different 
+00001950: 746f 2073 7570 706f 7274 206c 6f6e 6765  to support longe
+00001960: 7220 7261 6e67 6520 696e 7465 7261 6374  r range interact
+00001970: 696f 6e20 6f66 2066 6332 0a20 2020 2020  ion of fc2.     
+00001980: 2020 2020 2020 2074 6861 6e20 7468 6174         than that
+00001990: 206f 6620 6663 332e 2055 6e6c 6573 7320   of fc3. Unless 
+000019a0: 7365 7474 696e 6720 7468 6973 2c20 7375  setting this, su
+000019b0: 7065 7263 656c 6c5f 6d61 7472 6978 2069  percell_matrix i
+000019c0: 7320 7573 6564 2e0a 2020 2020 2020 2020  s used..        
+000019d0: 2020 2020 5468 6973 2069 7320 6f6e 6c79      This is only
+000019e0: 2076 616c 6964 6520 7768 656e 2075 6e69   valide when uni
+000019f0: 7463 656c 6c20 6f72 2075 6e69 7463 656c  tcell or unitcel
+00001a00: 6c5f 6669 6c65 6e61 6d65 2069 7320 6769  l_filename is gi
+00001a10: 7665 6e2e 0a20 2020 2020 2020 2020 2020  ven..           
+00001a20: 2044 6566 6175 6c74 2069 7320 4e6f 6e65   Default is None
+00001a30: 2e0a 2020 2020 2020 2020 6375 746f 6666  ..        cutoff
+00001a40: 5f66 7265 7175 656e 6379 203a 2066 6c6f  _frequency : flo
+00001a50: 6174 2c20 6f70 7469 6f6e 616c 0a20 2020  at, optional.   
+00001a60: 2020 2020 2020 2020 2050 686f 6e6f 6e20           Phonon 
+00001a70: 6672 6571 7565 6e63 7920 6265 6c6f 7720  frequency below 
+00001a80: 7468 6973 2076 616c 7565 2069 7320 6967  this value is ig
+00001a90: 6e6f 7265 6420 7768 656e 2074 6865 2063  nored when the c
+00001aa0: 7574 6f66 6620 6973 0a20 2020 2020 2020  utoff is.       
+00001ab0: 2020 2020 206e 6565 6465 6420 666f 7220       needed for 
+00001ac0: 7468 6520 636f 6d70 7574 6174 696f 6e2e  the computation.
+00001ad0: 2044 6566 6175 6c74 2069 7320 3165 2d34   Default is 1e-4
+00001ae0: 2e0a 2020 2020 2020 2020 6672 6571 7565  ..        freque
+00001af0: 6e63 795f 6661 6374 6f72 5f74 6f5f 5448  ncy_factor_to_TH
+00001b00: 7a20 3a20 666c 6f61 742c 206f 7074 696f  z : float, optio
+00001b10: 6e61 6c0a 2020 2020 2020 2020 2020 2020  nal.            
+00001b20: 5068 6f6e 6f6e 2066 7265 7175 656e 6379  Phonon frequency
+00001b30: 2075 6e69 7420 636f 6e76 6572 7369 6f6e   unit conversion
+00001b40: 2066 6163 746f 722e 2055 6e6c 6573 7320   factor. Unless 
+00001b50: 7370 6563 6966 6965 642c 2064 6566 6175  specified, defau
+00001b60: 6c74 0a20 2020 2020 2020 2020 2020 2075  lt.            u
+00001b70: 6e69 7420 636f 6e76 6572 7369 6f6e 2066  nit conversion f
+00001b80: 6163 746f 7220 666f 7220 6561 6368 2063  actor for each c
+00001b90: 616c 6375 6c61 746f 7220 6973 2075 7365  alculator is use
+00001ba0: 642e 0a20 2020 2020 2020 2069 735f 7379  d..        is_sy
+00001bb0: 6d6d 6574 7279 203a 2062 6f6f 6c2c 206f  mmetry : bool, o
+00001bc0: 7074 696f 6e61 6c0a 2020 2020 2020 2020  ptional.        
+00001bd0: 2020 2020 5573 6520 6372 7973 7461 6c20      Use crystal 
+00001be0: 7379 6d6d 6574 7279 2069 6e20 6d6f 7374  symmetry in most
+00001bf0: 2063 616c 6375 6c61 7469 6f6e 7320 7768   calculations wh
+00001c00: 656e 2054 7275 652e 2044 6566 6175 6c74  en True. Default
+00001c10: 2069 730a 2020 2020 2020 2020 2020 2020   is.            
+00001c20: 5472 7565 2e0a 2020 2020 2020 2020 6973  True..        is
+00001c30: 5f6d 6573 685f 7379 6d6d 6574 7279 203a  _mesh_symmetry :
+00001c40: 2062 6f6f 6c2c 206f 7074 696f 6e61 6c0a   bool, optional.
+00001c50: 2020 2020 2020 2020 2020 2020 5573 6520              Use 
+00001c60: 6372 7973 7461 6c20 7379 6d6d 6574 7279  crystal symmetry
+00001c70: 2069 6e20 7265 6369 7072 6f63 616c 2073   in reciprocal s
+00001c80: 7061 6365 2067 7269 6420 6861 6e64 6c69  pace grid handli
+00001c90: 6e67 2077 6865 6e20 5472 7565 2e0a 2020  ng when True..  
+00001ca0: 2020 2020 2020 2020 2020 4465 6661 756c            Defaul
+00001cb0: 7420 6973 2054 7275 652e 0a20 2020 2020  t is True..     
+00001cc0: 2020 2075 7365 5f67 7267 203a 2062 6f6f     use_grg : boo
+00001cd0: 6c2c 206f 7074 696f 6e61 6c0a 2020 2020  l, optional.    
+00001ce0: 2020 2020 2020 2020 5573 6520 6765 6e65          Use gene
+00001cf0: 7261 6c69 7a65 6420 7265 6775 6c61 7220  ralized regular 
+00001d00: 6772 6964 2077 6865 6e20 5472 7565 2e20  grid when True. 
+00001d10: 4465 6661 756c 7420 6973 2046 616c 7365  Default is False
+00001d20: 2e0a 2020 2020 2020 2020 534e 465f 636f  ..        SNF_co
+00001d30: 6f72 6469 6e61 7465 7320 3a20 7374 722c  ordinates : str,
+00001d40: 206f 7074 696f 6e61 6c0a 2020 2020 2020   optional.      
+00001d50: 2020 2020 2020 6072 6563 6970 726f 6361        `reciproca
+00001d60: 6c60 206f 7220 6064 6972 6563 7460 2e20  l` or `direct`. 
+00001d70: 5370 6163 6520 6f66 2063 6f6f 7264 696e  Space of coordin
+00001d80: 6174 6573 2074 6f20 6765 6e65 7261 7465  ates to generate
+00001d90: 2067 7269 640a 2020 2020 2020 2020 2020   grid.          
+00001da0: 2020 6765 6e65 7261 7469 6e67 206d 6174    generating mat
+00001db0: 7269 7820 6569 7468 6572 2069 6e20 6469  rix either in di
+00001dc0: 7265 6374 206f 7220 7265 6369 7072 6f63  rect or reciproc
+00001dd0: 616c 2073 7061 6365 2e20 5468 6520 6465  al space. The de
+00001de0: 6661 756c 740a 2020 2020 2020 2020 2020  fault.          
+00001df0: 2020 6973 2060 7265 6369 7072 6f63 616c    is `reciprocal
+00001e00: 602e 0a20 2020 2020 2020 206d 616b 655f  `..        make_
+00001e10: 7230 5f61 7665 7261 6765 203a 2062 6f6f  r0_average : boo
+00001e20: 6c2c 206f 7074 696f 6e61 6c0a 2020 2020  l, optional.    
+00001e30: 2020 2020 2020 2020 6663 3320 7472 616e          fc3 tran
+00001e40: 7366 6f72 6d61 7469 6f6e 2066 726f 6d20  sformation from 
+00001e50: 7265 616c 2074 6f20 7265 6369 7072 6f63  real to reciproc
+00001e60: 616c 2073 7061 6365 2069 7320 646f 6e65  al space is done
+00001e70: 0a20 2020 2020 2020 2020 2020 2061 726f  .            aro
+00001e80: 756e 6420 7468 7265 6520 6174 6f6d 7320  und three atoms 
+00001e90: 616e 6420 6176 6572 6167 6564 2077 6865  and averaged whe
+00001ea0: 6e20 5472 7565 2e20 4465 6661 756c 7420  n True. Default 
+00001eb0: 6973 2046 616c 7365 2c20 692e 652e 2c0a  is False, i.e.,.
+00001ec0: 2020 2020 2020 2020 2020 2020 6f6e 6c79              only
+00001ed0: 2061 726f 756e 6420 7468 6520 6669 7273   around the firs
+00001ee0: 7420 6174 6f6d 2e20 5365 7474 696e 6720  t atom. Setting 
+00001ef0: 4661 6c73 6520 6973 2066 6f72 2072 6f75  False is for rou
+00001f00: 6768 2063 6f6d 7061 7469 6269 6c69 7479  gh compatibility
+00001f10: 0a20 2020 2020 2020 2020 2020 2077 6974  .            wit
+00001f20: 6820 7632 2e78 2e20 4465 6661 756c 7420  h v2.x. Default 
+00001f30: 6973 2054 7275 652e 0a20 2020 2020 2020  is True..       
+00001f40: 2073 796d 7072 6563 203a 2066 6c6f 6174   symprec : float
+00001f50: 2c20 6f70 7469 6f6e 616c 0a20 2020 2020  , optional.     
+00001f60: 2020 2020 2020 2054 6f6c 6572 616e 6365         Tolerance
+00001f70: 2075 7365 6420 746f 2066 696e 6420 6372   used to find cr
+00001f80: 7973 7461 6c20 7379 6d6d 6574 7279 2e20  ystal symmetry. 
+00001f90: 4465 6661 756c 7420 6973 2031 652d 352e  Default is 1e-5.
+00001fa0: 0a20 2020 2020 2020 2063 616c 6375 6c61  .        calcula
+00001fb0: 746f 7220 3a20 7374 722c 206f 7074 696f  tor : str, optio
+00001fc0: 6e61 6c2e 0a20 2020 2020 2020 2020 2020  nal..           
+00001fd0: 2043 616c 6375 6c61 746f 7220 7573 6564   Calculator used
+00001fe0: 2066 6f72 2063 6f6d 7075 7469 6e67 2066   for computing f
+00001ff0: 6f72 6365 732e 2054 6869 7320 6973 2075  orces. This is u
+00002000: 7365 6420 746f 2073 7769 7463 6820 7468  sed to switch th
+00002010: 6520 7365 740a 2020 2020 2020 2020 2020  e set.          
+00002020: 2020 6f66 2070 6879 7369 6361 6c20 756e    of physical un
+00002030: 6974 732e 2044 6566 6175 6c74 2069 7320  its. Default is 
+00002040: 4e6f 6e65 2c20 7768 6963 6820 6973 2065  None, which is e
+00002050: 7175 6976 616c 656e 7420 746f 2022 7661  quivalent to "va
+00002060: 7370 222e 0a20 2020 2020 2020 206c 6f67  sp"..        log
+00002070: 5f6c 6576 656c 203a 2069 6e74 2c20 6f70  _level : int, op
+00002080: 7469 6f6e 616c 0a20 2020 2020 2020 2020  tional.         
+00002090: 2020 2056 6572 626f 7369 7479 2063 6f6e     Verbosity con
+000020a0: 7472 6f6c 2e20 4465 6661 756c 7420 6973  trol. Default is
+000020b0: 2030 2e20 5468 6973 2063 616e 2062 6520   0. This can be 
+000020c0: 302c 2031 2c20 6f72 2032 2e0a 0a20 2020  0, 1, or 2...   
+000020d0: 2020 2020 2022 2222 0a20 2020 2020 2020       """.       
+000020e0: 2073 656c 662e 5f73 796d 7072 6563 203d   self._symprec =
+000020f0: 2073 796d 7072 6563 0a20 2020 2020 2020   symprec.       
+00002100: 2073 656c 662e 5f66 7265 7175 656e 6379   self._frequency
+00002110: 5f66 6163 746f 725f 746f 5f54 487a 203d  _factor_to_THz =
+00002120: 2066 7265 7175 656e 6379 5f66 6163 746f   frequency_facto
+00002130: 725f 746f 5f54 487a 0a20 2020 2020 2020  r_to_THz.       
+00002140: 2073 656c 662e 5f69 735f 7379 6d6d 6574   self._is_symmet
+00002150: 7279 203d 2069 735f 7379 6d6d 6574 7279  ry = is_symmetry
+00002160: 0a20 2020 2020 2020 2073 656c 662e 5f69  .        self._i
+00002170: 735f 6d65 7368 5f73 796d 6d65 7472 7920  s_mesh_symmetry 
+00002180: 3d20 6973 5f6d 6573 685f 7379 6d6d 6574  = is_mesh_symmet
+00002190: 7279 0a20 2020 2020 2020 2073 656c 662e  ry.        self.
+000021a0: 5f75 7365 5f67 7267 203d 2075 7365 5f67  _use_grg = use_g
+000021b0: 7267 0a20 2020 2020 2020 2073 656c 662e  rg.        self.
+000021c0: 5f53 4e46 5f63 6f6f 7264 696e 6174 6573  _SNF_coordinates
+000021d0: 203d 2053 4e46 5f63 6f6f 7264 696e 6174   = SNF_coordinat
+000021e0: 6573 0a0a 2020 2020 2020 2020 7365 6c66  es..        self
+000021f0: 2e5f 6d61 6b65 5f72 305f 6176 6572 6167  ._make_r0_averag
+00002200: 6520 3d20 6d61 6b65 5f72 305f 6176 6572  e = make_r0_aver
+00002210: 6167 650a 0a20 2020 2020 2020 2073 656c  age..        sel
+00002220: 662e 5f63 7574 6f66 665f 6672 6571 7565  f._cutoff_freque
+00002230: 6e63 7920 3d20 6375 746f 6666 5f66 7265  ncy = cutoff_fre
+00002240: 7175 656e 6379 0a20 2020 2020 2020 2073  quency.        s
+00002250: 656c 662e 5f63 616c 6375 6c61 746f 723a  elf._calculator:
+00002260: 204f 7074 696f 6e61 6c5b 7374 725d 203d   Optional[str] =
+00002270: 2063 616c 6375 6c61 746f 720a 2020 2020   calculator.    
+00002280: 2020 2020 7365 6c66 2e5f 6c6f 675f 6c65      self._log_le
+00002290: 7665 6c20 3d20 6c6f 675f 6c65 7665 6c0a  vel = log_level.
+000022a0: 0a20 2020 2020 2020 2023 2043 7265 6174  .        # Creat
+000022b0: 6520 7375 7065 7263 656c 6c20 616e 6420  e supercell and 
+000022c0: 7072 696d 6974 6976 6520 6365 6c6c 0a20  primitive cell. 
+000022d0: 2020 2020 2020 2073 656c 662e 5f75 6e69         self._uni
+000022e0: 7463 656c 6c20 3d20 756e 6974 6365 6c6c  tcell = unitcell
+000022f0: 0a20 2020 2020 2020 2073 656c 662e 5f73  .        self._s
+00002300: 7570 6572 6365 6c6c 5f6d 6174 7269 7820  upercell_matrix 
+00002310: 3d20 6e70 2e61 7272 6179 280a 2020 2020  = np.array(.    
+00002320: 2020 2020 2020 2020 7368 6170 655f 7375          shape_su
+00002330: 7065 7263 656c 6c5f 6d61 7472 6978 2873  percell_matrix(s
+00002340: 7570 6572 6365 6c6c 5f6d 6174 7269 7829  upercell_matrix)
+00002350: 2c20 6474 7970 653d 2269 6e74 5f22 2c20  , dtype="int_", 
+00002360: 6f72 6465 723d 2243 220a 2020 2020 2020  order="C".      
+00002370: 2020 290a 2020 2020 2020 2020 706d 6174    ).        pmat
+00002380: 203d 2073 656c 662e 5f64 6574 6572 6d69   = self._determi
+00002390: 6e65 5f70 7269 6d69 7469 7665 5f6d 6174  ne_primitive_mat
+000023a0: 7269 7828 7072 696d 6974 6976 655f 6d61  rix(primitive_ma
+000023b0: 7472 6978 290a 2020 2020 2020 2020 7365  trix).        se
+000023c0: 6c66 2e5f 7072 696d 6974 6976 655f 6d61  lf._primitive_ma
+000023d0: 7472 6978 203d 2070 6d61 740a 2020 2020  trix = pmat.    
+000023e0: 2020 2020 7365 6c66 2e5f 6e61 635f 7061      self._nac_pa
+000023f0: 7261 6d73 203d 204e 6f6e 650a 2020 2020  rams = None.    
+00002400: 2020 2020 6966 2070 686f 6e6f 6e5f 7375      if phonon_su
+00002410: 7065 7263 656c 6c5f 6d61 7472 6978 2069  percell_matrix i
+00002420: 7320 6e6f 7420 4e6f 6e65 3a0a 2020 2020  s not None:.    
+00002430: 2020 2020 2020 2020 7365 6c66 2e5f 7068          self._ph
+00002440: 6f6e 6f6e 5f73 7570 6572 6365 6c6c 5f6d  onon_supercell_m
+00002450: 6174 7269 7820 3d20 6e70 2e61 7272 6179  atrix = np.array
+00002460: 280a 2020 2020 2020 2020 2020 2020 2020  (.              
+00002470: 2020 7368 6170 655f 7375 7065 7263 656c    shape_supercel
+00002480: 6c5f 6d61 7472 6978 2870 686f 6e6f 6e5f  l_matrix(phonon_
+00002490: 7375 7065 7263 656c 6c5f 6d61 7472 6978  supercell_matrix
+000024a0: 292c 2064 7479 7065 3d22 696e 745f 222c  ), dtype="int_",
+000024b0: 206f 7264 6572 3d22 4322 0a20 2020 2020   order="C".     
+000024c0: 2020 2020 2020 2029 0a20 2020 2020 2020         ).       
+000024d0: 2065 6c73 653a 0a20 2020 2020 2020 2020   else:.         
+000024e0: 2020 2073 656c 662e 5f70 686f 6e6f 6e5f     self._phonon_
+000024f0: 7375 7065 7263 656c 6c5f 6d61 7472 6978  supercell_matrix
+00002500: 203d 204e 6f6e 650a 2020 2020 2020 2020   = None.        
+00002510: 7365 6c66 2e5f 7375 7065 7263 656c 6c20  self._supercell 
+00002520: 3d20 4e6f 6e65 0a20 2020 2020 2020 2073  = None.        s
+00002530: 656c 662e 5f70 7269 6d69 7469 7665 203d  elf._primitive =
+00002540: 204e 6f6e 650a 2020 2020 2020 2020 7365   None.        se
+00002550: 6c66 2e5f 7068 6f6e 6f6e 5f73 7570 6572  lf._phonon_super
+00002560: 6365 6c6c 203d 204e 6f6e 650a 2020 2020  cell = None.    
+00002570: 2020 2020 7365 6c66 2e5f 7068 6f6e 6f6e      self._phonon
+00002580: 5f70 7269 6d69 7469 7665 203d 204e 6f6e  _primitive = Non
+00002590: 650a 2020 2020 2020 2020 7365 6c66 2e5f  e.        self._
+000025a0: 6275 696c 645f 7375 7065 7263 656c 6c28  build_supercell(
+000025b0: 290a 2020 2020 2020 2020 7365 6c66 2e5f  ).        self._
+000025c0: 6275 696c 645f 7072 696d 6974 6976 655f  build_primitive_
+000025d0: 6365 6c6c 2829 0a20 2020 2020 2020 2073  cell().        s
+000025e0: 656c 662e 5f62 7569 6c64 5f70 686f 6e6f  elf._build_phono
+000025f0: 6e5f 7375 7065 7263 656c 6c28 290a 2020  n_supercell().  
+00002600: 2020 2020 2020 7365 6c66 2e5f 6275 696c        self._buil
+00002610: 645f 7068 6f6e 6f6e 5f70 7269 6d69 7469  d_phonon_primiti
+00002620: 7665 5f63 656c 6c28 290a 0a20 2020 2020  ve_cell()..     
+00002630: 2020 2073 656c 662e 5f73 6967 6d61 7320     self._sigmas 
+00002640: 3d20 5b0a 2020 2020 2020 2020 2020 2020  = [.            
+00002650: 4e6f 6e65 2c0a 2020 2020 2020 2020 5d0a  None,.        ].
+00002660: 2020 2020 2020 2020 7365 6c66 2e5f 7369          self._si
+00002670: 676d 615f 6375 746f 6666 203d 204e 6f6e  gma_cutoff = Non
+00002680: 650a 0a20 2020 2020 2020 2023 2047 7269  e..        # Gri
+00002690: 640a 2020 2020 2020 2020 7365 6c66 2e5f  d.        self._
+000026a0: 627a 5f67 7269 6420 3d20 4e6f 6e65 0a0a  bz_grid = None..
+000026b0: 2020 2020 2020 2020 2320 5365 7420 7375          # Set su
+000026c0: 7065 7263 656c 6c2c 2070 7269 6d69 7469  percell, primiti
+000026d0: 7665 2c20 616e 6420 7068 6f6e 6f6e 2073  ve, and phonon s
+000026e0: 7570 6572 6365 6c6c 2073 796d 6d65 7472  upercell symmetr
+000026f0: 6965 730a 2020 2020 2020 2020 7365 6c66  ies.        self
+00002700: 2e5f 7379 6d6d 6574 7279 203d 204e 6f6e  ._symmetry = Non
+00002710: 650a 2020 2020 2020 2020 7365 6c66 2e5f  e.        self._
+00002720: 7072 696d 6974 6976 655f 7379 6d6d 6574  primitive_symmet
+00002730: 7279 203d 204e 6f6e 650a 2020 2020 2020  ry = None.      
+00002740: 2020 7365 6c66 2e5f 7068 6f6e 6f6e 5f73    self._phonon_s
+00002750: 7570 6572 6365 6c6c 5f73 796d 6d65 7472  upercell_symmetr
+00002760: 7920 3d20 4e6f 6e65 0a20 2020 2020 2020  y = None.       
+00002770: 2073 656c 662e 5f73 6561 7263 685f 7379   self._search_sy
+00002780: 6d6d 6574 7279 2829 0a20 2020 2020 2020  mmetry().       
+00002790: 2073 656c 662e 5f73 6561 7263 685f 7072   self._search_pr
+000027a0: 696d 6974 6976 655f 7379 6d6d 6574 7279  imitive_symmetry
+000027b0: 2829 0a20 2020 2020 2020 2073 656c 662e  ().        self.
+000027c0: 5f73 6561 7263 685f 7068 6f6e 6f6e 5f73  _search_phonon_s
+000027d0: 7570 6572 6365 6c6c 5f73 796d 6d65 7472  upercell_symmetr
+000027e0: 7928 290a 0a20 2020 2020 2020 2023 2044  y()..        # D
+000027f0: 6973 706c 6163 656d 656e 7473 2061 6e64  isplacements and
+00002800: 2073 7570 6572 6365 6c6c 730a 2020 2020   supercells.    
+00002810: 2020 2020 7365 6c66 2e5f 7375 7065 7263      self._superc
+00002820: 656c 6c73 5f77 6974 685f 6469 7370 6c61  ells_with_displa
+00002830: 6365 6d65 6e74 7320 3d20 4e6f 6e65 0a20  cements = None. 
+00002840: 2020 2020 2020 2073 656c 662e 5f64 6174         self._dat
+00002850: 6173 6574 203d 204e 6f6e 650a 2020 2020  aset = None.    
+00002860: 2020 2020 7365 6c66 2e5f 7068 6f6e 6f6e      self._phonon
+00002870: 5f64 6174 6173 6574 203d 204e 6f6e 650a  _dataset = None.
+00002880: 2020 2020 2020 2020 7365 6c66 2e5f 7068          self._ph
+00002890: 6f6e 6f6e 5f73 7570 6572 6365 6c6c 735f  onon_supercells_
+000028a0: 7769 7468 5f64 6973 706c 6163 656d 656e  with_displacemen
+000028b0: 7473 203d 204e 6f6e 650a 0a20 2020 2020  ts = None..     
+000028c0: 2020 2023 2054 6865 726d 616c 2063 6f6e     # Thermal con
+000028d0: 6475 6374 6976 6974 790a 2020 2020 2020  ductivity.      
+000028e0: 2020 2320 636f 6e64 7563 7469 7669 7479    # conductivity
+000028f0: 5f52 5441 206f 7220 636f 6e64 7563 7469  _RTA or conducti
+00002900: 7669 7479 5f4c 4254 4520 636c 6173 7320  vity_LBTE class 
+00002910: 696e 7374 616e 6365 0a20 2020 2020 2020  instance.       
+00002920: 2073 656c 662e 5f74 6865 726d 616c 5f63   self._thermal_c
+00002930: 6f6e 6475 6374 6976 6974 7920 3d20 4e6f  onductivity = No
+00002940: 6e65 0a0a 2020 2020 2020 2020 2320 496d  ne..        # Im
+00002950: 6167 696e 6172 7920 7061 7274 206f 6620  aginary part of 
+00002960: 7365 6c66 2065 6e65 7267 7920 6174 2066  self energy at f
+00002970: 7265 7175 656e 6379 2070 6f69 6e74 730a  requency points.
+00002980: 2020 2020 2020 2020 7365 6c66 2e5f 6761          self._ga
+00002990: 6d6d 6173 203d 204e 6f6e 650a 2020 2020  mmas = None.    
+000029a0: 2020 2020 7365 6c66 2e5f 7363 6174 7465      self._scatte
+000029b0: 7269 6e67 5f65 7665 6e74 5f63 6c61 7373  ring_event_class
+000029c0: 203d 204e 6f6e 650a 0a20 2020 2020 2020   = None..       
+000029d0: 2023 2046 7265 7175 656e 6379 2073 6869   # Frequency shi
+000029e0: 6674 2028 7265 616c 2070 6172 7420 6f66  ft (real part of
+000029f0: 2062 7562 626c 6520 6469 6167 7261 6d29   bubble diagram)
+00002a00: 0a20 2020 2020 2020 2073 656c 662e 5f72  .        self._r
+00002a10: 6561 6c5f 7365 6c66 5f65 6e65 7267 7920  eal_self_energy 
+00002a20: 3d20 4e6f 6e65 0a0a 2020 2020 2020 2020  = None..        
+00002a30: 7365 6c66 2e5f 6772 6964 5f70 6f69 6e74  self._grid_point
+00002a40: 7320 3d20 4e6f 6e65 0a20 2020 2020 2020  s = None.       
+00002a50: 2073 656c 662e 5f66 7265 7175 656e 6379   self._frequency
+00002a60: 5f70 6f69 6e74 7320 3d20 4e6f 6e65 0a20  _points = None. 
+00002a70: 2020 2020 2020 2073 656c 662e 5f74 656d         self._tem
+00002a80: 7065 7261 7475 7265 7320 3d20 4e6f 6e65  peratures = None
+00002a90: 0a0a 2020 2020 2020 2020 2320 4f74 6865  ..        # Othe
+00002aa0: 7220 7661 7269 6162 6c65 730a 2020 2020  r variables.    
+00002ab0: 2020 2020 7365 6c66 2e5f 6663 3220 3d20      self._fc2 = 
+00002ac0: 4e6f 6e65 0a20 2020 2020 2020 2073 656c  None.        sel
+00002ad0: 662e 5f66 6333 203d 204e 6f6e 650a 0a20  f._fc3 = None.. 
+00002ae0: 2020 2020 2020 2023 2053 6574 7570 2069         # Setup i
+00002af0: 6e74 6572 6163 7469 6f6e 0a20 2020 2020  nteraction.     
+00002b00: 2020 2073 656c 662e 5f69 6e74 6572 6163     self._interac
+00002b10: 7469 6f6e 203d 204e 6f6e 650a 2020 2020  tion = None.    
+00002b20: 2020 2020 7365 6c66 2e5f 6261 6e64 5f69      self._band_i
+00002b30: 6e64 6963 6573 203d 204e 6f6e 650a 2020  ndices = None.  
+00002b40: 2020 2020 2020 7365 6c66 2e5f 6261 6e64        self._band
+00002b50: 5f69 6e64 6963 6573 5f66 6c61 7474 656e  _indices_flatten
+00002b60: 203d 204e 6f6e 650a 2020 2020 2020 2020   = None.        
+00002b70: 7365 6c66 2e5f 7365 745f 6261 6e64 5f69  self._set_band_i
+00002b80: 6e64 6963 6573 2829 0a0a 2020 2020 4070  ndices()..    @p
+00002b90: 726f 7065 7274 790a 2020 2020 6465 6620  roperty.    def 
+00002ba0: 7665 7273 696f 6e28 7365 6c66 293a 0a20  version(self):. 
+00002bb0: 2020 2020 2020 2022 2222 5265 7475 726e         """Return
+00002bc0: 2070 686f 6e6f 3370 7920 7265 6c65 6173   phono3py releas
+00002bd0: 6520 7665 7273 696f 6e20 6e75 6d62 6572  e version number
+00002be0: 2e0a 0a20 2020 2020 2020 2073 7472 0a20  ...        str. 
+00002bf0: 2020 2020 2020 2020 2020 2050 686f 6e6f             Phono
+00002c00: 3370 7920 7265 6c65 6173 6520 7665 7273  3py release vers
+00002c10: 696f 6e20 6e75 6d62 6572 0a0a 2020 2020  ion number..    
+00002c20: 2020 2020 2222 220a 2020 2020 2020 2020      """.        
+00002c30: 7265 7475 726e 205f 5f76 6572 7369 6f6e  return __version
+00002c40: 5f5f 0a0a 2020 2020 4070 726f 7065 7274  __..    @propert
+00002c50: 790a 2020 2020 6465 6620 6361 6c63 756c  y.    def calcul
+00002c60: 6174 6f72 2873 656c 6629 202d 3e20 4f70  ator(self) -> Op
+00002c70: 7469 6f6e 616c 5b73 7472 5d3a 0a20 2020  tional[str]:.   
+00002c80: 2020 2020 2022 2222 5265 7475 726e 2063       """Return c
+00002c90: 616c 6375 6c61 746f 7220 696e 7465 7266  alculator interf
+00002ca0: 6163 6520 6e61 6d65 2e0a 0a20 2020 2020  ace name...     
+00002cb0: 2020 2073 7472 0a20 2020 2020 2020 2020     str.         
+00002cc0: 2020 2043 616c 6375 6c61 746f 7220 6e61     Calculator na
+00002cd0: 6d65 2073 7563 6820 6173 2027 7661 7370  me such as 'vasp
+00002ce0: 272c 2027 7165 272c 2065 7463 2e0a 0a20  ', 'qe', etc... 
+00002cf0: 2020 2020 2020 2022 2222 0a20 2020 2020         """.     
+00002d00: 2020 2072 6574 7572 6e20 7365 6c66 2e5f     return self._
+00002d10: 6361 6c63 756c 6174 6f72 0a0a 2020 2020  calculator..    
+00002d20: 4070 726f 7065 7274 790a 2020 2020 6465  @property.    de
+00002d30: 6620 6663 3328 7365 6c66 293a 0a20 2020  f fc3(self):.   
+00002d40: 2020 2020 2022 2222 5365 7474 6572 2061       """Setter a
+00002d50: 6e64 2067 6574 7465 7220 6f66 2074 6869  nd getter of thi
+00002d60: 7264 206f 7264 6572 2066 6f72 6365 2063  rd order force c
+00002d70: 6f6e 7374 616e 7473 2028 6663 3329 2e0a  onstants (fc3)..
+00002d80: 0a20 2020 2020 2020 206e 6461 7272 6179  .        ndarray
+00002d90: 0a20 2020 2020 2020 2020 2020 2066 6333  .            fc3
+00002da0: 2073 6861 7065 2069 7320 6569 7468 6572   shape is either
+00002db0: 2028 7375 7065 7263 656c 6c2c 2073 7570   (supercell, sup
+00002dc0: 6563 656c 6c2c 2073 7570 6572 6365 6c6c  ecell, supercell
+00002dd0: 2c20 332c 2033 2c20 3329 206f 720a 2020  , 3, 3, 3) or.  
+00002de0: 2020 2020 2020 2020 2020 2870 7269 6d69            (primi
+00002df0: 7469 7665 2c20 7375 7065 7263 656c 6c2c  tive, supercell,
+00002e00: 2073 7570 6563 656c 6c2c 2033 2c20 332c   supecell, 3, 3,
+00002e10: 2033 292c 0a20 2020 2020 2020 2020 2020   3),.           
+00002e20: 2077 6865 7265 2027 7375 7065 7263 656c   where 'supercel
+00002e30: 6c27 2061 6e64 2027 7072 696d 6974 6976  l' and 'primitiv
+00002e40: 6527 2069 6e64 6963 6174 6520 6e75 6d62  e' indicate numb
+00002e50: 6572 206f 6620 6174 6f6d 7320 696e 0a20  er of atoms in. 
+00002e60: 2020 2020 2020 2020 2020 2074 6865 7365             these
+00002e70: 2063 656c 6c73 2e0a 0a20 2020 2020 2020   cells...       
+00002e80: 2022 2222 0a20 2020 2020 2020 2072 6574   """.        ret
+00002e90: 7572 6e20 7365 6c66 2e5f 6663 330a 0a20  urn self._fc3.. 
+00002ea0: 2020 2040 6663 332e 7365 7474 6572 0a20     @fc3.setter. 
+00002eb0: 2020 2064 6566 2066 6333 2873 656c 662c     def fc3(self,
+00002ec0: 2066 6333 293a 0a20 2020 2020 2020 2073   fc3):.        s
+00002ed0: 656c 662e 5f66 6333 203d 2066 6333 0a0a  elf._fc3 = fc3..
+00002ee0: 2020 2020 4070 726f 7065 7274 790a 2020      @property.  
+00002ef0: 2020 6465 6620 6663 3228 7365 6c66 293a    def fc2(self):
+00002f00: 0a20 2020 2020 2020 2022 2222 5365 7474  .        """Sett
+00002f10: 6572 2061 6e64 2067 6574 7465 7220 6f66  er and getter of
+00002f20: 2073 6563 6f6e 6420 6f72 6465 7220 666f   second order fo
+00002f30: 7263 6520 636f 6e73 7461 6e74 7320 2866  rce constants (f
+00002f40: 6332 292e 0a0a 2020 2020 2020 2020 6e64  c2)...        nd
+00002f50: 6172 7261 790a 2020 2020 2020 2020 2020  array.          
+00002f60: 2020 6663 3220 7368 6170 6520 6973 2065    fc2 shape is e
+00002f70: 6974 6865 7220 2873 7570 6572 6365 6c6c  ither (supercell
+00002f80: 2c20 7375 7065 6365 6c6c 2c20 332c 2033  , supecell, 3, 3
+00002f90: 2920 6f72 0a20 2020 2020 2020 2020 2020  ) or.           
+00002fa0: 2028 7072 696d 6974 6976 652c 2073 7570   (primitive, sup
+00002fb0: 6563 656c 6c2c 2033 2c20 3329 2c0a 2020  ecell, 3, 3),.  
+00002fc0: 2020 2020 2020 2020 2020 7768 6572 6520            where 
+00002fd0: 2773 7570 6572 6365 6c6c 2720 616e 6420  'supercell' and 
+00002fe0: 2770 7269 6d69 7469 7665 2720 696e 6469  'primitive' indi
+00002ff0: 6361 7465 206e 756d 6265 7220 6f66 2061  cate number of a
+00003000: 746f 6d73 2069 6e0a 2020 2020 2020 2020  toms in.        
+00003010: 2020 2020 7468 6573 6520 6365 6c6c 732e      these cells.
+00003020: 0a0a 2020 2020 2020 2020 2222 220a 2020  ..        """.  
+00003030: 2020 2020 2020 7265 7475 726e 2073 656c        return sel
+00003040: 662e 5f66 6332 0a0a 2020 2020 4066 6332  f._fc2..    @fc2
+00003050: 2e73 6574 7465 720a 2020 2020 6465 6620  .setter.    def 
+00003060: 6663 3228 7365 6c66 2c20 6663 3229 3a0a  fc2(self, fc2):.
+00003070: 2020 2020 2020 2020 7365 6c66 2e5f 6663          self._fc
+00003080: 3220 3d20 6663 320a 0a20 2020 2040 7072  2 = fc2..    @pr
+00003090: 6f70 6572 7479 0a20 2020 2064 6566 2066  operty.    def f
+000030a0: 6f72 6365 5f63 6f6e 7374 616e 7473 2873  orce_constants(s
+000030b0: 656c 6629 3a0a 2020 2020 2020 2020 2222  elf):.        ""
+000030c0: 2252 6574 7572 6e20 6663 322e 2054 6869  "Return fc2. Thi
+000030d0: 7320 6973 2073 616d 6520 6173 2074 6865  s is same as the
+000030e0: 2067 6574 7465 7220 6174 7472 6962 7574   getter attribut
+000030f0: 6520 6066 6332 602e 2222 220a 2020 2020  e `fc2`.""".    
+00003100: 2020 2020 7265 7475 726e 2073 656c 662e      return self.
+00003110: 6663 320a 0a20 2020 2040 7072 6f70 6572  fc2..    @proper
+00003120: 7479 0a20 2020 2064 6566 2073 6967 6d61  ty.    def sigma
+00003130: 7328 7365 6c66 293a 0a20 2020 2020 2020  s(self):.       
+00003140: 2022 2222 5365 7474 6572 2061 6e64 2067   """Setter and g
+00003150: 6574 7465 7220 6f66 2073 6d65 6172 696e  etter of smearin
+00003160: 6720 7769 6474 6873 2e0a 0a20 2020 2020  g widths...     
+00003170: 2020 206c 6973 740a 2020 2020 2020 2020     list.        
+00003180: 2020 2020 5468 6520 666c 6f61 7420 7661      The float va
+00003190: 6c75 6573 2061 7265 2067 6976 656e 2061  lues are given a
+000031a0: 7320 7468 6520 7374 616e 6461 7264 2064  s the standard d
+000031b0: 6576 6961 7469 6f6e 7320 6f66 2047 6175  eviations of Gau
+000031c0: 7373 6961 6e0a 2020 2020 2020 2020 2020  ssian.          
+000031d0: 2020 6675 6e63 7469 6f6e 2e20 4966 204e    function. If N
+000031e0: 6f6e 6520 6973 2067 6976 656e 2061 7320  one is given as 
+000031f0: 616e 2065 6c65 6d65 6e74 206f 6620 7468  an element of th
+00003200: 6973 206c 6973 742c 206c 696e 6561 720a  is list, linear.
+00003210: 2020 2020 2020 2020 2020 2020 7465 7472              tetr
+00003220: 6168 6564 726f 6e20 6d65 7468 6f64 2069  ahedron method i
+00003230: 7320 7573 6564 2069 6e73 7465 6164 206f  s used instead o
+00003240: 6620 736d 6561 7269 6e67 206d 6574 686f  f smearing metho
+00003250: 642e 0a0a 2020 2020 2020 2020 2222 220a  d...        """.
+00003260: 2020 2020 2020 2020 7265 7475 726e 2073          return s
+00003270: 656c 662e 5f73 6967 6d61 730a 0a20 2020  elf._sigmas..   
+00003280: 2040 7369 676d 6173 2e73 6574 7465 720a   @sigmas.setter.
+00003290: 2020 2020 6465 6620 7369 676d 6173 2873      def sigmas(s
+000032a0: 656c 662c 2073 6967 6d61 7329 3a0a 2020  elf, sigmas):.  
+000032b0: 2020 2020 2020 6966 2073 6967 6d61 7320        if sigmas 
+000032c0: 6973 204e 6f6e 653a 0a20 2020 2020 2020  is None:.       
+000032d0: 2020 2020 2073 656c 662e 5f73 6967 6d61       self._sigma
+000032e0: 7320 3d20 5b0a 2020 2020 2020 2020 2020  s = [.          
+000032f0: 2020 2020 2020 4e6f 6e65 2c0a 2020 2020        None,.    
+00003300: 2020 2020 2020 2020 5d0a 2020 2020 2020          ].      
+00003310: 2020 656c 6966 2069 7369 6e73 7461 6e63    elif isinstanc
+00003320: 6528 7369 676d 6173 2c20 666c 6f61 7429  e(sigmas, float)
+00003330: 206f 7220 6973 696e 7374 616e 6365 2873   or isinstance(s
+00003340: 6967 6d61 732c 2069 6e74 293a 0a20 2020  igmas, int):.   
+00003350: 2020 2020 2020 2020 2073 656c 662e 5f73           self._s
+00003360: 6967 6d61 7320 3d20 5b0a 2020 2020 2020  igmas = [.      
+00003370: 2020 2020 2020 2020 2020 666c 6f61 7428            float(
+00003380: 7369 676d 6173 292c 0a20 2020 2020 2020  sigmas),.       
+00003390: 2020 2020 205d 0a20 2020 2020 2020 2065       ].        e
+000033a0: 6c73 653a 0a20 2020 2020 2020 2020 2020  lse:.           
+000033b0: 2073 656c 662e 5f73 6967 6d61 7320 3d20   self._sigmas = 
+000033c0: 5b5d 0a20 2020 2020 2020 2020 2020 2066  [].            f
+000033d0: 6f72 2073 2069 6e20 7369 676d 6173 3a0a  or s in sigmas:.
+000033e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000033f0: 6966 2069 7369 6e73 7461 6e63 6528 732c  if isinstance(s,
+00003400: 2066 6c6f 6174 2920 6f72 2069 7369 6e73   float) or isins
+00003410: 7461 6e63 6528 732c 2069 6e74 293a 0a20  tance(s, int):. 
+00003420: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003430: 2020 2073 656c 662e 5f73 6967 6d61 732e     self._sigmas.
+00003440: 6170 7065 6e64 2866 6c6f 6174 2873 2929  append(float(s))
+00003450: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00003460: 2065 6c69 6620 7320 6973 204e 6f6e 653a   elif s is None:
+00003470: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00003480: 2020 2020 2073 656c 662e 5f73 6967 6d61       self._sigma
+00003490: 732e 6170 7065 6e64 284e 6f6e 6529 0a0a  s.append(None)..
+000034a0: 2020 2020 4070 726f 7065 7274 790a 2020      @property.  
+000034b0: 2020 6465 6620 7369 676d 615f 6375 746f    def sigma_cuto
+000034c0: 6666 2873 656c 6629 3a0a 2020 2020 2020  ff(self):.      
+000034d0: 2020 2222 2253 6574 7465 7220 616e 6420    """Setter and 
+000034e0: 6765 7474 6572 206f 6620 536d 6561 7269  getter of Smeari
+000034f0: 6e67 2063 7574 6f66 6620 7769 6474 682e  ng cutoff width.
+00003500: 0a0a 2020 2020 2020 2020 5468 6973 2069  ..        This i
+00003510: 7320 6769 7665 6e20 6173 2061 206d 756c  s given as a mul
+00003520: 7469 706c 6520 6f66 2074 6865 2073 7461  tiple of the sta
+00003530: 6e64 6172 6420 6465 7669 6174 696f 6e2e  ndard deviation.
+00003540: 0a0a 2020 2020 2020 2020 666c 6f61 740a  ..        float.
+00003550: 2020 2020 2020 2020 2020 2020 466f 7220              For 
+00003560: 6578 616d 706c 652c 2069 6620 7468 6973  example, if this
+00003570: 2076 616c 7565 2069 7320 352c 2074 6865   value is 5, the
+00003580: 2074 6169 6c20 6f66 2074 6865 2047 6175   tail of the Gau
+00003590: 7373 6961 6e20 6675 6e63 7469 6f6e 0a20  ssian function. 
+000035a0: 2020 2020 2020 2020 2020 2069 7320 6375             is cu
+000035b0: 7420 6174 2035 2073 6967 6d61 2e0a 0a20  t at 5 sigma... 
+000035c0: 2020 2020 2020 2022 2222 0a20 2020 2020         """.     
+000035d0: 2020 2072 6574 7572 6e20 7365 6c66 2e5f     return self._
+000035e0: 7369 676d 615f 6375 746f 6666 0a0a 2020  sigma_cutoff..  
+000035f0: 2020 4073 6967 6d61 5f63 7574 6f66 662e    @sigma_cutoff.
+00003600: 7365 7474 6572 0a20 2020 2064 6566 2073  setter.    def s
+00003610: 6967 6d61 5f63 7574 6f66 6628 7365 6c66  igma_cutoff(self
+00003620: 2c20 7369 676d 615f 6375 746f 6666 293a  , sigma_cutoff):
+00003630: 0a20 2020 2020 2020 2073 656c 662e 5f73  .        self._s
+00003640: 6967 6d61 5f63 7574 6f66 6620 3d20 7369  igma_cutoff = si
+00003650: 676d 615f 6375 746f 6666 0a0a 2020 2020  gma_cutoff..    
+00003660: 4070 726f 7065 7274 790a 2020 2020 6465  @property.    de
+00003670: 6620 6e61 635f 7061 7261 6d73 2873 656c  f nac_params(sel
+00003680: 6629 3a0a 2020 2020 2020 2020 2222 2253  f):.        """S
+00003690: 6574 7465 7220 616e 6420 6765 7474 6572  etter and getter
+000036a0: 206f 6620 7061 7261 6d65 7465 7273 2066   of parameters f
+000036b0: 6f72 206e 6f6e 2d61 6e61 6c79 7469 6361  or non-analytica
+000036c0: 6c20 7465 726d 2063 6f72 7265 6374 696f  l term correctio
+000036d0: 6e2e 0a0a 2020 2020 2020 2020 6469 6374  n...        dict
+000036e0: 0a20 2020 2020 2020 2020 2020 2050 6172  .            Par
+000036f0: 616d 6574 6572 7320 7573 6564 2066 6f72  ameters used for
+00003700: 206e 6f6e 2d61 6e61 6c79 7469 6361 6c20   non-analytical 
+00003710: 7465 726d 2063 6f72 7265 6374 696f 6e0a  term correction.
+00003720: 2020 2020 2020 2020 2020 2020 2762 6f72              'bor
+00003730: 6e27 3a20 6e64 6172 7261 790a 2020 2020  n': ndarray.    
+00003740: 2020 2020 2020 2020 2020 2020 426f 726e              Born
+00003750: 2065 6666 6563 7469 7665 2063 6861 7267   effective charg
+00003760: 6573 0a20 2020 2020 2020 2020 2020 2020  es.             
+00003770: 2020 2073 6861 7065 3d28 7072 696d 6974     shape=(primit
+00003780: 6976 6520 6365 6c6c 2061 746f 6d73 2c20  ive cell atoms, 
+00003790: 332c 2033 292c 2064 7479 7065 3d27 646f  3, 3), dtype='do
+000037a0: 7562 6c65 272c 206f 7264 6572 3d27 4327  uble', order='C'
+000037b0: 0a20 2020 2020 2020 2020 2020 2027 6661  .            'fa
+000037c0: 6374 6f72 273a 2066 6c6f 6174 0a20 2020  ctor': float.   
+000037d0: 2020 2020 2020 2020 2020 2020 2055 6e69               Uni
+000037e0: 7420 636f 6e76 6572 7369 6f6e 2066 6163  t conversion fac
+000037f0: 746f 720a 2020 2020 2020 2020 2020 2020  tor.            
+00003800: 2764 6965 6c65 6374 7269 6327 3a20 6e64  'dielectric': nd
+00003810: 6172 7261 790a 2020 2020 2020 2020 2020  array.          
+00003820: 2020 2020 2020 4469 656c 6563 7472 6963        Dielectric
+00003830: 2063 6f6e 7374 616e 7420 7465 6e73 6f72   constant tensor
+00003840: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00003850: 2073 6861 7065 3d28 332c 2033 292c 2064   shape=(3, 3), d
+00003860: 7479 7065 3d27 646f 7562 6c65 272c 206f  type='double', o
+00003870: 7264 6572 3d27 4327 0a0a 2020 2020 2020  rder='C'..      
+00003880: 2020 2222 220a 2020 2020 2020 2020 7265    """.        re
+00003890: 7475 726e 2073 656c 662e 5f6e 6163 5f70  turn self._nac_p
+000038a0: 6172 616d 730a 0a20 2020 2040 6e61 635f  arams..    @nac_
+000038b0: 7061 7261 6d73 2e73 6574 7465 720a 2020  params.setter.  
+000038c0: 2020 6465 6620 6e61 635f 7061 7261 6d73    def nac_params
+000038d0: 2873 656c 662c 206e 6163 5f70 6172 616d  (self, nac_param
+000038e0: 7329 3a0a 2020 2020 2020 2020 7365 6c66  s):.        self
+000038f0: 2e5f 6e61 635f 7061 7261 6d73 203d 206e  ._nac_params = n
+00003900: 6163 5f70 6172 616d 730a 2020 2020 2020  ac_params.      
+00003910: 2020 6966 2073 656c 662e 5f69 6e74 6572    if self._inter
+00003920: 6163 7469 6f6e 2069 7320 6e6f 7420 4e6f  action is not No
+00003930: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
+00003940: 7365 6c66 2e5f 696e 6974 5f64 796e 616d  self._init_dynam
+00003950: 6963 616c 5f6d 6174 7269 7828 290a 0a20  ical_matrix().. 
+00003960: 2020 2040 7072 6f70 6572 7479 0a20 2020     @property.   
+00003970: 2064 6566 2064 796e 616d 6963 616c 5f6d   def dynamical_m
+00003980: 6174 7269 7828 7365 6c66 293a 0a20 2020  atrix(self):.   
+00003990: 2020 2020 2022 2222 5265 7475 726e 2044       """Return D
+000039a0: 796e 616d 6963 616c 4d61 7472 6978 2069  ynamicalMatrix i
+000039b0: 6e73 7461 6e63 652e 0a0a 2020 2020 2020  nstance...      
+000039c0: 2020 5468 6973 2069 7320 6e6f 7420 6479    This is not dy
+000039d0: 6e61 6d69 6361 6c20 6d61 7472 6963 6573  namical matrices
+000039e0: 2062 7574 2074 6865 2069 6e73 7461 6e63   but the instanc
+000039f0: 6520 6f66 2044 796e 616d 6963 616c 4d61  e of DynamicalMa
+00003a00: 7472 6978 0a20 2020 2020 2020 2063 6c61  trix.        cla
+00003a10: 7373 2e0a 0a20 2020 2020 2020 2022 2222  ss...        """
+00003a20: 0a20 2020 2020 2020 2069 6620 7365 6c66  .        if self
+00003a30: 2e5f 696e 7465 7261 6374 696f 6e20 6973  ._interaction is
+00003a40: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
+00003a50: 2020 2072 6574 7572 6e20 4e6f 6e65 0a20     return None. 
+00003a60: 2020 2020 2020 2065 6c73 653a 0a20 2020         else:.   
+00003a70: 2020 2020 2020 2020 2072 6574 7572 6e20           return 
+00003a80: 7365 6c66 2e5f 696e 7465 7261 6374 696f  self._interactio
+00003a90: 6e2e 6479 6e61 6d69 6361 6c5f 6d61 7472  n.dynamical_matr
+00003aa0: 6978 0a0a 2020 2020 4070 726f 7065 7274  ix..    @propert
+00003ab0: 790a 2020 2020 6465 6620 7072 696d 6974  y.    def primit
+00003ac0: 6976 6528 7365 6c66 2920 2d3e 2050 7269  ive(self) -> Pri
+00003ad0: 6d69 7469 7665 3a0a 2020 2020 2020 2020  mitive:.        
+00003ae0: 2222 2252 6574 7572 6e20 7072 696d 6974  """Return primit
+00003af0: 6976 6520 6365 6c6c 2e0a 0a20 2020 2020  ive cell...     
+00003b00: 2020 2050 7269 6d69 7469 7665 0a20 2020     Primitive.   
+00003b10: 2020 2020 2020 2020 2050 7269 6d69 7469           Primiti
+00003b20: 7665 2063 656c 6c2e 0a0a 2020 2020 2020  ve cell...      
+00003b30: 2020 2222 220a 2020 2020 2020 2020 7265    """.        re
+00003b40: 7475 726e 2073 656c 662e 5f70 7269 6d69  turn self._primi
+00003b50: 7469 7665 0a0a 2020 2020 4070 726f 7065  tive..    @prope
+00003b60: 7274 790a 2020 2020 6465 6620 756e 6974  rty.    def unit
+00003b70: 6365 6c6c 2873 656c 6629 202d 3e20 5068  cell(self) -> Ph
+00003b80: 6f6e 6f70 7941 746f 6d73 3a0a 2020 2020  onopyAtoms:.    
+00003b90: 2020 2020 2222 2252 6574 7572 6e20 556e      """Return Un
+00003ba0: 6974 2063 656c 6c2e 0a0a 2020 2020 2020  it cell...      
+00003bb0: 2020 5068 6f6e 6f70 7941 746f 6d73 0a20    PhonopyAtoms. 
+00003bc0: 2020 2020 2020 2020 2020 2055 6e69 7420             Unit 
+00003bd0: 6365 6c6c 2e0a 0a20 2020 2020 2020 2022  cell...        "
+00003be0: 2222 0a20 2020 2020 2020 2072 6574 7572  "".        retur
+00003bf0: 6e20 7365 6c66 2e5f 756e 6974 6365 6c6c  n self._unitcell
+00003c00: 0a0a 2020 2020 4070 726f 7065 7274 790a  ..    @property.
+00003c10: 2020 2020 6465 6620 7375 7065 7263 656c      def supercel
+00003c20: 6c28 7365 6c66 2920 2d3e 2053 7570 6572  l(self) -> Super
+00003c30: 6365 6c6c 3a0a 2020 2020 2020 2020 2222  cell:.        ""
+00003c40: 2252 6574 7572 6e20 7375 7065 7263 656c  "Return supercel
+00003c50: 6c2e 0a0a 2020 2020 2020 2020 5375 7065  l...        Supe
+00003c60: 7263 656c 6c0a 2020 2020 2020 2020 2020  rcell.          
+00003c70: 2020 5375 7065 7263 656c 6c2e 0a0a 2020    Supercell...  
+00003c80: 2020 2020 2020 2222 220a 2020 2020 2020        """.      
+00003c90: 2020 7265 7475 726e 2073 656c 662e 5f73    return self._s
+00003ca0: 7570 6572 6365 6c6c 0a0a 2020 2020 4070  upercell..    @p
+00003cb0: 726f 7065 7274 790a 2020 2020 6465 6620  roperty.    def 
+00003cc0: 7068 6f6e 6f6e 5f73 7570 6572 6365 6c6c  phonon_supercell
+00003cd0: 2873 656c 6629 202d 3e20 5375 7065 7263  (self) -> Superc
+00003ce0: 656c 6c3a 0a20 2020 2020 2020 2022 2222  ell:.        """
+00003cf0: 5265 7475 726e 2073 7570 6572 6365 6c6c  Return supercell
+00003d00: 2066 6f72 2066 6332 2e0a 0a20 2020 2020   for fc2...     
+00003d10: 2020 2053 7570 6572 6365 6c6c 0a20 2020     Supercell.   
+00003d20: 2020 2020 2020 2020 2053 7570 6572 6365           Superce
+00003d30: 6c6c 2066 6f72 2066 6332 2e0a 0a20 2020  ll for fc2...   
+00003d40: 2020 2020 2022 2222 0a20 2020 2020 2020       """.       
+00003d50: 2072 6574 7572 6e20 7365 6c66 2e5f 7068   return self._ph
+00003d60: 6f6e 6f6e 5f73 7570 6572 6365 6c6c 0a0a  onon_supercell..
+00003d70: 2020 2020 4070 726f 7065 7274 790a 2020      @property.  
+00003d80: 2020 6465 6620 7068 6f6e 6f6e 5f70 7269    def phonon_pri
+00003d90: 6d69 7469 7665 2873 656c 6629 202d 3e20  mitive(self) -> 
+00003da0: 5072 696d 6974 6976 653a 0a20 2020 2020  Primitive:.     
+00003db0: 2020 2022 2222 5265 7475 726e 2070 7269     """Return pri
+00003dc0: 6d69 7469 7665 2063 656c 6c20 666f 7220  mitive cell for 
+00003dd0: 6663 322e 0a0a 2020 2020 2020 2020 5072  fc2...        Pr
+00003de0: 696d 6974 6976 650a 2020 2020 2020 2020  imitive.        
+00003df0: 2020 2020 5072 696d 6974 6976 6520 6365      Primitive ce
+00003e00: 6c6c 2066 6f72 2066 6332 2e20 5468 6973  ll for fc2. This
+00003e10: 2073 686f 756c 6420 6265 2074 6865 2073   should be the s
+00003e20: 616d 6520 6173 2074 6865 2070 7269 6d69  ame as the primi
+00003e30: 7469 7665 0a20 2020 2020 2020 2020 2020  tive.           
+00003e40: 2063 656c 6c20 666f 7220 6663 332c 2062   cell for fc3, b
+00003e50: 7574 2074 6869 7320 6973 2063 7265 6174  ut this is creat
+00003e60: 6564 2066 726f 6d20 7375 7065 7263 656c  ed from supercel
+00003e70: 6c20 666f 7220 6663 3220 616e 640a 2020  l for fc2 and.  
+00003e80: 2020 2020 2020 2020 2020 6361 6e20 6265            can be
+00003e90: 206e 6f74 206e 756d 6572 6963 616c 6c79   not numerically
+00003ea0: 2070 6572 6665 6374 6c79 2069 6465 6e74   perfectly ident
+00003eb0: 6963 616c 2e0a 0a20 2020 2020 2020 2022  ical...        "
+00003ec0: 2222 0a20 2020 2020 2020 2072 6574 7572  "".        retur
+00003ed0: 6e20 7365 6c66 2e5f 7068 6f6e 6f6e 5f70  n self._phonon_p
+00003ee0: 7269 6d69 7469 7665 0a0a 2020 2020 4070  rimitive..    @p
+00003ef0: 726f 7065 7274 790a 2020 2020 6465 6620  roperty.    def 
+00003f00: 7379 6d6d 6574 7279 2873 656c 6629 202d  symmetry(self) -
+00003f10: 3e20 5379 6d6d 6574 7279 3a0a 2020 2020  > Symmetry:.    
+00003f20: 2020 2020 2222 2252 6574 7572 6e20 7379      """Return sy
+00003f30: 6d6d 6574 7279 206f 6620 7375 7065 7263  mmetry of superc
+00003f40: 656c 6c2e 0a0a 2020 2020 2020 2020 5379  ell...        Sy
+00003f50: 6d6d 6574 7279 0a20 2020 2020 2020 2020  mmetry.         
+00003f60: 2020 2053 796d 6d65 7472 7920 6f66 2073     Symmetry of s
+00003f70: 7570 6572 6365 6c6c 0a0a 2020 2020 2020  upercell..      
+00003f80: 2020 2222 220a 2020 2020 2020 2020 7265    """.        re
+00003f90: 7475 726e 2073 656c 662e 5f73 796d 6d65  turn self._symme
+00003fa0: 7472 790a 0a20 2020 2040 7072 6f70 6572  try..    @proper
+00003fb0: 7479 0a20 2020 2064 6566 2070 7269 6d69  ty.    def primi
+00003fc0: 7469 7665 5f73 796d 6d65 7472 7928 7365  tive_symmetry(se
+00003fd0: 6c66 2920 2d3e 2053 796d 6d65 7472 793a  lf) -> Symmetry:
+00003fe0: 0a20 2020 2020 2020 2022 2222 5265 7475  .        """Retu
+00003ff0: 726e 2073 796d 6d65 7472 7920 6f66 2070  rn symmetry of p
+00004000: 7269 6d69 7469 7665 2063 656c 6c2e 0a0a  rimitive cell...
 00004010: 2020 2020 2020 2020 5379 6d6d 6574 7279          Symmetry
-00004020: 206f 6620 7072 696d 6974 6976 6520 6365   of primitive ce
-00004030: 6c6c 2e0a 0a20 2020 2020 2020 2022 2222  ll...        """
-00004040: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
-00004050: 7365 6c66 2e5f 7072 696d 6974 6976 655f  self._primitive_
-00004060: 7379 6d6d 6574 7279 0a0a 2020 2020 4070  symmetry..    @p
-00004070: 726f 7065 7274 790a 2020 2020 6465 6620  roperty.    def 
-00004080: 7068 6f6e 6f6e 5f73 7570 6572 6365 6c6c  phonon_supercell
-00004090: 5f73 796d 6d65 7472 7928 7365 6c66 2920  _symmetry(self) 
-000040a0: 2d3e 2053 796d 6d65 7472 793a 0a20 2020  -> Symmetry:.   
-000040b0: 2020 2020 2022 2222 5265 7475 726e 2073       """Return s
-000040c0: 796d 6d65 7472 7920 6f66 2073 7570 6572  ymmetry of super
-000040d0: 6365 6c6c 2066 6f72 2066 6332 2e0a 0a20  cell for fc2... 
-000040e0: 2020 2020 2020 2053 796d 6d65 7472 790a         Symmetry.
-000040f0: 2020 2020 2020 2020 2020 2020 5379 6d6d              Symm
-00004100: 6574 7279 206f 6620 7375 7065 7263 656c  etry of supercel
-00004110: 6c20 666f 7220 6663 3220 2870 686f 6e6f  l for fc2 (phono
-00004120: 6e5f 7375 7065 7263 656c 6c29 2e0a 0a20  n_supercell)... 
-00004130: 2020 2020 2020 2022 2222 0a20 2020 2020         """.     
-00004140: 2020 2072 6574 7572 6e20 7365 6c66 2e5f     return self._
-00004150: 7068 6f6e 6f6e 5f73 7570 6572 6365 6c6c  phonon_supercell
-00004160: 5f73 796d 6d65 7472 790a 0a20 2020 2040  _symmetry..    @
-00004170: 7072 6f70 6572 7479 0a20 2020 2064 6566  property.    def
-00004180: 2073 7570 6572 6365 6c6c 5f6d 6174 7269   supercell_matri
-00004190: 7828 7365 6c66 293a 0a20 2020 2020 2020  x(self):.       
-000041a0: 2022 2222 5265 7475 726e 2074 7261 6e73   """Return trans
-000041b0: 666f 726d 6174 696f 6e20 6d61 7472 6978  formation matrix
-000041c0: 2074 6f20 7375 7065 7263 656c 6c20 6365   to supercell ce
-000041d0: 6c6c 2066 726f 6d20 756e 6974 2063 656c  ll from unit cel
-000041e0: 6c2e 0a0a 2020 2020 2020 2020 6e64 6172  l...        ndar
-000041f0: 7261 790a 2020 2020 2020 2020 2020 2020  ray.            
-00004200: 5375 7065 7263 656c 6c20 6d61 7472 6978  Supercell matrix
-00004210: 2077 6974 6820 7265 7370 6563 7420 746f   with respect to
-00004220: 2075 6e69 7420 6365 6c6c 2e0a 2020 2020   unit cell..    
-00004230: 2020 2020 2020 2020 7368 6170 653d 2833          shape=(3
-00004240: 2c20 3329 2c20 6474 7970 653d 2769 6e74  , 3), dtype='int
-00004250: 5f27 2c20 6f72 6465 723d 2743 270a 0a20  _', order='C'.. 
-00004260: 2020 2020 2020 2022 2222 0a20 2020 2020         """.     
-00004270: 2020 2072 6574 7572 6e20 7365 6c66 2e5f     return self._
-00004280: 7375 7065 7263 656c 6c5f 6d61 7472 6978  supercell_matrix
-00004290: 0a0a 2020 2020 4070 726f 7065 7274 790a  ..    @property.
-000042a0: 2020 2020 6465 6620 7068 6f6e 6f6e 5f73      def phonon_s
-000042b0: 7570 6572 6365 6c6c 5f6d 6174 7269 7828  upercell_matrix(
-000042c0: 7365 6c66 293a 0a20 2020 2020 2020 2022  self):.        "
-000042d0: 2222 5265 7475 726e 2074 7261 6e73 666f  ""Return transfo
-000042e0: 726d 6174 696f 6e20 6d61 7472 6978 2074  rmation matrix t
-000042f0: 6f20 7068 6f6e 6f6e 2073 7570 6572 6365  o phonon superce
-00004300: 6c6c 2066 726f 6d20 756e 6974 2063 656c  ll from unit cel
-00004310: 6c2e 0a0a 2020 2020 2020 2020 6e64 6172  l...        ndar
-00004320: 7261 790a 2020 2020 2020 2020 2020 2020  ray.            
-00004330: 5375 7065 7263 656c 6c20 6d61 7472 6978  Supercell matrix
-00004340: 2077 6974 6820 7265 7370 6563 7420 746f   with respect to
-00004350: 2075 6e69 7420 6365 6c6c 2e0a 2020 2020   unit cell..    
-00004360: 2020 2020 2020 2020 7368 6170 653d 2833          shape=(3
-00004370: 2c20 3329 2c20 6474 7970 653d 2769 6e74  , 3), dtype='int
-00004380: 5f27 2c20 6f72 6465 723d 2743 270a 0a20  _', order='C'.. 
-00004390: 2020 2020 2020 2022 2222 0a20 2020 2020         """.     
-000043a0: 2020 2072 6574 7572 6e20 7365 6c66 2e5f     return self._
-000043b0: 7068 6f6e 6f6e 5f73 7570 6572 6365 6c6c  phonon_supercell
-000043c0: 5f6d 6174 7269 780a 0a20 2020 2040 7072  _matrix..    @pr
-000043d0: 6f70 6572 7479 0a20 2020 2064 6566 2070  operty.    def p
-000043e0: 7269 6d69 7469 7665 5f6d 6174 7269 7828  rimitive_matrix(
-000043f0: 7365 6c66 293a 0a20 2020 2020 2020 2022  self):.        "
-00004400: 2222 5265 7475 726e 2074 7261 6e73 666f  ""Return transfo
-00004410: 726d 6174 696f 6e20 6d61 7472 6978 2074  rmation matrix t
-00004420: 6f20 7072 696d 6974 6976 6520 6365 6c6c  o primitive cell
-00004430: 2066 726f 6d20 756e 6974 2063 656c 6c2e   from unit cell.
-00004440: 0a0a 2020 2020 2020 2020 6e64 6172 7261  ..        ndarra
-00004450: 790a 2020 2020 2020 2020 2020 2020 5072  y.            Pr
-00004460: 696d 6974 6976 6520 6d61 7472 6978 2077  imitive matrix w
-00004470: 6974 6820 7265 7370 6563 7420 746f 2075  ith respect to u
-00004480: 6e69 7420 6365 6c6c 2e0a 2020 2020 2020  nit cell..      
-00004490: 2020 2020 2020 7368 6170 653d 2833 2c20        shape=(3, 
-000044a0: 3329 2c20 6474 7970 653d 2764 6f75 626c  3), dtype='doubl
-000044b0: 6527 2c20 6f72 6465 723d 2743 270a 0a20  e', order='C'.. 
-000044c0: 2020 2020 2020 2022 2222 0a20 2020 2020         """.     
-000044d0: 2020 2072 6574 7572 6e20 7365 6c66 2e5f     return self._
-000044e0: 7072 696d 6974 6976 655f 6d61 7472 6978  primitive_matrix
-000044f0: 0a0a 2020 2020 4070 726f 7065 7274 790a  ..    @property.
-00004500: 2020 2020 6465 6620 756e 6974 5f63 6f6e      def unit_con
-00004510: 7665 7273 696f 6e5f 6661 6374 6f72 2873  version_factor(s
-00004520: 656c 6629 3a0a 2020 2020 2020 2020 2222  elf):.        ""
-00004530: 2252 6574 7572 6e20 7068 6f6e 6f6e 2066  "Return phonon f
-00004540: 7265 7175 656e 6379 2075 6e69 7420 636f  requency unit co
-00004550: 6e76 6572 7369 6f6e 2066 6163 746f 722e  nversion factor.
-00004560: 0a0a 2020 2020 2020 2020 666c 6f61 740a  ..        float.
-00004570: 2020 2020 2020 2020 2020 2020 5068 6f6e              Phon
-00004580: 6f6e 2066 7265 7175 656e 6379 2075 6e69  on frequency uni
-00004590: 7420 636f 6e76 6572 7369 6f6e 2066 6163  t conversion fac
-000045a0: 746f 722e 2054 6869 7320 6661 6374 6f72  tor. This factor
-000045b0: 0a20 2020 2020 2020 2020 2020 2063 6f6e  .            con
-000045c0: 7665 7274 7320 7371 7274 283c 666f 7263  verts sqrt(<forc
-000045d0: 653e 2f3c 6469 7374 616e 6365 3e2f 3c41  e>/<distance>/<A
-000045e0: 4d55 3e29 2f32 7069 2f31 6531 3220 746f  MU>)/2pi/1e12 to
-000045f0: 2054 487a 0a20 2020 2020 2020 2020 2020   THz.           
-00004600: 2028 6f72 6469 6e61 7279 2066 7265 7175   (ordinary frequ
-00004610: 656e 6379 292e 0a0a 2020 2020 2020 2020  ency)...        
-00004620: 2222 220a 2020 2020 2020 2020 7265 7475  """.        retu
-00004630: 726e 2073 656c 662e 5f66 7265 7175 656e  rn self._frequen
-00004640: 6379 5f66 6163 746f 725f 746f 5f54 487a  cy_factor_to_THz
-00004650: 0a0a 2020 2020 4070 726f 7065 7274 790a  ..    @property.
-00004660: 2020 2020 6465 6620 6461 7461 7365 7428      def dataset(
-00004670: 7365 6c66 293a 0a20 2020 2020 2020 2022  self):.        "
-00004680: 2222 5365 7474 6572 2061 6e64 2067 6574  ""Setter and get
-00004690: 7465 7220 6f66 2064 6973 706c 6163 656d  ter of displacem
-000046a0: 656e 742d 666f 7263 6520 6461 7461 7365  ent-force datase
-000046b0: 742e 0a0a 2020 2020 2020 2020 6469 6374  t...        dict
-000046c0: 0a20 2020 2020 2020 2020 2020 2044 6973  .            Dis
-000046d0: 706c 6163 656d 656e 7473 2069 6e20 7375  placements in su
-000046e0: 7065 7263 656c 6c73 2e20 5468 6572 6520  percells. There 
-000046f0: 6172 6520 7477 6f20 7479 7065 7320 6f66  are two types of
-00004700: 2066 6f72 6d61 7473 2e0a 2020 2020 2020   formats..      
-00004710: 2020 2020 2020 5479 7065 2031 2e20 5477        Type 1. Tw
-00004720: 6f20 6174 6f6d 6963 2064 6973 706c 6163  o atomic displac
-00004730: 656d 656e 7420 696e 2065 6163 6820 7375  ement in each su
-00004740: 7065 7263 656c 6c3a 0a20 2020 2020 2020  percell:.       
-00004750: 2020 2020 2020 2020 207b 276e 6174 6f6d           {'natom
-00004760: 273a 206e 756d 6265 7220 6f66 2061 746f  ': number of ato
-00004770: 6d73 2069 6e20 7375 7065 7263 656c 6c2c  ms in supercell,
-00004780: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00004790: 2020 2766 6972 7374 5f61 746f 6d73 273a    'first_atoms':
-000047a0: 205b 0a20 2020 2020 2020 2020 2020 2020   [.             
-000047b0: 2020 2020 2020 7b27 6e75 6d62 6572 273a        {'number':
-000047c0: 2061 746f 6d20 696e 6465 7820 6f66 2066   atom index of f
-000047d0: 6972 7374 2064 6973 706c 6163 6564 2061  irst displaced a
-000047e0: 746f 6d2c 0a20 2020 2020 2020 2020 2020  tom,.           
-000047f0: 2020 2020 2020 2020 2027 6469 7370 6c61           'displa
-00004800: 6365 6d65 6e74 273a 2064 6973 706c 6163  cement': displac
-00004810: 656d 656e 7420 696e 2043 6172 7465 7369  ement in Cartesi
-00004820: 616e 2063 6f6f 7264 696e 6174 6573 2c0a  an coordinates,.
-00004830: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004840: 2020 2020 2766 6f72 6365 7327 3a20 666f      'forces': fo
-00004850: 7263 6573 206f 6e20 6174 6f6d 7320 696e  rces on atoms in
-00004860: 2073 7570 6572 6365 6c6c 2c0a 2020 2020   supercell,.    
-00004870: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004880: 2769 6427 3a20 6469 7370 6c61 6365 6d65  'id': displaceme
-00004890: 6e74 2069 6420 2831 2c20 322c 2e2e 2e2c  nt id (1, 2,...,
-000048a0: 6e5f 6669 7273 745f 6174 6f6d 7329 0a20  n_first_atoms). 
-000048b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000048c0: 2020 2027 7365 636f 6e64 5f61 746f 6d73     'second_atoms
-000048d0: 273a 205b 0a20 2020 2020 2020 2020 2020  ': [.           
-000048e0: 2020 2020 2020 2020 2020 207b 276e 756d             {'num
-000048f0: 6265 7227 3a20 6174 6f6d 2069 6e64 6578  ber': atom index
-00004900: 206f 6620 7365 636f 6e64 2064 6973 706c   of second displ
-00004910: 6163 6564 2061 746f 6d2c 0a20 2020 2020  aced atom,.     
-00004920: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004930: 2020 2764 6973 706c 6163 656d 656e 7427    'displacement'
-00004940: 3a20 6469 7370 6c61 6365 6d65 6e74 2069  : displacement i
-00004950: 6e20 4361 7274 6573 6961 6e20 636f 6f72  n Cartesian coor
-00004960: 6469 6e61 7465 737d 2c0a 2020 2020 2020  dinates},.      
-00004970: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004980: 2027 666f 7263 6573 273a 2066 6f72 6365   'forces': force
-00004990: 7320 6f6e 2061 746f 6d73 2069 6e20 7375  s on atoms in su
-000049a0: 7065 7263 656c 6c2c 0a20 2020 2020 2020  percell,.       
-000049b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000049c0: 2770 6169 725f 6469 7374 616e 6365 273a  'pair_distance':
-000049d0: 2064 6973 7461 6e63 6520 6265 7477 6565   distance betwee
-000049e0: 6e20 7061 6972 6564 2061 746f 6d73 2c0a  n paired atoms,.
-000049f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004a00: 2020 2020 2020 2027 696e 636c 7564 6564         'included
-00004a10: 273a 2077 6974 6820 6375 746f 6666 2070  ': with cutoff p
-00004a20: 6169 7220 6469 7374 616e 6365 2069 6e20  air distance in 
-00004a30: 6469 7370 6c61 6365 6d65 6e74 0a20 2020  displacement.   
-00004a40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004a50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004a60: 7061 6972 2067 656e 6572 6174 696f 6e2c  pair generation,
-00004a70: 2074 6869 7320 696e 6469 6361 7465 7320   this indicates 
-00004a80: 6966 2074 6869 730a 2020 2020 2020 2020  if this.        
-00004a90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004aa0: 2020 2020 2020 2020 2020 2070 6169 7220             pair 
-00004ab0: 6469 7370 6c61 6365 6d65 6e74 7320 6973  displacements is
-00004ac0: 2069 6e63 6c75 6465 6420 746f 2063 6f6d   included to com
-00004ad0: 7075 7465 0a20 2020 2020 2020 2020 2020  pute.           
+00004020: 0a20 2020 2020 2020 2020 2020 2053 796d  .            Sym
+00004030: 6d65 7472 7920 6f66 2070 7269 6d69 7469  metry of primiti
+00004040: 7665 2063 656c 6c2e 0a0a 2020 2020 2020  ve cell...      
+00004050: 2020 2222 220a 2020 2020 2020 2020 7265    """.        re
+00004060: 7475 726e 2073 656c 662e 5f70 7269 6d69  turn self._primi
+00004070: 7469 7665 5f73 796d 6d65 7472 790a 0a20  tive_symmetry.. 
+00004080: 2020 2040 7072 6f70 6572 7479 0a20 2020     @property.   
+00004090: 2064 6566 2070 686f 6e6f 6e5f 7375 7065   def phonon_supe
+000040a0: 7263 656c 6c5f 7379 6d6d 6574 7279 2873  rcell_symmetry(s
+000040b0: 656c 6629 202d 3e20 5379 6d6d 6574 7279  elf) -> Symmetry
+000040c0: 3a0a 2020 2020 2020 2020 2222 2252 6574  :.        """Ret
+000040d0: 7572 6e20 7379 6d6d 6574 7279 206f 6620  urn symmetry of 
+000040e0: 7375 7065 7263 656c 6c20 666f 7220 6663  supercell for fc
+000040f0: 322e 0a0a 2020 2020 2020 2020 5379 6d6d  2...        Symm
+00004100: 6574 7279 0a20 2020 2020 2020 2020 2020  etry.           
+00004110: 2053 796d 6d65 7472 7920 6f66 2073 7570   Symmetry of sup
+00004120: 6572 6365 6c6c 2066 6f72 2066 6332 2028  ercell for fc2 (
+00004130: 7068 6f6e 6f6e 5f73 7570 6572 6365 6c6c  phonon_supercell
+00004140: 292e 0a0a 2020 2020 2020 2020 2222 220a  )...        """.
+00004150: 2020 2020 2020 2020 7265 7475 726e 2073          return s
+00004160: 656c 662e 5f70 686f 6e6f 6e5f 7375 7065  elf._phonon_supe
+00004170: 7263 656c 6c5f 7379 6d6d 6574 7279 0a0a  rcell_symmetry..
+00004180: 2020 2020 4070 726f 7065 7274 790a 2020      @property.  
+00004190: 2020 6465 6620 7375 7065 7263 656c 6c5f    def supercell_
+000041a0: 6d61 7472 6978 2873 656c 6629 3a0a 2020  matrix(self):.  
+000041b0: 2020 2020 2020 2222 2252 6574 7572 6e20        """Return 
+000041c0: 7472 616e 7366 6f72 6d61 7469 6f6e 206d  transformation m
+000041d0: 6174 7269 7820 746f 2073 7570 6572 6365  atrix to superce
+000041e0: 6c6c 2063 656c 6c20 6672 6f6d 2075 6e69  ll cell from uni
+000041f0: 7420 6365 6c6c 2e0a 0a20 2020 2020 2020  t cell...       
+00004200: 206e 6461 7272 6179 0a20 2020 2020 2020   ndarray.       
+00004210: 2020 2020 2053 7570 6572 6365 6c6c 206d       Supercell m
+00004220: 6174 7269 7820 7769 7468 2072 6573 7065  atrix with respe
+00004230: 6374 2074 6f20 756e 6974 2063 656c 6c2e  ct to unit cell.
+00004240: 0a20 2020 2020 2020 2020 2020 2073 6861  .            sha
+00004250: 7065 3d28 332c 2033 292c 2064 7479 7065  pe=(3, 3), dtype
+00004260: 3d27 696e 745f 272c 206f 7264 6572 3d27  ='int_', order='
+00004270: 4327 0a0a 2020 2020 2020 2020 2222 220a  C'..        """.
+00004280: 2020 2020 2020 2020 7265 7475 726e 2073          return s
+00004290: 656c 662e 5f73 7570 6572 6365 6c6c 5f6d  elf._supercell_m
+000042a0: 6174 7269 780a 0a20 2020 2040 7072 6f70  atrix..    @prop
+000042b0: 6572 7479 0a20 2020 2064 6566 2070 686f  erty.    def pho
+000042c0: 6e6f 6e5f 7375 7065 7263 656c 6c5f 6d61  non_supercell_ma
+000042d0: 7472 6978 2873 656c 6629 3a0a 2020 2020  trix(self):.    
+000042e0: 2020 2020 2222 2252 6574 7572 6e20 7472      """Return tr
+000042f0: 616e 7366 6f72 6d61 7469 6f6e 206d 6174  ansformation mat
+00004300: 7269 7820 746f 2070 686f 6e6f 6e20 7375  rix to phonon su
+00004310: 7065 7263 656c 6c20 6672 6f6d 2075 6e69  percell from uni
+00004320: 7420 6365 6c6c 2e0a 0a20 2020 2020 2020  t cell...       
+00004330: 206e 6461 7272 6179 0a20 2020 2020 2020   ndarray.       
+00004340: 2020 2020 2053 7570 6572 6365 6c6c 206d       Supercell m
+00004350: 6174 7269 7820 7769 7468 2072 6573 7065  atrix with respe
+00004360: 6374 2074 6f20 756e 6974 2063 656c 6c2e  ct to unit cell.
+00004370: 0a20 2020 2020 2020 2020 2020 2073 6861  .            sha
+00004380: 7065 3d28 332c 2033 292c 2064 7479 7065  pe=(3, 3), dtype
+00004390: 3d27 696e 745f 272c 206f 7264 6572 3d27  ='int_', order='
+000043a0: 4327 0a0a 2020 2020 2020 2020 2222 220a  C'..        """.
+000043b0: 2020 2020 2020 2020 7265 7475 726e 2073          return s
+000043c0: 656c 662e 5f70 686f 6e6f 6e5f 7375 7065  elf._phonon_supe
+000043d0: 7263 656c 6c5f 6d61 7472 6978 0a0a 2020  rcell_matrix..  
+000043e0: 2020 4070 726f 7065 7274 790a 2020 2020    @property.    
+000043f0: 6465 6620 7072 696d 6974 6976 655f 6d61  def primitive_ma
+00004400: 7472 6978 2873 656c 6629 3a0a 2020 2020  trix(self):.    
+00004410: 2020 2020 2222 2252 6574 7572 6e20 7472      """Return tr
+00004420: 616e 7366 6f72 6d61 7469 6f6e 206d 6174  ansformation mat
+00004430: 7269 7820 746f 2070 7269 6d69 7469 7665  rix to primitive
+00004440: 2063 656c 6c20 6672 6f6d 2075 6e69 7420   cell from unit 
+00004450: 6365 6c6c 2e0a 0a20 2020 2020 2020 206e  cell...        n
+00004460: 6461 7272 6179 0a20 2020 2020 2020 2020  darray.         
+00004470: 2020 2050 7269 6d69 7469 7665 206d 6174     Primitive mat
+00004480: 7269 7820 7769 7468 2072 6573 7065 6374  rix with respect
+00004490: 2074 6f20 756e 6974 2063 656c 6c2e 0a20   to unit cell.. 
+000044a0: 2020 2020 2020 2020 2020 2073 6861 7065             shape
+000044b0: 3d28 332c 2033 292c 2064 7479 7065 3d27  =(3, 3), dtype='
+000044c0: 646f 7562 6c65 272c 206f 7264 6572 3d27  double', order='
+000044d0: 4327 0a0a 2020 2020 2020 2020 2222 220a  C'..        """.
+000044e0: 2020 2020 2020 2020 7265 7475 726e 2073          return s
+000044f0: 656c 662e 5f70 7269 6d69 7469 7665 5f6d  elf._primitive_m
+00004500: 6174 7269 780a 0a20 2020 2040 7072 6f70  atrix..    @prop
+00004510: 6572 7479 0a20 2020 2064 6566 2075 6e69  erty.    def uni
+00004520: 745f 636f 6e76 6572 7369 6f6e 5f66 6163  t_conversion_fac
+00004530: 746f 7228 7365 6c66 293a 0a20 2020 2020  tor(self):.     
+00004540: 2020 2022 2222 5265 7475 726e 2070 686f     """Return pho
+00004550: 6e6f 6e20 6672 6571 7565 6e63 7920 756e  non frequency un
+00004560: 6974 2063 6f6e 7665 7273 696f 6e20 6661  it conversion fa
+00004570: 6374 6f72 2e0a 0a20 2020 2020 2020 2066  ctor...        f
+00004580: 6c6f 6174 0a20 2020 2020 2020 2020 2020  loat.           
+00004590: 2050 686f 6e6f 6e20 6672 6571 7565 6e63   Phonon frequenc
+000045a0: 7920 756e 6974 2063 6f6e 7665 7273 696f  y unit conversio
+000045b0: 6e20 6661 6374 6f72 2e20 5468 6973 2066  n factor. This f
+000045c0: 6163 746f 720a 2020 2020 2020 2020 2020  actor.          
+000045d0: 2020 636f 6e76 6572 7473 2073 7172 7428    converts sqrt(
+000045e0: 3c66 6f72 6365 3e2f 3c64 6973 7461 6e63  <force>/<distanc
+000045f0: 653e 2f3c 414d 553e 292f 3270 692f 3165  e>/<AMU>)/2pi/1e
+00004600: 3132 2074 6f20 5448 7a0a 2020 2020 2020  12 to THz.      
+00004610: 2020 2020 2020 286f 7264 696e 6172 7920        (ordinary 
+00004620: 6672 6571 7565 6e63 7929 2e0a 0a20 2020  frequency)...   
+00004630: 2020 2020 2022 2222 0a20 2020 2020 2020       """.       
+00004640: 2072 6574 7572 6e20 7365 6c66 2e5f 6672   return self._fr
+00004650: 6571 7565 6e63 795f 6661 6374 6f72 5f74  equency_factor_t
+00004660: 6f5f 5448 7a0a 0a20 2020 2040 7072 6f70  o_THz..    @prop
+00004670: 6572 7479 0a20 2020 2064 6566 2064 6174  erty.    def dat
+00004680: 6173 6574 2873 656c 6629 3a0a 2020 2020  aset(self):.    
+00004690: 2020 2020 2222 2253 6574 7465 7220 616e      """Setter an
+000046a0: 6420 6765 7474 6572 206f 6620 6469 7370  d getter of disp
+000046b0: 6c61 6365 6d65 6e74 2d66 6f72 6365 2064  lacement-force d
+000046c0: 6174 6173 6574 2e0a 0a20 2020 2020 2020  ataset...       
+000046d0: 2064 6963 740a 2020 2020 2020 2020 2020   dict.          
+000046e0: 2020 4469 7370 6c61 6365 6d65 6e74 7320    Displacements 
+000046f0: 696e 2073 7570 6572 6365 6c6c 732e 2054  in supercells. T
+00004700: 6865 7265 2061 7265 2074 776f 2074 7970  here are two typ
+00004710: 6573 206f 6620 666f 726d 6174 732e 0a20  es of formats.. 
+00004720: 2020 2020 2020 2020 2020 2054 7970 6520             Type 
+00004730: 312e 2054 776f 2061 746f 6d69 6320 6469  1. Two atomic di
+00004740: 7370 6c61 6365 6d65 6e74 2069 6e20 6561  splacement in ea
+00004750: 6368 2073 7570 6572 6365 6c6c 3a0a 2020  ch supercell:.  
+00004760: 2020 2020 2020 2020 2020 2020 2020 7b27                {'
+00004770: 6e61 746f 6d27 3a20 6e75 6d62 6572 206f  natom': number o
+00004780: 6620 6174 6f6d 7320 696e 2073 7570 6572  f atoms in super
+00004790: 6365 6c6c 2c0a 2020 2020 2020 2020 2020  cell,.          
+000047a0: 2020 2020 2020 2027 6669 7273 745f 6174         'first_at
+000047b0: 6f6d 7327 3a20 5b0a 2020 2020 2020 2020  oms': [.        
+000047c0: 2020 2020 2020 2020 2020 207b 276e 756d             {'num
+000047d0: 6265 7227 3a20 6174 6f6d 2069 6e64 6578  ber': atom index
+000047e0: 206f 6620 6669 7273 7420 6469 7370 6c61   of first displa
+000047f0: 6365 6420 6174 6f6d 2c0a 2020 2020 2020  ced atom,.      
+00004800: 2020 2020 2020 2020 2020 2020 2020 2764                'd
+00004810: 6973 706c 6163 656d 656e 7427 3a20 6469  isplacement': di
+00004820: 7370 6c61 6365 6d65 6e74 2069 6e20 4361  splacement in Ca
+00004830: 7274 6573 6961 6e20 636f 6f72 6469 6e61  rtesian coordina
+00004840: 7465 732c 0a20 2020 2020 2020 2020 2020  tes,.           
+00004850: 2020 2020 2020 2020 2027 666f 7263 6573           'forces
+00004860: 273a 2066 6f72 6365 7320 6f6e 2061 746f  ': forces on ato
+00004870: 6d73 2069 6e20 7375 7065 7263 656c 6c2c  ms in supercell,
+00004880: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00004890: 2020 2020 2027 6964 273a 2064 6973 706c       'id': displ
+000048a0: 6163 656d 656e 7420 6964 2028 312c 2032  acement id (1, 2
+000048b0: 2c2e 2e2e 2c6e 5f66 6972 7374 5f61 746f  ,...,n_first_ato
+000048c0: 6d73 290a 2020 2020 2020 2020 2020 2020  ms).            
+000048d0: 2020 2020 2020 2020 2773 6563 6f6e 645f          'second_
+000048e0: 6174 6f6d 7327 3a20 5b0a 2020 2020 2020  atoms': [.      
+000048f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004900: 7b27 6e75 6d62 6572 273a 2061 746f 6d20  {'number': atom 
+00004910: 696e 6465 7820 6f66 2073 6563 6f6e 6420  index of second 
+00004920: 6469 7370 6c61 6365 6420 6174 6f6d 2c0a  displaced atom,.
+00004930: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004940: 2020 2020 2020 2027 6469 7370 6c61 6365         'displace
+00004950: 6d65 6e74 273a 2064 6973 706c 6163 656d  ment': displacem
+00004960: 656e 7420 696e 2043 6172 7465 7369 616e  ent in Cartesian
+00004970: 2063 6f6f 7264 696e 6174 6573 7d2c 0a20   coordinates},. 
+00004980: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004990: 2020 2020 2020 2766 6f72 6365 7327 3a20        'forces': 
+000049a0: 666f 7263 6573 206f 6e20 6174 6f6d 7320  forces on atoms 
+000049b0: 696e 2073 7570 6572 6365 6c6c 2c0a 2020  in supercell,.  
+000049c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000049d0: 2020 2020 2027 7375 7065 7263 656c 6c5f       'supercell_
+000049e0: 656e 6572 6779 273a 2065 6e65 7267 7920  energy': energy 
+000049f0: 6f66 2073 7570 6572 6365 6c6c 2c0a 2020  of supercell,.  
+00004a00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004a10: 2020 2020 2027 7061 6972 5f64 6973 7461       'pair_dista
+00004a20: 6e63 6527 3a20 6469 7374 616e 6365 2062  nce': distance b
+00004a30: 6574 7765 656e 2070 6169 7265 6420 6174  etween paired at
+00004a40: 6f6d 732c 0a20 2020 2020 2020 2020 2020  oms,.           
+00004a50: 2020 2020 2020 2020 2020 2020 2769 6e63              'inc
+00004a60: 6c75 6465 6427 3a20 7769 7468 2063 7574  luded': with cut
+00004a70: 6f66 6620 7061 6972 2064 6973 7461 6e63  off pair distanc
+00004a80: 6520 696e 2064 6973 706c 6163 656d 656e  e in displacemen
+00004a90: 740a 2020 2020 2020 2020 2020 2020 2020  t.              
+00004aa0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004ab0: 2020 2020 2070 6169 7220 6765 6e65 7261       pair genera
+00004ac0: 7469 6f6e 2c20 7468 6973 2069 6e64 6963  tion, this indic
+00004ad0: 6174 6573 2069 6620 7468 6973 0a20 2020  ates if this.   
 00004ae0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004af0: 2020 2020 2020 2020 6663 3320 6f72 206e          fc3 or n
-00004b00: 6f74 2c0a 2020 2020 2020 2020 2020 2020  ot,.            
-00004b10: 2020 2020 2020 2020 2020 2027 6964 273a             'id':
-00004b20: 2064 6973 706c 6163 656d 656e 7420 6964   displacement id
-00004b30: 2e20 286e 5f66 6972 7374 5f61 746f 6d73  . (n_first_atoms
-00004b40: 202b 2031 2c20 2e2e 2e29 0a20 2020 2020   + 1, ...).     
-00004b50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004b60: 202e 2e2e 205d 207d 2c20 2e2e 2e20 5d20   ... ] }, ... ] 
-00004b70: 7d0a 2020 2020 2020 2020 2020 2020 5479  }.            Ty
-00004b80: 7065 2032 2e20 416c 6c20 6174 6f6d 6963  pe 2. All atomic
-00004b90: 2064 6973 706c 6163 656d 656e 7473 2069   displacements i
-00004ba0: 6e20 6561 6368 2073 7570 6572 6365 6c6c  n each supercell
-00004bb0: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-00004bc0: 2020 7b27 6469 7370 6c61 6365 6d65 6e74    {'displacement
-00004bd0: 7327 3a20 6e64 6172 7261 792c 2064 7479  s': ndarray, dty
-00004be0: 7065 3d27 646f 7562 6c65 272c 206f 7264  pe='double', ord
-00004bf0: 6572 3d27 4327 2c0a 2020 2020 2020 2020  er='C',.        
-00004c00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004c10: 2020 2020 2020 2020 2020 7368 6170 653d            shape=
-00004c20: 2873 7570 6572 6365 6c6c 732c 2061 746f  (supercells, ato
-00004c30: 6d73 2069 6e20 7375 7065 7263 656c 6c2c  ms in supercell,
-00004c40: 2033 290a 2020 2020 2020 2020 2020 2020   3).            
-00004c50: 2020 2020 2027 666f 7263 6573 273a 206e       'forces': n
-00004c60: 6461 7272 6179 2c20 6474 7970 653d 2764  darray, dtype='d
-00004c70: 6f75 626c 6527 2c2c 206f 7264 6572 3d27  ouble',, order='
-00004c80: 4327 2c0a 2020 2020 2020 2020 2020 2020  C',.            
-00004c90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004ca0: 2020 2020 2020 7368 6170 653d 2873 7570        shape=(sup
-00004cb0: 6572 6365 6c6c 732c 2061 746f 6d73 2069  ercells, atoms i
-00004cc0: 6e20 7375 7065 7263 656c 6c2c 2033 297d  n supercell, 3)}
-00004cd0: 0a20 2020 2020 2020 2020 2020 2049 6e20  .            In 
-00004ce0: 7479 7065 2032 2c20 6469 7370 6c61 6365  type 2, displace
-00004cf0: 6d65 6e74 7320 616e 6420 666f 7263 6573  ments and forces
-00004d00: 2063 616e 2062 6520 6769 7665 6e20 6279   can be given by
-00004d10: 206e 756d 7079 2061 7272 6179 0a20 2020   numpy array.   
-00004d20: 2020 2020 2020 2020 2077 6974 6820 6469           with di
-00004d30: 6666 6572 656e 7420 7368 6170 6520 6275  fferent shape bu
-00004d40: 7420 7468 6174 2063 616e 2062 6520 7265  t that can be re
-00004d50: 7368 6170 6564 2074 6f0a 2020 2020 2020  shaped to.      
-00004d60: 2020 2020 2020 2873 7570 6572 6365 6c6c        (supercell
-00004d70: 732c 206e 6174 6f6d 2c20 3329 2e0a 0a20  s, natom, 3)... 
-00004d80: 2020 2020 2020 2020 2020 2049 6e20 6164             In ad
-00004d90: 6469 7469 6f6e 2c20 2764 7570 6c69 6361  dition, 'duplica
-00004da0: 7465 7327 2061 6e64 2027 6375 746f 6666  tes' and 'cutoff
-00004db0: 5f64 6973 7461 6e63 6527 2063 616e 2065  _distance' can e
-00004dc0: 7869 7374 2069 6e20 7468 6973 0a20 2020  xist in this.   
-00004dd0: 2020 2020 2020 2020 2064 6174 6173 6574           dataset
-00004de0: 2069 6e20 6469 7370 6c61 6365 6d65 6e74   in displacement
-00004df0: 2070 6169 7220 6765 6e65 7261 7469 6f6e   pair generation
-00004e00: 2e20 2764 7570 6c69 6361 7465 7327 2067  . 'duplicates' g
-00004e10: 6976 6573 0a20 2020 2020 2020 2020 2020  ives.           
-00004e20: 2064 7570 6c69 6361 7465 6420 7375 7065   duplicated supe
-00004e30: 7263 656c 6c20 6964 7320 6173 2070 6169  rcell ids as pai
-00004e40: 7273 2e0a 0a20 2020 2020 2020 2022 2222  rs...        """
-00004e50: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
-00004e60: 7365 6c66 2e5f 6461 7461 7365 740a 0a20  self._dataset.. 
-00004e70: 2020 2040 6461 7461 7365 742e 7365 7474     @dataset.sett
-00004e80: 6572 0a20 2020 2064 6566 2064 6174 6173  er.    def datas
-00004e90: 6574 2873 656c 662c 2064 6174 6173 6574  et(self, dataset
-00004ea0: 293a 0a20 2020 2020 2020 2073 656c 662e  ):.        self.
-00004eb0: 5f64 6174 6173 6574 203d 2064 6174 6173  _dataset = datas
-00004ec0: 6574 0a20 2020 2020 2020 2073 656c 662e  et.        self.
-00004ed0: 5f73 7570 6572 6365 6c6c 735f 7769 7468  _supercells_with
-00004ee0: 5f64 6973 706c 6163 656d 656e 7473 203d  _displacements =
-00004ef0: 204e 6f6e 650a 2020 2020 2020 2020 7365   None.        se
-00004f00: 6c66 2e5f 7068 6f6e 6f6e 5f73 7570 6572  lf._phonon_super
-00004f10: 6365 6c6c 735f 7769 7468 5f64 6973 706c  cells_with_displ
-00004f20: 6163 656d 656e 7473 203d 204e 6f6e 650a  acements = None.
-00004f30: 0a20 2020 2040 7072 6f70 6572 7479 0a20  .    @property. 
-00004f40: 2020 2064 6566 2070 686f 6e6f 6e5f 6461     def phonon_da
-00004f50: 7461 7365 7428 7365 6c66 293a 0a20 2020  taset(self):.   
-00004f60: 2020 2020 2022 2222 5365 7474 6572 2061       """Setter a
-00004f70: 6e64 2067 6574 7465 7220 6f66 2064 6973  nd getter of dis
-00004f80: 706c 6163 656d 656e 742d 666f 7263 6520  placement-force 
-00004f90: 6461 7461 7365 7420 666f 7220 6663 322e  dataset for fc2.
-00004fa0: 0a0a 2020 2020 2020 2020 6469 6374 0a20  ..        dict. 
-00004fb0: 2020 2020 2020 2020 2020 2044 6973 706c             Displ
-00004fc0: 6163 656d 656e 7473 2069 6e20 7375 7065  acements in supe
-00004fd0: 7263 656c 6c73 2e20 5468 6572 6520 6172  rcells. There ar
-00004fe0: 6520 7477 6f20 7479 7065 7320 6f66 2066  e two types of f
-00004ff0: 6f72 6d61 7473 2e0a 2020 2020 2020 2020  ormats..        
-00005000: 2020 2020 5479 7065 2031 2e20 5477 6f20      Type 1. Two 
-00005010: 6174 6f6d 6963 2064 6973 706c 6163 656d  atomic displacem
-00005020: 656e 7420 696e 2065 6163 6820 7375 7065  ent in each supe
-00005030: 7263 656c 6c3a 0a20 2020 2020 2020 2020  rcell:.         
-00005040: 2020 2020 2020 207b 276e 6174 6f6d 273a         {'natom':
-00005050: 206e 756d 6265 7220 6f66 2061 746f 6d73   number of atoms
-00005060: 2069 6e20 7375 7065 7263 656c 6c2c 0a20   in supercell,. 
-00005070: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005080: 2766 6972 7374 5f61 746f 6d73 273a 205b  'first_atoms': [
-00005090: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000050a0: 2020 2020 7b27 6e75 6d62 6572 273a 2061      {'number': a
-000050b0: 746f 6d20 696e 6465 7820 6f66 2066 6972  tom index of fir
-000050c0: 7374 2064 6973 706c 6163 6564 2061 746f  st displaced ato
-000050d0: 6d2c 0a20 2020 2020 2020 2020 2020 2020  m,.             
-000050e0: 2020 2020 2020 2027 6469 7370 6c61 6365         'displace
-000050f0: 6d65 6e74 273a 2064 6973 706c 6163 656d  ment': displacem
-00005100: 656e 7420 696e 2043 6172 7465 7369 616e  ent in Cartesian
-00005110: 2063 6f6f 7264 696e 6174 6573 2c0a 2020   coordinates,.  
-00005120: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005130: 2020 2766 6f72 6365 7327 3a20 666f 7263    'forces': forc
-00005140: 6573 206f 6e20 6174 6f6d 7320 696e 2073  es on atoms in s
-00005150: 7570 6572 6365 6c6c 7d20 2e2e 2e20 5d7d  upercell} ... ]}
-00005160: 0a20 2020 2020 2020 2020 2020 2054 7970  .            Typ
-00005170: 6520 322e 2041 6c6c 2061 746f 6d69 6320  e 2. All atomic 
-00005180: 6469 7370 6c61 6365 6d65 6e74 7320 696e  displacements in
-00005190: 2065 6163 6820 7375 7065 7263 656c 6c3a   each supercell:
-000051a0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000051b0: 207b 2764 6973 706c 6163 656d 656e 7473   {'displacements
-000051c0: 273a 206e 6461 7272 6179 2c20 6474 7970  ': ndarray, dtyp
-000051d0: 653d 2764 6f75 626c 6527 2c20 6f72 6465  e='double', orde
-000051e0: 723d 2743 272c 0a20 2020 2020 2020 2020  r='C',.         
-000051f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005200: 2020 2020 2020 2020 2073 6861 7065 3d28           shape=(
-00005210: 7375 7065 7263 656c 6c73 2c20 6174 6f6d  supercells, atom
-00005220: 7320 696e 2073 7570 6572 6365 6c6c 2c20  s in supercell, 
-00005230: 3329 0a20 2020 2020 2020 2020 2020 2020  3).             
-00005240: 2020 2020 2766 6f72 6365 7327 3a20 6e64      'forces': nd
-00005250: 6172 7261 792c 2064 7479 7065 3d27 646f  array, dtype='do
-00005260: 7562 6c65 272c 2c20 6f72 6465 723d 2743  uble',, order='C
-00005270: 272c 0a20 2020 2020 2020 2020 2020 2020  ',.             
-00005280: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005290: 2020 2020 2073 6861 7065 3d28 7375 7065       shape=(supe
-000052a0: 7263 656c 6c73 2c20 6174 6f6d 7320 696e  rcells, atoms in
-000052b0: 2073 7570 6572 6365 6c6c 2c20 3329 7d0a   supercell, 3)}.
-000052c0: 2020 2020 2020 2020 2020 2020 496e 2074              In t
-000052d0: 7970 6520 322c 2064 6973 706c 6163 656d  ype 2, displacem
-000052e0: 656e 7473 2061 6e64 2066 6f72 6365 7320  ents and forces 
-000052f0: 6361 6e20 6265 2067 6976 656e 2062 7920  can be given by 
-00005300: 6e75 6d70 7920 6172 7261 790a 2020 2020  numpy array.    
-00005310: 2020 2020 2020 2020 7769 7468 2064 6966          with dif
-00005320: 6665 7265 6e74 2073 6861 7065 2062 7574  ferent shape but
-00005330: 2074 6861 7420 6361 6e20 6265 2072 6573   that can be res
-00005340: 6861 7065 6420 746f 0a20 2020 2020 2020  haped to.       
-00005350: 2020 2020 2028 7375 7065 7263 656c 6c73       (supercells
-00005360: 2c20 6e61 746f 6d2c 2033 292e 0a0a 2020  , natom, 3)...  
-00005370: 2020 2020 2020 2222 220a 2020 2020 2020        """.      
-00005380: 2020 7265 7475 726e 2073 656c 662e 5f70    return self._p
-00005390: 686f 6e6f 6e5f 6461 7461 7365 740a 0a20  honon_dataset.. 
-000053a0: 2020 2040 7068 6f6e 6f6e 5f64 6174 6173     @phonon_datas
-000053b0: 6574 2e73 6574 7465 720a 2020 2020 6465  et.setter.    de
-000053c0: 6620 7068 6f6e 6f6e 5f64 6174 6173 6574  f phonon_dataset
-000053d0: 2873 656c 662c 2064 6174 6173 6574 293a  (self, dataset):
-000053e0: 0a20 2020 2020 2020 2073 656c 662e 5f70  .        self._p
-000053f0: 686f 6e6f 6e5f 6461 7461 7365 7420 3d20  honon_dataset = 
-00005400: 6461 7461 7365 740a 0a20 2020 2040 7072  dataset..    @pr
-00005410: 6f70 6572 7479 0a20 2020 2064 6566 2062  operty.    def b
-00005420: 616e 645f 696e 6469 6365 7328 7365 6c66  and_indices(self
-00005430: 293a 0a20 2020 2020 2020 2022 2222 5365  ):.        """Se
-00005440: 7474 6572 2061 6e64 2067 6574 7465 7220  tter and getter 
-00005450: 6f66 2062 616e 6420 696e 6469 6365 732e  of band indices.
-00005460: 0a0a 2020 2020 2020 2020 6172 7261 795f  ..        array_
-00005470: 6c69 6b65 0a20 2020 2020 2020 2020 2020  like.           
-00005480: 204c 6973 7420 6f66 2062 616e 6420 696e   List of band in
-00005490: 6469 6365 7320 7370 6563 6966 6965 6420  dices specified 
-000054a0: 746f 2073 656c 6563 7420 7370 6563 6966  to select specif
-000054b0: 6963 2062 616e 6473 0a20 2020 2020 2020  ic bands.       
-000054c0: 2020 2020 2074 6f20 636f 6d70 7574 6572       to computer
-000054d0: 2070 682d 7068 2069 6e74 6572 6163 7469   ph-ph interacti
-000054e0: 6f6e 2072 656c 6174 6564 2070 726f 7065  on related prope
-000054f0: 7274 6965 732e 0a0a 2020 2020 2020 2020  rties...        
-00005500: 2222 220a 2020 2020 2020 2020 7265 7475  """.        retu
-00005510: 726e 2073 656c 662e 5f62 616e 645f 696e  rn self._band_in
-00005520: 6469 6365 730a 0a20 2020 2040 6261 6e64  dices..    @band
-00005530: 5f69 6e64 6963 6573 2e73 6574 7465 720a  _indices.setter.
-00005540: 2020 2020 6465 6620 6261 6e64 5f69 6e64      def band_ind
-00005550: 6963 6573 2873 656c 662c 2062 616e 645f  ices(self, band_
-00005560: 696e 6469 6365 7329 3a0a 2020 2020 2020  indices):.      
-00005570: 2020 7365 6c66 2e5f 7365 745f 6261 6e64    self._set_band
-00005580: 5f69 6e64 6963 6573 2862 616e 645f 696e  _indices(band_in
-00005590: 6469 6365 733d 6261 6e64 5f69 6e64 6963  dices=band_indic
-000055a0: 6573 290a 0a20 2020 2064 6566 205f 7365  es)..    def _se
-000055b0: 745f 6261 6e64 5f69 6e64 6963 6573 2873  t_band_indices(s
-000055c0: 656c 662c 2062 616e 645f 696e 6469 6365  elf, band_indice
-000055d0: 733d 4e6f 6e65 293a 0a20 2020 2020 2020  s=None):.       
-000055e0: 2069 6620 6261 6e64 5f69 6e64 6963 6573   if band_indices
-000055f0: 2069 7320 4e6f 6e65 3a0a 2020 2020 2020   is None:.      
-00005600: 2020 2020 2020 6e75 6d5f 6261 6e64 203d        num_band =
-00005610: 206c 656e 2873 656c 662e 5f70 7269 6d69   len(self._primi
-00005620: 7469 7665 2920 2a20 330a 2020 2020 2020  tive) * 3.      
-00005630: 2020 2020 2020 7365 6c66 2e5f 6261 6e64        self._band
-00005640: 5f69 6e64 6963 6573 203d 205b 6e70 2e61  _indices = [np.a
-00005650: 7261 6e67 6528 6e75 6d5f 6261 6e64 2c20  range(num_band, 
-00005660: 6474 7970 653d 2269 6e74 5f22 295d 0a20  dtype="int_")]. 
-00005670: 2020 2020 2020 2065 6c73 653a 0a20 2020         else:.   
-00005680: 2020 2020 2020 2020 2073 656c 662e 5f62           self._b
-00005690: 616e 645f 696e 6469 6365 7320 3d20 6261  and_indices = ba
-000056a0: 6e64 5f69 6e64 6963 6573 0a20 2020 2020  nd_indices.     
-000056b0: 2020 2073 656c 662e 5f62 616e 645f 696e     self._band_in
-000056c0: 6469 6365 735f 666c 6174 7465 6e20 3d20  dices_flatten = 
-000056d0: 6e70 2e68 7374 6163 6b28 7365 6c66 2e5f  np.hstack(self._
-000056e0: 6261 6e64 5f69 6e64 6963 6573 292e 6173  band_indices).as
-000056f0: 7479 7065 2822 696e 745f 2229 0a0a 2020  type("int_")..  
-00005700: 2020 4070 726f 7065 7274 790a 2020 2020    @property.    
-00005710: 6465 6620 6d61 7373 6573 2873 656c 6629  def masses(self)
-00005720: 3a0a 2020 2020 2020 2020 2222 2253 6574  :.        """Set
-00005730: 7465 7220 616e 6420 6765 7474 6572 206f  ter and getter o
-00005740: 6620 6174 6f6d 6963 206d 6173 7365 7320  f atomic masses 
-00005750: 6f66 2070 7269 6d69 7469 7665 2063 656c  of primitive cel
-00005760: 6c2e 2222 220a 2020 2020 2020 2020 7265  l.""".        re
-00005770: 7475 726e 2073 656c 662e 5f70 7269 6d69  turn self._primi
-00005780: 7469 7665 2e6d 6173 7365 730a 0a20 2020  tive.masses..   
-00005790: 2040 6d61 7373 6573 2e73 6574 7465 720a   @masses.setter.
-000057a0: 2020 2020 6465 6620 6d61 7373 6573 2873      def masses(s
-000057b0: 656c 662c 206d 6173 7365 7329 3a0a 2020  elf, masses):.  
-000057c0: 2020 2020 2020 6966 206d 6173 7365 7320        if masses 
-000057d0: 6973 204e 6f6e 653a 0a20 2020 2020 2020  is None:.       
-000057e0: 2020 2020 2072 6574 7572 6e0a 2020 2020       return.    
-000057f0: 2020 2020 705f 6d61 7373 6573 203d 206e      p_masses = n
-00005800: 702e 6172 7261 7928 6d61 7373 6573 290a  p.array(masses).
-00005810: 2020 2020 2020 2020 7365 6c66 2e5f 7072          self._pr
-00005820: 696d 6974 6976 652e 6d61 7373 6573 203d  imitive.masses =
-00005830: 2070 5f6d 6173 7365 730a 2020 2020 2020   p_masses.      
-00005840: 2020 7032 705f 6d61 7020 3d20 7365 6c66    p2p_map = self
-00005850: 2e5f 7072 696d 6974 6976 652e 7032 705f  ._primitive.p2p_
-00005860: 6d61 700a 2020 2020 2020 2020 735f 6d61  map.        s_ma
-00005870: 7373 6573 203d 2070 5f6d 6173 7365 735b  sses = p_masses[
-00005880: 5b70 3270 5f6d 6170 5b78 5d20 666f 7220  [p2p_map[x] for 
-00005890: 7820 696e 2073 656c 662e 5f70 7269 6d69  x in self._primi
-000058a0: 7469 7665 2e73 3270 5f6d 6170 5d5d 0a20  tive.s2p_map]]. 
-000058b0: 2020 2020 2020 2073 656c 662e 5f73 7570         self._sup
-000058c0: 6572 6365 6c6c 2e6d 6173 7365 7320 3d20  ercell.masses = 
-000058d0: 735f 6d61 7373 6573 0a20 2020 2020 2020  s_masses.       
-000058e0: 2075 3273 5f6d 6170 203d 2073 656c 662e   u2s_map = self.
-000058f0: 5f73 7570 6572 6365 6c6c 2e75 3273 5f6d  _supercell.u2s_m
-00005900: 6170 0a20 2020 2020 2020 2075 5f6d 6173  ap.        u_mas
-00005910: 7365 7320 3d20 735f 6d61 7373 6573 5b75  ses = s_masses[u
-00005920: 3273 5f6d 6170 5d0a 2020 2020 2020 2020  2s_map].        
-00005930: 7365 6c66 2e5f 756e 6974 6365 6c6c 2e6d  self._unitcell.m
-00005940: 6173 7365 7320 3d20 755f 6d61 7373 6573  asses = u_masses
-00005950: 0a20 2020 2020 2020 2073 656c 662e 5f70  .        self._p
-00005960: 686f 6e6f 6e5f 7072 696d 6974 6976 652e  honon_primitive.
-00005970: 6d61 7373 6573 203d 2070 5f6d 6173 7365  masses = p_masse
-00005980: 730a 2020 2020 2020 2020 7032 705f 6d61  s.        p2p_ma
-00005990: 7020 3d20 7365 6c66 2e5f 7068 6f6e 6f6e  p = self._phonon
-000059a0: 5f70 7269 6d69 7469 7665 2e70 3270 5f6d  _primitive.p2p_m
-000059b0: 6170 0a20 2020 2020 2020 2073 5f6d 6173  ap.        s_mas
-000059c0: 7365 7320 3d20 705f 6d61 7373 6573 5b5b  ses = p_masses[[
-000059d0: 7032 705f 6d61 705b 785d 2066 6f72 2078  p2p_map[x] for x
-000059e0: 2069 6e20 7365 6c66 2e5f 7068 6f6e 6f6e   in self._phonon
-000059f0: 5f70 7269 6d69 7469 7665 2e73 3270 5f6d  _primitive.s2p_m
-00005a00: 6170 5d5d 0a20 2020 2020 2020 2073 656c  ap]].        sel
-00005a10: 662e 5f70 686f 6e6f 6e5f 7375 7065 7263  f._phonon_superc
-00005a20: 656c 6c2e 6d61 7373 6573 203d 2073 5f6d  ell.masses = s_m
-00005a30: 6173 7365 730a 0a20 2020 2040 7072 6f70  asses..    @prop
-00005a40: 6572 7479 0a20 2020 2064 6566 2073 7570  erty.    def sup
-00005a50: 6572 6365 6c6c 735f 7769 7468 5f64 6973  ercells_with_dis
-00005a60: 706c 6163 656d 656e 7473 2873 656c 6629  placements(self)
-00005a70: 3a0a 2020 2020 2020 2020 2222 2252 6574  :.        """Ret
-00005a80: 7572 6e20 7375 7065 7263 656c 6c73 2077  urn supercells w
-00005a90: 6974 6820 6469 7370 6c61 6365 6d65 6e74  ith displacement
-00005aa0: 732e 0a0a 2020 2020 2020 2020 6c69 7374  s...        list
-00005ab0: 206f 6620 5068 6f6e 6f70 7941 746f 6d73   of PhonopyAtoms
-00005ac0: 0a20 2020 2020 2020 2020 2020 2053 7570  .            Sup
-00005ad0: 6572 6365 6c6c 7320 7769 7468 2064 6973  ercells with dis
-00005ae0: 706c 6163 656d 656e 7473 2067 656e 6572  placements gener
-00005af0: 6174 6564 2062 790a 2020 2020 2020 2020  ated by.        
-00005b00: 2020 2020 5068 6f6e 6f33 7079 2e67 656e      Phono3py.gen
-00005b10: 6572 6174 655f 6469 7370 6c61 6365 6d65  erate_displaceme
-00005b20: 6e74 732e 0a0a 2020 2020 2020 2020 2222  nts...        ""
-00005b30: 220a 2020 2020 2020 2020 6966 2073 656c  ".        if sel
-00005b40: 662e 5f73 7570 6572 6365 6c6c 735f 7769  f._supercells_wi
-00005b50: 7468 5f64 6973 706c 6163 656d 656e 7473  th_displacements
-00005b60: 2069 7320 4e6f 6e65 3a0a 2020 2020 2020   is None:.      
-00005b70: 2020 2020 2020 7365 6c66 2e5f 6275 696c        self._buil
-00005b80: 645f 7375 7065 7263 656c 6c73 5f77 6974  d_supercells_wit
-00005b90: 685f 6469 7370 6c61 6365 6d65 6e74 7328  h_displacements(
-00005ba0: 290a 2020 2020 2020 2020 7265 7475 726e  ).        return
-00005bb0: 2073 656c 662e 5f73 7570 6572 6365 6c6c   self._supercell
-00005bc0: 735f 7769 7468 5f64 6973 706c 6163 656d  s_with_displacem
-00005bd0: 656e 7473 0a0a 2020 2020 4070 726f 7065  ents..    @prope
-00005be0: 7274 790a 2020 2020 6465 6620 7068 6f6e  rty.    def phon
-00005bf0: 6f6e 5f73 7570 6572 6365 6c6c 735f 7769  on_supercells_wi
-00005c00: 7468 5f64 6973 706c 6163 656d 656e 7473  th_displacements
-00005c10: 2873 656c 6629 3a0a 2020 2020 2020 2020  (self):.        
-00005c20: 2222 2252 6574 7572 6e20 7375 7065 7263  """Return superc
-00005c30: 656c 6c73 2077 6974 6820 6469 7370 6c61  ells with displa
-00005c40: 6365 6d65 6e74 7320 666f 7220 6663 322e  cements for fc2.
-00005c50: 0a0a 2020 2020 2020 2020 6c69 7374 206f  ..        list o
-00005c60: 6620 5068 6f6e 6f70 7941 746f 6d73 0a20  f PhonopyAtoms. 
-00005c70: 2020 2020 2020 2020 2020 2053 7570 6572             Super
-00005c80: 6365 6c6c 7320 7769 7468 2064 6973 706c  cells with displ
-00005c90: 6163 656d 656e 7473 2067 656e 6572 6174  acements generat
-00005ca0: 6564 2062 790a 2020 2020 2020 2020 2020  ed by.          
-00005cb0: 2020 5068 6f6e 6f33 7079 2e67 656e 6572    Phono3py.gener
-00005cc0: 6174 655f 6469 7370 6c61 6365 6d65 6e74  ate_displacement
-00005cd0: 732e 0a0a 2020 2020 2020 2020 2222 220a  s...        """.
-00005ce0: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
-00005cf0: 5f70 686f 6e6f 6e5f 7375 7065 7263 656c  _phonon_supercel
-00005d00: 6c73 5f77 6974 685f 6469 7370 6c61 6365  ls_with_displace
-00005d10: 6d65 6e74 7320 6973 204e 6f6e 653a 0a20  ments is None:. 
-00005d20: 2020 2020 2020 2020 2020 2069 6620 7365             if se
-00005d30: 6c66 2e5f 7068 6f6e 6f6e 5f64 6174 6173  lf._phonon_datas
-00005d40: 6574 2069 7320 6e6f 7420 4e6f 6e65 3a0a  et is not None:.
-00005d50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005d60: 7365 6c66 2e5f 7068 6f6e 6f6e 5f73 7570  self._phonon_sup
-00005d70: 6572 6365 6c6c 735f 7769 7468 5f64 6973  ercells_with_dis
-00005d80: 706c 6163 656d 656e 7473 203d 2028 0a20  placements = (. 
-00005d90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005da0: 2020 2073 656c 662e 5f62 7569 6c64 5f70     self._build_p
-00005db0: 686f 6e6f 6e5f 7375 7065 7263 656c 6c73  honon_supercells
-00005dc0: 5f77 6974 685f 6469 7370 6c61 6365 6d65  _with_displaceme
-00005dd0: 6e74 7328 0a20 2020 2020 2020 2020 2020  nts(.           
-00005de0: 2020 2020 2020 2020 2020 2020 2073 656c               sel
-00005df0: 662e 5f70 686f 6e6f 6e5f 7375 7065 7263  f._phonon_superc
-00005e00: 656c 6c2c 2073 656c 662e 5f70 686f 6e6f  ell, self._phono
-00005e10: 6e5f 6461 7461 7365 740a 2020 2020 2020  n_dataset.      
-00005e20: 2020 2020 2020 2020 2020 2020 2020 290a                ).
-00005e30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005e40: 290a 2020 2020 2020 2020 7265 7475 726e  ).        return
-00005e50: 2073 656c 662e 5f70 686f 6e6f 6e5f 7375   self._phonon_su
-00005e60: 7065 7263 656c 6c73 5f77 6974 685f 6469  percells_with_di
-00005e70: 7370 6c61 6365 6d65 6e74 730a 0a20 2020  splacements..   
-00005e80: 2040 7072 6f70 6572 7479 0a20 2020 2064   @property.    d
-00005e90: 6566 206d 6573 685f 6e75 6d62 6572 7328  ef mesh_numbers(
-00005ea0: 7365 6c66 293a 0a20 2020 2020 2020 2022  self):.        "
-00005eb0: 2222 5365 7474 6572 2061 6e64 2067 6574  ""Setter and get
-00005ec0: 7465 7220 6f66 2073 616d 706c 696e 6720  ter of sampling 
-00005ed0: 6d65 7368 206e 756d 6265 7273 2069 6e20  mesh numbers in 
-00005ee0: 7265 6369 7072 6f63 616c 2073 7061 6365  reciprocal space
-00005ef0: 2e22 2222 0a20 2020 2020 2020 2069 6620  .""".        if 
-00005f00: 7365 6c66 2e5f 627a 5f67 7269 6420 6973  self._bz_grid is
-00005f10: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
-00005f20: 2020 2072 6574 7572 6e20 4e6f 6e65 0a20     return None. 
-00005f30: 2020 2020 2020 2065 6c73 653a 0a20 2020         else:.   
-00005f40: 2020 2020 2020 2020 2072 6574 7572 6e20           return 
-00005f50: 7365 6c66 2e5f 627a 5f67 7269 642e 445f  self._bz_grid.D_
-00005f60: 6469 6167 0a0a 2020 2020 406d 6573 685f  diag..    @mesh_
-00005f70: 6e75 6d62 6572 732e 7365 7474 6572 0a20  numbers.setter. 
-00005f80: 2020 2064 6566 206d 6573 685f 6e75 6d62     def mesh_numb
-00005f90: 6572 7328 7365 6c66 2c20 6d65 7368 5f6e  ers(self, mesh_n
-00005fa0: 756d 6265 7273 3a20 556e 696f 6e5b 696e  umbers: Union[in
-00005fb0: 742c 2066 6c6f 6174 2c20 5365 7175 656e  t, float, Sequen
-00005fc0: 6365 2c20 6e70 2e6e 6461 7272 6179 5d29  ce, np.ndarray])
-00005fd0: 3a0a 2020 2020 2020 2020 7365 6c66 2e5f  :.        self._
-00005fe0: 7365 745f 6d65 7368 5f6e 756d 6265 7273  set_mesh_numbers
-00005ff0: 286d 6573 685f 6e75 6d62 6572 7329 0a0a  (mesh_numbers)..
-00006000: 2020 2020 4070 726f 7065 7274 790a 2020      @property.  
-00006010: 2020 6465 6620 7468 6572 6d61 6c5f 636f    def thermal_co
-00006020: 6e64 7563 7469 7669 7479 2873 656c 6629  nductivity(self)
-00006030: 3a0a 2020 2020 2020 2020 2222 2252 6574  :.        """Ret
-00006040: 7572 6e20 7468 6572 6d61 6c20 636f 6e64  urn thermal cond
-00006050: 7563 7469 7669 7479 2063 6c61 7373 2069  uctivity class i
-00006060: 6e73 7461 6e63 652e 2222 220a 2020 2020  nstance.""".    
-00006070: 2020 2020 7265 7475 726e 2073 656c 662e      return self.
-00006080: 5f74 6865 726d 616c 5f63 6f6e 6475 6374  _thermal_conduct
-00006090: 6976 6974 790a 0a20 2020 2040 7072 6f70  ivity..    @prop
-000060a0: 6572 7479 0a20 2020 2064 6566 2064 6973  erty.    def dis
-000060b0: 706c 6163 656d 656e 7473 2873 656c 6629  placements(self)
-000060c0: 3a0a 2020 2020 2020 2020 2222 2253 6574  :.        """Set
-000060d0: 7465 7220 616e 6420 6765 7474 6572 2064  ter and getter d
-000060e0: 6973 706c 6163 656d 656e 7473 2069 6e20  isplacements in 
-000060f0: 7375 7065 7263 656c 6c73 2e0a 0a20 2020  supercells...   
-00006100: 2020 2020 2054 6865 7265 2061 7265 2074       There are t
-00006110: 776f 2074 7970 6573 206f 6620 6469 7370  wo types of disp
-00006120: 6c61 6365 6d65 6e74 2064 6174 6173 6574  lacement dataset
-00006130: 2e20 5365 6520 7468 6520 646f 6373 7472  . See the docstr
-00006140: 696e 670a 2020 2020 2020 2020 6f66 2064  ing.        of d
-00006150: 6174 6173 6574 2061 626f 7574 2074 7970  ataset about typ
-00006160: 6573 2031 2061 6e64 2032 2066 6f72 2074  es 1 and 2 for t
-00006170: 6865 2064 6973 706c 6163 656d 656e 7420  he displacement 
-00006180: 6461 7461 7365 7420 666f 726d 6174 732e  dataset formats.
-00006190: 0a20 2020 2020 2020 2044 6973 706c 6163  .        Displac
-000061a0: 656d 656e 7473 2073 6574 2072 6574 7572  ements set retur
-000061b0: 6e65 6420 6465 7065 6e64 7320 6f6e 2065  ned depends on e
-000061c0: 6974 6865 7220 7479 7065 2d31 206f 7220  ither type-1 or 
-000061d0: 7479 7065 2d32 2061 730a 2020 2020 2020  type-2 as.      
-000061e0: 2020 666f 6c6c 6f77 733a 0a0a 2020 2020    follows:..    
-000061f0: 2020 2020 5479 7065 2d31 2c20 4c69 7374      Type-1, List
-00006200: 206f 6620 6c69 7374 0a20 2020 2020 2020   of list.       
-00006210: 2020 2020 2054 6865 2069 6e74 6572 6e61       The interna
-00006220: 6c20 6c69 7374 2068 6173 2034 2065 6c65  l list has 4 ele
-00006230: 6d65 6e74 7320 7375 6368 2061 7320 5b33  ments such as [3
-00006240: 322c 2030 2e30 312c 2030 2e30 2c20 302e  2, 0.01, 0.0, 0.
-00006250: 305d 5d2e 0a20 2020 2020 2020 2020 2020  0]]..           
-00006260: 2054 6865 2066 6972 7374 2065 6c65 6d65   The first eleme
-00006270: 6e74 2069 7320 7468 6520 7375 7065 7263  nt is the superc
-00006280: 656c 6c20 6174 6f6d 2069 6e64 6578 2073  ell atom index s
-00006290: 7461 7274 696e 6720 7769 7468 2030 2e0a  tarting with 0..
-000062a0: 2020 2020 2020 2020 2020 2020 5468 6520              The 
-000062b0: 7265 6d61 696e 696e 6720 7468 7265 6520  remaining three 
-000062c0: 656c 656d 656e 7473 2067 6976 6520 7468  elements give th
-000062d0: 6520 6469 7370 6c61 6365 6d65 6e74 2069  e displacement i
-000062e0: 6e20 4361 7274 6573 6961 6e0a 2020 2020  n Cartesian.    
-000062f0: 2020 2020 2020 2020 636f 6f72 6469 6e61          coordina
-00006300: 7465 732e 0a20 2020 2020 2020 2054 7970  tes..        Typ
-00006310: 652d 322c 2061 7272 6179 5f6c 696b 650a  e-2, array_like.
-00006320: 2020 2020 2020 2020 2020 2020 4469 7370              Disp
-00006330: 6c61 6365 6d65 6e74 7320 6f66 2061 6c6c  lacements of all
-00006340: 2061 746f 6d73 206f 6620 616c 6c20 7375   atoms of all su
-00006350: 7065 7263 656c 6c73 2069 6e20 4361 7274  percells in Cart
-00006360: 6573 6961 6e0a 2020 2020 2020 2020 2020  esian.          
-00006370: 2020 636f 6f72 6469 6e61 7465 732e 0a20    coordinates.. 
-00006380: 2020 2020 2020 2020 2020 2073 6861 7065             shape
-00006390: 3d28 7375 7065 7263 656c 6c73 2c20 6e61  =(supercells, na
-000063a0: 746f 6d2c 2033 290a 2020 2020 2020 2020  tom, 3).        
-000063b0: 2020 2020 6474 7970 653d 2764 6f75 626c      dtype='doubl
-000063c0: 6527 0a0a 0a20 2020 2020 2020 2046 6f72  e'...        For
-000063d0: 2073 6574 7465 722c 206f 6e6c 7920 7479   setter, only ty
-000063e0: 7065 2d32 2064 6174 6173 6574 2066 6f72  pe-2 dataset for
-000063f0: 6d61 7420 6973 2061 6c6c 6f77 6564 2e0a  mat is allowed..
-00006400: 0a20 2020 2020 2020 2064 6973 706c 6163  .        displac
-00006410: 656d 656e 7473 203a 2061 7272 6179 5f6c  ements : array_l
-00006420: 696b 650a 2020 2020 2020 2020 2020 2020  ike.            
-00006430: 4174 6f6d 6963 2064 6973 706c 6163 656d  Atomic displacem
-00006440: 656e 7473 206f 6620 616c 6c20 6174 6f6d  ents of all atom
-00006450: 7320 6f66 2061 6c6c 2073 7570 6572 6365  s of all superce
-00006460: 6c6c 732e 0a20 2020 2020 2020 2020 2020  lls..           
-00006470: 204f 6e6c 7920 616c 6c20 6469 7370 6c61   Only all displa
-00006480: 6365 6d65 6e74 7320 696e 2065 6163 6820  cements in each 
-00006490: 7375 7065 7263 656c 6c20 6361 7365 2028  supercell case (
-000064a0: 7479 7065 2d32 2920 6973 0a20 2020 2020  type-2) is.     
-000064b0: 2020 2020 2020 2073 7570 706f 7274 6564         supported
-000064c0: 2e0a 2020 2020 2020 2020 2020 2020 7368  ..            sh
-000064d0: 6170 653d 2873 7570 6572 6365 6c6c 732c  ape=(supercells,
-000064e0: 206e 6174 6f6d 2c20 3329 2c20 6474 7970   natom, 3), dtyp
-000064f0: 653d 2764 6f75 626c 6527 2c20 6f72 6465  e='double', orde
-00006500: 723d 2743 270a 0a20 2020 2020 2020 2022  r='C'..        "
-00006510: 2222 0a20 2020 2020 2020 2064 6174 6173  "".        datas
-00006520: 6574 203d 2073 656c 662e 5f64 6174 6173  et = self._datas
-00006530: 6574 0a0a 2020 2020 2020 2020 6966 2022  et..        if "
-00006540: 6669 7273 745f 6174 6f6d 7322 2069 6e20  first_atoms" in 
-00006550: 6461 7461 7365 743a 0a20 2020 2020 2020  dataset:.       
-00006560: 2020 2020 206e 756d 5f73 6365 6c6c 7320       num_scells 
-00006570: 3d20 6c65 6e28 6461 7461 7365 745b 2266  = len(dataset["f
-00006580: 6972 7374 5f61 746f 6d73 225d 290a 2020  irst_atoms"]).  
-00006590: 2020 2020 2020 2020 2020 666f 7220 6469            for di
-000065a0: 7370 3120 696e 2064 6174 6173 6574 5b22  sp1 in dataset["
-000065b0: 6669 7273 745f 6174 6f6d 7322 5d3a 0a20  first_atoms"]:. 
-000065c0: 2020 2020 2020 2020 2020 2020 2020 206e                 n
-000065d0: 756d 5f73 6365 6c6c 7320 2b3d 206c 656e  um_scells += len
-000065e0: 2864 6973 7031 5b22 7365 636f 6e64 5f61  (disp1["second_a
-000065f0: 746f 6d73 225d 290a 2020 2020 2020 2020  toms"]).        
-00006600: 2020 2020 6469 7370 6c61 6365 6d65 6e74      displacement
-00006610: 7320 3d20 6e70 2e7a 6572 6f73 280a 2020  s = np.zeros(.  
-00006620: 2020 2020 2020 2020 2020 2020 2020 286e                (n
-00006630: 756d 5f73 6365 6c6c 732c 2073 656c 662e  um_scells, self.
-00006640: 5f73 7570 6572 6365 6c6c 2e67 6574 5f6e  _supercell.get_n
-00006650: 756d 6265 725f 6f66 5f61 746f 6d73 2829  umber_of_atoms()
-00006660: 2c20 3329 2c0a 2020 2020 2020 2020 2020  , 3),.          
-00006670: 2020 2020 2020 6474 7970 653d 2264 6f75        dtype="dou
-00006680: 626c 6522 2c0a 2020 2020 2020 2020 2020  ble",.          
-00006690: 2020 2020 2020 6f72 6465 723d 2243 222c        order="C",
-000066a0: 0a20 2020 2020 2020 2020 2020 2029 0a20  .            ). 
-000066b0: 2020 2020 2020 2020 2020 2069 203d 2030             i = 0
-000066c0: 0a20 2020 2020 2020 2020 2020 2066 6f72  .            for
-000066d0: 2064 6973 7031 2069 6e20 6461 7461 7365   disp1 in datase
-000066e0: 745b 2266 6972 7374 5f61 746f 6d73 225d  t["first_atoms"]
-000066f0: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-00006700: 2020 6469 7370 6c61 6365 6d65 6e74 735b    displacements[
-00006710: 692c 2064 6973 7031 5b22 6e75 6d62 6572  i, disp1["number
-00006720: 225d 5d20 3d20 6469 7370 315b 2264 6973  "]] = disp1["dis
-00006730: 706c 6163 656d 656e 7422 5d0a 2020 2020  placement"].    
-00006740: 2020 2020 2020 2020 2020 2020 6920 2b3d              i +=
-00006750: 2031 0a20 2020 2020 2020 2020 2020 2066   1.            f
-00006760: 6f72 2064 6973 7031 2069 6e20 6461 7461  or disp1 in data
-00006770: 7365 745b 2266 6972 7374 5f61 746f 6d73  set["first_atoms
-00006780: 225d 3a0a 2020 2020 2020 2020 2020 2020  "]:.            
-00006790: 2020 2020 666f 7220 6469 7370 3220 696e      for disp2 in
-000067a0: 2064 6973 7031 5b22 7365 636f 6e64 5f61   disp1["second_a
-000067b0: 746f 6d73 225d 3a0a 2020 2020 2020 2020  toms"]:.        
-000067c0: 2020 2020 2020 2020 2020 2020 6469 7370              disp
-000067d0: 6c61 6365 6d65 6e74 735b 692c 2064 6973  lacements[i, dis
-000067e0: 7032 5b22 6e75 6d62 6572 225d 5d20 3d20  p2["number"]] = 
-000067f0: 6469 7370 325b 2264 6973 706c 6163 656d  disp2["displacem
-00006800: 656e 7422 5d0a 2020 2020 2020 2020 2020  ent"].          
-00006810: 2020 2020 2020 2020 2020 6920 2b3d 2031            i += 1
-00006820: 0a20 2020 2020 2020 2065 6c69 6620 2266  .        elif "f
-00006830: 6f72 6365 7322 2069 6e20 6461 7461 7365  orces" in datase
-00006840: 7420 6f72 2022 6469 7370 6c61 6365 6d65  t or "displaceme
-00006850: 6e74 7322 2069 6e20 6461 7461 7365 743a  nts" in dataset:
-00006860: 0a20 2020 2020 2020 2020 2020 2064 6973  .            dis
-00006870: 706c 6163 656d 656e 7473 203d 2064 6174  placements = dat
-00006880: 6173 6574 5b22 6469 7370 6c61 6365 6d65  aset["displaceme
-00006890: 6e74 7322 5d0a 2020 2020 2020 2020 656c  nts"].        el
-000068a0: 7365 3a0a 2020 2020 2020 2020 2020 2020  se:.            
-000068b0: 7261 6973 6520 5275 6e74 696d 6545 7272  raise RuntimeErr
-000068c0: 6f72 2822 6469 7370 6c61 6365 6d65 6e74  or("displacement
-000068d0: 2064 6174 6173 6574 2068 6173 2077 726f   dataset has wro
-000068e0: 6e67 2066 6f72 6d61 742e 2229 0a0a 2020  ng format.")..  
-000068f0: 2020 2020 2020 7265 7475 726e 2064 6973        return dis
-00006900: 706c 6163 656d 656e 7473 0a0a 2020 2020  placements..    
-00006910: 4064 6973 706c 6163 656d 656e 7473 2e73  @displacements.s
-00006920: 6574 7465 720a 2020 2020 6465 6620 6469  etter.    def di
-00006930: 7370 6c61 6365 6d65 6e74 7328 7365 6c66  splacements(self
-00006940: 2c20 6469 7370 6c61 6365 6d65 6e74 7329  , displacements)
-00006950: 3a0a 2020 2020 2020 2020 6469 7370 7320  :.        disps 
-00006960: 3d20 6e70 2e61 7272 6179 2864 6973 706c  = np.array(displ
-00006970: 6163 656d 656e 7473 2c20 6474 7970 653d  acements, dtype=
-00006980: 2264 6f75 626c 6522 2c20 6f72 6465 723d  "double", order=
-00006990: 2243 2229 0a20 2020 2020 2020 206e 6174  "C").        nat
-000069a0: 6f6d 203d 206c 656e 2873 656c 662e 5f73  om = len(self._s
-000069b0: 7570 6572 6365 6c6c 290a 2020 2020 2020  upercell).      
-000069c0: 2020 6966 2064 6973 7073 2e6e 6469 6d20    if disps.ndim 
-000069d0: 213d 2033 206f 7220 6469 7370 732e 7368  != 3 or disps.sh
-000069e0: 6170 655b 313a 5d20 213d 2028 6e61 746f  ape[1:] != (nato
-000069f0: 6d2c 2033 293a 0a20 2020 2020 2020 2020  m, 3):.         
-00006a00: 2020 2072 6169 7365 2052 756e 7469 6d65     raise Runtime
-00006a10: 4572 726f 7228 2241 7272 6179 2073 6861  Error("Array sha
-00006a20: 7065 206f 6620 6469 7370 6c61 6365 6d65  pe of displaceme
-00006a30: 6e74 7320 6973 2069 6e63 6f72 7265 6374  nts is incorrect
-00006a40: 2e22 290a 2020 2020 2020 2020 6966 2073  .").        if s
-00006a50: 656c 662e 5f64 6174 6173 6574 2069 7320  elf._dataset is 
-00006a60: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
-00006a70: 2020 7365 6c66 2e5f 6461 7461 7365 7420    self._dataset 
-00006a80: 3d20 7b7d 0a20 2020 2020 2020 2065 6c69  = {}.        eli
-00006a90: 6620 2266 6972 7374 5f61 746f 6d73 2220  f "first_atoms" 
-00006aa0: 696e 2073 656c 662e 5f64 6174 6173 6574  in self._dataset
-00006ab0: 3a0a 2020 2020 2020 2020 2020 2020 7261  :.            ra
-00006ac0: 6973 6520 5275 6e74 696d 6545 7272 6f72  ise RuntimeError
-00006ad0: 2822 4469 7370 6c61 6365 6d65 6e74 7320  ("Displacements 
-00006ae0: 6172 6520 696e 636f 6d70 6174 6962 6c65  are incompatible
-00006af0: 2077 6974 6820 6461 7461 7365 742e 2229   with dataset.")
-00006b00: 0a20 2020 2020 2020 2073 656c 662e 5f64  .        self._d
-00006b10: 6174 6173 6574 5b22 6469 7370 6c61 6365  ataset["displace
-00006b20: 6d65 6e74 7322 5d20 3d20 6469 7370 730a  ments"] = disps.
-00006b30: 2020 2020 2020 2020 7365 6c66 2e5f 7375          self._su
-00006b40: 7065 7263 656c 6c73 5f77 6974 685f 6469  percells_with_di
-00006b50: 7370 6c61 6365 6d65 6e74 7320 3d20 4e6f  splacements = No
-00006b60: 6e65 0a0a 2020 2020 4070 726f 7065 7274  ne..    @propert
-00006b70: 790a 2020 2020 6465 6620 666f 7263 6573  y.    def forces
-00006b80: 2873 656c 6629 3a0a 2020 2020 2020 2020  (self):.        
-00006b90: 2222 2253 6574 7465 7220 616e 6420 6765  """Setter and ge
-00006ba0: 7474 6572 206f 6620 666f 7263 6573 2069  tter of forces i
-00006bb0: 6e20 6469 7370 6c61 6365 6d65 6e74 2064  n displacement d
-00006bc0: 6174 6173 6574 2e0a 0a20 2020 2020 2020  ataset...       
-00006bd0: 2041 2073 6574 206f 6620 6174 6f6d 6963   A set of atomic
-00006be0: 2066 6f72 6365 7320 696e 2064 6973 706c   forces in displ
-00006bf0: 6163 6564 2073 7570 6572 6365 6c6c 732e  aced supercells.
-00006c00: 2054 6865 206f 7264 6572 206f 660a 2020   The order of.  
-00006c10: 2020 2020 2020 6469 7370 6c61 6365 6420        displaced 
-00006c20: 7375 7065 7263 656c 6c73 2068 6173 2074  supercells has t
-00006c30: 6f20 6d61 7463 6820 7769 7468 2074 6861  o match with tha
-00006c40: 7420 696e 2064 6973 706c 6163 656d 656e  t in displacemen
-00006c50: 7420 6461 7461 7365 742e 0a20 2020 2020  t dataset..     
-00006c60: 2020 2073 6861 7065 3d28 6469 7370 6c61     shape=(displa
-00006c70: 6365 6420 7375 7065 7263 656c 6c73 2c20  ced supercells, 
-00006c80: 6174 6f6d 7320 696e 2073 7570 6572 6365  atoms in superce
-00006c90: 6c6c 2c20 3329 0a0a 2020 2020 2020 2020  ll, 3)..        
-00006ca0: 6765 7474 6572 203a 206e 6461 7272 6179  getter : ndarray
-00006cb0: 0a0a 2020 2020 2020 2020 7365 7474 6572  ..        setter
-00006cc0: 203a 2061 7272 6179 5f6c 696b 650a 2020   : array_like.  
-00006cd0: 2020 2020 2020 2020 2020 5468 6520 6f72            The or
-00006ce0: 6465 7220 6f66 2073 7570 6572 6365 6c6c  der of supercell
-00006cf0: 7320 7573 6564 2066 6f72 2063 616c 6375  s used for calcu
-00006d00: 6c61 7469 6e67 2066 6f72 6365 7320 6861  lating forces ha
-00006d10: 7320 746f 0a20 2020 2020 2020 2020 2020  s to.           
-00006d20: 2062 6520 7468 6520 7361 6d65 206f 7264   be the same ord
-00006d30: 6572 206f 6620 7375 7065 7263 656c 6c73  er of supercells
-00006d40: 5f77 6974 685f 6469 7370 6c61 6365 6d65  _with_displaceme
-00006d50: 6e74 732e 0a0a 2020 2020 2020 2020 2222  nts...        ""
-00006d60: 220a 2020 2020 2020 2020 6461 7461 7365  ".        datase
-00006d70: 7420 3d20 7365 6c66 2e5f 6461 7461 7365  t = self._datase
-00006d80: 740a 2020 2020 2020 2020 6966 2022 666f  t.        if "fo
-00006d90: 7263 6573 2220 696e 2064 6174 6173 6574  rces" in dataset
-00006da0: 3a0a 2020 2020 2020 2020 2020 2020 7265  :.            re
-00006db0: 7475 726e 2064 6174 6173 6574 5b22 666f  turn dataset["fo
-00006dc0: 7263 6573 225d 0a20 2020 2020 2020 2065  rces"].        e
-00006dd0: 6c69 6620 2266 6972 7374 5f61 746f 6d73  lif "first_atoms
-00006de0: 2220 696e 2064 6174 6173 6574 3a0a 2020  " in dataset:.  
-00006df0: 2020 2020 2020 2020 2020 6e75 6d5f 7363            num_sc
-00006e00: 656c 6c73 203d 206c 656e 2864 6174 6173  ells = len(datas
-00006e10: 6574 5b22 6669 7273 745f 6174 6f6d 7322  et["first_atoms"
-00006e20: 5d29 0a20 2020 2020 2020 2020 2020 2066  ]).            f
-00006e30: 6f72 2064 6973 7031 2069 6e20 6461 7461  or disp1 in data
-00006e40: 7365 745b 2266 6972 7374 5f61 746f 6d73  set["first_atoms
-00006e50: 225d 3a0a 2020 2020 2020 2020 2020 2020  "]:.            
-00006e60: 2020 2020 6e75 6d5f 7363 656c 6c73 202b      num_scells +
-00006e70: 3d20 6c65 6e28 6469 7370 315b 2273 6563  = len(disp1["sec
-00006e80: 6f6e 645f 6174 6f6d 7322 5d29 0a20 2020  ond_atoms"]).   
-00006e90: 2020 2020 2020 2020 2066 6f72 6365 7320           forces 
-00006ea0: 3d20 6e70 2e7a 6572 6f73 280a 2020 2020  = np.zeros(.    
-00006eb0: 2020 2020 2020 2020 2020 2020 286e 756d              (num
-00006ec0: 5f73 6365 6c6c 732c 2073 656c 662e 5f73  _scells, self._s
-00006ed0: 7570 6572 6365 6c6c 2e67 6574 5f6e 756d  upercell.get_num
-00006ee0: 6265 725f 6f66 5f61 746f 6d73 2829 2c20  ber_of_atoms(), 
-00006ef0: 3329 2c0a 2020 2020 2020 2020 2020 2020  3),.            
-00006f00: 2020 2020 6474 7970 653d 2264 6f75 626c      dtype="doubl
-00006f10: 6522 2c0a 2020 2020 2020 2020 2020 2020  e",.            
-00006f20: 2020 2020 6f72 6465 723d 2243 222c 0a20      order="C",. 
-00006f30: 2020 2020 2020 2020 2020 2029 0a20 2020             ).   
-00006f40: 2020 2020 2020 2020 2069 203d 2030 0a20           i = 0. 
-00006f50: 2020 2020 2020 2020 2020 2066 6f72 2064             for d
-00006f60: 6973 7031 2069 6e20 6461 7461 7365 745b  isp1 in dataset[
-00006f70: 2266 6972 7374 5f61 746f 6d73 225d 3a0a  "first_atoms"]:.
-00006f80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006f90: 666f 7263 6573 5b69 5d20 3d20 6469 7370  forces[i] = disp
-00006fa0: 315b 2266 6f72 6365 7322 5d0a 2020 2020  1["forces"].    
-00006fb0: 2020 2020 2020 2020 2020 2020 6920 2b3d              i +=
-00006fc0: 2031 0a20 2020 2020 2020 2020 2020 2066   1.            f
-00006fd0: 6f72 2064 6973 7031 2069 6e20 6461 7461  or disp1 in data
-00006fe0: 7365 745b 2266 6972 7374 5f61 746f 6d73  set["first_atoms
-00006ff0: 225d 3a0a 2020 2020 2020 2020 2020 2020  "]:.            
-00007000: 2020 2020 666f 7220 6469 7370 3220 696e      for disp2 in
-00007010: 2064 6973 7031 5b22 7365 636f 6e64 5f61   disp1["second_a
-00007020: 746f 6d73 225d 3a0a 2020 2020 2020 2020  toms"]:.        
-00007030: 2020 2020 2020 2020 2020 2020 666f 7263              forc
-00007040: 6573 5b69 5d20 3d20 6469 7370 325b 2266  es[i] = disp2["f
-00007050: 6f72 6365 7322 5d0a 2020 2020 2020 2020  orces"].        
-00007060: 2020 2020 2020 2020 2020 2020 6920 2b3d              i +=
-00007070: 2031 0a20 2020 2020 2020 2020 2020 2072   1.            r
-00007080: 6574 7572 6e20 666f 7263 6573 0a20 2020  eturn forces.   
-00007090: 2020 2020 2065 6c73 653a 0a20 2020 2020       else:.     
-000070a0: 2020 2020 2020 2072 6169 7365 2052 756e         raise Run
-000070b0: 7469 6d65 4572 726f 7228 2264 6973 706c  timeError("displ
-000070c0: 6163 656d 656e 7420 6461 7461 7365 7420  acement dataset 
-000070d0: 6861 7320 7772 6f6e 6720 666f 726d 6174  has wrong format
-000070e0: 2e22 290a 0a20 2020 2040 666f 7263 6573  .")..    @forces
-000070f0: 2e73 6574 7465 720a 2020 2020 6465 6620  .setter.    def 
-00007100: 666f 7263 6573 2873 656c 662c 2066 6f72  forces(self, for
-00007110: 6365 735f 6663 3329 3a0a 2020 2020 2020  ces_fc3):.      
-00007120: 2020 666f 7263 6573 203d 206e 702e 6172    forces = np.ar
-00007130: 7261 7928 666f 7263 6573 5f66 6333 2c20  ray(forces_fc3, 
-00007140: 6474 7970 653d 2264 6f75 626c 6522 2c20  dtype="double", 
-00007150: 6f72 6465 723d 2243 2229 0a20 2020 2020  order="C").     
-00007160: 2020 2064 6174 6173 6574 203d 2073 656c     dataset = sel
-00007170: 662e 5f64 6174 6173 6574 0a20 2020 2020  f._dataset.     
-00007180: 2020 2069 6620 2266 6972 7374 5f61 746f     if "first_ato
-00007190: 6d73 2220 696e 2064 6174 6173 6574 3a0a  ms" in dataset:.
-000071a0: 2020 2020 2020 2020 2020 2020 6920 3d20              i = 
-000071b0: 300a 2020 2020 2020 2020 2020 2020 666f  0.            fo
-000071c0: 7220 6469 7370 3120 696e 2064 6174 6173  r disp1 in datas
-000071d0: 6574 5b22 6669 7273 745f 6174 6f6d 7322  et["first_atoms"
-000071e0: 5d3a 0a20 2020 2020 2020 2020 2020 2020  ]:.             
-000071f0: 2020 2064 6973 7031 5b22 666f 7263 6573     disp1["forces
-00007200: 225d 203d 2066 6f72 6365 735b 695d 0a20  "] = forces[i]. 
-00007210: 2020 2020 2020 2020 2020 2020 2020 2069                 i
-00007220: 202b 3d20 310a 2020 2020 2020 2020 2020   += 1.          
-00007230: 2020 666f 7220 6469 7370 3120 696e 2064    for disp1 in d
-00007240: 6174 6173 6574 5b22 6669 7273 745f 6174  ataset["first_at
-00007250: 6f6d 7322 5d3a 0a20 2020 2020 2020 2020  oms"]:.         
-00007260: 2020 2020 2020 2066 6f72 2064 6973 7032         for disp2
-00007270: 2069 6e20 6469 7370 315b 2273 6563 6f6e   in disp1["secon
-00007280: 645f 6174 6f6d 7322 5d3a 0a20 2020 2020  d_atoms"]:.     
-00007290: 2020 2020 2020 2020 2020 2020 2020 2064                 d
-000072a0: 6973 7032 5b22 666f 7263 6573 225d 203d  isp2["forces"] =
-000072b0: 2066 6f72 6365 735b 695d 0a20 2020 2020   forces[i].     
-000072c0: 2020 2020 2020 2020 2020 2020 2020 2069                 i
-000072d0: 202b 3d20 310a 2020 2020 2020 2020 656c   += 1.        el
-000072e0: 6966 2022 6469 7370 6c61 6365 6d65 6e74  if "displacement
-000072f0: 7322 2069 6e20 6461 7461 7365 7420 6f72  s" in dataset or
-00007300: 2022 666f 7263 6573 2220 696e 2064 6174   "forces" in dat
-00007310: 6173 6574 3a0a 2020 2020 2020 2020 2020  aset:.          
-00007320: 2020 6461 7461 7365 745b 2266 6f72 6365    dataset["force
-00007330: 7322 5d20 3d20 666f 7263 6573 0a0a 2020  s"] = forces..  
-00007340: 2020 4070 726f 7065 7274 790a 2020 2020    @property.    
-00007350: 6465 6620 7068 6f6e 6f6e 5f64 6973 706c  def phonon_displ
-00007360: 6163 656d 656e 7473 2873 656c 6629 3a0a  acements(self):.
-00007370: 2020 2020 2020 2020 2222 2253 6574 7465          """Sette
-00007380: 7220 616e 6420 6765 7474 6572 206f 6620  r and getter of 
-00007390: 6469 7370 6c61 6365 6d65 6e74 7320 696e  displacements in
-000073a0: 2073 7570 6572 6365 6c6c 7320 666f 7220   supercells for 
-000073b0: 6663 322e 0a0a 2020 2020 2020 2020 5468  fc2...        Th
-000073c0: 6572 6520 6172 6520 7477 6f20 7479 7065  ere are two type
-000073d0: 7320 6f66 2064 6973 706c 6163 656d 656e  s of displacemen
-000073e0: 7420 6461 7461 7365 742e 2053 6565 2074  t dataset. See t
-000073f0: 6865 2064 6f63 7374 7269 6e67 0a20 2020  he docstring.   
-00007400: 2020 2020 206f 6620 6461 7461 7365 7420       of dataset 
-00007410: 6162 6f75 7420 7479 7065 7320 3120 616e  about types 1 an
-00007420: 6420 3220 666f 7220 7468 6520 6469 7370  d 2 for the disp
-00007430: 6c61 6365 6d65 6e74 2064 6174 6173 6574  lacement dataset
-00007440: 2066 6f72 6d61 7473 2e0a 2020 2020 2020   formats..      
-00007450: 2020 4469 7370 6c61 6365 6d65 6e74 7320    Displacements 
-00007460: 7365 7420 7265 7475 726e 6564 2064 6570  set returned dep
-00007470: 656e 6473 206f 6e20 6569 7468 6572 2074  ends on either t
-00007480: 7970 652d 3120 6f72 2074 7970 652d 3220  ype-1 or type-2 
-00007490: 6173 0a20 2020 2020 2020 2066 6f6c 6c6f  as.        follo
-000074a0: 7773 3a0a 0a20 2020 2020 2020 2054 7970  ws:..        Typ
-000074b0: 652d 312c 204c 6973 7420 6f66 206c 6973  e-1, List of lis
-000074c0: 740a 2020 2020 2020 2020 2020 2020 5468  t.            Th
-000074d0: 6520 696e 7465 726e 616c 206c 6973 7420  e internal list 
-000074e0: 6861 7320 3420 656c 656d 656e 7473 2073  has 4 elements s
-000074f0: 7563 6820 6173 205b 3332 2c20 302e 3031  uch as [32, 0.01
-00007500: 2c20 302e 302c 2030 2e30 5d5d 2e0a 2020  , 0.0, 0.0]]..  
-00007510: 2020 2020 2020 2020 2020 5468 6520 6669            The fi
-00007520: 7273 7420 656c 656d 656e 7420 6973 2074  rst element is t
-00007530: 6865 2073 7570 6572 6365 6c6c 2061 746f  he supercell ato
-00007540: 6d20 696e 6465 7820 7374 6172 7469 6e67  m index starting
-00007550: 2077 6974 6820 302e 0a20 2020 2020 2020   with 0..       
-00007560: 2020 2020 2054 6865 2072 656d 6169 6e69       The remaini
-00007570: 6e67 2074 6872 6565 2065 6c65 6d65 6e74  ng three element
-00007580: 7320 6769 7665 2074 6865 2064 6973 706c  s give the displ
-00007590: 6163 656d 656e 7420 696e 2043 6172 7465  acement in Carte
-000075a0: 7369 616e 0a20 2020 2020 2020 2020 2020  sian.           
-000075b0: 2063 6f6f 7264 696e 6174 6573 2e0a 2020   coordinates..  
-000075c0: 2020 2020 2020 5479 7065 2d32 2c20 6172        Type-2, ar
-000075d0: 7261 795f 6c69 6b65 0a20 2020 2020 2020  ray_like.       
-000075e0: 2020 2020 2044 6973 706c 6163 656d 656e       Displacemen
-000075f0: 7473 206f 6620 616c 6c20 6174 6f6d 7320  ts of all atoms 
-00007600: 6f66 2061 6c6c 2073 7570 6572 6365 6c6c  of all supercell
-00007610: 7320 696e 2043 6172 7465 7369 616e 0a20  s in Cartesian. 
-00007620: 2020 2020 2020 2020 2020 2063 6f6f 7264             coord
-00007630: 696e 6174 6573 2e0a 2020 2020 2020 2020  inates..        
-00007640: 2020 2020 7368 6170 653d 2873 7570 6572      shape=(super
-00007650: 6365 6c6c 732c 206e 6174 6f6d 2c20 3329  cells, natom, 3)
-00007660: 0a20 2020 2020 2020 2020 2020 2064 7479  .            dty
-00007670: 7065 3d27 646f 7562 6c65 270a 0a0a 2020  pe='double'...  
-00007680: 2020 2020 2020 466f 7220 7365 7474 6572        For setter
-00007690: 2c20 6f6e 6c79 2074 7970 652d 3220 6461  , only type-2 da
-000076a0: 7461 7365 7420 666f 726d 6174 2069 7320  taset format is 
-000076b0: 616c 6c6f 7765 642e 0a0a 2020 2020 2020  allowed...      
-000076c0: 2020 6469 7370 6c61 6365 6d65 6e74 7320    displacements 
-000076d0: 3a20 6172 7261 795f 6c69 6b65 0a20 2020  : array_like.   
-000076e0: 2020 2020 2020 2020 2041 746f 6d69 6320           Atomic 
-000076f0: 6469 7370 6c61 6365 6d65 6e74 7320 6f66  displacements of
-00007700: 2061 6c6c 2061 746f 6d73 206f 6620 616c   all atoms of al
-00007710: 6c20 7375 7065 7263 656c 6c73 2e0a 2020  l supercells..  
-00007720: 2020 2020 2020 2020 2020 4f6e 6c79 2061            Only a
-00007730: 6c6c 2064 6973 706c 6163 656d 656e 7473  ll displacements
-00007740: 2069 6e20 6561 6368 2073 7570 6572 6365   in each superce
-00007750: 6c6c 2063 6173 6520 2874 7970 652d 3229  ll case (type-2)
-00007760: 2069 730a 2020 2020 2020 2020 2020 2020   is.            
-00007770: 7375 7070 6f72 7465 642e 0a20 2020 2020  supported..     
-00007780: 2020 2020 2020 2073 6861 7065 3d28 7375         shape=(su
-00007790: 7065 7263 656c 6c73 2c20 6e61 746f 6d2c  percells, natom,
-000077a0: 2033 292c 2064 7479 7065 3d27 646f 7562   3), dtype='doub
-000077b0: 6c65 272c 206f 7264 6572 3d27 4327 0a0a  le', order='C'..
-000077c0: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
-000077d0: 2020 2020 6966 2073 656c 662e 5f70 686f      if self._pho
-000077e0: 6e6f 6e5f 7375 7065 7263 656c 6c5f 6d61  non_supercell_ma
-000077f0: 7472 6978 2069 7320 4e6f 6e65 3a0a 2020  trix is None:.  
-00007800: 2020 2020 2020 2020 2020 7261 6973 6520            raise 
-00007810: 5275 6e74 696d 6545 7272 6f72 2822 7068  RuntimeError("ph
-00007820: 6f6e 6f6e 5f73 7570 6572 6365 6c6c 5f6d  onon_supercell_m
-00007830: 6174 7269 7820 6973 206e 6f74 2073 6574  atrix is not set
-00007840: 2e22 290a 0a20 2020 2020 2020 2064 6174  .")..        dat
-00007850: 6173 6574 203d 2073 656c 662e 5f70 686f  aset = self._pho
-00007860: 6e6f 6e5f 6461 7461 7365 740a 2020 2020  non_dataset.    
-00007870: 2020 2020 6966 2022 6669 7273 745f 6174      if "first_at
-00007880: 6f6d 7322 2069 6e20 6461 7461 7365 743a  oms" in dataset:
-00007890: 0a20 2020 2020 2020 2020 2020 206e 756d  .            num
-000078a0: 5f73 6365 6c6c 7320 3d20 6c65 6e28 6461  _scells = len(da
-000078b0: 7461 7365 745b 2266 6972 7374 5f61 746f  taset["first_ato
-000078c0: 6d73 225d 290a 2020 2020 2020 2020 2020  ms"]).          
-000078d0: 2020 6e61 746f 6d20 3d20 6c65 6e28 7365    natom = len(se
-000078e0: 6c66 2e5f 7068 6f6e 6f6e 5f73 7570 6572  lf._phonon_super
-000078f0: 6365 6c6c 290a 2020 2020 2020 2020 2020  cell).          
-00007900: 2020 6469 7370 6c61 6365 6d65 6e74 7320    displacements 
-00007910: 3d20 6e70 2e7a 6572 6f73 2828 6e75 6d5f  = np.zeros((num_
-00007920: 7363 656c 6c73 2c20 6e61 746f 6d2c 2033  scells, natom, 3
-00007930: 292c 2064 7479 7065 3d22 646f 7562 6c65  ), dtype="double
-00007940: 222c 206f 7264 6572 3d22 4322 290a 2020  ", order="C").  
-00007950: 2020 2020 2020 2020 2020 666f 7220 692c            for i,
-00007960: 2064 6973 7031 2069 6e20 656e 756d 6572   disp1 in enumer
-00007970: 6174 6528 6461 7461 7365 745b 2266 6972  ate(dataset["fir
-00007980: 7374 5f61 746f 6d73 225d 293a 0a20 2020  st_atoms"]):.   
-00007990: 2020 2020 2020 2020 2020 2020 2064 6973               dis
-000079a0: 706c 6163 656d 656e 7473 5b69 2c20 6469  placements[i, di
-000079b0: 7370 315b 226e 756d 6265 7222 5d5d 203d  sp1["number"]] =
-000079c0: 2064 6973 7031 5b22 6469 7370 6c61 6365   disp1["displace
-000079d0: 6d65 6e74 225d 0a20 2020 2020 2020 2065  ment"].        e
-000079e0: 6c69 6620 2266 6f72 6365 7322 2069 6e20  lif "forces" in 
-000079f0: 6461 7461 7365 7420 6f72 2022 6469 7370  dataset or "disp
-00007a00: 6c61 6365 6d65 6e74 7322 2069 6e20 6461  lacements" in da
-00007a10: 7461 7365 743a 0a20 2020 2020 2020 2020  taset:.         
-00007a20: 2020 2064 6973 706c 6163 656d 656e 7473     displacements
-00007a30: 203d 2064 6174 6173 6574 5b22 6469 7370   = dataset["disp
-00007a40: 6c61 6365 6d65 6e74 7322 5d0a 2020 2020  lacements"].    
-00007a50: 2020 2020 656c 7365 3a0a 2020 2020 2020      else:.      
-00007a60: 2020 2020 2020 7261 6973 6520 5275 6e74        raise Runt
-00007a70: 696d 6545 7272 6f72 2822 6469 7370 6c61  imeError("displa
-00007a80: 6365 6d65 6e74 2064 6174 6173 6574 2068  cement dataset h
-00007a90: 6173 2077 726f 6e67 2066 6f72 6d61 742e  as wrong format.
-00007aa0: 2229 0a0a 2020 2020 2020 2020 7265 7475  ")..        retu
-00007ab0: 726e 2064 6973 706c 6163 656d 656e 7473  rn displacements
-00007ac0: 0a0a 2020 2020 4070 686f 6e6f 6e5f 6469  ..    @phonon_di
-00007ad0: 7370 6c61 6365 6d65 6e74 732e 7365 7474  splacements.sett
-00007ae0: 6572 0a20 2020 2064 6566 2070 686f 6e6f  er.    def phono
-00007af0: 6e5f 6469 7370 6c61 6365 6d65 6e74 7328  n_displacements(
-00007b00: 7365 6c66 2c20 6469 7370 6c61 6365 6d65  self, displaceme
-00007b10: 6e74 7329 3a0a 2020 2020 2020 2020 6966  nts):.        if
-00007b20: 2073 656c 662e 5f70 686f 6e6f 6e5f 7375   self._phonon_su
-00007b30: 7065 7263 656c 6c5f 6d61 7472 6978 2069  percell_matrix i
-00007b40: 7320 4e6f 6e65 3a0a 2020 2020 2020 2020  s None:.        
-00007b50: 2020 2020 7261 6973 6520 5275 6e74 696d      raise Runtim
-00007b60: 6545 7272 6f72 2822 7068 6f6e 6f6e 5f73  eError("phonon_s
-00007b70: 7570 6572 6365 6c6c 5f6d 6174 7269 7820  upercell_matrix 
-00007b80: 6973 206e 6f74 2073 6574 2e22 290a 0a20  is not set.").. 
-00007b90: 2020 2020 2020 2064 6973 7073 203d 206e         disps = n
-00007ba0: 702e 6172 7261 7928 6469 7370 6c61 6365  p.array(displace
-00007bb0: 6d65 6e74 732c 2064 7479 7065 3d22 646f  ments, dtype="do
-00007bc0: 7562 6c65 222c 206f 7264 6572 3d22 4322  uble", order="C"
-00007bd0: 290a 2020 2020 2020 2020 6e61 746f 6d20  ).        natom 
-00007be0: 3d20 6c65 6e28 7365 6c66 2e5f 7068 6f6e  = len(self._phon
-00007bf0: 6f6e 5f73 7570 6572 6365 6c6c 290a 2020  on_supercell).  
-00007c00: 2020 2020 2020 6966 2064 6973 7073 2e6e        if disps.n
-00007c10: 6469 6d20 213d 2033 206f 7220 6469 7370  dim != 3 or disp
-00007c20: 732e 7368 6170 655b 313a 5d20 213d 2028  s.shape[1:] != (
-00007c30: 6e61 746f 6d2c 2033 293a 0a20 2020 2020  natom, 3):.     
-00007c40: 2020 2020 2020 2072 6169 7365 2052 756e         raise Run
-00007c50: 7469 6d65 4572 726f 7228 2241 7272 6179  timeError("Array
-00007c60: 2073 6861 7065 206f 6620 6469 7370 6c61   shape of displa
-00007c70: 6365 6d65 6e74 7320 6973 2069 6e63 6f72  cements is incor
-00007c80: 7265 6374 2e22 290a 2020 2020 2020 2020  rect.").        
-00007c90: 6966 2073 656c 662e 5f70 686f 6e6f 6e5f  if self._phonon_
-00007ca0: 6461 7461 7365 7420 6973 204e 6f6e 653a  dataset is None:
-00007cb0: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
-00007cc0: 662e 5f70 686f 6e6f 6e5f 6461 7461 7365  f._phonon_datase
-00007cd0: 7420 3d20 7b7d 0a20 2020 2020 2020 2065  t = {}.        e
-00007ce0: 6c69 6620 2266 6972 7374 5f61 746f 6d73  lif "first_atoms
-00007cf0: 2220 696e 2073 656c 662e 5f70 686f 6e6f  " in self._phono
-00007d00: 6e5f 6461 7461 7365 743a 0a20 2020 2020  n_dataset:.     
-00007d10: 2020 2020 2020 2072 6169 7365 2052 756e         raise Run
-00007d20: 7469 6d65 4572 726f 7228 2244 6973 706c  timeError("Displ
-00007d30: 6163 656d 656e 7473 2061 7265 2069 6e63  acements are inc
-00007d40: 6f6d 7061 7469 626c 6520 7769 7468 2064  ompatible with d
-00007d50: 6174 6173 6574 2e22 290a 0a20 2020 2020  ataset.")..     
-00007d60: 2020 2073 656c 662e 5f70 686f 6e6f 6e5f     self._phonon_
-00007d70: 6461 7461 7365 745b 2264 6973 706c 6163  dataset["displac
-00007d80: 656d 656e 7473 225d 203d 2064 6973 7073  ements"] = disps
-00007d90: 0a20 2020 2020 2020 2073 656c 662e 5f70  .        self._p
-00007da0: 686f 6e6f 6e5f 7375 7065 7263 656c 6c73  honon_supercells
-00007db0: 5f77 6974 685f 6469 7370 6c61 6365 6d65  _with_displaceme
-00007dc0: 6e74 7320 3d20 4e6f 6e65 0a0a 2020 2020  nts = None..    
-00007dd0: 4070 726f 7065 7274 790a 2020 2020 6465  @property.    de
-00007de0: 6620 7068 6f6e 6f6e 5f66 6f72 6365 7328  f phonon_forces(
-00007df0: 7365 6c66 293a 0a20 2020 2020 2020 2022  self):.        "
-00007e00: 2222 5365 7474 6572 2061 6e64 2067 6574  ""Setter and get
-00007e10: 7465 7220 6f66 2066 6f72 6365 7320 696e  ter of forces in
-00007e20: 2064 6973 706c 6163 656d 656e 7420 6461   displacement da
-00007e30: 7461 7365 7420 666f 7220 6663 322e 0a0a  taset for fc2...
-00007e40: 2020 2020 2020 2020 4120 7365 7420 6f66          A set of
-00007e50: 2061 746f 6d69 6320 666f 7263 6573 2069   atomic forces i
-00007e60: 6e20 6469 7370 6c61 6365 6420 7375 7065  n displaced supe
-00007e70: 7263 656c 6c73 2e20 5468 6520 6f72 6465  rcells. The orde
-00007e80: 7220 6f66 0a20 2020 2020 2020 2064 6973  r of.        dis
-00007e90: 706c 6163 6564 2073 7570 6572 6365 6c6c  placed supercell
-00007ea0: 7320 6861 7320 746f 206d 6174 6368 2077  s has to match w
-00007eb0: 6974 6820 7468 6174 2069 6e20 7068 6f6e  ith that in phon
-00007ec0: 6f6e 2064 6973 706c 6163 656d 656e 740a  on displacement.
-00007ed0: 2020 2020 2020 2020 6461 7461 7365 742e          dataset.
-00007ee0: 0a20 2020 2020 2020 2073 6861 7065 3d28  .        shape=(
-00007ef0: 6469 7370 6c61 6365 6420 7375 7065 7263  displaced superc
-00007f00: 656c 6c73 2c20 6174 6f6d 7320 696e 2073  ells, atoms in s
-00007f10: 7570 6572 6365 6c6c 2c20 3329 0a0a 2020  upercell, 3)..  
-00007f20: 2020 2020 2020 6765 7474 6572 203a 206e        getter : n
-00007f30: 6461 7272 6179 0a0a 2020 2020 2020 2020  darray..        
-00007f40: 7365 7474 6572 203a 2061 7272 6179 5f6c  setter : array_l
-00007f50: 696b 650a 2020 2020 2020 2020 2020 2020  ike.            
-00007f60: 5468 6520 6f72 6465 7220 6f66 2073 7570  The order of sup
-00007f70: 6572 6365 6c6c 7320 7573 6564 2066 6f72  ercells used for
-00007f80: 2063 616c 6375 6c61 7469 6e67 2066 6f72   calculating for
-00007f90: 6365 7320 6861 7320 746f 0a20 2020 2020  ces has to.     
-00007fa0: 2020 2020 2020 2062 6520 7468 6520 7361         be the sa
-00007fb0: 6d65 206f 7264 6572 206f 6620 7068 6f6e  me order of phon
-00007fc0: 6f6e 5f73 7570 6572 6365 6c6c 735f 7769  on_supercells_wi
-00007fd0: 7468 5f64 6973 706c 6163 656d 656e 7473  th_displacements
-00007fe0: 2e0a 0a20 2020 2020 2020 2022 2222 0a20  ...        """. 
-00007ff0: 2020 2020 2020 2069 6620 7365 6c66 2e5f         if self._
-00008000: 7068 6f6e 6f6e 5f64 6174 6173 6574 2069  phonon_dataset i
-00008010: 7320 4e6f 6e65 3a0a 2020 2020 2020 2020  s None:.        
-00008020: 2020 2020 7261 6973 6520 5275 6e74 696d      raise Runtim
-00008030: 6545 7272 6f72 2822 7068 6f6e 6f6e 5f64  eError("phonon_d
-00008040: 6973 706c 6163 656d 656e 745f 6461 7461  isplacement_data
-00008050: 7365 7420 646f 6573 206e 6f74 2065 7869  set does not exi
-00008060: 7374 2e22 290a 0a20 2020 2020 2020 2064  st.")..        d
-00008070: 6174 6173 6574 203d 2073 656c 662e 5f70  ataset = self._p
-00008080: 686f 6e6f 6e5f 6461 7461 7365 740a 2020  honon_dataset.  
-00008090: 2020 2020 2020 6966 2022 666f 7263 6573        if "forces
-000080a0: 2220 696e 2064 6174 6173 6574 3a0a 2020  " in dataset:.  
-000080b0: 2020 2020 2020 2020 2020 7265 7475 726e            return
-000080c0: 2064 6174 6173 6574 5b22 666f 7263 6573   dataset["forces
-000080d0: 225d 0a20 2020 2020 2020 2065 6c69 6620  "].        elif 
-000080e0: 2266 6972 7374 5f61 746f 6d73 2220 696e  "first_atoms" in
-000080f0: 2064 6174 6173 6574 3a0a 2020 2020 2020   dataset:.      
-00008100: 2020 2020 2020 6e75 6d5f 7363 656c 6c73        num_scells
-00008110: 203d 206c 656e 2864 6174 6173 6574 5b22   = len(dataset["
-00008120: 6669 7273 745f 6174 6f6d 7322 5d29 0a20  first_atoms"]). 
-00008130: 2020 2020 2020 2020 2020 2066 6f72 6365             force
-00008140: 7320 3d20 6e70 2e7a 6572 6f73 280a 2020  s = np.zeros(.  
-00008150: 2020 2020 2020 2020 2020 2020 2020 286e                (n
-00008160: 756d 5f73 6365 6c6c 732c 2073 656c 662e  um_scells, self.
-00008170: 5f70 686f 6e6f 6e5f 7375 7065 7263 656c  _phonon_supercel
-00008180: 6c2e 6765 745f 6e75 6d62 6572 5f6f 665f  l.get_number_of_
-00008190: 6174 6f6d 7328 292c 2033 292c 0a20 2020  atoms(), 3),.   
-000081a0: 2020 2020 2020 2020 2020 2020 2064 7479               dty
-000081b0: 7065 3d22 646f 7562 6c65 222c 0a20 2020  pe="double",.   
-000081c0: 2020 2020 2020 2020 2020 2020 206f 7264               ord
-000081d0: 6572 3d22 4322 2c0a 2020 2020 2020 2020  er="C",.        
-000081e0: 2020 2020 290a 2020 2020 2020 2020 2020      ).          
-000081f0: 2020 666f 7220 692c 2064 6973 7031 2069    for i, disp1 i
-00008200: 6e20 656e 756d 6572 6174 6528 6461 7461  n enumerate(data
-00008210: 7365 745b 2266 6972 7374 5f61 746f 6d73  set["first_atoms
-00008220: 225d 293a 0a20 2020 2020 2020 2020 2020  "]):.           
-00008230: 2020 2020 2066 6f72 6365 735b 695d 203d       forces[i] =
-00008240: 2064 6973 7031 5b22 666f 7263 6573 225d   disp1["forces"]
-00008250: 0a20 2020 2020 2020 2020 2020 2072 6574  .            ret
-00008260: 7572 6e20 666f 7263 6573 0a20 2020 2020  urn forces.     
-00008270: 2020 2065 6c73 653a 0a20 2020 2020 2020     else:.       
-00008280: 2020 2020 2072 6169 7365 2052 756e 7469       raise Runti
-00008290: 6d65 4572 726f 7228 2264 6973 706c 6163  meError("displac
-000082a0: 656d 656e 7420 6461 7461 7365 7420 6861  ement dataset ha
-000082b0: 7320 7772 6f6e 6720 666f 726d 6174 2e22  s wrong format."
-000082c0: 290a 0a20 2020 2040 7068 6f6e 6f6e 5f66  )..    @phonon_f
-000082d0: 6f72 6365 732e 7365 7474 6572 0a20 2020  orces.setter.   
-000082e0: 2064 6566 2070 686f 6e6f 6e5f 666f 7263   def phonon_forc
-000082f0: 6573 2873 656c 662c 2066 6f72 6365 735f  es(self, forces_
-00008300: 6663 3229 3a0a 2020 2020 2020 2020 6966  fc2):.        if
-00008310: 2073 656c 662e 5f70 686f 6e6f 6e5f 6461   self._phonon_da
-00008320: 7461 7365 7420 6973 204e 6f6e 653a 0a20  taset is None:. 
-00008330: 2020 2020 2020 2020 2020 2072 6169 7365             raise
-00008340: 2052 756e 7469 6d65 4572 726f 7228 2270   RuntimeError("p
-00008350: 686f 6e6f 6e5f 6469 7370 6c61 6365 6d65  honon_displaceme
-00008360: 6e74 5f64 6174 6173 6574 2064 6f65 7320  nt_dataset does 
-00008370: 6e6f 7420 6578 6973 742e 2229 0a0a 2020  not exist.")..  
-00008380: 2020 2020 2020 666f 7263 6573 203d 206e        forces = n
-00008390: 702e 6172 7261 7928 666f 7263 6573 5f66  p.array(forces_f
-000083a0: 6332 2c20 6474 7970 653d 2264 6f75 626c  c2, dtype="doubl
-000083b0: 6522 2c20 6f72 6465 723d 2243 2229 0a20  e", order="C"). 
-000083c0: 2020 2020 2020 2064 6174 6173 6574 203d         dataset =
-000083d0: 2073 656c 662e 5f70 686f 6e6f 6e5f 6461   self._phonon_da
-000083e0: 7461 7365 740a 2020 2020 2020 2020 6966  taset.        if
-000083f0: 2022 6669 7273 745f 6174 6f6d 7322 2069   "first_atoms" i
-00008400: 6e20 6461 7461 7365 743a 0a20 2020 2020  n dataset:.     
-00008410: 2020 2020 2020 2069 203d 2030 0a20 2020         i = 0.   
-00008420: 2020 2020 2020 2020 2066 6f72 2069 2c20           for i, 
-00008430: 6469 7370 3120 696e 2065 6e75 6d65 7261  disp1 in enumera
-00008440: 7465 2864 6174 6173 6574 5b22 6669 7273  te(dataset["firs
-00008450: 745f 6174 6f6d 7322 5d29 3a0a 2020 2020  t_atoms"]):.    
-00008460: 2020 2020 2020 2020 2020 2020 6469 7370              disp
-00008470: 315b 2266 6f72 6365 7322 5d20 3d20 666f  1["forces"] = fo
-00008480: 7263 6573 5b69 5d0a 2020 2020 2020 2020  rces[i].        
-00008490: 2020 2020 2020 2020 6920 2b3d 2031 0a20          i += 1. 
-000084a0: 2020 2020 2020 2065 6c69 6620 2264 6973         elif "dis
-000084b0: 706c 6163 656d 656e 7473 2220 696e 2064  placements" in d
-000084c0: 6174 6173 6574 206f 7220 2266 6f72 6365  ataset or "force
-000084d0: 7322 2069 6e20 6461 7461 7365 743a 0a20  s" in dataset:. 
-000084e0: 2020 2020 2020 2020 2020 2064 6174 6173             datas
-000084f0: 6574 5b22 666f 7263 6573 225d 203d 2066  et["forces"] = f
-00008500: 6f72 6365 730a 0a20 2020 2040 7072 6f70  orces..    @prop
-00008510: 6572 7479 0a20 2020 2064 6566 2070 6870  erty.    def php
-00008520: 685f 696e 7465 7261 6374 696f 6e28 7365  h_interaction(se
-00008530: 6c66 293a 0a20 2020 2020 2020 2022 2222  lf):.        """
-00008540: 5265 7475 726e 2049 6e74 6572 6163 7469  Return Interacti
-00008550: 6f6e 2069 6e73 7461 6e63 652e 2222 220a  on instance.""".
-00008560: 2020 2020 2020 2020 7265 7475 726e 2073          return s
-00008570: 656c 662e 5f69 6e74 6572 6163 7469 6f6e  elf._interaction
-00008580: 0a0a 2020 2020 4070 726f 7065 7274 790a  ..    @property.
-00008590: 2020 2020 6465 6620 6465 7461 696c 6564      def detailed
-000085a0: 5f67 616d 6d61 7328 7365 6c66 293a 0a20  _gammas(self):. 
-000085b0: 2020 2020 2020 2022 2222 5265 7475 726e         """Return
-000085c0: 2064 6574 6169 6c65 6420 6761 6d6d 612e   detailed gamma.
-000085d0: 2222 220a 2020 2020 2020 2020 7265 7475  """.        retu
-000085e0: 726e 2073 656c 662e 5f64 6574 6169 6c65  rn self._detaile
-000085f0: 645f 6761 6d6d 6173 0a0a 2020 2020 4070  d_gammas..    @p
-00008600: 726f 7065 7274 790a 2020 2020 6465 6620  roperty.    def 
-00008610: 6772 6964 2873 656c 6629 3a0a 2020 2020  grid(self):.    
-00008620: 2020 2020 2222 2252 6574 7572 6e20 4272      """Return Br
-00008630: 696c 6c6f 7569 6e20 7a6f 6e65 2067 7269  illouin zone gri
-00008640: 6420 696e 666f 726d 6174 696f 6e2e 0a0a  d information...
-00008650: 2020 2020 2020 2020 425a 4772 6964 0a20          BZGrid. 
-00008660: 2020 2020 2020 2020 2020 2041 6e20 696e             An in
-00008670: 7374 616e 6365 206f 6620 425a 4772 6964  stance of BZGrid
-00008680: 2075 7365 6420 666f 7220 656e 7469 7265   used for entire
-00008690: 2070 686f 6e6f 3370 7920 6361 6c63 756c   phono3py calcul
-000086a0: 6174 696f 6e2e 0a0a 2020 2020 2020 2020  ation...        
-000086b0: 2222 220a 2020 2020 2020 2020 7265 7475  """.        retu
-000086c0: 726e 2073 656c 662e 5f62 7a5f 6772 6964  rn self._bz_grid
-000086d0: 0a0a 2020 2020 6465 6620 696e 6974 5f70  ..    def init_p
-000086e0: 6870 685f 696e 7465 7261 6374 696f 6e28  hph_interaction(
-000086f0: 0a20 2020 2020 2020 2073 656c 662c 0a20  .        self,. 
-00008700: 2020 2020 2020 206e 6163 5f71 5f64 6972         nac_q_dir
-00008710: 6563 7469 6f6e 3d4e 6f6e 652c 0a20 2020  ection=None,.   
-00008720: 2020 2020 2063 6f6e 7374 616e 745f 6176       constant_av
-00008730: 6572 6167 6564 5f69 6e74 6572 6163 7469  eraged_interacti
-00008740: 6f6e 3d4e 6f6e 652c 0a20 2020 2020 2020  on=None,.       
-00008750: 2066 7265 7175 656e 6379 5f73 6361 6c65   frequency_scale
-00008760: 5f66 6163 746f 723d 4e6f 6e65 2c0a 2020  _factor=None,.  
-00008770: 2020 2020 2020 7379 6d6d 6574 7269 7a65        symmetrize
-00008780: 5f66 6333 713a 2062 6f6f 6c20 3d20 4661  _fc3q: bool = Fa
-00008790: 6c73 652c 0a20 2020 2020 2020 206c 6170  lse,.        lap
-000087a0: 6163 6b5f 7a68 6565 765f 7570 6c6f 3d22  ack_zheev_uplo="
-000087b0: 4c22 2c0a 2020 2020 2020 2020 6f70 656e  L",.        open
-000087c0: 6d70 5f70 6572 5f74 7269 706c 6574 733d  mp_per_triplets=
-000087d0: 4e6f 6e65 2c0a 2020 2020 293a 0a20 2020  None,.    ):.   
-000087e0: 2020 2020 2022 2222 496e 6974 6961 6c69       """Initiali
-000087f0: 7a65 2070 682d 7068 2069 6e74 6572 6163  ze ph-ph interac
-00008800: 7469 6f6e 2063 616c 6375 6c61 7469 6f6e  tion calculation
-00008810: 2e0a 0a20 2020 2020 2020 2054 6869 7320  ...        This 
-00008820: 6d65 7468 6f64 2063 7265 6174 6573 2061  method creates a
-00008830: 6e20 696e 7374 616e 6365 206f 6620 496e  n instance of In
-00008840: 7465 7261 6374 696f 6e20 636c 6173 732c  teraction class,
-00008850: 2077 6869 6368 0a20 2020 2020 2020 2069   which.        i
-00008860: 7320 6e65 6365 7373 6172 7920 746f 2072  s necessary to r
-00008870: 756e 2070 682d 7068 2069 6e74 6572 6163  un ph-ph interac
-00008880: 7469 6f6e 2063 616c 6375 6c61 7469 6f6e  tion calculation
-00008890: 2e0a 2020 2020 2020 2020 5468 6520 696e  ..        The in
-000088a0: 7075 7420 6461 7461 2073 7563 6820 6173  put data such as
-000088b0: 2067 7269 6473 2c20 666f 7263 6520 636f   grids, force co
-000088c0: 6e73 7461 6e74 732c 2065 7463 2c20 6172  nstants, etc, ar
-000088d0: 650a 2020 2020 2020 2020 7374 6f72 6564  e.        stored
-000088e0: 2074 6f20 6265 2072 6561 6479 2066 6f72   to be ready for
-000088f0: 2074 6865 2063 616c 6375 6c61 7469 6f6e   the calculation
-00008900: 2e0a 0a20 2020 2020 2020 204e 6f74 650a  ...        Note.
-00008910: 2020 2020 2020 2020 2d2d 2d2d 0a20 2020          ----.   
-00008920: 2020 2020 2066 6333 2061 6e64 2066 6332       fc3 and fc2
-00008930: 2c20 616e 6420 6f70 7469 6f6e 616c 6c79  , and optionally
-00008940: 206e 6163 5f70 6172 616d 7320 6861 7665   nac_params have
-00008950: 2074 6f20 6265 2073 6574 2062 6566 6f72   to be set befor
-00008960: 6520 6361 6c6c 696e 670a 2020 2020 2020  e calling.      
-00008970: 2020 7468 6973 206d 6574 686f 642e 2066    this method. f
-00008980: 6333 2061 6e64 2066 6332 2063 616e 2062  c3 and fc2 can b
-00008990: 6520 6d61 6465 2065 6974 6865 7220 6672  e made either fr
-000089a0: 6f6d 2073 6574 7320 6f66 2066 6f72 6365  om sets of force
-000089b0: 730a 2020 2020 2020 2020 616e 6420 6469  s.        and di
-000089c0: 7370 6c61 6365 6d65 6e74 7320 6f66 2073  splacements of s
-000089d0: 7570 6572 6365 6c6c 7320 6f72 2062 6520  upercells or be 
-000089e0: 7365 7420 7369 6d70 6c79 2076 6961 2061  set simply via a
-000089f0: 7474 7269 6275 7465 732e 0a0a 2020 2020  ttributes...    
-00008a00: 2020 2020 5061 7261 6d65 7465 7273 0a20      Parameters. 
-00008a10: 2020 2020 2020 202d 2d2d 2d2d 2d2d 2d2d         ---------
-00008a20: 2d0a 2020 2020 2020 2020 6e61 635f 715f  -.        nac_q_
-00008a30: 6469 7265 6374 696f 6e20 3a20 6172 7261  direction : arra
-00008a40: 795f 6c69 6b65 2c20 6f70 7469 6f6e 616c  y_like, optional
-00008a50: 0a20 2020 2020 2020 2020 2020 2044 6972  .            Dir
-00008a60: 6563 7469 6f6e 206f 6620 712d 7665 6374  ection of q-vect
-00008a70: 6f72 2077 6174 6368 696e 6720 6672 6f6d  or watching from
-00008a80: 2047 616d 6d61 2070 6f69 6e74 2075 7365   Gamma point use
-00008a90: 6420 666f 720a 2020 2020 2020 2020 2020  d for.          
-00008aa0: 2020 6e6f 6e2d 616e 616c 7974 6963 616c    non-analytical
-00008ab0: 2074 6572 6d20 636f 7272 6563 7469 6f6e   term correction
-00008ac0: 2e20 5468 6973 2069 7320 6566 6665 6374  . This is effect
-00008ad0: 6976 6520 6f6e 6c79 2061 7420 713d 300a  ive only at q=0.
-00008ae0: 2020 2020 2020 2020 2020 2020 2870 6879              (phy
-00008af0: 7369 6361 6c6c 7920 712d 3e30 292e 2054  sically q->0). T
-00008b00: 6865 2064 6972 6563 7469 6f6e 2069 7320  he direction is 
-00008b10: 6769 7665 6e20 696e 2063 7279 7374 616c  given in crystal
-00008b20: 6c6f 6772 6170 6869 630a 2020 2020 2020  lographic.      
-00008b30: 2020 2020 2020 2866 7261 6374 696f 6e61        (fractiona
-00008b40: 6c29 2063 6f6f 7264 696e 6174 6573 2e0a  l) coordinates..
-00008b50: 2020 2020 2020 2020 2020 2020 7368 6170              shap
-00008b60: 653d 2833 2c29 2c20 6474 7970 653d 2764  e=(3,), dtype='d
-00008b70: 6f75 626c 6527 2e0a 2020 2020 2020 2020  ouble'..        
-00008b80: 2020 2020 4465 6661 756c 7420 7661 6c75      Default valu
-00008b90: 6520 6973 204e 6f6e 652c 2077 6869 6368  e is None, which
-00008ba0: 206d 6561 6e73 2074 6869 7320 6665 6174   means this feat
-00008bb0: 7572 6520 6973 206e 6f74 2075 7365 642e  ure is not used.
-00008bc0: 0a20 2020 2020 2020 2063 6f6e 7374 616e  .        constan
-00008bd0: 745f 6176 6572 6167 6564 5f69 6e74 6572  t_averaged_inter
-00008be0: 6163 7469 6f6e 203a 2066 6c6f 6174 2c20  action : float, 
-00008bf0: 6f70 7469 6f6e 616c 0a20 2020 2020 2020  optional.       
-00008c00: 2020 2020 2050 682d 7068 2069 6e74 6572       Ph-ph inter
-00008c10: 6163 7469 6f6e 2073 7472 656e 6774 6820  action strength 
-00008c20: 6172 7261 7920 6973 2072 6570 6c61 6365  array is replace
-00008c30: 6420 6279 2061 2073 6361 6c61 7220 7661  d by a scalar va
-00008c40: 6c75 652e 0a20 2020 2020 2020 2020 2020  lue..           
-00008c50: 2044 6566 6175 6c74 2069 7320 4e6f 6e65   Default is None
-00008c60: 2c20 7768 6963 6820 6d65 616e 7320 7468  , which means th
-00008c70: 6973 2066 6561 7475 7265 2069 7320 6e6f  is feature is no
-00008c80: 7420 7573 6564 2e0a 2020 2020 2020 2020  t used..        
-00008c90: 6672 6571 7565 6e63 795f 7363 616c 655f  frequency_scale_
-00008ca0: 6661 6374 6f72 203a 2066 6c6f 6174 2c20  factor : float, 
-00008cb0: 6f70 7469 6f6e 616c 0a20 2020 2020 2020  optional.       
-00008cc0: 2020 2020 2041 6c6c 2070 686f 6e6f 6e20       All phonon 
-00008cd0: 6672 6571 7565 6e63 6573 2061 7265 2073  frequences are s
-00008ce0: 6361 6c65 6420 6279 2074 6869 7320 7661  caled by this va
-00008cf0: 6c75 652e 2044 6566 6175 6c74 2069 7320  lue. Default is 
-00008d00: 4e6f 6e65 2c0a 2020 2020 2020 2020 2020  None,.          
-00008d10: 2020 7768 6963 6820 6d65 616e 7320 7068    which means ph
-00008d20: 6f6e 6f6e 2066 7265 7175 656e 6369 6573  onon frequencies
-00008d30: 2061 7265 206e 6f74 2073 6361 6c65 642e   are not scaled.
-00008d40: 0a20 2020 2020 2020 2073 796d 6d65 7472  .        symmetr
-00008d50: 697a 655f 6663 3371 203a 2062 6f6f 6c2c  ize_fc3q : bool,
-00008d60: 206f 7074 696f 6e61 6c0a 2020 2020 2020   optional.      
-00008d70: 2020 2020 2020 6663 3320 696e 2070 686f        fc3 in pho
-00008d80: 6e6f 6e20 7370 6163 6520 6973 2073 796d  non space is sym
-00008d90: 6d65 7472 697a 6564 2062 7920 7065 726d  metrized by perm
-00008da0: 7574 6174 696f 6e20 7379 6d6d 6574 7279  utation symmetry
-00008db0: 2e0a 2020 2020 2020 2020 2020 2020 4465  ..            De
-00008dc0: 6661 756c 7420 6973 2046 616c 7365 2e0a  fault is False..
-00008dd0: 2020 2020 2020 2020 6c61 7061 636b 5f7a          lapack_z
-00008de0: 6865 6576 5f75 706c 6f20 3a20 7374 722c  heev_uplo : str,
-00008df0: 206f 7074 696f 6e61 6c0a 2020 2020 2020   optional.      
-00008e00: 2020 2020 2020 274c 2720 6f72 2027 5527        'L' or 'U'
-00008e10: 2e20 4465 6661 756c 7420 6973 2027 4c27  . Default is 'L'
-00008e20: 2e20 5468 6973 2069 7320 7061 7373 6564  . This is passed
-00008e30: 2074 6f20 4c41 5041 434b 207a 6865 6576   to LAPACK zheev
-00008e40: 0a20 2020 2020 2020 2020 2020 2075 7365  .            use
-00008e50: 6420 666f 7220 7068 6f6e 6f6e 2073 6f6c  d for phonon sol
-00008e60: 7665 722e 0a20 2020 2020 2020 206f 7065  ver..        ope
-00008e70: 6e6d 705f 7065 725f 7472 6970 6c65 7473  nmp_per_triplets
-00008e80: 203a 2062 6f6f 6c20 6f72 204e 6f6e 652c   : bool or None,
-00008e90: 206f 7074 696f 6e61 6c2c 2064 6566 6175   optional, defau
-00008ea0: 6c74 2069 7320 4e6f 6e65 0a20 2020 2020  lt is None.     
-00008eb0: 2020 2020 2020 204e 6f72 6d61 6c6c 7920         Normally 
-00008ec0: 7468 6973 2070 6172 616d 6574 6572 2073  this parameter s
-00008ed0: 686f 756c 6420 6e6f 7420 6265 2074 6f75  hould not be tou
-00008ee0: 6368 6564 2e0a 2020 2020 2020 2020 2020  ched..          
-00008ef0: 2020 5768 656e 2060 5472 7565 602c 2070    When `True`, p
-00008f00: 682d 7068 2069 6e74 6572 6163 7469 6f6e  h-ph interaction
-00008f10: 2073 7472 656e 6774 6820 6361 6c63 756c   strength calcul
-00008f20: 6174 696f 6e20 7275 6e73 2077 6974 680a  ation runs with.
-00008f30: 2020 2020 2020 2020 2020 2020 4f70 656e              Open
-00008f40: 4d50 2064 6973 7472 6962 7574 696f 6e20  MP distribution 
-00008f50: 6f76 6572 2074 7269 706c 6574 732c 2061  over triplets, a
-00008f60: 6e64 206f 7665 7220 6261 6e64 7320 7768  nd over bands wh
-00008f70: 656e 2060 4661 6c73 6560 2e0a 2020 2020  en `False`..    
-00008f80: 2020 2020 2020 2020 604e 6f6e 6560 2077          `None` w
-00008f90: 696c 6c20 6368 6f6f 7365 206f 6e65 206f  ill choose one o
-00008fa0: 6620 7468 656d 2061 7574 6f6d 6174 6963  f them automatic
-00008fb0: 616c 6c79 2e0a 0a20 2020 2020 2020 2022  ally...        "
-00008fc0: 2222 0a20 2020 2020 2020 2069 6620 7365  "".        if se
-00008fd0: 6c66 2e6d 6573 685f 6e75 6d62 6572 7320  lf.mesh_numbers 
-00008fe0: 6973 204e 6f6e 653a 0a20 2020 2020 2020  is None:.       
-00008ff0: 2020 2020 206d 7367 203d 2022 5068 6f6e       msg = "Phon
-00009000: 6f33 7079 2e6d 6573 685f 6e75 6d62 6572  o3py.mesh_number
-00009010: 7320 6f66 2069 6e73 7461 6e63 6520 6861  s of instance ha
-00009020: 7320 746f 2062 6520 7365 742e 220a 2020  s to be set.".  
-00009030: 2020 2020 2020 2020 2020 7261 6973 6520            raise 
-00009040: 5275 6e74 696d 6545 7272 6f72 286d 7367  RuntimeError(msg
-00009050: 290a 0a20 2020 2020 2020 2069 6620 7365  )..        if se
-00009060: 6c66 2e5f 6663 3220 6973 204e 6f6e 653a  lf._fc2 is None:
-00009070: 0a20 2020 2020 2020 2020 2020 206d 7367  .            msg
-00009080: 203d 2022 5068 6f6e 6f33 7079 2e66 6332   = "Phono3py.fc2
-00009090: 206f 6620 696e 7374 616e 6365 2069 7320   of instance is 
-000090a0: 6e6f 7420 666f 756e 642e 220a 2020 2020  not found.".    
-000090b0: 2020 2020 2020 2020 7261 6973 6520 5275          raise Ru
-000090c0: 6e74 696d 6545 7272 6f72 286d 7367 290a  ntimeError(msg).
-000090d0: 0a20 2020 2020 2020 2073 656c 662e 5f69  .        self._i
-000090e0: 6e74 6572 6163 7469 6f6e 203d 2049 6e74  nteraction = Int
-000090f0: 6572 6163 7469 6f6e 280a 2020 2020 2020  eraction(.      
-00009100: 2020 2020 2020 7365 6c66 2e5f 7072 696d        self._prim
-00009110: 6974 6976 652c 0a20 2020 2020 2020 2020  itive,.         
-00009120: 2020 2073 656c 662e 5f62 7a5f 6772 6964     self._bz_grid
-00009130: 2c0a 2020 2020 2020 2020 2020 2020 7365  ,.            se
-00009140: 6c66 2e5f 7072 696d 6974 6976 655f 7379  lf._primitive_sy
-00009150: 6d6d 6574 7279 2c0a 2020 2020 2020 2020  mmetry,.        
-00009160: 2020 2020 6663 333d 7365 6c66 2e5f 6663      fc3=self._fc
-00009170: 332c 0a20 2020 2020 2020 2020 2020 2062  3,.            b
-00009180: 616e 645f 696e 6469 6365 733d 7365 6c66  and_indices=self
-00009190: 2e5f 6261 6e64 5f69 6e64 6963 6573 5f66  ._band_indices_f
-000091a0: 6c61 7474 656e 2c0a 2020 2020 2020 2020  latten,.        
-000091b0: 2020 2020 636f 6e73 7461 6e74 5f61 7665      constant_ave
-000091c0: 7261 6765 645f 696e 7465 7261 6374 696f  raged_interactio
-000091d0: 6e3d 636f 6e73 7461 6e74 5f61 7665 7261  n=constant_avera
-000091e0: 6765 645f 696e 7465 7261 6374 696f 6e2c  ged_interaction,
-000091f0: 0a20 2020 2020 2020 2020 2020 2066 7265  .            fre
-00009200: 7175 656e 6379 5f66 6163 746f 725f 746f  quency_factor_to
-00009210: 5f54 487a 3d73 656c 662e 5f66 7265 7175  _THz=self._frequ
-00009220: 656e 6379 5f66 6163 746f 725f 746f 5f54  ency_factor_to_T
-00009230: 487a 2c0a 2020 2020 2020 2020 2020 2020  Hz,.            
-00009240: 6672 6571 7565 6e63 795f 7363 616c 655f  frequency_scale_
-00009250: 6661 6374 6f72 3d66 7265 7175 656e 6379  factor=frequency
-00009260: 5f73 6361 6c65 5f66 6163 746f 722c 0a20  _scale_factor,. 
-00009270: 2020 2020 2020 2020 2020 2063 7574 6f66             cutof
-00009280: 665f 6672 6571 7565 6e63 793d 7365 6c66  f_frequency=self
-00009290: 2e5f 6375 746f 6666 5f66 7265 7175 656e  ._cutoff_frequen
-000092a0: 6379 2c0a 2020 2020 2020 2020 2020 2020  cy,.            
-000092b0: 6973 5f6d 6573 685f 7379 6d6d 6574 7279  is_mesh_symmetry
-000092c0: 3d73 656c 662e 5f69 735f 6d65 7368 5f73  =self._is_mesh_s
-000092d0: 796d 6d65 7472 792c 0a20 2020 2020 2020  ymmetry,.       
-000092e0: 2020 2020 2073 796d 6d65 7472 697a 655f       symmetrize_
-000092f0: 6663 3371 3d73 796d 6d65 7472 697a 655f  fc3q=symmetrize_
-00009300: 6663 3371 2c0a 2020 2020 2020 2020 2020  fc3q,.          
-00009310: 2020 6d61 6b65 5f72 305f 6176 6572 6167    make_r0_averag
-00009320: 653d 7365 6c66 2e5f 6d61 6b65 5f72 305f  e=self._make_r0_
-00009330: 6176 6572 6167 652c 0a20 2020 2020 2020  average,.       
-00009340: 2020 2020 206c 6170 6163 6b5f 7a68 6565       lapack_zhee
-00009350: 765f 7570 6c6f 3d6c 6170 6163 6b5f 7a68  v_uplo=lapack_zh
-00009360: 6565 765f 7570 6c6f 2c0a 2020 2020 2020  eev_uplo,.      
-00009370: 2020 2020 2020 6f70 656e 6d70 5f70 6572        openmp_per
-00009380: 5f74 7269 706c 6574 733d 6f70 656e 6d70  _triplets=openmp
-00009390: 5f70 6572 5f74 7269 706c 6574 732c 0a20  _per_triplets,. 
-000093a0: 2020 2020 2020 2029 0a20 2020 2020 2020         ).       
-000093b0: 2073 656c 662e 5f69 6e74 6572 6163 7469   self._interacti
-000093c0: 6f6e 2e6e 6163 5f71 5f64 6972 6563 7469  on.nac_q_directi
-000093d0: 6f6e 203d 206e 6163 5f71 5f64 6972 6563  on = nac_q_direc
-000093e0: 7469 6f6e 0a20 2020 2020 2020 2073 656c  tion.        sel
-000093f0: 662e 5f69 6e69 745f 6479 6e61 6d69 6361  f._init_dynamica
-00009400: 6c5f 6d61 7472 6978 2829 0a0a 2020 2020  l_matrix()..    
-00009410: 6465 6620 7365 745f 7068 6f6e 6f6e 5f64  def set_phonon_d
-00009420: 6174 6128 7365 6c66 2c20 6672 6571 7565  ata(self, freque
-00009430: 6e63 6965 732c 2065 6967 656e 7665 6374  ncies, eigenvect
-00009440: 6f72 732c 2067 7269 645f 6164 6472 6573  ors, grid_addres
-00009450: 7329 3a0a 2020 2020 2020 2020 2222 2253  s):.        """S
-00009460: 6574 2070 686f 6e6f 6e20 6672 6571 7565  et phonon freque
-00009470: 6e63 6965 7320 616e 6420 6569 6765 6e76  ncies and eigenv
-00009480: 6563 746f 7273 2069 6e20 496e 7465 7261  ectors in Intera
-00009490: 6374 696f 6e20 696e 7374 616e 6365 2e0a  ction instance..
-000094a0: 0a20 2020 2020 2020 2048 6172 6d6f 6e69  .        Harmoni
-000094b0: 6320 7068 6f6e 6f6e 2069 6e66 6f72 6d61  c phonon informa
-000094c0: 7469 6f6e 2069 7320 7374 6f72 6564 2069  tion is stored i
-000094d0: 6e20 496e 7465 7261 6374 696f 6e20 696e  n Interaction in
-000094e0: 7374 616e 6365 2e20 466f 720a 2020 2020  stance. For.    
-000094f0: 2020 2020 6578 616d 706c 652c 2074 6869      example, thi
-00009500: 7320 696e 666f 726d 6174 696f 6e20 7374  s information st
-00009510: 6f72 6520 696e 2061 2066 696c 6520 6973  ore in a file is
-00009520: 2072 6561 6420 616e 6420 7061 7373 6564   read and passed
-00009530: 2074 6f0a 2020 2020 2020 2020 5068 6f6e   to.        Phon
-00009540: 6f33 7079 2069 6e73 7461 6e63 6520 6279  o3py instance by
-00009550: 2075 7369 6e67 2074 6869 7320 6d65 7468   using this meth
-00009560: 6f64 2e20 5468 6520 6772 6964 5f61 6464  od. The grid_add
-00009570: 7265 7373 2069 7320 7573 6564 0a20 2020  ress is used.   
-00009580: 2020 2020 2066 6f72 2074 6865 2063 6f6e       for the con
-00009590: 7369 7374 656e 6379 2063 6865 636b 2e0a  sistency check..
-000095a0: 0a20 2020 2020 2020 2050 6172 616d 6574  .        Paramet
-000095b0: 6572 730a 2020 2020 2020 2020 2d2d 2d2d  ers.        ----
-000095c0: 2d2d 2d2d 2d2d 0a20 2020 2020 2020 2066  ------.        f
-000095d0: 7265 7175 656e 6369 6573 203a 2061 7272  requencies : arr
-000095e0: 6179 5f6c 696b 650a 2020 2020 2020 2020  ay_like.        
-000095f0: 2020 2020 5068 6f6e 6f6e 2066 7265 7175      Phonon frequ
-00009600: 656e 6369 6573 2e0a 2020 2020 2020 2020  encies..        
-00009610: 2020 2020 7368 6170 653d 286e 756d 5f67      shape=(num_g
-00009620: 7269 645f 706f 696e 7473 2c20 6e75 6d5f  rid_points, num_
-00009630: 6261 6e64 292c 2064 7479 7065 3d27 646f  band), dtype='do
-00009640: 7562 6c65 272c 206f 7264 6572 3d27 4327  uble', order='C'
-00009650: 0a20 2020 2020 2020 2065 6967 656e 7665  .        eigenve
-00009660: 6374 6f72 7320 3a20 6172 7261 795f 6c69  ctors : array_li
-00009670: 6b65 0a20 2020 2020 2020 2020 2020 2050  ke.            P
-00009680: 686f 6e6f 6e20 6569 6765 6e76 6563 746f  honon eigenvecto
-00009690: 7273 0a20 2020 2020 2020 2020 2020 2073  rs.            s
-000096a0: 6861 7065 3d28 6e75 6d5f 6772 6964 5f70  hape=(num_grid_p
-000096b0: 6f69 6e74 732c 206e 756d 5f62 616e 642c  oints, num_band,
-000096c0: 206e 756d 5f62 616e 6429 0a20 2020 2020   num_band).     
-000096d0: 2020 2020 2020 2064 7479 7065 3d27 636f         dtype='co
-000096e0: 6d70 6c65 7831 3238 272c 206f 7264 6572  mplex128', order
-000096f0: 3d27 4327 0a20 2020 2020 2020 2067 7269  ='C'.        gri
-00009700: 645f 6164 6472 6573 7320 3a20 6172 7261  d_address : arra
-00009710: 795f 6c69 6b65 0a20 2020 2020 2020 2020  y_like.         
-00009720: 2020 2047 7269 6420 706f 696e 7420 6164     Grid point ad
-00009730: 6472 6573 7365 7320 6279 2069 6e74 6567  dresses by integ
-00009740: 6572 732e 2054 6865 2066 6972 7374 2064  ers. The first d
-00009750: 696d 656e 7369 6f6e 206d 6179 206e 6f74  imension may not
-00009760: 2062 650a 2020 2020 2020 2020 2020 2020   be.            
-00009770: 7072 6f64 286d 6573 6829 2062 6563 6175  prod(mesh) becau
-00009780: 7365 2069 7420 696e 636c 7564 6573 2042  se it includes B
-00009790: 7269 6c6c 6f75 696e 207a 6f6e 6520 626f  rillouin zone bo
-000097a0: 756e 6461 7279 2e20 5468 6520 6465 7461  undary. The deta
-000097b0: 696c 0a20 2020 2020 2020 2020 2020 2069  il.            i
-000097c0: 7320 666f 756e 6420 696e 2074 6865 2064  s found in the d
-000097d0: 6f63 7374 7269 6e67 206f 660a 2020 2020  ocstring of.    
-000097e0: 2020 2020 2020 2020 7068 6f6e 6f33 7079          phono3py
-000097f0: 2e70 686f 6e6f 6e33 2e74 7269 706c 6574  .phonon3.triplet
-00009800: 732e 6765 745f 7472 6970 6c65 7473 5f61  s.get_triplets_a
-00009810: 745f 712e 0a20 2020 2020 2020 2020 2020  t_q..           
-00009820: 2073 6861 7065 3d28 6e75 6d5f 6772 6964   shape=(num_grid
-00009830: 5f70 6f69 6e74 732c 2033 292c 2064 7479  _points, 3), dty
-00009840: 7065 3d69 6e74 0a0a 2020 2020 2020 2020  pe=int..        
-00009850: 2222 220a 2020 2020 2020 2020 6966 2073  """.        if s
-00009860: 656c 662e 5f69 6e74 6572 6163 7469 6f6e  elf._interaction
-00009870: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
-00009880: 2020 2020 2020 2020 2020 7365 6c66 2e5f            self._
-00009890: 696e 7465 7261 6374 696f 6e2e 7365 745f  interaction.set_
-000098a0: 7068 6f6e 6f6e 5f64 6174 6128 6672 6571  phonon_data(freq
-000098b0: 7565 6e63 6965 732c 2065 6967 656e 7665  uencies, eigenve
-000098c0: 6374 6f72 732c 2067 7269 645f 6164 6472  ctors, grid_addr
-000098d0: 6573 7329 0a0a 2020 2020 6465 6620 6765  ess)..    def ge
-000098e0: 745f 7068 6f6e 6f6e 5f64 6174 6128 7365  t_phonon_data(se
-000098f0: 6c66 293a 0a20 2020 2020 2020 2022 2222  lf):.        """
-00009900: 4765 7420 7068 6f6e 6f6e 2066 7265 7175  Get phonon frequ
-00009910: 656e 6369 6573 2061 6e64 2065 6967 656e  encies and eigen
-00009920: 7665 6374 6f72 7320 696e 2049 6e74 6572  vectors in Inter
-00009930: 6163 7469 6f6e 2069 6e73 7461 6e63 652e  action instance.
-00009940: 0a0a 2020 2020 2020 2020 4861 726d 6f6e  ..        Harmon
-00009950: 6963 2070 686f 6e6f 6e20 696e 666f 726d  ic phonon inform
-00009960: 6174 696f 6e20 6973 2073 746f 7265 6420  ation is stored 
-00009970: 696e 2049 6e74 6572 6163 7469 6f6e 2069  in Interaction i
-00009980: 6e73 7461 6e63 652e 2054 6869 730a 2020  nstance. This.  
-00009990: 2020 2020 2020 696e 666f 726d 6174 696f        informatio
-000099a0: 6e20 6361 6e20 6265 206f 6274 6169 6e65  n can be obtaine
-000099b0: 642e 2054 6865 2067 7269 645f 6164 6472  d. The grid_addr
-000099c0: 6573 7320 7265 7475 726e 6564 2067 6976  ess returned giv
-000099d0: 6520 7468 650a 2020 2020 2020 2020 712d  e the.        q-
-000099e0: 706f 696e 7473 206c 6f63 6174 696f 6e73  points locations
-000099f0: 2077 6974 6820 7265 7370 6563 7420 746f   with respect to
-00009a00: 2072 6563 6970 726f 6361 6c20 6261 7369   reciprocal basi
-00009a10: 7320 7665 6374 6f72 7320 6279 0a20 2020  s vectors by.   
-00009a20: 2020 2020 2069 6e74 6567 6572 7320 696e       integers in
-00009a30: 2074 6865 2077 6179 2074 6861 740a 2020   the way that.  
-00009a40: 2020 2020 2020 2020 2020 715f 706f 696e            q_poin
-00009a50: 7473 203d 2067 7269 645f 6164 6472 6573  ts = grid_addres
-00009a60: 7320 2f20 6e70 2e61 7272 6179 286d 6573  s / np.array(mes
-00009a70: 682c 2064 7479 7065 3d27 646f 7562 6c65  h, dtype='double
-00009a80: 2729 2e0a 0a20 2020 2020 2020 2052 6574  ')...        Ret
-00009a90: 7572 6e73 0a20 2020 2020 2020 202d 2d2d  urns.        ---
-00009aa0: 2d2d 2d2d 0a20 2020 2020 2020 2074 7570  ----.        tup
-00009ab0: 6c65 0a20 2020 2020 2020 2020 2020 2028  le.            (
-00009ac0: 6672 6571 7565 6e63 6965 732c 2065 6967  frequencies, eig
-00009ad0: 656e 7665 6374 6f72 732c 2067 7269 645f  envectors, grid_
-00009ae0: 6164 6472 6573 7329 0a20 2020 2020 2020  address).       
-00009af0: 2020 2020 2053 6565 206d 6f72 6520 6465       See more de
-00009b00: 7461 696c 7320 6174 2074 6865 2064 6f63  tails at the doc
-00009b10: 7374 7269 6e67 206f 6620 7365 745f 7068  string of set_ph
-00009b20: 6f6e 6f6e 5f64 6174 612e 0a0a 2020 2020  onon_data...    
-00009b30: 2020 2020 2222 220a 2020 2020 2020 2020      """.        
-00009b40: 6966 2073 656c 662e 5f69 6e74 6572 6163  if self._interac
-00009b50: 7469 6f6e 2069 7320 6e6f 7420 4e6f 6e65  tion is not None
-00009b60: 3a0a 2020 2020 2020 2020 2020 2020 6672  :.            fr
-00009b70: 6571 732c 2065 6967 7665 6373 2c20 5f20  eqs, eigvecs, _ 
-00009b80: 3d20 7365 6c66 2e5f 696e 7465 7261 6374  = self._interact
-00009b90: 696f 6e2e 6765 745f 7068 6f6e 6f6e 7328  ion.get_phonons(
-00009ba0: 290a 2020 2020 2020 2020 2020 2020 7265  ).            re
-00009bb0: 7475 726e 2066 7265 7173 2c20 6569 6776  turn freqs, eigv
-00009bc0: 6563 732c 2073 656c 662e 5f69 6e74 6572  ecs, self._inter
-00009bd0: 6163 7469 6f6e 2e62 7a5f 6772 6964 2e61  action.bz_grid.a
-00009be0: 6464 7265 7373 6573 0a20 2020 2020 2020  ddresses.       
-00009bf0: 2065 6c73 653a 0a20 2020 2020 2020 2020   else:.         
-00009c00: 2020 206d 7367 203d 2028 0a20 2020 2020     msg = (.     
-00009c10: 2020 2020 2020 2020 2020 2022 5068 6f6e             "Phon
-00009c20: 6f33 7079 2e69 6e69 745f 7068 7068 5f69  o3py.init_phph_i
-00009c30: 6e74 6572 6163 7469 6f6e 2068 6173 2074  nteraction has t
-00009c40: 6f20 6265 2063 616c 6c65 6420 220a 2020  o be called ".  
-00009c50: 2020 2020 2020 2020 2020 2020 2020 2262                "b
-00009c60: 6566 6f72 6520 7275 6e6e 696e 6720 7468  efore running th
-00009c70: 6973 206d 6574 686f 642e 220a 2020 2020  is method.".    
-00009c80: 2020 2020 2020 2020 290a 2020 2020 2020          ).      
-00009c90: 2020 2020 2020 7261 6973 6520 5275 6e74        raise Runt
-00009ca0: 696d 6545 7272 6f72 286d 7367 290a 0a20  imeError(msg).. 
-00009cb0: 2020 2064 6566 2072 756e 5f70 686f 6e6f     def run_phono
-00009cc0: 6e5f 736f 6c76 6572 2873 656c 662c 2067  n_solver(self, g
-00009cd0: 7269 645f 706f 696e 7473 3d4e 6f6e 6529  rid_points=None)
-00009ce0: 3a0a 2020 2020 2020 2020 2222 2252 756e  :.        """Run
-00009cf0: 2068 6172 6d6f 6e69 6320 7068 6f6e 6f6e   harmonic phonon
-00009d00: 2063 616c 6375 6c61 7469 6f6e 206f 6e20   calculation on 
-00009d10: 6772 6964 2070 6f69 6e74 732e 0a0a 2020  grid points...  
-00009d20: 2020 2020 2020 5061 7261 6d65 7465 7273        Parameters
-00009d30: 0a20 2020 2020 2020 202d 2d2d 2d2d 2d2d  .        -------
-00009d40: 2d2d 2d0a 2020 2020 2020 2020 6772 6964  ---.        grid
-00009d50: 5f70 6f69 6e74 7320 3a20 6172 7261 795f  _points : array_
-00009d60: 6c69 6b65 206f 7220 4e6f 6e65 2c20 6f70  like or None, op
-00009d70: 7469 6f6e 616c 0a20 2020 2020 2020 2020  tional.         
-00009d80: 2020 2041 206c 6973 7420 6f66 2067 7269     A list of gri
-00009d90: 6420 706f 696e 7420 696e 6469 6365 7320  d point indices 
-00009da0: 6f66 2050 686f 6e6f 3370 792e 6772 6964  of Phono3py.grid
-00009db0: 2e61 6464 7265 7373 6573 2e0a 2020 2020  .addresses..    
-00009dc0: 2020 2020 2020 2020 5370 6563 6966 7969          Specifyi
-00009dd0: 6e67 204e 6f6e 6520 7275 6e73 2061 6c6c  ng None runs all
-00009de0: 2070 686f 6e6f 6e73 206f 6e20 7468 6520   phonons on the 
-00009df0: 6772 6964 2070 6f69 6e74 7320 756e 6c65  grid points unle
-00009e00: 7373 0a20 2020 2020 2020 2020 2020 2074  ss.            t
-00009e10: 686f 7365 2070 686f 6e6f 6e73 2077 6572  hose phonons wer
-00009e20: 6520 616c 7265 6164 7920 6361 6c63 756c  e already calcul
-00009e30: 6174 6564 2e20 4e6f 726d 616c 6c79 2070  ated. Normally p
-00009e40: 686f 6e6f 6e73 2061 740a 2020 2020 2020  honons at.      
-00009e50: 2020 2020 2020 5b30 2c20 302c 2030 5d20        [0, 0, 0] 
-00009e60: 706f 696e 7420 6973 2061 6c72 6561 6479  point is already
-00009e70: 2063 616c 6375 6c61 7465 6420 6265 666f   calculated befo
-00009e80: 7265 2063 616c 6c69 6e67 2074 6869 7320  re calling this 
-00009e90: 6d65 7468 6f64 2e0a 2020 2020 2020 2020  method..        
-00009ea0: 2020 2020 5068 6f6e 6f6e 2063 616c 6375      Phonon calcu
-00009eb0: 6c61 7469 6f6e 7320 6172 6520 7065 7266  lations are perf
-00009ec0: 6f72 6d65 6420 6175 746f 6d61 7469 6361  ormed automatica
-00009ed0: 6c6c 7920 7768 656e 206e 6565 6465 640a  lly when needed.
-00009ee0: 2020 2020 2020 2020 2020 2020 696e 7465              inte
-00009ef0: 726e 616c 6c79 2066 6f72 2070 682d 7068  rnally for ph-ph
-00009f00: 2063 616c 6375 6c61 7469 6f6e 2e20 5468   calculation. Th
-00009f10: 6572 6566 6f72 6520 6361 6c6c 696e 6720  erefore calling 
-00009f20: 7468 6973 206d 6574 686f 640a 2020 2020  this method.    
-00009f30: 2020 2020 2020 2020 6973 206e 6f74 206e          is not n
-00009f40: 6563 6573 7361 7279 2069 6e20 6d6f 7374  ecessary in most
-00009f50: 2063 6173 6573 2e0a 2020 2020 2020 2020   cases..        
-00009f60: 2020 2020 5468 6520 7068 6f6e 6f6e 2072      The phonon r
-00009f70: 6573 756c 7473 2061 7265 206f 6274 6169  esults are obtai
-00009f80: 6e65 6420 6279 2050 686f 6e6f 3370 792e  ned by Phono3py.
-00009f90: 6765 745f 7068 6f6e 6f6e 5f64 6174 6128  get_phonon_data(
-00009fa0: 292e 0a0a 2020 2020 2020 2020 2222 220a  )...        """.
-00009fb0: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
-00009fc0: 5f69 6e74 6572 6163 7469 6f6e 2069 7320  _interaction is 
-00009fd0: 6e6f 7420 4e6f 6e65 3a0a 2020 2020 2020  not None:.      
-00009fe0: 2020 2020 2020 7365 6c66 2e5f 696e 7465        self._inte
-00009ff0: 7261 6374 696f 6e2e 7275 6e5f 7068 6f6e  raction.run_phon
-0000a000: 6f6e 5f73 6f6c 7665 7228 6772 6964 5f70  on_solver(grid_p
-0000a010: 6f69 6e74 733d 6772 6964 5f70 6f69 6e74  oints=grid_point
-0000a020: 7329 0a20 2020 2020 2020 2065 6c73 653a  s).        else:
-0000a030: 0a20 2020 2020 2020 2020 2020 206d 7367  .            msg
-0000a040: 203d 2028 0a20 2020 2020 2020 2020 2020   = (.           
-0000a050: 2020 2020 2022 5068 6f6e 6f33 7079 2e69       "Phono3py.i
-0000a060: 6e69 745f 7068 7068 5f69 6e74 6572 6163  nit_phph_interac
-0000a070: 7469 6f6e 2068 6173 2074 6f20 6265 2063  tion has to be c
-0000a080: 616c 6c65 6420 220a 2020 2020 2020 2020  alled ".        
-0000a090: 2020 2020 2020 2020 2262 6566 6f72 6520          "before 
-0000a0a0: 7275 6e6e 696e 6720 7468 6973 206d 6574  running this met
-0000a0b0: 686f 642e 220a 2020 2020 2020 2020 2020  hod.".          
-0000a0c0: 2020 290a 2020 2020 2020 2020 2020 2020    ).            
-0000a0d0: 7261 6973 6520 5275 6e74 696d 6545 7272  raise RuntimeErr
-0000a0e0: 6f72 286d 7367 290a 0a20 2020 2064 6566  or(msg)..    def
-0000a0f0: 2067 656e 6572 6174 655f 6469 7370 6c61   generate_displa
-0000a100: 6365 6d65 6e74 7328 0a20 2020 2020 2020  cements(.       
-0000a110: 2073 656c 662c 0a20 2020 2020 2020 2064   self,.        d
-0000a120: 6973 7461 6e63 653d 302e 3033 2c0a 2020  istance=0.03,.  
-0000a130: 2020 2020 2020 6375 746f 6666 5f70 6169        cutoff_pai
-0000a140: 725f 6469 7374 616e 6365 3d4e 6f6e 652c  r_distance=None,
-0000a150: 0a20 2020 2020 2020 2069 735f 706c 7573  .        is_plus
-0000a160: 6d69 6e75 733d 2261 7574 6f22 2c0a 2020  minus="auto",.  
-0000a170: 2020 2020 2020 6973 5f64 6961 676f 6e61        is_diagona
-0000a180: 6c3d 5472 7565 2c0a 2020 2020 293a 0a20  l=True,.    ):. 
-0000a190: 2020 2020 2020 2022 2222 4765 6e65 7261         """Genera
-0000a1a0: 7465 2064 6973 706c 6163 656d 656e 7420  te displacement 
-0000a1b0: 6461 7461 7365 7420 696e 2073 7570 6572  dataset in super
-0000a1c0: 6365 6c6c 2066 6f72 2066 6333 2e0a 0a20  cell for fc3... 
-0000a1d0: 2020 2020 2020 2054 6869 7320 7379 7374         This syst
-0000a1e0: 656d 6174 6963 616c 6c79 2067 656e 6572  ematically gener
-0000a1f0: 6174 6573 2073 696e 676c 6520 616e 6420  ates single and 
-0000a200: 7061 6972 2061 746f 6d69 6320 6469 7370  pair atomic disp
-0000a210: 6c61 6365 6d65 6e74 730a 2020 2020 2020  lacements.      
-0000a220: 2020 696e 2073 7570 6572 6365 6c6c 7320    in supercells 
-0000a230: 746f 2063 616c 6375 6c61 7465 2066 6333  to calculate fc3
-0000a240: 2063 6f6e 7369 6465 7269 6e67 2063 7279   considering cry
-0000a250: 7374 616c 2073 796d 6d65 7472 792e 0a20  stal symmetry.. 
-0000a260: 2020 2020 2020 2057 6865 6e20 7468 6973         When this
-0000a270: 206d 6574 686f 6420 6973 2063 616c 6c65   method is calle
-0000a280: 642c 2065 7869 7374 696e 6720 6361 6368  d, existing cach
-0000a290: 6520 6f66 2073 7570 6572 6365 6c6c 7320  e of supercells 
-0000a2a0: 7769 7468 0a20 2020 2020 2020 2064 6973  with.        dis
-0000a2b0: 706c 6163 656d 656e 7473 2066 6f72 2066  placements for f
-0000a2c0: 6333 2061 7265 2072 656d 6f76 6564 2e0a  c3 are removed..
-0000a2d0: 0a20 2020 2020 2020 2046 6f72 2066 6333  .        For fc3
-0000a2e0: 2c20 7477 6f20 6174 6f6d 7320 6172 6520  , two atoms are 
-0000a2f0: 6469 7370 6c61 6365 6420 666f 7220 6561  displaced for ea
-0000a300: 6368 2063 6f6e 6669 6775 7261 7469 6f6e  ch configuration
-0000a310: 0a20 2020 2020 2020 2063 6f6e 7369 6465  .        conside
-0000a320: 7269 6e67 2063 7279 7374 616c 2073 796d  ring crystal sym
-0000a330: 6d65 7472 792e 2054 6865 2066 6972 7374  metry. The first
-0000a340: 2064 6973 706c 6163 656d 656e 7420 6973   displacement is
-0000a350: 2063 686f 7365 6e0a 2020 2020 2020 2020   chosen.        
-0000a360: 696e 2074 6865 2070 6572 6665 6374 2073  in the perfect s
-0000a370: 7570 6572 6365 6c6c 2c20 616e 6420 7468  upercell, and th
-0000a380: 6520 7365 636f 6e64 2064 6973 706c 6163  e second displac
-0000a390: 656d 656e 7420 696e 2074 6865 0a20 2020  ement in the.   
-0000a3a0: 2020 2020 2064 6973 706c 6163 6564 2073       displaced s
-0000a3b0: 7570 6572 6365 6c6c 2e20 5468 6520 6669  upercell. The fi
-0000a3c0: 7273 7420 6469 7370 6c61 6365 6d65 6e74  rst displacement
-0000a3d0: 7320 6172 6520 7461 6b65 6e20 616c 6f6e  s are taken alon
-0000a3e0: 670a 2020 2020 2020 2020 7468 6520 6261  g.        the ba
-0000a3f0: 7369 7320 7665 6374 6f72 7320 6f66 2074  sis vectors of t
-0000a400: 6865 2073 7570 6572 6365 6c6c 2e20 5468  he supercell. Th
-0000a410: 6973 2069 7320 6265 6361 7573 6520 7468  is is because th
-0000a420: 650a 2020 2020 2020 2020 7379 6d6d 6574  e.        symmet
-0000a430: 7279 2069 7320 6578 7065 6374 6564 2074  ry is expected t
-0000a440: 6f20 6265 206c 6573 7320 6272 6f6b 656e  o be less broken
-0000a450: 2062 7920 7468 6520 696e 7472 6f64 7563   by the introduc
-0000a460: 6564 2066 6972 7374 0a20 2020 2020 2020  ed first.       
-0000a470: 2064 6973 706c 6163 656d 656e 742c 2061   displacement, a
-0000a480: 6e64 2061 7320 7468 6520 7265 7375 6c74  nd as the result
-0000a490: 2c20 7468 6520 6e75 6d62 6572 206f 6620  , the number of 
-0000a4a0: 7365 636f 6e64 0a20 2020 2020 2020 2064  second.        d
-0000a4b0: 6973 706c 6163 656d 656e 7473 206d 6179  isplacements may
-0000a4c0: 2062 6563 6f6d 6520 736d 616c 6c65 7220   become smaller 
-0000a4d0: 7468 616e 2074 6865 2063 6173 6520 7468  than the case th
-0000a4e0: 6174 2074 6865 2066 6972 7374 0a20 2020  at the first.   
-0000a4f0: 2020 2020 2061 746f 6d20 6973 2064 6973       atom is dis
-0000a500: 706c 6163 6564 206e 6f74 2061 6c6f 6e67  placed not along
-0000a510: 2074 6865 2062 6173 6973 2076 6563 746f   the basis vecto
-0000a520: 7273 2e0a 0a20 2020 2020 2020 204e 6f74  rs...        Not
-0000a530: 650a 2020 2020 2020 2020 2d2d 2d2d 0a20  e.        ----. 
-0000a540: 2020 2020 2020 2057 6865 6e20 7068 6f6e         When phon
-0000a550: 6f6e 5f73 7570 6572 6365 6c6c 5f6d 6174  on_supercell_mat
-0000a560: 7269 7820 6973 206e 6f74 2067 6976 656e  rix is not given
-0000a570: 2c20 6663 3220 6973 2061 6c73 6f0a 2020  , fc2 is also.  
-0000a580: 2020 2020 2020 636f 6d70 7574 6564 2066        computed f
-0000a590: 726f 6d20 7468 6520 7361 6d65 2073 6574  rom the same set
-0000a5a0: 206f 6620 7468 6520 6469 7370 6c61 6365   of the displace
-0000a5b0: 6d65 6e74 7320 666f 7220 6663 3320 616e  ments for fc3 an
-0000a5c0: 640a 2020 2020 2020 2020 7265 7370 6563  d.        respec
-0000a5d0: 7469 7665 2073 7570 6572 6365 6c6c 2066  tive supercell f
-0000a5e0: 6f72 6365 732e 2057 6865 6e20 7068 6f6e  orces. When phon
-0000a5f0: 6f6e 5f73 7570 6572 6365 6c6c 5f6d 6174  on_supercell_mat
-0000a600: 7269 7820 6973 0a20 2020 2020 2020 2073  rix is.        s
-0000a610: 6574 2c20 7468 6520 6469 7370 6c61 6365  et, the displace
-0000a620: 6d65 6e74 7320 696e 2070 686f 6e6f 6e5f  ments in phonon_
-0000a630: 7375 7065 7263 656c 6c20 6172 6520 6765  supercell are ge
-0000a640: 6e65 7261 7465 6420 756e 6c65 7373 0a20  nerated unless. 
-0000a650: 2020 2020 2020 2074 686f 7365 2061 6c72         those alr
-0000a660: 6561 6479 2065 7869 7374 2e0a 0a20 2020  eady exist...   
-0000a670: 2020 2020 2050 6172 616d 6574 6572 730a       Parameters.
-0000a680: 2020 2020 2020 2020 2d2d 2d2d 2d2d 2d2d          --------
-0000a690: 2d2d 0a20 2020 2020 2020 2064 6973 7461  --.        dista
-0000a6a0: 6e63 6520 3a20 666c 6f61 742c 206f 7074  nce : float, opt
-0000a6b0: 696f 6e61 6c0a 2020 2020 2020 2020 2020  ional.          
-0000a6c0: 2020 436f 6e73 7461 6e74 2064 6973 706c    Constant displ
-0000a6d0: 6163 656d 656e 7420 4575 636c 6964 6561  acement Euclidea
-0000a6e0: 6e20 6469 7374 616e 6365 2e20 4465 6661  n distance. Defa
-0000a6f0: 756c 7420 6973 2030 2e30 332e 0a20 2020  ult is 0.03..   
-0000a700: 2020 2020 2063 7574 6f66 665f 7061 6972       cutoff_pair
-0000a710: 5f64 6973 7461 6e63 6520 3a20 666c 6f61  _distance : floa
-0000a720: 742c 206f 7074 696f 6e61 6c0a 2020 2020  t, optional.    
-0000a730: 2020 2020 2020 2020 5468 6973 2069 7320          This is 
-0000a740: 7573 6564 2061 7320 6120 6375 746f 6666  used as a cutoff
-0000a750: 2045 7563 6c69 6465 616e 2064 6973 7461   Euclidean dista
-0000a760: 6e63 6520 746f 2064 6574 6572 6d69 6e65  nce to determine
-0000a770: 2069 660a 2020 2020 2020 2020 2020 2020   if.            
-0000a780: 6561 6368 2070 6169 7220 6f66 2064 6973  each pair of dis
-0000a790: 706c 6163 656d 656e 7473 2069 7320 636f  placements is co
-0000a7a0: 6e73 6964 6572 6564 2074 6f20 6361 6c63  nsidered to calc
-0000a7b0: 756c 6174 6520 6663 3320 6f72 206e 6f74  ulate fc3 or not
-0000a7c0: 2e0a 2020 2020 2020 2020 2020 2020 4465  ..            De
-0000a7d0: 6661 756c 7420 6973 204e 6f6e 652c 2077  fault is None, w
-0000a7e0: 6869 6368 206d 6561 6e73 2063 7574 6f66  hich means cutof
-0000a7f0: 6620 6973 206e 6f74 2075 7365 642e 0a20  f is not used.. 
-0000a800: 2020 2020 2020 2069 735f 706c 7573 6d69         is_plusmi
-0000a810: 6e75 7320 3a20 5472 7565 2c20 4661 6c73  nus : True, Fals
-0000a820: 652c 206f 7220 2761 7574 6f27 2c20 6f70  e, or 'auto', op
-0000a830: 7469 6f6e 616c 0a20 2020 2020 2020 2020  tional.         
-0000a840: 2020 2057 6974 6820 5472 7565 2c20 6174     With True, at
-0000a850: 6f6d 6973 2061 7265 2064 6973 706c 6163  omis are displac
-0000a860: 6564 2069 6e20 626f 7468 2070 6f73 6974  ed in both posit
-0000a870: 6976 6520 616e 6420 6e65 6761 7469 7665  ive and negative
-0000a880: 0a20 2020 2020 2020 2020 2020 2064 6972  .            dir
-0000a890: 6563 7469 6f6e 732e 2057 6974 6820 4661  ections. With Fa
-0000a8a0: 6c73 652c 206f 6e6c 7920 6f6e 6520 6469  lse, only one di
-0000a8b0: 7265 6374 696f 6e2e 2057 6974 6820 2761  rection. With 'a
-0000a8c0: 7574 6f27 2c0a 2020 2020 2020 2020 2020  uto',.          
-0000a8d0: 2020 6d6f 7374 6c79 2065 7175 6976 616c    mostly equival
-0000a8e0: 656e 7420 746f 2069 735f 706c 7573 6d69  ent to is_plusmi
-0000a8f0: 6e75 733d 5472 7565 2c20 6275 7420 6f6e  nus=True, but on
-0000a900: 6c79 206f 6e65 2064 6972 6563 7469 6f6e  ly one direction
-0000a910: 0a20 2020 2020 2020 2020 2020 2069 7320  .            is 
-0000a920: 6368 6f73 656e 2077 6865 6e20 7468 6520  chosen when the 
-0000a930: 6469 7370 6c61 6365 6d65 6e74 7320 696e  displacements in
-0000a940: 2062 6f74 6820 6469 7265 6374 696f 6e73   both directions
-0000a950: 2061 7265 0a20 2020 2020 2020 2020 2020   are.           
-0000a960: 2073 796d 6d65 7472 6963 616c 6c79 2065   symmetrically e
-0000a970: 7175 6976 616c 656e 742e 2044 6566 6175  quivalent. Defau
-0000a980: 6c74 2069 7320 2761 7574 6f27 2e0a 2020  lt is 'auto'..  
-0000a990: 2020 2020 2020 6973 5f64 6961 676f 6e61        is_diagona
-0000a9a0: 6c20 3a20 426f 6f6c 2c20 6f70 7469 6f6e  l : Bool, option
-0000a9b0: 616c 0a20 2020 2020 2020 2020 2020 2057  al.            W
-0000a9c0: 6974 6820 4661 6c73 652c 2074 6865 2073  ith False, the s
-0000a9d0: 6563 6f6e 6420 6469 7370 6c61 6365 6d65  econd displaceme
-0000a9e0: 6e74 7320 6172 6520 6d61 6465 2061 6c6f  nts are made alo
-0000a9f0: 6e67 2074 6865 2062 6173 6973 0a20 2020  ng the basis.   
-0000aa00: 2020 2020 2020 2020 2076 6563 746f 7273           vectors
-0000aa10: 206f 6620 7468 6520 7375 7065 7263 656c   of the supercel
-0000aa20: 6c2e 2057 6974 6820 5472 7565 2c20 6469  l. With True, di
-0000aa30: 7265 6374 696f 6e20 6e6f 7420 616c 6f6e  rection not alon
-0000aa40: 6720 7468 6520 6261 7369 730a 2020 2020  g the basis.    
-0000aa50: 2020 2020 2020 2020 7665 6374 6f72 7320          vectors 
-0000aa60: 6361 6e20 6265 2063 686f 7365 6e20 7768  can be chosen wh
-0000aa70: 656e 2074 6865 206e 756d 6265 7220 6f66  en the number of
-0000aa80: 2074 6865 2064 6973 706c 6163 656d 656e   the displacemen
-0000aa90: 7473 0a20 2020 2020 2020 2020 2020 206d  ts.            m
-0000aaa0: 6179 2062 6520 7265 6475 6365 642e 0a0a  ay be reduced...
-0000aab0: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
-0000aac0: 2020 2020 6469 7265 6374 696f 6e5f 6461      direction_da
-0000aad0: 7461 7365 7420 3d20 6765 745f 7468 6972  taset = get_thir
-0000aae0: 645f 6f72 6465 725f 6469 7370 6c61 6365  d_order_displace
-0000aaf0: 6d65 6e74 7328 0a20 2020 2020 2020 2020  ments(.         
-0000ab00: 2020 2073 656c 662e 5f73 7570 6572 6365     self._superce
-0000ab10: 6c6c 2c0a 2020 2020 2020 2020 2020 2020  ll,.            
-0000ab20: 7365 6c66 2e5f 7379 6d6d 6574 7279 2c0a  self._symmetry,.
-0000ab30: 2020 2020 2020 2020 2020 2020 6973 5f70              is_p
-0000ab40: 6c75 736d 696e 7573 3d69 735f 706c 7573  lusminus=is_plus
-0000ab50: 6d69 6e75 732c 0a20 2020 2020 2020 2020  minus,.         
-0000ab60: 2020 2069 735f 6469 6167 6f6e 616c 3d69     is_diagonal=i
-0000ab70: 735f 6469 6167 6f6e 616c 2c0a 2020 2020  s_diagonal,.    
-0000ab80: 2020 2020 290a 2020 2020 2020 2020 7365      ).        se
-0000ab90: 6c66 2e5f 6461 7461 7365 7420 3d20 6469  lf._dataset = di
-0000aba0: 7265 6374 696f 6e5f 746f 5f64 6973 706c  rection_to_displ
-0000abb0: 6163 656d 656e 7428 0a20 2020 2020 2020  acement(.       
-0000abc0: 2020 2020 2064 6972 6563 7469 6f6e 5f64       direction_d
-0000abd0: 6174 6173 6574 2c0a 2020 2020 2020 2020  ataset,.        
-0000abe0: 2020 2020 6469 7374 616e 6365 2c0a 2020      distance,.  
-0000abf0: 2020 2020 2020 2020 2020 7365 6c66 2e5f            self._
-0000ac00: 7375 7065 7263 656c 6c2c 0a20 2020 2020  supercell,.     
-0000ac10: 2020 2020 2020 2063 7574 6f66 665f 6469         cutoff_di
-0000ac20: 7374 616e 6365 3d63 7574 6f66 665f 7061  stance=cutoff_pa
-0000ac30: 6972 5f64 6973 7461 6e63 652c 0a20 2020  ir_distance,.   
-0000ac40: 2020 2020 2029 0a20 2020 2020 2020 2073       ).        s
-0000ac50: 656c 662e 5f73 7570 6572 6365 6c6c 735f  elf._supercells_
-0000ac60: 7769 7468 5f64 6973 706c 6163 656d 656e  with_displacemen
-0000ac70: 7473 203d 204e 6f6e 650a 0a20 2020 2020  ts = None..     
-0000ac80: 2020 2069 6620 7365 6c66 2e5f 7068 6f6e     if self._phon
-0000ac90: 6f6e 5f73 7570 6572 6365 6c6c 5f6d 6174  on_supercell_mat
-0000aca0: 7269 7820 6973 206e 6f74 204e 6f6e 6520  rix is not None 
-0000acb0: 616e 6420 7365 6c66 2e5f 7068 6f6e 6f6e  and self._phonon
-0000acc0: 5f64 6174 6173 6574 2069 7320 4e6f 6e65  _dataset is None
-0000acd0: 3a0a 2020 2020 2020 2020 2020 2020 7365  :.            se
-0000ace0: 6c66 2e67 656e 6572 6174 655f 6663 325f  lf.generate_fc2_
-0000acf0: 6469 7370 6c61 6365 6d65 6e74 7328 0a20  displacements(. 
-0000ad00: 2020 2020 2020 2020 2020 2020 2020 2064                 d
-0000ad10: 6973 7461 6e63 653d 6469 7374 616e 6365  istance=distance
-0000ad20: 2c20 6973 5f70 6c75 736d 696e 7573 3d69  , is_plusminus=i
-0000ad30: 735f 706c 7573 6d69 6e75 732c 2069 735f  s_plusminus, is_
-0000ad40: 6469 6167 6f6e 616c 3d46 616c 7365 0a20  diagonal=False. 
-0000ad50: 2020 2020 2020 2020 2020 2029 0a0a 2020             )..  
-0000ad60: 2020 6465 6620 6765 6e65 7261 7465 5f66    def generate_f
-0000ad70: 6332 5f64 6973 706c 6163 656d 656e 7473  c2_displacements
-0000ad80: 280a 2020 2020 2020 2020 7365 6c66 2c20  (.        self, 
-0000ad90: 6469 7374 616e 6365 3d30 2e30 332c 2069  distance=0.03, i
-0000ada0: 735f 706c 7573 6d69 6e75 733d 2261 7574  s_plusminus="aut
-0000adb0: 6f22 2c20 6973 5f64 6961 676f 6e61 6c3d  o", is_diagonal=
-0000adc0: 4661 6c73 650a 2020 2020 293a 0a20 2020  False.    ):.   
-0000add0: 2020 2020 2022 2222 4765 6e65 7261 7465       """Generate
-0000ade0: 2064 6973 706c 6163 656d 656e 7420 6461   displacement da
-0000adf0: 7461 7365 7420 696e 2070 686f 6e6f 6e20  taset in phonon 
-0000ae00: 7375 7065 7263 656c 6c20 666f 7220 6663  supercell for fc
-0000ae10: 322e 0a0a 2020 2020 2020 2020 5468 6973  2...        This
-0000ae20: 2073 7973 7465 6d61 7469 6361 6c6c 7920   systematically 
-0000ae30: 6765 6e65 7261 7465 7320 7369 6e67 6c65  generates single
-0000ae40: 2061 746f 6d69 6320 6469 7370 6c61 6365   atomic displace
-0000ae50: 6d65 6e74 730a 2020 2020 2020 2020 696e  ments.        in
-0000ae60: 2073 7570 6572 6365 6c6c 7320 746f 2063   supercells to c
-0000ae70: 616c 6375 6c61 7465 2070 686f 6e6f 6e5f  alculate phonon_
-0000ae80: 6663 3220 636f 6e73 6964 6572 696e 6720  fc2 considering 
-0000ae90: 6372 7973 7461 6c20 7379 6d6d 6574 7279  crystal symmetry
-0000aea0: 2e0a 2020 2020 2020 2020 5768 656e 2074  ..        When t
-0000aeb0: 6869 7320 6d65 7468 6f64 2069 7320 6361  his method is ca
-0000aec0: 6c6c 6564 2c20 6578 6973 7469 6e67 2063  lled, existing c
-0000aed0: 6163 6865 206f 6620 7375 7065 7263 656c  ache of supercel
-0000aee0: 6c73 2077 6974 680a 2020 2020 2020 2020  ls with.        
-0000aef0: 6469 7370 6c61 6365 6d65 6e74 7320 666f  displacements fo
-0000af00: 7220 6663 3220 6172 6520 7265 6d6f 7665  r fc2 are remove
-0000af10: 642e 0a0a 2020 2020 2020 2020 4e6f 7465  d...        Note
-0000af20: 0a20 2020 2020 2020 202d 2d2d 2d0a 2020  .        ----.  
-0000af30: 2020 2020 2020 6973 5f64 6961 676f 6e61        is_diagona
-0000af40: 6c3d 4661 6c73 6520 6973 2063 686f 7365  l=False is chose
-0000af50: 6e20 6173 2074 6865 2064 6566 6175 6c74  n as the default
-0000af60: 2073 6574 7469 6e67 2069 6e74 656e 7469   setting intenti
-0000af70: 6f6e 616c 6c79 0a20 2020 2020 2020 2074  onally.        t
-0000af80: 6f20 6265 2063 6f6e 7369 7374 656e 7420  o be consistent 
-0000af90: 746f 2074 6865 2066 6972 7374 2064 6973  to the first dis
-0000afa0: 706c 6163 656d 656e 7473 206f 6620 7468  placements of th
-0000afb0: 6520 6663 3320 7061 6972 0a20 2020 2020  e fc3 pair.     
-0000afc0: 2020 2064 6973 706c 6163 656d 6574 7320     displacemets 
-0000afd0: 696e 2073 7570 6572 6365 6c6c 2e0a 0a20  in supercell... 
-0000afe0: 2020 2020 2020 2050 6172 616d 6574 6572         Parameter
-0000aff0: 730a 2020 2020 2020 2020 2d2d 2d2d 2d2d  s.        ------
-0000b000: 2d2d 2d2d 0a20 2020 2020 2020 2064 6973  ----.        dis
-0000b010: 7461 6e63 6520 3a20 666c 6f61 742c 206f  tance : float, o
-0000b020: 7074 696f 6e61 6c0a 2020 2020 2020 2020  ptional.        
-0000b030: 2020 2020 436f 6e73 7461 6e74 2064 6973      Constant dis
-0000b040: 706c 6163 656d 656e 7420 4575 636c 6964  placement Euclid
-0000b050: 6561 6e20 6469 7374 616e 6365 2e20 4465  ean distance. De
-0000b060: 6661 756c 7420 6973 2030 2e30 332e 0a20  fault is 0.03.. 
-0000b070: 2020 2020 2020 2069 735f 706c 7573 6d69         is_plusmi
-0000b080: 6e75 7320 3a20 5472 7565 2c20 4661 6c73  nus : True, Fals
-0000b090: 652c 206f 7220 2761 7574 6f27 2c20 6f70  e, or 'auto', op
-0000b0a0: 7469 6f6e 616c 0a20 2020 2020 2020 2020  tional.         
-0000b0b0: 2020 2057 6974 6820 5472 7565 2c20 6174     With True, at
-0000b0c0: 6f6d 6973 2061 7265 2064 6973 706c 6163  omis are displac
-0000b0d0: 6564 2069 6e20 626f 7468 2070 6f73 6974  ed in both posit
-0000b0e0: 6976 6520 616e 6420 6e65 6761 7469 7665  ive and negative
-0000b0f0: 0a20 2020 2020 2020 2020 2020 2064 6972  .            dir
-0000b100: 6563 7469 6f6e 732e 2057 6974 6820 4661  ections. With Fa
-0000b110: 6c73 652c 206f 6e6c 7920 6f6e 6520 6469  lse, only one di
-0000b120: 7265 6374 696f 6e2e 2057 6974 6820 2761  rection. With 'a
-0000b130: 7574 6f27 2c0a 2020 2020 2020 2020 2020  uto',.          
-0000b140: 2020 6d6f 7374 6c79 2065 7175 6976 616c    mostly equival
-0000b150: 656e 7420 746f 2069 735f 706c 7573 6d69  ent to is_plusmi
-0000b160: 6e75 733d 5472 7565 2c20 6275 7420 6f6e  nus=True, but on
-0000b170: 6c79 206f 6e65 2064 6972 6563 7469 6f6e  ly one direction
-0000b180: 0a20 2020 2020 2020 2020 2020 2069 7320  .            is 
-0000b190: 6368 6f73 656e 2077 6865 6e20 7468 6520  chosen when the 
-0000b1a0: 6469 7370 6c61 6365 6d65 6e74 7320 696e  displacements in
-0000b1b0: 2062 6f74 6820 6469 7265 6374 696f 6e73   both directions
-0000b1c0: 2061 7265 0a20 2020 2020 2020 2020 2020   are.           
-0000b1d0: 2073 796d 6d65 7472 6963 616c 6c79 2065   symmetrically e
-0000b1e0: 7175 6976 616c 656e 742e 2044 6566 6175  quivalent. Defau
-0000b1f0: 6c74 2069 7320 2761 7574 6f27 2e0a 2020  lt is 'auto'..  
-0000b200: 2020 2020 2020 6973 5f64 6961 676f 6e61        is_diagona
-0000b210: 6c20 3a20 426f 6f6c 2c20 6f70 7469 6f6e  l : Bool, option
-0000b220: 616c 0a20 2020 2020 2020 2020 2020 2057  al.            W
-0000b230: 6974 6820 4661 6c73 652c 2074 6865 2064  ith False, the d
-0000b240: 6973 706c 6163 656d 656e 7473 2061 7265  isplacements are
-0000b250: 206d 6164 6520 616c 6f6e 6720 7468 6520   made along the 
-0000b260: 6261 7369 730a 2020 2020 2020 2020 2020  basis.          
-0000b270: 2020 7665 6374 6f72 7320 6f66 2074 6865    vectors of the
-0000b280: 2073 7570 6572 6365 6c6c 2e20 5769 7468   supercell. With
-0000b290: 2054 7275 652c 2064 6972 6563 7469 6f6e   True, direction
-0000b2a0: 206e 6f74 2061 6c6f 6e67 2074 6865 2062   not along the b
-0000b2b0: 6173 6973 0a20 2020 2020 2020 2020 2020  asis.           
-0000b2c0: 2076 6563 746f 7273 2063 616e 2062 6520   vectors can be 
-0000b2d0: 6368 6f73 656e 2077 6865 6e20 7468 6520  chosen when the 
-0000b2e0: 6e75 6d62 6572 206f 6620 7468 6520 6469  number of the di
-0000b2f0: 7370 6c61 6365 6d65 6e74 730a 2020 2020  splacements.    
-0000b300: 2020 2020 2020 2020 6d61 7920 6265 2072          may be r
-0000b310: 6564 7563 6564 2e20 4465 6661 756c 7420  educed. Default 
-0000b320: 6973 2046 616c 7365 2e0a 0a20 2020 2020  is False...     
-0000b330: 2020 2022 2222 0a20 2020 2020 2020 2069     """.        i
-0000b340: 6620 7365 6c66 2e5f 7068 6f6e 6f6e 5f73  f self._phonon_s
-0000b350: 7570 6572 6365 6c6c 5f6d 6174 7269 7820  upercell_matrix 
-0000b360: 6973 204e 6f6e 653a 0a20 2020 2020 2020  is None:.       
-0000b370: 2020 2020 206d 7367 203d 2028 0a20 2020       msg = (.   
-0000b380: 2020 2020 2020 2020 2020 2020 2022 7068               "ph
-0000b390: 6f6e 6f6e 5f73 7570 6572 6365 6c6c 5f6d  onon_supercell_m
-0000b3a0: 6174 7269 7820 6973 206e 6f74 2073 6574  atrix is not set
-0000b3b0: 2e20 220a 2020 2020 2020 2020 2020 2020  . ".            
-0000b3c0: 2020 2020 2254 6869 7320 6d65 7468 6f64      "This method
-0000b3d0: 2069 7320 7573 6564 2074 6f20 6765 6e65   is used to gene
-0000b3e0: 7261 7465 2064 6973 706c 6163 656d 656e  rate displacemen
-0000b3f0: 7473 2074 6f20 220a 2020 2020 2020 2020  ts to ".        
-0000b400: 2020 2020 2020 2020 2263 616c 6375 6c61          "calcula
-0000b410: 7465 2070 686f 6e6f 6e5f 6663 322e 220a  te phonon_fc2.".
-0000b420: 2020 2020 2020 2020 2020 2020 290a 2020              ).  
-0000b430: 2020 2020 2020 2020 2020 7261 6973 6520            raise 
-0000b440: 5275 6e74 696d 6545 7272 6f72 286d 7367  RuntimeError(msg
-0000b450: 290a 0a20 2020 2020 2020 2070 686f 6e6f  )..        phono
-0000b460: 6e5f 6469 7370 6c61 6365 6d65 6e74 5f64  n_displacement_d
-0000b470: 6972 6563 7469 6f6e 7320 3d20 6765 745f  irections = get_
-0000b480: 6c65 6173 745f 6469 7370 6c61 6365 6d65  least_displaceme
-0000b490: 6e74 7328 0a20 2020 2020 2020 2020 2020  nts(.           
-0000b4a0: 2073 656c 662e 5f70 686f 6e6f 6e5f 7375   self._phonon_su
-0000b4b0: 7065 7263 656c 6c5f 7379 6d6d 6574 7279  percell_symmetry
-0000b4c0: 2c0a 2020 2020 2020 2020 2020 2020 6973  ,.            is
-0000b4d0: 5f70 6c75 736d 696e 7573 3d69 735f 706c  _plusminus=is_pl
-0000b4e0: 7573 6d69 6e75 732c 0a20 2020 2020 2020  usminus,.       
-0000b4f0: 2020 2020 2069 735f 6469 6167 6f6e 616c       is_diagonal
-0000b500: 3d69 735f 6469 6167 6f6e 616c 2c0a 2020  =is_diagonal,.  
-0000b510: 2020 2020 2020 290a 2020 2020 2020 2020        ).        
-0000b520: 7365 6c66 2e5f 7068 6f6e 6f6e 5f64 6174  self._phonon_dat
-0000b530: 6173 6574 203d 2064 6972 6563 7469 6f6e  aset = direction
-0000b540: 735f 746f 5f64 6973 706c 6163 656d 656e  s_to_displacemen
-0000b550: 745f 6461 7461 7365 7428 0a20 2020 2020  t_dataset(.     
-0000b560: 2020 2020 2020 2070 686f 6e6f 6e5f 6469         phonon_di
-0000b570: 7370 6c61 6365 6d65 6e74 5f64 6972 6563  splacement_direc
-0000b580: 7469 6f6e 732c 2064 6973 7461 6e63 652c  tions, distance,
-0000b590: 2073 656c 662e 5f70 686f 6e6f 6e5f 7375   self._phonon_su
-0000b5a0: 7065 7263 656c 6c0a 2020 2020 2020 2020  percell.        
-0000b5b0: 290a 2020 2020 2020 2020 7365 6c66 2e5f  ).        self._
-0000b5c0: 7068 6f6e 6f6e 5f73 7570 6572 6365 6c6c  phonon_supercell
-0000b5d0: 735f 7769 7468 5f64 6973 706c 6163 656d  s_with_displacem
-0000b5e0: 656e 7473 203d 204e 6f6e 650a 0a20 2020  ents = None..   
-0000b5f0: 2064 6566 2070 726f 6475 6365 5f66 6333   def produce_fc3
-0000b600: 280a 2020 2020 2020 2020 7365 6c66 2c0a  (.        self,.
-0000b610: 2020 2020 2020 2020 7379 6d6d 6574 7269          symmetri
-0000b620: 7a65 5f66 6333 723d 4661 6c73 652c 0a20  ze_fc3r=False,. 
-0000b630: 2020 2020 2020 2069 735f 636f 6d70 6163         is_compac
-0000b640: 745f 6663 3d46 616c 7365 2c0a 2020 2020  t_fc=False,.    
-0000b650: 2020 2020 6663 5f63 616c 6375 6c61 746f      fc_calculato
-0000b660: 723d 4e6f 6e65 2c0a 2020 2020 2020 2020  r=None,.        
-0000b670: 6663 5f63 616c 6375 6c61 746f 725f 6f70  fc_calculator_op
-0000b680: 7469 6f6e 733d 4e6f 6e65 2c0a 2020 2020  tions=None,.    
-0000b690: 293a 0a20 2020 2020 2020 2022 2222 4361  ):.        """Ca
-0000b6a0: 6c63 756c 6174 6520 6663 3320 6672 6f6d  lculate fc3 from
-0000b6b0: 2064 6973 706c 6163 656d 656e 7473 2061   displacements a
-0000b6c0: 6e64 2066 6f72 6365 732e 0a0a 2020 2020  nd forces...    
-0000b6d0: 2020 2020 5061 7261 6d65 7465 7273 0a20      Parameters. 
-0000b6e0: 2020 2020 2020 202d 2d2d 2d2d 2d2d 2d2d         ---------
-0000b6f0: 2d0a 2020 2020 2020 2020 7379 6d6d 6574  -.        symmet
-0000b700: 7269 7a65 5f66 6333 7220 3a20 626f 6f6c  rize_fc3r : bool
-0000b710: 0a20 2020 2020 2020 2020 2020 204f 6e6c  .            Onl
-0000b720: 7920 666f 7220 7479 7065 2031 2064 6973  y for type 1 dis
-0000b730: 706c 6163 656d 656e 745f 6461 7461 7365  placement_datase
-0000b740: 742c 2074 7261 6e73 6c61 7469 6f6e 616c  t, translational
-0000b750: 2061 6e64 0a20 2020 2020 2020 2020 2020   and.           
-0000b760: 2070 6572 6d75 7461 7469 6f6e 2073 796d   permutation sym
-0000b770: 6d65 7472 6965 7320 6172 6520 6170 706c  metries are appl
-0000b780: 6965 6420 6166 7465 7220 6372 6561 7469  ied after creati
-0000b790: 6e67 2066 6333 2e20 5468 6973 0a20 2020  ng fc3. This.   
-0000b7a0: 2020 2020 2020 2020 2073 796d 6d65 7472           symmetr
-0000b7b0: 697a 6174 696f 6e20 6973 206e 6f74 2076  ization is not v
-0000b7c0: 6572 7920 736f 7068 6973 7469 6361 7465  ery sophisticate
-0000b7d0: 6420 616e 6420 6361 6e20 6272 6561 6b20  d and can break 
-0000b7e0: 7370 6163 650a 2020 2020 2020 2020 2020  space.          
-0000b7f0: 2020 6772 6f75 7020 7379 6d6d 6574 7279    group symmetry
-0000b800: 2c20 6275 7420 6f66 7465 6e20 7573 6566  , but often usef
-0000b810: 756c 2e20 4966 2062 6574 7465 7220 7379  ul. If better sy
-0000b820: 6d6d 6574 7269 7a61 7469 6f6e 2069 730a  mmetrization is.
-0000b830: 2020 2020 2020 2020 2020 2020 6578 7065              expe
-0000b840: 6374 6564 2c20 6974 2069 7320 7265 636f  cted, it is reco
-0000b850: 6d6d 656e 6465 6420 746f 2075 7365 2065  mmended to use e
-0000b860: 7874 6572 6e61 6c20 666f 7263 6520 636f  xternal force co
-0000b870: 6e73 7461 6e74 730a 2020 2020 2020 2020  nstants.        
-0000b880: 2020 2020 6361 6c63 756c 6174 6f72 2073      calculator s
-0000b890: 7563 6820 6173 2041 4c4d 2e20 4465 6661  uch as ALM. Defa
-0000b8a0: 756c 7420 6973 2046 616c 7365 2e0a 2020  ult is False..  
-0000b8b0: 2020 2020 2020 6973 5f63 6f6d 7061 6374        is_compact
-0000b8c0: 5f66 6320 3a20 626f 6f6c 0a20 2020 2020  _fc : bool.     
-0000b8d0: 2020 2020 2020 2066 6333 2073 6861 7065         fc3 shape
-0000b8e0: 2069 730a 2020 2020 2020 2020 2020 2020   is.            
-0000b8f0: 2020 2020 4661 6c73 653a 2028 7375 7065      False: (supe
-0000b900: 7263 656c 6c2c 2073 7570 6572 6365 6c6c  rcell, supercell
-0000b910: 2c20 7375 7065 6365 6c6c 2c20 332c 2033  , supecell, 3, 3
-0000b920: 2c20 3329 0a20 2020 2020 2020 2020 2020  , 3).           
-0000b930: 2020 2020 2054 7275 653a 2028 7072 696d       True: (prim
-0000b940: 6974 6976 652c 2073 7570 6572 6365 6c6c  itive, supercell
-0000b950: 2c20 7375 7065 6365 6c6c 2c20 332c 2033  , supecell, 3, 3
-0000b960: 2c20 3329 0a20 2020 2020 2020 2020 2020  , 3).           
-0000b970: 2077 6865 7265 2027 7375 7065 7263 656c   where 'supercel
-0000b980: 6c27 2061 6e64 2027 7072 696d 6974 6976  l' and 'primitiv
-0000b990: 6527 2069 6e64 6963 6174 6520 6e75 6d62  e' indicate numb
-0000b9a0: 6572 206f 6620 6174 6f6d 7320 696e 2074  er of atoms in t
-0000b9b0: 6865 7365 0a20 2020 2020 2020 2020 2020  hese.           
-0000b9c0: 2063 656c 6c73 2e20 4465 6661 756c 7420   cells. Default 
-0000b9d0: 6973 2046 616c 7365 2e0a 2020 2020 2020  is False..      
-0000b9e0: 2020 6663 5f63 616c 6375 6c61 746f 7220    fc_calculator 
-0000b9f0: 3a20 7374 7220 6f72 204e 6f6e 650a 2020  : str or None.  
-0000ba00: 2020 2020 2020 2020 2020 466f 7263 6520            Force 
-0000ba10: 636f 6e73 7461 6e74 7320 6361 6c63 756c  constants calcul
-0000ba20: 6174 6f72 2067 6976 656e 2062 7920 7374  ator given by st
-0000ba30: 722e 0a20 2020 2020 2020 2066 635f 6361  r..        fc_ca
-0000ba40: 6c63 756c 6174 6f72 5f6f 7074 696f 6e73  lculator_options
-0000ba50: 203a 2064 6963 740a 2020 2020 2020 2020   : dict.        
-0000ba60: 2020 2020 4f70 7469 6f6e 7320 666f 7220      Options for 
-0000ba70: 6578 7465 726e 616c 2066 6f72 6365 2063  external force c
-0000ba80: 6f6e 7374 616e 7473 2063 616c 6375 6c61  onstants calcula
-0000ba90: 746f 722e 0a0a 2020 2020 2020 2020 2222  tor...        ""
-0000baa0: 220a 2020 2020 2020 2020 6469 7370 5f64  ".        disp_d
-0000bab0: 6174 6173 6574 203d 2073 656c 662e 5f64  ataset = self._d
-0000bac0: 6174 6173 6574 0a0a 2020 2020 2020 2020  ataset..        
-0000bad0: 6663 335f 6361 6c63 756c 6174 6f72 2c20  fc3_calculator, 
-0000bae0: 6663 335f 6361 6c63 756c 6174 6f72 5f6f  fc3_calculator_o
-0000baf0: 7074 696f 6e73 203d 2073 656c 662e 5f65  ptions = self._e
-0000bb00: 7874 7261 6374 5f66 6332 5f66 6333 5f63  xtract_fc2_fc3_c
-0000bb10: 616c 6375 6c61 746f 7273 280a 2020 2020  alculators(.    
-0000bb20: 2020 2020 2020 2020 6663 5f63 616c 6375          fc_calcu
-0000bb30: 6c61 746f 722c 2066 635f 6361 6c63 756c  lator, fc_calcul
-0000bb40: 6174 6f72 5f6f 7074 696f 6e73 2c20 330a  ator_options, 3.
-0000bb50: 2020 2020 2020 2020 290a 0a20 2020 2020          )..     
-0000bb60: 2020 2069 6620 6663 335f 6361 6c63 756c     if fc3_calcul
-0000bb70: 6174 6f72 2069 7320 6e6f 7420 4e6f 6e65  ator is not None
-0000bb80: 3a0a 2020 2020 2020 2020 2020 2020 6469  :.            di
-0000bb90: 7370 732c 2066 6f72 6365 7320 3d20 6765  sps, forces = ge
-0000bba0: 745f 6469 7370 6c61 6365 6d65 6e74 735f  t_displacements_
-0000bbb0: 616e 645f 666f 7263 6573 5f66 6333 2864  and_forces_fc3(d
-0000bbc0: 6973 705f 6461 7461 7365 7429 0a20 2020  isp_dataset).   
-0000bbd0: 2020 2020 2020 2020 2066 6332 2c20 6663           fc2, fc
-0000bbe0: 3320 3d20 6765 745f 6663 3328 0a20 2020  3 = get_fc3(.   
-0000bbf0: 2020 2020 2020 2020 2020 2020 2073 656c               sel
-0000bc00: 662e 5f73 7570 6572 6365 6c6c 2c0a 2020  f._supercell,.  
-0000bc10: 2020 2020 2020 2020 2020 2020 2020 7365                se
-0000bc20: 6c66 2e5f 7072 696d 6974 6976 652c 0a20  lf._primitive,. 
-0000bc30: 2020 2020 2020 2020 2020 2020 2020 2064                 d
-0000bc40: 6973 7073 2c0a 2020 2020 2020 2020 2020  isps,.          
-0000bc50: 2020 2020 2020 666f 7263 6573 2c0a 2020        forces,.  
-0000bc60: 2020 2020 2020 2020 2020 2020 2020 6663                fc
-0000bc70: 5f63 616c 6375 6c61 746f 723d 6663 335f  _calculator=fc3_
-0000bc80: 6361 6c63 756c 6174 6f72 2c0a 2020 2020  calculator,.    
-0000bc90: 2020 2020 2020 2020 2020 2020 6663 5f63              fc_c
-0000bca0: 616c 6375 6c61 746f 725f 6f70 7469 6f6e  alculator_option
-0000bcb0: 733d 6663 335f 6361 6c63 756c 6174 6f72  s=fc3_calculator
-0000bcc0: 5f6f 7074 696f 6e73 2c0a 2020 2020 2020  _options,.      
-0000bcd0: 2020 2020 2020 2020 2020 6973 5f63 6f6d            is_com
-0000bce0: 7061 6374 5f66 633d 6973 5f63 6f6d 7061  pact_fc=is_compa
-0000bcf0: 6374 5f66 632c 0a20 2020 2020 2020 2020  ct_fc,.         
-0000bd00: 2020 2020 2020 206c 6f67 5f6c 6576 656c         log_level
-0000bd10: 3d73 656c 662e 5f6c 6f67 5f6c 6576 656c  =self._log_level
-0000bd20: 2c0a 2020 2020 2020 2020 2020 2020 290a  ,.            ).
-0000bd30: 2020 2020 2020 2020 656c 7365 3a0a 2020          else:.  
-0000bd40: 2020 2020 2020 2020 2020 6966 2022 6469            if "di
-0000bd50: 7370 6c61 6365 6d65 6e74 7322 2069 6e20  splacements" in 
-0000bd60: 6469 7370 5f64 6174 6173 6574 3a0a 2020  disp_dataset:.  
-0000bd70: 2020 2020 2020 2020 2020 2020 2020 6d73                ms
-0000bd80: 6720 3d20 280a 2020 2020 2020 2020 2020  g = (.          
-0000bd90: 2020 2020 2020 2020 2020 2266 635f 6361            "fc_ca
-0000bda0: 6c63 756c 6174 6f72 2068 6173 2074 6f20  lculator has to 
-0000bdb0: 6265 2073 6574 2074 6f20 7072 6f64 7563  be set to produc
-0000bdc0: 6520 666f 7263 6520 220a 2020 2020 2020  e force ".      
-0000bdd0: 2020 2020 2020 2020 2020 2020 2020 2263                "c
-0000bde0: 6f6e 7374 616e 7320 6672 6f6d 2074 6869  onstans from thi
-0000bdf0: 7320 6461 7461 7365 742e 220a 2020 2020  s dataset.".    
-0000be00: 2020 2020 2020 2020 2020 2020 290a 2020              ).  
-0000be10: 2020 2020 2020 2020 2020 2020 2020 7261                ra
-0000be20: 6973 6520 466f 7263 6543 616c 6375 6c61  ise ForceCalcula
-0000be30: 746f 7252 6571 7569 7265 6445 7272 6f72  torRequiredError
-0000be40: 286d 7367 290a 2020 2020 2020 2020 2020  (msg).          
-0000be50: 2020 6663 322c 2066 6333 203d 2067 6574    fc2, fc3 = get
-0000be60: 5f70 686f 6e6f 3370 795f 6663 3328 0a20  _phono3py_fc3(. 
-0000be70: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-0000be80: 656c 662e 5f73 7570 6572 6365 6c6c 2c0a  elf._supercell,.
-0000be90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000bea0: 7365 6c66 2e5f 7072 696d 6974 6976 652c  self._primitive,
-0000beb0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000bec0: 2064 6973 705f 6461 7461 7365 742c 0a20   disp_dataset,. 
-0000bed0: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-0000bee0: 656c 662e 5f73 796d 6d65 7472 792c 0a20  elf._symmetry,. 
-0000bef0: 2020 2020 2020 2020 2020 2020 2020 2069                 i
-0000bf00: 735f 636f 6d70 6163 745f 6663 3d69 735f  s_compact_fc=is_
-0000bf10: 636f 6d70 6163 745f 6663 2c0a 2020 2020  compact_fc,.    
-0000bf20: 2020 2020 2020 2020 2020 2020 7665 7262              verb
-0000bf30: 6f73 653d 7365 6c66 2e5f 6c6f 675f 6c65  ose=self._log_le
-0000bf40: 7665 6c2c 0a20 2020 2020 2020 2020 2020  vel,.           
-0000bf50: 2029 0a20 2020 2020 2020 2020 2020 2069   ).            i
-0000bf60: 6620 7379 6d6d 6574 7269 7a65 5f66 6333  f symmetrize_fc3
-0000bf70: 723a 0a20 2020 2020 2020 2020 2020 2020  r:.             
-0000bf80: 2020 2069 6620 6973 5f63 6f6d 7061 6374     if is_compact
-0000bf90: 5f66 633a 0a20 2020 2020 2020 2020 2020  _fc:.           
-0000bfa0: 2020 2020 2020 2020 2073 6574 5f74 7261           set_tra
-0000bfb0: 6e73 6c61 7469 6f6e 616c 5f69 6e76 6172  nslational_invar
-0000bfc0: 6961 6e63 655f 636f 6d70 6163 745f 6663  iance_compact_fc
-0000bfd0: 3328 6663 332c 2073 656c 662e 5f70 7269  3(fc3, self._pri
-0000bfe0: 6d69 7469 7665 290a 2020 2020 2020 2020  mitive).        
-0000bff0: 2020 2020 2020 2020 2020 2020 7365 745f              set_
-0000c000: 7065 726d 7574 6174 696f 6e5f 7379 6d6d  permutation_symm
-0000c010: 6574 7279 5f63 6f6d 7061 6374 5f66 6333  etry_compact_fc3
-0000c020: 2866 6333 2c20 7365 6c66 2e5f 7072 696d  (fc3, self._prim
-0000c030: 6974 6976 6529 0a20 2020 2020 2020 2020  itive).         
-0000c040: 2020 2020 2020 2020 2020 2069 6620 7365             if se
-0000c050: 6c66 2e5f 6663 3220 6973 204e 6f6e 653a  lf._fc2 is None:
-0000c060: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000c070: 2020 2020 2020 2020 2073 796d 6d65 7472           symmetr
-0000c080: 697a 655f 636f 6d70 6163 745f 666f 7263  ize_compact_forc
-0000c090: 655f 636f 6e73 7461 6e74 7328 6663 322c  e_constants(fc2,
-0000c0a0: 2073 656c 662e 5f70 7269 6d69 7469 7665   self._primitive
-0000c0b0: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
-0000c0c0: 2020 656c 7365 3a0a 2020 2020 2020 2020    else:.        
-0000c0d0: 2020 2020 2020 2020 2020 2020 7365 745f              set_
-0000c0e0: 7472 616e 736c 6174 696f 6e61 6c5f 696e  translational_in
-0000c0f0: 7661 7269 616e 6365 5f66 6333 2866 6333  variance_fc3(fc3
-0000c100: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
-0000c110: 2020 2020 2020 7365 745f 7065 726d 7574        set_permut
-0000c120: 6174 696f 6e5f 7379 6d6d 6574 7279 5f66  ation_symmetry_f
-0000c130: 6333 2866 6333 290a 2020 2020 2020 2020  c3(fc3).        
-0000c140: 2020 2020 2020 2020 2020 2020 6966 2073              if s
-0000c150: 656c 662e 5f66 6332 2069 7320 4e6f 6e65  elf._fc2 is None
-0000c160: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-0000c170: 2020 2020 2020 2020 2020 7379 6d6d 6574            symmet
-0000c180: 7269 7a65 5f66 6f72 6365 5f63 6f6e 7374  rize_force_const
-0000c190: 616e 7473 2866 6332 290a 0a20 2020 2020  ants(fc2)..     
-0000c1a0: 2020 2023 2053 6574 2066 6332 2061 6e64     # Set fc2 and
-0000c1b0: 2066 6333 0a20 2020 2020 2020 2073 656c   fc3.        sel
-0000c1c0: 662e 5f66 6333 203d 2066 6333 0a0a 2020  f._fc3 = fc3..  
-0000c1d0: 2020 2020 2020 2320 6663 3220 6173 206f        # fc2 as o
-0000c1e0: 6274 6169 6e65 6420 6162 6f76 6520 7769  btained above wi
-0000c1f0: 6c6c 206e 6f74 2062 6520 7365 7420 7768  ll not be set wh
-0000c200: 656e 2022 7c22 2069 6e20 6663 2d63 616c  en "|" in fc-cal
-0000c210: 6375 6c61 746f 7220 7365 7474 696e 672e  culator setting.
-0000c220: 0a20 2020 2020 2020 2069 6620 6663 5f63  .        if fc_c
-0000c230: 616c 6375 6c61 746f 7220 6973 206e 6f74  alculator is not
-0000c240: 204e 6f6e 6520 616e 6420 227c 2220 696e   None and "|" in
-0000c250: 2066 635f 6361 6c63 756c 6174 6f72 3a0a   fc_calculator:.
-0000c260: 2020 2020 2020 2020 2020 2020 6663 3220              fc2 
-0000c270: 3d20 4e6f 6e65 0a20 2020 2020 2020 2069  = None.        i
-0000c280: 6620 6663 5f63 616c 6375 6c61 746f 725f  f fc_calculator_
-0000c290: 6f70 7469 6f6e 7320 6973 206e 6f74 204e  options is not N
-0000c2a0: 6f6e 6520 616e 6420 227c 2220 696e 2066  one and "|" in f
-0000c2b0: 635f 6361 6c63 756c 6174 6f72 5f6f 7074  c_calculator_opt
-0000c2c0: 696f 6e73 3a0a 2020 2020 2020 2020 2020  ions:.          
-0000c2d0: 2020 6663 3220 3d20 4e6f 6e65 0a0a 2020    fc2 = None..  
-0000c2e0: 2020 2020 2020 2320 4e6f 726d 616c 6c79        # Normally
-0000c2f0: 2073 656c 662e 5f66 6332 2069 7320 6f76   self._fc2 is ov
-0000c300: 6572 7772 6974 7465 6e20 696e 2070 726f  erwritten in pro
-0000c310: 6475 6365 5f66 6332 0a20 2020 2020 2020  duce_fc2.       
-0000c320: 2069 6620 7365 6c66 2e5f 6663 3220 6973   if self._fc2 is
-0000c330: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
-0000c340: 2020 2073 656c 662e 5f66 6332 203d 2066     self._fc2 = f
-0000c350: 6332 0a0a 2020 2020 6465 6620 7072 6f64  c2..    def prod
-0000c360: 7563 655f 6663 3228 0a20 2020 2020 2020  uce_fc2(.       
-0000c370: 2073 656c 662c 0a20 2020 2020 2020 2073   self,.        s
-0000c380: 796d 6d65 7472 697a 655f 6663 323d 4661  ymmetrize_fc2=Fa
-0000c390: 6c73 652c 0a20 2020 2020 2020 2069 735f  lse,.        is_
-0000c3a0: 636f 6d70 6163 745f 6663 3d46 616c 7365  compact_fc=False
-0000c3b0: 2c0a 2020 2020 2020 2020 6663 5f63 616c  ,.        fc_cal
-0000c3c0: 6375 6c61 746f 723d 4e6f 6e65 2c0a 2020  culator=None,.  
-0000c3d0: 2020 2020 2020 6663 5f63 616c 6375 6c61        fc_calcula
-0000c3e0: 746f 725f 6f70 7469 6f6e 733d 4e6f 6e65  tor_options=None
-0000c3f0: 2c0a 2020 2020 293a 0a20 2020 2020 2020  ,.    ):.       
-0000c400: 2022 2222 4361 6c63 756c 6174 6520 6663   """Calculate fc
-0000c410: 3220 6672 6f6d 2064 6973 706c 6163 656d  2 from displacem
-0000c420: 656e 7473 2061 6e64 2066 6f72 6365 732e  ents and forces.
-0000c430: 0a0a 2020 2020 2020 2020 5061 7261 6d65  ..        Parame
-0000c440: 7465 7273 0a20 2020 2020 2020 202d 2d2d  ters.        ---
-0000c450: 2d2d 2d2d 2d2d 2d0a 2020 2020 2020 2020  -------.        
-0000c460: 7379 6d6d 6574 7269 7a65 5f66 6332 203a  symmetrize_fc2 :
-0000c470: 2062 6f6f 6c0a 2020 2020 2020 2020 2020   bool.          
-0000c480: 2020 4f6e 6c79 2066 6f72 2074 7970 6520    Only for type 
-0000c490: 3120 6469 7370 6c61 6365 6d65 6e74 5f64  1 displacement_d
-0000c4a0: 6174 6173 6574 2c20 7472 616e 736c 6174  ataset, translat
-0000c4b0: 696f 6e61 6c20 616e 640a 2020 2020 2020  ional and.      
-0000c4c0: 2020 2020 2020 7065 726d 7574 6174 696f        permutatio
-0000c4d0: 6e20 7379 6d6d 6574 7269 6573 2061 7265  n symmetries are
-0000c4e0: 2061 7070 6c69 6564 2061 6674 6572 2063   applied after c
-0000c4f0: 7265 6174 696e 6720 6663 332e 2054 6869  reating fc3. Thi
-0000c500: 730a 2020 2020 2020 2020 2020 2020 7379  s.            sy
-0000c510: 6d6d 6574 7269 7a61 7469 6f6e 2069 7320  mmetrization is 
-0000c520: 6e6f 7420 7665 7279 2073 6f70 6869 7374  not very sophist
-0000c530: 6963 6174 6564 2061 6e64 2063 616e 2062  icated and can b
-0000c540: 7265 616b 2073 7061 6365 0a20 2020 2020  reak space.     
-0000c550: 2020 2020 2020 2067 726f 7570 2073 796d         group sym
-0000c560: 6d65 7472 792c 2062 7574 206f 6674 656e  metry, but often
-0000c570: 2075 7365 6675 6c2e 2049 6620 6265 7474   useful. If bett
-0000c580: 6572 2073 796d 6d65 7472 697a 6174 696f  er symmetrizatio
-0000c590: 6e20 6973 0a20 2020 2020 2020 2020 2020  n is.           
-0000c5a0: 2065 7870 6563 7465 642c 2069 7420 6973   expected, it is
-0000c5b0: 2072 6563 6f6d 6d65 6e64 6564 2074 6f20   recommended to 
-0000c5c0: 7573 6520 6578 7465 726e 616c 2066 6f72  use external for
-0000c5d0: 6365 2063 6f6e 7374 616e 7473 0a20 2020  ce constants.   
-0000c5e0: 2020 2020 2020 2020 2063 616c 6375 6c61           calcula
-0000c5f0: 746f 7220 7375 6368 2061 7320 414c 4d2e  tor such as ALM.
-0000c600: 2044 6566 6175 6c74 2069 7320 4661 6c73   Default is Fals
-0000c610: 652e 0a20 2020 2020 2020 2069 735f 636f  e..        is_co
-0000c620: 6d70 6163 745f 6663 203a 2062 6f6f 6c0a  mpact_fc : bool.
-0000c630: 2020 2020 2020 2020 2020 2020 6663 3220              fc2 
-0000c640: 7368 6170 6520 6973 0a20 2020 2020 2020  shape is.       
-0000c650: 2020 2020 2020 2020 2046 616c 7365 3a20           False: 
-0000c660: 2873 7570 6572 6365 6c6c 2c20 7375 7065  (supercell, supe
-0000c670: 6365 6c6c 2c20 332c 2033 290a 2020 2020  cell, 3, 3).    
-0000c680: 2020 2020 2020 2020 2020 2020 5472 7565              True
-0000c690: 3a20 2870 7269 6d69 7469 7665 2c20 7375  : (primitive, su
-0000c6a0: 7065 6365 6c6c 2c20 332c 2033 290a 2020  pecell, 3, 3).  
-0000c6b0: 2020 2020 2020 2020 2020 7768 6572 6520            where 
-0000c6c0: 2773 7570 6572 6365 6c6c 2720 616e 6420  'supercell' and 
-0000c6d0: 2770 7269 6d69 7469 7665 2720 696e 6469  'primitive' indi
-0000c6e0: 6361 7465 206e 756d 6265 7220 6f66 2061  cate number of a
-0000c6f0: 746f 6d73 2069 6e20 7468 6573 650a 2020  toms in these.  
-0000c700: 2020 2020 2020 2020 2020 6365 6c6c 732e            cells.
-0000c710: 2044 6566 6175 6c74 2069 7320 4661 6c73   Default is Fals
-0000c720: 652e 0a20 2020 2020 2020 2066 635f 6361  e..        fc_ca
-0000c730: 6c63 756c 6174 6f72 203a 2073 7472 206f  lculator : str o
-0000c740: 7220 4e6f 6e65 0a20 2020 2020 2020 2020  r None.         
-0000c750: 2020 2046 6f72 6365 2063 6f6e 7374 616e     Force constan
-0000c760: 7473 2063 616c 6375 6c61 746f 7220 6769  ts calculator gi
-0000c770: 7665 6e20 6279 2073 7472 2e0a 2020 2020  ven by str..    
-0000c780: 2020 2020 6663 5f63 616c 6375 6c61 746f      fc_calculato
-0000c790: 725f 6f70 7469 6f6e 7320 3a20 6469 6374  r_options : dict
-0000c7a0: 0a20 2020 2020 2020 2020 2020 204f 7074  .            Opt
-0000c7b0: 696f 6e73 2066 6f72 2065 7874 6572 6e61  ions for externa
-0000c7c0: 6c20 666f 7263 6520 636f 6e73 7461 6e74  l force constant
-0000c7d0: 7320 6361 6c63 756c 6174 6f72 2e0a 0a20  s calculator... 
-0000c7e0: 2020 2020 2020 2022 2222 0a20 2020 2020         """.     
-0000c7f0: 2020 2069 6620 7365 6c66 2e5f 7068 6f6e     if self._phon
-0000c800: 6f6e 5f64 6174 6173 6574 2069 7320 4e6f  on_dataset is No
-0000c810: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
-0000c820: 6469 7370 5f64 6174 6173 6574 203d 2073  disp_dataset = s
-0000c830: 656c 662e 5f64 6174 6173 6574 0a20 2020  elf._dataset.   
-0000c840: 2020 2020 2065 6c73 653a 0a20 2020 2020       else:.     
-0000c850: 2020 2020 2020 2064 6973 705f 6461 7461         disp_data
-0000c860: 7365 7420 3d20 7365 6c66 2e5f 7068 6f6e  set = self._phon
-0000c870: 6f6e 5f64 6174 6173 6574 0a0a 2020 2020  on_dataset..    
-0000c880: 2020 2020 6966 2069 735f 636f 6d70 6163      if is_compac
-0000c890: 745f 6663 3a0a 2020 2020 2020 2020 2020  t_fc:.          
-0000c8a0: 2020 7032 735f 6d61 7020 3d20 7365 6c66    p2s_map = self
-0000c8b0: 2e5f 7068 6f6e 6f6e 5f70 7269 6d69 7469  ._phonon_primiti
-0000c8c0: 7665 2e70 3273 5f6d 6170 0a20 2020 2020  ve.p2s_map.     
-0000c8d0: 2020 2065 6c73 653a 0a20 2020 2020 2020     else:.       
-0000c8e0: 2020 2020 2070 3273 5f6d 6170 203d 204e       p2s_map = N
-0000c8f0: 6f6e 650a 0a20 2020 2020 2020 2066 6332  one..        fc2
-0000c900: 5f63 616c 6375 6c61 746f 722c 2066 6332  _calculator, fc2
-0000c910: 5f63 616c 6375 6c61 746f 725f 6f70 7469  _calculator_opti
-0000c920: 6f6e 7320 3d20 7365 6c66 2e5f 6578 7472  ons = self._extr
-0000c930: 6163 745f 6663 325f 6663 335f 6361 6c63  act_fc2_fc3_calc
-0000c940: 756c 6174 6f72 7328 0a20 2020 2020 2020  ulators(.       
-0000c950: 2020 2020 2066 635f 6361 6c63 756c 6174       fc_calculat
-0000c960: 6f72 2c20 6663 5f63 616c 6375 6c61 746f  or, fc_calculato
-0000c970: 725f 6f70 7469 6f6e 732c 2032 0a20 2020  r_options, 2.   
-0000c980: 2020 2020 2029 0a0a 2020 2020 2020 2020       )..        
-0000c990: 6966 2066 6332 5f63 616c 6375 6c61 746f  if fc2_calculato
-0000c9a0: 7220 6973 206e 6f74 204e 6f6e 653a 0a20  r is not None:. 
-0000c9b0: 2020 2020 2020 2020 2020 2064 6973 7073             disps
-0000c9c0: 2c20 666f 7263 6573 203d 2067 6574 5f64  , forces = get_d
-0000c9d0: 6973 706c 6163 656d 656e 7473 5f61 6e64  isplacements_and
-0000c9e0: 5f66 6f72 6365 7328 6469 7370 5f64 6174  _forces(disp_dat
-0000c9f0: 6173 6574 290a 2020 2020 2020 2020 2020  aset).          
-0000ca00: 2020 7365 6c66 2e5f 6663 3220 3d20 6765    self._fc2 = ge
-0000ca10: 745f 6663 3228 0a20 2020 2020 2020 2020  t_fc2(.         
-0000ca20: 2020 2020 2020 2073 656c 662e 5f70 686f         self._pho
-0000ca30: 6e6f 6e5f 7375 7065 7263 656c 6c2c 0a20  non_supercell,. 
-0000ca40: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-0000ca50: 656c 662e 5f70 686f 6e6f 6e5f 7072 696d  elf._phonon_prim
-0000ca60: 6974 6976 652c 0a20 2020 2020 2020 2020  itive,.         
-0000ca70: 2020 2020 2020 2064 6973 7073 2c0a 2020         disps,.  
-0000ca80: 2020 2020 2020 2020 2020 2020 2020 666f                fo
-0000ca90: 7263 6573 2c0a 2020 2020 2020 2020 2020  rces,.          
-0000caa0: 2020 2020 2020 6663 5f63 616c 6375 6c61        fc_calcula
-0000cab0: 746f 723d 6663 325f 6361 6c63 756c 6174  tor=fc2_calculat
-0000cac0: 6f72 2c0a 2020 2020 2020 2020 2020 2020  or,.            
-0000cad0: 2020 2020 6663 5f63 616c 6375 6c61 746f      fc_calculato
-0000cae0: 725f 6f70 7469 6f6e 733d 6663 325f 6361  r_options=fc2_ca
-0000caf0: 6c63 756c 6174 6f72 5f6f 7074 696f 6e73  lculator_options
-0000cb00: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-0000cb10: 2020 6174 6f6d 5f6c 6973 743d 7032 735f    atom_list=p2s_
-0000cb20: 6d61 702c 0a20 2020 2020 2020 2020 2020  map,.           
-0000cb30: 2020 2020 206c 6f67 5f6c 6576 656c 3d73       log_level=s
-0000cb40: 656c 662e 5f6c 6f67 5f6c 6576 656c 2c0a  elf._log_level,.
-0000cb50: 2020 2020 2020 2020 2020 2020 290a 2020              ).  
-0000cb60: 2020 2020 2020 656c 7365 3a0a 2020 2020        else:.    
-0000cb70: 2020 2020 2020 2020 6966 2022 6469 7370          if "disp
-0000cb80: 6c61 6365 6d65 6e74 7322 2069 6e20 6469  lacements" in di
-0000cb90: 7370 5f64 6174 6173 6574 3a0a 2020 2020  sp_dataset:.    
-0000cba0: 2020 2020 2020 2020 2020 2020 6d73 6720              msg 
-0000cbb0: 3d20 280a 2020 2020 2020 2020 2020 2020  = (.            
-0000cbc0: 2020 2020 2020 2020 2266 635f 6361 6c63          "fc_calc
-0000cbd0: 756c 6174 6f72 2068 6173 2074 6f20 6265  ulator has to be
-0000cbe0: 2073 6574 2074 6f20 7072 6f64 7563 6520   set to produce 
-0000cbf0: 666f 7263 6520 220a 2020 2020 2020 2020  force ".        
-0000cc00: 2020 2020 2020 2020 2020 2020 2263 6f6e              "con
-0000cc10: 7374 616e 7320 6672 6f6d 2074 6869 7320  stans from this 
-0000cc20: 6461 7461 7365 7420 666f 7220 6663 322e  dataset for fc2.
-0000cc30: 220a 2020 2020 2020 2020 2020 2020 2020  ".              
-0000cc40: 2020 290a 2020 2020 2020 2020 2020 2020    ).            
-0000cc50: 2020 2020 7261 6973 6520 5275 6e74 696d      raise Runtim
-0000cc60: 6545 7272 6f72 286d 7367 290a 2020 2020  eError(msg).    
-0000cc70: 2020 2020 2020 2020 7365 6c66 2e5f 6663          self._fc
-0000cc80: 3220 3d20 6765 745f 7068 6f6e 6f70 795f  2 = get_phonopy_
-0000cc90: 6663 3228 0a20 2020 2020 2020 2020 2020  fc2(.           
-0000cca0: 2020 2020 2073 656c 662e 5f70 686f 6e6f       self._phono
-0000ccb0: 6e5f 7375 7065 7263 656c 6c2c 0a20 2020  n_supercell,.   
-0000ccc0: 2020 2020 2020 2020 2020 2020 2073 656c               sel
-0000ccd0: 662e 5f70 686f 6e6f 6e5f 7375 7065 7263  f._phonon_superc
-0000cce0: 656c 6c5f 7379 6d6d 6574 7279 2c0a 2020  ell_symmetry,.  
-0000ccf0: 2020 2020 2020 2020 2020 2020 2020 6469                di
-0000cd00: 7370 5f64 6174 6173 6574 2c0a 2020 2020  sp_dataset,.    
-0000cd10: 2020 2020 2020 2020 2020 2020 6174 6f6d              atom
-0000cd20: 5f6c 6973 743d 7032 735f 6d61 702c 0a20  _list=p2s_map,. 
-0000cd30: 2020 2020 2020 2020 2020 2029 0a20 2020             ).   
-0000cd40: 2020 2020 2020 2020 2069 6620 7379 6d6d           if symm
-0000cd50: 6574 7269 7a65 5f66 6332 3a0a 2020 2020  etrize_fc2:.    
-0000cd60: 2020 2020 2020 2020 2020 2020 6966 2069              if i
-0000cd70: 735f 636f 6d70 6163 745f 6663 3a0a 2020  s_compact_fc:.  
-0000cd80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000cd90: 2020 7379 6d6d 6574 7269 7a65 5f63 6f6d    symmetrize_com
-0000cda0: 7061 6374 5f66 6f72 6365 5f63 6f6e 7374  pact_force_const
-0000cdb0: 616e 7473 280a 2020 2020 2020 2020 2020  ants(.          
-0000cdc0: 2020 2020 2020 2020 2020 2020 2020 7365                se
-0000cdd0: 6c66 2e5f 6663 322c 2073 656c 662e 5f70  lf._fc2, self._p
-0000cde0: 686f 6e6f 6e5f 7072 696d 6974 6976 650a  honon_primitive.
-0000cdf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ce00: 2020 2020 290a 2020 2020 2020 2020 2020      ).          
-0000ce10: 2020 2020 2020 656c 7365 3a0a 2020 2020        else:.    
-0000ce20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ce30: 7379 6d6d 6574 7269 7a65 5f66 6f72 6365  symmetrize_force
-0000ce40: 5f63 6f6e 7374 616e 7473 2873 656c 662e  _constants(self.
-0000ce50: 5f66 6332 290a 0a20 2020 2064 6566 2063  _fc2)..    def c
-0000ce60: 7574 6f66 665f 6663 335f 6279 5f7a 6572  utoff_fc3_by_zer
-0000ce70: 6f28 7365 6c66 2c20 6375 746f 6666 5f64  o(self, cutoff_d
-0000ce80: 6973 7461 6e63 652c 2066 6333 3d4e 6f6e  istance, fc3=Non
-0000ce90: 6529 3a0a 2020 2020 2020 2020 2222 2253  e):.        """S
-0000cea0: 6574 207a 6572 6f20 746f 2066 6333 2065  et zero to fc3 e
-0000ceb0: 6c65 6d65 6e74 7320 6f75 7420 6f66 2063  lements out of c
-0000cec0: 7574 6f66 6620 6469 7374 616e 6365 2e0a  utoff distance..
-0000ced0: 0a20 2020 2020 2020 204e 6f74 650a 2020  .        Note.  
-0000cee0: 2020 2020 2020 2d2d 2d2d 0a20 2020 2020        ----.     
-0000cef0: 2020 2066 6333 2069 7320 6f76 6572 7772     fc3 is overwr
-0000cf00: 6974 7465 6e2e 0a0a 2020 2020 2020 2020  itten...        
-0000cf10: 5061 7261 6d65 7465 7273 0a20 2020 2020  Parameters.     
-0000cf20: 2020 202d 2d2d 2d2d 2d2d 2d2d 2d0a 2020     ----------.  
-0000cf30: 2020 2020 2020 6375 746f 6666 5f64 6973        cutoff_dis
-0000cf40: 7461 6e63 6520 3a20 666c 6f61 740a 2020  tance : float.  
-0000cf50: 2020 2020 2020 2020 2020 4166 7465 7220            After 
-0000cf60: 6372 6561 7469 6e67 2066 6f72 6365 2063  creating force c
-0000cf70: 6f6e 7374 616e 7473 2c20 6663 2065 6c65  onstants, fc ele
-0000cf80: 6d65 6e74 7320 7768 6572 6520 616e 7920  ments where any 
-0000cf90: 7061 6972 0a20 2020 2020 2020 2020 2020  pair.           
-0000cfa0: 2064 6973 7461 6e63 6520 696e 2061 746f   distance in ato
-0000cfb0: 6d20 7472 6970 6c65 7473 206c 6172 6765  m triplets large
-0000cfc0: 7220 7468 616e 2063 7574 6f66 665f 6469  r than cutoff_di
-0000cfd0: 7374 616e 6365 2061 7265 2073 6574 207a  stance are set z
-0000cfe0: 6572 6f2e 0a0a 2020 2020 2020 2020 2222  ero...        ""
-0000cff0: 220a 2020 2020 2020 2020 6966 2066 6333  ".        if fc3
-0000d000: 2069 7320 4e6f 6e65 3a0a 2020 2020 2020   is None:.      
-0000d010: 2020 2020 2020 5f66 6333 203d 2073 656c        _fc3 = sel
-0000d020: 662e 5f66 6333 0a20 2020 2020 2020 2065  f._fc3.        e
-0000d030: 6c73 653a 0a20 2020 2020 2020 2020 2020  lse:.           
-0000d040: 205f 6663 3320 3d20 6663 330a 2020 2020   _fc3 = fc3.    
-0000d050: 2020 2020 6375 746f 6666 5f66 6333 5f62      cutoff_fc3_b
-0000d060: 795f 7a65 726f 280a 2020 2020 2020 2020  y_zero(.        
-0000d070: 2020 2020 5f66 6333 2c0a 2020 2020 2020      _fc3,.      
-0000d080: 2020 2020 2020 7365 6c66 2e5f 7375 7065        self._supe
-0000d090: 7263 656c 6c2c 0a20 2020 2020 2020 2020  rcell,.         
-0000d0a0: 2020 2063 7574 6f66 665f 6469 7374 616e     cutoff_distan
-0000d0b0: 6365 2c0a 2020 2020 2020 2020 2020 2020  ce,.            
-0000d0c0: 7032 735f 6d61 703d 7365 6c66 2e5f 7072  p2s_map=self._pr
-0000d0d0: 696d 6974 6976 652e 7032 735f 6d61 702c  imitive.p2s_map,
-0000d0e0: 0a20 2020 2020 2020 2020 2020 2073 796d  .            sym
-0000d0f0: 7072 6563 3d73 656c 662e 5f73 796d 7072  prec=self._sympr
-0000d100: 6563 2c0a 2020 2020 2020 2020 290a 0a20  ec,.        ).. 
-0000d110: 2020 2064 6566 2073 6574 5f70 6572 6d75     def set_permu
-0000d120: 7461 7469 6f6e 5f73 796d 6d65 7472 7928  tation_symmetry(
-0000d130: 7365 6c66 293a 0a20 2020 2020 2020 2022  self):.        "
-0000d140: 2222 456e 666f 7263 6520 7065 726d 7574  ""Enforce permut
-0000d150: 6174 696f 6e20 7379 6d6d 6574 7279 2074  ation symmetry t
-0000d160: 6f20 6663 3220 616e 6420 6663 332e 2222  o fc2 and fc3.""
-0000d170: 220a 2020 2020 2020 2020 6966 2073 656c  ".        if sel
-0000d180: 662e 5f66 6332 2069 7320 6e6f 7420 4e6f  f._fc2 is not No
-0000d190: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
-0000d1a0: 7365 745f 7065 726d 7574 6174 696f 6e5f  set_permutation_
-0000d1b0: 7379 6d6d 6574 7279 2873 656c 662e 5f66  symmetry(self._f
-0000d1c0: 6332 290a 2020 2020 2020 2020 6966 2073  c2).        if s
-0000d1d0: 656c 662e 5f66 6333 2069 7320 6e6f 7420  elf._fc3 is not 
-0000d1e0: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
-0000d1f0: 2020 7365 745f 7065 726d 7574 6174 696f    set_permutatio
-0000d200: 6e5f 7379 6d6d 6574 7279 5f66 6333 2873  n_symmetry_fc3(s
-0000d210: 656c 662e 5f66 6333 290a 0a20 2020 2064  elf._fc3)..    d
-0000d220: 6566 2073 6574 5f74 7261 6e73 6c61 7469  ef set_translati
-0000d230: 6f6e 616c 5f69 6e76 6172 6961 6e63 6528  onal_invariance(
-0000d240: 7365 6c66 293a 0a20 2020 2020 2020 2022  self):.        "
-0000d250: 2222 456e 666f 7263 6520 7472 616e 736c  ""Enforce transl
-0000d260: 6174 696f 6e20 696e 7661 7269 616e 6365  ation invariance
-0000d270: 2e0a 0a20 2020 2020 2020 2054 6869 7320  ...        This 
-0000d280: 7375 6274 7261 6374 7320 6472 6966 7420  subtracts drift 
-0000d290: 6469 7669 6465 6420 6279 206e 756d 6265  divided by numbe
-0000d2a0: 7220 6f66 2065 6c65 6d65 6e74 7320 696e  r of elements in
-0000d2b0: 2065 6163 6820 726f 7720 616e 640a 2020   each row and.  
-0000d2c0: 2020 2020 2020 636f 6c75 6d6e 2e0a 0a20        column... 
-0000d2d0: 2020 2020 2020 2022 2222 0a20 2020 2020         """.     
-0000d2e0: 2020 2069 6620 7365 6c66 2e5f 6663 3220     if self._fc2 
-0000d2f0: 6973 206e 6f74 204e 6f6e 653a 0a20 2020  is not None:.   
-0000d300: 2020 2020 2020 2020 2073 6574 5f74 7261           set_tra
-0000d310: 6e73 6c61 7469 6f6e 616c 5f69 6e76 6172  nslational_invar
-0000d320: 6961 6e63 6528 7365 6c66 2e5f 6663 3229  iance(self._fc2)
-0000d330: 0a20 2020 2020 2020 2069 6620 7365 6c66  .        if self
-0000d340: 2e5f 6663 3320 6973 206e 6f74 204e 6f6e  ._fc3 is not Non
-0000d350: 653a 0a20 2020 2020 2020 2020 2020 2073  e:.            s
-0000d360: 6574 5f74 7261 6e73 6c61 7469 6f6e 616c  et_translational
-0000d370: 5f69 6e76 6172 6961 6e63 655f 6663 3328  _invariance_fc3(
-0000d380: 7365 6c66 2e5f 6663 3329 0a0a 2020 2020  self._fc3)..    
-0000d390: 6465 6620 7275 6e5f 696d 6167 5f73 656c  def run_imag_sel
-0000d3a0: 665f 656e 6572 6779 280a 2020 2020 2020  f_energy(.      
-0000d3b0: 2020 7365 6c66 2c0a 2020 2020 2020 2020    self,.        
-0000d3c0: 6772 6964 5f70 6f69 6e74 732c 0a20 2020  grid_points,.   
-0000d3d0: 2020 2020 2074 656d 7065 7261 7475 7265       temperature
-0000d3e0: 732c 0a20 2020 2020 2020 2066 7265 7175  s,.        frequ
-0000d3f0: 656e 6379 5f70 6f69 6e74 733d 4e6f 6e65  ency_points=None
-0000d400: 2c0a 2020 2020 2020 2020 6672 6571 7565  ,.        freque
-0000d410: 6e63 795f 7374 6570 3d4e 6f6e 652c 0a20  ncy_step=None,. 
-0000d420: 2020 2020 2020 206e 756d 5f66 7265 7175         num_frequ
-0000d430: 656e 6379 5f70 6f69 6e74 733d 4e6f 6e65  ency_points=None
-0000d440: 2c0a 2020 2020 2020 2020 6e75 6d5f 706f  ,.        num_po
-0000d450: 696e 7473 5f69 6e5f 6261 7463 683d 4e6f  ints_in_batch=No
-0000d460: 6e65 2c0a 2020 2020 2020 2020 6672 6571  ne,.        freq
-0000d470: 7565 6e63 795f 706f 696e 7473 5f61 745f  uency_points_at_
-0000d480: 6261 6e64 733d 4661 6c73 652c 0a20 2020  bands=False,.   
-0000d490: 2020 2020 2073 6361 7474 6572 696e 675f       scattering_
-0000d4a0: 6576 656e 745f 636c 6173 733d 4e6f 6e65  event_class=None
-0000d4b0: 2c0a 2020 2020 2020 2020 7772 6974 655f  ,.        write_
-0000d4c0: 7478 743d 4661 6c73 652c 0a20 2020 2020  txt=False,.     
-0000d4d0: 2020 2077 7269 7465 5f67 616d 6d61 5f64     write_gamma_d
-0000d4e0: 6574 6169 6c3d 4661 6c73 652c 0a20 2020  etail=False,.   
-0000d4f0: 2020 2020 206b 6565 705f 6761 6d6d 615f       keep_gamma_
-0000d500: 6465 7461 696c 3d46 616c 7365 2c0a 2020  detail=False,.  
-0000d510: 2020 2020 2020 6f75 7470 7574 5f66 696c        output_fil
-0000d520: 656e 616d 653d 4e6f 6e65 2c0a 2020 2020  ename=None,.    
-0000d530: 293a 0a20 2020 2020 2020 2022 2222 4361  ):.        """Ca
-0000d540: 6c63 756c 6174 6520 696d 6167 696e 6172  lculate imaginar
-0000d550: 7920 7061 7274 206f 6620 7365 6c66 2d65  y part of self-e
-0000d560: 6e65 7267 7920 6f66 2062 7562 626c 6520  nergy of bubble 
-0000d570: 6469 6167 7261 6d20 2847 616d 6d61 292e  diagram (Gamma).
-0000d580: 0a0a 2020 2020 2020 2020 5069 203d 2044  ..        Pi = D
-0000d590: 656c 7461 202d 2069 2047 616d 6d61 2e0a  elta - i Gamma..
-0000d5a0: 0a20 2020 2020 2020 2050 6172 616d 6574  .        Paramet
-0000d5b0: 6572 730a 2020 2020 2020 2020 2d2d 2d2d  ers.        ----
-0000d5c0: 2d2d 2d2d 2d2d 0a20 2020 2020 2020 2067  ------.        g
-0000d5d0: 7269 645f 706f 696e 7473 203a 2061 7272  rid_points : arr
-0000d5e0: 6179 5f6c 696b 650a 2020 2020 2020 2020  ay_like.        
-0000d5f0: 2020 2020 4772 6964 2d70 6f69 6e74 2069      Grid-point i
-0000d600: 6e64 6963 6573 2077 6865 7265 2069 6d61  ndices where ima
-0000d610: 6769 6e61 7279 2070 6172 7420 6f66 2073  ginary part of s
-0000d620: 656c 662d 656e 6572 6769 6573 2061 7265  elf-energies are
-0000d630: 0a20 2020 2020 2020 2020 2020 2063 6163  .            cac
-0000d640: 6c63 756c 6174 6564 2e0a 2020 2020 2020  lculated..      
-0000d650: 2020 2020 2020 6474 7970 653d 696e 742c        dtype=int,
-0000d660: 2073 6861 7065 3d28 6772 6964 5f70 6f69   shape=(grid_poi
-0000d670: 6e74 732c 290a 2020 2020 2020 2020 7465  nts,).        te
-0000d680: 6d70 6572 6174 7572 6573 203a 2061 7272  mperatures : arr
-0000d690: 6179 5f6c 696b 650a 2020 2020 2020 2020  ay_like.        
-0000d6a0: 2020 2020 5465 6d70 6572 6174 7572 6573      Temperatures
-0000d6b0: 2077 6865 7265 2069 6d61 6769 6e61 7279   where imaginary
-0000d6c0: 2070 6172 7420 6f66 2073 656c 662d 656e   part of self-en
-0000d6d0: 6572 6769 6573 2061 7265 2063 616c 6375  ergies are calcu
-0000d6e0: 6c61 7465 642e 0a20 2020 2020 2020 2020  lated..         
-0000d6f0: 2020 2064 7479 7065 3d66 6c6f 6174 2c20     dtype=float, 
-0000d700: 7368 6170 653d 2874 656d 7065 7261 7475  shape=(temperatu
-0000d710: 7265 732c 290a 2020 2020 2020 2020 6672  res,).        fr
-0000d720: 6571 7565 6e63 795f 706f 696e 7473 203a  equency_points :
-0000d730: 2061 7272 6179 5f6c 696b 652c 206f 7074   array_like, opt
-0000d740: 696f 6e61 6c0a 2020 2020 2020 2020 2020  ional.          
-0000d750: 2020 4672 6571 7565 6e63 7920 7361 6d70    Frequency samp
-0000d760: 6c69 6e67 2070 6f69 6e74 732e 2044 6566  ling points. Def
-0000d770: 6175 6c74 2069 7320 4e6f 6e65 2e20 5769  ault is None. Wi
-0000d780: 7468 0a20 2020 2020 2020 2020 2020 2066  th.            f
-0000d790: 7265 7175 656e 6379 5f70 6f69 6e74 735f  requency_points_
-0000d7a0: 6174 5f62 616e 6473 3d46 616c 7365 2061  at_bands=False a
-0000d7b0: 6e64 2066 7265 7175 656e 6379 5f70 6f69  nd frequency_poi
-0000d7c0: 6e74 7320 6973 204e 6f6e 652c 0a20 2020  nts is None,.   
-0000d7d0: 2020 2020 2020 2020 206e 756d 5f66 7265           num_fre
-0000d7e0: 7175 656e 6379 5f70 6f69 6e74 7320 6f72  quency_points or
-0000d7f0: 2066 7265 7175 656e 6379 5f73 7465 7020   frequency_step 
-0000d800: 6973 2075 7365 6420 746f 2067 656e 6572  is used to gener
-0000d810: 6174 6520 756e 6966 6f72 6d0a 2020 2020  ate uniform.    
-0000d820: 2020 2020 2020 2020 6672 6571 7565 6e63          frequenc
-0000d830: 7920 7361 6d70 6c69 6e67 2070 6f69 6e74  y sampling point
-0000d840: 732e 0a20 2020 2020 2020 2020 2020 2064  s..            d
-0000d850: 7479 7065 3d66 6c6f 6174 2c20 7368 6170  type=float, shap
-0000d860: 653d 2866 7265 7175 656e 6379 5f70 6f69  e=(frequency_poi
-0000d870: 6e74 732c 290a 2020 2020 2020 2020 6672  nts,).        fr
-0000d880: 6571 7565 6e63 795f 7374 6570 203a 2066  equency_step : f
-0000d890: 6c6f 6174 2c20 6f70 7469 6f6e 616c 0a20  loat, optional. 
-0000d8a0: 2020 2020 2020 2020 2020 2055 6e69 666f             Unifo
-0000d8b0: 726d 2070 6974 6368 206f 6620 6672 6571  rm pitch of freq
-0000d8c0: 7565 6e63 7920 7361 6d70 6c69 6e67 2070  uency sampling p
-0000d8d0: 6f69 6e74 732e 2044 6566 6175 6c74 2069  oints. Default i
-0000d8e0: 7320 4e6f 6e65 2e20 5468 6973 0a20 2020  s None. This.   
-0000d8f0: 2020 2020 2020 2020 2072 6573 756c 7473           results
-0000d900: 2069 6e20 7573 696e 6720 6e75 6d5f 6672   in using num_fr
-0000d910: 6571 7565 6e63 795f 706f 696e 7473 2e0a  equency_points..
-0000d920: 2020 2020 2020 2020 6e75 6d5f 6672 6571          num_freq
-0000d930: 7565 6e63 795f 706f 696e 7473 3a20 496e  uency_points: In
-0000d940: 742c 206f 7074 696f 6e61 6c0a 2020 2020  t, optional.    
-0000d950: 2020 2020 2020 2020 4e75 6d62 6572 206f          Number o
-0000d960: 6620 7361 6d70 6c69 6e67 2073 616d 706c  f sampling sampl
-0000d970: 696e 6720 706f 696e 7473 2074 6f20 6265  ing points to be
-0000d980: 2075 7365 6420 696e 7374 6561 6420 6f66   used instead of
-0000d990: 0a20 2020 2020 2020 2020 2020 2066 7265  .            fre
-0000d9a0: 7175 656e 6379 5f73 7465 702e 2054 6869  quency_step. Thi
-0000d9b0: 7320 6e75 6d62 6572 2069 6e63 6c75 6465  s number include
-0000d9c0: 7320 656e 6420 706f 696e 7473 2e20 4465  s end points. De
-0000d9d0: 6661 756c 7420 6973 204e 6f6e 652c 0a20  fault is None,. 
-0000d9e0: 2020 2020 2020 2020 2020 2077 6869 6368             which
-0000d9f0: 2067 6976 6573 2032 3031 2e0a 2020 2020   gives 201..    
-0000da00: 2020 2020 6e75 6d5f 706f 696e 7473 5f69      num_points_i
-0000da10: 6e5f 6261 7463 683a 2069 6e74 2c20 6f70  n_batch: int, op
-0000da20: 7469 6f6e 616c 0a20 2020 2020 2020 2020  tional.         
-0000da30: 2020 204e 756d 6265 7220 6f66 2073 616d     Number of sam
-0000da40: 706c 696e 6720 706f 696e 7473 2069 6e20  pling points in 
-0000da50: 6f6e 6520 6261 7463 682e 2054 6869 7320  one batch. This 
-0000da60: 6973 2066 6f72 2074 6865 2066 7265 7175  is for the frequ
-0000da70: 656e 6379 0a20 2020 2020 2020 2020 2020  ency.           
-0000da80: 2073 616d 706c 696e 6720 6d6f 6465 2061   sampling mode a
-0000da90: 6e64 2074 6865 2073 616d 706c 696e 6720  nd the sampling 
-0000daa0: 706f 696e 7473 2061 7265 2064 6976 6964  points are divid
-0000dab0: 6564 2069 6e74 6f20 6261 7463 6865 732e  ed into batches.
-0000dac0: 0a20 2020 2020 2020 2020 2020 204c 6167  .            Lag
-0000dad0: 6572 206e 756d 6265 7220 7072 6f76 6964  er number provid
-0000dae0: 6573 2065 6666 6963 6965 6e74 2075 7365  es efficient use
-0000daf0: 206f 6620 6d75 6c74 692d 636f 7265 7320   of multi-cores 
-0000db00: 6275 7420 6d6f 7265 0a20 2020 2020 2020  but more.       
-0000db10: 2020 2020 206d 656d 6f72 7920 6465 6d61       memory dema
-0000db20: 6e64 696e 672e 2044 6566 6175 6c74 2069  nding. Default i
-0000db30: 7320 4e6f 6e65 2c20 7768 6963 6820 6769  s None, which gi
-0000db40: 7665 2074 6865 206e 756d 6265 7220 6f66  ve the number of
-0000db50: 2031 302e 0a20 2020 2020 2020 2066 7265   10..        fre
-0000db60: 7175 656e 6379 5f70 6f69 6e74 735f 6174  quency_points_at
-0000db70: 5f62 616e 6473 203a 2062 6f6f 6c2c 206f  _bands : bool, o
-0000db80: 7074 696f 6e61 6c0a 2020 2020 2020 2020  ptional.        
-0000db90: 2020 2020 5068 6f6e 6f6e 2062 616e 6420      Phonon band 
-0000dba0: 6672 6571 7565 6e63 6965 7320 6172 6520  frequencies are 
-0000dbb0: 7573 6564 2061 7320 6672 6571 7565 6e63  used as frequenc
-0000dbc0: 7920 706f 696e 7473 2077 6865 6e20 5472  y points when Tr
-0000dbd0: 7565 2e0a 2020 2020 2020 2020 2020 2020  ue..            
-0000dbe0: 4465 6661 756c 7420 6973 2046 616c 7365  Default is False
-0000dbf0: 2e0a 2020 2020 2020 2020 7363 6174 7465  ..        scatte
-0000dc00: 7269 6e67 5f65 7665 6e74 5f63 6c61 7373  ring_event_class
-0000dc10: 203a 2069 6e74 2c20 6f70 7469 6f6e 616c   : int, optional
-0000dc20: 0a20 2020 2020 2020 2020 2020 2053 7065  .            Spe
-0000dc30: 6369 6669 6320 6368 6f69 6365 206f 6620  cific choice of 
-0000dc40: 7363 6174 7465 7269 6e67 2065 7665 6e74  scattering event
-0000dc50: 2063 6c61 7373 2c20 3120 6f72 2032 2074   class, 1 or 2 t
-0000dc60: 6861 7420 6973 2073 7065 6369 6669 6564  hat is specified
-0000dc70: 0a20 2020 2020 2020 2020 2020 2031 206f  .            1 o
-0000dc80: 7220 322c 2072 6573 7065 6374 6976 656c  r 2, respectivel
-0000dc90: 792e 2054 6865 2072 6573 756c 7420 6973  y. The result is
-0000dca0: 2073 746f 7265 6420 696e 2067 616d 6d61   stored in gamma
-0000dcb0: 732e 2054 6865 7265 666f 7265 0a20 2020  s. Therefore.   
-0000dcc0: 2020 2020 2020 2020 2075 7375 616c 2067           usual g
-0000dcd0: 616d 6d61 7320 6172 6520 6e6f 7420 7374  ammas are not st
-0000dce0: 6f72 6564 2069 6e20 7468 6520 7661 7269  ored in the vari
-0000dcf0: 6162 6c65 2e20 4465 6661 756c 7420 6973  able. Default is
-0000dd00: 204e 6f6e 652c 2077 6869 6368 0a20 2020   None, which.   
-0000dd10: 2020 2020 2020 2020 2064 6f65 736e 2774           doesn't
-0000dd20: 2073 7065 6369 6679 2073 6361 7474 6572   specify scatter
-0000dd30: 696e 675f 6576 656e 745f 636c 6173 732e  ing_event_class.
-0000dd40: 0a20 2020 2020 2020 2077 7269 7465 5f74  .        write_t
-0000dd50: 7874 203a 2062 6f6f 6c2c 206f 7074 696f  xt : bool, optio
-0000dd60: 6e61 6c0a 2020 2020 2020 2020 2020 2020  nal.            
-0000dd70: 4672 6571 7565 6e63 7920 706f 696e 7473  Frequency points
-0000dd80: 2061 6e64 2069 6d61 6769 6e61 7279 2070   and imaginary p
-0000dd90: 6172 7420 6f66 2073 656c 662d 656e 6572  art of self-ener
-0000dda0: 6769 6573 2061 7265 2077 7269 7474 656e  gies are written
-0000ddb0: 0a20 2020 2020 2020 2020 2020 2069 6e74  .            int
-0000ddc0: 6f20 7465 7874 2066 696c 6573 2e0a 2020  o text files..  
-0000ddd0: 2020 2020 2020 7772 6974 655f 6761 6d6d        write_gamm
-0000dde0: 615f 6465 7461 696c 203a 2062 6f6f 6c2c  a_detail : bool,
-0000ddf0: 206f 7074 696f 6e61 6c0a 2020 2020 2020   optional.      
-0000de00: 2020 2020 2020 4465 7461 696c 6564 2067        Detailed g
-0000de10: 616d 6d61 7320 6172 6520 7772 6974 7465  ammas are writte
-0000de20: 6e20 696e 746f 2061 2066 696c 6520 696e  n into a file in
-0000de30: 2068 6466 352e 2044 6566 6175 6c74 2069   hdf5. Default i
-0000de40: 7320 4661 6c73 652e 0a20 2020 2020 2020  s False..       
-0000de50: 206b 6565 705f 6761 6d6d 615f 6465 7461   keep_gamma_deta
-0000de60: 696c 203a 2062 6f6f 6c2c 206f 7074 696f  il : bool, optio
-0000de70: 6e61 6c0a 2020 2020 2020 2020 2020 2020  nal.            
-0000de80: 5769 7468 2054 7275 652c 2064 6574 6169  With True, detai
-0000de90: 6c65 6420 6761 6d6d 6173 2061 7265 2073  led gammas are s
-0000dea0: 746f 7265 642e 2044 6566 6175 6c74 2069  tored. Default i
-0000deb0: 7320 4661 6c73 652e 0a20 2020 2020 2020  s False..       
-0000dec0: 206f 7574 7075 745f 6669 6c65 6e61 6d65   output_filename
-0000ded0: 203a 2073 7472 0a20 2020 2020 2020 2020   : str.         
-0000dee0: 2020 2054 6869 7320 7374 7269 6e67 2069     This string i
-0000def0: 7320 696e 7365 7274 6564 2069 6e20 7468  s inserted in th
-0000df00: 6520 6f75 7470 7574 2066 696c 6520 6e61  e output file na
-0000df10: 6d65 732e 0a0a 2020 2020 2020 2020 2222  mes...        ""
-0000df20: 220a 2020 2020 2020 2020 6966 2073 656c  ".        if sel
-0000df30: 662e 5f69 6e74 6572 6163 7469 6f6e 2069  f._interaction i
-0000df40: 7320 4e6f 6e65 3a0a 2020 2020 2020 2020  s None:.        
-0000df50: 2020 2020 6d73 6720 3d20 280a 2020 2020      msg = (.    
-0000df60: 2020 2020 2020 2020 2020 2020 2250 686f              "Pho
-0000df70: 6e6f 3370 792e 696e 6974 5f70 6870 685f  no3py.init_phph_
-0000df80: 696e 7465 7261 6374 696f 6e20 6861 7320  interaction has 
-0000df90: 746f 2062 6520 6361 6c6c 6564 2022 0a20  to be called ". 
-0000dfa0: 2020 2020 2020 2020 2020 2020 2020 2022                 "
-0000dfb0: 6265 666f 7265 2072 756e 6e69 6e67 2074  before running t
-0000dfc0: 6869 7320 6d65 7468 6f64 2e22 0a20 2020  his method.".   
-0000dfd0: 2020 2020 2020 2020 2029 0a20 2020 2020           ).     
-0000dfe0: 2020 2020 2020 2072 6169 7365 2052 756e         raise Run
-0000dff0: 7469 6d65 4572 726f 7228 6d73 6729 0a0a  timeError(msg)..
-0000e000: 2020 2020 2020 2020 6966 2074 656d 7065          if tempe
-0000e010: 7261 7475 7265 7320 6973 204e 6f6e 653a  ratures is None:
-0000e020: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
-0000e030: 662e 5f74 656d 7065 7261 7475 7265 7320  f._temperatures 
-0000e040: 3d20 5b0a 2020 2020 2020 2020 2020 2020  = [.            
-0000e050: 2020 2020 3330 302e 302c 0a20 2020 2020      300.0,.     
-0000e060: 2020 2020 2020 205d 0a20 2020 2020 2020         ].       
-0000e070: 2065 6c73 653a 0a20 2020 2020 2020 2020   else:.         
-0000e080: 2020 2073 656c 662e 5f74 656d 7065 7261     self._tempera
-0000e090: 7475 7265 7320 3d20 7465 6d70 6572 6174  tures = temperat
-0000e0a0: 7572 6573 0a20 2020 2020 2020 2073 656c  ures.        sel
-0000e0b0: 662e 5f67 7269 645f 706f 696e 7473 203d  f._grid_points =
-0000e0c0: 2067 7269 645f 706f 696e 7473 0a20 2020   grid_points.   
-0000e0d0: 2020 2020 2073 656c 662e 5f73 6361 7474       self._scatt
-0000e0e0: 6572 696e 675f 6576 656e 745f 636c 6173  ering_event_clas
-0000e0f0: 7320 3d20 7363 6174 7465 7269 6e67 5f65  s = scattering_e
-0000e100: 7665 6e74 5f63 6c61 7373 0a20 2020 2020  vent_class.     
-0000e110: 2020 2076 616c 7320 3d20 6765 745f 696d     vals = get_im
-0000e120: 6167 5f73 656c 665f 656e 6572 6779 280a  ag_self_energy(.
-0000e130: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-0000e140: 2e5f 696e 7465 7261 6374 696f 6e2c 0a20  ._interaction,. 
-0000e150: 2020 2020 2020 2020 2020 2067 7269 645f             grid_
-0000e160: 706f 696e 7473 2c0a 2020 2020 2020 2020  points,.        
-0000e170: 2020 2020 7465 6d70 6572 6174 7572 6573      temperatures
-0000e180: 2c0a 2020 2020 2020 2020 2020 2020 7369  ,.            si
-0000e190: 676d 6173 3d73 656c 662e 5f73 6967 6d61  gmas=self._sigma
-0000e1a0: 732c 0a20 2020 2020 2020 2020 2020 2066  s,.            f
-0000e1b0: 7265 7175 656e 6379 5f70 6f69 6e74 733d  requency_points=
-0000e1c0: 6672 6571 7565 6e63 795f 706f 696e 7473  frequency_points
-0000e1d0: 2c0a 2020 2020 2020 2020 2020 2020 6672  ,.            fr
-0000e1e0: 6571 7565 6e63 795f 7374 6570 3d66 7265  equency_step=fre
-0000e1f0: 7175 656e 6379 5f73 7465 702c 0a20 2020  quency_step,.   
-0000e200: 2020 2020 2020 2020 2066 7265 7175 656e           frequen
-0000e210: 6379 5f70 6f69 6e74 735f 6174 5f62 616e  cy_points_at_ban
-0000e220: 6473 3d66 7265 7175 656e 6379 5f70 6f69  ds=frequency_poi
-0000e230: 6e74 735f 6174 5f62 616e 6473 2c0a 2020  nts_at_bands,.  
-0000e240: 2020 2020 2020 2020 2020 6e75 6d5f 6672            num_fr
-0000e250: 6571 7565 6e63 795f 706f 696e 7473 3d6e  equency_points=n
-0000e260: 756d 5f66 7265 7175 656e 6379 5f70 6f69  um_frequency_poi
-0000e270: 6e74 732c 0a20 2020 2020 2020 2020 2020  nts,.           
-0000e280: 206e 756d 5f70 6f69 6e74 735f 696e 5f62   num_points_in_b
-0000e290: 6174 6368 3d6e 756d 5f70 6f69 6e74 735f  atch=num_points_
-0000e2a0: 696e 5f62 6174 6368 2c0a 2020 2020 2020  in_batch,.      
-0000e2b0: 2020 2020 2020 7363 6174 7465 7269 6e67        scattering
-0000e2c0: 5f65 7665 6e74 5f63 6c61 7373 3d73 6361  _event_class=sca
-0000e2d0: 7474 6572 696e 675f 6576 656e 745f 636c  ttering_event_cl
-0000e2e0: 6173 732c 0a20 2020 2020 2020 2020 2020  ass,.           
-0000e2f0: 2077 7269 7465 5f67 616d 6d61 5f64 6574   write_gamma_det
-0000e300: 6169 6c3d 7772 6974 655f 6761 6d6d 615f  ail=write_gamma_
-0000e310: 6465 7461 696c 2c0a 2020 2020 2020 2020  detail,.        
-0000e320: 2020 2020 7265 7475 726e 5f67 616d 6d61      return_gamma
-0000e330: 5f64 6574 6169 6c3d 6b65 6570 5f67 616d  _detail=keep_gam
-0000e340: 6d61 5f64 6574 6169 6c2c 0a20 2020 2020  ma_detail,.     
-0000e350: 2020 2020 2020 206f 7574 7075 745f 6669         output_fi
-0000e360: 6c65 6e61 6d65 3d6f 7574 7075 745f 6669  lename=output_fi
-0000e370: 6c65 6e61 6d65 2c0a 2020 2020 2020 2020  lename,.        
-0000e380: 2020 2020 6c6f 675f 6c65 7665 6c3d 7365      log_level=se
-0000e390: 6c66 2e5f 6c6f 675f 6c65 7665 6c2c 0a20  lf._log_level,. 
-0000e3a0: 2020 2020 2020 2029 0a20 2020 2020 2020         ).       
-0000e3b0: 2069 6620 6b65 6570 5f67 616d 6d61 5f64   if keep_gamma_d
-0000e3c0: 6574 6169 6c3a 0a20 2020 2020 2020 2020  etail:.         
-0000e3d0: 2020 2028 7365 6c66 2e5f 6672 6571 7565     (self._freque
-0000e3e0: 6e63 795f 706f 696e 7473 2c20 7365 6c66  ncy_points, self
-0000e3f0: 2e5f 6761 6d6d 6173 2c20 7365 6c66 2e5f  ._gammas, self._
-0000e400: 6465 7461 696c 6564 5f67 616d 6d61 7329  detailed_gammas)
-0000e410: 203d 2076 616c 730a 2020 2020 2020 2020   = vals.        
-0000e420: 656c 7365 3a0a 2020 2020 2020 2020 2020  else:.          
-0000e430: 2020 7365 6c66 2e5f 6672 6571 7565 6e63    self._frequenc
-0000e440: 795f 706f 696e 7473 2c20 7365 6c66 2e5f  y_points, self._
-0000e450: 6761 6d6d 6173 203d 2076 616c 730a 0a20  gammas = vals.. 
-0000e460: 2020 2020 2020 2069 6620 7772 6974 655f         if write_
-0000e470: 7478 743a 0a20 2020 2020 2020 2020 2020  txt:.           
-0000e480: 2073 656c 662e 5f77 7269 7465 5f69 6d61   self._write_ima
-0000e490: 675f 7365 6c66 5f65 6e65 7267 7928 6f75  g_self_energy(ou
-0000e4a0: 7470 7574 5f66 696c 656e 616d 653d 6f75  tput_filename=ou
-0000e4b0: 7470 7574 5f66 696c 656e 616d 6529 0a0a  tput_filename)..
-0000e4c0: 2020 2020 2020 2020 7265 7475 726e 2076          return v
-0000e4d0: 616c 730a 0a20 2020 2064 6566 205f 7772  als..    def _wr
-0000e4e0: 6974 655f 696d 6167 5f73 656c 665f 656e  ite_imag_self_en
-0000e4f0: 6572 6779 2873 656c 662c 206f 7574 7075  ergy(self, outpu
-0000e500: 745f 6669 6c65 6e61 6d65 3d4e 6f6e 6529  t_filename=None)
-0000e510: 3a0a 2020 2020 2020 2020 7772 6974 655f  :.        write_
-0000e520: 696d 6167 5f73 656c 665f 656e 6572 6779  imag_self_energy
-0000e530: 280a 2020 2020 2020 2020 2020 2020 7365  (.            se
-0000e540: 6c66 2e5f 6761 6d6d 6173 2c0a 2020 2020  lf._gammas,.    
-0000e550: 2020 2020 2020 2020 7365 6c66 2e6d 6573          self.mes
-0000e560: 685f 6e75 6d62 6572 732c 0a20 2020 2020  h_numbers,.     
-0000e570: 2020 2020 2020 2073 656c 662e 5f67 7269         self._gri
-0000e580: 645f 706f 696e 7473 2c0a 2020 2020 2020  d_points,.      
-0000e590: 2020 2020 2020 7365 6c66 2e5f 6261 6e64        self._band
-0000e5a0: 5f69 6e64 6963 6573 2c0a 2020 2020 2020  _indices,.      
-0000e5b0: 2020 2020 2020 7365 6c66 2e5f 6672 6571        self._freq
-0000e5c0: 7565 6e63 795f 706f 696e 7473 2c0a 2020  uency_points,.  
-0000e5d0: 2020 2020 2020 2020 2020 7365 6c66 2e5f            self._
-0000e5e0: 7465 6d70 6572 6174 7572 6573 2c0a 2020  temperatures,.  
-0000e5f0: 2020 2020 2020 2020 2020 7365 6c66 2e5f            self._
-0000e600: 7369 676d 6173 2c0a 2020 2020 2020 2020  sigmas,.        
-0000e610: 2020 2020 7363 6174 7465 7269 6e67 5f65      scattering_e
-0000e620: 7665 6e74 5f63 6c61 7373 3d73 656c 662e  vent_class=self.
-0000e630: 5f73 6361 7474 6572 696e 675f 6576 656e  _scattering_even
-0000e640: 745f 636c 6173 732c 0a20 2020 2020 2020  t_class,.       
-0000e650: 2020 2020 206f 7574 7075 745f 6669 6c65       output_file
-0000e660: 6e61 6d65 3d6f 7574 7075 745f 6669 6c65  name=output_file
-0000e670: 6e61 6d65 2c0a 2020 2020 2020 2020 2020  name,.          
-0000e680: 2020 6973 5f6d 6573 685f 7379 6d6d 6574    is_mesh_symmet
-0000e690: 7279 3d73 656c 662e 5f69 735f 6d65 7368  ry=self._is_mesh
-0000e6a0: 5f73 796d 6d65 7472 792c 0a20 2020 2020  _symmetry,.     
-0000e6b0: 2020 2020 2020 206c 6f67 5f6c 6576 656c         log_level
-0000e6c0: 3d73 656c 662e 5f6c 6f67 5f6c 6576 656c  =self._log_level
-0000e6d0: 2c0a 2020 2020 2020 2020 290a 0a20 2020  ,.        )..   
-0000e6e0: 2064 6566 2072 756e 5f72 6561 6c5f 7365   def run_real_se
-0000e6f0: 6c66 5f65 6e65 7267 7928 0a20 2020 2020  lf_energy(.     
-0000e700: 2020 2073 656c 662c 0a20 2020 2020 2020     self,.       
-0000e710: 2067 7269 645f 706f 696e 7473 2c0a 2020   grid_points,.  
-0000e720: 2020 2020 2020 7465 6d70 6572 6174 7572        temperatur
-0000e730: 6573 2c0a 2020 2020 2020 2020 6672 6571  es,.        freq
-0000e740: 7565 6e63 795f 706f 696e 7473 5f61 745f  uency_points_at_
-0000e750: 6261 6e64 733d 4661 6c73 652c 0a20 2020  bands=False,.   
-0000e760: 2020 2020 2066 7265 7175 656e 6379 5f70       frequency_p
-0000e770: 6f69 6e74 733d 4e6f 6e65 2c0a 2020 2020  oints=None,.    
-0000e780: 2020 2020 6672 6571 7565 6e63 795f 7374      frequency_st
-0000e790: 6570 3d4e 6f6e 652c 0a20 2020 2020 2020  ep=None,.       
-0000e7a0: 206e 756d 5f66 7265 7175 656e 6379 5f70   num_frequency_p
-0000e7b0: 6f69 6e74 733d 4e6f 6e65 2c0a 2020 2020  oints=None,.    
-0000e7c0: 2020 2020 6570 7369 6c6f 6e73 3d4e 6f6e      epsilons=Non
-0000e7d0: 652c 0a20 2020 2020 2020 2077 7269 7465  e,.        write
-0000e7e0: 5f74 7874 3d46 616c 7365 2c0a 2020 2020  _txt=False,.    
-0000e7f0: 2020 2020 7772 6974 655f 6864 6635 3d46      write_hdf5=F
-0000e800: 616c 7365 2c0a 2020 2020 2020 2020 6f75  alse,.        ou
-0000e810: 7470 7574 5f66 696c 656e 616d 653d 4e6f  tput_filename=No
-0000e820: 6e65 2c0a 2020 2020 293a 0a20 2020 2020  ne,.    ):.     
-0000e830: 2020 2022 2222 4361 6c63 756c 6174 6520     """Calculate 
-0000e840: 7265 616c 2d70 6172 7420 6f66 2073 656c  real-part of sel
-0000e850: 662d 656e 6572 6779 206f 6620 6275 6262  f-energy of bubb
-0000e860: 6c65 2064 6961 6772 616d 2028 4465 6c74  le diagram (Delt
-0000e870: 6129 2e0a 0a20 2020 2020 2020 2050 6920  a)...        Pi 
-0000e880: 3d20 4465 6c74 6120 2d20 6920 4761 6d6d  = Delta - i Gamm
-0000e890: 612e 0a0a 2020 2020 2020 2020 5061 7261  a...        Para
-0000e8a0: 6d65 7465 7273 0a20 2020 2020 2020 202d  meters.        -
-0000e8b0: 2d2d 2d2d 2d2d 2d2d 2d0a 2020 2020 2020  ---------.      
-0000e8c0: 2020 6772 6964 5f70 6f69 6e74 7320 3a20    grid_points : 
-0000e8d0: 6172 7261 795f 6c69 6b65 0a20 2020 2020  array_like.     
-0000e8e0: 2020 2020 2020 2047 7269 642d 706f 696e         Grid-poin
-0000e8f0: 7420 696e 6469 6365 7320 7768 6572 6520  t indices where 
-0000e900: 7265 616c 2070 6172 7420 6f66 2073 656c  real part of sel
-0000e910: 662d 656e 6572 6769 6573 2061 7265 0a20  f-energies are. 
-0000e920: 2020 2020 2020 2020 2020 2063 6163 6c63             caclc
-0000e930: 756c 6174 6564 2e0a 2020 2020 2020 2020  ulated..        
-0000e940: 2020 2020 6474 7970 653d 696e 742c 2073      dtype=int, s
-0000e950: 6861 7065 3d28 6772 6964 5f70 6f69 6e74  hape=(grid_point
-0000e960: 732c 290a 2020 2020 2020 2020 7465 6d70  s,).        temp
-0000e970: 6572 6174 7572 6573 203a 2061 7272 6179  eratures : array
-0000e980: 5f6c 696b 650a 2020 2020 2020 2020 2020  _like.          
-0000e990: 2020 5465 6d70 6572 6174 7572 6573 2077    Temperatures w
-0000e9a0: 6865 7265 2072 6561 6c20 7061 7274 206f  here real part o
-0000e9b0: 6620 7365 6c66 2d65 6e65 7267 6965 7320  f self-energies 
-0000e9c0: 2061 7265 2063 616c 6375 6c61 7465 642e   are calculated.
-0000e9d0: 0a20 2020 2020 2020 2020 2020 2064 7479  .            dty
-0000e9e0: 7065 3d66 6c6f 6174 2c20 7368 6170 653d  pe=float, shape=
-0000e9f0: 2874 656d 7065 7261 7475 7265 732c 290a  (temperatures,).
-0000ea00: 2020 2020 2020 2020 6672 6571 7565 6e63          frequenc
-0000ea10: 795f 706f 696e 7473 5f61 745f 6261 6e64  y_points_at_band
-0000ea20: 7320 3a20 626f 6f6c 2c20 6f70 7469 6f6e  s : bool, option
-0000ea30: 616c 0a20 2020 2020 2020 2020 2020 2057  al.            W
-0000ea40: 6974 6820 4661 6c73 652c 2066 7265 7175  ith False, frequ
-0000ea50: 656e 6379 2073 6869 6674 7320 6172 6520  ency shifts are 
-0000ea60: 6361 6c63 756c 6174 6564 2061 7420 6672  calculated at fr
-0000ea70: 7175 656e 6379 2073 616d 706c 696e 670a  quency sampling.
-0000ea80: 2020 2020 2020 2020 2020 2020 706f 696e              poin
-0000ea90: 7473 2e20 5768 656e 2054 7275 652c 2074  ts. When True, t
-0000eaa0: 6865 7920 6172 6520 646f 6e65 2061 7420  hey are done at 
-0000eab0: 7468 6520 7068 6f6e 6f6e 2066 7265 7175  the phonon frequ
-0000eac0: 656e 6369 6573 2e0a 2020 2020 2020 2020  encies..        
-0000ead0: 2020 2020 4465 6661 756c 7420 6973 2046      Default is F
-0000eae0: 616c 7365 2e0a 2020 2020 2020 2020 6672  alse..        fr
-0000eaf0: 6571 7565 6e63 795f 706f 696e 7473 203a  equency_points :
-0000eb00: 2061 7272 6179 5f6c 696b 652c 206f 7074   array_like, opt
-0000eb10: 696f 6e61 6c0a 2020 2020 2020 2020 2020  ional.          
-0000eb20: 2020 4672 6571 7565 6e63 7920 7361 6d70    Frequency samp
-0000eb30: 6c69 6e67 2070 6f69 6e74 732e 2044 6566  ling points. Def
-0000eb40: 6175 6c74 2069 7320 4e6f 6e65 2e20 496e  ault is None. In
-0000eb50: 2074 6869 7320 6361 7365 2c0a 2020 2020   this case,.    
-0000eb60: 2020 2020 2020 2020 6e75 6d5f 6672 6571          num_freq
-0000eb70: 7565 6e63 795f 706f 696e 7473 206f 7220  uency_points or 
-0000eb80: 6672 6571 7565 6e63 795f 7374 6570 2069  frequency_step i
-0000eb90: 7320 7573 6564 2074 6f20 6765 6e65 7261  s used to genera
-0000eba0: 7465 2075 6e69 666f 726d 0a20 2020 2020  te uniform.     
-0000ebb0: 2020 2020 2020 2066 7265 7175 656e 6379         frequency
-0000ebc0: 2073 616d 706c 696e 6720 706f 696e 7473   sampling points
-0000ebd0: 2e0a 2020 2020 2020 2020 2020 2020 6474  ..            dt
-0000ebe0: 7970 653d 666c 6f61 742c 2073 6861 7065  ype=float, shape
-0000ebf0: 3d28 6672 6571 7565 6e63 795f 706f 696e  =(frequency_poin
-0000ec00: 7473 2c29 0a20 2020 2020 2020 2066 7265  ts,).        fre
-0000ec10: 7175 656e 6379 5f73 7465 7020 3a20 666c  quency_step : fl
-0000ec20: 6f61 742c 206f 7074 696f 6e61 6c0a 2020  oat, optional.  
-0000ec30: 2020 2020 2020 2020 2020 556e 6966 6f72            Unifor
-0000ec40: 6d20 7069 7463 6820 6f66 2066 7265 7175  m pitch of frequ
-0000ec50: 656e 6379 2073 616d 706c 696e 6720 706f  ency sampling po
-0000ec60: 696e 7473 2e20 4465 6661 756c 7420 6973  ints. Default is
-0000ec70: 204e 6f6e 652e 2054 6869 730a 2020 2020   None. This.    
-0000ec80: 2020 2020 2020 2020 7265 7375 6c74 7320          results 
-0000ec90: 696e 2075 7369 6e67 206e 756d 5f66 7265  in using num_fre
-0000eca0: 7175 656e 6379 5f70 6f69 6e74 732e 0a20  quency_points.. 
-0000ecb0: 2020 2020 2020 206e 756d 5f66 7265 7175         num_frequ
-0000ecc0: 656e 6379 5f70 6f69 6e74 733a 2049 6e74  ency_points: Int
-0000ecd0: 2c20 6f70 7469 6f6e 616c 0a20 2020 2020  , optional.     
-0000ece0: 2020 2020 2020 204e 756d 6265 7220 6f66         Number of
-0000ecf0: 2073 616d 706c 696e 6720 7361 6d70 6c69   sampling sampli
-0000ed00: 6e67 2070 6f69 6e74 7320 746f 2062 6520  ng points to be 
-0000ed10: 7573 6564 2069 6e73 7465 6164 206f 660a  used instead of.
-0000ed20: 2020 2020 2020 2020 2020 2020 6672 6571              freq
-0000ed30: 7565 6e63 795f 7374 6570 2e20 5468 6973  uency_step. This
-0000ed40: 206e 756d 6265 7220 696e 636c 7564 6573   number includes
-0000ed50: 2065 6e64 2070 6f69 6e74 732e 2044 6566   end points. Def
-0000ed60: 6175 6c74 2069 7320 4e6f 6e65 2c0a 2020  ault is None,.  
-0000ed70: 2020 2020 2020 2020 2020 7768 6963 6820            which 
-0000ed80: 6769 7665 7320 3230 312e 0a20 2020 2020  gives 201..     
-0000ed90: 2020 2065 7073 696c 6f6e 7320 3a20 6172     epsilons : ar
-0000eda0: 7261 795f 6c69 6b65 0a20 2020 2020 2020  ray_like.       
-0000edb0: 2020 2020 2053 6d65 6172 696e 6720 7769       Smearing wi
-0000edc0: 6474 6873 2074 6f20 636f 6d70 7574 6572  dths to computer
-0000edd0: 2070 7269 6e63 6970 616c 2070 6172 742e   principal part.
-0000ede0: 2057 6865 6e20 6d75 6c74 6970 6c65 2076   When multiple v
-0000edf0: 616c 7565 730a 2020 2020 2020 2020 2020  alues.          
-0000ee00: 2020 6172 6520 6769 7665 6e20 6672 6571    are given freq
-0000ee10: 7565 6e63 7920 7368 6966 7473 2066 6f72  uency shifts for
-0000ee20: 2074 686f 7365 2076 616c 7565 7320 6172   those values ar
-0000ee30: 6520 7265 7475 726e 6564 2e0a 2020 2020  e returned..    
-0000ee40: 2020 2020 2020 2020 6474 7970 653d 666c          dtype=fl
-0000ee50: 6f61 742c 2073 6861 7065 3d28 6570 7369  oat, shape=(epsi
-0000ee60: 6c6f 6e73 2c29 0a20 2020 2020 2020 2077  lons,).        w
-0000ee70: 7269 7465 5f74 7874 203a 2062 6f6f 6c2c  rite_txt : bool,
-0000ee80: 206f 7074 696f 6e61 6c0a 2020 2020 2020   optional.      
-0000ee90: 2020 2020 2020 4672 6571 7565 6e63 7920        Frequency 
-0000eea0: 706f 696e 7473 2061 6e64 2072 6561 6c20  points and real 
-0000eeb0: 7061 7274 206f 6620 7365 6c66 2d65 6e65  part of self-ene
-0000eec0: 7267 6965 7320 6172 6520 7772 6974 7465  rgies are writte
-0000eed0: 6e0a 2020 2020 2020 2020 2020 2020 696e  n.            in
-0000eee0: 746f 2074 6578 7420 6669 6c65 732e 0a20  to text files.. 
-0000eef0: 2020 2020 2020 2077 7269 7465 5f68 6466         write_hdf
-0000ef00: 3520 3a20 626f 6f6c 0a20 2020 2020 2020  5 : bool.       
-0000ef10: 2020 2020 2052 6573 756c 7473 2061 7265       Results are
-0000ef20: 2073 746f 7265 6420 696e 2068 6466 3520   stored in hdf5 
-0000ef30: 6669 6c65 7320 696e 6465 7065 6e64 656e  files independen
-0000ef40: 746c 7920 6174 2067 7269 6420 706f 696e  tly at grid poin
-0000ef50: 7473 2c0a 2020 2020 2020 2020 2020 2020  ts,.            
-0000ef60: 6570 7369 6c6f 6e73 2c20 616e 6420 7465  epsilons, and te
-0000ef70: 6d70 6572 6174 7572 6573 2e0a 2020 2020  mperatures..    
-0000ef80: 2020 2020 6f75 7470 7574 5f66 696c 656e      output_filen
-0000ef90: 616d 6520 3a20 7374 720a 2020 2020 2020  ame : str.      
-0000efa0: 2020 2020 2020 5468 6973 2073 7472 696e        This strin
-0000efb0: 6720 6973 2069 6e73 6572 7465 6420 696e  g is inserted in
-0000efc0: 2074 6865 206f 7574 7075 7420 6669 6c65   the output file
-0000efd0: 206e 616d 6573 2e0a 0a20 2020 2020 2020   names...       
-0000efe0: 2022 2222 0a20 2020 2020 2020 2069 6620   """.        if 
-0000eff0: 7365 6c66 2e5f 696e 7465 7261 6374 696f  self._interactio
-0000f000: 6e20 6973 204e 6f6e 653a 0a20 2020 2020  n is None:.     
-0000f010: 2020 2020 2020 206d 7367 203d 2028 0a20         msg = (. 
-0000f020: 2020 2020 2020 2020 2020 2020 2020 2022                 "
-0000f030: 5068 6f6e 6f33 7079 2e69 6e69 745f 7068  Phono3py.init_ph
-0000f040: 7068 5f69 6e74 6572 6163 7469 6f6e 2068  ph_interaction h
-0000f050: 6173 2074 6f20 6265 2063 616c 6c65 6420  as to be called 
-0000f060: 220a 2020 2020 2020 2020 2020 2020 2020  ".              
-0000f070: 2020 2262 6566 6f72 6520 7275 6e6e 696e    "before runnin
-0000f080: 6720 7468 6973 206d 6574 686f 642e 220a  g this method.".
-0000f090: 2020 2020 2020 2020 2020 2020 290a 2020              ).  
-0000f0a0: 2020 2020 2020 2020 2020 7261 6973 6520            raise 
-0000f0b0: 5275 6e74 696d 6545 7272 6f72 286d 7367  RuntimeError(msg
-0000f0c0: 290a 0a20 2020 2020 2020 2069 6620 6570  )..        if ep
-0000f0d0: 7369 6c6f 6e73 2069 7320 6e6f 7420 4e6f  silons is not No
-0000f0e0: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
-0000f0f0: 5f65 7073 696c 6f6e 7320 3d20 6570 7369  _epsilons = epsi
-0000f100: 6c6f 6e73 0a20 2020 2020 2020 2065 6c73  lons.        els
-0000f110: 653a 0a20 2020 2020 2020 2020 2020 2069  e:.            i
-0000f120: 6620 6c65 6e28 7365 6c66 2e5f 7369 676d  f len(self._sigm
-0000f130: 6173 2920 3d3d 2031 2061 6e64 2073 656c  as) == 1 and sel
-0000f140: 662e 5f73 6967 6d61 735b 305d 2069 7320  f._sigmas[0] is 
-0000f150: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
-0000f160: 2020 2020 2020 5f65 7073 696c 6f6e 7320        _epsilons 
-0000f170: 3d20 4e6f 6e65 0a20 2020 2020 2020 2020  = None.         
-0000f180: 2020 2065 6c69 6620 7365 6c66 2e5f 7369     elif self._si
-0000f190: 676d 6173 5b30 5d20 6973 204e 6f6e 653a  gmas[0] is None:
-0000f1a0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000f1b0: 205f 6570 7369 6c6f 6e73 203d 2073 656c   _epsilons = sel
-0000f1c0: 662e 5f73 6967 6d61 735b 313a 5d0a 2020  f._sigmas[1:].  
-0000f1d0: 2020 2020 2020 2020 2020 656c 7365 3a0a            else:.
-0000f1e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000f1f0: 5f65 7073 696c 6f6e 7320 3d20 7365 6c66  _epsilons = self
-0000f200: 2e5f 7369 676d 6173 0a0a 2020 2020 2020  ._sigmas..      
-0000f210: 2020 2320 2865 7073 696c 6f6e 2c20 6772    # (epsilon, gr
-0000f220: 6964 5f70 6f69 6e74 2c20 7465 6d70 6572  id_point, temper
-0000f230: 6174 7572 652c 2062 616e 6429 0a20 2020  ature, band).   
-0000f240: 2020 2020 2066 7265 7175 656e 6379 5f70       frequency_p
-0000f250: 6f69 6e74 732c 2064 656c 7461 7320 3d20  oints, deltas = 
-0000f260: 6765 745f 7265 616c 5f73 656c 665f 656e  get_real_self_en
-0000f270: 6572 6779 280a 2020 2020 2020 2020 2020  ergy(.          
-0000f280: 2020 7365 6c66 2e5f 696e 7465 7261 6374    self._interact
-0000f290: 696f 6e2c 0a20 2020 2020 2020 2020 2020  ion,.           
-0000f2a0: 2067 7269 645f 706f 696e 7473 2c0a 2020   grid_points,.  
-0000f2b0: 2020 2020 2020 2020 2020 7465 6d70 6572            temper
-0000f2c0: 6174 7572 6573 2c0a 2020 2020 2020 2020  atures,.        
-0000f2d0: 2020 2020 6570 7369 6c6f 6e73 3d5f 6570      epsilons=_ep
-0000f2e0: 7369 6c6f 6e73 2c0a 2020 2020 2020 2020  silons,.        
-0000f2f0: 2020 2020 6672 6571 7565 6e63 795f 706f      frequency_po
-0000f300: 696e 7473 3d66 7265 7175 656e 6379 5f70  ints=frequency_p
-0000f310: 6f69 6e74 732c 0a20 2020 2020 2020 2020  oints,.         
-0000f320: 2020 2066 7265 7175 656e 6379 5f73 7465     frequency_ste
-0000f330: 703d 6672 6571 7565 6e63 795f 7374 6570  p=frequency_step
-0000f340: 2c0a 2020 2020 2020 2020 2020 2020 6e75  ,.            nu
-0000f350: 6d5f 6672 6571 7565 6e63 795f 706f 696e  m_frequency_poin
-0000f360: 7473 3d6e 756d 5f66 7265 7175 656e 6379  ts=num_frequency
-0000f370: 5f70 6f69 6e74 732c 0a20 2020 2020 2020  _points,.       
-0000f380: 2020 2020 2066 7265 7175 656e 6379 5f70       frequency_p
-0000f390: 6f69 6e74 735f 6174 5f62 616e 6473 3d66  oints_at_bands=f
-0000f3a0: 7265 7175 656e 6379 5f70 6f69 6e74 735f  requency_points_
-0000f3b0: 6174 5f62 616e 6473 2c0a 2020 2020 2020  at_bands,.      
-0000f3c0: 2020 2020 2020 7772 6974 655f 6864 6635        write_hdf5
-0000f3d0: 3d77 7269 7465 5f68 6466 352c 0a20 2020  =write_hdf5,.   
-0000f3e0: 2020 2020 2020 2020 206f 7574 7075 745f           output_
-0000f3f0: 6669 6c65 6e61 6d65 3d6f 7574 7075 745f  filename=output_
-0000f400: 6669 6c65 6e61 6d65 2c0a 2020 2020 2020  filename,.      
-0000f410: 2020 2020 2020 6c6f 675f 6c65 7665 6c3d        log_level=
-0000f420: 7365 6c66 2e5f 6c6f 675f 6c65 7665 6c2c  self._log_level,
-0000f430: 0a20 2020 2020 2020 2029 0a0a 2020 2020  .        )..    
-0000f440: 2020 2020 6966 2077 7269 7465 5f74 7874      if write_txt
-0000f450: 3a0a 2020 2020 2020 2020 2020 2020 7772  :.            wr
-0000f460: 6974 655f 7265 616c 5f73 656c 665f 656e  ite_real_self_en
-0000f470: 6572 6779 280a 2020 2020 2020 2020 2020  ergy(.          
-0000f480: 2020 2020 2020 6465 6c74 6173 2c0a 2020        deltas,.  
-0000f490: 2020 2020 2020 2020 2020 2020 2020 7365                se
-0000f4a0: 6c66 2e6d 6573 685f 6e75 6d62 6572 732c  lf.mesh_numbers,
-0000f4b0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000f4c0: 2067 7269 645f 706f 696e 7473 2c0a 2020   grid_points,.  
-0000f4d0: 2020 2020 2020 2020 2020 2020 2020 7365                se
-0000f4e0: 6c66 2e5f 6261 6e64 5f69 6e64 6963 6573  lf._band_indices
-0000f4f0: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-0000f500: 2020 6672 6571 7565 6e63 795f 706f 696e    frequency_poin
-0000f510: 7473 2c0a 2020 2020 2020 2020 2020 2020  ts,.            
-0000f520: 2020 2020 7465 6d70 6572 6174 7572 6573      temperatures
-0000f530: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-0000f540: 2020 5f65 7073 696c 6f6e 732c 0a20 2020    _epsilons,.   
-0000f550: 2020 2020 2020 2020 2020 2020 206f 7574               out
-0000f560: 7075 745f 6669 6c65 6e61 6d65 3d6f 7574  put_filename=out
-0000f570: 7075 745f 6669 6c65 6e61 6d65 2c0a 2020  put_filename,.  
-0000f580: 2020 2020 2020 2020 2020 2020 2020 6973                is
-0000f590: 5f6d 6573 685f 7379 6d6d 6574 7279 3d73  _mesh_symmetry=s
-0000f5a0: 656c 662e 5f69 735f 6d65 7368 5f73 796d  elf._is_mesh_sym
-0000f5b0: 6d65 7472 792c 0a20 2020 2020 2020 2020  metry,.         
-0000f5c0: 2020 2020 2020 206c 6f67 5f6c 6576 656c         log_level
-0000f5d0: 3d73 656c 662e 5f6c 6f67 5f6c 6576 656c  =self._log_level
-0000f5e0: 2c0a 2020 2020 2020 2020 2020 2020 290a  ,.            ).
-0000f5f0: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
-0000f600: 6672 6571 7565 6e63 795f 706f 696e 7473  frequency_points
-0000f610: 2c20 6465 6c74 6173 0a0a 2020 2020 6465  , deltas..    de
-0000f620: 6620 7275 6e5f 7370 6563 7472 616c 5f66  f run_spectral_f
-0000f630: 756e 6374 696f 6e28 0a20 2020 2020 2020  unction(.       
-0000f640: 2073 656c 662c 0a20 2020 2020 2020 2067   self,.        g
-0000f650: 7269 645f 706f 696e 7473 2c0a 2020 2020  rid_points,.    
-0000f660: 2020 2020 7465 6d70 6572 6174 7572 6573      temperatures
-0000f670: 2c0a 2020 2020 2020 2020 6672 6571 7565  ,.        freque
-0000f680: 6e63 795f 706f 696e 7473 3d4e 6f6e 652c  ncy_points=None,
-0000f690: 0a20 2020 2020 2020 2066 7265 7175 656e  .        frequen
-0000f6a0: 6379 5f73 7465 703d 4e6f 6e65 2c0a 2020  cy_step=None,.  
-0000f6b0: 2020 2020 2020 6e75 6d5f 6672 6571 7565        num_freque
-0000f6c0: 6e63 795f 706f 696e 7473 3d4e 6f6e 652c  ncy_points=None,
-0000f6d0: 0a20 2020 2020 2020 206e 756d 5f70 6f69  .        num_poi
-0000f6e0: 6e74 735f 696e 5f62 6174 6368 3d4e 6f6e  nts_in_batch=Non
-0000f6f0: 652c 0a20 2020 2020 2020 2077 7269 7465  e,.        write
-0000f700: 5f74 7874 3d46 616c 7365 2c0a 2020 2020  _txt=False,.    
-0000f710: 2020 2020 7772 6974 655f 6864 6635 3d46      write_hdf5=F
-0000f720: 616c 7365 2c0a 2020 2020 2020 2020 6f75  alse,.        ou
-0000f730: 7470 7574 5f66 696c 656e 616d 653d 4e6f  tput_filename=No
-0000f740: 6e65 2c0a 2020 2020 293a 0a20 2020 2020  ne,.    ):.     
-0000f750: 2020 2022 2222 4672 6571 7565 6e63 7920     """Frequency 
-0000f760: 7368 6966 7420 6672 6f6d 206c 6f77 6573  shift from lowes
-0000f770: 7420 6f72 6465 7220 6469 6167 7261 6d20  t order diagram 
-0000f780: 6973 2063 616c 6375 6c61 7465 642e 0a0a  is calculated...
-0000f790: 2020 2020 2020 2020 5061 7261 6d65 7465          Paramete
-0000f7a0: 7273 0a20 2020 2020 2020 202d 2d2d 2d2d  rs.        -----
-0000f7b0: 2d2d 2d2d 2d0a 2020 2020 2020 2020 6772  -----.        gr
-0000f7c0: 6964 5f70 6f69 6e74 7320 3a20 6172 7261  id_points : arra
-0000f7d0: 795f 6c69 6b65 0a20 2020 2020 2020 2020  y_like.         
-0000f7e0: 2020 2047 7269 642d 706f 696e 7420 696e     Grid-point in
-0000f7f0: 6469 6365 7320 7768 6572 6520 696d 6167  dices where imag
-0000f800: 2d73 656c 662d 656e 6572 6765 6973 2061  -self-energeis a
-0000f810: 7265 2063 6163 6c63 756c 6174 6564 2e0a  re caclculated..
-0000f820: 2020 2020 2020 2020 2020 2020 6474 7970              dtyp
-0000f830: 653d 696e 742c 2073 6861 7065 3d28 6772  e=int, shape=(gr
-0000f840: 6964 5f70 6f69 6e74 732c 290a 2020 2020  id_points,).    
-0000f850: 2020 2020 7465 6d70 6572 6174 7572 6573      temperatures
-0000f860: 203a 2061 7272 6179 5f6c 696b 650a 2020   : array_like.  
-0000f870: 2020 2020 2020 2020 2020 5465 6d70 6572            Temper
-0000f880: 6174 7572 6573 2077 6865 7265 2069 6d61  atures where ima
-0000f890: 672d 7365 6c66 2d65 6e65 7267 6965 7320  g-self-energies 
-0000f8a0: 6172 6520 6361 6c63 756c 6174 6564 2e0a  are calculated..
-0000f8b0: 2020 2020 2020 2020 2020 2020 6474 7970              dtyp
-0000f8c0: 653d 666c 6f61 742c 2073 6861 7065 3d28  e=float, shape=(
-0000f8d0: 7465 6d70 6572 6174 7572 6573 2c29 0a20  temperatures,). 
-0000f8e0: 2020 2020 2020 2066 7265 7175 656e 6379         frequency
-0000f8f0: 5f70 6f69 6e74 7320 3a20 6172 7261 795f  _points : array_
-0000f900: 6c69 6b65 2c20 6f70 7469 6f6e 616c 0a20  like, optional. 
-0000f910: 2020 2020 2020 2020 2020 2046 7265 7175             Frequ
-0000f920: 656e 6379 2073 616d 706c 696e 6720 706f  ency sampling po
-0000f930: 696e 7473 2e20 4465 6661 756c 7420 6973  ints. Default is
-0000f940: 204e 6f6e 652e 2049 6e20 7468 6973 2063   None. In this c
-0000f950: 6173 652c 0a20 2020 2020 2020 2020 2020  ase,.           
-0000f960: 206e 756d 5f66 7265 7175 656e 6379 5f70   num_frequency_p
-0000f970: 6f69 6e74 7320 6f72 2066 7265 7175 656e  oints or frequen
-0000f980: 6379 5f73 7465 7020 6973 2075 7365 6420  cy_step is used 
-0000f990: 746f 2067 656e 6572 6174 6520 756e 6966  to generate unif
-0000f9a0: 6f72 6d0a 2020 2020 2020 2020 2020 2020  orm.            
-0000f9b0: 6672 6571 7565 6e63 7920 7361 6d70 6c69  frequency sampli
-0000f9c0: 6e67 2070 6f69 6e74 732e 0a20 2020 2020  ng points..     
-0000f9d0: 2020 2020 2020 2064 7479 7065 3d66 6c6f         dtype=flo
-0000f9e0: 6174 2c20 7368 6170 653d 2866 7265 7175  at, shape=(frequ
-0000f9f0: 656e 6379 5f70 6f69 6e74 732c 290a 2020  ency_points,).  
-0000fa00: 2020 2020 2020 6672 6571 7565 6e63 795f        frequency_
-0000fa10: 7374 6570 203a 2066 6c6f 6174 2c20 6f70  step : float, op
-0000fa20: 7469 6f6e 616c 0a20 2020 2020 2020 2020  tional.         
-0000fa30: 2020 2055 6e69 666f 726d 2070 6974 6368     Uniform pitch
-0000fa40: 206f 6620 6672 6571 7565 6e63 7920 7361   of frequency sa
-0000fa50: 6d70 6c69 6e67 2070 6f69 6e74 732e 2044  mpling points. D
-0000fa60: 6566 6175 6c74 2069 7320 4e6f 6e65 2e20  efault is None. 
-0000fa70: 5468 6973 0a20 2020 2020 2020 2020 2020  This.           
-0000fa80: 2072 6573 756c 7473 2069 6e20 7573 696e   results in usin
-0000fa90: 6720 6e75 6d5f 6672 6571 7565 6e63 795f  g num_frequency_
-0000faa0: 706f 696e 7473 2e0a 2020 2020 2020 2020  points..        
-0000fab0: 6e75 6d5f 6672 6571 7565 6e63 795f 706f  num_frequency_po
-0000fac0: 696e 7473 3a20 496e 742c 206f 7074 696f  ints: Int, optio
-0000fad0: 6e61 6c0a 2020 2020 2020 2020 2020 2020  nal.            
-0000fae0: 4e75 6d62 6572 206f 6620 7361 6d70 6c69  Number of sampli
-0000faf0: 6e67 2073 616d 706c 696e 6720 706f 696e  ng sampling poin
-0000fb00: 7473 2074 6f20 6265 2075 7365 6420 696e  ts to be used in
-0000fb10: 7374 6561 6420 6f66 0a20 2020 2020 2020  stead of.       
-0000fb20: 2020 2020 2066 7265 7175 656e 6379 5f73       frequency_s
-0000fb30: 7465 702e 2054 6869 7320 6e75 6d62 6572  tep. This number
-0000fb40: 2069 6e63 6c75 6465 7320 656e 6420 706f   includes end po
-0000fb50: 696e 7473 2e20 4465 6661 756c 7420 6973  ints. Default is
-0000fb60: 204e 6f6e 652c 0a20 2020 2020 2020 2020   None,.         
-0000fb70: 2020 2077 6869 6368 2067 6976 6573 2032     which gives 2
-0000fb80: 3031 2e0a 2020 2020 2020 2020 6e75 6d5f  01..        num_
-0000fb90: 706f 696e 7473 5f69 6e5f 6261 7463 683a  points_in_batch:
-0000fba0: 2069 6e74 2c20 6f70 7469 6f6e 616c 0a20   int, optional. 
-0000fbb0: 2020 2020 2020 2020 2020 204e 756d 6265             Numbe
-0000fbc0: 7220 6f66 2073 616d 706c 696e 6720 706f  r of sampling po
-0000fbd0: 696e 7473 2069 6e20 6f6e 6520 6261 7463  ints in one batc
-0000fbe0: 682e 2054 6869 7320 6973 2066 6f72 2074  h. This is for t
-0000fbf0: 6865 2066 7265 7175 656e 6379 0a20 2020  he frequency.   
-0000fc00: 2020 2020 2020 2020 2073 616d 706c 696e           samplin
-0000fc10: 6720 6d6f 6465 2061 6e64 2074 6865 2073  g mode and the s
-0000fc20: 616d 706c 696e 6720 706f 696e 7473 2061  ampling points a
-0000fc30: 7265 2064 6976 6964 6564 2069 6e74 6f20  re divided into 
-0000fc40: 6261 7463 6865 732e 0a20 2020 2020 2020  batches..       
-0000fc50: 2020 2020 204c 6167 6572 206e 756d 6265       Lager numbe
-0000fc60: 7220 7072 6f76 6964 6573 2065 6666 6963  r provides effic
-0000fc70: 6965 6e74 2075 7365 206f 6620 6d75 6c74  ient use of mult
-0000fc80: 692d 636f 7265 7320 6275 7420 6d6f 7265  i-cores but more
-0000fc90: 0a20 2020 2020 2020 2020 2020 206d 656d  .            mem
-0000fca0: 6f72 7920 6465 6d61 6e64 696e 672e 2044  ory demanding. D
-0000fcb0: 6566 6175 6c74 2069 7320 4e6f 6e65 2c20  efault is None, 
-0000fcc0: 7768 6963 6820 6769 7665 2074 6865 206e  which give the n
-0000fcd0: 756d 6265 7220 6f66 2031 302e 0a20 2020  umber of 10..   
-0000fce0: 2020 2020 2077 7269 7465 5f74 7874 203a       write_txt :
-0000fcf0: 2062 6f6f 6c2c 206f 7074 696f 6e61 6c0a   bool, optional.
-0000fd00: 2020 2020 2020 2020 2020 2020 4672 6571              Freq
-0000fd10: 7565 6e63 7920 706f 696e 7473 2061 6e64  uency points and
-0000fd20: 2073 7065 6374 7261 6c20 6675 6e63 7469   spectral functi
-0000fd30: 6f6e 7320 6172 6520 7772 6974 7465 6e0a  ons are written.
-0000fd40: 2020 2020 2020 2020 2020 2020 696e 746f              into
-0000fd50: 2074 6578 7420 6669 6c65 732e 2044 6566   text files. Def
-0000fd60: 6175 6c74 2069 7320 4661 6c73 652e 0a20  ault is False.. 
-0000fd70: 2020 2020 2020 2077 7269 7465 5f68 6466         write_hdf
-0000fd80: 3520 3a20 626f 6f6c 0a20 2020 2020 2020  5 : bool.       
-0000fd90: 2020 2020 2052 6573 756c 7473 2061 7265       Results are
-0000fda0: 2073 746f 7265 6420 696e 2068 6466 3520   stored in hdf5 
-0000fdb0: 6669 6c65 7320 696e 6465 7065 6e64 656e  files independen
-0000fdc0: 746c 7920 6174 2067 7269 6420 706f 696e  tly at grid poin
-0000fdd0: 7473 2c0a 2020 2020 2020 2020 2020 2020  ts,.            
-0000fde0: 6570 7369 6c6f 6e73 2e20 4465 6661 756c  epsilons. Defaul
-0000fdf0: 7420 6973 2046 616c 7365 2e0a 2020 2020  t is False..    
-0000fe00: 2020 2020 6f75 7470 7574 5f66 696c 656e      output_filen
-0000fe10: 616d 6520 3a20 7374 720a 2020 2020 2020  ame : str.      
-0000fe20: 2020 2020 2020 5468 6973 2073 7472 696e        This strin
-0000fe30: 6720 6973 2069 6e73 6572 7465 6420 696e  g is inserted in
-0000fe40: 2074 6865 206f 7574 7075 7420 6669 6c65   the output file
-0000fe50: 206e 616d 6573 2e0a 0a20 2020 2020 2020   names...       
-0000fe60: 2022 2222 0a20 2020 2020 2020 2069 6620   """.        if 
-0000fe70: 7365 6c66 2e5f 696e 7465 7261 6374 696f  self._interactio
-0000fe80: 6e20 6973 204e 6f6e 653a 0a20 2020 2020  n is None:.     
-0000fe90: 2020 2020 2020 206d 7367 203d 2028 0a20         msg = (. 
-0000fea0: 2020 2020 2020 2020 2020 2020 2020 2022                 "
-0000feb0: 5068 6f6e 6f33 7079 2e69 6e69 745f 7068  Phono3py.init_ph
-0000fec0: 7068 5f69 6e74 6572 6163 7469 6f6e 2068  ph_interaction h
-0000fed0: 6173 2074 6f20 6265 2063 616c 6c65 6420  as to be called 
-0000fee0: 220a 2020 2020 2020 2020 2020 2020 2020  ".              
-0000fef0: 2020 2262 6566 6f72 6520 7275 6e6e 696e    "before runnin
-0000ff00: 6720 7468 6973 206d 6574 686f 642e 220a  g this method.".
-0000ff10: 2020 2020 2020 2020 2020 2020 290a 2020              ).  
-0000ff20: 2020 2020 2020 2020 2020 7261 6973 6520            raise 
-0000ff30: 5275 6e74 696d 6545 7272 6f72 286d 7367  RuntimeError(msg
-0000ff40: 290a 0a20 2020 2020 2020 2073 656c 662e  )..        self.
-0000ff50: 5f73 7065 6374 7261 6c5f 6675 6e63 7469  _spectral_functi
-0000ff60: 6f6e 203d 2072 756e 5f73 7065 6374 7261  on = run_spectra
-0000ff70: 6c5f 6675 6e63 7469 6f6e 280a 2020 2020  l_function(.    
-0000ff80: 2020 2020 2020 2020 7365 6c66 2e5f 696e          self._in
-0000ff90: 7465 7261 6374 696f 6e2c 0a20 2020 2020  teraction,.     
-0000ffa0: 2020 2020 2020 2067 7269 645f 706f 696e         grid_poin
-0000ffb0: 7473 2c0a 2020 2020 2020 2020 2020 2020  ts,.            
-0000ffc0: 7465 6d70 6572 6174 7572 6573 3d74 656d  temperatures=tem
-0000ffd0: 7065 7261 7475 7265 732c 0a20 2020 2020  peratures,.     
-0000ffe0: 2020 2020 2020 2073 6967 6d61 733d 7365         sigmas=se
-0000fff0: 6c66 2e5f 7369 676d 6173 2c0a 2020 2020  lf._sigmas,.    
-00010000: 2020 2020 2020 2020 6672 6571 7565 6e63          frequenc
-00010010: 795f 706f 696e 7473 3d66 7265 7175 656e  y_points=frequen
-00010020: 6379 5f70 6f69 6e74 732c 0a20 2020 2020  cy_points,.     
-00010030: 2020 2020 2020 2066 7265 7175 656e 6379         frequency
-00010040: 5f73 7465 703d 6672 6571 7565 6e63 795f  _step=frequency_
-00010050: 7374 6570 2c0a 2020 2020 2020 2020 2020  step,.          
-00010060: 2020 6e75 6d5f 6672 6571 7565 6e63 795f    num_frequency_
-00010070: 706f 696e 7473 3d6e 756d 5f66 7265 7175  points=num_frequ
-00010080: 656e 6379 5f70 6f69 6e74 732c 0a20 2020  ency_points,.   
-00010090: 2020 2020 2020 2020 206e 756d 5f70 6f69           num_poi
-000100a0: 6e74 735f 696e 5f62 6174 6368 3d6e 756d  nts_in_batch=num
-000100b0: 5f70 6f69 6e74 735f 696e 5f62 6174 6368  _points_in_batch
-000100c0: 2c0a 2020 2020 2020 2020 2020 2020 6261  ,.            ba
-000100d0: 6e64 5f69 6e64 6963 6573 3d73 656c 662e  nd_indices=self.
-000100e0: 5f62 616e 645f 696e 6469 6365 732c 0a20  _band_indices,. 
-000100f0: 2020 2020 2020 2020 2020 2077 7269 7465             write
-00010100: 5f74 7874 3d77 7269 7465 5f74 7874 2c0a  _txt=write_txt,.
-00010110: 2020 2020 2020 2020 2020 2020 7772 6974              writ
-00010120: 655f 6864 6635 3d77 7269 7465 5f68 6466  e_hdf5=write_hdf
-00010130: 352c 0a20 2020 2020 2020 2020 2020 206f  5,.            o
-00010140: 7574 7075 745f 6669 6c65 6e61 6d65 3d6f  utput_filename=o
-00010150: 7574 7075 745f 6669 6c65 6e61 6d65 2c0a  utput_filename,.
-00010160: 2020 2020 2020 2020 2020 2020 6c6f 675f              log_
-00010170: 6c65 7665 6c3d 7365 6c66 2e5f 6c6f 675f  level=self._log_
-00010180: 6c65 7665 6c2c 0a20 2020 2020 2020 2029  level,.        )
-00010190: 0a0a 2020 2020 6465 6620 7275 6e5f 7468  ..    def run_th
-000101a0: 6572 6d61 6c5f 636f 6e64 7563 7469 7669  ermal_conductivi
-000101b0: 7479 280a 2020 2020 2020 2020 7365 6c66  ty(.        self
-000101c0: 2c0a 2020 2020 2020 2020 6973 5f4c 4254  ,.        is_LBT
-000101d0: 453d 4661 6c73 652c 0a20 2020 2020 2020  E=False,.       
-000101e0: 2074 656d 7065 7261 7475 7265 733d 4e6f   temperatures=No
-000101f0: 6e65 2c0a 2020 2020 2020 2020 6973 5f69  ne,.        is_i
-00010200: 736f 746f 7065 3d46 616c 7365 2c0a 2020  sotope=False,.  
-00010210: 2020 2020 2020 6d61 7373 5f76 6172 6961        mass_varia
-00010220: 6e63 6573 3d4e 6f6e 652c 0a20 2020 2020  nces=None,.     
-00010230: 2020 2067 7269 645f 706f 696e 7473 3d4e     grid_points=N
-00010240: 6f6e 652c 0a20 2020 2020 2020 2062 6f75  one,.        bou
-00010250: 6e64 6172 795f 6d66 703d 4e6f 6e65 2c20  ndary_mfp=None, 
-00010260: 2023 2069 6e20 6d69 6372 6f6d 6574 7265   # in micrometre
-00010270: 0a20 2020 2020 2020 2073 6f6c 7665 5f63  .        solve_c
-00010280: 6f6c 6c65 6374 6976 655f 7068 6f6e 6f6e  ollective_phonon
-00010290: 3d46 616c 7365 2c0a 2020 2020 2020 2020  =False,.        
-000102a0: 7573 655f 6176 655f 7070 3d46 616c 7365  use_ave_pp=False
-000102b0: 2c0a 2020 2020 2020 2020 6973 5f72 6564  ,.        is_red
-000102c0: 7563 6962 6c65 5f63 6f6c 6c69 7369 6f6e  ucible_collision
-000102d0: 5f6d 6174 7269 783d 4661 6c73 652c 0a20  _matrix=False,. 
-000102e0: 2020 2020 2020 2069 735f 6b61 7070 615f         is_kappa_
-000102f0: 7374 6172 3d54 7275 652c 0a20 2020 2020  star=True,.     
-00010300: 2020 2067 765f 6465 6c74 615f 713d 4e6f     gv_delta_q=No
-00010310: 6e65 2c20 2023 2066 6f72 2067 726f 7570  ne,  # for group
-00010320: 2076 656c 6f63 6974 790a 2020 2020 2020   velocity.      
-00010330: 2020 6973 5f66 756c 6c5f 7070 3d46 616c    is_full_pp=Fal
-00010340: 7365 2c0a 2020 2020 2020 2020 7069 6e76  se,.        pinv
-00010350: 5f63 7574 6f66 663d 312e 3065 2d38 2c20  _cutoff=1.0e-8, 
-00010360: 2023 2066 6f72 2070 7365 7564 6f2d 696e   # for pseudo-in
-00010370: 7665 7273 696f 6e20 6f66 2063 6f6c 6c69  version of colli
-00010380: 7369 6f6e 206d 6174 7269 780a 2020 2020  sion matrix.    
-00010390: 2020 2020 7069 6e76 5f6d 6574 686f 643d      pinv_method=
-000103a0: 302c 2020 2320 666f 7220 7073 6575 646f  0,  # for pseudo
-000103b0: 2d69 6e76 6572 7369 6f6e 206f 6620 636f  -inversion of co
-000103c0: 6c6c 6973 696f 6e20 6d61 7472 6978 0a20  llision matrix. 
-000103d0: 2020 2020 2020 2070 696e 765f 736f 6c76         pinv_solv
-000103e0: 6572 3d30 2c20 2023 2073 6f6c 7665 7220  er=0,  # solver 
-000103f0: 6f66 2070 7365 7564 6f2d 696e 7665 7273  of pseudo-invers
-00010400: 696f 6e20 6f66 2063 6f6c 6c69 7369 6f6e  ion of collision
-00010410: 206d 6174 7269 780a 2020 2020 2020 2020   matrix.        
-00010420: 7772 6974 655f 6761 6d6d 613d 4661 6c73  write_gamma=Fals
-00010430: 652c 0a20 2020 2020 2020 2072 6561 645f  e,.        read_
-00010440: 6761 6d6d 613d 4661 6c73 652c 0a20 2020  gamma=False,.   
-00010450: 2020 2020 2069 735f 4e5f 553d 4661 6c73       is_N_U=Fals
-00010460: 652c 0a20 2020 2020 2020 2063 6f6e 6475  e,.        condu
-00010470: 6374 6976 6974 795f 7479 7065 3d4e 6f6e  ctivity_type=Non
-00010480: 652c 0a20 2020 2020 2020 2077 7269 7465  e,.        write
-00010490: 5f6b 6170 7061 3d46 616c 7365 2c0a 2020  _kappa=False,.  
-000104a0: 2020 2020 2020 7772 6974 655f 6761 6d6d        write_gamm
-000104b0: 615f 6465 7461 696c 3d46 616c 7365 2c0a  a_detail=False,.
-000104c0: 2020 2020 2020 2020 7772 6974 655f 636f          write_co
-000104d0: 6c6c 6973 696f 6e3d 4661 6c73 652c 0a20  llision=False,. 
-000104e0: 2020 2020 2020 2072 6561 645f 636f 6c6c         read_coll
-000104f0: 6973 696f 6e3d 4661 6c73 652c 0a20 2020  ision=False,.   
-00010500: 2020 2020 2077 7269 7465 5f70 703d 4661       write_pp=Fa
-00010510: 6c73 652c 0a20 2020 2020 2020 2072 6561  lse,.        rea
-00010520: 645f 7070 3d46 616c 7365 2c0a 2020 2020  d_pp=False,.    
-00010530: 2020 2020 7772 6974 655f 4c42 5445 5f73      write_LBTE_s
-00010540: 6f6c 7574 696f 6e3d 4661 6c73 652c 0a20  olution=False,. 
-00010550: 2020 2020 2020 2063 6f6d 7072 6573 7369         compressi
-00010560: 6f6e 3d22 677a 6970 222c 0a20 2020 2020  on="gzip",.     
-00010570: 2020 2069 6e70 7574 5f66 696c 656e 616d     input_filenam
-00010580: 653d 4e6f 6e65 2c0a 2020 2020 2020 2020  e=None,.        
-00010590: 6f75 7470 7574 5f66 696c 656e 616d 653d  output_filename=
-000105a0: 4e6f 6e65 2c0a 2020 2020 293a 0a20 2020  None,.    ):.   
-000105b0: 2020 2020 2022 2222 5275 6e20 7468 6572       """Run ther
-000105c0: 6d61 6c20 636f 6e64 7563 7469 7669 7479  mal conductivity
-000105d0: 2063 616c 6375 6c61 7469 6f6e 2e0a 0a20   calculation... 
-000105e0: 2020 2020 2020 2050 6172 616d 6574 6572         Parameter
-000105f0: 730a 2020 2020 2020 2020 2d2d 2d2d 2d2d  s.        ------
-00010600: 2d2d 2d2d 0a20 2020 2020 2020 2069 735f  ----.        is_
-00010610: 4c42 5445 203a 2062 6f6f 6c2c 206f 7074  LBTE : bool, opt
-00010620: 696f 6e61 6c2c 2064 6566 6175 6c74 2069  ional, default i
-00010630: 7320 4661 6c73 650a 2020 2020 2020 2020  s False.        
-00010640: 2020 2020 5254 4120 2846 616c 7365 2920      RTA (False) 
-00010650: 6f72 2064 6972 6563 7420 736f 6c75 7469  or direct soluti
-00010660: 6f6e 2028 5472 7565 292e 0a20 2020 2020  on (True)..     
-00010670: 2020 2074 656d 7065 7261 7475 7265 7320     temperatures 
-00010680: 3a20 6172 7261 795f 6c69 6b65 2c20 6f70  : array_like, op
-00010690: 7469 6f6e 616c 2c20 6465 6661 756c 7420  tional, default 
-000106a0: 6973 204e 6f6e 650a 2020 2020 2020 2020  is None.        
-000106b0: 2020 2020 5465 6d70 6572 6174 7572 6573      Temperatures
-000106c0: 2061 7420 7768 6963 6820 7468 6572 6d61   at which therma
-000106d0: 6c20 636f 6e64 7563 7469 7669 7479 2069  l conductivity i
-000106e0: 7320 6361 6c63 756c 6174 6564 2e0a 2020  s calculated..  
-000106f0: 2020 2020 2020 2020 2020 7368 6170 653d            shape=
-00010700: 2874 656d 7065 7261 7475 7265 5f70 6f69  (temperature_poi
-00010710: 6e74 732c 2029 2c20 6474 7970 653d 2764  nts, ), dtype='d
-00010720: 6f75 626c 6527 2e0a 2020 2020 2020 2020  ouble'..        
-00010730: 2020 2020 5769 7468 204e 6f6e 652c 0a20      With None,. 
-00010740: 2020 2020 2020 2020 2020 2020 2020 2060                 `
-00010750: 6973 5f4c 4254 453d 4661 6c73 6560 2067  is_LBTE=False` g
-00010760: 6976 6573 2074 656d 7065 7261 7475 7265  ives temperature
-00010770: 733d 5b30 2c20 3130 2c20 2e2e 2e2c 2031  s=[0, 10, ..., 1
-00010780: 3030 305d 2e0a 2020 2020 2020 2020 2020  000]..          
-00010790: 2020 2020 2020 6069 735f 4c42 5445 3d54        `is_LBTE=T
-000107a0: 7275 6560 2067 6976 6573 2074 656d 7065  rue` gives tempe
-000107b0: 7261 7475 7265 733d 5b33 3030 2c20 5d2e  ratures=[300, ].
-000107c0: 0a20 2020 2020 2020 2069 735f 6973 6f74  .        is_isot
-000107d0: 6f70 6520 3a20 626f 6f6c 2c20 6f70 7469  ope : bool, opti
-000107e0: 6f6e 616c 2c20 6465 6661 756c 7420 6973  onal, default is
-000107f0: 2046 616c 7365 0a20 2020 2020 2020 2020   False.         
-00010800: 2020 2057 6974 6820 6f72 2077 6974 686f     With or witho
-00010810: 7574 2069 736f 746f 7065 2073 6361 7474  ut isotope scatt
-00010820: 6572 696e 672e 0a20 2020 2020 2020 206d  ering..        m
-00010830: 6173 735f 7661 7269 616e 6365 7320 3a20  ass_variances : 
-00010840: 6172 7261 795f 6c69 6b65 2c20 6f70 7469  array_like, opti
-00010850: 6f6e 616c 2c20 6465 6661 756c 7420 6973  onal, default is
-00010860: 204e 6f6e 650a 2020 2020 2020 2020 2020   None.          
-00010870: 2020 4d61 7373 2076 6172 6961 6e63 6573    Mass variances
-00010880: 2066 6f72 2069 736f 746f 7065 2073 6361   for isotope sca
-00010890: 7474 6572 696e 6720 6361 6c63 756c 6174  ttering calculat
-000108a0: 696f 6e2e 2057 6865 6e20 4e6f 6e65 2c0a  ion. When None,.
-000108b0: 2020 2020 2020 2020 2020 2020 7468 6520              the 
-000108c0: 7661 6c75 6573 2073 746f 7265 6420 696e  values stored in
-000108d0: 2070 686f 6e6f 3370 7920 6172 6520 7573   phono3py are us
-000108e0: 6564 2077 6974 6820 6069 735f 6973 6f74  ed with `is_isot
-000108f0: 6f70 653d 5472 7565 602e 0a20 2020 2020  ope=True`..     
-00010900: 2020 2020 2020 2073 6861 7065 2861 746f         shape(ato
-00010910: 6d73 5f69 6e5f 7072 696d 6974 6976 652c  ms_in_primitive,
-00010920: 2029 2c20 6474 7970 653d 2764 6f75 626c   ), dtype='doubl
-00010930: 6527 2e0a 2020 2020 2020 2020 6772 6964  e'..        grid
-00010940: 5f70 6f69 6e74 7320 3a20 6172 7261 795f  _points : array_
-00010950: 6c69 6b65 2c20 6f70 7469 6f6e 616c 2c20  like, optional, 
-00010960: 6465 6661 756c 7420 6973 204e 6f6e 650a  default is None.
-00010970: 2020 2020 2020 2020 2020 2020 4c69 7374              List
-00010980: 206f 6620 6772 6964 2070 6f69 6e74 2069   of grid point i
-00010990: 6e64 6963 6573 2077 6865 7265 206d 6f64  ndices where mod
-000109a0: 6520 7468 6572 6d61 6c20 636f 6e64 7563  e thermal conduc
-000109b0: 7469 7669 7469 6573 2061 7265 0a20 2020  tivities are.   
-000109c0: 2020 2020 2020 2020 2063 616c 6375 6c61           calcula
-000109d0: 7465 642e 2057 6974 6820 4e6f 6e65 2c20  ted. With None, 
-000109e0: 616c 6c20 7468 6520 6772 6964 2070 6f69  all the grid poi
-000109f0: 6e74 7320 7468 6174 2061 7265 206e 6563  nts that are nec
-00010a00: 6573 7361 7279 0a20 2020 2020 2020 2020  essary.         
-00010a10: 2020 2066 6f72 2074 6865 726d 616c 2063     for thermal c
-00010a20: 6f6e 6475 6374 6976 6974 7920 6172 6520  onductivity are 
-00010a30: 7365 7420 696e 7465 726e 616c 6c79 2e0a  set internally..
-00010a40: 2020 2020 2020 2020 2020 2020 7368 6170              shap
-00010a50: 6528 6e75 6d5f 6772 6964 5f70 6f69 6e74  e(num_grid_point
-00010a60: 732c 2029 2c20 6474 7970 653d 2769 6e74  s, ), dtype='int
-00010a70: 5f27 2e0a 2020 2020 2020 2020 626f 756e  _'..        boun
-00010a80: 6461 7279 5f6d 6670 203a 2066 6c6f 6174  dary_mfp : float
-00010a90: 2c20 6f70 7469 6f6e 612c 2064 6566 6175  , optiona, defau
-00010aa0: 6c74 2069 7320 4e6f 6e65 0a20 2020 2020  lt is None.     
-00010ab0: 2020 2020 2020 204d 6561 6e20 6672 6565         Mean free
-00010ac0: 2070 6174 6820 696e 206d 6963 726f 6d65   path in microme
-00010ad0: 7472 6520 746f 2063 616c 6375 6c61 7465  tre to calculate
-00010ae0: 2073 696d 706c 6520 626f 756e 6461 7279   simple boundary
-00010af0: 0a20 2020 2020 2020 2020 2020 2073 6361  .            sca
-00010b00: 7474 6572 696e 6720 636f 6e74 7269 6275  ttering contribu
-00010b10: 7469 6f6e 2074 6f20 7468 6572 6d61 6c20  tion to thermal 
-00010b20: 636f 6e64 7563 7469 7669 7479 2e0a 2020  conductivity..  
-00010b30: 2020 2020 2020 2020 2020 4e6f 6e65 2069            None i
-00010b40: 676e 6f72 6573 2074 6869 7320 636f 6e74  gnores this cont
-00010b50: 7269 6275 7469 6f6e 2e0a 2020 2020 2020  ribution..      
-00010b60: 2020 736f 6c76 655f 636f 6c6c 6563 7469    solve_collecti
-00010b70: 7665 5f70 686f 6e6f 6e20 3a20 626f 6f6c  ve_phonon : bool
-00010b80: 2c20 6f70 7469 6f6e 616c 2c20 6465 6661  , optional, defa
-00010b90: 756c 7420 6973 2046 616c 7365 0a20 2020  ult is False.   
-00010ba0: 2020 2020 2020 2020 2054 6869 7320 6973           This is
-00010bb0: 2061 6e20 6f70 7469 6f6e 2066 6f72 2074   an option for t
-00010bc0: 6865 2066 6561 7475 7265 2075 6e64 6572  he feature under
-00010bd0: 2064 6576 656c 6f70 6d65 6e74 2e0a 2020   development..  
-00010be0: 2020 2020 2020 7573 655f 6176 655f 7070        use_ave_pp
-00010bf0: 203a 2062 6f6f 6c2c 206f 7074 696f 6e61   : bool, optiona
-00010c00: 6c2c 2064 6566 6175 6c74 2069 7320 4661  l, default is Fa
-00010c10: 6c73 650a 2020 2020 2020 2020 2020 2020  lse.            
-00010c20: 5254 4120 6f6e 6c79 2028 6069 735f 4c42  RTA only (`is_LB
-00010c30: 5445 3d46 616c 7365 6029 2e20 4176 6572  TE=False`). Aver
-00010c40: 6167 6564 2070 686f 6e6f 6e2d 7068 6f6e  aged phonon-phon
-00010c50: 6f6e 2069 6e74 6572 6163 7469 6f6e 0a20  on interaction. 
-00010c60: 2020 2020 2020 2020 2020 2073 7472 656e             stren
-00010c70: 6774 6820 6973 2075 7365 6420 746f 2063  gth is used to c
-00010c80: 616c 6375 6c61 7465 2070 686f 6e6f 6e20  alculate phonon 
-00010c90: 6c69 6665 7469 6d65 2e20 5468 6973 2064  lifetime. This d
-00010ca0: 6f65 7320 6e6f 740a 2020 2020 2020 2020  oes not.        
-00010cb0: 2020 2020 7265 6475 6365 2063 6f6d 7075      reduce compu
-00010cc0: 7461 7469 6f6e 616c 2064 656d 616e 642c  tational demand,
-00010cd0: 2062 7574 206d 6179 2062 6520 7573 6564   but may be used
-00010ce0: 2074 6f20 6d6f 6465 6c20 7468 6572 6d61   to model therma
-00010cf0: 6c0a 2020 2020 2020 2020 2020 2020 636f  l.            co
-00010d00: 6e64 7563 7469 7669 7479 2066 6f72 2061  nductivity for a
-00010d10: 6e61 6c79 7a65 2074 6865 2063 616c 6375  nalyze the calcu
-00010d20: 6c61 7469 6f6e 2072 6573 756c 7473 2e0a  lation results..
-00010d30: 2020 2020 2020 2020 6973 5f72 6564 7563          is_reduc
-00010d40: 6962 6c65 5f63 6f6c 6c69 7369 6f6e 5f6d  ible_collision_m
-00010d50: 6174 7269 7820 3a20 626f 6f6c 2c20 6f70  atrix : bool, op
-00010d60: 7469 6f6e 616c 2c20 6465 6661 756c 7420  tional, default 
-00010d70: 6973 2046 616c 7365 0a20 2020 2020 2020  is False.       
-00010d80: 2020 2020 2044 6972 6563 7420 736f 6c75       Direct solu
-00010d90: 7469 6f6e 206f 6e6c 7920 2860 6973 5f4c  tion only (`is_L
-00010da0: 4254 453d 5472 7565 6029 2e20 5468 6973  BTE=True`). This
-00010db0: 2069 7320 616e 2065 7870 6572 696d 656e   is an experimen
-00010dc0: 7461 6c0a 2020 2020 2020 2020 2020 2020  tal.            
-00010dd0: 6f70 7469 6f6e 2e20 5769 7468 2054 7275  option. With Tru
-00010de0: 652c 2066 756c 6c20 636f 6c6c 6973 696f  e, full collisio
-00010df0: 6e20 6d61 7472 6978 2069 7320 6372 6561  n matrix is crea
-00010e00: 7465 6420 616e 6420 736f 6c76 6564 2e0a  ted and solved..
-00010e10: 2020 2020 2020 2020 6973 5f6b 6170 7061          is_kappa
-00010e20: 5f73 7461 7220 3a20 626f 6f6c 2c20 6f70  _star : bool, op
-00010e30: 7469 6f6e 616c 2c20 6465 6661 756c 7420  tional, default 
-00010e40: 6973 2054 7275 650a 2020 2020 2020 2020  is True.        
-00010e50: 2020 2020 5769 7468 2074 7275 652c 2073      With true, s
-00010e60: 796d 6d65 7472 7920 6973 2063 6f6e 7369  ymmetry is consi
-00010e70: 6465 7265 6420 7768 656e 2073 616d 706c  dered when sampl
-00010e80: 696e 6720 6772 6964 2070 6f69 6e74 730a  ing grid points.
-00010e90: 2020 2020 2020 2020 2020 2020 6174 2077              at w
-00010ea0: 6869 6368 206d 6f64 6520 7468 6572 6d61  hich mode therma
-00010eb0: 6c20 636f 6e64 7563 7469 7669 7469 6573  l conductivities
-00010ec0: 2061 7265 2063 616c 6375 6c61 7465 642e   are calculated.
-00010ed0: 0a20 2020 2020 2020 2067 765f 6465 6c74  .        gv_delt
-00010ee0: 615f 7120 3a20 666c 6f61 742c 206f 7074  a_q : float, opt
-00010ef0: 696f 6e61 6c2c 2064 6566 6175 6c74 2069  ional, default i
-00010f00: 7320 4e6f 6e65 2c20 2023 2066 6f72 2067  s None,  # for g
-00010f10: 726f 7570 2076 656c 6f63 6974 790a 2020  roup velocity.  
-00010f20: 2020 2020 2020 2020 2020 5769 7468 206e            With n
-00010f30: 6f6e 2d61 6e61 6c79 7469 6361 6c20 636f  on-analytical co
-00010f40: 7272 6563 7469 6f6e 2c20 6772 6f75 7020  rrection, group 
-00010f50: 7665 6c6f 6369 7479 2069 7320 6361 6c63  velocity is calc
-00010f60: 756c 6174 6564 0a20 2020 2020 2020 2020  ulated.         
-00010f70: 2020 2062 7920 6365 6e74 7261 6c20 6669     by central fi
-00010f80: 6e69 7465 2064 6966 6665 7265 6e63 6520  nite difference 
-00010f90: 6d65 7468 6f64 2e20 5468 6973 2076 616c  method. This val
-00010fa0: 7565 2067 6976 6573 2074 6865 2064 6973  ue gives the dis
-00010fb0: 7461 6e63 650a 2020 2020 2020 2020 2020  tance.          
-00010fc0: 2020 696e 2062 6f74 6820 6469 7265 6374    in both direct
-00010fd0: 696f 6e73 2069 6e20 312f 416e 6773 7472  ions in 1/Angstr
-00010fe0: 6f6d 2e20 5468 6520 6465 6661 756c 7420  om. The default 
-00010ff0: 7661 6c75 6520 7769 6c6c 2062 6520 3165  value will be 1e
-00011000: 2d35 2e0a 2020 2020 2020 2020 6973 5f66  -5..        is_f
-00011010: 756c 6c5f 7070 203a 2062 6f6f 6c2c 206f  ull_pp : bool, o
-00011020: 7074 696f 6e61 6c2c 2064 6566 6175 6c74  ptional, default
-00011030: 2069 7320 4661 6c73 650a 2020 2020 2020   is False.      
-00011040: 2020 2020 2020 5769 7468 2054 7275 652c        With True,
-00011050: 2066 756c 6c20 656c 656d 656e 7473 206f   full elements o
-00011060: 6620 7068 6f6e 6f6e 2d70 686f 6e6f 6e20  f phonon-phonon 
-00011070: 696e 7465 7261 6374 696f 6e20 7374 7265  interaction stre
-00011080: 6e67 7468 0a20 2020 2020 2020 2020 2020  ngth.           
-00011090: 2061 7265 2063 6f6d 7075 7465 642e 2048   are computed. H
-000110a0: 6f77 6576 6572 2077 6974 6820 7465 7472  owever with tetr
-000110b0: 6168 6564 726f 6e20 6d65 7468 6f64 2c20  ahedron method, 
-000110c0: 7061 7274 206f 6620 7468 656d 2061 7265  part of them are
-000110d0: 0a20 2020 2020 2020 2020 2020 206b 6e6f  .            kno
-000110e0: 776e 2074 6f20 6265 207a 6572 6f20 616e  wn to be zero an
-000110f0: 6420 756e 6e65 6365 7373 6172 7920 746f  d unnecessary to
-00011100: 2063 616c 6375 6c61 7469 6f6e 2e20 5769   calculation. Wi
-00011110: 7468 2046 616c 7365 2c0a 2020 2020 2020  th False,.      
-00011120: 2020 2020 2020 7468 6f73 6520 656c 656d        those elem
-00011130: 656e 7473 2061 7265 206e 6f74 2063 616c  ents are not cal
-00011140: 6375 6c61 7465 642c 2062 7920 7768 6963  culated, by whic
-00011150: 6820 636f 6e73 6964 6572 6162 6c65 0a20  h considerable. 
-00011160: 2020 2020 2020 2020 2020 2069 6d70 726f             impro
-00011170: 7665 206f 6620 6566 6669 6369 656e 6379  ve of efficiency
-00011180: 2069 7320 6578 7065 6374 6564 2e0a 2020   is expected..  
-00011190: 2020 2020 2020 2020 2020 5769 7468 2073            With s
-000111a0: 6d65 6172 696e 6720 6d65 7468 6f64 2c20  mearing method, 
-000111b0: 6576 656e 2069 6620 7468 6973 2069 7320  even if this is 
-000111c0: 7365 7420 4661 6c73 652c 2066 756c 6c20  set False, full 
-000111d0: 656c 656d 656e 7473 0a20 2020 2020 2020  elements.       
-000111e0: 2020 2020 2061 7265 2063 6f6d 7075 7465       are compute
-000111f0: 6420 756e 6c65 7373 2060 7369 676d 615f  d unless `sigma_
-00011200: 6375 746f 6666 6020 6973 2073 7065 6369  cutoff` is speci
-00011210: 6669 6564 2e0a 2020 2020 2020 2020 7069  fied..        pi
-00011220: 6e76 5f63 7574 6f66 6620 3a20 666c 6f61  nv_cutoff : floa
-00011230: 742c 206f 7074 696f 6e61 6c2c 2064 6566  t, optional, def
-00011240: 6175 6c74 2069 7320 312e 3065 2d38 0a20  ault is 1.0e-8. 
-00011250: 2020 2020 2020 2020 2020 2044 6972 6563             Direc
-00011260: 7420 736f 6c75 7469 6f6e 206f 6e6c 7920  t solution only 
-00011270: 2860 6973 5f4c 4254 453d 5472 7565 6029  (`is_LBTE=True`)
-00011280: 2e20 5468 6973 2069 7320 7573 6564 2061  . This is used a
-00011290: 7320 6120 6372 6974 6572 696f 6e0a 2020  s a criterion.  
-000112a0: 2020 2020 2020 2020 2020 746f 206a 7564            to jud
-000112b0: 6765 2074 6865 2065 6967 656e 7661 6c75  ge the eigenvalu
-000112c0: 6573 2061 7265 2063 6f6e 7369 6465 7265  es are considere
-000112d0: 6420 6173 207a 6572 6f20 6f72 206e 6f74  d as zero or not
-000112e0: 2069 6e0a 2020 2020 2020 2020 2020 2020   in.            
-000112f0: 7073 6575 646f 2d69 6e76 6572 7369 6f6e  pseudo-inversion
-00011300: 206f 6620 636f 6c6c 6973 696f 6e20 6d61   of collision ma
-00011310: 7472 6978 2e20 5365 6520 616c 736f 2060  trix. See also `
-00011320: 7069 6e76 5f6d 6574 686f 6460 2e0a 2020  pinv_method`..  
-00011330: 2020 2020 2020 7069 6e76 5f6d 6574 686f        pinv_metho
-00011340: 6420 3a20 696e 742c 206f 7074 696f 6e61  d : int, optiona
-00011350: 6c2c 2064 6566 6175 6c74 2069 7320 302e  l, default is 0.
-00011360: 0a20 2020 2020 2020 2020 2020 2044 6972  .            Dir
-00011370: 6563 7420 736f 6c75 7469 6f6e 206f 6e6c  ect solution onl
-00011380: 7920 2860 6973 5f4c 4254 453d 5472 7565  y (`is_LBTE=True
-00011390: 6029 2e0a 2020 2020 2020 2020 2020 2020  `)..            
-000113a0: 2020 2020 302e 2061 6273 2865 6967 656e      0. abs(eigen
-000113b0: 7661 6c75 6529 203c 2060 7069 6e76 5f63  value) < `pinv_c
-000113c0: 7574 6f66 6660 0a20 2020 2020 2020 2020  utoff`.         
-000113d0: 2020 2020 2020 2031 2e20 6569 6765 6e76         1. eigenv
-000113e0: 616c 7565 203c 2060 7069 6e76 5f63 7574  alue < `pinv_cut
-000113f0: 6f66 6660 0a20 2020 2020 2020 2070 696e  off`.        pin
-00011400: 765f 736f 6c76 6572 203a 2069 6e74 2c20  v_solver : int, 
-00011410: 6f70 7469 6f6e 616c 2c20 6465 6661 756c  optional, defaul
-00011420: 7420 6973 2030 0a20 2020 2020 2020 2020  t is 0.         
-00011430: 2020 2044 6972 6563 7420 736f 6c75 7469     Direct soluti
-00011440: 6f6e 206f 6e6c 7920 2860 6973 5f4c 4254  on only (`is_LBT
-00011450: 453d 5472 7565 6029 2e20 4368 6f69 6365  E=True`). Choice
-00011460: 206f 6620 736f 6c76 6572 206f 660a 2020   of solver of.  
-00011470: 2020 2020 2020 2020 2020 7073 6575 646f            pseudo
-00011480: 2d69 6e76 6572 7369 6f6e 206f 6620 636f  -inversion of co
-00011490: 6c6c 6973 696f 6e20 6d61 7472 6978 2e20  llision matrix. 
-000114a0: 3020 6d65 616e 7320 7468 6520 6465 6661  0 means the defa
-000114b0: 756c 7420 6368 6f69 6365 2e0a 2020 2020  ult choice..    
-000114c0: 2020 2020 2020 2020 2020 2020 312e 204c              1. L
-000114d0: 6170 6163 6b65 2064 7379 6576 3a20 536d  apacke dsyev: Sm
-000114e0: 616c 6c65 7220 6d65 6d6f 7279 2063 6f6e  aller memory con
-000114f0: 7375 6d70 7469 6f6e 2074 6861 6e20 6473  sumption than ds
-00011500: 7965 7664 2c20 6275 740a 2020 2020 2020  yevd, but.      
-00011510: 2020 2020 2020 2020 2020 2020 2073 6c6f               slo
-00011520: 7765 722e 2054 6869 7320 6973 2074 6865  wer. This is the
-00011530: 2064 6566 6175 6c74 2073 6f6c 7665 7220   default solver 
-00011540: 7768 656e 204d 4b4c 204c 4150 4143 4b45  when MKL LAPACKE
-00011550: 2069 730a 2020 2020 2020 2020 2020 2020   is.            
-00011560: 2020 2020 2020 2069 6e74 6567 7261 7465         integrate
-00011570: 6420 6f72 2073 6369 7079 2069 7320 6e6f  d or scipy is no
-00011580: 7420 696e 7374 616c 6c65 642e 0a20 2020  t installed..   
-00011590: 2020 2020 2020 2020 2020 2020 2032 2e20               2. 
-000115a0: 4c61 7061 636b 6520 6473 7965 7664 3a20  Lapacke dsyevd: 
-000115b0: 4c61 7267 6572 206d 656d 6f72 7920 636f  Larger memory co
-000115c0: 6e73 756d 7074 696f 6e20 7468 616e 2064  nsumption than d
-000115d0: 7379 6576 2c20 6275 740a 2020 2020 2020  syev, but.      
-000115e0: 2020 2020 2020 2020 2020 2020 2066 6173               fas
-000115f0: 7465 722e 2054 6869 7320 6973 206e 6f74  ter. This is not
-00011600: 2072 6563 6f6d 6d65 6e64 6564 2062 6563   recommended bec
-00011610: 6175 7365 2073 6f6d 6574 696d 6573 2061  ause sometimes a
-00011620: 2077 726f 6e67 0a20 2020 2020 2020 2020   wrong.         
-00011630: 2020 2020 2020 2020 2020 7265 7375 6c74            result
-00011640: 2069 7320 6f62 7461 696e 6564 2e0a 2020   is obtained..  
-00011650: 2020 2020 2020 2020 2020 2020 2020 332e                3.
-00011660: 204e 756d 7079 e280 9973 2064 7379 6576   Numpy...s dsyev
-00011670: 6420 286c 696e 616c 672e 6569 6768 292e  d (linalg.eigh).
-00011680: 2054 6869 7320 6973 206e 6f74 2072 6563   This is not rec
-00011690: 6f6d 6d65 6e64 6564 0a20 2020 2020 2020  ommended.       
-000116a0: 2020 2020 2020 2020 2020 2020 6265 6361              beca
-000116b0: 7573 6520 736f 6d65 7469 6d65 7320 6120  use sometimes a 
-000116c0: 7772 6f6e 6720 7265 7375 6c74 2069 7320  wrong result is 
-000116d0: 6f62 7461 696e 6564 2e0a 2020 2020 2020  obtained..      
-000116e0: 2020 2020 2020 2020 2020 342e 2053 6369            4. Sci
-000116f0: 7079 e280 9973 2064 7379 6576 3a20 5468  py...s dsyev: Th
-00011700: 6973 2069 7320 7468 6520 6465 6661 756c  is is the defaul
-00011710: 7420 736f 6c76 6572 2077 6865 6e20 7363  t solver when sc
-00011720: 6970 7920 6973 0a20 2020 2020 2020 2020  ipy is.         
-00011730: 2020 2020 2020 2020 2020 696e 7374 616c            instal
-00011740: 6c65 6420 616e 6420 4d4b 4c20 4c41 5041  led and MKL LAPA
-00011750: 434b 4520 6973 206e 6f74 2069 6e74 6567  CKE is not integ
-00011760: 7261 7465 642e 0a20 2020 2020 2020 2020  rated..         
-00011770: 2020 2020 2020 2035 2e20 5363 6970 79e2         5. Scipy.
-00011780: 8099 7320 6473 7965 7664 2e20 5468 6973  ..s dsyevd. This
-00011790: 2069 7320 6e6f 7420 7265 636f 6d6d 656e   is not recommen
-000117a0: 6465 6420 6265 6361 7573 6520 736f 6d65  ded because some
-000117b0: 7469 6d65 730a 2020 2020 2020 2020 2020  times.          
-000117c0: 2020 2020 2020 2020 2061 2077 726f 6e67           a wrong
-000117d0: 2072 6573 756c 7420 6973 206f 6274 6169   result is obtai
-000117e0: 6e65 642e 0a20 2020 2020 2020 2020 2020  ned..           
-000117f0: 2054 6865 2073 6f6c 7665 7220 6368 6f69   The solver choi
-00011800: 6365 7320 6f74 6865 7220 7468 616e 202d  ces other than -
-00011810: 2d70 696e 762d 736f 6c76 6572 3d31 2061  -pinv-solver=1 a
-00011820: 6e64 0a20 2020 2020 2020 2020 2020 202d  nd.            -
-00011830: 2d70 696e 762d 736f 6c76 6572 3d34 2061  -pinv-solver=4 a
-00011840: 7265 2064 616e 6765 726f 7573 2061 6e64  re dangerous and
-00011850: 206e 6f74 2072 6563 6f6d 6d65 6e64 2e0a   not recommend..
-00011860: 2020 2020 2020 2020 7772 6974 655f 6761          write_ga
-00011870: 6d6d 6120 3a20 626f 6f6c 2c20 6f70 7469  mma : bool, opti
-00011880: 6f6e 616c 2c20 6465 6661 756c 7420 6973  onal, default is
-00011890: 2046 616c 7365 0a20 2020 2020 2020 2020   False.         
-000118a0: 2020 2052 5441 206f 6e6c 7920 2860 6973     RTA only (`is
-000118b0: 5f4c 4254 453d 4661 6c73 6560 292e 2057  _LBTE=False`). W
-000118c0: 6974 6820 5472 7565 2c20 5772 6974 6520  ith True, Write 
-000118d0: 6d6f 6465 2074 6865 726d 616c 0a20 2020  mode thermal.   
-000118e0: 2020 2020 2020 2020 2063 6f6e 6475 6374           conduct
-000118f0: 6976 6974 7920 7072 6f70 6572 7469 6573  ivity properties
-00011900: 2069 6e74 6f20 6669 6c65 7320 6174 2065   into files at e
-00011910: 6163 6820 6772 6964 2070 6f69 6e74 2e20  ach grid point. 
-00011920: 5769 7468 0a20 2020 2020 2020 2020 2020  With.           
-00011930: 2060 6261 6e64 5f69 6e64 6963 6573 6020   `band_indices` 
-00011940: 6f72 206d 756c 7469 706c 6520 6073 6967  or multiple `sig
-00011950: 6d61 7360 2069 7320 7370 6563 6966 6965  mas` is specifie
-00011960: 642c 2074 6865 2066 696c 6573 0a20 2020  d, the files.   
-00011970: 2020 2020 2020 2020 2061 7265 206d 6164           are mad
-00011980: 6520 666f 7220 6561 6368 206f 6620 7468  e for each of th
-00011990: 656d 2c20 746f 6f2e 0a20 2020 2020 2020  em, too..       
-000119a0: 2072 6561 645f 6761 6d6d 6120 3a20 626f   read_gamma : bo
-000119b0: 6f6c 2c20 6f70 7469 6f6e 616c 2c20 6465  ol, optional, de
-000119c0: 6661 756c 7420 6973 2046 616c 7365 0a20  fault is False. 
-000119d0: 2020 2020 2020 2020 2020 2052 5441 206f             RTA o
-000119e0: 6e6c 7920 2860 6973 5f4c 4254 453d 4661  nly (`is_LBTE=Fa
-000119f0: 6c73 6560 292e 2057 6974 6820 5472 7565  lse`). With True
-00011a00: 2c20 6465 6164 2066 696c 6573 2063 7265  , dead files cre
-00011a10: 6174 6564 2062 790a 2020 2020 2020 2020  ated by.        
-00011a20: 2020 2020 6077 7269 7465 5f67 616d 6d61      `write_gamma
-00011a30: 3d54 7275 6560 2069 6e73 7465 6164 206f  =True` instead o
-00011a40: 6620 6361 6c63 756c 6174 696e 6720 7068  f calculating ph
-00011a50: 6f6e 6f6e 2d70 686f 6e6f 6e0a 2020 2020  onon-phonon.    
-00011a60: 2020 2020 2020 2020 696e 7465 7261 6374          interact
-00011a70: 696f 6e20 7374 7265 6e67 7468 2061 6e64  ion strength and
-00011a80: 2069 6d61 6769 6e61 7279 2070 6172 7473   imaginary parts
-00011a90: 206f 6620 7365 6c66 2d65 6e65 7267 792e   of self-energy.
-00011aa0: 0a20 2020 2020 2020 2069 735f 4e5f 5520  .        is_N_U 
-00011ab0: 3a20 626f 6f6c 2c20 6f70 7469 6f6e 616c  : bool, optional
-00011ac0: 2c20 6465 6661 756c 7420 6973 2046 616c  , default is Fal
-00011ad0: 7365 0a20 2020 2020 2020 2020 2020 2052  se.            R
-00011ae0: 5441 206f 6e6c 7920 2860 6973 5f4c 4254  TA only (`is_LBT
-00011af0: 453d 4661 6c73 6560 292e 2057 6974 6820  E=False`). With 
-00011b00: 5472 7565 2c20 6361 7465 676f 7269 7a61  True, categoriza
-00011b10: 7469 6f6e 206f 6620 6e6f 726d 616c 0a20  tion of normal. 
-00011b20: 2020 2020 2020 2020 2020 2061 6e64 2055             and U
-00011b30: 6d6b 6c61 7070 2073 6361 7474 6572 696e  mklapp scatterin
-00011b40: 6720 6973 206d 6164 6520 616e 6420 696d  g is made and im
-00011b50: 6167 696e 6172 7920 7061 7274 7320 6f66  aginary parts of
-00011b60: 2073 656c 6620 656e 6572 6779 0a20 2020   self energy.   
-00011b70: 2020 2020 2020 2020 2066 6f72 2074 6865           for the
-00011b80: 6d20 6172 6520 7365 7061 7261 7465 642e  m are separated.
-00011b90: 0a20 2020 2020 2020 2063 6f6e 6475 6374  .        conduct
-00011ba0: 6976 6974 795f 7479 7065 203a 2073 7472  ivity_type : str
-00011bb0: 2c20 6f70 7469 6f6e 616c 0a20 2020 2020  , optional.     
-00011bc0: 2020 2020 2020 2022 7769 676e 6572 222c         "wigner",
-00011bd0: 2022 6b75 626f 222c 206f 7220 4e6f 6e65   "kubo", or None
-00011be0: 2e20 4465 6661 756c 7420 6973 204e 6f6e  . Default is Non
-00011bf0: 652e 0a20 2020 2020 2020 2077 7269 7465  e..        write
-00011c00: 5f6b 6170 7061 203a 2062 6f6f 6c2c 206f  _kappa : bool, o
-00011c10: 7074 696f 6e61 6c2c 2064 6566 6175 6c74  ptional, default
-00011c20: 2069 7320 4661 6c73 650a 2020 2020 2020   is False.      
-00011c30: 2020 2020 2020 5769 7468 2054 7275 652c        With True,
-00011c40: 2074 6865 726d 616c 2063 6f6e 6475 6374   thermal conduct
-00011c50: 6976 6974 7920 616e 6420 7265 6c61 7465  ivity and relate
-00011c60: 6420 7072 6f70 6572 7469 6573 2061 7265  d properties are
-00011c70: 0a20 2020 2020 2020 2020 2020 2077 7269  .            wri
-00011c80: 7474 656e 2069 6e74 6f20 6120 6669 6c65  tten into a file
-00011c90: 2e20 5769 7468 206d 756c 7469 706c 6520  . With multiple 
-00011ca0: 6073 6967 6d61 7360 2c20 7265 7370 6563  `sigmas`, respec
-00011cb0: 7469 7665 2066 696c 6573 0a20 2020 2020  tive files.     
-00011cc0: 2020 2020 2020 2061 7265 2063 7265 6174         are creat
-00011cd0: 6564 2e0a 2020 2020 2020 2020 7772 6974  ed..        writ
-00011ce0: 655f 6761 6d6d 615f 6465 7461 696c 203a  e_gamma_detail :
-00011cf0: 2062 6f6f 6c2c 206f 7074 696f 6e61 6c2c   bool, optional,
-00011d00: 2064 6566 6175 6c74 2069 7320 4661 6c73   default is Fals
-00011d10: 650a 2020 2020 2020 2020 2020 2020 5254  e.            RT
-00011d20: 4120 6f6e 6c79 2028 6069 735f 4c42 5445  A only (`is_LBTE
-00011d30: 3d46 616c 7365 6029 2e20 5769 7468 2054  =False`). With T
-00011d40: 7275 652c 2064 6574 6169 6c65 6420 696e  rue, detailed in
-00011d50: 666f 726d 6174 696f 6e20 6f66 0a20 2020  formation of.   
-00011d60: 2020 2020 2020 2020 2069 6d61 6769 6e61           imagina
-00011d70: 7279 2070 6172 7473 206f 6620 7365 6c66  ry parts of self
-00011d80: 2065 6e65 7267 7920 6973 2073 746f 7265   energy is store
-00011d90: 6420 696e 746f 2066 696c 6573 2073 7563  d into files suc
-00011da0: 6820 6173 0a20 2020 2020 2020 2020 2020  h as.           
-00011db0: 2074 686f 7365 206d 6164 6520 6279 2060   those made by `
-00011dc0: 7772 6974 655f 6761 6d6d 6160 2e0a 2020  write_gamma`..  
-00011dd0: 2020 2020 2020 7772 6974 655f 636f 6c6c        write_coll
-00011de0: 6973 696f 6e20 3a20 626f 6f6c 2c20 6f70  ision : bool, op
-00011df0: 7469 6f6e 616c 2c20 6465 6661 756c 7420  tional, default 
-00011e00: 6973 2046 616c 7365 0a20 2020 2020 2020  is False.       
-00011e10: 2020 2020 2044 6972 6563 7420 736f 6c75       Direct solu
-00011e20: 7469 6f6e 206f 6e6c 7920 2860 6973 5f4c  tion only (`is_L
-00011e30: 4254 453d 5472 7565 6029 2e20 5769 7468  BTE=True`). With
-00011e40: 2054 7275 652c 2063 6f6c 6c69 7369 6f6e   True, collision
-00011e50: 206d 6174 7269 780a 2020 2020 2020 2020   matrix.        
-00011e60: 2020 2020 6973 2077 7269 7474 656e 2069      is written i
-00011e70: 6e74 6f20 6120 6669 6c65 2e20 5769 7468  nto a file. With
-00011e80: 206d 756c 7469 706c 6520 6073 6967 6d61   multiple `sigma
-00011e90: 7360 2073 7065 6369 6669 6564 2c0a 2020  s` specified,.  
-00011ea0: 2020 2020 2020 2020 2020 7265 7370 6563            respec
-00011eb0: 7469 7665 2066 696c 6573 2061 7265 2063  tive files are c
-00011ec0: 7265 6174 6564 2e20 4265 2063 6172 6566  reated. Be caref
-00011ed0: 756c 2074 6861 7420 7468 6973 2066 696c  ul that this fil
-00011ee0: 6520 6361 6e20 6265 0a20 2020 2020 2020  e can be.       
-00011ef0: 2020 2020 2068 7567 652e 0a20 2020 2020       huge..     
-00011f00: 2020 2072 6561 645f 636f 6c6c 6973 696f     read_collisio
-00011f10: 6e20 3a20 626f 6f6c 2c20 6f70 7469 6f6e  n : bool, option
-00011f20: 616c 2c20 6465 6661 756c 7420 6973 2046  al, default is F
-00011f30: 616c 7365 0a20 2020 2020 2020 2020 2020  alse.           
-00011f40: 2044 6972 6563 7420 736f 6c75 7469 6f6e   Direct solution
-00011f50: 206f 6e6c 7920 2860 6973 5f4c 4254 453d   only (`is_LBTE=
-00011f60: 5472 7565 6029 2e20 5769 7468 2054 7275  True`). With Tru
-00011f70: 652c 2063 6f6c 6c69 7369 6f6e 206d 6174  e, collision mat
-00011f80: 7269 780a 2020 2020 2020 2020 2020 2020  rix.            
-00011f90: 6973 2072 6561 6420 6672 6f6d 2061 2066  is read from a f
-00011fa0: 696c 652e 0a20 2020 2020 2020 2077 7269  ile..        wri
-00011fb0: 7465 5f70 7020 3a20 626f 6f6c 2c20 6f70  te_pp : bool, op
-00011fc0: 7469 6f6e 616c 2c20 6465 6661 756c 7420  tional, default 
-00011fd0: 6973 2046 616c 7365 0a20 2020 2020 2020  is False.       
-00011fe0: 2020 2020 2057 6974 6820 5472 7565 2c20       With True, 
-00011ff0: 7068 6f6e 6f6e 2d70 686f 6e6f 6e20 696e  phonon-phonon in
-00012000: 7465 7261 6374 696f 6e20 7374 7265 6e67  teraction streng
-00012010: 7468 2069 7320 7772 6974 7465 6e20 696e  th is written in
-00012020: 746f 0a20 2020 2020 2020 2020 2020 2066  to.            f
-00012030: 696c 6573 2061 7420 6561 6368 2067 7269  iles at each gri
-00012040: 6420 706f 696e 742e 2054 6869 7320 6f70  d point. This op
-00012050: 7469 6f6e 2061 7373 756d 6573 2073 696e  tion assumes sin
-00012060: 676c 6520 7661 6c75 6520 6973 2069 6e0a  gle value is in.
-00012070: 2020 2020 2020 2020 2020 2020 6073 6967              `sig
-00012080: 6d61 7360 2e0a 2020 2020 2020 2020 7265  mas`..        re
-00012090: 6164 5f70 7020 3a20 626f 6f6c 2c20 6f70  ad_pp : bool, op
-000120a0: 7469 6f6e 616c 2c20 6465 6661 756c 7420  tional, default 
-000120b0: 6973 2046 616c 7365 0a20 2020 2020 2020  is False.       
-000120c0: 2020 2020 2057 6974 6820 5472 7565 2c20       With True, 
-000120d0: 7068 6f6e 6f6e 2d70 686f 6e6f 6e20 696e  phonon-phonon in
-000120e0: 7465 7261 6374 696f 6e20 7374 7265 6e67  teraction streng
-000120f0: 7468 2069 7320 7265 6164 2066 726f 6d20  th is read from 
-00012100: 6669 6c65 732e 0a20 2020 2020 2020 2077  files..        w
-00012110: 7269 7465 5f4c 4254 455f 736f 6c75 7469  rite_LBTE_soluti
-00012120: 6f6e 203a 2062 6f6f 6c2c 206f 7074 696f  on : bool, optio
-00012130: 6e61 6c2c 2064 6566 6175 6c74 2069 7320  nal, default is 
-00012140: 4661 6c73 650a 2020 2020 2020 2020 2020  False.          
-00012150: 2020 4469 7265 6374 2073 6f6c 7574 696f    Direct solutio
-00012160: 6e20 6f6e 6c79 2028 6069 735f 4c42 5445  n only (`is_LBTE
-00012170: 3d54 7275 6560 292e 2057 6974 6820 5472  =True`). With Tr
-00012180: 7565 2c20 6569 6765 6e76 6563 746f 7273  ue, eigenvectors
-00012190: 206f 660a 2020 2020 2020 2020 2020 2020   of.            
-000121a0: 636f 6c6c 6973 696f 6e20 6d61 7472 6978  collision matrix
-000121b0: 2069 7320 7772 6974 7465 6e20 696e 2061   is written in a
-000121c0: 2066 696c 6520 6173 2074 6865 2072 6f77   file as the row
-000121d0: 2076 6563 746f 7273 2065 7863 6570 740a   vectors except.
-000121e0: 2020 2020 2020 2020 2020 2020 756e 6c65              unle
-000121f0: 7373 2060 7069 6e76 5f73 6f6c 7665 723d  ss `pinv_solver=
-00012200: 3360 2028 666f 7220 7468 6973 2c20 636f  3` (for this, co
-00012210: 6c75 6d6e 2076 6563 746f 7273 292e 2057  lumn vectors). W
-00012220: 6974 6820 6d75 6c74 6970 6c65 0a20 2020  ith multiple.   
-00012230: 2020 2020 2020 2020 2060 7369 676d 6173           `sigmas
-00012240: 6020 7370 6563 6966 6965 642c 2072 6573  ` specified, res
-00012250: 7065 6374 6976 6520 6669 6c65 7320 6172  pective files ar
-00012260: 6520 6372 6561 7465 642e 2042 6520 6361  e created. Be ca
-00012270: 7265 6675 6c20 7468 6174 0a20 2020 2020  reful that.     
-00012280: 2020 2020 2020 2074 6869 7320 6669 6c65         this file
-00012290: 2063 616e 2062 6520 6875 6765 2e0a 2020   can be huge..  
-000122a0: 2020 2020 2020 636f 6d70 7265 7373 696f        compressio
-000122b0: 6e3a 2073 7472 2c20 6f70 7469 6f6e 616c  n: str, optional
-000122c0: 2c20 6465 6661 756c 7420 6973 2022 677a  , default is "gz
-000122d0: 6970 220a 2020 2020 2020 2020 2020 2020  ip".            
-000122e0: 5768 656e 2077 7269 7469 6e67 2072 6573  When writing res
-000122f0: 756c 7473 2069 6e74 6f20 6669 6c65 7320  ults into files 
-00012300: 696e 2068 6466 352c 206c 6172 6765 2064  in hdf5, large d
-00012310: 6174 6120 6172 6520 636f 6d70 7265 7373  ata are compress
-00012320: 6564 0a20 2020 2020 2020 2020 2020 2062  ed.            b
-00012330: 7920 7468 6973 206f 7074 696f 6e73 2e20  y this options. 
-00012340: 5365 6520 7468 6520 6465 7461 696c 2061  See the detail a
-00012350: 7420 6835 7079 2064 6f63 756d 656e 7461  t h5py documenta
-00012360: 7469 6f6e 2e0a 2020 2020 2020 2020 696e  tion..        in
-00012370: 7075 745f 6669 6c65 6e61 6d65 203a 2073  put_filename : s
-00012380: 7472 2c20 6f70 7469 6f6e 616c 2c20 6465  tr, optional, de
-00012390: 6661 756c 7420 6973 204e 6f6e 650a 2020  fault is None.  
-000123a0: 2020 2020 2020 2020 2020 5768 656e 2073            When s
-000123b0: 7065 6369 6669 6564 2c20 7468 6520 7374  pecified, the st
-000123c0: 7269 6e67 2069 7320 696e 7365 7274 6564  ring is inserted
-000123d0: 2062 6566 6f72 6520 6669 6c65 6e61 6d65   before filename
-000123e0: 2065 7874 656e 7369 6f6e 0a20 2020 2020   extension.     
-000123f0: 2020 2020 2020 2069 6e20 7265 6164 696e         in readin
-00012400: 6720 6669 6c65 732e 0a20 2020 2020 2020  g files..       
-00012410: 206f 7574 7075 745f 6669 6c65 6e61 6d65   output_filename
-00012420: 203a 2073 7472 2c20 6f70 7469 6f6e 616c   : str, optional
-00012430: 2c20 6465 6661 756c 7420 6973 204e 6f6e  , default is Non
-00012440: 650a 2020 2020 2020 2020 2020 2020 5768  e.            Wh
-00012450: 656e 2073 7065 6369 6669 6564 2c20 7468  en specified, th
-00012460: 6520 7374 7269 6e67 2069 7320 696e 7365  e string is inse
-00012470: 7274 6564 2062 6566 6f72 6520 6669 6c65  rted before file
-00012480: 6e61 6d65 2065 7874 656e 7369 6f6e 0a20  name extension. 
-00012490: 2020 2020 2020 2020 2020 2069 6e20 7772             in wr
-000124a0: 6974 696e 6720 6669 6c65 732e 0a0a 2020  iting files...  
-000124b0: 2020 2020 2020 2222 220a 2020 2020 2020        """.      
-000124c0: 2020 6966 2073 656c 662e 5f69 6e74 6572    if self._inter
-000124d0: 6163 7469 6f6e 2069 7320 4e6f 6e65 3a0a  action is None:.
-000124e0: 2020 2020 2020 2020 2020 2020 6d73 6720              msg 
-000124f0: 3d20 280a 2020 2020 2020 2020 2020 2020  = (.            
-00012500: 2020 2020 2250 686f 6e6f 3370 792e 696e      "Phono3py.in
-00012510: 6974 5f70 6870 685f 696e 7465 7261 6374  it_phph_interact
-00012520: 696f 6e20 6861 7320 746f 2062 6520 6361  ion has to be ca
-00012530: 6c6c 6564 2022 0a20 2020 2020 2020 2020  lled ".         
-00012540: 2020 2020 2020 2022 6265 666f 7265 2072         "before r
-00012550: 756e 6e69 6e67 2074 6869 7320 6d65 7468  unning this meth
-00012560: 6f64 2e22 0a20 2020 2020 2020 2020 2020  od.".           
-00012570: 2029 0a20 2020 2020 2020 2020 2020 2072   ).            r
-00012580: 6169 7365 2052 756e 7469 6d65 4572 726f  aise RuntimeErro
-00012590: 7228 6d73 6729 0a0a 2020 2020 2020 2020  r(msg)..        
-000125a0: 6966 2069 735f 4c42 5445 3a0a 2020 2020  if is_LBTE:.    
-000125b0: 2020 2020 2020 2020 6966 2074 656d 7065          if tempe
-000125c0: 7261 7475 7265 7320 6973 204e 6f6e 653a  ratures is None:
-000125d0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000125e0: 205f 7465 6d70 6572 6174 7572 6573 203d   _temperatures =
-000125f0: 205b 0a20 2020 2020 2020 2020 2020 2020   [.             
-00012600: 2020 2020 2020 2033 3030 2c0a 2020 2020         300,.    
-00012610: 2020 2020 2020 2020 2020 2020 5d0a 2020              ].  
-00012620: 2020 2020 2020 2020 2020 656c 7365 3a0a            else:.
-00012630: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012640: 5f74 656d 7065 7261 7475 7265 7320 3d20  _temperatures = 
-00012650: 7465 6d70 6572 6174 7572 6573 0a20 2020  temperatures.   
-00012660: 2020 2020 2020 2020 2073 656c 662e 5f74           self._t
-00012670: 6865 726d 616c 5f63 6f6e 6475 6374 6976  hermal_conductiv
-00012680: 6974 7920 3d20 6765 745f 7468 6572 6d61  ity = get_therma
-00012690: 6c5f 636f 6e64 7563 7469 7669 7479 5f4c  l_conductivity_L
-000126a0: 4254 4528 0a20 2020 2020 2020 2020 2020  BTE(.           
-000126b0: 2020 2020 2073 656c 662e 5f69 6e74 6572       self._inter
-000126c0: 6163 7469 6f6e 2c0a 2020 2020 2020 2020  action,.        
-000126d0: 2020 2020 2020 2020 7465 6d70 6572 6174          temperat
-000126e0: 7572 6573 3d5f 7465 6d70 6572 6174 7572  ures=_temperatur
-000126f0: 6573 2c0a 2020 2020 2020 2020 2020 2020  es,.            
-00012700: 2020 2020 7369 676d 6173 3d73 656c 662e      sigmas=self.
-00012710: 5f73 6967 6d61 732c 0a20 2020 2020 2020  _sigmas,.       
-00012720: 2020 2020 2020 2020 2073 6967 6d61 5f63           sigma_c
-00012730: 7574 6f66 663d 7365 6c66 2e5f 7369 676d  utoff=self._sigm
-00012740: 615f 6375 746f 6666 2c0a 2020 2020 2020  a_cutoff,.      
-00012750: 2020 2020 2020 2020 2020 6973 5f69 736f            is_iso
-00012760: 746f 7065 3d69 735f 6973 6f74 6f70 652c  tope=is_isotope,
-00012770: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00012780: 206d 6173 735f 7661 7269 616e 6365 733d   mass_variances=
-00012790: 6d61 7373 5f76 6172 6961 6e63 6573 2c0a  mass_variances,.
-000127a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000127b0: 6772 6964 5f70 6f69 6e74 733d 6772 6964  grid_points=grid
-000127c0: 5f70 6f69 6e74 732c 0a20 2020 2020 2020  _points,.       
-000127d0: 2020 2020 2020 2020 2062 6f75 6e64 6172           boundar
-000127e0: 795f 6d66 703d 626f 756e 6461 7279 5f6d  y_mfp=boundary_m
-000127f0: 6670 2c0a 2020 2020 2020 2020 2020 2020  fp,.            
-00012800: 2020 2020 736f 6c76 655f 636f 6c6c 6563      solve_collec
-00012810: 7469 7665 5f70 686f 6e6f 6e3d 736f 6c76  tive_phonon=solv
-00012820: 655f 636f 6c6c 6563 7469 7665 5f70 686f  e_collective_pho
-00012830: 6e6f 6e2c 0a20 2020 2020 2020 2020 2020  non,.           
-00012840: 2020 2020 2069 735f 7265 6475 6369 626c       is_reducibl
-00012850: 655f 636f 6c6c 6973 696f 6e5f 6d61 7472  e_collision_matr
-00012860: 6978 3d69 735f 7265 6475 6369 626c 655f  ix=is_reducible_
-00012870: 636f 6c6c 6973 696f 6e5f 6d61 7472 6978  collision_matrix
-00012880: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-00012890: 2020 6973 5f6b 6170 7061 5f73 7461 723d    is_kappa_star=
-000128a0: 6973 5f6b 6170 7061 5f73 7461 722c 0a20  is_kappa_star,. 
-000128b0: 2020 2020 2020 2020 2020 2020 2020 2067                 g
-000128c0: 765f 6465 6c74 615f 713d 6776 5f64 656c  v_delta_q=gv_del
-000128d0: 7461 5f71 2c0a 2020 2020 2020 2020 2020  ta_q,.          
-000128e0: 2020 2020 2020 6973 5f66 756c 6c5f 7070        is_full_pp
-000128f0: 3d69 735f 6675 6c6c 5f70 702c 0a20 2020  =is_full_pp,.   
-00012900: 2020 2020 2020 2020 2020 2020 2063 6f6e               con
-00012910: 6475 6374 6976 6974 795f 7479 7065 3d63  ductivity_type=c
-00012920: 6f6e 6475 6374 6976 6974 795f 7479 7065  onductivity_type
-00012930: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-00012940: 2020 7069 6e76 5f63 7574 6f66 663d 7069    pinv_cutoff=pi
-00012950: 6e76 5f63 7574 6f66 662c 0a20 2020 2020  nv_cutoff,.     
-00012960: 2020 2020 2020 2020 2020 2070 696e 765f             pinv_
-00012970: 736f 6c76 6572 3d70 696e 765f 736f 6c76  solver=pinv_solv
-00012980: 6572 2c0a 2020 2020 2020 2020 2020 2020  er,.            
-00012990: 2020 2020 7069 6e76 5f6d 6574 686f 643d      pinv_method=
-000129a0: 7069 6e76 5f6d 6574 686f 642c 0a20 2020  pinv_method,.   
-000129b0: 2020 2020 2020 2020 2020 2020 2077 7269               wri
-000129c0: 7465 5f63 6f6c 6c69 7369 6f6e 3d77 7269  te_collision=wri
-000129d0: 7465 5f63 6f6c 6c69 7369 6f6e 2c0a 2020  te_collision,.  
-000129e0: 2020 2020 2020 2020 2020 2020 2020 7265                re
-000129f0: 6164 5f63 6f6c 6c69 7369 6f6e 3d72 6561  ad_collision=rea
-00012a00: 645f 636f 6c6c 6973 696f 6e2c 0a20 2020  d_collision,.   
-00012a10: 2020 2020 2020 2020 2020 2020 2077 7269               wri
-00012a20: 7465 5f6b 6170 7061 3d77 7269 7465 5f6b  te_kappa=write_k
-00012a30: 6170 7061 2c0a 2020 2020 2020 2020 2020  appa,.          
-00012a40: 2020 2020 2020 7772 6974 655f 7070 3d77        write_pp=w
-00012a50: 7269 7465 5f70 702c 0a20 2020 2020 2020  rite_pp,.       
-00012a60: 2020 2020 2020 2020 2072 6561 645f 7070           read_pp
-00012a70: 3d72 6561 645f 7070 2c0a 2020 2020 2020  =read_pp,.      
-00012a80: 2020 2020 2020 2020 2020 7772 6974 655f            write_
-00012a90: 4c42 5445 5f73 6f6c 7574 696f 6e3d 7772  LBTE_solution=wr
-00012aa0: 6974 655f 4c42 5445 5f73 6f6c 7574 696f  ite_LBTE_solutio
-00012ab0: 6e2c 0a20 2020 2020 2020 2020 2020 2020  n,.             
-00012ac0: 2020 2063 6f6d 7072 6573 7369 6f6e 3d63     compression=c
-00012ad0: 6f6d 7072 6573 7369 6f6e 2c0a 2020 2020  ompression,.    
-00012ae0: 2020 2020 2020 2020 2020 2020 696e 7075              inpu
-00012af0: 745f 6669 6c65 6e61 6d65 3d69 6e70 7574  t_filename=input
-00012b00: 5f66 696c 656e 616d 652c 0a20 2020 2020  _filename,.     
-00012b10: 2020 2020 2020 2020 2020 206f 7574 7075             outpu
-00012b20: 745f 6669 6c65 6e61 6d65 3d6f 7574 7075  t_filename=outpu
-00012b30: 745f 6669 6c65 6e61 6d65 2c0a 2020 2020  t_filename,.    
-00012b40: 2020 2020 2020 2020 2020 2020 6c6f 675f              log_
-00012b50: 6c65 7665 6c3d 7365 6c66 2e5f 6c6f 675f  level=self._log_
-00012b60: 6c65 7665 6c2c 0a20 2020 2020 2020 2020  level,.         
-00012b70: 2020 2029 0a20 2020 2020 2020 2065 6c73     ).        els
-00012b80: 653a 0a20 2020 2020 2020 2020 2020 2069  e:.            i
-00012b90: 6620 7465 6d70 6572 6174 7572 6573 2069  f temperatures i
-00012ba0: 7320 4e6f 6e65 3a0a 2020 2020 2020 2020  s None:.        
-00012bb0: 2020 2020 2020 2020 5f74 656d 7065 7261          _tempera
-00012bc0: 7475 7265 7320 3d20 6e70 2e61 7261 6e67  tures = np.arang
-00012bd0: 6528 302c 2031 3030 312c 2031 302c 2064  e(0, 1001, 10, d
-00012be0: 7479 7065 3d22 646f 7562 6c65 2229 0a20  type="double"). 
-00012bf0: 2020 2020 2020 2020 2020 2065 6c73 653a             else:
-00012c00: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00012c10: 205f 7465 6d70 6572 6174 7572 6573 203d   _temperatures =
-00012c20: 2074 656d 7065 7261 7475 7265 730a 2020   temperatures.  
-00012c30: 2020 2020 2020 2020 2020 7365 6c66 2e5f            self._
-00012c40: 7468 6572 6d61 6c5f 636f 6e64 7563 7469  thermal_conducti
-00012c50: 7669 7479 203d 2067 6574 5f74 6865 726d  vity = get_therm
-00012c60: 616c 5f63 6f6e 6475 6374 6976 6974 795f  al_conductivity_
-00012c70: 5254 4128 0a20 2020 2020 2020 2020 2020  RTA(.           
-00012c80: 2020 2020 2073 656c 662e 5f69 6e74 6572       self._inter
-00012c90: 6163 7469 6f6e 2c0a 2020 2020 2020 2020  action,.        
-00012ca0: 2020 2020 2020 2020 7465 6d70 6572 6174          temperat
-00012cb0: 7572 6573 3d5f 7465 6d70 6572 6174 7572  ures=_temperatur
-00012cc0: 6573 2c0a 2020 2020 2020 2020 2020 2020  es,.            
-00012cd0: 2020 2020 7369 676d 6173 3d73 656c 662e      sigmas=self.
-00012ce0: 5f73 6967 6d61 732c 0a20 2020 2020 2020  _sigmas,.       
-00012cf0: 2020 2020 2020 2020 2073 6967 6d61 5f63           sigma_c
-00012d00: 7574 6f66 663d 7365 6c66 2e5f 7369 676d  utoff=self._sigm
-00012d10: 615f 6375 746f 6666 2c0a 2020 2020 2020  a_cutoff,.      
-00012d20: 2020 2020 2020 2020 2020 6973 5f69 736f            is_iso
-00012d30: 746f 7065 3d69 735f 6973 6f74 6f70 652c  tope=is_isotope,
-00012d40: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00012d50: 206d 6173 735f 7661 7269 616e 6365 733d   mass_variances=
-00012d60: 6d61 7373 5f76 6172 6961 6e63 6573 2c0a  mass_variances,.
-00012d70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012d80: 6772 6964 5f70 6f69 6e74 733d 6772 6964  grid_points=grid
-00012d90: 5f70 6f69 6e74 732c 0a20 2020 2020 2020  _points,.       
-00012da0: 2020 2020 2020 2020 2062 6f75 6e64 6172           boundar
-00012db0: 795f 6d66 703d 626f 756e 6461 7279 5f6d  y_mfp=boundary_m
-00012dc0: 6670 2c0a 2020 2020 2020 2020 2020 2020  fp,.            
-00012dd0: 2020 2020 7573 655f 6176 655f 7070 3d75      use_ave_pp=u
-00012de0: 7365 5f61 7665 5f70 702c 0a20 2020 2020  se_ave_pp,.     
-00012df0: 2020 2020 2020 2020 2020 2069 735f 6b61             is_ka
-00012e00: 7070 615f 7374 6172 3d69 735f 6b61 7070  ppa_star=is_kapp
-00012e10: 615f 7374 6172 2c0a 2020 2020 2020 2020  a_star,.        
-00012e20: 2020 2020 2020 2020 6776 5f64 656c 7461          gv_delta
-00012e30: 5f71 3d67 765f 6465 6c74 615f 712c 0a20  _q=gv_delta_q,. 
-00012e40: 2020 2020 2020 2020 2020 2020 2020 2069                 i
-00012e50: 735f 6675 6c6c 5f70 703d 6973 5f66 756c  s_full_pp=is_ful
-00012e60: 6c5f 7070 2c0a 2020 2020 2020 2020 2020  l_pp,.          
-00012e70: 2020 2020 2020 6973 5f4e 5f55 3d69 735f        is_N_U=is_
-00012e80: 4e5f 552c 0a20 2020 2020 2020 2020 2020  N_U,.           
-00012e90: 2020 2020 2063 6f6e 6475 6374 6976 6974       conductivit
-00012ea0: 795f 7479 7065 3d63 6f6e 6475 6374 6976  y_type=conductiv
-00012eb0: 6974 795f 7479 7065 2c0a 2020 2020 2020  ity_type,.      
-00012ec0: 2020 2020 2020 2020 2020 7772 6974 655f            write_
-00012ed0: 6761 6d6d 613d 7772 6974 655f 6761 6d6d  gamma=write_gamm
-00012ee0: 612c 0a20 2020 2020 2020 2020 2020 2020  a,.             
-00012ef0: 2020 2072 6561 645f 6761 6d6d 613d 7265     read_gamma=re
-00012f00: 6164 5f67 616d 6d61 2c0a 2020 2020 2020  ad_gamma,.      
-00012f10: 2020 2020 2020 2020 2020 7772 6974 655f            write_
-00012f20: 6b61 7070 613d 7772 6974 655f 6b61 7070  kappa=write_kapp
-00012f30: 612c 0a20 2020 2020 2020 2020 2020 2020  a,.             
-00012f40: 2020 2077 7269 7465 5f70 703d 7772 6974     write_pp=writ
-00012f50: 655f 7070 2c0a 2020 2020 2020 2020 2020  e_pp,.          
-00012f60: 2020 2020 2020 7265 6164 5f70 703d 7265        read_pp=re
-00012f70: 6164 5f70 702c 0a20 2020 2020 2020 2020  ad_pp,.         
-00012f80: 2020 2020 2020 2077 7269 7465 5f67 616d         write_gam
-00012f90: 6d61 5f64 6574 6169 6c3d 7772 6974 655f  ma_detail=write_
-00012fa0: 6761 6d6d 615f 6465 7461 696c 2c0a 2020  gamma_detail,.  
-00012fb0: 2020 2020 2020 2020 2020 2020 2020 636f                co
-00012fc0: 6d70 7265 7373 696f 6e3d 636f 6d70 7265  mpression=compre
-00012fd0: 7373 696f 6e2c 0a20 2020 2020 2020 2020  ssion,.         
-00012fe0: 2020 2020 2020 2069 6e70 7574 5f66 696c         input_fil
-00012ff0: 656e 616d 653d 696e 7075 745f 6669 6c65  ename=input_file
-00013000: 6e61 6d65 2c0a 2020 2020 2020 2020 2020  name,.          
-00013010: 2020 2020 2020 6f75 7470 7574 5f66 696c        output_fil
-00013020: 656e 616d 653d 6f75 7470 7574 5f66 696c  ename=output_fil
-00013030: 656e 616d 652c 0a20 2020 2020 2020 2020  ename,.         
-00013040: 2020 2020 2020 206c 6f67 5f6c 6576 656c         log_level
-00013050: 3d73 656c 662e 5f6c 6f67 5f6c 6576 656c  =self._log_level
-00013060: 2c0a 2020 2020 2020 2020 2020 2020 290a  ,.            ).
-00013070: 0a20 2020 2064 6566 2073 6176 6528 7365  .    def save(se
-00013080: 6c66 2c20 6669 6c65 6e61 6d65 3d22 7068  lf, filename="ph
-00013090: 6f6e 6f33 7079 5f70 6172 616d 732e 7961  ono3py_params.ya
-000130a0: 6d6c 222c 2073 6574 7469 6e67 733d 4e6f  ml", settings=No
-000130b0: 6e65 293a 0a20 2020 2020 2020 2022 2222  ne):.        """
-000130c0: 5361 7665 2070 6172 616d 6574 6572 7320  Save parameters 
-000130d0: 696e 2050 686f 6e6f 3370 7920 696e 7374  in Phono3py inst
-000130e0: 616e 7473 2069 6e74 6f20 6669 6c65 2e0a  ants into file..
-000130f0: 0a20 2020 2020 2020 2050 6172 616d 6574  .        Paramet
-00013100: 6572 730a 2020 2020 2020 2020 2d2d 2d2d  ers.        ----
-00013110: 2d2d 2d2d 2d2d 0a20 2020 2020 2020 2066  ------.        f
-00013120: 696c 656e 616d 653a 2073 7472 2c20 6f70  ilename: str, op
-00013130: 7469 6f6e 616c 0a20 2020 2020 2020 2020  tional.         
-00013140: 2020 2046 696c 6520 6e61 6d65 2e20 4465     File name. De
-00013150: 6661 756c 7420 6973 2022 7068 6f6e 6f33  fault is "phono3
-00013160: 7079 5f70 6172 616d 732e 7961 6d6c 220a  py_params.yaml".
-00013170: 2020 2020 2020 2020 7365 7474 696e 6773          settings
-00013180: 3a20 6469 6374 2c20 6f70 7469 6f6e 616c  : dict, optional
-00013190: 0a20 2020 2020 2020 2020 2020 2049 7420  .            It 
-000131a0: 6973 2064 6573 6372 6962 6564 2077 6869  is described whi
-000131b0: 6368 2070 6172 616d 6574 6572 7320 6172  ch parameters ar
-000131c0: 6520 7772 6974 7465 6e20 6f75 742e 204f  e written out. O
-000131d0: 6e6c 790a 2020 2020 2020 2020 2020 2020  nly.            
-000131e0: 7468 6520 7365 7474 696e 6773 2065 7870  the settings exp
-000131f0: 6563 7465 6420 746f 2062 6520 7570 6461  ected to be upda
-00013200: 7465 6420 6672 6f6d 2074 6865 2066 6f6c  ted from the fol
-00013210: 6c6f 7769 6e67 0a20 2020 2020 2020 2020  lowing.         
-00013220: 2020 2064 6566 6175 6c74 2073 6574 7469     default setti
-00013230: 6e67 7320 6172 6520 6e65 6564 6564 2074  ngs are needed t
-00013240: 6f20 6265 2073 6574 2069 6e20 7468 6520  o be set in the 
-00013250: 6469 6374 696f 6e61 7279 2e0a 2020 2020  dictionary..    
-00013260: 2020 2020 2020 2020 5468 6520 706f 7373          The poss
-00013270: 6962 6c65 2070 6172 616d 6574 6572 7320  ible parameters 
-00013280: 616e 6420 7468 6569 7220 6465 6661 756c  and their defaul
-00013290: 7420 7365 7474 696e 6773 2061 7265 3a0a  t settings are:.
-000132a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000132b0: 7b27 666f 7263 655f 7365 7473 273a 2046  {'force_sets': F
-000132c0: 616c 7365 2c0a 2020 2020 2020 2020 2020  alse,.          
-000132d0: 2020 2020 2020 2027 6469 7370 6c61 6365         'displace
-000132e0: 6d65 6e74 7327 3a20 5472 7565 2c0a 2020  ments': True,.  
-000132f0: 2020 2020 2020 2020 2020 2020 2020 2027                 '
-00013300: 666f 7263 655f 636f 6e73 7461 6e74 7327  force_constants'
-00013310: 3a20 4661 6c73 652c 0a20 2020 2020 2020  : False,.       
-00013320: 2020 2020 2020 2020 2020 2762 6f72 6e5f            'born_
-00013330: 6566 6665 6374 6976 655f 6368 6172 6765  effective_charge
-00013340: 273a 2054 7275 652c 0a20 2020 2020 2020  ': True,.       
-00013350: 2020 2020 2020 2020 2020 2764 6965 6c65            'diele
-00013360: 6374 7269 635f 636f 6e73 7461 6e74 273a  ctric_constant':
-00013370: 2054 7275 657d 0a0a 2020 2020 2020 2020   True}..        
-00013380: 2222 220a 2020 2020 2020 2020 7068 3370  """.        ph3p
-00013390: 795f 7961 6d6c 203d 2050 686f 6e6f 3370  y_yaml = Phono3p
-000133a0: 7959 616d 6c28 7365 7474 696e 6773 3d73  yYaml(settings=s
-000133b0: 6574 7469 6e67 7329 0a20 2020 2020 2020  ettings).       
-000133c0: 2070 6833 7079 5f79 616d 6c2e 7365 745f   ph3py_yaml.set_
-000133d0: 7068 6f6e 6f6e 5f69 6e66 6f28 7365 6c66  phonon_info(self
-000133e0: 290a 2020 2020 2020 2020 7769 7468 206f  ).        with o
-000133f0: 7065 6e28 6669 6c65 6e61 6d65 2c20 2277  pen(filename, "w
-00013400: 2229 2061 7320 773a 0a20 2020 2020 2020  ") as w:.       
-00013410: 2020 2020 2077 2e77 7269 7465 2873 7472       w.write(str
-00013420: 2870 6833 7079 5f79 616d 6c29 290a 0a20  (ph3py_yaml)).. 
-00013430: 2020 2023 2323 2323 2323 2323 2323 2323     #############
-00013440: 2323 2323 2323 0a20 2020 2023 2070 7269  ######.    # pri
-00013450: 7661 7465 206d 6574 686f 6473 2023 0a20  vate methods #. 
-00013460: 2020 2023 2323 2323 2323 2323 2323 2323     #############
-00013470: 2323 2323 2323 0a20 2020 2064 6566 205f  ######.    def _
-00013480: 7365 6172 6368 5f73 796d 6d65 7472 7928  search_symmetry(
-00013490: 7365 6c66 293a 0a20 2020 2020 2020 2073  self):.        s
-000134a0: 656c 662e 5f73 796d 6d65 7472 7920 3d20  elf._symmetry = 
-000134b0: 5379 6d6d 6574 7279 2873 656c 662e 5f73  Symmetry(self._s
-000134c0: 7570 6572 6365 6c6c 2c20 7365 6c66 2e5f  upercell, self._
-000134d0: 7379 6d70 7265 632c 2073 656c 662e 5f69  symprec, self._i
-000134e0: 735f 7379 6d6d 6574 7279 290a 0a20 2020  s_symmetry)..   
-000134f0: 2064 6566 205f 7365 6172 6368 5f70 7269   def _search_pri
-00013500: 6d69 7469 7665 5f73 796d 6d65 7472 7928  mitive_symmetry(
-00013510: 7365 6c66 293a 0a20 2020 2020 2020 2073  self):.        s
-00013520: 656c 662e 5f70 7269 6d69 7469 7665 5f73  elf._primitive_s
-00013530: 796d 6d65 7472 7920 3d20 5379 6d6d 6574  ymmetry = Symmet
-00013540: 7279 280a 2020 2020 2020 2020 2020 2020  ry(.            
-00013550: 7365 6c66 2e5f 7072 696d 6974 6976 652c  self._primitive,
-00013560: 2073 656c 662e 5f73 796d 7072 6563 2c20   self._symprec, 
-00013570: 7365 6c66 2e5f 6973 5f73 796d 6d65 7472  self._is_symmetr
-00013580: 790a 2020 2020 2020 2020 290a 2020 2020  y.        ).    
-00013590: 2020 2020 6966 206c 656e 2873 656c 662e      if len(self.
-000135a0: 5f73 796d 6d65 7472 792e 706f 696e 7467  _symmetry.pointg
-000135b0: 726f 7570 5f6f 7065 7261 7469 6f6e 7329  roup_operations)
-000135c0: 2021 3d20 6c65 6e28 0a20 2020 2020 2020   != len(.       
-000135d0: 2020 2020 2073 656c 662e 5f70 7269 6d69       self._primi
-000135e0: 7469 7665 5f73 796d 6d65 7472 792e 706f  tive_symmetry.po
-000135f0: 696e 7467 726f 7570 5f6f 7065 7261 7469  intgroup_operati
-00013600: 6f6e 730a 2020 2020 2020 2020 293a 2020  ons.        ):  
-00013610: 2320 6e6f 7161 2045 3132 390a 2020 2020  # noqa E129.    
-00013620: 2020 2020 2020 2020 7072 696e 7428 0a20          print(. 
-00013630: 2020 2020 2020 2020 2020 2020 2020 2022                 "
-00013640: 5761 726e 696e 673a 2070 6f69 6e74 2067  Warning: point g
-00013650: 726f 7570 2073 796d 6d65 7472 6965 7320  roup symmetries 
-00013660: 6f66 2073 7570 6572 6365 6c6c 2061 6e64  of supercell and
-00013670: 2070 7269 6d69 7469 7665 220a 2020 2020   primitive".    
-00013680: 2020 2020 2020 2020 2020 2020 2263 656c              "cel
-00013690: 6c20 6172 6520 6469 6666 6572 656e 742e  l are different.
-000136a0: 220a 2020 2020 2020 2020 2020 2020 290a  ".            ).
-000136b0: 0a20 2020 2064 6566 205f 7365 6172 6368  .    def _search
-000136c0: 5f70 686f 6e6f 6e5f 7375 7065 7263 656c  _phonon_supercel
-000136d0: 6c5f 7379 6d6d 6574 7279 2873 656c 6629  l_symmetry(self)
-000136e0: 3a0a 2020 2020 2020 2020 6966 2073 656c  :.        if sel
-000136f0: 662e 5f70 686f 6e6f 6e5f 7375 7065 7263  f._phonon_superc
-00013700: 656c 6c5f 6d61 7472 6978 2069 7320 4e6f  ell_matrix is No
-00013710: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
-00013720: 7365 6c66 2e5f 7068 6f6e 6f6e 5f73 7570  self._phonon_sup
-00013730: 6572 6365 6c6c 5f73 796d 6d65 7472 7920  ercell_symmetry 
-00013740: 3d20 7365 6c66 2e5f 7379 6d6d 6574 7279  = self._symmetry
-00013750: 0a20 2020 2020 2020 2065 6c73 653a 0a20  .        else:. 
-00013760: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-00013770: 5f70 686f 6e6f 6e5f 7375 7065 7263 656c  _phonon_supercel
-00013780: 6c5f 7379 6d6d 6574 7279 203d 2053 796d  l_symmetry = Sym
-00013790: 6d65 7472 7928 0a20 2020 2020 2020 2020  metry(.         
-000137a0: 2020 2020 2020 2073 656c 662e 5f70 686f         self._pho
-000137b0: 6e6f 6e5f 7375 7065 7263 656c 6c2c 2073  non_supercell, s
-000137c0: 656c 662e 5f73 796d 7072 6563 2c20 7365  elf._symprec, se
-000137d0: 6c66 2e5f 6973 5f73 796d 6d65 7472 790a  lf._is_symmetry.
-000137e0: 2020 2020 2020 2020 2020 2020 290a 0a20              ).. 
-000137f0: 2020 2064 6566 205f 6275 696c 645f 7375     def _build_su
-00013800: 7065 7263 656c 6c28 7365 6c66 293a 0a20  percell(self):. 
-00013810: 2020 2020 2020 2073 656c 662e 5f73 7570         self._sup
-00013820: 6572 6365 6c6c 203d 2067 6574 5f73 7570  ercell = get_sup
-00013830: 6572 6365 6c6c 280a 2020 2020 2020 2020  ercell(.        
-00013840: 2020 2020 7365 6c66 2e5f 756e 6974 6365      self._unitce
-00013850: 6c6c 2c20 7365 6c66 2e5f 7375 7065 7263  ll, self._superc
-00013860: 656c 6c5f 6d61 7472 6978 2c20 7365 6c66  ell_matrix, self
-00013870: 2e5f 7379 6d70 7265 630a 2020 2020 2020  ._symprec.      
-00013880: 2020 290a 0a20 2020 2064 6566 205f 6275    )..    def _bu
-00013890: 696c 645f 7072 696d 6974 6976 655f 6365  ild_primitive_ce
-000138a0: 6c6c 2873 656c 6629 3a0a 2020 2020 2020  ll(self):.      
-000138b0: 2020 2222 2243 7265 6174 6520 7072 696d    """Create prim
-000138c0: 6974 6976 6520 6365 6c6c 2e0a 0a20 2020  itive cell...   
-000138d0: 2020 2020 2070 7269 6d69 7469 7665 5f6d       primitive_m
-000138e0: 6174 7269 783a 0a20 2020 2020 2020 2020  atrix:.         
-000138f0: 2052 656c 6174 6976 6520 6178 6573 206f   Relative axes o
-00013900: 6620 7072 696d 6974 6976 6520 6365 6c6c  f primitive cell
-00013910: 2074 6f20 7468 6520 696e 7075 7420 756e   to the input un
-00013920: 6974 2063 656c 6c2e 0a20 2020 2020 2020  it cell..       
-00013930: 2020 2052 656c 6174 6976 6520 6178 6573     Relative axes
-00013940: 2074 6f20 7468 6520 7375 7065 7263 656c   to the supercel
-00013950: 6c20 6973 2063 616c 6375 6c61 7465 6420  l is calculated 
-00013960: 6279 3a0a 2020 2020 2020 2020 2020 2020  by:.            
-00013970: 2073 7570 6572 6365 6c6c 5f6d 6174 7269   supercell_matri
-00013980: 785e 2d31 202a 2070 7269 6d69 7469 7665  x^-1 * primitive
-00013990: 5f6d 6174 7269 780a 2020 2020 2020 2020  _matrix.        
-000139a0: 2020 5468 6572 6566 6f72 6520 7072 696d    Therefore prim
-000139b0: 6974 6976 6520 6365 6c6c 206c 6174 7469  itive cell latti
-000139c0: 6365 2069 7320 6669 6e61 6c6c 7920 6361  ce is finally ca
-000139d0: 6c63 756c 6174 6564 2062 793a 0a20 2020  lculated by:.   
-000139e0: 2020 2020 2020 2020 2020 2873 7570 6572            (super
-000139f0: 6365 6c6c 5f6c 6174 7469 6365 202a 2028  cell_lattice * (
-00013a00: 7375 7065 7263 656c 6c5f 6d61 7472 6978  supercell_matrix
-00013a10: 295e 2d31 202a 2070 7269 6d69 7469 7665  )^-1 * primitive
-00013a20: 5f6d 6174 7269 7829 5e54 0a0a 2020 2020  _matrix)^T..    
-00013a30: 2020 2020 2222 220a 2020 2020 2020 2020      """.        
-00013a40: 7365 6c66 2e5f 7072 696d 6974 6976 6520  self._primitive 
-00013a50: 3d20 7365 6c66 2e5f 6765 745f 7072 696d  = self._get_prim
-00013a60: 6974 6976 655f 6365 6c6c 280a 2020 2020  itive_cell(.    
-00013a70: 2020 2020 2020 2020 7365 6c66 2e5f 7375          self._su
-00013a80: 7065 7263 656c 6c2c 2073 656c 662e 5f73  percell, self._s
-00013a90: 7570 6572 6365 6c6c 5f6d 6174 7269 782c  upercell_matrix,
-00013aa0: 2073 656c 662e 5f70 7269 6d69 7469 7665   self._primitive
-00013ab0: 5f6d 6174 7269 780a 2020 2020 2020 2020  _matrix.        
-00013ac0: 290a 0a20 2020 2064 6566 205f 6275 696c  )..    def _buil
-00013ad0: 645f 7068 6f6e 6f6e 5f73 7570 6572 6365  d_phonon_superce
-00013ae0: 6c6c 2873 656c 6629 3a0a 2020 2020 2020  ll(self):.      
-00013af0: 2020 2222 2243 7265 6174 6520 7068 6f6e    """Create phon
-00013b00: 6f6e 2073 7570 6572 6365 6c6c 2066 6f72  on supercell for
-00013b10: 2066 6332 2e0a 0a20 2020 2020 2020 2070   fc2...        p
-00013b20: 686f 6e6f 6e5f 7375 7065 7263 656c 6c3a  honon_supercell:
-00013b30: 0a20 2020 2020 2020 2020 2054 6869 7320  .          This 
-00013b40: 7375 7065 7263 656c 6c20 6973 2075 7365  supercell is use
-00013b50: 6420 666f 7220 6861 726d 6f6e 6963 2070  d for harmonic p
-00013b60: 686f 6e6f 6e73 2028 6672 6571 7565 6e63  honons (frequenc
-00013b70: 6965 732c 0a20 2020 2020 2020 2020 2065  ies,.          e
-00013b80: 6967 656e 7665 6374 6f72 732c 2067 726f  igenvectors, gro
-00013b90: 7570 2076 656c 6f63 6974 6965 732c 202e  up velocities, .
-00013ba0: 2e2e 290a 2020 2020 2020 2020 7068 6f6e  ..).        phon
-00013bb0: 6f6e 5f73 7570 6572 6365 6c6c 5f6d 6174  on_supercell_mat
-00013bc0: 7269 783a 0a20 2020 2020 2020 2020 2044  rix:.          D
-00013bd0: 6966 6665 7265 6e74 2073 7570 6572 6365  ifferent superce
-00013be0: 6c6c 2073 697a 6520 6361 6e20 6265 2073  ll size can be s
-00013bf0: 7065 6369 6669 6564 2e0a 0a20 2020 2020  pecified...     
-00013c00: 2020 2022 2222 0a20 2020 2020 2020 2069     """.        i
-00013c10: 6620 7365 6c66 2e5f 7068 6f6e 6f6e 5f73  f self._phonon_s
-00013c20: 7570 6572 6365 6c6c 5f6d 6174 7269 7820  upercell_matrix 
-00013c30: 6973 204e 6f6e 653a 0a20 2020 2020 2020  is None:.       
-00013c40: 2020 2020 2073 656c 662e 5f70 686f 6e6f       self._phono
-00013c50: 6e5f 7375 7065 7263 656c 6c20 3d20 7365  n_supercell = se
-00013c60: 6c66 2e5f 7375 7065 7263 656c 6c0a 2020  lf._supercell.  
-00013c70: 2020 2020 2020 656c 7365 3a0a 2020 2020        else:.    
-00013c80: 2020 2020 2020 2020 7365 6c66 2e5f 7068          self._ph
-00013c90: 6f6e 6f6e 5f73 7570 6572 6365 6c6c 203d  onon_supercell =
-00013ca0: 2067 6574 5f73 7570 6572 6365 6c6c 280a   get_supercell(.
-00013cb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013cc0: 7365 6c66 2e5f 756e 6974 6365 6c6c 2c20  self._unitcell, 
-00013cd0: 7365 6c66 2e5f 7068 6f6e 6f6e 5f73 7570  self._phonon_sup
-00013ce0: 6572 6365 6c6c 5f6d 6174 7269 782c 2073  ercell_matrix, s
-00013cf0: 656c 662e 5f73 796d 7072 6563 0a20 2020  elf._symprec.   
-00013d00: 2020 2020 2020 2020 2029 0a0a 2020 2020           )..    
-00013d10: 6465 6620 5f62 7569 6c64 5f70 686f 6e6f  def _build_phono
-00013d20: 6e5f 7072 696d 6974 6976 655f 6365 6c6c  n_primitive_cell
-00013d30: 2873 656c 6629 3a0a 2020 2020 2020 2020  (self):.        
-00013d40: 6966 2073 656c 662e 5f70 686f 6e6f 6e5f  if self._phonon_
-00013d50: 7375 7065 7263 656c 6c5f 6d61 7472 6978  supercell_matrix
-00013d60: 2069 7320 4e6f 6e65 3a0a 2020 2020 2020   is None:.      
-00013d70: 2020 2020 2020 7365 6c66 2e5f 7068 6f6e        self._phon
-00013d80: 6f6e 5f70 7269 6d69 7469 7665 203d 2073  on_primitive = s
-00013d90: 656c 662e 5f70 7269 6d69 7469 7665 0a20  elf._primitive. 
-00013da0: 2020 2020 2020 2065 6c73 653a 0a20 2020         else:.   
-00013db0: 2020 2020 2020 2020 2073 656c 662e 5f70           self._p
-00013dc0: 686f 6e6f 6e5f 7072 696d 6974 6976 6520  honon_primitive 
-00013dd0: 3d20 7365 6c66 2e5f 6765 745f 7072 696d  = self._get_prim
-00013de0: 6974 6976 655f 6365 6c6c 280a 2020 2020  itive_cell(.    
-00013df0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-00013e00: 2e5f 7068 6f6e 6f6e 5f73 7570 6572 6365  ._phonon_superce
-00013e10: 6c6c 2c0a 2020 2020 2020 2020 2020 2020  ll,.            
-00013e20: 2020 2020 7365 6c66 2e5f 7068 6f6e 6f6e      self._phonon
-00013e30: 5f73 7570 6572 6365 6c6c 5f6d 6174 7269  _supercell_matri
-00013e40: 782c 0a20 2020 2020 2020 2020 2020 2020  x,.             
-00013e50: 2020 2073 656c 662e 5f70 7269 6d69 7469     self._primiti
-00013e60: 7665 5f6d 6174 7269 782c 0a20 2020 2020  ve_matrix,.     
-00013e70: 2020 2020 2020 2029 0a20 2020 2020 2020         ).       
-00013e80: 2020 2020 2069 6620 280a 2020 2020 2020       if (.      
-00013e90: 2020 2020 2020 2020 2020 7365 6c66 2e5f            self._
-00013ea0: 7072 696d 6974 6976 6520 6973 206e 6f74  primitive is not
-00013eb0: 204e 6f6e 650a 2020 2020 2020 2020 2020   None.          
-00013ec0: 2020 2020 2020 616e 6420 2873 656c 662e        and (self.
-00013ed0: 5f70 7269 6d69 7469 7665 2e6e 756d 6265  _primitive.numbe
-00013ee0: 7273 2021 3d20 7365 6c66 2e5f 7068 6f6e  rs != self._phon
-00013ef0: 6f6e 5f70 7269 6d69 7469 7665 2e6e 756d  on_primitive.num
-00013f00: 6265 7273 292e 616e 7928 290a 2020 2020  bers).any().    
-00013f10: 2020 2020 2020 2020 293a 0a20 2020 2020          ):.     
-00013f20: 2020 2020 2020 2020 2020 2070 7269 6e74             print
-00013f30: 2822 2050 7269 6d69 7469 7665 2063 656c  (" Primitive cel
-00013f40: 6c73 2066 6f72 2066 6332 2061 6e64 2066  ls for fc2 and f
-00013f50: 6333 2063 616e 2062 6520 6469 6666 6572  c3 can be differ
-00013f60: 656e 742e 2229 0a20 2020 2020 2020 2020  ent.").         
-00013f70: 2020 2020 2020 2072 6169 7365 2052 756e         raise Run
-00013f80: 7469 6d65 4572 726f 720a 0a20 2020 2064  timeError..    d
-00013f90: 6566 205f 6275 696c 645f 7068 6f6e 6f6e  ef _build_phonon
-00013fa0: 5f73 7570 6572 6365 6c6c 735f 7769 7468  _supercells_with
-00013fb0: 5f64 6973 706c 6163 656d 656e 7473 280a  _displacements(.
-00013fc0: 2020 2020 2020 2020 7365 6c66 2c20 7375          self, su
-00013fd0: 7065 7263 656c 6c3a 2050 686f 6e6f 7079  percell: Phonopy
-00013fe0: 4174 6f6d 732c 2064 6973 706c 6163 656d  Atoms, displacem
-00013ff0: 656e 745f 6461 7461 7365 740a 2020 2020  ent_dataset.    
-00014000: 293a 0a20 2020 2020 2020 2073 7570 6572  ):.        super
-00014010: 6365 6c6c 7320 3d20 5b5d 0a20 2020 2020  cells = [].     
-00014020: 2020 206d 6167 6d6f 6d73 203d 2073 7570     magmoms = sup
-00014030: 6572 6365 6c6c 2e6d 6167 6e65 7469 635f  ercell.magnetic_
-00014040: 6d6f 6d65 6e74 730a 2020 2020 2020 2020  moments.        
-00014050: 6d61 7373 6573 203d 2073 7570 6572 6365  masses = superce
-00014060: 6c6c 2e6d 6173 7365 730a 2020 2020 2020  ll.masses.      
-00014070: 2020 6e75 6d62 6572 7320 3d20 7375 7065    numbers = supe
-00014080: 7263 656c 6c2e 6e75 6d62 6572 730a 2020  rcell.numbers.  
-00014090: 2020 2020 2020 6c61 7474 6963 6520 3d20        lattice = 
-000140a0: 7375 7065 7263 656c 6c2e 6365 6c6c 0a0a  supercell.cell..
-000140b0: 2020 2020 2020 2020 666f 7220 6469 7370          for disp
-000140c0: 3120 696e 2064 6973 706c 6163 656d 656e  1 in displacemen
-000140d0: 745f 6461 7461 7365 745b 2266 6972 7374  t_dataset["first
-000140e0: 5f61 746f 6d73 225d 3a0a 2020 2020 2020  _atoms"]:.      
-000140f0: 2020 2020 2020 6469 7370 5f63 6172 7431        disp_cart1
-00014100: 203d 2064 6973 7031 5b22 6469 7370 6c61   = disp1["displa
-00014110: 6365 6d65 6e74 225d 0a20 2020 2020 2020  cement"].       
-00014120: 2020 2020 2070 6f73 6974 696f 6e73 203d       positions =
-00014130: 2073 7570 6572 6365 6c6c 2e70 6f73 6974   supercell.posit
-00014140: 696f 6e73 0a20 2020 2020 2020 2020 2020  ions.           
-00014150: 2070 6f73 6974 696f 6e73 5b64 6973 7031   positions[disp1
-00014160: 5b22 6e75 6d62 6572 225d 5d20 2b3d 2064  ["number"]] += d
-00014170: 6973 705f 6361 7274 310a 2020 2020 2020  isp_cart1.      
-00014180: 2020 2020 2020 7375 7065 7263 656c 6c73        supercells
-00014190: 2e61 7070 656e 6428 0a20 2020 2020 2020  .append(.       
-000141a0: 2020 2020 2020 2020 2050 686f 6e6f 7079           Phonopy
-000141b0: 4174 6f6d 7328 0a20 2020 2020 2020 2020  Atoms(.         
-000141c0: 2020 2020 2020 2020 2020 206e 756d 6265             numbe
-000141d0: 7273 3d6e 756d 6265 7273 2c0a 2020 2020  rs=numbers,.    
-000141e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000141f0: 6d61 7373 6573 3d6d 6173 7365 732c 0a20  masses=masses,. 
-00014200: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014210: 2020 206d 6167 6e65 7469 635f 6d6f 6d65     magnetic_mome
-00014220: 6e74 733d 6d61 676d 6f6d 732c 0a20 2020  nts=magmoms,.   
-00014230: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014240: 2070 6f73 6974 696f 6e73 3d70 6f73 6974   positions=posit
-00014250: 696f 6e73 2c0a 2020 2020 2020 2020 2020  ions,.          
-00014260: 2020 2020 2020 2020 2020 6365 6c6c 3d6c            cell=l
-00014270: 6174 7469 6365 2c0a 2020 2020 2020 2020  attice,.        
-00014280: 2020 2020 2020 2020 290a 2020 2020 2020          ).      
-00014290: 2020 2020 2020 290a 0a20 2020 2020 2020        )..       
-000142a0: 2072 6574 7572 6e20 7375 7065 7263 656c   return supercel
-000142b0: 6c73 0a0a 2020 2020 6465 6620 5f62 7569  ls..    def _bui
-000142c0: 6c64 5f73 7570 6572 6365 6c6c 735f 7769  ld_supercells_wi
-000142d0: 7468 5f64 6973 706c 6163 656d 656e 7473  th_displacements
-000142e0: 2873 656c 6629 3a0a 2020 2020 2020 2020  (self):.        
-000142f0: 7375 7065 7263 656c 6c73 203d 205b 5d0a  supercells = [].
-00014300: 2020 2020 2020 2020 6d61 676d 6f6d 7320          magmoms 
-00014310: 3d20 7365 6c66 2e5f 7375 7065 7263 656c  = self._supercel
-00014320: 6c2e 6d61 676e 6574 6963 5f6d 6f6d 656e  l.magnetic_momen
-00014330: 7473 0a20 2020 2020 2020 206d 6173 7365  ts.        masse
-00014340: 7320 3d20 7365 6c66 2e5f 7375 7065 7263  s = self._superc
-00014350: 656c 6c2e 6d61 7373 6573 0a20 2020 2020  ell.masses.     
-00014360: 2020 206e 756d 6265 7273 203d 2073 656c     numbers = sel
-00014370: 662e 5f73 7570 6572 6365 6c6c 2e6e 756d  f._supercell.num
-00014380: 6265 7273 0a20 2020 2020 2020 206c 6174  bers.        lat
-00014390: 7469 6365 203d 2073 656c 662e 5f73 7570  tice = self._sup
-000143a0: 6572 6365 6c6c 2e63 656c 6c0a 0a20 2020  ercell.cell..   
-000143b0: 2020 2020 2073 7570 6572 6365 6c6c 7320       supercells 
-000143c0: 3d20 7365 6c66 2e5f 6275 696c 645f 7068  = self._build_ph
-000143d0: 6f6e 6f6e 5f73 7570 6572 6365 6c6c 735f  onon_supercells_
-000143e0: 7769 7468 5f64 6973 706c 6163 656d 656e  with_displacemen
-000143f0: 7473 280a 2020 2020 2020 2020 2020 2020  ts(.            
-00014400: 7365 6c66 2e5f 7375 7065 7263 656c 6c2c  self._supercell,
-00014410: 2073 656c 662e 5f64 6174 6173 6574 0a20   self._dataset. 
-00014420: 2020 2020 2020 2029 0a0a 2020 2020 2020         )..      
-00014430: 2020 666f 7220 6469 7370 3120 696e 2073    for disp1 in s
-00014440: 656c 662e 5f64 6174 6173 6574 5b22 6669  elf._dataset["fi
-00014450: 7273 745f 6174 6f6d 7322 5d3a 0a20 2020  rst_atoms"]:.   
-00014460: 2020 2020 2020 2020 2064 6973 705f 6361           disp_ca
-00014470: 7274 3120 3d20 6469 7370 315b 2264 6973  rt1 = disp1["dis
-00014480: 706c 6163 656d 656e 7422 5d0a 2020 2020  placement"].    
-00014490: 2020 2020 2020 2020 666f 7220 6469 7370          for disp
-000144a0: 3220 696e 2064 6973 7031 5b22 7365 636f  2 in disp1["seco
-000144b0: 6e64 5f61 746f 6d73 225d 3a0a 2020 2020  nd_atoms"]:.    
-000144c0: 2020 2020 2020 2020 2020 2020 6966 2022              if "
-000144d0: 696e 636c 7564 6564 2220 696e 2064 6973  included" in dis
-000144e0: 7032 3a0a 2020 2020 2020 2020 2020 2020  p2:.            
-000144f0: 2020 2020 2020 2020 696e 636c 7564 6564          included
-00014500: 203d 2064 6973 7032 5b22 696e 636c 7564   = disp2["includ
-00014510: 6564 225d 0a20 2020 2020 2020 2020 2020  ed"].           
-00014520: 2020 2020 2065 6c73 653a 0a20 2020 2020       else:.     
-00014530: 2020 2020 2020 2020 2020 2020 2020 2069                 i
-00014540: 6e63 6c75 6465 6420 3d20 5472 7565 0a20  ncluded = True. 
-00014550: 2020 2020 2020 2020 2020 2020 2020 2069                 i
-00014560: 6620 696e 636c 7564 6564 3a0a 2020 2020  f included:.    
-00014570: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014580: 706f 7369 7469 6f6e 7320 3d20 7365 6c66  positions = self
-00014590: 2e5f 7375 7065 7263 656c 6c2e 706f 7369  ._supercell.posi
-000145a0: 7469 6f6e 730a 2020 2020 2020 2020 2020  tions.          
-000145b0: 2020 2020 2020 2020 2020 706f 7369 7469            positi
-000145c0: 6f6e 735b 6469 7370 315b 226e 756d 6265  ons[disp1["numbe
-000145d0: 7222 5d5d 202b 3d20 6469 7370 5f63 6172  r"]] += disp_car
-000145e0: 7431 0a20 2020 2020 2020 2020 2020 2020  t1.             
-000145f0: 2020 2020 2020 2070 6f73 6974 696f 6e73         positions
-00014600: 5b64 6973 7032 5b22 6e75 6d62 6572 225d  [disp2["number"]
-00014610: 5d20 2b3d 2064 6973 7032 5b22 6469 7370  ] += disp2["disp
-00014620: 6c61 6365 6d65 6e74 225d 0a20 2020 2020  lacement"].     
-00014630: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-00014640: 7570 6572 6365 6c6c 732e 6170 7065 6e64  upercells.append
-00014650: 280a 2020 2020 2020 2020 2020 2020 2020  (.              
-00014660: 2020 2020 2020 2020 2020 5068 6f6e 6f70            Phonop
-00014670: 7941 746f 6d73 280a 2020 2020 2020 2020  yAtoms(.        
-00014680: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014690: 2020 2020 6e75 6d62 6572 733d 6e75 6d62      numbers=numb
-000146a0: 6572 732c 0a20 2020 2020 2020 2020 2020  ers,.           
-000146b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000146c0: 206d 6173 7365 733d 6d61 7373 6573 2c0a   masses=masses,.
+00004af0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004b00: 7061 6972 2064 6973 706c 6163 656d 656e  pair displacemen
+00004b10: 7473 2069 7320 696e 636c 7564 6564 2074  ts is included t
+00004b20: 6f20 636f 6d70 7574 650a 2020 2020 2020  o compute.      
+00004b30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004b40: 2020 2020 2020 2020 2020 2020 2066 6333               fc3
+00004b50: 206f 7220 6e6f 742c 0a20 2020 2020 2020   or not,.       
+00004b60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004b70: 2769 6427 3a20 6469 7370 6c61 6365 6d65  'id': displaceme
+00004b80: 6e74 2069 642e 2028 6e5f 6669 7273 745f  nt id. (n_first_
+00004b90: 6174 6f6d 7320 2b20 312c 202e 2e2e 290a  atoms + 1, ...).
+00004ba0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004bb0: 2020 2020 2020 2e2e 2e20 5d20 7d2c 202e        ... ] }, .
+00004bc0: 2e2e 205d 207d 0a20 2020 2020 2020 2020  .. ] }.         
+00004bd0: 2020 2054 7970 6520 322e 2041 6c6c 2061     Type 2. All a
+00004be0: 746f 6d69 6320 6469 7370 6c61 6365 6d65  tomic displaceme
+00004bf0: 6e74 7320 696e 2065 6163 6820 7375 7065  nts in each supe
+00004c00: 7263 656c 6c3a 0a20 2020 2020 2020 2020  rcell:.         
+00004c10: 2020 2020 2020 207b 2764 6973 706c 6163         {'displac
+00004c20: 656d 656e 7473 273a 206e 6461 7272 6179  ements': ndarray
+00004c30: 2c20 6474 7970 653d 2764 6f75 626c 6527  , dtype='double'
+00004c40: 2c20 6f72 6465 723d 2743 272c 0a20 2020  , order='C',.   
+00004c50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004c60: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+00004c70: 6861 7065 3d28 7375 7065 7263 656c 6c73  hape=(supercells
+00004c80: 2c20 6174 6f6d 7320 696e 2073 7570 6572  , atoms in super
+00004c90: 6365 6c6c 2c20 3329 2c0a 2020 2020 2020  cell, 3),.      
+00004ca0: 2020 2020 2020 2020 2020 2027 666f 7263             'forc
+00004cb0: 6573 273a 206e 6461 7272 6179 2c20 6474  es': ndarray, dt
+00004cc0: 7970 653d 2764 6f75 626c 6527 2c2c 206f  ype='double',, o
+00004cd0: 7264 6572 3d27 4327 2c0a 2020 2020 2020  rder='C',.      
+00004ce0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004cf0: 2020 2020 2020 2020 2020 2020 7368 6170              shap
+00004d00: 653d 2873 7570 6572 6365 6c6c 732c 2061  e=(supercells, a
+00004d10: 746f 6d73 2069 6e20 7375 7065 7263 656c  toms in supercel
+00004d20: 6c2c 2033 292c 0a20 2020 2020 2020 2020  l, 3),.         
+00004d30: 2020 2020 2020 2020 2773 7570 6572 6365          'superce
+00004d40: 6c6c 5f65 6e65 7267 6965 7327 3a20 6e64  ll_energies': nd
+00004d50: 6172 7261 792c 2064 7479 7065 3d27 646f  array, dtype='do
+00004d60: 7562 6c65 272c 0a20 2020 2020 2020 2020  uble',.         
+00004d70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004d80: 2020 2020 2020 2020 2073 6861 7065 3d28           shape=(
+00004d90: 7375 7065 7263 656c 6c73 2c29 7d0a 2020  supercells,)}.  
+00004da0: 2020 2020 2020 2020 2020 496e 2074 7970            In typ
+00004db0: 6520 322c 2064 6973 706c 6163 656d 656e  e 2, displacemen
+00004dc0: 7473 2061 6e64 2066 6f72 6365 7320 6361  ts and forces ca
+00004dd0: 6e20 6265 2067 6976 656e 2062 7920 6e75  n be given by nu
+00004de0: 6d70 7920 6172 7261 790a 2020 2020 2020  mpy array.      
+00004df0: 2020 2020 2020 7769 7468 2064 6966 6665        with diffe
+00004e00: 7265 6e74 2073 6861 7065 2062 7574 2074  rent shape but t
+00004e10: 6861 7420 6361 6e20 6265 2072 6573 6861  hat can be resha
+00004e20: 7065 6420 746f 0a20 2020 2020 2020 2020  ped to.         
+00004e30: 2020 2028 7375 7065 7263 656c 6c73 2c20     (supercells, 
+00004e40: 6e61 746f 6d2c 2033 292e 0a0a 2020 2020  natom, 3)...    
+00004e50: 2020 2020 2020 2020 496e 2061 6464 6974          In addit
+00004e60: 696f 6e2c 2027 6475 706c 6963 6174 6573  ion, 'duplicates
+00004e70: 2720 616e 6420 2763 7574 6f66 665f 6469  ' and 'cutoff_di
+00004e80: 7374 616e 6365 2720 6361 6e20 6578 6973  stance' can exis
+00004e90: 7420 696e 2074 6869 730a 2020 2020 2020  t in this.      
+00004ea0: 2020 2020 2020 6461 7461 7365 7420 696e        dataset in
+00004eb0: 2064 6973 706c 6163 656d 656e 7420 7061   displacement pa
+00004ec0: 6972 2067 656e 6572 6174 696f 6e2e 2027  ir generation. '
+00004ed0: 6475 706c 6963 6174 6573 2720 6769 7665  duplicates' give
+00004ee0: 730a 2020 2020 2020 2020 2020 2020 6475  s.            du
+00004ef0: 706c 6963 6174 6564 2073 7570 6572 6365  plicated superce
+00004f00: 6c6c 2069 6473 2061 7320 7061 6972 732e  ll ids as pairs.
+00004f10: 0a0a 2020 2020 2020 2020 2222 220a 2020  ..        """.  
+00004f20: 2020 2020 2020 7265 7475 726e 2073 656c        return sel
+00004f30: 662e 5f64 6174 6173 6574 0a0a 2020 2020  f._dataset..    
+00004f40: 4064 6174 6173 6574 2e73 6574 7465 720a  @dataset.setter.
+00004f50: 2020 2020 6465 6620 6461 7461 7365 7428      def dataset(
+00004f60: 7365 6c66 2c20 6461 7461 7365 7429 3a0a  self, dataset):.
+00004f70: 2020 2020 2020 2020 6966 2064 6174 6173          if datas
+00004f80: 6574 2069 7320 4e6f 6e65 3a0a 2020 2020  et is None:.    
+00004f90: 2020 2020 2020 2020 7365 6c66 2e5f 6461          self._da
+00004fa0: 7461 7365 7420 3d20 4e6f 6e65 0a20 2020  taset = None.   
+00004fb0: 2020 2020 2065 6c69 6620 2266 6972 7374       elif "first
+00004fc0: 5f61 746f 6d73 2220 696e 2064 6174 6173  _atoms" in datas
+00004fd0: 6574 3a0a 2020 2020 2020 2020 2020 2020  et:.            
+00004fe0: 7365 6c66 2e5f 6461 7461 7365 7420 3d20  self._dataset = 
+00004ff0: 636f 7079 2e64 6565 7063 6f70 7928 6461  copy.deepcopy(da
+00005000: 7461 7365 7429 0a20 2020 2020 2020 2065  taset).        e
+00005010: 6c69 6620 2264 6973 706c 6163 656d 656e  lif "displacemen
+00005020: 7473 2220 696e 2064 6174 6173 6574 3a0a  ts" in dataset:.
+00005030: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+00005040: 2e5f 6461 7461 7365 7420 3d20 7b7d 0a20  ._dataset = {}. 
+00005050: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+00005060: 6469 7370 6c61 6365 6d65 6e74 7320 3d20  displacements = 
+00005070: 6461 7461 7365 745b 2264 6973 706c 6163  dataset["displac
+00005080: 656d 656e 7473 225d 0a20 2020 2020 2020  ements"].       
+00005090: 2020 2020 2069 6620 2266 6f72 6365 7322       if "forces"
+000050a0: 2069 6e20 6461 7461 7365 743a 0a20 2020   in dataset:.   
+000050b0: 2020 2020 2020 2020 2020 2020 2073 656c               sel
+000050c0: 662e 666f 7263 6573 203d 2064 6174 6173  f.forces = datas
+000050d0: 6574 5b22 666f 7263 6573 225d 0a20 2020  et["forces"].   
+000050e0: 2020 2020 2020 2020 2069 6620 2273 7570           if "sup
+000050f0: 6572 6365 6c6c 5f65 6e65 7267 6965 7322  ercell_energies"
+00005100: 2069 6e20 6461 7461 7365 743a 0a20 2020   in dataset:.   
+00005110: 2020 2020 2020 2020 2020 2020 2073 656c               sel
+00005120: 662e 7375 7065 7263 656c 6c5f 656e 6572  f.supercell_ener
+00005130: 6769 6573 203d 2064 6174 6173 6574 5b22  gies = dataset["
+00005140: 7375 7065 7263 656c 6c5f 656e 6572 6769  supercell_energi
+00005150: 6573 225d 0a20 2020 2020 2020 2065 6c73  es"].        els
+00005160: 653a 0a20 2020 2020 2020 2020 2020 2072  e:.            r
+00005170: 6169 7365 2052 756e 7469 6d65 4572 726f  aise RuntimeErro
+00005180: 7228 2244 6174 6120 666f 726d 6174 206f  r("Data format o
+00005190: 6620 6461 7461 7365 7420 6973 2077 726f  f dataset is wro
+000051a0: 6e67 2e22 290a 0a20 2020 2020 2020 2073  ng.")..        s
+000051b0: 656c 662e 5f73 7570 6572 6365 6c6c 735f  elf._supercells_
+000051c0: 7769 7468 5f64 6973 706c 6163 656d 656e  with_displacemen
+000051d0: 7473 203d 204e 6f6e 650a 2020 2020 2020  ts = None.      
+000051e0: 2020 7365 6c66 2e5f 7068 6f6e 6f6e 5f73    self._phonon_s
+000051f0: 7570 6572 6365 6c6c 735f 7769 7468 5f64  upercells_with_d
+00005200: 6973 706c 6163 656d 656e 7473 203d 204e  isplacements = N
+00005210: 6f6e 650a 0a20 2020 2040 7072 6f70 6572  one..    @proper
+00005220: 7479 0a20 2020 2064 6566 2070 686f 6e6f  ty.    def phono
+00005230: 6e5f 6461 7461 7365 7428 7365 6c66 293a  n_dataset(self):
+00005240: 0a20 2020 2020 2020 2022 2222 5365 7474  .        """Sett
+00005250: 6572 2061 6e64 2067 6574 7465 7220 6f66  er and getter of
+00005260: 2064 6973 706c 6163 656d 656e 742d 666f   displacement-fo
+00005270: 7263 6520 6461 7461 7365 7420 666f 7220  rce dataset for 
+00005280: 6663 322e 0a0a 2020 2020 2020 2020 6469  fc2...        di
+00005290: 6374 0a20 2020 2020 2020 2020 2020 2044  ct.            D
+000052a0: 6973 706c 6163 656d 656e 7473 2069 6e20  isplacements in 
+000052b0: 7375 7065 7263 656c 6c73 2e20 5468 6572  supercells. Ther
+000052c0: 6520 6172 6520 7477 6f20 7479 7065 7320  e are two types 
+000052d0: 6f66 2066 6f72 6d61 7473 2e0a 2020 2020  of formats..    
+000052e0: 2020 2020 2020 2020 5479 7065 2031 2e20          Type 1. 
+000052f0: 5477 6f20 6174 6f6d 6963 2064 6973 706c  Two atomic displ
+00005300: 6163 656d 656e 7420 696e 2065 6163 6820  acement in each 
+00005310: 7375 7065 7263 656c 6c3a 0a20 2020 2020  supercell:.     
+00005320: 2020 2020 2020 2020 2020 207b 276e 6174             {'nat
+00005330: 6f6d 273a 206e 756d 6265 7220 6f66 2061  om': number of a
+00005340: 746f 6d73 2069 6e20 7375 7065 7263 656c  toms in supercel
+00005350: 6c2c 0a20 2020 2020 2020 2020 2020 2020  l,.             
+00005360: 2020 2020 2766 6972 7374 5f61 746f 6d73      'first_atoms
+00005370: 273a 205b 0a20 2020 2020 2020 2020 2020  ': [.           
+00005380: 2020 2020 2020 2020 7b27 6e75 6d62 6572          {'number
+00005390: 273a 2061 746f 6d20 696e 6465 7820 6f66  ': atom index of
+000053a0: 2066 6972 7374 2064 6973 706c 6163 6564   first displaced
+000053b0: 2061 746f 6d2c 0a20 2020 2020 2020 2020   atom,.         
+000053c0: 2020 2020 2020 2020 2020 2027 6469 7370             'disp
+000053d0: 6c61 6365 6d65 6e74 273a 2064 6973 706c  lacement': displ
+000053e0: 6163 656d 656e 7420 696e 2043 6172 7465  acement in Carte
+000053f0: 7369 616e 2063 6f6f 7264 696e 6174 6573  sian coordinates
+00005400: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+00005410: 2020 2020 2020 2766 6f72 6365 7327 3a20        'forces': 
+00005420: 666f 7263 6573 206f 6e20 6174 6f6d 7320  forces on atoms 
+00005430: 696e 2073 7570 6572 6365 6c6c 2c0a 2020  in supercell,.  
+00005440: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005450: 2020 2773 7570 6572 6365 6c6c 5f65 6e65    'supercell_ene
+00005460: 7267 7927 3a20 656e 6572 6779 206f 6620  rgy': energy of 
+00005470: 7375 7065 7263 656c 6c7d 2c20 2e2e 2e20  supercell}, ... 
+00005480: 5d7d 0a20 2020 2020 2020 2020 2020 2054  ]}.            T
+00005490: 7970 6520 322e 2041 6c6c 2061 746f 6d69  ype 2. All atomi
+000054a0: 6320 6469 7370 6c61 6365 6d65 6e74 7320  c displacements 
+000054b0: 696e 2065 6163 6820 7375 7065 7263 656c  in each supercel
+000054c0: 6c3a 0a20 2020 2020 2020 2020 2020 2020  l:.             
+000054d0: 2020 207b 2764 6973 706c 6163 656d 656e     {'displacemen
+000054e0: 7473 273a 206e 6461 7272 6179 2c20 6474  ts': ndarray, dt
+000054f0: 7970 653d 2764 6f75 626c 6527 2c20 6f72  ype='double', or
+00005500: 6465 723d 2743 272c 0a20 2020 2020 2020  der='C',.       
+00005510: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005520: 2020 2020 2020 2020 2020 2073 6861 7065             shape
+00005530: 3d28 7375 7065 7263 656c 6c73 2c20 6174  =(supercells, at
+00005540: 6f6d 7320 696e 2073 7570 6572 6365 6c6c  oms in supercell
+00005550: 2c20 3329 2c0a 2020 2020 2020 2020 2020  , 3),.          
+00005560: 2020 2020 2020 2027 666f 7263 6573 273a         'forces':
+00005570: 206e 6461 7272 6179 2c20 6474 7970 653d   ndarray, dtype=
+00005580: 2764 6f75 626c 6527 2c2c 206f 7264 6572  'double',, order
+00005590: 3d27 4327 2c0a 2020 2020 2020 2020 2020  ='C',.          
+000055a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000055b0: 2020 2020 2020 2020 7368 6170 653d 2873          shape=(s
+000055c0: 7570 6572 6365 6c6c 732c 2061 746f 6d73  upercells, atoms
+000055d0: 2069 6e20 7375 7065 7263 656c 6c2c 2033   in supercell, 3
+000055e0: 292c 0a20 2020 2020 2020 2020 2020 2020  ),.             
+000055f0: 2020 2020 2773 7570 6572 6365 6c6c 5f65      'supercell_e
+00005600: 6e65 7267 6965 7327 3a20 6e64 6172 7261  nergies': ndarra
+00005610: 792c 2064 7479 7065 3d27 646f 7562 6c65  y, dtype='double
+00005620: 272c 0a20 2020 2020 2020 2020 2020 2020  ',.             
+00005630: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005640: 2020 2020 2073 6861 7065 3d28 7375 7065       shape=(supe
+00005650: 7263 656c 6c73 2c29 7d0a 2020 2020 2020  rcells,)}.      
+00005660: 2020 2020 2020 496e 2074 7970 6520 322c        In type 2,
+00005670: 2064 6973 706c 6163 656d 656e 7473 2061   displacements a
+00005680: 6e64 2066 6f72 6365 7320 6361 6e20 6265  nd forces can be
+00005690: 2067 6976 656e 2062 7920 6e75 6d70 7920   given by numpy 
+000056a0: 6172 7261 790a 2020 2020 2020 2020 2020  array.          
+000056b0: 2020 7769 7468 2064 6966 6665 7265 6e74    with different
+000056c0: 2073 6861 7065 2062 7574 2074 6861 7420   shape but that 
+000056d0: 6361 6e20 6265 2072 6573 6861 7065 6420  can be reshaped 
+000056e0: 746f 0a20 2020 2020 2020 2020 2020 2028  to.            (
+000056f0: 7375 7065 7263 656c 6c73 2c20 6e61 746f  supercells, nato
+00005700: 6d2c 2033 292e 0a0a 2020 2020 2020 2020  m, 3)...        
+00005710: 2222 220a 2020 2020 2020 2020 7265 7475  """.        retu
+00005720: 726e 2073 656c 662e 5f70 686f 6e6f 6e5f  rn self._phonon_
+00005730: 6461 7461 7365 740a 0a20 2020 2040 7068  dataset..    @ph
+00005740: 6f6e 6f6e 5f64 6174 6173 6574 2e73 6574  onon_dataset.set
+00005750: 7465 720a 2020 2020 6465 6620 7068 6f6e  ter.    def phon
+00005760: 6f6e 5f64 6174 6173 6574 2873 656c 662c  on_dataset(self,
+00005770: 2064 6174 6173 6574 293a 0a20 2020 2020   dataset):.     
+00005780: 2020 2069 6620 6461 7461 7365 7420 6973     if dataset is
+00005790: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
+000057a0: 2020 2073 656c 662e 5f70 686f 6e6f 6e5f     self._phonon_
+000057b0: 6461 7461 7365 7420 3d20 4e6f 6e65 0a20  dataset = None. 
+000057c0: 2020 2020 2020 2065 6c69 6620 2266 6972         elif "fir
+000057d0: 7374 5f61 746f 6d73 2220 696e 2064 6174  st_atoms" in dat
+000057e0: 6173 6574 3a0a 2020 2020 2020 2020 2020  aset:.          
+000057f0: 2020 7365 6c66 2e5f 7068 6f6e 6f6e 5f64    self._phonon_d
+00005800: 6174 6173 6574 203d 2063 6f70 792e 6465  ataset = copy.de
+00005810: 6570 636f 7079 2864 6174 6173 6574 290a  epcopy(dataset).
+00005820: 2020 2020 2020 2020 656c 6966 2022 6469          elif "di
+00005830: 7370 6c61 6365 6d65 6e74 7322 2069 6e20  splacements" in 
+00005840: 6461 7461 7365 743a 0a20 2020 2020 2020  dataset:.       
+00005850: 2020 2020 2073 656c 662e 5f70 686f 6e6f       self._phono
+00005860: 6e5f 6461 7461 7365 7420 3d20 7b7d 0a20  n_dataset = {}. 
+00005870: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+00005880: 7068 6f6e 6f6e 5f64 6973 706c 6163 656d  phonon_displacem
+00005890: 656e 7473 203d 2064 6174 6173 6574 5b22  ents = dataset["
+000058a0: 6469 7370 6c61 6365 6d65 6e74 7322 5d0a  displacements"].
+000058b0: 2020 2020 2020 2020 2020 2020 6966 2022              if "
+000058c0: 666f 7263 6573 2220 696e 2064 6174 6173  forces" in datas
+000058d0: 6574 3a0a 2020 2020 2020 2020 2020 2020  et:.            
+000058e0: 2020 2020 7365 6c66 2e70 686f 6e6f 6e5f      self.phonon_
+000058f0: 666f 7263 6573 203d 2064 6174 6173 6574  forces = dataset
+00005900: 5b22 666f 7263 6573 225d 0a20 2020 2020  ["forces"].     
+00005910: 2020 2020 2020 2069 6620 2273 7570 6572         if "super
+00005920: 6365 6c6c 5f65 6e65 7267 6965 7322 2069  cell_energies" i
+00005930: 6e20 6461 7461 7365 743a 0a20 2020 2020  n dataset:.     
+00005940: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+00005950: 7068 6f6e 6f6e 5f73 7570 6572 6365 6c6c  phonon_supercell
+00005960: 5f65 6e65 7267 6965 7320 3d20 6461 7461  _energies = data
+00005970: 7365 745b 2273 7570 6572 6365 6c6c 5f65  set["supercell_e
+00005980: 6e65 7267 6965 7322 5d0a 2020 2020 2020  nergies"].      
+00005990: 2020 656c 7365 3a0a 2020 2020 2020 2020    else:.        
+000059a0: 2020 2020 7261 6973 6520 5275 6e74 696d      raise Runtim
+000059b0: 6545 7272 6f72 2822 4461 7461 2066 6f72  eError("Data for
+000059c0: 6d61 7420 6f66 2064 6174 6173 6574 2069  mat of dataset i
+000059d0: 7320 7772 6f6e 672e 2229 0a0a 2020 2020  s wrong.")..    
+000059e0: 2020 2020 7365 6c66 2e5f 7068 6f6e 6f6e      self._phonon
+000059f0: 5f73 7570 6572 6365 6c6c 735f 7769 7468  _supercells_with
+00005a00: 5f64 6973 706c 6163 656d 656e 7473 203d  _displacements =
+00005a10: 204e 6f6e 650a 0a20 2020 2040 7072 6f70   None..    @prop
+00005a20: 6572 7479 0a20 2020 2064 6566 2062 616e  erty.    def ban
+00005a30: 645f 696e 6469 6365 7328 7365 6c66 293a  d_indices(self):
+00005a40: 0a20 2020 2020 2020 2022 2222 5365 7474  .        """Sett
+00005a50: 6572 2061 6e64 2067 6574 7465 7220 6f66  er and getter of
+00005a60: 2062 616e 6420 696e 6469 6365 732e 0a0a   band indices...
+00005a70: 2020 2020 2020 2020 6172 7261 795f 6c69          array_li
+00005a80: 6b65 0a20 2020 2020 2020 2020 2020 204c  ke.            L
+00005a90: 6973 7420 6f66 2062 616e 6420 696e 6469  ist of band indi
+00005aa0: 6365 7320 7370 6563 6966 6965 6420 746f  ces specified to
+00005ab0: 2073 656c 6563 7420 7370 6563 6966 6963   select specific
+00005ac0: 2062 616e 6473 0a20 2020 2020 2020 2020   bands.         
+00005ad0: 2020 2074 6f20 636f 6d70 7574 6572 2070     to computer p
+00005ae0: 682d 7068 2069 6e74 6572 6163 7469 6f6e  h-ph interaction
+00005af0: 2072 656c 6174 6564 2070 726f 7065 7274   related propert
+00005b00: 6965 732e 0a0a 2020 2020 2020 2020 2222  ies...        ""
+00005b10: 220a 2020 2020 2020 2020 7265 7475 726e  ".        return
+00005b20: 2073 656c 662e 5f62 616e 645f 696e 6469   self._band_indi
+00005b30: 6365 730a 0a20 2020 2040 6261 6e64 5f69  ces..    @band_i
+00005b40: 6e64 6963 6573 2e73 6574 7465 720a 2020  ndices.setter.  
+00005b50: 2020 6465 6620 6261 6e64 5f69 6e64 6963    def band_indic
+00005b60: 6573 2873 656c 662c 2062 616e 645f 696e  es(self, band_in
+00005b70: 6469 6365 7329 3a0a 2020 2020 2020 2020  dices):.        
+00005b80: 7365 6c66 2e5f 7365 745f 6261 6e64 5f69  self._set_band_i
+00005b90: 6e64 6963 6573 2862 616e 645f 696e 6469  ndices(band_indi
+00005ba0: 6365 733d 6261 6e64 5f69 6e64 6963 6573  ces=band_indices
+00005bb0: 290a 0a20 2020 2064 6566 205f 7365 745f  )..    def _set_
+00005bc0: 6261 6e64 5f69 6e64 6963 6573 2873 656c  band_indices(sel
+00005bd0: 662c 2062 616e 645f 696e 6469 6365 733d  f, band_indices=
+00005be0: 4e6f 6e65 293a 0a20 2020 2020 2020 2069  None):.        i
+00005bf0: 6620 6261 6e64 5f69 6e64 6963 6573 2069  f band_indices i
+00005c00: 7320 4e6f 6e65 3a0a 2020 2020 2020 2020  s None:.        
+00005c10: 2020 2020 6e75 6d5f 6261 6e64 203d 206c      num_band = l
+00005c20: 656e 2873 656c 662e 5f70 7269 6d69 7469  en(self._primiti
+00005c30: 7665 2920 2a20 330a 2020 2020 2020 2020  ve) * 3.        
+00005c40: 2020 2020 7365 6c66 2e5f 6261 6e64 5f69      self._band_i
+00005c50: 6e64 6963 6573 203d 205b 6e70 2e61 7261  ndices = [np.ara
+00005c60: 6e67 6528 6e75 6d5f 6261 6e64 2c20 6474  nge(num_band, dt
+00005c70: 7970 653d 2269 6e74 5f22 295d 0a20 2020  ype="int_")].   
+00005c80: 2020 2020 2065 6c73 653a 0a20 2020 2020       else:.     
+00005c90: 2020 2020 2020 2073 656c 662e 5f62 616e         self._ban
+00005ca0: 645f 696e 6469 6365 7320 3d20 6261 6e64  d_indices = band
+00005cb0: 5f69 6e64 6963 6573 0a20 2020 2020 2020  _indices.       
+00005cc0: 2073 656c 662e 5f62 616e 645f 696e 6469   self._band_indi
+00005cd0: 6365 735f 666c 6174 7465 6e20 3d20 6e70  ces_flatten = np
+00005ce0: 2e68 7374 6163 6b28 7365 6c66 2e5f 6261  .hstack(self._ba
+00005cf0: 6e64 5f69 6e64 6963 6573 292e 6173 7479  nd_indices).asty
+00005d00: 7065 2822 696e 745f 2229 0a0a 2020 2020  pe("int_")..    
+00005d10: 4070 726f 7065 7274 790a 2020 2020 6465  @property.    de
+00005d20: 6620 6d61 7373 6573 2873 656c 6629 3a0a  f masses(self):.
+00005d30: 2020 2020 2020 2020 2222 2253 6574 7465          """Sette
+00005d40: 7220 616e 6420 6765 7474 6572 206f 6620  r and getter of 
+00005d50: 6174 6f6d 6963 206d 6173 7365 7320 6f66  atomic masses of
+00005d60: 2070 7269 6d69 7469 7665 2063 656c 6c2e   primitive cell.
+00005d70: 2222 220a 2020 2020 2020 2020 7265 7475  """.        retu
+00005d80: 726e 2073 656c 662e 5f70 7269 6d69 7469  rn self._primiti
+00005d90: 7665 2e6d 6173 7365 730a 0a20 2020 2040  ve.masses..    @
+00005da0: 6d61 7373 6573 2e73 6574 7465 720a 2020  masses.setter.  
+00005db0: 2020 6465 6620 6d61 7373 6573 2873 656c    def masses(sel
+00005dc0: 662c 206d 6173 7365 7329 3a0a 2020 2020  f, masses):.    
+00005dd0: 2020 2020 6966 206d 6173 7365 7320 6973      if masses is
+00005de0: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
+00005df0: 2020 2072 6574 7572 6e0a 2020 2020 2020     return.      
+00005e00: 2020 705f 6d61 7373 6573 203d 206e 702e    p_masses = np.
+00005e10: 6172 7261 7928 6d61 7373 6573 290a 2020  array(masses).  
+00005e20: 2020 2020 2020 7365 6c66 2e5f 7072 696d        self._prim
+00005e30: 6974 6976 652e 6d61 7373 6573 203d 2070  itive.masses = p
+00005e40: 5f6d 6173 7365 730a 2020 2020 2020 2020  _masses.        
+00005e50: 7032 705f 6d61 7020 3d20 7365 6c66 2e5f  p2p_map = self._
+00005e60: 7072 696d 6974 6976 652e 7032 705f 6d61  primitive.p2p_ma
+00005e70: 700a 2020 2020 2020 2020 735f 6d61 7373  p.        s_mass
+00005e80: 6573 203d 2070 5f6d 6173 7365 735b 5b70  es = p_masses[[p
+00005e90: 3270 5f6d 6170 5b78 5d20 666f 7220 7820  2p_map[x] for x 
+00005ea0: 696e 2073 656c 662e 5f70 7269 6d69 7469  in self._primiti
+00005eb0: 7665 2e73 3270 5f6d 6170 5d5d 0a20 2020  ve.s2p_map]].   
+00005ec0: 2020 2020 2073 656c 662e 5f73 7570 6572       self._super
+00005ed0: 6365 6c6c 2e6d 6173 7365 7320 3d20 735f  cell.masses = s_
+00005ee0: 6d61 7373 6573 0a20 2020 2020 2020 2075  masses.        u
+00005ef0: 3273 5f6d 6170 203d 2073 656c 662e 5f73  2s_map = self._s
+00005f00: 7570 6572 6365 6c6c 2e75 3273 5f6d 6170  upercell.u2s_map
+00005f10: 0a20 2020 2020 2020 2075 5f6d 6173 7365  .        u_masse
+00005f20: 7320 3d20 735f 6d61 7373 6573 5b75 3273  s = s_masses[u2s
+00005f30: 5f6d 6170 5d0a 2020 2020 2020 2020 7365  _map].        se
+00005f40: 6c66 2e5f 756e 6974 6365 6c6c 2e6d 6173  lf._unitcell.mas
+00005f50: 7365 7320 3d20 755f 6d61 7373 6573 0a20  ses = u_masses. 
+00005f60: 2020 2020 2020 2073 656c 662e 5f70 686f         self._pho
+00005f70: 6e6f 6e5f 7072 696d 6974 6976 652e 6d61  non_primitive.ma
+00005f80: 7373 6573 203d 2070 5f6d 6173 7365 730a  sses = p_masses.
+00005f90: 2020 2020 2020 2020 7032 705f 6d61 7020          p2p_map 
+00005fa0: 3d20 7365 6c66 2e5f 7068 6f6e 6f6e 5f70  = self._phonon_p
+00005fb0: 7269 6d69 7469 7665 2e70 3270 5f6d 6170  rimitive.p2p_map
+00005fc0: 0a20 2020 2020 2020 2073 5f6d 6173 7365  .        s_masse
+00005fd0: 7320 3d20 705f 6d61 7373 6573 5b5b 7032  s = p_masses[[p2
+00005fe0: 705f 6d61 705b 785d 2066 6f72 2078 2069  p_map[x] for x i
+00005ff0: 6e20 7365 6c66 2e5f 7068 6f6e 6f6e 5f70  n self._phonon_p
+00006000: 7269 6d69 7469 7665 2e73 3270 5f6d 6170  rimitive.s2p_map
+00006010: 5d5d 0a20 2020 2020 2020 2073 656c 662e  ]].        self.
+00006020: 5f70 686f 6e6f 6e5f 7375 7065 7263 656c  _phonon_supercel
+00006030: 6c2e 6d61 7373 6573 203d 2073 5f6d 6173  l.masses = s_mas
+00006040: 7365 730a 0a20 2020 2040 7072 6f70 6572  ses..    @proper
+00006050: 7479 0a20 2020 2064 6566 2073 7570 6572  ty.    def super
+00006060: 6365 6c6c 735f 7769 7468 5f64 6973 706c  cells_with_displ
+00006070: 6163 656d 656e 7473 2873 656c 6629 3a0a  acements(self):.
+00006080: 2020 2020 2020 2020 2222 2252 6574 7572          """Retur
+00006090: 6e20 7375 7065 7263 656c 6c73 2077 6974  n supercells wit
+000060a0: 6820 6469 7370 6c61 6365 6d65 6e74 732e  h displacements.
+000060b0: 0a0a 2020 2020 2020 2020 6c69 7374 206f  ..        list o
+000060c0: 6620 5068 6f6e 6f70 7941 746f 6d73 0a20  f PhonopyAtoms. 
+000060d0: 2020 2020 2020 2020 2020 2053 7570 6572             Super
+000060e0: 6365 6c6c 7320 7769 7468 2064 6973 706c  cells with displ
+000060f0: 6163 656d 656e 7473 2067 656e 6572 6174  acements generat
+00006100: 6564 2062 790a 2020 2020 2020 2020 2020  ed by.          
+00006110: 2020 5068 6f6e 6f33 7079 2e67 656e 6572    Phono3py.gener
+00006120: 6174 655f 6469 7370 6c61 6365 6d65 6e74  ate_displacement
+00006130: 732e 0a0a 2020 2020 2020 2020 2222 220a  s...        """.
+00006140: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
+00006150: 5f73 7570 6572 6365 6c6c 735f 7769 7468  _supercells_with
+00006160: 5f64 6973 706c 6163 656d 656e 7473 2069  _displacements i
+00006170: 7320 4e6f 6e65 3a0a 2020 2020 2020 2020  s None:.        
+00006180: 2020 2020 7365 6c66 2e5f 6275 696c 645f      self._build_
+00006190: 7375 7065 7263 656c 6c73 5f77 6974 685f  supercells_with_
+000061a0: 6469 7370 6c61 6365 6d65 6e74 7328 290a  displacements().
+000061b0: 2020 2020 2020 2020 7265 7475 726e 2073          return s
+000061c0: 656c 662e 5f73 7570 6572 6365 6c6c 735f  elf._supercells_
+000061d0: 7769 7468 5f64 6973 706c 6163 656d 656e  with_displacemen
+000061e0: 7473 0a0a 2020 2020 4070 726f 7065 7274  ts..    @propert
+000061f0: 790a 2020 2020 6465 6620 7068 6f6e 6f6e  y.    def phonon
+00006200: 5f73 7570 6572 6365 6c6c 735f 7769 7468  _supercells_with
+00006210: 5f64 6973 706c 6163 656d 656e 7473 2873  _displacements(s
+00006220: 656c 6629 3a0a 2020 2020 2020 2020 2222  elf):.        ""
+00006230: 2252 6574 7572 6e20 7375 7065 7263 656c  "Return supercel
+00006240: 6c73 2077 6974 6820 6469 7370 6c61 6365  ls with displace
+00006250: 6d65 6e74 7320 666f 7220 6663 322e 0a0a  ments for fc2...
+00006260: 2020 2020 2020 2020 6c69 7374 206f 6620          list of 
+00006270: 5068 6f6e 6f70 7941 746f 6d73 0a20 2020  PhonopyAtoms.   
+00006280: 2020 2020 2020 2020 2053 7570 6572 6365           Superce
+00006290: 6c6c 7320 7769 7468 2064 6973 706c 6163  lls with displac
+000062a0: 656d 656e 7473 2067 656e 6572 6174 6564  ements generated
+000062b0: 2062 790a 2020 2020 2020 2020 2020 2020   by.            
+000062c0: 5068 6f6e 6f33 7079 2e67 656e 6572 6174  Phono3py.generat
+000062d0: 655f 6469 7370 6c61 6365 6d65 6e74 732e  e_displacements.
+000062e0: 0a0a 2020 2020 2020 2020 2222 220a 2020  ..        """.  
+000062f0: 2020 2020 2020 6966 2073 656c 662e 5f70        if self._p
+00006300: 686f 6e6f 6e5f 7375 7065 7263 656c 6c73  honon_supercells
+00006310: 5f77 6974 685f 6469 7370 6c61 6365 6d65  _with_displaceme
+00006320: 6e74 7320 6973 204e 6f6e 653a 0a20 2020  nts is None:.   
+00006330: 2020 2020 2020 2020 2069 6620 7365 6c66           if self
+00006340: 2e5f 7068 6f6e 6f6e 5f64 6174 6173 6574  ._phonon_dataset
+00006350: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
+00006360: 2020 2020 2020 2020 2020 2020 2020 7365                se
+00006370: 6c66 2e5f 7068 6f6e 6f6e 5f73 7570 6572  lf._phonon_super
+00006380: 6365 6c6c 735f 7769 7468 5f64 6973 706c  cells_with_displ
+00006390: 6163 656d 656e 7473 203d 2028 0a20 2020  acements = (.   
+000063a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000063b0: 2073 656c 662e 5f62 7569 6c64 5f70 686f   self._build_pho
+000063c0: 6e6f 6e5f 7375 7065 7263 656c 6c73 5f77  non_supercells_w
+000063d0: 6974 685f 6469 7370 6c61 6365 6d65 6e74  ith_displacement
+000063e0: 7328 0a20 2020 2020 2020 2020 2020 2020  s(.             
+000063f0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+00006400: 5f70 686f 6e6f 6e5f 7375 7065 7263 656c  _phonon_supercel
+00006410: 6c2c 2073 656c 662e 5f70 686f 6e6f 6e5f  l, self._phonon_
+00006420: 6461 7461 7365 740a 2020 2020 2020 2020  dataset.        
+00006430: 2020 2020 2020 2020 2020 2020 290a 2020              ).  
+00006440: 2020 2020 2020 2020 2020 2020 2020 290a                ).
+00006450: 2020 2020 2020 2020 7265 7475 726e 2073          return s
+00006460: 656c 662e 5f70 686f 6e6f 6e5f 7375 7065  elf._phonon_supe
+00006470: 7263 656c 6c73 5f77 6974 685f 6469 7370  rcells_with_disp
+00006480: 6c61 6365 6d65 6e74 730a 0a20 2020 2040  lacements..    @
+00006490: 7072 6f70 6572 7479 0a20 2020 2064 6566  property.    def
+000064a0: 206d 6573 685f 6e75 6d62 6572 7328 7365   mesh_numbers(se
+000064b0: 6c66 293a 0a20 2020 2020 2020 2022 2222  lf):.        """
+000064c0: 5365 7474 6572 2061 6e64 2067 6574 7465  Setter and gette
+000064d0: 7220 6f66 2073 616d 706c 696e 6720 6d65  r of sampling me
+000064e0: 7368 206e 756d 6265 7273 2069 6e20 7265  sh numbers in re
+000064f0: 6369 7072 6f63 616c 2073 7061 6365 2e22  ciprocal space."
+00006500: 2222 0a20 2020 2020 2020 2069 6620 7365  "".        if se
+00006510: 6c66 2e5f 627a 5f67 7269 6420 6973 204e  lf._bz_grid is N
+00006520: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
+00006530: 2072 6574 7572 6e20 4e6f 6e65 0a20 2020   return None.   
+00006540: 2020 2020 2065 6c73 653a 0a20 2020 2020       else:.     
+00006550: 2020 2020 2020 2072 6574 7572 6e20 7365         return se
+00006560: 6c66 2e5f 627a 5f67 7269 642e 445f 6469  lf._bz_grid.D_di
+00006570: 6167 0a0a 2020 2020 406d 6573 685f 6e75  ag..    @mesh_nu
+00006580: 6d62 6572 732e 7365 7474 6572 0a20 2020  mbers.setter.   
+00006590: 2064 6566 206d 6573 685f 6e75 6d62 6572   def mesh_number
+000065a0: 7328 7365 6c66 2c20 6d65 7368 5f6e 756d  s(self, mesh_num
+000065b0: 6265 7273 3a20 556e 696f 6e5b 696e 742c  bers: Union[int,
+000065c0: 2066 6c6f 6174 2c20 5365 7175 656e 6365   float, Sequence
+000065d0: 2c20 6e70 2e6e 6461 7272 6179 5d29 3a0a  , np.ndarray]):.
+000065e0: 2020 2020 2020 2020 7365 6c66 2e5f 7365          self._se
+000065f0: 745f 6d65 7368 5f6e 756d 6265 7273 286d  t_mesh_numbers(m
+00006600: 6573 685f 6e75 6d62 6572 7329 0a0a 2020  esh_numbers)..  
+00006610: 2020 4070 726f 7065 7274 790a 2020 2020    @property.    
+00006620: 6465 6620 7468 6572 6d61 6c5f 636f 6e64  def thermal_cond
+00006630: 7563 7469 7669 7479 2873 656c 6629 3a0a  uctivity(self):.
+00006640: 2020 2020 2020 2020 2222 2252 6574 7572          """Retur
+00006650: 6e20 7468 6572 6d61 6c20 636f 6e64 7563  n thermal conduc
+00006660: 7469 7669 7479 2063 6c61 7373 2069 6e73  tivity class ins
+00006670: 7461 6e63 652e 2222 220a 2020 2020 2020  tance.""".      
+00006680: 2020 7265 7475 726e 2073 656c 662e 5f74    return self._t
+00006690: 6865 726d 616c 5f63 6f6e 6475 6374 6976  hermal_conductiv
+000066a0: 6974 790a 0a20 2020 2040 7072 6f70 6572  ity..    @proper
+000066b0: 7479 0a20 2020 2064 6566 2064 6973 706c  ty.    def displ
+000066c0: 6163 656d 656e 7473 2873 656c 6629 3a0a  acements(self):.
+000066d0: 2020 2020 2020 2020 2222 2253 6574 7465          """Sette
+000066e0: 7220 616e 6420 6765 7474 6572 2064 6973  r and getter dis
+000066f0: 706c 6163 656d 656e 7473 2069 6e20 7375  placements in su
+00006700: 7065 7263 656c 6c73 2e0a 0a20 2020 2020  percells...     
+00006710: 2020 2054 6865 7265 2061 7265 2074 776f     There are two
+00006720: 2074 7970 6573 206f 6620 6469 7370 6c61   types of displa
+00006730: 6365 6d65 6e74 2064 6174 6173 6574 2e20  cement dataset. 
+00006740: 5365 6520 7468 6520 646f 6373 7472 696e  See the docstrin
+00006750: 670a 2020 2020 2020 2020 6f66 2064 6174  g.        of dat
+00006760: 6173 6574 2061 626f 7574 2074 7970 6573  aset about types
+00006770: 2031 2061 6e64 2032 2066 6f72 2074 6865   1 and 2 for the
+00006780: 2064 6973 706c 6163 656d 656e 7420 6461   displacement da
+00006790: 7461 7365 7420 666f 726d 6174 732e 0a20  taset formats.. 
+000067a0: 2020 2020 2020 2044 6973 706c 6163 656d         Displacem
+000067b0: 656e 7473 2073 6574 2072 6574 7572 6e65  ents set returne
+000067c0: 6420 6465 7065 6e64 7320 6f6e 2065 6974  d depends on eit
+000067d0: 6865 7220 7479 7065 2d31 206f 7220 7479  her type-1 or ty
+000067e0: 7065 2d32 2061 730a 2020 2020 2020 2020  pe-2 as.        
+000067f0: 666f 6c6c 6f77 733a 0a0a 2020 2020 2020  follows:..      
+00006800: 2020 5479 7065 2d31 2c20 4c69 7374 206f    Type-1, List o
+00006810: 6620 6c69 7374 0a20 2020 2020 2020 2020  f list.         
+00006820: 2020 2054 6865 2069 6e74 6572 6e61 6c20     The internal 
+00006830: 6c69 7374 2068 6173 2034 2065 6c65 6d65  list has 4 eleme
+00006840: 6e74 7320 7375 6368 2061 7320 5b33 322c  nts such as [32,
+00006850: 2030 2e30 312c 2030 2e30 2c20 302e 305d   0.01, 0.0, 0.0]
+00006860: 5d2e 0a20 2020 2020 2020 2020 2020 2054  ]..            T
+00006870: 6865 2066 6972 7374 2065 6c65 6d65 6e74  he first element
+00006880: 2069 7320 7468 6520 7375 7065 7263 656c   is the supercel
+00006890: 6c20 6174 6f6d 2069 6e64 6578 2073 7461  l atom index sta
+000068a0: 7274 696e 6720 7769 7468 2030 2e0a 2020  rting with 0..  
+000068b0: 2020 2020 2020 2020 2020 5468 6520 7265            The re
+000068c0: 6d61 696e 696e 6720 7468 7265 6520 656c  maining three el
+000068d0: 656d 656e 7473 2067 6976 6520 7468 6520  ements give the 
+000068e0: 6469 7370 6c61 6365 6d65 6e74 2069 6e20  displacement in 
+000068f0: 4361 7274 6573 6961 6e0a 2020 2020 2020  Cartesian.      
+00006900: 2020 2020 2020 636f 6f72 6469 6e61 7465        coordinate
+00006910: 732e 0a20 2020 2020 2020 2054 7970 652d  s..        Type-
+00006920: 322c 2061 7272 6179 5f6c 696b 650a 2020  2, array_like.  
+00006930: 2020 2020 2020 2020 2020 4469 7370 6c61            Displa
+00006940: 6365 6d65 6e74 7320 6f66 2061 6c6c 2061  cements of all a
+00006950: 746f 6d73 206f 6620 616c 6c20 7375 7065  toms of all supe
+00006960: 7263 656c 6c73 2069 6e20 4361 7274 6573  rcells in Cartes
+00006970: 6961 6e0a 2020 2020 2020 2020 2020 2020  ian.            
+00006980: 636f 6f72 6469 6e61 7465 732e 0a20 2020  coordinates..   
+00006990: 2020 2020 2020 2020 2073 6861 7065 3d28           shape=(
+000069a0: 7375 7065 7263 656c 6c73 2c20 6e61 746f  supercells, nato
+000069b0: 6d2c 2033 290a 2020 2020 2020 2020 2020  m, 3).          
+000069c0: 2020 6474 7970 653d 2764 6f75 626c 6527    dtype='double'
+000069d0: 0a0a 0a20 2020 2020 2020 2046 6f72 2073  ...        For s
+000069e0: 6574 7465 722c 206f 6e6c 7920 7479 7065  etter, only type
+000069f0: 2d32 2064 6174 6173 6574 2066 6f72 6d61  -2 dataset forma
+00006a00: 7420 6973 2061 6c6c 6f77 6564 2e0a 0a20  t is allowed... 
+00006a10: 2020 2020 2020 2064 6973 706c 6163 656d         displacem
+00006a20: 656e 7473 203a 2061 7272 6179 5f6c 696b  ents : array_lik
+00006a30: 650a 2020 2020 2020 2020 2020 2020 4174  e.            At
+00006a40: 6f6d 6963 2064 6973 706c 6163 656d 656e  omic displacemen
+00006a50: 7473 206f 6620 616c 6c20 6174 6f6d 7320  ts of all atoms 
+00006a60: 6f66 2061 6c6c 2073 7570 6572 6365 6c6c  of all supercell
+00006a70: 732e 0a20 2020 2020 2020 2020 2020 204f  s..            O
+00006a80: 6e6c 7920 616c 6c20 6469 7370 6c61 6365  nly all displace
+00006a90: 6d65 6e74 7320 696e 2065 6163 6820 7375  ments in each su
+00006aa0: 7065 7263 656c 6c20 6361 7365 2028 7479  percell case (ty
+00006ab0: 7065 2d32 2920 6973 0a20 2020 2020 2020  pe-2) is.       
+00006ac0: 2020 2020 2073 7570 706f 7274 6564 2e0a       supported..
+00006ad0: 2020 2020 2020 2020 2020 2020 7368 6170              shap
+00006ae0: 653d 2873 7570 6572 6365 6c6c 732c 206e  e=(supercells, n
+00006af0: 6174 6f6d 2c20 3329 2c20 6474 7970 653d  atom, 3), dtype=
+00006b00: 2764 6f75 626c 6527 2c20 6f72 6465 723d  'double', order=
+00006b10: 2743 270a 0a20 2020 2020 2020 2022 2222  'C'..        """
+00006b20: 0a20 2020 2020 2020 2064 6174 6173 6574  .        dataset
+00006b30: 203d 2073 656c 662e 5f64 6174 6173 6574   = self._dataset
+00006b40: 0a0a 2020 2020 2020 2020 6966 2022 6669  ..        if "fi
+00006b50: 7273 745f 6174 6f6d 7322 2069 6e20 6461  rst_atoms" in da
+00006b60: 7461 7365 743a 0a20 2020 2020 2020 2020  taset:.         
+00006b70: 2020 206e 756d 5f73 6365 6c6c 7320 3d20     num_scells = 
+00006b80: 6c65 6e28 6461 7461 7365 745b 2266 6972  len(dataset["fir
+00006b90: 7374 5f61 746f 6d73 225d 290a 2020 2020  st_atoms"]).    
+00006ba0: 2020 2020 2020 2020 666f 7220 6469 7370          for disp
+00006bb0: 3120 696e 2064 6174 6173 6574 5b22 6669  1 in dataset["fi
+00006bc0: 7273 745f 6174 6f6d 7322 5d3a 0a20 2020  rst_atoms"]:.   
+00006bd0: 2020 2020 2020 2020 2020 2020 206e 756d               num
+00006be0: 5f73 6365 6c6c 7320 2b3d 206c 656e 2864  _scells += len(d
+00006bf0: 6973 7031 5b22 7365 636f 6e64 5f61 746f  isp1["second_ato
+00006c00: 6d73 225d 290a 2020 2020 2020 2020 2020  ms"]).          
+00006c10: 2020 6469 7370 6c61 6365 6d65 6e74 7320    displacements 
+00006c20: 3d20 6e70 2e7a 6572 6f73 280a 2020 2020  = np.zeros(.    
+00006c30: 2020 2020 2020 2020 2020 2020 286e 756d              (num
+00006c40: 5f73 6365 6c6c 732c 2073 656c 662e 5f73  _scells, self._s
+00006c50: 7570 6572 6365 6c6c 2e67 6574 5f6e 756d  upercell.get_num
+00006c60: 6265 725f 6f66 5f61 746f 6d73 2829 2c20  ber_of_atoms(), 
+00006c70: 3329 2c0a 2020 2020 2020 2020 2020 2020  3),.            
+00006c80: 2020 2020 6474 7970 653d 2264 6f75 626c      dtype="doubl
+00006c90: 6522 2c0a 2020 2020 2020 2020 2020 2020  e",.            
+00006ca0: 2020 2020 6f72 6465 723d 2243 222c 0a20      order="C",. 
+00006cb0: 2020 2020 2020 2020 2020 2029 0a20 2020             ).   
+00006cc0: 2020 2020 2020 2020 2069 203d 2030 0a20           i = 0. 
+00006cd0: 2020 2020 2020 2020 2020 2066 6f72 2064             for d
+00006ce0: 6973 7031 2069 6e20 6461 7461 7365 745b  isp1 in dataset[
+00006cf0: 2266 6972 7374 5f61 746f 6d73 225d 3a0a  "first_atoms"]:.
+00006d00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006d10: 6469 7370 6c61 6365 6d65 6e74 735b 692c  displacements[i,
+00006d20: 2064 6973 7031 5b22 6e75 6d62 6572 225d   disp1["number"]
+00006d30: 5d20 3d20 6469 7370 315b 2264 6973 706c  ] = disp1["displ
+00006d40: 6163 656d 656e 7422 5d0a 2020 2020 2020  acement"].      
+00006d50: 2020 2020 2020 2020 2020 6920 2b3d 2031            i += 1
+00006d60: 0a20 2020 2020 2020 2020 2020 2066 6f72  .            for
+00006d70: 2064 6973 7031 2069 6e20 6461 7461 7365   disp1 in datase
+00006d80: 745b 2266 6972 7374 5f61 746f 6d73 225d  t["first_atoms"]
+00006d90: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+00006da0: 2020 666f 7220 6469 7370 3220 696e 2064    for disp2 in d
+00006db0: 6973 7031 5b22 7365 636f 6e64 5f61 746f  isp1["second_ato
+00006dc0: 6d73 225d 3a0a 2020 2020 2020 2020 2020  ms"]:.          
+00006dd0: 2020 2020 2020 2020 2020 6469 7370 6c61            displa
+00006de0: 6365 6d65 6e74 735b 692c 2064 6973 7032  cements[i, disp2
+00006df0: 5b22 6e75 6d62 6572 225d 5d20 3d20 6469  ["number"]] = di
+00006e00: 7370 325b 2264 6973 706c 6163 656d 656e  sp2["displacemen
+00006e10: 7422 5d0a 2020 2020 2020 2020 2020 2020  t"].            
+00006e20: 2020 2020 2020 2020 6920 2b3d 2031 0a20          i += 1. 
+00006e30: 2020 2020 2020 2065 6c69 6620 2266 6f72         elif "for
+00006e40: 6365 7322 2069 6e20 6461 7461 7365 7420  ces" in dataset 
+00006e50: 6f72 2022 6469 7370 6c61 6365 6d65 6e74  or "displacement
+00006e60: 7322 2069 6e20 6461 7461 7365 743a 0a20  s" in dataset:. 
+00006e70: 2020 2020 2020 2020 2020 2064 6973 706c             displ
+00006e80: 6163 656d 656e 7473 203d 2064 6174 6173  acements = datas
+00006e90: 6574 5b22 6469 7370 6c61 6365 6d65 6e74  et["displacement
+00006ea0: 7322 5d0a 2020 2020 2020 2020 656c 7365  s"].        else
+00006eb0: 3a0a 2020 2020 2020 2020 2020 2020 7261  :.            ra
+00006ec0: 6973 6520 5275 6e74 696d 6545 7272 6f72  ise RuntimeError
+00006ed0: 2822 6469 7370 6c61 6365 6d65 6e74 2064  ("displacement d
+00006ee0: 6174 6173 6574 2068 6173 2077 726f 6e67  ataset has wrong
+00006ef0: 2066 6f72 6d61 742e 2229 0a0a 2020 2020   format.")..    
+00006f00: 2020 2020 7265 7475 726e 2064 6973 706c      return displ
+00006f10: 6163 656d 656e 7473 0a0a 2020 2020 4064  acements..    @d
+00006f20: 6973 706c 6163 656d 656e 7473 2e73 6574  isplacements.set
+00006f30: 7465 720a 2020 2020 6465 6620 6469 7370  ter.    def disp
+00006f40: 6c61 6365 6d65 6e74 7328 7365 6c66 2c20  lacements(self, 
+00006f50: 6469 7370 6c61 6365 6d65 6e74 7329 3a0a  displacements):.
+00006f60: 2020 2020 2020 2020 6469 7370 7320 3d20          disps = 
+00006f70: 6e70 2e61 7272 6179 2864 6973 706c 6163  np.array(displac
+00006f80: 656d 656e 7473 2c20 6474 7970 653d 2264  ements, dtype="d
+00006f90: 6f75 626c 6522 2c20 6f72 6465 723d 2243  ouble", order="C
+00006fa0: 2229 0a20 2020 2020 2020 206e 6174 6f6d  ").        natom
+00006fb0: 203d 206c 656e 2873 656c 662e 5f73 7570   = len(self._sup
+00006fc0: 6572 6365 6c6c 290a 2020 2020 2020 2020  ercell).        
+00006fd0: 6966 2064 6973 7073 2e6e 6469 6d20 213d  if disps.ndim !=
+00006fe0: 2033 206f 7220 6469 7370 732e 7368 6170   3 or disps.shap
+00006ff0: 655b 313a 5d20 213d 2028 6e61 746f 6d2c  e[1:] != (natom,
+00007000: 2033 293a 0a20 2020 2020 2020 2020 2020   3):.           
+00007010: 2072 6169 7365 2052 756e 7469 6d65 4572   raise RuntimeEr
+00007020: 726f 7228 2241 7272 6179 2073 6861 7065  ror("Array shape
+00007030: 206f 6620 6469 7370 6c61 6365 6d65 6e74   of displacement
+00007040: 7320 6973 2069 6e63 6f72 7265 6374 2e22  s is incorrect."
+00007050: 290a 2020 2020 2020 2020 6966 2073 656c  ).        if sel
+00007060: 662e 5f64 6174 6173 6574 2069 7320 4e6f  f._dataset is No
+00007070: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
+00007080: 7365 6c66 2e5f 6461 7461 7365 7420 3d20  self._dataset = 
+00007090: 7b7d 0a20 2020 2020 2020 2065 6c69 6620  {}.        elif 
+000070a0: 2266 6972 7374 5f61 746f 6d73 2220 696e  "first_atoms" in
+000070b0: 2073 656c 662e 5f64 6174 6173 6574 3a0a   self._dataset:.
+000070c0: 2020 2020 2020 2020 2020 2020 7261 6973              rais
+000070d0: 6520 5275 6e74 696d 6545 7272 6f72 2822  e RuntimeError("
+000070e0: 4469 7370 6c61 6365 6d65 6e74 7320 6172  Displacements ar
+000070f0: 6520 696e 636f 6d70 6174 6962 6c65 2077  e incompatible w
+00007100: 6974 6820 6461 7461 7365 742e 2229 0a20  ith dataset."). 
+00007110: 2020 2020 2020 2073 656c 662e 5f64 6174         self._dat
+00007120: 6173 6574 5b22 6469 7370 6c61 6365 6d65  aset["displaceme
+00007130: 6e74 7322 5d20 3d20 6469 7370 730a 2020  nts"] = disps.  
+00007140: 2020 2020 2020 7365 6c66 2e5f 7375 7065        self._supe
+00007150: 7263 656c 6c73 5f77 6974 685f 6469 7370  rcells_with_disp
+00007160: 6c61 6365 6d65 6e74 7320 3d20 4e6f 6e65  lacements = None
+00007170: 0a0a 2020 2020 4070 726f 7065 7274 790a  ..    @property.
+00007180: 2020 2020 6465 6620 666f 7263 6573 2873      def forces(s
+00007190: 656c 6629 3a0a 2020 2020 2020 2020 2222  elf):.        ""
+000071a0: 2253 6574 7465 7220 616e 6420 6765 7474  "Setter and gett
+000071b0: 6572 206f 6620 666f 7263 6573 2069 6e20  er of forces in 
+000071c0: 6469 7370 6c61 6365 6d65 6e74 2064 6174  displacement dat
+000071d0: 6173 6574 2e0a 0a20 2020 2020 2020 2041  aset...        A
+000071e0: 2073 6574 206f 6620 6174 6f6d 6963 2066   set of atomic f
+000071f0: 6f72 6365 7320 696e 2064 6973 706c 6163  orces in displac
+00007200: 6564 2073 7570 6572 6365 6c6c 732e 2054  ed supercells. T
+00007210: 6865 206f 7264 6572 206f 660a 2020 2020  he order of.    
+00007220: 2020 2020 6469 7370 6c61 6365 6420 7375      displaced su
+00007230: 7065 7263 656c 6c73 2068 6173 2074 6f20  percells has to 
+00007240: 6d61 7463 6820 7769 7468 2074 6861 7420  match with that 
+00007250: 696e 2064 6973 706c 6163 656d 656e 7420  in displacement 
+00007260: 6461 7461 7365 742e 0a20 2020 2020 2020  dataset..       
+00007270: 2073 6861 7065 3d28 6469 7370 6c61 6365   shape=(displace
+00007280: 6420 7375 7065 7263 656c 6c73 2c20 6174  d supercells, at
+00007290: 6f6d 7320 696e 2073 7570 6572 6365 6c6c  oms in supercell
+000072a0: 2c20 3329 0a0a 2020 2020 2020 2020 6765  , 3)..        ge
+000072b0: 7474 6572 203a 206e 6461 7272 6179 0a0a  tter : ndarray..
+000072c0: 2020 2020 2020 2020 7365 7474 6572 203a          setter :
+000072d0: 2061 7272 6179 5f6c 696b 650a 2020 2020   array_like.    
+000072e0: 2020 2020 2020 2020 5468 6520 6f72 6465          The orde
+000072f0: 7220 6f66 2073 7570 6572 6365 6c6c 7320  r of supercells 
+00007300: 7573 6564 2066 6f72 2063 616c 6375 6c61  used for calcula
+00007310: 7469 6e67 2066 6f72 6365 7320 6861 7320  ting forces has 
+00007320: 746f 0a20 2020 2020 2020 2020 2020 2062  to.            b
+00007330: 6520 7468 6520 7361 6d65 206f 7264 6572  e the same order
+00007340: 206f 6620 7375 7065 7263 656c 6c73 5f77   of supercells_w
+00007350: 6974 685f 6469 7370 6c61 6365 6d65 6e74  ith_displacement
+00007360: 732e 0a0a 2020 2020 2020 2020 2222 220a  s...        """.
+00007370: 2020 2020 2020 2020 7265 7475 726e 2073          return s
+00007380: 656c 662e 5f67 6574 5f66 6f72 6365 735f  elf._get_forces_
+00007390: 656e 6572 6769 6573 2874 6172 6765 743d  energies(target=
+000073a0: 2266 6f72 6365 7322 290a 0a20 2020 2040  "forces")..    @
+000073b0: 666f 7263 6573 2e73 6574 7465 720a 2020  forces.setter.  
+000073c0: 2020 6465 6620 666f 7263 6573 2873 656c    def forces(sel
+000073d0: 662c 2076 616c 7565 7329 3a0a 2020 2020  f, values):.    
+000073e0: 2020 2020 7365 6c66 2e5f 7365 745f 666f      self._set_fo
+000073f0: 7263 6573 5f65 6e65 7267 6965 7328 7661  rces_energies(va
+00007400: 6c75 6573 2c20 7461 7267 6574 3d22 666f  lues, target="fo
+00007410: 7263 6573 2229 0a0a 2020 2020 4070 726f  rces")..    @pro
+00007420: 7065 7274 790a 2020 2020 6465 6620 7375  perty.    def su
+00007430: 7065 7263 656c 6c5f 656e 6572 6769 6573  percell_energies
+00007440: 2873 656c 6629 3a0a 2020 2020 2020 2020  (self):.        
+00007450: 2222 2253 6574 7465 7220 616e 6420 6765  """Setter and ge
+00007460: 7474 6572 206f 6620 7375 7065 7263 656c  tter of supercel
+00007470: 6c20 656e 6572 6769 6573 2069 6e20 6469  l energies in di
+00007480: 7370 6c61 6365 6d65 6e74 2064 6174 6173  splacement datas
+00007490: 6574 2e0a 0a20 2020 2020 2020 2041 2073  et...        A s
+000074a0: 6574 206f 6620 7375 7065 7263 656c 6c20  et of supercell 
+000074b0: 656e 6572 6769 6573 206f 6620 6469 7370  energies of disp
+000074c0: 6c61 6365 6420 7375 7065 7263 656c 6c73  laced supercells
+000074d0: 2e20 5468 6520 6f72 6465 7220 6f66 0a20  . The order of. 
+000074e0: 2020 2020 2020 2064 6973 706c 6163 6564         displaced
+000074f0: 2073 7570 6572 6365 6c6c 7320 6861 7320   supercells has 
+00007500: 746f 206d 6174 6368 2077 6974 6820 7468  to match with th
+00007510: 6174 2069 6e20 6469 7370 6c61 6365 6d65  at in displaceme
+00007520: 6e74 2064 6174 6173 6574 2e0a 2020 2020  nt dataset..    
+00007530: 2020 2020 7368 6170 653d 2864 6973 706c      shape=(displ
+00007540: 6163 6564 2073 7570 6572 6365 6c6c 732c  aced supercells,
+00007550: 290a 0a20 2020 2020 2020 2067 6574 7465  )..        gette
+00007560: 7220 3a20 6e64 6172 7261 790a 0a20 2020  r : ndarray..   
+00007570: 2020 2020 2073 6574 7465 7220 3a20 6172       setter : ar
+00007580: 7261 795f 6c69 6b65 0a20 2020 2020 2020  ray_like.       
+00007590: 2020 2020 2054 6865 206f 7264 6572 206f       The order o
+000075a0: 6620 7375 7065 7263 656c 6c73 2075 7365  f supercells use
+000075b0: 6420 666f 7220 6361 6c63 756c 6174 696e  d for calculatin
+000075c0: 6720 7375 7065 7263 656c 6c20 656e 6572  g supercell ener
+000075d0: 6769 6573 2068 6173 0a20 2020 2020 2020  gies has.       
+000075e0: 2020 2020 2074 6f20 6265 2074 6865 2073       to be the s
+000075f0: 616d 6520 6f72 6465 7220 6f66 2073 7570  ame order of sup
+00007600: 6572 6365 6c6c 735f 7769 7468 5f64 6973  ercells_with_dis
+00007610: 706c 6163 656d 656e 7473 2e0a 0a20 2020  placements...   
+00007620: 2020 2020 2022 2222 0a20 2020 2020 2020       """.       
+00007630: 2072 6574 7572 6e20 7365 6c66 2e5f 6765   return self._ge
+00007640: 745f 666f 7263 6573 5f65 6e65 7267 6965  t_forces_energie
+00007650: 7328 7461 7267 6574 3d22 7375 7065 7263  s(target="superc
+00007660: 656c 6c5f 656e 6572 6769 6573 2229 0a0a  ell_energies")..
+00007670: 2020 2020 4073 7570 6572 6365 6c6c 5f65      @supercell_e
+00007680: 6e65 7267 6965 732e 7365 7474 6572 0a20  nergies.setter. 
+00007690: 2020 2064 6566 2073 7570 6572 6365 6c6c     def supercell
+000076a0: 5f65 6e65 7267 6965 7328 7365 6c66 2c20  _energies(self, 
+000076b0: 7661 6c75 6573 293a 0a20 2020 2020 2020  values):.       
+000076c0: 2073 656c 662e 5f73 6574 5f66 6f72 6365   self._set_force
+000076d0: 735f 656e 6572 6769 6573 2876 616c 7565  s_energies(value
+000076e0: 732c 2074 6172 6765 743d 2273 7570 6572  s, target="super
+000076f0: 6365 6c6c 5f65 6e65 7267 6965 7322 290a  cell_energies").
+00007700: 0a20 2020 2040 7072 6f70 6572 7479 0a20  .    @property. 
+00007710: 2020 2064 6566 2070 686f 6e6f 6e5f 6469     def phonon_di
+00007720: 7370 6c61 6365 6d65 6e74 7328 7365 6c66  splacements(self
+00007730: 293a 0a20 2020 2020 2020 2022 2222 5365  ):.        """Se
+00007740: 7474 6572 2061 6e64 2067 6574 7465 7220  tter and getter 
+00007750: 6f66 2064 6973 706c 6163 656d 656e 7473  of displacements
+00007760: 2069 6e20 7375 7065 7263 656c 6c73 2066   in supercells f
+00007770: 6f72 2066 6332 2e0a 0a20 2020 2020 2020  or fc2...       
+00007780: 2054 6865 7265 2061 7265 2074 776f 2074   There are two t
+00007790: 7970 6573 206f 6620 6469 7370 6c61 6365  ypes of displace
+000077a0: 6d65 6e74 2064 6174 6173 6574 2e20 5365  ment dataset. Se
+000077b0: 6520 7468 6520 646f 6373 7472 696e 670a  e the docstring.
+000077c0: 2020 2020 2020 2020 6f66 2064 6174 6173          of datas
+000077d0: 6574 2061 626f 7574 2074 7970 6573 2031  et about types 1
+000077e0: 2061 6e64 2032 2066 6f72 2074 6865 2064   and 2 for the d
+000077f0: 6973 706c 6163 656d 656e 7420 6461 7461  isplacement data
+00007800: 7365 7420 666f 726d 6174 732e 0a20 2020  set formats..   
+00007810: 2020 2020 2044 6973 706c 6163 656d 656e       Displacemen
+00007820: 7473 2073 6574 2072 6574 7572 6e65 6420  ts set returned 
+00007830: 6465 7065 6e64 7320 6f6e 2065 6974 6865  depends on eithe
+00007840: 7220 7479 7065 2d31 206f 7220 7479 7065  r type-1 or type
+00007850: 2d32 2061 730a 2020 2020 2020 2020 666f  -2 as.        fo
+00007860: 6c6c 6f77 733a 0a0a 2020 2020 2020 2020  llows:..        
+00007870: 5479 7065 2d31 2c20 4c69 7374 206f 6620  Type-1, List of 
+00007880: 6c69 7374 0a20 2020 2020 2020 2020 2020  list.           
+00007890: 2054 6865 2069 6e74 6572 6e61 6c20 6c69   The internal li
+000078a0: 7374 2068 6173 2034 2065 6c65 6d65 6e74  st has 4 element
+000078b0: 7320 7375 6368 2061 7320 5b33 322c 2030  s such as [32, 0
+000078c0: 2e30 312c 2030 2e30 2c20 302e 305d 5d2e  .01, 0.0, 0.0]].
+000078d0: 0a20 2020 2020 2020 2020 2020 2054 6865  .            The
+000078e0: 2066 6972 7374 2065 6c65 6d65 6e74 2069   first element i
+000078f0: 7320 7468 6520 7375 7065 7263 656c 6c20  s the supercell 
+00007900: 6174 6f6d 2069 6e64 6578 2073 7461 7274  atom index start
+00007910: 696e 6720 7769 7468 2030 2e0a 2020 2020  ing with 0..    
+00007920: 2020 2020 2020 2020 5468 6520 7265 6d61          The rema
+00007930: 696e 696e 6720 7468 7265 6520 656c 656d  ining three elem
+00007940: 656e 7473 2067 6976 6520 7468 6520 6469  ents give the di
+00007950: 7370 6c61 6365 6d65 6e74 2069 6e20 4361  splacement in Ca
+00007960: 7274 6573 6961 6e0a 2020 2020 2020 2020  rtesian.        
+00007970: 2020 2020 636f 6f72 6469 6e61 7465 732e      coordinates.
+00007980: 0a20 2020 2020 2020 2054 7970 652d 322c  .        Type-2,
+00007990: 2061 7272 6179 5f6c 696b 650a 2020 2020   array_like.    
+000079a0: 2020 2020 2020 2020 4469 7370 6c61 6365          Displace
+000079b0: 6d65 6e74 7320 6f66 2061 6c6c 2061 746f  ments of all ato
+000079c0: 6d73 206f 6620 616c 6c20 7375 7065 7263  ms of all superc
+000079d0: 656c 6c73 2069 6e20 4361 7274 6573 6961  ells in Cartesia
+000079e0: 6e0a 2020 2020 2020 2020 2020 2020 636f  n.            co
+000079f0: 6f72 6469 6e61 7465 732e 0a20 2020 2020  ordinates..     
+00007a00: 2020 2020 2020 2073 6861 7065 3d28 7375         shape=(su
+00007a10: 7065 7263 656c 6c73 2c20 6e61 746f 6d2c  percells, natom,
+00007a20: 2033 290a 2020 2020 2020 2020 2020 2020   3).            
+00007a30: 6474 7970 653d 2764 6f75 626c 6527 0a0a  dtype='double'..
+00007a40: 0a20 2020 2020 2020 2046 6f72 2073 6574  .        For set
+00007a50: 7465 722c 206f 6e6c 7920 7479 7065 2d32  ter, only type-2
+00007a60: 2064 6174 6173 6574 2066 6f72 6d61 7420   dataset format 
+00007a70: 6973 2061 6c6c 6f77 6564 2e0a 0a20 2020  is allowed...   
+00007a80: 2020 2020 2064 6973 706c 6163 656d 656e       displacemen
+00007a90: 7473 203a 2061 7272 6179 5f6c 696b 650a  ts : array_like.
+00007aa0: 2020 2020 2020 2020 2020 2020 4174 6f6d              Atom
+00007ab0: 6963 2064 6973 706c 6163 656d 656e 7473  ic displacements
+00007ac0: 206f 6620 616c 6c20 6174 6f6d 7320 6f66   of all atoms of
+00007ad0: 2061 6c6c 2073 7570 6572 6365 6c6c 732e   all supercells.
+00007ae0: 0a20 2020 2020 2020 2020 2020 204f 6e6c  .            Onl
+00007af0: 7920 616c 6c20 6469 7370 6c61 6365 6d65  y all displaceme
+00007b00: 6e74 7320 696e 2065 6163 6820 7375 7065  nts in each supe
+00007b10: 7263 656c 6c20 6361 7365 2028 7479 7065  rcell case (type
+00007b20: 2d32 2920 6973 0a20 2020 2020 2020 2020  -2) is.         
+00007b30: 2020 2073 7570 706f 7274 6564 2e0a 2020     supported..  
+00007b40: 2020 2020 2020 2020 2020 7368 6170 653d            shape=
+00007b50: 2873 7570 6572 6365 6c6c 732c 206e 6174  (supercells, nat
+00007b60: 6f6d 2c20 3329 2c20 6474 7970 653d 2764  om, 3), dtype='d
+00007b70: 6f75 626c 6527 2c20 6f72 6465 723d 2743  ouble', order='C
+00007b80: 270a 0a20 2020 2020 2020 2022 2222 0a20  '..        """. 
+00007b90: 2020 2020 2020 2069 6620 7365 6c66 2e5f         if self._
+00007ba0: 7068 6f6e 6f6e 5f73 7570 6572 6365 6c6c  phonon_supercell
+00007bb0: 5f6d 6174 7269 7820 6973 204e 6f6e 653a  _matrix is None:
+00007bc0: 0a20 2020 2020 2020 2020 2020 2072 6169  .            rai
+00007bd0: 7365 2052 756e 7469 6d65 4572 726f 7228  se RuntimeError(
+00007be0: 2270 686f 6e6f 6e5f 7375 7065 7263 656c  "phonon_supercel
+00007bf0: 6c5f 6d61 7472 6978 2069 7320 6e6f 7420  l_matrix is not 
+00007c00: 7365 742e 2229 0a0a 2020 2020 2020 2020  set.")..        
+00007c10: 6461 7461 7365 7420 3d20 7365 6c66 2e5f  dataset = self._
+00007c20: 7068 6f6e 6f6e 5f64 6174 6173 6574 0a20  phonon_dataset. 
+00007c30: 2020 2020 2020 2069 6620 2266 6972 7374         if "first
+00007c40: 5f61 746f 6d73 2220 696e 2064 6174 6173  _atoms" in datas
+00007c50: 6574 3a0a 2020 2020 2020 2020 2020 2020  et:.            
+00007c60: 6e75 6d5f 7363 656c 6c73 203d 206c 656e  num_scells = len
+00007c70: 2864 6174 6173 6574 5b22 6669 7273 745f  (dataset["first_
+00007c80: 6174 6f6d 7322 5d29 0a20 2020 2020 2020  atoms"]).       
+00007c90: 2020 2020 206e 6174 6f6d 203d 206c 656e       natom = len
+00007ca0: 2873 656c 662e 5f70 686f 6e6f 6e5f 7375  (self._phonon_su
+00007cb0: 7065 7263 656c 6c29 0a20 2020 2020 2020  percell).       
+00007cc0: 2020 2020 2064 6973 706c 6163 656d 656e       displacemen
+00007cd0: 7473 203d 206e 702e 7a65 726f 7328 286e  ts = np.zeros((n
+00007ce0: 756d 5f73 6365 6c6c 732c 206e 6174 6f6d  um_scells, natom
+00007cf0: 2c20 3329 2c20 6474 7970 653d 2264 6f75  , 3), dtype="dou
+00007d00: 626c 6522 2c20 6f72 6465 723d 2243 2229  ble", order="C")
+00007d10: 0a20 2020 2020 2020 2020 2020 2066 6f72  .            for
+00007d20: 2069 2c20 6469 7370 3120 696e 2065 6e75   i, disp1 in enu
+00007d30: 6d65 7261 7465 2864 6174 6173 6574 5b22  merate(dataset["
+00007d40: 6669 7273 745f 6174 6f6d 7322 5d29 3a0a  first_atoms"]):.
+00007d50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007d60: 6469 7370 6c61 6365 6d65 6e74 735b 692c  displacements[i,
+00007d70: 2064 6973 7031 5b22 6e75 6d62 6572 225d   disp1["number"]
+00007d80: 5d20 3d20 6469 7370 315b 2264 6973 706c  ] = disp1["displ
+00007d90: 6163 656d 656e 7422 5d0a 2020 2020 2020  acement"].      
+00007da0: 2020 656c 6966 2022 666f 7263 6573 2220    elif "forces" 
+00007db0: 696e 2064 6174 6173 6574 206f 7220 2264  in dataset or "d
+00007dc0: 6973 706c 6163 656d 656e 7473 2220 696e  isplacements" in
+00007dd0: 2064 6174 6173 6574 3a0a 2020 2020 2020   dataset:.      
+00007de0: 2020 2020 2020 6469 7370 6c61 6365 6d65        displaceme
+00007df0: 6e74 7320 3d20 6461 7461 7365 745b 2264  nts = dataset["d
+00007e00: 6973 706c 6163 656d 656e 7473 225d 0a20  isplacements"]. 
+00007e10: 2020 2020 2020 2065 6c73 653a 0a20 2020         else:.   
+00007e20: 2020 2020 2020 2020 2072 6169 7365 2052           raise R
+00007e30: 756e 7469 6d65 4572 726f 7228 2264 6973  untimeError("dis
+00007e40: 706c 6163 656d 656e 7420 6461 7461 7365  placement datase
+00007e50: 7420 6861 7320 7772 6f6e 6720 666f 726d  t has wrong form
+00007e60: 6174 2e22 290a 0a20 2020 2020 2020 2072  at.")..        r
+00007e70: 6574 7572 6e20 6469 7370 6c61 6365 6d65  eturn displaceme
+00007e80: 6e74 730a 0a20 2020 2040 7068 6f6e 6f6e  nts..    @phonon
+00007e90: 5f64 6973 706c 6163 656d 656e 7473 2e73  _displacements.s
+00007ea0: 6574 7465 720a 2020 2020 6465 6620 7068  etter.    def ph
+00007eb0: 6f6e 6f6e 5f64 6973 706c 6163 656d 656e  onon_displacemen
+00007ec0: 7473 2873 656c 662c 2064 6973 706c 6163  ts(self, displac
+00007ed0: 656d 656e 7473 293a 0a20 2020 2020 2020  ements):.       
+00007ee0: 2069 6620 7365 6c66 2e5f 7068 6f6e 6f6e   if self._phonon
+00007ef0: 5f73 7570 6572 6365 6c6c 5f6d 6174 7269  _supercell_matri
+00007f00: 7820 6973 204e 6f6e 653a 0a20 2020 2020  x is None:.     
+00007f10: 2020 2020 2020 2072 6169 7365 2052 756e         raise Run
+00007f20: 7469 6d65 4572 726f 7228 2270 686f 6e6f  timeError("phono
+00007f30: 6e5f 7375 7065 7263 656c 6c5f 6d61 7472  n_supercell_matr
+00007f40: 6978 2069 7320 6e6f 7420 7365 742e 2229  ix is not set.")
+00007f50: 0a0a 2020 2020 2020 2020 6469 7370 7320  ..        disps 
+00007f60: 3d20 6e70 2e61 7272 6179 2864 6973 706c  = np.array(displ
+00007f70: 6163 656d 656e 7473 2c20 6474 7970 653d  acements, dtype=
+00007f80: 2264 6f75 626c 6522 2c20 6f72 6465 723d  "double", order=
+00007f90: 2243 2229 0a20 2020 2020 2020 206e 6174  "C").        nat
+00007fa0: 6f6d 203d 206c 656e 2873 656c 662e 5f70  om = len(self._p
+00007fb0: 686f 6e6f 6e5f 7375 7065 7263 656c 6c29  honon_supercell)
+00007fc0: 0a20 2020 2020 2020 2069 6620 6469 7370  .        if disp
+00007fd0: 732e 6e64 696d 2021 3d20 3320 6f72 2064  s.ndim != 3 or d
+00007fe0: 6973 7073 2e73 6861 7065 5b31 3a5d 2021  isps.shape[1:] !
+00007ff0: 3d20 286e 6174 6f6d 2c20 3329 3a0a 2020  = (natom, 3):.  
+00008000: 2020 2020 2020 2020 2020 7261 6973 6520            raise 
+00008010: 5275 6e74 696d 6545 7272 6f72 2822 4172  RuntimeError("Ar
+00008020: 7261 7920 7368 6170 6520 6f66 2064 6973  ray shape of dis
+00008030: 706c 6163 656d 656e 7473 2069 7320 696e  placements is in
+00008040: 636f 7272 6563 742e 2229 0a20 2020 2020  correct.").     
+00008050: 2020 2069 6620 7365 6c66 2e5f 7068 6f6e     if self._phon
+00008060: 6f6e 5f64 6174 6173 6574 2069 7320 4e6f  on_dataset is No
+00008070: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
+00008080: 7365 6c66 2e5f 7068 6f6e 6f6e 5f64 6174  self._phonon_dat
+00008090: 6173 6574 203d 207b 7d0a 2020 2020 2020  aset = {}.      
+000080a0: 2020 656c 6966 2022 6669 7273 745f 6174    elif "first_at
+000080b0: 6f6d 7322 2069 6e20 7365 6c66 2e5f 7068  oms" in self._ph
+000080c0: 6f6e 6f6e 5f64 6174 6173 6574 3a0a 2020  onon_dataset:.  
+000080d0: 2020 2020 2020 2020 2020 7261 6973 6520            raise 
+000080e0: 5275 6e74 696d 6545 7272 6f72 2822 4469  RuntimeError("Di
+000080f0: 7370 6c61 6365 6d65 6e74 7320 6172 6520  splacements are 
+00008100: 696e 636f 6d70 6174 6962 6c65 2077 6974  incompatible wit
+00008110: 6820 6461 7461 7365 742e 2229 0a0a 2020  h dataset.")..  
+00008120: 2020 2020 2020 7365 6c66 2e5f 7068 6f6e        self._phon
+00008130: 6f6e 5f64 6174 6173 6574 5b22 6469 7370  on_dataset["disp
+00008140: 6c61 6365 6d65 6e74 7322 5d20 3d20 6469  lacements"] = di
+00008150: 7370 730a 2020 2020 2020 2020 7365 6c66  sps.        self
+00008160: 2e5f 7068 6f6e 6f6e 5f73 7570 6572 6365  ._phonon_superce
+00008170: 6c6c 735f 7769 7468 5f64 6973 706c 6163  lls_with_displac
+00008180: 656d 656e 7473 203d 204e 6f6e 650a 0a20  ements = None.. 
+00008190: 2020 2040 7072 6f70 6572 7479 0a20 2020     @property.   
+000081a0: 2064 6566 2070 686f 6e6f 6e5f 666f 7263   def phonon_forc
+000081b0: 6573 2873 656c 6629 3a0a 2020 2020 2020  es(self):.      
+000081c0: 2020 2222 2253 6574 7465 7220 616e 6420    """Setter and 
+000081d0: 6765 7474 6572 206f 6620 666f 7263 6573  getter of forces
+000081e0: 2069 6e20 6663 3220 6469 7370 6c61 6365   in fc2 displace
+000081f0: 6d65 6e74 2064 6174 6173 6574 2e0a 0a20  ment dataset... 
+00008200: 2020 2020 2020 2041 2073 6574 206f 6620         A set of 
+00008210: 6174 6f6d 6963 2066 6f72 6365 7320 696e  atomic forces in
+00008220: 2064 6973 706c 6163 6564 2073 7570 6572   displaced super
+00008230: 6365 6c6c 732e 2054 6865 206f 7264 6572  cells. The order
+00008240: 206f 660a 2020 2020 2020 2020 6469 7370   of.        disp
+00008250: 6c61 6365 6420 7375 7065 7263 656c 6c73  laced supercells
+00008260: 2068 6173 2074 6f20 6d61 7463 6820 7769   has to match wi
+00008270: 7468 2074 6861 7420 696e 2070 686f 6e6f  th that in phono
+00008280: 6e20 6469 7370 6c61 6365 6d65 6e74 0a20  n displacement. 
+00008290: 2020 2020 2020 2064 6174 6173 6574 2e0a         dataset..
+000082a0: 2020 2020 2020 2020 7368 6170 653d 2864          shape=(d
+000082b0: 6973 706c 6163 6564 2073 7570 6572 6365  isplaced superce
+000082c0: 6c6c 732c 2061 746f 6d73 2069 6e20 7375  lls, atoms in su
+000082d0: 7065 7263 656c 6c2c 2033 290a 0a20 2020  percell, 3)..   
+000082e0: 2020 2020 2067 6574 7465 7220 3a20 6e64       getter : nd
+000082f0: 6172 7261 790a 0a20 2020 2020 2020 2073  array..        s
+00008300: 6574 7465 7220 3a20 6172 7261 795f 6c69  etter : array_li
+00008310: 6b65 0a20 2020 2020 2020 2020 2020 2054  ke.            T
+00008320: 6865 206f 7264 6572 206f 6620 7375 7065  he order of supe
+00008330: 7263 656c 6c73 2075 7365 6420 666f 7220  rcells used for 
+00008340: 6361 6c63 756c 6174 696e 6720 666f 7263  calculating forc
+00008350: 6573 2068 6173 2074 6f0a 2020 2020 2020  es has to.      
+00008360: 2020 2020 2020 6265 2074 6865 2073 616d        be the sam
+00008370: 6520 6f72 6465 7220 6f66 2070 686f 6e6f  e order of phono
+00008380: 6e5f 7375 7065 7263 656c 6c73 5f77 6974  n_supercells_wit
+00008390: 685f 6469 7370 6c61 6365 6d65 6e74 732e  h_displacements.
+000083a0: 0a0a 2020 2020 2020 2020 2222 220a 2020  ..        """.  
+000083b0: 2020 2020 2020 7265 7475 726e 2073 656c        return sel
+000083c0: 662e 5f67 6574 5f70 686f 6e6f 6e5f 666f  f._get_phonon_fo
+000083d0: 7263 6573 5f65 6e65 7267 6965 7328 7461  rces_energies(ta
+000083e0: 7267 6574 3d22 666f 7263 6573 2229 0a0a  rget="forces")..
+000083f0: 2020 2020 4070 686f 6e6f 6e5f 666f 7263      @phonon_forc
+00008400: 6573 2e73 6574 7465 720a 2020 2020 6465  es.setter.    de
+00008410: 6620 7068 6f6e 6f6e 5f66 6f72 6365 7328  f phonon_forces(
+00008420: 7365 6c66 2c20 7661 6c75 6573 293a 0a20  self, values):. 
+00008430: 2020 2020 2020 2073 656c 662e 5f73 6574         self._set
+00008440: 5f70 686f 6e6f 6e5f 666f 7263 6573 5f65  _phonon_forces_e
+00008450: 6e65 7267 6965 7328 7661 6c75 6573 2c20  nergies(values, 
+00008460: 7461 7267 6574 3d22 666f 7263 6573 2229  target="forces")
+00008470: 0a0a 2020 2020 4070 726f 7065 7274 790a  ..    @property.
+00008480: 2020 2020 6465 6620 7068 6f6e 6f6e 5f73      def phonon_s
+00008490: 7570 6572 6365 6c6c 5f65 6e65 7267 6965  upercell_energie
+000084a0: 7328 7365 6c66 293a 0a20 2020 2020 2020  s(self):.       
+000084b0: 2022 2222 5365 7474 6572 2061 6e64 2067   """Setter and g
+000084c0: 6574 7465 7220 6f66 2073 7570 6572 6365  etter of superce
+000084d0: 6c6c 2065 6e65 7267 6965 7320 696e 2066  ll energies in f
+000084e0: 6332 2064 6973 706c 6163 656d 656e 7420  c2 displacement 
+000084f0: 6461 7461 7365 742e 0a0a 2020 2020 2020  dataset...      
+00008500: 2020 7368 6170 653d 2864 6973 706c 6163    shape=(displac
+00008510: 6564 2073 7570 6572 6365 6c6c 732c 290a  ed supercells,).
+00008520: 0a20 2020 2020 2020 2067 6574 7465 7220  .        getter 
+00008530: 3a20 6e64 6172 7261 790a 0a20 2020 2020  : ndarray..     
+00008540: 2020 2073 6574 7465 7220 3a20 6172 7261     setter : arra
+00008550: 795f 6c69 6b65 0a20 2020 2020 2020 2020  y_like.         
+00008560: 2020 2054 6865 206f 7264 6572 206f 6620     The order of 
+00008570: 7375 7065 7263 656c 6c73 2075 7365 6420  supercells used 
+00008580: 666f 7220 6361 6c63 756c 6174 696e 6720  for calculating 
+00008590: 7375 7065 7263 656c 6c20 656e 6572 6769  supercell energi
+000085a0: 6573 2068 6173 0a20 2020 2020 2020 2020  es has.         
+000085b0: 2020 2074 6f20 6265 2074 6865 2073 616d     to be the sam
+000085c0: 6520 6f72 6465 7220 6f66 2070 686f 6e6f  e order of phono
+000085d0: 6e5f 7375 7065 7263 656c 6c73 5f77 6974  n_supercells_wit
+000085e0: 685f 6469 7370 6c61 6365 6d65 6e74 732e  h_displacements.
+000085f0: 0a0a 2020 2020 2020 2020 2222 220a 2020  ..        """.  
+00008600: 2020 2020 2020 7265 7475 726e 2073 656c        return sel
+00008610: 662e 5f67 6574 5f70 686f 6e6f 6e5f 666f  f._get_phonon_fo
+00008620: 7263 6573 5f65 6e65 7267 6965 7328 7461  rces_energies(ta
+00008630: 7267 6574 3d22 7375 7065 7263 656c 6c5f  rget="supercell_
+00008640: 656e 6572 6769 6573 2229 0a0a 2020 2020  energies")..    
+00008650: 4070 686f 6e6f 6e5f 7375 7065 7263 656c  @phonon_supercel
+00008660: 6c5f 656e 6572 6769 6573 2e73 6574 7465  l_energies.sette
+00008670: 720a 2020 2020 6465 6620 7068 6f6e 6f6e  r.    def phonon
+00008680: 5f73 7570 6572 6365 6c6c 5f65 6e65 7267  _supercell_energ
+00008690: 6965 7328 7365 6c66 2c20 7661 6c75 6573  ies(self, values
+000086a0: 293a 0a20 2020 2020 2020 2073 656c 662e  ):.        self.
+000086b0: 5f73 6574 5f70 686f 6e6f 6e5f 666f 7263  _set_phonon_forc
+000086c0: 6573 5f65 6e65 7267 6965 7328 7661 6c75  es_energies(valu
+000086d0: 6573 2c20 7461 7267 6574 3d22 7375 7065  es, target="supe
+000086e0: 7263 656c 6c5f 656e 6572 6769 6573 2229  rcell_energies")
+000086f0: 0a0a 2020 2020 4070 726f 7065 7274 790a  ..    @property.
+00008700: 2020 2020 6465 6620 7068 7068 5f69 6e74      def phph_int
+00008710: 6572 6163 7469 6f6e 2873 656c 6629 3a0a  eraction(self):.
+00008720: 2020 2020 2020 2020 2222 2252 6574 7572          """Retur
+00008730: 6e20 496e 7465 7261 6374 696f 6e20 696e  n Interaction in
+00008740: 7374 616e 6365 2e22 2222 0a20 2020 2020  stance.""".     
+00008750: 2020 2072 6574 7572 6e20 7365 6c66 2e5f     return self._
+00008760: 696e 7465 7261 6374 696f 6e0a 0a20 2020  interaction..   
+00008770: 2040 7072 6f70 6572 7479 0a20 2020 2064   @property.    d
+00008780: 6566 2064 6574 6169 6c65 645f 6761 6d6d  ef detailed_gamm
+00008790: 6173 2873 656c 6629 3a0a 2020 2020 2020  as(self):.      
+000087a0: 2020 2222 2252 6574 7572 6e20 6465 7461    """Return deta
+000087b0: 696c 6564 2067 616d 6d61 2e22 2222 0a20  iled gamma.""". 
+000087c0: 2020 2020 2020 2072 6574 7572 6e20 7365         return se
+000087d0: 6c66 2e5f 6465 7461 696c 6564 5f67 616d  lf._detailed_gam
+000087e0: 6d61 730a 0a20 2020 2040 7072 6f70 6572  mas..    @proper
+000087f0: 7479 0a20 2020 2064 6566 2067 7269 6428  ty.    def grid(
+00008800: 7365 6c66 293a 0a20 2020 2020 2020 2022  self):.        "
+00008810: 2222 5265 7475 726e 2042 7269 6c6c 6f75  ""Return Brillou
+00008820: 696e 207a 6f6e 6520 6772 6964 2069 6e66  in zone grid inf
+00008830: 6f72 6d61 7469 6f6e 2e0a 0a20 2020 2020  ormation...     
+00008840: 2020 2042 5a47 7269 640a 2020 2020 2020     BZGrid.      
+00008850: 2020 2020 2020 416e 2069 6e73 7461 6e63        An instanc
+00008860: 6520 6f66 2042 5a47 7269 6420 7573 6564  e of BZGrid used
+00008870: 2066 6f72 2065 6e74 6972 6520 7068 6f6e   for entire phon
+00008880: 6f33 7079 2063 616c 6375 6c61 7469 6f6e  o3py calculation
+00008890: 2e0a 0a20 2020 2020 2020 2022 2222 0a20  ...        """. 
+000088a0: 2020 2020 2020 2072 6574 7572 6e20 7365         return se
+000088b0: 6c66 2e5f 627a 5f67 7269 640a 0a20 2020  lf._bz_grid..   
+000088c0: 2064 6566 2069 6e69 745f 7068 7068 5f69   def init_phph_i
+000088d0: 6e74 6572 6163 7469 6f6e 280a 2020 2020  nteraction(.    
+000088e0: 2020 2020 7365 6c66 2c0a 2020 2020 2020      self,.      
+000088f0: 2020 6e61 635f 715f 6469 7265 6374 696f    nac_q_directio
+00008900: 6e3d 4e6f 6e65 2c0a 2020 2020 2020 2020  n=None,.        
+00008910: 636f 6e73 7461 6e74 5f61 7665 7261 6765  constant_average
+00008920: 645f 696e 7465 7261 6374 696f 6e3d 4e6f  d_interaction=No
+00008930: 6e65 2c0a 2020 2020 2020 2020 6672 6571  ne,.        freq
+00008940: 7565 6e63 795f 7363 616c 655f 6661 6374  uency_scale_fact
+00008950: 6f72 3d4e 6f6e 652c 0a20 2020 2020 2020  or=None,.       
+00008960: 2073 796d 6d65 7472 697a 655f 6663 3371   symmetrize_fc3q
+00008970: 3a20 626f 6f6c 203d 2046 616c 7365 2c0a  : bool = False,.
+00008980: 2020 2020 2020 2020 6c61 7061 636b 5f7a          lapack_z
+00008990: 6865 6576 5f75 706c 6f3d 224c 222c 0a20  heev_uplo="L",. 
+000089a0: 2020 2020 2020 206f 7065 6e6d 705f 7065         openmp_pe
+000089b0: 725f 7472 6970 6c65 7473 3d4e 6f6e 652c  r_triplets=None,
+000089c0: 0a20 2020 2029 3a0a 2020 2020 2020 2020  .    ):.        
+000089d0: 2222 2249 6e69 7469 616c 697a 6520 7068  """Initialize ph
+000089e0: 2d70 6820 696e 7465 7261 6374 696f 6e20  -ph interaction 
+000089f0: 6361 6c63 756c 6174 696f 6e2e 0a0a 2020  calculation...  
+00008a00: 2020 2020 2020 5468 6973 206d 6574 686f        This metho
+00008a10: 6420 6372 6561 7465 7320 616e 2069 6e73  d creates an ins
+00008a20: 7461 6e63 6520 6f66 2049 6e74 6572 6163  tance of Interac
+00008a30: 7469 6f6e 2063 6c61 7373 2c20 7768 6963  tion class, whic
+00008a40: 680a 2020 2020 2020 2020 6973 206e 6563  h.        is nec
+00008a50: 6573 7361 7279 2074 6f20 7275 6e20 7068  essary to run ph
+00008a60: 2d70 6820 696e 7465 7261 6374 696f 6e20  -ph interaction 
+00008a70: 6361 6c63 756c 6174 696f 6e2e 0a20 2020  calculation..   
+00008a80: 2020 2020 2054 6865 2069 6e70 7574 2064       The input d
+00008a90: 6174 6120 7375 6368 2061 7320 6772 6964  ata such as grid
+00008aa0: 732c 2066 6f72 6365 2063 6f6e 7374 616e  s, force constan
+00008ab0: 7473 2c20 6574 632c 2061 7265 0a20 2020  ts, etc, are.   
+00008ac0: 2020 2020 2073 746f 7265 6420 746f 2062       stored to b
+00008ad0: 6520 7265 6164 7920 666f 7220 7468 6520  e ready for the 
+00008ae0: 6361 6c63 756c 6174 696f 6e2e 0a0a 2020  calculation...  
+00008af0: 2020 2020 2020 4e6f 7465 0a20 2020 2020        Note.     
+00008b00: 2020 202d 2d2d 2d0a 2020 2020 2020 2020     ----.        
+00008b10: 6663 3320 616e 6420 6663 322c 2061 6e64  fc3 and fc2, and
+00008b20: 206f 7074 696f 6e61 6c6c 7920 6e61 635f   optionally nac_
+00008b30: 7061 7261 6d73 2068 6176 6520 746f 2062  params have to b
+00008b40: 6520 7365 7420 6265 666f 7265 2063 616c  e set before cal
+00008b50: 6c69 6e67 0a20 2020 2020 2020 2074 6869  ling.        thi
+00008b60: 7320 6d65 7468 6f64 2e20 6663 3320 616e  s method. fc3 an
+00008b70: 6420 6663 3220 6361 6e20 6265 206d 6164  d fc2 can be mad
+00008b80: 6520 6569 7468 6572 2066 726f 6d20 7365  e either from se
+00008b90: 7473 206f 6620 666f 7263 6573 0a20 2020  ts of forces.   
+00008ba0: 2020 2020 2061 6e64 2064 6973 706c 6163       and displac
+00008bb0: 656d 656e 7473 206f 6620 7375 7065 7263  ements of superc
+00008bc0: 656c 6c73 206f 7220 6265 2073 6574 2073  ells or be set s
+00008bd0: 696d 706c 7920 7669 6120 6174 7472 6962  imply via attrib
+00008be0: 7574 6573 2e0a 0a20 2020 2020 2020 2050  utes...        P
+00008bf0: 6172 616d 6574 6572 730a 2020 2020 2020  arameters.      
+00008c00: 2020 2d2d 2d2d 2d2d 2d2d 2d2d 0a20 2020    ----------.   
+00008c10: 2020 2020 206e 6163 5f71 5f64 6972 6563       nac_q_direc
+00008c20: 7469 6f6e 203a 2061 7272 6179 5f6c 696b  tion : array_lik
+00008c30: 652c 206f 7074 696f 6e61 6c0a 2020 2020  e, optional.    
+00008c40: 2020 2020 2020 2020 4469 7265 6374 696f          Directio
+00008c50: 6e20 6f66 2071 2d76 6563 746f 7220 7761  n of q-vector wa
+00008c60: 7463 6869 6e67 2066 726f 6d20 4761 6d6d  tching from Gamm
+00008c70: 6120 706f 696e 7420 7573 6564 2066 6f72  a point used for
+00008c80: 0a20 2020 2020 2020 2020 2020 206e 6f6e  .            non
+00008c90: 2d61 6e61 6c79 7469 6361 6c20 7465 726d  -analytical term
+00008ca0: 2063 6f72 7265 6374 696f 6e2e 2054 6869   correction. Thi
+00008cb0: 7320 6973 2065 6666 6563 7469 7665 206f  s is effective o
+00008cc0: 6e6c 7920 6174 2071 3d30 0a20 2020 2020  nly at q=0.     
+00008cd0: 2020 2020 2020 2028 7068 7973 6963 616c         (physical
+00008ce0: 6c79 2071 2d3e 3029 2e20 5468 6520 6469  ly q->0). The di
+00008cf0: 7265 6374 696f 6e20 6973 2067 6976 656e  rection is given
+00008d00: 2069 6e20 6372 7973 7461 6c6c 6f67 7261   in crystallogra
+00008d10: 7068 6963 0a20 2020 2020 2020 2020 2020  phic.           
+00008d20: 2028 6672 6163 7469 6f6e 616c 2920 636f   (fractional) co
+00008d30: 6f72 6469 6e61 7465 732e 0a20 2020 2020  ordinates..     
+00008d40: 2020 2020 2020 2073 6861 7065 3d28 332c         shape=(3,
+00008d50: 292c 2064 7479 7065 3d27 646f 7562 6c65  ), dtype='double
+00008d60: 272e 0a20 2020 2020 2020 2020 2020 2044  '..            D
+00008d70: 6566 6175 6c74 2076 616c 7565 2069 7320  efault value is 
+00008d80: 4e6f 6e65 2c20 7768 6963 6820 6d65 616e  None, which mean
+00008d90: 7320 7468 6973 2066 6561 7475 7265 2069  s this feature i
+00008da0: 7320 6e6f 7420 7573 6564 2e0a 2020 2020  s not used..    
+00008db0: 2020 2020 636f 6e73 7461 6e74 5f61 7665      constant_ave
+00008dc0: 7261 6765 645f 696e 7465 7261 6374 696f  raged_interactio
+00008dd0: 6e20 3a20 666c 6f61 742c 206f 7074 696f  n : float, optio
+00008de0: 6e61 6c0a 2020 2020 2020 2020 2020 2020  nal.            
+00008df0: 5068 2d70 6820 696e 7465 7261 6374 696f  Ph-ph interactio
+00008e00: 6e20 7374 7265 6e67 7468 2061 7272 6179  n strength array
+00008e10: 2069 7320 7265 706c 6163 6564 2062 7920   is replaced by 
+00008e20: 6120 7363 616c 6172 2076 616c 7565 2e0a  a scalar value..
+00008e30: 2020 2020 2020 2020 2020 2020 4465 6661              Defa
+00008e40: 756c 7420 6973 204e 6f6e 652c 2077 6869  ult is None, whi
+00008e50: 6368 206d 6561 6e73 2074 6869 7320 6665  ch means this fe
+00008e60: 6174 7572 6520 6973 206e 6f74 2075 7365  ature is not use
+00008e70: 642e 0a20 2020 2020 2020 2066 7265 7175  d..        frequ
+00008e80: 656e 6379 5f73 6361 6c65 5f66 6163 746f  ency_scale_facto
+00008e90: 7220 3a20 666c 6f61 742c 206f 7074 696f  r : float, optio
+00008ea0: 6e61 6c0a 2020 2020 2020 2020 2020 2020  nal.            
+00008eb0: 416c 6c20 7068 6f6e 6f6e 2066 7265 7175  All phonon frequ
+00008ec0: 656e 6365 7320 6172 6520 7363 616c 6564  ences are scaled
+00008ed0: 2062 7920 7468 6973 2076 616c 7565 2e20   by this value. 
+00008ee0: 4465 6661 756c 7420 6973 204e 6f6e 652c  Default is None,
+00008ef0: 0a20 2020 2020 2020 2020 2020 2077 6869  .            whi
+00008f00: 6368 206d 6561 6e73 2070 686f 6e6f 6e20  ch means phonon 
+00008f10: 6672 6571 7565 6e63 6965 7320 6172 6520  frequencies are 
+00008f20: 6e6f 7420 7363 616c 6564 2e0a 2020 2020  not scaled..    
+00008f30: 2020 2020 7379 6d6d 6574 7269 7a65 5f66      symmetrize_f
+00008f40: 6333 7120 3a20 626f 6f6c 2c20 6f70 7469  c3q : bool, opti
+00008f50: 6f6e 616c 0a20 2020 2020 2020 2020 2020  onal.           
+00008f60: 2066 6333 2069 6e20 7068 6f6e 6f6e 2073   fc3 in phonon s
+00008f70: 7061 6365 2069 7320 7379 6d6d 6574 7269  pace is symmetri
+00008f80: 7a65 6420 6279 2070 6572 6d75 7461 7469  zed by permutati
+00008f90: 6f6e 2073 796d 6d65 7472 792e 0a20 2020  on symmetry..   
+00008fa0: 2020 2020 2020 2020 2044 6566 6175 6c74           Default
+00008fb0: 2069 7320 4661 6c73 652e 0a20 2020 2020   is False..     
+00008fc0: 2020 206c 6170 6163 6b5f 7a68 6565 765f     lapack_zheev_
+00008fd0: 7570 6c6f 203a 2073 7472 2c20 6f70 7469  uplo : str, opti
+00008fe0: 6f6e 616c 0a20 2020 2020 2020 2020 2020  onal.           
+00008ff0: 2027 4c27 206f 7220 2755 272e 2044 6566   'L' or 'U'. Def
+00009000: 6175 6c74 2069 7320 274c 272e 2054 6869  ault is 'L'. Thi
+00009010: 7320 6973 2070 6173 7365 6420 746f 204c  s is passed to L
+00009020: 4150 4143 4b20 7a68 6565 760a 2020 2020  APACK zheev.    
+00009030: 2020 2020 2020 2020 7573 6564 2066 6f72          used for
+00009040: 2070 686f 6e6f 6e20 736f 6c76 6572 2e0a   phonon solver..
+00009050: 2020 2020 2020 2020 6f70 656e 6d70 5f70          openmp_p
+00009060: 6572 5f74 7269 706c 6574 7320 3a20 626f  er_triplets : bo
+00009070: 6f6c 206f 7220 4e6f 6e65 2c20 6f70 7469  ol or None, opti
+00009080: 6f6e 616c 2c20 6465 6661 756c 7420 6973  onal, default is
+00009090: 204e 6f6e 650a 2020 2020 2020 2020 2020   None.          
+000090a0: 2020 4e6f 726d 616c 6c79 2074 6869 7320    Normally this 
+000090b0: 7061 7261 6d65 7465 7220 7368 6f75 6c64  parameter should
+000090c0: 206e 6f74 2062 6520 746f 7563 6865 642e   not be touched.
+000090d0: 0a20 2020 2020 2020 2020 2020 2057 6865  .            Whe
+000090e0: 6e20 6054 7275 6560 2c20 7068 2d70 6820  n `True`, ph-ph 
+000090f0: 696e 7465 7261 6374 696f 6e20 7374 7265  interaction stre
+00009100: 6e67 7468 2063 616c 6375 6c61 7469 6f6e  ngth calculation
+00009110: 2072 756e 7320 7769 7468 0a20 2020 2020   runs with.     
+00009120: 2020 2020 2020 204f 7065 6e4d 5020 6469         OpenMP di
+00009130: 7374 7269 6275 7469 6f6e 206f 7665 7220  stribution over 
+00009140: 7472 6970 6c65 7473 2c20 616e 6420 6f76  triplets, and ov
+00009150: 6572 2062 616e 6473 2077 6865 6e20 6046  er bands when `F
+00009160: 616c 7365 602e 0a20 2020 2020 2020 2020  alse`..         
+00009170: 2020 2060 4e6f 6e65 6020 7769 6c6c 2063     `None` will c
+00009180: 686f 6f73 6520 6f6e 6520 6f66 2074 6865  hoose one of the
+00009190: 6d20 6175 746f 6d61 7469 6361 6c6c 792e  m automatically.
+000091a0: 0a0a 2020 2020 2020 2020 2222 220a 2020  ..        """.  
+000091b0: 2020 2020 2020 6966 2073 656c 662e 6d65        if self.me
+000091c0: 7368 5f6e 756d 6265 7273 2069 7320 4e6f  sh_numbers is No
+000091d0: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
+000091e0: 6d73 6720 3d20 2250 686f 6e6f 3370 792e  msg = "Phono3py.
+000091f0: 6d65 7368 5f6e 756d 6265 7273 206f 6620  mesh_numbers of 
+00009200: 696e 7374 616e 6365 2068 6173 2074 6f20  instance has to 
+00009210: 6265 2073 6574 2e22 0a20 2020 2020 2020  be set.".       
+00009220: 2020 2020 2072 6169 7365 2052 756e 7469       raise Runti
+00009230: 6d65 4572 726f 7228 6d73 6729 0a0a 2020  meError(msg)..  
+00009240: 2020 2020 2020 6966 2073 656c 662e 5f66        if self._f
+00009250: 6332 2069 7320 4e6f 6e65 3a0a 2020 2020  c2 is None:.    
+00009260: 2020 2020 2020 2020 6d73 6720 3d20 2250          msg = "P
+00009270: 686f 6e6f 3370 792e 6663 3220 6f66 2069  hono3py.fc2 of i
+00009280: 6e73 7461 6e63 6520 6973 206e 6f74 2066  nstance is not f
+00009290: 6f75 6e64 2e22 0a20 2020 2020 2020 2020  ound.".         
+000092a0: 2020 2072 6169 7365 2052 756e 7469 6d65     raise Runtime
+000092b0: 4572 726f 7228 6d73 6729 0a0a 2020 2020  Error(msg)..    
+000092c0: 2020 2020 7365 6c66 2e5f 696e 7465 7261      self._intera
+000092d0: 6374 696f 6e20 3d20 496e 7465 7261 6374  ction = Interact
+000092e0: 696f 6e28 0a20 2020 2020 2020 2020 2020  ion(.           
+000092f0: 2073 656c 662e 5f70 7269 6d69 7469 7665   self._primitive
+00009300: 2c0a 2020 2020 2020 2020 2020 2020 7365  ,.            se
+00009310: 6c66 2e5f 627a 5f67 7269 642c 0a20 2020  lf._bz_grid,.   
+00009320: 2020 2020 2020 2020 2073 656c 662e 5f70           self._p
+00009330: 7269 6d69 7469 7665 5f73 796d 6d65 7472  rimitive_symmetr
+00009340: 792c 0a20 2020 2020 2020 2020 2020 2066  y,.            f
+00009350: 6333 3d73 656c 662e 5f66 6333 2c0a 2020  c3=self._fc3,.  
+00009360: 2020 2020 2020 2020 2020 6261 6e64 5f69            band_i
+00009370: 6e64 6963 6573 3d73 656c 662e 5f62 616e  ndices=self._ban
+00009380: 645f 696e 6469 6365 735f 666c 6174 7465  d_indices_flatte
+00009390: 6e2c 0a20 2020 2020 2020 2020 2020 2063  n,.            c
+000093a0: 6f6e 7374 616e 745f 6176 6572 6167 6564  onstant_averaged
+000093b0: 5f69 6e74 6572 6163 7469 6f6e 3d63 6f6e  _interaction=con
+000093c0: 7374 616e 745f 6176 6572 6167 6564 5f69  stant_averaged_i
+000093d0: 6e74 6572 6163 7469 6f6e 2c0a 2020 2020  nteraction,.    
+000093e0: 2020 2020 2020 2020 6672 6571 7565 6e63          frequenc
+000093f0: 795f 6661 6374 6f72 5f74 6f5f 5448 7a3d  y_factor_to_THz=
+00009400: 7365 6c66 2e5f 6672 6571 7565 6e63 795f  self._frequency_
+00009410: 6661 6374 6f72 5f74 6f5f 5448 7a2c 0a20  factor_to_THz,. 
+00009420: 2020 2020 2020 2020 2020 2066 7265 7175             frequ
+00009430: 656e 6379 5f73 6361 6c65 5f66 6163 746f  ency_scale_facto
+00009440: 723d 6672 6571 7565 6e63 795f 7363 616c  r=frequency_scal
+00009450: 655f 6661 6374 6f72 2c0a 2020 2020 2020  e_factor,.      
+00009460: 2020 2020 2020 6375 746f 6666 5f66 7265        cutoff_fre
+00009470: 7175 656e 6379 3d73 656c 662e 5f63 7574  quency=self._cut
+00009480: 6f66 665f 6672 6571 7565 6e63 792c 0a20  off_frequency,. 
+00009490: 2020 2020 2020 2020 2020 2069 735f 6d65             is_me
+000094a0: 7368 5f73 796d 6d65 7472 793d 7365 6c66  sh_symmetry=self
+000094b0: 2e5f 6973 5f6d 6573 685f 7379 6d6d 6574  ._is_mesh_symmet
+000094c0: 7279 2c0a 2020 2020 2020 2020 2020 2020  ry,.            
+000094d0: 7379 6d6d 6574 7269 7a65 5f66 6333 713d  symmetrize_fc3q=
+000094e0: 7379 6d6d 6574 7269 7a65 5f66 6333 712c  symmetrize_fc3q,
+000094f0: 0a20 2020 2020 2020 2020 2020 206d 616b  .            mak
+00009500: 655f 7230 5f61 7665 7261 6765 3d73 656c  e_r0_average=sel
+00009510: 662e 5f6d 616b 655f 7230 5f61 7665 7261  f._make_r0_avera
+00009520: 6765 2c0a 2020 2020 2020 2020 2020 2020  ge,.            
+00009530: 6c61 7061 636b 5f7a 6865 6576 5f75 706c  lapack_zheev_upl
+00009540: 6f3d 6c61 7061 636b 5f7a 6865 6576 5f75  o=lapack_zheev_u
+00009550: 706c 6f2c 0a20 2020 2020 2020 2020 2020  plo,.           
+00009560: 206f 7065 6e6d 705f 7065 725f 7472 6970   openmp_per_trip
+00009570: 6c65 7473 3d6f 7065 6e6d 705f 7065 725f  lets=openmp_per_
+00009580: 7472 6970 6c65 7473 2c0a 2020 2020 2020  triplets,.      
+00009590: 2020 290a 2020 2020 2020 2020 7365 6c66    ).        self
+000095a0: 2e5f 696e 7465 7261 6374 696f 6e2e 6e61  ._interaction.na
+000095b0: 635f 715f 6469 7265 6374 696f 6e20 3d20  c_q_direction = 
+000095c0: 6e61 635f 715f 6469 7265 6374 696f 6e0a  nac_q_direction.
+000095d0: 2020 2020 2020 2020 7365 6c66 2e5f 696e          self._in
+000095e0: 6974 5f64 796e 616d 6963 616c 5f6d 6174  it_dynamical_mat
+000095f0: 7269 7828 290a 0a20 2020 2064 6566 2073  rix()..    def s
+00009600: 6574 5f70 686f 6e6f 6e5f 6461 7461 2873  et_phonon_data(s
+00009610: 656c 662c 2066 7265 7175 656e 6369 6573  elf, frequencies
+00009620: 2c20 6569 6765 6e76 6563 746f 7273 2c20  , eigenvectors, 
+00009630: 6772 6964 5f61 6464 7265 7373 293a 0a20  grid_address):. 
+00009640: 2020 2020 2020 2022 2222 5365 7420 7068         """Set ph
+00009650: 6f6e 6f6e 2066 7265 7175 656e 6369 6573  onon frequencies
+00009660: 2061 6e64 2065 6967 656e 7665 6374 6f72   and eigenvector
+00009670: 7320 696e 2049 6e74 6572 6163 7469 6f6e  s in Interaction
+00009680: 2069 6e73 7461 6e63 652e 0a0a 2020 2020   instance...    
+00009690: 2020 2020 4861 726d 6f6e 6963 2070 686f      Harmonic pho
+000096a0: 6e6f 6e20 696e 666f 726d 6174 696f 6e20  non information 
+000096b0: 6973 2073 746f 7265 6420 696e 2049 6e74  is stored in Int
+000096c0: 6572 6163 7469 6f6e 2069 6e73 7461 6e63  eraction instanc
+000096d0: 652e 2046 6f72 0a20 2020 2020 2020 2065  e. For.        e
+000096e0: 7861 6d70 6c65 2c20 7468 6973 2069 6e66  xample, this inf
+000096f0: 6f72 6d61 7469 6f6e 2073 746f 7265 2069  ormation store i
+00009700: 6e20 6120 6669 6c65 2069 7320 7265 6164  n a file is read
+00009710: 2061 6e64 2070 6173 7365 6420 746f 0a20   and passed to. 
+00009720: 2020 2020 2020 2050 686f 6e6f 3370 7920         Phono3py 
+00009730: 696e 7374 616e 6365 2062 7920 7573 696e  instance by usin
+00009740: 6720 7468 6973 206d 6574 686f 642e 2054  g this method. T
+00009750: 6865 2067 7269 645f 6164 6472 6573 7320  he grid_address 
+00009760: 6973 2075 7365 640a 2020 2020 2020 2020  is used.        
+00009770: 666f 7220 7468 6520 636f 6e73 6973 7465  for the consiste
+00009780: 6e63 7920 6368 6563 6b2e 0a0a 2020 2020  ncy check...    
+00009790: 2020 2020 5061 7261 6d65 7465 7273 0a20      Parameters. 
+000097a0: 2020 2020 2020 202d 2d2d 2d2d 2d2d 2d2d         ---------
+000097b0: 2d0a 2020 2020 2020 2020 6672 6571 7565  -.        freque
+000097c0: 6e63 6965 7320 3a20 6172 7261 795f 6c69  ncies : array_li
+000097d0: 6b65 0a20 2020 2020 2020 2020 2020 2050  ke.            P
+000097e0: 686f 6e6f 6e20 6672 6571 7565 6e63 6965  honon frequencie
+000097f0: 732e 0a20 2020 2020 2020 2020 2020 2073  s..            s
+00009800: 6861 7065 3d28 6e75 6d5f 6772 6964 5f70  hape=(num_grid_p
+00009810: 6f69 6e74 732c 206e 756d 5f62 616e 6429  oints, num_band)
+00009820: 2c20 6474 7970 653d 2764 6f75 626c 6527  , dtype='double'
+00009830: 2c20 6f72 6465 723d 2743 270a 2020 2020  , order='C'.    
+00009840: 2020 2020 6569 6765 6e76 6563 746f 7273      eigenvectors
+00009850: 203a 2061 7272 6179 5f6c 696b 650a 2020   : array_like.  
+00009860: 2020 2020 2020 2020 2020 5068 6f6e 6f6e            Phonon
+00009870: 2065 6967 656e 7665 6374 6f72 730a 2020   eigenvectors.  
+00009880: 2020 2020 2020 2020 2020 7368 6170 653d            shape=
+00009890: 286e 756d 5f67 7269 645f 706f 696e 7473  (num_grid_points
+000098a0: 2c20 6e75 6d5f 6261 6e64 2c20 6e75 6d5f  , num_band, num_
+000098b0: 6261 6e64 290a 2020 2020 2020 2020 2020  band).          
+000098c0: 2020 6474 7970 653d 2763 6f6d 706c 6578    dtype='complex
+000098d0: 3132 3827 2c20 6f72 6465 723d 2743 270a  128', order='C'.
+000098e0: 2020 2020 2020 2020 6772 6964 5f61 6464          grid_add
+000098f0: 7265 7373 203a 2061 7272 6179 5f6c 696b  ress : array_lik
+00009900: 650a 2020 2020 2020 2020 2020 2020 4772  e.            Gr
+00009910: 6964 2070 6f69 6e74 2061 6464 7265 7373  id point address
+00009920: 6573 2062 7920 696e 7465 6765 7273 2e20  es by integers. 
+00009930: 5468 6520 6669 7273 7420 6469 6d65 6e73  The first dimens
+00009940: 696f 6e20 6d61 7920 6e6f 7420 6265 0a20  ion may not be. 
+00009950: 2020 2020 2020 2020 2020 2070 726f 6428             prod(
+00009960: 6d65 7368 2920 6265 6361 7573 6520 6974  mesh) because it
+00009970: 2069 6e63 6c75 6465 7320 4272 696c 6c6f   includes Brillo
+00009980: 7569 6e20 7a6f 6e65 2062 6f75 6e64 6172  uin zone boundar
+00009990: 792e 2054 6865 2064 6574 6169 6c0a 2020  y. The detail.  
+000099a0: 2020 2020 2020 2020 2020 6973 2066 6f75            is fou
+000099b0: 6e64 2069 6e20 7468 6520 646f 6373 7472  nd in the docstr
+000099c0: 696e 6720 6f66 0a20 2020 2020 2020 2020  ing of.         
+000099d0: 2020 2070 686f 6e6f 3370 792e 7068 6f6e     phono3py.phon
+000099e0: 6f6e 332e 7472 6970 6c65 7473 2e67 6574  on3.triplets.get
+000099f0: 5f74 7269 706c 6574 735f 6174 5f71 2e0a  _triplets_at_q..
+00009a00: 2020 2020 2020 2020 2020 2020 7368 6170              shap
+00009a10: 653d 286e 756d 5f67 7269 645f 706f 696e  e=(num_grid_poin
+00009a20: 7473 2c20 3329 2c20 6474 7970 653d 696e  ts, 3), dtype=in
+00009a30: 740a 0a20 2020 2020 2020 2022 2222 0a20  t..        """. 
+00009a40: 2020 2020 2020 2069 6620 7365 6c66 2e5f         if self._
+00009a50: 696e 7465 7261 6374 696f 6e20 6973 206e  interaction is n
+00009a60: 6f74 204e 6f6e 653a 0a20 2020 2020 2020  ot None:.       
+00009a70: 2020 2020 2073 656c 662e 5f69 6e74 6572       self._inter
+00009a80: 6163 7469 6f6e 2e73 6574 5f70 686f 6e6f  action.set_phono
+00009a90: 6e5f 6461 7461 2866 7265 7175 656e 6369  n_data(frequenci
+00009aa0: 6573 2c20 6569 6765 6e76 6563 746f 7273  es, eigenvectors
+00009ab0: 2c20 6772 6964 5f61 6464 7265 7373 290a  , grid_address).
+00009ac0: 0a20 2020 2064 6566 2067 6574 5f70 686f  .    def get_pho
+00009ad0: 6e6f 6e5f 6461 7461 2873 656c 6629 3a0a  non_data(self):.
+00009ae0: 2020 2020 2020 2020 2222 2247 6574 2070          """Get p
+00009af0: 686f 6e6f 6e20 6672 6571 7565 6e63 6965  honon frequencie
+00009b00: 7320 616e 6420 6569 6765 6e76 6563 746f  s and eigenvecto
+00009b10: 7273 2069 6e20 496e 7465 7261 6374 696f  rs in Interactio
+00009b20: 6e20 696e 7374 616e 6365 2e0a 0a20 2020  n instance...   
+00009b30: 2020 2020 2048 6172 6d6f 6e69 6320 7068       Harmonic ph
+00009b40: 6f6e 6f6e 2069 6e66 6f72 6d61 7469 6f6e  onon information
+00009b50: 2069 7320 7374 6f72 6564 2069 6e20 496e   is stored in In
+00009b60: 7465 7261 6374 696f 6e20 696e 7374 616e  teraction instan
+00009b70: 6365 2e20 5468 6973 0a20 2020 2020 2020  ce. This.       
+00009b80: 2069 6e66 6f72 6d61 7469 6f6e 2063 616e   information can
+00009b90: 2062 6520 6f62 7461 696e 6564 2e20 5468   be obtained. Th
+00009ba0: 6520 6772 6964 5f61 6464 7265 7373 2072  e grid_address r
+00009bb0: 6574 7572 6e65 6420 6769 7665 2074 6865  eturned give the
+00009bc0: 0a20 2020 2020 2020 2071 2d70 6f69 6e74  .        q-point
+00009bd0: 7320 6c6f 6361 7469 6f6e 7320 7769 7468  s locations with
+00009be0: 2072 6573 7065 6374 2074 6f20 7265 6369   respect to reci
+00009bf0: 7072 6f63 616c 2062 6173 6973 2076 6563  procal basis vec
+00009c00: 746f 7273 2062 790a 2020 2020 2020 2020  tors by.        
+00009c10: 696e 7465 6765 7273 2069 6e20 7468 6520  integers in the 
+00009c20: 7761 7920 7468 6174 0a20 2020 2020 2020  way that.       
+00009c30: 2020 2020 2071 5f70 6f69 6e74 7320 3d20       q_points = 
+00009c40: 6772 6964 5f61 6464 7265 7373 202f 206e  grid_address / n
+00009c50: 702e 6172 7261 7928 6d65 7368 2c20 6474  p.array(mesh, dt
+00009c60: 7970 653d 2764 6f75 626c 6527 292e 0a0a  ype='double')...
+00009c70: 2020 2020 2020 2020 5265 7475 726e 730a          Returns.
+00009c80: 2020 2020 2020 2020 2d2d 2d2d 2d2d 2d0a          -------.
+00009c90: 2020 2020 2020 2020 7475 706c 650a 2020          tuple.  
+00009ca0: 2020 2020 2020 2020 2020 2866 7265 7175            (frequ
+00009cb0: 656e 6369 6573 2c20 6569 6765 6e76 6563  encies, eigenvec
+00009cc0: 746f 7273 2c20 6772 6964 5f61 6464 7265  tors, grid_addre
+00009cd0: 7373 290a 2020 2020 2020 2020 2020 2020  ss).            
+00009ce0: 5365 6520 6d6f 7265 2064 6574 6169 6c73  See more details
+00009cf0: 2061 7420 7468 6520 646f 6373 7472 696e   at the docstrin
+00009d00: 6720 6f66 2073 6574 5f70 686f 6e6f 6e5f  g of set_phonon_
+00009d10: 6461 7461 2e0a 0a20 2020 2020 2020 2022  data...        "
+00009d20: 2222 0a20 2020 2020 2020 2069 6620 7365  "".        if se
+00009d30: 6c66 2e5f 696e 7465 7261 6374 696f 6e20  lf._interaction 
+00009d40: 6973 206e 6f74 204e 6f6e 653a 0a20 2020  is not None:.   
+00009d50: 2020 2020 2020 2020 2066 7265 7173 2c20           freqs, 
+00009d60: 6569 6776 6563 732c 205f 203d 2073 656c  eigvecs, _ = sel
+00009d70: 662e 5f69 6e74 6572 6163 7469 6f6e 2e67  f._interaction.g
+00009d80: 6574 5f70 686f 6e6f 6e73 2829 0a20 2020  et_phonons().   
+00009d90: 2020 2020 2020 2020 2072 6574 7572 6e20           return 
+00009da0: 6672 6571 732c 2065 6967 7665 6373 2c20  freqs, eigvecs, 
+00009db0: 7365 6c66 2e5f 696e 7465 7261 6374 696f  self._interactio
+00009dc0: 6e2e 627a 5f67 7269 642e 6164 6472 6573  n.bz_grid.addres
+00009dd0: 7365 730a 2020 2020 2020 2020 656c 7365  ses.        else
+00009de0: 3a0a 2020 2020 2020 2020 2020 2020 6d73  :.            ms
+00009df0: 6720 3d20 280a 2020 2020 2020 2020 2020  g = (.          
+00009e00: 2020 2020 2020 2250 686f 6e6f 3370 792e        "Phono3py.
+00009e10: 696e 6974 5f70 6870 685f 696e 7465 7261  init_phph_intera
+00009e20: 6374 696f 6e20 6861 7320 746f 2062 6520  ction has to be 
+00009e30: 6361 6c6c 6564 2022 0a20 2020 2020 2020  called ".       
+00009e40: 2020 2020 2020 2020 2022 6265 666f 7265           "before
+00009e50: 2072 756e 6e69 6e67 2074 6869 7320 6d65   running this me
+00009e60: 7468 6f64 2e22 0a20 2020 2020 2020 2020  thod.".         
+00009e70: 2020 2029 0a20 2020 2020 2020 2020 2020     ).           
+00009e80: 2072 6169 7365 2052 756e 7469 6d65 4572   raise RuntimeEr
+00009e90: 726f 7228 6d73 6729 0a0a 2020 2020 6465  ror(msg)..    de
+00009ea0: 6620 7275 6e5f 7068 6f6e 6f6e 5f73 6f6c  f run_phonon_sol
+00009eb0: 7665 7228 7365 6c66 2c20 6772 6964 5f70  ver(self, grid_p
+00009ec0: 6f69 6e74 733d 4e6f 6e65 293a 0a20 2020  oints=None):.   
+00009ed0: 2020 2020 2022 2222 5275 6e20 6861 726d       """Run harm
+00009ee0: 6f6e 6963 2070 686f 6e6f 6e20 6361 6c63  onic phonon calc
+00009ef0: 756c 6174 696f 6e20 6f6e 2067 7269 6420  ulation on grid 
+00009f00: 706f 696e 7473 2e0a 0a20 2020 2020 2020  points...       
+00009f10: 2050 6172 616d 6574 6572 730a 2020 2020   Parameters.    
+00009f20: 2020 2020 2d2d 2d2d 2d2d 2d2d 2d2d 0a20      ----------. 
+00009f30: 2020 2020 2020 2067 7269 645f 706f 696e         grid_poin
+00009f40: 7473 203a 2061 7272 6179 5f6c 696b 6520  ts : array_like 
+00009f50: 6f72 204e 6f6e 652c 206f 7074 696f 6e61  or None, optiona
+00009f60: 6c0a 2020 2020 2020 2020 2020 2020 4120  l.            A 
+00009f70: 6c69 7374 206f 6620 6772 6964 2070 6f69  list of grid poi
+00009f80: 6e74 2069 6e64 6963 6573 206f 6620 5068  nt indices of Ph
+00009f90: 6f6e 6f33 7079 2e67 7269 642e 6164 6472  ono3py.grid.addr
+00009fa0: 6573 7365 732e 0a20 2020 2020 2020 2020  esses..         
+00009fb0: 2020 2053 7065 6369 6679 696e 6720 4e6f     Specifying No
+00009fc0: 6e65 2072 756e 7320 616c 6c20 7068 6f6e  ne runs all phon
+00009fd0: 6f6e 7320 6f6e 2074 6865 2067 7269 6420  ons on the grid 
+00009fe0: 706f 696e 7473 2075 6e6c 6573 730a 2020  points unless.  
+00009ff0: 2020 2020 2020 2020 2020 7468 6f73 6520            those 
+0000a000: 7068 6f6e 6f6e 7320 7765 7265 2061 6c72  phonons were alr
+0000a010: 6561 6479 2063 616c 6375 6c61 7465 642e  eady calculated.
+0000a020: 204e 6f72 6d61 6c6c 7920 7068 6f6e 6f6e   Normally phonon
+0000a030: 7320 6174 0a20 2020 2020 2020 2020 2020  s at.           
+0000a040: 205b 302c 2030 2c20 305d 2070 6f69 6e74   [0, 0, 0] point
+0000a050: 2069 7320 616c 7265 6164 7920 6361 6c63   is already calc
+0000a060: 756c 6174 6564 2062 6566 6f72 6520 6361  ulated before ca
+0000a070: 6c6c 696e 6720 7468 6973 206d 6574 686f  lling this metho
+0000a080: 642e 0a20 2020 2020 2020 2020 2020 2050  d..            P
+0000a090: 686f 6e6f 6e20 6361 6c63 756c 6174 696f  honon calculatio
+0000a0a0: 6e73 2061 7265 2070 6572 666f 726d 6564  ns are performed
+0000a0b0: 2061 7574 6f6d 6174 6963 616c 6c79 2077   automatically w
+0000a0c0: 6865 6e20 6e65 6564 6564 0a20 2020 2020  hen needed.     
+0000a0d0: 2020 2020 2020 2069 6e74 6572 6e61 6c6c         internall
+0000a0e0: 7920 666f 7220 7068 2d70 6820 6361 6c63  y for ph-ph calc
+0000a0f0: 756c 6174 696f 6e2e 2054 6865 7265 666f  ulation. Therefo
+0000a100: 7265 2063 616c 6c69 6e67 2074 6869 7320  re calling this 
+0000a110: 6d65 7468 6f64 0a20 2020 2020 2020 2020  method.         
+0000a120: 2020 2069 7320 6e6f 7420 6e65 6365 7373     is not necess
+0000a130: 6172 7920 696e 206d 6f73 7420 6361 7365  ary in most case
+0000a140: 732e 0a20 2020 2020 2020 2020 2020 2054  s..            T
+0000a150: 6865 2070 686f 6e6f 6e20 7265 7375 6c74  he phonon result
+0000a160: 7320 6172 6520 6f62 7461 696e 6564 2062  s are obtained b
+0000a170: 7920 5068 6f6e 6f33 7079 2e67 6574 5f70  y Phono3py.get_p
+0000a180: 686f 6e6f 6e5f 6461 7461 2829 2e0a 0a20  honon_data()... 
+0000a190: 2020 2020 2020 2022 2222 0a20 2020 2020         """.     
+0000a1a0: 2020 2069 6620 7365 6c66 2e5f 696e 7465     if self._inte
+0000a1b0: 7261 6374 696f 6e20 6973 206e 6f74 204e  raction is not N
+0000a1c0: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
+0000a1d0: 2073 656c 662e 5f69 6e74 6572 6163 7469   self._interacti
+0000a1e0: 6f6e 2e72 756e 5f70 686f 6e6f 6e5f 736f  on.run_phonon_so
+0000a1f0: 6c76 6572 2867 7269 645f 706f 696e 7473  lver(grid_points
+0000a200: 3d67 7269 645f 706f 696e 7473 290a 2020  =grid_points).  
+0000a210: 2020 2020 2020 656c 7365 3a0a 2020 2020        else:.    
+0000a220: 2020 2020 2020 2020 6d73 6720 3d20 280a          msg = (.
+0000a230: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a240: 2250 686f 6e6f 3370 792e 696e 6974 5f70  "Phono3py.init_p
+0000a250: 6870 685f 696e 7465 7261 6374 696f 6e20  hph_interaction 
+0000a260: 6861 7320 746f 2062 6520 6361 6c6c 6564  has to be called
+0000a270: 2022 0a20 2020 2020 2020 2020 2020 2020   ".             
+0000a280: 2020 2022 6265 666f 7265 2072 756e 6e69     "before runni
+0000a290: 6e67 2074 6869 7320 6d65 7468 6f64 2e22  ng this method."
+0000a2a0: 0a20 2020 2020 2020 2020 2020 2029 0a20  .            ). 
+0000a2b0: 2020 2020 2020 2020 2020 2072 6169 7365             raise
+0000a2c0: 2052 756e 7469 6d65 4572 726f 7228 6d73   RuntimeError(ms
+0000a2d0: 6729 0a0a 2020 2020 6465 6620 6765 6e65  g)..    def gene
+0000a2e0: 7261 7465 5f64 6973 706c 6163 656d 656e  rate_displacemen
+0000a2f0: 7473 280a 2020 2020 2020 2020 7365 6c66  ts(.        self
+0000a300: 2c0a 2020 2020 2020 2020 6469 7374 616e  ,.        distan
+0000a310: 6365 3d30 2e30 332c 0a20 2020 2020 2020  ce=0.03,.       
+0000a320: 2063 7574 6f66 665f 7061 6972 5f64 6973   cutoff_pair_dis
+0000a330: 7461 6e63 653d 4e6f 6e65 2c0a 2020 2020  tance=None,.    
+0000a340: 2020 2020 6973 5f70 6c75 736d 696e 7573      is_plusminus
+0000a350: 3d22 6175 746f 222c 0a20 2020 2020 2020  ="auto",.       
+0000a360: 2069 735f 6469 6167 6f6e 616c 3d54 7275   is_diagonal=Tru
+0000a370: 652c 0a20 2020 2029 3a0a 2020 2020 2020  e,.    ):.      
+0000a380: 2020 2222 2247 656e 6572 6174 6520 6469    """Generate di
+0000a390: 7370 6c61 6365 6d65 6e74 2064 6174 6173  splacement datas
+0000a3a0: 6574 2069 6e20 7375 7065 7263 656c 6c20  et in supercell 
+0000a3b0: 666f 7220 6663 332e 0a0a 2020 2020 2020  for fc3...      
+0000a3c0: 2020 5468 6973 2073 7973 7465 6d61 7469    This systemati
+0000a3d0: 6361 6c6c 7920 6765 6e65 7261 7465 7320  cally generates 
+0000a3e0: 7369 6e67 6c65 2061 6e64 2070 6169 7220  single and pair 
+0000a3f0: 6174 6f6d 6963 2064 6973 706c 6163 656d  atomic displacem
+0000a400: 656e 7473 0a20 2020 2020 2020 2069 6e20  ents.        in 
+0000a410: 7375 7065 7263 656c 6c73 2074 6f20 6361  supercells to ca
+0000a420: 6c63 756c 6174 6520 6663 3320 636f 6e73  lculate fc3 cons
+0000a430: 6964 6572 696e 6720 6372 7973 7461 6c20  idering crystal 
+0000a440: 7379 6d6d 6574 7279 2e0a 2020 2020 2020  symmetry..      
+0000a450: 2020 5768 656e 2074 6869 7320 6d65 7468    When this meth
+0000a460: 6f64 2069 7320 6361 6c6c 6564 2c20 6578  od is called, ex
+0000a470: 6973 7469 6e67 2063 6163 6865 206f 6620  isting cache of 
+0000a480: 7375 7065 7263 656c 6c73 2077 6974 680a  supercells with.
+0000a490: 2020 2020 2020 2020 6469 7370 6c61 6365          displace
+0000a4a0: 6d65 6e74 7320 666f 7220 6663 3320 6172  ments for fc3 ar
+0000a4b0: 6520 7265 6d6f 7665 642e 0a0a 2020 2020  e removed...    
+0000a4c0: 2020 2020 466f 7220 6663 332c 2074 776f      For fc3, two
+0000a4d0: 2061 746f 6d73 2061 7265 2064 6973 706c   atoms are displ
+0000a4e0: 6163 6564 2066 6f72 2065 6163 6820 636f  aced for each co
+0000a4f0: 6e66 6967 7572 6174 696f 6e0a 2020 2020  nfiguration.    
+0000a500: 2020 2020 636f 6e73 6964 6572 696e 6720      considering 
+0000a510: 6372 7973 7461 6c20 7379 6d6d 6574 7279  crystal symmetry
+0000a520: 2e20 5468 6520 6669 7273 7420 6469 7370  . The first disp
+0000a530: 6c61 6365 6d65 6e74 2069 7320 6368 6f73  lacement is chos
+0000a540: 656e 0a20 2020 2020 2020 2069 6e20 7468  en.        in th
+0000a550: 6520 7065 7266 6563 7420 7375 7065 7263  e perfect superc
+0000a560: 656c 6c2c 2061 6e64 2074 6865 2073 6563  ell, and the sec
+0000a570: 6f6e 6420 6469 7370 6c61 6365 6d65 6e74  ond displacement
+0000a580: 2069 6e20 7468 650a 2020 2020 2020 2020   in the.        
+0000a590: 6469 7370 6c61 6365 6420 7375 7065 7263  displaced superc
+0000a5a0: 656c 6c2e 2054 6865 2066 6972 7374 2064  ell. The first d
+0000a5b0: 6973 706c 6163 656d 656e 7473 2061 7265  isplacements are
+0000a5c0: 2074 616b 656e 2061 6c6f 6e67 0a20 2020   taken along.   
+0000a5d0: 2020 2020 2074 6865 2062 6173 6973 2076       the basis v
+0000a5e0: 6563 746f 7273 206f 6620 7468 6520 7375  ectors of the su
+0000a5f0: 7065 7263 656c 6c2e 2054 6869 7320 6973  percell. This is
+0000a600: 2062 6563 6175 7365 2074 6865 0a20 2020   because the.   
+0000a610: 2020 2020 2073 796d 6d65 7472 7920 6973       symmetry is
+0000a620: 2065 7870 6563 7465 6420 746f 2062 6520   expected to be 
+0000a630: 6c65 7373 2062 726f 6b65 6e20 6279 2074  less broken by t
+0000a640: 6865 2069 6e74 726f 6475 6365 6420 6669  he introduced fi
+0000a650: 7273 740a 2020 2020 2020 2020 6469 7370  rst.        disp
+0000a660: 6c61 6365 6d65 6e74 2c20 616e 6420 6173  lacement, and as
+0000a670: 2074 6865 2072 6573 756c 742c 2074 6865   the result, the
+0000a680: 206e 756d 6265 7220 6f66 2073 6563 6f6e   number of secon
+0000a690: 640a 2020 2020 2020 2020 6469 7370 6c61  d.        displa
+0000a6a0: 6365 6d65 6e74 7320 6d61 7920 6265 636f  cements may beco
+0000a6b0: 6d65 2073 6d61 6c6c 6572 2074 6861 6e20  me smaller than 
+0000a6c0: 7468 6520 6361 7365 2074 6861 7420 7468  the case that th
+0000a6d0: 6520 6669 7273 740a 2020 2020 2020 2020  e first.        
+0000a6e0: 6174 6f6d 2069 7320 6469 7370 6c61 6365  atom is displace
+0000a6f0: 6420 6e6f 7420 616c 6f6e 6720 7468 6520  d not along the 
+0000a700: 6261 7369 7320 7665 6374 6f72 732e 0a0a  basis vectors...
+0000a710: 2020 2020 2020 2020 4e6f 7465 0a20 2020          Note.   
+0000a720: 2020 2020 202d 2d2d 2d0a 2020 2020 2020       ----.      
+0000a730: 2020 5768 656e 2070 686f 6e6f 6e5f 7375    When phonon_su
+0000a740: 7065 7263 656c 6c5f 6d61 7472 6978 2069  percell_matrix i
+0000a750: 7320 6e6f 7420 6769 7665 6e2c 2066 6332  s not given, fc2
+0000a760: 2069 7320 616c 736f 0a20 2020 2020 2020   is also.       
+0000a770: 2063 6f6d 7075 7465 6420 6672 6f6d 2074   computed from t
+0000a780: 6865 2073 616d 6520 7365 7420 6f66 2074  he same set of t
+0000a790: 6865 2064 6973 706c 6163 656d 656e 7473  he displacements
+0000a7a0: 2066 6f72 2066 6333 2061 6e64 0a20 2020   for fc3 and.   
+0000a7b0: 2020 2020 2072 6573 7065 6374 6976 6520       respective 
+0000a7c0: 7375 7065 7263 656c 6c20 666f 7263 6573  supercell forces
+0000a7d0: 2e20 5768 656e 2070 686f 6e6f 6e5f 7375  . When phonon_su
+0000a7e0: 7065 7263 656c 6c5f 6d61 7472 6978 2069  percell_matrix i
+0000a7f0: 730a 2020 2020 2020 2020 7365 742c 2074  s.        set, t
+0000a800: 6865 2064 6973 706c 6163 656d 656e 7473  he displacements
+0000a810: 2069 6e20 7068 6f6e 6f6e 5f73 7570 6572   in phonon_super
+0000a820: 6365 6c6c 2061 7265 2067 656e 6572 6174  cell are generat
+0000a830: 6564 2075 6e6c 6573 730a 2020 2020 2020  ed unless.      
+0000a840: 2020 7468 6f73 6520 616c 7265 6164 7920    those already 
+0000a850: 6578 6973 742e 0a0a 2020 2020 2020 2020  exist...        
+0000a860: 5061 7261 6d65 7465 7273 0a20 2020 2020  Parameters.     
+0000a870: 2020 202d 2d2d 2d2d 2d2d 2d2d 2d0a 2020     ----------.  
+0000a880: 2020 2020 2020 6469 7374 616e 6365 203a        distance :
+0000a890: 2066 6c6f 6174 2c20 6f70 7469 6f6e 616c   float, optional
+0000a8a0: 0a20 2020 2020 2020 2020 2020 2043 6f6e  .            Con
+0000a8b0: 7374 616e 7420 6469 7370 6c61 6365 6d65  stant displaceme
+0000a8c0: 6e74 2045 7563 6c69 6465 616e 2064 6973  nt Euclidean dis
+0000a8d0: 7461 6e63 652e 2044 6566 6175 6c74 2069  tance. Default i
+0000a8e0: 7320 302e 3033 2e0a 2020 2020 2020 2020  s 0.03..        
+0000a8f0: 6375 746f 6666 5f70 6169 725f 6469 7374  cutoff_pair_dist
+0000a900: 616e 6365 203a 2066 6c6f 6174 2c20 6f70  ance : float, op
+0000a910: 7469 6f6e 616c 0a20 2020 2020 2020 2020  tional.         
+0000a920: 2020 2054 6869 7320 6973 2075 7365 6420     This is used 
+0000a930: 6173 2061 2063 7574 6f66 6620 4575 636c  as a cutoff Eucl
+0000a940: 6964 6561 6e20 6469 7374 616e 6365 2074  idean distance t
+0000a950: 6f20 6465 7465 726d 696e 6520 6966 0a20  o determine if. 
+0000a960: 2020 2020 2020 2020 2020 2065 6163 6820             each 
+0000a970: 7061 6972 206f 6620 6469 7370 6c61 6365  pair of displace
+0000a980: 6d65 6e74 7320 6973 2063 6f6e 7369 6465  ments is conside
+0000a990: 7265 6420 746f 2063 616c 6375 6c61 7465  red to calculate
+0000a9a0: 2066 6333 206f 7220 6e6f 742e 0a20 2020   fc3 or not..   
+0000a9b0: 2020 2020 2020 2020 2044 6566 6175 6c74           Default
+0000a9c0: 2069 7320 4e6f 6e65 2c20 7768 6963 6820   is None, which 
+0000a9d0: 6d65 616e 7320 6375 746f 6666 2069 7320  means cutoff is 
+0000a9e0: 6e6f 7420 7573 6564 2e0a 2020 2020 2020  not used..      
+0000a9f0: 2020 6973 5f70 6c75 736d 696e 7573 203a    is_plusminus :
+0000aa00: 2054 7275 652c 2046 616c 7365 2c20 6f72   True, False, or
+0000aa10: 2027 6175 746f 272c 206f 7074 696f 6e61   'auto', optiona
+0000aa20: 6c0a 2020 2020 2020 2020 2020 2020 5769  l.            Wi
+0000aa30: 7468 2054 7275 652c 2061 746f 6d69 7320  th True, atomis 
+0000aa40: 6172 6520 6469 7370 6c61 6365 6420 696e  are displaced in
+0000aa50: 2062 6f74 6820 706f 7369 7469 7665 2061   both positive a
+0000aa60: 6e64 206e 6567 6174 6976 650a 2020 2020  nd negative.    
+0000aa70: 2020 2020 2020 2020 6469 7265 6374 696f          directio
+0000aa80: 6e73 2e20 5769 7468 2046 616c 7365 2c20  ns. With False, 
+0000aa90: 6f6e 6c79 206f 6e65 2064 6972 6563 7469  only one directi
+0000aaa0: 6f6e 2e20 5769 7468 2027 6175 746f 272c  on. With 'auto',
+0000aab0: 0a20 2020 2020 2020 2020 2020 206d 6f73  .            mos
+0000aac0: 746c 7920 6571 7569 7661 6c65 6e74 2074  tly equivalent t
+0000aad0: 6f20 6973 5f70 6c75 736d 696e 7573 3d54  o is_plusminus=T
+0000aae0: 7275 652c 2062 7574 206f 6e6c 7920 6f6e  rue, but only on
+0000aaf0: 6520 6469 7265 6374 696f 6e0a 2020 2020  e direction.    
+0000ab00: 2020 2020 2020 2020 6973 2063 686f 7365          is chose
+0000ab10: 6e20 7768 656e 2074 6865 2064 6973 706c  n when the displ
+0000ab20: 6163 656d 656e 7473 2069 6e20 626f 7468  acements in both
+0000ab30: 2064 6972 6563 7469 6f6e 7320 6172 650a   directions are.
+0000ab40: 2020 2020 2020 2020 2020 2020 7379 6d6d              symm
+0000ab50: 6574 7269 6361 6c6c 7920 6571 7569 7661  etrically equiva
+0000ab60: 6c65 6e74 2e20 4465 6661 756c 7420 6973  lent. Default is
+0000ab70: 2027 6175 746f 272e 0a20 2020 2020 2020   'auto'..       
+0000ab80: 2069 735f 6469 6167 6f6e 616c 203a 2042   is_diagonal : B
+0000ab90: 6f6f 6c2c 206f 7074 696f 6e61 6c0a 2020  ool, optional.  
+0000aba0: 2020 2020 2020 2020 2020 5769 7468 2046            With F
+0000abb0: 616c 7365 2c20 7468 6520 7365 636f 6e64  alse, the second
+0000abc0: 2064 6973 706c 6163 656d 656e 7473 2061   displacements a
+0000abd0: 7265 206d 6164 6520 616c 6f6e 6720 7468  re made along th
+0000abe0: 6520 6261 7369 730a 2020 2020 2020 2020  e basis.        
+0000abf0: 2020 2020 7665 6374 6f72 7320 6f66 2074      vectors of t
+0000ac00: 6865 2073 7570 6572 6365 6c6c 2e20 5769  he supercell. Wi
+0000ac10: 7468 2054 7275 652c 2064 6972 6563 7469  th True, directi
+0000ac20: 6f6e 206e 6f74 2061 6c6f 6e67 2074 6865  on not along the
+0000ac30: 2062 6173 6973 0a20 2020 2020 2020 2020   basis.         
+0000ac40: 2020 2076 6563 746f 7273 2063 616e 2062     vectors can b
+0000ac50: 6520 6368 6f73 656e 2077 6865 6e20 7468  e chosen when th
+0000ac60: 6520 6e75 6d62 6572 206f 6620 7468 6520  e number of the 
+0000ac70: 6469 7370 6c61 6365 6d65 6e74 730a 2020  displacements.  
+0000ac80: 2020 2020 2020 2020 2020 6d61 7920 6265            may be
+0000ac90: 2072 6564 7563 6564 2e0a 0a20 2020 2020   reduced...     
+0000aca0: 2020 2022 2222 0a20 2020 2020 2020 2064     """.        d
+0000acb0: 6972 6563 7469 6f6e 5f64 6174 6173 6574  irection_dataset
+0000acc0: 203d 2067 6574 5f74 6869 7264 5f6f 7264   = get_third_ord
+0000acd0: 6572 5f64 6973 706c 6163 656d 656e 7473  er_displacements
+0000ace0: 280a 2020 2020 2020 2020 2020 2020 7365  (.            se
+0000acf0: 6c66 2e5f 7375 7065 7263 656c 6c2c 0a20  lf._supercell,. 
+0000ad00: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+0000ad10: 5f73 796d 6d65 7472 792c 0a20 2020 2020  _symmetry,.     
+0000ad20: 2020 2020 2020 2069 735f 706c 7573 6d69         is_plusmi
+0000ad30: 6e75 733d 6973 5f70 6c75 736d 696e 7573  nus=is_plusminus
+0000ad40: 2c0a 2020 2020 2020 2020 2020 2020 6973  ,.            is
+0000ad50: 5f64 6961 676f 6e61 6c3d 6973 5f64 6961  _diagonal=is_dia
+0000ad60: 676f 6e61 6c2c 0a20 2020 2020 2020 2029  gonal,.        )
+0000ad70: 0a20 2020 2020 2020 2073 656c 662e 5f64  .        self._d
+0000ad80: 6174 6173 6574 203d 2064 6972 6563 7469  ataset = directi
+0000ad90: 6f6e 5f74 6f5f 6469 7370 6c61 6365 6d65  on_to_displaceme
+0000ada0: 6e74 280a 2020 2020 2020 2020 2020 2020  nt(.            
+0000adb0: 6469 7265 6374 696f 6e5f 6461 7461 7365  direction_datase
+0000adc0: 742c 0a20 2020 2020 2020 2020 2020 2064  t,.            d
+0000add0: 6973 7461 6e63 652c 0a20 2020 2020 2020  istance,.       
+0000ade0: 2020 2020 2073 656c 662e 5f73 7570 6572       self._super
+0000adf0: 6365 6c6c 2c0a 2020 2020 2020 2020 2020  cell,.          
+0000ae00: 2020 6375 746f 6666 5f64 6973 7461 6e63    cutoff_distanc
+0000ae10: 653d 6375 746f 6666 5f70 6169 725f 6469  e=cutoff_pair_di
+0000ae20: 7374 616e 6365 2c0a 2020 2020 2020 2020  stance,.        
+0000ae30: 290a 2020 2020 2020 2020 7365 6c66 2e5f  ).        self._
+0000ae40: 7375 7065 7263 656c 6c73 5f77 6974 685f  supercells_with_
+0000ae50: 6469 7370 6c61 6365 6d65 6e74 7320 3d20  displacements = 
+0000ae60: 4e6f 6e65 0a0a 2020 2020 2020 2020 6966  None..        if
+0000ae70: 2073 656c 662e 5f70 686f 6e6f 6e5f 7375   self._phonon_su
+0000ae80: 7065 7263 656c 6c5f 6d61 7472 6978 2069  percell_matrix i
+0000ae90: 7320 6e6f 7420 4e6f 6e65 2061 6e64 2073  s not None and s
+0000aea0: 656c 662e 5f70 686f 6e6f 6e5f 6461 7461  elf._phonon_data
+0000aeb0: 7365 7420 6973 204e 6f6e 653a 0a20 2020  set is None:.   
+0000aec0: 2020 2020 2020 2020 2073 656c 662e 6765           self.ge
+0000aed0: 6e65 7261 7465 5f66 6332 5f64 6973 706c  nerate_fc2_displ
+0000aee0: 6163 656d 656e 7473 280a 2020 2020 2020  acements(.      
+0000aef0: 2020 2020 2020 2020 2020 6469 7374 616e            distan
+0000af00: 6365 3d64 6973 7461 6e63 652c 2069 735f  ce=distance, is_
+0000af10: 706c 7573 6d69 6e75 733d 6973 5f70 6c75  plusminus=is_plu
+0000af20: 736d 696e 7573 2c20 6973 5f64 6961 676f  sminus, is_diago
+0000af30: 6e61 6c3d 4661 6c73 650a 2020 2020 2020  nal=False.      
+0000af40: 2020 2020 2020 290a 0a20 2020 2064 6566        )..    def
+0000af50: 2067 656e 6572 6174 655f 6663 325f 6469   generate_fc2_di
+0000af60: 7370 6c61 6365 6d65 6e74 7328 0a20 2020  splacements(.   
+0000af70: 2020 2020 2073 656c 662c 2064 6973 7461       self, dista
+0000af80: 6e63 653d 302e 3033 2c20 6973 5f70 6c75  nce=0.03, is_plu
+0000af90: 736d 696e 7573 3d22 6175 746f 222c 2069  sminus="auto", i
+0000afa0: 735f 6469 6167 6f6e 616c 3d46 616c 7365  s_diagonal=False
+0000afb0: 0a20 2020 2029 3a0a 2020 2020 2020 2020  .    ):.        
+0000afc0: 2222 2247 656e 6572 6174 6520 6469 7370  """Generate disp
+0000afd0: 6c61 6365 6d65 6e74 2064 6174 6173 6574  lacement dataset
+0000afe0: 2069 6e20 7068 6f6e 6f6e 2073 7570 6572   in phonon super
+0000aff0: 6365 6c6c 2066 6f72 2066 6332 2e0a 0a20  cell for fc2... 
+0000b000: 2020 2020 2020 2054 6869 7320 7379 7374         This syst
+0000b010: 656d 6174 6963 616c 6c79 2067 656e 6572  ematically gener
+0000b020: 6174 6573 2073 696e 676c 6520 6174 6f6d  ates single atom
+0000b030: 6963 2064 6973 706c 6163 656d 656e 7473  ic displacements
+0000b040: 0a20 2020 2020 2020 2069 6e20 7375 7065  .        in supe
+0000b050: 7263 656c 6c73 2074 6f20 6361 6c63 756c  rcells to calcul
+0000b060: 6174 6520 7068 6f6e 6f6e 5f66 6332 2063  ate phonon_fc2 c
+0000b070: 6f6e 7369 6465 7269 6e67 2063 7279 7374  onsidering cryst
+0000b080: 616c 2073 796d 6d65 7472 792e 0a20 2020  al symmetry..   
+0000b090: 2020 2020 2057 6865 6e20 7468 6973 206d       When this m
+0000b0a0: 6574 686f 6420 6973 2063 616c 6c65 642c  ethod is called,
+0000b0b0: 2065 7869 7374 696e 6720 6361 6368 6520   existing cache 
+0000b0c0: 6f66 2073 7570 6572 6365 6c6c 7320 7769  of supercells wi
+0000b0d0: 7468 0a20 2020 2020 2020 2064 6973 706c  th.        displ
+0000b0e0: 6163 656d 656e 7473 2066 6f72 2066 6332  acements for fc2
+0000b0f0: 2061 7265 2072 656d 6f76 6564 2e0a 0a20   are removed... 
+0000b100: 2020 2020 2020 204e 6f74 650a 2020 2020         Note.    
+0000b110: 2020 2020 2d2d 2d2d 0a20 2020 2020 2020      ----.       
+0000b120: 2069 735f 6469 6167 6f6e 616c 3d46 616c   is_diagonal=Fal
+0000b130: 7365 2069 7320 6368 6f73 656e 2061 7320  se is chosen as 
+0000b140: 7468 6520 6465 6661 756c 7420 7365 7474  the default sett
+0000b150: 696e 6720 696e 7465 6e74 696f 6e61 6c6c  ing intentionall
+0000b160: 790a 2020 2020 2020 2020 746f 2062 6520  y.        to be 
+0000b170: 636f 6e73 6973 7465 6e74 2074 6f20 7468  consistent to th
+0000b180: 6520 6669 7273 7420 6469 7370 6c61 6365  e first displace
+0000b190: 6d65 6e74 7320 6f66 2074 6865 2066 6333  ments of the fc3
+0000b1a0: 2070 6169 720a 2020 2020 2020 2020 6469   pair.        di
+0000b1b0: 7370 6c61 6365 6d65 7473 2069 6e20 7375  splacemets in su
+0000b1c0: 7065 7263 656c 6c2e 0a0a 2020 2020 2020  percell...      
+0000b1d0: 2020 5061 7261 6d65 7465 7273 0a20 2020    Parameters.   
+0000b1e0: 2020 2020 202d 2d2d 2d2d 2d2d 2d2d 2d0a       ----------.
+0000b1f0: 2020 2020 2020 2020 6469 7374 616e 6365          distance
+0000b200: 203a 2066 6c6f 6174 2c20 6f70 7469 6f6e   : float, option
+0000b210: 616c 0a20 2020 2020 2020 2020 2020 2043  al.            C
+0000b220: 6f6e 7374 616e 7420 6469 7370 6c61 6365  onstant displace
+0000b230: 6d65 6e74 2045 7563 6c69 6465 616e 2064  ment Euclidean d
+0000b240: 6973 7461 6e63 652e 2044 6566 6175 6c74  istance. Default
+0000b250: 2069 7320 302e 3033 2e0a 2020 2020 2020   is 0.03..      
+0000b260: 2020 6973 5f70 6c75 736d 696e 7573 203a    is_plusminus :
+0000b270: 2054 7275 652c 2046 616c 7365 2c20 6f72   True, False, or
+0000b280: 2027 6175 746f 272c 206f 7074 696f 6e61   'auto', optiona
+0000b290: 6c0a 2020 2020 2020 2020 2020 2020 5769  l.            Wi
+0000b2a0: 7468 2054 7275 652c 2061 746f 6d69 7320  th True, atomis 
+0000b2b0: 6172 6520 6469 7370 6c61 6365 6420 696e  are displaced in
+0000b2c0: 2062 6f74 6820 706f 7369 7469 7665 2061   both positive a
+0000b2d0: 6e64 206e 6567 6174 6976 650a 2020 2020  nd negative.    
+0000b2e0: 2020 2020 2020 2020 6469 7265 6374 696f          directio
+0000b2f0: 6e73 2e20 5769 7468 2046 616c 7365 2c20  ns. With False, 
+0000b300: 6f6e 6c79 206f 6e65 2064 6972 6563 7469  only one directi
+0000b310: 6f6e 2e20 5769 7468 2027 6175 746f 272c  on. With 'auto',
+0000b320: 0a20 2020 2020 2020 2020 2020 206d 6f73  .            mos
+0000b330: 746c 7920 6571 7569 7661 6c65 6e74 2074  tly equivalent t
+0000b340: 6f20 6973 5f70 6c75 736d 696e 7573 3d54  o is_plusminus=T
+0000b350: 7275 652c 2062 7574 206f 6e6c 7920 6f6e  rue, but only on
+0000b360: 6520 6469 7265 6374 696f 6e0a 2020 2020  e direction.    
+0000b370: 2020 2020 2020 2020 6973 2063 686f 7365          is chose
+0000b380: 6e20 7768 656e 2074 6865 2064 6973 706c  n when the displ
+0000b390: 6163 656d 656e 7473 2069 6e20 626f 7468  acements in both
+0000b3a0: 2064 6972 6563 7469 6f6e 7320 6172 650a   directions are.
+0000b3b0: 2020 2020 2020 2020 2020 2020 7379 6d6d              symm
+0000b3c0: 6574 7269 6361 6c6c 7920 6571 7569 7661  etrically equiva
+0000b3d0: 6c65 6e74 2e20 4465 6661 756c 7420 6973  lent. Default is
+0000b3e0: 2027 6175 746f 272e 0a20 2020 2020 2020   'auto'..       
+0000b3f0: 2069 735f 6469 6167 6f6e 616c 203a 2042   is_diagonal : B
+0000b400: 6f6f 6c2c 206f 7074 696f 6e61 6c0a 2020  ool, optional.  
+0000b410: 2020 2020 2020 2020 2020 5769 7468 2046            With F
+0000b420: 616c 7365 2c20 7468 6520 6469 7370 6c61  alse, the displa
+0000b430: 6365 6d65 6e74 7320 6172 6520 6d61 6465  cements are made
+0000b440: 2061 6c6f 6e67 2074 6865 2062 6173 6973   along the basis
+0000b450: 0a20 2020 2020 2020 2020 2020 2076 6563  .            vec
+0000b460: 746f 7273 206f 6620 7468 6520 7375 7065  tors of the supe
+0000b470: 7263 656c 6c2e 2057 6974 6820 5472 7565  rcell. With True
+0000b480: 2c20 6469 7265 6374 696f 6e20 6e6f 7420  , direction not 
+0000b490: 616c 6f6e 6720 7468 6520 6261 7369 730a  along the basis.
+0000b4a0: 2020 2020 2020 2020 2020 2020 7665 6374              vect
+0000b4b0: 6f72 7320 6361 6e20 6265 2063 686f 7365  ors can be chose
+0000b4c0: 6e20 7768 656e 2074 6865 206e 756d 6265  n when the numbe
+0000b4d0: 7220 6f66 2074 6865 2064 6973 706c 6163  r of the displac
+0000b4e0: 656d 656e 7473 0a20 2020 2020 2020 2020  ements.         
+0000b4f0: 2020 206d 6179 2062 6520 7265 6475 6365     may be reduce
+0000b500: 642e 2044 6566 6175 6c74 2069 7320 4661  d. Default is Fa
+0000b510: 6c73 652e 0a0a 2020 2020 2020 2020 2222  lse...        ""
+0000b520: 220a 2020 2020 2020 2020 6966 2073 656c  ".        if sel
+0000b530: 662e 5f70 686f 6e6f 6e5f 7375 7065 7263  f._phonon_superc
+0000b540: 656c 6c5f 6d61 7472 6978 2069 7320 4e6f  ell_matrix is No
+0000b550: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
+0000b560: 6d73 6720 3d20 280a 2020 2020 2020 2020  msg = (.        
+0000b570: 2020 2020 2020 2020 2270 686f 6e6f 6e5f          "phonon_
+0000b580: 7375 7065 7263 656c 6c5f 6d61 7472 6978  supercell_matrix
+0000b590: 2069 7320 6e6f 7420 7365 742e 2022 0a20   is not set. ". 
+0000b5a0: 2020 2020 2020 2020 2020 2020 2020 2022                 "
+0000b5b0: 5468 6973 206d 6574 686f 6420 6973 2075  This method is u
+0000b5c0: 7365 6420 746f 2067 656e 6572 6174 6520  sed to generate 
+0000b5d0: 6469 7370 6c61 6365 6d65 6e74 7320 746f  displacements to
+0000b5e0: 2022 0a20 2020 2020 2020 2020 2020 2020   ".             
+0000b5f0: 2020 2022 6361 6c63 756c 6174 6520 7068     "calculate ph
+0000b600: 6f6e 6f6e 5f66 6332 2e22 0a20 2020 2020  onon_fc2.".     
+0000b610: 2020 2020 2020 2029 0a20 2020 2020 2020         ).       
+0000b620: 2020 2020 2072 6169 7365 2052 756e 7469       raise Runti
+0000b630: 6d65 4572 726f 7228 6d73 6729 0a0a 2020  meError(msg)..  
+0000b640: 2020 2020 2020 7068 6f6e 6f6e 5f64 6973        phonon_dis
+0000b650: 706c 6163 656d 656e 745f 6469 7265 6374  placement_direct
+0000b660: 696f 6e73 203d 2067 6574 5f6c 6561 7374  ions = get_least
+0000b670: 5f64 6973 706c 6163 656d 656e 7473 280a  _displacements(.
+0000b680: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+0000b690: 2e5f 7068 6f6e 6f6e 5f73 7570 6572 6365  ._phonon_superce
+0000b6a0: 6c6c 5f73 796d 6d65 7472 792c 0a20 2020  ll_symmetry,.   
+0000b6b0: 2020 2020 2020 2020 2069 735f 706c 7573           is_plus
+0000b6c0: 6d69 6e75 733d 6973 5f70 6c75 736d 696e  minus=is_plusmin
+0000b6d0: 7573 2c0a 2020 2020 2020 2020 2020 2020  us,.            
+0000b6e0: 6973 5f64 6961 676f 6e61 6c3d 6973 5f64  is_diagonal=is_d
+0000b6f0: 6961 676f 6e61 6c2c 0a20 2020 2020 2020  iagonal,.       
+0000b700: 2029 0a20 2020 2020 2020 2073 656c 662e   ).        self.
+0000b710: 5f70 686f 6e6f 6e5f 6461 7461 7365 7420  _phonon_dataset 
+0000b720: 3d20 6469 7265 6374 696f 6e73 5f74 6f5f  = directions_to_
+0000b730: 6469 7370 6c61 6365 6d65 6e74 5f64 6174  displacement_dat
+0000b740: 6173 6574 280a 2020 2020 2020 2020 2020  aset(.          
+0000b750: 2020 7068 6f6e 6f6e 5f64 6973 706c 6163    phonon_displac
+0000b760: 656d 656e 745f 6469 7265 6374 696f 6e73  ement_directions
+0000b770: 2c20 6469 7374 616e 6365 2c20 7365 6c66  , distance, self
+0000b780: 2e5f 7068 6f6e 6f6e 5f73 7570 6572 6365  ._phonon_superce
+0000b790: 6c6c 0a20 2020 2020 2020 2029 0a20 2020  ll.        ).   
+0000b7a0: 2020 2020 2073 656c 662e 5f70 686f 6e6f       self._phono
+0000b7b0: 6e5f 7375 7065 7263 656c 6c73 5f77 6974  n_supercells_wit
+0000b7c0: 685f 6469 7370 6c61 6365 6d65 6e74 7320  h_displacements 
+0000b7d0: 3d20 4e6f 6e65 0a0a 2020 2020 6465 6620  = None..    def 
+0000b7e0: 7072 6f64 7563 655f 6663 3328 0a20 2020  produce_fc3(.   
+0000b7f0: 2020 2020 2073 656c 662c 0a20 2020 2020       self,.     
+0000b800: 2020 2073 796d 6d65 7472 697a 655f 6663     symmetrize_fc
+0000b810: 3372 3d46 616c 7365 2c0a 2020 2020 2020  3r=False,.      
+0000b820: 2020 6973 5f63 6f6d 7061 6374 5f66 633d    is_compact_fc=
+0000b830: 4661 6c73 652c 0a20 2020 2020 2020 2066  False,.        f
+0000b840: 635f 6361 6c63 756c 6174 6f72 3d4e 6f6e  c_calculator=Non
+0000b850: 652c 0a20 2020 2020 2020 2066 635f 6361  e,.        fc_ca
+0000b860: 6c63 756c 6174 6f72 5f6f 7074 696f 6e73  lculator_options
+0000b870: 3d4e 6f6e 652c 0a20 2020 2029 3a0a 2020  =None,.    ):.  
+0000b880: 2020 2020 2020 2222 2243 616c 6375 6c61        """Calcula
+0000b890: 7465 2066 6333 2066 726f 6d20 6469 7370  te fc3 from disp
+0000b8a0: 6c61 6365 6d65 6e74 7320 616e 6420 666f  lacements and fo
+0000b8b0: 7263 6573 2e0a 0a20 2020 2020 2020 2050  rces...        P
+0000b8c0: 6172 616d 6574 6572 730a 2020 2020 2020  arameters.      
+0000b8d0: 2020 2d2d 2d2d 2d2d 2d2d 2d2d 0a20 2020    ----------.   
+0000b8e0: 2020 2020 2073 796d 6d65 7472 697a 655f       symmetrize_
+0000b8f0: 6663 3372 203a 2062 6f6f 6c0a 2020 2020  fc3r : bool.    
+0000b900: 2020 2020 2020 2020 4f6e 6c79 2066 6f72          Only for
+0000b910: 2074 7970 6520 3120 6469 7370 6c61 6365   type 1 displace
+0000b920: 6d65 6e74 5f64 6174 6173 6574 2c20 7472  ment_dataset, tr
+0000b930: 616e 736c 6174 696f 6e61 6c20 616e 640a  anslational and.
+0000b940: 2020 2020 2020 2020 2020 2020 7065 726d              perm
+0000b950: 7574 6174 696f 6e20 7379 6d6d 6574 7269  utation symmetri
+0000b960: 6573 2061 7265 2061 7070 6c69 6564 2061  es are applied a
+0000b970: 6674 6572 2063 7265 6174 696e 6720 6663  fter creating fc
+0000b980: 332e 2054 6869 730a 2020 2020 2020 2020  3. This.        
+0000b990: 2020 2020 7379 6d6d 6574 7269 7a61 7469      symmetrizati
+0000b9a0: 6f6e 2069 7320 6e6f 7420 7665 7279 2073  on is not very s
+0000b9b0: 6f70 6869 7374 6963 6174 6564 2061 6e64  ophisticated and
+0000b9c0: 2063 616e 2062 7265 616b 2073 7061 6365   can break space
+0000b9d0: 0a20 2020 2020 2020 2020 2020 2067 726f  .            gro
+0000b9e0: 7570 2073 796d 6d65 7472 792c 2062 7574  up symmetry, but
+0000b9f0: 206f 6674 656e 2075 7365 6675 6c2e 2049   often useful. I
+0000ba00: 6620 6265 7474 6572 2073 796d 6d65 7472  f better symmetr
+0000ba10: 697a 6174 696f 6e20 6973 0a20 2020 2020  ization is.     
+0000ba20: 2020 2020 2020 2065 7870 6563 7465 642c         expected,
+0000ba30: 2069 7420 6973 2072 6563 6f6d 6d65 6e64   it is recommend
+0000ba40: 6564 2074 6f20 7573 6520 6578 7465 726e  ed to use extern
+0000ba50: 616c 2066 6f72 6365 2063 6f6e 7374 616e  al force constan
+0000ba60: 7473 0a20 2020 2020 2020 2020 2020 2063  ts.            c
+0000ba70: 616c 6375 6c61 746f 7220 7375 6368 2061  alculator such a
+0000ba80: 7320 414c 4d2e 2044 6566 6175 6c74 2069  s ALM. Default i
+0000ba90: 7320 4661 6c73 652e 0a20 2020 2020 2020  s False..       
+0000baa0: 2069 735f 636f 6d70 6163 745f 6663 203a   is_compact_fc :
+0000bab0: 2062 6f6f 6c0a 2020 2020 2020 2020 2020   bool.          
+0000bac0: 2020 6663 3320 7368 6170 6520 6973 0a20    fc3 shape is. 
+0000bad0: 2020 2020 2020 2020 2020 2020 2020 2046                 F
+0000bae0: 616c 7365 3a20 2873 7570 6572 6365 6c6c  alse: (supercell
+0000baf0: 2c20 7375 7065 7263 656c 6c2c 2073 7570  , supercell, sup
+0000bb00: 6563 656c 6c2c 2033 2c20 332c 2033 290a  ecell, 3, 3, 3).
+0000bb10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000bb20: 5472 7565 3a20 2870 7269 6d69 7469 7665  True: (primitive
+0000bb30: 2c20 7375 7065 7263 656c 6c2c 2073 7570  , supercell, sup
+0000bb40: 6563 656c 6c2c 2033 2c20 332c 2033 290a  ecell, 3, 3, 3).
+0000bb50: 2020 2020 2020 2020 2020 2020 7768 6572              wher
+0000bb60: 6520 2773 7570 6572 6365 6c6c 2720 616e  e 'supercell' an
+0000bb70: 6420 2770 7269 6d69 7469 7665 2720 696e  d 'primitive' in
+0000bb80: 6469 6361 7465 206e 756d 6265 7220 6f66  dicate number of
+0000bb90: 2061 746f 6d73 2069 6e20 7468 6573 650a   atoms in these.
+0000bba0: 2020 2020 2020 2020 2020 2020 6365 6c6c              cell
+0000bbb0: 732e 2044 6566 6175 6c74 2069 7320 4661  s. Default is Fa
+0000bbc0: 6c73 652e 0a20 2020 2020 2020 2066 635f  lse..        fc_
+0000bbd0: 6361 6c63 756c 6174 6f72 203a 2073 7472  calculator : str
+0000bbe0: 206f 7220 4e6f 6e65 0a20 2020 2020 2020   or None.       
+0000bbf0: 2020 2020 2046 6f72 6365 2063 6f6e 7374       Force const
+0000bc00: 616e 7473 2063 616c 6375 6c61 746f 7220  ants calculator 
+0000bc10: 6769 7665 6e20 6279 2073 7472 2e0a 2020  given by str..  
+0000bc20: 2020 2020 2020 6663 5f63 616c 6375 6c61        fc_calcula
+0000bc30: 746f 725f 6f70 7469 6f6e 7320 3a20 6469  tor_options : di
+0000bc40: 6374 0a20 2020 2020 2020 2020 2020 204f  ct.            O
+0000bc50: 7074 696f 6e73 2066 6f72 2065 7874 6572  ptions for exter
+0000bc60: 6e61 6c20 666f 7263 6520 636f 6e73 7461  nal force consta
+0000bc70: 6e74 7320 6361 6c63 756c 6174 6f72 2e0a  nts calculator..
+0000bc80: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
+0000bc90: 2020 2020 2064 6973 705f 6461 7461 7365       disp_datase
+0000bca0: 7420 3d20 7365 6c66 2e5f 6461 7461 7365  t = self._datase
+0000bcb0: 740a 0a20 2020 2020 2020 2066 6333 5f63  t..        fc3_c
+0000bcc0: 616c 6375 6c61 746f 722c 2066 6333 5f63  alculator, fc3_c
+0000bcd0: 616c 6375 6c61 746f 725f 6f70 7469 6f6e  alculator_option
+0000bce0: 7320 3d20 7365 6c66 2e5f 6578 7472 6163  s = self._extrac
+0000bcf0: 745f 6663 325f 6663 335f 6361 6c63 756c  t_fc2_fc3_calcul
+0000bd00: 6174 6f72 7328 0a20 2020 2020 2020 2020  ators(.         
+0000bd10: 2020 2066 635f 6361 6c63 756c 6174 6f72     fc_calculator
+0000bd20: 2c20 6663 5f63 616c 6375 6c61 746f 725f  , fc_calculator_
+0000bd30: 6f70 7469 6f6e 732c 2033 0a20 2020 2020  options, 3.     
+0000bd40: 2020 2029 0a0a 2020 2020 2020 2020 6966     )..        if
+0000bd50: 2066 6333 5f63 616c 6375 6c61 746f 7220   fc3_calculator 
+0000bd60: 6973 206e 6f74 204e 6f6e 653a 0a20 2020  is not None:.   
+0000bd70: 2020 2020 2020 2020 2064 6973 7073 2c20           disps, 
+0000bd80: 666f 7263 6573 203d 2067 6574 5f64 6973  forces = get_dis
+0000bd90: 706c 6163 656d 656e 7473 5f61 6e64 5f66  placements_and_f
+0000bda0: 6f72 6365 735f 6663 3328 6469 7370 5f64  orces_fc3(disp_d
+0000bdb0: 6174 6173 6574 290a 2020 2020 2020 2020  ataset).        
+0000bdc0: 2020 2020 6663 322c 2066 6333 203d 2067      fc2, fc3 = g
+0000bdd0: 6574 5f66 6333 280a 2020 2020 2020 2020  et_fc3(.        
+0000bde0: 2020 2020 2020 2020 7365 6c66 2e5f 7375          self._su
+0000bdf0: 7065 7263 656c 6c2c 0a20 2020 2020 2020  percell,.       
+0000be00: 2020 2020 2020 2020 2073 656c 662e 5f70           self._p
+0000be10: 7269 6d69 7469 7665 2c0a 2020 2020 2020  rimitive,.      
+0000be20: 2020 2020 2020 2020 2020 6469 7370 732c            disps,
+0000be30: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000be40: 2066 6f72 6365 732c 0a20 2020 2020 2020   forces,.       
+0000be50: 2020 2020 2020 2020 2066 635f 6361 6c63           fc_calc
+0000be60: 756c 6174 6f72 3d66 6333 5f63 616c 6375  ulator=fc3_calcu
+0000be70: 6c61 746f 722c 0a20 2020 2020 2020 2020  lator,.         
+0000be80: 2020 2020 2020 2066 635f 6361 6c63 756c         fc_calcul
+0000be90: 6174 6f72 5f6f 7074 696f 6e73 3d66 6333  ator_options=fc3
+0000bea0: 5f63 616c 6375 6c61 746f 725f 6f70 7469  _calculator_opti
+0000beb0: 6f6e 732c 0a20 2020 2020 2020 2020 2020  ons,.           
+0000bec0: 2020 2020 2069 735f 636f 6d70 6163 745f       is_compact_
+0000bed0: 6663 3d69 735f 636f 6d70 6163 745f 6663  fc=is_compact_fc
+0000bee0: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+0000bef0: 2020 6c6f 675f 6c65 7665 6c3d 7365 6c66    log_level=self
+0000bf00: 2e5f 6c6f 675f 6c65 7665 6c2c 0a20 2020  ._log_level,.   
+0000bf10: 2020 2020 2020 2020 2029 0a20 2020 2020           ).     
+0000bf20: 2020 2065 6c73 653a 0a20 2020 2020 2020     else:.       
+0000bf30: 2020 2020 2069 6620 2264 6973 706c 6163       if "displac
+0000bf40: 656d 656e 7473 2220 696e 2064 6973 705f  ements" in disp_
+0000bf50: 6461 7461 7365 743a 0a20 2020 2020 2020  dataset:.       
+0000bf60: 2020 2020 2020 2020 206d 7367 203d 2028           msg = (
+0000bf70: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000bf80: 2020 2020 2022 6663 5f63 616c 6375 6c61       "fc_calcula
+0000bf90: 746f 7220 6861 7320 746f 2062 6520 7365  tor has to be se
+0000bfa0: 7420 746f 2070 726f 6475 6365 2066 6f72  t to produce for
+0000bfb0: 6365 2022 0a20 2020 2020 2020 2020 2020  ce ".           
+0000bfc0: 2020 2020 2020 2020 2022 636f 6e73 7461           "consta
+0000bfd0: 6e73 2066 726f 6d20 7468 6973 2064 6174  ns from this dat
+0000bfe0: 6173 6574 2e22 0a20 2020 2020 2020 2020  aset.".         
+0000bff0: 2020 2020 2020 2029 0a20 2020 2020 2020         ).       
+0000c000: 2020 2020 2020 2020 2072 6169 7365 2046           raise F
+0000c010: 6f72 6365 4361 6c63 756c 6174 6f72 5265  orceCalculatorRe
+0000c020: 7175 6972 6564 4572 726f 7228 6d73 6729  quiredError(msg)
+0000c030: 0a20 2020 2020 2020 2020 2020 2066 6332  .            fc2
+0000c040: 2c20 6663 3320 3d20 6765 745f 7068 6f6e  , fc3 = get_phon
+0000c050: 6f33 7079 5f66 6333 280a 2020 2020 2020  o3py_fc3(.      
+0000c060: 2020 2020 2020 2020 2020 7365 6c66 2e5f            self._
+0000c070: 7375 7065 7263 656c 6c2c 0a20 2020 2020  supercell,.     
+0000c080: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+0000c090: 5f70 7269 6d69 7469 7665 2c0a 2020 2020  _primitive,.    
+0000c0a0: 2020 2020 2020 2020 2020 2020 6469 7370              disp
+0000c0b0: 5f64 6174 6173 6574 2c0a 2020 2020 2020  _dataset,.      
+0000c0c0: 2020 2020 2020 2020 2020 7365 6c66 2e5f            self._
+0000c0d0: 7379 6d6d 6574 7279 2c0a 2020 2020 2020  symmetry,.      
+0000c0e0: 2020 2020 2020 2020 2020 6973 5f63 6f6d            is_com
+0000c0f0: 7061 6374 5f66 633d 6973 5f63 6f6d 7061  pact_fc=is_compa
+0000c100: 6374 5f66 632c 0a20 2020 2020 2020 2020  ct_fc,.         
+0000c110: 2020 2020 2020 2076 6572 626f 7365 3d73         verbose=s
+0000c120: 656c 662e 5f6c 6f67 5f6c 6576 656c 2c0a  elf._log_level,.
+0000c130: 2020 2020 2020 2020 2020 2020 290a 2020              ).  
+0000c140: 2020 2020 2020 2020 2020 6966 2073 796d            if sym
+0000c150: 6d65 7472 697a 655f 6663 3372 3a0a 2020  metrize_fc3r:.  
+0000c160: 2020 2020 2020 2020 2020 2020 2020 6966                if
+0000c170: 2069 735f 636f 6d70 6163 745f 6663 3a0a   is_compact_fc:.
+0000c180: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c190: 2020 2020 7365 745f 7472 616e 736c 6174      set_translat
+0000c1a0: 696f 6e61 6c5f 696e 7661 7269 616e 6365  ional_invariance
+0000c1b0: 5f63 6f6d 7061 6374 5f66 6333 2866 6333  _compact_fc3(fc3
+0000c1c0: 2c20 7365 6c66 2e5f 7072 696d 6974 6976  , self._primitiv
+0000c1d0: 6529 0a20 2020 2020 2020 2020 2020 2020  e).             
+0000c1e0: 2020 2020 2020 2073 6574 5f70 6572 6d75         set_permu
+0000c1f0: 7461 7469 6f6e 5f73 796d 6d65 7472 795f  tation_symmetry_
+0000c200: 636f 6d70 6163 745f 6663 3328 6663 332c  compact_fc3(fc3,
+0000c210: 2073 656c 662e 5f70 7269 6d69 7469 7665   self._primitive
+0000c220: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
+0000c230: 2020 2020 2020 6966 2073 656c 662e 5f66        if self._f
+0000c240: 6332 2069 7320 4e6f 6e65 3a0a 2020 2020  c2 is None:.    
+0000c250: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c260: 2020 2020 7379 6d6d 6574 7269 7a65 5f63      symmetrize_c
+0000c270: 6f6d 7061 6374 5f66 6f72 6365 5f63 6f6e  ompact_force_con
+0000c280: 7374 616e 7473 2866 6332 2c20 7365 6c66  stants(fc2, self
+0000c290: 2e5f 7072 696d 6974 6976 6529 0a20 2020  ._primitive).   
+0000c2a0: 2020 2020 2020 2020 2020 2020 2065 6c73               els
+0000c2b0: 653a 0a20 2020 2020 2020 2020 2020 2020  e:.             
+0000c2c0: 2020 2020 2020 2073 6574 5f74 7261 6e73         set_trans
+0000c2d0: 6c61 7469 6f6e 616c 5f69 6e76 6172 6961  lational_invaria
+0000c2e0: 6e63 655f 6663 3328 6663 3329 0a20 2020  nce_fc3(fc3).   
+0000c2f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c300: 2073 6574 5f70 6572 6d75 7461 7469 6f6e   set_permutation
+0000c310: 5f73 796d 6d65 7472 795f 6663 3328 6663  _symmetry_fc3(fc
+0000c320: 3329 0a20 2020 2020 2020 2020 2020 2020  3).             
+0000c330: 2020 2020 2020 2069 6620 7365 6c66 2e5f         if self._
+0000c340: 6663 3220 6973 204e 6f6e 653a 0a20 2020  fc2 is None:.   
+0000c350: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c360: 2020 2020 2073 796d 6d65 7472 697a 655f       symmetrize_
+0000c370: 666f 7263 655f 636f 6e73 7461 6e74 7328  force_constants(
+0000c380: 6663 3229 0a0a 2020 2020 2020 2020 2320  fc2)..        # 
+0000c390: 5365 7420 6663 3220 616e 6420 6663 330a  Set fc2 and fc3.
+0000c3a0: 2020 2020 2020 2020 7365 6c66 2e5f 6663          self._fc
+0000c3b0: 3320 3d20 6663 330a 0a20 2020 2020 2020  3 = fc3..       
+0000c3c0: 2023 2066 6332 2061 7320 6f62 7461 696e   # fc2 as obtain
+0000c3d0: 6564 2061 626f 7665 2077 696c 6c20 6e6f  ed above will no
+0000c3e0: 7420 6265 2073 6574 2077 6865 6e20 227c  t be set when "|
+0000c3f0: 2220 696e 2066 632d 6361 6c63 756c 6174  " in fc-calculat
+0000c400: 6f72 2073 6574 7469 6e67 2e0a 2020 2020  or setting..    
+0000c410: 2020 2020 6966 2066 635f 6361 6c63 756c      if fc_calcul
+0000c420: 6174 6f72 2069 7320 6e6f 7420 4e6f 6e65  ator is not None
+0000c430: 2061 6e64 2022 7c22 2069 6e20 6663 5f63   and "|" in fc_c
+0000c440: 616c 6375 6c61 746f 723a 0a20 2020 2020  alculator:.     
+0000c450: 2020 2020 2020 2066 6332 203d 204e 6f6e         fc2 = Non
+0000c460: 650a 2020 2020 2020 2020 6966 2066 635f  e.        if fc_
+0000c470: 6361 6c63 756c 6174 6f72 5f6f 7074 696f  calculator_optio
+0000c480: 6e73 2069 7320 6e6f 7420 4e6f 6e65 2061  ns is not None a
+0000c490: 6e64 2022 7c22 2069 6e20 6663 5f63 616c  nd "|" in fc_cal
+0000c4a0: 6375 6c61 746f 725f 6f70 7469 6f6e 733a  culator_options:
+0000c4b0: 0a20 2020 2020 2020 2020 2020 2066 6332  .            fc2
+0000c4c0: 203d 204e 6f6e 650a 0a20 2020 2020 2020   = None..       
+0000c4d0: 2023 204e 6f72 6d61 6c6c 7920 7365 6c66   # Normally self
+0000c4e0: 2e5f 6663 3220 6973 206f 7665 7277 7269  ._fc2 is overwri
+0000c4f0: 7474 656e 2069 6e20 7072 6f64 7563 655f  tten in produce_
+0000c500: 6663 320a 2020 2020 2020 2020 6966 2073  fc2.        if s
+0000c510: 656c 662e 5f66 6332 2069 7320 4e6f 6e65  elf._fc2 is None
+0000c520: 3a0a 2020 2020 2020 2020 2020 2020 7365  :.            se
+0000c530: 6c66 2e5f 6663 3220 3d20 6663 320a 0a20  lf._fc2 = fc2.. 
+0000c540: 2020 2064 6566 2070 726f 6475 6365 5f66     def produce_f
+0000c550: 6332 280a 2020 2020 2020 2020 7365 6c66  c2(.        self
+0000c560: 2c0a 2020 2020 2020 2020 7379 6d6d 6574  ,.        symmet
+0000c570: 7269 7a65 5f66 6332 3d46 616c 7365 2c0a  rize_fc2=False,.
+0000c580: 2020 2020 2020 2020 6973 5f63 6f6d 7061          is_compa
+0000c590: 6374 5f66 633d 4661 6c73 652c 0a20 2020  ct_fc=False,.   
+0000c5a0: 2020 2020 2066 635f 6361 6c63 756c 6174       fc_calculat
+0000c5b0: 6f72 3d4e 6f6e 652c 0a20 2020 2020 2020  or=None,.       
+0000c5c0: 2066 635f 6361 6c63 756c 6174 6f72 5f6f   fc_calculator_o
+0000c5d0: 7074 696f 6e73 3d4e 6f6e 652c 0a20 2020  ptions=None,.   
+0000c5e0: 2029 3a0a 2020 2020 2020 2020 2222 2243   ):.        """C
+0000c5f0: 616c 6375 6c61 7465 2066 6332 2066 726f  alculate fc2 fro
+0000c600: 6d20 6469 7370 6c61 6365 6d65 6e74 7320  m displacements 
+0000c610: 616e 6420 666f 7263 6573 2e0a 0a20 2020  and forces...   
+0000c620: 2020 2020 2050 6172 616d 6574 6572 730a       Parameters.
+0000c630: 2020 2020 2020 2020 2d2d 2d2d 2d2d 2d2d          --------
+0000c640: 2d2d 0a20 2020 2020 2020 2073 796d 6d65  --.        symme
+0000c650: 7472 697a 655f 6663 3220 3a20 626f 6f6c  trize_fc2 : bool
+0000c660: 0a20 2020 2020 2020 2020 2020 204f 6e6c  .            Onl
+0000c670: 7920 666f 7220 7479 7065 2031 2064 6973  y for type 1 dis
+0000c680: 706c 6163 656d 656e 745f 6461 7461 7365  placement_datase
+0000c690: 742c 2074 7261 6e73 6c61 7469 6f6e 616c  t, translational
+0000c6a0: 2061 6e64 0a20 2020 2020 2020 2020 2020   and.           
+0000c6b0: 2070 6572 6d75 7461 7469 6f6e 2073 796d   permutation sym
+0000c6c0: 6d65 7472 6965 7320 6172 6520 6170 706c  metries are appl
+0000c6d0: 6965 6420 6166 7465 7220 6372 6561 7469  ied after creati
+0000c6e0: 6e67 2066 6333 2e20 5468 6973 0a20 2020  ng fc3. This.   
+0000c6f0: 2020 2020 2020 2020 2073 796d 6d65 7472           symmetr
+0000c700: 697a 6174 696f 6e20 6973 206e 6f74 2076  ization is not v
+0000c710: 6572 7920 736f 7068 6973 7469 6361 7465  ery sophisticate
+0000c720: 6420 616e 6420 6361 6e20 6272 6561 6b20  d and can break 
+0000c730: 7370 6163 650a 2020 2020 2020 2020 2020  space.          
+0000c740: 2020 6772 6f75 7020 7379 6d6d 6574 7279    group symmetry
+0000c750: 2c20 6275 7420 6f66 7465 6e20 7573 6566  , but often usef
+0000c760: 756c 2e20 4966 2062 6574 7465 7220 7379  ul. If better sy
+0000c770: 6d6d 6574 7269 7a61 7469 6f6e 2069 730a  mmetrization is.
+0000c780: 2020 2020 2020 2020 2020 2020 6578 7065              expe
+0000c790: 6374 6564 2c20 6974 2069 7320 7265 636f  cted, it is reco
+0000c7a0: 6d6d 656e 6465 6420 746f 2075 7365 2065  mmended to use e
+0000c7b0: 7874 6572 6e61 6c20 666f 7263 6520 636f  xternal force co
+0000c7c0: 6e73 7461 6e74 730a 2020 2020 2020 2020  nstants.        
+0000c7d0: 2020 2020 6361 6c63 756c 6174 6f72 2073      calculator s
+0000c7e0: 7563 6820 6173 2041 4c4d 2e20 4465 6661  uch as ALM. Defa
+0000c7f0: 756c 7420 6973 2046 616c 7365 2e0a 2020  ult is False..  
+0000c800: 2020 2020 2020 6973 5f63 6f6d 7061 6374        is_compact
+0000c810: 5f66 6320 3a20 626f 6f6c 0a20 2020 2020  _fc : bool.     
+0000c820: 2020 2020 2020 2066 6332 2073 6861 7065         fc2 shape
+0000c830: 2069 730a 2020 2020 2020 2020 2020 2020   is.            
+0000c840: 2020 2020 4661 6c73 653a 2028 7375 7065      False: (supe
+0000c850: 7263 656c 6c2c 2073 7570 6563 656c 6c2c  rcell, supecell,
+0000c860: 2033 2c20 3329 0a20 2020 2020 2020 2020   3, 3).         
+0000c870: 2020 2020 2020 2054 7275 653a 2028 7072         True: (pr
+0000c880: 696d 6974 6976 652c 2073 7570 6563 656c  imitive, supecel
+0000c890: 6c2c 2033 2c20 3329 0a20 2020 2020 2020  l, 3, 3).       
+0000c8a0: 2020 2020 2077 6865 7265 2027 7375 7065       where 'supe
+0000c8b0: 7263 656c 6c27 2061 6e64 2027 7072 696d  rcell' and 'prim
+0000c8c0: 6974 6976 6527 2069 6e64 6963 6174 6520  itive' indicate 
+0000c8d0: 6e75 6d62 6572 206f 6620 6174 6f6d 7320  number of atoms 
+0000c8e0: 696e 2074 6865 7365 0a20 2020 2020 2020  in these.       
+0000c8f0: 2020 2020 2063 656c 6c73 2e20 4465 6661       cells. Defa
+0000c900: 756c 7420 6973 2046 616c 7365 2e0a 2020  ult is False..  
+0000c910: 2020 2020 2020 6663 5f63 616c 6375 6c61        fc_calcula
+0000c920: 746f 7220 3a20 7374 7220 6f72 204e 6f6e  tor : str or Non
+0000c930: 650a 2020 2020 2020 2020 2020 2020 466f  e.            Fo
+0000c940: 7263 6520 636f 6e73 7461 6e74 7320 6361  rce constants ca
+0000c950: 6c63 756c 6174 6f72 2067 6976 656e 2062  lculator given b
+0000c960: 7920 7374 722e 0a20 2020 2020 2020 2066  y str..        f
+0000c970: 635f 6361 6c63 756c 6174 6f72 5f6f 7074  c_calculator_opt
+0000c980: 696f 6e73 203a 2064 6963 740a 2020 2020  ions : dict.    
+0000c990: 2020 2020 2020 2020 4f70 7469 6f6e 7320          Options 
+0000c9a0: 666f 7220 6578 7465 726e 616c 2066 6f72  for external for
+0000c9b0: 6365 2063 6f6e 7374 616e 7473 2063 616c  ce constants cal
+0000c9c0: 6375 6c61 746f 722e 0a0a 2020 2020 2020  culator...      
+0000c9d0: 2020 2222 220a 2020 2020 2020 2020 6966    """.        if
+0000c9e0: 2073 656c 662e 5f70 686f 6e6f 6e5f 6461   self._phonon_da
+0000c9f0: 7461 7365 7420 6973 204e 6f6e 653a 0a20  taset is None:. 
+0000ca00: 2020 2020 2020 2020 2020 2064 6973 705f             disp_
+0000ca10: 6461 7461 7365 7420 3d20 7365 6c66 2e5f  dataset = self._
+0000ca20: 6461 7461 7365 740a 2020 2020 2020 2020  dataset.        
+0000ca30: 656c 7365 3a0a 2020 2020 2020 2020 2020  else:.          
+0000ca40: 2020 6469 7370 5f64 6174 6173 6574 203d    disp_dataset =
+0000ca50: 2073 656c 662e 5f70 686f 6e6f 6e5f 6461   self._phonon_da
+0000ca60: 7461 7365 740a 0a20 2020 2020 2020 2069  taset..        i
+0000ca70: 6620 6973 5f63 6f6d 7061 6374 5f66 633a  f is_compact_fc:
+0000ca80: 0a20 2020 2020 2020 2020 2020 2070 3273  .            p2s
+0000ca90: 5f6d 6170 203d 2073 656c 662e 5f70 686f  _map = self._pho
+0000caa0: 6e6f 6e5f 7072 696d 6974 6976 652e 7032  non_primitive.p2
+0000cab0: 735f 6d61 700a 2020 2020 2020 2020 656c  s_map.        el
+0000cac0: 7365 3a0a 2020 2020 2020 2020 2020 2020  se:.            
+0000cad0: 7032 735f 6d61 7020 3d20 4e6f 6e65 0a0a  p2s_map = None..
+0000cae0: 2020 2020 2020 2020 6663 325f 6361 6c63          fc2_calc
+0000caf0: 756c 6174 6f72 2c20 6663 325f 6361 6c63  ulator, fc2_calc
+0000cb00: 756c 6174 6f72 5f6f 7074 696f 6e73 203d  ulator_options =
+0000cb10: 2073 656c 662e 5f65 7874 7261 6374 5f66   self._extract_f
+0000cb20: 6332 5f66 6333 5f63 616c 6375 6c61 746f  c2_fc3_calculato
+0000cb30: 7273 280a 2020 2020 2020 2020 2020 2020  rs(.            
+0000cb40: 6663 5f63 616c 6375 6c61 746f 722c 2066  fc_calculator, f
+0000cb50: 635f 6361 6c63 756c 6174 6f72 5f6f 7074  c_calculator_opt
+0000cb60: 696f 6e73 2c20 320a 2020 2020 2020 2020  ions, 2.        
+0000cb70: 290a 0a20 2020 2020 2020 2069 6620 6663  )..        if fc
+0000cb80: 325f 6361 6c63 756c 6174 6f72 2069 7320  2_calculator is 
+0000cb90: 6e6f 7420 4e6f 6e65 3a0a 2020 2020 2020  not None:.      
+0000cba0: 2020 2020 2020 6469 7370 732c 2066 6f72        disps, for
+0000cbb0: 6365 7320 3d20 6765 745f 6469 7370 6c61  ces = get_displa
+0000cbc0: 6365 6d65 6e74 735f 616e 645f 666f 7263  cements_and_forc
+0000cbd0: 6573 2864 6973 705f 6461 7461 7365 7429  es(disp_dataset)
+0000cbe0: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
+0000cbf0: 662e 5f66 6332 203d 2067 6574 5f66 6332  f._fc2 = get_fc2
+0000cc00: 280a 2020 2020 2020 2020 2020 2020 2020  (.              
+0000cc10: 2020 7365 6c66 2e5f 7068 6f6e 6f6e 5f73    self._phonon_s
+0000cc20: 7570 6572 6365 6c6c 2c0a 2020 2020 2020  upercell,.      
+0000cc30: 2020 2020 2020 2020 2020 7365 6c66 2e5f            self._
+0000cc40: 7068 6f6e 6f6e 5f70 7269 6d69 7469 7665  phonon_primitive
+0000cc50: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+0000cc60: 2020 6469 7370 732c 0a20 2020 2020 2020    disps,.       
+0000cc70: 2020 2020 2020 2020 2066 6f72 6365 732c           forces,
+0000cc80: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000cc90: 2066 635f 6361 6c63 756c 6174 6f72 3d66   fc_calculator=f
+0000cca0: 6332 5f63 616c 6375 6c61 746f 722c 0a20  c2_calculator,. 
+0000ccb0: 2020 2020 2020 2020 2020 2020 2020 2066                 f
+0000ccc0: 635f 6361 6c63 756c 6174 6f72 5f6f 7074  c_calculator_opt
+0000ccd0: 696f 6e73 3d66 6332 5f63 616c 6375 6c61  ions=fc2_calcula
+0000cce0: 746f 725f 6f70 7469 6f6e 732c 0a20 2020  tor_options,.   
+0000ccf0: 2020 2020 2020 2020 2020 2020 2061 746f               ato
+0000cd00: 6d5f 6c69 7374 3d70 3273 5f6d 6170 2c0a  m_list=p2s_map,.
+0000cd10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000cd20: 6c6f 675f 6c65 7665 6c3d 7365 6c66 2e5f  log_level=self._
+0000cd30: 6c6f 675f 6c65 7665 6c2c 0a20 2020 2020  log_level,.     
+0000cd40: 2020 2020 2020 2029 0a20 2020 2020 2020         ).       
+0000cd50: 2065 6c73 653a 0a20 2020 2020 2020 2020   else:.         
+0000cd60: 2020 2069 6620 2264 6973 706c 6163 656d     if "displacem
+0000cd70: 656e 7473 2220 696e 2064 6973 705f 6461  ents" in disp_da
+0000cd80: 7461 7365 743a 0a20 2020 2020 2020 2020  taset:.         
+0000cd90: 2020 2020 2020 206d 7367 203d 2028 0a20         msg = (. 
+0000cda0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000cdb0: 2020 2022 6663 5f63 616c 6375 6c61 746f     "fc_calculato
+0000cdc0: 7220 6861 7320 746f 2062 6520 7365 7420  r has to be set 
+0000cdd0: 746f 2070 726f 6475 6365 2066 6f72 6365  to produce force
+0000cde0: 2022 0a20 2020 2020 2020 2020 2020 2020   ".             
+0000cdf0: 2020 2020 2020 2022 636f 6e73 7461 6e73         "constans
+0000ce00: 2066 726f 6d20 7468 6973 2064 6174 6173   from this datas
+0000ce10: 6574 2066 6f72 2066 6332 2e22 0a20 2020  et for fc2.".   
+0000ce20: 2020 2020 2020 2020 2020 2020 2029 0a20               ). 
+0000ce30: 2020 2020 2020 2020 2020 2020 2020 2072                 r
+0000ce40: 6169 7365 2052 756e 7469 6d65 4572 726f  aise RuntimeErro
+0000ce50: 7228 6d73 6729 0a20 2020 2020 2020 2020  r(msg).         
+0000ce60: 2020 2073 656c 662e 5f66 6332 203d 2067     self._fc2 = g
+0000ce70: 6574 5f70 686f 6e6f 7079 5f66 6332 280a  et_phonopy_fc2(.
+0000ce80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ce90: 7365 6c66 2e5f 7068 6f6e 6f6e 5f73 7570  self._phonon_sup
+0000cea0: 6572 6365 6c6c 2c0a 2020 2020 2020 2020  ercell,.        
+0000ceb0: 2020 2020 2020 2020 7365 6c66 2e5f 7068          self._ph
+0000cec0: 6f6e 6f6e 5f73 7570 6572 6365 6c6c 5f73  onon_supercell_s
+0000ced0: 796d 6d65 7472 792c 0a20 2020 2020 2020  ymmetry,.       
+0000cee0: 2020 2020 2020 2020 2064 6973 705f 6461           disp_da
+0000cef0: 7461 7365 742c 0a20 2020 2020 2020 2020  taset,.         
+0000cf00: 2020 2020 2020 2061 746f 6d5f 6c69 7374         atom_list
+0000cf10: 3d70 3273 5f6d 6170 2c0a 2020 2020 2020  =p2s_map,.      
+0000cf20: 2020 2020 2020 290a 2020 2020 2020 2020        ).        
+0000cf30: 2020 2020 6966 2073 796d 6d65 7472 697a      if symmetriz
+0000cf40: 655f 6663 323a 0a20 2020 2020 2020 2020  e_fc2:.         
+0000cf50: 2020 2020 2020 2069 6620 6973 5f63 6f6d         if is_com
+0000cf60: 7061 6374 5f66 633a 0a20 2020 2020 2020  pact_fc:.       
+0000cf70: 2020 2020 2020 2020 2020 2020 2073 796d               sym
+0000cf80: 6d65 7472 697a 655f 636f 6d70 6163 745f  metrize_compact_
+0000cf90: 666f 7263 655f 636f 6e73 7461 6e74 7328  force_constants(
+0000cfa0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000cfb0: 2020 2020 2020 2020 2073 656c 662e 5f66           self._f
+0000cfc0: 6332 2c20 7365 6c66 2e5f 7068 6f6e 6f6e  c2, self._phonon
+0000cfd0: 5f70 7269 6d69 7469 7665 0a20 2020 2020  _primitive.     
+0000cfe0: 2020 2020 2020 2020 2020 2020 2020 2029                 )
+0000cff0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000d000: 2065 6c73 653a 0a20 2020 2020 2020 2020   else:.         
+0000d010: 2020 2020 2020 2020 2020 2073 796d 6d65             symme
+0000d020: 7472 697a 655f 666f 7263 655f 636f 6e73  trize_force_cons
+0000d030: 7461 6e74 7328 7365 6c66 2e5f 6663 3229  tants(self._fc2)
+0000d040: 0a0a 2020 2020 6465 6620 6375 746f 6666  ..    def cutoff
+0000d050: 5f66 6333 5f62 795f 7a65 726f 2873 656c  _fc3_by_zero(sel
+0000d060: 662c 2063 7574 6f66 665f 6469 7374 616e  f, cutoff_distan
+0000d070: 6365 2c20 6663 333d 4e6f 6e65 293a 0a20  ce, fc3=None):. 
+0000d080: 2020 2020 2020 2022 2222 5365 7420 7a65         """Set ze
+0000d090: 726f 2074 6f20 6663 3320 656c 656d 656e  ro to fc3 elemen
+0000d0a0: 7473 206f 7574 206f 6620 6375 746f 6666  ts out of cutoff
+0000d0b0: 2064 6973 7461 6e63 652e 0a0a 2020 2020   distance...    
+0000d0c0: 2020 2020 4e6f 7465 0a20 2020 2020 2020      Note.       
+0000d0d0: 202d 2d2d 2d0a 2020 2020 2020 2020 6663   ----.        fc
+0000d0e0: 3320 6973 206f 7665 7277 7269 7474 656e  3 is overwritten
+0000d0f0: 2e0a 0a20 2020 2020 2020 2050 6172 616d  ...        Param
+0000d100: 6574 6572 730a 2020 2020 2020 2020 2d2d  eters.        --
+0000d110: 2d2d 2d2d 2d2d 2d2d 0a20 2020 2020 2020  --------.       
+0000d120: 2063 7574 6f66 665f 6469 7374 616e 6365   cutoff_distance
+0000d130: 203a 2066 6c6f 6174 0a20 2020 2020 2020   : float.       
+0000d140: 2020 2020 2041 6674 6572 2063 7265 6174       After creat
+0000d150: 696e 6720 666f 7263 6520 636f 6e73 7461  ing force consta
+0000d160: 6e74 732c 2066 6320 656c 656d 656e 7473  nts, fc elements
+0000d170: 2077 6865 7265 2061 6e79 2070 6169 720a   where any pair.
+0000d180: 2020 2020 2020 2020 2020 2020 6469 7374              dist
+0000d190: 616e 6365 2069 6e20 6174 6f6d 2074 7269  ance in atom tri
+0000d1a0: 706c 6574 7320 6c61 7267 6572 2074 6861  plets larger tha
+0000d1b0: 6e20 6375 746f 6666 5f64 6973 7461 6e63  n cutoff_distanc
+0000d1c0: 6520 6172 6520 7365 7420 7a65 726f 2e0a  e are set zero..
+0000d1d0: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
+0000d1e0: 2020 2020 2069 6620 6663 3320 6973 204e       if fc3 is N
+0000d1f0: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
+0000d200: 205f 6663 3320 3d20 7365 6c66 2e5f 6663   _fc3 = self._fc
+0000d210: 330a 2020 2020 2020 2020 656c 7365 3a0a  3.        else:.
+0000d220: 2020 2020 2020 2020 2020 2020 5f66 6333              _fc3
+0000d230: 203d 2066 6333 0a20 2020 2020 2020 2063   = fc3.        c
+0000d240: 7574 6f66 665f 6663 335f 6279 5f7a 6572  utoff_fc3_by_zer
+0000d250: 6f28 0a20 2020 2020 2020 2020 2020 205f  o(.            _
+0000d260: 6663 332c 0a20 2020 2020 2020 2020 2020  fc3,.           
+0000d270: 2073 656c 662e 5f73 7570 6572 6365 6c6c   self._supercell
+0000d280: 2c0a 2020 2020 2020 2020 2020 2020 6375  ,.            cu
+0000d290: 746f 6666 5f64 6973 7461 6e63 652c 0a20  toff_distance,. 
+0000d2a0: 2020 2020 2020 2020 2020 2070 3273 5f6d             p2s_m
+0000d2b0: 6170 3d73 656c 662e 5f70 7269 6d69 7469  ap=self._primiti
+0000d2c0: 7665 2e70 3273 5f6d 6170 2c0a 2020 2020  ve.p2s_map,.    
+0000d2d0: 2020 2020 2020 2020 7379 6d70 7265 633d          symprec=
+0000d2e0: 7365 6c66 2e5f 7379 6d70 7265 632c 0a20  self._symprec,. 
+0000d2f0: 2020 2020 2020 2029 0a0a 2020 2020 6465         )..    de
+0000d300: 6620 7365 745f 7065 726d 7574 6174 696f  f set_permutatio
+0000d310: 6e5f 7379 6d6d 6574 7279 2873 656c 6629  n_symmetry(self)
+0000d320: 3a0a 2020 2020 2020 2020 2222 2245 6e66  :.        """Enf
+0000d330: 6f72 6365 2070 6572 6d75 7461 7469 6f6e  orce permutation
+0000d340: 2073 796d 6d65 7472 7920 746f 2066 6332   symmetry to fc2
+0000d350: 2061 6e64 2066 6333 2e22 2222 0a20 2020   and fc3.""".   
+0000d360: 2020 2020 2069 6620 7365 6c66 2e5f 6663       if self._fc
+0000d370: 3220 6973 206e 6f74 204e 6f6e 653a 0a20  2 is not None:. 
+0000d380: 2020 2020 2020 2020 2020 2073 6574 5f70             set_p
+0000d390: 6572 6d75 7461 7469 6f6e 5f73 796d 6d65  ermutation_symme
+0000d3a0: 7472 7928 7365 6c66 2e5f 6663 3229 0a20  try(self._fc2). 
+0000d3b0: 2020 2020 2020 2069 6620 7365 6c66 2e5f         if self._
+0000d3c0: 6663 3320 6973 206e 6f74 204e 6f6e 653a  fc3 is not None:
+0000d3d0: 0a20 2020 2020 2020 2020 2020 2073 6574  .            set
+0000d3e0: 5f70 6572 6d75 7461 7469 6f6e 5f73 796d  _permutation_sym
+0000d3f0: 6d65 7472 795f 6663 3328 7365 6c66 2e5f  metry_fc3(self._
+0000d400: 6663 3329 0a0a 2020 2020 6465 6620 7365  fc3)..    def se
+0000d410: 745f 7472 616e 736c 6174 696f 6e61 6c5f  t_translational_
+0000d420: 696e 7661 7269 616e 6365 2873 656c 6629  invariance(self)
+0000d430: 3a0a 2020 2020 2020 2020 2222 2245 6e66  :.        """Enf
+0000d440: 6f72 6365 2074 7261 6e73 6c61 7469 6f6e  orce translation
+0000d450: 2069 6e76 6172 6961 6e63 652e 0a0a 2020   invariance...  
+0000d460: 2020 2020 2020 5468 6973 2073 7562 7472        This subtr
+0000d470: 6163 7473 2064 7269 6674 2064 6976 6964  acts drift divid
+0000d480: 6564 2062 7920 6e75 6d62 6572 206f 6620  ed by number of 
+0000d490: 656c 656d 656e 7473 2069 6e20 6561 6368  elements in each
+0000d4a0: 2072 6f77 2061 6e64 0a20 2020 2020 2020   row and.       
+0000d4b0: 2063 6f6c 756d 6e2e 0a0a 2020 2020 2020   column...      
+0000d4c0: 2020 2222 220a 2020 2020 2020 2020 6966    """.        if
+0000d4d0: 2073 656c 662e 5f66 6332 2069 7320 6e6f   self._fc2 is no
+0000d4e0: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
+0000d4f0: 2020 2020 7365 745f 7472 616e 736c 6174      set_translat
+0000d500: 696f 6e61 6c5f 696e 7661 7269 616e 6365  ional_invariance
+0000d510: 2873 656c 662e 5f66 6332 290a 2020 2020  (self._fc2).    
+0000d520: 2020 2020 6966 2073 656c 662e 5f66 6333      if self._fc3
+0000d530: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
+0000d540: 2020 2020 2020 2020 2020 7365 745f 7472            set_tr
+0000d550: 616e 736c 6174 696f 6e61 6c5f 696e 7661  anslational_inva
+0000d560: 7269 616e 6365 5f66 6333 2873 656c 662e  riance_fc3(self.
+0000d570: 5f66 6333 290a 0a20 2020 2064 6566 2072  _fc3)..    def r
+0000d580: 756e 5f69 6d61 675f 7365 6c66 5f65 6e65  un_imag_self_ene
+0000d590: 7267 7928 0a20 2020 2020 2020 2073 656c  rgy(.        sel
+0000d5a0: 662c 0a20 2020 2020 2020 2067 7269 645f  f,.        grid_
+0000d5b0: 706f 696e 7473 2c0a 2020 2020 2020 2020  points,.        
+0000d5c0: 7465 6d70 6572 6174 7572 6573 2c0a 2020  temperatures,.  
+0000d5d0: 2020 2020 2020 6672 6571 7565 6e63 795f        frequency_
+0000d5e0: 706f 696e 7473 3d4e 6f6e 652c 0a20 2020  points=None,.   
+0000d5f0: 2020 2020 2066 7265 7175 656e 6379 5f73       frequency_s
+0000d600: 7465 703d 4e6f 6e65 2c0a 2020 2020 2020  tep=None,.      
+0000d610: 2020 6e75 6d5f 6672 6571 7565 6e63 795f    num_frequency_
+0000d620: 706f 696e 7473 3d4e 6f6e 652c 0a20 2020  points=None,.   
+0000d630: 2020 2020 206e 756d 5f70 6f69 6e74 735f       num_points_
+0000d640: 696e 5f62 6174 6368 3d4e 6f6e 652c 0a20  in_batch=None,. 
+0000d650: 2020 2020 2020 2066 7265 7175 656e 6379         frequency
+0000d660: 5f70 6f69 6e74 735f 6174 5f62 616e 6473  _points_at_bands
+0000d670: 3d46 616c 7365 2c0a 2020 2020 2020 2020  =False,.        
+0000d680: 7363 6174 7465 7269 6e67 5f65 7665 6e74  scattering_event
+0000d690: 5f63 6c61 7373 3d4e 6f6e 652c 0a20 2020  _class=None,.   
+0000d6a0: 2020 2020 2077 7269 7465 5f74 7874 3d46       write_txt=F
+0000d6b0: 616c 7365 2c0a 2020 2020 2020 2020 7772  alse,.        wr
+0000d6c0: 6974 655f 6761 6d6d 615f 6465 7461 696c  ite_gamma_detail
+0000d6d0: 3d46 616c 7365 2c0a 2020 2020 2020 2020  =False,.        
+0000d6e0: 6b65 6570 5f67 616d 6d61 5f64 6574 6169  keep_gamma_detai
+0000d6f0: 6c3d 4661 6c73 652c 0a20 2020 2020 2020  l=False,.       
+0000d700: 206f 7574 7075 745f 6669 6c65 6e61 6d65   output_filename
+0000d710: 3d4e 6f6e 652c 0a20 2020 2029 3a0a 2020  =None,.    ):.  
+0000d720: 2020 2020 2020 2222 2243 616c 6375 6c61        """Calcula
+0000d730: 7465 2069 6d61 6769 6e61 7279 2070 6172  te imaginary par
+0000d740: 7420 6f66 2073 656c 662d 656e 6572 6779  t of self-energy
+0000d750: 206f 6620 6275 6262 6c65 2064 6961 6772   of bubble diagr
+0000d760: 616d 2028 4761 6d6d 6129 2e0a 0a20 2020  am (Gamma)...   
+0000d770: 2020 2020 2050 6920 3d20 4465 6c74 6120       Pi = Delta 
+0000d780: 2d20 6920 4761 6d6d 612e 0a0a 2020 2020  - i Gamma...    
+0000d790: 2020 2020 5061 7261 6d65 7465 7273 0a20      Parameters. 
+0000d7a0: 2020 2020 2020 202d 2d2d 2d2d 2d2d 2d2d         ---------
+0000d7b0: 2d0a 2020 2020 2020 2020 6772 6964 5f70  -.        grid_p
+0000d7c0: 6f69 6e74 7320 3a20 6172 7261 795f 6c69  oints : array_li
+0000d7d0: 6b65 0a20 2020 2020 2020 2020 2020 2047  ke.            G
+0000d7e0: 7269 642d 706f 696e 7420 696e 6469 6365  rid-point indice
+0000d7f0: 7320 7768 6572 6520 696d 6167 696e 6172  s where imaginar
+0000d800: 7920 7061 7274 206f 6620 7365 6c66 2d65  y part of self-e
+0000d810: 6e65 7267 6965 7320 6172 650a 2020 2020  nergies are.    
+0000d820: 2020 2020 2020 2020 6361 636c 6375 6c61          caclcula
+0000d830: 7465 642e 0a20 2020 2020 2020 2020 2020  ted..           
+0000d840: 2064 7479 7065 3d69 6e74 2c20 7368 6170   dtype=int, shap
+0000d850: 653d 2867 7269 645f 706f 696e 7473 2c29  e=(grid_points,)
+0000d860: 0a20 2020 2020 2020 2074 656d 7065 7261  .        tempera
+0000d870: 7475 7265 7320 3a20 6172 7261 795f 6c69  tures : array_li
+0000d880: 6b65 0a20 2020 2020 2020 2020 2020 2054  ke.            T
+0000d890: 656d 7065 7261 7475 7265 7320 7768 6572  emperatures wher
+0000d8a0: 6520 696d 6167 696e 6172 7920 7061 7274  e imaginary part
+0000d8b0: 206f 6620 7365 6c66 2d65 6e65 7267 6965   of self-energie
+0000d8c0: 7320 6172 6520 6361 6c63 756c 6174 6564  s are calculated
+0000d8d0: 2e0a 2020 2020 2020 2020 2020 2020 6474  ..            dt
+0000d8e0: 7970 653d 666c 6f61 742c 2073 6861 7065  ype=float, shape
+0000d8f0: 3d28 7465 6d70 6572 6174 7572 6573 2c29  =(temperatures,)
+0000d900: 0a20 2020 2020 2020 2066 7265 7175 656e  .        frequen
+0000d910: 6379 5f70 6f69 6e74 7320 3a20 6172 7261  cy_points : arra
+0000d920: 795f 6c69 6b65 2c20 6f70 7469 6f6e 616c  y_like, optional
+0000d930: 0a20 2020 2020 2020 2020 2020 2046 7265  .            Fre
+0000d940: 7175 656e 6379 2073 616d 706c 696e 6720  quency sampling 
+0000d950: 706f 696e 7473 2e20 4465 6661 756c 7420  points. Default 
+0000d960: 6973 204e 6f6e 652e 2057 6974 680a 2020  is None. With.  
+0000d970: 2020 2020 2020 2020 2020 6672 6571 7565            freque
+0000d980: 6e63 795f 706f 696e 7473 5f61 745f 6261  ncy_points_at_ba
+0000d990: 6e64 733d 4661 6c73 6520 616e 6420 6672  nds=False and fr
+0000d9a0: 6571 7565 6e63 795f 706f 696e 7473 2069  equency_points i
+0000d9b0: 7320 4e6f 6e65 2c0a 2020 2020 2020 2020  s None,.        
+0000d9c0: 2020 2020 6e75 6d5f 6672 6571 7565 6e63      num_frequenc
+0000d9d0: 795f 706f 696e 7473 206f 7220 6672 6571  y_points or freq
+0000d9e0: 7565 6e63 795f 7374 6570 2069 7320 7573  uency_step is us
+0000d9f0: 6564 2074 6f20 6765 6e65 7261 7465 2075  ed to generate u
+0000da00: 6e69 666f 726d 0a20 2020 2020 2020 2020  niform.         
+0000da10: 2020 2066 7265 7175 656e 6379 2073 616d     frequency sam
+0000da20: 706c 696e 6720 706f 696e 7473 2e0a 2020  pling points..  
+0000da30: 2020 2020 2020 2020 2020 6474 7970 653d            dtype=
+0000da40: 666c 6f61 742c 2073 6861 7065 3d28 6672  float, shape=(fr
+0000da50: 6571 7565 6e63 795f 706f 696e 7473 2c29  equency_points,)
+0000da60: 0a20 2020 2020 2020 2066 7265 7175 656e  .        frequen
+0000da70: 6379 5f73 7465 7020 3a20 666c 6f61 742c  cy_step : float,
+0000da80: 206f 7074 696f 6e61 6c0a 2020 2020 2020   optional.      
+0000da90: 2020 2020 2020 556e 6966 6f72 6d20 7069        Uniform pi
+0000daa0: 7463 6820 6f66 2066 7265 7175 656e 6379  tch of frequency
+0000dab0: 2073 616d 706c 696e 6720 706f 696e 7473   sampling points
+0000dac0: 2e20 4465 6661 756c 7420 6973 204e 6f6e  . Default is Non
+0000dad0: 652e 2054 6869 730a 2020 2020 2020 2020  e. This.        
+0000dae0: 2020 2020 7265 7375 6c74 7320 696e 2075      results in u
+0000daf0: 7369 6e67 206e 756d 5f66 7265 7175 656e  sing num_frequen
+0000db00: 6379 5f70 6f69 6e74 732e 0a20 2020 2020  cy_points..     
+0000db10: 2020 206e 756d 5f66 7265 7175 656e 6379     num_frequency
+0000db20: 5f70 6f69 6e74 733a 2049 6e74 2c20 6f70  _points: Int, op
+0000db30: 7469 6f6e 616c 0a20 2020 2020 2020 2020  tional.         
+0000db40: 2020 204e 756d 6265 7220 6f66 2073 616d     Number of sam
+0000db50: 706c 696e 6720 7361 6d70 6c69 6e67 2070  pling sampling p
+0000db60: 6f69 6e74 7320 746f 2062 6520 7573 6564  oints to be used
+0000db70: 2069 6e73 7465 6164 206f 660a 2020 2020   instead of.    
+0000db80: 2020 2020 2020 2020 6672 6571 7565 6e63          frequenc
+0000db90: 795f 7374 6570 2e20 5468 6973 206e 756d  y_step. This num
+0000dba0: 6265 7220 696e 636c 7564 6573 2065 6e64  ber includes end
+0000dbb0: 2070 6f69 6e74 732e 2044 6566 6175 6c74   points. Default
+0000dbc0: 2069 7320 4e6f 6e65 2c0a 2020 2020 2020   is None,.      
+0000dbd0: 2020 2020 2020 7768 6963 6820 6769 7665        which give
+0000dbe0: 7320 3230 312e 0a20 2020 2020 2020 206e  s 201..        n
+0000dbf0: 756d 5f70 6f69 6e74 735f 696e 5f62 6174  um_points_in_bat
+0000dc00: 6368 3a20 696e 742c 206f 7074 696f 6e61  ch: int, optiona
+0000dc10: 6c0a 2020 2020 2020 2020 2020 2020 4e75  l.            Nu
+0000dc20: 6d62 6572 206f 6620 7361 6d70 6c69 6e67  mber of sampling
+0000dc30: 2070 6f69 6e74 7320 696e 206f 6e65 2062   points in one b
+0000dc40: 6174 6368 2e20 5468 6973 2069 7320 666f  atch. This is fo
+0000dc50: 7220 7468 6520 6672 6571 7565 6e63 790a  r the frequency.
+0000dc60: 2020 2020 2020 2020 2020 2020 7361 6d70              samp
+0000dc70: 6c69 6e67 206d 6f64 6520 616e 6420 7468  ling mode and th
+0000dc80: 6520 7361 6d70 6c69 6e67 2070 6f69 6e74  e sampling point
+0000dc90: 7320 6172 6520 6469 7669 6465 6420 696e  s are divided in
+0000dca0: 746f 2062 6174 6368 6573 2e0a 2020 2020  to batches..    
+0000dcb0: 2020 2020 2020 2020 4c61 6765 7220 6e75          Lager nu
+0000dcc0: 6d62 6572 2070 726f 7669 6465 7320 6566  mber provides ef
+0000dcd0: 6669 6369 656e 7420 7573 6520 6f66 206d  ficient use of m
+0000dce0: 756c 7469 2d63 6f72 6573 2062 7574 206d  ulti-cores but m
+0000dcf0: 6f72 650a 2020 2020 2020 2020 2020 2020  ore.            
+0000dd00: 6d65 6d6f 7279 2064 656d 616e 6469 6e67  memory demanding
+0000dd10: 2e20 4465 6661 756c 7420 6973 204e 6f6e  . Default is Non
+0000dd20: 652c 2077 6869 6368 2067 6976 6520 7468  e, which give th
+0000dd30: 6520 6e75 6d62 6572 206f 6620 3130 2e0a  e number of 10..
+0000dd40: 2020 2020 2020 2020 6672 6571 7565 6e63          frequenc
+0000dd50: 795f 706f 696e 7473 5f61 745f 6261 6e64  y_points_at_band
+0000dd60: 7320 3a20 626f 6f6c 2c20 6f70 7469 6f6e  s : bool, option
+0000dd70: 616c 0a20 2020 2020 2020 2020 2020 2050  al.            P
+0000dd80: 686f 6e6f 6e20 6261 6e64 2066 7265 7175  honon band frequ
+0000dd90: 656e 6369 6573 2061 7265 2075 7365 6420  encies are used 
+0000dda0: 6173 2066 7265 7175 656e 6379 2070 6f69  as frequency poi
+0000ddb0: 6e74 7320 7768 656e 2054 7275 652e 0a20  nts when True.. 
+0000ddc0: 2020 2020 2020 2020 2020 2044 6566 6175             Defau
+0000ddd0: 6c74 2069 7320 4661 6c73 652e 0a20 2020  lt is False..   
+0000dde0: 2020 2020 2073 6361 7474 6572 696e 675f       scattering_
+0000ddf0: 6576 656e 745f 636c 6173 7320 3a20 696e  event_class : in
+0000de00: 742c 206f 7074 696f 6e61 6c0a 2020 2020  t, optional.    
+0000de10: 2020 2020 2020 2020 5370 6563 6966 6963          Specific
+0000de20: 2063 686f 6963 6520 6f66 2073 6361 7474   choice of scatt
+0000de30: 6572 696e 6720 6576 656e 7420 636c 6173  ering event clas
+0000de40: 732c 2031 206f 7220 3220 7468 6174 2069  s, 1 or 2 that i
+0000de50: 7320 7370 6563 6966 6965 640a 2020 2020  s specified.    
+0000de60: 2020 2020 2020 2020 3120 6f72 2032 2c20          1 or 2, 
+0000de70: 7265 7370 6563 7469 7665 6c79 2e20 5468  respectively. Th
+0000de80: 6520 7265 7375 6c74 2069 7320 7374 6f72  e result is stor
+0000de90: 6564 2069 6e20 6761 6d6d 6173 2e20 5468  ed in gammas. Th
+0000dea0: 6572 6566 6f72 650a 2020 2020 2020 2020  erefore.        
+0000deb0: 2020 2020 7573 7561 6c20 6761 6d6d 6173      usual gammas
+0000dec0: 2061 7265 206e 6f74 2073 746f 7265 6420   are not stored 
+0000ded0: 696e 2074 6865 2076 6172 6961 626c 652e  in the variable.
+0000dee0: 2044 6566 6175 6c74 2069 7320 4e6f 6e65   Default is None
+0000def0: 2c20 7768 6963 680a 2020 2020 2020 2020  , which.        
+0000df00: 2020 2020 646f 6573 6e27 7420 7370 6563      doesn't spec
+0000df10: 6966 7920 7363 6174 7465 7269 6e67 5f65  ify scattering_e
+0000df20: 7665 6e74 5f63 6c61 7373 2e0a 2020 2020  vent_class..    
+0000df30: 2020 2020 7772 6974 655f 7478 7420 3a20      write_txt : 
+0000df40: 626f 6f6c 2c20 6f70 7469 6f6e 616c 0a20  bool, optional. 
+0000df50: 2020 2020 2020 2020 2020 2046 7265 7175             Frequ
+0000df60: 656e 6379 2070 6f69 6e74 7320 616e 6420  ency points and 
+0000df70: 696d 6167 696e 6172 7920 7061 7274 206f  imaginary part o
+0000df80: 6620 7365 6c66 2d65 6e65 7267 6965 7320  f self-energies 
+0000df90: 6172 6520 7772 6974 7465 6e0a 2020 2020  are written.    
+0000dfa0: 2020 2020 2020 2020 696e 746f 2074 6578          into tex
+0000dfb0: 7420 6669 6c65 732e 0a20 2020 2020 2020  t files..       
+0000dfc0: 2077 7269 7465 5f67 616d 6d61 5f64 6574   write_gamma_det
+0000dfd0: 6169 6c20 3a20 626f 6f6c 2c20 6f70 7469  ail : bool, opti
+0000dfe0: 6f6e 616c 0a20 2020 2020 2020 2020 2020  onal.           
+0000dff0: 2044 6574 6169 6c65 6420 6761 6d6d 6173   Detailed gammas
+0000e000: 2061 7265 2077 7269 7474 656e 2069 6e74   are written int
+0000e010: 6f20 6120 6669 6c65 2069 6e20 6864 6635  o a file in hdf5
+0000e020: 2e20 4465 6661 756c 7420 6973 2046 616c  . Default is Fal
+0000e030: 7365 2e0a 2020 2020 2020 2020 6b65 6570  se..        keep
+0000e040: 5f67 616d 6d61 5f64 6574 6169 6c20 3a20  _gamma_detail : 
+0000e050: 626f 6f6c 2c20 6f70 7469 6f6e 616c 0a20  bool, optional. 
+0000e060: 2020 2020 2020 2020 2020 2057 6974 6820             With 
+0000e070: 5472 7565 2c20 6465 7461 696c 6564 2067  True, detailed g
+0000e080: 616d 6d61 7320 6172 6520 7374 6f72 6564  ammas are stored
+0000e090: 2e20 4465 6661 756c 7420 6973 2046 616c  . Default is Fal
+0000e0a0: 7365 2e0a 2020 2020 2020 2020 6f75 7470  se..        outp
+0000e0b0: 7574 5f66 696c 656e 616d 6520 3a20 7374  ut_filename : st
+0000e0c0: 720a 2020 2020 2020 2020 2020 2020 5468  r.            Th
+0000e0d0: 6973 2073 7472 696e 6720 6973 2069 6e73  is string is ins
+0000e0e0: 6572 7465 6420 696e 2074 6865 206f 7574  erted in the out
+0000e0f0: 7075 7420 6669 6c65 206e 616d 6573 2e0a  put file names..
+0000e100: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
+0000e110: 2020 2020 2069 6620 7365 6c66 2e5f 696e       if self._in
+0000e120: 7465 7261 6374 696f 6e20 6973 204e 6f6e  teraction is Non
+0000e130: 653a 0a20 2020 2020 2020 2020 2020 206d  e:.            m
+0000e140: 7367 203d 2028 0a20 2020 2020 2020 2020  sg = (.         
+0000e150: 2020 2020 2020 2022 5068 6f6e 6f33 7079         "Phono3py
+0000e160: 2e69 6e69 745f 7068 7068 5f69 6e74 6572  .init_phph_inter
+0000e170: 6163 7469 6f6e 2068 6173 2074 6f20 6265  action has to be
+0000e180: 2063 616c 6c65 6420 220a 2020 2020 2020   called ".      
+0000e190: 2020 2020 2020 2020 2020 2262 6566 6f72            "befor
+0000e1a0: 6520 7275 6e6e 696e 6720 7468 6973 206d  e running this m
+0000e1b0: 6574 686f 642e 220a 2020 2020 2020 2020  ethod.".        
+0000e1c0: 2020 2020 290a 2020 2020 2020 2020 2020      ).          
+0000e1d0: 2020 7261 6973 6520 5275 6e74 696d 6545    raise RuntimeE
+0000e1e0: 7272 6f72 286d 7367 290a 0a20 2020 2020  rror(msg)..     
+0000e1f0: 2020 2069 6620 7465 6d70 6572 6174 7572     if temperatur
+0000e200: 6573 2069 7320 4e6f 6e65 3a0a 2020 2020  es is None:.    
+0000e210: 2020 2020 2020 2020 7365 6c66 2e5f 7465          self._te
+0000e220: 6d70 6572 6174 7572 6573 203d 205b 0a20  mperatures = [. 
+0000e230: 2020 2020 2020 2020 2020 2020 2020 2033                 3
+0000e240: 3030 2e30 2c0a 2020 2020 2020 2020 2020  00.0,.          
+0000e250: 2020 5d0a 2020 2020 2020 2020 656c 7365    ].        else
+0000e260: 3a0a 2020 2020 2020 2020 2020 2020 7365  :.            se
+0000e270: 6c66 2e5f 7465 6d70 6572 6174 7572 6573  lf._temperatures
+0000e280: 203d 2074 656d 7065 7261 7475 7265 730a   = temperatures.
+0000e290: 2020 2020 2020 2020 7365 6c66 2e5f 6772          self._gr
+0000e2a0: 6964 5f70 6f69 6e74 7320 3d20 6772 6964  id_points = grid
+0000e2b0: 5f70 6f69 6e74 730a 2020 2020 2020 2020  _points.        
+0000e2c0: 7365 6c66 2e5f 7363 6174 7465 7269 6e67  self._scattering
+0000e2d0: 5f65 7665 6e74 5f63 6c61 7373 203d 2073  _event_class = s
+0000e2e0: 6361 7474 6572 696e 675f 6576 656e 745f  cattering_event_
+0000e2f0: 636c 6173 730a 2020 2020 2020 2020 7661  class.        va
+0000e300: 6c73 203d 2067 6574 5f69 6d61 675f 7365  ls = get_imag_se
+0000e310: 6c66 5f65 6e65 7267 7928 0a20 2020 2020  lf_energy(.     
+0000e320: 2020 2020 2020 2073 656c 662e 5f69 6e74         self._int
+0000e330: 6572 6163 7469 6f6e 2c0a 2020 2020 2020  eraction,.      
+0000e340: 2020 2020 2020 6772 6964 5f70 6f69 6e74        grid_point
+0000e350: 732c 0a20 2020 2020 2020 2020 2020 2074  s,.            t
+0000e360: 656d 7065 7261 7475 7265 732c 0a20 2020  emperatures,.   
+0000e370: 2020 2020 2020 2020 2073 6967 6d61 733d           sigmas=
+0000e380: 7365 6c66 2e5f 7369 676d 6173 2c0a 2020  self._sigmas,.  
+0000e390: 2020 2020 2020 2020 2020 6672 6571 7565            freque
+0000e3a0: 6e63 795f 706f 696e 7473 3d66 7265 7175  ncy_points=frequ
+0000e3b0: 656e 6379 5f70 6f69 6e74 732c 0a20 2020  ency_points,.   
+0000e3c0: 2020 2020 2020 2020 2066 7265 7175 656e           frequen
+0000e3d0: 6379 5f73 7465 703d 6672 6571 7565 6e63  cy_step=frequenc
+0000e3e0: 795f 7374 6570 2c0a 2020 2020 2020 2020  y_step,.        
+0000e3f0: 2020 2020 6672 6571 7565 6e63 795f 706f      frequency_po
+0000e400: 696e 7473 5f61 745f 6261 6e64 733d 6672  ints_at_bands=fr
+0000e410: 6571 7565 6e63 795f 706f 696e 7473 5f61  equency_points_a
+0000e420: 745f 6261 6e64 732c 0a20 2020 2020 2020  t_bands,.       
+0000e430: 2020 2020 206e 756d 5f66 7265 7175 656e       num_frequen
+0000e440: 6379 5f70 6f69 6e74 733d 6e75 6d5f 6672  cy_points=num_fr
+0000e450: 6571 7565 6e63 795f 706f 696e 7473 2c0a  equency_points,.
+0000e460: 2020 2020 2020 2020 2020 2020 6e75 6d5f              num_
+0000e470: 706f 696e 7473 5f69 6e5f 6261 7463 683d  points_in_batch=
+0000e480: 6e75 6d5f 706f 696e 7473 5f69 6e5f 6261  num_points_in_ba
+0000e490: 7463 682c 0a20 2020 2020 2020 2020 2020  tch,.           
+0000e4a0: 2073 6361 7474 6572 696e 675f 6576 656e   scattering_even
+0000e4b0: 745f 636c 6173 733d 7363 6174 7465 7269  t_class=scatteri
+0000e4c0: 6e67 5f65 7665 6e74 5f63 6c61 7373 2c0a  ng_event_class,.
+0000e4d0: 2020 2020 2020 2020 2020 2020 7772 6974              writ
+0000e4e0: 655f 6761 6d6d 615f 6465 7461 696c 3d77  e_gamma_detail=w
+0000e4f0: 7269 7465 5f67 616d 6d61 5f64 6574 6169  rite_gamma_detai
+0000e500: 6c2c 0a20 2020 2020 2020 2020 2020 2072  l,.            r
+0000e510: 6574 7572 6e5f 6761 6d6d 615f 6465 7461  eturn_gamma_deta
+0000e520: 696c 3d6b 6565 705f 6761 6d6d 615f 6465  il=keep_gamma_de
+0000e530: 7461 696c 2c0a 2020 2020 2020 2020 2020  tail,.          
+0000e540: 2020 6f75 7470 7574 5f66 696c 656e 616d    output_filenam
+0000e550: 653d 6f75 7470 7574 5f66 696c 656e 616d  e=output_filenam
+0000e560: 652c 0a20 2020 2020 2020 2020 2020 206c  e,.            l
+0000e570: 6f67 5f6c 6576 656c 3d73 656c 662e 5f6c  og_level=self._l
+0000e580: 6f67 5f6c 6576 656c 2c0a 2020 2020 2020  og_level,.      
+0000e590: 2020 290a 2020 2020 2020 2020 6966 206b    ).        if k
+0000e5a0: 6565 705f 6761 6d6d 615f 6465 7461 696c  eep_gamma_detail
+0000e5b0: 3a0a 2020 2020 2020 2020 2020 2020 2873  :.            (s
+0000e5c0: 656c 662e 5f66 7265 7175 656e 6379 5f70  elf._frequency_p
+0000e5d0: 6f69 6e74 732c 2073 656c 662e 5f67 616d  oints, self._gam
+0000e5e0: 6d61 732c 2073 656c 662e 5f64 6574 6169  mas, self._detai
+0000e5f0: 6c65 645f 6761 6d6d 6173 2920 3d20 7661  led_gammas) = va
+0000e600: 6c73 0a20 2020 2020 2020 2065 6c73 653a  ls.        else:
+0000e610: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
+0000e620: 662e 5f66 7265 7175 656e 6379 5f70 6f69  f._frequency_poi
+0000e630: 6e74 732c 2073 656c 662e 5f67 616d 6d61  nts, self._gamma
+0000e640: 7320 3d20 7661 6c73 0a0a 2020 2020 2020  s = vals..      
+0000e650: 2020 6966 2077 7269 7465 5f74 7874 3a0a    if write_txt:.
+0000e660: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+0000e670: 2e5f 7772 6974 655f 696d 6167 5f73 656c  ._write_imag_sel
+0000e680: 665f 656e 6572 6779 286f 7574 7075 745f  f_energy(output_
+0000e690: 6669 6c65 6e61 6d65 3d6f 7574 7075 745f  filename=output_
+0000e6a0: 6669 6c65 6e61 6d65 290a 0a20 2020 2020  filename)..     
+0000e6b0: 2020 2072 6574 7572 6e20 7661 6c73 0a0a     return vals..
+0000e6c0: 2020 2020 6465 6620 5f77 7269 7465 5f69      def _write_i
+0000e6d0: 6d61 675f 7365 6c66 5f65 6e65 7267 7928  mag_self_energy(
+0000e6e0: 7365 6c66 2c20 6f75 7470 7574 5f66 696c  self, output_fil
+0000e6f0: 656e 616d 653d 4e6f 6e65 293a 0a20 2020  ename=None):.   
+0000e700: 2020 2020 2077 7269 7465 5f69 6d61 675f       write_imag_
+0000e710: 7365 6c66 5f65 6e65 7267 7928 0a20 2020  self_energy(.   
+0000e720: 2020 2020 2020 2020 2073 656c 662e 5f67           self._g
+0000e730: 616d 6d61 732c 0a20 2020 2020 2020 2020  ammas,.         
+0000e740: 2020 2073 656c 662e 6d65 7368 5f6e 756d     self.mesh_num
+0000e750: 6265 7273 2c0a 2020 2020 2020 2020 2020  bers,.          
+0000e760: 2020 7365 6c66 2e5f 6772 6964 5f70 6f69    self._grid_poi
+0000e770: 6e74 732c 0a20 2020 2020 2020 2020 2020  nts,.           
+0000e780: 2073 656c 662e 5f62 616e 645f 696e 6469   self._band_indi
+0000e790: 6365 732c 0a20 2020 2020 2020 2020 2020  ces,.           
+0000e7a0: 2073 656c 662e 5f66 7265 7175 656e 6379   self._frequency
+0000e7b0: 5f70 6f69 6e74 732c 0a20 2020 2020 2020  _points,.       
+0000e7c0: 2020 2020 2073 656c 662e 5f74 656d 7065       self._tempe
+0000e7d0: 7261 7475 7265 732c 0a20 2020 2020 2020  ratures,.       
+0000e7e0: 2020 2020 2073 656c 662e 5f73 6967 6d61       self._sigma
+0000e7f0: 732c 0a20 2020 2020 2020 2020 2020 2073  s,.            s
+0000e800: 6361 7474 6572 696e 675f 6576 656e 745f  cattering_event_
+0000e810: 636c 6173 733d 7365 6c66 2e5f 7363 6174  class=self._scat
+0000e820: 7465 7269 6e67 5f65 7665 6e74 5f63 6c61  tering_event_cla
+0000e830: 7373 2c0a 2020 2020 2020 2020 2020 2020  ss,.            
+0000e840: 6f75 7470 7574 5f66 696c 656e 616d 653d  output_filename=
+0000e850: 6f75 7470 7574 5f66 696c 656e 616d 652c  output_filename,
+0000e860: 0a20 2020 2020 2020 2020 2020 2069 735f  .            is_
+0000e870: 6d65 7368 5f73 796d 6d65 7472 793d 7365  mesh_symmetry=se
+0000e880: 6c66 2e5f 6973 5f6d 6573 685f 7379 6d6d  lf._is_mesh_symm
+0000e890: 6574 7279 2c0a 2020 2020 2020 2020 2020  etry,.          
+0000e8a0: 2020 6c6f 675f 6c65 7665 6c3d 7365 6c66    log_level=self
+0000e8b0: 2e5f 6c6f 675f 6c65 7665 6c2c 0a20 2020  ._log_level,.   
+0000e8c0: 2020 2020 2029 0a0a 2020 2020 6465 6620       )..    def 
+0000e8d0: 7275 6e5f 7265 616c 5f73 656c 665f 656e  run_real_self_en
+0000e8e0: 6572 6779 280a 2020 2020 2020 2020 7365  ergy(.        se
+0000e8f0: 6c66 2c0a 2020 2020 2020 2020 6772 6964  lf,.        grid
+0000e900: 5f70 6f69 6e74 732c 0a20 2020 2020 2020  _points,.       
+0000e910: 2074 656d 7065 7261 7475 7265 732c 0a20   temperatures,. 
+0000e920: 2020 2020 2020 2066 7265 7175 656e 6379         frequency
+0000e930: 5f70 6f69 6e74 735f 6174 5f62 616e 6473  _points_at_bands
+0000e940: 3d46 616c 7365 2c0a 2020 2020 2020 2020  =False,.        
+0000e950: 6672 6571 7565 6e63 795f 706f 696e 7473  frequency_points
+0000e960: 3d4e 6f6e 652c 0a20 2020 2020 2020 2066  =None,.        f
+0000e970: 7265 7175 656e 6379 5f73 7465 703d 4e6f  requency_step=No
+0000e980: 6e65 2c0a 2020 2020 2020 2020 6e75 6d5f  ne,.        num_
+0000e990: 6672 6571 7565 6e63 795f 706f 696e 7473  frequency_points
+0000e9a0: 3d4e 6f6e 652c 0a20 2020 2020 2020 2065  =None,.        e
+0000e9b0: 7073 696c 6f6e 733d 4e6f 6e65 2c0a 2020  psilons=None,.  
+0000e9c0: 2020 2020 2020 7772 6974 655f 7478 743d        write_txt=
+0000e9d0: 4661 6c73 652c 0a20 2020 2020 2020 2077  False,.        w
+0000e9e0: 7269 7465 5f68 6466 353d 4661 6c73 652c  rite_hdf5=False,
+0000e9f0: 0a20 2020 2020 2020 206f 7574 7075 745f  .        output_
+0000ea00: 6669 6c65 6e61 6d65 3d4e 6f6e 652c 0a20  filename=None,. 
+0000ea10: 2020 2029 3a0a 2020 2020 2020 2020 2222     ):.        ""
+0000ea20: 2243 616c 6375 6c61 7465 2072 6561 6c2d  "Calculate real-
+0000ea30: 7061 7274 206f 6620 7365 6c66 2d65 6e65  part of self-ene
+0000ea40: 7267 7920 6f66 2062 7562 626c 6520 6469  rgy of bubble di
+0000ea50: 6167 7261 6d20 2844 656c 7461 292e 0a0a  agram (Delta)...
+0000ea60: 2020 2020 2020 2020 5069 203d 2044 656c          Pi = Del
+0000ea70: 7461 202d 2069 2047 616d 6d61 2e0a 0a20  ta - i Gamma... 
+0000ea80: 2020 2020 2020 2050 6172 616d 6574 6572         Parameter
+0000ea90: 730a 2020 2020 2020 2020 2d2d 2d2d 2d2d  s.        ------
+0000eaa0: 2d2d 2d2d 0a20 2020 2020 2020 2067 7269  ----.        gri
+0000eab0: 645f 706f 696e 7473 203a 2061 7272 6179  d_points : array
+0000eac0: 5f6c 696b 650a 2020 2020 2020 2020 2020  _like.          
+0000ead0: 2020 4772 6964 2d70 6f69 6e74 2069 6e64    Grid-point ind
+0000eae0: 6963 6573 2077 6865 7265 2072 6561 6c20  ices where real 
+0000eaf0: 7061 7274 206f 6620 7365 6c66 2d65 6e65  part of self-ene
+0000eb00: 7267 6965 7320 6172 650a 2020 2020 2020  rgies are.      
+0000eb10: 2020 2020 2020 6361 636c 6375 6c61 7465        caclculate
+0000eb20: 642e 0a20 2020 2020 2020 2020 2020 2064  d..            d
+0000eb30: 7479 7065 3d69 6e74 2c20 7368 6170 653d  type=int, shape=
+0000eb40: 2867 7269 645f 706f 696e 7473 2c29 0a20  (grid_points,). 
+0000eb50: 2020 2020 2020 2074 656d 7065 7261 7475         temperatu
+0000eb60: 7265 7320 3a20 6172 7261 795f 6c69 6b65  res : array_like
+0000eb70: 0a20 2020 2020 2020 2020 2020 2054 656d  .            Tem
+0000eb80: 7065 7261 7475 7265 7320 7768 6572 6520  peratures where 
+0000eb90: 7265 616c 2070 6172 7420 6f66 2073 656c  real part of sel
+0000eba0: 662d 656e 6572 6769 6573 2020 6172 6520  f-energies  are 
+0000ebb0: 6361 6c63 756c 6174 6564 2e0a 2020 2020  calculated..    
+0000ebc0: 2020 2020 2020 2020 6474 7970 653d 666c          dtype=fl
+0000ebd0: 6f61 742c 2073 6861 7065 3d28 7465 6d70  oat, shape=(temp
+0000ebe0: 6572 6174 7572 6573 2c29 0a20 2020 2020  eratures,).     
+0000ebf0: 2020 2066 7265 7175 656e 6379 5f70 6f69     frequency_poi
+0000ec00: 6e74 735f 6174 5f62 616e 6473 203a 2062  nts_at_bands : b
+0000ec10: 6f6f 6c2c 206f 7074 696f 6e61 6c0a 2020  ool, optional.  
+0000ec20: 2020 2020 2020 2020 2020 5769 7468 2046            With F
+0000ec30: 616c 7365 2c20 6672 6571 7565 6e63 7920  alse, frequency 
+0000ec40: 7368 6966 7473 2061 7265 2063 616c 6375  shifts are calcu
+0000ec50: 6c61 7465 6420 6174 2066 7271 7565 6e63  lated at frquenc
+0000ec60: 7920 7361 6d70 6c69 6e67 0a20 2020 2020  y sampling.     
+0000ec70: 2020 2020 2020 2070 6f69 6e74 732e 2057         points. W
+0000ec80: 6865 6e20 5472 7565 2c20 7468 6579 2061  hen True, they a
+0000ec90: 7265 2064 6f6e 6520 6174 2074 6865 2070  re done at the p
+0000eca0: 686f 6e6f 6e20 6672 6571 7565 6e63 6965  honon frequencie
+0000ecb0: 732e 0a20 2020 2020 2020 2020 2020 2044  s..            D
+0000ecc0: 6566 6175 6c74 2069 7320 4661 6c73 652e  efault is False.
+0000ecd0: 0a20 2020 2020 2020 2066 7265 7175 656e  .        frequen
+0000ece0: 6379 5f70 6f69 6e74 7320 3a20 6172 7261  cy_points : arra
+0000ecf0: 795f 6c69 6b65 2c20 6f70 7469 6f6e 616c  y_like, optional
+0000ed00: 0a20 2020 2020 2020 2020 2020 2046 7265  .            Fre
+0000ed10: 7175 656e 6379 2073 616d 706c 696e 6720  quency sampling 
+0000ed20: 706f 696e 7473 2e20 4465 6661 756c 7420  points. Default 
+0000ed30: 6973 204e 6f6e 652e 2049 6e20 7468 6973  is None. In this
+0000ed40: 2063 6173 652c 0a20 2020 2020 2020 2020   case,.         
+0000ed50: 2020 206e 756d 5f66 7265 7175 656e 6379     num_frequency
+0000ed60: 5f70 6f69 6e74 7320 6f72 2066 7265 7175  _points or frequ
+0000ed70: 656e 6379 5f73 7465 7020 6973 2075 7365  ency_step is use
+0000ed80: 6420 746f 2067 656e 6572 6174 6520 756e  d to generate un
+0000ed90: 6966 6f72 6d0a 2020 2020 2020 2020 2020  iform.          
+0000eda0: 2020 6672 6571 7565 6e63 7920 7361 6d70    frequency samp
+0000edb0: 6c69 6e67 2070 6f69 6e74 732e 0a20 2020  ling points..   
+0000edc0: 2020 2020 2020 2020 2064 7479 7065 3d66           dtype=f
+0000edd0: 6c6f 6174 2c20 7368 6170 653d 2866 7265  loat, shape=(fre
+0000ede0: 7175 656e 6379 5f70 6f69 6e74 732c 290a  quency_points,).
+0000edf0: 2020 2020 2020 2020 6672 6571 7565 6e63          frequenc
+0000ee00: 795f 7374 6570 203a 2066 6c6f 6174 2c20  y_step : float, 
+0000ee10: 6f70 7469 6f6e 616c 0a20 2020 2020 2020  optional.       
+0000ee20: 2020 2020 2055 6e69 666f 726d 2070 6974       Uniform pit
+0000ee30: 6368 206f 6620 6672 6571 7565 6e63 7920  ch of frequency 
+0000ee40: 7361 6d70 6c69 6e67 2070 6f69 6e74 732e  sampling points.
+0000ee50: 2044 6566 6175 6c74 2069 7320 4e6f 6e65   Default is None
+0000ee60: 2e20 5468 6973 0a20 2020 2020 2020 2020  . This.         
+0000ee70: 2020 2072 6573 756c 7473 2069 6e20 7573     results in us
+0000ee80: 696e 6720 6e75 6d5f 6672 6571 7565 6e63  ing num_frequenc
+0000ee90: 795f 706f 696e 7473 2e0a 2020 2020 2020  y_points..      
+0000eea0: 2020 6e75 6d5f 6672 6571 7565 6e63 795f    num_frequency_
+0000eeb0: 706f 696e 7473 3a20 496e 742c 206f 7074  points: Int, opt
+0000eec0: 696f 6e61 6c0a 2020 2020 2020 2020 2020  ional.          
+0000eed0: 2020 4e75 6d62 6572 206f 6620 7361 6d70    Number of samp
+0000eee0: 6c69 6e67 2073 616d 706c 696e 6720 706f  ling sampling po
+0000eef0: 696e 7473 2074 6f20 6265 2075 7365 6420  ints to be used 
+0000ef00: 696e 7374 6561 6420 6f66 0a20 2020 2020  instead of.     
+0000ef10: 2020 2020 2020 2066 7265 7175 656e 6379         frequency
+0000ef20: 5f73 7465 702e 2054 6869 7320 6e75 6d62  _step. This numb
+0000ef30: 6572 2069 6e63 6c75 6465 7320 656e 6420  er includes end 
+0000ef40: 706f 696e 7473 2e20 4465 6661 756c 7420  points. Default 
+0000ef50: 6973 204e 6f6e 652c 0a20 2020 2020 2020  is None,.       
+0000ef60: 2020 2020 2077 6869 6368 2067 6976 6573       which gives
+0000ef70: 2032 3031 2e0a 2020 2020 2020 2020 6570   201..        ep
+0000ef80: 7369 6c6f 6e73 203a 2061 7272 6179 5f6c  silons : array_l
+0000ef90: 696b 650a 2020 2020 2020 2020 2020 2020  ike.            
+0000efa0: 536d 6561 7269 6e67 2077 6964 7468 7320  Smearing widths 
+0000efb0: 746f 2063 6f6d 7075 7465 7220 7072 696e  to computer prin
+0000efc0: 6369 7061 6c20 7061 7274 2e20 5768 656e  cipal part. When
+0000efd0: 206d 756c 7469 706c 6520 7661 6c75 6573   multiple values
+0000efe0: 0a20 2020 2020 2020 2020 2020 2061 7265  .            are
+0000eff0: 2067 6976 656e 2066 7265 7175 656e 6379   given frequency
+0000f000: 2073 6869 6674 7320 666f 7220 7468 6f73   shifts for thos
+0000f010: 6520 7661 6c75 6573 2061 7265 2072 6574  e values are ret
+0000f020: 7572 6e65 642e 0a20 2020 2020 2020 2020  urned..         
+0000f030: 2020 2064 7479 7065 3d66 6c6f 6174 2c20     dtype=float, 
+0000f040: 7368 6170 653d 2865 7073 696c 6f6e 732c  shape=(epsilons,
+0000f050: 290a 2020 2020 2020 2020 7772 6974 655f  ).        write_
+0000f060: 7478 7420 3a20 626f 6f6c 2c20 6f70 7469  txt : bool, opti
+0000f070: 6f6e 616c 0a20 2020 2020 2020 2020 2020  onal.           
+0000f080: 2046 7265 7175 656e 6379 2070 6f69 6e74   Frequency point
+0000f090: 7320 616e 6420 7265 616c 2070 6172 7420  s and real part 
+0000f0a0: 6f66 2073 656c 662d 656e 6572 6769 6573  of self-energies
+0000f0b0: 2061 7265 2077 7269 7474 656e 0a20 2020   are written.   
+0000f0c0: 2020 2020 2020 2020 2069 6e74 6f20 7465           into te
+0000f0d0: 7874 2066 696c 6573 2e0a 2020 2020 2020  xt files..      
+0000f0e0: 2020 7772 6974 655f 6864 6635 203a 2062    write_hdf5 : b
+0000f0f0: 6f6f 6c0a 2020 2020 2020 2020 2020 2020  ool.            
+0000f100: 5265 7375 6c74 7320 6172 6520 7374 6f72  Results are stor
+0000f110: 6564 2069 6e20 6864 6635 2066 696c 6573  ed in hdf5 files
+0000f120: 2069 6e64 6570 656e 6465 6e74 6c79 2061   independently a
+0000f130: 7420 6772 6964 2070 6f69 6e74 732c 0a20  t grid points,. 
+0000f140: 2020 2020 2020 2020 2020 2065 7073 696c             epsil
+0000f150: 6f6e 732c 2061 6e64 2074 656d 7065 7261  ons, and tempera
+0000f160: 7475 7265 732e 0a20 2020 2020 2020 206f  tures..        o
+0000f170: 7574 7075 745f 6669 6c65 6e61 6d65 203a  utput_filename :
+0000f180: 2073 7472 0a20 2020 2020 2020 2020 2020   str.           
+0000f190: 2054 6869 7320 7374 7269 6e67 2069 7320   This string is 
+0000f1a0: 696e 7365 7274 6564 2069 6e20 7468 6520  inserted in the 
+0000f1b0: 6f75 7470 7574 2066 696c 6520 6e61 6d65  output file name
+0000f1c0: 732e 0a0a 2020 2020 2020 2020 2222 220a  s...        """.
+0000f1d0: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
+0000f1e0: 5f69 6e74 6572 6163 7469 6f6e 2069 7320  _interaction is 
+0000f1f0: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
+0000f200: 2020 6d73 6720 3d20 280a 2020 2020 2020    msg = (.      
+0000f210: 2020 2020 2020 2020 2020 2250 686f 6e6f            "Phono
+0000f220: 3370 792e 696e 6974 5f70 6870 685f 696e  3py.init_phph_in
+0000f230: 7465 7261 6374 696f 6e20 6861 7320 746f  teraction has to
+0000f240: 2062 6520 6361 6c6c 6564 2022 0a20 2020   be called ".   
+0000f250: 2020 2020 2020 2020 2020 2020 2022 6265               "be
+0000f260: 666f 7265 2072 756e 6e69 6e67 2074 6869  fore running thi
+0000f270: 7320 6d65 7468 6f64 2e22 0a20 2020 2020  s method.".     
+0000f280: 2020 2020 2020 2029 0a20 2020 2020 2020         ).       
+0000f290: 2020 2020 2072 6169 7365 2052 756e 7469       raise Runti
+0000f2a0: 6d65 4572 726f 7228 6d73 6729 0a0a 2020  meError(msg)..  
+0000f2b0: 2020 2020 2020 6966 2065 7073 696c 6f6e        if epsilon
+0000f2c0: 7320 6973 206e 6f74 204e 6f6e 653a 0a20  s is not None:. 
+0000f2d0: 2020 2020 2020 2020 2020 205f 6570 7369             _epsi
+0000f2e0: 6c6f 6e73 203d 2065 7073 696c 6f6e 730a  lons = epsilons.
+0000f2f0: 2020 2020 2020 2020 656c 7365 3a0a 2020          else:.  
+0000f300: 2020 2020 2020 2020 2020 6966 206c 656e            if len
+0000f310: 2873 656c 662e 5f73 6967 6d61 7329 203d  (self._sigmas) =
+0000f320: 3d20 3120 616e 6420 7365 6c66 2e5f 7369  = 1 and self._si
+0000f330: 676d 6173 5b30 5d20 6973 204e 6f6e 653a  gmas[0] is None:
+0000f340: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000f350: 205f 6570 7369 6c6f 6e73 203d 204e 6f6e   _epsilons = Non
+0000f360: 650a 2020 2020 2020 2020 2020 2020 656c  e.            el
+0000f370: 6966 2073 656c 662e 5f73 6967 6d61 735b  if self._sigmas[
+0000f380: 305d 2069 7320 4e6f 6e65 3a0a 2020 2020  0] is None:.    
+0000f390: 2020 2020 2020 2020 2020 2020 5f65 7073              _eps
+0000f3a0: 696c 6f6e 7320 3d20 7365 6c66 2e5f 7369  ilons = self._si
+0000f3b0: 676d 6173 5b31 3a5d 0a20 2020 2020 2020  gmas[1:].       
+0000f3c0: 2020 2020 2065 6c73 653a 0a20 2020 2020       else:.     
+0000f3d0: 2020 2020 2020 2020 2020 205f 6570 7369             _epsi
+0000f3e0: 6c6f 6e73 203d 2073 656c 662e 5f73 6967  lons = self._sig
+0000f3f0: 6d61 730a 0a20 2020 2020 2020 2023 2028  mas..        # (
+0000f400: 6570 7369 6c6f 6e2c 2067 7269 645f 706f  epsilon, grid_po
+0000f410: 696e 742c 2074 656d 7065 7261 7475 7265  int, temperature
+0000f420: 2c20 6261 6e64 290a 2020 2020 2020 2020  , band).        
+0000f430: 6672 6571 7565 6e63 795f 706f 696e 7473  frequency_points
+0000f440: 2c20 6465 6c74 6173 203d 2067 6574 5f72  , deltas = get_r
+0000f450: 6561 6c5f 7365 6c66 5f65 6e65 7267 7928  eal_self_energy(
+0000f460: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
+0000f470: 662e 5f69 6e74 6572 6163 7469 6f6e 2c0a  f._interaction,.
+0000f480: 2020 2020 2020 2020 2020 2020 6772 6964              grid
+0000f490: 5f70 6f69 6e74 732c 0a20 2020 2020 2020  _points,.       
+0000f4a0: 2020 2020 2074 656d 7065 7261 7475 7265       temperature
+0000f4b0: 732c 0a20 2020 2020 2020 2020 2020 2065  s,.            e
+0000f4c0: 7073 696c 6f6e 733d 5f65 7073 696c 6f6e  psilons=_epsilon
+0000f4d0: 732c 0a20 2020 2020 2020 2020 2020 2066  s,.            f
+0000f4e0: 7265 7175 656e 6379 5f70 6f69 6e74 733d  requency_points=
+0000f4f0: 6672 6571 7565 6e63 795f 706f 696e 7473  frequency_points
+0000f500: 2c0a 2020 2020 2020 2020 2020 2020 6672  ,.            fr
+0000f510: 6571 7565 6e63 795f 7374 6570 3d66 7265  equency_step=fre
+0000f520: 7175 656e 6379 5f73 7465 702c 0a20 2020  quency_step,.   
+0000f530: 2020 2020 2020 2020 206e 756d 5f66 7265           num_fre
+0000f540: 7175 656e 6379 5f70 6f69 6e74 733d 6e75  quency_points=nu
+0000f550: 6d5f 6672 6571 7565 6e63 795f 706f 696e  m_frequency_poin
+0000f560: 7473 2c0a 2020 2020 2020 2020 2020 2020  ts,.            
+0000f570: 6672 6571 7565 6e63 795f 706f 696e 7473  frequency_points
+0000f580: 5f61 745f 6261 6e64 733d 6672 6571 7565  _at_bands=freque
+0000f590: 6e63 795f 706f 696e 7473 5f61 745f 6261  ncy_points_at_ba
+0000f5a0: 6e64 732c 0a20 2020 2020 2020 2020 2020  nds,.           
+0000f5b0: 2077 7269 7465 5f68 6466 353d 7772 6974   write_hdf5=writ
+0000f5c0: 655f 6864 6635 2c0a 2020 2020 2020 2020  e_hdf5,.        
+0000f5d0: 2020 2020 6f75 7470 7574 5f66 696c 656e      output_filen
+0000f5e0: 616d 653d 6f75 7470 7574 5f66 696c 656e  ame=output_filen
+0000f5f0: 616d 652c 0a20 2020 2020 2020 2020 2020  ame,.           
+0000f600: 206c 6f67 5f6c 6576 656c 3d73 656c 662e   log_level=self.
+0000f610: 5f6c 6f67 5f6c 6576 656c 2c0a 2020 2020  _log_level,.    
+0000f620: 2020 2020 290a 0a20 2020 2020 2020 2069      )..        i
+0000f630: 6620 7772 6974 655f 7478 743a 0a20 2020  f write_txt:.   
+0000f640: 2020 2020 2020 2020 2077 7269 7465 5f72           write_r
+0000f650: 6561 6c5f 7365 6c66 5f65 6e65 7267 7928  eal_self_energy(
+0000f660: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000f670: 2064 656c 7461 732c 0a20 2020 2020 2020   deltas,.       
+0000f680: 2020 2020 2020 2020 2073 656c 662e 6d65           self.me
+0000f690: 7368 5f6e 756d 6265 7273 2c0a 2020 2020  sh_numbers,.    
+0000f6a0: 2020 2020 2020 2020 2020 2020 6772 6964              grid
+0000f6b0: 5f70 6f69 6e74 732c 0a20 2020 2020 2020  _points,.       
+0000f6c0: 2020 2020 2020 2020 2073 656c 662e 5f62           self._b
+0000f6d0: 616e 645f 696e 6469 6365 732c 0a20 2020  and_indices,.   
+0000f6e0: 2020 2020 2020 2020 2020 2020 2066 7265               fre
+0000f6f0: 7175 656e 6379 5f70 6f69 6e74 732c 0a20  quency_points,. 
+0000f700: 2020 2020 2020 2020 2020 2020 2020 2074                 t
+0000f710: 656d 7065 7261 7475 7265 732c 0a20 2020  emperatures,.   
+0000f720: 2020 2020 2020 2020 2020 2020 205f 6570               _ep
+0000f730: 7369 6c6f 6e73 2c0a 2020 2020 2020 2020  silons,.        
+0000f740: 2020 2020 2020 2020 6f75 7470 7574 5f66          output_f
+0000f750: 696c 656e 616d 653d 6f75 7470 7574 5f66  ilename=output_f
+0000f760: 696c 656e 616d 652c 0a20 2020 2020 2020  ilename,.       
+0000f770: 2020 2020 2020 2020 2069 735f 6d65 7368           is_mesh
+0000f780: 5f73 796d 6d65 7472 793d 7365 6c66 2e5f  _symmetry=self._
+0000f790: 6973 5f6d 6573 685f 7379 6d6d 6574 7279  is_mesh_symmetry
+0000f7a0: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+0000f7b0: 2020 6c6f 675f 6c65 7665 6c3d 7365 6c66    log_level=self
+0000f7c0: 2e5f 6c6f 675f 6c65 7665 6c2c 0a20 2020  ._log_level,.   
+0000f7d0: 2020 2020 2020 2020 2029 0a0a 2020 2020           )..    
+0000f7e0: 2020 2020 7265 7475 726e 2066 7265 7175      return frequ
+0000f7f0: 656e 6379 5f70 6f69 6e74 732c 2064 656c  ency_points, del
+0000f800: 7461 730a 0a20 2020 2064 6566 2072 756e  tas..    def run
+0000f810: 5f73 7065 6374 7261 6c5f 6675 6e63 7469  _spectral_functi
+0000f820: 6f6e 280a 2020 2020 2020 2020 7365 6c66  on(.        self
+0000f830: 2c0a 2020 2020 2020 2020 6772 6964 5f70  ,.        grid_p
+0000f840: 6f69 6e74 732c 0a20 2020 2020 2020 2074  oints,.        t
+0000f850: 656d 7065 7261 7475 7265 732c 0a20 2020  emperatures,.   
+0000f860: 2020 2020 2066 7265 7175 656e 6379 5f70       frequency_p
+0000f870: 6f69 6e74 733d 4e6f 6e65 2c0a 2020 2020  oints=None,.    
+0000f880: 2020 2020 6672 6571 7565 6e63 795f 7374      frequency_st
+0000f890: 6570 3d4e 6f6e 652c 0a20 2020 2020 2020  ep=None,.       
+0000f8a0: 206e 756d 5f66 7265 7175 656e 6379 5f70   num_frequency_p
+0000f8b0: 6f69 6e74 733d 4e6f 6e65 2c0a 2020 2020  oints=None,.    
+0000f8c0: 2020 2020 6e75 6d5f 706f 696e 7473 5f69      num_points_i
+0000f8d0: 6e5f 6261 7463 683d 4e6f 6e65 2c0a 2020  n_batch=None,.  
+0000f8e0: 2020 2020 2020 7772 6974 655f 7478 743d        write_txt=
+0000f8f0: 4661 6c73 652c 0a20 2020 2020 2020 2077  False,.        w
+0000f900: 7269 7465 5f68 6466 353d 4661 6c73 652c  rite_hdf5=False,
+0000f910: 0a20 2020 2020 2020 206f 7574 7075 745f  .        output_
+0000f920: 6669 6c65 6e61 6d65 3d4e 6f6e 652c 0a20  filename=None,. 
+0000f930: 2020 2029 3a0a 2020 2020 2020 2020 2222     ):.        ""
+0000f940: 2246 7265 7175 656e 6379 2073 6869 6674  "Frequency shift
+0000f950: 2066 726f 6d20 6c6f 7765 7374 206f 7264   from lowest ord
+0000f960: 6572 2064 6961 6772 616d 2069 7320 6361  er diagram is ca
+0000f970: 6c63 756c 6174 6564 2e0a 0a20 2020 2020  lculated...     
+0000f980: 2020 2050 6172 616d 6574 6572 730a 2020     Parameters.  
+0000f990: 2020 2020 2020 2d2d 2d2d 2d2d 2d2d 2d2d        ----------
+0000f9a0: 0a20 2020 2020 2020 2067 7269 645f 706f  .        grid_po
+0000f9b0: 696e 7473 203a 2061 7272 6179 5f6c 696b  ints : array_lik
+0000f9c0: 650a 2020 2020 2020 2020 2020 2020 4772  e.            Gr
+0000f9d0: 6964 2d70 6f69 6e74 2069 6e64 6963 6573  id-point indices
+0000f9e0: 2077 6865 7265 2069 6d61 672d 7365 6c66   where imag-self
+0000f9f0: 2d65 6e65 7267 6569 7320 6172 6520 6361  -energeis are ca
+0000fa00: 636c 6375 6c61 7465 642e 0a20 2020 2020  clculated..     
+0000fa10: 2020 2020 2020 2064 7479 7065 3d69 6e74         dtype=int
+0000fa20: 2c20 7368 6170 653d 2867 7269 645f 706f  , shape=(grid_po
+0000fa30: 696e 7473 2c29 0a20 2020 2020 2020 2074  ints,).        t
+0000fa40: 656d 7065 7261 7475 7265 7320 3a20 6172  emperatures : ar
+0000fa50: 7261 795f 6c69 6b65 0a20 2020 2020 2020  ray_like.       
+0000fa60: 2020 2020 2054 656d 7065 7261 7475 7265       Temperature
+0000fa70: 7320 7768 6572 6520 696d 6167 2d73 656c  s where imag-sel
+0000fa80: 662d 656e 6572 6769 6573 2061 7265 2063  f-energies are c
+0000fa90: 616c 6375 6c61 7465 642e 0a20 2020 2020  alculated..     
+0000faa0: 2020 2020 2020 2064 7479 7065 3d66 6c6f         dtype=flo
+0000fab0: 6174 2c20 7368 6170 653d 2874 656d 7065  at, shape=(tempe
+0000fac0: 7261 7475 7265 732c 290a 2020 2020 2020  ratures,).      
+0000fad0: 2020 6672 6571 7565 6e63 795f 706f 696e    frequency_poin
+0000fae0: 7473 203a 2061 7272 6179 5f6c 696b 652c  ts : array_like,
+0000faf0: 206f 7074 696f 6e61 6c0a 2020 2020 2020   optional.      
+0000fb00: 2020 2020 2020 4672 6571 7565 6e63 7920        Frequency 
+0000fb10: 7361 6d70 6c69 6e67 2070 6f69 6e74 732e  sampling points.
+0000fb20: 2044 6566 6175 6c74 2069 7320 4e6f 6e65   Default is None
+0000fb30: 2e20 496e 2074 6869 7320 6361 7365 2c0a  . In this case,.
+0000fb40: 2020 2020 2020 2020 2020 2020 6e75 6d5f              num_
+0000fb50: 6672 6571 7565 6e63 795f 706f 696e 7473  frequency_points
+0000fb60: 206f 7220 6672 6571 7565 6e63 795f 7374   or frequency_st
+0000fb70: 6570 2069 7320 7573 6564 2074 6f20 6765  ep is used to ge
+0000fb80: 6e65 7261 7465 2075 6e69 666f 726d 0a20  nerate uniform. 
+0000fb90: 2020 2020 2020 2020 2020 2066 7265 7175             frequ
+0000fba0: 656e 6379 2073 616d 706c 696e 6720 706f  ency sampling po
+0000fbb0: 696e 7473 2e0a 2020 2020 2020 2020 2020  ints..          
+0000fbc0: 2020 6474 7970 653d 666c 6f61 742c 2073    dtype=float, s
+0000fbd0: 6861 7065 3d28 6672 6571 7565 6e63 795f  hape=(frequency_
+0000fbe0: 706f 696e 7473 2c29 0a20 2020 2020 2020  points,).       
+0000fbf0: 2066 7265 7175 656e 6379 5f73 7465 7020   frequency_step 
+0000fc00: 3a20 666c 6f61 742c 206f 7074 696f 6e61  : float, optiona
+0000fc10: 6c0a 2020 2020 2020 2020 2020 2020 556e  l.            Un
+0000fc20: 6966 6f72 6d20 7069 7463 6820 6f66 2066  iform pitch of f
+0000fc30: 7265 7175 656e 6379 2073 616d 706c 696e  requency samplin
+0000fc40: 6720 706f 696e 7473 2e20 4465 6661 756c  g points. Defaul
+0000fc50: 7420 6973 204e 6f6e 652e 2054 6869 730a  t is None. This.
+0000fc60: 2020 2020 2020 2020 2020 2020 7265 7375              resu
+0000fc70: 6c74 7320 696e 2075 7369 6e67 206e 756d  lts in using num
+0000fc80: 5f66 7265 7175 656e 6379 5f70 6f69 6e74  _frequency_point
+0000fc90: 732e 0a20 2020 2020 2020 206e 756d 5f66  s..        num_f
+0000fca0: 7265 7175 656e 6379 5f70 6f69 6e74 733a  requency_points:
+0000fcb0: 2049 6e74 2c20 6f70 7469 6f6e 616c 0a20   Int, optional. 
+0000fcc0: 2020 2020 2020 2020 2020 204e 756d 6265             Numbe
+0000fcd0: 7220 6f66 2073 616d 706c 696e 6720 7361  r of sampling sa
+0000fce0: 6d70 6c69 6e67 2070 6f69 6e74 7320 746f  mpling points to
+0000fcf0: 2062 6520 7573 6564 2069 6e73 7465 6164   be used instead
+0000fd00: 206f 660a 2020 2020 2020 2020 2020 2020   of.            
+0000fd10: 6672 6571 7565 6e63 795f 7374 6570 2e20  frequency_step. 
+0000fd20: 5468 6973 206e 756d 6265 7220 696e 636c  This number incl
+0000fd30: 7564 6573 2065 6e64 2070 6f69 6e74 732e  udes end points.
+0000fd40: 2044 6566 6175 6c74 2069 7320 4e6f 6e65   Default is None
+0000fd50: 2c0a 2020 2020 2020 2020 2020 2020 7768  ,.            wh
+0000fd60: 6963 6820 6769 7665 7320 3230 312e 0a20  ich gives 201.. 
+0000fd70: 2020 2020 2020 206e 756d 5f70 6f69 6e74         num_point
+0000fd80: 735f 696e 5f62 6174 6368 3a20 696e 742c  s_in_batch: int,
+0000fd90: 206f 7074 696f 6e61 6c0a 2020 2020 2020   optional.      
+0000fda0: 2020 2020 2020 4e75 6d62 6572 206f 6620        Number of 
+0000fdb0: 7361 6d70 6c69 6e67 2070 6f69 6e74 7320  sampling points 
+0000fdc0: 696e 206f 6e65 2062 6174 6368 2e20 5468  in one batch. Th
+0000fdd0: 6973 2069 7320 666f 7220 7468 6520 6672  is is for the fr
+0000fde0: 6571 7565 6e63 790a 2020 2020 2020 2020  equency.        
+0000fdf0: 2020 2020 7361 6d70 6c69 6e67 206d 6f64      sampling mod
+0000fe00: 6520 616e 6420 7468 6520 7361 6d70 6c69  e and the sampli
+0000fe10: 6e67 2070 6f69 6e74 7320 6172 6520 6469  ng points are di
+0000fe20: 7669 6465 6420 696e 746f 2062 6174 6368  vided into batch
+0000fe30: 6573 2e0a 2020 2020 2020 2020 2020 2020  es..            
+0000fe40: 4c61 6765 7220 6e75 6d62 6572 2070 726f  Lager number pro
+0000fe50: 7669 6465 7320 6566 6669 6369 656e 7420  vides efficient 
+0000fe60: 7573 6520 6f66 206d 756c 7469 2d63 6f72  use of multi-cor
+0000fe70: 6573 2062 7574 206d 6f72 650a 2020 2020  es but more.    
+0000fe80: 2020 2020 2020 2020 6d65 6d6f 7279 2064          memory d
+0000fe90: 656d 616e 6469 6e67 2e20 4465 6661 756c  emanding. Defaul
+0000fea0: 7420 6973 204e 6f6e 652c 2077 6869 6368  t is None, which
+0000feb0: 2067 6976 6520 7468 6520 6e75 6d62 6572   give the number
+0000fec0: 206f 6620 3130 2e0a 2020 2020 2020 2020   of 10..        
+0000fed0: 7772 6974 655f 7478 7420 3a20 626f 6f6c  write_txt : bool
+0000fee0: 2c20 6f70 7469 6f6e 616c 0a20 2020 2020  , optional.     
+0000fef0: 2020 2020 2020 2046 7265 7175 656e 6379         Frequency
+0000ff00: 2070 6f69 6e74 7320 616e 6420 7370 6563   points and spec
+0000ff10: 7472 616c 2066 756e 6374 696f 6e73 2061  tral functions a
+0000ff20: 7265 2077 7269 7474 656e 0a20 2020 2020  re written.     
+0000ff30: 2020 2020 2020 2069 6e74 6f20 7465 7874         into text
+0000ff40: 2066 696c 6573 2e20 4465 6661 756c 7420   files. Default 
+0000ff50: 6973 2046 616c 7365 2e0a 2020 2020 2020  is False..      
+0000ff60: 2020 7772 6974 655f 6864 6635 203a 2062    write_hdf5 : b
+0000ff70: 6f6f 6c0a 2020 2020 2020 2020 2020 2020  ool.            
+0000ff80: 5265 7375 6c74 7320 6172 6520 7374 6f72  Results are stor
+0000ff90: 6564 2069 6e20 6864 6635 2066 696c 6573  ed in hdf5 files
+0000ffa0: 2069 6e64 6570 656e 6465 6e74 6c79 2061   independently a
+0000ffb0: 7420 6772 6964 2070 6f69 6e74 732c 0a20  t grid points,. 
+0000ffc0: 2020 2020 2020 2020 2020 2065 7073 696c             epsil
+0000ffd0: 6f6e 732e 2044 6566 6175 6c74 2069 7320  ons. Default is 
+0000ffe0: 4661 6c73 652e 0a20 2020 2020 2020 206f  False..        o
+0000fff0: 7574 7075 745f 6669 6c65 6e61 6d65 203a  utput_filename :
+00010000: 2073 7472 0a20 2020 2020 2020 2020 2020   str.           
+00010010: 2054 6869 7320 7374 7269 6e67 2069 7320   This string is 
+00010020: 696e 7365 7274 6564 2069 6e20 7468 6520  inserted in the 
+00010030: 6f75 7470 7574 2066 696c 6520 6e61 6d65  output file name
+00010040: 732e 0a0a 2020 2020 2020 2020 2222 220a  s...        """.
+00010050: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
+00010060: 5f69 6e74 6572 6163 7469 6f6e 2069 7320  _interaction is 
+00010070: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
+00010080: 2020 6d73 6720 3d20 280a 2020 2020 2020    msg = (.      
+00010090: 2020 2020 2020 2020 2020 2250 686f 6e6f            "Phono
+000100a0: 3370 792e 696e 6974 5f70 6870 685f 696e  3py.init_phph_in
+000100b0: 7465 7261 6374 696f 6e20 6861 7320 746f  teraction has to
+000100c0: 2062 6520 6361 6c6c 6564 2022 0a20 2020   be called ".   
+000100d0: 2020 2020 2020 2020 2020 2020 2022 6265               "be
+000100e0: 666f 7265 2072 756e 6e69 6e67 2074 6869  fore running thi
+000100f0: 7320 6d65 7468 6f64 2e22 0a20 2020 2020  s method.".     
+00010100: 2020 2020 2020 2029 0a20 2020 2020 2020         ).       
+00010110: 2020 2020 2072 6169 7365 2052 756e 7469       raise Runti
+00010120: 6d65 4572 726f 7228 6d73 6729 0a0a 2020  meError(msg)..  
+00010130: 2020 2020 2020 7365 6c66 2e5f 7370 6563        self._spec
+00010140: 7472 616c 5f66 756e 6374 696f 6e20 3d20  tral_function = 
+00010150: 7275 6e5f 7370 6563 7472 616c 5f66 756e  run_spectral_fun
+00010160: 6374 696f 6e28 0a20 2020 2020 2020 2020  ction(.         
+00010170: 2020 2073 656c 662e 5f69 6e74 6572 6163     self._interac
+00010180: 7469 6f6e 2c0a 2020 2020 2020 2020 2020  tion,.          
+00010190: 2020 6772 6964 5f70 6f69 6e74 732c 0a20    grid_points,. 
+000101a0: 2020 2020 2020 2020 2020 2074 656d 7065             tempe
+000101b0: 7261 7475 7265 733d 7465 6d70 6572 6174  ratures=temperat
+000101c0: 7572 6573 2c0a 2020 2020 2020 2020 2020  ures,.          
+000101d0: 2020 7369 676d 6173 3d73 656c 662e 5f73    sigmas=self._s
+000101e0: 6967 6d61 732c 0a20 2020 2020 2020 2020  igmas,.         
+000101f0: 2020 2066 7265 7175 656e 6379 5f70 6f69     frequency_poi
+00010200: 6e74 733d 6672 6571 7565 6e63 795f 706f  nts=frequency_po
+00010210: 696e 7473 2c0a 2020 2020 2020 2020 2020  ints,.          
+00010220: 2020 6672 6571 7565 6e63 795f 7374 6570    frequency_step
+00010230: 3d66 7265 7175 656e 6379 5f73 7465 702c  =frequency_step,
+00010240: 0a20 2020 2020 2020 2020 2020 206e 756d  .            num
+00010250: 5f66 7265 7175 656e 6379 5f70 6f69 6e74  _frequency_point
+00010260: 733d 6e75 6d5f 6672 6571 7565 6e63 795f  s=num_frequency_
+00010270: 706f 696e 7473 2c0a 2020 2020 2020 2020  points,.        
+00010280: 2020 2020 6e75 6d5f 706f 696e 7473 5f69      num_points_i
+00010290: 6e5f 6261 7463 683d 6e75 6d5f 706f 696e  n_batch=num_poin
+000102a0: 7473 5f69 6e5f 6261 7463 682c 0a20 2020  ts_in_batch,.   
+000102b0: 2020 2020 2020 2020 2062 616e 645f 696e           band_in
+000102c0: 6469 6365 733d 7365 6c66 2e5f 6261 6e64  dices=self._band
+000102d0: 5f69 6e64 6963 6573 2c0a 2020 2020 2020  _indices,.      
+000102e0: 2020 2020 2020 7772 6974 655f 7478 743d        write_txt=
+000102f0: 7772 6974 655f 7478 742c 0a20 2020 2020  write_txt,.     
+00010300: 2020 2020 2020 2077 7269 7465 5f68 6466         write_hdf
+00010310: 353d 7772 6974 655f 6864 6635 2c0a 2020  5=write_hdf5,.  
+00010320: 2020 2020 2020 2020 2020 6f75 7470 7574            output
+00010330: 5f66 696c 656e 616d 653d 6f75 7470 7574  _filename=output
+00010340: 5f66 696c 656e 616d 652c 0a20 2020 2020  _filename,.     
+00010350: 2020 2020 2020 206c 6f67 5f6c 6576 656c         log_level
+00010360: 3d73 656c 662e 5f6c 6f67 5f6c 6576 656c  =self._log_level
+00010370: 2c0a 2020 2020 2020 2020 290a 0a20 2020  ,.        )..   
+00010380: 2064 6566 2072 756e 5f74 6865 726d 616c   def run_thermal
+00010390: 5f63 6f6e 6475 6374 6976 6974 7928 0a20  _conductivity(. 
+000103a0: 2020 2020 2020 2073 656c 662c 0a20 2020         self,.   
+000103b0: 2020 2020 2069 735f 4c42 5445 3d46 616c       is_LBTE=Fal
+000103c0: 7365 2c0a 2020 2020 2020 2020 7465 6d70  se,.        temp
+000103d0: 6572 6174 7572 6573 3d4e 6f6e 652c 0a20  eratures=None,. 
+000103e0: 2020 2020 2020 2069 735f 6973 6f74 6f70         is_isotop
+000103f0: 653d 4661 6c73 652c 0a20 2020 2020 2020  e=False,.       
+00010400: 206d 6173 735f 7661 7269 616e 6365 733d   mass_variances=
+00010410: 4e6f 6e65 2c0a 2020 2020 2020 2020 6772  None,.        gr
+00010420: 6964 5f70 6f69 6e74 733d 4e6f 6e65 2c0a  id_points=None,.
+00010430: 2020 2020 2020 2020 626f 756e 6461 7279          boundary
+00010440: 5f6d 6670 3d4e 6f6e 652c 2020 2320 696e  _mfp=None,  # in
+00010450: 206d 6963 726f 6d65 7472 650a 2020 2020   micrometre.    
+00010460: 2020 2020 736f 6c76 655f 636f 6c6c 6563      solve_collec
+00010470: 7469 7665 5f70 686f 6e6f 6e3d 4661 6c73  tive_phonon=Fals
+00010480: 652c 0a20 2020 2020 2020 2075 7365 5f61  e,.        use_a
+00010490: 7665 5f70 703d 4661 6c73 652c 0a20 2020  ve_pp=False,.   
+000104a0: 2020 2020 2069 735f 7265 6475 6369 626c       is_reducibl
+000104b0: 655f 636f 6c6c 6973 696f 6e5f 6d61 7472  e_collision_matr
+000104c0: 6978 3d46 616c 7365 2c0a 2020 2020 2020  ix=False,.      
+000104d0: 2020 6973 5f6b 6170 7061 5f73 7461 723d    is_kappa_star=
+000104e0: 5472 7565 2c0a 2020 2020 2020 2020 6776  True,.        gv
+000104f0: 5f64 656c 7461 5f71 3d4e 6f6e 652c 2020  _delta_q=None,  
+00010500: 2320 666f 7220 6772 6f75 7020 7665 6c6f  # for group velo
+00010510: 6369 7479 0a20 2020 2020 2020 2069 735f  city.        is_
+00010520: 6675 6c6c 5f70 703d 4661 6c73 652c 0a20  full_pp=False,. 
+00010530: 2020 2020 2020 2070 696e 765f 6375 746f         pinv_cuto
+00010540: 6666 3d31 2e30 652d 382c 2020 2320 666f  ff=1.0e-8,  # fo
+00010550: 7220 7073 6575 646f 2d69 6e76 6572 7369  r pseudo-inversi
+00010560: 6f6e 206f 6620 636f 6c6c 6973 696f 6e20  on of collision 
+00010570: 6d61 7472 6978 0a20 2020 2020 2020 2070  matrix.        p
+00010580: 696e 765f 6d65 7468 6f64 3d30 2c20 2023  inv_method=0,  #
+00010590: 2066 6f72 2070 7365 7564 6f2d 696e 7665   for pseudo-inve
+000105a0: 7273 696f 6e20 6f66 2063 6f6c 6c69 7369  rsion of collisi
+000105b0: 6f6e 206d 6174 7269 780a 2020 2020 2020  on matrix.      
+000105c0: 2020 7069 6e76 5f73 6f6c 7665 723d 302c    pinv_solver=0,
+000105d0: 2020 2320 736f 6c76 6572 206f 6620 7073    # solver of ps
+000105e0: 6575 646f 2d69 6e76 6572 7369 6f6e 206f  eudo-inversion o
+000105f0: 6620 636f 6c6c 6973 696f 6e20 6d61 7472  f collision matr
+00010600: 6978 0a20 2020 2020 2020 2077 7269 7465  ix.        write
+00010610: 5f67 616d 6d61 3d46 616c 7365 2c0a 2020  _gamma=False,.  
+00010620: 2020 2020 2020 7265 6164 5f67 616d 6d61        read_gamma
+00010630: 3d46 616c 7365 2c0a 2020 2020 2020 2020  =False,.        
+00010640: 6973 5f4e 5f55 3d46 616c 7365 2c0a 2020  is_N_U=False,.  
+00010650: 2020 2020 2020 636f 6e64 7563 7469 7669        conductivi
+00010660: 7479 5f74 7970 653d 4e6f 6e65 2c0a 2020  ty_type=None,.  
+00010670: 2020 2020 2020 7772 6974 655f 6b61 7070        write_kapp
+00010680: 613d 4661 6c73 652c 0a20 2020 2020 2020  a=False,.       
+00010690: 2077 7269 7465 5f67 616d 6d61 5f64 6574   write_gamma_det
+000106a0: 6169 6c3d 4661 6c73 652c 0a20 2020 2020  ail=False,.     
+000106b0: 2020 2077 7269 7465 5f63 6f6c 6c69 7369     write_collisi
+000106c0: 6f6e 3d46 616c 7365 2c0a 2020 2020 2020  on=False,.      
+000106d0: 2020 7265 6164 5f63 6f6c 6c69 7369 6f6e    read_collision
+000106e0: 3d46 616c 7365 2c0a 2020 2020 2020 2020  =False,.        
+000106f0: 7772 6974 655f 7070 3d46 616c 7365 2c0a  write_pp=False,.
+00010700: 2020 2020 2020 2020 7265 6164 5f70 703d          read_pp=
+00010710: 4661 6c73 652c 0a20 2020 2020 2020 2077  False,.        w
+00010720: 7269 7465 5f4c 4254 455f 736f 6c75 7469  rite_LBTE_soluti
+00010730: 6f6e 3d46 616c 7365 2c0a 2020 2020 2020  on=False,.      
+00010740: 2020 636f 6d70 7265 7373 696f 6e3d 2267    compression="g
+00010750: 7a69 7022 2c0a 2020 2020 2020 2020 696e  zip",.        in
+00010760: 7075 745f 6669 6c65 6e61 6d65 3d4e 6f6e  put_filename=Non
+00010770: 652c 0a20 2020 2020 2020 206f 7574 7075  e,.        outpu
+00010780: 745f 6669 6c65 6e61 6d65 3d4e 6f6e 652c  t_filename=None,
+00010790: 0a20 2020 2029 3a0a 2020 2020 2020 2020  .    ):.        
+000107a0: 2222 2252 756e 2074 6865 726d 616c 2063  """Run thermal c
+000107b0: 6f6e 6475 6374 6976 6974 7920 6361 6c63  onductivity calc
+000107c0: 756c 6174 696f 6e2e 0a0a 2020 2020 2020  ulation...      
+000107d0: 2020 5061 7261 6d65 7465 7273 0a20 2020    Parameters.   
+000107e0: 2020 2020 202d 2d2d 2d2d 2d2d 2d2d 2d0a       ----------.
+000107f0: 2020 2020 2020 2020 6973 5f4c 4254 4520          is_LBTE 
+00010800: 3a20 626f 6f6c 2c20 6f70 7469 6f6e 616c  : bool, optional
+00010810: 2c20 6465 6661 756c 7420 6973 2046 616c  , default is Fal
+00010820: 7365 0a20 2020 2020 2020 2020 2020 2052  se.            R
+00010830: 5441 2028 4661 6c73 6529 206f 7220 6469  TA (False) or di
+00010840: 7265 6374 2073 6f6c 7574 696f 6e20 2854  rect solution (T
+00010850: 7275 6529 2e0a 2020 2020 2020 2020 7465  rue)..        te
+00010860: 6d70 6572 6174 7572 6573 203a 2061 7272  mperatures : arr
+00010870: 6179 5f6c 696b 652c 206f 7074 696f 6e61  ay_like, optiona
+00010880: 6c2c 2064 6566 6175 6c74 2069 7320 4e6f  l, default is No
+00010890: 6e65 0a20 2020 2020 2020 2020 2020 2054  ne.            T
+000108a0: 656d 7065 7261 7475 7265 7320 6174 2077  emperatures at w
+000108b0: 6869 6368 2074 6865 726d 616c 2063 6f6e  hich thermal con
+000108c0: 6475 6374 6976 6974 7920 6973 2063 616c  ductivity is cal
+000108d0: 6375 6c61 7465 642e 0a20 2020 2020 2020  culated..       
+000108e0: 2020 2020 2073 6861 7065 3d28 7465 6d70       shape=(temp
+000108f0: 6572 6174 7572 655f 706f 696e 7473 2c20  erature_points, 
+00010900: 292c 2064 7479 7065 3d27 646f 7562 6c65  ), dtype='double
+00010910: 272e 0a20 2020 2020 2020 2020 2020 2057  '..            W
+00010920: 6974 6820 4e6f 6e65 2c0a 2020 2020 2020  ith None,.      
+00010930: 2020 2020 2020 2020 2020 6069 735f 4c42            `is_LB
+00010940: 5445 3d46 616c 7365 6020 6769 7665 7320  TE=False` gives 
+00010950: 7465 6d70 6572 6174 7572 6573 3d5b 302c  temperatures=[0,
+00010960: 2031 302c 202e 2e2e 2c20 3130 3030 5d2e   10, ..., 1000].
+00010970: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00010980: 2060 6973 5f4c 4254 453d 5472 7565 6020   `is_LBTE=True` 
+00010990: 6769 7665 7320 7465 6d70 6572 6174 7572  gives temperatur
+000109a0: 6573 3d5b 3330 302c 205d 2e0a 2020 2020  es=[300, ]..    
+000109b0: 2020 2020 6973 5f69 736f 746f 7065 203a      is_isotope :
+000109c0: 2062 6f6f 6c2c 206f 7074 696f 6e61 6c2c   bool, optional,
+000109d0: 2064 6566 6175 6c74 2069 7320 4661 6c73   default is Fals
+000109e0: 650a 2020 2020 2020 2020 2020 2020 5769  e.            Wi
+000109f0: 7468 206f 7220 7769 7468 6f75 7420 6973  th or without is
+00010a00: 6f74 6f70 6520 7363 6174 7465 7269 6e67  otope scattering
+00010a10: 2e0a 2020 2020 2020 2020 6d61 7373 5f76  ..        mass_v
+00010a20: 6172 6961 6e63 6573 203a 2061 7272 6179  ariances : array
+00010a30: 5f6c 696b 652c 206f 7074 696f 6e61 6c2c  _like, optional,
+00010a40: 2064 6566 6175 6c74 2069 7320 4e6f 6e65   default is None
+00010a50: 0a20 2020 2020 2020 2020 2020 204d 6173  .            Mas
+00010a60: 7320 7661 7269 616e 6365 7320 666f 7220  s variances for 
+00010a70: 6973 6f74 6f70 6520 7363 6174 7465 7269  isotope scatteri
+00010a80: 6e67 2063 616c 6375 6c61 7469 6f6e 2e20  ng calculation. 
+00010a90: 5768 656e 204e 6f6e 652c 0a20 2020 2020  When None,.     
+00010aa0: 2020 2020 2020 2074 6865 2076 616c 7565         the value
+00010ab0: 7320 7374 6f72 6564 2069 6e20 7068 6f6e  s stored in phon
+00010ac0: 6f33 7079 2061 7265 2075 7365 6420 7769  o3py are used wi
+00010ad0: 7468 2060 6973 5f69 736f 746f 7065 3d54  th `is_isotope=T
+00010ae0: 7275 6560 2e0a 2020 2020 2020 2020 2020  rue`..          
+00010af0: 2020 7368 6170 6528 6174 6f6d 735f 696e    shape(atoms_in
+00010b00: 5f70 7269 6d69 7469 7665 2c20 292c 2064  _primitive, ), d
+00010b10: 7479 7065 3d27 646f 7562 6c65 272e 0a20  type='double'.. 
+00010b20: 2020 2020 2020 2067 7269 645f 706f 696e         grid_poin
+00010b30: 7473 203a 2061 7272 6179 5f6c 696b 652c  ts : array_like,
+00010b40: 206f 7074 696f 6e61 6c2c 2064 6566 6175   optional, defau
+00010b50: 6c74 2069 7320 4e6f 6e65 0a20 2020 2020  lt is None.     
+00010b60: 2020 2020 2020 204c 6973 7420 6f66 2067         List of g
+00010b70: 7269 6420 706f 696e 7420 696e 6469 6365  rid point indice
+00010b80: 7320 7768 6572 6520 6d6f 6465 2074 6865  s where mode the
+00010b90: 726d 616c 2063 6f6e 6475 6374 6976 6974  rmal conductivit
+00010ba0: 6965 7320 6172 650a 2020 2020 2020 2020  ies are.        
+00010bb0: 2020 2020 6361 6c63 756c 6174 6564 2e20      calculated. 
+00010bc0: 5769 7468 204e 6f6e 652c 2061 6c6c 2074  With None, all t
+00010bd0: 6865 2067 7269 6420 706f 696e 7473 2074  he grid points t
+00010be0: 6861 7420 6172 6520 6e65 6365 7373 6172  hat are necessar
+00010bf0: 790a 2020 2020 2020 2020 2020 2020 666f  y.            fo
+00010c00: 7220 7468 6572 6d61 6c20 636f 6e64 7563  r thermal conduc
+00010c10: 7469 7669 7479 2061 7265 2073 6574 2069  tivity are set i
+00010c20: 6e74 6572 6e61 6c6c 792e 0a20 2020 2020  nternally..     
+00010c30: 2020 2020 2020 2073 6861 7065 286e 756d         shape(num
+00010c40: 5f67 7269 645f 706f 696e 7473 2c20 292c  _grid_points, ),
+00010c50: 2064 7479 7065 3d27 696e 745f 272e 0a20   dtype='int_'.. 
+00010c60: 2020 2020 2020 2062 6f75 6e64 6172 795f         boundary_
+00010c70: 6d66 7020 3a20 666c 6f61 742c 206f 7074  mfp : float, opt
+00010c80: 696f 6e61 2c20 6465 6661 756c 7420 6973  iona, default is
+00010c90: 204e 6f6e 650a 2020 2020 2020 2020 2020   None.          
+00010ca0: 2020 4d65 616e 2066 7265 6520 7061 7468    Mean free path
+00010cb0: 2069 6e20 6d69 6372 6f6d 6574 7265 2074   in micrometre t
+00010cc0: 6f20 6361 6c63 756c 6174 6520 7369 6d70  o calculate simp
+00010cd0: 6c65 2062 6f75 6e64 6172 790a 2020 2020  le boundary.    
+00010ce0: 2020 2020 2020 2020 7363 6174 7465 7269          scatteri
+00010cf0: 6e67 2063 6f6e 7472 6962 7574 696f 6e20  ng contribution 
+00010d00: 746f 2074 6865 726d 616c 2063 6f6e 6475  to thermal condu
+00010d10: 6374 6976 6974 792e 0a20 2020 2020 2020  ctivity..       
+00010d20: 2020 2020 204e 6f6e 6520 6967 6e6f 7265       None ignore
+00010d30: 7320 7468 6973 2063 6f6e 7472 6962 7574  s this contribut
+00010d40: 696f 6e2e 0a20 2020 2020 2020 2073 6f6c  ion..        sol
+00010d50: 7665 5f63 6f6c 6c65 6374 6976 655f 7068  ve_collective_ph
+00010d60: 6f6e 6f6e 203a 2062 6f6f 6c2c 206f 7074  onon : bool, opt
+00010d70: 696f 6e61 6c2c 2064 6566 6175 6c74 2069  ional, default i
+00010d80: 7320 4661 6c73 650a 2020 2020 2020 2020  s False.        
+00010d90: 2020 2020 5468 6973 2069 7320 616e 206f      This is an o
+00010da0: 7074 696f 6e20 666f 7220 7468 6520 6665  ption for the fe
+00010db0: 6174 7572 6520 756e 6465 7220 6465 7665  ature under deve
+00010dc0: 6c6f 706d 656e 742e 0a20 2020 2020 2020  lopment..       
+00010dd0: 2075 7365 5f61 7665 5f70 7020 3a20 626f   use_ave_pp : bo
+00010de0: 6f6c 2c20 6f70 7469 6f6e 616c 2c20 6465  ol, optional, de
+00010df0: 6661 756c 7420 6973 2046 616c 7365 0a20  fault is False. 
+00010e00: 2020 2020 2020 2020 2020 2052 5441 206f             RTA o
+00010e10: 6e6c 7920 2860 6973 5f4c 4254 453d 4661  nly (`is_LBTE=Fa
+00010e20: 6c73 6560 292e 2041 7665 7261 6765 6420  lse`). Averaged 
+00010e30: 7068 6f6e 6f6e 2d70 686f 6e6f 6e20 696e  phonon-phonon in
+00010e40: 7465 7261 6374 696f 6e0a 2020 2020 2020  teraction.      
+00010e50: 2020 2020 2020 7374 7265 6e67 7468 2069        strength i
+00010e60: 7320 7573 6564 2074 6f20 6361 6c63 756c  s used to calcul
+00010e70: 6174 6520 7068 6f6e 6f6e 206c 6966 6574  ate phonon lifet
+00010e80: 696d 652e 2054 6869 7320 646f 6573 206e  ime. This does n
+00010e90: 6f74 0a20 2020 2020 2020 2020 2020 2072  ot.            r
+00010ea0: 6564 7563 6520 636f 6d70 7574 6174 696f  educe computatio
+00010eb0: 6e61 6c20 6465 6d61 6e64 2c20 6275 7420  nal demand, but 
+00010ec0: 6d61 7920 6265 2075 7365 6420 746f 206d  may be used to m
+00010ed0: 6f64 656c 2074 6865 726d 616c 0a20 2020  odel thermal.   
+00010ee0: 2020 2020 2020 2020 2063 6f6e 6475 6374           conduct
+00010ef0: 6976 6974 7920 666f 7220 616e 616c 797a  ivity for analyz
+00010f00: 6520 7468 6520 6361 6c63 756c 6174 696f  e the calculatio
+00010f10: 6e20 7265 7375 6c74 732e 0a20 2020 2020  n results..     
+00010f20: 2020 2069 735f 7265 6475 6369 626c 655f     is_reducible_
+00010f30: 636f 6c6c 6973 696f 6e5f 6d61 7472 6978  collision_matrix
+00010f40: 203a 2062 6f6f 6c2c 206f 7074 696f 6e61   : bool, optiona
+00010f50: 6c2c 2064 6566 6175 6c74 2069 7320 4661  l, default is Fa
+00010f60: 6c73 650a 2020 2020 2020 2020 2020 2020  lse.            
+00010f70: 4469 7265 6374 2073 6f6c 7574 696f 6e20  Direct solution 
+00010f80: 6f6e 6c79 2028 6069 735f 4c42 5445 3d54  only (`is_LBTE=T
+00010f90: 7275 6560 292e 2054 6869 7320 6973 2061  rue`). This is a
+00010fa0: 6e20 6578 7065 7269 6d65 6e74 616c 0a20  n experimental. 
+00010fb0: 2020 2020 2020 2020 2020 206f 7074 696f             optio
+00010fc0: 6e2e 2057 6974 6820 5472 7565 2c20 6675  n. With True, fu
+00010fd0: 6c6c 2063 6f6c 6c69 7369 6f6e 206d 6174  ll collision mat
+00010fe0: 7269 7820 6973 2063 7265 6174 6564 2061  rix is created a
+00010ff0: 6e64 2073 6f6c 7665 642e 0a20 2020 2020  nd solved..     
+00011000: 2020 2069 735f 6b61 7070 615f 7374 6172     is_kappa_star
+00011010: 203a 2062 6f6f 6c2c 206f 7074 696f 6e61   : bool, optiona
+00011020: 6c2c 2064 6566 6175 6c74 2069 7320 5472  l, default is Tr
+00011030: 7565 0a20 2020 2020 2020 2020 2020 2057  ue.            W
+00011040: 6974 6820 7472 7565 2c20 7379 6d6d 6574  ith true, symmet
+00011050: 7279 2069 7320 636f 6e73 6964 6572 6564  ry is considered
+00011060: 2077 6865 6e20 7361 6d70 6c69 6e67 2067   when sampling g
+00011070: 7269 6420 706f 696e 7473 0a20 2020 2020  rid points.     
+00011080: 2020 2020 2020 2061 7420 7768 6963 6820         at which 
+00011090: 6d6f 6465 2074 6865 726d 616c 2063 6f6e  mode thermal con
+000110a0: 6475 6374 6976 6974 6965 7320 6172 6520  ductivities are 
+000110b0: 6361 6c63 756c 6174 6564 2e0a 2020 2020  calculated..    
+000110c0: 2020 2020 6776 5f64 656c 7461 5f71 203a      gv_delta_q :
+000110d0: 2066 6c6f 6174 2c20 6f70 7469 6f6e 616c   float, optional
+000110e0: 2c20 6465 6661 756c 7420 6973 204e 6f6e  , default is Non
+000110f0: 652c 2020 2320 666f 7220 6772 6f75 7020  e,  # for group 
+00011100: 7665 6c6f 6369 7479 0a20 2020 2020 2020  velocity.       
+00011110: 2020 2020 2057 6974 6820 6e6f 6e2d 616e       With non-an
+00011120: 616c 7974 6963 616c 2063 6f72 7265 6374  alytical correct
+00011130: 696f 6e2c 2067 726f 7570 2076 656c 6f63  ion, group veloc
+00011140: 6974 7920 6973 2063 616c 6375 6c61 7465  ity is calculate
+00011150: 640a 2020 2020 2020 2020 2020 2020 6279  d.            by
+00011160: 2063 656e 7472 616c 2066 696e 6974 6520   central finite 
+00011170: 6469 6666 6572 656e 6365 206d 6574 686f  difference metho
+00011180: 642e 2054 6869 7320 7661 6c75 6520 6769  d. This value gi
+00011190: 7665 7320 7468 6520 6469 7374 616e 6365  ves the distance
+000111a0: 0a20 2020 2020 2020 2020 2020 2069 6e20  .            in 
+000111b0: 626f 7468 2064 6972 6563 7469 6f6e 7320  both directions 
+000111c0: 696e 2031 2f41 6e67 7374 726f 6d2e 2054  in 1/Angstrom. T
+000111d0: 6865 2064 6566 6175 6c74 2076 616c 7565  he default value
+000111e0: 2077 696c 6c20 6265 2031 652d 352e 0a20   will be 1e-5.. 
+000111f0: 2020 2020 2020 2069 735f 6675 6c6c 5f70         is_full_p
+00011200: 7020 3a20 626f 6f6c 2c20 6f70 7469 6f6e  p : bool, option
+00011210: 616c 2c20 6465 6661 756c 7420 6973 2046  al, default is F
+00011220: 616c 7365 0a20 2020 2020 2020 2020 2020  alse.           
+00011230: 2057 6974 6820 5472 7565 2c20 6675 6c6c   With True, full
+00011240: 2065 6c65 6d65 6e74 7320 6f66 2070 686f   elements of pho
+00011250: 6e6f 6e2d 7068 6f6e 6f6e 2069 6e74 6572  non-phonon inter
+00011260: 6163 7469 6f6e 2073 7472 656e 6774 680a  action strength.
+00011270: 2020 2020 2020 2020 2020 2020 6172 6520              are 
+00011280: 636f 6d70 7574 6564 2e20 486f 7765 7665  computed. Howeve
+00011290: 7220 7769 7468 2074 6574 7261 6865 6472  r with tetrahedr
+000112a0: 6f6e 206d 6574 686f 642c 2070 6172 7420  on method, part 
+000112b0: 6f66 2074 6865 6d20 6172 650a 2020 2020  of them are.    
+000112c0: 2020 2020 2020 2020 6b6e 6f77 6e20 746f          known to
+000112d0: 2062 6520 7a65 726f 2061 6e64 2075 6e6e   be zero and unn
+000112e0: 6563 6573 7361 7279 2074 6f20 6361 6c63  ecessary to calc
+000112f0: 756c 6174 696f 6e2e 2057 6974 6820 4661  ulation. With Fa
+00011300: 6c73 652c 0a20 2020 2020 2020 2020 2020  lse,.           
+00011310: 2074 686f 7365 2065 6c65 6d65 6e74 7320   those elements 
+00011320: 6172 6520 6e6f 7420 6361 6c63 756c 6174  are not calculat
+00011330: 6564 2c20 6279 2077 6869 6368 2063 6f6e  ed, by which con
+00011340: 7369 6465 7261 626c 650a 2020 2020 2020  siderable.      
+00011350: 2020 2020 2020 696d 7072 6f76 6520 6f66        improve of
+00011360: 2065 6666 6963 6965 6e63 7920 6973 2065   efficiency is e
+00011370: 7870 6563 7465 642e 0a20 2020 2020 2020  xpected..       
+00011380: 2020 2020 2057 6974 6820 736d 6561 7269       With smeari
+00011390: 6e67 206d 6574 686f 642c 2065 7665 6e20  ng method, even 
+000113a0: 6966 2074 6869 7320 6973 2073 6574 2046  if this is set F
+000113b0: 616c 7365 2c20 6675 6c6c 2065 6c65 6d65  alse, full eleme
+000113c0: 6e74 730a 2020 2020 2020 2020 2020 2020  nts.            
+000113d0: 6172 6520 636f 6d70 7574 6564 2075 6e6c  are computed unl
+000113e0: 6573 7320 6073 6967 6d61 5f63 7574 6f66  ess `sigma_cutof
+000113f0: 6660 2069 7320 7370 6563 6966 6965 642e  f` is specified.
+00011400: 0a20 2020 2020 2020 2070 696e 765f 6375  .        pinv_cu
+00011410: 746f 6666 203a 2066 6c6f 6174 2c20 6f70  toff : float, op
+00011420: 7469 6f6e 616c 2c20 6465 6661 756c 7420  tional, default 
+00011430: 6973 2031 2e30 652d 380a 2020 2020 2020  is 1.0e-8.      
+00011440: 2020 2020 2020 4469 7265 6374 2073 6f6c        Direct sol
+00011450: 7574 696f 6e20 6f6e 6c79 2028 6069 735f  ution only (`is_
+00011460: 4c42 5445 3d54 7275 6560 292e 2054 6869  LBTE=True`). Thi
+00011470: 7320 6973 2075 7365 6420 6173 2061 2063  s is used as a c
+00011480: 7269 7465 7269 6f6e 0a20 2020 2020 2020  riterion.       
+00011490: 2020 2020 2074 6f20 6a75 6467 6520 7468       to judge th
+000114a0: 6520 6569 6765 6e76 616c 7565 7320 6172  e eigenvalues ar
+000114b0: 6520 636f 6e73 6964 6572 6564 2061 7320  e considered as 
+000114c0: 7a65 726f 206f 7220 6e6f 7420 696e 0a20  zero or not in. 
+000114d0: 2020 2020 2020 2020 2020 2070 7365 7564             pseud
+000114e0: 6f2d 696e 7665 7273 696f 6e20 6f66 2063  o-inversion of c
+000114f0: 6f6c 6c69 7369 6f6e 206d 6174 7269 782e  ollision matrix.
+00011500: 2053 6565 2061 6c73 6f20 6070 696e 765f   See also `pinv_
+00011510: 6d65 7468 6f64 602e 0a20 2020 2020 2020  method`..       
+00011520: 2070 696e 765f 6d65 7468 6f64 203a 2069   pinv_method : i
+00011530: 6e74 2c20 6f70 7469 6f6e 616c 2c20 6465  nt, optional, de
+00011540: 6661 756c 7420 6973 2030 2e0a 2020 2020  fault is 0..    
+00011550: 2020 2020 2020 2020 4469 7265 6374 2073          Direct s
+00011560: 6f6c 7574 696f 6e20 6f6e 6c79 2028 6069  olution only (`i
+00011570: 735f 4c42 5445 3d54 7275 6560 292e 0a20  s_LBTE=True`).. 
+00011580: 2020 2020 2020 2020 2020 2020 2020 2030                 0
+00011590: 2e20 6162 7328 6569 6765 6e76 616c 7565  . abs(eigenvalue
+000115a0: 2920 3c20 6070 696e 765f 6375 746f 6666  ) < `pinv_cutoff
+000115b0: 600a 2020 2020 2020 2020 2020 2020 2020  `.              
+000115c0: 2020 312e 2065 6967 656e 7661 6c75 6520    1. eigenvalue 
+000115d0: 3c20 6070 696e 765f 6375 746f 6666 600a  < `pinv_cutoff`.
+000115e0: 2020 2020 2020 2020 7069 6e76 5f73 6f6c          pinv_sol
+000115f0: 7665 7220 3a20 696e 742c 206f 7074 696f  ver : int, optio
+00011600: 6e61 6c2c 2064 6566 6175 6c74 2069 7320  nal, default is 
+00011610: 300a 2020 2020 2020 2020 2020 2020 4469  0.            Di
+00011620: 7265 6374 2073 6f6c 7574 696f 6e20 6f6e  rect solution on
+00011630: 6c79 2028 6069 735f 4c42 5445 3d54 7275  ly (`is_LBTE=Tru
+00011640: 6560 292e 2043 686f 6963 6520 6f66 2073  e`). Choice of s
+00011650: 6f6c 7665 7220 6f66 0a20 2020 2020 2020  olver of.       
+00011660: 2020 2020 2070 7365 7564 6f2d 696e 7665       pseudo-inve
+00011670: 7273 696f 6e20 6f66 2063 6f6c 6c69 7369  rsion of collisi
+00011680: 6f6e 206d 6174 7269 782e 2030 206d 6561  on matrix. 0 mea
+00011690: 6e73 2074 6865 2064 6566 6175 6c74 2063  ns the default c
+000116a0: 686f 6963 652e 0a20 2020 2020 2020 2020  hoice..         
+000116b0: 2020 2020 2020 2031 2e20 4c61 7061 636b         1. Lapack
+000116c0: 6520 6473 7965 763a 2053 6d61 6c6c 6572  e dsyev: Smaller
+000116d0: 206d 656d 6f72 7920 636f 6e73 756d 7074   memory consumpt
+000116e0: 696f 6e20 7468 616e 2064 7379 6576 642c  ion than dsyevd,
+000116f0: 2062 7574 0a20 2020 2020 2020 2020 2020   but.           
+00011700: 2020 2020 2020 2020 736c 6f77 6572 2e20          slower. 
+00011710: 5468 6973 2069 7320 7468 6520 6465 6661  This is the defa
+00011720: 756c 7420 736f 6c76 6572 2077 6865 6e20  ult solver when 
+00011730: 4d4b 4c20 4c41 5041 434b 4520 6973 0a20  MKL LAPACKE is. 
+00011740: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011750: 2020 696e 7465 6772 6174 6564 206f 7220    integrated or 
+00011760: 7363 6970 7920 6973 206e 6f74 2069 6e73  scipy is not ins
+00011770: 7461 6c6c 6564 2e0a 2020 2020 2020 2020  talled..        
+00011780: 2020 2020 2020 2020 322e 204c 6170 6163          2. Lapac
+00011790: 6b65 2064 7379 6576 643a 204c 6172 6765  ke dsyevd: Large
+000117a0: 7220 6d65 6d6f 7279 2063 6f6e 7375 6d70  r memory consump
+000117b0: 7469 6f6e 2074 6861 6e20 6473 7965 762c  tion than dsyev,
+000117c0: 2062 7574 0a20 2020 2020 2020 2020 2020   but.           
+000117d0: 2020 2020 2020 2020 6661 7374 6572 2e20          faster. 
+000117e0: 5468 6973 2069 7320 6e6f 7420 7265 636f  This is not reco
+000117f0: 6d6d 656e 6465 6420 6265 6361 7573 6520  mmended because 
+00011800: 736f 6d65 7469 6d65 7320 6120 7772 6f6e  sometimes a wron
+00011810: 670a 2020 2020 2020 2020 2020 2020 2020  g.              
+00011820: 2020 2020 2072 6573 756c 7420 6973 206f       result is o
+00011830: 6274 6169 6e65 642e 0a20 2020 2020 2020  btained..       
+00011840: 2020 2020 2020 2020 2033 2e20 4e75 6d70           3. Nump
+00011850: 79e2 8099 7320 6473 7965 7664 2028 6c69  y...s dsyevd (li
+00011860: 6e61 6c67 2e65 6967 6829 2e20 5468 6973  nalg.eigh). This
+00011870: 2069 7320 6e6f 7420 7265 636f 6d6d 656e   is not recommen
+00011880: 6465 640a 2020 2020 2020 2020 2020 2020  ded.            
+00011890: 2020 2020 2020 2062 6563 6175 7365 2073         because s
+000118a0: 6f6d 6574 696d 6573 2061 2077 726f 6e67  ometimes a wrong
+000118b0: 2072 6573 756c 7420 6973 206f 6274 6169   result is obtai
+000118c0: 6e65 642e 0a20 2020 2020 2020 2020 2020  ned..           
+000118d0: 2020 2020 2034 2e20 5363 6970 79e2 8099       4. Scipy...
+000118e0: 7320 6473 7965 763a 2054 6869 7320 6973  s dsyev: This is
+000118f0: 2074 6865 2064 6566 6175 6c74 2073 6f6c   the default sol
+00011900: 7665 7220 7768 656e 2073 6369 7079 2069  ver when scipy i
+00011910: 730a 2020 2020 2020 2020 2020 2020 2020  s.              
+00011920: 2020 2020 2069 6e73 7461 6c6c 6564 2061       installed a
+00011930: 6e64 204d 4b4c 204c 4150 4143 4b45 2069  nd MKL LAPACKE i
+00011940: 7320 6e6f 7420 696e 7465 6772 6174 6564  s not integrated
+00011950: 2e0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00011960: 2020 352e 2053 6369 7079 e280 9973 2064    5. Scipy...s d
+00011970: 7379 6576 642e 2054 6869 7320 6973 206e  syevd. This is n
+00011980: 6f74 2072 6563 6f6d 6d65 6e64 6564 2062  ot recommended b
+00011990: 6563 6175 7365 2073 6f6d 6574 696d 6573  ecause sometimes
+000119a0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000119b0: 2020 2020 6120 7772 6f6e 6720 7265 7375      a wrong resu
+000119c0: 6c74 2069 7320 6f62 7461 696e 6564 2e0a  lt is obtained..
+000119d0: 2020 2020 2020 2020 2020 2020 5468 6520              The 
+000119e0: 736f 6c76 6572 2063 686f 6963 6573 206f  solver choices o
+000119f0: 7468 6572 2074 6861 6e20 2d2d 7069 6e76  ther than --pinv
+00011a00: 2d73 6f6c 7665 723d 3120 616e 640a 2020  -solver=1 and.  
+00011a10: 2020 2020 2020 2020 2020 2d2d 7069 6e76            --pinv
+00011a20: 2d73 6f6c 7665 723d 3420 6172 6520 6461  -solver=4 are da
+00011a30: 6e67 6572 6f75 7320 616e 6420 6e6f 7420  ngerous and not 
+00011a40: 7265 636f 6d6d 656e 642e 0a20 2020 2020  recommend..     
+00011a50: 2020 2077 7269 7465 5f67 616d 6d61 203a     write_gamma :
+00011a60: 2062 6f6f 6c2c 206f 7074 696f 6e61 6c2c   bool, optional,
+00011a70: 2064 6566 6175 6c74 2069 7320 4661 6c73   default is Fals
+00011a80: 650a 2020 2020 2020 2020 2020 2020 5254  e.            RT
+00011a90: 4120 6f6e 6c79 2028 6069 735f 4c42 5445  A only (`is_LBTE
+00011aa0: 3d46 616c 7365 6029 2e20 5769 7468 2054  =False`). With T
+00011ab0: 7275 652c 2057 7269 7465 206d 6f64 6520  rue, Write mode 
+00011ac0: 7468 6572 6d61 6c0a 2020 2020 2020 2020  thermal.        
+00011ad0: 2020 2020 636f 6e64 7563 7469 7669 7479      conductivity
+00011ae0: 2070 726f 7065 7274 6965 7320 696e 746f   properties into
+00011af0: 2066 696c 6573 2061 7420 6561 6368 2067   files at each g
+00011b00: 7269 6420 706f 696e 742e 2057 6974 680a  rid point. With.
+00011b10: 2020 2020 2020 2020 2020 2020 6062 616e              `ban
+00011b20: 645f 696e 6469 6365 7360 206f 7220 6d75  d_indices` or mu
+00011b30: 6c74 6970 6c65 2060 7369 676d 6173 6020  ltiple `sigmas` 
+00011b40: 6973 2073 7065 6369 6669 6564 2c20 7468  is specified, th
+00011b50: 6520 6669 6c65 730a 2020 2020 2020 2020  e files.        
+00011b60: 2020 2020 6172 6520 6d61 6465 2066 6f72      are made for
+00011b70: 2065 6163 6820 6f66 2074 6865 6d2c 2074   each of them, t
+00011b80: 6f6f 2e0a 2020 2020 2020 2020 7265 6164  oo..        read
+00011b90: 5f67 616d 6d61 203a 2062 6f6f 6c2c 206f  _gamma : bool, o
+00011ba0: 7074 696f 6e61 6c2c 2064 6566 6175 6c74  ptional, default
+00011bb0: 2069 7320 4661 6c73 650a 2020 2020 2020   is False.      
+00011bc0: 2020 2020 2020 5254 4120 6f6e 6c79 2028        RTA only (
+00011bd0: 6069 735f 4c42 5445 3d46 616c 7365 6029  `is_LBTE=False`)
+00011be0: 2e20 5769 7468 2054 7275 652c 2064 6561  . With True, dea
+00011bf0: 6420 6669 6c65 7320 6372 6561 7465 6420  d files created 
+00011c00: 6279 0a20 2020 2020 2020 2020 2020 2060  by.            `
+00011c10: 7772 6974 655f 6761 6d6d 613d 5472 7565  write_gamma=True
+00011c20: 6020 696e 7374 6561 6420 6f66 2063 616c  ` instead of cal
+00011c30: 6375 6c61 7469 6e67 2070 686f 6e6f 6e2d  culating phonon-
+00011c40: 7068 6f6e 6f6e 0a20 2020 2020 2020 2020  phonon.         
+00011c50: 2020 2069 6e74 6572 6163 7469 6f6e 2073     interaction s
+00011c60: 7472 656e 6774 6820 616e 6420 696d 6167  trength and imag
+00011c70: 696e 6172 7920 7061 7274 7320 6f66 2073  inary parts of s
+00011c80: 656c 662d 656e 6572 6779 2e0a 2020 2020  elf-energy..    
+00011c90: 2020 2020 6973 5f4e 5f55 203a 2062 6f6f      is_N_U : boo
+00011ca0: 6c2c 206f 7074 696f 6e61 6c2c 2064 6566  l, optional, def
+00011cb0: 6175 6c74 2069 7320 4661 6c73 650a 2020  ault is False.  
+00011cc0: 2020 2020 2020 2020 2020 5254 4120 6f6e            RTA on
+00011cd0: 6c79 2028 6069 735f 4c42 5445 3d46 616c  ly (`is_LBTE=Fal
+00011ce0: 7365 6029 2e20 5769 7468 2054 7275 652c  se`). With True,
+00011cf0: 2063 6174 6567 6f72 697a 6174 696f 6e20   categorization 
+00011d00: 6f66 206e 6f72 6d61 6c0a 2020 2020 2020  of normal.      
+00011d10: 2020 2020 2020 616e 6420 556d 6b6c 6170        and Umklap
+00011d20: 7020 7363 6174 7465 7269 6e67 2069 7320  p scattering is 
+00011d30: 6d61 6465 2061 6e64 2069 6d61 6769 6e61  made and imagina
+00011d40: 7279 2070 6172 7473 206f 6620 7365 6c66  ry parts of self
+00011d50: 2065 6e65 7267 790a 2020 2020 2020 2020   energy.        
+00011d60: 2020 2020 666f 7220 7468 656d 2061 7265      for them are
+00011d70: 2073 6570 6172 6174 6564 2e0a 2020 2020   separated..    
+00011d80: 2020 2020 636f 6e64 7563 7469 7669 7479      conductivity
+00011d90: 5f74 7970 6520 3a20 7374 722c 206f 7074  _type : str, opt
+00011da0: 696f 6e61 6c0a 2020 2020 2020 2020 2020  ional.          
+00011db0: 2020 2277 6967 6e65 7222 2c20 226b 7562    "wigner", "kub
+00011dc0: 6f22 2c20 6f72 204e 6f6e 652e 2044 6566  o", or None. Def
+00011dd0: 6175 6c74 2069 7320 4e6f 6e65 2e0a 2020  ault is None..  
+00011de0: 2020 2020 2020 7772 6974 655f 6b61 7070        write_kapp
+00011df0: 6120 3a20 626f 6f6c 2c20 6f70 7469 6f6e  a : bool, option
+00011e00: 616c 2c20 6465 6661 756c 7420 6973 2046  al, default is F
+00011e10: 616c 7365 0a20 2020 2020 2020 2020 2020  alse.           
+00011e20: 2057 6974 6820 5472 7565 2c20 7468 6572   With True, ther
+00011e30: 6d61 6c20 636f 6e64 7563 7469 7669 7479  mal conductivity
+00011e40: 2061 6e64 2072 656c 6174 6564 2070 726f   and related pro
+00011e50: 7065 7274 6965 7320 6172 650a 2020 2020  perties are.    
+00011e60: 2020 2020 2020 2020 7772 6974 7465 6e20          written 
+00011e70: 696e 746f 2061 2066 696c 652e 2057 6974  into a file. Wit
+00011e80: 6820 6d75 6c74 6970 6c65 2060 7369 676d  h multiple `sigm
+00011e90: 6173 602c 2072 6573 7065 6374 6976 6520  as`, respective 
+00011ea0: 6669 6c65 730a 2020 2020 2020 2020 2020  files.          
+00011eb0: 2020 6172 6520 6372 6561 7465 642e 0a20    are created.. 
+00011ec0: 2020 2020 2020 2077 7269 7465 5f67 616d         write_gam
+00011ed0: 6d61 5f64 6574 6169 6c20 3a20 626f 6f6c  ma_detail : bool
+00011ee0: 2c20 6f70 7469 6f6e 616c 2c20 6465 6661  , optional, defa
+00011ef0: 756c 7420 6973 2046 616c 7365 0a20 2020  ult is False.   
+00011f00: 2020 2020 2020 2020 2052 5441 206f 6e6c           RTA onl
+00011f10: 7920 2860 6973 5f4c 4254 453d 4661 6c73  y (`is_LBTE=Fals
+00011f20: 6560 292e 2057 6974 6820 5472 7565 2c20  e`). With True, 
+00011f30: 6465 7461 696c 6564 2069 6e66 6f72 6d61  detailed informa
+00011f40: 7469 6f6e 206f 660a 2020 2020 2020 2020  tion of.        
+00011f50: 2020 2020 696d 6167 696e 6172 7920 7061      imaginary pa
+00011f60: 7274 7320 6f66 2073 656c 6620 656e 6572  rts of self ener
+00011f70: 6779 2069 7320 7374 6f72 6564 2069 6e74  gy is stored int
+00011f80: 6f20 6669 6c65 7320 7375 6368 2061 730a  o files such as.
+00011f90: 2020 2020 2020 2020 2020 2020 7468 6f73              thos
+00011fa0: 6520 6d61 6465 2062 7920 6077 7269 7465  e made by `write
+00011fb0: 5f67 616d 6d61 602e 0a20 2020 2020 2020  _gamma`..       
+00011fc0: 2077 7269 7465 5f63 6f6c 6c69 7369 6f6e   write_collision
+00011fd0: 203a 2062 6f6f 6c2c 206f 7074 696f 6e61   : bool, optiona
+00011fe0: 6c2c 2064 6566 6175 6c74 2069 7320 4661  l, default is Fa
+00011ff0: 6c73 650a 2020 2020 2020 2020 2020 2020  lse.            
+00012000: 4469 7265 6374 2073 6f6c 7574 696f 6e20  Direct solution 
+00012010: 6f6e 6c79 2028 6069 735f 4c42 5445 3d54  only (`is_LBTE=T
+00012020: 7275 6560 292e 2057 6974 6820 5472 7565  rue`). With True
+00012030: 2c20 636f 6c6c 6973 696f 6e20 6d61 7472  , collision matr
+00012040: 6978 0a20 2020 2020 2020 2020 2020 2069  ix.            i
+00012050: 7320 7772 6974 7465 6e20 696e 746f 2061  s written into a
+00012060: 2066 696c 652e 2057 6974 6820 6d75 6c74   file. With mult
+00012070: 6970 6c65 2060 7369 676d 6173 6020 7370  iple `sigmas` sp
+00012080: 6563 6966 6965 642c 0a20 2020 2020 2020  ecified,.       
+00012090: 2020 2020 2072 6573 7065 6374 6976 6520       respective 
+000120a0: 6669 6c65 7320 6172 6520 6372 6561 7465  files are create
+000120b0: 642e 2042 6520 6361 7265 6675 6c20 7468  d. Be careful th
+000120c0: 6174 2074 6869 7320 6669 6c65 2063 616e  at this file can
+000120d0: 2062 650a 2020 2020 2020 2020 2020 2020   be.            
+000120e0: 6875 6765 2e0a 2020 2020 2020 2020 7265  huge..        re
+000120f0: 6164 5f63 6f6c 6c69 7369 6f6e 203a 2062  ad_collision : b
+00012100: 6f6f 6c2c 206f 7074 696f 6e61 6c2c 2064  ool, optional, d
+00012110: 6566 6175 6c74 2069 7320 4661 6c73 650a  efault is False.
+00012120: 2020 2020 2020 2020 2020 2020 4469 7265              Dire
+00012130: 6374 2073 6f6c 7574 696f 6e20 6f6e 6c79  ct solution only
+00012140: 2028 6069 735f 4c42 5445 3d54 7275 6560   (`is_LBTE=True`
+00012150: 292e 2057 6974 6820 5472 7565 2c20 636f  ). With True, co
+00012160: 6c6c 6973 696f 6e20 6d61 7472 6978 0a20  llision matrix. 
+00012170: 2020 2020 2020 2020 2020 2069 7320 7265             is re
+00012180: 6164 2066 726f 6d20 6120 6669 6c65 2e0a  ad from a file..
+00012190: 2020 2020 2020 2020 7772 6974 655f 7070          write_pp
+000121a0: 203a 2062 6f6f 6c2c 206f 7074 696f 6e61   : bool, optiona
+000121b0: 6c2c 2064 6566 6175 6c74 2069 7320 4661  l, default is Fa
+000121c0: 6c73 650a 2020 2020 2020 2020 2020 2020  lse.            
+000121d0: 5769 7468 2054 7275 652c 2070 686f 6e6f  With True, phono
+000121e0: 6e2d 7068 6f6e 6f6e 2069 6e74 6572 6163  n-phonon interac
+000121f0: 7469 6f6e 2073 7472 656e 6774 6820 6973  tion strength is
+00012200: 2077 7269 7474 656e 2069 6e74 6f0a 2020   written into.  
+00012210: 2020 2020 2020 2020 2020 6669 6c65 7320            files 
+00012220: 6174 2065 6163 6820 6772 6964 2070 6f69  at each grid poi
+00012230: 6e74 2e20 5468 6973 206f 7074 696f 6e20  nt. This option 
+00012240: 6173 7375 6d65 7320 7369 6e67 6c65 2076  assumes single v
+00012250: 616c 7565 2069 7320 696e 0a20 2020 2020  alue is in.     
+00012260: 2020 2020 2020 2060 7369 676d 6173 602e         `sigmas`.
+00012270: 0a20 2020 2020 2020 2072 6561 645f 7070  .        read_pp
+00012280: 203a 2062 6f6f 6c2c 206f 7074 696f 6e61   : bool, optiona
+00012290: 6c2c 2064 6566 6175 6c74 2069 7320 4661  l, default is Fa
+000122a0: 6c73 650a 2020 2020 2020 2020 2020 2020  lse.            
+000122b0: 5769 7468 2054 7275 652c 2070 686f 6e6f  With True, phono
+000122c0: 6e2d 7068 6f6e 6f6e 2069 6e74 6572 6163  n-phonon interac
+000122d0: 7469 6f6e 2073 7472 656e 6774 6820 6973  tion strength is
+000122e0: 2072 6561 6420 6672 6f6d 2066 696c 6573   read from files
+000122f0: 2e0a 2020 2020 2020 2020 7772 6974 655f  ..        write_
+00012300: 4c42 5445 5f73 6f6c 7574 696f 6e20 3a20  LBTE_solution : 
+00012310: 626f 6f6c 2c20 6f70 7469 6f6e 616c 2c20  bool, optional, 
+00012320: 6465 6661 756c 7420 6973 2046 616c 7365  default is False
+00012330: 0a20 2020 2020 2020 2020 2020 2044 6972  .            Dir
+00012340: 6563 7420 736f 6c75 7469 6f6e 206f 6e6c  ect solution onl
+00012350: 7920 2860 6973 5f4c 4254 453d 5472 7565  y (`is_LBTE=True
+00012360: 6029 2e20 5769 7468 2054 7275 652c 2065  `). With True, e
+00012370: 6967 656e 7665 6374 6f72 7320 6f66 0a20  igenvectors of. 
+00012380: 2020 2020 2020 2020 2020 2063 6f6c 6c69             colli
+00012390: 7369 6f6e 206d 6174 7269 7820 6973 2077  sion matrix is w
+000123a0: 7269 7474 656e 2069 6e20 6120 6669 6c65  ritten in a file
+000123b0: 2061 7320 7468 6520 726f 7720 7665 6374   as the row vect
+000123c0: 6f72 7320 6578 6365 7074 0a20 2020 2020  ors except.     
+000123d0: 2020 2020 2020 2075 6e6c 6573 7320 6070         unless `p
+000123e0: 696e 765f 736f 6c76 6572 3d33 6020 2866  inv_solver=3` (f
+000123f0: 6f72 2074 6869 732c 2063 6f6c 756d 6e20  or this, column 
+00012400: 7665 6374 6f72 7329 2e20 5769 7468 206d  vectors). With m
+00012410: 756c 7469 706c 650a 2020 2020 2020 2020  ultiple.        
+00012420: 2020 2020 6073 6967 6d61 7360 2073 7065      `sigmas` spe
+00012430: 6369 6669 6564 2c20 7265 7370 6563 7469  cified, respecti
+00012440: 7665 2066 696c 6573 2061 7265 2063 7265  ve files are cre
+00012450: 6174 6564 2e20 4265 2063 6172 6566 756c  ated. Be careful
+00012460: 2074 6861 740a 2020 2020 2020 2020 2020   that.          
+00012470: 2020 7468 6973 2066 696c 6520 6361 6e20    this file can 
+00012480: 6265 2068 7567 652e 0a20 2020 2020 2020  be huge..       
+00012490: 2063 6f6d 7072 6573 7369 6f6e 3a20 7374   compression: st
+000124a0: 722c 206f 7074 696f 6e61 6c2c 2064 6566  r, optional, def
+000124b0: 6175 6c74 2069 7320 2267 7a69 7022 0a20  ault is "gzip". 
+000124c0: 2020 2020 2020 2020 2020 2057 6865 6e20             When 
+000124d0: 7772 6974 696e 6720 7265 7375 6c74 7320  writing results 
+000124e0: 696e 746f 2066 696c 6573 2069 6e20 6864  into files in hd
+000124f0: 6635 2c20 6c61 7267 6520 6461 7461 2061  f5, large data a
+00012500: 7265 2063 6f6d 7072 6573 7365 640a 2020  re compressed.  
+00012510: 2020 2020 2020 2020 2020 6279 2074 6869            by thi
+00012520: 7320 6f70 7469 6f6e 732e 2053 6565 2074  s options. See t
+00012530: 6865 2064 6574 6169 6c20 6174 2068 3570  he detail at h5p
+00012540: 7920 646f 6375 6d65 6e74 6174 696f 6e2e  y documentation.
+00012550: 0a20 2020 2020 2020 2069 6e70 7574 5f66  .        input_f
+00012560: 696c 656e 616d 6520 3a20 7374 722c 206f  ilename : str, o
+00012570: 7074 696f 6e61 6c2c 2064 6566 6175 6c74  ptional, default
+00012580: 2069 7320 4e6f 6e65 0a20 2020 2020 2020   is None.       
+00012590: 2020 2020 2057 6865 6e20 7370 6563 6966       When specif
+000125a0: 6965 642c 2074 6865 2073 7472 696e 6720  ied, the string 
+000125b0: 6973 2069 6e73 6572 7465 6420 6265 666f  is inserted befo
+000125c0: 7265 2066 696c 656e 616d 6520 6578 7465  re filename exte
+000125d0: 6e73 696f 6e0a 2020 2020 2020 2020 2020  nsion.          
+000125e0: 2020 696e 2072 6561 6469 6e67 2066 696c    in reading fil
+000125f0: 6573 2e0a 2020 2020 2020 2020 6f75 7470  es..        outp
+00012600: 7574 5f66 696c 656e 616d 6520 3a20 7374  ut_filename : st
+00012610: 722c 206f 7074 696f 6e61 6c2c 2064 6566  r, optional, def
+00012620: 6175 6c74 2069 7320 4e6f 6e65 0a20 2020  ault is None.   
+00012630: 2020 2020 2020 2020 2057 6865 6e20 7370           When sp
+00012640: 6563 6966 6965 642c 2074 6865 2073 7472  ecified, the str
+00012650: 696e 6720 6973 2069 6e73 6572 7465 6420  ing is inserted 
+00012660: 6265 666f 7265 2066 696c 656e 616d 6520  before filename 
+00012670: 6578 7465 6e73 696f 6e0a 2020 2020 2020  extension.      
+00012680: 2020 2020 2020 696e 2077 7269 7469 6e67        in writing
+00012690: 2066 696c 6573 2e0a 0a20 2020 2020 2020   files...       
+000126a0: 2022 2222 0a20 2020 2020 2020 2069 6620   """.        if 
+000126b0: 7365 6c66 2e5f 696e 7465 7261 6374 696f  self._interactio
+000126c0: 6e20 6973 204e 6f6e 653a 0a20 2020 2020  n is None:.     
+000126d0: 2020 2020 2020 206d 7367 203d 2028 0a20         msg = (. 
+000126e0: 2020 2020 2020 2020 2020 2020 2020 2022                 "
+000126f0: 5068 6f6e 6f33 7079 2e69 6e69 745f 7068  Phono3py.init_ph
+00012700: 7068 5f69 6e74 6572 6163 7469 6f6e 2068  ph_interaction h
+00012710: 6173 2074 6f20 6265 2063 616c 6c65 6420  as to be called 
+00012720: 220a 2020 2020 2020 2020 2020 2020 2020  ".              
+00012730: 2020 2262 6566 6f72 6520 7275 6e6e 696e    "before runnin
+00012740: 6720 7468 6973 206d 6574 686f 642e 220a  g this method.".
+00012750: 2020 2020 2020 2020 2020 2020 290a 2020              ).  
+00012760: 2020 2020 2020 2020 2020 7261 6973 6520            raise 
+00012770: 5275 6e74 696d 6545 7272 6f72 286d 7367  RuntimeError(msg
+00012780: 290a 0a20 2020 2020 2020 2069 6620 6973  )..        if is
+00012790: 5f4c 4254 453a 0a20 2020 2020 2020 2020  _LBTE:.         
+000127a0: 2020 2069 6620 7465 6d70 6572 6174 7572     if temperatur
+000127b0: 6573 2069 7320 4e6f 6e65 3a0a 2020 2020  es is None:.    
+000127c0: 2020 2020 2020 2020 2020 2020 5f74 656d              _tem
+000127d0: 7065 7261 7475 7265 7320 3d20 5b0a 2020  peratures = [.  
+000127e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000127f0: 2020 3330 302c 0a20 2020 2020 2020 2020    300,.         
+00012800: 2020 2020 2020 205d 0a20 2020 2020 2020         ].       
+00012810: 2020 2020 2065 6c73 653a 0a20 2020 2020       else:.     
+00012820: 2020 2020 2020 2020 2020 205f 7465 6d70             _temp
+00012830: 6572 6174 7572 6573 203d 2074 656d 7065  eratures = tempe
+00012840: 7261 7475 7265 730a 2020 2020 2020 2020  ratures.        
+00012850: 2020 2020 7365 6c66 2e5f 7468 6572 6d61      self._therma
+00012860: 6c5f 636f 6e64 7563 7469 7669 7479 203d  l_conductivity =
+00012870: 2067 6574 5f74 6865 726d 616c 5f63 6f6e   get_thermal_con
+00012880: 6475 6374 6976 6974 795f 4c42 5445 280a  ductivity_LBTE(.
+00012890: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000128a0: 7365 6c66 2e5f 696e 7465 7261 6374 696f  self._interactio
+000128b0: 6e2c 0a20 2020 2020 2020 2020 2020 2020  n,.             
+000128c0: 2020 2074 656d 7065 7261 7475 7265 733d     temperatures=
+000128d0: 5f74 656d 7065 7261 7475 7265 732c 0a20  _temperatures,. 
+000128e0: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+000128f0: 6967 6d61 733d 7365 6c66 2e5f 7369 676d  igmas=self._sigm
+00012900: 6173 2c0a 2020 2020 2020 2020 2020 2020  as,.            
+00012910: 2020 2020 7369 676d 615f 6375 746f 6666      sigma_cutoff
+00012920: 3d73 656c 662e 5f73 6967 6d61 5f63 7574  =self._sigma_cut
+00012930: 6f66 662c 0a20 2020 2020 2020 2020 2020  off,.           
+00012940: 2020 2020 2069 735f 6973 6f74 6f70 653d       is_isotope=
+00012950: 6973 5f69 736f 746f 7065 2c0a 2020 2020  is_isotope,.    
+00012960: 2020 2020 2020 2020 2020 2020 6d61 7373              mass
+00012970: 5f76 6172 6961 6e63 6573 3d6d 6173 735f  _variances=mass_
+00012980: 7661 7269 616e 6365 732c 0a20 2020 2020  variances,.     
+00012990: 2020 2020 2020 2020 2020 2067 7269 645f             grid_
+000129a0: 706f 696e 7473 3d67 7269 645f 706f 696e  points=grid_poin
+000129b0: 7473 2c0a 2020 2020 2020 2020 2020 2020  ts,.            
+000129c0: 2020 2020 626f 756e 6461 7279 5f6d 6670      boundary_mfp
+000129d0: 3d62 6f75 6e64 6172 795f 6d66 702c 0a20  =boundary_mfp,. 
+000129e0: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+000129f0: 6f6c 7665 5f63 6f6c 6c65 6374 6976 655f  olve_collective_
+00012a00: 7068 6f6e 6f6e 3d73 6f6c 7665 5f63 6f6c  phonon=solve_col
+00012a10: 6c65 6374 6976 655f 7068 6f6e 6f6e 2c0a  lective_phonon,.
+00012a20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012a30: 6973 5f72 6564 7563 6962 6c65 5f63 6f6c  is_reducible_col
+00012a40: 6c69 7369 6f6e 5f6d 6174 7269 783d 6973  lision_matrix=is
+00012a50: 5f72 6564 7563 6962 6c65 5f63 6f6c 6c69  _reducible_colli
+00012a60: 7369 6f6e 5f6d 6174 7269 782c 0a20 2020  sion_matrix,.   
+00012a70: 2020 2020 2020 2020 2020 2020 2069 735f               is_
+00012a80: 6b61 7070 615f 7374 6172 3d69 735f 6b61  kappa_star=is_ka
+00012a90: 7070 615f 7374 6172 2c0a 2020 2020 2020  ppa_star,.      
+00012aa0: 2020 2020 2020 2020 2020 6776 5f64 656c            gv_del
+00012ab0: 7461 5f71 3d67 765f 6465 6c74 615f 712c  ta_q=gv_delta_q,
+00012ac0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00012ad0: 2069 735f 6675 6c6c 5f70 703d 6973 5f66   is_full_pp=is_f
+00012ae0: 756c 6c5f 7070 2c0a 2020 2020 2020 2020  ull_pp,.        
+00012af0: 2020 2020 2020 2020 636f 6e64 7563 7469          conducti
+00012b00: 7669 7479 5f74 7970 653d 636f 6e64 7563  vity_type=conduc
+00012b10: 7469 7669 7479 5f74 7970 652c 0a20 2020  tivity_type,.   
+00012b20: 2020 2020 2020 2020 2020 2020 2070 696e               pin
+00012b30: 765f 6375 746f 6666 3d70 696e 765f 6375  v_cutoff=pinv_cu
+00012b40: 746f 6666 2c0a 2020 2020 2020 2020 2020  toff,.          
+00012b50: 2020 2020 2020 7069 6e76 5f73 6f6c 7665        pinv_solve
+00012b60: 723d 7069 6e76 5f73 6f6c 7665 722c 0a20  r=pinv_solver,. 
+00012b70: 2020 2020 2020 2020 2020 2020 2020 2070                 p
+00012b80: 696e 765f 6d65 7468 6f64 3d70 696e 765f  inv_method=pinv_
+00012b90: 6d65 7468 6f64 2c0a 2020 2020 2020 2020  method,.        
+00012ba0: 2020 2020 2020 2020 7772 6974 655f 636f          write_co
+00012bb0: 6c6c 6973 696f 6e3d 7772 6974 655f 636f  llision=write_co
+00012bc0: 6c6c 6973 696f 6e2c 0a20 2020 2020 2020  llision,.       
+00012bd0: 2020 2020 2020 2020 2072 6561 645f 636f           read_co
+00012be0: 6c6c 6973 696f 6e3d 7265 6164 5f63 6f6c  llision=read_col
+00012bf0: 6c69 7369 6f6e 2c0a 2020 2020 2020 2020  lision,.        
+00012c00: 2020 2020 2020 2020 7772 6974 655f 6b61          write_ka
+00012c10: 7070 613d 7772 6974 655f 6b61 7070 612c  ppa=write_kappa,
+00012c20: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00012c30: 2077 7269 7465 5f70 703d 7772 6974 655f   write_pp=write_
+00012c40: 7070 2c0a 2020 2020 2020 2020 2020 2020  pp,.            
+00012c50: 2020 2020 7265 6164 5f70 703d 7265 6164      read_pp=read
+00012c60: 5f70 702c 0a20 2020 2020 2020 2020 2020  _pp,.           
+00012c70: 2020 2020 2077 7269 7465 5f4c 4254 455f       write_LBTE_
+00012c80: 736f 6c75 7469 6f6e 3d77 7269 7465 5f4c  solution=write_L
+00012c90: 4254 455f 736f 6c75 7469 6f6e 2c0a 2020  BTE_solution,.  
+00012ca0: 2020 2020 2020 2020 2020 2020 2020 636f                co
+00012cb0: 6d70 7265 7373 696f 6e3d 636f 6d70 7265  mpression=compre
+00012cc0: 7373 696f 6e2c 0a20 2020 2020 2020 2020  ssion,.         
+00012cd0: 2020 2020 2020 2069 6e70 7574 5f66 696c         input_fil
+00012ce0: 656e 616d 653d 696e 7075 745f 6669 6c65  ename=input_file
+00012cf0: 6e61 6d65 2c0a 2020 2020 2020 2020 2020  name,.          
+00012d00: 2020 2020 2020 6f75 7470 7574 5f66 696c        output_fil
+00012d10: 656e 616d 653d 6f75 7470 7574 5f66 696c  ename=output_fil
+00012d20: 656e 616d 652c 0a20 2020 2020 2020 2020  ename,.         
+00012d30: 2020 2020 2020 206c 6f67 5f6c 6576 656c         log_level
+00012d40: 3d73 656c 662e 5f6c 6f67 5f6c 6576 656c  =self._log_level
+00012d50: 2c0a 2020 2020 2020 2020 2020 2020 290a  ,.            ).
+00012d60: 2020 2020 2020 2020 656c 7365 3a0a 2020          else:.  
+00012d70: 2020 2020 2020 2020 2020 6966 2074 656d            if tem
+00012d80: 7065 7261 7475 7265 7320 6973 204e 6f6e  peratures is Non
+00012d90: 653a 0a20 2020 2020 2020 2020 2020 2020  e:.             
+00012da0: 2020 205f 7465 6d70 6572 6174 7572 6573     _temperatures
+00012db0: 203d 206e 702e 6172 616e 6765 2830 2c20   = np.arange(0, 
+00012dc0: 3130 3031 2c20 3130 2c20 6474 7970 653d  1001, 10, dtype=
+00012dd0: 2264 6f75 626c 6522 290a 2020 2020 2020  "double").      
+00012de0: 2020 2020 2020 656c 7365 3a0a 2020 2020        else:.    
+00012df0: 2020 2020 2020 2020 2020 2020 5f74 656d              _tem
+00012e00: 7065 7261 7475 7265 7320 3d20 7465 6d70  peratures = temp
+00012e10: 6572 6174 7572 6573 0a20 2020 2020 2020  eratures.       
+00012e20: 2020 2020 2073 656c 662e 5f74 6865 726d       self._therm
+00012e30: 616c 5f63 6f6e 6475 6374 6976 6974 7920  al_conductivity 
+00012e40: 3d20 6765 745f 7468 6572 6d61 6c5f 636f  = get_thermal_co
+00012e50: 6e64 7563 7469 7669 7479 5f52 5441 280a  nductivity_RTA(.
+00012e60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012e70: 7365 6c66 2e5f 696e 7465 7261 6374 696f  self._interactio
+00012e80: 6e2c 0a20 2020 2020 2020 2020 2020 2020  n,.             
+00012e90: 2020 2074 656d 7065 7261 7475 7265 733d     temperatures=
+00012ea0: 5f74 656d 7065 7261 7475 7265 732c 0a20  _temperatures,. 
+00012eb0: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+00012ec0: 6967 6d61 733d 7365 6c66 2e5f 7369 676d  igmas=self._sigm
+00012ed0: 6173 2c0a 2020 2020 2020 2020 2020 2020  as,.            
+00012ee0: 2020 2020 7369 676d 615f 6375 746f 6666      sigma_cutoff
+00012ef0: 3d73 656c 662e 5f73 6967 6d61 5f63 7574  =self._sigma_cut
+00012f00: 6f66 662c 0a20 2020 2020 2020 2020 2020  off,.           
+00012f10: 2020 2020 2069 735f 6973 6f74 6f70 653d       is_isotope=
+00012f20: 6973 5f69 736f 746f 7065 2c0a 2020 2020  is_isotope,.    
+00012f30: 2020 2020 2020 2020 2020 2020 6d61 7373              mass
+00012f40: 5f76 6172 6961 6e63 6573 3d6d 6173 735f  _variances=mass_
+00012f50: 7661 7269 616e 6365 732c 0a20 2020 2020  variances,.     
+00012f60: 2020 2020 2020 2020 2020 2067 7269 645f             grid_
+00012f70: 706f 696e 7473 3d67 7269 645f 706f 696e  points=grid_poin
+00012f80: 7473 2c0a 2020 2020 2020 2020 2020 2020  ts,.            
+00012f90: 2020 2020 626f 756e 6461 7279 5f6d 6670      boundary_mfp
+00012fa0: 3d62 6f75 6e64 6172 795f 6d66 702c 0a20  =boundary_mfp,. 
+00012fb0: 2020 2020 2020 2020 2020 2020 2020 2075                 u
+00012fc0: 7365 5f61 7665 5f70 703d 7573 655f 6176  se_ave_pp=use_av
+00012fd0: 655f 7070 2c0a 2020 2020 2020 2020 2020  e_pp,.          
+00012fe0: 2020 2020 2020 6973 5f6b 6170 7061 5f73        is_kappa_s
+00012ff0: 7461 723d 6973 5f6b 6170 7061 5f73 7461  tar=is_kappa_sta
+00013000: 722c 0a20 2020 2020 2020 2020 2020 2020  r,.             
+00013010: 2020 2067 765f 6465 6c74 615f 713d 6776     gv_delta_q=gv
+00013020: 5f64 656c 7461 5f71 2c0a 2020 2020 2020  _delta_q,.      
+00013030: 2020 2020 2020 2020 2020 6973 5f66 756c            is_ful
+00013040: 6c5f 7070 3d69 735f 6675 6c6c 5f70 702c  l_pp=is_full_pp,
+00013050: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00013060: 2069 735f 4e5f 553d 6973 5f4e 5f55 2c0a   is_N_U=is_N_U,.
+00013070: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00013080: 636f 6e64 7563 7469 7669 7479 5f74 7970  conductivity_typ
+00013090: 653d 636f 6e64 7563 7469 7669 7479 5f74  e=conductivity_t
+000130a0: 7970 652c 0a20 2020 2020 2020 2020 2020  ype,.           
+000130b0: 2020 2020 2077 7269 7465 5f67 616d 6d61       write_gamma
+000130c0: 3d77 7269 7465 5f67 616d 6d61 2c0a 2020  =write_gamma,.  
+000130d0: 2020 2020 2020 2020 2020 2020 2020 7265                re
+000130e0: 6164 5f67 616d 6d61 3d72 6561 645f 6761  ad_gamma=read_ga
+000130f0: 6d6d 612c 0a20 2020 2020 2020 2020 2020  mma,.           
+00013100: 2020 2020 2077 7269 7465 5f6b 6170 7061       write_kappa
+00013110: 3d77 7269 7465 5f6b 6170 7061 2c0a 2020  =write_kappa,.  
+00013120: 2020 2020 2020 2020 2020 2020 2020 7772                wr
+00013130: 6974 655f 7070 3d77 7269 7465 5f70 702c  ite_pp=write_pp,
+00013140: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00013150: 2072 6561 645f 7070 3d72 6561 645f 7070   read_pp=read_pp
+00013160: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+00013170: 2020 7772 6974 655f 6761 6d6d 615f 6465    write_gamma_de
+00013180: 7461 696c 3d77 7269 7465 5f67 616d 6d61  tail=write_gamma
+00013190: 5f64 6574 6169 6c2c 0a20 2020 2020 2020  _detail,.       
+000131a0: 2020 2020 2020 2020 2063 6f6d 7072 6573           compres
+000131b0: 7369 6f6e 3d63 6f6d 7072 6573 7369 6f6e  sion=compression
+000131c0: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+000131d0: 2020 696e 7075 745f 6669 6c65 6e61 6d65    input_filename
+000131e0: 3d69 6e70 7574 5f66 696c 656e 616d 652c  =input_filename,
+000131f0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00013200: 206f 7574 7075 745f 6669 6c65 6e61 6d65   output_filename
+00013210: 3d6f 7574 7075 745f 6669 6c65 6e61 6d65  =output_filename
+00013220: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+00013230: 2020 6c6f 675f 6c65 7665 6c3d 7365 6c66    log_level=self
+00013240: 2e5f 6c6f 675f 6c65 7665 6c2c 0a20 2020  ._log_level,.   
+00013250: 2020 2020 2020 2020 2029 0a0a 2020 2020           )..    
+00013260: 6465 6620 7361 7665 2873 656c 662c 2066  def save(self, f
+00013270: 696c 656e 616d 653d 2270 686f 6e6f 3370  ilename="phono3p
+00013280: 795f 7061 7261 6d73 2e79 616d 6c22 2c20  y_params.yaml", 
+00013290: 7365 7474 696e 6773 3d4e 6f6e 6529 3a0a  settings=None):.
+000132a0: 2020 2020 2020 2020 2222 2253 6176 6520          """Save 
+000132b0: 7061 7261 6d65 7465 7273 2069 6e20 5068  parameters in Ph
+000132c0: 6f6e 6f33 7079 2069 6e73 7461 6e74 7320  ono3py instants 
+000132d0: 696e 746f 2066 696c 652e 0a0a 2020 2020  into file...    
+000132e0: 2020 2020 5061 7261 6d65 7465 7273 0a20      Parameters. 
+000132f0: 2020 2020 2020 202d 2d2d 2d2d 2d2d 2d2d         ---------
+00013300: 2d0a 2020 2020 2020 2020 6669 6c65 6e61  -.        filena
+00013310: 6d65 3a20 7374 722c 206f 7074 696f 6e61  me: str, optiona
+00013320: 6c0a 2020 2020 2020 2020 2020 2020 4669  l.            Fi
+00013330: 6c65 206e 616d 652e 2044 6566 6175 6c74  le name. Default
+00013340: 2069 7320 2270 686f 6e6f 3370 795f 7061   is "phono3py_pa
+00013350: 7261 6d73 2e79 616d 6c22 0a20 2020 2020  rams.yaml".     
+00013360: 2020 2073 6574 7469 6e67 733a 2064 6963     settings: dic
+00013370: 742c 206f 7074 696f 6e61 6c0a 2020 2020  t, optional.    
+00013380: 2020 2020 2020 2020 4974 2069 7320 6465          It is de
+00013390: 7363 7269 6265 6420 7768 6963 6820 7061  scribed which pa
+000133a0: 7261 6d65 7465 7273 2061 7265 2077 7269  rameters are wri
+000133b0: 7474 656e 206f 7574 2e20 4f6e 6c79 0a20  tten out. Only. 
+000133c0: 2020 2020 2020 2020 2020 2074 6865 2073             the s
+000133d0: 6574 7469 6e67 7320 6578 7065 6374 6564  ettings expected
+000133e0: 2074 6f20 6265 2075 7064 6174 6564 2066   to be updated f
+000133f0: 726f 6d20 7468 6520 666f 6c6c 6f77 696e  rom the followin
+00013400: 670a 2020 2020 2020 2020 2020 2020 6465  g.            de
+00013410: 6661 756c 7420 7365 7474 696e 6773 2061  fault settings a
+00013420: 7265 206e 6565 6465 6420 746f 2062 6520  re needed to be 
+00013430: 7365 7420 696e 2074 6865 2064 6963 7469  set in the dicti
+00013440: 6f6e 6172 792e 0a20 2020 2020 2020 2020  onary..         
+00013450: 2020 2054 6865 2070 6f73 7369 626c 6520     The possible 
+00013460: 7061 7261 6d65 7465 7273 2061 6e64 2074  parameters and t
+00013470: 6865 6972 2064 6566 6175 6c74 2073 6574  heir default set
+00013480: 7469 6e67 7320 6172 653a 0a20 2020 2020  tings are:.     
+00013490: 2020 2020 2020 2020 2020 207b 2766 6f72             {'for
+000134a0: 6365 5f73 6574 7327 3a20 4661 6c73 652c  ce_sets': False,
+000134b0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000134c0: 2020 2764 6973 706c 6163 656d 656e 7473    'displacements
+000134d0: 273a 2054 7275 652c 0a20 2020 2020 2020  ': True,.       
+000134e0: 2020 2020 2020 2020 2020 2766 6f72 6365            'force
+000134f0: 5f63 6f6e 7374 616e 7473 273a 2046 616c  _constants': Fal
+00013500: 7365 2c0a 2020 2020 2020 2020 2020 2020  se,.            
+00013510: 2020 2020 2027 626f 726e 5f65 6666 6563       'born_effec
+00013520: 7469 7665 5f63 6861 7267 6527 3a20 5472  tive_charge': Tr
+00013530: 7565 2c0a 2020 2020 2020 2020 2020 2020  ue,.            
+00013540: 2020 2020 2027 6469 656c 6563 7472 6963       'dielectric
+00013550: 5f63 6f6e 7374 616e 7427 3a20 5472 7565  _constant': True
+00013560: 7d0a 0a20 2020 2020 2020 2022 2222 0a20  }..        """. 
+00013570: 2020 2020 2020 2070 6833 7079 5f79 616d         ph3py_yam
+00013580: 6c20 3d20 5068 6f6e 6f33 7079 5961 6d6c  l = Phono3pyYaml
+00013590: 2873 6574 7469 6e67 733d 7365 7474 696e  (settings=settin
+000135a0: 6773 290a 2020 2020 2020 2020 7068 3370  gs).        ph3p
+000135b0: 795f 7961 6d6c 2e73 6574 5f70 686f 6e6f  y_yaml.set_phono
+000135c0: 6e5f 696e 666f 2873 656c 6629 0a20 2020  n_info(self).   
+000135d0: 2020 2020 2077 6974 6820 6f70 656e 2866       with open(f
+000135e0: 696c 656e 616d 652c 2022 7722 2920 6173  ilename, "w") as
+000135f0: 2077 3a0a 2020 2020 2020 2020 2020 2020   w:.            
+00013600: 772e 7772 6974 6528 7374 7228 7068 3370  w.write(str(ph3p
+00013610: 795f 7961 6d6c 2929 0a0a 2020 2020 2323  y_yaml))..    ##
+00013620: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+00013630: 230a 2020 2020 2320 7072 6976 6174 6520  #.    # private 
+00013640: 6d65 7468 6f64 7320 230a 2020 2020 2323  methods #.    ##
+00013650: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+00013660: 230a 2020 2020 6465 6620 5f73 6561 7263  #.    def _searc
+00013670: 685f 7379 6d6d 6574 7279 2873 656c 6629  h_symmetry(self)
+00013680: 3a0a 2020 2020 2020 2020 7365 6c66 2e5f  :.        self._
+00013690: 7379 6d6d 6574 7279 203d 2053 796d 6d65  symmetry = Symme
+000136a0: 7472 7928 7365 6c66 2e5f 7375 7065 7263  try(self._superc
+000136b0: 656c 6c2c 2073 656c 662e 5f73 796d 7072  ell, self._sympr
+000136c0: 6563 2c20 7365 6c66 2e5f 6973 5f73 796d  ec, self._is_sym
+000136d0: 6d65 7472 7929 0a0a 2020 2020 6465 6620  metry)..    def 
+000136e0: 5f73 6561 7263 685f 7072 696d 6974 6976  _search_primitiv
+000136f0: 655f 7379 6d6d 6574 7279 2873 656c 6629  e_symmetry(self)
+00013700: 3a0a 2020 2020 2020 2020 7365 6c66 2e5f  :.        self._
+00013710: 7072 696d 6974 6976 655f 7379 6d6d 6574  primitive_symmet
+00013720: 7279 203d 2053 796d 6d65 7472 7928 0a20  ry = Symmetry(. 
+00013730: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+00013740: 5f70 7269 6d69 7469 7665 2c20 7365 6c66  _primitive, self
+00013750: 2e5f 7379 6d70 7265 632c 2073 656c 662e  ._symprec, self.
+00013760: 5f69 735f 7379 6d6d 6574 7279 0a20 2020  _is_symmetry.   
+00013770: 2020 2020 2029 0a20 2020 2020 2020 2069       ).        i
+00013780: 6620 6c65 6e28 7365 6c66 2e5f 7379 6d6d  f len(self._symm
+00013790: 6574 7279 2e70 6f69 6e74 6772 6f75 705f  etry.pointgroup_
+000137a0: 6f70 6572 6174 696f 6e73 2920 213d 206c  operations) != l
+000137b0: 656e 280a 2020 2020 2020 2020 2020 2020  en(.            
+000137c0: 7365 6c66 2e5f 7072 696d 6974 6976 655f  self._primitive_
+000137d0: 7379 6d6d 6574 7279 2e70 6f69 6e74 6772  symmetry.pointgr
+000137e0: 6f75 705f 6f70 6572 6174 696f 6e73 0a20  oup_operations. 
+000137f0: 2020 2020 2020 2029 3a20 2023 206e 6f71         ):  # noq
+00013800: 6120 4531 3239 0a20 2020 2020 2020 2020  a E129.         
+00013810: 2020 2070 7269 6e74 280a 2020 2020 2020     print(.      
+00013820: 2020 2020 2020 2020 2020 2257 6172 6e69            "Warni
+00013830: 6e67 3a20 706f 696e 7420 6772 6f75 7020  ng: point group 
+00013840: 7379 6d6d 6574 7269 6573 206f 6620 7375  symmetries of su
+00013850: 7065 7263 656c 6c20 616e 6420 7072 696d  percell and prim
+00013860: 6974 6976 6522 0a20 2020 2020 2020 2020  itive".         
+00013870: 2020 2020 2020 2022 6365 6c6c 2061 7265         "cell are
+00013880: 2064 6966 6665 7265 6e74 2e22 0a20 2020   different.".   
+00013890: 2020 2020 2020 2020 2029 0a0a 2020 2020           )..    
+000138a0: 6465 6620 5f73 6561 7263 685f 7068 6f6e  def _search_phon
+000138b0: 6f6e 5f73 7570 6572 6365 6c6c 5f73 796d  on_supercell_sym
+000138c0: 6d65 7472 7928 7365 6c66 293a 0a20 2020  metry(self):.   
+000138d0: 2020 2020 2069 6620 7365 6c66 2e5f 7068       if self._ph
+000138e0: 6f6e 6f6e 5f73 7570 6572 6365 6c6c 5f6d  onon_supercell_m
+000138f0: 6174 7269 7820 6973 204e 6f6e 653a 0a20  atrix is None:. 
+00013900: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+00013910: 5f70 686f 6e6f 6e5f 7375 7065 7263 656c  _phonon_supercel
+00013920: 6c5f 7379 6d6d 6574 7279 203d 2073 656c  l_symmetry = sel
+00013930: 662e 5f73 796d 6d65 7472 790a 2020 2020  f._symmetry.    
+00013940: 2020 2020 656c 7365 3a0a 2020 2020 2020      else:.      
+00013950: 2020 2020 2020 7365 6c66 2e5f 7068 6f6e        self._phon
+00013960: 6f6e 5f73 7570 6572 6365 6c6c 5f73 796d  on_supercell_sym
+00013970: 6d65 7472 7920 3d20 5379 6d6d 6574 7279  metry = Symmetry
+00013980: 280a 2020 2020 2020 2020 2020 2020 2020  (.              
+00013990: 2020 7365 6c66 2e5f 7068 6f6e 6f6e 5f73    self._phonon_s
+000139a0: 7570 6572 6365 6c6c 2c20 7365 6c66 2e5f  upercell, self._
+000139b0: 7379 6d70 7265 632c 2073 656c 662e 5f69  symprec, self._i
+000139c0: 735f 7379 6d6d 6574 7279 0a20 2020 2020  s_symmetry.     
+000139d0: 2020 2020 2020 2029 0a0a 2020 2020 6465         )..    de
+000139e0: 6620 5f62 7569 6c64 5f73 7570 6572 6365  f _build_superce
+000139f0: 6c6c 2873 656c 6629 3a0a 2020 2020 2020  ll(self):.      
+00013a00: 2020 7365 6c66 2e5f 7375 7065 7263 656c    self._supercel
+00013a10: 6c20 3d20 6765 745f 7375 7065 7263 656c  l = get_supercel
+00013a20: 6c28 0a20 2020 2020 2020 2020 2020 2073  l(.            s
+00013a30: 656c 662e 5f75 6e69 7463 656c 6c2c 2073  elf._unitcell, s
+00013a40: 656c 662e 5f73 7570 6572 6365 6c6c 5f6d  elf._supercell_m
+00013a50: 6174 7269 782c 2073 656c 662e 5f73 796d  atrix, self._sym
+00013a60: 7072 6563 0a20 2020 2020 2020 2029 0a0a  prec.        )..
+00013a70: 2020 2020 6465 6620 5f62 7569 6c64 5f70      def _build_p
+00013a80: 7269 6d69 7469 7665 5f63 656c 6c28 7365  rimitive_cell(se
+00013a90: 6c66 293a 0a20 2020 2020 2020 2022 2222  lf):.        """
+00013aa0: 4372 6561 7465 2070 7269 6d69 7469 7665  Create primitive
+00013ab0: 2063 656c 6c2e 0a0a 2020 2020 2020 2020   cell...        
+00013ac0: 7072 696d 6974 6976 655f 6d61 7472 6978  primitive_matrix
+00013ad0: 3a0a 2020 2020 2020 2020 2020 5265 6c61  :.          Rela
+00013ae0: 7469 7665 2061 7865 7320 6f66 2070 7269  tive axes of pri
+00013af0: 6d69 7469 7665 2063 656c 6c20 746f 2074  mitive cell to t
+00013b00: 6865 2069 6e70 7574 2075 6e69 7420 6365  he input unit ce
+00013b10: 6c6c 2e0a 2020 2020 2020 2020 2020 5265  ll..          Re
+00013b20: 6c61 7469 7665 2061 7865 7320 746f 2074  lative axes to t
+00013b30: 6865 2073 7570 6572 6365 6c6c 2069 7320  he supercell is 
+00013b40: 6361 6c63 756c 6174 6564 2062 793a 0a20  calculated by:. 
+00013b50: 2020 2020 2020 2020 2020 2020 7375 7065              supe
+00013b60: 7263 656c 6c5f 6d61 7472 6978 5e2d 3120  rcell_matrix^-1 
+00013b70: 2a20 7072 696d 6974 6976 655f 6d61 7472  * primitive_matr
+00013b80: 6978 0a20 2020 2020 2020 2020 2054 6865  ix.          The
+00013b90: 7265 666f 7265 2070 7269 6d69 7469 7665  refore primitive
+00013ba0: 2063 656c 6c20 6c61 7474 6963 6520 6973   cell lattice is
+00013bb0: 2066 696e 616c 6c79 2063 616c 6375 6c61   finally calcula
+00013bc0: 7465 6420 6279 3a0a 2020 2020 2020 2020  ted by:.        
+00013bd0: 2020 2020 2028 7375 7065 7263 656c 6c5f       (supercell_
+00013be0: 6c61 7474 6963 6520 2a20 2873 7570 6572  lattice * (super
+00013bf0: 6365 6c6c 5f6d 6174 7269 7829 5e2d 3120  cell_matrix)^-1 
+00013c00: 2a20 7072 696d 6974 6976 655f 6d61 7472  * primitive_matr
+00013c10: 6978 295e 540a 0a20 2020 2020 2020 2022  ix)^T..        "
+00013c20: 2222 0a20 2020 2020 2020 2073 656c 662e  "".        self.
+00013c30: 5f70 7269 6d69 7469 7665 203d 2073 656c  _primitive = sel
+00013c40: 662e 5f67 6574 5f70 7269 6d69 7469 7665  f._get_primitive
+00013c50: 5f63 656c 6c28 0a20 2020 2020 2020 2020  _cell(.         
+00013c60: 2020 2073 656c 662e 5f73 7570 6572 6365     self._superce
+00013c70: 6c6c 2c20 7365 6c66 2e5f 7375 7065 7263  ll, self._superc
+00013c80: 656c 6c5f 6d61 7472 6978 2c20 7365 6c66  ell_matrix, self
+00013c90: 2e5f 7072 696d 6974 6976 655f 6d61 7472  ._primitive_matr
+00013ca0: 6978 0a20 2020 2020 2020 2029 0a0a 2020  ix.        )..  
+00013cb0: 2020 6465 6620 5f62 7569 6c64 5f70 686f    def _build_pho
+00013cc0: 6e6f 6e5f 7375 7065 7263 656c 6c28 7365  non_supercell(se
+00013cd0: 6c66 293a 0a20 2020 2020 2020 2022 2222  lf):.        """
+00013ce0: 4372 6561 7465 2070 686f 6e6f 6e20 7375  Create phonon su
+00013cf0: 7065 7263 656c 6c20 666f 7220 6663 322e  percell for fc2.
+00013d00: 0a0a 2020 2020 2020 2020 7068 6f6e 6f6e  ..        phonon
+00013d10: 5f73 7570 6572 6365 6c6c 3a0a 2020 2020  _supercell:.    
+00013d20: 2020 2020 2020 5468 6973 2073 7570 6572        This super
+00013d30: 6365 6c6c 2069 7320 7573 6564 2066 6f72  cell is used for
+00013d40: 2068 6172 6d6f 6e69 6320 7068 6f6e 6f6e   harmonic phonon
+00013d50: 7320 2866 7265 7175 656e 6369 6573 2c0a  s (frequencies,.
+00013d60: 2020 2020 2020 2020 2020 6569 6765 6e76            eigenv
+00013d70: 6563 746f 7273 2c20 6772 6f75 7020 7665  ectors, group ve
+00013d80: 6c6f 6369 7469 6573 2c20 2e2e 2e29 0a20  locities, ...). 
+00013d90: 2020 2020 2020 2070 686f 6e6f 6e5f 7375         phonon_su
+00013da0: 7065 7263 656c 6c5f 6d61 7472 6978 3a0a  percell_matrix:.
+00013db0: 2020 2020 2020 2020 2020 4469 6666 6572            Differ
+00013dc0: 656e 7420 7375 7065 7263 656c 6c20 7369  ent supercell si
+00013dd0: 7a65 2063 616e 2062 6520 7370 6563 6966  ze can be specif
+00013de0: 6965 642e 0a0a 2020 2020 2020 2020 2222  ied...        ""
+00013df0: 220a 2020 2020 2020 2020 6966 2073 656c  ".        if sel
+00013e00: 662e 5f70 686f 6e6f 6e5f 7375 7065 7263  f._phonon_superc
+00013e10: 656c 6c5f 6d61 7472 6978 2069 7320 4e6f  ell_matrix is No
+00013e20: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
+00013e30: 7365 6c66 2e5f 7068 6f6e 6f6e 5f73 7570  self._phonon_sup
+00013e40: 6572 6365 6c6c 203d 2073 656c 662e 5f73  ercell = self._s
+00013e50: 7570 6572 6365 6c6c 0a20 2020 2020 2020  upercell.       
+00013e60: 2065 6c73 653a 0a20 2020 2020 2020 2020   else:.         
+00013e70: 2020 2073 656c 662e 5f70 686f 6e6f 6e5f     self._phonon_
+00013e80: 7375 7065 7263 656c 6c20 3d20 6765 745f  supercell = get_
+00013e90: 7375 7065 7263 656c 6c28 0a20 2020 2020  supercell(.     
+00013ea0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+00013eb0: 5f75 6e69 7463 656c 6c2c 2073 656c 662e  _unitcell, self.
+00013ec0: 5f70 686f 6e6f 6e5f 7375 7065 7263 656c  _phonon_supercel
+00013ed0: 6c5f 6d61 7472 6978 2c20 7365 6c66 2e5f  l_matrix, self._
+00013ee0: 7379 6d70 7265 630a 2020 2020 2020 2020  symprec.        
+00013ef0: 2020 2020 290a 0a20 2020 2064 6566 205f      )..    def _
+00013f00: 6275 696c 645f 7068 6f6e 6f6e 5f70 7269  build_phonon_pri
+00013f10: 6d69 7469 7665 5f63 656c 6c28 7365 6c66  mitive_cell(self
+00013f20: 293a 0a20 2020 2020 2020 2069 6620 7365  ):.        if se
+00013f30: 6c66 2e5f 7068 6f6e 6f6e 5f73 7570 6572  lf._phonon_super
+00013f40: 6365 6c6c 5f6d 6174 7269 7820 6973 204e  cell_matrix is N
+00013f50: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
+00013f60: 2073 656c 662e 5f70 686f 6e6f 6e5f 7072   self._phonon_pr
+00013f70: 696d 6974 6976 6520 3d20 7365 6c66 2e5f  imitive = self._
+00013f80: 7072 696d 6974 6976 650a 2020 2020 2020  primitive.      
+00013f90: 2020 656c 7365 3a0a 2020 2020 2020 2020    else:.        
+00013fa0: 2020 2020 7365 6c66 2e5f 7068 6f6e 6f6e      self._phonon
+00013fb0: 5f70 7269 6d69 7469 7665 203d 2073 656c  _primitive = sel
+00013fc0: 662e 5f67 6574 5f70 7269 6d69 7469 7665  f._get_primitive
+00013fd0: 5f63 656c 6c28 0a20 2020 2020 2020 2020  _cell(.         
+00013fe0: 2020 2020 2020 2073 656c 662e 5f70 686f         self._pho
+00013ff0: 6e6f 6e5f 7375 7065 7263 656c 6c2c 0a20  non_supercell,. 
+00014000: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+00014010: 656c 662e 5f70 686f 6e6f 6e5f 7375 7065  elf._phonon_supe
+00014020: 7263 656c 6c5f 6d61 7472 6978 2c0a 2020  rcell_matrix,.  
+00014030: 2020 2020 2020 2020 2020 2020 2020 7365                se
+00014040: 6c66 2e5f 7072 696d 6974 6976 655f 6d61  lf._primitive_ma
+00014050: 7472 6978 2c0a 2020 2020 2020 2020 2020  trix,.          
+00014060: 2020 290a 2020 2020 2020 2020 2020 2020    ).            
+00014070: 6966 2028 0a20 2020 2020 2020 2020 2020  if (.           
+00014080: 2020 2020 2073 656c 662e 5f70 7269 6d69       self._primi
+00014090: 7469 7665 2069 7320 6e6f 7420 4e6f 6e65  tive is not None
+000140a0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000140b0: 2061 6e64 2028 7365 6c66 2e5f 7072 696d   and (self._prim
+000140c0: 6974 6976 652e 6e75 6d62 6572 7320 213d  itive.numbers !=
+000140d0: 2073 656c 662e 5f70 686f 6e6f 6e5f 7072   self._phonon_pr
+000140e0: 696d 6974 6976 652e 6e75 6d62 6572 7329  imitive.numbers)
+000140f0: 2e61 6e79 2829 0a20 2020 2020 2020 2020  .any().         
+00014100: 2020 2029 3a0a 2020 2020 2020 2020 2020     ):.          
+00014110: 2020 2020 2020 7072 696e 7428 2220 5072        print(" Pr
+00014120: 696d 6974 6976 6520 6365 6c6c 7320 666f  imitive cells fo
+00014130: 7220 6663 3220 616e 6420 6663 3320 6361  r fc2 and fc3 ca
+00014140: 6e20 6265 2064 6966 6665 7265 6e74 2e22  n be different."
+00014150: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
+00014160: 2020 7261 6973 6520 5275 6e74 696d 6545    raise RuntimeE
+00014170: 7272 6f72 0a0a 2020 2020 6465 6620 5f62  rror..    def _b
+00014180: 7569 6c64 5f70 686f 6e6f 6e5f 7375 7065  uild_phonon_supe
+00014190: 7263 656c 6c73 5f77 6974 685f 6469 7370  rcells_with_disp
+000141a0: 6c61 6365 6d65 6e74 7328 0a20 2020 2020  lacements(.     
+000141b0: 2020 2073 656c 662c 2073 7570 6572 6365     self, superce
+000141c0: 6c6c 3a20 5068 6f6e 6f70 7941 746f 6d73  ll: PhonopyAtoms
+000141d0: 2c20 6469 7370 6c61 6365 6d65 6e74 5f64  , displacement_d
+000141e0: 6174 6173 6574 0a20 2020 2029 3a0a 2020  ataset.    ):.  
+000141f0: 2020 2020 2020 7375 7065 7263 656c 6c73        supercells
+00014200: 203d 205b 5d0a 2020 2020 2020 2020 6d61   = [].        ma
+00014210: 676d 6f6d 7320 3d20 7375 7065 7263 656c  gmoms = supercel
+00014220: 6c2e 6d61 676e 6574 6963 5f6d 6f6d 656e  l.magnetic_momen
+00014230: 7473 0a20 2020 2020 2020 206d 6173 7365  ts.        masse
+00014240: 7320 3d20 7375 7065 7263 656c 6c2e 6d61  s = supercell.ma
+00014250: 7373 6573 0a20 2020 2020 2020 206e 756d  sses.        num
+00014260: 6265 7273 203d 2073 7570 6572 6365 6c6c  bers = supercell
+00014270: 2e6e 756d 6265 7273 0a20 2020 2020 2020  .numbers.       
+00014280: 206c 6174 7469 6365 203d 2073 7570 6572   lattice = super
+00014290: 6365 6c6c 2e63 656c 6c0a 0a20 2020 2020  cell.cell..     
+000142a0: 2020 2066 6f72 2064 6973 7031 2069 6e20     for disp1 in 
+000142b0: 6469 7370 6c61 6365 6d65 6e74 5f64 6174  displacement_dat
+000142c0: 6173 6574 5b22 6669 7273 745f 6174 6f6d  aset["first_atom
+000142d0: 7322 5d3a 0a20 2020 2020 2020 2020 2020  s"]:.           
+000142e0: 2064 6973 705f 6361 7274 3120 3d20 6469   disp_cart1 = di
+000142f0: 7370 315b 2264 6973 706c 6163 656d 656e  sp1["displacemen
+00014300: 7422 5d0a 2020 2020 2020 2020 2020 2020  t"].            
+00014310: 706f 7369 7469 6f6e 7320 3d20 7375 7065  positions = supe
+00014320: 7263 656c 6c2e 706f 7369 7469 6f6e 730a  rcell.positions.
+00014330: 2020 2020 2020 2020 2020 2020 706f 7369              posi
+00014340: 7469 6f6e 735b 6469 7370 315b 226e 756d  tions[disp1["num
+00014350: 6265 7222 5d5d 202b 3d20 6469 7370 5f63  ber"]] += disp_c
+00014360: 6172 7431 0a20 2020 2020 2020 2020 2020  art1.           
+00014370: 2073 7570 6572 6365 6c6c 732e 6170 7065   supercells.appe
+00014380: 6e64 280a 2020 2020 2020 2020 2020 2020  nd(.            
+00014390: 2020 2020 5068 6f6e 6f70 7941 746f 6d73      PhonopyAtoms
+000143a0: 280a 2020 2020 2020 2020 2020 2020 2020  (.              
+000143b0: 2020 2020 2020 6e75 6d62 6572 733d 6e75        numbers=nu
+000143c0: 6d62 6572 732c 0a20 2020 2020 2020 2020  mbers,.         
+000143d0: 2020 2020 2020 2020 2020 206d 6173 7365             masse
+000143e0: 733d 6d61 7373 6573 2c0a 2020 2020 2020  s=masses,.      
+000143f0: 2020 2020 2020 2020 2020 2020 2020 6d61                ma
+00014400: 676e 6574 6963 5f6d 6f6d 656e 7473 3d6d  gnetic_moments=m
+00014410: 6167 6d6f 6d73 2c0a 2020 2020 2020 2020  agmoms,.        
+00014420: 2020 2020 2020 2020 2020 2020 706f 7369              posi
+00014430: 7469 6f6e 733d 706f 7369 7469 6f6e 732c  tions=positions,
+00014440: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00014450: 2020 2020 2063 656c 6c3d 6c61 7474 6963       cell=lattic
+00014460: 652c 0a20 2020 2020 2020 2020 2020 2020  e,.             
+00014470: 2020 2029 0a20 2020 2020 2020 2020 2020     ).           
+00014480: 2029 0a0a 2020 2020 2020 2020 7265 7475   )..        retu
+00014490: 726e 2073 7570 6572 6365 6c6c 730a 0a20  rn supercells.. 
+000144a0: 2020 2064 6566 205f 6275 696c 645f 7375     def _build_su
+000144b0: 7065 7263 656c 6c73 5f77 6974 685f 6469  percells_with_di
+000144c0: 7370 6c61 6365 6d65 6e74 7328 7365 6c66  splacements(self
+000144d0: 293a 0a20 2020 2020 2020 2073 7570 6572  ):.        super
+000144e0: 6365 6c6c 7320 3d20 5b5d 0a20 2020 2020  cells = [].     
+000144f0: 2020 206d 6167 6d6f 6d73 203d 2073 656c     magmoms = sel
+00014500: 662e 5f73 7570 6572 6365 6c6c 2e6d 6167  f._supercell.mag
+00014510: 6e65 7469 635f 6d6f 6d65 6e74 730a 2020  netic_moments.  
+00014520: 2020 2020 2020 6d61 7373 6573 203d 2073        masses = s
+00014530: 656c 662e 5f73 7570 6572 6365 6c6c 2e6d  elf._supercell.m
+00014540: 6173 7365 730a 2020 2020 2020 2020 6e75  asses.        nu
+00014550: 6d62 6572 7320 3d20 7365 6c66 2e5f 7375  mbers = self._su
+00014560: 7065 7263 656c 6c2e 6e75 6d62 6572 730a  percell.numbers.
+00014570: 2020 2020 2020 2020 6c61 7474 6963 6520          lattice 
+00014580: 3d20 7365 6c66 2e5f 7375 7065 7263 656c  = self._supercel
+00014590: 6c2e 6365 6c6c 0a0a 2020 2020 2020 2020  l.cell..        
+000145a0: 7375 7065 7263 656c 6c73 203d 2073 656c  supercells = sel
+000145b0: 662e 5f62 7569 6c64 5f70 686f 6e6f 6e5f  f._build_phonon_
+000145c0: 7375 7065 7263 656c 6c73 5f77 6974 685f  supercells_with_
+000145d0: 6469 7370 6c61 6365 6d65 6e74 7328 0a20  displacements(. 
+000145e0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+000145f0: 5f73 7570 6572 6365 6c6c 2c20 7365 6c66  _supercell, self
+00014600: 2e5f 6461 7461 7365 740a 2020 2020 2020  ._dataset.      
+00014610: 2020 290a 0a20 2020 2020 2020 2066 6f72    )..        for
+00014620: 2064 6973 7031 2069 6e20 7365 6c66 2e5f   disp1 in self._
+00014630: 6461 7461 7365 745b 2266 6972 7374 5f61  dataset["first_a
+00014640: 746f 6d73 225d 3a0a 2020 2020 2020 2020  toms"]:.        
+00014650: 2020 2020 6469 7370 5f63 6172 7431 203d      disp_cart1 =
+00014660: 2064 6973 7031 5b22 6469 7370 6c61 6365   disp1["displace
+00014670: 6d65 6e74 225d 0a20 2020 2020 2020 2020  ment"].         
+00014680: 2020 2066 6f72 2064 6973 7032 2069 6e20     for disp2 in 
+00014690: 6469 7370 315b 2273 6563 6f6e 645f 6174  disp1["second_at
+000146a0: 6f6d 7322 5d3a 0a20 2020 2020 2020 2020  oms"]:.         
+000146b0: 2020 2020 2020 2069 6620 2269 6e63 6c75         if "inclu
+000146c0: 6465 6422 2069 6e20 6469 7370 323a 0a20  ded" in disp2:. 
 000146d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000146e0: 2020 2020 2020 2020 2020 2020 6d61 676e              magn
-000146f0: 6574 6963 5f6d 6f6d 656e 7473 3d6d 6167  etic_moments=mag
-00014700: 6d6f 6d73 2c0a 2020 2020 2020 2020 2020  moms,.          
-00014710: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014720: 2020 706f 7369 7469 6f6e 733d 706f 7369    positions=posi
-00014730: 7469 6f6e 732c 0a20 2020 2020 2020 2020  tions,.         
-00014740: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014750: 2020 2063 656c 6c3d 6c61 7474 6963 652c     cell=lattice,
-00014760: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00014770: 2020 2020 2020 2020 2029 0a20 2020 2020           ).     
-00014780: 2020 2020 2020 2020 2020 2020 2020 2029                 )
+000146e0: 2020 2069 6e63 6c75 6465 6420 3d20 6469     included = di
+000146f0: 7370 325b 2269 6e63 6c75 6465 6422 5d0a  sp2["included"].
+00014700: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00014710: 656c 7365 3a0a 2020 2020 2020 2020 2020  else:.          
+00014720: 2020 2020 2020 2020 2020 696e 636c 7564            includ
+00014730: 6564 203d 2054 7275 650a 2020 2020 2020  ed = True.      
+00014740: 2020 2020 2020 2020 2020 6966 2069 6e63            if inc
+00014750: 6c75 6465 643a 0a20 2020 2020 2020 2020  luded:.         
+00014760: 2020 2020 2020 2020 2020 2070 6f73 6974             posit
+00014770: 696f 6e73 203d 2073 656c 662e 5f73 7570  ions = self._sup
+00014780: 6572 6365 6c6c 2e70 6f73 6974 696f 6e73  ercell.positions
 00014790: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000147a0: 2065 6c73 653a 0a20 2020 2020 2020 2020   else:.         
-000147b0: 2020 2020 2020 2020 2020 2073 7570 6572             super
-000147c0: 6365 6c6c 732e 6170 7065 6e64 284e 6f6e  cells.append(Non
-000147d0: 6529 0a0a 2020 2020 2020 2020 7365 6c66  e)..        self
-000147e0: 2e5f 7375 7065 7263 656c 6c73 5f77 6974  ._supercells_wit
-000147f0: 685f 6469 7370 6c61 6365 6d65 6e74 7320  h_displacements 
-00014800: 3d20 7375 7065 7263 656c 6c73 0a0a 2020  = supercells..  
-00014810: 2020 6465 6620 5f67 6574 5f70 7269 6d69    def _get_primi
-00014820: 7469 7665 5f63 656c 6c28 7365 6c66 2c20  tive_cell(self, 
-00014830: 7375 7065 7263 656c 6c2c 2073 7570 6572  supercell, super
-00014840: 6365 6c6c 5f6d 6174 7269 782c 2070 7269  cell_matrix, pri
-00014850: 6d69 7469 7665 5f6d 6174 7269 7829 3a0a  mitive_matrix):.
-00014860: 2020 2020 2020 2020 696e 765f 7375 7065          inv_supe
-00014870: 7263 656c 6c5f 6d61 7472 6978 203d 206e  rcell_matrix = n
-00014880: 702e 6c69 6e61 6c67 2e69 6e76 2873 7570  p.linalg.inv(sup
-00014890: 6572 6365 6c6c 5f6d 6174 7269 7829 0a20  ercell_matrix). 
-000148a0: 2020 2020 2020 2069 6620 7072 696d 6974         if primit
-000148b0: 6976 655f 6d61 7472 6978 2069 7320 4e6f  ive_matrix is No
-000148c0: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
-000148d0: 745f 6d61 7420 3d20 696e 765f 7375 7065  t_mat = inv_supe
-000148e0: 7263 656c 6c5f 6d61 7472 6978 0a20 2020  rcell_matrix.   
-000148f0: 2020 2020 2065 6c73 653a 0a20 2020 2020       else:.     
-00014900: 2020 2020 2020 2074 5f6d 6174 203d 206e         t_mat = n
-00014910: 702e 646f 7428 696e 765f 7375 7065 7263  p.dot(inv_superc
-00014920: 656c 6c5f 6d61 7472 6978 2c20 7072 696d  ell_matrix, prim
-00014930: 6974 6976 655f 6d61 7472 6978 290a 0a20  itive_matrix).. 
-00014940: 2020 2020 2020 2072 6574 7572 6e20 6765         return ge
-00014950: 745f 7072 696d 6974 6976 6528 7375 7065  t_primitive(supe
-00014960: 7263 656c 6c2c 2074 5f6d 6174 2c20 7365  rcell, t_mat, se
-00014970: 6c66 2e5f 7379 6d70 7265 632c 2073 746f  lf._symprec, sto
-00014980: 7265 5f64 656e 7365 5f73 7665 6373 3d54  re_dense_svecs=T
-00014990: 7275 6529 0a0a 2020 2020 6465 6620 5f64  rue)..    def _d
-000149a0: 6574 6572 6d69 6e65 5f70 7269 6d69 7469  etermine_primiti
-000149b0: 7665 5f6d 6174 7269 7828 7365 6c66 2c20  ve_matrix(self, 
-000149c0: 7072 696d 6974 6976 655f 6d61 7472 6978  primitive_matrix
-000149d0: 293a 0a20 2020 2020 2020 2070 6d61 7420  ):.        pmat 
-000149e0: 3d20 6765 745f 7072 696d 6974 6976 655f  = get_primitive_
-000149f0: 6d61 7472 6978 2870 7269 6d69 7469 7665  matrix(primitive
-00014a00: 5f6d 6174 7269 782c 2073 796d 7072 6563  _matrix, symprec
-00014a10: 3d73 656c 662e 5f73 796d 7072 6563 290a  =self._symprec).
-00014a20: 2020 2020 2020 2020 6966 2069 7369 6e73          if isins
-00014a30: 7461 6e63 6528 706d 6174 2c20 7374 7229  tance(pmat, str)
-00014a40: 2061 6e64 2070 6d61 7420 3d3d 2022 6175   and pmat == "au
-00014a50: 746f 223a 0a20 2020 2020 2020 2020 2020  to":.           
-00014a60: 2072 6574 7572 6e20 6775 6573 735f 7072   return guess_pr
-00014a70: 696d 6974 6976 655f 6d61 7472 6978 2873  imitive_matrix(s
-00014a80: 656c 662e 5f75 6e69 7463 656c 6c2c 2073  elf._unitcell, s
-00014a90: 796d 7072 6563 3d73 656c 662e 5f73 796d  ymprec=self._sym
-00014aa0: 7072 6563 290a 2020 2020 2020 2020 656c  prec).        el
-00014ab0: 7365 3a0a 2020 2020 2020 2020 2020 2020  se:.            
-00014ac0: 7265 7475 726e 2070 6d61 740a 0a20 2020  return pmat..   
-00014ad0: 2064 6566 205f 7365 745f 6d65 7368 5f6e   def _set_mesh_n
-00014ae0: 756d 6265 7273 280a 2020 2020 2020 2020  umbers(.        
-00014af0: 7365 6c66 2c0a 2020 2020 2020 2020 6d65  self,.        me
-00014b00: 7368 3a20 556e 696f 6e5b 696e 742c 2066  sh: Union[int, f
-00014b10: 6c6f 6174 2c20 5365 7175 656e 6365 2c20  loat, Sequence, 
-00014b20: 6e70 2e6e 6461 7272 6179 5d2c 0a20 2020  np.ndarray],.   
-00014b30: 2029 3a0a 2020 2020 2020 2020 2320 696e   ):.        # in
-00014b40: 6974 6961 6c69 7a61 7469 6f6e 2072 656c  itialization rel
-00014b50: 6174 6564 2074 6f20 6d65 7368 0a20 2020  ated to mesh.   
-00014b60: 2020 2020 2073 656c 662e 5f69 6e74 6572       self._inter
-00014b70: 6163 7469 6f6e 203d 204e 6f6e 650a 0a20  action = None.. 
-00014b80: 2020 2020 2020 2073 656c 662e 5f62 7a5f         self._bz_
-00014b90: 6772 6964 203d 2042 5a47 7269 6428 0a20  grid = BZGrid(. 
-00014ba0: 2020 2020 2020 2020 2020 206d 6573 682c             mesh,
-00014bb0: 0a20 2020 2020 2020 2020 2020 206c 6174  .            lat
-00014bc0: 7469 6365 3d73 656c 662e 5f70 7269 6d69  tice=self._primi
-00014bd0: 7469 7665 2e63 656c 6c2c 0a20 2020 2020  tive.cell,.     
-00014be0: 2020 2020 2020 2073 796d 6d65 7472 795f         symmetry_
-00014bf0: 6461 7461 7365 743d 7365 6c66 2e5f 7072  dataset=self._pr
-00014c00: 696d 6974 6976 655f 7379 6d6d 6574 7279  imitive_symmetry
-00014c10: 2e64 6174 6173 6574 2c0a 2020 2020 2020  .dataset,.      
-00014c20: 2020 2020 2020 6973 5f74 696d 655f 7265        is_time_re
-00014c30: 7665 7273 616c 3d73 656c 662e 5f69 735f  versal=self._is_
-00014c40: 7379 6d6d 6574 7279 2c0a 2020 2020 2020  symmetry,.      
-00014c50: 2020 2020 2020 7573 655f 6772 673d 7365        use_grg=se
-00014c60: 6c66 2e5f 7573 655f 6772 672c 0a20 2020  lf._use_grg,.   
-00014c70: 2020 2020 2020 2020 2066 6f72 6365 5f53           force_S
-00014c80: 4e46 3d46 616c 7365 2c0a 2020 2020 2020  NF=False,.      
-00014c90: 2020 2020 2020 534e 465f 636f 6f72 6469        SNF_coordi
-00014ca0: 6e61 7465 733d 7365 6c66 2e5f 534e 465f  nates=self._SNF_
-00014cb0: 636f 6f72 6469 6e61 7465 732c 0a20 2020  coordinates,.   
-00014cc0: 2020 2020 2020 2020 2073 746f 7265 5f64           store_d
-00014cd0: 656e 7365 5f67 705f 6d61 703d 5472 7565  ense_gp_map=True
-00014ce0: 2c0a 2020 2020 2020 2020 290a 0a20 2020  ,.        )..   
-00014cf0: 2064 6566 205f 696e 6974 5f64 796e 616d   def _init_dynam
-00014d00: 6963 616c 5f6d 6174 7269 7828 7365 6c66  ical_matrix(self
-00014d10: 293a 0a20 2020 2020 2020 2069 6620 7365  ):.        if se
-00014d20: 6c66 2e5f 696e 7465 7261 6374 696f 6e20  lf._interaction 
-00014d30: 6973 204e 6f6e 653a 0a20 2020 2020 2020  is None:.       
-00014d40: 2020 2020 206d 7367 203d 2028 0a20 2020       msg = (.   
-00014d50: 2020 2020 2020 2020 2020 2020 2022 5068               "Ph
-00014d60: 6f6e 6f33 7079 2e69 6e69 745f 7068 7068  ono3py.init_phph
-00014d70: 5f69 6e74 6572 6163 7469 6f6e 2068 6173  _interaction has
-00014d80: 2074 6f20 6265 2063 616c 6c65 6420 220a   to be called ".
-00014d90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014da0: 2262 6566 6f72 6520 7275 6e6e 696e 6720  "before running 
-00014db0: 7468 6973 206d 6574 686f 642e 220a 2020  this method.".  
-00014dc0: 2020 2020 2020 2020 2020 290a 2020 2020            ).    
-00014dd0: 2020 2020 2020 2020 7261 6973 6520 5275          raise Ru
-00014de0: 6e74 696d 6545 7272 6f72 286d 7367 290a  ntimeError(msg).
-00014df0: 0a20 2020 2020 2020 2073 656c 662e 5f69  .        self._i
-00014e00: 6e74 6572 6163 7469 6f6e 2e69 6e69 745f  nteraction.init_
-00014e10: 6479 6e61 6d69 6361 6c5f 6d61 7472 6978  dynamical_matrix
-00014e20: 280a 2020 2020 2020 2020 2020 2020 7365  (.            se
-00014e30: 6c66 2e5f 6663 322c 0a20 2020 2020 2020  lf._fc2,.       
-00014e40: 2020 2020 2073 656c 662e 5f70 686f 6e6f       self._phono
-00014e50: 6e5f 7375 7065 7263 656c 6c2c 0a20 2020  n_supercell,.   
-00014e60: 2020 2020 2020 2020 2073 656c 662e 5f70           self._p
-00014e70: 686f 6e6f 6e5f 7072 696d 6974 6976 652c  honon_primitive,
-00014e80: 0a20 2020 2020 2020 2020 2020 206e 6163  .            nac
-00014e90: 5f70 6172 616d 733d 7365 6c66 2e5f 6e61  _params=self._na
-00014ea0: 635f 7061 7261 6d73 2c0a 2020 2020 2020  c_params,.      
-00014eb0: 2020 290a 2020 2020 2020 2020 6672 6571    ).        freq
-00014ec0: 732c 205f 2c20 5f20 3d20 7365 6c66 2e67  s, _, _ = self.g
-00014ed0: 6574 5f70 686f 6e6f 6e5f 6461 7461 2829  et_phonon_data()
-00014ee0: 0a20 2020 2020 2020 2067 705f 4761 6d6d  .        gp_Gamm
-00014ef0: 6120 3d20 7365 6c66 2e5f 627a 5f67 7269  a = self._bz_gri
-00014f00: 642e 6770 5f47 616d 6d61 0a20 2020 2020  d.gp_Gamma.     
-00014f10: 2020 2069 6620 6e70 2e73 756d 2866 7265     if np.sum(fre
-00014f20: 7173 5b67 705f 4761 6d6d 615d 203c 2073  qs[gp_Gamma] < s
-00014f30: 656c 662e 5f63 7574 6f66 665f 6672 6571  elf._cutoff_freq
-00014f40: 7565 6e63 7929 203c 2033 3a0a 2020 2020  uency) < 3:.    
-00014f50: 2020 2020 2020 2020 666f 7220 692c 2066          for i, f
-00014f60: 2069 6e20 656e 756d 6572 6174 6528 6672   in enumerate(fr
-00014f70: 6571 735b 6770 5f47 616d 6d61 2c20 3a33  eqs[gp_Gamma, :3
-00014f80: 5d29 3a0a 2020 2020 2020 2020 2020 2020  ]):.            
-00014f90: 2020 2020 6966 206e 6f74 2028 6620 3c20      if not (f < 
-00014fa0: 7365 6c66 2e5f 6375 746f 6666 5f66 7265  self._cutoff_fre
-00014fb0: 7175 656e 6379 293a 0a20 2020 2020 2020  quency):.       
-00014fc0: 2020 2020 2020 2020 2020 2020 2066 7265               fre
-00014fd0: 7173 5b67 705f 4761 6d6d 612c 2069 5d20  qs[gp_Gamma, i] 
-00014fe0: 3d20 300a 2020 2020 2020 2020 2020 2020  = 0.            
-00014ff0: 2020 2020 2020 2020 7072 696e 7428 223d          print("=
-00015000: 2220 2a20 3236 202b 2022 2057 6172 6e69  " * 26 + " Warni
-00015010: 6e67 2022 202b 2022 3d22 202a 2032 3629  ng " + "=" * 26)
-00015020: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00015030: 2020 2020 2070 7269 6e74 280a 2020 2020       print(.    
-00015040: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00015050: 2020 2020 2220 5068 6f6e 6f6e 2066 7265      " Phonon fre
-00015060: 7175 656e 6379 206f 6620 6261 6e64 2069  quency of band i
-00015070: 6e64 6578 2025 6420 6174 2047 616d 6d61  ndex %d at Gamma
-00015080: 2022 0a20 2020 2020 2020 2020 2020 2020   ".             
-00015090: 2020 2020 2020 2020 2020 2022 6973 2063             "is c
-000150a0: 616c 6375 6c61 7465 6420 746f 2062 6520  alculated to be 
-000150b0: 2566 2e22 2025 2028 6920 2b20 312c 2066  %f." % (i + 1, f
-000150c0: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
-000150d0: 2020 2020 2020 290a 2020 2020 2020 2020        ).        
-000150e0: 2020 2020 2020 2020 2020 2020 7072 696e              prin
-000150f0: 7428 2220 4275 7420 7468 6973 2066 7265  t(" But this fre
-00015100: 7175 656e 6379 2069 7320 666f 7263 6564  quency is forced
-00015110: 2074 6f20 6265 207a 6572 6f2e 2229 0a20   to be zero."). 
-00015120: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00015130: 2020 2070 7269 6e74 2822 3d22 202a 2036     print("=" * 6
-00015140: 3129 0a0a 2020 2020 6465 6620 5f65 7874  1)..    def _ext
-00015150: 7261 6374 5f66 6332 5f66 6333 5f63 616c  ract_fc2_fc3_cal
-00015160: 6375 6c61 746f 7273 2873 656c 662c 2066  culators(self, f
-00015170: 635f 6361 6c63 756c 6174 6f72 2c20 6663  c_calculator, fc
-00015180: 5f63 616c 6375 6c61 746f 725f 6f70 7469  _calculator_opti
-00015190: 6f6e 732c 206f 7264 6572 293a 0a20 2020  ons, order):.   
-000151a0: 2020 2020 2022 2222 4578 7472 6163 7420       """Extract 
-000151b0: 6663 5f63 616c 6375 6c61 746f 7220 616e  fc_calculator an
-000151c0: 6420 6663 5f63 616c 6375 6c61 746f 725f  d fc_calculator_
-000151d0: 6f70 7469 6f6e 7320 666f 7220 6663 3220  options for fc2 
-000151e0: 616e 6420 6663 332e 0a0a 2020 2020 2020  and fc3...      
-000151f0: 2020 6663 5f63 616c 6375 6c61 746f 7220    fc_calculator 
-00015200: 3a20 7374 720a 2020 2020 2020 2020 2020  : str.          
-00015210: 2020 4643 2063 616c 6375 6c61 746f 722e    FC calculator.
-00015220: 2022 7c22 2073 6570 6172 6174 6573 2066   "|" separates f
-00015230: 6332 2061 6e64 2066 6333 2e20 4669 7273  c2 and fc3. Firs
-00015240: 7420 616e 6420 6c61 7374 0a20 2020 2020  t and last.     
-00015250: 2020 2020 2020 2070 6172 7473 2073 6570         parts sep
-00015260: 6172 6174 6564 2063 6f72 7265 7370 6f6e  arated correspon
-00015270: 6420 746f 2066 6332 2061 6e64 2066 6333  d to fc2 and fc3
-00015280: 2063 616c 6375 6c61 746f 7273 2c20 7265   calculators, re
-00015290: 7370 6563 7469 7665 6c79 2e0a 2020 2020  spectively..    
-000152a0: 2020 2020 6663 5f63 616c 6375 6c61 746f      fc_calculato
-000152b0: 725f 6f70 7469 6f6e 7320 3a20 7374 720a  r_options : str.
-000152c0: 2020 2020 2020 2020 2020 2020 4643 2063              FC c
-000152d0: 616c 6375 6c61 746f 7220 6f70 7469 6f6e  alculator option
-000152e0: 732e 2022 7c22 2073 6570 6172 6174 6573  s. "|" separates
-000152f0: 2066 6332 2061 6e64 2066 6333 2e20 4669   fc2 and fc3. Fi
-00015300: 7273 7420 616e 6420 6c61 7374 0a20 2020  rst and last.   
-00015310: 2020 2020 2020 2020 2070 6172 7473 2073           parts s
-00015320: 6570 6172 6174 6564 2063 6f72 7265 7370  eparated corresp
-00015330: 6f6e 6420 746f 2066 6332 2061 6e64 2066  ond to fc2 and f
-00015340: 6333 206f 7074 696f 6e73 2c20 7265 7370  c3 options, resp
-00015350: 6563 7469 7665 6c79 2e0a 2020 2020 2020  ectively..      
-00015360: 2020 6f72 6465 7220 3a20 696e 7420 3d20    order : int = 
-00015370: 3220 6f72 2033 0a20 2020 2020 2020 2020  2 or 3.         
-00015380: 2020 2032 2061 6e64 2033 2069 6e64 6963     2 and 3 indic
-00015390: 6174 6520 6663 3220 616e 6420 6663 332c  ate fc2 and fc3,
-000153a0: 2072 6573 7065 6374 6976 656c 792e 0a0a   respectively...
-000153b0: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
-000153c0: 2020 2020 6966 2066 635f 6361 6c63 756c      if fc_calcul
-000153d0: 6174 6f72 2069 7320 6e6f 7420 4e6f 6e65  ator is not None
-000153e0: 3a0a 2020 2020 2020 2020 2020 2020 6966  :.            if
-000153f0: 2022 7c22 2069 6e20 6663 5f63 616c 6375   "|" in fc_calcu
-00015400: 6c61 746f 723a 0a20 2020 2020 2020 2020  lator:.         
-00015410: 2020 2020 2020 205f 6663 5f63 616c 6375         _fc_calcu
-00015420: 6c61 746f 7220 3d20 6663 5f63 616c 6375  lator = fc_calcu
-00015430: 6c61 746f 722e 7370 6c69 7428 227c 2229  lator.split("|")
-00015440: 5b6f 7264 6572 202d 2032 5d0a 2020 2020  [order - 2].    
-00015450: 2020 2020 2020 2020 2020 2020 6966 205f              if _
-00015460: 6663 5f63 616c 6375 6c61 746f 7220 3d3d  fc_calculator ==
-00015470: 2022 223a 0a20 2020 2020 2020 2020 2020   "":.           
-00015480: 2020 2020 2020 2020 205f 6663 5f63 616c           _fc_cal
-00015490: 6375 6c61 746f 7220 3d20 4e6f 6e65 0a20  culator = None. 
-000154a0: 2020 2020 2020 2020 2020 2065 6c73 653a             else:
-000154b0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000154c0: 205f 6663 5f63 616c 6375 6c61 746f 7220   _fc_calculator 
-000154d0: 3d20 6663 5f63 616c 6375 6c61 746f 720a  = fc_calculator.
-000154e0: 2020 2020 2020 2020 656c 7365 3a0a 2020          else:.  
-000154f0: 2020 2020 2020 2020 2020 5f66 635f 6361            _fc_ca
-00015500: 6c63 756c 6174 6f72 203d 204e 6f6e 650a  lculator = None.
-00015510: 0a20 2020 2020 2020 2069 6620 6663 5f63  .        if fc_c
-00015520: 616c 6375 6c61 746f 725f 6f70 7469 6f6e  alculator_option
-00015530: 7320 6973 206e 6f74 204e 6f6e 653a 0a20  s is not None:. 
-00015540: 2020 2020 2020 2020 2020 2069 6620 227c             if "|
-00015550: 2220 696e 2066 635f 6361 6c63 756c 6174  " in fc_calculat
-00015560: 6f72 5f6f 7074 696f 6e73 3a0a 2020 2020  or_options:.    
-00015570: 2020 2020 2020 2020 2020 2020 5f66 635f              _fc_
-00015580: 6361 6c63 756c 6174 6f72 5f6f 7074 696f  calculator_optio
-00015590: 6e73 203d 2066 635f 6361 6c63 756c 6174  ns = fc_calculat
-000155a0: 6f72 5f6f 7074 696f 6e73 2e73 706c 6974  or_options.split
-000155b0: 2822 7c22 295b 6f72 6465 7220 2d20 325d  ("|")[order - 2]
-000155c0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000155d0: 2069 6620 5f66 635f 6361 6c63 756c 6174   if _fc_calculat
-000155e0: 6f72 5f6f 7074 696f 6e73 203d 3d20 2222  or_options == ""
+000147a0: 2020 2020 2070 6f73 6974 696f 6e73 5b64       positions[d
+000147b0: 6973 7031 5b22 6e75 6d62 6572 225d 5d20  isp1["number"]] 
+000147c0: 2b3d 2064 6973 705f 6361 7274 310a 2020  += disp_cart1.  
+000147d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000147e0: 2020 706f 7369 7469 6f6e 735b 6469 7370    positions[disp
+000147f0: 325b 226e 756d 6265 7222 5d5d 202b 3d20  2["number"]] += 
+00014800: 6469 7370 325b 2264 6973 706c 6163 656d  disp2["displacem
+00014810: 656e 7422 5d0a 2020 2020 2020 2020 2020  ent"].          
+00014820: 2020 2020 2020 2020 2020 7375 7065 7263            superc
+00014830: 656c 6c73 2e61 7070 656e 6428 0a20 2020  ells.append(.   
+00014840: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00014850: 2020 2020 2050 686f 6e6f 7079 4174 6f6d       PhonopyAtom
+00014860: 7328 0a20 2020 2020 2020 2020 2020 2020  s(.             
+00014870: 2020 2020 2020 2020 2020 2020 2020 206e                 n
+00014880: 756d 6265 7273 3d6e 756d 6265 7273 2c0a  umbers=numbers,.
+00014890: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000148a0: 2020 2020 2020 2020 2020 2020 6d61 7373              mass
+000148b0: 6573 3d6d 6173 7365 732c 0a20 2020 2020  es=masses,.     
+000148c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000148d0: 2020 2020 2020 206d 6167 6e65 7469 635f         magnetic_
+000148e0: 6d6f 6d65 6e74 733d 6d61 676d 6f6d 732c  moments=magmoms,
+000148f0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00014900: 2020 2020 2020 2020 2020 2020 2070 6f73               pos
+00014910: 6974 696f 6e73 3d70 6f73 6974 696f 6e73  itions=positions
+00014920: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+00014930: 2020 2020 2020 2020 2020 2020 2020 6365                ce
+00014940: 6c6c 3d6c 6174 7469 6365 2c0a 2020 2020  ll=lattice,.    
+00014950: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00014960: 2020 2020 290a 2020 2020 2020 2020 2020      ).          
+00014970: 2020 2020 2020 2020 2020 290a 2020 2020            ).    
+00014980: 2020 2020 2020 2020 2020 2020 656c 7365              else
+00014990: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+000149a0: 2020 2020 2020 7375 7065 7263 656c 6c73        supercells
+000149b0: 2e61 7070 656e 6428 4e6f 6e65 290a 0a20  .append(None).. 
+000149c0: 2020 2020 2020 2073 656c 662e 5f73 7570         self._sup
+000149d0: 6572 6365 6c6c 735f 7769 7468 5f64 6973  ercells_with_dis
+000149e0: 706c 6163 656d 656e 7473 203d 2073 7570  placements = sup
+000149f0: 6572 6365 6c6c 730a 0a20 2020 2064 6566  ercells..    def
+00014a00: 205f 6765 745f 7072 696d 6974 6976 655f   _get_primitive_
+00014a10: 6365 6c6c 2873 656c 662c 2073 7570 6572  cell(self, super
+00014a20: 6365 6c6c 2c20 7375 7065 7263 656c 6c5f  cell, supercell_
+00014a30: 6d61 7472 6978 2c20 7072 696d 6974 6976  matrix, primitiv
+00014a40: 655f 6d61 7472 6978 293a 0a20 2020 2020  e_matrix):.     
+00014a50: 2020 2069 6e76 5f73 7570 6572 6365 6c6c     inv_supercell
+00014a60: 5f6d 6174 7269 7820 3d20 6e70 2e6c 696e  _matrix = np.lin
+00014a70: 616c 672e 696e 7628 7375 7065 7263 656c  alg.inv(supercel
+00014a80: 6c5f 6d61 7472 6978 290a 2020 2020 2020  l_matrix).      
+00014a90: 2020 6966 2070 7269 6d69 7469 7665 5f6d    if primitive_m
+00014aa0: 6174 7269 7820 6973 204e 6f6e 653a 0a20  atrix is None:. 
+00014ab0: 2020 2020 2020 2020 2020 2074 5f6d 6174             t_mat
+00014ac0: 203d 2069 6e76 5f73 7570 6572 6365 6c6c   = inv_supercell
+00014ad0: 5f6d 6174 7269 780a 2020 2020 2020 2020  _matrix.        
+00014ae0: 656c 7365 3a0a 2020 2020 2020 2020 2020  else:.          
+00014af0: 2020 745f 6d61 7420 3d20 6e70 2e64 6f74    t_mat = np.dot
+00014b00: 2869 6e76 5f73 7570 6572 6365 6c6c 5f6d  (inv_supercell_m
+00014b10: 6174 7269 782c 2070 7269 6d69 7469 7665  atrix, primitive
+00014b20: 5f6d 6174 7269 7829 0a0a 2020 2020 2020  _matrix)..      
+00014b30: 2020 7265 7475 726e 2067 6574 5f70 7269    return get_pri
+00014b40: 6d69 7469 7665 2873 7570 6572 6365 6c6c  mitive(supercell
+00014b50: 2c20 745f 6d61 742c 2073 656c 662e 5f73  , t_mat, self._s
+00014b60: 796d 7072 6563 2c20 7374 6f72 655f 6465  ymprec, store_de
+00014b70: 6e73 655f 7376 6563 733d 5472 7565 290a  nse_svecs=True).
+00014b80: 0a20 2020 2064 6566 205f 6465 7465 726d  .    def _determ
+00014b90: 696e 655f 7072 696d 6974 6976 655f 6d61  ine_primitive_ma
+00014ba0: 7472 6978 2873 656c 662c 2070 7269 6d69  trix(self, primi
+00014bb0: 7469 7665 5f6d 6174 7269 7829 3a0a 2020  tive_matrix):.  
+00014bc0: 2020 2020 2020 706d 6174 203d 2067 6574        pmat = get
+00014bd0: 5f70 7269 6d69 7469 7665 5f6d 6174 7269  _primitive_matri
+00014be0: 7828 7072 696d 6974 6976 655f 6d61 7472  x(primitive_matr
+00014bf0: 6978 2c20 7379 6d70 7265 633d 7365 6c66  ix, symprec=self
+00014c00: 2e5f 7379 6d70 7265 6329 0a20 2020 2020  ._symprec).     
+00014c10: 2020 2069 6620 6973 696e 7374 616e 6365     if isinstance
+00014c20: 2870 6d61 742c 2073 7472 2920 616e 6420  (pmat, str) and 
+00014c30: 706d 6174 203d 3d20 2261 7574 6f22 3a0a  pmat == "auto":.
+00014c40: 2020 2020 2020 2020 2020 2020 7265 7475              retu
+00014c50: 726e 2067 7565 7373 5f70 7269 6d69 7469  rn guess_primiti
+00014c60: 7665 5f6d 6174 7269 7828 7365 6c66 2e5f  ve_matrix(self._
+00014c70: 756e 6974 6365 6c6c 2c20 7379 6d70 7265  unitcell, sympre
+00014c80: 633d 7365 6c66 2e5f 7379 6d70 7265 6329  c=self._symprec)
+00014c90: 0a20 2020 2020 2020 2065 6c73 653a 0a20  .        else:. 
+00014ca0: 2020 2020 2020 2020 2020 2072 6574 7572             retur
+00014cb0: 6e20 706d 6174 0a0a 2020 2020 6465 6620  n pmat..    def 
+00014cc0: 5f73 6574 5f6d 6573 685f 6e75 6d62 6572  _set_mesh_number
+00014cd0: 7328 0a20 2020 2020 2020 2073 656c 662c  s(.        self,
+00014ce0: 0a20 2020 2020 2020 206d 6573 683a 2055  .        mesh: U
+00014cf0: 6e69 6f6e 5b69 6e74 2c20 666c 6f61 742c  nion[int, float,
+00014d00: 2053 6571 7565 6e63 652c 206e 702e 6e64   Sequence, np.nd
+00014d10: 6172 7261 795d 2c0a 2020 2020 293a 0a20  array],.    ):. 
+00014d20: 2020 2020 2020 2023 2069 6e69 7469 616c         # initial
+00014d30: 697a 6174 696f 6e20 7265 6c61 7465 6420  ization related 
+00014d40: 746f 206d 6573 680a 2020 2020 2020 2020  to mesh.        
+00014d50: 7365 6c66 2e5f 696e 7465 7261 6374 696f  self._interactio
+00014d60: 6e20 3d20 4e6f 6e65 0a0a 2020 2020 2020  n = None..      
+00014d70: 2020 7365 6c66 2e5f 627a 5f67 7269 6420    self._bz_grid 
+00014d80: 3d20 425a 4772 6964 280a 2020 2020 2020  = BZGrid(.      
+00014d90: 2020 2020 2020 6d65 7368 2c0a 2020 2020        mesh,.    
+00014da0: 2020 2020 2020 2020 6c61 7474 6963 653d          lattice=
+00014db0: 7365 6c66 2e5f 7072 696d 6974 6976 652e  self._primitive.
+00014dc0: 6365 6c6c 2c0a 2020 2020 2020 2020 2020  cell,.          
+00014dd0: 2020 7379 6d6d 6574 7279 5f64 6174 6173    symmetry_datas
+00014de0: 6574 3d73 656c 662e 5f70 7269 6d69 7469  et=self._primiti
+00014df0: 7665 5f73 796d 6d65 7472 792e 6461 7461  ve_symmetry.data
+00014e00: 7365 742c 0a20 2020 2020 2020 2020 2020  set,.           
+00014e10: 2069 735f 7469 6d65 5f72 6576 6572 7361   is_time_reversa
+00014e20: 6c3d 7365 6c66 2e5f 6973 5f73 796d 6d65  l=self._is_symme
+00014e30: 7472 792c 0a20 2020 2020 2020 2020 2020  try,.           
+00014e40: 2075 7365 5f67 7267 3d73 656c 662e 5f75   use_grg=self._u
+00014e50: 7365 5f67 7267 2c0a 2020 2020 2020 2020  se_grg,.        
+00014e60: 2020 2020 666f 7263 655f 534e 463d 4661      force_SNF=Fa
+00014e70: 6c73 652c 0a20 2020 2020 2020 2020 2020  lse,.           
+00014e80: 2053 4e46 5f63 6f6f 7264 696e 6174 6573   SNF_coordinates
+00014e90: 3d73 656c 662e 5f53 4e46 5f63 6f6f 7264  =self._SNF_coord
+00014ea0: 696e 6174 6573 2c0a 2020 2020 2020 2020  inates,.        
+00014eb0: 2020 2020 7374 6f72 655f 6465 6e73 655f      store_dense_
+00014ec0: 6770 5f6d 6170 3d54 7275 652c 0a20 2020  gp_map=True,.   
+00014ed0: 2020 2020 2029 0a0a 2020 2020 6465 6620       )..    def 
+00014ee0: 5f69 6e69 745f 6479 6e61 6d69 6361 6c5f  _init_dynamical_
+00014ef0: 6d61 7472 6978 2873 656c 6629 3a0a 2020  matrix(self):.  
+00014f00: 2020 2020 2020 6966 2073 656c 662e 5f69        if self._i
+00014f10: 6e74 6572 6163 7469 6f6e 2069 7320 4e6f  nteraction is No
+00014f20: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
+00014f30: 6d73 6720 3d20 280a 2020 2020 2020 2020  msg = (.        
+00014f40: 2020 2020 2020 2020 2250 686f 6e6f 3370          "Phono3p
+00014f50: 792e 696e 6974 5f70 6870 685f 696e 7465  y.init_phph_inte
+00014f60: 7261 6374 696f 6e20 6861 7320 746f 2062  raction has to b
+00014f70: 6520 6361 6c6c 6564 2022 0a20 2020 2020  e called ".     
+00014f80: 2020 2020 2020 2020 2020 2022 6265 666f             "befo
+00014f90: 7265 2072 756e 6e69 6e67 2074 6869 7320  re running this 
+00014fa0: 6d65 7468 6f64 2e22 0a20 2020 2020 2020  method.".       
+00014fb0: 2020 2020 2029 0a20 2020 2020 2020 2020       ).         
+00014fc0: 2020 2072 6169 7365 2052 756e 7469 6d65     raise Runtime
+00014fd0: 4572 726f 7228 6d73 6729 0a0a 2020 2020  Error(msg)..    
+00014fe0: 2020 2020 7365 6c66 2e5f 696e 7465 7261      self._intera
+00014ff0: 6374 696f 6e2e 696e 6974 5f64 796e 616d  ction.init_dynam
+00015000: 6963 616c 5f6d 6174 7269 7828 0a20 2020  ical_matrix(.   
+00015010: 2020 2020 2020 2020 2073 656c 662e 5f66           self._f
+00015020: 6332 2c0a 2020 2020 2020 2020 2020 2020  c2,.            
+00015030: 7365 6c66 2e5f 7068 6f6e 6f6e 5f73 7570  self._phonon_sup
+00015040: 6572 6365 6c6c 2c0a 2020 2020 2020 2020  ercell,.        
+00015050: 2020 2020 7365 6c66 2e5f 7068 6f6e 6f6e      self._phonon
+00015060: 5f70 7269 6d69 7469 7665 2c0a 2020 2020  _primitive,.    
+00015070: 2020 2020 2020 2020 6e61 635f 7061 7261          nac_para
+00015080: 6d73 3d73 656c 662e 5f6e 6163 5f70 6172  ms=self._nac_par
+00015090: 616d 732c 0a20 2020 2020 2020 2029 0a20  ams,.        ). 
+000150a0: 2020 2020 2020 2066 7265 7173 2c20 5f2c         freqs, _,
+000150b0: 205f 203d 2073 656c 662e 6765 745f 7068   _ = self.get_ph
+000150c0: 6f6e 6f6e 5f64 6174 6128 290a 2020 2020  onon_data().    
+000150d0: 2020 2020 6770 5f47 616d 6d61 203d 2073      gp_Gamma = s
+000150e0: 656c 662e 5f62 7a5f 6772 6964 2e67 705f  elf._bz_grid.gp_
+000150f0: 4761 6d6d 610a 2020 2020 2020 2020 6966  Gamma.        if
+00015100: 206e 702e 7375 6d28 6672 6571 735b 6770   np.sum(freqs[gp
+00015110: 5f47 616d 6d61 5d20 3c20 7365 6c66 2e5f  _Gamma] < self._
+00015120: 6375 746f 6666 5f66 7265 7175 656e 6379  cutoff_frequency
+00015130: 2920 3c20 333a 0a20 2020 2020 2020 2020  ) < 3:.         
+00015140: 2020 2066 6f72 2069 2c20 6620 696e 2065     for i, f in e
+00015150: 6e75 6d65 7261 7465 2866 7265 7173 5b67  numerate(freqs[g
+00015160: 705f 4761 6d6d 612c 203a 335d 293a 0a20  p_Gamma, :3]):. 
+00015170: 2020 2020 2020 2020 2020 2020 2020 2069                 i
+00015180: 6620 6e6f 7420 2866 203c 2073 656c 662e  f not (f < self.
+00015190: 5f63 7574 6f66 665f 6672 6571 7565 6e63  _cutoff_frequenc
+000151a0: 7929 3a0a 2020 2020 2020 2020 2020 2020  y):.            
+000151b0: 2020 2020 2020 2020 6672 6571 735b 6770          freqs[gp
+000151c0: 5f47 616d 6d61 2c20 695d 203d 2030 0a20  _Gamma, i] = 0. 
+000151d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000151e0: 2020 2070 7269 6e74 2822 3d22 202a 2032     print("=" * 2
+000151f0: 3620 2b20 2220 5761 726e 696e 6720 2220  6 + " Warning " 
+00015200: 2b20 223d 2220 2a20 3236 290a 2020 2020  + "=" * 26).    
+00015210: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00015220: 7072 696e 7428 0a20 2020 2020 2020 2020  print(.         
+00015230: 2020 2020 2020 2020 2020 2020 2020 2022                 "
+00015240: 2050 686f 6e6f 6e20 6672 6571 7565 6e63   Phonon frequenc
+00015250: 7920 6f66 2062 616e 6420 696e 6465 7820  y of band index 
+00015260: 2564 2061 7420 4761 6d6d 6120 220a 2020  %d at Gamma ".  
+00015270: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00015280: 2020 2020 2020 2269 7320 6361 6c63 756c        "is calcul
+00015290: 6174 6564 2074 6f20 6265 2025 662e 2220  ated to be %f." 
+000152a0: 2520 2869 202b 2031 2c20 6629 0a20 2020  % (i + 1, f).   
+000152b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000152c0: 2029 0a20 2020 2020 2020 2020 2020 2020   ).             
+000152d0: 2020 2020 2020 2070 7269 6e74 2822 2042         print(" B
+000152e0: 7574 2074 6869 7320 6672 6571 7565 6e63  ut this frequenc
+000152f0: 7920 6973 2066 6f72 6365 6420 746f 2062  y is forced to b
+00015300: 6520 7a65 726f 2e22 290a 2020 2020 2020  e zero.").      
+00015310: 2020 2020 2020 2020 2020 2020 2020 7072                pr
+00015320: 696e 7428 223d 2220 2a20 3631 290a 0a20  int("=" * 61).. 
+00015330: 2020 2064 6566 205f 6578 7472 6163 745f     def _extract_
+00015340: 6663 325f 6663 335f 6361 6c63 756c 6174  fc2_fc3_calculat
+00015350: 6f72 7328 7365 6c66 2c20 6663 5f63 616c  ors(self, fc_cal
+00015360: 6375 6c61 746f 722c 2066 635f 6361 6c63  culator, fc_calc
+00015370: 756c 6174 6f72 5f6f 7074 696f 6e73 2c20  ulator_options, 
+00015380: 6f72 6465 7229 3a0a 2020 2020 2020 2020  order):.        
+00015390: 2222 2245 7874 7261 6374 2066 635f 6361  """Extract fc_ca
+000153a0: 6c63 756c 6174 6f72 2061 6e64 2066 635f  lculator and fc_
+000153b0: 6361 6c63 756c 6174 6f72 5f6f 7074 696f  calculator_optio
+000153c0: 6e73 2066 6f72 2066 6332 2061 6e64 2066  ns for fc2 and f
+000153d0: 6333 2e0a 0a20 2020 2020 2020 2066 635f  c3...        fc_
+000153e0: 6361 6c63 756c 6174 6f72 203a 2073 7472  calculator : str
+000153f0: 0a20 2020 2020 2020 2020 2020 2046 4320  .            FC 
+00015400: 6361 6c63 756c 6174 6f72 2e20 227c 2220  calculator. "|" 
+00015410: 7365 7061 7261 7465 7320 6663 3220 616e  separates fc2 an
+00015420: 6420 6663 332e 2046 6972 7374 2061 6e64  d fc3. First and
+00015430: 206c 6173 740a 2020 2020 2020 2020 2020   last.          
+00015440: 2020 7061 7274 7320 7365 7061 7261 7465    parts separate
+00015450: 6420 636f 7272 6573 706f 6e64 2074 6f20  d correspond to 
+00015460: 6663 3220 616e 6420 6663 3320 6361 6c63  fc2 and fc3 calc
+00015470: 756c 6174 6f72 732c 2072 6573 7065 6374  ulators, respect
+00015480: 6976 656c 792e 0a20 2020 2020 2020 2066  ively..        f
+00015490: 635f 6361 6c63 756c 6174 6f72 5f6f 7074  c_calculator_opt
+000154a0: 696f 6e73 203a 2073 7472 0a20 2020 2020  ions : str.     
+000154b0: 2020 2020 2020 2046 4320 6361 6c63 756c         FC calcul
+000154c0: 6174 6f72 206f 7074 696f 6e73 2e20 227c  ator options. "|
+000154d0: 2220 7365 7061 7261 7465 7320 6663 3220  " separates fc2 
+000154e0: 616e 6420 6663 332e 2046 6972 7374 2061  and fc3. First a
+000154f0: 6e64 206c 6173 740a 2020 2020 2020 2020  nd last.        
+00015500: 2020 2020 7061 7274 7320 7365 7061 7261      parts separa
+00015510: 7465 6420 636f 7272 6573 706f 6e64 2074  ted correspond t
+00015520: 6f20 6663 3220 616e 6420 6663 3320 6f70  o fc2 and fc3 op
+00015530: 7469 6f6e 732c 2072 6573 7065 6374 6976  tions, respectiv
+00015540: 656c 792e 0a20 2020 2020 2020 206f 7264  ely..        ord
+00015550: 6572 203a 2069 6e74 203d 2032 206f 7220  er : int = 2 or 
+00015560: 330a 2020 2020 2020 2020 2020 2020 3220  3.            2 
+00015570: 616e 6420 3320 696e 6469 6361 7465 2066  and 3 indicate f
+00015580: 6332 2061 6e64 2066 6333 2c20 7265 7370  c2 and fc3, resp
+00015590: 6563 7469 7665 6c79 2e0a 0a20 2020 2020  ectively...     
+000155a0: 2020 2022 2222 0a20 2020 2020 2020 2069     """.        i
+000155b0: 6620 6663 5f63 616c 6375 6c61 746f 7220  f fc_calculator 
+000155c0: 6973 206e 6f74 204e 6f6e 653a 0a20 2020  is not None:.   
+000155d0: 2020 2020 2020 2020 2069 6620 227c 2220           if "|" 
+000155e0: 696e 2066 635f 6361 6c63 756c 6174 6f72  in fc_calculator
 000155f0: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-00015600: 2020 2020 2020 5f66 635f 6361 6c63 756c        _fc_calcul
-00015610: 6174 6f72 5f6f 7074 696f 6e73 203d 204e  ator_options = N
-00015620: 6f6e 650a 2020 2020 2020 2020 2020 2020  one.            
-00015630: 656c 7365 3a0a 2020 2020 2020 2020 2020  else:.          
-00015640: 2020 2020 2020 5f66 635f 6361 6c63 756c        _fc_calcul
-00015650: 6174 6f72 5f6f 7074 696f 6e73 203d 2066  ator_options = f
-00015660: 635f 6361 6c63 756c 6174 6f72 5f6f 7074  c_calculator_opt
-00015670: 696f 6e73 0a20 2020 2020 2020 2065 6c73  ions.        els
-00015680: 653a 0a20 2020 2020 2020 2020 2020 205f  e:.            _
-00015690: 6663 5f63 616c 6375 6c61 746f 725f 6f70  fc_calculator_op
-000156a0: 7469 6f6e 7320 3d20 4e6f 6e65 0a0a 2020  tions = None..  
-000156b0: 2020 2020 2020 7265 7475 726e 205f 6663        return _fc
-000156c0: 5f63 616c 6375 6c61 746f 722c 205f 6663  _calculator, _fc
-000156d0: 5f63 616c 6375 6c61 746f 725f 6f70 7469  _calculator_opti
-000156e0: 6f6e 730a                                ons.
+00015600: 2020 5f66 635f 6361 6c63 756c 6174 6f72    _fc_calculator
+00015610: 203d 2066 635f 6361 6c63 756c 6174 6f72   = fc_calculator
+00015620: 2e73 706c 6974 2822 7c22 295b 6f72 6465  .split("|")[orde
+00015630: 7220 2d20 325d 0a20 2020 2020 2020 2020  r - 2].         
+00015640: 2020 2020 2020 2069 6620 5f66 635f 6361         if _fc_ca
+00015650: 6c63 756c 6174 6f72 203d 3d20 2222 3a0a  lculator == "":.
+00015660: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00015670: 2020 2020 5f66 635f 6361 6c63 756c 6174      _fc_calculat
+00015680: 6f72 203d 204e 6f6e 650a 2020 2020 2020  or = None.      
+00015690: 2020 2020 2020 656c 7365 3a0a 2020 2020        else:.    
+000156a0: 2020 2020 2020 2020 2020 2020 5f66 635f              _fc_
+000156b0: 6361 6c63 756c 6174 6f72 203d 2066 635f  calculator = fc_
+000156c0: 6361 6c63 756c 6174 6f72 0a20 2020 2020  calculator.     
+000156d0: 2020 2065 6c73 653a 0a20 2020 2020 2020     else:.       
+000156e0: 2020 2020 205f 6663 5f63 616c 6375 6c61       _fc_calcula
+000156f0: 746f 7220 3d20 4e6f 6e65 0a0a 2020 2020  tor = None..    
+00015700: 2020 2020 6966 2066 635f 6361 6c63 756c      if fc_calcul
+00015710: 6174 6f72 5f6f 7074 696f 6e73 2069 7320  ator_options is 
+00015720: 6e6f 7420 4e6f 6e65 3a0a 2020 2020 2020  not None:.      
+00015730: 2020 2020 2020 6966 2022 7c22 2069 6e20        if "|" in 
+00015740: 6663 5f63 616c 6375 6c61 746f 725f 6f70  fc_calculator_op
+00015750: 7469 6f6e 733a 0a20 2020 2020 2020 2020  tions:.         
+00015760: 2020 2020 2020 205f 6663 5f63 616c 6375         _fc_calcu
+00015770: 6c61 746f 725f 6f70 7469 6f6e 7320 3d20  lator_options = 
+00015780: 6663 5f63 616c 6375 6c61 746f 725f 6f70  fc_calculator_op
+00015790: 7469 6f6e 732e 7370 6c69 7428 227c 2229  tions.split("|")
+000157a0: 5b6f 7264 6572 202d 2032 5d0a 2020 2020  [order - 2].    
+000157b0: 2020 2020 2020 2020 2020 2020 6966 205f              if _
+000157c0: 6663 5f63 616c 6375 6c61 746f 725f 6f70  fc_calculator_op
+000157d0: 7469 6f6e 7320 3d3d 2022 223a 0a20 2020  tions == "":.   
+000157e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000157f0: 205f 6663 5f63 616c 6375 6c61 746f 725f   _fc_calculator_
+00015800: 6f70 7469 6f6e 7320 3d20 4e6f 6e65 0a20  options = None. 
+00015810: 2020 2020 2020 2020 2020 2065 6c73 653a             else:
+00015820: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00015830: 205f 6663 5f63 616c 6375 6c61 746f 725f   _fc_calculator_
+00015840: 6f70 7469 6f6e 7320 3d20 6663 5f63 616c  options = fc_cal
+00015850: 6375 6c61 746f 725f 6f70 7469 6f6e 730a  culator_options.
+00015860: 2020 2020 2020 2020 656c 7365 3a0a 2020          else:.  
+00015870: 2020 2020 2020 2020 2020 5f66 635f 6361            _fc_ca
+00015880: 6c63 756c 6174 6f72 5f6f 7074 696f 6e73  lculator_options
+00015890: 203d 204e 6f6e 650a 0a20 2020 2020 2020   = None..       
+000158a0: 2072 6574 7572 6e20 5f66 635f 6361 6c63   return _fc_calc
+000158b0: 756c 6174 6f72 2c20 5f66 635f 6361 6c63  ulator, _fc_calc
+000158c0: 756c 6174 6f72 5f6f 7074 696f 6e73 0a0a  ulator_options..
+000158d0: 2020 2020 6465 6620 5f67 6574 5f66 6f72      def _get_for
+000158e0: 6365 735f 656e 6572 6769 6573 280a 2020  ces_energies(.  
+000158f0: 2020 2020 2020 7365 6c66 2c20 7461 7267        self, targ
+00015900: 6574 3a20 4c69 7465 7261 6c5b 2266 6f72  et: Literal["for
+00015910: 6365 7322 2c20 2273 7570 6572 6365 6c6c  ces", "supercell
+00015920: 5f65 6e65 7267 6965 7322 5d0a 2020 2020  _energies"].    
+00015930: 2920 2d3e 204f 7074 696f 6e61 6c5b 6e70  ) -> Optional[np
+00015940: 2e6e 6461 7272 6179 5d3a 0a20 2020 2020  .ndarray]:.     
+00015950: 2020 2022 2222 5265 7475 726e 2066 6333     """Return fc3
+00015960: 2066 6f72 6365 7320 616e 6420 7375 7065   forces and supe
+00015970: 7263 656c 6c20 656e 6572 6769 6573 2e0a  rcell energies..
+00015980: 0a20 2020 2020 2020 2052 6574 7572 6e20  .        Return 
+00015990: 4e6f 6e65 2069 6620 7461 6765 7274 2064  None if tagert d
+000159a0: 6174 6120 6973 206e 6f74 2066 6f75 6e64  ata is not found
+000159b0: 2072 6174 6865 7220 7468 616e 2072 6169   rather than rai
+000159c0: 7369 6e67 2065 7863 6570 7469 6f6e 2e0a  sing exception..
+000159d0: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
+000159e0: 2020 2020 2069 6620 7461 7267 6574 2069       if target i
+000159f0: 6e20 7365 6c66 2e5f 6461 7461 7365 743a  n self._dataset:
+00015a00: 2020 2320 7479 7065 2d32 0a20 2020 2020    # type-2.     
+00015a10: 2020 2020 2020 2072 6574 7572 6e20 7365         return se
+00015a20: 6c66 2e5f 6461 7461 7365 745b 7461 7267  lf._dataset[targ
+00015a30: 6574 5d0a 2020 2020 2020 2020 656c 6966  et].        elif
+00015a40: 2022 6669 7273 745f 6174 6f6d 7322 2069   "first_atoms" i
+00015a50: 6e20 7365 6c66 2e5f 6461 7461 7365 743a  n self._dataset:
+00015a60: 2020 2320 7479 7065 2d31 0a20 2020 2020    # type-1.     
+00015a70: 2020 2020 2020 206e 756d 5f73 6365 6c6c         num_scell
+00015a80: 7320 3d20 6c65 6e28 7365 6c66 2e5f 6461  s = len(self._da
+00015a90: 7461 7365 745b 2266 6972 7374 5f61 746f  taset["first_ato
+00015aa0: 6d73 225d 290a 2020 2020 2020 2020 2020  ms"]).          
+00015ab0: 2020 666f 7220 6469 7370 3120 696e 2073    for disp1 in s
+00015ac0: 656c 662e 5f64 6174 6173 6574 5b22 6669  elf._dataset["fi
+00015ad0: 7273 745f 6174 6f6d 7322 5d3a 0a20 2020  rst_atoms"]:.   
+00015ae0: 2020 2020 2020 2020 2020 2020 206e 756d               num
+00015af0: 5f73 6365 6c6c 7320 2b3d 206c 656e 2864  _scells += len(d
+00015b00: 6973 7031 5b22 7365 636f 6e64 5f61 746f  isp1["second_ato
+00015b10: 6d73 225d 290a 2020 2020 2020 2020 2020  ms"]).          
+00015b20: 2020 6966 2074 6172 6765 7420 3d3d 2022    if target == "
+00015b30: 666f 7263 6573 223a 0a20 2020 2020 2020  forces":.       
+00015b40: 2020 2020 2020 2020 2076 616c 7565 7320           values 
+00015b50: 3d20 6e70 2e7a 6572 6f73 280a 2020 2020  = np.zeros(.    
+00015b60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00015b70: 286e 756d 5f73 6365 6c6c 732c 206c 656e  (num_scells, len
+00015b80: 2873 656c 662e 5f73 7570 6572 6365 6c6c  (self._supercell
+00015b90: 292c 2033 292c 0a20 2020 2020 2020 2020  ), 3),.         
+00015ba0: 2020 2020 2020 2020 2020 2064 7479 7065             dtype
+00015bb0: 3d22 646f 7562 6c65 222c 0a20 2020 2020  ="double",.     
+00015bc0: 2020 2020 2020 2020 2020 2020 2020 206f                 o
+00015bd0: 7264 6572 3d22 4322 2c0a 2020 2020 2020  rder="C",.      
+00015be0: 2020 2020 2020 2020 2020 290a 2020 2020            ).    
+00015bf0: 2020 2020 2020 2020 2020 2020 7479 7065              type
+00015c00: 315f 7461 7267 6574 203d 2022 666f 7263  1_target = "forc
+00015c10: 6573 220a 2020 2020 2020 2020 2020 2020  es".            
+00015c20: 656c 6966 2074 6172 6765 7420 3d3d 2022  elif target == "
+00015c30: 7375 7065 7263 656c 6c5f 656e 6572 6769  supercell_energi
+00015c40: 6573 223a 0a20 2020 2020 2020 2020 2020  es":.           
+00015c50: 2020 2020 2076 616c 7565 7320 3d20 6e70       values = np
+00015c60: 2e7a 6572 6f73 286e 756d 5f73 6365 6c6c  .zeros(num_scell
+00015c70: 732c 2064 7479 7065 3d22 646f 7562 6c65  s, dtype="double
+00015c80: 2229 0a20 2020 2020 2020 2020 2020 2020  ").             
+00015c90: 2020 2074 7970 6531 5f74 6172 6765 7420     type1_target 
+00015ca0: 3d20 2273 7570 6572 6365 6c6c 5f65 6e65  = "supercell_ene
+00015cb0: 7267 7922 0a20 2020 2020 2020 2020 2020  rgy".           
+00015cc0: 2063 6f75 6e74 203d 2030 0a20 2020 2020   count = 0.     
+00015cd0: 2020 2020 2020 2066 6f72 2064 6973 7031         for disp1
+00015ce0: 2069 6e20 7365 6c66 2e5f 6461 7461 7365   in self._datase
+00015cf0: 745b 2266 6972 7374 5f61 746f 6d73 225d  t["first_atoms"]
+00015d00: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+00015d10: 2020 7661 6c75 6573 5b63 6f75 6e74 5d20    values[count] 
+00015d20: 3d20 6469 7370 315b 7479 7065 315f 7461  = disp1[type1_ta
+00015d30: 7267 6574 5d0a 2020 2020 2020 2020 2020  rget].          
+00015d40: 2020 2020 2020 636f 756e 7420 2b3d 2031        count += 1
+00015d50: 0a20 2020 2020 2020 2020 2020 2066 6f72  .            for
+00015d60: 2064 6973 7031 2069 6e20 7365 6c66 2e5f   disp1 in self._
+00015d70: 6461 7461 7365 745b 2266 6972 7374 5f61  dataset["first_a
+00015d80: 746f 6d73 225d 3a0a 2020 2020 2020 2020  toms"]:.        
+00015d90: 2020 2020 2020 2020 666f 7220 6469 7370          for disp
+00015da0: 3220 696e 2064 6973 7031 5b22 7365 636f  2 in disp1["seco
+00015db0: 6e64 5f61 746f 6d73 225d 3a0a 2020 2020  nd_atoms"]:.    
+00015dc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00015dd0: 7661 6c75 6573 5b63 6f75 6e74 5d20 3d20  values[count] = 
+00015de0: 6469 7370 325b 7479 7065 315f 7461 7267  disp2[type1_targ
+00015df0: 6574 5d0a 2020 2020 2020 2020 2020 2020  et].            
+00015e00: 2020 2020 2020 2020 636f 756e 7420 2b3d          count +=
+00015e10: 2031 0a20 2020 2020 2020 2020 2020 2072   1.            r
+00015e20: 6574 7572 6e20 7661 6c75 6573 0a20 2020  eturn values.   
+00015e30: 2020 2020 2072 6574 7572 6e20 4e6f 6e65       return None
+00015e40: 0a0a 2020 2020 6465 6620 5f73 6574 5f66  ..    def _set_f
+00015e50: 6f72 6365 735f 656e 6572 6769 6573 280a  orces_energies(.
+00015e60: 2020 2020 2020 2020 7365 6c66 2c20 7661          self, va
+00015e70: 6c75 6573 2c20 7461 7267 6574 3a20 4c69  lues, target: Li
+00015e80: 7465 7261 6c5b 2266 6f72 6365 7322 2c20  teral["forces", 
+00015e90: 2273 7570 6572 6365 6c6c 5f65 6e65 7267  "supercell_energ
+00015ea0: 6965 7322 5d0a 2020 2020 293a 0a20 2020  ies"].    ):.   
+00015eb0: 2020 2020 2069 6620 2266 6972 7374 5f61       if "first_a
+00015ec0: 746f 6d73 2220 696e 2073 656c 662e 5f64  toms" in self._d
+00015ed0: 6174 6173 6574 3a20 2023 2074 7970 652d  ataset:  # type-
+00015ee0: 310a 2020 2020 2020 2020 2020 2020 636f  1.            co
+00015ef0: 756e 7420 3d20 300a 2020 2020 2020 2020  unt = 0.        
+00015f00: 2020 2020 666f 7220 6469 7370 3120 696e      for disp1 in
+00015f10: 2073 656c 662e 5f64 6174 6173 6574 5b22   self._dataset["
+00015f20: 6669 7273 745f 6174 6f6d 7322 5d3a 0a20  first_atoms"]:. 
+00015f30: 2020 2020 2020 2020 2020 2020 2020 2069                 i
+00015f40: 6620 7461 7267 6574 203d 3d20 2266 6f72  f target == "for
+00015f50: 6365 7322 3a0a 2020 2020 2020 2020 2020  ces":.          
+00015f60: 2020 2020 2020 2020 2020 6469 7370 315b            disp1[
+00015f70: 7461 7267 6574 5d20 3d20 6e70 2e61 7272  target] = np.arr
+00015f80: 6179 2876 616c 7565 735b 636f 756e 745d  ay(values[count]
+00015f90: 2c20 6474 7970 653d 2264 6f75 626c 6522  , dtype="double"
+00015fa0: 2c20 6f72 6465 723d 2243 2229 0a20 2020  , order="C").   
+00015fb0: 2020 2020 2020 2020 2020 2020 2065 6c69               eli
+00015fc0: 6620 7461 7267 6574 203d 3d20 2273 7570  f target == "sup
+00015fd0: 6572 6365 6c6c 5f65 6e65 7267 6965 7322  ercell_energies"
+00015fe0: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+00015ff0: 2020 2020 2020 6469 7370 315b 2273 7570        disp1["sup
+00016000: 6572 6365 6c6c 5f65 6e65 7267 7922 5d20  ercell_energy"] 
+00016010: 3d20 666c 6f61 7428 7661 6c75 6573 5b63  = float(values[c
+00016020: 6f75 6e74 5d29 0a20 2020 2020 2020 2020  ount]).         
+00016030: 2020 2020 2020 2063 6f75 6e74 202b 3d20         count += 
+00016040: 310a 2020 2020 2020 2020 2020 2020 666f  1.            fo
+00016050: 7220 6469 7370 3120 696e 2073 656c 662e  r disp1 in self.
+00016060: 5f64 6174 6173 6574 5b22 6669 7273 745f  _dataset["first_
+00016070: 6174 6f6d 7322 5d3a 0a20 2020 2020 2020  atoms"]:.       
+00016080: 2020 2020 2020 2020 2066 6f72 2064 6973           for dis
+00016090: 7032 2069 6e20 6469 7370 315b 2273 6563  p2 in disp1["sec
+000160a0: 6f6e 645f 6174 6f6d 7322 5d3a 0a20 2020  ond_atoms"]:.   
+000160b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000160c0: 2069 6620 7461 7267 6574 203d 3d20 2266   if target == "f
+000160d0: 6f72 6365 7322 3a0a 2020 2020 2020 2020  orces":.        
+000160e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000160f0: 6469 7370 325b 7461 7267 6574 5d20 3d20  disp2[target] = 
+00016100: 6e70 2e61 7272 6179 280a 2020 2020 2020  np.array(.      
+00016110: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00016120: 2020 2020 2020 7661 6c75 6573 5b63 6f75        values[cou
+00016130: 6e74 5d2c 2064 7479 7065 3d22 646f 7562  nt], dtype="doub
+00016140: 6c65 222c 206f 7264 6572 3d22 4322 0a20  le", order="C". 
+00016150: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00016160: 2020 2020 2020 2029 0a20 2020 2020 2020         ).       
+00016170: 2020 2020 2020 2020 2020 2020 2065 6c69               eli
+00016180: 6620 7461 7267 6574 203d 3d20 2273 7570  f target == "sup
+00016190: 6572 6365 6c6c 5f65 6e65 7267 6965 7322  ercell_energies"
+000161a0: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+000161b0: 2020 2020 2020 2020 2020 6469 7370 325b            disp2[
+000161c0: 2273 7570 6572 6365 6c6c 5f65 6e65 7267  "supercell_energ
+000161d0: 7922 5d20 3d20 666c 6f61 7428 7661 6c75  y"] = float(valu
+000161e0: 6573 5b63 6f75 6e74 5d29 0a20 2020 2020  es[count]).     
+000161f0: 2020 2020 2020 2020 2020 2020 2020 2063                 c
+00016200: 6f75 6e74 202b 3d20 310a 2020 2020 2020  ount += 1.      
+00016210: 2020 656c 6966 2022 6469 7370 6c61 6365    elif "displace
+00016220: 6d65 6e74 7322 2069 6e20 7365 6c66 2e5f  ments" in self._
+00016230: 6461 7461 7365 7420 6f72 2022 666f 7263  dataset or "forc
+00016240: 6573 2220 696e 2073 656c 662e 5f64 6174  es" in self._dat
+00016250: 6173 6574 3a20 2023 2074 7970 652d 320a  aset:  # type-2.
+00016260: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+00016270: 2e5f 6461 7461 7365 745b 7461 7267 6574  ._dataset[target
+00016280: 5d20 3d20 6e70 2e61 7272 6179 2876 616c  ] = np.array(val
+00016290: 7565 732c 2064 7479 7065 3d22 646f 7562  ues, dtype="doub
+000162a0: 6c65 222c 206f 7264 6572 3d22 4322 290a  le", order="C").
+000162b0: 2020 2020 2020 2020 656c 7365 3a0a 2020          else:.  
+000162c0: 2020 2020 2020 2020 2020 7261 6973 6520            raise 
+000162d0: 5275 6e74 696d 6545 7272 6f72 2822 5365  RuntimeError("Se
+000162e0: 7420 6f66 2046 4333 2064 6973 706c 6163  t of FC3 displac
+000162f0: 656d 656e 7473 2069 7320 6e6f 7420 6176  ements is not av
+00016300: 6169 6c61 626c 652e 2229 0a0a 2020 2020  ailable.")..    
+00016310: 6465 6620 5f67 6574 5f70 686f 6e6f 6e5f  def _get_phonon_
+00016320: 666f 7263 6573 5f65 6e65 7267 6965 7328  forces_energies(
+00016330: 0a20 2020 2020 2020 2073 656c 662c 2074  .        self, t
+00016340: 6172 6765 743a 204c 6974 6572 616c 5b22  arget: Literal["
+00016350: 666f 7263 6573 222c 2022 7375 7065 7263  forces", "superc
+00016360: 656c 6c5f 656e 6572 6769 6573 225d 0a20  ell_energies"]. 
+00016370: 2020 2029 202d 3e20 4f70 7469 6f6e 616c     ) -> Optional
+00016380: 5b6e 702e 6e64 6172 7261 795d 3a0a 2020  [np.ndarray]:.  
+00016390: 2020 2020 2020 2222 2252 6574 7572 6e20        """Return 
+000163a0: 6663 3220 666f 7263 6573 2061 6e64 2073  fc2 forces and s
+000163b0: 7570 6572 6365 6c6c 2065 6e65 7267 6965  upercell energie
+000163c0: 732e 0a0a 2020 2020 2020 2020 5265 7475  s...        Retu
+000163d0: 726e 204e 6f6e 6520 6966 2074 6167 6572  rn None if tager
+000163e0: 7420 6461 7461 2069 7320 6e6f 7420 666f  t data is not fo
+000163f0: 756e 6420 7261 7468 6572 2074 6861 6e20  und rather than 
+00016400: 7261 6973 696e 6720 6578 6365 7074 696f  raising exceptio
+00016410: 6e2e 0a0a 2020 2020 2020 2020 2222 220a  n...        """.
+00016420: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
+00016430: 5f70 686f 6e6f 6e5f 6461 7461 7365 7420  _phonon_dataset 
+00016440: 6973 204e 6f6e 653a 0a20 2020 2020 2020  is None:.       
+00016450: 2020 2020 2072 6169 7365 2052 756e 7469       raise Runti
+00016460: 6d65 4572 726f 7228 2244 6174 6173 6574  meError("Dataset
+00016470: 2066 6f72 2066 6332 646f 6573 206e 6f74   for fc2does not
+00016480: 2065 7869 7374 2e22 290a 0a20 2020 2020   exist.")..     
+00016490: 2020 2069 6620 7461 7267 6574 2069 6e20     if target in 
+000164a0: 7365 6c66 2e5f 7068 6f6e 6f6e 5f64 6174  self._phonon_dat
+000164b0: 6173 6574 3a20 2023 2074 7970 652d 320a  aset:  # type-2.
+000164c0: 2020 2020 2020 2020 2020 2020 7265 7475              retu
+000164d0: 726e 2073 656c 662e 5f70 686f 6e6f 6e5f  rn self._phonon_
+000164e0: 6461 7461 7365 745b 7461 7267 6574 5d0a  dataset[target].
+000164f0: 2020 2020 2020 2020 656c 6966 2022 6669          elif "fi
+00016500: 7273 745f 6174 6f6d 7322 2069 6e20 7365  rst_atoms" in se
+00016510: 6c66 2e5f 7068 6f6e 6f6e 5f64 6174 6173  lf._phonon_datas
+00016520: 6574 3a20 2023 2074 7970 652d 310a 2020  et:  # type-1.  
+00016530: 2020 2020 2020 2020 2020 7661 6c75 6573            values
+00016540: 203d 205b 5d0a 2020 2020 2020 2020 2020   = [].          
+00016550: 2020 666f 7220 6469 7370 2069 6e20 7365    for disp in se
+00016560: 6c66 2e5f 7068 6f6e 6f6e 5f64 6174 6173  lf._phonon_datas
+00016570: 6574 5b22 6669 7273 745f 6174 6f6d 7322  et["first_atoms"
+00016580: 5d3a 0a20 2020 2020 2020 2020 2020 2020  ]:.             
+00016590: 2020 2069 6620 7461 7267 6574 203d 3d20     if target == 
+000165a0: 2266 6f72 6365 7322 3a0a 2020 2020 2020  "forces":.      
+000165b0: 2020 2020 2020 2020 2020 2020 2020 6966                if
+000165c0: 2074 6172 6765 7420 696e 2064 6973 703a   target in disp:
+000165d0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000165e0: 2020 2020 2020 2020 2076 616c 7565 732e           values.
+000165f0: 6170 7065 6e64 2864 6973 705b 7461 7267  append(disp[targ
+00016600: 6574 5d29 0a20 2020 2020 2020 2020 2020  et]).           
+00016610: 2020 2020 2065 6c69 6620 7461 7267 6574       elif target
+00016620: 203d 3d20 2273 7570 6572 6365 6c6c 5f65   == "supercell_e
+00016630: 6e65 7267 6965 7322 3a0a 2020 2020 2020  nergies":.      
+00016640: 2020 2020 2020 2020 2020 2020 2020 6966                if
+00016650: 2022 7375 7065 7263 656c 6c5f 656e 6572   "supercell_ener
+00016660: 6779 2220 696e 2064 6973 703a 0a20 2020  gy" in disp:.   
+00016670: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00016680: 2020 2020 2076 616c 7565 732e 6170 7065       values.appe
+00016690: 6e64 2864 6973 705b 2273 7570 6572 6365  nd(disp["superce
+000166a0: 6c6c 5f65 6e65 7267 7922 5d29 0a20 2020  ll_energy"]).   
+000166b0: 2020 2020 2020 2020 2069 6620 7661 6c75           if valu
+000166c0: 6573 3a0a 2020 2020 2020 2020 2020 2020  es:.            
+000166d0: 2020 2020 7265 7475 726e 206e 702e 6172      return np.ar
+000166e0: 7261 7928 7661 6c75 6573 2c20 6474 7970  ray(values, dtyp
+000166f0: 653d 2264 6f75 626c 6522 2c20 6f72 6465  e="double", orde
+00016700: 723d 2243 2229 0a20 2020 2020 2020 2072  r="C").        r
+00016710: 6574 7572 6e20 4e6f 6e65 0a0a 2020 2020  eturn None..    
+00016720: 6465 6620 5f73 6574 5f70 686f 6e6f 6e5f  def _set_phonon_
+00016730: 666f 7263 6573 5f65 6e65 7267 6965 7328  forces_energies(
+00016740: 0a20 2020 2020 2020 2073 656c 662c 2076  .        self, v
+00016750: 616c 7565 732c 2074 6172 6765 743a 204c  alues, target: L
+00016760: 6974 6572 616c 5b22 666f 7263 6573 222c  iteral["forces",
+00016770: 2022 7375 7065 7263 656c 6c5f 656e 6572   "supercell_ener
+00016780: 6769 6573 225d 0a20 2020 2029 3a0a 2020  gies"].    ):.  
+00016790: 2020 2020 2020 6966 2073 656c 662e 5f70        if self._p
+000167a0: 686f 6e6f 6e5f 6461 7461 7365 7420 6973  honon_dataset is
+000167b0: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
+000167c0: 2020 2072 6169 7365 2052 756e 7469 6d65     raise Runtime
+000167d0: 4572 726f 7228 2244 6174 6173 6574 2066  Error("Dataset f
+000167e0: 6f72 2066 6332 2064 6f65 7320 6e6f 7420  or fc2 does not 
+000167f0: 6578 6973 742e 2229 0a0a 2020 2020 2020  exist.")..      
+00016800: 2020 6966 2022 6669 7273 745f 6174 6f6d    if "first_atom
+00016810: 7322 2069 6e20 7365 6c66 2e5f 7068 6f6e  s" in self._phon
+00016820: 6f6e 5f64 6174 6173 6574 3a0a 2020 2020  on_dataset:.    
+00016830: 2020 2020 2020 2020 666f 7220 6469 7370          for disp
+00016840: 2c20 7620 696e 207a 6970 2873 656c 662e  , v in zip(self.
+00016850: 5f70 686f 6e6f 6e5f 6461 7461 7365 745b  _phonon_dataset[
+00016860: 2266 6972 7374 5f61 746f 6d73 225d 2c20  "first_atoms"], 
+00016870: 7661 6c75 6573 293a 0a20 2020 2020 2020  values):.       
+00016880: 2020 2020 2020 2020 2069 6620 7461 7267           if targ
+00016890: 6574 203d 3d20 2266 6f72 6365 7322 3a0a  et == "forces":.
+000168a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000168b0: 2020 2020 6469 7370 5b74 6172 6765 745d      disp[target]
+000168c0: 203d 206e 702e 6172 7261 7928 762c 2064   = np.array(v, d
+000168d0: 7479 7065 3d22 646f 7562 6c65 222c 206f  type="double", o
+000168e0: 7264 6572 3d22 4322 290a 2020 2020 2020  rder="C").      
+000168f0: 2020 2020 2020 2020 2020 656c 6966 2074            elif t
+00016900: 6172 6765 7420 3d3d 2022 7375 7065 7263  arget == "superc
+00016910: 656c 6c5f 656e 6572 6769 6573 223a 0a20  ell_energies":. 
+00016920: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00016930: 2020 2064 6973 705b 2273 7570 6572 6365     disp["superce
+00016940: 6c6c 5f65 6e65 7267 7922 5d20 3d20 666c  ll_energy"] = fl
+00016950: 6f61 7428 7629 0a20 2020 2020 2020 2065  oat(v).        e
+00016960: 6c69 6620 2264 6973 706c 6163 656d 656e  lif "displacemen
+00016970: 7473 2220 696e 2073 656c 662e 5f70 686f  ts" in self._pho
+00016980: 6e6f 6e5f 6461 7461 7365 743a 0a20 2020  non_dataset:.   
+00016990: 2020 2020 2020 2020 205f 7661 6c75 6573           _values
+000169a0: 203d 206e 702e 6172 7261 7928 7661 6c75   = np.array(valu
+000169b0: 6573 2c20 6474 7970 653d 2264 6f75 626c  es, dtype="doubl
+000169c0: 6522 2c20 6f72 6465 723d 2243 2229 0a20  e", order="C"). 
+000169d0: 2020 2020 2020 2020 2020 206e 6174 6f6d             natom
+000169e0: 203d 206c 656e 2873 656c 662e 5f70 686f   = len(self._pho
+000169f0: 6e6f 6e5f 7375 7065 7263 656c 6c29 0a20  non_supercell). 
+00016a00: 2020 2020 2020 2020 2020 206e 6469 7370             ndisp
+00016a10: 7320 3d20 6c65 6e28 7365 6c66 2e5f 7068  s = len(self._ph
+00016a20: 6f6e 6f6e 5f64 6174 6173 6574 5b22 6469  onon_dataset["di
+00016a30: 7370 6c61 6365 6d65 6e74 7322 5d29 0a20  splacements"]). 
+00016a40: 2020 2020 2020 2020 2020 2069 6620 7461             if ta
+00016a50: 7267 6574 203d 3d20 2266 6f72 6365 7322  rget == "forces"
+00016a60: 2061 6e64 2028 0a20 2020 2020 2020 2020   and (.         
+00016a70: 2020 2020 2020 205f 7661 6c75 6573 2e6e         _values.n
+00016a80: 6469 6d20 213d 2033 206f 7220 5f76 616c  dim != 3 or _val
+00016a90: 7565 732e 7368 6170 6520 213d 2028 6e64  ues.shape != (nd
+00016aa0: 6973 7073 2c20 6e61 746f 6d2c 2033 290a  isps, natom, 3).
+00016ab0: 2020 2020 2020 2020 2020 2020 293a 0a20              ):. 
+00016ac0: 2020 2020 2020 2020 2020 2020 2020 2072                 r
+00016ad0: 6169 7365 2052 756e 7469 6d65 4572 726f  aise RuntimeErro
+00016ae0: 7228 6622 4172 7261 7920 7368 6170 6520  r(f"Array shape 
+00016af0: 6f66 2069 6e70 7574 207b 7461 7267 6574  of input {target
+00016b00: 7d20 6973 2069 6e63 6f72 7265 6374 2e22  } is incorrect."
+00016b10: 290a 2020 2020 2020 2020 2020 2020 656c  ).            el
+00016b20: 6966 2074 6172 6765 7420 3d3d 2022 7375  if target == "su
+00016b30: 7065 7263 656c 6c5f 656e 6572 6769 6573  percell_energies
+00016b40: 223a 0a20 2020 2020 2020 2020 2020 2020  ":.             
+00016b50: 2020 2069 6620 5f76 616c 7565 732e 6e64     if _values.nd
+00016b60: 696d 2021 3d20 3120 6f72 205f 7661 6c75  im != 1 or _valu
+00016b70: 6573 2e73 6861 7065 2021 3d20 286e 6469  es.shape != (ndi
+00016b80: 7370 732c 293a 0a20 2020 2020 2020 2020  sps,):.         
+00016b90: 2020 2020 2020 2020 2020 2072 6169 7365             raise
+00016ba0: 2052 756e 7469 6d65 4572 726f 7228 6622   RuntimeError(f"
+00016bb0: 4172 7261 7920 7368 6170 6520 6f66 2069  Array shape of i
+00016bc0: 6e70 7574 207b 7461 7267 6574 7d20 6973  nput {target} is
+00016bd0: 2069 6e63 6f72 7265 6374 2e22 290a 2020   incorrect.").  
+00016be0: 2020 2020 2020 2020 2020 7365 6c66 2e5f            self._
+00016bf0: 7068 6f6e 6f6e 5f64 6174 6173 6574 5b74  phonon_dataset[t
+00016c00: 6172 6765 745d 203d 205f 7661 6c75 6573  arget] = _values
+00016c10: 0a20 2020 2020 2020 2065 6c73 653a 0a20  .        else:. 
+00016c20: 2020 2020 2020 2020 2020 2072 6169 7365             raise
+00016c30: 2052 756e 7469 6d65 4572 726f 7228 2253   RuntimeError("S
+00016c40: 6574 206f 6620 4643 3220 6469 7370 6c61  et of FC2 displa
+00016c50: 6365 6d65 6e74 7320 6973 206e 6f74 2061  cements is not a
+00016c60: 7661 696c 6162 6c65 2e22 290a            vailable.").
```

### Comparing `phono3py-3.0.2/phono3py/conductivity/base.py` & `phono3py-3.0.3/phono3py/conductivity/base.py`

 * *Files identical despite different names*

### Comparing `phono3py-3.0.2/phono3py/conductivity/direct_solution.py` & `phono3py-3.0.3/phono3py/conductivity/direct_solution.py`

 * *Files identical despite different names*

### Comparing `phono3py-3.0.2/phono3py/conductivity/kubo.py` & `phono3py-3.0.3/phono3py/conductivity/kubo.py`

 * *Files identical despite different names*

### Comparing `phono3py-3.0.2/phono3py/conductivity/rta.py` & `phono3py-3.0.3/phono3py/conductivity/rta.py`

 * *Files identical despite different names*

### Comparing `phono3py-3.0.2/phono3py/conductivity/utils.py` & `phono3py-3.0.3/phono3py/conductivity/utils.py`

 * *Files identical despite different names*

### Comparing `phono3py-3.0.2/phono3py/conductivity/wigner.py` & `phono3py-3.0.3/phono3py/conductivity/wigner.py`

 * *Files identical despite different names*

### Comparing `phono3py-3.0.2/phono3py/cui/create_force_constants.py` & `phono3py-3.0.3/phono3py/cui/create_force_constants.py`

 * *Files identical despite different names*

### Comparing `phono3py-3.0.2/phono3py/cui/create_supercells.py` & `phono3py-3.0.3/phono3py/cui/create_supercells.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-"""Utilities of main CUI script."""
+"""Command line user interface to create supercells."""
 
 # Copyright (C) 2015 Atsushi Togo
 # All rights reserved.
 #
 # This file is part of phono3py.
 #
 # Redistribution and use in source and binary forms, with or without
@@ -44,15 +44,14 @@
 )
 
 
 def create_phono3py_supercells(
     cell_info,
     settings,
     symprec,
-    output_filename=None,
     interface_mode="vasp",
     log_level=1,
 ):
     """Create displacements and supercells.
 
     Distance unit used is that for the calculator interface.
     The default unit is Angstron.
@@ -117,15 +116,15 @@
 
     if phono3py.phonon_supercell_matrix is not None:
         additional_info = get_additional_info_to_write_fc2_supercells(
             interface_mode, phono3py.phonon_supercell_matrix
         )
         write_supercells_with_displacements(
             interface_mode,
-            phono3py.supercell,
+            phono3py.phonon_supercell,
             phono3py.phonon_supercells_with_displacements,
             optional_structure_info,
             zfill_width=5,
             additional_info=additional_info,
         )
 
         if log_level:
```

### Comparing `phono3py-3.0.2/phono3py/cui/kaccum_script.py` & `phono3py-3.0.3/phono3py/cui/kaccum_script.py`

 * *Files identical despite different names*

### Comparing `phono3py-3.0.2/phono3py/cui/load.py` & `phono3py-3.0.3/phono3py/cui/load.py`

 * *Files 0% similar despite different names*

```diff
@@ -386,21 +386,22 @@
         ph3py_yaml=ph3py_yaml,
         fc3_filename=fc3_filename,
         forces_fc3_filename=forces_fc3_filename,
         phono3py_yaml_filename=phono3py_yaml_filename,
         cutoff_pair_distance=cutoff_pair_distance,
         log_level=log_level,
     )
-    read_fc["fc2"] = _set_dataset_phonon_dataset_or_fc2(
-        ph3py,
-        ph3py_yaml=ph3py_yaml,
-        fc2_filename=fc2_filename,
-        forces_fc2_filename=forces_fc2_filename,
-        log_level=log_level,
-    )
+    if ph3py.phonon_supercell_matrix is not None:
+        read_fc["fc2"] = _set_dataset_phonon_dataset_or_fc2(
+            ph3py,
+            ph3py_yaml=ph3py_yaml,
+            fc2_filename=fc2_filename,
+            forces_fc2_filename=forces_fc2_filename,
+            log_level=log_level,
+        )
 
     # Cases that dataset is in phono3py.yaml but not forces.
     if ph3py.dataset is None:
         if ph3py_yaml is not None and ph3py_yaml.dataset is not None:
             ph3py.dataset = ph3py_yaml.dataset
         if ph3py_yaml is not None and ph3py_yaml.phonon_dataset is not None:
             ph3py.phonon_dataset = ph3py_yaml.phonon_dataset
```

### Comparing `phono3py-3.0.2/phono3py/cui/phono3py_argparse.py` & `phono3py-3.0.3/phono3py/cui/phono3py_argparse.py`

 * *Files 0% similar despite different names*

```diff
@@ -678,14 +678,22 @@
         "--rse",
         dest="is_real_self_energy",
         action="store_true",
         default=False,
         help="Calculate real part of self energy",
     )
     parser.add_argument(
+        "--sp",
+        "--save-params",
+        dest="save_params",
+        action="store_true",
+        default=None,
+        help="Save parameters that can run phono3py in phono3py_params.yaml.",
+    )
+    parser.add_argument(
         "--scattering-event-class",
         dest="scattering_event_class",
         type=int,
         default=None,
         help=("Scattering event class 1 or 2 to draw imaginary part of self " "energy"),
     )
     parser.add_argument(
```

### Comparing `phono3py-3.0.2/phono3py/cui/phono3py_script.py` & `phono3py-3.0.3/phono3py/cui/phono3py_script.py`

 * *Files 12% similar despite different names*

```diff
@@ -32,73 +32,67 @@
 # CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT
 # LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN
 # ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF ADVISED OF THE
 # POSSIBILITY OF SUCH DAMAGE.
 
 from __future__ import annotations
 
-import copy
 import datetime
 import sys
-from typing import Optional, Union
 
 import numpy as np
 from phonopy.cui.collect_cell_info import collect_cell_info
-from phonopy.cui.create_force_sets import check_number_of_force_files
 from phonopy.cui.phonopy_argparse import show_deprecated_option_warnings
 from phonopy.cui.phonopy_script import (
     file_exists,
-    files_exist,
     print_end,
     print_error,
     print_error_message,
     print_version,
     set_magnetic_moments,
     store_nac_params,
 )
 from phonopy.exception import ForceCalculatorRequiredError
-from phonopy.file_IO import is_file_phonopy_yaml, parse_FORCE_SETS, write_FORCE_SETS
+from phonopy.file_IO import is_file_phonopy_yaml
 from phonopy.harmonic.force_constants import show_drift_force_constants
-from phonopy.interface.calculator import get_default_physical_units, get_force_sets
+from phonopy.interface.calculator import get_default_physical_units
 from phonopy.phonon.band_structure import get_band_qpoints
 from phonopy.structure.cells import isclose as cells_isclose
 from phonopy.units import Bohr, Hartree, VaspToTHz
 
 from phono3py import Phono3py, Phono3pyIsotope, Phono3pyJointDos
 from phono3py.cui.create_force_constants import (
     create_phono3py_force_constants,
     get_fc_calculator_params,
 )
+from phono3py.cui.create_force_sets import (
+    create_FORCE_SETS_from_FORCES_FCx,
+    create_FORCES_FC2_from_FORCE_SETS,
+    create_FORCES_FC3_and_FORCES_FC2,
+)
 from phono3py.cui.create_supercells import create_phono3py_supercells
 from phono3py.cui.load import (
     compute_force_constants_from_datasets,
     set_dataset_and_force_constants,
 )
 from phono3py.cui.phono3py_argparse import get_parser
 from phono3py.cui.settings import Phono3pyConfParser
 from phono3py.cui.show_log import (
     show_general_settings,
     show_phono3py_cells,
     show_phono3py_settings,
 )
 from phono3py.cui.triplets_info import show_num_triplets, write_grid_points
 from phono3py.file_IO import (
-    get_length_of_first_line,
-    parse_FORCES_FC2,
     read_phonon_from_hdf5,
     write_fc2_to_hdf5,
     write_fc3_to_hdf5,
-    write_FORCES_FC2,
-    write_FORCES_FC3,
     write_phonon_to_hdf5,
 )
-from phono3py.interface.phono3py_yaml import (
-    Phono3pyYaml,
-    displacements_yaml_lines_type1,
-)
+from phono3py.interface.phono3py_yaml import Phono3pyYaml
 from phono3py.phonon3.fc3 import show_drift_fc3
 from phono3py.phonon3.gruneisen import run_gruneisen_parameters
 from phono3py.phonon.grid import get_grid_point_from_address, get_ir_grid_points
 from phono3py.version import __version__
 
 # import logging
 # logging.basicConfig()
@@ -295,263 +289,14 @@
 
     confs_dict = phono3py_conf_parser.confs.copy()
     settings = phono3py_conf_parser.settings
 
     return settings, confs_dict, cell_filename
 
 
-def create_FORCES_FC2_from_FORCE_SETS_then_exit(log_level):
-    """Convert FORCE_SETS to FORCES_FC2."""
-    filename = "FORCE_SETS"
-    file_exists(filename, log_level)
-    disp_dataset = parse_FORCE_SETS(filename=filename)
-    write_FORCES_FC2(disp_dataset)
-
-    if log_level:
-        print("")
-        print("FORCES_FC2 has been created from FORCE_SETS.")
-        print("The following yaml lines should replace respective part of")
-        print("phono3py_disp.yaml made with --dim-fc2=dim_of_FORCE_SETS.")
-
-    print("")
-    print("\n".join(displacements_yaml_lines_type1(disp_dataset)))
-
-    if log_level:
-        print_end_phono3py()
-    sys.exit(0)
-
-
-def create_FORCE_SETS_from_FORCES_FCx_then_exit(
-    phonon_smat, input_filename: Optional[str], cell_filename: Optional[str], log_level
-):
-    """Convert FORCES_FC3 or FORCES_FC2 to FORCE_SETS."""
-    if cell_filename is not None:
-        disp_filename = cell_filename
-    elif input_filename is None:
-        disp_filename = "phono3py_disp.yaml"
-    else:
-        disp_filename = f"phono3py_disp.{input_filename}.yaml"
-    if phonon_smat is not None:
-        forces_filename = "FORCES_FC2"
-    else:
-        forces_filename = "FORCES_FC3"
-
-    if log_level:
-        print(f'Displacement dataset is read from "{disp_filename}".')
-        print(f'Forces are read from "{forces_filename}"')
-
-    with open(forces_filename, "r") as f:
-        len_first_line = get_length_of_first_line(f)
-
-    if len_first_line == 3:
-        file_exists(disp_filename, log_level)
-        file_exists(forces_filename, log_level)
-        ph3yml = Phono3pyYaml()
-        ph3yml.read(disp_filename)
-        if phonon_smat is None:
-            dataset = copy.deepcopy(ph3yml.dataset)
-            smat = ph3yml.supercell_matrix
-        else:
-            dataset = copy.deepcopy(ph3yml.phonon_dataset)
-            smat = ph3yml.phonon_supercell_matrix
-
-        if smat is None or (phonon_smat is not None and (phonon_smat != smat).any()):
-            if log_level:
-                print("")
-                print("Supercell matrix is inconsistent.")
-                print(f'Supercell matrix read from "{disp_filename}":')
-                print(smat)
-                print("Supercell matrix given by --dim-fc2:")
-                print(phonon_smat)
-                print_error()
-            sys.exit(1)
-
-        parse_FORCES_FC2(dataset, filename=forces_filename)
-        write_FORCE_SETS(dataset)
-
-        if log_level:
-            print("FORCE_SETS has been created.")
-            print_end_phono3py()
-    else:
-        if log_level:
-            print(
-                "The file format of %s is already readable by phonopy."
-                % forces_filename
-            )
-            print_end_phono3py()
-    sys.exit(0)
-
-
-def create_FORCES_FC3_and_FORCES_FC2_then_exit(
-    settings,
-    cell_filename: Optional[str],
-    log_level: Union[bool, int],
-):
-    """Create FORCES_FC3 and FORCES_FC2 from files."""
-    interface_mode = settings.calculator
-    ph3py_yaml = None
-
-    #####################
-    # Create FORCES_FC3 #
-    #####################
-    if settings.create_forces_fc3 or settings.create_forces_fc3_file:
-        disp_filename_candidates = [
-            "phono3py_disp.yaml",
-        ]
-        if cell_filename is not None:
-            disp_filename_candidates.insert(0, cell_filename)
-        disp_filenames = files_exist(disp_filename_candidates, log_level, is_any=True)
-        disp_filename = disp_filenames[0]
-        ph3py_yaml = Phono3pyYaml()
-        ph3py_yaml.read(disp_filename)
-        if ph3py_yaml.calculator is not None:
-            interface_mode = ph3py_yaml.calculator  # overwrite
-        disp_dataset = ph3py_yaml.dataset
-
-        if log_level:
-            print("")
-            print('Displacement dataset was read from "%s".' % disp_filename)
-
-        num_atoms = disp_dataset["natom"]
-        num_disps = len(disp_dataset["first_atoms"])
-        for d1 in disp_dataset["first_atoms"]:
-            for d2 in d1["second_atoms"]:
-                if "included" not in d2 or d2["included"]:
-                    num_disps += 1
-
-        if settings.create_forces_fc3_file:
-            file_exists(settings.create_forces_fc3_file, log_level)
-            force_filenames = [x.strip() for x in open(settings.create_forces_fc3_file)]
-        else:
-            force_filenames = settings.create_forces_fc3
-
-        for filename in force_filenames:
-            file_exists(filename, log_level)
-
-        if log_level > 0:
-            print("Number of displacements: %d" % num_disps)
-            print("Number of supercell files: %d" % len(force_filenames))
-
-        if not check_number_of_force_files(num_disps, force_filenames, disp_filename):
-            force_sets = []
-        else:
-            force_sets = get_force_sets(
-                interface_mode,
-                num_atoms,
-                force_filenames,
-                verbose=(log_level > 0),
-            )
-
-        if settings.subtract_forces:
-            force_filename = settings.subtract_forces
-            file_exists(force_filename, log_level)
-            force_set_zero = get_force_sets(
-                interface_mode,
-                num_atoms,
-                [
-                    force_filename,
-                ],
-                verbose=(log_level > 0),
-            )[0]
-            for fs in force_sets:
-                fs -= force_set_zero
-
-            if log_level > 0:
-                print(
-                    "Forces in '%s' were subtracted from supercell forces."
-                    % force_filename
-                )
-
-        if force_sets:
-            write_FORCES_FC3(disp_dataset, forces_fc3=force_sets, filename="FORCES_FC3")
-            if log_level:
-                print("")
-                print("%s has been created." % "FORCES_FC3")
-                print_end_phono3py()
-            sys.exit(0)
-        else:
-            if log_level:
-                print("")
-                print("%s could not be created." % "FORCES_FC3")
-                print_error()
-            sys.exit(1)
-
-    #####################
-    # Create FORCES_FC2 #
-    #####################
-    if settings.create_forces_fc2:
-        disp_filename_candidates = [
-            "phono3py_disp.yaml",
-        ]
-        if cell_filename is not None:
-            disp_filename_candidates.insert(0, cell_filename)
-        disp_filenames = files_exist(disp_filename_candidates, log_level, is_any=True)
-        disp_filename = disp_filenames[0]
-
-        # ph3py_yaml is not None, phono3py_disp.yaml is already read.
-        if ph3py_yaml is None:
-            ph3py_yaml = Phono3pyYaml()
-            ph3py_yaml.read(disp_filename)
-            if ph3py_yaml.calculator is not None:
-                interface_mode = ph3py_yaml.calculator  # overwrite
-        disp_dataset = ph3py_yaml.phonon_dataset
-
-        if log_level:
-            print('Displacement dataset was read from "%s".' % disp_filename)
-        num_atoms = disp_dataset["natom"]
-        num_disps = len(disp_dataset["first_atoms"])
-        force_filenames = settings.create_forces_fc2
-        for filename in force_filenames:
-            file_exists(filename, log_level)
-
-        if log_level > 0:
-            print("Number of displacements: %d" % num_disps)
-            print("Number of supercell files: %d" % len(force_filenames))
-        force_sets = get_force_sets(
-            interface_mode,
-            num_atoms,
-            force_filenames,
-            verbose=(log_level > 0),
-        )
-
-        if settings.subtract_forces:
-            force_filename = settings.subtract_forces
-            file_exists(force_filename, log_level)
-            force_set_zero = get_force_sets(
-                interface_mode,
-                num_atoms,
-                [
-                    force_filename,
-                ],
-                verbose=(log_level > 0),
-            )[0]
-            for fs in force_sets:
-                fs -= force_set_zero
-
-            if log_level > 0:
-                print(
-                    "Forces in '%s' were subtracted from supercell forces."
-                    % force_filename
-                )
-
-        if force_sets:
-            write_FORCES_FC2(disp_dataset, forces_fc2=force_sets, filename="FORCES_FC2")
-            if log_level:
-                print("")
-                print("%s has been created." % "FORCES_FC2")
-                print_end_phono3py()
-            sys.exit(0)
-        else:
-            if log_level:
-                print("")
-                print("%s could not be created." % "FORCES_FC2")
-                print_error()
-            sys.exit(1)
-
-
 def get_input_output_filenames_from_args(args):
     """Return strings inserted to input and output filenames."""
     input_filename = args.input_filename
     output_filename = args.output_filename
     if args.input_output_filename is not None:
         input_filename = args.input_output_filename
         output_filename = args.input_output_filename
@@ -1100,34 +845,48 @@
         output_yaml_filename = None
 
     settings, confs_dict, cell_filename = read_phono3py_settings(
         args, argparse_control, log_level
     )
 
     if args.force_sets_to_forces_fc2_mode:
-        create_FORCES_FC2_from_FORCE_SETS_then_exit(log_level)
+        create_FORCES_FC2_from_FORCE_SETS(log_level)
+        if log_level:
+            print_end_phono3py()
+        sys.exit(0)
     if args.force_sets_mode:
-        create_FORCE_SETS_from_FORCES_FCx_then_exit(
+        create_FORCE_SETS_from_FORCES_FCx(
             settings.phonon_supercell_matrix, input_filename, cell_filename, log_level
         )
+        if log_level:
+            print_end_phono3py()
+        sys.exit(0)
     if args.write_grid_points:
         run_mode = "write_grid_info"
     elif args.show_num_triplets:
         run_mode = "show_triplets_info"
     else:
         run_mode = None
 
     # -----------------------------------------------------------------------
     # ----------------- 'args' should not be used below. --------------------
     # -----------------------------------------------------------------------
 
     ####################################
     # Create FORCES_FC3 and FORCES_FC2 #
     ####################################
-    create_FORCES_FC3_and_FORCES_FC2_then_exit(settings, cell_filename, log_level)
+    if (
+        settings.create_forces_fc3
+        or settings.create_forces_fc3_file
+        or settings.create_forces_fc2
+    ):
+        create_FORCES_FC3_and_FORCES_FC2(settings, cell_filename, log_level=log_level)
+        if log_level:
+            print_end_phono3py()
+        sys.exit(0)
 
     ###########################################################
     # Symmetry tolerance. Distance unit depends on interface. #
     ###########################################################
     if settings.symmetry_tolerance is None:
         symprec = 1e-5
     else:
@@ -1145,15 +904,14 @@
     # Create supercells with displacements and then exit #
     ######################################################
     if settings.create_displacements:
         phono3py = create_phono3py_supercells(
             cell_info,
             settings,
             symprec,
-            output_filename=output_filename,
             interface_mode=interface_mode,
             log_level=log_level,
         )
 
         if phono3py.supercell.magnetic_moments is None:
             print("Spacegroup: %s" % phono3py.symmetry.get_international_table())
         else:
```

### Comparing `phono3py-3.0.2/phono3py/cui/settings.py` & `phono3py-3.0.3/phono3py/cui/settings.py`

 * *Files identical despite different names*

### Comparing `phono3py-3.0.2/phono3py/cui/show_log.py` & `phono3py-3.0.3/phono3py/cui/show_log.py`

 * *Files identical despite different names*

### Comparing `phono3py-3.0.2/phono3py/cui/triplets_info.py` & `phono3py-3.0.3/phono3py/cui/triplets_info.py`

 * *Files identical despite different names*

### Comparing `phono3py-3.0.2/phono3py/file_IO.py` & `phono3py-3.0.3/phono3py/file_IO.py`

 * *Files identical despite different names*

### Comparing `phono3py-3.0.2/phono3py/interface/alm.py` & `phono3py-3.0.3/phono3py/interface/alm.py`

 * *Files identical despite different names*

### Comparing `phono3py-3.0.2/phono3py/interface/calculator.py` & `phono3py-3.0.3/phono3py/interface/calculator.py`

 * *Files identical despite different names*

### Comparing `phono3py-3.0.2/phono3py/interface/fc_calculator.py` & `phono3py-3.0.3/phono3py/interface/fc_calculator.py`

 * *Files identical despite different names*

### Comparing `phono3py-3.0.2/phono3py/interface/phono3py_yaml.py` & `phono3py-3.0.3/phono3py/interface/phono3py_yaml.py`

 * *Files 4% similar despite different names*

```diff
@@ -129,22 +129,19 @@
             )
 
     def _parse_dataset(self):
         """Parse phonon_dataset.
 
         This method override PhonopyYaml._parse_dataset.
 
-        key="phonon_displacements" at v2.2 or later.
-        key="displacements" at older version than v2.2.
-
         """
         self._data.phonon_dataset = self._get_dataset(
-            self._data.phonon_supercell, key="phonon_displacements"
+            self._data.phonon_supercell, key_prefix="phonon_"
         )
-        if self._data.phonon_dataset is None:  # key="displacements"
+        if self._data.phonon_dataset is None:
             self._data.phonon_dataset = self._get_dataset(self._data.phonon_supercell)
 
     def _parse_fc3_dataset(self):
         """Parse force dataset for fc3.
 
         'duplicates' can be either dict (<v1.21) or list in phono3py.yaml.
         From v1.21, it was changed to list of list because
@@ -188,14 +185,16 @@
                 d1_id = d1["displacement_id"]
                 if disp1_id + 1 != d1_id:
                     msg = f"{d1_id} != {disp1_id + 1}. Dataset may be broken."
                     raise RuntimeError(msg)
                 data1["id"] = d1_id
             if "forces" in d1:
                 data1["forces"] = np.array(d1["forces"], dtype="double", order="C")
+            if "supercell_energy" in d1:
+                data1["supercell_energy"] = d1["supercell_energy"]
             d2_list = d1.get("paired_with")
             if d2_list is None:  # backward compatibility
                 d2_list = d1.get("second_atoms")
             for d2 in d2_list:
                 if "forces" in d2:
                     disp2_id = self._parse_fc3_dataset_type1_with_forces(
                         data1, d2, disp2_id
@@ -222,14 +221,16 @@
             d2_id = d2["displacement_id"]
             if disp2_id + 1 != d2_id:
                 msg = f"{d2_id} != {disp2_id + 1}. Dataset may be broken."
                 raise RuntimeError(msg)
             second_atom_dict["id"] = d2_id
         if "pair_distance" in d2:
             second_atom_dict["pair_distance"] = d2["pair_distance"]
+        if "supercell_energy" in d2:
+            second_atom_dict["supercell_energy"] = d2["supercell_energy"]
         disp2_id += 1
         data1["second_atoms"].append(second_atom_dict)
         return disp2_id
 
     def _parse_fc3_dataset_type1_without_forces(self, data1, d2, disp2_id):
         """Parse fc3 type1-dataset that doesn't have forces in it.
 
@@ -290,23 +291,14 @@
         )
         lines += self._primitive_yaml_lines(
             self._data.phonon_primitive, "phonon_primitive_cell"
         )
         lines += self._phonon_supercell_yaml_lines()
         return lines
 
-    def _phonon_supercell_matrix_yaml_lines(self):
-        lines = []
-        if self._data.phonon_supercell_matrix is not None:
-            lines.append("phonon_supercell_matrix:")
-            for v in self._data.supercell_matrix:
-                lines.append("- [ %3d, %3d, %3d ]" % tuple(v))
-            lines.append("")
-        return lines
-
     def _phonon_supercell_yaml_lines(self):
         lines = []
         if self._data.phonon_supercell is not None:
             s2p_map = getattr(self._data.phonon_primitive, "s2p_map", None)
             lines += self._cell_yaml_lines(
                 self._data.phonon_supercell, "phonon_supercell", s2p_map
             )
@@ -322,43 +314,47 @@
         if self._data.phonon_primitive is not None:
             return self._nac_yaml_lines_given_symbols(
                 self._data.phonon_primitive.symbols
             )
         else:
             return self._nac_yaml_lines_given_symbols(self._data.primitive.symbols)
 
-    def _displacements_yaml_lines(self, with_forces=False, key="displacements"):
+    def _displacements_yaml_lines(self, with_forces: bool = False) -> list:
         """Get YAML lines for phonon_dataset and dataset.
 
         This method override PhonopyYaml._displacements_yaml_lines.
         PhonopyYaml._displacements_yaml_lines_2types is written
         to be also used by Phono3pyYaml.
 
         """
         lines = []
         if self._data.phonon_supercell_matrix is not None:
             lines += self._displacements_yaml_lines_2types(
-                self._data.phonon_dataset, with_forces=with_forces, key=f"phonon_{key}"
+                self._data.phonon_dataset,
+                with_forces=with_forces,
+                key_prefix="phonon_",
             )
         lines += self._displacements_yaml_lines_2types(
-            self._data.dataset, with_forces=with_forces, key=key
+            self._data.dataset, with_forces=with_forces
         )
         return lines
 
     def _displacements_yaml_lines_type1(
-        self, dataset, with_forces=False, key="displacements"
-    ):
+        self, dataset: dict, with_forces: bool = False, key_prefix: str = ""
+    ) -> list:
         """Get YAML lines for type1 phonon_dataset and dataset.
 
         This method override PhonopyYaml._displacements_yaml_lines_type1.
         PhonopyYaml._displacements_yaml_lines_2types calls
         Phono3pyYaml._displacements_yaml_lines_type1.
 
         """
-        return displacements_yaml_lines_type1(dataset, with_forces=with_forces, key=key)
+        return displacements_yaml_lines_type1(
+            dataset, with_forces=with_forces, key_prefix=key_prefix
+        )
 
 
 class Phono3pyYaml(PhonopyYaml):
     """phono3py.yaml reader and writer.
 
     Details are found in the docstring of PhonopyYaml.
     The common usages are as follows:
@@ -437,37 +433,45 @@
         super().set_phonon_info(phono3py)
         self._data.phonon_supercell_matrix = phono3py.phonon_supercell_matrix
         self._data.phonon_dataset = phono3py.phonon_dataset
         self._data.phonon_primitive = phono3py.phonon_primitive
         self._data.phonon_supercell = phono3py.phonon_supercell
 
 
-def displacements_yaml_lines_type1(dataset, with_forces=False, key="displacements"):
+def displacements_yaml_lines_type1(
+    dataset: dict, with_forces: bool = False, key_prefix: str = ""
+) -> list:
     """Get YAML lines for type1 phonon_dataset and dataset.
 
     This is a function but not class method because used by other function.
 
     """
     id_offset = len(dataset["first_atoms"])
 
     if "second_atoms" in dataset["first_atoms"][0]:
         lines = ["displacement_pairs:"]
     else:
-        lines = [f"{key}:"]
+        lines = [f"{key_prefix}displacements:"]
     for disp1_id, d1 in enumerate(dataset["first_atoms"]):
         lines.append("- atom: %4d" % (d1["number"] + 1))
         lines.append("  displacement:")
         lines.append("    [ %19.16f, %19.16f, %19.16f ]" % tuple(d1["displacement"]))
         if "id" in d1:
             assert disp1_id + 1 == d1["id"]
         lines.append(f"  displacement_id: {disp1_id + 1}")
         if with_forces and "forces" in d1:
             lines.append("  forces:")
             for v in d1["forces"]:
                 lines.append("  - [ %19.16f, %19.16f, %19.16f ]" % tuple(v))
+            if "supercell_energy" in d1:
+                lines.append(
+                    "  supercell_energy: {energy:.8f}".format(
+                        energy=d1["supercell_energy"]
+                    )
+                )
         if "second_atoms" in d1:
             ret_lines, id_offset = _second_displacements_yaml_lines(
                 d1["second_atoms"], id_offset, with_forces=with_forces
             )
             lines += ret_lines
     lines.append("")
 
@@ -538,14 +542,20 @@
                 if "id" in dataset2[j]:
                     assert dataset2[j]["id"] == disp2_id
                 lines.append("    displacement_id: %d" % disp2_id)
 
                 lines.append("    forces:")
                 for v in dataset2[j]["forces"]:
                     lines.append("    - [ %19.16f, %19.16f, %19.16f ]" % tuple(v))
+                if "supercell_energy" in dataset2[j]:
+                    lines.append(
+                        "    supercell_energy: {energy:.8f}".format(
+                            energy=dataset2[j]["supercell_energy"]
+                        )
+                    )
         else:
             lines.append("  - atom: %4d" % (i + 1))
             lines.append(
                 "    pair_distance: %.8f" % dataset2[indices_eq_i[0]]["pair_distance"]
             )
             if "included" in dataset2[indices_eq_i[0]]:
                 included = dataset2[indices_eq_i[0]]["included"]
```

### Comparing `phono3py-3.0.2/phono3py/other/isotope.py` & `phono3py-3.0.3/phono3py/other/isotope.py`

 * *Files identical despite different names*

### Comparing `phono3py-3.0.2/phono3py/other/kaccum.py` & `phono3py-3.0.3/phono3py/other/kaccum.py`

 * *Files identical despite different names*

### Comparing `phono3py-3.0.2/phono3py/other/tetrahedron_method.py` & `phono3py-3.0.3/phono3py/other/tetrahedron_method.py`

 * *Files identical despite different names*

### Comparing `phono3py-3.0.2/phono3py/phonon/func.py` & `phono3py-3.0.3/phono3py/phonon/func.py`

 * *Files identical despite different names*

### Comparing `phono3py-3.0.2/phono3py/phonon/grid.py` & `phono3py-3.0.3/phono3py/phonon/grid.py`

 * *Files identical despite different names*

### Comparing `phono3py-3.0.2/phono3py/phonon/group_velocity_matrix.py` & `phono3py-3.0.3/phono3py/phonon/group_velocity_matrix.py`

 * *Files identical despite different names*

### Comparing `phono3py-3.0.2/phono3py/phonon/heat_capacity_matrix.py` & `phono3py-3.0.3/phono3py/phonon/heat_capacity_matrix.py`

 * *Files identical despite different names*

### Comparing `phono3py-3.0.2/phono3py/phonon/solver.py` & `phono3py-3.0.3/phono3py/phonon/solver.py`

 * *Files identical despite different names*

### Comparing `phono3py-3.0.2/phono3py/phonon/velocity_operator.py` & `phono3py-3.0.3/phono3py/phonon/velocity_operator.py`

 * *Files identical despite different names*

### Comparing `phono3py-3.0.2/phono3py/phonon3/collision_matrix.py` & `phono3py-3.0.3/phono3py/phonon3/collision_matrix.py`

 * *Files identical despite different names*

### Comparing `phono3py-3.0.2/phono3py/phonon3/dataset.py` & `phono3py-3.0.3/phono3py/phonon3/dataset.py`

 * *Files identical despite different names*

### Comparing `phono3py-3.0.2/phono3py/phonon3/displacement_fc3.py` & `phono3py-3.0.3/phono3py/phonon3/displacement_fc3.py`

 * *Files identical despite different names*

### Comparing `phono3py-3.0.2/phono3py/phonon3/fc3.py` & `phono3py-3.0.3/phono3py/phonon3/fc3.py`

 * *Files identical despite different names*

### Comparing `phono3py-3.0.2/phono3py/phonon3/gruneisen.py` & `phono3py-3.0.3/phono3py/phonon3/gruneisen.py`

 * *Files identical despite different names*

### Comparing `phono3py-3.0.2/phono3py/phonon3/imag_self_energy.py` & `phono3py-3.0.3/phono3py/phonon3/imag_self_energy.py`

 * *Files identical despite different names*

### Comparing `phono3py-3.0.2/phono3py/phonon3/interaction.py` & `phono3py-3.0.3/phono3py/phonon3/interaction.py`

 * *Files identical despite different names*

### Comparing `phono3py-3.0.2/phono3py/phonon3/joint_dos.py` & `phono3py-3.0.3/phono3py/phonon3/joint_dos.py`

 * *Files identical despite different names*

### Comparing `phono3py-3.0.2/phono3py/phonon3/real_self_energy.py` & `phono3py-3.0.3/phono3py/phonon3/real_self_energy.py`

 * *Files identical despite different names*

### Comparing `phono3py-3.0.2/phono3py/phonon3/real_to_reciprocal.py` & `phono3py-3.0.3/phono3py/phonon3/real_to_reciprocal.py`

 * *Files identical despite different names*

### Comparing `phono3py-3.0.2/phono3py/phonon3/reciprocal_to_normal.py` & `phono3py-3.0.3/phono3py/phonon3/reciprocal_to_normal.py`

 * *Files identical despite different names*

### Comparing `phono3py-3.0.2/phono3py/phonon3/spectral_function.py` & `phono3py-3.0.3/phono3py/phonon3/spectral_function.py`

 * *Files identical despite different names*

### Comparing `phono3py-3.0.2/phono3py/phonon3/triplets.py` & `phono3py-3.0.3/phono3py/phonon3/triplets.py`

 * *Files identical despite different names*

### Comparing `phono3py-3.0.2/phono3py/sscha/sscha.py` & `phono3py-3.0.3/phono3py/sscha/sscha.py`

 * *Files identical despite different names*

### Comparing `phono3py-3.0.2/phono3py/version.py` & `phono3py-3.0.3/phono3py/version.py`

 * *Files 0% similar despite different names*

```diff
@@ -30,8 +30,8 @@
 # BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES;
 # LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER
 # CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT
 # LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN
 # ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF ADVISED OF THE
 # POSSIBILITY OF SUCH DAMAGE.
 
-__version__ = "3.0.2"
+__version__ = "3.0.3"
```

### Comparing `phono3py-3.0.2/phono3py.egg-info/SOURCES.txt` & `phono3py-3.0.3/phono3py.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -16,14 +16,15 @@
 ./phono3py/conductivity/direct_solution.py
 ./phono3py/conductivity/kubo.py
 ./phono3py/conductivity/rta.py
 ./phono3py/conductivity/utils.py
 ./phono3py/conductivity/wigner.py
 ./phono3py/cui/__init__.py
 ./phono3py/cui/create_force_constants.py
+./phono3py/cui/create_force_sets.py
 ./phono3py/cui/create_supercells.py
 ./phono3py/cui/kaccum_script.py
 ./phono3py/cui/load.py
 ./phono3py/cui/phono3py_argparse.py
 ./phono3py/cui/phono3py_script.py
 ./phono3py/cui/settings.py
 ./phono3py/cui/show_log.py
@@ -182,19 +183,23 @@
 scripts/phono3py-kaccum
 scripts/phono3py-kdeplot
 scripts/phono3py-load
 test/AgNO2_cell.yaml
 test/BORN_NaCl
 test/FORCES_FC3_si_pbesol
 test/FORCE_SETS_NaCl
+test/Si-111-222-fd.tar.xz
+test/Si-111-222-rd.tar.xz
 test/conftest.py
 test/phono3py_params-Si111-rd.yaml.xz
 test/phono3py_params_AlN332.yaml.xz
 test/phono3py_params_NaCl111.yaml
 test/phono3py_params_NaCl222.yaml.xz
+test/phono3py_params_Si-111-222-fd.yaml.xz
+test/phono3py_params_Si-111-222-rd.yaml.xz
 test/phono3py_params_Si-111-222.yaml
 test/phono3py_params_Si111.yaml
 test/phono3py_si_pbesol.yaml
 test/phonopy_disp_NaCl.yaml
 test/phonopy_params-Si111-iterha.yaml.gz
 test/phonopy_params_Si.yaml
 test/api/test_api_phono3py.py
```

### Comparing `phono3py-3.0.2/scripts/phono3py` & `phono3py-3.0.3/scripts/phono3py`

 * *Files identical despite different names*

### Comparing `phono3py-3.0.2/scripts/phono3py-coleigplot` & `phono3py-3.0.3/scripts/phono3py-coleigplot`

 * *Files identical despite different names*

### Comparing `phono3py-3.0.2/scripts/phono3py-kaccum` & `phono3py-3.0.3/scripts/phono3py-kaccum`

 * *Files identical despite different names*

### Comparing `phono3py-3.0.2/scripts/phono3py-kdeplot` & `phono3py-3.0.3/scripts/phono3py-kdeplot`

 * *Files identical despite different names*

### Comparing `phono3py-3.0.2/scripts/phono3py-load` & `phono3py-3.0.3/scripts/phono3py-load`

 * *Files identical despite different names*

### Comparing `phono3py-3.0.2/setup.py` & `phono3py-3.0.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -322,15 +322,15 @@
         install_requires=[
             "numpy>=1.17.0",
             "scipy",
             "PyYAML>=5.3",
             "matplotlib>=2.2.2",
             "h5py>=3.0",
             "spglib>=2.0",
-            "phonopy>=2.22,<2.23",
+            "phonopy>=2.23,<2.24",
         ],
         provides=["phono3py"],
         scripts=scripts_phono3py,
         ext_modules=_get_extensions(build_dir),
     )
     _clean_cmake(build_dir)
```

### Comparing `phono3py-3.0.2/test/AgNO2_cell.yaml` & `phono3py-3.0.3/test/AgNO2_cell.yaml`

 * *Files identical despite different names*

### Comparing `phono3py-3.0.2/test/FORCES_FC3_si_pbesol` & `phono3py-3.0.3/test/FORCES_FC3_si_pbesol`

 * *Files identical despite different names*

### Comparing `phono3py-3.0.2/test/FORCE_SETS_NaCl` & `phono3py-3.0.3/test/FORCE_SETS_NaCl`

 * *Files identical despite different names*

### Comparing `phono3py-3.0.2/test/conductivity/test_kappa_LBTE.py` & `phono3py-3.0.3/test/conductivity/test_kappa_LBTE.py`

 * *Files identical despite different names*

### Comparing `phono3py-3.0.2/test/conductivity/test_kappa_LBTE_Wigner.py` & `phono3py-3.0.3/test/conductivity/test_kappa_LBTE_Wigner.py`

 * *Files identical despite different names*

### Comparing `phono3py-3.0.2/test/conductivity/test_kappa_RTA.py` & `phono3py-3.0.3/test/conductivity/test_kappa_RTA.py`

 * *Files identical despite different names*

### Comparing `phono3py-3.0.2/test/conductivity/test_kappa_RTA_Wigner.py` & `phono3py-3.0.3/test/conductivity/test_kappa_RTA_Wigner.py`

 * *Files identical despite different names*

### Comparing `phono3py-3.0.2/test/conftest.py` & `phono3py-3.0.3/test/conftest.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 """Pytest conftest.py."""
 
+import tarfile
 from pathlib import Path
 
 import numpy as np
 import phonopy
 import pytest
 from phonopy import Phonopy
 from phonopy.interface.phonopy_yaml import read_cell_yaml
@@ -479,14 +480,28 @@
         yaml_filename,
         make_r0_average=not enable_v2,
         log_level=1,
     )
 
 
 @pytest.fixture(scope="session")
+def si_111_222_fd() -> Phono3py:
+    """Return Phono3py class instance of Si-1x1x1-2x2x2 FD."""
+    yaml_filename = cwd / "phono3py_params_Si-111-222-fd.yaml.xz"
+    return phono3py.load(yaml_filename, produce_fc=False, log_level=1)
+
+
+@pytest.fixture(scope="session")
+def si_111_222_rd() -> Phono3py:
+    """Return Phono3py class instance of Si-1x1x1-2x2x2 RD."""
+    yaml_filename = cwd / "phono3py_params_Si-111-222-rd.yaml.xz"
+    return phono3py.load(yaml_filename, produce_fc=False, log_level=1)
+
+
+@pytest.fixture(scope="session")
 def ph_nacl() -> Phonopy:
     """Return Phonopy class instance of NaCl 2x2x2."""
     yaml_filename = cwd / "phonopy_disp_NaCl.yaml"
     force_sets_filename = cwd / "FORCE_SETS_NaCl"
     born_filename = cwd / "BORN_NaCl"
     return phonopy.load(
         yaml_filename,
@@ -504,7 +519,80 @@
     yaml_filename = cwd / "phonopy_params_Si.yaml"
     return phonopy.load(
         yaml_filename,
         is_compact_fc=False,
         log_level=1,
         produce_fc=True,
     )
+
+
+@pytest.fixture(scope="session")
+def si_111_222_fd_raw_data() -> tarfile.TarFile:
+    """Return Si fc3 111 fc2 222 vasp inputs.
+
+    tar.getnames()
+    ['Si-111-222-fd',
+     'Si-111-222-fd/vasprun-001.xml',
+     'Si-111-222-fd/vasprun-015.xml',
+     'Si-111-222-fd/vasprun-014.xml',
+     'Si-111-222-fd/vasprun-000.xml',
+     'Si-111-222-fd/vasprun-016.xml',
+     'Si-111-222-fd/vasprun-002.xml',
+     'Si-111-222-fd/vasprun-003.xml',
+     'Si-111-222-fd/vasprun-013.xml',
+     'Si-111-222-fd/vasprun-007.xml',
+     'Si-111-222-fd/vasprun-fc2-000.xml',
+     'Si-111-222-fd/vasprun-fc2-001.xml',
+     'Si-111-222-fd/vasprun-006.xml',
+     'Si-111-222-fd/vasprun-012.xml',
+     'Si-111-222-fd/vasprun-004.xml',
+     'Si-111-222-fd/vasprun-010.xml',
+     'Si-111-222-fd/vasprun-011.xml',
+     'Si-111-222-fd/vasprun-005.xml',
+     'Si-111-222-fd/phono3py_disp.yaml',
+     'Si-111-222-fd/vasprun-008.xml',
+     'Si-111-222-fd/vasprun-009.xml']
+    member = tar.getmember("Si-111-222-fd/phono3py_disp.yaml")
+    tar.extractfile(member)  -> byte file object
+
+    """
+    tar = tarfile.open(cwd / "Si-111-222-fd.tar.xz")
+    return tar
+
+
+@pytest.fixture(scope="session")
+def si_111_222_rd_raw_data() -> tarfile.TarFile:
+    """Return Si fc3 111 fc2 222 vasp inputs.
+
+    tar.getnames()
+    ['Si-111-222-rd',
+     'Si-111-222-rd/vasprun-001.xml',
+     'Si-111-222-rd/vasprun-015.xml',
+     'Si-111-222-rd/vasprun-014.xml',
+     'Si-111-222-rd/vasprun-000.xml',
+     'Si-111-222-rd/vasprun-016.xml',
+     'Si-111-222-rd/vasprun-002.xml',
+     'Si-111-222-rd/vasprun-003.xml',
+     'Si-111-222-rd/vasprun-017.xml',
+     'Si-111-222-rd/vasprun-013.xml',
+     'Si-111-222-rd/vasprun-007.xml',
+     'Si-111-222-rd/vasprun-fc2-000.xml',
+     'Si-111-222-rd/vasprun-fc2-001.xml',
+     'Si-111-222-rd/vasprun-006.xml',
+     'Si-111-222-rd/vasprun-012.xml',
+     'Si-111-222-rd/vasprun-004.xml',
+     'Si-111-222-rd/vasprun-010.xml',
+     'Si-111-222-rd/vasprun-fc2-002.xml',
+     'Si-111-222-rd/vasprun-011.xml',
+     'Si-111-222-rd/vasprun-005.xml',
+     'Si-111-222-rd/phono3py_disp.yaml',
+     'Si-111-222-rd/vasprun-020.xml',
+     'Si-111-222-rd/vasprun-008.xml',
+     'Si-111-222-rd/vasprun-009.xml',
+     'Si-111-222-rd/vasprun-019.xml',
+     'Si-111-222-rd/vasprun-018.xml']
+    member = tar.getmember("Si-111-222-rd/phono3py_disp.yaml")
+    tar.extractfile(member)  -> byte file object
+
+    """
+    tar = tarfile.open(cwd / "Si-111-222-fd.tar.xz")
+    return tar
```

### Comparing `phono3py-3.0.2/test/cui/phono3py_params-qe-Si222.yaml.xz` & `phono3py-3.0.3/test/cui/phono3py_params-qe-Si222.yaml.xz`

 * *Files identical despite different names*

### Comparing `phono3py-3.0.2/test/cui/test_phono3py_load_script.py` & `phono3py-3.0.3/test/cui/test_phono3py_load_script.py`

 * *Files identical despite different names*

### Comparing `phono3py-3.0.2/test/file_IO/test_file_IO.py` & `phono3py-3.0.3/test/file_IO/test_file_IO.py`

 * *Files identical despite different names*

### Comparing `phono3py-3.0.2/test/interface/test_phono3py_yaml.py` & `phono3py-3.0.3/test/interface/test_phono3py_yaml.py`

 * *Files identical despite different names*

### Comparing `phono3py-3.0.2/test/other/test_isotope.py` & `phono3py-3.0.3/test/other/test_isotope.py`

 * *Files identical despite different names*

### Comparing `phono3py-3.0.2/test/other/test_kaccum.py` & `phono3py-3.0.3/test/other/test_kaccum.py`

 * *Files identical despite different names*

### Comparing `phono3py-3.0.2/test/phono3py_params-Si111-rd.yaml.xz` & `phono3py-3.0.3/test/phono3py_params-Si111-rd.yaml.xz`

 * *Files identical despite different names*

### Comparing `phono3py-3.0.2/test/phono3py_params_AlN332.yaml.xz` & `phono3py-3.0.3/test/phono3py_params_AlN332.yaml.xz`

 * *Files identical despite different names*

### Comparing `phono3py-3.0.2/test/phono3py_params_NaCl111.yaml` & `phono3py-3.0.3/test/phono3py_params_NaCl111.yaml`

 * *Files identical despite different names*

### Comparing `phono3py-3.0.2/test/phono3py_params_NaCl222.yaml.xz` & `phono3py-3.0.3/test/phono3py_params_NaCl222.yaml.xz`

 * *Files identical despite different names*

### Comparing `phono3py-3.0.2/test/phono3py_params_Si-111-222.yaml` & `phono3py-3.0.3/test/phono3py_params_Si-111-222.yaml`

 * *Files identical despite different names*

### Comparing `phono3py-3.0.2/test/phono3py_params_Si111.yaml` & `phono3py-3.0.3/test/phono3py_params_Si111.yaml`

 * *Files identical despite different names*

### Comparing `phono3py-3.0.2/test/phono3py_si_pbesol.yaml` & `phono3py-3.0.3/test/phono3py_si_pbesol.yaml`

 * *Files identical despite different names*

### Comparing `phono3py-3.0.2/test/phonon/test_grid.py` & `phono3py-3.0.3/test/phonon/test_grid.py`

 * *Files identical despite different names*

### Comparing `phono3py-3.0.2/test/phonon/test_velocity_operator.py` & `phono3py-3.0.3/test/phonon/test_velocity_operator.py`

 * *Files identical despite different names*

### Comparing `phono3py-3.0.2/test/phonon3/test_displacements.py` & `phono3py-3.0.3/test/phonon3/test_displacements.py`

 * *Files identical despite different names*

### Comparing `phono3py-3.0.2/test/phonon3/test_fc3.py` & `phono3py-3.0.3/test/phonon3/test_fc3.py`

 * *Files identical despite different names*

### Comparing `phono3py-3.0.2/test/phonon3/test_imag_self_energy.py` & `phono3py-3.0.3/test/phonon3/test_imag_self_energy.py`

 * *Files identical despite different names*

### Comparing `phono3py-3.0.2/test/phonon3/test_interaction.py` & `phono3py-3.0.3/test/phonon3/test_interaction.py`

 * *Files identical despite different names*

### Comparing `phono3py-3.0.2/test/phonon3/test_joint_dos.py` & `phono3py-3.0.3/test/phonon3/test_joint_dos.py`

 * *Files identical despite different names*

### Comparing `phono3py-3.0.2/test/phonon3/test_real_self_energy.py` & `phono3py-3.0.3/test/phonon3/test_real_self_energy.py`

 * *Files identical despite different names*

### Comparing `phono3py-3.0.2/test/phonon3/test_spectral_function.py` & `phono3py-3.0.3/test/phonon3/test_spectral_function.py`

 * *Files identical despite different names*

### Comparing `phono3py-3.0.2/test/phonon3/test_triplets.py` & `phono3py-3.0.3/test/phonon3/test_triplets.py`

 * *Files identical despite different names*

### Comparing `phono3py-3.0.2/test/phonopy_disp_NaCl.yaml` & `phono3py-3.0.3/test/phonopy_disp_NaCl.yaml`

 * *Files identical despite different names*

### Comparing `phono3py-3.0.2/test/phonopy_params-Si111-iterha.yaml.gz` & `phono3py-3.0.3/test/phonopy_params-Si111-iterha.yaml.gz`

 * *Files identical despite different names*

### Comparing `phono3py-3.0.2/test/phonopy_params_Si.yaml` & `phono3py-3.0.3/test/phonopy_params_Si.yaml`

 * *Files identical despite different names*

### Comparing `phono3py-3.0.2/test/sscha/test_sscha.py` & `phono3py-3.0.3/test/sscha/test_sscha.py`

 * *Files identical despite different names*

