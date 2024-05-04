# Comparing `tmp/super_rubik_cube-1.0.1.tar.gz` & `tmp/super_rubik_cube-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "super_rubik_cube-1.0.1.tar", last modified: Sat May  4 16:27:52 2024, max compression
+gzip compressed data, was "super_rubik_cube-1.0.2.tar", last modified: Sat May  4 16:47:59 2024, max compression
```

## Comparing `super_rubik_cube-1.0.1.tar` & `super_rubik_cube-1.0.2.tar`

### file list

```diff
@@ -1,62 +1,62 @@
-drwxrwxrwx   0        0        0        0 2024-05-04 16:27:52.970192 super_rubik_cube-1.0.1/
--rw-rw-rw-   0        0        0    35816 2024-05-03 20:00:15.000000 super_rubik_cube-1.0.1/LICENSE
--rw-rw-rw-   0        0        0    20792 2024-05-04 16:27:52.970192 super_rubik_cube-1.0.1/PKG-INFO
--rw-rw-rw-   0        0        0    20379 2024-05-04 16:27:14.000000 super_rubik_cube-1.0.1/README.md
--rw-rw-rw-   0        0        0       42 2024-05-04 16:27:52.970192 super_rubik_cube-1.0.1/setup.cfg
--rw-rw-rw-   0        0        0      772 2024-05-04 16:27:14.000000 super_rubik_cube-1.0.1/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-04 16:27:52.968194 super_rubik_cube-1.0.1/super_rubik_cube.egg-info/
--rw-rw-rw-   0        0        0    20792 2024-05-04 16:27:52.000000 super_rubik_cube-1.0.1/super_rubik_cube.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2057 2024-05-04 16:27:52.000000 super_rubik_cube-1.0.1/super_rubik_cube.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-04 16:27:52.000000 super_rubik_cube-1.0.1/super_rubik_cube.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       10 2024-05-04 16:27:52.000000 super_rubik_cube-1.0.1/super_rubik_cube.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-05-04 16:27:52.929027 super_rubik_cube-1.0.1/supercube/
--rw-rw-rw-   0        0        0  3674160 2024-05-03 18:33:03.000000 super_rubik_cube-1.0.1/supercube/.cornerprun
--rw-rw-rw-   0        0        0    90720 2024-05-03 18:32:54.000000 super_rubik_cube-1.0.1/supercube/.move_cornperm
--rw-rw-rw-   0        0        0      297 2024-05-03 15:53:19.000000 super_rubik_cube-1.0.1/supercube/NCube.py
--rw-rw-rw-   0        0        0     1215 2024-05-03 17:20:04.000000 super_rubik_cube-1.0.1/supercube/PocketCube.py
--rw-rw-rw-   0        0        0     1207 2024-05-03 17:17:11.000000 super_rubik_cube-1.0.1/supercube/RubiksCube.py
--rw-rw-rw-   0        0        0       96 2024-05-03 15:43:15.000000 super_rubik_cube-1.0.1/supercube/__init__.py
--rw-rw-rw-   0        0        0    31193 2024-04-14 21:26:56.000000 super_rubik_cube-1.0.1/supercube/cube.py
-drwxrwxrwx   0        0        0        0 2024-05-04 16:27:52.931026 super_rubik_cube-1.0.1/supercube/kociemba/
--rw-rw-rw-   0        0        0     1462 2024-05-03 17:19:32.000000 super_rubik_cube-1.0.1/supercube/kociemba/__init__.py
--rw-rw-rw-   0        0        0     1119 2024-03-25 18:55:50.000000 super_rubik_cube-1.0.1/supercube/kociemba/build_ckociemba.py
--rw-rw-rw-   0        0        0      413 2024-03-25 18:55:50.000000 super_rubik_cube-1.0.1/supercube/kociemba/command_line.py
-drwxrwxrwx   0        0        0        0 2024-05-04 16:27:52.936035 super_rubik_cube-1.0.1/supercube/kociemba/pykociemba/
--rw-rw-rw-   0        0        0        0 2024-03-25 18:55:50.000000 super_rubik_cube-1.0.1/supercube/kociemba/pykociemba/__init__.py
--rw-rw-rw-   0        0        0      412 2024-03-25 18:55:50.000000 super_rubik_cube-1.0.1/supercube/kociemba/pykociemba/color.py
--rw-rw-rw-   0        0        0    19234 2024-03-25 18:55:50.000000 super_rubik_cube-1.0.1/supercube/kociemba/pykociemba/coordcube.py
--rw-rw-rw-   0        0        0      529 2024-03-25 18:55:50.000000 super_rubik_cube-1.0.1/supercube/kociemba/pykociemba/corner.py
--rw-rw-rw-   0        0        0    20176 2024-03-25 18:55:50.000000 super_rubik_cube-1.0.1/supercube/kociemba/pykociemba/cubiecube.py
--rw-rw-rw-   0        0        0      598 2024-03-25 18:55:50.000000 super_rubik_cube-1.0.1/supercube/kociemba/pykociemba/edge.py
--rw-rw-rw-   0        0        0     4060 2024-03-25 18:55:50.000000 super_rubik_cube-1.0.1/supercube/kociemba/pykociemba/facecube.py
--rw-rw-rw-   0        0        0     3178 2024-03-25 18:55:50.000000 super_rubik_cube-1.0.1/supercube/kociemba/pykociemba/facelet.py
-drwxrwxrwx   0        0        0        0 2024-05-04 16:27:52.958193 super_rubik_cube-1.0.1/supercube/kociemba/pykociemba/prunetables/
--rw-rw-rw-   0        0        0  1844165 2024-03-25 18:55:50.000000 super_rubik_cube-1.0.1/supercube/kociemba/pykociemba/prunetables/FRtoBR_Move.pkl
--rw-rw-rw-   0        0        0   729671 2024-03-25 18:55:50.000000 super_rubik_cube-1.0.1/supercube/kociemba/pykociemba/prunetables/MergeURtoULandUBtoDF.pkl
--rw-rw-rw-   0        0        0  3524721 2024-03-25 18:55:50.000000 super_rubik_cube-1.0.1/supercube/kociemba/pykociemba/prunetables/Slice_Flip_Prun.pkl
--rw-rw-rw-   0        0        0  3758442 2024-03-25 18:55:50.000000 super_rubik_cube-1.0.1/supercube/kociemba/pykociemba/prunetables/Slice_Twist_Prun.pkl
--rw-rw-rw-   0        0        0  3381387 2024-03-25 18:55:50.000000 super_rubik_cube-1.0.1/supercube/kociemba/pykociemba/prunetables/Slice_URFtoDLF_Parity_Prun.pkl
--rw-rw-rw-   0        0        0  3375661 2024-03-25 18:55:50.000000 super_rubik_cube-1.0.1/supercube/kociemba/pykociemba/prunetables/Slice_URtoDF_Parity_Prun.pkl
--rw-rw-rw-   0        0        0   182203 2024-03-25 18:55:50.000000 super_rubik_cube-1.0.1/supercube/kociemba/pykociemba/prunetables/UBtoDF_Move.pkl
--rw-rw-rw-   0        0        0  3276605 2024-03-25 18:55:50.000000 super_rubik_cube-1.0.1/supercube/kociemba/pykociemba/prunetables/URFtoDLF_Move.pkl
--rw-rw-rw-   0        0        0  3483565 2024-03-25 18:55:50.000000 super_rubik_cube-1.0.1/supercube/kociemba/pykociemba/prunetables/URtoDF_Move.pkl
--rw-rw-rw-   0        0        0   182203 2024-03-25 18:55:50.000000 super_rubik_cube-1.0.1/supercube/kociemba/pykociemba/prunetables/URtoUL_Move.pkl
--rw-rw-rw-   0        0        0   294315 2024-03-25 18:55:50.000000 super_rubik_cube-1.0.1/supercube/kociemba/pykociemba/prunetables/flipMove.pkl
--rw-rw-rw-   0        0        0   315721 2024-03-25 18:55:50.000000 super_rubik_cube-1.0.1/supercube/kociemba/pykociemba/prunetables/twistMove.pkl
--rw-rw-rw-   0        0        0    13523 2024-03-25 18:55:50.000000 super_rubik_cube-1.0.1/supercube/kociemba/pykociemba/search.py
--rw-rw-rw-   0        0        0     2485 2024-03-25 18:55:50.000000 super_rubik_cube-1.0.1/supercube/kociemba/pykociemba/tools.py
-drwxrwxrwx   0        0        0        0 2024-05-04 16:27:52.967194 super_rubik_cube-1.0.1/supercube/kociemba_2x2/
--rw-rw-rw-   0        0        0        0 2024-04-02 12:07:35.000000 super_rubik_cube-1.0.1/supercube/kociemba_2x2/__init__.py
--rw-rw-rw-   0        0        0     7752 2024-03-29 20:50:57.000000 super_rubik_cube-1.0.1/supercube/kociemba_2x2/client_gui.py
--rw-rw-rw-   0        0        0     1150 2024-05-03 17:23:20.000000 super_rubik_cube-1.0.1/supercube/kociemba_2x2/coord.py
--rw-rw-rw-   0        0        0     7188 2024-05-03 17:22:29.000000 super_rubik_cube-1.0.1/supercube/kociemba_2x2/cubie.py
--rw-rw-rw-   0        0        0     1122 2024-05-03 17:21:59.000000 super_rubik_cube-1.0.1/supercube/kociemba_2x2/defs.py
--rw-rw-rw-   0        0        0     2021 2024-03-29 20:50:57.000000 super_rubik_cube-1.0.1/supercube/kociemba_2x2/enums.py
--rw-rw-rw-   0        0        0     2980 2024-03-29 20:50:57.000000 super_rubik_cube-1.0.1/supercube/kociemba_2x2/example.py
--rw-rw-rw-   0        0        0     4874 2024-05-03 17:21:50.000000 super_rubik_cube-1.0.1/supercube/kociemba_2x2/face.py
--rw-rw-rw-   0        0        0      493 2024-03-29 20:50:57.000000 super_rubik_cube-1.0.1/supercube/kociemba_2x2/misc.py
--rw-rw-rw-   0        0        0     2177 2024-05-03 18:32:52.000000 super_rubik_cube-1.0.1/supercube/kociemba_2x2/moves.py
--rw-rw-rw-   0        0        0     1928 2024-05-03 18:32:52.000000 super_rubik_cube-1.0.1/supercube/kociemba_2x2/pruning.py
--rw-rw-rw-   0        0        0     2598 2024-03-29 20:50:57.000000 super_rubik_cube-1.0.1/supercube/kociemba_2x2/sockets.py
--rw-rw-rw-   0        0        0     2758 2024-05-03 17:21:32.000000 super_rubik_cube-1.0.1/supercube/kociemba_2x2/solver.py
--rw-rw-rw-   0        0        0      412 2024-03-29 20:50:57.000000 super_rubik_cube-1.0.1/supercube/kociemba_2x2/start_server.py
+drwxrwxrwx   0        0        0        0 2024-05-04 16:47:59.628768 super_rubik_cube-1.0.2/
+-rw-rw-rw-   0        0        0    35816 2024-05-03 20:00:15.000000 super_rubik_cube-1.0.2/LICENSE
+-rw-rw-rw-   0        0        0    20792 2024-05-04 16:47:59.627725 super_rubik_cube-1.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0    20379 2024-05-04 16:27:14.000000 super_rubik_cube-1.0.2/README.md
+-rw-rw-rw-   0        0        0       42 2024-05-04 16:47:59.628768 super_rubik_cube-1.0.2/setup.cfg
+-rw-rw-rw-   0        0        0      772 2024-05-04 16:47:53.000000 super_rubik_cube-1.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-04 16:47:59.626725 super_rubik_cube-1.0.2/super_rubik_cube.egg-info/
+-rw-rw-rw-   0        0        0    20792 2024-05-04 16:47:59.000000 super_rubik_cube-1.0.2/super_rubik_cube.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2057 2024-05-04 16:47:59.000000 super_rubik_cube-1.0.2/super_rubik_cube.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-04 16:47:59.000000 super_rubik_cube-1.0.2/super_rubik_cube.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       10 2024-05-04 16:47:59.000000 super_rubik_cube-1.0.2/super_rubik_cube.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-04 16:47:59.591132 super_rubik_cube-1.0.2/supercube/
+-rw-rw-rw-   0        0        0  3674160 2024-05-03 18:33:03.000000 super_rubik_cube-1.0.2/supercube/.cornerprun
+-rw-rw-rw-   0        0        0    90720 2024-05-03 18:32:54.000000 super_rubik_cube-1.0.2/supercube/.move_cornperm
+-rw-rw-rw-   0        0        0      297 2024-05-03 15:53:19.000000 super_rubik_cube-1.0.2/supercube/NCube.py
+-rw-rw-rw-   0        0        0     1215 2024-05-03 17:20:04.000000 super_rubik_cube-1.0.2/supercube/PocketCube.py
+-rw-rw-rw-   0        0        0     1207 2024-05-03 17:17:11.000000 super_rubik_cube-1.0.2/supercube/RubiksCube.py
+-rw-rw-rw-   0        0        0       96 2024-05-03 15:43:15.000000 super_rubik_cube-1.0.2/supercube/__init__.py
+-rw-rw-rw-   0        0        0    31193 2024-04-14 21:26:56.000000 super_rubik_cube-1.0.2/supercube/cube.py
+drwxrwxrwx   0        0        0        0 2024-05-04 16:47:59.593132 super_rubik_cube-1.0.2/supercube/kociemba/
+-rw-rw-rw-   0        0        0     1462 2024-05-03 17:19:32.000000 super_rubik_cube-1.0.2/supercube/kociemba/__init__.py
+-rw-rw-rw-   0        0        0     1119 2024-03-25 18:55:50.000000 super_rubik_cube-1.0.2/supercube/kociemba/build_ckociemba.py
+-rw-rw-rw-   0        0        0      413 2024-03-25 18:55:50.000000 super_rubik_cube-1.0.2/supercube/kociemba/command_line.py
+drwxrwxrwx   0        0        0        0 2024-05-04 16:47:59.597659 super_rubik_cube-1.0.2/supercube/kociemba/pykociemba/
+-rw-rw-rw-   0        0        0        0 2024-03-25 18:55:50.000000 super_rubik_cube-1.0.2/supercube/kociemba/pykociemba/__init__.py
+-rw-rw-rw-   0        0        0      412 2024-03-25 18:55:50.000000 super_rubik_cube-1.0.2/supercube/kociemba/pykociemba/color.py
+-rw-rw-rw-   0        0        0    19234 2024-03-25 18:55:50.000000 super_rubik_cube-1.0.2/supercube/kociemba/pykociemba/coordcube.py
+-rw-rw-rw-   0        0        0      529 2024-03-25 18:55:50.000000 super_rubik_cube-1.0.2/supercube/kociemba/pykociemba/corner.py
+-rw-rw-rw-   0        0        0    20176 2024-03-25 18:55:50.000000 super_rubik_cube-1.0.2/supercube/kociemba/pykociemba/cubiecube.py
+-rw-rw-rw-   0        0        0      598 2024-03-25 18:55:50.000000 super_rubik_cube-1.0.2/supercube/kociemba/pykociemba/edge.py
+-rw-rw-rw-   0        0        0     4060 2024-03-25 18:55:50.000000 super_rubik_cube-1.0.2/supercube/kociemba/pykociemba/facecube.py
+-rw-rw-rw-   0        0        0     3178 2024-03-25 18:55:50.000000 super_rubik_cube-1.0.2/supercube/kociemba/pykociemba/facelet.py
+drwxrwxrwx   0        0        0        0 2024-05-04 16:47:59.618216 super_rubik_cube-1.0.2/supercube/kociemba/pykociemba/prunetables/
+-rw-rw-rw-   0        0        0  1844165 2024-03-25 18:55:50.000000 super_rubik_cube-1.0.2/supercube/kociemba/pykociemba/prunetables/FRtoBR_Move.pkl
+-rw-rw-rw-   0        0        0   729671 2024-03-25 18:55:50.000000 super_rubik_cube-1.0.2/supercube/kociemba/pykociemba/prunetables/MergeURtoULandUBtoDF.pkl
+-rw-rw-rw-   0        0        0  3524721 2024-03-25 18:55:50.000000 super_rubik_cube-1.0.2/supercube/kociemba/pykociemba/prunetables/Slice_Flip_Prun.pkl
+-rw-rw-rw-   0        0        0  3758442 2024-03-25 18:55:50.000000 super_rubik_cube-1.0.2/supercube/kociemba/pykociemba/prunetables/Slice_Twist_Prun.pkl
+-rw-rw-rw-   0        0        0  3381387 2024-03-25 18:55:50.000000 super_rubik_cube-1.0.2/supercube/kociemba/pykociemba/prunetables/Slice_URFtoDLF_Parity_Prun.pkl
+-rw-rw-rw-   0        0        0  3375661 2024-03-25 18:55:50.000000 super_rubik_cube-1.0.2/supercube/kociemba/pykociemba/prunetables/Slice_URtoDF_Parity_Prun.pkl
+-rw-rw-rw-   0        0        0   182203 2024-03-25 18:55:50.000000 super_rubik_cube-1.0.2/supercube/kociemba/pykociemba/prunetables/UBtoDF_Move.pkl
+-rw-rw-rw-   0        0        0  3276605 2024-03-25 18:55:50.000000 super_rubik_cube-1.0.2/supercube/kociemba/pykociemba/prunetables/URFtoDLF_Move.pkl
+-rw-rw-rw-   0        0        0  3483565 2024-03-25 18:55:50.000000 super_rubik_cube-1.0.2/supercube/kociemba/pykociemba/prunetables/URtoDF_Move.pkl
+-rw-rw-rw-   0        0        0   182203 2024-03-25 18:55:50.000000 super_rubik_cube-1.0.2/supercube/kociemba/pykociemba/prunetables/URtoUL_Move.pkl
+-rw-rw-rw-   0        0        0   294315 2024-03-25 18:55:50.000000 super_rubik_cube-1.0.2/supercube/kociemba/pykociemba/prunetables/flipMove.pkl
+-rw-rw-rw-   0        0        0   315721 2024-03-25 18:55:50.000000 super_rubik_cube-1.0.2/supercube/kociemba/pykociemba/prunetables/twistMove.pkl
+-rw-rw-rw-   0        0        0    13523 2024-03-25 18:55:50.000000 super_rubik_cube-1.0.2/supercube/kociemba/pykociemba/search.py
+-rw-rw-rw-   0        0        0     2485 2024-03-25 18:55:50.000000 super_rubik_cube-1.0.2/supercube/kociemba/pykociemba/tools.py
+drwxrwxrwx   0        0        0        0 2024-05-04 16:47:59.626725 super_rubik_cube-1.0.2/supercube/kociemba_2x2/
+-rw-rw-rw-   0        0        0        0 2024-04-02 12:07:35.000000 super_rubik_cube-1.0.2/supercube/kociemba_2x2/__init__.py
+-rw-rw-rw-   0        0        0     7752 2024-03-29 20:50:57.000000 super_rubik_cube-1.0.2/supercube/kociemba_2x2/client_gui.py
+-rw-rw-rw-   0        0        0     1150 2024-05-03 17:23:20.000000 super_rubik_cube-1.0.2/supercube/kociemba_2x2/coord.py
+-rw-rw-rw-   0        0        0     7188 2024-05-03 17:22:29.000000 super_rubik_cube-1.0.2/supercube/kociemba_2x2/cubie.py
+-rw-rw-rw-   0        0        0     1122 2024-05-03 17:21:59.000000 super_rubik_cube-1.0.2/supercube/kociemba_2x2/defs.py
+-rw-rw-rw-   0        0        0     2021 2024-03-29 20:50:57.000000 super_rubik_cube-1.0.2/supercube/kociemba_2x2/enums.py
+-rw-rw-rw-   0        0        0     2980 2024-03-29 20:50:57.000000 super_rubik_cube-1.0.2/supercube/kociemba_2x2/example.py
+-rw-rw-rw-   0        0        0     4874 2024-05-03 17:21:50.000000 super_rubik_cube-1.0.2/supercube/kociemba_2x2/face.py
+-rw-rw-rw-   0        0        0      493 2024-03-29 20:50:57.000000 super_rubik_cube-1.0.2/supercube/kociemba_2x2/misc.py
+-rw-rw-rw-   0        0        0     2157 2024-05-04 16:45:18.000000 super_rubik_cube-1.0.2/supercube/kociemba_2x2/moves.py
+-rw-rw-rw-   0        0        0     1918 2024-05-04 16:45:26.000000 super_rubik_cube-1.0.2/supercube/kociemba_2x2/pruning.py
+-rw-rw-rw-   0        0        0     2598 2024-03-29 20:50:57.000000 super_rubik_cube-1.0.2/supercube/kociemba_2x2/sockets.py
+-rw-rw-rw-   0        0        0     2758 2024-05-03 17:21:32.000000 super_rubik_cube-1.0.2/supercube/kociemba_2x2/solver.py
+-rw-rw-rw-   0        0        0      412 2024-03-29 20:50:57.000000 super_rubik_cube-1.0.2/supercube/kociemba_2x2/start_server.py
```

### Comparing `super_rubik_cube-1.0.1/LICENSE` & `super_rubik_cube-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `super_rubik_cube-1.0.1/PKG-INFO` & `super_rubik_cube-1.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: super-rubik-cube
-Version: 1.0.1
+Version: 1.0.2
 Summary: Library for simulating rubik's cubes of different sizes (N x N), and for solving 2 x 2 and 3 x 3 cubes with kociemba algorithm.
 Author: Ilmi28
 Author-email: <ilmialiev28@gmail.com>
 Keywords: python,rubik,cube,solve,3x3,2x2,rubik's cube,pocket cube,NxN,kociemba,supercube
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `super_rubik_cube-1.0.1/README.md` & `super_rubik_cube-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `super_rubik_cube-1.0.1/setup.py` & `super_rubik_cube-1.0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 DESCRIPTION="Library for simulating rubik's cubes of different sizes (N x N), and for solving 2 x 2 and 3 x 3 cubes with kociemba algorithm."
 LONG_DESCRIPTION = open("README.md", encoding="utf8").read()
 
 
 setup(
     name="super-rubik-cube",
-    version="1.0.1",
+    version="1.0.2",
     author="Ilmi28",
     author_email="<ilmialiev28@gmail.com>",
     description=DESCRIPTION,
     long_description_content_type="text/markdown",
     long_description=LONG_DESCRIPTION,
     package_data={'supercube': ['.cornerprun', '.move_cornperm', 'kociemba/pykociemba/prunetables/*']},
     packages=find_packages(),
```

