# Comparing `tmp/MulensModel-2.7.2.tar.gz` & `tmp/MulensModel-2.8.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "MulensModel-2.7.2.tar", last modified: Mon Mar 21 16:19:46 2022, max compression
+gzip compressed data, was "MulensModel-2.8.1.tar", last modified: Sat Apr  9 09:50:59 2022, max compression
```

## Comparing `MulensModel-2.7.2.tar` & `MulensModel-2.8.1.tar`

### file list

```diff
@@ -1,148 +1,154 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-21 16:19:46.698057 MulensModel-2.7.2/
--rw-r--r--   0 runner    (1001) docker     (121)     1081 2022-03-21 16:19:38.000000 MulensModel-2.7.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)      100 2022-03-21 16:19:38.000000 MulensModel-2.7.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)      403 2022-03-21 16:19:46.698057 MulensModel-2.7.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     3737 2022-03-21 16:19:38.000000 MulensModel-2.7.2/README.md
--rw-r--r--   0 runner    (1001) docker     (121)      100 2022-03-21 16:19:38.000000 MulensModel-2.7.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)       63 2022-03-21 16:19:38.000000 MulensModel-2.7.2/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-03-21 16:19:46.698057 MulensModel-2.7.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1794 2022-03-21 16:19:38.000000 MulensModel-2.7.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-21 16:19:46.658055 MulensModel-2.7.2/source/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-21 16:19:46.662055 MulensModel-2.7.2/source/AdaptiveContouring/
--rw-r--r--   0 runner    (1001) docker     (121)      841 2022-03-21 16:19:38.000000 MulensModel-2.7.2/source/AdaptiveContouring/AdaptiveContouring_wrapper.c
--rw-r--r--   0 runner    (1001) docker     (121)      652 2022-03-21 16:19:38.000000 MulensModel-2.7.2/source/AdaptiveContouring/Makefile
--rw-r--r--   0 runner    (1001) docker     (121)     3970 2022-03-21 16:19:38.000000 MulensModel-2.7.2/source/AdaptiveContouring/README.adaptivecontouring
--rw-r--r--   0 runner    (1001) docker     (121)     1271 2022-03-21 16:19:38.000000 MulensModel-2.7.2/source/AdaptiveContouring/ac_wrap.c
--rw-r--r--   0 runner    (1001) docker     (121)    59956 2022-03-21 16:19:38.000000 MulensModel-2.7.2/source/AdaptiveContouring/adaptive_contour.c
--rw-r--r--   0 runner    (1001) docker     (121)     7793 2022-03-21 16:19:38.000000 MulensModel-2.7.2/source/AdaptiveContouring/binary_pt.c
--rw-r--r--   0 runner    (1001) docker     (121)     4382 2022-03-21 16:19:38.000000 MulensModel-2.7.2/source/AdaptiveContouring/binext_adap.c
--rw-r--r--   0 runner    (1001) docker     (121)     2031 2022-03-21 16:19:38.000000 MulensModel-2.7.2/source/AdaptiveContouring/complex.c
--rw-r--r--   0 runner    (1001) docker     (121)      531 2022-03-21 16:19:38.000000 MulensModel-2.7.2/source/AdaptiveContouring/complex.h
--rw-r--r--   0 runner    (1001) docker     (121)     1054 2022-03-21 16:19:38.000000 MulensModel-2.7.2/source/AdaptiveContouring/dyn_array.c
--rw-r--r--   0 runner    (1001) docker     (121)    57862 2022-03-21 16:19:38.000000 MulensModel-2.7.2/source/AdaptiveContouring/erdlcaust.c
--rw-r--r--   0 runner    (1001) docker     (121)     6443 2022-03-21 16:19:38.000000 MulensModel-2.7.2/source/AdaptiveContouring/integrate.c
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-21 16:19:46.670055 MulensModel-2.7.2/source/MulensModel/
--rw-r--r--   0 runner    (1001) docker     (121)     1235 2022-03-21 16:19:38.000000 MulensModel-2.7.2/source/MulensModel/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    28927 2022-03-21 16:19:38.000000 MulensModel-2.7.2/source/MulensModel/binarylens.py
--rw-r--r--   0 runner    (1001) docker     (121)     5563 2022-03-21 16:19:38.000000 MulensModel-2.7.2/source/MulensModel/caustics.py
--rw-r--r--   0 runner    (1001) docker     (121)     5370 2022-03-21 16:19:38.000000 MulensModel-2.7.2/source/MulensModel/coordinates.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-21 16:19:46.674056 MulensModel-2.7.2/source/MulensModel/data/
--rw-r--r--   0 runner    (1001) docker     (121)  1555125 2022-03-21 16:19:38.000000 MulensModel-2.7.2/source/MulensModel/data/WFIRST_1827.dat
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-21 16:19:46.674056 MulensModel-2.7.2/source/MulensModel/data/ephemeris_files/
--rw-r--r--   0 runner    (1001) docker     (121)    41053 2022-03-21 16:19:38.000000 MulensModel-2.7.2/source/MulensModel/data/ephemeris_files/K2_ephemeris_01.dat
--rw-r--r--   0 runner    (1001) docker     (121)    83691 2022-03-21 16:19:38.000000 MulensModel-2.7.2/source/MulensModel/data/ephemeris_files/Spitzer_ephemeris_01.dat
--rw-r--r--   0 runner    (1001) docker     (121)   149352 2022-03-21 16:19:38.000000 MulensModel-2.7.2/source/MulensModel/data/ephemeris_files/Spitzer_ephemeris_02.dat
--rw-r--r--   0 runner    (1001) docker     (121)    18781 2022-03-21 16:19:38.000000 MulensModel-2.7.2/source/MulensModel/data/interpolate_elliptic_integral_1_2.dat
--rw-r--r--   0 runner    (1001) docker     (121)     1994 2022-03-21 16:19:38.000000 MulensModel-2.7.2/source/MulensModel/data/interpolate_elliptic_integral_1_2.py
--rw-r--r--   0 runner    (1001) docker     (121)   222778 2022-03-21 16:19:38.000000 MulensModel-2.7.2/source/MulensModel/data/interpolate_elliptic_integral_3.dat
--rw-r--r--   0 runner    (1001) docker     (121)     2981 2022-03-21 16:19:38.000000 MulensModel-2.7.2/source/MulensModel/data/interpolate_elliptic_integral_3.py
--rw-r--r--   0 runner    (1001) docker     (121)   224553 2022-03-21 16:19:38.000000 MulensModel-2.7.2/source/MulensModel/data/interpolation_table_b0b1_v1.dat
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-21 16:19:46.658055 MulensModel-2.7.2/source/MulensModel/data/photometry_files/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-21 16:19:46.674056 MulensModel-2.7.2/source/MulensModel/data/photometry_files/KB180003/
--rw-r--r--   0 runner    (1001) docker     (121)      156 2022-03-21 16:19:38.000000 MulensModel-2.7.2/source/MulensModel/data/photometry_files/KB180003/00README.txt
--rw-r--r--   0 runner    (1001) docker     (121)    17761 2022-03-21 16:19:38.000000 MulensModel-2.7.2/source/MulensModel/data/photometry_files/KB180003/KMTA12_I.pysis
--rw-r--r--   0 runner    (1001) docker     (121)     3995 2022-03-21 16:19:38.000000 MulensModel-2.7.2/source/MulensModel/data/photometry_files/KB180003/KMTA14_I.pysis
--rw-r--r--   0 runner    (1001) docker     (121)     4585 2022-03-21 16:19:38.000000 MulensModel-2.7.2/source/MulensModel/data/photometry_files/KB180003/KMTC12_I.pysis
--rw-r--r--   0 runner    (1001) docker     (121)    10013 2022-03-21 16:19:38.000000 MulensModel-2.7.2/source/MulensModel/data/photometry_files/KB180003/KMTC14_I.pysis
--rw-r--r--   0 runner    (1001) docker     (121)     2225 2022-03-21 16:19:38.000000 MulensModel-2.7.2/source/MulensModel/data/photometry_files/KB180003/KMTS12_I.pysis
--rw-r--r--   0 runner    (1001) docker     (121)     3346 2022-03-21 16:19:38.000000 MulensModel-2.7.2/source/MulensModel/data/photometry_files/KB180003/KMTS14_I.pysis
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-21 16:19:46.678056 MulensModel-2.7.2/source/MulensModel/data/photometry_files/MB08310/
--rw-r--r--   0 runner    (1001) docker     (121)     5913 2022-03-21 16:19:38.000000 MulensModel-2.7.2/source/MulensModel/data/photometry_files/MB08310/Auck_0300089_PLC_001.tbl
--rw-r--r--   0 runner    (1001) docker     (121)    10231 2022-03-21 16:19:38.000000 MulensModel-2.7.2/source/MulensModel/data/photometry_files/MB08310/Bron_0300089_PLC_002.tbl
--rw-r--r--   0 runner    (1001) docker     (121)    17693 2022-03-21 16:19:38.000000 MulensModel-2.7.2/source/MulensModel/data/photometry_files/MB08310/CTIO_H_0300089_PLC_004.tbl
--rw-r--r--   0 runner    (1001) docker     (121)     4108 2022-03-21 16:19:38.000000 MulensModel-2.7.2/source/MulensModel/data/photometry_files/MB08310/CTIO_I_0300089_PLC_005.tbl
--rw-r--r--   0 runner    (1001) docker     (121)     2144 2022-03-21 16:19:38.000000 MulensModel-2.7.2/source/MulensModel/data/photometry_files/MB08310/Canopus_0300089_PLC_003.tbl
--rw-r--r--   0 runner    (1001) docker     (121)     4420 2022-03-21 16:19:38.000000 MulensModel-2.7.2/source/MulensModel/data/photometry_files/MB08310/Danish_0300089_PLC_006.tbl
--rw-r--r--   0 runner    (1001) docker     (121)   170275 2022-03-21 16:19:38.000000 MulensModel-2.7.2/source/MulensModel/data/photometry_files/MB08310/MOA_0300089_PLC_007.tbl
--rw-r--r--   0 runner    (1001) docker     (121)      417 2022-03-21 16:19:38.000000 MulensModel-2.7.2/source/MulensModel/data/photometry_files/MB08310/README.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-21 16:19:46.678056 MulensModel-2.7.2/source/MulensModel/data/photometry_files/OB03235/
--rw-r--r--   0 runner    (1001) docker     (121)    80276 2022-03-21 16:19:38.000000 MulensModel-2.7.2/source/MulensModel/data/photometry_files/OB03235/OB03235_MOA.tbl.txt
--rw-r--r--   0 runner    (1001) docker     (121)    18686 2022-03-21 16:19:38.000000 MulensModel-2.7.2/source/MulensModel/data/photometry_files/OB03235/OB03235_OGLE.tbl.txt
--rw-r--r--   0 runner    (1001) docker     (121)      429 2022-03-21 16:19:38.000000 MulensModel-2.7.2/source/MulensModel/data/photometry_files/OB03235/README.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-21 16:19:46.678056 MulensModel-2.7.2/source/MulensModel/data/photometry_files/OB05086/
--rw-r--r--   0 runner    (1001) docker     (121)      255 2022-03-21 16:19:38.000000 MulensModel-2.7.2/source/MulensModel/data/photometry_files/OB05086/README.txt
--rw-r--r--   0 runner    (1001) docker     (121)    15360 2022-03-21 16:19:38.000000 MulensModel-2.7.2/source/MulensModel/data/photometry_files/OB05086/starBLG234.6.I.218982.dat
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-21 16:19:46.678056 MulensModel-2.7.2/source/MulensModel/data/photometry_files/OB08092/
--rw-r--r--   0 runner    (1001) docker     (121)      175 2022-03-21 16:19:38.000000 MulensModel-2.7.2/source/MulensModel/data/photometry_files/OB08092/README.txt
--rw-r--r--   0 runner    (1001) docker     (121)     9958 2022-03-21 16:19:38.000000 MulensModel-2.7.2/source/MulensModel/data/photometry_files/OB08092/phot_ob08092_O4.dat
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-21 16:19:46.678056 MulensModel-2.7.2/source/MulensModel/data/photometry_files/OB140939/
--rw-r--r--   0 runner    (1001) docker     (121)      412 2022-03-21 16:19:38.000000 MulensModel-2.7.2/source/MulensModel/data/photometry_files/OB140939/README.txt
--rw-r--r--   0 runner    (1001) docker     (121)    18449 2022-03-21 16:19:38.000000 MulensModel-2.7.2/source/MulensModel/data/photometry_files/OB140939/ob140939_OGLE.dat
--rw-r--r--   0 runner    (1001) docker     (121)      899 2022-03-21 16:19:38.000000 MulensModel-2.7.2/source/MulensModel/data/photometry_files/OB140939/ob140939_Spitzer.dat
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-21 16:19:46.678056 MulensModel-2.7.2/source/MulensModel/data/photometry_files/OB161195/
--rw-r--r--   0 runner    (1001) docker     (121)    49569 2022-03-21 16:19:38.000000 MulensModel-2.7.2/source/MulensModel/data/photometry_files/OB161195/KCT01I.dat
--rw-r--r--   0 runner    (1001) docker     (121)    46159 2022-03-21 16:19:38.000000 MulensModel-2.7.2/source/MulensModel/data/photometry_files/OB161195/KCT41I.dat
--rw-r--r--   0 runner    (1001) docker     (121)    35495 2022-03-21 16:19:38.000000 MulensModel-2.7.2/source/MulensModel/data/photometry_files/OB161195/KCT42I.dat
--rw-r--r--   0 runner    (1001) docker     (121)    42253 2022-03-21 16:19:38.000000 MulensModel-2.7.2/source/MulensModel/data/photometry_files/OB161195/KSA01I.dat
--rw-r--r--   0 runner    (1001) docker     (121)    38161 2022-03-21 16:19:38.000000 MulensModel-2.7.2/source/MulensModel/data/photometry_files/OB161195/KSA41I.dat
--rw-r--r--   0 runner    (1001) docker     (121)    33573 2022-03-21 16:19:38.000000 MulensModel-2.7.2/source/MulensModel/data/photometry_files/OB161195/KSA42I.dat
--rw-r--r--   0 runner    (1001) docker     (121)    24614 2022-03-21 16:19:38.000000 MulensModel-2.7.2/source/MulensModel/data/photometry_files/OB161195/KSS01I.dat
--rw-r--r--   0 runner    (1001) docker     (121)    28800 2022-03-21 16:19:38.000000 MulensModel-2.7.2/source/MulensModel/data/photometry_files/OB161195/KSS41I.dat
--rw-r--r--   0 runner    (1001) docker     (121)    22072 2022-03-21 16:19:38.000000 MulensModel-2.7.2/source/MulensModel/data/photometry_files/OB161195/KSS42I.dat
--rw-r--r--   0 runner    (1001) docker     (121)      146 2022-03-21 16:19:38.000000 MulensModel-2.7.2/source/MulensModel/data/photometry_files/OB161195/README.txt
--rw-r--r--   0 runner    (1001) docker     (121)      459 2022-03-21 16:19:38.000000 MulensModel-2.7.2/source/MulensModel/data/photometry_files/OB161195/spitzer_b12.dat
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-21 16:19:46.682056 MulensModel-2.7.2/source/MulensModel/data/unit_test_files/
--rw-r--r--   0 runner    (1001) docker     (121)    34596 2022-03-21 16:19:38.000000 MulensModel-2.7.2/source/MulensModel/data/unit_test_files/FSPL_test.dat
--rw-r--r--   0 runner    (1001) docker     (121)      924 2022-03-21 16:19:38.000000 MulensModel-2.7.2/source/MulensModel/data/unit_test_files/FSPL_test_1.dat
--rw-r--r--   0 runner    (1001) docker     (121)   132376 2022-03-21 16:19:38.000000 MulensModel-2.7.2/source/MulensModel/data/unit_test_files/MB11293_caustics.dat
--rw-r--r--   0 runner    (1001) docker     (121)     1375 2022-03-21 16:19:38.000000 MulensModel-2.7.2/source/MulensModel/data/unit_test_files/earth_position_1.dat
--rw-r--r--   0 runner    (1001) docker     (121)     1320 2022-03-21 16:19:38.000000 MulensModel-2.7.2/source/MulensModel/data/unit_test_files/earth_position_2.dat
--rw-r--r--   0 runner    (1001) docker     (121)    22548 2022-03-21 16:19:38.000000 MulensModel-2.7.2/source/MulensModel/data/unit_test_files/ob140939_OGLE_ref_v1.dat
--rw-r--r--   0 runner    (1001) docker     (121)     1457 2022-03-21 16:19:38.000000 MulensModel-2.7.2/source/MulensModel/data/unit_test_files/ob140939_Spitzer_ref_v1.dat
--rw-r--r--   0 runner    (1001) docker     (121)    10894 2022-03-21 16:19:38.000000 MulensModel-2.7.2/source/MulensModel/data/unit_test_files/ob151100_OGLE_ref_v1.dat
--rw-r--r--   0 runner    (1001) docker     (121)     3910 2022-03-21 16:19:38.000000 MulensModel-2.7.2/source/MulensModel/data/unit_test_files/ob151100_Spitzer_ref_v1.dat
--rw-r--r--   0 runner    (1001) docker     (121)    13637 2022-03-21 16:19:38.000000 MulensModel-2.7.2/source/MulensModel/data/unit_test_files/parallax_test_1.dat
--rw-r--r--   0 runner    (1001) docker     (121)    13637 2022-03-21 16:19:38.000000 MulensModel-2.7.2/source/MulensModel/data/unit_test_files/parallax_test_2.dat
--rw-r--r--   0 runner    (1001) docker     (121)    13639 2022-03-21 16:19:38.000000 MulensModel-2.7.2/source/MulensModel/data/unit_test_files/parallax_test_3.dat
--rw-r--r--   0 runner    (1001) docker     (121)    14044 2022-03-21 16:19:38.000000 MulensModel-2.7.2/source/MulensModel/data/unit_test_files/parallax_test_4.dat
--rw-r--r--   0 runner    (1001) docker     (121)    14044 2022-03-21 16:19:38.000000 MulensModel-2.7.2/source/MulensModel/data/unit_test_files/parallax_test_5.dat
--rw-r--r--   0 runner    (1001) docker     (121)    35023 2022-03-21 16:19:38.000000 MulensModel-2.7.2/source/MulensModel/event.py
--rw-r--r--   0 runner    (1001) docker     (121)    31362 2022-03-21 16:19:38.000000 MulensModel-2.7.2/source/MulensModel/fitdata.py
--rw-r--r--   0 runner    (1001) docker     (121)     4586 2022-03-21 16:19:38.000000 MulensModel-2.7.2/source/MulensModel/horizons.py
--rw-r--r--   0 runner    (1001) docker     (121)     3719 2022-03-21 16:19:38.000000 MulensModel-2.7.2/source/MulensModel/limbdarkeningcoeffs.py
--rw-r--r--   0 runner    (1001) docker     (121)    18860 2022-03-21 16:19:38.000000 MulensModel-2.7.2/source/MulensModel/magnificationcurve.py
--rw-r--r--   0 runner    (1001) docker     (121)    60689 2022-03-21 16:19:38.000000 MulensModel-2.7.2/source/MulensModel/model.py
--rw-r--r--   0 runner    (1001) docker     (121)    58126 2022-03-21 16:19:38.000000 MulensModel-2.7.2/source/MulensModel/modelparameters.py
--rw-r--r--   0 runner    (1001) docker     (121)    27239 2022-03-21 16:19:38.000000 MulensModel-2.7.2/source/MulensModel/mulensdata.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-21 16:19:46.682056 MulensModel-2.7.2/source/MulensModel/mulensobjects/
--rw-r--r--   0 runner    (1001) docker     (121)      145 2022-03-21 16:19:38.000000 MulensModel-2.7.2/source/MulensModel/mulensobjects/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    14263 2022-03-21 16:19:38.000000 MulensModel-2.7.2/source/MulensModel/mulensobjects/lens.py
--rw-r--r--   0 runner    (1001) docker     (121)     7706 2022-03-21 16:19:38.000000 MulensModel-2.7.2/source/MulensModel/mulensobjects/mulenssystem.py
--rw-r--r--   0 runner    (1001) docker     (121)     2773 2022-03-21 16:19:38.000000 MulensModel-2.7.2/source/MulensModel/mulensobjects/source.py
--rw-r--r--   0 runner    (1001) docker     (121)    24711 2022-03-21 16:19:38.000000 MulensModel-2.7.2/source/MulensModel/pointlens.py
--rw-r--r--   0 runner    (1001) docker     (121)     2709 2022-03-21 16:19:38.000000 MulensModel-2.7.2/source/MulensModel/satelliteskycoord.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-21 16:19:46.698057 MulensModel-2.7.2/source/MulensModel/tests/
--rw-r--r--   0 runner    (1001) docker     (121)      439 2022-03-21 16:19:38.000000 MulensModel-2.7.2/source/MulensModel/tests/check_architecture.py
--rw-r--r--   0 runner    (1001) docker     (121)     2154 2022-03-21 16:19:38.000000 MulensModel-2.7.2/source/MulensModel/tests/test_BinaryLens.py
--rw-r--r--   0 runner    (1001) docker     (121)      742 2022-03-21 16:19:38.000000 MulensModel-2.7.2/source/MulensModel/tests/test_Caustic.py
--rw-r--r--   0 runner    (1001) docker     (121)     3949 2022-03-21 16:19:38.000000 MulensModel-2.7.2/source/MulensModel/tests/test_Coords.py
--rw-r--r--   0 runner    (1001) docker     (121)    36548 2022-03-21 16:19:38.000000 MulensModel-2.7.2/source/MulensModel/tests/test_Event.py
--rw-r--r--   0 runner    (1001) docker     (121)    19307 2022-03-21 16:19:38.000000 MulensModel-2.7.2/source/MulensModel/tests/test_FitData.py
--rw-r--r--   0 runner    (1001) docker     (121)     3035 2022-03-21 16:19:38.000000 MulensModel-2.7.2/source/MulensModel/tests/test_Lens.py
--rw-r--r--   0 runner    (1001) docker     (121)     5338 2022-03-21 16:19:38.000000 MulensModel-2.7.2/source/MulensModel/tests/test_MagnificationCurve.py
--rw-r--r--   0 runner    (1001) docker     (121)    15381 2022-03-21 16:19:38.000000 MulensModel-2.7.2/source/MulensModel/tests/test_Model.py
--rw-r--r--   0 runner    (1001) docker     (121)     8473 2022-03-21 16:19:38.000000 MulensModel-2.7.2/source/MulensModel/tests/test_ModelParameters.py
--rw-r--r--   0 runner    (1001) docker     (121)    10941 2022-03-21 16:19:38.000000 MulensModel-2.7.2/source/MulensModel/tests/test_Model_Parallax.py
--rw-r--r--   0 runner    (1001) docker     (121)     1459 2022-03-21 16:19:38.000000 MulensModel-2.7.2/source/MulensModel/tests/test_MulensData.py
--rw-r--r--   0 runner    (1001) docker     (121)     1389 2022-03-21 16:19:38.000000 MulensModel-2.7.2/source/MulensModel/tests/test_MulensSystem.py
--rw-r--r--   0 runner    (1001) docker     (121)     2389 2022-03-21 16:19:38.000000 MulensModel-2.7.2/source/MulensModel/tests/test_PointLens.py
--rw-r--r--   0 runner    (1001) docker     (121)     1346 2022-03-21 16:19:38.000000 MulensModel-2.7.2/source/MulensModel/tests/test_Trajectory.py
--rw-r--r--   0 runner    (1001) docker     (121)     2697 2022-03-21 16:19:38.000000 MulensModel-2.7.2/source/MulensModel/tests/test_UniformCausticSampling.py
--rw-r--r--   0 runner    (1001) docker     (121)     1870 2022-03-21 16:19:38.000000 MulensModel-2.7.2/source/MulensModel/tests/test_Utils.py
--rw-r--r--   0 runner    (1001) docker     (121)    12770 2022-03-21 16:19:38.000000 MulensModel-2.7.2/source/MulensModel/trajectory.py
--rw-r--r--   0 runner    (1001) docker     (121)    31504 2022-03-21 16:19:38.000000 MulensModel-2.7.2/source/MulensModel/uniformcausticsampling.py
--rw-r--r--   0 runner    (1001) docker     (121)    15164 2022-03-21 16:19:38.000000 MulensModel-2.7.2/source/MulensModel/utils.py
--rw-r--r--   0 runner    (1001) docker     (121)       22 2022-03-21 16:19:38.000000 MulensModel-2.7.2/source/MulensModel/version.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-21 16:19:46.670055 MulensModel-2.7.2/source/MulensModel.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)      403 2022-03-21 16:19:46.000000 MulensModel-2.7.2/source/MulensModel.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     6262 2022-03-21 16:19:46.000000 MulensModel-2.7.2/source/MulensModel.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-03-21 16:19:46.000000 MulensModel-2.7.2/source/MulensModel.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       63 2022-03-21 16:19:46.000000 MulensModel-2.7.2/source/MulensModel.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       12 2022-03-21 16:19:46.000000 MulensModel-2.7.2/source/MulensModel.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-21 16:19:46.698057 MulensModel-2.7.2/source/VBBL/
--rw-r--r--   0 runner    (1001) docker     (121)      566 2022-03-21 16:19:38.000000 MulensModel-2.7.2/source/VBBL/Makefile
--rw-r--r--   0 runner    (1001) docker     (121)      870 2022-03-21 16:19:38.000000 MulensModel-2.7.2/source/VBBL/README.md
--rw-r--r--   0 runner    (1001) docker     (121)   105644 2022-03-21 16:19:38.000000 MulensModel-2.7.2/source/VBBL/VBBinaryLensingLibrary.cpp
--rw-r--r--   0 runner    (1001) docker     (121)     9103 2022-03-21 16:19:38.000000 MulensModel-2.7.2/source/VBBL/VBBinaryLensingLibrary.h
--rw-r--r--   0 runner    (1001) docker     (121)     1236 2022-03-21 16:19:38.000000 MulensModel-2.7.2/source/VBBL/VBBinaryLensingLibrary_wrapper.cpp
--rw-r--r--   0 runner    (1001) docker     (121)     2375 2022-03-21 16:19:38.000000 MulensModel-2.7.2/source/VBBL/vbbl_wrapper.cpp
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-09 09:50:59.034529 MulensModel-2.8.1/
+-rw-r--r--   0 runner    (1001) docker     (121)    10086 2022-04-09 09:50:54.000000 MulensModel-2.8.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (121)      100 2022-04-09 09:50:54.000000 MulensModel-2.8.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (121)      403 2022-04-09 09:50:59.034529 MulensModel-2.8.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     3844 2022-04-09 09:50:54.000000 MulensModel-2.8.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (121)      100 2022-04-09 09:50:54.000000 MulensModel-2.8.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (121)       63 2022-04-09 09:50:54.000000 MulensModel-2.8.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       38 2022-04-09 09:50:59.034529 MulensModel-2.8.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)     1794 2022-04-09 09:50:54.000000 MulensModel-2.8.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-09 09:50:59.018529 MulensModel-2.8.1/source/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-09 09:50:59.022529 MulensModel-2.8.1/source/AdaptiveContouring/
+-rw-r--r--   0 runner    (1001) docker     (121)      841 2022-04-09 09:50:54.000000 MulensModel-2.8.1/source/AdaptiveContouring/AdaptiveContouring_wrapper.c
+-rw-r--r--   0 runner    (1001) docker     (121)      652 2022-04-09 09:50:54.000000 MulensModel-2.8.1/source/AdaptiveContouring/Makefile
+-rw-r--r--   0 runner    (1001) docker     (121)     3970 2022-04-09 09:50:54.000000 MulensModel-2.8.1/source/AdaptiveContouring/README.adaptivecontouring
+-rw-r--r--   0 runner    (1001) docker     (121)     1271 2022-04-09 09:50:54.000000 MulensModel-2.8.1/source/AdaptiveContouring/ac_wrap.c
+-rw-r--r--   0 runner    (1001) docker     (121)    59956 2022-04-09 09:50:54.000000 MulensModel-2.8.1/source/AdaptiveContouring/adaptive_contour.c
+-rw-r--r--   0 runner    (1001) docker     (121)     7793 2022-04-09 09:50:54.000000 MulensModel-2.8.1/source/AdaptiveContouring/binary_pt.c
+-rw-r--r--   0 runner    (1001) docker     (121)     4382 2022-04-09 09:50:54.000000 MulensModel-2.8.1/source/AdaptiveContouring/binext_adap.c
+-rw-r--r--   0 runner    (1001) docker     (121)     2031 2022-04-09 09:50:54.000000 MulensModel-2.8.1/source/AdaptiveContouring/complex.c
+-rw-r--r--   0 runner    (1001) docker     (121)      531 2022-04-09 09:50:54.000000 MulensModel-2.8.1/source/AdaptiveContouring/complex.h
+-rw-r--r--   0 runner    (1001) docker     (121)     1054 2022-04-09 09:50:54.000000 MulensModel-2.8.1/source/AdaptiveContouring/dyn_array.c
+-rw-r--r--   0 runner    (1001) docker     (121)    57862 2022-04-09 09:50:54.000000 MulensModel-2.8.1/source/AdaptiveContouring/erdlcaust.c
+-rw-r--r--   0 runner    (1001) docker     (121)     6443 2022-04-09 09:50:54.000000 MulensModel-2.8.1/source/AdaptiveContouring/integrate.c
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-09 09:50:59.022529 MulensModel-2.8.1/source/MulensModel/
+-rw-r--r--   0 runner    (1001) docker     (121)     1359 2022-04-09 09:50:54.000000 MulensModel-2.8.1/source/MulensModel/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    25851 2022-04-09 09:50:54.000000 MulensModel-2.8.1/source/MulensModel/binarylens.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3502 2022-04-09 09:50:54.000000 MulensModel-2.8.1/source/MulensModel/binarylensimports.py
+-rw-r--r--   0 runner    (1001) docker     (121)    33199 2022-04-09 09:50:54.000000 MulensModel-2.8.1/source/MulensModel/binarylenswithshear.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5560 2022-04-09 09:50:54.000000 MulensModel-2.8.1/source/MulensModel/caustics.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3196 2022-04-09 09:50:54.000000 MulensModel-2.8.1/source/MulensModel/causticswithshear.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5370 2022-04-09 09:50:54.000000 MulensModel-2.8.1/source/MulensModel/coordinates.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-09 09:50:59.026529 MulensModel-2.8.1/source/MulensModel/data/
+-rw-r--r--   0 runner    (1001) docker     (121)  1555125 2022-04-09 09:50:54.000000 MulensModel-2.8.1/source/MulensModel/data/WFIRST_1827.dat
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-09 09:50:59.026529 MulensModel-2.8.1/source/MulensModel/data/ephemeris_files/
+-rw-r--r--   0 runner    (1001) docker     (121)    41053 2022-04-09 09:50:54.000000 MulensModel-2.8.1/source/MulensModel/data/ephemeris_files/K2_ephemeris_01.dat
+-rw-r--r--   0 runner    (1001) docker     (121)    83691 2022-04-09 09:50:54.000000 MulensModel-2.8.1/source/MulensModel/data/ephemeris_files/Spitzer_ephemeris_01.dat
+-rw-r--r--   0 runner    (1001) docker     (121)   149352 2022-04-09 09:50:54.000000 MulensModel-2.8.1/source/MulensModel/data/ephemeris_files/Spitzer_ephemeris_02.dat
+-rw-r--r--   0 runner    (1001) docker     (121)    18781 2022-04-09 09:50:54.000000 MulensModel-2.8.1/source/MulensModel/data/interpolate_elliptic_integral_1_2.dat
+-rw-r--r--   0 runner    (1001) docker     (121)     1994 2022-04-09 09:50:54.000000 MulensModel-2.8.1/source/MulensModel/data/interpolate_elliptic_integral_1_2.py
+-rw-r--r--   0 runner    (1001) docker     (121)   222778 2022-04-09 09:50:54.000000 MulensModel-2.8.1/source/MulensModel/data/interpolate_elliptic_integral_3.dat
+-rw-r--r--   0 runner    (1001) docker     (121)     2981 2022-04-09 09:50:54.000000 MulensModel-2.8.1/source/MulensModel/data/interpolate_elliptic_integral_3.py
+-rw-r--r--   0 runner    (1001) docker     (121)   224553 2022-04-09 09:50:54.000000 MulensModel-2.8.1/source/MulensModel/data/interpolation_table_b0b1_v1.dat
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-09 09:50:59.018529 MulensModel-2.8.1/source/MulensModel/data/photometry_files/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-09 09:50:59.026529 MulensModel-2.8.1/source/MulensModel/data/photometry_files/KB180003/
+-rw-r--r--   0 runner    (1001) docker     (121)      156 2022-04-09 09:50:54.000000 MulensModel-2.8.1/source/MulensModel/data/photometry_files/KB180003/00README.txt
+-rw-r--r--   0 runner    (1001) docker     (121)    17761 2022-04-09 09:50:54.000000 MulensModel-2.8.1/source/MulensModel/data/photometry_files/KB180003/KMTA12_I.pysis
+-rw-r--r--   0 runner    (1001) docker     (121)     3995 2022-04-09 09:50:54.000000 MulensModel-2.8.1/source/MulensModel/data/photometry_files/KB180003/KMTA14_I.pysis
+-rw-r--r--   0 runner    (1001) docker     (121)     4585 2022-04-09 09:50:54.000000 MulensModel-2.8.1/source/MulensModel/data/photometry_files/KB180003/KMTC12_I.pysis
+-rw-r--r--   0 runner    (1001) docker     (121)    10013 2022-04-09 09:50:54.000000 MulensModel-2.8.1/source/MulensModel/data/photometry_files/KB180003/KMTC14_I.pysis
+-rw-r--r--   0 runner    (1001) docker     (121)     2225 2022-04-09 09:50:54.000000 MulensModel-2.8.1/source/MulensModel/data/photometry_files/KB180003/KMTS12_I.pysis
+-rw-r--r--   0 runner    (1001) docker     (121)     3346 2022-04-09 09:50:54.000000 MulensModel-2.8.1/source/MulensModel/data/photometry_files/KB180003/KMTS14_I.pysis
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-09 09:50:59.026529 MulensModel-2.8.1/source/MulensModel/data/photometry_files/MB08310/
+-rw-r--r--   0 runner    (1001) docker     (121)     5913 2022-04-09 09:50:54.000000 MulensModel-2.8.1/source/MulensModel/data/photometry_files/MB08310/Auck_0300089_PLC_001.tbl
+-rw-r--r--   0 runner    (1001) docker     (121)    10231 2022-04-09 09:50:54.000000 MulensModel-2.8.1/source/MulensModel/data/photometry_files/MB08310/Bron_0300089_PLC_002.tbl
+-rw-r--r--   0 runner    (1001) docker     (121)    17693 2022-04-09 09:50:54.000000 MulensModel-2.8.1/source/MulensModel/data/photometry_files/MB08310/CTIO_H_0300089_PLC_004.tbl
+-rw-r--r--   0 runner    (1001) docker     (121)     4108 2022-04-09 09:50:54.000000 MulensModel-2.8.1/source/MulensModel/data/photometry_files/MB08310/CTIO_I_0300089_PLC_005.tbl
+-rw-r--r--   0 runner    (1001) docker     (121)     2144 2022-04-09 09:50:54.000000 MulensModel-2.8.1/source/MulensModel/data/photometry_files/MB08310/Canopus_0300089_PLC_003.tbl
+-rw-r--r--   0 runner    (1001) docker     (121)     4420 2022-04-09 09:50:54.000000 MulensModel-2.8.1/source/MulensModel/data/photometry_files/MB08310/Danish_0300089_PLC_006.tbl
+-rw-r--r--   0 runner    (1001) docker     (121)   170275 2022-04-09 09:50:54.000000 MulensModel-2.8.1/source/MulensModel/data/photometry_files/MB08310/MOA_0300089_PLC_007.tbl
+-rw-r--r--   0 runner    (1001) docker     (121)      417 2022-04-09 09:50:54.000000 MulensModel-2.8.1/source/MulensModel/data/photometry_files/MB08310/README.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-09 09:50:59.026529 MulensModel-2.8.1/source/MulensModel/data/photometry_files/OB03235/
+-rw-r--r--   0 runner    (1001) docker     (121)    80276 2022-04-09 09:50:54.000000 MulensModel-2.8.1/source/MulensModel/data/photometry_files/OB03235/OB03235_MOA.tbl.txt
+-rw-r--r--   0 runner    (1001) docker     (121)    18686 2022-04-09 09:50:54.000000 MulensModel-2.8.1/source/MulensModel/data/photometry_files/OB03235/OB03235_OGLE.tbl.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      429 2022-04-09 09:50:54.000000 MulensModel-2.8.1/source/MulensModel/data/photometry_files/OB03235/README.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-09 09:50:59.026529 MulensModel-2.8.1/source/MulensModel/data/photometry_files/OB05086/
+-rw-r--r--   0 runner    (1001) docker     (121)      255 2022-04-09 09:50:54.000000 MulensModel-2.8.1/source/MulensModel/data/photometry_files/OB05086/README.txt
+-rw-r--r--   0 runner    (1001) docker     (121)    15360 2022-04-09 09:50:54.000000 MulensModel-2.8.1/source/MulensModel/data/photometry_files/OB05086/starBLG234.6.I.218982.dat
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-09 09:50:59.026529 MulensModel-2.8.1/source/MulensModel/data/photometry_files/OB08092/
+-rw-r--r--   0 runner    (1001) docker     (121)      175 2022-04-09 09:50:54.000000 MulensModel-2.8.1/source/MulensModel/data/photometry_files/OB08092/README.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     9958 2022-04-09 09:50:54.000000 MulensModel-2.8.1/source/MulensModel/data/photometry_files/OB08092/phot_ob08092_O4.dat
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-09 09:50:59.030529 MulensModel-2.8.1/source/MulensModel/data/photometry_files/OB140939/
+-rw-r--r--   0 runner    (1001) docker     (121)      412 2022-04-09 09:50:54.000000 MulensModel-2.8.1/source/MulensModel/data/photometry_files/OB140939/README.txt
+-rw-r--r--   0 runner    (1001) docker     (121)    18449 2022-04-09 09:50:54.000000 MulensModel-2.8.1/source/MulensModel/data/photometry_files/OB140939/ob140939_OGLE.dat
+-rw-r--r--   0 runner    (1001) docker     (121)      899 2022-04-09 09:50:54.000000 MulensModel-2.8.1/source/MulensModel/data/photometry_files/OB140939/ob140939_Spitzer.dat
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-09 09:50:59.030529 MulensModel-2.8.1/source/MulensModel/data/photometry_files/OB161195/
+-rw-r--r--   0 runner    (1001) docker     (121)    49569 2022-04-09 09:50:54.000000 MulensModel-2.8.1/source/MulensModel/data/photometry_files/OB161195/KCT01I.dat
+-rw-r--r--   0 runner    (1001) docker     (121)    46159 2022-04-09 09:50:54.000000 MulensModel-2.8.1/source/MulensModel/data/photometry_files/OB161195/KCT41I.dat
+-rw-r--r--   0 runner    (1001) docker     (121)    35495 2022-04-09 09:50:54.000000 MulensModel-2.8.1/source/MulensModel/data/photometry_files/OB161195/KCT42I.dat
+-rw-r--r--   0 runner    (1001) docker     (121)    42253 2022-04-09 09:50:54.000000 MulensModel-2.8.1/source/MulensModel/data/photometry_files/OB161195/KSA01I.dat
+-rw-r--r--   0 runner    (1001) docker     (121)    38161 2022-04-09 09:50:54.000000 MulensModel-2.8.1/source/MulensModel/data/photometry_files/OB161195/KSA41I.dat
+-rw-r--r--   0 runner    (1001) docker     (121)    33573 2022-04-09 09:50:54.000000 MulensModel-2.8.1/source/MulensModel/data/photometry_files/OB161195/KSA42I.dat
+-rw-r--r--   0 runner    (1001) docker     (121)    24614 2022-04-09 09:50:54.000000 MulensModel-2.8.1/source/MulensModel/data/photometry_files/OB161195/KSS01I.dat
+-rw-r--r--   0 runner    (1001) docker     (121)    28800 2022-04-09 09:50:54.000000 MulensModel-2.8.1/source/MulensModel/data/photometry_files/OB161195/KSS41I.dat
+-rw-r--r--   0 runner    (1001) docker     (121)    22072 2022-04-09 09:50:54.000000 MulensModel-2.8.1/source/MulensModel/data/photometry_files/OB161195/KSS42I.dat
+-rw-r--r--   0 runner    (1001) docker     (121)      146 2022-04-09 09:50:54.000000 MulensModel-2.8.1/source/MulensModel/data/photometry_files/OB161195/README.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      459 2022-04-09 09:50:54.000000 MulensModel-2.8.1/source/MulensModel/data/photometry_files/OB161195/spitzer_b12.dat
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-09 09:50:59.030529 MulensModel-2.8.1/source/MulensModel/data/unit_test_files/
+-rw-r--r--   0 runner    (1001) docker     (121)    34596 2022-04-09 09:50:54.000000 MulensModel-2.8.1/source/MulensModel/data/unit_test_files/FSPL_test.dat
+-rw-r--r--   0 runner    (1001) docker     (121)      924 2022-04-09 09:50:54.000000 MulensModel-2.8.1/source/MulensModel/data/unit_test_files/FSPL_test_1.dat
+-rw-r--r--   0 runner    (1001) docker     (121)   132376 2022-04-09 09:50:54.000000 MulensModel-2.8.1/source/MulensModel/data/unit_test_files/MB11293_caustics.dat
+-rw-r--r--   0 runner    (1001) docker     (121)     1375 2022-04-09 09:50:54.000000 MulensModel-2.8.1/source/MulensModel/data/unit_test_files/earth_position_1.dat
+-rw-r--r--   0 runner    (1001) docker     (121)     1320 2022-04-09 09:50:54.000000 MulensModel-2.8.1/source/MulensModel/data/unit_test_files/earth_position_2.dat
+-rw-r--r--   0 runner    (1001) docker     (121)    22548 2022-04-09 09:50:54.000000 MulensModel-2.8.1/source/MulensModel/data/unit_test_files/ob140939_OGLE_ref_v1.dat
+-rw-r--r--   0 runner    (1001) docker     (121)     1457 2022-04-09 09:50:54.000000 MulensModel-2.8.1/source/MulensModel/data/unit_test_files/ob140939_Spitzer_ref_v1.dat
+-rw-r--r--   0 runner    (1001) docker     (121)    10894 2022-04-09 09:50:54.000000 MulensModel-2.8.1/source/MulensModel/data/unit_test_files/ob151100_OGLE_ref_v1.dat
+-rw-r--r--   0 runner    (1001) docker     (121)     3910 2022-04-09 09:50:54.000000 MulensModel-2.8.1/source/MulensModel/data/unit_test_files/ob151100_Spitzer_ref_v1.dat
+-rw-r--r--   0 runner    (1001) docker     (121)    13637 2022-04-09 09:50:54.000000 MulensModel-2.8.1/source/MulensModel/data/unit_test_files/parallax_test_1.dat
+-rw-r--r--   0 runner    (1001) docker     (121)    13637 2022-04-09 09:50:54.000000 MulensModel-2.8.1/source/MulensModel/data/unit_test_files/parallax_test_2.dat
+-rw-r--r--   0 runner    (1001) docker     (121)    13639 2022-04-09 09:50:54.000000 MulensModel-2.8.1/source/MulensModel/data/unit_test_files/parallax_test_3.dat
+-rw-r--r--   0 runner    (1001) docker     (121)    14044 2022-04-09 09:50:54.000000 MulensModel-2.8.1/source/MulensModel/data/unit_test_files/parallax_test_4.dat
+-rw-r--r--   0 runner    (1001) docker     (121)    14044 2022-04-09 09:50:54.000000 MulensModel-2.8.1/source/MulensModel/data/unit_test_files/parallax_test_5.dat
+-rw-r--r--   0 runner    (1001) docker     (121)    35016 2022-04-09 09:50:54.000000 MulensModel-2.8.1/source/MulensModel/event.py
+-rw-r--r--   0 runner    (1001) docker     (121)    31358 2022-04-09 09:50:54.000000 MulensModel-2.8.1/source/MulensModel/fitdata.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4586 2022-04-09 09:50:54.000000 MulensModel-2.8.1/source/MulensModel/horizons.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3720 2022-04-09 09:50:54.000000 MulensModel-2.8.1/source/MulensModel/limbdarkeningcoeffs.py
+-rw-r--r--   0 runner    (1001) docker     (121)    20719 2022-04-09 09:50:54.000000 MulensModel-2.8.1/source/MulensModel/magnificationcurve.py
+-rw-r--r--   0 runner    (1001) docker     (121)    60656 2022-04-09 09:50:54.000000 MulensModel-2.8.1/source/MulensModel/model.py
+-rw-r--r--   0 runner    (1001) docker     (121)    60469 2022-04-09 09:50:54.000000 MulensModel-2.8.1/source/MulensModel/modelparameters.py
+-rw-r--r--   0 runner    (1001) docker     (121)    27219 2022-04-09 09:50:54.000000 MulensModel-2.8.1/source/MulensModel/mulensdata.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-09 09:50:59.030529 MulensModel-2.8.1/source/MulensModel/mulensobjects/
+-rw-r--r--   0 runner    (1001) docker     (121)      145 2022-04-09 09:50:54.000000 MulensModel-2.8.1/source/MulensModel/mulensobjects/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    14264 2022-04-09 09:50:54.000000 MulensModel-2.8.1/source/MulensModel/mulensobjects/lens.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7703 2022-04-09 09:50:54.000000 MulensModel-2.8.1/source/MulensModel/mulensobjects/mulenssystem.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2774 2022-04-09 09:50:54.000000 MulensModel-2.8.1/source/MulensModel/mulensobjects/source.py
+-rw-r--r--   0 runner    (1001) docker     (121)    24700 2022-04-09 09:50:54.000000 MulensModel-2.8.1/source/MulensModel/pointlens.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2709 2022-04-09 09:50:54.000000 MulensModel-2.8.1/source/MulensModel/satelliteskycoord.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-09 09:50:59.034529 MulensModel-2.8.1/source/MulensModel/tests/
+-rw-r--r--   0 runner    (1001) docker     (121)      439 2022-04-09 09:50:54.000000 MulensModel-2.8.1/source/MulensModel/tests/check_architecture.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2402 2022-04-09 09:50:54.000000 MulensModel-2.8.1/source/MulensModel/tests/test_BinaryLens.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2492 2022-04-09 09:50:54.000000 MulensModel-2.8.1/source/MulensModel/tests/test_BinaryLensWithShear.py
+-rw-r--r--   0 runner    (1001) docker     (121)      808 2022-04-09 09:50:54.000000 MulensModel-2.8.1/source/MulensModel/tests/test_Caustics.py
+-rw-r--r--   0 runner    (1001) docker     (121)      901 2022-04-09 09:50:54.000000 MulensModel-2.8.1/source/MulensModel/tests/test_CausticsWithShear.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3949 2022-04-09 09:50:54.000000 MulensModel-2.8.1/source/MulensModel/tests/test_Coords.py
+-rw-r--r--   0 runner    (1001) docker     (121)    36548 2022-04-09 09:50:54.000000 MulensModel-2.8.1/source/MulensModel/tests/test_Event.py
+-rw-r--r--   0 runner    (1001) docker     (121)    19299 2022-04-09 09:50:54.000000 MulensModel-2.8.1/source/MulensModel/tests/test_FitData.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3035 2022-04-09 09:50:54.000000 MulensModel-2.8.1/source/MulensModel/tests/test_Lens.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5338 2022-04-09 09:50:54.000000 MulensModel-2.8.1/source/MulensModel/tests/test_MagnificationCurve.py
+-rw-r--r--   0 runner    (1001) docker     (121)    16693 2022-04-09 09:50:54.000000 MulensModel-2.8.1/source/MulensModel/tests/test_Model.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8919 2022-04-09 09:50:54.000000 MulensModel-2.8.1/source/MulensModel/tests/test_ModelParameters.py
+-rw-r--r--   0 runner    (1001) docker     (121)    10934 2022-04-09 09:50:54.000000 MulensModel-2.8.1/source/MulensModel/tests/test_Model_Parallax.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1459 2022-04-09 09:50:54.000000 MulensModel-2.8.1/source/MulensModel/tests/test_MulensData.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1389 2022-04-09 09:50:54.000000 MulensModel-2.8.1/source/MulensModel/tests/test_MulensSystem.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2389 2022-04-09 09:50:54.000000 MulensModel-2.8.1/source/MulensModel/tests/test_PointLens.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1346 2022-04-09 09:50:54.000000 MulensModel-2.8.1/source/MulensModel/tests/test_Trajectory.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2697 2022-04-09 09:50:54.000000 MulensModel-2.8.1/source/MulensModel/tests/test_UniformCausticSampling.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1870 2022-04-09 09:50:54.000000 MulensModel-2.8.1/source/MulensModel/tests/test_Utils.py
+-rw-r--r--   0 runner    (1001) docker     (121)    12529 2022-04-09 09:50:54.000000 MulensModel-2.8.1/source/MulensModel/trajectory.py
+-rw-r--r--   0 runner    (1001) docker     (121)    31505 2022-04-09 09:50:54.000000 MulensModel-2.8.1/source/MulensModel/uniformcausticsampling.py
+-rw-r--r--   0 runner    (1001) docker     (121)    15160 2022-04-09 09:50:54.000000 MulensModel-2.8.1/source/MulensModel/utils.py
+-rw-r--r--   0 runner    (1001) docker     (121)       22 2022-04-09 09:50:54.000000 MulensModel-2.8.1/source/MulensModel/version.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-09 09:50:59.022529 MulensModel-2.8.1/source/MulensModel.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)      403 2022-04-09 09:50:58.000000 MulensModel-2.8.1/source/MulensModel.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     6513 2022-04-09 09:50:59.000000 MulensModel-2.8.1/source/MulensModel.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-04-09 09:50:58.000000 MulensModel-2.8.1/source/MulensModel.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       63 2022-04-09 09:50:58.000000 MulensModel-2.8.1/source/MulensModel.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       12 2022-04-09 09:50:58.000000 MulensModel-2.8.1/source/MulensModel.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-09 09:50:59.034529 MulensModel-2.8.1/source/VBBL/
+-rw-r--r--   0 runner    (1001) docker     (121)     8807 2022-04-09 09:50:54.000000 MulensModel-2.8.1/source/VBBL/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      566 2022-04-09 09:50:54.000000 MulensModel-2.8.1/source/VBBL/Makefile
+-rw-r--r--   0 runner    (1001) docker     (121)      870 2022-04-09 09:50:54.000000 MulensModel-2.8.1/source/VBBL/README.md
+-rw-r--r--   0 runner    (1001) docker     (121)   131731 2022-04-09 09:50:54.000000 MulensModel-2.8.1/source/VBBL/VBBinaryLensingLibrary.cpp
+-rw-r--r--   0 runner    (1001) docker     (121)     9492 2022-04-09 09:50:54.000000 MulensModel-2.8.1/source/VBBL/VBBinaryLensingLibrary.h
+-rw-r--r--   0 runner    (1001) docker     (121)     2538 2022-04-09 09:50:54.000000 MulensModel-2.8.1/source/VBBL/VBBinaryLensingLibrary_wrapper.cpp
+-rw-r--r--   0 runner    (1001) docker     (121)     4013 2022-04-09 09:50:54.000000 MulensModel-2.8.1/source/VBBL/vbbl_wrapper.cpp
```

### Comparing `MulensModel-2.7.2/README.md` & `MulensModel-2.8.1/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 # MulensModel
 
 <dl>MulensModel is package for modeling microlensing (or &mu;-lensing) events. </dl>
 
