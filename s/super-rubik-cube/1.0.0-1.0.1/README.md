# Comparing `tmp/super_rubik_cube-1.0.0.tar.gz` & `tmp/super_rubik_cube-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "super_rubik_cube-1.0.0.tar", last modified: Sat May  4 16:15:25 2024, max compression
+gzip compressed data, was "super_rubik_cube-1.0.1.tar", last modified: Sat May  4 16:27:52 2024, max compression
```

## Comparing `super_rubik_cube-1.0.0.tar` & `super_rubik_cube-1.0.1.tar`

### file list

```diff
@@ -1,62 +1,62 @@
-drwxrwxrwx   0        0        0        0 2024-05-04 16:15:25.036956 super_rubik_cube-1.0.0/
--rw-rw-rw-   0        0        0    35816 2024-05-03 20:00:15.000000 super_rubik_cube-1.0.0/LICENSE
--rw-rw-rw-   0        0        0    20687 2024-05-04 16:15:25.035951 super_rubik_cube-1.0.0/PKG-INFO
--rw-rw-rw-   0        0        0    20274 2024-05-04 14:50:12.000000 super_rubik_cube-1.0.0/README.md
--rw-rw-rw-   0        0        0       42 2024-05-04 16:15:25.036956 super_rubik_cube-1.0.0/setup.cfg
--rw-rw-rw-   0        0        0      772 2024-05-04 16:08:19.000000 super_rubik_cube-1.0.0/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-04 16:15:25.035951 super_rubik_cube-1.0.0/super_rubik_cube.egg-info/
--rw-rw-rw-   0        0        0    20687 2024-05-04 16:15:24.000000 super_rubik_cube-1.0.0/super_rubik_cube.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2057 2024-05-04 16:15:24.000000 super_rubik_cube-1.0.0/super_rubik_cube.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-04 16:15:24.000000 super_rubik_cube-1.0.0/super_rubik_cube.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       10 2024-05-04 16:15:24.000000 super_rubik_cube-1.0.0/super_rubik_cube.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-05-04 16:15:24.995707 super_rubik_cube-1.0.0/supercube/
--rw-rw-rw-   0        0        0  3674160 2024-05-03 18:33:03.000000 super_rubik_cube-1.0.0/supercube/.cornerprun
--rw-rw-rw-   0        0        0    90720 2024-05-03 18:32:54.000000 super_rubik_cube-1.0.0/supercube/.move_cornperm
--rw-rw-rw-   0        0        0      297 2024-05-03 15:53:19.000000 super_rubik_cube-1.0.0/supercube/NCube.py
--rw-rw-rw-   0        0        0     1215 2024-05-03 17:20:04.000000 super_rubik_cube-1.0.0/supercube/PocketCube.py
--rw-rw-rw-   0        0        0     1207 2024-05-03 17:17:11.000000 super_rubik_cube-1.0.0/supercube/RubiksCube.py
--rw-rw-rw-   0        0        0       96 2024-05-03 15:43:15.000000 super_rubik_cube-1.0.0/supercube/__init__.py
--rw-rw-rw-   0        0        0    31193 2024-04-14 21:26:56.000000 super_rubik_cube-1.0.0/supercube/cube.py
-drwxrwxrwx   0        0        0        0 2024-05-04 16:15:24.998706 super_rubik_cube-1.0.0/supercube/kociemba/
--rw-rw-rw-   0        0        0     1462 2024-05-03 17:19:32.000000 super_rubik_cube-1.0.0/supercube/kociemba/__init__.py
--rw-rw-rw-   0        0        0     1119 2024-03-25 18:55:50.000000 super_rubik_cube-1.0.0/supercube/kociemba/build_ckociemba.py
--rw-rw-rw-   0        0        0      413 2024-03-25 18:55:50.000000 super_rubik_cube-1.0.0/supercube/kociemba/command_line.py
-drwxrwxrwx   0        0        0        0 2024-05-04 16:15:25.005258 super_rubik_cube-1.0.0/supercube/kociemba/pykociemba/
--rw-rw-rw-   0        0        0        0 2024-03-25 18:55:50.000000 super_rubik_cube-1.0.0/supercube/kociemba/pykociemba/__init__.py
--rw-rw-rw-   0        0        0      412 2024-03-25 18:55:50.000000 super_rubik_cube-1.0.0/supercube/kociemba/pykociemba/color.py
--rw-rw-rw-   0        0        0    19234 2024-03-25 18:55:50.000000 super_rubik_cube-1.0.0/supercube/kociemba/pykociemba/coordcube.py
--rw-rw-rw-   0        0        0      529 2024-03-25 18:55:50.000000 super_rubik_cube-1.0.0/supercube/kociemba/pykociemba/corner.py
--rw-rw-rw-   0        0        0    20176 2024-03-25 18:55:50.000000 super_rubik_cube-1.0.0/supercube/kociemba/pykociemba/cubiecube.py
--rw-rw-rw-   0        0        0      598 2024-03-25 18:55:50.000000 super_rubik_cube-1.0.0/supercube/kociemba/pykociemba/edge.py
--rw-rw-rw-   0        0        0     4060 2024-03-25 18:55:50.000000 super_rubik_cube-1.0.0/supercube/kociemba/pykociemba/facecube.py
--rw-rw-rw-   0        0        0     3178 2024-03-25 18:55:50.000000 super_rubik_cube-1.0.0/supercube/kociemba/pykociemba/facelet.py
-drwxrwxrwx   0        0        0        0 2024-05-04 16:15:25.025802 super_rubik_cube-1.0.0/supercube/kociemba/pykociemba/prunetables/
--rw-rw-rw-   0        0        0  1844165 2024-03-25 18:55:50.000000 super_rubik_cube-1.0.0/supercube/kociemba/pykociemba/prunetables/FRtoBR_Move.pkl
--rw-rw-rw-   0        0        0   729671 2024-03-25 18:55:50.000000 super_rubik_cube-1.0.0/supercube/kociemba/pykociemba/prunetables/MergeURtoULandUBtoDF.pkl
--rw-rw-rw-   0        0        0  3524721 2024-03-25 18:55:50.000000 super_rubik_cube-1.0.0/supercube/kociemba/pykociemba/prunetables/Slice_Flip_Prun.pkl
--rw-rw-rw-   0        0        0  3758442 2024-03-25 18:55:50.000000 super_rubik_cube-1.0.0/supercube/kociemba/pykociemba/prunetables/Slice_Twist_Prun.pkl
--rw-rw-rw-   0        0        0  3381387 2024-03-25 18:55:50.000000 super_rubik_cube-1.0.0/supercube/kociemba/pykociemba/prunetables/Slice_URFtoDLF_Parity_Prun.pkl
--rw-rw-rw-   0        0        0  3375661 2024-03-25 18:55:50.000000 super_rubik_cube-1.0.0/supercube/kociemba/pykociemba/prunetables/Slice_URtoDF_Parity_Prun.pkl
--rw-rw-rw-   0        0        0   182203 2024-03-25 18:55:50.000000 super_rubik_cube-1.0.0/supercube/kociemba/pykociemba/prunetables/UBtoDF_Move.pkl
--rw-rw-rw-   0        0        0  3276605 2024-03-25 18:55:50.000000 super_rubik_cube-1.0.0/supercube/kociemba/pykociemba/prunetables/URFtoDLF_Move.pkl
--rw-rw-rw-   0        0        0  3483565 2024-03-25 18:55:50.000000 super_rubik_cube-1.0.0/supercube/kociemba/pykociemba/prunetables/URtoDF_Move.pkl
--rw-rw-rw-   0        0        0   182203 2024-03-25 18:55:50.000000 super_rubik_cube-1.0.0/supercube/kociemba/pykociemba/prunetables/URtoUL_Move.pkl
--rw-rw-rw-   0        0        0   294315 2024-03-25 18:55:50.000000 super_rubik_cube-1.0.0/supercube/kociemba/pykociemba/prunetables/flipMove.pkl
--rw-rw-rw-   0        0        0   315721 2024-03-25 18:55:50.000000 super_rubik_cube-1.0.0/supercube/kociemba/pykociemba/prunetables/twistMove.pkl
--rw-rw-rw-   0        0        0    13523 2024-03-25 18:55:50.000000 super_rubik_cube-1.0.0/supercube/kociemba/pykociemba/search.py
--rw-rw-rw-   0        0        0     2485 2024-03-25 18:55:50.000000 super_rubik_cube-1.0.0/supercube/kociemba/pykociemba/tools.py
-drwxrwxrwx   0        0        0        0 2024-05-04 16:15:25.034910 super_rubik_cube-1.0.0/supercube/kociemba_2x2/
--rw-rw-rw-   0        0        0        0 2024-04-02 12:07:35.000000 super_rubik_cube-1.0.0/supercube/kociemba_2x2/__init__.py
--rw-rw-rw-   0        0        0     7752 2024-03-29 20:50:57.000000 super_rubik_cube-1.0.0/supercube/kociemba_2x2/client_gui.py
--rw-rw-rw-   0        0        0     1150 2024-05-03 17:23:20.000000 super_rubik_cube-1.0.0/supercube/kociemba_2x2/coord.py
--rw-rw-rw-   0        0        0     7188 2024-05-03 17:22:29.000000 super_rubik_cube-1.0.0/supercube/kociemba_2x2/cubie.py
--rw-rw-rw-   0        0        0     1122 2024-05-03 17:21:59.000000 super_rubik_cube-1.0.0/supercube/kociemba_2x2/defs.py
--rw-rw-rw-   0        0        0     2021 2024-03-29 20:50:57.000000 super_rubik_cube-1.0.0/supercube/kociemba_2x2/enums.py
--rw-rw-rw-   0        0        0     2980 2024-03-29 20:50:57.000000 super_rubik_cube-1.0.0/supercube/kociemba_2x2/example.py
--rw-rw-rw-   0        0        0     4874 2024-05-03 17:21:50.000000 super_rubik_cube-1.0.0/supercube/kociemba_2x2/face.py
--rw-rw-rw-   0        0        0      493 2024-03-29 20:50:57.000000 super_rubik_cube-1.0.0/supercube/kociemba_2x2/misc.py
--rw-rw-rw-   0        0        0     2177 2024-05-03 18:32:52.000000 super_rubik_cube-1.0.0/supercube/kociemba_2x2/moves.py
--rw-rw-rw-   0        0        0     1928 2024-05-03 18:32:52.000000 super_rubik_cube-1.0.0/supercube/kociemba_2x2/pruning.py
--rw-rw-rw-   0        0        0     2598 2024-03-29 20:50:57.000000 super_rubik_cube-1.0.0/supercube/kociemba_2x2/sockets.py
--rw-rw-rw-   0        0        0     2758 2024-05-03 17:21:32.000000 super_rubik_cube-1.0.0/supercube/kociemba_2x2/solver.py
--rw-rw-rw-   0        0        0      412 2024-03-29 20:50:57.000000 super_rubik_cube-1.0.0/supercube/kociemba_2x2/start_server.py
+drwxrwxrwx   0        0        0        0 2024-05-04 16:27:52.970192 super_rubik_cube-1.0.1/
+-rw-rw-rw-   0        0        0    35816 2024-05-03 20:00:15.000000 super_rubik_cube-1.0.1/LICENSE
+-rw-rw-rw-   0        0        0    20792 2024-05-04 16:27:52.970192 super_rubik_cube-1.0.1/PKG-INFO
+-rw-rw-rw-   0        0        0    20379 2024-05-04 16:27:14.000000 super_rubik_cube-1.0.1/README.md
+-rw-rw-rw-   0        0        0       42 2024-05-04 16:27:52.970192 super_rubik_cube-1.0.1/setup.cfg
+-rw-rw-rw-   0        0        0      772 2024-05-04 16:27:14.000000 super_rubik_cube-1.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-04 16:27:52.968194 super_rubik_cube-1.0.1/super_rubik_cube.egg-info/
+-rw-rw-rw-   0        0        0    20792 2024-05-04 16:27:52.000000 super_rubik_cube-1.0.1/super_rubik_cube.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2057 2024-05-04 16:27:52.000000 super_rubik_cube-1.0.1/super_rubik_cube.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-04 16:27:52.000000 super_rubik_cube-1.0.1/super_rubik_cube.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       10 2024-05-04 16:27:52.000000 super_rubik_cube-1.0.1/super_rubik_cube.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-04 16:27:52.929027 super_rubik_cube-1.0.1/supercube/
+-rw-rw-rw-   0        0        0  3674160 2024-05-03 18:33:03.000000 super_rubik_cube-1.0.1/supercube/.cornerprun
+-rw-rw-rw-   0        0        0    90720 2024-05-03 18:32:54.000000 super_rubik_cube-1.0.1/supercube/.move_cornperm
+-rw-rw-rw-   0        0        0      297 2024-05-03 15:53:19.000000 super_rubik_cube-1.0.1/supercube/NCube.py
+-rw-rw-rw-   0        0        0     1215 2024-05-03 17:20:04.000000 super_rubik_cube-1.0.1/supercube/PocketCube.py
+-rw-rw-rw-   0        0        0     1207 2024-05-03 17:17:11.000000 super_rubik_cube-1.0.1/supercube/RubiksCube.py
+-rw-rw-rw-   0        0        0       96 2024-05-03 15:43:15.000000 super_rubik_cube-1.0.1/supercube/__init__.py
+-rw-rw-rw-   0        0        0    31193 2024-04-14 21:26:56.000000 super_rubik_cube-1.0.1/supercube/cube.py
+drwxrwxrwx   0        0        0        0 2024-05-04 16:27:52.931026 super_rubik_cube-1.0.1/supercube/kociemba/
+-rw-rw-rw-   0        0        0     1462 2024-05-03 17:19:32.000000 super_rubik_cube-1.0.1/supercube/kociemba/__init__.py
+-rw-rw-rw-   0        0        0     1119 2024-03-25 18:55:50.000000 super_rubik_cube-1.0.1/supercube/kociemba/build_ckociemba.py
+-rw-rw-rw-   0        0        0      413 2024-03-25 18:55:50.000000 super_rubik_cube-1.0.1/supercube/kociemba/command_line.py
+drwxrwxrwx   0        0        0        0 2024-05-04 16:27:52.936035 super_rubik_cube-1.0.1/supercube/kociemba/pykociemba/
+-rw-rw-rw-   0        0        0        0 2024-03-25 18:55:50.000000 super_rubik_cube-1.0.1/supercube/kociemba/pykociemba/__init__.py
+-rw-rw-rw-   0        0        0      412 2024-03-25 18:55:50.000000 super_rubik_cube-1.0.1/supercube/kociemba/pykociemba/color.py
+-rw-rw-rw-   0        0        0    19234 2024-03-25 18:55:50.000000 super_rubik_cube-1.0.1/supercube/kociemba/pykociemba/coordcube.py
+-rw-rw-rw-   0        0        0      529 2024-03-25 18:55:50.000000 super_rubik_cube-1.0.1/supercube/kociemba/pykociemba/corner.py
+-rw-rw-rw-   0        0        0    20176 2024-03-25 18:55:50.000000 super_rubik_cube-1.0.1/supercube/kociemba/pykociemba/cubiecube.py
+-rw-rw-rw-   0        0        0      598 2024-03-25 18:55:50.000000 super_rubik_cube-1.0.1/supercube/kociemba/pykociemba/edge.py
+-rw-rw-rw-   0        0        0     4060 2024-03-25 18:55:50.000000 super_rubik_cube-1.0.1/supercube/kociemba/pykociemba/facecube.py
+-rw-rw-rw-   0        0        0     3178 2024-03-25 18:55:50.000000 super_rubik_cube-1.0.1/supercube/kociemba/pykociemba/facelet.py
+drwxrwxrwx   0        0        0        0 2024-05-04 16:27:52.958193 super_rubik_cube-1.0.1/supercube/kociemba/pykociemba/prunetables/
+-rw-rw-rw-   0        0        0  1844165 2024-03-25 18:55:50.000000 super_rubik_cube-1.0.1/supercube/kociemba/pykociemba/prunetables/FRtoBR_Move.pkl
+-rw-rw-rw-   0        0        0   729671 2024-03-25 18:55:50.000000 super_rubik_cube-1.0.1/supercube/kociemba/pykociemba/prunetables/MergeURtoULandUBtoDF.pkl
+-rw-rw-rw-   0        0        0  3524721 2024-03-25 18:55:50.000000 super_rubik_cube-1.0.1/supercube/kociemba/pykociemba/prunetables/Slice_Flip_Prun.pkl
+-rw-rw-rw-   0        0        0  3758442 2024-03-25 18:55:50.000000 super_rubik_cube-1.0.1/supercube/kociemba/pykociemba/prunetables/Slice_Twist_Prun.pkl
+-rw-rw-rw-   0        0        0  3381387 2024-03-25 18:55:50.000000 super_rubik_cube-1.0.1/supercube/kociemba/pykociemba/prunetables/Slice_URFtoDLF_Parity_Prun.pkl
+-rw-rw-rw-   0        0        0  3375661 2024-03-25 18:55:50.000000 super_rubik_cube-1.0.1/supercube/kociemba/pykociemba/prunetables/Slice_URtoDF_Parity_Prun.pkl
+-rw-rw-rw-   0        0        0   182203 2024-03-25 18:55:50.000000 super_rubik_cube-1.0.1/supercube/kociemba/pykociemba/prunetables/UBtoDF_Move.pkl
+-rw-rw-rw-   0        0        0  3276605 2024-03-25 18:55:50.000000 super_rubik_cube-1.0.1/supercube/kociemba/pykociemba/prunetables/URFtoDLF_Move.pkl
+-rw-rw-rw-   0        0        0  3483565 2024-03-25 18:55:50.000000 super_rubik_cube-1.0.1/supercube/kociemba/pykociemba/prunetables/URtoDF_Move.pkl
+-rw-rw-rw-   0        0        0   182203 2024-03-25 18:55:50.000000 super_rubik_cube-1.0.1/supercube/kociemba/pykociemba/prunetables/URtoUL_Move.pkl
+-rw-rw-rw-   0        0        0   294315 2024-03-25 18:55:50.000000 super_rubik_cube-1.0.1/supercube/kociemba/pykociemba/prunetables/flipMove.pkl
+-rw-rw-rw-   0        0        0   315721 2024-03-25 18:55:50.000000 super_rubik_cube-1.0.1/supercube/kociemba/pykociemba/prunetables/twistMove.pkl
+-rw-rw-rw-   0        0        0    13523 2024-03-25 18:55:50.000000 super_rubik_cube-1.0.1/supercube/kociemba/pykociemba/search.py
+-rw-rw-rw-   0        0        0     2485 2024-03-25 18:55:50.000000 super_rubik_cube-1.0.1/supercube/kociemba/pykociemba/tools.py
+drwxrwxrwx   0        0        0        0 2024-05-04 16:27:52.967194 super_rubik_cube-1.0.1/supercube/kociemba_2x2/
+-rw-rw-rw-   0        0        0        0 2024-04-02 12:07:35.000000 super_rubik_cube-1.0.1/supercube/kociemba_2x2/__init__.py
+-rw-rw-rw-   0        0        0     7752 2024-03-29 20:50:57.000000 super_rubik_cube-1.0.1/supercube/kociemba_2x2/client_gui.py
+-rw-rw-rw-   0        0        0     1150 2024-05-03 17:23:20.000000 super_rubik_cube-1.0.1/supercube/kociemba_2x2/coord.py
+-rw-rw-rw-   0        0        0     7188 2024-05-03 17:22:29.000000 super_rubik_cube-1.0.1/supercube/kociemba_2x2/cubie.py
+-rw-rw-rw-   0        0        0     1122 2024-05-03 17:21:59.000000 super_rubik_cube-1.0.1/supercube/kociemba_2x2/defs.py
+-rw-rw-rw-   0        0        0     2021 2024-03-29 20:50:57.000000 super_rubik_cube-1.0.1/supercube/kociemba_2x2/enums.py
+-rw-rw-rw-   0        0        0     2980 2024-03-29 20:50:57.000000 super_rubik_cube-1.0.1/supercube/kociemba_2x2/example.py
+-rw-rw-rw-   0        0        0     4874 2024-05-03 17:21:50.000000 super_rubik_cube-1.0.1/supercube/kociemba_2x2/face.py
+-rw-rw-rw-   0        0        0      493 2024-03-29 20:50:57.000000 super_rubik_cube-1.0.1/supercube/kociemba_2x2/misc.py
+-rw-rw-rw-   0        0        0     2177 2024-05-03 18:32:52.000000 super_rubik_cube-1.0.1/supercube/kociemba_2x2/moves.py
+-rw-rw-rw-   0        0        0     1928 2024-05-03 18:32:52.000000 super_rubik_cube-1.0.1/supercube/kociemba_2x2/pruning.py
+-rw-rw-rw-   0        0        0     2598 2024-03-29 20:50:57.000000 super_rubik_cube-1.0.1/supercube/kociemba_2x2/sockets.py
+-rw-rw-rw-   0        0        0     2758 2024-05-03 17:21:32.000000 super_rubik_cube-1.0.1/supercube/kociemba_2x2/solver.py
+-rw-rw-rw-   0        0        0      412 2024-03-29 20:50:57.000000 super_rubik_cube-1.0.1/supercube/kociemba_2x2/start_server.py
```

### Comparing `super_rubik_cube-1.0.0/LICENSE` & `super_rubik_cube-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `super_rubik_cube-1.0.0/PKG-INFO` & `super_rubik_cube-1.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 Metadata-Version: 2.1
 Name: super-rubik-cube
-Version: 1.0.0
+Version: 1.0.1
 Summary: Library for simulating rubik's cubes of different sizes (N x N), and for solving 2 x 2 and 3 x 3 cubes with kociemba algorithm.
 Author: Ilmi28
 Author-email: <ilmialiev28@gmail.com>
 Keywords: python,rubik,cube,solve,3x3,2x2,rubik's cube,pocket cube,NxN,kociemba,supercube
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Description
 Library for Rubik's Cube manipulation. Creator and customizer for cubes of any size, and solver for 2x2 and 3x3 cubes (Herbert Kociemba's algorithms)
 
 # Usage
+> Note: 2D number cube grid looks a bit weird in output examples, but in console everything looks fine.
 ## Creating instance of cube
 You can create Rubik's cube, Pocket cube and NxN cube, where N means positive number.
 ```
 import supercube
 
 rubiks_cube = supercube.RubiksCube() # creates 3X3 cube
 pocket_cube = supercube.PocketCube() # creates 2x2 cube
