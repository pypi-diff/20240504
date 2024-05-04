# Comparing `tmp/SAMBA_ilum-1.0.0.7.tar.gz` & `tmp/SAMBA_ilum-1.0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "SAMBA_ilum-1.0.0.7.tar", last modified: Fri Apr 26 20:49:52 2024, max compression
+gzip compressed data, was "SAMBA_ilum-1.0.0.8.tar", last modified: Fri May  3 16:13:59 2024, max compression
```

## Comparing `SAMBA_ilum-1.0.0.7.tar` & `SAMBA_ilum-1.0.0.8.tar`

### file list

```diff
@@ -1,57 +1,57 @@
-drwxrwxrwx   0        0        0        0 2024-04-26 20:49:52.206739 SAMBA_ilum-1.0.0.7/
--rw-rw-rw-   0        0        0       13 2024-04-24 12:22:55.000000 SAMBA_ilum-1.0.0.7/LICENSE.txt
--rw-rw-rw-   0        0        0      297 2024-04-26 20:49:52.206739 SAMBA_ilum-1.0.0.7/PKG-INFO
--rw-rw-rw-   0        0        0       56 2024-04-24 12:23:43.000000 SAMBA_ilum-1.0.0.7/README.md
-drwxrwxrwx   0        0        0        0 2024-04-26 20:49:52.113001 SAMBA_ilum-1.0.0.7/SAMBA_ilum.egg-info/
--rw-rw-rw-   0        0        0      297 2024-04-26 20:49:51.000000 SAMBA_ilum-1.0.0.7/SAMBA_ilum.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1711 2024-04-26 20:49:51.000000 SAMBA_ilum-1.0.0.7/SAMBA_ilum.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-26 20:49:51.000000 SAMBA_ilum-1.0.0.7/SAMBA_ilum.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       47 2024-04-26 20:49:51.000000 SAMBA_ilum-1.0.0.7/SAMBA_ilum.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       34 2024-04-26 20:49:51.000000 SAMBA_ilum-1.0.0.7/SAMBA_ilum.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2024-04-26 20:49:51.000000 SAMBA_ilum-1.0.0.7/SAMBA_ilum.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-04-26 20:49:52.113001 SAMBA_ilum-1.0.0.7/samba_ilum/
--rw-rw-rw-   0        0        0       57 2024-04-24 12:22:49.000000 SAMBA_ilum-1.0.0.7/samba_ilum/__init__.py
--rw-rw-rw-   0        0        0     8209 2024-04-26 20:49:34.000000 SAMBA_ilum-1.0.0.7/samba_ilum/__main__.py
-drwxrwxrwx   0        0        0        0 2024-04-26 20:49:52.175495 SAMBA_ilum-1.0.0.7/samba_ilum/src/
--rw-rw-rw-   0        0        0    67526 2024-04-24 12:21:15.000000 SAMBA_ilum-1.0.0.7/samba_ilum/src/HeteroStructure_Generator.py
-drwxrwxrwx   0        0        0        0 2024-04-26 20:49:52.191113 SAMBA_ilum-1.0.0.7/samba_ilum/src/INPUTS/
--rw-rw-rw-   0        0        0      267 2024-04-17 14:51:50.000000 SAMBA_ilum-1.0.0.7/samba_ilum/src/INPUTS/INCAR_bader
--rw-rw-rw-   0        0        0      308 2024-04-17 14:52:00.000000 SAMBA_ilum-1.0.0.7/samba_ilum/src/INPUTS/INCAR_bader.SO
--rw-rw-rw-   0        0        0      262 2024-04-17 14:52:22.000000 SAMBA_ilum-1.0.0.7/samba_ilum/src/INPUTS/INCAR_bands
--rw-rw-rw-   0        0        0      303 2024-04-17 14:52:42.000000 SAMBA_ilum-1.0.0.7/samba_ilum/src/INPUTS/INCAR_bands.SO
--rw-rw-rw-   0        0        0      251 2024-04-17 15:10:48.000000 SAMBA_ilum-1.0.0.7/samba_ilum/src/INPUTS/INCAR_dos
--rw-rw-rw-   0        0        0      292 2024-04-17 14:53:00.000000 SAMBA_ilum-1.0.0.7/samba_ilum/src/INPUTS/INCAR_dos.SO
--rw-rw-rw-   0        0        0      240 2024-04-17 14:53:10.000000 SAMBA_ilum-1.0.0.7/samba_ilum/src/INPUTS/INCAR_relax
--rw-rw-rw-   0        0        0      253 2024-04-17 14:53:18.000000 SAMBA_ilum-1.0.0.7/samba_ilum/src/INPUTS/INCAR_scf
--rw-rw-rw-   0        0        0      294 2024-04-17 14:53:24.000000 SAMBA_ilum-1.0.0.7/samba_ilum/src/INPUTS/INCAR_scf.SO
--rw-rw-rw-   0        0        0      238 2024-04-19 19:19:42.000000 SAMBA_ilum-1.0.0.7/samba_ilum/src/INPUTS/INCAR_xy-scan
--rw-rw-rw-   0        0        0      238 2024-04-19 19:19:50.000000 SAMBA_ilum-1.0.0.7/samba_ilum/src/INPUTS/INCAR_z-scan
-drwxrwxrwx   0        0        0        0 2024-04-26 20:49:52.206739 SAMBA_ilum-1.0.0.7/samba_ilum/src/INPUTS/inputs_VASProcar/
--rw-rw-rw-   0        0        0     4485 2024-03-20 16:04:46.000000 SAMBA_ilum-1.0.0.7/samba_ilum/src/INPUTS/inputs_VASProcar/input.vasprocar.bands
--rw-rw-rw-   0        0        0     3123 2024-04-08 15:25:48.000000 SAMBA_ilum-1.0.0.7/samba_ilum/src/INPUTS/inputs_VASProcar/input.vasprocar.chgcar
--rw-rw-rw-   0        0        0     2525 2024-03-20 16:04:58.000000 SAMBA_ilum-1.0.0.7/samba_ilum/src/INPUTS/inputs_VASProcar/input.vasprocar.dos
--rw-rw-rw-   0        0        0     9603 2024-03-21 16:46:56.000000 SAMBA_ilum-1.0.0.7/samba_ilum/src/INPUTS/inputs_VASProcar/input.vasprocar.location
--rw-rw-rw-   0        0        0     1187 2024-03-23 20:35:58.000000 SAMBA_ilum-1.0.0.7/samba_ilum/src/INPUTS/inputs_VASProcar/input.vasprocar.locpot
--rw-rw-rw-   0        0        0     6378 2024-03-20 16:05:20.000000 SAMBA_ilum-1.0.0.7/samba_ilum/src/INPUTS/inputs_VASProcar/input.vasprocar.orbitals
--rw-rw-rw-   0        0        0     7790 2024-03-20 16:06:00.000000 SAMBA_ilum-1.0.0.7/samba_ilum/src/INPUTS/inputs_VASProcar/input.vasprocar.spin
--rw-rw-rw-   0        0        0     3968 2024-04-10 01:37:38.000000 SAMBA_ilum-1.0.0.7/samba_ilum/src/SAMBA_HeteroStructure.input
--rw-rw-rw-   0        0        0     3048 2024-04-26 12:23:25.000000 SAMBA_ilum-1.0.0.7/samba_ilum/src/SAMBA_WorkFlow.input
--rw-rw-rw-   0        0        0     1094 2024-04-24 12:22:37.000000 SAMBA_ilum-1.0.0.7/samba_ilum/src/_info_pseudo.py
--rw-rw-rw-   0        0        0  4715152 2023-08-19 14:41:30.000000 SAMBA_ilum-1.0.0.7/samba_ilum/src/bader
--rw-rw-rw-   0        0        0     4527 2024-04-24 12:20:31.000000 SAMBA_ilum-1.0.0.7/samba_ilum/src/bader_poscar.py
--rw-rw-rw-   0        0        0     2527 2024-04-24 12:20:40.000000 SAMBA_ilum-1.0.0.7/samba_ilum/src/bader_update.py
--rw-rw-rw-   0        0        0     7060 2024-04-24 12:20:49.000000 SAMBA_ilum-1.0.0.7/samba_ilum/src/charge_transfer.py
--rw-rw-rw-   0        0        0     2139 2019-12-02 15:59:08.000000 SAMBA_ilum-1.0.0.7/samba_ilum/src/chgsum.pl
--rw-rw-rw-   0        0        0      330 2024-04-24 12:20:58.000000 SAMBA_ilum-1.0.0.7/samba_ilum/src/contcar_update.py
--rw-rw-rw-   0        0        0      600 2024-04-24 12:21:06.000000 SAMBA_ilum-1.0.0.7/samba_ilum/src/energy_scan.py
--rw-rw-rw-   0        0        0    13083 2024-04-24 12:21:25.000000 SAMBA_ilum-1.0.0.7/samba_ilum/src/job.py
--rw-rw-rw-   0        0        0     7163 2024-04-26 12:22:49.000000 SAMBA_ilum-1.0.0.7/samba_ilum/src/kpoints.py
--rw-rw-rw-   0        0        0    21404 2024-04-24 12:21:42.000000 SAMBA_ilum-1.0.0.7/samba_ilum/src/make_files.py
--rw-rw-rw-   0        0        0     5959 2024-04-24 12:21:48.000000 SAMBA_ilum-1.0.0.7/samba_ilum/src/output.py
--rw-rw-rw-   0        0        0     1053 2024-04-24 12:21:58.000000 SAMBA_ilum-1.0.0.7/samba_ilum/src/potcar.py
--rw-rw-rw-   0        0        0     7975 2024-04-24 12:22:07.000000 SAMBA_ilum-1.0.0.7/samba_ilum/src/xy-scan.py
--rw-rw-rw-   0        0        0    15612 2024-04-24 12:22:13.000000 SAMBA_ilum-1.0.0.7/samba_ilum/src/xy-scan_analysis.py
--rw-rw-rw-   0        0        0     9644 2024-04-24 12:22:20.000000 SAMBA_ilum-1.0.0.7/samba_ilum/src/z-scan.py
--rw-rw-rw-   0        0        0     4348 2024-04-24 12:22:26.000000 SAMBA_ilum-1.0.0.7/samba_ilum/src/z-scan_analysis.py
--rw-rw-rw-   0        0        0      167 2024-04-26 20:49:52.222364 SAMBA_ilum-1.0.0.7/setup.cfg
--rw-rw-rw-   0        0        0      733 2024-04-26 20:49:17.000000 SAMBA_ilum-1.0.0.7/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-03 16:13:59.520748 SAMBA_ilum-1.0.0.8/
+-rw-rw-rw-   0        0        0       13 2024-04-24 12:22:54.000000 SAMBA_ilum-1.0.0.8/LICENSE.txt
+-rw-rw-rw-   0        0        0      297 2024-05-03 16:13:59.520748 SAMBA_ilum-1.0.0.8/PKG-INFO
+-rw-rw-rw-   0        0        0       56 2024-04-24 12:23:42.000000 SAMBA_ilum-1.0.0.8/README.md
+drwxrwxrwx   0        0        0        0 2024-05-03 16:13:59.130198 SAMBA_ilum-1.0.0.8/SAMBA_ilum.egg-info/
+-rw-rw-rw-   0        0        0      297 2024-05-03 16:13:58.000000 SAMBA_ilum-1.0.0.8/SAMBA_ilum.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1711 2024-05-03 16:13:58.000000 SAMBA_ilum-1.0.0.8/SAMBA_ilum.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-03 16:13:58.000000 SAMBA_ilum-1.0.0.8/SAMBA_ilum.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       47 2024-05-03 16:13:58.000000 SAMBA_ilum-1.0.0.8/SAMBA_ilum.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       34 2024-05-03 16:13:58.000000 SAMBA_ilum-1.0.0.8/SAMBA_ilum.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2024-05-03 16:13:58.000000 SAMBA_ilum-1.0.0.8/SAMBA_ilum.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-03 16:13:59.130198 SAMBA_ilum-1.0.0.8/samba_ilum/
+-rw-rw-rw-   0        0        0       57 2024-04-24 12:22:48.000000 SAMBA_ilum-1.0.0.8/samba_ilum/__init__.py
+-rw-rw-rw-   0        0        0     8214 2024-05-03 16:13:44.000000 SAMBA_ilum-1.0.0.8/samba_ilum/__main__.py
+drwxrwxrwx   0        0        0        0 2024-05-03 16:13:59.364494 SAMBA_ilum-1.0.0.8/samba_ilum/src/
+-rw-rw-rw-   0        0        0    67526 2024-04-24 12:21:14.000000 SAMBA_ilum-1.0.0.8/samba_ilum/src/HeteroStructure_Generator.py
+drwxrwxrwx   0        0        0        0 2024-05-03 16:13:59.458246 SAMBA_ilum-1.0.0.8/samba_ilum/src/INPUTS/
+-rw-rw-rw-   0        0        0      267 2024-04-17 14:51:50.000000 SAMBA_ilum-1.0.0.8/samba_ilum/src/INPUTS/INCAR_bader
+-rw-rw-rw-   0        0        0      308 2024-04-17 14:52:00.000000 SAMBA_ilum-1.0.0.8/samba_ilum/src/INPUTS/INCAR_bader.SO
+-rw-rw-rw-   0        0        0      262 2024-04-17 14:52:22.000000 SAMBA_ilum-1.0.0.8/samba_ilum/src/INPUTS/INCAR_bands
+-rw-rw-rw-   0        0        0      303 2024-04-17 14:52:42.000000 SAMBA_ilum-1.0.0.8/samba_ilum/src/INPUTS/INCAR_bands.SO
+-rw-rw-rw-   0        0        0      251 2024-04-17 15:10:48.000000 SAMBA_ilum-1.0.0.8/samba_ilum/src/INPUTS/INCAR_dos
+-rw-rw-rw-   0        0        0      292 2024-04-17 14:53:00.000000 SAMBA_ilum-1.0.0.8/samba_ilum/src/INPUTS/INCAR_dos.SO
+-rw-rw-rw-   0        0        0      240 2024-04-17 14:53:10.000000 SAMBA_ilum-1.0.0.8/samba_ilum/src/INPUTS/INCAR_relax
+-rw-rw-rw-   0        0        0      253 2024-04-17 14:53:18.000000 SAMBA_ilum-1.0.0.8/samba_ilum/src/INPUTS/INCAR_scf
+-rw-rw-rw-   0        0        0      294 2024-04-17 14:53:24.000000 SAMBA_ilum-1.0.0.8/samba_ilum/src/INPUTS/INCAR_scf.SO
+-rw-rw-rw-   0        0        0      238 2024-04-19 19:19:42.000000 SAMBA_ilum-1.0.0.8/samba_ilum/src/INPUTS/INCAR_xy-scan
+-rw-rw-rw-   0        0        0      238 2024-04-19 19:19:50.000000 SAMBA_ilum-1.0.0.8/samba_ilum/src/INPUTS/INCAR_z-scan
+drwxrwxrwx   0        0        0        0 2024-05-03 16:13:59.520748 SAMBA_ilum-1.0.0.8/samba_ilum/src/INPUTS/inputs_VASProcar/
+-rw-rw-rw-   0        0        0     4485 2024-03-20 16:04:46.000000 SAMBA_ilum-1.0.0.8/samba_ilum/src/INPUTS/inputs_VASProcar/input.vasprocar.bands
+-rw-rw-rw-   0        0        0     3123 2024-04-08 15:25:48.000000 SAMBA_ilum-1.0.0.8/samba_ilum/src/INPUTS/inputs_VASProcar/input.vasprocar.chgcar
+-rw-rw-rw-   0        0        0     2525 2024-03-20 16:04:58.000000 SAMBA_ilum-1.0.0.8/samba_ilum/src/INPUTS/inputs_VASProcar/input.vasprocar.dos
+-rw-rw-rw-   0        0        0     9603 2024-03-21 16:46:56.000000 SAMBA_ilum-1.0.0.8/samba_ilum/src/INPUTS/inputs_VASProcar/input.vasprocar.location
+-rw-rw-rw-   0        0        0     1187 2024-03-23 20:35:58.000000 SAMBA_ilum-1.0.0.8/samba_ilum/src/INPUTS/inputs_VASProcar/input.vasprocar.locpot
+-rw-rw-rw-   0        0        0     6378 2024-03-20 16:05:20.000000 SAMBA_ilum-1.0.0.8/samba_ilum/src/INPUTS/inputs_VASProcar/input.vasprocar.orbitals
+-rw-rw-rw-   0        0        0     7790 2024-03-20 16:06:00.000000 SAMBA_ilum-1.0.0.8/samba_ilum/src/INPUTS/inputs_VASProcar/input.vasprocar.spin
+-rw-rw-rw-   0        0        0     3968 2024-04-10 01:37:38.000000 SAMBA_ilum-1.0.0.8/samba_ilum/src/SAMBA_HeteroStructure.input
+-rw-rw-rw-   0        0        0     3048 2024-04-26 12:23:24.000000 SAMBA_ilum-1.0.0.8/samba_ilum/src/SAMBA_WorkFlow.input
+-rw-rw-rw-   0        0        0     1094 2024-04-24 12:22:36.000000 SAMBA_ilum-1.0.0.8/samba_ilum/src/_info_pseudo.py
+-rw-rw-rw-   0        0        0  4715152 2023-08-19 14:41:30.000000 SAMBA_ilum-1.0.0.8/samba_ilum/src/bader
+-rw-rw-rw-   0        0        0     4527 2024-04-24 12:20:30.000000 SAMBA_ilum-1.0.0.8/samba_ilum/src/bader_poscar.py
+-rw-rw-rw-   0        0        0     2527 2024-04-24 12:20:40.000000 SAMBA_ilum-1.0.0.8/samba_ilum/src/bader_update.py
+-rw-rw-rw-   0        0        0     7082 2024-05-03 16:12:30.000000 SAMBA_ilum-1.0.0.8/samba_ilum/src/charge_transfer.py
+-rw-rw-rw-   0        0        0     2139 2019-12-02 15:59:08.000000 SAMBA_ilum-1.0.0.8/samba_ilum/src/chgsum.pl
+-rw-rw-rw-   0        0        0      330 2024-04-24 12:20:58.000000 SAMBA_ilum-1.0.0.8/samba_ilum/src/contcar_update.py
+-rw-rw-rw-   0        0        0      600 2024-04-24 12:21:06.000000 SAMBA_ilum-1.0.0.8/samba_ilum/src/energy_scan.py
+-rw-rw-rw-   0        0        0    13083 2024-04-24 12:21:24.000000 SAMBA_ilum-1.0.0.8/samba_ilum/src/job.py
+-rw-rw-rw-   0        0        0     7163 2024-04-26 12:22:48.000000 SAMBA_ilum-1.0.0.8/samba_ilum/src/kpoints.py
+-rw-rw-rw-   0        0        0    21404 2024-04-24 12:21:42.000000 SAMBA_ilum-1.0.0.8/samba_ilum/src/make_files.py
+-rw-rw-rw-   0        0        0     5974 2024-05-03 16:13:18.000000 SAMBA_ilum-1.0.0.8/samba_ilum/src/output.py
+-rw-rw-rw-   0        0        0     1053 2024-04-24 12:21:58.000000 SAMBA_ilum-1.0.0.8/samba_ilum/src/potcar.py
+-rw-rw-rw-   0        0        0     7975 2024-04-24 12:22:06.000000 SAMBA_ilum-1.0.0.8/samba_ilum/src/xy-scan.py
+-rw-rw-rw-   0        0        0    15612 2024-04-24 12:22:12.000000 SAMBA_ilum-1.0.0.8/samba_ilum/src/xy-scan_analysis.py
+-rw-rw-rw-   0        0        0     9646 2024-04-27 11:31:28.000000 SAMBA_ilum-1.0.0.8/samba_ilum/src/z-scan.py
+-rw-rw-rw-   0        0        0     4348 2024-04-24 12:22:26.000000 SAMBA_ilum-1.0.0.8/samba_ilum/src/z-scan_analysis.py
+-rw-rw-rw-   0        0        0      167 2024-05-03 16:13:59.520748 SAMBA_ilum-1.0.0.8/setup.cfg
+-rw-rw-rw-   0        0        0      733 2024-05-03 16:13:34.000000 SAMBA_ilum-1.0.0.8/setup.py
```

### Comparing `SAMBA_ilum-1.0.0.7/SAMBA_ilum.egg-info/SOURCES.txt` & `SAMBA_ilum-1.0.0.8/SAMBA_ilum.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `SAMBA_ilum-1.0.0.7/samba_ilum/__main__.py` & `SAMBA_ilum-1.0.0.8/samba_ilum/__main__.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 import pyfiglet
 import shutil
 import time
 import sys
 import os
 
 
-version = '1.0.0.7'
+version = '1.0.0.8'
 
 
 print(" ")
 print("=============================================================")
 print(f'SAMBA_ilum v{version} Copyright (C) 2024 ----------------------')
 print("Closed source: Adalberto Fazzio's research group (Ilum|CNPEM)")
 print("Author: Augusto de Lelis Araujo -----------------------------")
 print("=============================================================")
-texto = pyfiglet.figlet_format("SAMBA", font="slant", width=100, justify="left")
+texto = pyfiglet.figlet_format("SAMBA ilum", font="slant", width=100, justify="left")
 print(texto)
 
 
 #----------------------
 dir_codes = 'src'
 dir_files = os.getcwd()
 os.chdir(os.path.dirname(os.path.realpath(__file__)))
```