+<!-- ![example workflow](https://github.com/alpv95/MulensModel/actions/workflows/tests.yml/badge.svg) -->
+
 [**Detailed documentation: https://rpoleski.github.io/MulensModel/**](https://rpoleski.github.io/MulensModel/)
 
-[Latest release: 2.7.2](https://github.com/rpoleski/MulensModel/releases/latest) and we're working on further developing the code.
+[Latest release: 2.8.1](https://github.com/rpoleski/MulensModel/releases/latest) and we're working on further developing the code.
 
 MulensModel can generate a microlensing light curve for a given set of microlensing parameters, fit that light curve to some data, and return a chi2 value. That chi2 can then be input into an arbitrary likelihood function to find the best-fit parameters.
 
 If you want to learn more about microlensing, please visit [Microlensing Source website](http://microlensing-source.org/).
 
 Currently, MulensModel supports:
 * Lens Systems: point lens or binary lens.
@@ -50,9 +52,9 @@
 [![astropy](http://img.shields.io/badge/powered%20by-AstroPy-orange.svg?style=flat)](http://www.astropy.org/) 
 [![PyPI version shields.io](https://img.shields.io/pypi/v/MulensModel.svg)](https://pypi.python.org/pypi/MulensModel/) 
 [![GitHub stars](https://badgen.net/github/stars/rpoleski/MulensModel)](https://GitHub.com/rpoleski/MulensModel/stargazers/) 
 [![MIT license](https://img.shields.io/badge/License-MIT-blue.svg)](https://lbesson.mit-license.org/) 
 [![Poleski & Yee 2019](https://img.shields.io/badge/ADS-Poleski%20%26%20Yee%202019-brightgreen.svg)](https://ui.adsabs.harvard.edu/abs/2019A%26C....26...35P/abstract)
 [![astro-ph/1803.01003](https://img.shields.io/badge/astro--ph-1803.01003-brightgreen.svg)](https://arxiv.org/abs/1803.01003)
 
-file revised Mar 2022
+file revised Apr 2022
```

### Comparing `MulensModel-2.7.2/setup.py` & `MulensModel-2.8.1/setup.py`

 * *Files identical despite different names*

### Comparing `MulensModel-2.7.2/source/AdaptiveContouring/AdaptiveContouring_wrapper.c` & `MulensModel-2.8.1/source/AdaptiveContouring/AdaptiveContouring_wrapper.c`

 * *Files identical despite different names*

### Comparing `MulensModel-2.7.2/source/AdaptiveContouring/Makefile` & `MulensModel-2.8.1/source/AdaptiveContouring/Makefile`

 * *Files identical despite different names*

### Comparing `MulensModel-2.7.2/source/AdaptiveContouring/README.adaptivecontouring` & `MulensModel-2.8.1/source/AdaptiveContouring/README.adaptivecontouring`

 * *Files identical despite different names*

### Comparing `MulensModel-2.7.2/source/AdaptiveContouring/ac_wrap.c` & `MulensModel-2.8.1/source/AdaptiveContouring/ac_wrap.c`

 * *Files identical despite different names*

### Comparing `MulensModel-2.7.2/source/AdaptiveContouring/adaptive_contour.c` & `MulensModel-2.8.1/source/AdaptiveContouring/adaptive_contour.c`

 * *Files identical despite different names*

### Comparing `MulensModel-2.7.2/source/AdaptiveContouring/binary_pt.c` & `MulensModel-2.8.1/source/AdaptiveContouring/binary_pt.c`

 * *Files identical despite different names*

### Comparing `MulensModel-2.7.2/source/AdaptiveContouring/binext_adap.c` & `MulensModel-2.8.1/source/AdaptiveContouring/binext_adap.c`

 * *Files identical despite different names*

### Comparing `MulensModel-2.7.2/source/AdaptiveContouring/complex.c` & `MulensModel-2.8.1/source/AdaptiveContouring/complex.c`

 * *Files identical despite different names*

### Comparing `MulensModel-2.7.2/source/AdaptiveContouring/complex.h` & `MulensModel-2.8.1/source/AdaptiveContouring/complex.h`

 * *Files identical despite different names*

### Comparing `MulensModel-2.7.2/source/AdaptiveContouring/dyn_array.c` & `MulensModel-2.8.1/source/AdaptiveContouring/dyn_array.c`

 * *Files identical despite different names*

### Comparing `MulensModel-2.7.2/source/AdaptiveContouring/erdlcaust.c` & `MulensModel-2.8.1/source/AdaptiveContouring/erdlcaust.c`

 * *Files identical despite different names*

### Comparing `MulensModel-2.7.2/source/AdaptiveContouring/integrate.c` & `MulensModel-2.8.1/source/AdaptiveContouring/integrate.c`

 * *Files identical despite different names*

### Comparing `MulensModel-2.7.2/source/MulensModel/__init__.py` & `MulensModel-2.8.1/source/MulensModel/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 from os import path
 
 from MulensModel.binarylens import BinaryLens
+from MulensModel.binarylenswithshear import BinaryLensWithShear
 from MulensModel.caustics import Caustics
+from MulensModel.causticswithshear import CausticsWithShear
 from MulensModel.coordinates import Coordinates
 from MulensModel.event import Event
 from MulensModel.fitdata import FitData
 from MulensModel.horizons import Horizons
 from MulensModel.limbdarkeningcoeffs import LimbDarkeningCoeffs
 from MulensModel.magnificationcurve import MagnificationCurve
 from MulensModel.model import Model
```

### Comparing `MulensModel-2.7.2/source/MulensModel/binarylens.py` & `MulensModel-2.8.1/source/MulensModel/binarylens.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,115 +1,15 @@
-import sys
-import os
-import ctypes
-import glob
 import warnings
 import numpy as np
 from math import fsum, sqrt
 
+from MulensModel.binarylensimports import (
+    _vbbl_wrapped, _adaptive_contouring_wrapped, _vbbl_binary_mag_dark,
+    _vbbl_SG12_5, _adaptive_contouring_linear, _solver)
 import MulensModel as mm
-try:
-    import MulensModel.VBBL as mm_vbbl
-except Exception:
-    _vbbl_wrapped = False
-else:
-    _vbbl_wrapped = True
-try:
-    import MulensModel.AdaptiveContouring as mm_ac
-except Exception:
-    _adaptive_contouring_wrapped = False
-else:
-    _adaptive_contouring_wrapped = True
-
-
-def _try_load(path, name):
-    """
-    Try loading compiled C library.
-    Input is *str* or *list* of *str*.
-    """
-    if isinstance(path, str):
-        path = [path]
-    for path_ in path:
-        try:
-            out = ctypes.cdll.LoadLibrary(path_)
-        except OSError:
-            print("WARNING - File not loaded:", path_)
-            print("Everything should work except:", name)
-            pass
-        else:
-            return out
-    return None
-
-
-def _get_path_2(name_1, name_2):
-    """convenience function"""
-    module_path = os.path.abspath(__file__)
-    for i in range(3):
-        module_path = os.path.dirname(module_path)
-    return os.path.join(module_path, 'source', name_1, name_2)
-
-
-def _import_compiled_VBBL():
-    """try importing manually compiled VBBL package"""
-    vbbl = _try_load(
-        _get_path_2('VBBL', "VBBinaryLensingLibrary_wrapper.so"), "VBBL")
-    _vbbl_wrapped = (vbbl is not None)
-    if not _vbbl_wrapped:
-        return (_vbbl_wrapped, None, None)
-
-    vbbl.VBBinaryLensing_BinaryMagDark.argtypes = 7 * [ctypes.c_double]
-    vbbl.VBBinaryLensing_BinaryMagDark.restype = ctypes.c_double
-
-    vbbl.VBBL_SG12_5.argtypes = 12 * [ctypes.c_double]
-    vbbl.VBBL_SG12_5.restype = np.ctypeslib.ndpointer(
-        dtype=ctypes.c_double, shape=(10,))
-
-    vbbl.VBBL_BinaryMag.argtypes = 4 * [ctypes.c_double]
-    vbbl.VBBL_BinaryMag.restype = ctypes.c_double
-
-    return (_vbbl_wrapped,
-            vbbl.VBBinaryLensing_BinaryMagDark, vbbl.VBBL_SG12_5,
-            vbbl.VBBL_BinaryMag)
-
-
-def _import_compiled_AdaptiveContouring():
-    """try importing manually compiled AdaptiveContouring package"""
-    ac = "AdaptiveContouring"
-    adaptive_contour = _try_load(_get_path_2(ac, ac + "_wrapper.so"), ac)
-    _adaptive_contouring_wrapped = (adaptive_contour is not None)
-    if not _adaptive_contouring_wrapped:
-        return (_adaptive_contouring_wrapped, None)
-    adaptive_contour.Adaptive_Contouring_Linear.argtypes = (
-        8 * [ctypes.c_double])
-    adaptive_contour.Adaptive_Contouring_Linear.restype = ctypes.c_double
-    return (_adaptive_contouring_wrapped,
-            adaptive_contour.Adaptive_Contouring_Linear)
-
-
-# Check import and try manually compiled versions.
-if _vbbl_wrapped:
-    _vbbl_binary_mag_dark = mm_vbbl.VBBinaryLensing_BinaryMagDark
-    _vbbl_SG12_5 = mm_vbbl.VBBL_SG12_5
-    _vbbl_binary_mag = mm_vbbl.VBBL_BinaryMag
-else:
-    out = _import_compiled_VBBL()
-    _vbbl_wrapped = out[0]
-    _vbbl_binary_mag_dark = out[1]
-    _vbbl_SG12_5 = out[2]
-    _vbbl_binary_mag = out[3]
-if not _vbbl_wrapped:
-    _solver = 'numpy'
-else:
-    _solver = 'Skowron_and_Gould_12'
-if _adaptive_contouring_wrapped:
-    _adaptive_contouring_linear = mm_ac.Adaptive_Contouring_Linear
-else:
-    out = _import_compiled_AdaptiveContouring()
-    _adaptive_contouring_wrapped = out[0]
-    _adaptive_contouring_linear = out[1]
 
 
 class BinaryLens(object):
     """
     The binary lens equation - its solutions, images, parities,
     magnifications, etc.
 
@@ -130,14 +30,15 @@
 
     Note: mass_1 and mass_2 may be defined as a fraction of some other
     mass than the total mass. This is possible but not recommended -
     make sure you know what you're doing before you start using this
     possibility.
 
     """
+
     def __init__(self, mass_1=None, mass_2=None, separation=None):
         self.mass_1 = float(mass_1)  # This speeds-up code for np.float input.
         self.mass_2 = float(mass_2)
         self.separation = float(separation)
         self._total_mass = None
         self._mass_difference = None
         self._position_z1 = None
@@ -241,37 +142,37 @@
         z1 = self._position_z1
 
         coeff_5 = c_sum([z1, -zeta_conj]) * zeta_conj
         coeff_4 = c_sum([
             (-m_diff + total_m) * z1,
             -c_sum([2. * total_m, z1 * c_sum([2. * z1, zeta])]) * zeta_conj,
             c_sum([2. * z1 + zeta]) * zeta_conj**2
-            ])
+        ])
         coeff_3 = c_sum([
             z1 * c_sum([m_diff * z1, -total_m * c_sum([z1, 2. * zeta])]),
             zeta_conj * c_sum([
                 2. * m_diff * z1,
                 c_sum([2. * total_m, z1**2]) * c_sum([z1, 2. * zeta])
-                ]),
+            ]),
             -z1 * c_sum([z1, 2. * zeta]) * zeta_conj**2
-            ])
+        ])
         coeff_2 = c_sum([
             m_diff * z1 * c_sum([2. * total_m, z1 * zeta]),
             total_m * c_sum([
                 -2. * total_m * z1, 4. * total_m * zeta, 3. * z1**2 * zeta]),
             -z1 * zeta_conj * c_sum([
                 zeta * c_sum([6. * total_m, z1**2]),
                 2. * m_diff * c_sum([z1, zeta])
-                ]),
+            ]),
             z1**2 * zeta * zeta_conj**2
-            ])
+        ])
         coeff_1 = -z1 * (m_diff + total_m) * c_sum([
             m_diff * z1, -total_m * z1, 4. * total_m * zeta, z1**2 * zeta,
             -2. * z1 * zeta * zeta_conj
-            ])
+        ])
         coeff_0 = (m_diff + total_m)**2 * z1**2 * zeta
 
         coeffs_list = [coeff_0, coeff_1, coeff_2, coeff_3, coeff_4, coeff_5]
         return np.array(coeffs_list).reshape(6)
 
     def _get_polynomial_roots(self, source_x, source_y):
         """roots of the polynomial"""
@@ -302,15 +203,15 @@
                     out[3]+out[8]*1.j, out[4]+out[9]*1.j])
         else:
             raise ValueError('Unknown solver: {:}'.format(self._solver))
         self._last_polynomial_input = polynomial_input
 
         return self._polynomial_roots
 
-    def _polynomial_roots_ok(
+    def _verify_polynomial_roots(
             self, source_x, source_y, return_distances=False):
         """verified roots of polynomial i.e. roots of lens equation"""
         roots = self._get_polynomial_roots(
             source_x=source_x, source_y=source_y)
 
         # Two lines below are simplified assuming
         # self._position_z1.imag = 0 and same for z2.
@@ -368,39 +269,39 @@
             raise ValueError(txt)
 
         if return_distances:
             return (np.array(out), np.array(distances))
         else:
             return np.array(out)
 
-    def _jacobian_determinant_ok(self, source_x, source_y):
+    def _get_jacobian_determinant(self, source_x, source_y):
         """determinants of lens equation Jacobian for verified roots"""
-        roots_ok_bar = np.conjugate(self._polynomial_roots_ok(
-                                   source_x=source_x, source_y=source_y))
+        roots_ok_bar = np.conjugate(self._verify_polynomial_roots(
+            source_x=source_x, source_y=source_y))
         # Variable X_bar is conjugate of variable X.
         add_1 = self.mass_1 / (self._position_z1 - roots_ok_bar)**2
         add_2 = self.mass_2 / (self._position_z2 - roots_ok_bar)**2
         derivative = add_1 + add_2
 
         return 1. - derivative * np.conjugate(derivative)
 
-    def _signed_magnification(self, source_x, source_y):
+    def _get_signed_magnification(self, source_x, source_y):
         """signed magnification for each image separately"""
-        return 1. / self._jacobian_determinant_ok(
-                source_x=source_x, source_y=source_y)
+        return 1. / self._get_jacobian_determinant(
+            source_x=source_x, source_y=source_y)
 
-    def _point_source(self, source_x, source_y):
+    def _get_point_source(self, source_x, source_y):
         """calculate point source magnification"""
-        signed_magnification = self._signed_magnification(
+        signed_magnification = self._get_signed_magnification(
             source_x=source_x, source_y=source_y)
         return fsum(abs(signed_magnification))
 
-    def _point_source_Witt_Mao_95(self, source_x, source_y):
+    def _get_point_source_Witt_Mao_95(self, source_x, source_y):
         """calculate point source magnification"""
-        return self._point_source(source_x=source_x, source_y=source_y)
+        return self._get_point_source(source_x=source_x, source_y=source_y)
 
     def point_source_magnification(self, source_x, source_y):
         """
         Calculate point source magnification for given position. The
         origin of the coordinate system is at the center of mass and
         both masses are on X axis with higher mass at negative X; this
         means that the higher mass is at (X, Y)=(-s*q/(1+q), 0) and
@@ -440,52 +341,53 @@
         the polynomial and MM code for rest.
         """
         if self._use_planet_frame:
             x_shift = -self.mass_1 / (self.mass_1 + self.mass_2)
         else:
             x_shift = self.mass_2 / (self.mass_1 + self.mass_2) - 0.5
         x_shift *= self.separation
-        return self._point_source_Witt_Mao_95(
-                source_x=float(source_x)+x_shift, source_y=float(source_y))
+        # We need to add this because in order to shift to correct frame.
+        return self._get_point_source_Witt_Mao_95(
+            source_x=float(source_x)+x_shift, source_y=float(source_y))
         # Casting to float speeds-up code for np.float input.
 
     def _get_magnification_w_plus(self, source_x, source_y, radius,
                                   magnification_center=None):
         """Evaluates Gould (2008) eq. 7"""
         dx = [1., 0., -1., 0.]
         dy = [0., 1., 0., -1.]
         out = []
         for (i, dxval) in enumerate(dx):
             x = source_x + dxval * radius
             y = source_y + dy[i] * radius
             out.append(self.point_source_magnification(
-                                              source_x=x, source_y=y))
+                source_x=x, source_y=y))
         if magnification_center is None:
             magnification_center = self.point_source_magnification(
-                                    source_x=source_x, source_y=source_y)
+                source_x=source_x, source_y=source_y)
         return 0.25 * fsum(out) - magnification_center
 
     def _get_magnification_w_times(self, source_x, source_y, radius,
                                    magnification_center=None):
         """Evaluates Gould (2008) eq. 8"""
         shift = radius / sqrt(2.)
         dx = [1., -1., -1., 1.]
         dy = [1., 1., -1., -1.]
         out = []
         for (i, dxval) in enumerate(dx):
             x = source_x + dxval * shift
             y = source_y + dy[i] * shift
             out.append(self.point_source_magnification(
-                                              source_x=x, source_y=y))
+                source_x=x, source_y=y))
         if magnification_center is None:
             magnification_center = self.point_source_magnification(
-                                    source_x=source_x, source_y=source_y)
+                source_x=source_x, source_y=source_y)
         return 0.25 * fsum(out) - magnification_center
 