```

### Comparing `super_rubik_cube-1.0.0/README.md` & `super_rubik_cube-1.0.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # Description
 Library for Rubik's Cube manipulation. Creator and customizer for cubes of any size, and solver for 2x2 and 3x3 cubes (Herbert Kociemba's algorithms)
 
 # Usage
+> Note: 2D number cube grid looks a bit weird in output examples, but in console everything looks fine.
 ## Creating instance of cube
 You can create Rubik's cube, Pocket cube and NxN cube, where N means positive number.
 ```
 import supercube
 
 rubiks_cube = supercube.RubiksCube() # creates 3X3 cube
 pocket_cube = supercube.PocketCube() # creates 2x2 cube
```

### Comparing `super_rubik_cube-1.0.0/setup.py` & `super_rubik_cube-1.0.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 DESCRIPTION="Library for simulating rubik's cubes of different sizes (N x N), and for solving 2 x 2 and 3 x 3 cubes with kociemba algorithm."
 LONG_DESCRIPTION = open("README.md", encoding="utf8").read()
 
 
 setup(
     name="super-rubik-cube",
-    version="1.0.0",
+    version="1.0.1",
     author="Ilmi28",
     author_email="<ilmialiev28@gmail.com>",
     description=DESCRIPTION,
     long_description_content_type="text/markdown",
     long_description=LONG_DESCRIPTION,
     package_data={'supercube': ['.cornerprun', '.move_cornperm', 'kociemba/pykociemba/prunetables/*']},
     packages=find_packages(),
```

### Comparing `super_rubik_cube-1.0.0/super_rubik_cube.egg-info/PKG-INFO` & `super_rubik_cube-1.0.1/super_rubik_cube.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 Metadata-Version: 2.1
 Name: super-rubik-cube
-Version: 1.0.0
+Version: 1.0.1
 Summary: Library for simulating rubik's cubes of different sizes (N x N), and for solving 2 x 2 and 3 x 3 cubes with kociemba algorithm.
 Author: Ilmi28
 Author-email: <ilmialiev28@gmail.com>
 Keywords: python,rubik,cube,solve,3x3,2x2,rubik's cube,pocket cube,NxN,kociemba,supercube
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Description
 Library for Rubik's Cube manipulation. Creator and customizer for cubes of any size, and solver for 2x2 and 3x3 cubes (Herbert Kociemba's algorithms)
 
 # Usage