### Comparing `SAMBA_ilum-1.0.0.7/samba_ilum/src/HeteroStructure_Generator.py` & `SAMBA_ilum-1.0.0.8/samba_ilum/src/HeteroStructure_Generator.py`

 * *Files identical despite different names*

### Comparing `SAMBA_ilum-1.0.0.7/samba_ilum/src/INPUTS/inputs_VASProcar/input.vasprocar.bands` & `SAMBA_ilum-1.0.0.8/samba_ilum/src/INPUTS/inputs_VASProcar/input.vasprocar.bands`

 * *Files identical despite different names*

### Comparing `SAMBA_ilum-1.0.0.7/samba_ilum/src/INPUTS/inputs_VASProcar/input.vasprocar.chgcar` & `SAMBA_ilum-1.0.0.8/samba_ilum/src/INPUTS/inputs_VASProcar/input.vasprocar.chgcar`

 * *Files identical despite different names*

### Comparing `SAMBA_ilum-1.0.0.7/samba_ilum/src/INPUTS/inputs_VASProcar/input.vasprocar.dos` & `SAMBA_ilum-1.0.0.8/samba_ilum/src/INPUTS/inputs_VASProcar/input.vasprocar.dos`

 * *Files identical despite different names*

### Comparing `SAMBA_ilum-1.0.0.7/samba_ilum/src/INPUTS/inputs_VASProcar/input.vasprocar.location` & `SAMBA_ilum-1.0.0.8/samba_ilum/src/INPUTS/inputs_VASProcar/input.vasprocar.location`

 * *Files identical despite different names*

