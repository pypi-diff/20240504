# Comparing `tmp/ndispers-0.2.7.tar.gz` & `tmp/ndispers-0.2.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ndispers-0.2.7.tar", last modified: Sat Feb  4 11:14:56 2023, max compression
+gzip compressed data, was "ndispers-0.2.8.tar", last modified: Sat May  4 11:00:47 2024, max compression
```

## Comparing `ndispers-0.2.7.tar` & `ndispers-0.2.8.tar`

### file list

```diff
@@ -1,64 +1,64 @@
-drwxr-xr-x   0 shimura-akihiko (1850392416) 1166438733        0 2023-02-04 11:14:56.122742 ndispers-0.2.7/
--rw-r--r--   0 shimura-akihiko (1850392416) 1166438733       66 2021-12-18 09:42:00.000000 ndispers-0.2.7/.gitattributes
--rw-r--r--   0 shimura-akihiko (1850392416) 1166438733      762 2022-01-04 17:38:54.000000 ndispers-0.2.7/.gitignore
-drwxr-xr-x   0 shimura-akihiko (1850392416) 1166438733        0 2023-02-04 11:14:56.077093 ndispers-0.2.7/.vscode/
--rw-r--r--   0 shimura-akihiko (1850392416) 1166438733       72 2022-05-21 10:02:47.000000 ndispers-0.2.7/.vscode/settings.json
--rw-r--r--   0 shimura-akihiko (1850392416) 1166438733     1072 2021-12-18 09:42:00.000000 ndispers-0.2.7/LICENSE
--rw-r--r--   0 shimura-akihiko (1850392416) 1166438733     3441 2023-02-04 11:14:56.122535 ndispers-0.2.7/PKG-INFO
--rw-r--r--   0 shimura-akihiko (1850392416) 1166438733     2813 2022-10-11 13:44:03.000000 ndispers-0.2.7/README.md
-drwxr-xr-x   0 shimura-akihiko (1850392416) 1166438733        0 2023-02-04 11:14:56.077574 ndispers-0.2.7/docs/
--rw-r--r--   0 shimura-akihiko (1850392416) 1166438733      638 2022-01-04 16:35:21.000000 ndispers-0.2.7/docs/Makefile
--rw-r--r--   0 shimura-akihiko (1850392416) 1166438733      804 2022-01-04 16:35:21.000000 ndispers-0.2.7/docs/make.bat
-drwxr-xr-x   0 shimura-akihiko (1850392416) 1166438733        0 2023-02-04 11:14:56.078107 ndispers-0.2.7/docs/source/
--rw-r--r--   0 shimura-akihiko (1850392416) 1166438733      712 2022-05-22 08:55:24.000000 ndispers-0.2.7/docs/source/conf.py
--rw-r--r--   0 shimura-akihiko (1850392416) 1166438733     2657 2022-05-22 07:49:10.000000 ndispers-0.2.7/docs/source/index.rst
-drwxr-xr-x   0 shimura-akihiko (1850392416) 1166438733        0 2023-02-04 11:14:56.078917 ndispers-0.2.7/docs/source/intro/
--rw-r--r--   0 shimura-akihiko (1850392416) 1166438733       42 2022-05-22 09:24:25.000000 ndispers-0.2.7/docs/source/intro/basic.rst
--rw-r--r--   0 shimura-akihiko (1850392416) 1166438733      159 2022-05-22 14:47:33.000000 ndispers-0.2.7/docs/source/intro/index.rst
--rw-r--r--   0 shimura-akihiko (1850392416) 1166438733     1493 2022-05-23 06:54:49.000000 ndispers-0.2.7/docs/source/intro/install.rst
-drwxr-xr-x   0 shimura-akihiko (1850392416) 1166438733        0 2023-02-04 11:14:56.079765 ndispers-0.2.7/ndispers/
--rw-r--r--   0 shimura-akihiko (1850392416) 1166438733       85 2021-12-18 09:42:00.000000 ndispers-0.2.7/ndispers/__init__.py
--rw-r--r--   0 shimura-akihiko (1850392416) 1166438733    10489 2022-10-10 15:41:09.000000 ndispers-0.2.7/ndispers/_baseclass.py
-drwxr-xr-x   0 shimura-akihiko (1850392416) 1166438733        0 2023-02-04 11:14:56.113178 ndispers-0.2.7/ndispers/groups/
--rw-r--r--   0 shimura-akihiko (1850392416) 1166438733      168 2022-10-24 12:23:10.000000 ndispers-0.2.7/ndispers/groups/__init__.py
--rw-r--r--   0 shimura-akihiko (1850392416) 1166438733     6104 2022-10-24 15:14:13.000000 ndispers-0.2.7/ndispers/groups/_uniax_neg_32.py
--rw-r--r--   0 shimura-akihiko (1850392416) 1166438733     6629 2022-10-24 15:11:13.000000 ndispers-0.2.7/ndispers/groups/_uniax_neg_3m.py
--rw-r--r--   0 shimura-akihiko (1850392416) 1166438733      839 2021-12-18 09:42:00.000000 ndispers-0.2.7/ndispers/helper.py
-drwxr-xr-x   0 shimura-akihiko (1850392416) 1166438733        0 2023-02-04 11:14:56.113517 ndispers-0.2.7/ndispers/media/
--rw-r--r--   0 shimura-akihiko (1850392416) 1166438733      128 2022-10-10 15:38:25.000000 ndispers-0.2.7/ndispers/media/__init__.py
-drwxr-xr-x   0 shimura-akihiko (1850392416) 1166438733        0 2023-02-04 11:14:56.120371 ndispers-0.2.7/ndispers/media/crystals/
--rw-r--r--   0 shimura-akihiko (1850392416) 1166438733     6007 2022-10-24 12:12:13.000000 ndispers-0.2.7/ndispers/media/crystals/_CLBO.py
--rw-r--r--   0 shimura-akihiko (1850392416) 1166438733     6877 2022-10-24 12:28:22.000000 ndispers-0.2.7/ndispers/media/crystals/_KBBF_Li2016.py
--rw-r--r--   0 shimura-akihiko (1850392416) 1166438733     4903 2022-10-24 12:12:13.000000 ndispers-0.2.7/ndispers/media/crystals/_KDP.py
--rw-r--r--   0 shimura-akihiko (1850392416) 1166438733    14630 2022-10-24 12:12:13.000000 ndispers-0.2.7/ndispers/media/crystals/_KTP.py
--rw-r--r--   0 shimura-akihiko (1850392416) 1166438733     6368 2022-10-24 12:12:13.000000 ndispers-0.2.7/ndispers/media/crystals/_LB4.py
--rw-r--r--   0 shimura-akihiko (1850392416) 1166438733    15288 2022-10-24 12:12:13.000000 ndispers-0.2.7/ndispers/media/crystals/_LBO_Castech.py
--rw-r--r--   0 shimura-akihiko (1850392416) 1166438733    15416 2022-10-24 12:12:13.000000 ndispers-0.2.7/ndispers/media/crystals/_LBO_EKSMA.py
--rw-r--r--   0 shimura-akihiko (1850392416) 1166438733    16071 2022-10-24 12:12:13.000000 ndispers-0.2.7/ndispers/media/crystals/_LBO_Ghosh1995.py
--rw-r--r--   0 shimura-akihiko (1850392416) 1166438733    15864 2022-10-24 12:11:56.000000 ndispers-0.2.7/ndispers/media/crystals/_LBO_KK1994.py
--rw-r--r--   0 shimura-akihiko (1850392416) 1166438733    15670 2022-10-24 12:12:13.000000 ndispers-0.2.7/ndispers/media/crystals/_LBO_KK2018.py
--rw-r--r--   0 shimura-akihiko (1850392416) 1166438733    15314 2022-10-24 12:12:13.000000 ndispers-0.2.7/ndispers/media/crystals/_LBO_Newlight.py
--rw-r--r--   0 shimura-akihiko (1850392416) 1166438733     6191 2022-10-19 11:16:59.000000 ndispers-0.2.7/ndispers/media/crystals/_SLN_MgO_doped_1pc.py
--rw-r--r--   0 shimura-akihiko (1850392416) 1166438733     1083 2022-10-24 12:14:54.000000 ndispers-0.2.7/ndispers/media/crystals/__init__.py
--rw-r--r--   0 shimura-akihiko (1850392416) 1166438733     4660 2022-10-19 11:16:59.000000 ndispers-0.2.7/ndispers/media/crystals/_alphaBBO.py
--rw-r--r--   0 shimura-akihiko (1850392416) 1166438733     6677 2022-10-24 12:12:13.000000 ndispers-0.2.7/ndispers/media/crystals/_betaBBO_Eimerl1987.py
--rw-r--r--   0 shimura-akihiko (1850392416) 1166438733     7505 2022-10-24 12:12:13.000000 ndispers-0.2.7/ndispers/media/crystals/_betaBBO_Ghosh1995.py
--rw-r--r--   0 shimura-akihiko (1850392416) 1166438733     7906 2022-10-24 12:12:13.000000 ndispers-0.2.7/ndispers/media/crystals/_betaBBO_KK2010.py
--rw-r--r--   0 shimura-akihiko (1850392416) 1166438733     7778 2022-10-24 12:12:13.000000 ndispers-0.2.7/ndispers/media/crystals/_betaBBO_Tamosauskas2018.py
--rw-r--r--   0 shimura-akihiko (1850392416) 1166438733     5554 2022-10-24 12:12:13.000000 ndispers-0.2.7/ndispers/media/crystals/_calcite.py
-drwxr-xr-x   0 shimura-akihiko (1850392416) 1166438733        0 2023-02-04 11:14:56.121444 ndispers-0.2.7/ndispers/media/glasses/
--rw-r--r--   0 shimura-akihiko (1850392416) 1166438733      134 2021-12-18 09:42:00.000000 ndispers-0.2.7/ndispers/media/glasses/__init__.py
--rw-r--r--   0 shimura-akihiko (1850392416) 1166438733     3157 2022-05-05 14:54:55.000000 ndispers-0.2.7/ndispers/media/glasses/_caf2.py
--rw-r--r--   0 shimura-akihiko (1850392416) 1166438733     3342 2022-05-05 14:45:43.000000 ndispers-0.2.7/ndispers/media/glasses/_fusedsilica.py
-drwxr-xr-x   0 shimura-akihiko (1850392416) 1166438733        0 2023-02-04 11:14:56.122134 ndispers-0.2.7/ndispers/tests/
--rw-r--r--   0 shimura-akihiko (1850392416) 1166438733     2206 2022-05-22 15:07:53.000000 ndispers-0.2.7/ndispers/tests/test_LBO.py
--rw-r--r--   0 shimura-akihiko (1850392416) 1166438733     1953 2022-05-22 15:07:55.000000 ndispers-0.2.7/ndispers/tests/test_betaBBO.py
-drwxr-xr-x   0 shimura-akihiko (1850392416) 1166438733        0 2023-02-04 11:14:56.112164 ndispers-0.2.7/ndispers.egg-info/
--rw-r--r--   0 shimura-akihiko (1850392416) 1166438733     3441 2023-02-04 11:14:55.000000 ndispers-0.2.7/ndispers.egg-info/PKG-INFO
--rw-r--r--   0 shimura-akihiko (1850392416) 1166438733     1503 2023-02-04 11:14:56.000000 ndispers-0.2.7/ndispers.egg-info/SOURCES.txt
--rw-r--r--   0 shimura-akihiko (1850392416) 1166438733        1 2023-02-04 11:14:55.000000 ndispers-0.2.7/ndispers.egg-info/dependency_links.txt
--rw-r--r--   0 shimura-akihiko (1850392416) 1166438733       25 2023-02-04 11:14:55.000000 ndispers-0.2.7/ndispers.egg-info/requires.txt
--rw-r--r--   0 shimura-akihiko (1850392416) 1166438733        9 2023-02-04 11:14:55.000000 ndispers-0.2.7/ndispers.egg-info/top_level.txt
--rw-rw-r--   0 shimura-akihiko (1850392416) 1166438733      219 2022-01-04 17:49:31.000000 ndispers-0.2.7/pyproject.toml
--rw-r--r--   0 shimura-akihiko (1850392416) 1166438733       38 2023-02-04 11:14:56.122803 ndispers-0.2.7/setup.cfg
--rw-r--r--   0 shimura-akihiko (1850392416) 1166438733      987 2023-02-04 11:14:35.000000 ndispers-0.2.7/setup.py
+drwxr-xr-x   0 shimura-akihiko (1850392416) 1166438733        0 2024-05-04 11:00:47.128442 ndispers-0.2.8/
+-rw-r--r--   0 shimura-akihiko (1850392416) 1166438733       66 2021-12-18 09:42:00.000000 ndispers-0.2.8/.gitattributes
+-rw-r--r--   0 shimura-akihiko (1850392416) 1166438733      762 2022-01-04 17:38:54.000000 ndispers-0.2.8/.gitignore
+drwxr-xr-x   0 shimura-akihiko (1850392416) 1166438733        0 2024-05-04 11:00:47.083011 ndispers-0.2.8/.vscode/
+-rw-r--r--   0 shimura-akihiko (1850392416) 1166438733       72 2022-05-21 10:02:47.000000 ndispers-0.2.8/.vscode/settings.json
+-rw-r--r--   0 shimura-akihiko (1850392416) 1166438733     1072 2021-12-18 09:42:00.000000 ndispers-0.2.8/LICENSE
+-rw-r--r--   0 shimura-akihiko (1850392416) 1166438733     3865 2024-05-04 11:00:47.128260 ndispers-0.2.8/PKG-INFO
+-rw-r--r--   0 shimura-akihiko (1850392416) 1166438733     3116 2024-05-04 10:26:36.000000 ndispers-0.2.8/README.md
+drwxr-xr-x   0 shimura-akihiko (1850392416) 1166438733        0 2024-05-04 11:00:47.083629 ndispers-0.2.8/docs/
+-rw-r--r--   0 shimura-akihiko (1850392416) 1166438733      638 2022-01-04 16:35:21.000000 ndispers-0.2.8/docs/Makefile
+-rw-r--r--   0 shimura-akihiko (1850392416) 1166438733      804 2024-05-04 11:00:20.000000 ndispers-0.2.8/docs/make.bat
+drwxr-xr-x   0 shimura-akihiko (1850392416) 1166438733        0 2024-05-04 11:00:47.084329 ndispers-0.2.8/docs/source/
+-rw-r--r--   0 shimura-akihiko (1850392416) 1166438733      712 2023-08-16 16:05:32.000000 ndispers-0.2.8/docs/source/conf.py
+-rw-r--r--   0 shimura-akihiko (1850392416) 1166438733     2657 2022-05-22 07:49:10.000000 ndispers-0.2.8/docs/source/index.rst
+drwxr-xr-x   0 shimura-akihiko (1850392416) 1166438733        0 2024-05-04 11:00:47.085572 ndispers-0.2.8/docs/source/intro/
+-rw-r--r--   0 shimura-akihiko (1850392416) 1166438733       42 2022-05-22 09:24:25.000000 ndispers-0.2.8/docs/source/intro/basic.rst
+-rw-r--r--   0 shimura-akihiko (1850392416) 1166438733      159 2022-05-22 14:47:33.000000 ndispers-0.2.8/docs/source/intro/index.rst
+-rw-r--r--   0 shimura-akihiko (1850392416) 1166438733     1493 2022-05-23 06:54:49.000000 ndispers-0.2.8/docs/source/intro/install.rst
+drwxr-xr-x   0 shimura-akihiko (1850392416) 1166438733        0 2024-05-04 11:00:47.086799 ndispers-0.2.8/ndispers/
+-rw-r--r--   0 shimura-akihiko (1850392416) 1166438733       85 2021-12-18 09:42:00.000000 ndispers-0.2.8/ndispers/__init__.py
+-rw-r--r--   0 shimura-akihiko (1850392416) 1166438733    10488 2023-02-04 11:55:16.000000 ndispers-0.2.8/ndispers/_baseclass.py
+drwxr-xr-x   0 shimura-akihiko (1850392416) 1166438733        0 2024-05-04 11:00:47.104662 ndispers-0.2.8/ndispers/groups/
+-rw-r--r--   0 shimura-akihiko (1850392416) 1166438733      168 2022-10-24 12:23:10.000000 ndispers-0.2.8/ndispers/groups/__init__.py
+-rw-r--r--   0 shimura-akihiko (1850392416) 1166438733     6104 2022-10-24 15:14:13.000000 ndispers-0.2.8/ndispers/groups/_uniax_neg_32.py
+-rw-r--r--   0 shimura-akihiko (1850392416) 1166438733     6629 2022-10-24 15:11:13.000000 ndispers-0.2.8/ndispers/groups/_uniax_neg_3m.py
+-rw-r--r--   0 shimura-akihiko (1850392416) 1166438733      839 2021-12-18 09:42:00.000000 ndispers-0.2.8/ndispers/helper.py
+drwxr-xr-x   0 shimura-akihiko (1850392416) 1166438733        0 2024-05-04 11:00:47.104983 ndispers-0.2.8/ndispers/media/
+-rw-r--r--   0 shimura-akihiko (1850392416) 1166438733      128 2022-10-10 15:38:25.000000 ndispers-0.2.8/ndispers/media/__init__.py
+drwxr-xr-x   0 shimura-akihiko (1850392416) 1166438733        0 2024-05-04 11:00:47.125139 ndispers-0.2.8/ndispers/media/crystals/
+-rw-r--r--   0 shimura-akihiko (1850392416) 1166438733     6007 2022-10-24 12:12:13.000000 ndispers-0.2.8/ndispers/media/crystals/_CLBO.py
+-rw-r--r--   0 shimura-akihiko (1850392416) 1166438733     6877 2022-10-24 12:28:22.000000 ndispers-0.2.8/ndispers/media/crystals/_KBBF_Li2016.py
+-rw-r--r--   0 shimura-akihiko (1850392416) 1166438733     4903 2022-10-24 12:12:13.000000 ndispers-0.2.8/ndispers/media/crystals/_KDP.py
+-rw-r--r--   0 shimura-akihiko (1850392416) 1166438733    14630 2022-10-24 12:12:13.000000 ndispers-0.2.8/ndispers/media/crystals/_KTP.py
+-rw-r--r--   0 shimura-akihiko (1850392416) 1166438733     6368 2022-10-24 12:12:13.000000 ndispers-0.2.8/ndispers/media/crystals/_LB4.py
+-rw-r--r--   0 shimura-akihiko (1850392416) 1166438733    15288 2022-10-24 12:12:13.000000 ndispers-0.2.8/ndispers/media/crystals/_LBO_Castech.py
+-rw-r--r--   0 shimura-akihiko (1850392416) 1166438733    15416 2022-10-24 12:12:13.000000 ndispers-0.2.8/ndispers/media/crystals/_LBO_EKSMA.py
+-rw-r--r--   0 shimura-akihiko (1850392416) 1166438733    16071 2022-10-24 12:12:13.000000 ndispers-0.2.8/ndispers/media/crystals/_LBO_Ghosh1995.py
+-rw-r--r--   0 shimura-akihiko (1850392416) 1166438733    15864 2022-10-24 12:11:56.000000 ndispers-0.2.8/ndispers/media/crystals/_LBO_KK1994.py
+-rw-r--r--   0 shimura-akihiko (1850392416) 1166438733    15670 2022-10-24 12:12:13.000000 ndispers-0.2.8/ndispers/media/crystals/_LBO_KK2018.py
+-rw-r--r--   0 shimura-akihiko (1850392416) 1166438733    15314 2022-10-24 12:12:13.000000 ndispers-0.2.8/ndispers/media/crystals/_LBO_Newlight.py
+-rw-r--r--   0 shimura-akihiko (1850392416) 1166438733     6191 2022-10-19 11:16:59.000000 ndispers-0.2.8/ndispers/media/crystals/_SLN_MgO_doped_1pc.py
+-rw-r--r--   0 shimura-akihiko (1850392416) 1166438733     1083 2022-10-24 12:14:54.000000 ndispers-0.2.8/ndispers/media/crystals/__init__.py
+-rw-r--r--   0 shimura-akihiko (1850392416) 1166438733     4660 2022-10-19 11:16:59.000000 ndispers-0.2.8/ndispers/media/crystals/_alphaBBO.py
+-rw-r--r--   0 shimura-akihiko (1850392416) 1166438733     6677 2022-10-24 12:12:13.000000 ndispers-0.2.8/ndispers/media/crystals/_betaBBO_Eimerl1987.py
+-rw-r--r--   0 shimura-akihiko (1850392416) 1166438733     7505 2022-10-24 12:12:13.000000 ndispers-0.2.8/ndispers/media/crystals/_betaBBO_Ghosh1995.py
+-rw-r--r--   0 shimura-akihiko (1850392416) 1166438733     7906 2022-10-24 12:12:13.000000 ndispers-0.2.8/ndispers/media/crystals/_betaBBO_KK2010.py
+-rw-r--r--   0 shimura-akihiko (1850392416) 1166438733     7778 2022-10-24 12:12:13.000000 ndispers-0.2.8/ndispers/media/crystals/_betaBBO_Tamosauskas2018.py
+-rw-r--r--   0 shimura-akihiko (1850392416) 1166438733     5554 2022-10-24 12:12:13.000000 ndispers-0.2.8/ndispers/media/crystals/_calcite.py
+drwxr-xr-x   0 shimura-akihiko (1850392416) 1166438733        0 2024-05-04 11:00:47.126938 ndispers-0.2.8/ndispers/media/glasses/
+-rw-r--r--   0 shimura-akihiko (1850392416) 1166438733      134 2021-12-18 09:42:00.000000 ndispers-0.2.8/ndispers/media/glasses/__init__.py
+-rw-r--r--   0 shimura-akihiko (1850392416) 1166438733     3157 2022-05-05 14:54:55.000000 ndispers-0.2.8/ndispers/media/glasses/_caf2.py
+-rw-r--r--   0 shimura-akihiko (1850392416) 1166438733     3342 2022-05-05 14:45:43.000000 ndispers-0.2.8/ndispers/media/glasses/_fusedsilica.py
+drwxr-xr-x   0 shimura-akihiko (1850392416) 1166438733        0 2024-05-04 11:00:47.127869 ndispers-0.2.8/ndispers/tests/
+-rw-r--r--   0 shimura-akihiko (1850392416) 1166438733     2206 2022-05-22 15:07:53.000000 ndispers-0.2.8/ndispers/tests/test_LBO.py
+-rw-r--r--   0 shimura-akihiko (1850392416) 1166438733     1953 2022-05-22 15:07:55.000000 ndispers-0.2.8/ndispers/tests/test_betaBBO.py
+drwxr-xr-x   0 shimura-akihiko (1850392416) 1166438733        0 2024-05-04 11:00:47.103712 ndispers-0.2.8/ndispers.egg-info/
+-rw-r--r--   0 shimura-akihiko (1850392416) 1166438733     3865 2024-05-04 11:00:46.000000 ndispers-0.2.8/ndispers.egg-info/PKG-INFO
+-rw-r--r--   0 shimura-akihiko (1850392416) 1166438733     1503 2024-05-04 11:00:46.000000 ndispers-0.2.8/ndispers.egg-info/SOURCES.txt
+-rw-r--r--   0 shimura-akihiko (1850392416) 1166438733        1 2024-05-04 11:00:46.000000 ndispers-0.2.8/ndispers.egg-info/dependency_links.txt
+-rw-r--r--   0 shimura-akihiko (1850392416) 1166438733       25 2024-05-04 11:00:46.000000 ndispers-0.2.8/ndispers.egg-info/requires.txt
+-rw-r--r--   0 shimura-akihiko (1850392416) 1166438733        9 2024-05-04 11:00:46.000000 ndispers-0.2.8/ndispers.egg-info/top_level.txt
+-rw-rw-r--   0 shimura-akihiko (1850392416) 1166438733      229 2024-05-04 10:43:19.000000 ndispers-0.2.8/pyproject.toml
+-rw-r--r--   0 shimura-akihiko (1850392416) 1166438733       38 2024-05-04 11:00:47.128496 ndispers-0.2.8/setup.cfg
+-rw-r--r--   0 shimura-akihiko (1850392416) 1166438733     1088 2024-05-04 10:59:45.000000 ndispers-0.2.8/setup.py
```

### Comparing `ndispers-0.2.7/.gitignore` & `ndispers-0.2.8/.gitignore`

 * *Files identical despite different names*

### Comparing `ndispers-0.2.7/LICENSE` & `ndispers-0.2.8/LICENSE`

 * *Files identical despite different names*

### Comparing `ndispers-0.2.7/PKG-INFO` & `ndispers-0.2.8/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -1,41 +1,34 @@
-Metadata-Version: 2.1
-Name: ndispers
-Version: 0.2.7
-Summary: Python package for calculating refractive index dispersion of various materials
-Home-page: https://github.com/akihiko-shimura/ndispers
-Author: Akihiko Shimura
-Author-email: akihiko-shimura <akhksh@gmail.com>
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Operating System :: OS Independent
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # ndispers
 *ndispers* is a Python package for calculating refractive index dispersion of various crystals and glasses used in the field of nonlinear/ultrafast optics. It is based on Sellmeier equartions and thermo-optic coefficients (dn/dT) reported in literature.
 
 You can easily compute
 - Refractive index
 - Group delay
 - Group velocity
 - Group index
 - Group velocity dispersion
 - Third-order dispersion
 - Walk-off angles