-    def _rho_check(self, rho):
+    def _check_rho(self, rho):
         """
         Check if rho is float and positive.
         """
         if rho is None:
             raise TypeError(
                 'rho must be positive float, but None was provided')
         if not isinstance(rho, float):
@@ -536,15 +438,15 @@
                 point source approximations (*sequence* of three
                 *floats*) if *all_approximations* parameter is *True*.
         """
         # In this function, variables named a_* depict magnification.
         if quadrupole and all_approximations:
             raise ValueError('Inconsistent parameters of ' +
                              'BinaryLens.hexadecapole_magnification()')
-        self._rho_check(rho)
+        self._check_rho(rho)
 
         a_center = self.point_source_magnification(
             source_x=source_x, source_y=source_y)
         a_rho_half_plus = self._get_magnification_w_plus(
             source_x=source_x, source_y=source_y, radius=0.5*rho,
             magnification_center=a_center)
         a_rho_plus = self._get_magnification_w_plus(
@@ -635,15 +537,15 @@
 
         """
         if accuracy <= 0.:
             raise ValueError('adaptive_contouring requires accuracy > 0')
         if ld_accuracy <= 0.:
             raise ValueError('adaptive_contouring requires ld_accuracy > 0')
         # Note that this accuracy is not guaranteed.