### Comparing `SAMBA_ilum-1.0.0.7/samba_ilum/src/INPUTS/inputs_VASProcar/input.vasprocar.locpot` & `SAMBA_ilum-1.0.0.8/samba_ilum/src/INPUTS/inputs_VASProcar/input.vasprocar.locpot`

 * *Files identical despite different names*

### Comparing `SAMBA_ilum-1.0.0.7/samba_ilum/src/INPUTS/inputs_VASProcar/input.vasprocar.orbitals` & `SAMBA_ilum-1.0.0.8/samba_ilum/src/INPUTS/inputs_VASProcar/input.vasprocar.orbitals`

 * *Files identical despite different names*

### Comparing `SAMBA_ilum-1.0.0.7/samba_ilum/src/INPUTS/inputs_VASProcar/input.vasprocar.spin` & `SAMBA_ilum-1.0.0.8/samba_ilum/src/INPUTS/inputs_VASProcar/input.vasprocar.spin`

 * *Files identical despite different names*

### Comparing `SAMBA_ilum-1.0.0.7/samba_ilum/src/SAMBA_HeteroStructure.input` & `SAMBA_ilum-1.0.0.8/samba_ilum/src/SAMBA_HeteroStructure.input`

 * *Files identical despite different names*

### Comparing `SAMBA_ilum-1.0.0.7/samba_ilum/src/SAMBA_WorkFlow.input` & `SAMBA_ilum-1.0.0.8/samba_ilum/src/SAMBA_WorkFlow.input`

 * *Files identical despite different names*