### Comparing `super_rubik_cube-1.0.1/super_rubik_cube.egg-info/PKG-INFO` & `super_rubik_cube-1.0.2/super_rubik_cube.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: super-rubik-cube
-Version: 1.0.1
+Version: 1.0.2
 Summary: Library for simulating rubik's cubes of different sizes (N x N), and for solving 2 x 2 and 3 x 3 cubes with kociemba algorithm.
 Author: Ilmi28
 Author-email: <ilmialiev28@gmail.com>
 Keywords: python,rubik,cube,solve,3x3,2x2,rubik's cube,pocket cube,NxN,kociemba,supercube
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `super_rubik_cube-1.0.1/super_rubik_cube.egg-info/SOURCES.txt` & `super_rubik_cube-1.0.2/super_rubik_cube.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `super_rubik_cube-1.0.1/supercube/.cornerprun` & `super_rubik_cube-1.0.2/supercube/.cornerprun`

 * *Files identical despite different names*

### Comparing `super_rubik_cube-1.0.1/supercube/.move_cornperm` & `super_rubik_cube-1.0.2/supercube/.move_cornperm`

 * *Files identical despite different names*

### Comparing `super_rubik_cube-1.0.1/supercube/PocketCube.py` & `super_rubik_cube-1.0.2/supercube/PocketCube.py`

 * *Files identical despite different names*

### Comparing `super_rubik_cube-1.0.1/supercube/RubiksCube.py` & `super_rubik_cube-1.0.2/supercube/RubiksCube.py`

 * *Files identical despite different names*

### Comparing `super_rubik_cube-1.0.1/supercube/cube.py` & `super_rubik_cube-1.0.2/supercube/cube.py`

 * *Files identical despite different names*

### Comparing `super_rubik_cube-1.0.1/supercube/kociemba/__init__.py` & `super_rubik_cube-1.0.2/supercube/kociemba/__init__.py`

 * *Files identical despite different names*

### Comparing `super_rubik_cube-1.0.1/supercube/kociemba/build_ckociemba.py` & `super_rubik_cube-1.0.2/supercube/kociemba/build_ckociemba.py`

 * *Files identical despite different names*

### Comparing `super_rubik_cube-1.0.1/supercube/kociemba/pykociemba/coordcube.py` & `super_rubik_cube-1.0.2/supercube/kociemba/pykociemba/coordcube.py`

 * *Files identical despite different names*

### Comparing `super_rubik_cube-1.0.1/supercube/kociemba/pykociemba/corner.py` & `super_rubik_cube-1.0.2/supercube/kociemba/pykociemba/corner.py`

 * *Files identical despite different names*

### Comparing `super_rubik_cube-1.0.1/supercube/kociemba/pykociemba/cubiecube.py` & `super_rubik_cube-1.0.2/supercube/kociemba/pykociemba/cubiecube.py`

 * *Files identical despite different names*

### Comparing `super_rubik_cube-1.0.1/supercube/kociemba/pykociemba/edge.py` & `super_rubik_cube-1.0.2/supercube/kociemba/pykociemba/edge.py`

 * *Files identical despite different names*

### Comparing `super_rubik_cube-1.0.1/supercube/kociemba/pykociemba/facecube.py` & `super_rubik_cube-1.0.2/supercube/kociemba/pykociemba/facecube.py`

 * *Files identical despite different names*

### Comparing `super_rubik_cube-1.0.1/supercube/kociemba/pykociemba/facelet.py` & `super_rubik_cube-1.0.2/supercube/kociemba/pykociemba/facelet.py`

 * *Files identical despite different names*

### Comparing `super_rubik_cube-1.0.1/supercube/kociemba/pykociemba/prunetables/FRtoBR_Move.pkl` & `super_rubik_cube-1.0.2/supercube/kociemba/pykociemba/prunetables/FRtoBR_Move.pkl`

 * *Files identical despite different names*

### Comparing `super_rubik_cube-1.0.1/supercube/kociemba/pykociemba/prunetables/MergeURtoULandUBtoDF.pkl` & `super_rubik_cube-1.0.2/supercube/kociemba/pykociemba/prunetables/MergeURtoULandUBtoDF.pkl`

 * *Files identical despite different names*

### Comparing `super_rubik_cube-1.0.1/supercube/kociemba/pykociemba/prunetables/Slice_Flip_Prun.pkl` & `super_rubik_cube-1.0.2/supercube/kociemba/pykociemba/prunetables/Slice_Flip_Prun.pkl`

 * *Files identical despite different names*

### Comparing `super_rubik_cube-1.0.1/supercube/kociemba/pykociemba/prunetables/Slice_Twist_Prun.pkl` & `super_rubik_cube-1.0.2/supercube/kociemba/pykociemba/prunetables/Slice_Twist_Prun.pkl`

 * *Files identical despite different names*

### Comparing `super_rubik_cube-1.0.1/supercube/kociemba/pykociemba/prunetables/Slice_URFtoDLF_Parity_Prun.pkl` & `super_rubik_cube-1.0.2/supercube/kociemba/pykociemba/prunetables/Slice_URFtoDLF_Parity_Prun.pkl`

 * *Files identical despite different names*

### Comparing `super_rubik_cube-1.0.1/supercube/kociemba/pykociemba/prunetables/Slice_URtoDF_Parity_Prun.pkl` & `super_rubik_cube-1.0.2/supercube/kociemba/pykociemba/prunetables/Slice_URtoDF_Parity_Prun.pkl`

 * *Files identical despite different names*

### Comparing `super_rubik_cube-1.0.1/supercube/kociemba/pykociemba/prunetables/UBtoDF_Move.pkl` & `super_rubik_cube-1.0.2/supercube/kociemba/pykociemba/prunetables/UBtoDF_Move.pkl`

 * *Files identical despite different names*

### Comparing `super_rubik_cube-1.0.1/supercube/kociemba/pykociemba/prunetables/URFtoDLF_Move.pkl` & `super_rubik_cube-1.0.2/supercube/kociemba/pykociemba/prunetables/URFtoDLF_Move.pkl`

 * *Files identical despite different names*

### Comparing `super_rubik_cube-1.0.1/supercube/kociemba/pykociemba/prunetables/URtoDF_Move.pkl` & `super_rubik_cube-1.0.2/supercube/kociemba/pykociemba/prunetables/URtoDF_Move.pkl`

 * *Files identical despite different names*

### Comparing `super_rubik_cube-1.0.1/supercube/kociemba/pykociemba/prunetables/URtoUL_Move.pkl` & `super_rubik_cube-1.0.2/supercube/kociemba/pykociemba/prunetables/URtoUL_Move.pkl`

 * *Files identical despite different names*

### Comparing `super_rubik_cube-1.0.1/supercube/kociemba/pykociemba/prunetables/flipMove.pkl` & `super_rubik_cube-1.0.2/supercube/kociemba/pykociemba/prunetables/flipMove.pkl`

 * *Files identical despite different names*

### Comparing `super_rubik_cube-1.0.1/supercube/kociemba/pykociemba/prunetables/twistMove.pkl` & `super_rubik_cube-1.0.2/supercube/kociemba/pykociemba/prunetables/twistMove.pkl`

 * *Files identical despite different names*

### Comparing `super_rubik_cube-1.0.1/supercube/kociemba/pykociemba/search.py` & `super_rubik_cube-1.0.2/supercube/kociemba/pykociemba/search.py`

 * *Files identical despite different names*

### Comparing `super_rubik_cube-1.0.1/supercube/kociemba/pykociemba/tools.py` & `super_rubik_cube-1.0.2/supercube/kociemba/pykociemba/tools.py`

 * *Files identical despite different names*

### Comparing `super_rubik_cube-1.0.1/supercube/kociemba_2x2/client_gui.py` & `super_rubik_cube-1.0.2/supercube/kociemba_2x2/client_gui.py`

 * *Files identical despite different names*

### Comparing `super_rubik_cube-1.0.1/supercube/kociemba_2x2/coord.py` & `super_rubik_cube-1.0.2/supercube/kociemba_2x2/coord.py`

 * *Files identical despite different names*

### Comparing `super_rubik_cube-1.0.1/supercube/kociemba_2x2/cubie.py` & `super_rubik_cube-1.0.2/supercube/kociemba_2x2/cubie.py`

 * *Files identical despite different names*

### Comparing `super_rubik_cube-1.0.1/supercube/kociemba_2x2/defs.py` & `super_rubik_cube-1.0.2/supercube/kociemba_2x2/defs.py`

 * *Files identical despite different names*

### Comparing `super_rubik_cube-1.0.1/supercube/kociemba_2x2/enums.py` & `super_rubik_cube-1.0.2/supercube/kociemba_2x2/enums.py`

 * *Files identical despite different names*

### Comparing `super_rubik_cube-1.0.1/supercube/kociemba_2x2/example.py` & `super_rubik_cube-1.0.2/supercube/kociemba_2x2/example.py`

 * *Files identical despite different names*

### Comparing `super_rubik_cube-1.0.1/supercube/kociemba_2x2/face.py` & `super_rubik_cube-1.0.2/supercube/kociemba_2x2/face.py`

 * *Files identical despite different names*

### Comparing `super_rubik_cube-1.0.1/supercube/kociemba_2x2/moves.py` & `super_rubik_cube-1.0.2/supercube/kociemba_2x2/moves.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,28 +6,28 @@
 from supercube.kociemba_2x2 import enums
 from supercube.kociemba_2x2.defs import N_TWIST, N_CORNERS, N_MOVE
 
 a = cb.CubieCube()
 # ############################ Move table for the the corners. ##################################
 
 # The twist coordinate describes the 3^6 = 729 possible orientations of the 8 corners