-        self._rho_check(rho)
+        self._check_rho(rho)
 
         if not _adaptive_contouring_wrapped:
             raise ValueError('Adaptive Contouring was not imported properly')
 
         if gamma is not None and u_limb_darkening is not None:
             raise ValueError(
                 'Only one limb darkening parameters can be set' +
@@ -707,15 +609,15 @@
                 Requested accuracy of the result.
 
         Returns :
             magnification: *float*
                 Magnification.
 
         """
-        self._rho_check(rho)
+        self._check_rho(rho)
         if accuracy <= 0.:
             raise ValueError(
                 "VBBL requires accuracy > 0 e.g. 0.01 or 0.001;" +
                 "\n{:} was  provided".format(accuracy))
 
         if not _vbbl_wrapped:
             raise ValueError('VBBL was not imported properly')
```

### Comparing `MulensModel-2.7.2/source/MulensModel/caustics.py` & `MulensModel-2.8.1/source/MulensModel/caustics.py`

 * *Files 0% similar despite different names*

```diff
@@ -111,15 +111,15 @@
 
         # Distance between primary mass and center of mass
         xcm_offset = self.q * self.s / (1. + self.q)
 
         # Solve for the critical curve (and caustic) in complex coordinates.
         for phi in np.linspace(0., 2.*np.pi, n_angles, endpoint=False):
             # Change the angle to a complex number
-            eiphi = np.complex(cos(phi), sin(phi))
+            eiphi = complex(cos(phi), sin(phi))
 
             # Coefficients of Eq. 6
             coeff_4 = 1.
             coeff_3 = -2. * self.s
             coeff_2 = Utils.complex_fsum([self.s**2, -eiphi])
             coeff_1 = eiphi * (2. * self.s / (1. + self.q))  # The additional
             # parenthesis make it more stable numerically.
```

### Comparing `MulensModel-2.7.2/source/MulensModel/coordinates.py` & `MulensModel-2.8.1/source/MulensModel/coordinates.py`

 * *Files identical despite different names*

### Comparing `MulensModel-2.7.2/source/MulensModel/data/WFIRST_1827.dat` & `MulensModel-2.8.1/source/MulensModel/data/WFIRST_1827.dat`

 * *Files identical despite different names*

### Comparing `MulensModel-2.7.2/source/MulensModel/data/ephemeris_files/K2_ephemeris_01.dat` & `MulensModel-2.8.1/source/MulensModel/data/ephemeris_files/K2_ephemeris_01.dat`

 * *Files identical despite different names*

### Comparing `MulensModel-2.7.2/source/MulensModel/data/ephemeris_files/Spitzer_ephemeris_01.dat` & `MulensModel-2.8.1/source/MulensModel/data/ephemeris_files/Spitzer_ephemeris_01.dat`

 * *Files identical despite different names*

### Comparing `MulensModel-2.7.2/source/MulensModel/data/ephemeris_files/Spitzer_ephemeris_02.dat` & `MulensModel-2.8.1/source/MulensModel/data/ephemeris_files/Spitzer_ephemeris_02.dat`

 * *Files identical despite different names*

### Comparing `MulensModel-2.7.2/source/MulensModel/data/interpolate_elliptic_integral_1_2.dat` & `MulensModel-2.8.1/source/MulensModel/data/interpolate_elliptic_integral_1_2.dat`

 * *Files identical despite different names*

### Comparing `MulensModel-2.7.2/source/MulensModel/data/interpolate_elliptic_integral_1_2.py` & `MulensModel-2.8.1/source/MulensModel/data/interpolate_elliptic_integral_1_2.py`

 * *Files identical despite different names*

### Comparing `MulensModel-2.7.2/source/MulensModel/data/interpolate_elliptic_integral_3.dat` & `MulensModel-2.8.1/source/MulensModel/data/interpolate_elliptic_integral_3.dat`

 * *Files identical despite different names*

### Comparing `MulensModel-2.7.2/source/MulensModel/data/interpolate_elliptic_integral_3.py` & `MulensModel-2.8.1/source/MulensModel/data/interpolate_elliptic_integral_3.py`

 * *Files identical despite different names*

### Comparing `MulensModel-2.7.2/source/MulensModel/data/interpolation_table_b0b1_v1.dat` & `MulensModel-2.8.1/source/MulensModel/data/interpolation_table_b0b1_v1.dat`

 * *Files identical despite different names*

### Comparing `MulensModel-2.7.2/source/MulensModel/data/photometry_files/KB180003/KMTA12_I.pysis` & `MulensModel-2.8.1/source/MulensModel/data/photometry_files/KB180003/KMTA12_I.pysis`

 * *Files identical despite different names*

### Comparing `MulensModel-2.7.2/source/MulensModel/data/photometry_files/KB180003/KMTA14_I.pysis` & `MulensModel-2.8.1/source/MulensModel/data/photometry_files/KB180003/KMTA14_I.pysis`

 * *Files identical despite different names*

### Comparing `MulensModel-2.7.2/source/MulensModel/data/photometry_files/KB180003/KMTC12_I.pysis` & `MulensModel-2.8.1/source/MulensModel/data/photometry_files/KB180003/KMTC12_I.pysis`

 * *Files identical despite different names*

### Comparing `MulensModel-2.7.2/source/MulensModel/data/photometry_files/KB180003/KMTC14_I.pysis` & `MulensModel-2.8.1/source/MulensModel/data/photometry_files/KB180003/KMTC14_I.pysis`

 * *Files identical despite different names*

### Comparing `MulensModel-2.7.2/source/MulensModel/data/photometry_files/KB180003/KMTS12_I.pysis` & `MulensModel-2.8.1/source/MulensModel/data/photometry_files/KB180003/KMTS12_I.pysis`

 * *Files identical despite different names*

### Comparing `MulensModel-2.7.2/source/MulensModel/data/photometry_files/KB180003/KMTS14_I.pysis` & `MulensModel-2.8.1/source/MulensModel/data/photometry_files/KB180003/KMTS14_I.pysis`

 * *Files identical despite different names*

### Comparing `MulensModel-2.7.2/source/MulensModel/data/photometry_files/MB08310/Auck_0300089_PLC_001.tbl` & `MulensModel-2.8.1/source/MulensModel/data/photometry_files/MB08310/Auck_0300089_PLC_001.tbl`

 * *Files identical despite different names*

### Comparing `MulensModel-2.7.2/source/MulensModel/data/photometry_files/MB08310/Bron_0300089_PLC_002.tbl` & `MulensModel-2.8.1/source/MulensModel/data/photometry_files/MB08310/Bron_0300089_PLC_002.tbl`

 * *Files identical despite different names*

### Comparing `MulensModel-2.7.2/source/MulensModel/data/photometry_files/MB08310/CTIO_H_0300089_PLC_004.tbl` & `MulensModel-2.8.1/source/MulensModel/data/photometry_files/MB08310/CTIO_H_0300089_PLC_004.tbl`

 * *Files identical despite different names*

### Comparing `MulensModel-2.7.2/source/MulensModel/data/photometry_files/MB08310/CTIO_I_0300089_PLC_005.tbl` & `MulensModel-2.8.1/source/MulensModel/data/photometry_files/MB08310/CTIO_I_0300089_PLC_005.tbl`

 * *Files identical despite different names*

### Comparing `MulensModel-2.7.2/source/MulensModel/data/photometry_files/MB08310/Canopus_0300089_PLC_003.tbl` & `MulensModel-2.8.1/source/MulensModel/data/photometry_files/MB08310/Canopus_0300089_PLC_003.tbl`

 * *Files identical despite different names*

### Comparing `MulensModel-2.7.2/source/MulensModel/data/photometry_files/MB08310/Danish_0300089_PLC_006.tbl` & `MulensModel-2.8.1/source/MulensModel/data/photometry_files/MB08310/Danish_0300089_PLC_006.tbl`

 * *Files identical despite different names*

### Comparing `MulensModel-2.7.2/source/MulensModel/data/photometry_files/MB08310/MOA_0300089_PLC_007.tbl` & `MulensModel-2.8.1/source/MulensModel/data/photometry_files/MB08310/MOA_0300089_PLC_007.tbl`

 * *Files identical despite different names*

### Comparing `MulensModel-2.7.2/source/MulensModel/data/photometry_files/OB03235/OB03235_MOA.tbl.txt` & `MulensModel-2.8.1/source/MulensModel/data/photometry_files/OB03235/OB03235_MOA.tbl.txt`

 * *Files identical despite different names*

### Comparing `MulensModel-2.7.2/source/MulensModel/data/photometry_files/OB03235/OB03235_OGLE.tbl.txt` & `MulensModel-2.8.1/source/MulensModel/data/photometry_files/OB03235/OB03235_OGLE.tbl.txt`

 * *Files identical despite different names*

### Comparing `MulensModel-2.7.2/source/MulensModel/data/photometry_files/OB05086/starBLG234.6.I.218982.dat` & `MulensModel-2.8.1/source/MulensModel/data/photometry_files/OB05086/starBLG234.6.I.218982.dat`

 * *Files identical despite different names*

### Comparing `MulensModel-2.7.2/source/MulensModel/data/photometry_files/OB08092/phot_ob08092_O4.dat` & `MulensModel-2.8.1/source/MulensModel/data/photometry_files/OB08092/phot_ob08092_O4.dat`

 * *Files identical despite different names*

### Comparing `MulensModel-2.7.2/source/MulensModel/data/photometry_files/OB140939/ob140939_OGLE.dat` & `MulensModel-2.8.1/source/MulensModel/data/photometry_files/OB140939/ob140939_OGLE.dat`

 * *Files identical despite different names*

### Comparing `MulensModel-2.7.2/source/MulensModel/data/photometry_files/OB140939/ob140939_Spitzer.dat` & `MulensModel-2.8.1/source/MulensModel/data/photometry_files/OB140939/ob140939_Spitzer.dat`

 * *Files identical despite different names*

### Comparing `MulensModel-2.7.2/source/MulensModel/data/photometry_files/OB161195/KCT01I.dat` & `MulensModel-2.8.1/source/MulensModel/data/photometry_files/OB161195/KCT01I.dat`

 * *Files identical despite different names*

### Comparing `MulensModel-2.7.2/source/MulensModel/data/photometry_files/OB161195/KCT41I.dat` & `MulensModel-2.8.1/source/MulensModel/data/photometry_files/OB161195/KCT41I.dat`

 * *Files identical despite different names*

### Comparing `MulensModel-2.7.2/source/MulensModel/data/photometry_files/OB161195/KCT42I.dat` & `MulensModel-2.8.1/source/MulensModel/data/photometry_files/OB161195/KCT42I.dat`

 * *Files identical despite different names*

### Comparing `MulensModel-2.7.2/source/MulensModel/data/photometry_files/OB161195/KSA01I.dat` & `MulensModel-2.8.1/source/MulensModel/data/photometry_files/OB161195/KSA01I.dat`

 * *Files identical despite different names*

### Comparing `MulensModel-2.7.2/source/MulensModel/data/photometry_files/OB161195/KSA41I.dat` & `MulensModel-2.8.1/source/MulensModel/data/photometry_files/OB161195/KSA41I.dat`

 * *Files identical despite different names*

### Comparing `MulensModel-2.7.2/source/MulensModel/data/photometry_files/OB161195/KSA42I.dat` & `MulensModel-2.8.1/source/MulensModel/data/photometry_files/OB161195/KSA42I.dat`

 * *Files identical despite different names*

### Comparing `MulensModel-2.7.2/source/MulensModel/data/photometry_files/OB161195/KSS01I.dat` & `MulensModel-2.8.1/source/MulensModel/data/photometry_files/OB161195/KSS01I.dat`

 * *Files identical despite different names*

### Comparing `MulensModel-2.7.2/source/MulensModel/data/photometry_files/OB161195/KSS41I.dat` & `MulensModel-2.8.1/source/MulensModel/data/photometry_files/OB161195/KSS41I.dat`

 * *Files identical despite different names*

### Comparing `MulensModel-2.7.2/source/MulensModel/data/photometry_files/OB161195/KSS42I.dat` & `MulensModel-2.8.1/source/MulensModel/data/photometry_files/OB161195/KSS42I.dat`

 * *Files identical despite different names*

### Comparing `MulensModel-2.7.2/source/MulensModel/data/unit_test_files/FSPL_test.dat` & `MulensModel-2.8.1/source/MulensModel/data/unit_test_files/FSPL_test.dat`

 * *Files identical despite different names*

### Comparing `MulensModel-2.7.2/source/MulensModel/data/unit_test_files/FSPL_test_1.dat` & `MulensModel-2.8.1/source/MulensModel/data/unit_test_files/FSPL_test_1.dat`

 * *Files identical despite different names*

### Comparing `MulensModel-2.7.2/source/MulensModel/data/unit_test_files/MB11293_caustics.dat` & `MulensModel-2.8.1/source/MulensModel/data/unit_test_files/MB11293_caustics.dat`

 * *Files identical despite different names*

### Comparing `MulensModel-2.7.2/source/MulensModel/data/unit_test_files/earth_position_1.dat` & `MulensModel-2.8.1/source/MulensModel/data/unit_test_files/earth_position_1.dat`

 * *Files identical despite different names*

### Comparing `MulensModel-2.7.2/source/MulensModel/data/unit_test_files/earth_position_2.dat` & `MulensModel-2.8.1/source/MulensModel/data/unit_test_files/earth_position_2.dat`

 * *Files identical despite different names*

### Comparing `MulensModel-2.7.2/source/MulensModel/data/unit_test_files/ob140939_OGLE_ref_v1.dat` & `MulensModel-2.8.1/source/MulensModel/data/unit_test_files/ob140939_OGLE_ref_v1.dat`

 * *Files identical despite different names*

### Comparing `MulensModel-2.7.2/source/MulensModel/data/unit_test_files/ob140939_Spitzer_ref_v1.dat` & `MulensModel-2.8.1/source/MulensModel/data/unit_test_files/ob140939_Spitzer_ref_v1.dat`

 * *Files identical despite different names*

### Comparing `MulensModel-2.7.2/source/MulensModel/data/unit_test_files/ob151100_OGLE_ref_v1.dat` & `MulensModel-2.8.1/source/MulensModel/data/unit_test_files/ob151100_OGLE_ref_v1.dat`

 * *Files identical despite different names*

### Comparing `MulensModel-2.7.2/source/MulensModel/data/unit_test_files/ob151100_Spitzer_ref_v1.dat` & `MulensModel-2.8.1/source/MulensModel/data/unit_test_files/ob151100_Spitzer_ref_v1.dat`

 * *Files identical despite different names*

### Comparing `MulensModel-2.7.2/source/MulensModel/data/unit_test_files/parallax_test_1.dat` & `MulensModel-2.8.1/source/MulensModel/data/unit_test_files/parallax_test_1.dat`

 * *Files identical despite different names*

### Comparing `MulensModel-2.7.2/source/MulensModel/data/unit_test_files/parallax_test_2.dat` & `MulensModel-2.8.1/source/MulensModel/data/unit_test_files/parallax_test_2.dat`

 * *Files identical despite different names*

### Comparing `MulensModel-2.7.2/source/MulensModel/data/unit_test_files/parallax_test_3.dat` & `MulensModel-2.8.1/source/MulensModel/data/unit_test_files/parallax_test_3.dat`

 * *Files identical despite different names*

### Comparing `MulensModel-2.7.2/source/MulensModel/data/unit_test_files/parallax_test_4.dat` & `MulensModel-2.8.1/source/MulensModel/data/unit_test_files/parallax_test_4.dat`

 * *Files identical despite different names*

### Comparing `MulensModel-2.7.2/source/MulensModel/data/unit_test_files/parallax_test_5.dat` & `MulensModel-2.8.1/source/MulensModel/data/unit_test_files/parallax_test_5.dat`

 * *Files identical despite different names*

### Comparing `MulensModel-2.7.2/source/MulensModel/event.py` & `MulensModel-2.8.1/source/MulensModel/event.py`

 * *Files 0% similar despite different names*

```diff
@@ -757,16 +757,16 @@
         """an instance of :py:class:`~MulensModel.model.Model`"""
         return self._model
 
     @model.setter
     def model(self, new_value):
         if not isinstance(new_value, Model):
             raise TypeError((
-                    'wrong type of Event.model: {:} instead of ' +
-                    'MulensModel.Model()').format(type(new_value)))
+                'wrong type of Event.model: {:} instead of ' +
+                'MulensModel.Model()').format(type(new_value)))
         self._model = new_value
 
         if new_value.coords is not None:
             self._update_coords(coords=new_value.coords)
 
         self._fits = None  # reset the fits if the model changed.
 
@@ -837,15 +837,15 @@
             except ValueError:
                 pass
             else:
                 raise ValueError(
                     'Dataset is included in Event.datasets more than once.')
 
             self._data_ref = index
-        elif isinstance(new_value, (int, np.int)):
+        elif isinstance(new_value, (int, np.int_)):
             self._data_ref = new_value
         else:
             raise TypeError(
                 'data_ref must be set using either *int* or *MulensData*: ' +
                 '{0}'.format(type(new_value)))
 
     @property
```

### Comparing `MulensModel-2.7.2/source/MulensModel/fitdata.py` & `MulensModel-2.8.1/source/MulensModel/fitdata.py`

 * *Files 0% similar despite different names*

```diff
@@ -385,15 +385,15 @@
 
         model_flux = np.ones(self._dataset.n_epochs) * self.blend_flux
         if self._model.n_sources == 1:
             model_flux += self.source_flux * self._data_magnification
         else:
             for i in range(self._model.n_sources):
                 model_flux += self.source_fluxes[i] \
-                        * self._data_magnification[i]
+                    * self._data_magnification[i]
 
         return model_flux
 
     def get_model_magnitudes(self, **kwargs):
         """
         Calculate model in magnitude space
```

### Comparing `MulensModel-2.7.2/source/MulensModel/horizons.py` & `MulensModel-2.8.1/source/MulensModel/horizons.py`

 * *Files identical despite different names*

### Comparing `MulensModel-2.7.2/source/MulensModel/limbdarkeningcoeffs.py` & `MulensModel-2.8.1/source/MulensModel/limbdarkeningcoeffs.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,14 +13,15 @@
     gamma = (2 * u) / (3 - u)
 
     u = 3 * gamma / (2 + gamma)
 
     Note that the gamma convention has fixed total flux.
 
     """
+
     def __init__(self):
         self._gammas_for_band = dict()
 
     def set_limb_coeff_gamma(self, bandpass, gamma):
         """
         Remembers limb darkening gamma coefficient for given band.
```

### Comparing `MulensModel-2.7.2/source/MulensModel/magnificationcurve.py` & `MulensModel-2.8.1/source/MulensModel/magnificationcurve.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,17 @@
-import numpy as np
 import math
 import warnings
 
-from MulensModel.trajectory import Trajectory
-from MulensModel.pointlens import PointLens, get_pspl_magnification
+import numpy as np
+
 from MulensModel.binarylens import BinaryLens
+from MulensModel.binarylenswithshear import BinaryLensWithShear
 from MulensModel.modelparameters import ModelParameters
+from MulensModel.pointlens import PointLens, get_pspl_magnification
+from MulensModel.trajectory import Trajectory
 
 
 class MagnificationCurve(object):
     """
     The magnification curve calculated from the model light curve.
 
     The key function is :py:func:`set_magnification_methods`, which
@@ -40,21 +42,19 @@
             limb darkening coefficient in gamma convention; defaults to 0
 
     Attributes :
         trajectory: :py:class:`~MulensModel.Trajectory.trajectory`
             Trajectory used to calculate positions of
             the source that are used to calculate magnification values.
     """
+
     def __init__(self, times, parameters, parallax=None,
                  coords=None, satellite_skycoord=None, gamma=0.):
         # Set times
-        if isinstance(times, (list, tuple, np.ndarray)):
-            self.times = times
-        else:
-            self.times = np.array(times)
+        self.times = np.asarray(times)
 
         # Check for ModelParameters and set.
         if isinstance(parameters, ModelParameters):
             self.parameters = parameters
         else:
             raise ValueError(
                 'parameters is a required keyword and must be a ' +
@@ -156,15 +156,15 @@
 
         """
         if self.parameters.rho is not None:
             self._check_for_finite_source_method()
 
         if self.parameters.n_lenses == 1:
             magnification = self.get_point_lens_magnification()
-        elif self.parameters.n_lenses == 2:
+        elif (self.parameters.n_lenses == 2):
             magnification = self.get_binary_lens_magnification()
         else:
             raise NotImplementedError(
                 "magnification for more than 2 lenses not handled yet")
         self._magnification = magnification
         return self._magnification
 
@@ -179,15 +179,16 @@
             warnings.warn('no finite-source method is set', UserWarning)
             return
 
     def get_point_lens_magnification(self):
         """
         Calculate the Point Lens magnification.
 
-        Allowed magnification methods :
+        Allowed magnification methods
+        (set by :py:func:`set_magnification_methods()`) :
             ``point_source``:
                 standard Paczynski equation for a point source/point lens.
 
             ``finite_source_uniform_Gould94``:
                 Uses the `Gould 1994 ApJ, 421L, 71
                 <https://ui.adsabs.harvard.edu/abs/1994ApJ...421L..71G/abstract>`_
                 prescription assuming a
@@ -243,14 +244,19 @@
                 compared to other methods.
 
         Returns :
             magnification: *np.ndarray*
                 Vector of magnifications.
 
         """
+        if self.parameters.n_lenses != 1:
+            raise ValueError(
+                "You're trying to calculate single lens magnification, but "
+                "the model provided has " + str(self.parameters.n_lenses) +
+                " lenses")
 
         pspl_magnification = get_pspl_magnification(self.trajectory)
         if self._methods_epochs is None:
             return pspl_magnification
         point_lens = PointLens(self.parameters)
         magnification = pspl_magnification
         u2 = self.trajectory.x**2 + self.trajectory.y**2
@@ -321,16 +327,18 @@
                 raise ValueError(msg.format(method))
 
         return magnification
 
     def get_binary_lens_magnification(self):
         """
         Calculate the binary lens magnification.
+        If the shear or convergence are set, then they are used.
 
-        Allowed magnification methods :
+        Allowed magnification methods
+        (set by :py:func:`set_magnification_methods()`) :
             ``point_source``:
                 standard point source magnification calculation.
 
             ``quadrupole``:
                 From `Gould 2008 ApJ, 681, 1593
                 <https://ui.adsabs.harvard.edu/abs/2008ApJ...681.1593G/abstract>`_.
                 See
@@ -352,44 +360,70 @@
                 Uses AdaptiveContouring (a Stokes theorem/contour
                 integration code) by Martin Dominik
                 (`Dominik 2007 MNRAS, 377, 1679
                 <https://ui.adsabs.harvard.edu/abs/2007MNRAS.377.1679D/abstract>`_).
                 See
                 :py:func:`~MulensModel.binarylens.BinaryLens.adaptive_contouring_magnification()`
 
+                Note that it doesn't work if shear or convergence are set.
+
             ``point_source_point_lens``:
                 Uses point-source _point_-_lens_ approximation; useful when you
                 consider binary lens but need magnification very far from
                 the lens (e.g. at separation u = 100).
 
         Returns :
             magnification: *np.ndarray*
                 Vector of magnifications.
 
         """
-        # Set up the binary lens system
+        if self.parameters.n_lenses != 2:
+            raise ValueError(
+                "You're trying to calculate binary lens magnification, but "
+                "the model provided has " + str(self.parameters.n_lenses) +
+                " lenses")
+
+        if not self.parameters.is_external_mass_sheet:
+            binary_lens_class = BinaryLens
+            kwargs = dict()
+        else:
+            binary_lens_class = BinaryLensWithShear
+            kwargs = {'convergence_K': self.parameters.convergence_K,
+                      'shear_G': self.parameters.shear_G}
+
+        out = self._get_binary_lens_magnification(binary_lens_class, kwargs)
+
+        return out
+
+    def _get_binary_lens_magnification(self, binary_lens_class,
+                                       optional_kwargs):
+        """
+        Run binary lens calculation with proper class (binary_lens_class) and
+        some kwargs (optional_kwargs of type *dict*).
+        """
         q = self.parameters.q
-        m_1 = 1. / (1. + q)
-        m_2 = q / (1. + q)
+        binary_kwargs = optional_kwargs
+        binary_kwargs['mass_1'] = 1. / (1. + q)
+        binary_kwargs['mass_2'] = q / (1. + q)
+
         is_static = self.parameters.is_static()
         if is_static:
-            binary_lens = BinaryLens(
-                mass_1=m_1, mass_2=m_2, separation=self.parameters.s)
+            binary_lens = binary_lens_class(separation=self.parameters.s,
+                                            **binary_kwargs)
         methods = self._methods_for_epochs()
 
-        # Calculate the magnification
         magnification = []
         for index in range(len(self.times)):
             x = self.trajectory.x[index]
             y = self.trajectory.y[index]
             method = methods[index].lower()
             if not is_static:
-                binary_lens = BinaryLens(
-                    mass_1=m_1, mass_2=m_2,
-                    separation=self.parameters.get_s(self.times[index]))
+                binary_lens = binary_lens_class(
+                    separation=self.parameters.get_s(self.times[index]),
+                    **binary_kwargs)
 
             kwargs = {}
             if self._methods_parameters is not None:
                 if method in self._methods_parameters.keys():
                     kwargs = self._methods_parameters[method]
                     if method not in ['vbbl', 'adaptive_contouring']:
                         msg = ('Methods parameters passed for method {:}' +
@@ -410,17 +444,23 @@
                 m = binary_lens.hexadecapole_magnification(
                     x, y, rho=self.parameters.rho, quadrupole=True,
                     gamma=self._gamma)
             elif method == 'hexadecapole':
                 m = binary_lens.hexadecapole_magnification(
                     x, y, rho=self.parameters.rho, gamma=self._gamma)
             elif method == 'vbbl':
+                if isinstance(binary_lens, BinaryLensWithShear):
+                    raise ValueError("Finite source VBBL is not available "
+                                     "for BinaryLensWithShear")
                 m = binary_lens.vbbl_magnification(
                     x, y, rho=self.parameters.rho, gamma=self._gamma, **kwargs)
             elif method == 'adaptive_contouring':
+                if isinstance(binary_lens, BinaryLensWithShear):
+                    raise ValueError("Adaptive contouring is not available "
+                                     "for BinaryLensWithShear")
                 m = binary_lens.adaptive_contouring_magnification(
                     x, y, rho=self.parameters.rho, gamma=self._gamma, **kwargs)
             elif method == 'point_source_point_lens':
                 u = math.sqrt(x**2 + y**2)
                 m = get_pspl_magnification(u)
             else:
                 msg = 'Unknown method specified for binary lens: {:}'
```

### Comparing `MulensModel-2.7.2/source/MulensModel/model.py` & `MulensModel-2.8.1/source/MulensModel/model.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import warnings
 import numpy as np
 import matplotlib.pyplot as plt
 
 from astropy.coordinates import SkyCoord
 
 from MulensModel.caustics import Caustics
+from MulensModel.causticswithshear import CausticsWithShear
 from MulensModel.coordinates import Coordinates
 from MulensModel.limbdarkeningcoeffs import LimbDarkeningCoeffs
 from MulensModel.magnificationcurve import MagnificationCurve
 from MulensModel.modelparameters import ModelParameters
 from MulensModel.mulensdata import MulensData
 from MulensModel.satelliteskycoord import SatelliteSkyCoord
 from MulensModel.trajectory import Trajectory
@@ -465,15 +466,22 @@
         else:
             s = self.parameters.get_s(epoch)
 
         if self._caustics is not None:
             if s == self._caustics.s and self.parameters.q == self._caustics.q:
                 return
 
-        self._caustics = Caustics(q=self.parameters.q, s=s)
+        # check if covergence_K and shear_G are in parameters
+        if self.parameters.is_external_mass_sheet:
+            self._caustics = CausticsWithShear(
+                q=self.parameters.q, s=s,
+                convergence_K=self.parameters.convergence_K,
+                shear_G=self.parameters.shear_G)
+        else:
+            self._caustics = Caustics(q=self.parameters.q, s=s)
 
     def plot_trajectory(
             self, times=None, t_range=None, t_start=None, t_stop=None,
             dt=None, n_epochs=None, caustics=False,
             arrow=True, satellite_skycoord=None, arrow_kwargs=None,
             show_data=None, **kwargs):
         """
@@ -567,15 +575,15 @@
                 times, self.parameters.source_1_parameters,
                 satellite_skycoord, arrow, arrow_kwargs, **kwargs)
             self._plot_single_trajectory(
                 times, self.parameters.source_2_parameters,
                 satellite_skycoord, arrow, arrow_kwargs, **kwargs)
         else:
             raise ValueError(
-                    'Wrong number of sources: {:}'.format(self.n_sources))
+                'Wrong number of sources: {:}'.format(self.n_sources))
 
         if caustics:
             self.plot_caustics(marker='.', color='red')
 
     def _plot_single_trajectory(self, times, parameters, satellite_skycoord,
                                 arrow, arrow_kwargs, **kwargs):
         """
@@ -635,18 +643,15 @@
         (the other possible options are ``'scaled'`` or ``'square'``).
 
         .. _matplotlib.Circle:
           https://matplotlib.org/api/_as_gen/matplotlib.patches.Circle.html
         .. _matplotlib.plot:
           https://matplotlib.org/api/_as_gen/matplotlib.pyplot.plot.html
         """