### Comparing `SAMBA_ilum-1.0.0.7/samba_ilum/src/_info_pseudo.py` & `SAMBA_ilum-1.0.0.8/samba_ilum/src/_info_pseudo.py`

 * *Files identical despite different names*

### Comparing `SAMBA_ilum-1.0.0.7/samba_ilum/src/bader` & `SAMBA_ilum-1.0.0.8/samba_ilum/src/bader`

 * *Files identical despite different names*

### Comparing `SAMBA_ilum-1.0.0.7/samba_ilum/src/bader_poscar.py` & `SAMBA_ilum-1.0.0.8/samba_ilum/src/bader_poscar.py`

 * *Files identical despite different names*

### Comparing `SAMBA_ilum-1.0.0.7/samba_ilum/src/bader_update.py` & `SAMBA_ilum-1.0.0.8/samba_ilum/src/bader_update.py`

 * *Files identical despite different names*

### Comparing `SAMBA_ilum-1.0.0.7/samba_ilum/src/charge_transfer.py` & `SAMBA_ilum-1.0.0.8/samba_ilum/src/charge_transfer.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 # SAMBA_ilum Copyright (C) 2024 - Closed source
 
 
+import numpy as np
+
 
 #---------------------------
 poscar = open('POSCAR', 'r')
 VTemp = poscar.readline().split()
 #----------------------------------------------------------------------------
 # Obtendo o rotulo e o nº de átomos para cada material da Heteroestrutura ---
 #----------------------------------------------------------------------------