+> Note: 2D number cube grid looks a bit weird in output examples, but in console everything looks fine.
 ## Creating instance of cube
 You can create Rubik's cube, Pocket cube and NxN cube, where N means positive number.
 ```
 import supercube
 
 rubiks_cube = supercube.RubiksCube() # creates 3X3 cube
 pocket_cube = supercube.PocketCube() # creates 2x2 cube
```

### Comparing `super_rubik_cube-1.0.0/super_rubik_cube.egg-info/SOURCES.txt` & `super_rubik_cube-1.0.1/super_rubik_cube.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `super_rubik_cube-1.0.0/supercube/.cornerprun` & `super_rubik_cube-1.0.1/supercube/.cornerprun`

 * *Files identical despite different names*

### Comparing `super_rubik_cube-1.0.0/supercube/.move_cornperm` & `super_rubik_cube-1.0.1/supercube/.move_cornperm`

 * *Files identical despite different names*

### Comparing `super_rubik_cube-1.0.0/supercube/PocketCube.py` & `super_rubik_cube-1.0.1/supercube/PocketCube.py`

 * *Files identical despite different names*

### Comparing `super_rubik_cube-1.0.0/supercube/RubiksCube.py` & `super_rubik_cube-1.0.1/supercube/RubiksCube.py`

 * *Files identical despite different names*