-        if isinstance(times, float):
-            times = [times]
-        if isinstance(times, list):
-            times = np.array(times)
+        times = np.atleast_1d(times)
 
         kwargs_ = {
             'times': times, 'parallax': self._parallax, 'coords': self._coords,
             'satellite_skycoord': self.get_satellite_coords(times)}
 
         if self.n_sources == 1:
             trajectory = Trajectory(parameters=self.parameters, **kwargs_)
@@ -1024,15 +1029,15 @@
                 `ephemerides_file` is not set, returns *None*.
 
         """
         if self.ephemerides_file is None:
             return None
         else:
             satellite_skycoords = SatelliteSkyCoord(
-                 ephemerides_file=self.ephemerides_file)
+                ephemerides_file=self.ephemerides_file)
             return satellite_skycoords.get_satellite_coords(times)
 
     def get_magnification(self, time, satellite_skycoord=None, gamma=None,
                           bandpass=None, source_flux_ratio=None,
                           separate=False, flux_ratio_constraint=None):
         """
         Calculate the model magnification for the given time(s).
@@ -1122,22 +1127,15 @@
         return self.get_magnification(*args, **kwargs)
 
     def _get_magnification(self, time, satellite_skycoord, gamma,
                            source_flux_ratio, separate):
         """
         Internal function that calculates magnification.
         """