```

### Comparing `SAMBA_ilum-1.0.0.7/samba_ilum/src/chgsum.pl` & `SAMBA_ilum-1.0.0.8/samba_ilum/src/chgsum.pl`

 * *Files identical despite different names*

### Comparing `SAMBA_ilum-1.0.0.7/samba_ilum/src/energy_scan.py` & `SAMBA_ilum-1.0.0.8/samba_ilum/src/energy_scan.py`

 * *Files identical despite different names*

### Comparing `SAMBA_ilum-1.0.0.7/samba_ilum/src/job.py` & `SAMBA_ilum-1.0.0.8/samba_ilum/src/job.py`

 * *Files identical despite different names*

### Comparing `SAMBA_ilum-1.0.0.7/samba_ilum/src/kpoints.py` & `SAMBA_ilum-1.0.0.8/samba_ilum/src/kpoints.py`

 * *Files identical despite different names*

### Comparing `SAMBA_ilum-1.0.0.7/samba_ilum/src/make_files.py` & `SAMBA_ilum-1.0.0.8/samba_ilum/src/make_files.py`

 * *Files identical despite different names*

### Comparing `SAMBA_ilum-1.0.0.7/samba_ilum/src/output.py` & `SAMBA_ilum-1.0.0.8/samba_ilum/src/output.py`

 * *Files 3% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 
 for i in range(len(folders)):
     #-----------------------------------
     dir_folders = folders[i] + '/output'
     #-----------------------------------
     if (folders[i] == 'z-scan'):
        os.mkdir('output/z-scan')
-       if os.path.isfile(folders[i] + '/info_z-scan.dat'):  shutil.copy(folders[i] + '/info_z-scan.dat',  'output/xy-scan/info_z-scan.dat')
+       if os.path.isfile(folders[i] + '/info_z-scan.dat'):  shutil.copy(folders[i] + '/info_z-scan.dat',  'output/z-scan/info_z-scan.dat')
        if os.path.isfile(folders[i] + '/POSCAR.0'):  shutil.copy(folders[i] + '/POSCAR.0',  'output/z-scan/POSCAR_initial_z-scan.vasp')
        if os.path.isfile(folders[i] + '/POSCAR'):  shutil.copy(folders[i] + '/POSCAR',  'output/z-scan/POSCAR_final_z-scan.vasp')
        if os.path.isfile(folders[i] + '/z-scan.dat'):  shutil.copy(folders[i] + '/z-scan.dat',  'output/z-scan/z-scan.dat')
        if os.path.isfile(folders[i] + '/z-scan.png'):  shutil.copy(folders[i] + '/z-scan.png',  'output/z-scan/z-scan.png')
     #--------------------------------
     if (folders[i] == 'xy-scan'):
        os.mkdir('output/xy-scan')
@@ -36,52 +36,52 @@
        if os.path.isfile(folders[i] + '/xy-scan_direct.dat'):  shutil.copy(folders[i] + '/xy-scan_direct.dat',  'output/xy-scan/xy-scan_direct.dat')
        if os.path.isfile(folders[i] + '/info_xy-scan.dat'):  shutil.copy(folders[i] + '/info_xy-scan.dat',  'output/xy-scan/info_xy-scan.dat')
        if os.path.isfile(folders[i] + '/POSCAR.0'):  shutil.copy(folders[i] + '/POSCAR.0',  'output/xy-scan/POSCAR_initial_xy-scan.vasp')
        if os.path.isfile(folders[i] + '/POSCAR'):  shutil.copy(folders[i] + '/POSCAR',  'output/xy-scan/POSCAR_final_xy-scan.vasp')
     #--------------------------------
     if (folders[i] == 'scf'):
        if os.path.isdir(dir_folders + '/Potencial'):  shutil.copytree(dir_folders + '/Potencial',  'output/Potencial_scf')
-       if os.path.isdir(dir_folders):                 shutil.rmtree(dir_folders)
+       # if os.path.isdir(dir_folders):                 shutil.rmtree(dir_folders)
     #--------------------------------
     if (folders[i] == 'scf.SO'):
        if os.path.isdir(dir_folders + '/Potencial'):  shutil.copytree(dir_folders + '/Potencial',  'output/Potencial_scf_SO')
-       if os.path.isdir(dir_folders):                 shutil.rmtree(dir_folders)
+       # if os.path.isdir(dir_folders):                 shutil.rmtree(dir_folders)
     #--------------------------------
     if (folders[i] == 'dos'):
        if os.path.isdir(dir_folders + '/DOS'):  shutil.copytree(dir_folders + '/DOS',  'output/DOS')
-       if os.path.isdir(dir_folders):           shutil.rmtree(dir_folders)
+       # if os.path.isdir(dir_folders):           shutil.rmtree(dir_folders)
     #--------------------------------
     if (folders[i] == 'dos.SO'):
        if os.path.isdir(dir_folders + '/DOS'):  shutil.copytree(dir_folders + '/DOS',  'output/DOS_SO')
-       if os.path.isdir(dir_folders):           shutil.rmtree(dir_folders)
+       # if os.path.isdir(dir_folders):           shutil.rmtree(dir_folders)
     #--------------------------------
     if (folders[i] == 'bands'):
        if os.path.isdir(dir_folders + '/Bandas'):       shutil.copytree(dir_folders + '/Bandas',  'output/Bandas')
        if os.path.isdir(dir_folders + '/Orbitais'):     shutil.copytree(dir_folders + '/Orbitais',  'output/Orbitais')
        if os.path.isdir(dir_folders + '/Localizacao'):  shutil.copytree(dir_folders + '/Localizacao',  'output/Localizacao')
        if os.path.isdir(dir_folders + '/Potencial'):    shutil.copytree(dir_folders + '/Potencial',  'output/Potencial_bands')
        if os.path.isdir(dir_folders):                   shutil.copyfile(dir_folders + '/informacoes.txt',  'output/informacoes.txt')
-       if os.path.isdir(dir_folders):                   shutil.rmtree(dir_folders)
+       # if os.path.isdir(dir_folders):                   shutil.rmtree(dir_folders)
     #--------------------------------
     if (folders[i] == 'bands.SO'):
        if os.path.isdir(dir_folders + '/Spin'):         shutil.copytree(dir_folders + '/Spin',  'output/Spin')
        if os.path.isdir(dir_folders + '/Bandas'):       shutil.copytree(dir_folders + '/Bandas',  'output/Bandas_SO')
        if os.path.isdir(dir_folders + '/Orbitais'):     shutil.copytree(dir_folders + '/Orbitais',  'output/Orbitais_SO')
        if os.path.isdir(dir_folders + '/Localizacao'):  shutil.copytree(dir_folders + '/Localizacao',  'output/Localizacao_SO')
        if os.path.isdir(dir_folders + '/Potencial'):    shutil.copytree(dir_folders + '/Potencial',  'output/Potencial_bands_SO')
        if os.path.isdir(dir_folders):                   shutil.copyfile(dir_folders + '/informacoes.txt',  'output/informacoes_SO.txt')
-       if os.path.isdir(dir_folders):                   shutil.rmtree(dir_folders)
+       # if os.path.isdir(dir_folders):                   shutil.rmtree(dir_folders)
     #--------------------------------
     if (folders[i] == 'bader'):
        if os.path.isdir(folders[i] + '/Charge_transfer'):  shutil.copytree(folders[i] + '/Charge_transfer',  'output/Charge_transfer')
-       if os.path.isdir(folders[i] + '/Charge_transfer'):  shutil.rmtree(folders[i] + '/Charge_transfer')
+       # if os.path.isdir(folders[i] + '/Charge_transfer'):  shutil.rmtree(folders[i] + '/Charge_transfer')
     #--------------------------------
     if (folders[i] == 'bader.SO'):
        if os.path.isdir(folders[i] + '/Charge_transfer'):  shutil.copytree(folders[i] + '/Charge_transfer',  'output/Charge_transfer_SO')
-       if os.path.isdir(folders[i] + '/Charge_transfer'):  shutil.rmtree(folders[i] + '/Charge_transfer')
+       # if os.path.isdir(folders[i] + '/Charge_transfer'):  shutil.rmtree(folders[i] + '/Charge_transfer')
     #--------------------------------
```