### Comparing `super_rubik_cube-1.0.0/supercube/cube.py` & `super_rubik_cube-1.0.1/supercube/cube.py`

 * *Files identical despite different names*

### Comparing `super_rubik_cube-1.0.0/supercube/kociemba/__init__.py` & `super_rubik_cube-1.0.1/supercube/kociemba/__init__.py`

 * *Files identical despite different names*

### Comparing `super_rubik_cube-1.0.0/supercube/kociemba/build_ckociemba.py` & `super_rubik_cube-1.0.1/supercube/kociemba/build_ckociemba.py`

 * *Files identical despite different names*

### Comparing `super_rubik_cube-1.0.0/supercube/kociemba/pykociemba/coordcube.py` & `super_rubik_cube-1.0.1/supercube/kociemba/pykociemba/coordcube.py`

 * *Files identical despite different names*

### Comparing `super_rubik_cube-1.0.0/supercube/kociemba/pykociemba/corner.py` & `super_rubik_cube-1.0.1/supercube/kociemba/pykociemba/corner.py`

 * *Files identical despite different names*

### Comparing `super_rubik_cube-1.0.0/supercube/kociemba/pykociemba/cubiecube.py` & `super_rubik_cube-1.0.1/supercube/kociemba/pykociemba/cubiecube.py`

 * *Files identical despite different names*