-        if not isinstance(time, np.ndarray):
-            if isinstance(time, (np.float, float, np.int, int)):
-                time = np.array([time])
-            elif isinstance(time, list):
-                time = np.array(time)
-            else:
-                raise TypeError(
-                    'time must be a float, int, list, or np.ndarray')
+        time = np.atleast_1d(time)
 
         if satellite_skycoord is None:
             satellite_skycoord = self.get_satellite_coords(time)
 
         if self.n_sources == 1:
             if source_flux_ratio is not None:
                 raise ValueError(
@@ -1199,15 +1197,15 @@
         if separate and (source_flux_ratio is not None):
             raise ValueError(
                 'You cannot set both source_flux_ratio and separate' +
                 " parameters in Model.get_magnification(). This doesn't " +
                 'make sense')
 
         (mag_1, mag_2) = self._separate_magnifications(
-                time, satellite_skycoord, gamma)
+            time, satellite_skycoord, gamma)
 
         if separate:
             return (mag_1, mag_2)
         else:
             magnification = mag_1 + mag_2 * source_flux_ratio
             magnification /= (1. + source_flux_ratio)
             return magnification
```

### Comparing `MulensModel-2.7.2/source/MulensModel/modelparameters.py` & `MulensModel-2.8.1/source/MulensModel/modelparameters.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,22 +7,24 @@
 
 # For definition of class ModelParameters see below.
 
 # Different parameter sets. Any parameters that may be given as
 # 'basic' should be a list. Parameters that may be 'optional' should
 # be a list of length 2. The second item will only be printed if the
 # effect is included in the 'optional' list (see _get_effect_strings()).
+
 _valid_parameters = {
     'point lens': ['t_0, u_0, t_E'],
     'point lens alt': 'alternate: t_eff may be substituted for u_0 or t_E',
     'binary lens': ['s, q, alpha'],
     'binary lens alt':
         'alternate: ' +
         '(x_caustic_in, x_caustic_out, t_caustic_in, t_caustic_out) ' +
         'may be substituted for (t_0, u_0, t_E, alpha)',
+    'binary_lens_shear': ['convergence_K', 'shear_G'],
     'finite source': ['rho', '(for finite source effects)'],
     'finite source alt': 'alternate: t_star may be substituted for t_E or rho',
     'parallax': ['(pi_E_N, pi_E_E) OR pi_E', '(for parallax)'],
     'parallax opt': [
         't_0_par',
         'may also be specified for parallax models. Defaults to t_0.'],
     'lens orbital motion': ['dalpha_dt, ds_dt', '(for orbital motion)'],
@@ -120,15 +122,15 @@
     if len(components['alternate']) > 0:
         for item in components['alternate']:
             print('{0}'.format(_valid_parameters[item]))
 
     if len(components['optional']) > 0:
         for item in components['optional']:
             print('optional: {0} {1}'.format(
-                    _valid_parameters[item][0], _valid_parameters[item][1]))
+                _valid_parameters[item][0], _valid_parameters[item][1]))
 
 
 def _print_all():
     """
     Give the user general information about common models and effects.
     """
     print('------------------------')
@@ -177,16 +179,16 @@
         header = '---------\n{0} parameters:'.format(args[0])
         _print_parameters(header, components)
 
 
 class ModelParameters(object):
     """
     A class for the basic microlensing model parameters (t_0, u_0,
-    t_E, rho, s, q, alpha, pi_E). Can handle point lens or binary
-    lens. The pi_E assumes NE coordinates (Parallel, Perpendicular
+    t_E, s, q, alpha, etc.). Can handle point lens or binary lens.
+    The pi_E assumes NE coordinates (Parallel, Perpendicular
     coordinates are not supported).
 
     Arguments :
         parameters: *dictionary*
             A dictionary of parameters and their values. See
             :py:func:`which_parameters()` for valid parameter combinations.
 
@@ -202,14 +204,15 @@
             ``params = ModelParameters({'t_0': 2450000., 'u_0': 0.3,
             't_E': 35.})``
 
         Then you can print the parameters:
             ``print(params)``
 
     """
+
     def __init__(self, parameters):
         if not isinstance(parameters, dict):
             raise TypeError(
                 'ModelParameters must be initialized with dict ' +
                 "as a parameter\ne.g., ModelParameters({'t_0': " +
                 "2456789.0, 'u_0': 0.123, 't_E': 23.45})")
 
@@ -271,15 +274,15 @@
         sets self._type property, which indicates what type of a model we have
         """
         types = ['finite source', 'parallax', 'Cassan08',
                  'lens 2-parameter orbital motion']
         out = {type_: False for type_ in types}
 
         parameter_to_type = dict()
-        for key in ['rho' 't_star', 'rho_1', 'rho_2', 't_star_1', 't_star_2']:
+        for key in ['rho', 't_star', 'rho_1', 'rho_2', 't_star_1', 't_star_2']:
             parameter_to_type[key] = 'finite source'
         for key in ['pi_E', 'pi_E_N', 'pi_E_E']:
             parameter_to_type[key] = 'parallax'
         keys_Cassan08 = ['x_caustic_in', 'x_caustic_out',
                          't_caustic_in', 't_caustic_out']
         for key in keys_Cassan08:
             parameter_to_type[key] = 'Cassan08'
@@ -356,14 +359,16 @@
             'rho': {'width': 7, 'precision': 5},
             't_star': {'width': 13, 'precision': 6, 'unit': 'd'},
             'pi_E_N': {'width': 9, 'precision': 5},
             'pi_E_E': {'width': 9, 'precision': 5},
             's': {'width': 9, 'precision': 5},
             'q': {'width': 12, 'precision': 8},
             'alpha': {'width': 11, 'precision': 5, 'unit': 'deg'},
+            'convergence_K': {'width': 12, 'precision': 8},
+            'shear_G': {'width': 12, 'precision': 8},
             'ds_dt': {
                 'width': 11, 'precision': 5, 'unit': '/yr', 'name': 'ds/dt'},
             'dalpha_dt': {
                 'width': 18, 'precision': 5, 'unit': 'deg/yr',
                 'name': 'dalpha/dt'},
             'x_caustic_in': {'width': 13, 'precision': 7},
             'x_caustic_out': {'width': 13, 'precision': 7},
@@ -380,15 +385,16 @@
             if 'unit' in form:
                 formats[key]['unit'] = form['unit']
             if 'name' in form:
                 raise KeyError('internal issue: {:}'.format(key))
         formats_keys = [
             't_0', 't_0_1', 't_0_2', 'u_0', 'u_0_1', 'u_0_2', 't_eff', 't_E',
             'rho', 'rho_1', 'rho_2', 't_star', 't_star_1', 't_star_2',
-            'pi_E_N', 'pi_E_E', 's', 'q', 'alpha', 'ds_dt', 'dalpha_dt',
+            'pi_E_N', 'pi_E_E', 's', 'q', 'alpha',
+            'convergence_K', 'shear_G', 'ds_dt', 'dalpha_dt',
             'x_caustic_in', 'x_caustic_out', 't_caustic_in', 't_caustic_out',
         ]
 
         variables = ''
         values = ''
 
         for key in formats_keys:
@@ -415,15 +421,15 @@
         """
         binary_params = ['t_0_1', 't_0_2', 'u_0_1', 'u_0_2', 'rho_1', 'rho_2',
                          't_star_1', 't_star_2']
         for parameter in binary_params:
             if parameter in keys:
                 if parameter[:-2] in keys:
                     raise ValueError('You cannot set {:} and {:}'.format(
-                                        parameter, parameter[:-2]))
+                        parameter, parameter[:-2]))
 
     def _check_valid_combination_1_source_standard(self, keys):
         """
         Here we check parameters for non-Cassan08 parameterization.
         """
         self._check_valid_combination_1_source_1_lens(keys)
         self._check_valid_combination_1_source_parallax(keys)
@@ -482,21 +488,29 @@
                     'Parallax is defined, hence either t_0 or t_0_par has ' +
                     'to be set.')
 
     def _check_valid_combination_1_source_binary_lens(self, keys):
         """
         Here we check binary lens parameters for non-Cassan08 parameterization.
         """
-        # If s, q, and alpha must all be defined if one is defined
+        # s, q, and alpha must all be defined if one is defined
         if ('s' in keys) or ('q' in keys) or ('alpha' in keys):
             if (('s' not in keys) or
                     ('q' not in keys) or ('alpha' not in keys)):
                 raise KeyError(
                     'A binary model requires all three of (s, q, alpha).')
 
+        # convergence_K and shear_G must both be defined if one is defined
+        if ('convergence_K' in keys) or ('shear_G' in keys):
+            if (('convergence_K' not in keys) or
+                    ('shear_G' not in keys)):
+                raise KeyError(
+                    'A binary model with external shear requires both of '
+                    '(convergence_K, shear_G).')
+
         # If ds_dt is defined, dalpha_dt must be defined
         if ('ds_dt' in keys) or ('dalpha_dt' in keys):
             if ('ds_dt' not in keys) or ('dalpha_dt' not in keys):
                 raise KeyError(
                     'Lens orbital motion requires both ds_dt and dalpha_dt.' +
                     '\nNote that you can set either of them to 0.')
         # If orbital motion is defined, then reference epoch has to be set.
@@ -533,16 +547,18 @@
 
     def _check_valid_combination_1_source(self, keys):
         """
         Check that the user hasn't over-defined the ModelParameters.
         """
         # Make sure that there are no unwanted keys
         allowed_keys = set([
-            't_0', 'u_0', 't_E', 't_eff', 's', 'q', 'alpha', 'rho', 't_star',
-            'pi_E', 'pi_E_N', 'pi_E_E', 't_0_par', 'dalpha_dt', 'ds_dt',
+            't_0', 'u_0', 't_E', 't_eff', 'rho', 't_star',
+            'pi_E', 'pi_E_N', 'pi_E_E', 't_0_par',
+            's', 'q', 'alpha', 'convergence_K', 'shear_G',
+            'dalpha_dt', 'ds_dt',
             't_0_kep', 't_0_1', 't_0_2', 'u_0_1', 'u_0_2', 'rho_1', 'rho_2',
             't_star_1', 't_star_2', 'x_caustic_in', 'x_caustic_out',
             't_caustic_in', 't_caustic_out'])
         difference = set(keys) - allowed_keys
         if len(difference) > 0:
             derived_1 = ['gamma', 'gamma_perp', 'gamma_parallel']
             if set(keys).intersection(derived_1):
@@ -558,29 +574,29 @@
             self._check_valid_combination_1_source_Cassan08(keys)
         else:
             self._check_valid_combination_1_source_standard(keys)
 
     def _check_valid_parameter_values(self, parameters):
         """
         Prevent user from setting negative (unphysical) values for
-        t_E, t_star, rho etc.
+        t_E, t_star, rho etc. Shear_G should be complex.
 
         Also, check that all values are scalars (except pi_E vector).
         """
-        names = ['t_E', 't_star', 'rho', 's']
+        names = ['t_E', 't_star', 'rho', 's', 'convergence_K']
         full_names = {
             't_E': 'Einstein timescale',
             't_star': 'Source crossing time', 'rho': 'Source size',
-            's': 'separation'}
+            's': 'separation', 'convergence_K': 'external convergence'}
 
         for name in names:
             if name in parameters.keys():
                 if parameters[name] < 0.:
                     raise ValueError("{:} cannot be negative: {:}".format(
-                            full_names[name], parameters[name]))
+                        full_names[name], parameters[name]))
 
         for (key, value) in parameters.items():
             if key == 'pi_E':
                 continue
             check = (not np.isscalar(value) or isinstance(value, str))
             if not isinstance(value, u.Quantity) and check:
                 msg = "{:} must be a scalar: {:}, {:}"