+- dn/dT
+- d^2n/dT^2
 
 as a function of
 1. Wavelength of light
 2. Polar (theta) or azimuthal (phi) angles of wavevector with respect to dielectric principal axes of anisotropic crystals
 3. Temperature of crystal
 4. Polarization of light (ordinary- or extraordinary-ray)
 
+The crystals have nonlinear-optics methods:
+- Phase-mismacth, dk
+- Phase-matching angles
+- Phase-mathcing factor, sinc^2(dk*L/2)
+- Effective nonlinear coefficient, deff
+
+In the latest version v0.2.7, these methods are only for sum-frequency mixing, and deff method only for BetaBBO.
 
 ## Installation
 
 In terminal,
 ```zsh
 pip install ndispers
 ```
```

### Comparing `ndispers-0.2.7/docs/Makefile` & `ndispers-0.2.8/docs/Makefile`

 * *Files identical despite different names*

### Comparing `ndispers-0.2.7/docs/make.bat` & `ndispers-0.2.8/docs/make.bat`

 * *Files identical despite different names*

### Comparing `ndispers-0.2.7/docs/source/conf.py` & `ndispers-0.2.8/docs/source/conf.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 # -- Project information
 
 project = 'ndispers'
 copyright = '2022, akihiko-shimura'
 author = ''
 
 release = '0.2'