### Comparing `super_rubik_cube-1.0.0/supercube/kociemba/pykociemba/edge.py` & `super_rubik_cube-1.0.1/supercube/kociemba/pykociemba/edge.py`

 * *Files identical despite different names*

### Comparing `super_rubik_cube-1.0.0/supercube/kociemba/pykociemba/facecube.py` & `super_rubik_cube-1.0.1/supercube/kociemba/pykociemba/facecube.py`

 * *Files identical despite different names*

### Comparing `super_rubik_cube-1.0.0/supercube/kociemba/pykociemba/facelet.py` & `super_rubik_cube-1.0.1/supercube/kociemba/pykociemba/facelet.py`

 * *Files identical despite different names*

### Comparing `super_rubik_cube-1.0.0/supercube/kociemba/pykociemba/prunetables/FRtoBR_Move.pkl` & `super_rubik_cube-1.0.1/supercube/kociemba/pykociemba/prunetables/FRtoBR_Move.pkl`

 * *Files identical despite different names*

### Comparing `super_rubik_cube-1.0.0/supercube/kociemba/pykociemba/prunetables/MergeURtoULandUBtoDF.pkl` & `super_rubik_cube-1.0.1/supercube/kociemba/pykociemba/prunetables/MergeURtoULandUBtoDF.pkl`

 * *Files identical despite different names*