@@ -588,14 +604,18 @@
 
         for name in ['x_caustic_in', 'x_caustic_out', 'q']:
             if name in parameters.keys():
                 if parameters[name] < 0. or parameters[name] > 1.:
                     msg = "Parameter {:} has to be in (0, 1) range, not {:}"
                     raise ValueError(msg.format(name, parameters[name]))
 
+        if 'shear_G' in parameters.keys():
+            if not isinstance(parameters['shear_G'], complex):
+                raise TypeError("External shear (shear_G) must be complex")
+
     def _set_parameters(self, parameters):
         """
         check if parameter values make sense and remember the copy of the dict
         """
         self._check_valid_parameter_values(parameters)
         self.parameters = dict(parameters)
 
@@ -901,14 +921,54 @@
     def q(self, new_q):
         if new_q < 0. or new_q > 1.:
             raise ValueError('mass ratio q has to be between 0 and 1')
         self.parameters['q'] = new_q
         self._update_sources('q', new_q)
 
     @property
+    def convergence_K(self):
+        """
+        *float*
+
+        Convergence of external mass sheet.
+        """
+        if 'convergence_K' in self.parameters.keys():
+            return self.parameters['convergence_K']
+        else:
+            raise KeyError('convergence_K is not a parameter of this model.')
+
+    @convergence_K.setter
+    def convergence_K(self, new_K):
+        if 'convergence_K' in self.parameters.keys():
+            self.parameters['convergence_K'] = new_K
+            self._update_sources('convergence_K', new_K)
+        else:
+            raise KeyError('convergence_K is not a parameter of this model.')
+
+    @property
+    def shear_G(self):
+        """
+        *complex*
+
+        Shear of external mass sheet.
+        """
+        if 'shear_G' in self.parameters.keys():
+            return self.parameters['shear_G']
+        else:
+            return None
+
+    @shear_G.setter
+    def shear_G(self, new_G):
+        if 'shear_G' in self.parameters.keys():
+            self.parameters['shear_G'] = new_G
+            self._update_sources('shear_G', new_G)
+        else:
+            raise KeyError('shear_G is not a parameter of this model.')
+
+    @property
     def s(self):
         """
         *float*
 
         separation of the two lens components relative to Einstein ring size
         """
         return self.parameters['s']
@@ -1523,14 +1583,24 @@
         *int*
 
         number of luminous sources; it's possible to be 1 for xallarap model
         """
         return self._n_sources
 
     @property
+    def is_external_mass_sheet(self):
+        """
+        *bool*
+
+        Whether an external mass sheet is included in the model
+        """
+        return (('convergence_K' in self.parameters.keys()) or
+                ('shear_G' in self.parameters.keys()))
+
+    @property
     def source_1_parameters(self):
         """
         :py:class:`~MulensModel.modelparameters.ModelParameters`
 
         Parameters of source 1 in multi-source model.
 
         **Do not change returned values.** To change
```

### Comparing `MulensModel-2.7.2/source/MulensModel/mulensdata.py` & `MulensModel-2.8.1/source/MulensModel/mulensdata.py`

 * *Files 0% similar despite different names*

```diff
@@ -217,16 +217,16 @@
         if self._init_keys['add245'] and self._init_keys['add246']:
             raise ValueError(
                 'You cannot initialize MulensData with both ' +
                 'add_2450000 and add_2460000 being True')
 
         if time.dtype != np.float64:
             raise TypeError((
-                    'time vector in MulensData() must be of ' +
-                    'numpy.float64 type, not {:}').format(time.dtype))
+                'time vector in MulensData() must be of ' +
+                'numpy.float64 type, not {:}').format(time.dtype))
 
         # Adjust the time vector as necessary.
         if self._init_keys['add245']:
             time += 2450000.
         elif self._init_keys['add246']:
             time += 2460000.
 
@@ -334,15 +334,15 @@
         """
         if phot_fmt is None:
             phot_fmt = self.input_fmt
         if phot_fmt not in ['mag', 'flux']:
             raise ValueError('wrong value of phot_fmt: {:}'.format(phot_fmt))
         if plot_residuals and model is None:
             raise ValueError(
-                    'MulensData.plot() requires model to plot residuals')
+                'MulensData.plot() requires model to plot residuals')
 
         if model is None:
             (y_value, y_err) = self._get_y_value_y_err(phot_fmt,
                                                        self.flux,
                                                        self.err_flux)
         else:
             raise KeyError(
@@ -660,15 +660,15 @@
             data = self.mag
             err_data = self.err_mag
         elif self.input_fmt == "flux":
             data = self.flux
             err_data = self.err_flux
         else:
             raise ValueError('Unrecognized data format: {:}'.format(
-                    self.input_fmt))
+                self.input_fmt))
 
         return (data, err_data)
 
     def data_and_err_in_chi2_fmt(self):
         """
         Gives photometry in format used for chi2 calculation
         (flux in most cases, but magnitude possible).
@@ -685,15 +685,15 @@
             data = self.mag
             err_data = self.err_mag
         elif self.chi2_fmt == "flux":
             data = self.flux
             err_data = self.err_flux
         else:
             raise ValueError('Unrecognized data format: {:}'.format(
-                    self.chi2_fmt))
+                self.chi2_fmt))
 
         return (data, err_data)
 
     @property
     def bandpass(self):
         """
         *String*
```

### Comparing `MulensModel-2.7.2/source/MulensModel/mulensobjects/lens.py` & `MulensModel-2.8.1/source/MulensModel/mulensobjects/lens.py`

 * *Files 0% similar despite different names*

```diff
@@ -31,14 +31,15 @@
     If units are not specified for a given mass, it is assumed the
     value given is in Solar Masses.
 
     If units are not specified for distance it is assumed the value is
     given in kpc.
 
     """
+
     def __init__(self, total_mass=None, mass=None, mass_1=None, mass_2=None,
                  a_proj=None, distance=None, q=None, s=None, epsilon=None):
         self._caustics = None
 
         # Set up system from s and q if defined
         if q is not None:
             self.q = q
```

### Comparing `MulensModel-2.7.2/source/MulensModel/mulensobjects/mulenssystem.py` & `MulensModel-2.8.1/source/MulensModel/mulensobjects/mulenssystem.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 from MulensModel.model import Model
 
 
 class MulensSystem(object):
     """
     A microlensing system consisting of a lens and a source.
     """
+
     def __init__(self, lens=None, source=None, mu_rel=None):
         self._lens = None
         self._source = None
         if lens is not None:
             if source is None:
                 raise AttributeError(
                     'If lens is specified, source must also be specified.')
@@ -79,15 +80,15 @@
                 "source must be a MulensModel.mulensobjects.source.Source" +
                 "object")
         if (self.lens is not None and self.source.distance is not None and
                 self.lens.distance is not None and
                 self.source.distance.value < self.lens.distance.value):
             msg = 'Source cannot be closer than lens: {:} {:}'
             raise ValueError(msg.format(
-                    self.source.distance, self.lens.distance))
+                self.source.distance, self.lens.distance))
 
     @property
     def mu_rel(self):
         """
         *astropy.Quantity*
 
         Relative proper motion between the source and lens
```

### Comparing `MulensModel-2.7.2/source/MulensModel/mulensobjects/source.py` & `MulensModel-2.8.1/source/MulensModel/mulensobjects/source.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,14 +10,15 @@
     Attributes :
         limb_darkening:
         :py:class:`~MulensModel.limbdarkeningcoeffs.LimbDarkeningCoeffs`
 
             Limb darkening coefficients of the source.
 
     """
+
     def __init__(self, distance=None, pi_S=None, angular_radius=None,
                  limb_darkening=None):
 
         self.distance = distance
         self.pi_S = pi_S
         self.angular_radius = angular_radius
```

### Comparing `MulensModel-2.7.2/source/MulensModel/pointlens.py` & `MulensModel-2.8.1/source/MulensModel/pointlens.py`

 * *Files 2% similar despite different names*

```diff
@@ -73,15 +73,15 @@
         file_ = os.path.join(
             mm.DATA_PATH, 'interpolation_table_b0b1_v1.dat')
         if not os.path.exists(file_):
             raise ValueError('File with FSPL data does not exist.\n' + file_)
         (z, B0, B0_minus_B1) = np.loadtxt(file_, unpack=True)
         PointLens._B0_interpolation = interp1d(z, B0, kind='cubic')
         PointLens._B0_minus_B1_interpolation = interp1d(
-                z, B0_minus_B1, kind='cubic')
+            z, B0_minus_B1, kind='cubic')
         PointLens._z_min = np.min(z)
         PointLens._z_max = np.max(z)
 
         PointLens._B0B1_file_read = True
 
     def _read_elliptic_files(self):
         """
@@ -124,15 +124,15 @@
         Yoo J. et al. 2004 ApJ 603, 139 "OGLE-2003-BLG-262: Finite-Source
         Effects from a Point-Mass Lens"
         https://ui.adsabs.harvard.edu/abs/2004ApJ...603..139Y/abstract
 
         """
 
         out = 4. * z / np.pi
-        function = lambda x: (1.-value**2*sin(x)**2)**.5
+        def function(x): return (1.-value**2*sin(x)**2)**.5
 
         for (i, value) in enumerate(z):
             if value < 1.:
                 out[i] *= ellipe(value*value)
             else:
                 out[i] *= integrate.quad(function, 0., np.arcsin(1./value))[0]
         return out
@@ -151,32 +151,32 @@
         """
         if B_0 is None:
             B_0 = self._B_0_function(z)
 
         def function(r, theta):
             r_2 = r * r
             val = (1. - r_2) / (
-                    r_2 + function.arg_2 + r*function.arg_3*cos(theta))
+                r_2 + function.arg_2 + r*function.arg_3*cos(theta))
             return r * sqrt(val)
 
-        lim_0 = lambda x: 0
-        lim_1 = lambda x: 1
+        def lim_0(x): return 0
+        def lim_1(x): return 1
         rho_W_1 = 0. * z  # This equals rho * W_1().
         for (i, zz) in enumerate(z):
             function.arg_1 = zz
             function.arg_2 = zz * zz
             function.arg_3 = -2. * zz
             rho_W_1[i] = integrate.dblquad(
                 function, 0., 2.*np.pi, lim_0, lim_1)[0]
 
         rho_W_1 /= np.pi
         return B_0 - 1.5 * z * rho_W_1
 
     def get_point_lens_finite_source_magnification(
-                self, u, pspl_magnification, direct=False):
+            self, u, pspl_magnification, direct=False):
         """
         Calculate magnification for point lens and finite source (for
         a *uniform* source).  The approximation was proposed by:
 
         `Gould A. 1994 ApJ 421L, 71 "Proper motions of MACHOs"
         <https://ui.adsabs.harvard.edu/abs/1994ApJ...421L..71G/abstract>`_
 
@@ -206,15 +206,15 @@
                 Type is the same as of u parameter.
 
         """
         return self._get_point_lens_finite_source_magnification(
             u, pspl_magnification, rho=self.parameters.rho, direct=direct)
 
     def _get_point_lens_finite_source_magnification(
-                self, u, pspl_magnification, rho, direct=False):
+            self, u, pspl_magnification, rho, direct=False):
         """
         Calculate large source magnification assuming rho provided directly,
         not as self.parameters.rho
         """
         z = u / rho
         try:
             _ = iter(z)
@@ -238,15 +238,15 @@
             B0[mask] = self._B_0_function(z[mask])
 
         magnification = pspl_magnification * B0
         # More accurate calculations can be performed - see Yoo+04 eq. 11 & 12.
         return magnification
 
     def get_point_lens_limb_darkening_magnification(
-                self, u, pspl_magnification, gamma, direct=False):
+            self, u, pspl_magnification, gamma, direct=False):
         """
         calculate magnification for point lens and finite source *with
         limb darkening*. The approximation was proposed by:
 
         `Gould A. 1994 ApJ 421L, 71 "Proper motions of MACHOs"
         <https://ui.adsabs.harvard.edu/abs/1994ApJ...421L..71G/abstract>`_
```

### Comparing `MulensModel-2.7.2/source/MulensModel/satelliteskycoord.py` & `MulensModel-2.8.1/source/MulensModel/satelliteskycoord.py`

 * *Files identical despite different names*

### Comparing `MulensModel-2.7.2/source/MulensModel/tests/test_BinaryLens.py` & `MulensModel-2.8.1/source/MulensModel/tests/test_BinaryLens.py`

 * *Files 7% similar despite different names*

```diff
@@ -72,10 +72,14 @@
     s = 0.8
     q = 0.1
 
     m_1 = 1. / (1. + q)
     m_2 = q / (1. + q)
     bl = mm.BinaryLens(m_1, m_2, s)
 
+    # Previous version was failing because of bug in AC:
+    # result = bl.adaptive_contouring_magnification(
+    #     0.01, 0.01, 0.01, accuracy=0.019, ld_accuracy=1e-3)
+    # np.testing.assert_almost_equal(result, 18.2834436, decimal=3)
     result = bl.adaptive_contouring_magnification(
-        0.01, 0.01, 0.01, accuracy=0.019, ld_accuracy=1e-3)
-    np.testing.assert_almost_equal(result, 18.2834436, decimal=3)
+        0.06, 0.01, 0.01, accuracy=0.019, ld_accuracy=1e-3)
+    np.testing.assert_almost_equal(result, 11.403036510555962, decimal=3)
```

### Comparing `MulensModel-2.7.2/source/MulensModel/tests/test_Caustic.py` & `MulensModel-2.8.1/source/MulensModel/tests/test_Caustics.py`

 * *Files 22% similar despite different names*

```diff
@@ -8,14 +8,17 @@
 SAMPLE_FILE_01 = os.path.join(
     mm.DATA_PATH, "unit_test_files", "MB11293_caustics.dat")
 
 test_caustics = np.genfromtxt(SAMPLE_FILE_01, names=['X', 'Y'], dtype=None)
 
 
 def test_caustic():
+    """
+    Make sure the caustic is properly calculated.
+    """
     s = 0.548
     q = 0.0053
 
     caustics = mm.Caustics(q=q, s=s)
 
     x, y = caustics.get_caustics(n_points=1000)
     for i in range(0, len(x), 100):