-fname = "supercube/.move_corntwist"
+fname = ".move_corntwist"
 #print("creating " + fname + " table...")
 corntwist_move = ar.array('H', [0 for i in range(N_TWIST * N_MOVE)])
 for i in range(N_TWIST):
     a.set_cornertwist(i)
     for j in (enums.Color.U, enums.Color.R, enums.Color.F):  # three faces U, R, F
         for k in range(3):  # three moves for each face, for example U, U2, U3 = U'
             a.multiply(cb.basicMoveCube[j])
             corntwist_move[N_MOVE * i + 3 * j + k] = a.get_corntwist()
         a.multiply(cb.basicMoveCube[j])  # 4. move restores face
 
 
 # The corners coordinate describes the 7! = 5040 permutations of the corners.
-fname = "supercube/.move_cornperm"
+fname = ".move_cornperm"
 if not path.isfile(fname):
     #print("creating " + fname + " table...")
     cornperm_move = ar.array('H', [0 for i in range(N_CORNERS * N_MOVE)])
     # Move table for the corners. corner  < 40320
     for i in range(N_CORNERS):
         #if (i+1) % 200 == 0:
             #print('.', end='', flush=True)
```

### Comparing `super_rubik_cube-1.0.1/supercube/kociemba_2x2/pruning.py` & `super_rubik_cube-1.0.2/supercube/kociemba_2x2/pruning.py`

 * *Files 8% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 import array as ar
 
 corner_depth = None
 
 
 def create_cornerprun_table():
     """Creates/loads the corner pruning table."""
-    fname = "supercube/.cornerprun"
+    fname = ".cornerprun"
     global corner_depth
     if not path.isfile(fname):
         #print("creating " + fname + " table...")
         corner_depth = ar.array('b', [-1] * (defs.N_CORNERS * defs.N_TWIST))
         corners = 0  # values for solved cube
         twist = 0
         corner_depth[defs.N_TWIST * corners + twist] = 0
```

### Comparing `super_rubik_cube-1.0.1/supercube/kociemba_2x2/sockets.py` & `super_rubik_cube-1.0.2/supercube/kociemba_2x2/sockets.py`

 * *Files identical despite different names*

### Comparing `super_rubik_cube-1.0.1/supercube/kociemba_2x2/solver.py` & `super_rubik_cube-1.0.2/supercube/kociemba_2x2/solver.py`

 * *Files identical despite different names*