### Comparing `super_rubik_cube-1.0.0/supercube/kociemba/pykociemba/prunetables/Slice_Flip_Prun.pkl` & `super_rubik_cube-1.0.1/supercube/kociemba/pykociemba/prunetables/Slice_Flip_Prun.pkl`

 * *Files identical despite different names*

### Comparing `super_rubik_cube-1.0.0/supercube/kociemba/pykociemba/prunetables/Slice_Twist_Prun.pkl` & `super_rubik_cube-1.0.1/supercube/kociemba/pykociemba/prunetables/Slice_Twist_Prun.pkl`

 * *Files identical despite different names*

### Comparing `super_rubik_cube-1.0.0/supercube/kociemba/pykociemba/prunetables/Slice_URFtoDLF_Parity_Prun.pkl` & `super_rubik_cube-1.0.1/supercube/kociemba/pykociemba/prunetables/Slice_URFtoDLF_Parity_Prun.pkl`

 * *Files identical despite different names*

### Comparing `super_rubik_cube-1.0.0/supercube/kociemba/pykociemba/prunetables/Slice_URtoDF_Parity_Prun.pkl` & `super_rubik_cube-1.0.1/supercube/kociemba/pykociemba/prunetables/Slice_URtoDF_Parity_Prun.pkl`

 * *Files identical despite different names*