```

### Comparing `MulensModel-2.7.2/source/MulensModel/tests/test_Coords.py` & `MulensModel-2.8.1/source/MulensModel/tests/test_Coords.py`

 * *Files identical despite different names*

### Comparing `MulensModel-2.7.2/source/MulensModel/tests/test_Event.py` & `MulensModel-2.8.1/source/MulensModel/tests/test_Event.py`

 * *Files identical despite different names*

### Comparing `MulensModel-2.7.2/source/MulensModel/tests/test_FitData.py` & `MulensModel-2.8.1/source/MulensModel/tests/test_FitData.py`

 * *Files 0% similar despite different names*

```diff
@@ -357,15 +357,15 @@
     """
 
     # test that chi2 changes when using all data points vs. eliminating the
     # planet.
     (t_planet_start, t_planet_stop) = (2460982., 2460985.)
     data = mm.MulensData(file_name=SAMPLE_FILE_04_WF)
     flag_planet = (data.time > t_planet_start) & (
-                data.time < t_planet_stop) | np.isnan(data.err_mag)
+        data.time < t_planet_stop) | np.isnan(data.err_mag)
     data_bad = mm.MulensData(file_name=SAMPLE_FILE_04_WF, bad=flag_planet)
 
     (t_0, u_0, t_E) = (2460962.36458, 0.411823, 22.8092)
     point_lens_model = mm.Model({'t_0': t_0, 'u_0': u_0, 't_E': t_E})
     fit_all = mm.FitData(dataset=data, model=point_lens_model)
     fit_bad = mm.FitData(dataset=data_bad, model=point_lens_model)
     assert(fit_all.chi2 is None)
```

### Comparing `MulensModel-2.7.2/source/MulensModel/tests/test_Lens.py` & `MulensModel-2.8.1/source/MulensModel/tests/test_Lens.py`

 * *Files identical despite different names*

### Comparing `MulensModel-2.7.2/source/MulensModel/tests/test_MagnificationCurve.py` & `MulensModel-2.8.1/source/MulensModel/tests/test_MagnificationCurve.py`

 * *Files identical despite different names*

### Comparing `MulensModel-2.7.2/source/MulensModel/tests/test_Model.py` & `MulensModel-2.8.1/source/MulensModel/tests/test_Model.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,23 +1,28 @@
 import numpy as np
 from numpy.testing import assert_almost_equal as almost
+from math import isclose
 import unittest
 from astropy import units as u
 
 import MulensModel as mm
 import check_architecture
 
 
 def test_n_lenses():
     """check n_lenses property"""
     model_1 = mm.Model({"t_0": 2456789., "u_0": 1., "t_E": 30.})
     model_2 = mm.Model({"t_0": 2456789., "u_0": 1., "t_E": 30.,
                         "s": 1.1234, "q": 0.123, 'alpha': 12.34})
+    model_3 = mm.Model({"t_0": 2456789., "u_0": 1., "t_E": 30.,
+                        "s": 1.1234, "q": 0.123, 'alpha': 12.34,
+                        'convergence_K': 0.04, 'shear_G': complex(0.1, -0.05)})
     assert model_1.n_lenses == 1
     assert model_2.n_lenses == 2
+    assert model_3.n_lenses == 2
 
 
 # Point Lens Tests
 def test_model_PSPL_1():
     """tests basic evaluation of Paczynski model"""
     t_0 = 5379.57091
     u_0 = 0.52298
@@ -138,36 +143,66 @@
 t_0 = 2456141.593 + delta_t_0
 u_0 = 0.5425 + delta_u_0
 
 
 def test_BLPS_01():
     """simple binary lens with point source"""
     params = mm.ModelParameters({
-            't_0': t_0, 'u_0': u_0, 't_E': t_E, 'alpha': alpha, 's': s,
-            'q': q})
+        't_0': t_0, 'u_0': u_0, 't_E': t_E, 'alpha': alpha, 's': s,
+        'q': q})
 
     model = mm.Model(parameters=params)
     t = np.array([2456112.5])
     data = mm.MulensData(data_list=[t, t*0.+16., t*0.+0.01])
     magnification = model.get_magnification(data.time[0])
     almost(magnification, 4.691830781584699)
 # This value comes from early version of this code.
 # almost(m, 4.710563917)
 # This value comes from Andy's getbinp().
 
 
+def test_BLPS_shear_active():
+    """
+    simple binary lens with point source and external convergence and shear
+    """
+    params = mm.ModelParameters({
+        't_0': t_0, 'u_0': u_0, 't_E': t_E, 'alpha': alpha, 's': s,
+        'q': q, 'convergence_K': 0.08, 'shear_G': complex(0.1, -0.1)})
+
+    model = mm.Model(parameters=params)
+    t = np.array([2456112.5])
+    data = mm.MulensData(data_list=[t, t*0.+16., t*0.+0.01])
+    magnification = model.get_magnification(data.time[0])
+    assert not isclose(magnification, 4.691830781584699, abs_tol=1e-2)
+
+
+def test_BLPS_shear():
+    """
+    simple binary lens with point source and external convergence and shear
+    """
+    params = mm.ModelParameters({
+        't_0': t_0, 'u_0': u_0, 't_E': t_E, 'alpha': alpha, 's': s,
+        'q': q, 'convergence_K': 0.0, 'shear_G': complex(0, 0)})
+
+    model = mm.Model(parameters=params)
+    t = np.array([2456112.5])
+    data = mm.MulensData(data_list=[t, t*0.+16., t*0.+0.01])
+    magnification = model.get_magnification(data.time[0])
+    almost(magnification, 4.691830781584699)
+
+
 def test_BLPS_02():
     """
     simple binary lens with extended source and different methods to
     evaluate magnification
     """
 
     params = mm.ModelParameters({
-            't_0': t_0, 'u_0': u_0, 't_E': t_E, 'alpha': alpha, 's': s,
-            'q': q, 'rho': rho})
+        't_0': t_0, 'u_0': u_0, 't_E': t_E, 'alpha': alpha, 's': s,
+        'q': q, 'rho': rho})
     model = mm.Model(parameters=params)
 
     t = np.array([6112.5, 6113., 6114., 6115., 6116., 6117., 6118., 6119])
     t += 2450000.
     methods = [2456113.5, 'Quadrupole', 2456114.5, 'Hexadecapole', 2456116.5,
                'VBBL', 2456117.5]
     model.set_magnification_methods(methods)
@@ -195,16 +230,16 @@
     """
     simple binary lens with extended source and different methods to evaluate
     magnification - version with adaptivecontouring
     """
     check_architecture.skip_m1(msg='Adaptive Contouring')
 
     params = mm.ModelParameters({
-            't_0': t_0, 'u_0': u_0, 't_E': t_E, 'alpha': alpha, 's': s,
-            'q': q, 'rho': rho})
+        't_0': t_0, 'u_0': u_0, 't_E': t_E, 'alpha': alpha, 's': s,
+        'q': q, 'rho': rho})
     model = mm.Model(parameters=params)
 
     t = np.array([6112.5, 6113., 6114., 6115., 6116., 6117., 6118., 6119])
     t += 2450000.
     ac_name = 'Adaptive_Contouring'
     methods = [2456113.5, 'Quadrupole', 2456114.5, 'Hexadecapole', 2456116.5,
                ac_name, 2456117.5]
@@ -232,16 +267,16 @@
 
 
 def test_methods_parameters():
     """
     make sure additional parameters are properly passed to very inner functions
     """
     params = mm.ModelParameters({
-            't_0': t_0, 'u_0': u_0, 't_E': t_E, 'alpha': alpha, 's': s,
-            'q': q, 'rho': rho})
+        't_0': t_0, 'u_0': u_0, 't_E': t_E, 'alpha': alpha, 's': s,
+        'q': q, 'rho': rho})
     model = mm.Model(parameters=params)
 
     t = np.array([2456117.])
     methods = [2456113.5, 'Quadrupole', 2456114.5, 'Hexadecapole', 2456116.5,
                'VBBL', 2456117.5]
     model.set_magnification_methods(methods)
```

### Comparing `MulensModel-2.7.2/source/MulensModel/tests/test_ModelParameters.py` & `MulensModel-2.8.1/source/MulensModel/tests/test_ModelParameters.py`

 * *Files 2% similar despite different names*

```diff
@@ -231,7 +231,21 @@
                               's': 10, 'q': 0.5, 'alpha': 100.})
     p_3 = mm.ModelParameters({'x_caustic_in': 0.1, 'x_caustic_out': 0.15,
                               't_caustic_in': 1000, 't_caustic_out': 2000.,
                               's': 1, 'q': 0.8})
     assert p_1.n_lenses == 1
     assert p_2.n_lenses == 2
     assert p_3.n_lenses == 2
+
+
+def test_is_finite_source():
+    """
+    Test if .is_finite_source() works properly for 1L1S
+    """
+    common = {'t_0': 1.23, 'u_0': 0.123, 't_E': 23.456}
+    params_1 = mm.ModelParameters(common)
+    params_2 = mm.ModelParameters({'rho': 0.001, **common})
+    params_3 = mm.ModelParameters({'t_star': 0.012, **common})
+
+    assert not params_1.is_finite_source()
+    assert params_2.is_finite_source()
+    assert params_3.is_finite_source()
```

### Comparing `MulensModel-2.7.2/source/MulensModel/tests/test_Model_Parallax.py` & `MulensModel-2.8.1/source/MulensModel/tests/test_Model_Parallax.py`

 * *Files 0% similar despite different names*

```diff
@@ -26,22 +26,23 @@
 
 
 class _ParallaxFile(object):
     """
     Private class to allow easy access to the contents of the parallax
     test files.
     """
+
     def __init__(self, filename):
         """
         Open the file and store parameters.
         """
         self.filename = filename
         self.data = np.genfromtxt(
-                self.filename, dtype=None,
-                names=['Time', 'Magnification', 'PLflux', 'u', 'qn', 'qe'])
+            self.filename, dtype=None,
+            names=['Time', 'Magnification', 'PLflux', 'u', 'qn', 'qe'])
 
         (self.ulens_params, self.event_params) = self.get_file_params()
 
     def get_file_params(self):
         """Read in the model parameters used to create the file"""
         with open(self.filename) as data_file:
             lines = data_file.readlines()
```

### Comparing `MulensModel-2.7.2/source/MulensModel/tests/test_MulensData.py` & `MulensModel-2.8.1/source/MulensModel/tests/test_MulensData.py`

 * *Files identical despite different names*

### Comparing `MulensModel-2.7.2/source/MulensModel/tests/test_MulensSystem.py` & `MulensModel-2.8.1/source/MulensModel/tests/test_MulensSystem.py`

 * *Files identical despite different names*

### Comparing `MulensModel-2.7.2/source/MulensModel/tests/test_PointLens.py` & `MulensModel-2.8.1/source/MulensModel/tests/test_PointLens.py`

 * *Files identical despite different names*

### Comparing `MulensModel-2.7.2/source/MulensModel/tests/test_Trajectory.py` & `MulensModel-2.8.1/source/MulensModel/tests/test_Trajectory.py`

 * *Files identical despite different names*

### Comparing `MulensModel-2.7.2/source/MulensModel/tests/test_UniformCausticSampling.py` & `MulensModel-2.8.1/source/MulensModel/tests/test_UniformCausticSampling.py`

 * *Files identical despite different names*

### Comparing `MulensModel-2.7.2/source/MulensModel/tests/test_Utils.py` & `MulensModel-2.8.1/source/MulensModel/tests/test_Utils.py`

 * *Files identical despite different names*

### Comparing `MulensModel-2.7.2/source/MulensModel/trajectory.py` & `MulensModel-2.8.1/source/MulensModel/trajectory.py`

 * *Files 1% similar despite different names*

```diff
@@ -74,23 +74,16 @@
     _get_delta_annual_results = dict()
     _get_delta_annual_last = None
     _get_delta_annual_last_index = None
     _get_delta_satellite_results = dict()
 
     def __init__(self, times, parameters, parallax=None,
                  coords=None, satellite_skycoord=None, earth_coords=None):
-        # Set times
-        if isinstance(times, np.ndarray):
-            self.times = times
-        elif isinstance(times, (list, tuple)):
-            self.times = np.array(times)
-        else:
-            self.times = np.array([times])
+        self.times = np.atleast_1d(times)
 
-        # Check for ModelParameters and set.
         if isinstance(parameters, ModelParameters):
             self.parameters = parameters
         else:
             m = 'parameters is a required and must be a ModelParameters object'
             raise TypeError(m)
 
         # Set parallax values
```

### Comparing `MulensModel-2.7.2/source/MulensModel/uniformcausticsampling.py` & `MulensModel-2.8.1/source/MulensModel/uniformcausticsampling.py`

 * *Files 0% similar despite different names*

```diff
@@ -88,14 +88,15 @@
     "A systematic fitting scheme for caustic-crossing microlensing events"
     <https://ui.adsabs.harvard.edu/abs/2009MNRAS.395..787K/abstract>`_
 
     `Kains N. et al. 2012 MNRAS 426, 2228 "A Bayesian algorithm for model
     selection applied to caustic-crossing binary-lens microlensing events"
     <https://ui.adsabs.harvard.edu/abs/2012MNRAS.426.2228K/abstract>`_
     """
+
     def __init__(self, s, q, n_points=10000):
         self._s = s
         self._q = q
         self._n_points = n_points
 
         self._n_caustics = Utils.get_n_caustics(s=self.s, q=self.q)
         self._get_phi()
```

### Comparing `MulensModel-2.7.2/source/MulensModel/utils.py` & `MulensModel-2.8.1/source/MulensModel/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -30,15 +30,15 @@
     'Jun': '06',
     'Jul': '07',
     'Aug': '08',
     'Sep': '09',
     'Oct': '10',
     'Nov': '11',
     'Dec': '12'
-    }
+}
 
 
 class Utils(object):
     """ A number of small functions used in different places """
 
     def get_flux_from_mag(mag, zeropoint=None):
         """
```

### Comparing `MulensModel-2.7.2/source/MulensModel.egg-info/SOURCES.txt` & `MulensModel-2.8.1/source/MulensModel.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -14,15 +14,18 @@
 source/AdaptiveContouring/complex.c
 source/AdaptiveContouring/complex.h
 source/AdaptiveContouring/dyn_array.c
 source/AdaptiveContouring/erdlcaust.c
 source/AdaptiveContouring/integrate.c
 source/MulensModel/__init__.py
 source/MulensModel/binarylens.py
+source/MulensModel/binarylensimports.py
+source/MulensModel/binarylenswithshear.py
 source/MulensModel/caustics.py
+source/MulensModel/causticswithshear.py
 source/MulensModel/coordinates.py
 source/MulensModel/event.py
 source/MulensModel/fitdata.py
 source/MulensModel/horizons.py
 source/MulensModel/limbdarkeningcoeffs.py
 source/MulensModel/magnificationcurve.py
 source/MulensModel/model.py
@@ -100,28 +103,31 @@
 source/MulensModel/data/unit_test_files/parallax_test_5.dat
 source/MulensModel/mulensobjects/__init__.py
 source/MulensModel/mulensobjects/lens.py
 source/MulensModel/mulensobjects/mulenssystem.py
 source/MulensModel/mulensobjects/source.py
 source/MulensModel/tests/check_architecture.py
 source/MulensModel/tests/test_BinaryLens.py
-source/MulensModel/tests/test_Caustic.py
+source/MulensModel/tests/test_BinaryLensWithShear.py
+source/MulensModel/tests/test_Caustics.py
+source/MulensModel/tests/test_CausticsWithShear.py
 source/MulensModel/tests/test_Coords.py
 source/MulensModel/tests/test_Event.py
 source/MulensModel/tests/test_FitData.py
 source/MulensModel/tests/test_Lens.py
 source/MulensModel/tests/test_MagnificationCurve.py
 source/MulensModel/tests/test_Model.py
 source/MulensModel/tests/test_ModelParameters.py
 source/MulensModel/tests/test_Model_Parallax.py
 source/MulensModel/tests/test_MulensData.py
 source/MulensModel/tests/test_MulensSystem.py
 source/MulensModel/tests/test_PointLens.py
 source/MulensModel/tests/test_Trajectory.py
 source/MulensModel/tests/test_UniformCausticSampling.py
 source/MulensModel/tests/test_Utils.py
+source/VBBL/LICENSE.txt
 source/VBBL/Makefile
 source/VBBL/README.md
 source/VBBL/VBBinaryLensingLibrary.cpp
 source/VBBL/VBBinaryLensingLibrary.h
 source/VBBL/VBBinaryLensingLibrary_wrapper.cpp
 source/VBBL/vbbl_wrapper.cpp
```

### Comparing `MulensModel-2.7.2/source/VBBL/Makefile` & `MulensModel-2.8.1/source/VBBL/Makefile`

 * *Files identical despite different names*

### Comparing `MulensModel-2.7.2/source/VBBL/README.md` & `MulensModel-2.8.1/source/VBBL/README.md`

 * *Files identical despite different names*

### Comparing `MulensModel-2.7.2/source/VBBL/VBBinaryLensingLibrary.h` & `MulensModel-2.8.1/source/VBBL/VBBinaryLensingLibrary.h`

 * *Files 2% similar despite different names*

```diff
@@ -19,14 +19,15 @@
 #ifndef __binlens
 #define __binlens
 #define __unmanaged
 
 #define _L1 x1-((x1+a/2.0)/((x1+a/2.0)*(x1+a/2.0)+x2*x2)+q*(x1-a/2.0)/((x1-a/2.0)*(x1-a/2.0)+x2*x2))/(1.0+q) // Used in PlotCrits
 #define _L2 x2-(x2/((x1+a/2.0)*(x1+a/2.0)+x2*x2)+q*x2/((x1-a/2.0)*(x1-a/2.0)+x2*x2))/(1.0+q)
 #define _LL (y-z)+coefs[21]/(zc-coefs[20])+coefs[22]/zc //Lens equation test
+#define _LL_shear (y-(1.0-coefs[26])*z)+coefs[27]*zc+coefs[21]/(zc-coefs[20])+coefs[22]/zc //Lens equation test
 #define _J1c coefs[21]/((zc-coefs[20])*(zc-coefs[20]))+coefs[22]/(zc*zc) //#define _J1 m1/((zc-0.5*a)*(zc-0.5*a))+m2/((zc+0.5*a)*(zc+0.5*a))
 #define _J2 -2.0*(coefs[21]/((z-coefs[20])*(z-coefs[20])*(z-coefs[20]))+coefs[22]/(z*z*z))
 #define _J3 6.0*(coefs[21]/((z-coefs[20])*(z-coefs[20])*(z-coefs[20])*(z-coefs[20]))+coefs[22]/(z*z*z*z))
 #define _skew(p1,p2,q1,q2) p1*q2-p2*q1
 #define _NP 200.0
 
 #define _sign(x) ((x>0)? +1 : -1)
@@ -57,14 +58,15 @@
 		double Eq2000[3],Quad2000[3],North2000[3]; 
 		double ESPLout[101][101], ESPLin[101][101];
 		bool ESPLoff, multidark;
 		annulus *annlist;
 
 		void ComputeParallax(double, double, double *);
 		_curve *NewImages(complex,complex  *,_theta *);
+		_curve *NewImages_shear(complex,complex  *,_theta *);
 		void OrderImages(_sols *,_curve *);
 		//void cmplx_roots_gen(complex *, complex *, int, bool, bool);
 		void cmplx_laguerre(complex *, int, complex *, int &, bool &);
 		void cmplx_newton_spec(complex *, int, complex *, int &, bool &);
 		void cmplx_laguerre2newton(complex *, int, complex *, int &, bool &, int);
 		void solve_quadratic_eq(complex &, complex &, complex *);
 		void solve_cubic_eq(complex &, complex &, complex &, complex *);
@@ -78,14 +80,16 @@
 
 		_sols *PlotCrit(double a,double q);
 		void PrintCau(double a,double q);
 		void SetObjectCoordinates(char *Coordinates_file, char *Directory_for_satellite_tables);
 
 	// Magnification calculation functions.
 
+		double BinaryMag0_shear(double s,double q,double y1,double y2, double K1, double G1, double Gi, _sols **Images);
+		double BinaryMag0_shear(double s, double q, double y1, double y2, double K1, double G1, double Gi);
 		double BinaryMag0(double s,double q,double y1,double y2, _sols **Images);
 		double BinaryMag0(double s, double q, double y1, double y2);
 		double BinaryMag(double s,double q,double y1,double y2,double rho,double accuracy, _sols **Images);
 		double BinaryMag(double s,double q ,double y1,double y2,double rho,double accuracy);
 		double BinaryMag2(double s, double q, double y1, double y2, double rho);
 		double BinaryMagDark(double s, double q, double y1, double y2, double rho, double a1,double accuracy);
 		void BinaryMagMultiDark(double s, double q, double y1, double y2, double rho, double *a1_list, int n_filters, double *mag_list, double accuracy);
```

### Comparing `MulensModel-2.7.2/source/VBBL/VBBinaryLensingLibrary_wrapper.cpp` & `MulensModel-2.8.1/source/VBBL/VBBinaryLensingLibrary_wrapper.cpp`

 * *Files 26% similar despite different names*

```diff
@@ -6,14 +6,22 @@
   double VBBinaryLensing_BinaryMagDark(double a, double q, double y1, double y2, double RSv, double a1, double Tol) {
     static VBBinaryLensing VBBL;
     
     return VBBL.BinaryMagDark(a, q, y1, y2, RSv, a1, Tol);
   }
 }
 
+extern "C" {
+  double VBBinaryLensing_BinaryMag0(double a,double q,double y1,double y2, double K, double G, double Gi) {
+    static VBBinaryLensing VBBL;
+    
+    return VBBL.BinaryMag0_shear(a, q, y1, y2, K, G, Gi);
+  }
+}
+
 extern "C" double* VBBL_SG12_5(double p0, double p1, 
                     double p2, double p3, double p4, double p5, double p6, 
                     double p7, double p8, double p9, double p10, double p11) {
     static VBBinaryLensing VBBL;
     complex complex_poly[6], complex_roots[5];
     static double roots[10];
     int i;
@@ -40,7 +48,37 @@
     static VBBinaryLensing VBBL;
 
     return VBBL.BinaryMag0(a, q, y1, y2);
   }
 }
 
 
+extern "C" double* VBBL_SG12_9(double p0, double p1, 
+                    double p2, double p3, double p4, double p5, double p6, 
+                    double p7, double p8, double p9, double p10, double p11,
+                    double p12, double p13, double p14, double p15,
+                    double p16, double p17, double p18, double p19) {
+    static VBBinaryLensing VBBL;
+    complex complex_poly[10], complex_roots[9];
+    static double roots[18];
+    int i;
+
+    complex_poly[0] = complex(p0, p10);
+    complex_poly[1] = complex(p1, p11);
+    complex_poly[2] = complex(p2, p12);
+    complex_poly[3] = complex(p3, p13);
+    complex_poly[4] = complex(p4, p14);
+    complex_poly[5] = complex(p5, p15);
+    complex_poly[6] = complex(p6, p16);
+    complex_poly[7] = complex(p7, p17);
+    complex_poly[8] = complex(p8, p18);
+    complex_poly[9] = complex(p9, p19);
+
+    VBBL.cmplx_roots_gen(complex_roots, complex_poly, 9, true, true);
+    
+    for (i=0; i<9; i++) {
+        roots[i] = complex_roots[i].re;
+        roots[i+9] = complex_roots[i].im;
+    }
+
+    return roots;
+}
```