-version = '0.2.5'
+version = '0.2.6'
 
 # -- General configuration
 
 extensions = [
     'sphinx.ext.duration',
     'sphinx.ext.doctest',
     'sphinx.ext.autodoc',
```

### Comparing `ndispers-0.2.7/docs/source/index.rst` & `ndispers-0.2.8/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `ndispers-0.2.7/docs/source/intro/install.rst` & `ndispers-0.2.8/docs/source/intro/install.rst`

 * *Files identical despite different names*

### Comparing `ndispers-0.2.7/ndispers/_baseclass.py` & `ndispers-0.2.8/ndispers/_baseclass.py`

 * *Files 0% similar despite different names*

```diff
@@ -265,15 +265,15 @@
         d['eoe'] = pmAngle_for_pol('e', 'o', 'e') #nega2
         d['eoo'] = pmAngle_for_pol('e', 'o', 'o') #posi1
         d['oeo'] = pmAngle_for_pol('o', 'e', 'o') #posi2
         return d
 
     def pmFactor_sfg(self, wl1, wl2, angle_rad, T_degC, pol1, pol2, pol3, L_mm):
         """
-        Phase-matching factor, sinc^2((0.5*dk*L)/(0.5*dk*L)), for sum-frequency generation (SFG).
+        Phase-matching factor, sin^2((0.5*dk*L)/(0.5*dk*L)), for sum-frequency generation (SFG).
 
         Parameters
         ----------
         wl1 : float or array_like
             1st pump wavelength in µm.
         wl2 : float or array_like
             2nd pump wavelength in µm.
```

### Comparing `ndispers-0.2.7/ndispers/groups/_uniax_neg_32.py` & `ndispers-0.2.8/ndispers/groups/_uniax_neg_32.py`

 * *Files identical despite different names*

### Comparing `ndispers-0.2.7/ndispers/groups/_uniax_neg_3m.py` & `ndispers-0.2.8/ndispers/groups/_uniax_neg_3m.py`

 * *Files identical despite different names*

### Comparing `ndispers-0.2.7/ndispers/helper.py` & `ndispers-0.2.8/ndispers/helper.py`

 * *Files identical despite different names*

### Comparing `ndispers-0.2.7/ndispers/media/crystals/_CLBO.py` & `ndispers-0.2.8/ndispers/media/crystals/_CLBO.py`

 * *Files identical despite different names*

### Comparing `ndispers-0.2.7/ndispers/media/crystals/_KBBF_Li2016.py` & `ndispers-0.2.8/ndispers/media/crystals/_KBBF_Li2016.py`

 * *Files identical despite different names*

### Comparing `ndispers-0.2.7/ndispers/media/crystals/_KDP.py` & `ndispers-0.2.8/ndispers/media/crystals/_KDP.py`

 * *Files identical despite different names*

### Comparing `ndispers-0.2.7/ndispers/media/crystals/_KTP.py` & `ndispers-0.2.8/ndispers/media/crystals/_KTP.py`

 * *Files identical despite different names*

### Comparing `ndispers-0.2.7/ndispers/media/crystals/_LB4.py` & `ndispers-0.2.8/ndispers/media/crystals/_LB4.py`

 * *Files identical despite different names*

### Comparing `ndispers-0.2.7/ndispers/media/crystals/_LBO_Castech.py` & `ndispers-0.2.8/ndispers/media/crystals/_LBO_Castech.py`

 * *Files identical despite different names*

### Comparing `ndispers-0.2.7/ndispers/media/crystals/_LBO_EKSMA.py` & `ndispers-0.2.8/ndispers/media/crystals/_LBO_EKSMA.py`

 * *Files identical despite different names*

### Comparing `ndispers-0.2.7/ndispers/media/crystals/_LBO_Ghosh1995.py` & `ndispers-0.2.8/ndispers/media/crystals/_LBO_Ghosh1995.py`

 * *Files identical despite different names*

### Comparing `ndispers-0.2.7/ndispers/media/crystals/_LBO_KK1994.py` & `ndispers-0.2.8/ndispers/media/crystals/_LBO_KK1994.py`

 * *Files identical despite different names*

### Comparing `ndispers-0.2.7/ndispers/media/crystals/_LBO_KK2018.py` & `ndispers-0.2.8/ndispers/media/crystals/_LBO_KK2018.py`

 * *Files identical despite different names*

### Comparing `ndispers-0.2.7/ndispers/media/crystals/_LBO_Newlight.py` & `ndispers-0.2.8/ndispers/media/crystals/_LBO_Newlight.py`

 * *Files identical despite different names*

### Comparing `ndispers-0.2.7/ndispers/media/crystals/_SLN_MgO_doped_1pc.py` & `ndispers-0.2.8/ndispers/media/crystals/_SLN_MgO_doped_1pc.py`

 * *Files identical despite different names*

### Comparing `ndispers-0.2.7/ndispers/media/crystals/__init__.py` & `ndispers-0.2.8/ndispers/media/crystals/__init__.py`

 * *Files identical despite different names*

### Comparing `ndispers-0.2.7/ndispers/media/crystals/_alphaBBO.py` & `ndispers-0.2.8/ndispers/media/crystals/_alphaBBO.py`

 * *Files identical despite different names*

### Comparing `ndispers-0.2.7/ndispers/media/crystals/_betaBBO_Eimerl1987.py` & `ndispers-0.2.8/ndispers/media/crystals/_betaBBO_Eimerl1987.py`

 * *Files identical despite different names*

### Comparing `ndispers-0.2.7/ndispers/media/crystals/_betaBBO_Ghosh1995.py` & `ndispers-0.2.8/ndispers/media/crystals/_betaBBO_Ghosh1995.py`

 * *Files identical despite different names*

### Comparing `ndispers-0.2.7/ndispers/media/crystals/_betaBBO_KK2010.py` & `ndispers-0.2.8/ndispers/media/crystals/_betaBBO_KK2010.py`

 * *Files identical despite different names*

### Comparing `ndispers-0.2.7/ndispers/media/crystals/_betaBBO_Tamosauskas2018.py` & `ndispers-0.2.8/ndispers/media/crystals/_betaBBO_Tamosauskas2018.py`

 * *Files identical despite different names*

### Comparing `ndispers-0.2.7/ndispers/media/crystals/_calcite.py` & `ndispers-0.2.8/ndispers/media/crystals/_calcite.py`

 * *Files identical despite different names*

### Comparing `ndispers-0.2.7/ndispers/media/glasses/_caf2.py` & `ndispers-0.2.8/ndispers/media/glasses/_caf2.py`

 * *Files identical despite different names*

### Comparing `ndispers-0.2.7/ndispers/media/glasses/_fusedsilica.py` & `ndispers-0.2.8/ndispers/media/glasses/_fusedsilica.py`

 * *Files identical despite different names*

### Comparing `ndispers-0.2.7/ndispers/tests/test_LBO.py` & `ndispers-0.2.8/ndispers/tests/test_LBO.py`

 * *Files identical despite different names*

### Comparing `ndispers-0.2.7/ndispers/tests/test_betaBBO.py` & `ndispers-0.2.8/ndispers/tests/test_betaBBO.py`

 * *Files identical despite different names*

### Comparing `ndispers-0.2.7/ndispers.egg-info/PKG-INFO` & `ndispers-0.2.8/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,19 +1,23 @@
 Metadata-Version: 2.1
 Name: ndispers
-Version: 0.2.7
+Version: 0.2.8
 Summary: Python package for calculating refractive index dispersion of various materials
 Home-page: https://github.com/akihiko-shimura/ndispers
 Author: Akihiko Shimura
-Author-email: akihiko-shimura <akhksh@gmail.com>
+Author-email: akhksh@gmail.com
+License: UNKNOWN
+Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # ndispers
 *ndispers* is a Python package for calculating refractive index dispersion of various crystals and glasses used in the field of nonlinear/ultrafast optics. It is based on Sellmeier equartions and thermo-optic coefficients (dn/dT) reported in literature.
 
@@ -21,21 +25,30 @@
 - Refractive index
 - Group delay
 - Group velocity
 - Group index
 - Group velocity dispersion
 - Third-order dispersion
 - Walk-off angles
+- dn/dT
+- d^2n/dT^2
 
 as a function of
 1. Wavelength of light
 2. Polar (theta) or azimuthal (phi) angles of wavevector with respect to dielectric principal axes of anisotropic crystals
 3. Temperature of crystal
 4. Polarization of light (ordinary- or extraordinary-ray)
 
+The crystals have nonlinear-optics methods:
+- Phase-mismacth, dk
+- Phase-matching angles
+- Phase-mathcing factor, sinc^2(dk*L/2)
+- Effective nonlinear coefficient, deff
+
+In the latest version v0.2.7, these methods are only for sum-frequency mixing, and deff method only for BetaBBO.
 
 ## Installation
 
 In terminal,
 ```zsh
 pip install ndispers
 ```
@@ -104,7 +117,9 @@
 >>> wl_ar
 array([0.2, 0.4, 0.6, 0.8, 1. , 1.2, 1.4])
 >>> bbo.n(wl_ar, 0, 25, pol='o')
 array([1.89625189, 1.692713, 1.66892613, 1.66039556, 1.65560236, 1.65199986, 1.64874414])
 ```
 
 See [documentation](https://ndispers.readthedocs.io/en/latest/) for more features and examples.
+
+
```

### Comparing `ndispers-0.2.7/ndispers.egg-info/SOURCES.txt` & `ndispers-0.2.8/ndispers.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ndispers-0.2.7/setup.py` & `ndispers-0.2.8/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,16 +1,17 @@
-from setuptools import setup, find_packages
 from codecs import open
 
+from setuptools import find_packages, setup
+
 with open('README.md', encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name="ndispers",
-    version='0.2.7',
+    version='0.2.8',
     packages=find_packages(),
 
     author='Akihiko Shimura',
     author_email='akhksh@gmail.com',
     url='https://github.com/akihiko-shimura/ndispers',
     description='Python package for calculating refractive index dispersion of various materials',
     long_description=long_description,
@@ -23,10 +24,12 @@
 
     classifiers=[
         'License :: OSI Approved :: MIT License',
         'Programming Language :: Python :: 3',
         'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3.9',
+        'Programming Language :: Python :: 3.10',
+        'Programming Language :: Python :: 3.11',
         'Operating System :: OS Independent',
     ],
 )
```