### Comparing `super_rubik_cube-1.0.0/supercube/kociemba/pykociemba/prunetables/UBtoDF_Move.pkl` & `super_rubik_cube-1.0.1/supercube/kociemba/pykociemba/prunetables/UBtoDF_Move.pkl`

 * *Files identical despite different names*

### Comparing `super_rubik_cube-1.0.0/supercube/kociemba/pykociemba/prunetables/URFtoDLF_Move.pkl` & `super_rubik_cube-1.0.1/supercube/kociemba/pykociemba/prunetables/URFtoDLF_Move.pkl`

 * *Files identical despite different names*

### Comparing `super_rubik_cube-1.0.0/supercube/kociemba/pykociemba/prunetables/URtoDF_Move.pkl` & `super_rubik_cube-1.0.1/supercube/kociemba/pykociemba/prunetables/URtoDF_Move.pkl`

 * *Files identical despite different names*

### Comparing `super_rubik_cube-1.0.0/supercube/kociemba/pykociemba/prunetables/URtoUL_Move.pkl` & `super_rubik_cube-1.0.1/supercube/kociemba/pykociemba/prunetables/URtoUL_Move.pkl`

 * *Files identical despite different names*

### Comparing `super_rubik_cube-1.0.0/supercube/kociemba/pykociemba/prunetables/flipMove.pkl` & `super_rubik_cube-1.0.1/supercube/kociemba/pykociemba/prunetables/flipMove.pkl`

 * *Files identical despite different names*