### Comparing `SAMBA_ilum-1.0.0.7/samba_ilum/src/potcar.py` & `SAMBA_ilum-1.0.0.8/samba_ilum/src/potcar.py`

 * *Files identical despite different names*

### Comparing `SAMBA_ilum-1.0.0.7/samba_ilum/src/xy-scan.py` & `SAMBA_ilum-1.0.0.8/samba_ilum/src/xy-scan.py`

 * *Files identical despite different names*

### Comparing `SAMBA_ilum-1.0.0.7/samba_ilum/src/xy-scan_analysis.py` & `SAMBA_ilum-1.0.0.8/samba_ilum/src/xy-scan_analysis.py`

 * *Files identical despite different names*

### Comparing `SAMBA_ilum-1.0.0.7/samba_ilum/src/z-scan.py` & `SAMBA_ilum-1.0.0.8/samba_ilum/src/z-scan.py`

 * *Files 0% similar despite different names*

```diff
@@ -182,17 +182,17 @@
     poscar = open('POSCAR_cart', "r")
     poscar_new = open(str(deltaZ) + '/POSCAR', "w")
     VTemp = poscar.readline();  poscar_new.write(f'{VTemp}')
     VTemp = poscar.readline();  poscar_new.write(f'{VTemp}')
     VTemp = poscar.readline();  poscar_new.write(f'{VTemp}');  VTemp = VTemp.split();  A = [float(VTemp[0])*param, float(VTemp[1])*param, float(VTemp[2])*param]
     VTemp = poscar.readline();  poscar_new.write(f'{VTemp}');  VTemp = VTemp.split();  B = [float(VTemp[0])*param, float(VTemp[1])*param, float(VTemp[2])*param]
     VTemp = poscar.readline().split();  C = [float(VTemp[0])*param, float(VTemp[1])*param, float(VTemp[2])*param]
-    #-------------------------------------------
-    # temp_Z = (dZ_total + deltaZ + vacuo)/param
-    temp_Z = (dZ_total + deltaZ_f + vacuo)/param
+    #---------------------------------------------
+    # temp_Z = (dZ_total + deltaZ_f + vacuo)/param
+    temp_Z = (dZ_total + deltaZ + vacuo)/param
     poscar_new.write(f'{float(VTemp[0]):>28,.21f} {float(VTemp[1]):>28,.21f} {float(temp_Z):>28,.21f} \n')
     #-----------------------------------------------------------------------------------------------------
     VTemp = poscar.readline();  poscar_new.write(f'{VTemp}')
     VTemp = poscar.readline();  poscar_new.write(f'{VTemp}')
     VTemp = poscar.readline();  poscar_new.write(f'Cartesian \n')
     #------------------------------------------------------------
     for k in range(n_Lattice):
```

### Comparing `SAMBA_ilum-1.0.0.7/samba_ilum/src/z-scan_analysis.py` & `SAMBA_ilum-1.0.0.8/samba_ilum/src/z-scan_analysis.py`

 * *Files identical despite different names*

### Comparing `SAMBA_ilum-1.0.0.7/setup.py` & `SAMBA_ilum-1.0.0.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from setuptools import setup, find_packages
 import json
 from pathlib import Path
 from typing import Optional
 
 setup(
     name = "SAMBA_ilum",
-    version = "1.0.0.7",
+    version = "1.0.0.8",
     entry_points={'console_scripts': ['samba_ilum = samba_ilum:main']},
     description = "...",
     author = "Augusto de Lelis Araujo", 
     author_email = "augusto-lelis@outlook.com",
     license = "Closed source",
     install_requires=['numpy',
                       'requests',
```