### Comparing `super_rubik_cube-1.0.0/supercube/kociemba/pykociemba/prunetables/twistMove.pkl` & `super_rubik_cube-1.0.1/supercube/kociemba/pykociemba/prunetables/twistMove.pkl`

 * *Files identical despite different names*

### Comparing `super_rubik_cube-1.0.0/supercube/kociemba/pykociemba/search.py` & `super_rubik_cube-1.0.1/supercube/kociemba/pykociemba/search.py`

 * *Files identical despite different names*

### Comparing `super_rubik_cube-1.0.0/supercube/kociemba/pykociemba/tools.py` & `super_rubik_cube-1.0.1/supercube/kociemba/pykociemba/tools.py`

 * *Files identical despite different names*

### Comparing `super_rubik_cube-1.0.0/supercube/kociemba_2x2/client_gui.py` & `super_rubik_cube-1.0.1/supercube/kociemba_2x2/client_gui.py`

 * *Files identical despite different names*

### Comparing `super_rubik_cube-1.0.0/supercube/kociemba_2x2/coord.py` & `super_rubik_cube-1.0.1/supercube/kociemba_2x2/coord.py`

 * *Files identical despite different names*

### Comparing `super_rubik_cube-1.0.0/supercube/kociemba_2x2/cubie.py` & `super_rubik_cube-1.0.1/supercube/kociemba_2x2/cubie.py`

 * *Files identical despite different names*

### Comparing `super_rubik_cube-1.0.0/supercube/kociemba_2x2/defs.py` & `super_rubik_cube-1.0.1/supercube/kociemba_2x2/defs.py`

 * *Files identical despite different names*

### Comparing `super_rubik_cube-1.0.0/supercube/kociemba_2x2/enums.py` & `super_rubik_cube-1.0.1/supercube/kociemba_2x2/enums.py`

 * *Files identical despite different names*

### Comparing `super_rubik_cube-1.0.0/supercube/kociemba_2x2/example.py` & `super_rubik_cube-1.0.1/supercube/kociemba_2x2/example.py`

 * *Files identical despite different names*

### Comparing `super_rubik_cube-1.0.0/supercube/kociemba_2x2/face.py` & `super_rubik_cube-1.0.1/supercube/kociemba_2x2/face.py`

 * *Files identical despite different names*

### Comparing `super_rubik_cube-1.0.0/supercube/kociemba_2x2/moves.py` & `super_rubik_cube-1.0.1/supercube/kociemba_2x2/moves.py`

 * *Files identical despite different names*

### Comparing `super_rubik_cube-1.0.0/supercube/kociemba_2x2/pruning.py` & `super_rubik_cube-1.0.1/supercube/kociemba_2x2/pruning.py`

 * *Files identical despite different names*

### Comparing `super_rubik_cube-1.0.0/supercube/kociemba_2x2/sockets.py` & `super_rubik_cube-1.0.1/supercube/kociemba_2x2/sockets.py`

 * *Files identical despite different names*

### Comparing `super_rubik_cube-1.0.0/supercube/kociemba_2x2/solver.py` & `super_rubik_cube-1.0.1/supercube/kociemba_2x2/solver.py`

 * *Files identical despite different names*

