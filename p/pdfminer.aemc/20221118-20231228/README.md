# Comparing `tmp/pdfminer.aemc-20221118.tar.gz` & `tmp/pdfminer_aemc-20231228.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pdfminer.aemc-20221118.tar", last modified: Tue Apr  2 11:28:22 2024, max compression
+gzip compressed data, was "pdfminer_aemc-20231228.tar", last modified: Sat May  4 04:32:45 2024, max compression
```

## Comparing `pdfminer.aemc-20221118.tar` & `pdfminer_aemc-20231228.tar`

### file list

```diff
@@ -1,214 +1,230 @@
-drwxr-xr-x   0 jun        (501) staff       (20)        0 2024-04-02 11:28:22.581486 pdfminer.aemc-20221118/
--rw-rw-r--   0 jun        (501) staff       (20)    14906 2022-11-05 16:22:08.000000 pdfminer.aemc-20221118/CHANGELOG.md
--rw-rw-r--   0 jun        (501) staff       (20)     2397 2022-11-05 16:22:08.000000 pdfminer.aemc-20221118/CONTRIBUTING.md
--rw-rw-r--   0 jun        (501) staff       (20)     1093 2022-11-05 16:22:08.000000 pdfminer.aemc-20221118/LICENSE
--rw-rw-r--   0 jun        (501) staff       (20)      160 2022-11-05 16:22:08.000000 pdfminer.aemc-20221118/MANIFEST.in
--rw-rw-r--   0 jun        (501) staff       (20)     1141 2022-11-05 16:22:08.000000 pdfminer.aemc-20221118/Makefile
--rw-r--r--   0 jun        (501) staff       (20)     3519 2024-04-02 11:28:22.581316 pdfminer.aemc-20221118/PKG-INFO
--rw-rw-r--   0 jun        (501) staff       (20)     2573 2022-11-05 16:22:08.000000 pdfminer.aemc-20221118/README.md
-drwxr-xr-x   0 jun        (501) staff       (20)        0 2024-04-02 11:28:22.550627 pdfminer.aemc-20221118/cmaprsrc/
--rw-rw-r--   0 jun        (501) staff       (20)     2917 2022-11-05 16:22:08.000000 pdfminer.aemc-20221118/cmaprsrc/README.txt
--rw-rw-r--   0 jun        (501) staff       (20)  2046762 2022-11-05 16:22:08.000000 pdfminer.aemc-20221118/cmaprsrc/cid2code_Adobe_CNS1.txt
--rw-rw-r--   0 jun        (501) staff       (20)  1900416 2022-11-05 16:22:08.000000 pdfminer.aemc-20221118/cmaprsrc/cid2code_Adobe_GB1.txt
--rw-rw-r--   0 jun        (501) staff       (20)  2681742 2022-11-05 16:22:08.000000 pdfminer.aemc-20221118/cmaprsrc/cid2code_Adobe_Japan1.txt
--rw-rw-r--   0 jun        (501) staff       (20)  1028252 2022-11-05 16:22:08.000000 pdfminer.aemc-20221118/cmaprsrc/cid2code_Adobe_Korea1.txt
--rw-rw-r--   0 jun        (501) staff       (20)     1181 2022-11-05 16:22:08.000000 pdfminer.aemc-20221118/noxfile.py
-drwxr-xr-x   0 jun        (501) staff       (20)        0 2024-04-02 11:28:22.555760 pdfminer.aemc-20221118/pdfminer/
--rw-rw-r--   0 jun        (501) staff       (20)      196 2024-04-02 11:26:56.000000 pdfminer.aemc-20221118/pdfminer/__init__.py
--rw-rw-r--   0 jun        (501) staff       (20)     3600 2022-11-05 16:22:08.000000 pdfminer.aemc-20221118/pdfminer/_saslprep.py
--rw-rw-r--   0 jun        (501) staff       (20)      929 2022-11-05 16:22:08.000000 pdfminer.aemc-20221118/pdfminer/arcfour.py
--rw-rw-r--   0 jun        (501) staff       (20)     2097 2022-11-05 16:22:08.000000 pdfminer.aemc-20221118/pdfminer/ascii85.py
--rw-rw-r--   0 jun        (501) staff       (20)    21391 2022-11-05 16:22:08.000000 pdfminer.aemc-20221118/pdfminer/ccitt.py
-drwxr-xr-x   0 jun        (501) staff       (20)        0 2024-04-02 11:28:22.579513 pdfminer.aemc-20221118/pdfminer/cmap/
--rw-rw-r--   0 jun        (501) staff       (20)    20532 2022-11-05 16:22:08.000000 pdfminer.aemc-20221118/pdfminer/cmap/78-EUC-H.pickle.gz
--rw-rw-r--   0 jun        (501) staff       (20)    20551 2022-11-05 16:22:08.000000 pdfminer.aemc-20221118/pdfminer/cmap/78-EUC-V.pickle.gz
--rw-rw-r--   0 jun        (501) staff       (20)    19882 2022-11-05 16:22:08.000000 pdfminer.aemc-20221118/pdfminer/cmap/78-H.pickle.gz
--rw-rw-r--   0 jun        (501) staff       (20)    22969 2022-11-05 16:22:08.000000 pdfminer.aemc-20221118/pdfminer/cmap/78-RKSJ-H.pickle.gz
--rw-rw-r--   0 jun        (501) staff       (20)    22990 2022-11-05 16:22:08.000000 pdfminer.aemc-20221118/pdfminer/cmap/78-RKSJ-V.pickle.gz
--rw-rw-r--   0 jun        (501) staff       (20)    19883 2022-11-05 16:22:08.000000 pdfminer.aemc-20221118/pdfminer/cmap/78-V.pickle.gz
--rw-rw-r--   0 jun        (501) staff       (20)    25942 2022-11-05 16:22:08.000000 pdfminer.aemc-20221118/pdfminer/cmap/78ms-RKSJ-H.pickle.gz
--rw-rw-r--   0 jun        (501) staff       (20)    25964 2022-11-05 16:22:08.000000 pdfminer.aemc-20221118/pdfminer/cmap/78ms-RKSJ-V.pickle.gz
--rw-rw-r--   0 jun        (501) staff       (20)    26305 2022-11-05 16:22:08.000000 pdfminer.aemc-20221118/pdfminer/cmap/83pv-RKSJ-H.pickle.gz
--rw-rw-r--   0 jun        (501) staff       (20)    26305 2022-11-05 16:22:08.000000 pdfminer.aemc-20221118/pdfminer/cmap/83pv-RKSJ-V.pickle.gz
--rw-rw-r--   0 jun        (501) staff       (20)    25732 2022-11-05 16:22:08.000000 pdfminer.aemc-20221118/pdfminer/cmap/90ms-RKSJ-H.pickle.gz
--rw-rw-r--   0 jun        (501) staff       (20)    25757 2022-11-05 16:22:08.000000 pdfminer.aemc-20221118/pdfminer/cmap/90ms-RKSJ-V.pickle.gz
--rw-rw-r--   0 jun        (501) staff       (20)    25670 2022-11-05 16:22:08.000000 pdfminer.aemc-20221118/pdfminer/cmap/90msp-RKSJ-H.pickle.gz
--rw-rw-r--   0 jun        (501) staff       (20)    25688 2022-11-05 16:22:08.000000 pdfminer.aemc-20221118/pdfminer/cmap/90msp-RKSJ-V.pickle.gz
--rw-rw-r--   0 jun        (501) staff       (20)    24226 2022-11-05 16:22:08.000000 pdfminer.aemc-20221118/pdfminer/cmap/90pv-RKSJ-H.pickle.gz
--rw-rw-r--   0 jun        (501) staff       (20)    24021 2022-11-05 16:22:08.000000 pdfminer.aemc-20221118/pdfminer/cmap/90pv-RKSJ-V.pickle.gz
--rw-rw-r--   0 jun        (501) staff       (20)    21027 2022-11-05 16:22:08.000000 pdfminer.aemc-20221118/pdfminer/cmap/Add-H.pickle.gz
--rw-rw-r--   0 jun        (501) staff       (20)    24275 2022-11-05 16:22:08.000000 pdfminer.aemc-20221118/pdfminer/cmap/Add-RKSJ-H.pickle.gz
--rw-rw-r--   0 jun        (501) staff       (20)    24079 2022-11-05 16:22:08.000000 pdfminer.aemc-20221118/pdfminer/cmap/Add-RKSJ-V.pickle.gz
--rw-rw-r--   0 jun        (501) staff       (20)    20874 2022-11-05 16:22:08.000000 pdfminer.aemc-20221118/pdfminer/cmap/Add-V.pickle.gz
--rw-rw-r--   0 jun        (501) staff       (20)    42594 2022-11-05 16:22:08.000000 pdfminer.aemc-20221118/pdfminer/cmap/B5-H.pickle.gz
--rw-rw-r--   0 jun        (501) staff       (20)    42549 2022-11-05 16:22:08.000000 pdfminer.aemc-20221118/pdfminer/cmap/B5-V.pickle.gz
--rw-rw-r--   0 jun        (501) staff       (20)    42602 2022-11-05 16:22:08.000000 pdfminer.aemc-20221118/pdfminer/cmap/B5pc-H.pickle.gz
--rw-rw-r--   0 jun        (501) staff       (20)    42557 2022-11-05 16:22:08.000000 pdfminer.aemc-20221118/pdfminer/cmap/B5pc-V.pickle.gz
--rw-rw-r--   0 jun        (501) staff       (20)    56990 2022-11-05 16:22:08.000000 pdfminer.aemc-20221118/pdfminer/cmap/CNS-EUC-H.pickle.gz
--rw-rw-r--   0 jun        (501) staff       (20)    56943 2022-11-05 16:22:08.000000 pdfminer.aemc-20221118/pdfminer/cmap/CNS-EUC-V.pickle.gz
--rw-rw-r--   0 jun        (501) staff       (20)    17615 2022-11-05 16:22:08.000000 pdfminer.aemc-20221118/pdfminer/cmap/CNS1-H.pickle.gz
--rw-rw-r--   0 jun        (501) staff       (20)    17564 2022-11-05 16:22:08.000000 pdfminer.aemc-20221118/pdfminer/cmap/CNS1-V.pickle.gz
--rw-rw-r--   0 jun        (501) staff       (20)    21723 2022-11-05 16:22:08.000000 pdfminer.aemc-20221118/pdfminer/cmap/CNS2-H.pickle.gz
--rw-rw-r--   0 jun        (501) staff       (20)    21723 2022-11-05 16:22:08.000000 pdfminer.aemc-20221118/pdfminer/cmap/CNS2-V.pickle.gz
--rw-rw-r--   0 jun        (501) staff       (20)    59548 2022-11-05 16:22:08.000000 pdfminer.aemc-20221118/pdfminer/cmap/ETHK-B5-H.pickle.gz
--rw-rw-r--   0 jun        (501) staff       (20)    59481 2022-11-05 16:22:08.000000 pdfminer.aemc-20221118/pdfminer/cmap/ETHK-B5-V.pickle.gz
--rw-rw-r--   0 jun        (501) staff       (20)    43982 2022-11-05 16:22:08.000000 pdfminer.aemc-20221118/pdfminer/cmap/ETen-B5-H.pickle.gz
--rw-rw-r--   0 jun        (501) staff       (20)    43924 2022-11-05 16:22:08.000000 pdfminer.aemc-20221118/pdfminer/cmap/ETen-B5-V.pickle.gz
--rw-rw-r--   0 jun        (501) staff       (20)      320 2022-11-05 16:22:08.000000 pdfminer.aemc-20221118/pdfminer/cmap/ETenms-B5-H.pickle.gz
--rw-rw-r--   0 jun        (501) staff       (20)      438 2022-11-05 16:22:08.000000 pdfminer.aemc-20221118/pdfminer/cmap/ETenms-B5-V.pickle.gz
--rw-rw-r--   0 jun        (501) staff       (20)    20429 2022-11-05 16:22:08.000000 pdfminer.aemc-20221118/pdfminer/cmap/EUC-H.pickle.gz
--rw-rw-r--   0 jun        (501) staff       (20)    20455 2022-11-05 16:22:08.000000 pdfminer.aemc-20221118/pdfminer/cmap/EUC-V.pickle.gz
--rw-rw-r--   0 jun        (501) staff       (20)    22272 2022-11-05 16:22:08.000000 pdfminer.aemc-20221118/pdfminer/cmap/Ext-H.pickle.gz
--rw-rw-r--   0 jun        (501) staff       (20)    25721 2022-11-05 16:22:08.000000 pdfminer.aemc-20221118/pdfminer/cmap/Ext-RKSJ-H.pickle.gz
--rw-rw-r--   0 jun        (501) staff       (20)    25750 2022-11-05 16:22:08.000000 pdfminer.aemc-20221118/pdfminer/cmap/Ext-RKSJ-V.pickle.gz
--rw-rw-r--   0 jun        (501) staff       (20)    22307 2022-11-05 16:22:08.000000 pdfminer.aemc-20221118/pdfminer/cmap/Ext-V.pickle.gz
--rw-rw-r--   0 jun        (501) staff       (20)    22118 2022-11-05 16:22:08.000000 pdfminer.aemc-20221118/pdfminer/cmap/GB-EUC-H.pickle.gz
--rw-rw-r--   0 jun        (501) staff       (20)    22111 2022-11-05 16:22:08.000000 pdfminer.aemc-20221118/pdfminer/cmap/GB-EUC-V.pickle.gz
--rw-rw-r--   0 jun        (501) staff       (20)    21699 2022-11-05 16:22:08.000000 pdfminer.aemc-20221118/pdfminer/cmap/GB-H.pickle.gz
--rw-rw-r--   0 jun        (501) staff       (20)    21694 2022-11-05 16:22:08.000000 pdfminer.aemc-20221118/pdfminer/cmap/GB-V.pickle.gz
--rw-rw-r--   0 jun        (501) staff       (20)    68254 2022-11-05 16:22:08.000000 pdfminer.aemc-20221118/pdfminer/cmap/GBK-EUC-H.pickle.gz
--rw-rw-r--   0 jun        (501) staff       (20)    68199 2022-11-05 16:22:08.000000 pdfminer.aemc-20221118/pdfminer/cmap/GBK-EUC-V.pickle.gz
--rw-rw-r--   0 jun        (501) staff       (20)    89917 2022-11-05 16:22:08.000000 pdfminer.aemc-20221118/pdfminer/cmap/GBK2K-H.pickle.gz
--rw-rw-r--   0 jun        (501) staff       (20)    89872 2022-11-05 16:22:08.000000 pdfminer.aemc-20221118/pdfminer/cmap/GBK2K-V.pickle.gz
--rw-rw-r--   0 jun        (501) staff       (20)    68148 2022-11-05 16:22:08.000000 pdfminer.aemc-20221118/pdfminer/cmap/GBKp-EUC-H.pickle.gz
--rw-rw-r--   0 jun        (501) staff       (20)    68102 2022-11-05 16:22:08.000000 pdfminer.aemc-20221118/pdfminer/cmap/GBKp-EUC-V.pickle.gz
--rw-rw-r--   0 jun        (501) staff       (20)    23815 2022-11-05 16:22:08.000000 pdfminer.aemc-20221118/pdfminer/cmap/GBT-EUC-H.pickle.gz
--rw-rw-r--   0 jun        (501) staff       (20)    23806 2022-11-05 16:22:08.000000 pdfminer.aemc-20221118/pdfminer/cmap/GBT-EUC-V.pickle.gz
--rw-rw-r--   0 jun        (501) staff       (20)    23339 2022-11-05 16:22:08.000000 pdfminer.aemc-20221118/pdfminer/cmap/GBT-H.pickle.gz
--rw-rw-r--   0 jun        (501) staff       (20)    23322 2022-11-05 16:22:08.000000 pdfminer.aemc-20221118/pdfminer/cmap/GBT-V.pickle.gz
--rw-rw-r--   0 jun        (501) staff       (20)    23650 2022-11-05 16:22:08.000000 pdfminer.aemc-20221118/pdfminer/cmap/GBTpc-EUC-H.pickle.gz
--rw-rw-r--   0 jun        (501) staff       (20)    23647 2022-11-05 16:22:08.000000 pdfminer.aemc-20221118/pdfminer/cmap/GBTpc-EUC-V.pickle.gz
--rw-rw-r--   0 jun        (501) staff       (20)    21945 2022-11-05 16:22:08.000000 pdfminer.aemc-20221118/pdfminer/cmap/GBpc-EUC-H.pickle.gz
--rw-rw-r--   0 jun        (501) staff       (20)    21956 2022-11-05 16:22:08.000000 pdfminer.aemc-20221118/pdfminer/cmap/GBpc-EUC-V.pickle.gz
--rw-rw-r--   0 jun        (501) staff       (20)    19781 2022-11-05 16:22:08.000000 pdfminer.aemc-20221118/pdfminer/cmap/H.pickle.gz
--rw-rw-r--   0 jun        (501) staff       (20)    45212 2022-11-05 16:22:08.000000 pdfminer.aemc-20221118/pdfminer/cmap/HKdla-B5-H.pickle.gz
--rw-rw-r--   0 jun        (501) staff       (20)    45167 2022-11-05 16:22:08.000000 pdfminer.aemc-20221118/pdfminer/cmap/HKdla-B5-V.pickle.gz
--rw-rw-r--   0 jun        (501) staff       (20)    44853 2022-11-05 16:22:08.000000 pdfminer.aemc-20221118/pdfminer/cmap/HKdlb-B5-H.pickle.gz
--rw-rw-r--   0 jun        (501) staff       (20)    44816 2022-11-05 16:22:08.000000 pdfminer.aemc-20221118/pdfminer/cmap/HKdlb-B5-V.pickle.gz
--rw-rw-r--   0 jun        (501) staff       (20)    53104 2022-11-05 16:22:08.000000 pdfminer.aemc-20221118/pdfminer/cmap/HKgccs-B5-H.pickle.gz
--rw-rw-r--   0 jun        (501) staff       (20)    53050 2022-11-05 16:22:08.000000 pdfminer.aemc-20221118/pdfminer/cmap/HKgccs-B5-V.pickle.gz
--rw-rw-r--   0 jun        (501) staff       (20)    43667 2022-11-05 16:22:08.000000 pdfminer.aemc-20221118/pdfminer/cmap/HKm314-B5-H.pickle.gz
--rw-rw-r--   0 jun        (501) staff       (20)    43618 2022-11-05 16:22:08.000000 pdfminer.aemc-20221118/pdfminer/cmap/HKm314-B5-V.pickle.gz
--rw-rw-r--   0 jun        (501) staff       (20)    44187 2022-11-05 16:22:08.000000 pdfminer.aemc-20221118/pdfminer/cmap/HKm471-B5-H.pickle.gz
--rw-rw-r--   0 jun        (501) staff       (20)    44144 2022-11-05 16:22:08.000000 pdfminer.aemc-20221118/pdfminer/cmap/HKm471-B5-V.pickle.gz
--rw-rw-r--   0 jun        (501) staff       (20)    59508 2022-11-05 16:22:08.000000 pdfminer.aemc-20221118/pdfminer/cmap/HKscs-B5-H.pickle.gz
--rw-rw-r--   0 jun        (501) staff       (20)    59473 2022-11-05 16:22:08.000000 pdfminer.aemc-20221118/pdfminer/cmap/HKscs-B5-V.pickle.gz
--rw-rw-r--   0 jun        (501) staff       (20)      840 2022-11-05 16:22:08.000000 pdfminer.aemc-20221118/pdfminer/cmap/Hankaku-H.pickle.gz
--rw-rw-r--   0 jun        (501) staff       (20)      839 2022-11-05 16:22:08.000000 pdfminer.aemc-20221118/pdfminer/cmap/Hankaku-V.pickle.gz
--rw-rw-r--   0 jun        (501) staff       (20)      391 2022-11-05 16:22:08.000000 pdfminer.aemc-20221118/pdfminer/cmap/Hiragana-H.pickle.gz
--rw-rw-r--   0 jun        (501) staff       (20)      391 2022-11-05 16:22:08.000000 pdfminer.aemc-20221118/pdfminer/cmap/Hiragana-V.pickle.gz
--rw-rw-r--   0 jun        (501) staff       (20)    24040 2022-11-05 16:22:08.000000 pdfminer.aemc-20221118/pdfminer/cmap/KSC-EUC-H.pickle.gz
--rw-rw-r--   0 jun        (501) staff       (20)    24078 2022-11-05 16:22:08.000000 pdfminer.aemc-20221118/pdfminer/cmap/KSC-EUC-V.pickle.gz
--rw-rw-r--   0 jun        (501) staff       (20)    23563 2022-11-05 16:22:08.000000 pdfminer.aemc-20221118/pdfminer/cmap/KSC-H.pickle.gz
--rw-rw-r--   0 jun        (501) staff       (20)    55016 2022-11-05 16:22:08.000000 pdfminer.aemc-20221118/pdfminer/cmap/KSC-Johab-H.pickle.gz
--rw-rw-r--   0 jun        (501) staff       (20)    55041 2022-11-05 16:22:08.000000 pdfminer.aemc-20221118/pdfminer/cmap/KSC-Johab-V.pickle.gz
--rw-rw-r--   0 jun        (501) staff       (20)    23644 2022-11-05 16:22:08.000000 pdfminer.aemc-20221118/pdfminer/cmap/KSC-V.pickle.gz
--rw-rw-r--   0 jun        (501) staff       (20)    51667 2022-11-05 16:22:08.000000 pdfminer.aemc-20221118/pdfminer/cmap/KSCms-UHC-H.pickle.gz
--rw-rw-r--   0 jun        (501) staff       (20)    51788 2022-11-05 16:22:08.000000 pdfminer.aemc-20221118/pdfminer/cmap/KSCms-UHC-HW-H.pickle.gz
--rw-rw-r--   0 jun        (501) staff       (20)    51821 2022-11-05 16:22:08.000000 pdfminer.aemc-20221118/pdfminer/cmap/KSCms-UHC-HW-V.pickle.gz
--rw-rw-r--   0 jun        (501) staff       (20)    51698 2022-11-05 16:22:08.000000 pdfminer.aemc-20221118/pdfminer/cmap/KSCms-UHC-V.pickle.gz
--rw-rw-r--   0 jun        (501) staff       (20)    27769 2022-11-05 16:22:08.000000 pdfminer.aemc-20221118/pdfminer/cmap/KSCpc-EUC-H.pickle.gz
--rw-rw-r--   0 jun        (501) staff       (20)    27820 2022-11-05 16:22:08.000000 pdfminer.aemc-20221118/pdfminer/cmap/KSCpc-EUC-V.pickle.gz
--rw-rw-r--   0 jun        (501) staff       (20)      404 2022-11-05 16:22:08.000000 pdfminer.aemc-20221118/pdfminer/cmap/Katakana-H.pickle.gz
--rw-rw-r--   0 jun        (501) staff       (20)      404 2022-11-05 16:22:08.000000 pdfminer.aemc-20221118/pdfminer/cmap/Katakana-V.pickle.gz
--rw-rw-r--   0 jun        (501) staff       (20)    21708 2022-11-05 16:22:08.000000 pdfminer.aemc-20221118/pdfminer/cmap/NWP-H.pickle.gz
--rw-rw-r--   0 jun        (501) staff       (20)    21779 2022-11-05 16:22:08.000000 pdfminer.aemc-20221118/pdfminer/cmap/NWP-V.pickle.gz
--rw-rw-r--   0 jun        (501) staff       (20)     3917 2022-11-05 16:22:08.000000 pdfminer.aemc-20221118/pdfminer/cmap/README.txt
--rw-rw-r--   0 jun        (501) staff       (20)    23030 2022-11-05 16:22:08.000000 pdfminer.aemc-20221118/pdfminer/cmap/RKSJ-H.pickle.gz
--rw-rw-r--   0 jun        (501) staff       (20)    23048 2022-11-05 16:22:08.000000 pdfminer.aemc-20221118/pdfminer/cmap/RKSJ-V.pickle.gz
--rw-rw-r--   0 jun        (501) staff       (20)      394 2022-11-05 16:22:08.000000 pdfminer.aemc-20221118/pdfminer/cmap/Roman-H.pickle.gz
--rw-rw-r--   0 jun        (501) staff       (20)      394 2022-11-05 16:22:08.000000 pdfminer.aemc-20221118/pdfminer/cmap/Roman-V.pickle.gz
--rw-rw-r--   0 jun        (501) staff       (20)    67459 2022-11-05 16:22:08.000000 pdfminer.aemc-20221118/pdfminer/cmap/UniCNS-UCS2-H.pickle.gz
--rw-rw-r--   0 jun        (501) staff       (20)    67395 2022-11-05 16:22:08.000000 pdfminer.aemc-20221118/pdfminer/cmap/UniCNS-UCS2-V.pickle.gz
--rw-rw-r--   0 jun        (501) staff       (20)    87819 2022-11-05 16:22:08.000000 pdfminer.aemc-20221118/pdfminer/cmap/UniCNS-UTF16-H.pickle.gz
--rw-rw-r--   0 jun        (501) staff       (20)    87751 2022-11-05 16:22:08.000000 pdfminer.aemc-20221118/pdfminer/cmap/UniCNS-UTF16-V.pickle.gz
--rw-rw-r--   0 jun        (501) staff       (20)    87400 2022-11-05 16:22:08.000000 pdfminer.aemc-20221118/pdfminer/cmap/UniCNS-UTF32-H.pickle.gz
--rw-rw-r--   0 jun        (501) staff       (20)    87327 2022-11-05 16:22:08.000000 pdfminer.aemc-20221118/pdfminer/cmap/UniCNS-UTF32-V.pickle.gz
--rw-rw-r--   0 jun        (501) staff       (20)    82631 2022-11-05 16:22:08.000000 pdfminer.aemc-20221118/pdfminer/cmap/UniCNS-UTF8-H.pickle.gz
--rw-rw-r--   0 jun        (501) staff       (20)    82562 2022-11-05 16:22:08.000000 pdfminer.aemc-20221118/pdfminer/cmap/UniCNS-UTF8-V.pickle.gz
--rw-rw-r--   0 jun        (501) staff       (20)    97445 2022-11-05 16:22:08.000000 pdfminer.aemc-20221118/pdfminer/cmap/UniGB-UCS2-H.pickle.gz
--rw-rw-r--   0 jun        (501) staff       (20)    97441 2022-11-05 16:22:08.000000 pdfminer.aemc-20221118/pdfminer/cmap/UniGB-UCS2-V.pickle.gz
--rw-rw-r--   0 jun        (501) staff       (20)   101459 2022-11-05 16:22:08.000000 pdfminer.aemc-20221118/pdfminer/cmap/UniGB-UTF16-H.pickle.gz
--rw-rw-r--   0 jun        (501) staff       (20)   101331 2022-11-05 16:22:08.000000 pdfminer.aemc-20221118/pdfminer/cmap/UniGB-UTF16-V.pickle.gz
--rw-rw-r--   0 jun        (501) staff       (20)   101490 2022-11-05 16:22:08.000000 pdfminer.aemc-20221118/pdfminer/cmap/UniGB-UTF32-H.pickle.gz
--rw-rw-r--   0 jun        (501) staff       (20)   101357 2022-11-05 16:22:08.000000 pdfminer.aemc-20221118/pdfminer/cmap/UniGB-UTF32-V.pickle.gz
--rw-rw-r--   0 jun        (501) staff       (20)    90500 2022-11-05 16:22:08.000000 pdfminer.aemc-20221118/pdfminer/cmap/UniGB-UTF8-H.pickle.gz
--rw-rw-r--   0 jun        (501) staff       (20)    90368 2022-11-05 16:22:08.000000 pdfminer.aemc-20221118/pdfminer/cmap/UniGB-UTF8-V.pickle.gz
--rw-rw-r--   0 jun        (501) staff       (20)    35934 2022-11-05 16:22:08.000000 pdfminer.aemc-20221118/pdfminer/cmap/UniJIS-UCS2-H.pickle.gz
--rw-rw-r--   0 jun        (501) staff       (20)      412 2022-11-05 16:22:08.000000 pdfminer.aemc-20221118/pdfminer/cmap/UniJIS-UCS2-HW-H.pickle.gz
--rw-rw-r--   0 jun        (501) staff       (20)     1402 2022-11-05 16:22:08.000000 pdfminer.aemc-20221118/pdfminer/cmap/UniJIS-UCS2-HW-V.pickle.gz
--rw-rw-r--   0 jun        (501) staff       (20)    35852 2022-11-05 16:22:08.000000 pdfminer.aemc-20221118/pdfminer/cmap/UniJIS-UCS2-V.pickle.gz
--rw-rw-r--   0 jun        (501) staff       (20)    58054 2022-11-05 16:22:08.000000 pdfminer.aemc-20221118/pdfminer/cmap/UniJIS-UTF16-H.pickle.gz
--rw-rw-r--   0 jun        (501) staff       (20)    57928 2022-11-05 16:22:08.000000 pdfminer.aemc-20221118/pdfminer/cmap/UniJIS-UTF16-V.pickle.gz
--rw-rw-r--   0 jun        (501) staff       (20)    57910 2022-11-05 16:22:08.000000 pdfminer.aemc-20221118/pdfminer/cmap/UniJIS-UTF32-H.pickle.gz
--rw-rw-r--   0 jun        (501) staff       (20)    57780 2022-11-05 16:22:08.000000 pdfminer.aemc-20221118/pdfminer/cmap/UniJIS-UTF32-V.pickle.gz
--rw-rw-r--   0 jun        (501) staff       (20)    54764 2022-11-05 16:22:08.000000 pdfminer.aemc-20221118/pdfminer/cmap/UniJIS-UTF8-H.pickle.gz
--rw-rw-r--   0 jun        (501) staff       (20)    54684 2022-11-05 16:22:08.000000 pdfminer.aemc-20221118/pdfminer/cmap/UniJIS-UTF8-V.pickle.gz
--rw-rw-r--   0 jun        (501) staff       (20)    58081 2022-11-05 16:22:08.000000 pdfminer.aemc-20221118/pdfminer/cmap/UniJIS2004-UTF16-H.pickle.gz
--rw-rw-r--   0 jun        (501) staff       (20)    57960 2022-11-05 16:22:08.000000 pdfminer.aemc-20221118/pdfminer/cmap/UniJIS2004-UTF16-V.pickle.gz
--rw-rw-r--   0 jun        (501) staff       (20)    57940 2022-11-05 16:22:08.000000 pdfminer.aemc-20221118/pdfminer/cmap/UniJIS2004-UTF32-H.pickle.gz
--rw-rw-r--   0 jun        (501) staff       (20)    57811 2022-11-05 16:22:08.000000 pdfminer.aemc-20221118/pdfminer/cmap/UniJIS2004-UTF32-V.pickle.gz
--rw-rw-r--   0 jun        (501) staff       (20)    54829 2022-11-05 16:22:08.000000 pdfminer.aemc-20221118/pdfminer/cmap/UniJIS2004-UTF8-H.pickle.gz
--rw-rw-r--   0 jun        (501) staff       (20)    54749 2022-11-05 16:22:08.000000 pdfminer.aemc-20221118/pdfminer/cmap/UniJIS2004-UTF8-V.pickle.gz
--rw-rw-r--   0 jun        (501) staff       (20)    57903 2022-11-05 16:22:08.000000 pdfminer.aemc-20221118/pdfminer/cmap/UniJISX0213-UTF32-H.pickle.gz
--rw-rw-r--   0 jun        (501) staff       (20)    57778 2022-11-05 16:22:08.000000 pdfminer.aemc-20221118/pdfminer/cmap/UniJISX0213-UTF32-V.pickle.gz
--rw-rw-r--   0 jun        (501) staff       (20)    57930 2022-11-05 16:22:08.000000 pdfminer.aemc-20221118/pdfminer/cmap/UniJISX02132004-UTF32-H.pickle.gz
--rw-rw-r--   0 jun        (501) staff       (20)    57808 2022-11-05 16:22:08.000000 pdfminer.aemc-20221118/pdfminer/cmap/UniJISX02132004-UTF32-V.pickle.gz
--rw-rw-r--   0 jun        (501) staff       (20)    60683 2022-11-05 16:22:08.000000 pdfminer.aemc-20221118/pdfminer/cmap/UniKS-UCS2-H.pickle.gz
--rw-rw-r--   0 jun        (501) staff       (20)    60699 2022-11-05 16:22:08.000000 pdfminer.aemc-20221118/pdfminer/cmap/UniKS-UCS2-V.pickle.gz
--rw-rw-r--   0 jun        (501) staff       (20)    61278 2022-11-05 16:22:08.000000 pdfminer.aemc-20221118/pdfminer/cmap/UniKS-UTF16-H.pickle.gz
--rw-rw-r--   0 jun        (501) staff       (20)    61298 2022-11-05 16:22:08.000000 pdfminer.aemc-20221118/pdfminer/cmap/UniKS-UTF16-V.pickle.gz
--rw-rw-r--   0 jun        (501) staff       (20)    61286 2022-11-05 16:22:08.000000 pdfminer.aemc-20221118/pdfminer/cmap/UniKS-UTF32-H.pickle.gz
--rw-rw-r--   0 jun        (501) staff       (20)    61309 2022-11-05 16:22:08.000000 pdfminer.aemc-20221118/pdfminer/cmap/UniKS-UTF32-V.pickle.gz
--rw-rw-r--   0 jun        (501) staff       (20)    54151 2022-11-05 16:22:08.000000 pdfminer.aemc-20221118/pdfminer/cmap/UniKS-UTF8-H.pickle.gz
--rw-rw-r--   0 jun        (501) staff       (20)    54172 2022-11-05 16:22:08.000000 pdfminer.aemc-20221118/pdfminer/cmap/UniKS-UTF8-V.pickle.gz
--rw-rw-r--   0 jun        (501) staff       (20)    19826 2022-11-05 16:22:08.000000 pdfminer.aemc-20221118/pdfminer/cmap/V.pickle.gz
--rw-rw-r--   0 jun        (501) staff       (20)      505 2022-11-05 16:22:08.000000 pdfminer.aemc-20221118/pdfminer/cmap/WP-Symbol-H.pickle.gz
--rw-rw-r--   0 jun        (501) staff       (20)      505 2022-11-05 16:22:08.000000 pdfminer.aemc-20221118/pdfminer/cmap/WP-Symbol-V.pickle.gz
--rw-rw-r--   0 jun        (501) staff       (20)   138237 2022-11-05 16:22:08.000000 pdfminer.aemc-20221118/pdfminer/cmap/to-unicode-Adobe-CNS1.pickle.gz
--rw-rw-r--   0 jun        (501) staff       (20)   204425 2022-11-05 16:22:08.000000 pdfminer.aemc-20221118/pdfminer/cmap/to-unicode-Adobe-GB1.pickle.gz
--rw-rw-r--   0 jun        (501) staff       (20)   112987 2022-11-05 16:22:08.000000 pdfminer.aemc-20221118/pdfminer/cmap/to-unicode-Adobe-Japan1.pickle.gz
--rw-rw-r--   0 jun        (501) staff       (20)   120859 2022-11-05 16:22:08.000000 pdfminer.aemc-20221118/pdfminer/cmap/to-unicode-Adobe-Korea1.pickle.gz
--rw-rw-r--   0 jun        (501) staff       (20)    16163 2024-03-27 08:04:45.000000 pdfminer.aemc-20221118/pdfminer/cmapdb.py
--rw-rw-r--   0 jun        (501) staff       (20)    34968 2022-11-05 16:22:08.000000 pdfminer.aemc-20221118/pdfminer/converter.py
--rw-rw-r--   0 jun        (501) staff       (20)     1654 2022-11-05 16:22:08.000000 pdfminer.aemc-20221118/pdfminer/data_structures.py
--rw-rw-r--   0 jun        (501) staff       (20)     3983 2022-11-05 16:22:08.000000 pdfminer.aemc-20221118/pdfminer/encodingdb.py
--rw-rw-r--   0 jun        (501) staff       (20)   112611 2022-11-05 16:22:08.000000 pdfminer.aemc-20221118/pdfminer/fontmetrics.py
--rw-rw-r--   0 jun        (501) staff       (20)   130804 2022-11-05 16:22:08.000000 pdfminer.aemc-20221118/pdfminer/glyphlist.py
--rw-rw-r--   0 jun        (501) staff       (20)     7276 2022-11-05 16:22:08.000000 pdfminer.aemc-20221118/pdfminer/high_level.py
--rw-rw-r--   0 jun        (501) staff       (20)     9299 2022-11-05 16:22:08.000000 pdfminer.aemc-20221118/pdfminer/image.py
--rw-rw-r--   0 jun        (501) staff       (20)    11391 2022-11-05 16:22:08.000000 pdfminer.aemc-20221118/pdfminer/jbig2.py
--rw-rw-r--   0 jun        (501) staff       (20)     8531 2022-11-05 16:22:08.000000 pdfminer.aemc-20221118/pdfminer/latin_enc.py
--rw-rw-r--   0 jun        (501) staff       (20)    35735 2024-04-02 11:27:07.000000 pdfminer.aemc-20221118/pdfminer/layout.py
--rw-rw-r--   0 jun        (501) staff       (20)     3177 2022-11-05 16:22:08.000000 pdfminer.aemc-20221118/pdfminer/lzw.py
--rw-rw-r--   0 jun        (501) staff       (20)      821 2022-11-05 16:22:08.000000 pdfminer.aemc-20221118/pdfminer/pdfcolor.py
--rw-rw-r--   0 jun        (501) staff       (20)     8787 2022-11-05 16:22:08.000000 pdfminer.aemc-20221118/pdfminer/pdfdevice.py
--rw-rw-r--   0 jun        (501) staff       (20)    37267 2022-11-05 16:22:08.000000 pdfminer.aemc-20221118/pdfminer/pdfdocument.py
--rw-rw-r--   0 jun        (501) staff       (20)    37786 2024-03-27 08:00:02.000000 pdfminer.aemc-20221118/pdfminer/pdffont.py
--rw-rw-r--   0 jun        (501) staff       (20)    34539 2022-11-05 16:22:08.000000 pdfminer.aemc-20221118/pdfminer/pdfinterp.py
--rw-rw-r--   0 jun        (501) staff       (20)     6803 2022-11-05 16:22:08.000000 pdfminer.aemc-20221118/pdfminer/pdfpage.py
--rw-rw-r--   0 jun        (501) staff       (20)     5896 2022-11-05 16:22:08.000000 pdfminer.aemc-20221118/pdfminer/pdfparser.py
--rw-rw-r--   0 jun        (501) staff       (20)    12109 2022-11-05 16:22:08.000000 pdfminer.aemc-20221118/pdfminer/pdftypes.py
--rwxr-xr-x   0 jun        (501) staff       (20)    19649 2022-11-05 16:22:08.000000 pdfminer.aemc-20221118/pdfminer/psparser.py
--rw-rw-r--   0 jun        (501) staff       (20)        0 2022-11-05 16:22:08.000000 pdfminer.aemc-20221118/pdfminer/py.typed
--rw-rw-r--   0 jun        (501) staff       (20)     1358 2022-11-05 16:22:08.000000 pdfminer.aemc-20221118/pdfminer/runlength.py
--rw-rw-r--   0 jun        (501) staff       (20)       15 2022-11-05 16:22:08.000000 pdfminer.aemc-20221118/pdfminer/settings.py
--rw-rw-r--   0 jun        (501) staff       (20)    20804 2022-11-05 16:22:08.000000 pdfminer.aemc-20221118/pdfminer/utils.py
-drwxr-xr-x   0 jun        (501) staff       (20)        0 2024-04-02 11:28:22.556282 pdfminer.aemc-20221118/pdfminer.aemc.egg-info/
--rw-r--r--   0 jun        (501) staff       (20)     3519 2024-04-02 11:28:22.000000 pdfminer.aemc-20221118/pdfminer.aemc.egg-info/PKG-INFO
--rw-r--r--   0 jun        (501) staff       (20)     6521 2024-04-02 11:28:22.000000 pdfminer.aemc-20221118/pdfminer.aemc.egg-info/SOURCES.txt
--rw-r--r--   0 jun        (501) staff       (20)        1 2024-04-02 11:28:22.000000 pdfminer.aemc-20221118/pdfminer.aemc.egg-info/dependency_links.txt
--rw-r--r--   0 jun        (501) staff       (20)      175 2024-04-02 11:28:22.000000 pdfminer.aemc-20221118/pdfminer.aemc.egg-info/requires.txt
--rw-r--r--   0 jun        (501) staff       (20)        9 2024-04-02 11:28:22.000000 pdfminer.aemc-20221118/pdfminer.aemc.egg-info/top_level.txt
--rw-r--r--   0 jun        (501) staff       (20)       38 2024-04-02 11:28:22.581532 pdfminer.aemc-20221118/setup.cfg
--rw-rw-r--   0 jun        (501) staff       (20)     1776 2024-03-27 08:10:12.000000 pdfminer.aemc-20221118/setup.py
-drwxr-xr-x   0 jun        (501) staff       (20)        0 2024-04-02 11:28:22.581106 pdfminer.aemc-20221118/tools/
--rw-rw-r--   0 jun        (501) staff       (20)        0 2022-11-05 16:22:08.000000 pdfminer.aemc-20221118/tools/__init__.py
--rwxr-xr-x   0 jun        (501) staff       (20)     1646 2022-11-05 16:22:08.000000 pdfminer.aemc-20221118/tools/conv_afm.py
--rwxr-xr-x   0 jun        (501) staff       (20)     6089 2022-11-05 16:22:08.000000 pdfminer.aemc-20221118/tools/conv_cmap.py
--rwxr-xr-x   0 jun        (501) staff       (20)      911 2022-11-05 16:22:08.000000 pdfminer.aemc-20221118/tools/conv_glyphlist.py
--rwxr-xr-x   0 jun        (501) staff       (20)    14316 2022-11-05 16:22:08.000000 pdfminer.aemc-20221118/tools/dumppdf.py
--rwxr-xr-x   0 jun        (501) staff       (20)     9779 2022-11-05 16:22:08.000000 pdfminer.aemc-20221118/tools/pdf2txt.py
--rw-rw-r--   0 jun        (501) staff       (20)     6266 2022-11-05 16:22:08.000000 pdfminer.aemc-20221118/tools/pdfdiff.py
--rwxr-xr-x   0 jun        (501) staff       (20)     2761 2022-11-05 16:22:08.000000 pdfminer.aemc-20221118/tools/pdfstats.py
--rw-rw-r--   0 jun        (501) staff       (20)     1415 2022-11-05 16:22:08.000000 pdfminer.aemc-20221118/tools/prof.py
+drwxr-xr-x   0 jun        (501) staff       (20)        0 2024-05-04 04:32:45.612769 pdfminer_aemc-20231228/
+-rw-rw-r--   0 jun        (501) staff       (20)    15840 2023-12-28 21:20:33.000000 pdfminer_aemc-20231228/CHANGELOG.md
+-rw-rw-r--   0 jun        (501) staff       (20)     2397 2023-12-28 21:20:33.000000 pdfminer_aemc-20231228/CONTRIBUTING.md
+-rw-rw-r--   0 jun        (501) staff       (20)     1093 2023-12-28 21:20:33.000000 pdfminer_aemc-20231228/LICENSE
+-rw-rw-r--   0 jun        (501) staff       (20)      160 2023-12-28 21:20:33.000000 pdfminer_aemc-20231228/MANIFEST.in
+-rw-rw-r--   0 jun        (501) staff       (20)     1141 2023-12-28 21:20:33.000000 pdfminer_aemc-20231228/Makefile
+-rw-r--r--   0 jun        (501) staff       (20)     4144 2024-05-04 04:32:45.612523 pdfminer_aemc-20231228/PKG-INFO
+-rw-rw-r--   0 jun        (501) staff       (20)     2573 2023-12-28 21:20:33.000000 pdfminer_aemc-20231228/README.md
+drwxr-xr-x   0 jun        (501) staff       (20)        0 2024-05-04 04:32:45.573107 pdfminer_aemc-20231228/cmaprsrc/
+-rw-rw-r--   0 jun        (501) staff       (20)     2917 2023-12-28 21:20:33.000000 pdfminer_aemc-20231228/cmaprsrc/README.txt
+-rw-rw-r--   0 jun        (501) staff       (20)  2046762 2023-12-28 21:20:33.000000 pdfminer_aemc-20231228/cmaprsrc/cid2code_Adobe_CNS1.txt
+-rw-rw-r--   0 jun        (501) staff       (20)  1900416 2023-12-28 21:20:33.000000 pdfminer_aemc-20231228/cmaprsrc/cid2code_Adobe_GB1.txt
+-rw-rw-r--   0 jun        (501) staff       (20)  2681742 2023-12-28 21:20:33.000000 pdfminer_aemc-20231228/cmaprsrc/cid2code_Adobe_Japan1.txt
+-rw-rw-r--   0 jun        (501) staff       (20)  1028252 2023-12-28 21:20:33.000000 pdfminer_aemc-20231228/cmaprsrc/cid2code_Adobe_Korea1.txt
+-rw-rw-r--   0 jun        (501) staff       (20)     1310 2023-12-28 21:20:33.000000 pdfminer_aemc-20231228/noxfile.py
+drwxr-xr-x   0 jun        (501) staff       (20)        0 2024-05-04 04:32:45.584051 pdfminer_aemc-20231228/pdfminer/
+-rw-rw-r--   0 jun        (501) staff       (20)      196 2024-04-24 11:19:45.000000 pdfminer_aemc-20231228/pdfminer/__init__.py
+-rw-rw-r--   0 jun        (501) staff       (20)     3600 2023-12-28 21:20:33.000000 pdfminer_aemc-20231228/pdfminer/_saslprep.py
+-rw-rw-r--   0 jun        (501) staff       (20)      929 2023-12-28 21:20:33.000000 pdfminer_aemc-20231228/pdfminer/arcfour.py
+-rw-rw-r--   0 jun        (501) staff       (20)     2097 2023-12-28 21:20:33.000000 pdfminer_aemc-20231228/pdfminer/ascii85.py
+-rw-rw-r--   0 jun        (501) staff       (20)    21391 2023-12-28 21:20:33.000000 pdfminer_aemc-20231228/pdfminer/ccitt.py
+drwxr-xr-x   0 jun        (501) staff       (20)        0 2024-05-04 04:32:45.606952 pdfminer_aemc-20231228/pdfminer/cmap/
+-rw-rw-r--   0 jun        (501) staff       (20)    20532 2023-12-28 21:20:33.000000 pdfminer_aemc-20231228/pdfminer/cmap/78-EUC-H.pickle.gz
+-rw-rw-r--   0 jun        (501) staff       (20)    20551 2023-12-28 21:20:33.000000 pdfminer_aemc-20231228/pdfminer/cmap/78-EUC-V.pickle.gz
+-rw-rw-r--   0 jun        (501) staff       (20)    19882 2023-12-28 21:20:33.000000 pdfminer_aemc-20231228/pdfminer/cmap/78-H.pickle.gz
+-rw-rw-r--   0 jun        (501) staff       (20)    22969 2023-12-28 21:20:33.000000 pdfminer_aemc-20231228/pdfminer/cmap/78-RKSJ-H.pickle.gz
+-rw-rw-r--   0 jun        (501) staff       (20)    22990 2023-12-28 21:20:33.000000 pdfminer_aemc-20231228/pdfminer/cmap/78-RKSJ-V.pickle.gz
+-rw-rw-r--   0 jun        (501) staff       (20)    19883 2023-12-28 21:20:33.000000 pdfminer_aemc-20231228/pdfminer/cmap/78-V.pickle.gz
+-rw-rw-r--   0 jun        (501) staff       (20)    25942 2023-12-28 21:20:33.000000 pdfminer_aemc-20231228/pdfminer/cmap/78ms-RKSJ-H.pickle.gz
+-rw-rw-r--   0 jun        (501) staff       (20)    25964 2023-12-28 21:20:33.000000 pdfminer_aemc-20231228/pdfminer/cmap/78ms-RKSJ-V.pickle.gz
+-rw-rw-r--   0 jun        (501) staff       (20)    26305 2023-12-28 21:20:33.000000 pdfminer_aemc-20231228/pdfminer/cmap/83pv-RKSJ-H.pickle.gz
+-rw-rw-r--   0 jun        (501) staff       (20)    26305 2023-12-28 21:20:33.000000 pdfminer_aemc-20231228/pdfminer/cmap/83pv-RKSJ-V.pickle.gz
+-rw-rw-r--   0 jun        (501) staff       (20)    25732 2023-12-28 21:20:33.000000 pdfminer_aemc-20231228/pdfminer/cmap/90ms-RKSJ-H.pickle.gz
+-rw-rw-r--   0 jun        (501) staff       (20)    25757 2023-12-28 21:20:33.000000 pdfminer_aemc-20231228/pdfminer/cmap/90ms-RKSJ-V.pickle.gz
+-rw-rw-r--   0 jun        (501) staff       (20)    25670 2023-12-28 21:20:33.000000 pdfminer_aemc-20231228/pdfminer/cmap/90msp-RKSJ-H.pickle.gz
+-rw-rw-r--   0 jun        (501) staff       (20)    25688 2023-12-28 21:20:33.000000 pdfminer_aemc-20231228/pdfminer/cmap/90msp-RKSJ-V.pickle.gz
+-rw-rw-r--   0 jun        (501) staff       (20)    24226 2023-12-28 21:20:33.000000 pdfminer_aemc-20231228/pdfminer/cmap/90pv-RKSJ-H.pickle.gz
+-rw-rw-r--   0 jun        (501) staff       (20)    24021 2023-12-28 21:20:33.000000 pdfminer_aemc-20231228/pdfminer/cmap/90pv-RKSJ-V.pickle.gz
+-rw-rw-r--   0 jun        (501) staff       (20)    21027 2023-12-28 21:20:33.000000 pdfminer_aemc-20231228/pdfminer/cmap/Add-H.pickle.gz
+-rw-rw-r--   0 jun        (501) staff       (20)    24275 2023-12-28 21:20:33.000000 pdfminer_aemc-20231228/pdfminer/cmap/Add-RKSJ-H.pickle.gz
+-rw-rw-r--   0 jun        (501) staff       (20)    24079 2023-12-28 21:20:33.000000 pdfminer_aemc-20231228/pdfminer/cmap/Add-RKSJ-V.pickle.gz
+-rw-rw-r--   0 jun        (501) staff       (20)    20874 2023-12-28 21:20:33.000000 pdfminer_aemc-20231228/pdfminer/cmap/Add-V.pickle.gz
+-rw-rw-r--   0 jun        (501) staff       (20)    42594 2023-12-28 21:20:33.000000 pdfminer_aemc-20231228/pdfminer/cmap/B5-H.pickle.gz
+-rw-rw-r--   0 jun        (501) staff       (20)    42549 2023-12-28 21:20:33.000000 pdfminer_aemc-20231228/pdfminer/cmap/B5-V.pickle.gz
+-rw-rw-r--   0 jun        (501) staff       (20)    42602 2023-12-28 21:20:33.000000 pdfminer_aemc-20231228/pdfminer/cmap/B5pc-H.pickle.gz
+-rw-rw-r--   0 jun        (501) staff       (20)    42557 2023-12-28 21:20:33.000000 pdfminer_aemc-20231228/pdfminer/cmap/B5pc-V.pickle.gz
+-rw-rw-r--   0 jun        (501) staff       (20)    56990 2023-12-28 21:20:33.000000 pdfminer_aemc-20231228/pdfminer/cmap/CNS-EUC-H.pickle.gz
+-rw-rw-r--   0 jun        (501) staff       (20)    56943 2023-12-28 21:20:33.000000 pdfminer_aemc-20231228/pdfminer/cmap/CNS-EUC-V.pickle.gz
+-rw-rw-r--   0 jun        (501) staff       (20)    17615 2023-12-28 21:20:33.000000 pdfminer_aemc-20231228/pdfminer/cmap/CNS1-H.pickle.gz
+-rw-rw-r--   0 jun        (501) staff       (20)    17564 2023-12-28 21:20:33.000000 pdfminer_aemc-20231228/pdfminer/cmap/CNS1-V.pickle.gz
+-rw-rw-r--   0 jun        (501) staff       (20)    21723 2023-12-28 21:20:33.000000 pdfminer_aemc-20231228/pdfminer/cmap/CNS2-H.pickle.gz
+-rw-rw-r--   0 jun        (501) staff       (20)    21723 2023-12-28 21:20:33.000000 pdfminer_aemc-20231228/pdfminer/cmap/CNS2-V.pickle.gz
+-rw-rw-r--   0 jun        (501) staff       (20)    59548 2023-12-28 21:20:33.000000 pdfminer_aemc-20231228/pdfminer/cmap/ETHK-B5-H.pickle.gz
+-rw-rw-r--   0 jun        (501) staff       (20)    59481 2023-12-28 21:20:33.000000 pdfminer_aemc-20231228/pdfminer/cmap/ETHK-B5-V.pickle.gz
+-rw-rw-r--   0 jun        (501) staff       (20)    43982 2023-12-28 21:20:33.000000 pdfminer_aemc-20231228/pdfminer/cmap/ETen-B5-H.pickle.gz
+-rw-rw-r--   0 jun        (501) staff       (20)    43924 2023-12-28 21:20:33.000000 pdfminer_aemc-20231228/pdfminer/cmap/ETen-B5-V.pickle.gz
+-rw-rw-r--   0 jun        (501) staff       (20)      320 2023-12-28 21:20:33.000000 pdfminer_aemc-20231228/pdfminer/cmap/ETenms-B5-H.pickle.gz
+-rw-rw-r--   0 jun        (501) staff       (20)      438 2023-12-28 21:20:33.000000 pdfminer_aemc-20231228/pdfminer/cmap/ETenms-B5-V.pickle.gz
+-rw-rw-r--   0 jun        (501) staff       (20)    20429 2023-12-28 21:20:33.000000 pdfminer_aemc-20231228/pdfminer/cmap/EUC-H.pickle.gz
+-rw-rw-r--   0 jun        (501) staff       (20)    20455 2023-12-28 21:20:33.000000 pdfminer_aemc-20231228/pdfminer/cmap/EUC-V.pickle.gz
+-rw-rw-r--   0 jun        (501) staff       (20)    22272 2023-12-28 21:20:33.000000 pdfminer_aemc-20231228/pdfminer/cmap/Ext-H.pickle.gz
+-rw-rw-r--   0 jun        (501) staff       (20)    25721 2023-12-28 21:20:33.000000 pdfminer_aemc-20231228/pdfminer/cmap/Ext-RKSJ-H.pickle.gz
+-rw-rw-r--   0 jun        (501) staff       (20)    25750 2023-12-28 21:20:33.000000 pdfminer_aemc-20231228/pdfminer/cmap/Ext-RKSJ-V.pickle.gz
+-rw-rw-r--   0 jun        (501) staff       (20)    22307 2023-12-28 21:20:33.000000 pdfminer_aemc-20231228/pdfminer/cmap/Ext-V.pickle.gz
+-rw-rw-r--   0 jun        (501) staff       (20)    22118 2023-12-28 21:20:33.000000 pdfminer_aemc-20231228/pdfminer/cmap/GB-EUC-H.pickle.gz
+-rw-rw-r--   0 jun        (501) staff       (20)    22111 2023-12-28 21:20:33.000000 pdfminer_aemc-20231228/pdfminer/cmap/GB-EUC-V.pickle.gz
+-rw-rw-r--   0 jun        (501) staff       (20)    21699 2023-12-28 21:20:33.000000 pdfminer_aemc-20231228/pdfminer/cmap/GB-H.pickle.gz
+-rw-rw-r--   0 jun        (501) staff       (20)    21694 2023-12-28 21:20:33.000000 pdfminer_aemc-20231228/pdfminer/cmap/GB-V.pickle.gz
+-rw-rw-r--   0 jun        (501) staff       (20)    68254 2023-12-28 21:20:33.000000 pdfminer_aemc-20231228/pdfminer/cmap/GBK-EUC-H.pickle.gz
+-rw-rw-r--   0 jun        (501) staff       (20)    68199 2023-12-28 21:20:33.000000 pdfminer_aemc-20231228/pdfminer/cmap/GBK-EUC-V.pickle.gz
+-rw-rw-r--   0 jun        (501) staff       (20)    89917 2023-12-28 21:20:33.000000 pdfminer_aemc-20231228/pdfminer/cmap/GBK2K-H.pickle.gz
+-rw-rw-r--   0 jun        (501) staff       (20)    89872 2023-12-28 21:20:33.000000 pdfminer_aemc-20231228/pdfminer/cmap/GBK2K-V.pickle.gz
+-rw-rw-r--   0 jun        (501) staff       (20)    68148 2023-12-28 21:20:33.000000 pdfminer_aemc-20231228/pdfminer/cmap/GBKp-EUC-H.pickle.gz
+-rw-rw-r--   0 jun        (501) staff       (20)    68102 2023-12-28 21:20:33.000000 pdfminer_aemc-20231228/pdfminer/cmap/GBKp-EUC-V.pickle.gz
+-rw-rw-r--   0 jun        (501) staff       (20)    23815 2023-12-28 21:20:33.000000 pdfminer_aemc-20231228/pdfminer/cmap/GBT-EUC-H.pickle.gz
+-rw-rw-r--   0 jun        (501) staff       (20)    23806 2023-12-28 21:20:33.000000 pdfminer_aemc-20231228/pdfminer/cmap/GBT-EUC-V.pickle.gz
+-rw-rw-r--   0 jun        (501) staff       (20)    23339 2023-12-28 21:20:33.000000 pdfminer_aemc-20231228/pdfminer/cmap/GBT-H.pickle.gz
+-rw-rw-r--   0 jun        (501) staff       (20)    23322 2023-12-28 21:20:33.000000 pdfminer_aemc-20231228/pdfminer/cmap/GBT-V.pickle.gz
+-rw-rw-r--   0 jun        (501) staff       (20)    23650 2023-12-28 21:20:33.000000 pdfminer_aemc-20231228/pdfminer/cmap/GBTpc-EUC-H.pickle.gz
+-rw-rw-r--   0 jun        (501) staff       (20)    23647 2023-12-28 21:20:33.000000 pdfminer_aemc-20231228/pdfminer/cmap/GBTpc-EUC-V.pickle.gz
+-rw-rw-r--   0 jun        (501) staff       (20)    21945 2023-12-28 21:20:33.000000 pdfminer_aemc-20231228/pdfminer/cmap/GBpc-EUC-H.pickle.gz
+-rw-rw-r--   0 jun        (501) staff       (20)    21956 2023-12-28 21:20:33.000000 pdfminer_aemc-20231228/pdfminer/cmap/GBpc-EUC-V.pickle.gz
+-rw-rw-r--   0 jun        (501) staff       (20)    19781 2023-12-28 21:20:33.000000 pdfminer_aemc-20231228/pdfminer/cmap/H.pickle.gz
+-rw-rw-r--   0 jun        (501) staff       (20)    45212 2023-12-28 21:20:33.000000 pdfminer_aemc-20231228/pdfminer/cmap/HKdla-B5-H.pickle.gz
+-rw-rw-r--   0 jun        (501) staff       (20)    45167 2023-12-28 21:20:33.000000 pdfminer_aemc-20231228/pdfminer/cmap/HKdla-B5-V.pickle.gz
+-rw-rw-r--   0 jun        (501) staff       (20)    44853 2023-12-28 21:20:33.000000 pdfminer_aemc-20231228/pdfminer/cmap/HKdlb-B5-H.pickle.gz
+-rw-rw-r--   0 jun        (501) staff       (20)    44816 2023-12-28 21:20:33.000000 pdfminer_aemc-20231228/pdfminer/cmap/HKdlb-B5-V.pickle.gz
+-rw-rw-r--   0 jun        (501) staff       (20)    53104 2023-12-28 21:20:33.000000 pdfminer_aemc-20231228/pdfminer/cmap/HKgccs-B5-H.pickle.gz
+-rw-rw-r--   0 jun        (501) staff       (20)    53050 2023-12-28 21:20:33.000000 pdfminer_aemc-20231228/pdfminer/cmap/HKgccs-B5-V.pickle.gz
+-rw-rw-r--   0 jun        (501) staff       (20)    43667 2023-12-28 21:20:33.000000 pdfminer_aemc-20231228/pdfminer/cmap/HKm314-B5-H.pickle.gz
+-rw-rw-r--   0 jun        (501) staff       (20)    43618 2023-12-28 21:20:33.000000 pdfminer_aemc-20231228/pdfminer/cmap/HKm314-B5-V.pickle.gz
+-rw-rw-r--   0 jun        (501) staff       (20)    44187 2023-12-28 21:20:33.000000 pdfminer_aemc-20231228/pdfminer/cmap/HKm471-B5-H.pickle.gz
+-rw-rw-r--   0 jun        (501) staff       (20)    44144 2023-12-28 21:20:33.000000 pdfminer_aemc-20231228/pdfminer/cmap/HKm471-B5-V.pickle.gz
+-rw-rw-r--   0 jun        (501) staff       (20)    59508 2023-12-28 21:20:33.000000 pdfminer_aemc-20231228/pdfminer/cmap/HKscs-B5-H.pickle.gz
+-rw-rw-r--   0 jun        (501) staff       (20)    59473 2023-12-28 21:20:33.000000 pdfminer_aemc-20231228/pdfminer/cmap/HKscs-B5-V.pickle.gz
+-rw-rw-r--   0 jun        (501) staff       (20)      840 2023-12-28 21:20:33.000000 pdfminer_aemc-20231228/pdfminer/cmap/Hankaku-H.pickle.gz
+-rw-rw-r--   0 jun        (501) staff       (20)      839 2023-12-28 21:20:33.000000 pdfminer_aemc-20231228/pdfminer/cmap/Hankaku-V.pickle.gz
+-rw-rw-r--   0 jun        (501) staff       (20)      391 2023-12-28 21:20:33.000000 pdfminer_aemc-20231228/pdfminer/cmap/Hiragana-H.pickle.gz
+-rw-rw-r--   0 jun        (501) staff       (20)      391 2023-12-28 21:20:33.000000 pdfminer_aemc-20231228/pdfminer/cmap/Hiragana-V.pickle.gz
+-rw-rw-r--   0 jun        (501) staff       (20)    24040 2023-12-28 21:20:33.000000 pdfminer_aemc-20231228/pdfminer/cmap/KSC-EUC-H.pickle.gz
+-rw-rw-r--   0 jun        (501) staff       (20)    24078 2023-12-28 21:20:33.000000 pdfminer_aemc-20231228/pdfminer/cmap/KSC-EUC-V.pickle.gz
+-rw-rw-r--   0 jun        (501) staff       (20)    23563 2023-12-28 21:20:33.000000 pdfminer_aemc-20231228/pdfminer/cmap/KSC-H.pickle.gz
+-rw-rw-r--   0 jun        (501) staff       (20)    55016 2023-12-28 21:20:33.000000 pdfminer_aemc-20231228/pdfminer/cmap/KSC-Johab-H.pickle.gz
+-rw-rw-r--   0 jun        (501) staff       (20)    55041 2023-12-28 21:20:33.000000 pdfminer_aemc-20231228/pdfminer/cmap/KSC-Johab-V.pickle.gz
+-rw-rw-r--   0 jun        (501) staff       (20)    23644 2023-12-28 21:20:33.000000 pdfminer_aemc-20231228/pdfminer/cmap/KSC-V.pickle.gz
+-rw-rw-r--   0 jun        (501) staff       (20)    51667 2023-12-28 21:20:33.000000 pdfminer_aemc-20231228/pdfminer/cmap/KSCms-UHC-H.pickle.gz
+-rw-rw-r--   0 jun        (501) staff       (20)    51788 2023-12-28 21:20:33.000000 pdfminer_aemc-20231228/pdfminer/cmap/KSCms-UHC-HW-H.pickle.gz
+-rw-rw-r--   0 jun        (501) staff       (20)    51821 2023-12-28 21:20:33.000000 pdfminer_aemc-20231228/pdfminer/cmap/KSCms-UHC-HW-V.pickle.gz
+-rw-rw-r--   0 jun        (501) staff       (20)    51698 2023-12-28 21:20:33.000000 pdfminer_aemc-20231228/pdfminer/cmap/KSCms-UHC-V.pickle.gz
+-rw-rw-r--   0 jun        (501) staff       (20)    27769 2023-12-28 21:20:33.000000 pdfminer_aemc-20231228/pdfminer/cmap/KSCpc-EUC-H.pickle.gz
+-rw-rw-r--   0 jun        (501) staff       (20)    27820 2023-12-28 21:20:33.000000 pdfminer_aemc-20231228/pdfminer/cmap/KSCpc-EUC-V.pickle.gz
+-rw-rw-r--   0 jun        (501) staff       (20)      404 2023-12-28 21:20:33.000000 pdfminer_aemc-20231228/pdfminer/cmap/Katakana-H.pickle.gz
+-rw-rw-r--   0 jun        (501) staff       (20)      404 2023-12-28 21:20:33.000000 pdfminer_aemc-20231228/pdfminer/cmap/Katakana-V.pickle.gz
+-rw-rw-r--   0 jun        (501) staff       (20)    21708 2023-12-28 21:20:33.000000 pdfminer_aemc-20231228/pdfminer/cmap/NWP-H.pickle.gz
+-rw-rw-r--   0 jun        (501) staff       (20)    21779 2023-12-28 21:20:33.000000 pdfminer_aemc-20231228/pdfminer/cmap/NWP-V.pickle.gz
+-rw-rw-r--   0 jun        (501) staff       (20)     3917 2023-12-28 21:20:33.000000 pdfminer_aemc-20231228/pdfminer/cmap/README.txt
+-rw-rw-r--   0 jun        (501) staff       (20)    23030 2023-12-28 21:20:33.000000 pdfminer_aemc-20231228/pdfminer/cmap/RKSJ-H.pickle.gz
+-rw-rw-r--   0 jun        (501) staff       (20)    23048 2023-12-28 21:20:33.000000 pdfminer_aemc-20231228/pdfminer/cmap/RKSJ-V.pickle.gz
+-rw-rw-r--   0 jun        (501) staff       (20)      394 2023-12-28 21:20:33.000000 pdfminer_aemc-20231228/pdfminer/cmap/Roman-H.pickle.gz
+-rw-rw-r--   0 jun        (501) staff       (20)      394 2023-12-28 21:20:33.000000 pdfminer_aemc-20231228/pdfminer/cmap/Roman-V.pickle.gz
+-rw-rw-r--   0 jun        (501) staff       (20)    67459 2023-12-28 21:20:33.000000 pdfminer_aemc-20231228/pdfminer/cmap/UniCNS-UCS2-H.pickle.gz
+-rw-rw-r--   0 jun        (501) staff       (20)    67395 2023-12-28 21:20:33.000000 pdfminer_aemc-20231228/pdfminer/cmap/UniCNS-UCS2-V.pickle.gz
+-rw-rw-r--   0 jun        (501) staff       (20)    87819 2023-12-28 21:20:33.000000 pdfminer_aemc-20231228/pdfminer/cmap/UniCNS-UTF16-H.pickle.gz
+-rw-rw-r--   0 jun        (501) staff       (20)    87751 2023-12-28 21:20:33.000000 pdfminer_aemc-20231228/pdfminer/cmap/UniCNS-UTF16-V.pickle.gz
+-rw-rw-r--   0 jun        (501) staff       (20)    87400 2023-12-28 21:20:33.000000 pdfminer_aemc-20231228/pdfminer/cmap/UniCNS-UTF32-H.pickle.gz
+-rw-rw-r--   0 jun        (501) staff       (20)    87327 2023-12-28 21:20:33.000000 pdfminer_aemc-20231228/pdfminer/cmap/UniCNS-UTF32-V.pickle.gz
+-rw-rw-r--   0 jun        (501) staff       (20)    82631 2023-12-28 21:20:33.000000 pdfminer_aemc-20231228/pdfminer/cmap/UniCNS-UTF8-H.pickle.gz
+-rw-rw-r--   0 jun        (501) staff       (20)    82562 2023-12-28 21:20:33.000000 pdfminer_aemc-20231228/pdfminer/cmap/UniCNS-UTF8-V.pickle.gz
+-rw-rw-r--   0 jun        (501) staff       (20)    97445 2023-12-28 21:20:33.000000 pdfminer_aemc-20231228/pdfminer/cmap/UniGB-UCS2-H.pickle.gz
+-rw-rw-r--   0 jun        (501) staff       (20)    97441 2023-12-28 21:20:33.000000 pdfminer_aemc-20231228/pdfminer/cmap/UniGB-UCS2-V.pickle.gz
+-rw-rw-r--   0 jun        (501) staff       (20)   101459 2023-12-28 21:20:33.000000 pdfminer_aemc-20231228/pdfminer/cmap/UniGB-UTF16-H.pickle.gz
+-rw-rw-r--   0 jun        (501) staff       (20)   101331 2023-12-28 21:20:33.000000 pdfminer_aemc-20231228/pdfminer/cmap/UniGB-UTF16-V.pickle.gz
+-rw-rw-r--   0 jun        (501) staff       (20)   101490 2023-12-28 21:20:33.000000 pdfminer_aemc-20231228/pdfminer/cmap/UniGB-UTF32-H.pickle.gz
+-rw-rw-r--   0 jun        (501) staff       (20)   101357 2023-12-28 21:20:33.000000 pdfminer_aemc-20231228/pdfminer/cmap/UniGB-UTF32-V.pickle.gz
+-rw-rw-r--   0 jun        (501) staff       (20)    90500 2023-12-28 21:20:33.000000 pdfminer_aemc-20231228/pdfminer/cmap/UniGB-UTF8-H.pickle.gz
+-rw-rw-r--   0 jun        (501) staff       (20)    90368 2023-12-28 21:20:33.000000 pdfminer_aemc-20231228/pdfminer/cmap/UniGB-UTF8-V.pickle.gz
+-rw-rw-r--   0 jun        (501) staff       (20)    35934 2023-12-28 21:20:33.000000 pdfminer_aemc-20231228/pdfminer/cmap/UniJIS-UCS2-H.pickle.gz
+-rw-rw-r--   0 jun        (501) staff       (20)      412 2023-12-28 21:20:33.000000 pdfminer_aemc-20231228/pdfminer/cmap/UniJIS-UCS2-HW-H.pickle.gz
+-rw-rw-r--   0 jun        (501) staff       (20)     1402 2023-12-28 21:20:33.000000 pdfminer_aemc-20231228/pdfminer/cmap/UniJIS-UCS2-HW-V.pickle.gz
+-rw-rw-r--   0 jun        (501) staff       (20)    35852 2023-12-28 21:20:33.000000 pdfminer_aemc-20231228/pdfminer/cmap/UniJIS-UCS2-V.pickle.gz
+-rw-rw-r--   0 jun        (501) staff       (20)    58054 2023-12-28 21:20:33.000000 pdfminer_aemc-20231228/pdfminer/cmap/UniJIS-UTF16-H.pickle.gz
+-rw-rw-r--   0 jun        (501) staff       (20)    57928 2023-12-28 21:20:33.000000 pdfminer_aemc-20231228/pdfminer/cmap/UniJIS-UTF16-V.pickle.gz
+-rw-rw-r--   0 jun        (501) staff       (20)    57910 2023-12-28 21:20:33.000000 pdfminer_aemc-20231228/pdfminer/cmap/UniJIS-UTF32-H.pickle.gz
+-rw-rw-r--   0 jun        (501) staff       (20)    57780 2023-12-28 21:20:33.000000 pdfminer_aemc-20231228/pdfminer/cmap/UniJIS-UTF32-V.pickle.gz
+-rw-rw-r--   0 jun        (501) staff       (20)    54764 2023-12-28 21:20:33.000000 pdfminer_aemc-20231228/pdfminer/cmap/UniJIS-UTF8-H.pickle.gz
+-rw-rw-r--   0 jun        (501) staff       (20)    54684 2023-12-28 21:20:33.000000 pdfminer_aemc-20231228/pdfminer/cmap/UniJIS-UTF8-V.pickle.gz
+-rw-rw-r--   0 jun        (501) staff       (20)    58081 2023-12-28 21:20:33.000000 pdfminer_aemc-20231228/pdfminer/cmap/UniJIS2004-UTF16-H.pickle.gz
+-rw-rw-r--   0 jun        (501) staff       (20)    57960 2023-12-28 21:20:33.000000 pdfminer_aemc-20231228/pdfminer/cmap/UniJIS2004-UTF16-V.pickle.gz
+-rw-rw-r--   0 jun        (501) staff       (20)    57940 2023-12-28 21:20:33.000000 pdfminer_aemc-20231228/pdfminer/cmap/UniJIS2004-UTF32-H.pickle.gz
+-rw-rw-r--   0 jun        (501) staff       (20)    57811 2023-12-28 21:20:33.000000 pdfminer_aemc-20231228/pdfminer/cmap/UniJIS2004-UTF32-V.pickle.gz
+-rw-rw-r--   0 jun        (501) staff       (20)    54829 2023-12-28 21:20:33.000000 pdfminer_aemc-20231228/pdfminer/cmap/UniJIS2004-UTF8-H.pickle.gz
+-rw-rw-r--   0 jun        (501) staff       (20)    54749 2023-12-28 21:20:33.000000 pdfminer_aemc-20231228/pdfminer/cmap/UniJIS2004-UTF8-V.pickle.gz
+-rw-rw-r--   0 jun        (501) staff       (20)    57903 2023-12-28 21:20:33.000000 pdfminer_aemc-20231228/pdfminer/cmap/UniJISX0213-UTF32-H.pickle.gz
+-rw-rw-r--   0 jun        (501) staff       (20)    57778 2023-12-28 21:20:33.000000 pdfminer_aemc-20231228/pdfminer/cmap/UniJISX0213-UTF32-V.pickle.gz
+-rw-rw-r--   0 jun        (501) staff       (20)    57930 2023-12-28 21:20:33.000000 pdfminer_aemc-20231228/pdfminer/cmap/UniJISX02132004-UTF32-H.pickle.gz
+-rw-rw-r--   0 jun        (501) staff       (20)    57808 2023-12-28 21:20:33.000000 pdfminer_aemc-20231228/pdfminer/cmap/UniJISX02132004-UTF32-V.pickle.gz
+-rw-rw-r--   0 jun        (501) staff       (20)    60683 2023-12-28 21:20:33.000000 pdfminer_aemc-20231228/pdfminer/cmap/UniKS-UCS2-H.pickle.gz
+-rw-rw-r--   0 jun        (501) staff       (20)    60699 2023-12-28 21:20:33.000000 pdfminer_aemc-20231228/pdfminer/cmap/UniKS-UCS2-V.pickle.gz
+-rw-rw-r--   0 jun        (501) staff       (20)    61278 2023-12-28 21:20:33.000000 pdfminer_aemc-20231228/pdfminer/cmap/UniKS-UTF16-H.pickle.gz
+-rw-rw-r--   0 jun        (501) staff       (20)    61298 2023-12-28 21:20:33.000000 pdfminer_aemc-20231228/pdfminer/cmap/UniKS-UTF16-V.pickle.gz
+-rw-rw-r--   0 jun        (501) staff       (20)    61286 2023-12-28 21:20:33.000000 pdfminer_aemc-20231228/pdfminer/cmap/UniKS-UTF32-H.pickle.gz
+-rw-rw-r--   0 jun        (501) staff       (20)    61309 2023-12-28 21:20:33.000000 pdfminer_aemc-20231228/pdfminer/cmap/UniKS-UTF32-V.pickle.gz
+-rw-rw-r--   0 jun        (501) staff       (20)    54151 2023-12-28 21:20:33.000000 pdfminer_aemc-20231228/pdfminer/cmap/UniKS-UTF8-H.pickle.gz
+-rw-rw-r--   0 jun        (501) staff       (20)    54172 2023-12-28 21:20:33.000000 pdfminer_aemc-20231228/pdfminer/cmap/UniKS-UTF8-V.pickle.gz
+-rw-rw-r--   0 jun        (501) staff       (20)    19826 2023-12-28 21:20:33.000000 pdfminer_aemc-20231228/pdfminer/cmap/V.pickle.gz
+-rw-rw-r--   0 jun        (501) staff       (20)      505 2023-12-28 21:20:33.000000 pdfminer_aemc-20231228/pdfminer/cmap/WP-Symbol-H.pickle.gz
+-rw-rw-r--   0 jun        (501) staff       (20)      505 2023-12-28 21:20:33.000000 pdfminer_aemc-20231228/pdfminer/cmap/WP-Symbol-V.pickle.gz
+-rw-rw-r--   0 jun        (501) staff       (20)   138237 2023-12-28 21:20:33.000000 pdfminer_aemc-20231228/pdfminer/cmap/to-unicode-Adobe-CNS1.pickle.gz
+-rw-rw-r--   0 jun        (501) staff       (20)   204425 2023-12-28 21:20:33.000000 pdfminer_aemc-20231228/pdfminer/cmap/to-unicode-Adobe-GB1.pickle.gz
+-rw-rw-r--   0 jun        (501) staff       (20)   112987 2023-12-28 21:20:33.000000 pdfminer_aemc-20231228/pdfminer/cmap/to-unicode-Adobe-Japan1.pickle.gz
+-rw-rw-r--   0 jun        (501) staff       (20)   120859 2023-12-28 21:20:33.000000 pdfminer_aemc-20231228/pdfminer/cmap/to-unicode-Adobe-Korea1.pickle.gz
+-rw-rw-r--   0 jun        (501) staff       (20)    16342 2024-04-24 11:07:22.000000 pdfminer_aemc-20231228/pdfminer/cmapdb.py
+-rw-rw-r--   0 jun        (501) staff       (20)    35804 2023-12-28 21:20:33.000000 pdfminer_aemc-20231228/pdfminer/converter.py
+-rw-rw-r--   0 jun        (501) staff       (20)     1654 2023-12-28 21:20:33.000000 pdfminer_aemc-20231228/pdfminer/data_structures.py
+-rw-rw-r--   0 jun        (501) staff       (20)     3983 2023-12-28 21:20:33.000000 pdfminer_aemc-20231228/pdfminer/encodingdb.py
+-rw-rw-r--   0 jun        (501) staff       (20)   112611 2023-12-28 21:20:33.000000 pdfminer_aemc-20231228/pdfminer/fontmetrics.py
+-rw-rw-r--   0 jun        (501) staff       (20)   130804 2023-12-28 21:20:33.000000 pdfminer_aemc-20231228/pdfminer/glyphlist.py
+-rw-rw-r--   0 jun        (501) staff       (20)     7276 2023-12-28 21:20:33.000000 pdfminer_aemc-20231228/pdfminer/high_level.py
+-rw-rw-r--   0 jun        (501) staff       (20)     9305 2023-12-28 21:20:33.000000 pdfminer_aemc-20231228/pdfminer/image.py
+-rw-rw-r--   0 jun        (501) staff       (20)    11391 2023-12-28 21:20:33.000000 pdfminer_aemc-20231228/pdfminer/jbig2.py
+-rw-rw-r--   0 jun        (501) staff       (20)     8531 2023-12-28 21:20:33.000000 pdfminer_aemc-20231228/pdfminer/latin_enc.py
+-rw-rw-r--   0 jun        (501) staff       (20)    35926 2024-04-24 11:12:53.000000 pdfminer_aemc-20231228/pdfminer/layout.py
+-rw-rw-r--   0 jun        (501) staff       (20)     3177 2023-12-28 21:20:33.000000 pdfminer_aemc-20231228/pdfminer/lzw.py
+-rw-rw-r--   0 jun        (501) staff       (20)      821 2023-12-28 21:20:33.000000 pdfminer_aemc-20231228/pdfminer/pdfcolor.py
+-rw-rw-r--   0 jun        (501) staff       (20)     8787 2023-12-28 21:20:33.000000 pdfminer_aemc-20231228/pdfminer/pdfdevice.py
+-rw-rw-r--   0 jun        (501) staff       (20)    37267 2023-12-28 21:20:33.000000 pdfminer_aemc-20231228/pdfminer/pdfdocument.py
+-rw-rw-r--   0 jun        (501) staff       (20)    38109 2024-04-24 11:09:47.000000 pdfminer_aemc-20231228/pdfminer/pdffont.py
+-rw-rw-r--   0 jun        (501) staff       (20)    34539 2023-12-28 21:20:33.000000 pdfminer_aemc-20231228/pdfminer/pdfinterp.py
+-rw-rw-r--   0 jun        (501) staff       (20)     6803 2023-12-28 21:20:33.000000 pdfminer_aemc-20231228/pdfminer/pdfpage.py
+-rw-rw-r--   0 jun        (501) staff       (20)     5896 2023-12-28 21:20:33.000000 pdfminer_aemc-20231228/pdfminer/pdfparser.py
+-rw-rw-r--   0 jun        (501) staff       (20)    12109 2023-12-28 21:20:33.000000 pdfminer_aemc-20231228/pdfminer/pdftypes.py
+-rwxr-xr-x   0 jun        (501) staff       (20)    19649 2023-12-28 21:20:33.000000 pdfminer_aemc-20231228/pdfminer/psparser.py
+-rw-rw-r--   0 jun        (501) staff       (20)        0 2023-12-28 21:20:33.000000 pdfminer_aemc-20231228/pdfminer/py.typed
+-rw-rw-r--   0 jun        (501) staff       (20)     1358 2023-12-28 21:20:33.000000 pdfminer_aemc-20231228/pdfminer/runlength.py
+-rw-rw-r--   0 jun        (501) staff       (20)       15 2023-12-28 21:20:33.000000 pdfminer_aemc-20231228/pdfminer/settings.py
+-rw-rw-r--   0 jun        (501) staff       (20)    20804 2023-12-28 21:20:33.000000 pdfminer_aemc-20231228/pdfminer/utils.py
+drwxr-xr-x   0 jun        (501) staff       (20)        0 2024-05-04 04:32:45.611856 pdfminer_aemc-20231228/pdfminer.aemc.egg-info/
+-rw-r--r--   0 jun        (501) staff       (20)     4144 2024-05-04 04:32:45.000000 pdfminer_aemc-20231228/pdfminer.aemc.egg-info/PKG-INFO
+-rw-r--r--   0 jun        (501) staff       (20)     6914 2024-05-04 04:32:45.000000 pdfminer_aemc-20231228/pdfminer.aemc.egg-info/SOURCES.txt
+-rw-r--r--   0 jun        (501) staff       (20)        1 2024-05-04 04:32:45.000000 pdfminer_aemc-20231228/pdfminer.aemc.egg-info/dependency_links.txt
+-rw-r--r--   0 jun        (501) staff       (20)      194 2024-05-04 04:32:45.000000 pdfminer_aemc-20231228/pdfminer.aemc.egg-info/requires.txt
+-rw-r--r--   0 jun        (501) staff       (20)        9 2024-05-04 04:32:45.000000 pdfminer_aemc-20231228/pdfminer.aemc.egg-info/top_level.txt
+-rw-r--r--   0 jun        (501) staff       (20)       38 2024-05-04 04:32:45.612825 pdfminer_aemc-20231228/setup.cfg
+-rw-rw-r--   0 jun        (501) staff       (20)     1980 2024-04-24 11:00:36.000000 pdfminer_aemc-20231228/setup.py
+drwxr-xr-x   0 jun        (501) staff       (20)        0 2024-05-04 04:32:45.610459 pdfminer_aemc-20231228/tests/
+-rw-rw-r--   0 jun        (501) staff       (20)     9692 2023-12-28 21:20:33.000000 pdfminer_aemc-20231228/tests/test_converter.py
+-rw-rw-r--   0 jun        (501) staff       (20)     5420 2023-12-28 21:20:33.000000 pdfminer_aemc-20231228/tests/test_encodingdb.py
+-rw-rw-r--   0 jun        (501) staff       (20)      779 2023-12-28 21:20:33.000000 pdfminer_aemc-20231228/tests/test_font_size.py
+-rw-rw-r--   0 jun        (501) staff       (20)     6451 2023-12-28 21:20:33.000000 pdfminer_aemc-20231228/tests/test_highlevel_extracttext.py
+-rw-rw-r--   0 jun        (501) staff       (20)     5038 2023-12-28 21:20:33.000000 pdfminer_aemc-20231228/tests/test_layout.py
+-rw-rw-r--   0 jun        (501) staff       (20)     1809 2023-12-28 21:20:33.000000 pdfminer_aemc-20231228/tests/test_pdfdocument.py
+-rw-rw-r--   0 jun        (501) staff       (20)     3972 2023-12-28 21:20:33.000000 pdfminer_aemc-20231228/tests/test_pdfencoding.py
+-rw-rw-r--   0 jun        (501) staff       (20)      604 2023-12-28 21:20:33.000000 pdfminer_aemc-20231228/tests/test_pdffont.py
+-rw-rw-r--   0 jun        (501) staff       (20)     4532 2023-12-28 21:20:33.000000 pdfminer_aemc-20231228/tests/test_pdfminer_ccitt.py
+-rw-rw-r--   0 jun        (501) staff       (20)     1598 2023-12-28 21:20:33.000000 pdfminer_aemc-20231228/tests/test_pdfminer_crypto.py
+-rw-rw-r--   0 jun        (501) staff       (20)     3405 2023-12-28 21:20:33.000000 pdfminer_aemc-20231228/tests/test_pdfminer_psparser.py
+-rw-rw-r--   0 jun        (501) staff       (20)      582 2023-12-28 21:20:33.000000 pdfminer_aemc-20231228/tests/test_pdfpage.py
+-rw-rw-r--   0 jun        (501) staff       (20)     1505 2023-12-28 21:20:33.000000 pdfminer_aemc-20231228/tests/test_tools_dumppdf.py
+-rw-rw-r--   0 jun        (501) staff       (20)     5497 2023-12-28 21:20:33.000000 pdfminer_aemc-20231228/tests/test_tools_pdf2txt.py
+-rw-rw-r--   0 jun        (501) staff       (20)     3912 2023-12-28 21:20:33.000000 pdfminer_aemc-20231228/tests/test_utils.py
+drwxr-xr-x   0 jun        (501) staff       (20)        0 2024-05-04 04:32:45.611675 pdfminer_aemc-20231228/tools/
+-rw-rw-r--   0 jun        (501) staff       (20)        0 2023-12-28 21:20:33.000000 pdfminer_aemc-20231228/tools/__init__.py
+-rwxr-xr-x   0 jun        (501) staff       (20)     1646 2023-12-28 21:20:33.000000 pdfminer_aemc-20231228/tools/conv_afm.py
+-rwxr-xr-x   0 jun        (501) staff       (20)     6089 2023-12-28 21:20:33.000000 pdfminer_aemc-20231228/tools/conv_cmap.py
+-rwxr-xr-x   0 jun        (501) staff       (20)      911 2023-12-28 21:20:33.000000 pdfminer_aemc-20231228/tools/conv_glyphlist.py
+-rwxr-xr-x   0 jun        (501) staff       (20)    14316 2023-12-28 21:20:33.000000 pdfminer_aemc-20231228/tools/dumppdf.py
+-rwxr-xr-x   0 jun        (501) staff       (20)     9779 2023-12-28 21:20:33.000000 pdfminer_aemc-20231228/tools/pdf2txt.py
+-rw-rw-r--   0 jun        (501) staff       (20)     6266 2023-12-28 21:20:33.000000 pdfminer_aemc-20231228/tools/pdfdiff.py
+-rwxr-xr-x   0 jun        (501) staff       (20)     2761 2023-12-28 21:20:33.000000 pdfminer_aemc-20231228/tools/pdfstats.py
+-rw-rw-r--   0 jun        (501) staff       (20)     1415 2023-12-28 21:20:33.000000 pdfminer_aemc-20231228/tools/prof.py
```

### Comparing `pdfminer.aemc-20221118/CHANGELOG.md` & `pdfminer_aemc-20231228/CHANGELOG.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,36 +1,56 @@
 # Changelog
 All notable changes in pdfminer.six will be documented in this file.
 
 The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/).
 
 ## [Unreleased]
 
+Nothing yet. 
+
+## [20231228]
+
+### Removed
+- Support for Python 3.6 and 3.7 ([#921](https://github.com/pdfminer/pdfminer.six/pull/921))
+
 ### Added
 
 - Output converter for the hOCR format ([#651](https://github.com/pdfminer/pdfminer.six/pull/651))
 - Font name aliases for Arial, Courier New and Times New Roman ([#790](https://github.com/pdfminer/pdfminer.six/pull/790))
 - Documentation on why special characters can sometimes not be extracted ([#829](https://github.com/pdfminer/pdfminer.six/pull/829))
+- Storing Bezier path and dashing style of line in LTCurve ([#801](https://github.com/pdfminer/pdfminer.six/pull/801))
 
 ### Fixed
 
+- Broken CI/CD pipeline by setting upper version limit for black, mypy, pip and setuptools ([#921](https://github.com/pdfminer/pdfminer.six/pull/921))
+- `flake8` failures ([#921](https://github.com/pdfminer/pdfminer.six/pull/921))
 - `ValueError` when bmp images with 1 bit channel are decoded ([#773](https://github.com/pdfminer/pdfminer.six/issues/773))
 - `ValueError` when trying to decrypt empty metadata values ([#766](https://github.com/pdfminer/pdfminer.six/issues/766))
 - Sphinx errors during building of documentation ([#760](https://github.com/pdfminer/pdfminer.six/pull/760))
 - `TypeError` when getting default width of font ([#720](https://github.com/pdfminer/pdfminer.six/issues/720))
 - Installing typing-extensions on Python 3.6 and 3.7 ([#775](https://github.com/pdfminer/pdfminer.six/pull/775))
 - `TypeError` in cmapdb.py when parsing null characters ([#768](https://github.com/pdfminer/pdfminer.six/pull/768))
 - Color "convenience operators" now (per spec) also set color space ([#794](https://github.com/pdfminer/pdfminer.six/pull/794))
 - `ValueError` when extracting images, due to breaking changes in Pillow ([#827](https://github.com/pdfminer/pdfminer.six/pull/827))
 - Small typo's and issues in the documentation ([#828](https://github.com/pdfminer/pdfminer.six/pull/828))
+- Ignore non-Unicode cmaps in TrueType fonts ([#806](https://github.com/pdfminer/pdfminer.six/pull/806))
+
+### Changed
+
+- Using non-hardcoded version string and setuptools-git-versioning to enable installation from source and building on Python 3.12 ([#922](https://github.com/pdfminer/pdfminer.six/issues/922))
+
 
 ### Deprecated
 
 - Usage of `if __name__ == "__main__"` where it was only intended for testing purposes ([#756](https://github.com/pdfminer/pdfminer.six/pull/756))
 
+### Removed
+
+- Support for Python 3.6 and 3.7 because they are end-of-life ([#923](https://github.com/pdfminer/pdfminer.six/pull/923))
+
 ## [20220524]
 
 ### Fixed
 
 - Ignoring (invalid) path constructors that do not begin with `m` ([#749](https://github.com/pdfminer/pdfminer.six/pull/749))
 
 ### Changed
```

### Comparing `pdfminer.aemc-20221118/CONTRIBUTING.md` & `pdfminer_aemc-20231228/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `pdfminer.aemc-20221118/LICENSE` & `pdfminer_aemc-20231228/LICENSE`

 * *Files identical despite different names*

### Comparing `pdfminer.aemc-20221118/Makefile` & `pdfminer_aemc-20231228/Makefile`

 * *Files identical despite different names*

### Comparing `pdfminer.aemc-20221118/PKG-INFO` & `pdfminer_aemc-20231228/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,32 +1,46 @@
 Metadata-Version: 2.1
 Name: pdfminer.aemc
-Version: 20221118
+Version: 20231228
 Summary: PDF parser and analyzer
 Home-page: https://github.com/pdfminer/pdfminer.aemc
 Author: Yusuke Shinyama + Philippe Guglielmetti + Liew Chun Fui
 Author-email: wargreymon28@gmail.com
 License: MIT/X
 Keywords: pdf parser,pdf converter,layout analysis,text mining
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Topic :: Text Processing
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: charset-normalizer>=2.0.0
+Requires-Dist: cryptography>=36.0.0
+Requires-Dist: typing_extensions; python_version < "3.8"
+Requires-Dist: importlib_metadata; python_version < "3.8"
 Provides-Extra: dev
+Requires-Dist: pytest; extra == "dev"
+Requires-Dist: nox; extra == "dev"
+Requires-Dist: black; extra == "dev"
+Requires-Dist: mypy==0.931; extra == "dev"
 Provides-Extra: docs
+Requires-Dist: sphinx; extra == "docs"
+Requires-Dist: sphinx-argparse; extra == "docs"
 Provides-Extra: image
-License-File: LICENSE
+Requires-Dist: Pillow; extra == "image"
 
 pdfminer.six
 ============
 
 [![Continuous integration](https://github.com/pdfminer/pdfminer.six/actions/workflows/actions.yml/badge.svg)](https://github.com/pdfminer/pdfminer.six/actions/workflows/actions.yml)
 [![PyPI version](https://img.shields.io/pypi/v/pdfminer.six.svg)](https://pypi.python.org/pypi/pdfminer.six/)
 [![gitter](https://badges.gitter.im/pdfminer-six/Lobby.svg)](https://gitter.im/pdfminer-six/Lobby?utm_source=badge&utm_medium)
@@ -61,15 +75,15 @@
 * Table of contents extraction.
 * Tagged contents extraction.
 * Automatic layout analysis.
 
 How to use
 ----------
 
-* Install Python 3.6 or newer.
+* Install Python 3.8 or newer.
 * Install pdfminer.six.
 
   `pip install pdfminer.six`
 
 * (Optionally) install extra dependencies for extracting images.
 
   `pip install 'pdfminer.six[image]'`
```

### Comparing `pdfminer.aemc-20221118/README.md` & `pdfminer_aemc-20231228/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -35,15 +35,15 @@
 * Table of contents extraction.
 * Tagged contents extraction.
 * Automatic layout analysis.
 
 How to use
 ----------
 
-* Install Python 3.6 or newer.
+* Install Python 3.8 or newer.
 * Install pdfminer.six.
 
   `pip install pdfminer.six`
 
 * (Optionally) install extra dependencies for extracting images.
 
   `pip install 'pdfminer.six[image]'`
```

### Comparing `pdfminer.aemc-20221118/cmaprsrc/README.txt` & `pdfminer_aemc-20231228/cmaprsrc/README.txt`

 * *Files identical despite different names*

### Comparing `pdfminer.aemc-20221118/cmaprsrc/cid2code_Adobe_CNS1.txt` & `pdfminer_aemc-20231228/cmaprsrc/cid2code_Adobe_CNS1.txt`

 * *Files identical despite different names*

### Comparing `pdfminer.aemc-20221118/cmaprsrc/cid2code_Adobe_GB1.txt` & `pdfminer_aemc-20231228/cmaprsrc/cid2code_Adobe_GB1.txt`

 * *Files identical despite different names*

### Comparing `pdfminer.aemc-20221118/cmaprsrc/cid2code_Adobe_Japan1.txt` & `pdfminer_aemc-20231228/cmaprsrc/cid2code_Adobe_Japan1.txt`

 * *Files identical despite different names*

### Comparing `pdfminer.aemc-20221118/cmaprsrc/cid2code_Adobe_Korea1.txt` & `pdfminer_aemc-20231228/cmaprsrc/cid2code_Adobe_Korea1.txt`

 * *Files identical despite different names*

### Comparing `pdfminer.aemc-20221118/noxfile.py` & `pdfminer_aemc-20231228/noxfile.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 import os
 
 import nox
 
 
-PYTHON_ALL_VERSIONS = ["3.6", "3.7", "3.8", "3.9", "3.10"]
+PYTHON_ALL_VERSIONS = ["3.8", "3.9", "3.10", "3.11", "3.12"]
 PYTHON_MODULES = ["pdfminer", "tools", "tests", "noxfile.py", "setup.py"]
 
 
 @nox.session
 def format(session):
-    session.install("black")
+    session.install("black<23")
     # Format files locally with black, but only check in cicd
     if "CI" in os.environ:
         session.run("black", "--check", *PYTHON_MODULES)
     else:
         session.run("black", *PYTHON_MODULES)
 
 
@@ -21,32 +21,36 @@
 def lint(session):
     session.install("flake8")
     session.run("flake8", *PYTHON_MODULES, "--count", "--statistics")
 
 
 @nox.session
 def types(session):
-    session.install("mypy")
+    session.install("mypy<1")
     session.run(
         "mypy",
         "--install-types",
         "--non-interactive",
         "--show-error-codes",
         *PYTHON_MODULES,
     )
 
 
 @nox.session(python=PYTHON_ALL_VERSIONS)
 def tests(session):
+    session.install("pip")
+    session.install("setuptools")
     session.install("-e", ".[dev]")
     session.run("pytest")
 
 
 @nox.session
 def docs(session):
+    session.install("pip")
+    session.install("setuptools")
     session.install("-e", ".[docs]")
     session.run(
         "python", "-m", "sphinx", "-b", "html", "docs/source", "docs/build/html"
     )
     session.run(
         "python", "-m", "sphinx", "-b", "doctest", "docs/source", "docs/build/doctest"
     )
```

### Comparing `pdfminer.aemc-20221118/pdfminer/_saslprep.py` & `pdfminer_aemc-20231228/pdfminer/_saslprep.py`

 * *Files identical despite different names*

### Comparing `pdfminer.aemc-20221118/pdfminer/arcfour.py` & `pdfminer_aemc-20231228/pdfminer/arcfour.py`

 * *Files identical despite different names*

### Comparing `pdfminer.aemc-20221118/pdfminer/ascii85.py` & `pdfminer_aemc-20231228/pdfminer/ascii85.py`

 * *Files identical despite different names*

### Comparing `pdfminer.aemc-20221118/pdfminer/ccitt.py` & `pdfminer_aemc-20231228/pdfminer/ccitt.py`

 * *Files identical despite different names*

### Comparing `pdfminer.aemc-20221118/pdfminer/cmap/78-EUC-H.pickle.gz` & `pdfminer_aemc-20231228/pdfminer/cmap/78-EUC-H.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer.aemc-20221118/pdfminer/cmap/78-EUC-V.pickle.gz` & `pdfminer_aemc-20231228/pdfminer/cmap/78-EUC-V.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer.aemc-20221118/pdfminer/cmap/78-H.pickle.gz` & `pdfminer_aemc-20231228/pdfminer/cmap/78-H.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer.aemc-20221118/pdfminer/cmap/78-RKSJ-H.pickle.gz` & `pdfminer_aemc-20231228/pdfminer/cmap/78-RKSJ-H.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer.aemc-20221118/pdfminer/cmap/78-RKSJ-V.pickle.gz` & `pdfminer_aemc-20231228/pdfminer/cmap/78-RKSJ-V.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer.aemc-20221118/pdfminer/cmap/78-V.pickle.gz` & `pdfminer_aemc-20231228/pdfminer/cmap/78-V.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer.aemc-20221118/pdfminer/cmap/78ms-RKSJ-H.pickle.gz` & `pdfminer_aemc-20231228/pdfminer/cmap/78ms-RKSJ-H.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer.aemc-20221118/pdfminer/cmap/78ms-RKSJ-V.pickle.gz` & `pdfminer_aemc-20231228/pdfminer/cmap/78ms-RKSJ-V.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer.aemc-20221118/pdfminer/cmap/83pv-RKSJ-H.pickle.gz` & `pdfminer_aemc-20231228/pdfminer/cmap/83pv-RKSJ-H.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer.aemc-20221118/pdfminer/cmap/83pv-RKSJ-V.pickle.gz` & `pdfminer_aemc-20231228/pdfminer/cmap/83pv-RKSJ-V.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer.aemc-20221118/pdfminer/cmap/90ms-RKSJ-H.pickle.gz` & `pdfminer_aemc-20231228/pdfminer/cmap/90ms-RKSJ-H.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer.aemc-20221118/pdfminer/cmap/90ms-RKSJ-V.pickle.gz` & `pdfminer_aemc-20231228/pdfminer/cmap/90ms-RKSJ-V.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer.aemc-20221118/pdfminer/cmap/90msp-RKSJ-H.pickle.gz` & `pdfminer_aemc-20231228/pdfminer/cmap/90msp-RKSJ-H.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer.aemc-20221118/pdfminer/cmap/90msp-RKSJ-V.pickle.gz` & `pdfminer_aemc-20231228/pdfminer/cmap/90msp-RKSJ-V.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer.aemc-20221118/pdfminer/cmap/90pv-RKSJ-H.pickle.gz` & `pdfminer_aemc-20231228/pdfminer/cmap/90pv-RKSJ-H.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer.aemc-20221118/pdfminer/cmap/90pv-RKSJ-V.pickle.gz` & `pdfminer_aemc-20231228/pdfminer/cmap/90pv-RKSJ-V.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer.aemc-20221118/pdfminer/cmap/Add-H.pickle.gz` & `pdfminer_aemc-20231228/pdfminer/cmap/Add-H.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer.aemc-20221118/pdfminer/cmap/Add-RKSJ-H.pickle.gz` & `pdfminer_aemc-20231228/pdfminer/cmap/Add-RKSJ-H.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer.aemc-20221118/pdfminer/cmap/Add-RKSJ-V.pickle.gz` & `pdfminer_aemc-20231228/pdfminer/cmap/Add-RKSJ-V.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer.aemc-20221118/pdfminer/cmap/Add-V.pickle.gz` & `pdfminer_aemc-20231228/pdfminer/cmap/Add-V.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer.aemc-20221118/pdfminer/cmap/B5-H.pickle.gz` & `pdfminer_aemc-20231228/pdfminer/cmap/B5-H.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer.aemc-20221118/pdfminer/cmap/B5-V.pickle.gz` & `pdfminer_aemc-20231228/pdfminer/cmap/B5-V.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer.aemc-20221118/pdfminer/cmap/B5pc-H.pickle.gz` & `pdfminer_aemc-20231228/pdfminer/cmap/B5pc-H.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer.aemc-20221118/pdfminer/cmap/B5pc-V.pickle.gz` & `pdfminer_aemc-20231228/pdfminer/cmap/B5pc-V.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer.aemc-20221118/pdfminer/cmap/CNS-EUC-H.pickle.gz` & `pdfminer_aemc-20231228/pdfminer/cmap/CNS-EUC-H.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer.aemc-20221118/pdfminer/cmap/CNS-EUC-V.pickle.gz` & `pdfminer_aemc-20231228/pdfminer/cmap/CNS-EUC-V.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer.aemc-20221118/pdfminer/cmap/CNS1-H.pickle.gz` & `pdfminer_aemc-20231228/pdfminer/cmap/CNS1-H.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer.aemc-20221118/pdfminer/cmap/CNS1-V.pickle.gz` & `pdfminer_aemc-20231228/pdfminer/cmap/CNS1-V.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer.aemc-20221118/pdfminer/cmap/CNS2-H.pickle.gz` & `pdfminer_aemc-20231228/pdfminer/cmap/CNS2-H.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer.aemc-20221118/pdfminer/cmap/CNS2-V.pickle.gz` & `pdfminer_aemc-20231228/pdfminer/cmap/CNS2-V.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer.aemc-20221118/pdfminer/cmap/ETHK-B5-H.pickle.gz` & `pdfminer_aemc-20231228/pdfminer/cmap/ETHK-B5-H.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer.aemc-20221118/pdfminer/cmap/ETHK-B5-V.pickle.gz` & `pdfminer_aemc-20231228/pdfminer/cmap/ETHK-B5-V.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer.aemc-20221118/pdfminer/cmap/ETen-B5-H.pickle.gz` & `pdfminer_aemc-20231228/pdfminer/cmap/ETen-B5-H.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer.aemc-20221118/pdfminer/cmap/ETen-B5-V.pickle.gz` & `pdfminer_aemc-20231228/pdfminer/cmap/ETen-B5-V.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer.aemc-20221118/pdfminer/cmap/EUC-H.pickle.gz` & `pdfminer_aemc-20231228/pdfminer/cmap/EUC-H.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer.aemc-20221118/pdfminer/cmap/EUC-V.pickle.gz` & `pdfminer_aemc-20231228/pdfminer/cmap/EUC-V.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer.aemc-20221118/pdfminer/cmap/Ext-H.pickle.gz` & `pdfminer_aemc-20231228/pdfminer/cmap/Ext-H.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer.aemc-20221118/pdfminer/cmap/Ext-RKSJ-H.pickle.gz` & `pdfminer_aemc-20231228/pdfminer/cmap/Ext-RKSJ-H.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer.aemc-20221118/pdfminer/cmap/Ext-RKSJ-V.pickle.gz` & `pdfminer_aemc-20231228/pdfminer/cmap/Ext-RKSJ-V.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer.aemc-20221118/pdfminer/cmap/Ext-V.pickle.gz` & `pdfminer_aemc-20231228/pdfminer/cmap/Ext-V.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer.aemc-20221118/pdfminer/cmap/GB-EUC-H.pickle.gz` & `pdfminer_aemc-20231228/pdfminer/cmap/GB-EUC-H.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer.aemc-20221118/pdfminer/cmap/GB-EUC-V.pickle.gz` & `pdfminer_aemc-20231228/pdfminer/cmap/GB-EUC-V.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer.aemc-20221118/pdfminer/cmap/GB-H.pickle.gz` & `pdfminer_aemc-20231228/pdfminer/cmap/GB-H.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer.aemc-20221118/pdfminer/cmap/GB-V.pickle.gz` & `pdfminer_aemc-20231228/pdfminer/cmap/GB-V.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer.aemc-20221118/pdfminer/cmap/GBK-EUC-H.pickle.gz` & `pdfminer_aemc-20231228/pdfminer/cmap/GBK-EUC-H.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer.aemc-20221118/pdfminer/cmap/GBK-EUC-V.pickle.gz` & `pdfminer_aemc-20231228/pdfminer/cmap/GBK-EUC-V.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer.aemc-20221118/pdfminer/cmap/GBK2K-H.pickle.gz` & `pdfminer_aemc-20231228/pdfminer/cmap/GBK2K-H.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer.aemc-20221118/pdfminer/cmap/GBK2K-V.pickle.gz` & `pdfminer_aemc-20231228/pdfminer/cmap/GBK2K-V.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer.aemc-20221118/pdfminer/cmap/GBKp-EUC-H.pickle.gz` & `pdfminer_aemc-20231228/pdfminer/cmap/GBKp-EUC-H.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer.aemc-20221118/pdfminer/cmap/GBKp-EUC-V.pickle.gz` & `pdfminer_aemc-20231228/pdfminer/cmap/GBKp-EUC-V.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer.aemc-20221118/pdfminer/cmap/GBT-EUC-H.pickle.gz` & `pdfminer_aemc-20231228/pdfminer/cmap/GBT-EUC-H.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer.aemc-20221118/pdfminer/cmap/GBT-EUC-V.pickle.gz` & `pdfminer_aemc-20231228/pdfminer/cmap/GBT-EUC-V.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer.aemc-20221118/pdfminer/cmap/GBT-H.pickle.gz` & `pdfminer_aemc-20231228/pdfminer/cmap/GBT-H.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer.aemc-20221118/pdfminer/cmap/GBT-V.pickle.gz` & `pdfminer_aemc-20231228/pdfminer/cmap/GBT-V.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer.aemc-20221118/pdfminer/cmap/GBTpc-EUC-H.pickle.gz` & `pdfminer_aemc-20231228/pdfminer/cmap/GBTpc-EUC-H.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer.aemc-20221118/pdfminer/cmap/GBTpc-EUC-V.pickle.gz` & `pdfminer_aemc-20231228/pdfminer/cmap/GBTpc-EUC-V.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer.aemc-20221118/pdfminer/cmap/GBpc-EUC-H.pickle.gz` & `pdfminer_aemc-20231228/pdfminer/cmap/GBpc-EUC-H.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer.aemc-20221118/pdfminer/cmap/GBpc-EUC-V.pickle.gz` & `pdfminer_aemc-20231228/pdfminer/cmap/GBpc-EUC-V.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer.aemc-20221118/pdfminer/cmap/H.pickle.gz` & `pdfminer_aemc-20231228/pdfminer/cmap/H.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer.aemc-20221118/pdfminer/cmap/HKdla-B5-H.pickle.gz` & `pdfminer_aemc-20231228/pdfminer/cmap/HKdla-B5-H.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer.aemc-20221118/pdfminer/cmap/HKdla-B5-V.pickle.gz` & `pdfminer_aemc-20231228/pdfminer/cmap/HKdla-B5-V.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer.aemc-20221118/pdfminer/cmap/HKdlb-B5-H.pickle.gz` & `pdfminer_aemc-20231228/pdfminer/cmap/HKdlb-B5-H.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer.aemc-20221118/pdfminer/cmap/HKdlb-B5-V.pickle.gz` & `pdfminer_aemc-20231228/pdfminer/cmap/HKdlb-B5-V.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer.aemc-20221118/pdfminer/cmap/HKgccs-B5-H.pickle.gz` & `pdfminer_aemc-20231228/pdfminer/cmap/HKgccs-B5-H.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer.aemc-20221118/pdfminer/cmap/HKgccs-B5-V.pickle.gz` & `pdfminer_aemc-20231228/pdfminer/cmap/HKgccs-B5-V.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer.aemc-20221118/pdfminer/cmap/HKm314-B5-H.pickle.gz` & `pdfminer_aemc-20231228/pdfminer/cmap/HKm314-B5-H.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer.aemc-20221118/pdfminer/cmap/HKm314-B5-V.pickle.gz` & `pdfminer_aemc-20231228/pdfminer/cmap/HKm314-B5-V.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer.aemc-20221118/pdfminer/cmap/HKm471-B5-H.pickle.gz` & `pdfminer_aemc-20231228/pdfminer/cmap/HKm471-B5-H.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer.aemc-20221118/pdfminer/cmap/HKm471-B5-V.pickle.gz` & `pdfminer_aemc-20231228/pdfminer/cmap/HKm471-B5-V.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer.aemc-20221118/pdfminer/cmap/HKscs-B5-H.pickle.gz` & `pdfminer_aemc-20231228/pdfminer/cmap/HKscs-B5-H.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer.aemc-20221118/pdfminer/cmap/HKscs-B5-V.pickle.gz` & `pdfminer_aemc-20231228/pdfminer/cmap/HKscs-B5-V.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer.aemc-20221118/pdfminer/cmap/Hankaku-H.pickle.gz` & `pdfminer_aemc-20231228/pdfminer/cmap/Hankaku-H.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer.aemc-20221118/pdfminer/cmap/Hankaku-V.pickle.gz` & `pdfminer_aemc-20231228/pdfminer/cmap/Hankaku-V.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer.aemc-20221118/pdfminer/cmap/KSC-EUC-H.pickle.gz` & `pdfminer_aemc-20231228/pdfminer/cmap/KSC-EUC-H.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer.aemc-20221118/pdfminer/cmap/KSC-EUC-V.pickle.gz` & `pdfminer_aemc-20231228/pdfminer/cmap/KSC-EUC-V.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer.aemc-20221118/pdfminer/cmap/KSC-H.pickle.gz` & `pdfminer_aemc-20231228/pdfminer/cmap/KSC-H.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer.aemc-20221118/pdfminer/cmap/KSC-Johab-H.pickle.gz` & `pdfminer_aemc-20231228/pdfminer/cmap/KSC-Johab-H.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer.aemc-20221118/pdfminer/cmap/KSC-Johab-V.pickle.gz` & `pdfminer_aemc-20231228/pdfminer/cmap/KSC-Johab-V.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer.aemc-20221118/pdfminer/cmap/KSC-V.pickle.gz` & `pdfminer_aemc-20231228/pdfminer/cmap/KSC-V.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer.aemc-20221118/pdfminer/cmap/KSCms-UHC-H.pickle.gz` & `pdfminer_aemc-20231228/pdfminer/cmap/KSCms-UHC-H.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer.aemc-20221118/pdfminer/cmap/KSCms-UHC-HW-H.pickle.gz` & `pdfminer_aemc-20231228/pdfminer/cmap/KSCms-UHC-HW-H.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer.aemc-20221118/pdfminer/cmap/KSCms-UHC-HW-V.pickle.gz` & `pdfminer_aemc-20231228/pdfminer/cmap/KSCms-UHC-HW-V.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer.aemc-20221118/pdfminer/cmap/KSCms-UHC-V.pickle.gz` & `pdfminer_aemc-20231228/pdfminer/cmap/KSCms-UHC-V.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer.aemc-20221118/pdfminer/cmap/KSCpc-EUC-H.pickle.gz` & `pdfminer_aemc-20231228/pdfminer/cmap/KSCpc-EUC-H.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer.aemc-20221118/pdfminer/cmap/KSCpc-EUC-V.pickle.gz` & `pdfminer_aemc-20231228/pdfminer/cmap/KSCpc-EUC-V.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer.aemc-20221118/pdfminer/cmap/NWP-H.pickle.gz` & `pdfminer_aemc-20231228/pdfminer/cmap/NWP-H.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer.aemc-20221118/pdfminer/cmap/NWP-V.pickle.gz` & `pdfminer_aemc-20231228/pdfminer/cmap/NWP-V.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer.aemc-20221118/pdfminer/cmap/README.txt` & `pdfminer_aemc-20231228/pdfminer/cmap/README.txt`

 * *Files identical despite different names*

### Comparing `pdfminer.aemc-20221118/pdfminer/cmap/RKSJ-H.pickle.gz` & `pdfminer_aemc-20231228/pdfminer/cmap/RKSJ-H.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer.aemc-20221118/pdfminer/cmap/RKSJ-V.pickle.gz` & `pdfminer_aemc-20231228/pdfminer/cmap/RKSJ-V.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer.aemc-20221118/pdfminer/cmap/UniCNS-UCS2-H.pickle.gz` & `pdfminer_aemc-20231228/pdfminer/cmap/UniCNS-UCS2-H.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer.aemc-20221118/pdfminer/cmap/UniCNS-UCS2-V.pickle.gz` & `pdfminer_aemc-20231228/pdfminer/cmap/UniCNS-UCS2-V.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer.aemc-20221118/pdfminer/cmap/UniCNS-UTF16-H.pickle.gz` & `pdfminer_aemc-20231228/pdfminer/cmap/UniCNS-UTF16-H.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer.aemc-20221118/pdfminer/cmap/UniCNS-UTF16-V.pickle.gz` & `pdfminer_aemc-20231228/pdfminer/cmap/UniCNS-UTF16-V.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer.aemc-20221118/pdfminer/cmap/UniCNS-UTF32-H.pickle.gz` & `pdfminer_aemc-20231228/pdfminer/cmap/UniCNS-UTF32-H.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer.aemc-20221118/pdfminer/cmap/UniCNS-UTF32-V.pickle.gz` & `pdfminer_aemc-20231228/pdfminer/cmap/UniCNS-UTF32-V.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer.aemc-20221118/pdfminer/cmap/UniCNS-UTF8-H.pickle.gz` & `pdfminer_aemc-20231228/pdfminer/cmap/UniCNS-UTF8-H.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer.aemc-20221118/pdfminer/cmap/UniCNS-UTF8-V.pickle.gz` & `pdfminer_aemc-20231228/pdfminer/cmap/UniCNS-UTF8-V.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer.aemc-20221118/pdfminer/cmap/UniGB-UCS2-H.pickle.gz` & `pdfminer_aemc-20231228/pdfminer/cmap/UniGB-UCS2-H.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer.aemc-20221118/pdfminer/cmap/UniGB-UCS2-V.pickle.gz` & `pdfminer_aemc-20231228/pdfminer/cmap/UniGB-UCS2-V.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer.aemc-20221118/pdfminer/cmap/UniGB-UTF16-H.pickle.gz` & `pdfminer_aemc-20231228/pdfminer/cmap/UniGB-UTF16-H.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer.aemc-20221118/pdfminer/cmap/UniGB-UTF16-V.pickle.gz` & `pdfminer_aemc-20231228/pdfminer/cmap/UniGB-UTF16-V.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer.aemc-20221118/pdfminer/cmap/UniGB-UTF32-H.pickle.gz` & `pdfminer_aemc-20231228/pdfminer/cmap/UniGB-UTF32-H.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer.aemc-20221118/pdfminer/cmap/UniGB-UTF32-V.pickle.gz` & `pdfminer_aemc-20231228/pdfminer/cmap/UniGB-UTF32-V.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer.aemc-20221118/pdfminer/cmap/UniGB-UTF8-H.pickle.gz` & `pdfminer_aemc-20231228/pdfminer/cmap/UniGB-UTF8-H.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer.aemc-20221118/pdfminer/cmap/UniGB-UTF8-V.pickle.gz` & `pdfminer_aemc-20231228/pdfminer/cmap/UniGB-UTF8-V.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer.aemc-20221118/pdfminer/cmap/UniJIS-UCS2-H.pickle.gz` & `pdfminer_aemc-20231228/pdfminer/cmap/UniJIS-UCS2-H.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer.aemc-20221118/pdfminer/cmap/UniJIS-UCS2-HW-V.pickle.gz` & `pdfminer_aemc-20231228/pdfminer/cmap/UniJIS-UCS2-HW-V.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer.aemc-20221118/pdfminer/cmap/UniJIS-UCS2-V.pickle.gz` & `pdfminer_aemc-20231228/pdfminer/cmap/UniJIS-UCS2-V.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer.aemc-20221118/pdfminer/cmap/UniJIS-UTF16-H.pickle.gz` & `pdfminer_aemc-20231228/pdfminer/cmap/UniJIS-UTF16-H.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer.aemc-20221118/pdfminer/cmap/UniJIS-UTF16-V.pickle.gz` & `pdfminer_aemc-20231228/pdfminer/cmap/UniJIS-UTF16-V.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer.aemc-20221118/pdfminer/cmap/UniJIS-UTF32-H.pickle.gz` & `pdfminer_aemc-20231228/pdfminer/cmap/UniJIS-UTF32-H.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer.aemc-20221118/pdfminer/cmap/UniJIS-UTF32-V.pickle.gz` & `pdfminer_aemc-20231228/pdfminer/cmap/UniJIS-UTF32-V.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer.aemc-20221118/pdfminer/cmap/UniJIS-UTF8-H.pickle.gz` & `pdfminer_aemc-20231228/pdfminer/cmap/UniJIS-UTF8-H.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer.aemc-20221118/pdfminer/cmap/UniJIS-UTF8-V.pickle.gz` & `pdfminer_aemc-20231228/pdfminer/cmap/UniJIS-UTF8-V.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer.aemc-20221118/pdfminer/cmap/UniJIS2004-UTF16-H.pickle.gz` & `pdfminer_aemc-20231228/pdfminer/cmap/UniJIS2004-UTF16-H.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer.aemc-20221118/pdfminer/cmap/UniJIS2004-UTF16-V.pickle.gz` & `pdfminer_aemc-20231228/pdfminer/cmap/UniJIS2004-UTF16-V.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer.aemc-20221118/pdfminer/cmap/UniJIS2004-UTF32-H.pickle.gz` & `pdfminer_aemc-20231228/pdfminer/cmap/UniJIS2004-UTF32-H.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer.aemc-20221118/pdfminer/cmap/UniJIS2004-UTF32-V.pickle.gz` & `pdfminer_aemc-20231228/pdfminer/cmap/UniJIS2004-UTF32-V.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer.aemc-20221118/pdfminer/cmap/UniJIS2004-UTF8-H.pickle.gz` & `pdfminer_aemc-20231228/pdfminer/cmap/UniJIS2004-UTF8-H.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer.aemc-20221118/pdfminer/cmap/UniJIS2004-UTF8-V.pickle.gz` & `pdfminer_aemc-20231228/pdfminer/cmap/UniJIS2004-UTF8-V.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer.aemc-20221118/pdfminer/cmap/UniJISX0213-UTF32-H.pickle.gz` & `pdfminer_aemc-20231228/pdfminer/cmap/UniJISX0213-UTF32-H.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer.aemc-20221118/pdfminer/cmap/UniJISX0213-UTF32-V.pickle.gz` & `pdfminer_aemc-20231228/pdfminer/cmap/UniJISX0213-UTF32-V.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer.aemc-20221118/pdfminer/cmap/UniJISX02132004-UTF32-H.pickle.gz` & `pdfminer_aemc-20231228/pdfminer/cmap/UniJISX02132004-UTF32-H.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer.aemc-20221118/pdfminer/cmap/UniJISX02132004-UTF32-V.pickle.gz` & `pdfminer_aemc-20231228/pdfminer/cmap/UniJISX02132004-UTF32-V.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer.aemc-20221118/pdfminer/cmap/UniKS-UCS2-H.pickle.gz` & `pdfminer_aemc-20231228/pdfminer/cmap/UniKS-UCS2-H.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer.aemc-20221118/pdfminer/cmap/UniKS-UCS2-V.pickle.gz` & `pdfminer_aemc-20231228/pdfminer/cmap/UniKS-UCS2-V.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer.aemc-20221118/pdfminer/cmap/UniKS-UTF16-H.pickle.gz` & `pdfminer_aemc-20231228/pdfminer/cmap/UniKS-UTF16-H.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer.aemc-20221118/pdfminer/cmap/UniKS-UTF16-V.pickle.gz` & `pdfminer_aemc-20231228/pdfminer/cmap/UniKS-UTF16-V.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer.aemc-20221118/pdfminer/cmap/UniKS-UTF32-H.pickle.gz` & `pdfminer_aemc-20231228/pdfminer/cmap/UniKS-UTF32-H.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer.aemc-20221118/pdfminer/cmap/UniKS-UTF32-V.pickle.gz` & `pdfminer_aemc-20231228/pdfminer/cmap/UniKS-UTF32-V.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer.aemc-20221118/pdfminer/cmap/UniKS-UTF8-H.pickle.gz` & `pdfminer_aemc-20231228/pdfminer/cmap/UniKS-UTF8-H.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer.aemc-20221118/pdfminer/cmap/UniKS-UTF8-V.pickle.gz` & `pdfminer_aemc-20231228/pdfminer/cmap/UniKS-UTF8-V.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer.aemc-20221118/pdfminer/cmap/V.pickle.gz` & `pdfminer_aemc-20231228/pdfminer/cmap/V.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer.aemc-20221118/pdfminer/cmap/to-unicode-Adobe-CNS1.pickle.gz` & `pdfminer_aemc-20231228/pdfminer/cmap/to-unicode-Adobe-CNS1.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer.aemc-20221118/pdfminer/cmap/to-unicode-Adobe-GB1.pickle.gz` & `pdfminer_aemc-20231228/pdfminer/cmap/to-unicode-Adobe-GB1.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer.aemc-20221118/pdfminer/cmap/to-unicode-Adobe-Japan1.pickle.gz` & `pdfminer_aemc-20231228/pdfminer/cmap/to-unicode-Adobe-Japan1.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer.aemc-20221118/pdfminer/cmap/to-unicode-Adobe-Korea1.pickle.gz` & `pdfminer_aemc-20231228/pdfminer/cmap/to-unicode-Adobe-Korea1.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer.aemc-20221118/pdfminer/cmapdb.py` & `pdfminer_aemc-20231228/pdfminer/cmapdb.py`

 * *Files 2% similar despite different names*

```diff
@@ -191,29 +191,34 @@
 
 class FileUnicodeMap(UnicodeMap):
     def add_cid2unichr(self, cid: int, code: Union[PSLiteral, bytes, int]) -> None:
         assert isinstance(cid, int), str(type(cid))
         if isinstance(code, PSLiteral):
             # Interpret as an Adobe glyph name.
             assert isinstance(code.name, str)
-            self.cid2unichr[cid] = name2unicode(code.name)
+            unichr = name2unicode(code.name)
         elif isinstance(code, bytes):
-            # # Interpret as UTF-16BE.
-            # self.cid2unichr[cid] = code.decode("UTF-16BE", "ignore")
-            char = code.decode("UTF-16BE", "ignore")
-            if len(char) == 1:
-                self.cid2unichr[cid] = char
-            else:
-                # bypass the strange ToUnicode map provided by Morisawa Inc.
-                self.cid2unichr[cid] = f"(cid2:{cid})"
+            # Interpret as UTF-16BE.
+            unichr = code.decode("UTF-16BE", "ignore")
+            # char = code.decode("UTF-16BE", "ignore")
+            # if len(char) == 1:
+            #     self.cid2unichr[cid] = char
+            # else:
+            #     # bypass the strange ToUnicode map provided by Morisawa Inc.
+            #     self.cid2unichr[cid] = f"(cid2:{cid})"
         elif isinstance(code, int):
-            self.cid2unichr[cid] = chr(code)
+            unichr = chr(code)
         else:
             raise TypeError(code)
 
+        # A0 = non-breaking space, some weird fonts can have a collision on a cid here.
+        if unichr == "\u00A0" and self.cid2unichr.get(cid) == " ":
+            return
+        self.cid2unichr[cid] = unichr
+
 
 class PyCMap(CMap):
     def __init__(self, name: str, module: Any) -> None:
         super().__init__(CMapName=name)
         self.code2cid = module.CODE2CID
         if module.IS_VERTICAL:
             self.attrs["WMode"] = 1
```

### Comparing `pdfminer.aemc-20221118/pdfminer/converter.py` & `pdfminer_aemc-20231228/pdfminer/converter.py`

 * *Files 2% similar despite different names*

```diff
@@ -134,28 +134,43 @@
             # their point-position in their final two arguments. (Any preceding
             # arguments represent control points on Bézier curves.)
             raw_pts = [
                 cast(Point, p[-2:] if p[0] != "h" else path[0][-2:]) for p in path
             ]
             pts = [apply_matrix_pt(self.ctm, pt) for pt in raw_pts]
 
+            operators = [str(operation[0]) for operation in path]
+            transformed_points = [
+                [
+                    apply_matrix_pt(self.ctm, (float(operand1), float(operand2)))
+                    for operand1, operand2 in zip(operation[1::2], operation[2::2])
+                ]
+                for operation in path
+            ]
+            transformed_path = [
+                cast(PathSegment, (o, *p))
+                for o, p in zip(operators, transformed_points)
+            ]
+
             if shape in {"mlh", "ml"}:
                 # single line segment
                 #
                 # Note: 'ml', in conditional above, is a frequent anomaly
                 # that we want to support.
                 line = LTLine(
                     gstate.linewidth,
                     pts[0],
                     pts[1],
                     stroke,
                     fill,
                     evenodd,
                     gstate.scolor,
                     gstate.ncolor,
+                    original_path=transformed_path,
+                    dashing_style=gstate.dash,
                 )
                 self.cur_item.add(line)
 
             elif shape in {"mlllh", "mllll"}:
                 (x0, y0), (x1, y1), (x2, y2), (x3, y3), _ = pts
 
                 is_closed_loop = pts[0] == pts[4]
@@ -167,37 +182,42 @@
                         gstate.linewidth,
                         (*pts[0], *pts[2]),
                         stroke,
                         fill,
                         evenodd,
                         gstate.scolor,
                         gstate.ncolor,
+                        transformed_path,
+                        gstate.dash,
                     )
                     self.cur_item.add(rect)
                 else:
                     curve = LTCurve(
                         gstate.linewidth,
                         pts,
                         stroke,
                         fill,
                         evenodd,
                         gstate.scolor,
                         gstate.ncolor,
+                        transformed_path,
+                        gstate.dash,
                     )
                     self.cur_item.add(curve)
-
             else:
                 curve = LTCurve(
                     gstate.linewidth,
                     pts,
                     stroke,
                     fill,
                     evenodd,
                     gstate.scolor,
                     gstate.ncolor,
+                    transformed_path,
+                    gstate.dash,
                 )
                 self.cur_item.add(curve)
 
     def render_char(
         self,
         matrix: Matrix,
         font: PDFFont,
```

### Comparing `pdfminer.aemc-20221118/pdfminer/data_structures.py` & `pdfminer_aemc-20231228/pdfminer/data_structures.py`

 * *Files identical despite different names*

### Comparing `pdfminer.aemc-20221118/pdfminer/encodingdb.py` & `pdfminer_aemc-20231228/pdfminer/encodingdb.py`

 * *Files identical despite different names*

### Comparing `pdfminer.aemc-20221118/pdfminer/fontmetrics.py` & `pdfminer_aemc-20231228/pdfminer/fontmetrics.py`

 * *Files identical despite different names*

### Comparing `pdfminer.aemc-20221118/pdfminer/glyphlist.py` & `pdfminer_aemc-20231228/pdfminer/glyphlist.py`

 * *Files identical despite different names*

### Comparing `pdfminer.aemc-20221118/pdfminer/high_level.py` & `pdfminer_aemc-20231228/pdfminer/high_level.py`

 * *Files identical despite different names*

### Comparing `pdfminer.aemc-20221118/pdfminer/image.py` & `pdfminer_aemc-20231228/pdfminer/image.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from io import BytesIO
 from typing import BinaryIO, Tuple
 
 try:
     from typing import Literal
 except ImportError:
     # Literal was introduced in Python 3.8
-    from typing_extensions import Literal  # type: ignore[misc]
+    from typing_extensions import Literal  # type: ignore[assignment]
 
 from .jbig2 import JBIG2StreamReader, JBIG2StreamWriter
 from .layout import LTImage
 from .pdfcolor import LITERAL_DEVICE_CMYK
 from .pdfcolor import LITERAL_DEVICE_GRAY
 from .pdfcolor import LITERAL_DEVICE_RGB
 from .pdftypes import (
```

### Comparing `pdfminer.aemc-20221118/pdfminer/jbig2.py` & `pdfminer_aemc-20231228/pdfminer/jbig2.py`

 * *Files identical despite different names*

### Comparing `pdfminer.aemc-20221118/pdfminer/latin_enc.py` & `pdfminer_aemc-20231228/pdfminer/latin_enc.py`

 * *Files identical despite different names*

### Comparing `pdfminer.aemc-20221118/pdfminer/layout.py` & `pdfminer_aemc-20231228/pdfminer/layout.py`

 * *Files 3% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 )
 
 from .pdfcolor import PDFColorSpace
 from .pdffont import PDFFont
 from .pdfinterp import Color
 from .pdfinterp import PDFGraphicState
 from .pdftypes import PDFStream
-from .utils import INF
+from .utils import INF, PathSegment
 from .utils import LTComponentT
 from .utils import Matrix
 from .utils import Plane
 from .utils import Point
 from .utils import Rect
 from .utils import apply_matrix_pt
 from .utils import bbox2str
@@ -206,34 +206,45 @@
         if self.is_voverlap(obj):
             return min(abs(self.y0 - obj.y1), abs(self.y1 - obj.y0))
         else:
             return 0
 
 
 class LTCurve(LTComponent):
-    """A generic Bezier curve"""
+    """
+    A generic Bezier curve
+
+    The parameter `original_path` contains the original
+    pathing information from the pdf (e.g. for reconstructing Bezier Curves).
+
+    `dashing_style` contains the Dashing information if any.
+    """
 
     def __init__(
         self,
         linewidth: float,
         pts: List[Point],
         stroke: bool = False,
         fill: bool = False,
         evenodd: bool = False,
         stroking_color: Optional[Color] = None,
         non_stroking_color: Optional[Color] = None,
+        original_path: Optional[List[PathSegment]] = None,
+        dashing_style: Optional[Tuple[object, object]] = None,
     ) -> None:
         LTComponent.__init__(self, get_bound(pts))
         self.pts = pts
         self.linewidth = linewidth
         self.stroke = stroke
         self.fill = fill
         self.evenodd = evenodd
         self.stroking_color = stroking_color
         self.non_stroking_color = non_stroking_color
+        self.original_path = original_path
+        self.dashing_style = dashing_style
 
     def get_pts(self) -> str:
         return ",".join("%.3f,%.3f" % p for p in self.pts)
 
 
 class LTLine(LTCurve):
     """A single straight line.
@@ -247,24 +258,28 @@
         p0: Point,
         p1: Point,
         stroke: bool = False,
         fill: bool = False,
         evenodd: bool = False,
         stroking_color: Optional[Color] = None,
         non_stroking_color: Optional[Color] = None,
+        original_path: Optional[List[PathSegment]] = None,
+        dashing_style: Optional[Tuple[object, object]] = None,
     ) -> None:
         LTCurve.__init__(
             self,
             linewidth,
             [p0, p1],
             stroke,
             fill,
             evenodd,
             stroking_color,
             non_stroking_color,
+            original_path,
+            dashing_style,
         )
 
 
 class LTRect(LTCurve):
     """A rectangle.
 
     Could be used for framing another pictures or figures.
@@ -275,25 +290,29 @@
         linewidth: float,
         bbox: Rect,
         stroke: bool = False,
         fill: bool = False,
         evenodd: bool = False,
         stroking_color: Optional[Color] = None,
         non_stroking_color: Optional[Color] = None,
+        original_path: Optional[List[PathSegment]] = None,
+        dashing_style: Optional[Tuple[object, object]] = None,
     ) -> None:
         (x0, y0, x1, y1) = bbox
         LTCurve.__init__(
             self,
             linewidth,
             [(x0, y0), (x1, y0), (x1, y1), (x0, y1)],
             stroke,
             fill,
             evenodd,
             stroking_color,
             non_stroking_color,
+            original_path,
+            dashing_style,
         )
 
 
 class LTImage(LTComponent):
     """An image object.
 
     Embedded images can be in JPEG, Bitmap or JBIG2.
@@ -369,43 +388,33 @@
                 vx = vx * fontsize * 0.001
             vy = (1000 - vy) * fontsize * 0.001
             bbox_lower_left = (-vx, vy + rise + self.adv)
             bbox_upper_right = (-vx + fontsize, vy + rise)
         else:
             # horizontal
             # Original (not good)
-            descent = font.get_descent() * fontsize
-            bbox_lower_left = (0, descent + rise)
-            bbox_upper_right = (self.adv, descent + rise + fontsize)
+            # descent = font.get_descent() * fontsize
+            # bbox_lower_left = (0, descent + rise)
+            # bbox_upper_right = (self.adv, descent + rise + fontsize)
             # Trial 1: Divided by 2 (overall a little bit better)
             #ascent = font.get_ascent() * fontsize / 2.0
             #descent = font.get_descent() * fontsize / 2.0
             #bbox_lower_left = (0, descent + rise)
             #bbox_upper_right = (self.adv, descent + rise + fontsize)
             # Trial 2: Offset by 0.2 (mostly better but not always)
             #ascent = (font.get_ascent() - 0.2) * fontsize
             #descent = (font.get_descent() + 0.2) * fontsize
             #bbox_lower_left = (0, descent + rise)
             #bbox_upper_right = (self.adv, descent + rise + fontsize)
-            # # Trial 3: Using StemV instead of descent (overall much better in 20201018)
-            # ascent = font.get_ascent() * fontsize
-            # descent = font.get_descent() * fontsize
-            # height = font.get_height() * fontsize
-            # stemv = font.get_stemv() * fontsize
-            # yAdj = -stemv if abs(stemv) < abs(descent) else 0
-            # bbox_lower_left = (0, yAdj + rise)
-            # bbox_upper_right = (self.adv, yAdj + rise + fontsize)
-            # # Trial 4: Using StemV instead of descent (overall much better in 20221105)
-            # ascent = font.get_ascent() * fontsize
-            # descent = font.get_descent() * fontsize
-            # height = font.get_height() * fontsize
-            # stemv = font.get_stemv() * fontsize
-            # yAdj = -stemv if abs(stemv) < abs(descent) else 0
-            # bbox_lower_left = (0, yAdj + rise)
-            # bbox_upper_right = (self.adv, yAdj + rise + fontsize)
+            # Trial 3: Using StemV instead of descent (overall much better in 20201018)
+            descent = font.get_descent() * fontsize
+            stemv = font.get_stemv() * fontsize
+            yAdj = -stemv if abs(stemv) < abs(descent) else 0
+            bbox_lower_left = (0, yAdj + rise)
+            bbox_upper_right = (self.adv, yAdj + rise + fontsize)
         (a, b, c, d, e, f) = self.matrix
         self.upright = 0 < a * d * scaling and b * c <= 0
         (x0, y0) = apply_matrix_pt(self.matrix, bbox_lower_left)
         (x1, y1) = apply_matrix_pt(self.matrix, bbox_upper_right)
         if x1 < x0:
             (x0, x1) = (x1, x0)
         if y1 < y0:
```

### Comparing `pdfminer.aemc-20221118/pdfminer/lzw.py` & `pdfminer_aemc-20231228/pdfminer/lzw.py`

 * *Files identical despite different names*

### Comparing `pdfminer.aemc-20221118/pdfminer/pdfcolor.py` & `pdfminer_aemc-20231228/pdfminer/pdfcolor.py`

 * *Files identical despite different names*

### Comparing `pdfminer.aemc-20221118/pdfminer/pdfdevice.py` & `pdfminer_aemc-20231228/pdfminer/pdfdevice.py`

 * *Files identical despite different names*

### Comparing `pdfminer.aemc-20221118/pdfminer/pdfdocument.py` & `pdfminer_aemc-20231228/pdfminer/pdfdocument.py`

 * *Files identical despite different names*

### Comparing `pdfminer.aemc-20221118/pdfminer/pdffont.py` & `pdfminer_aemc-20231228/pdfminer/pdffont.py`

 * *Files 1% similar despite different names*

```diff
@@ -751,15 +751,19 @@
         subtables: List[Tuple[int, int, int]] = []
         for i in range(nsubtables):
             subtables.append(
                 cast(Tuple[int, int, int], struct.unpack(">HHL", fp.read(8)))
             )
         char2gid: Dict[int, int] = {}
         # Only supports subtable type 0, 2 and 4.
-        for (_1, _2, st_offset) in subtables:
+        for (platform_id, encoding_id, st_offset) in subtables:
+            # Skip non-Unicode cmaps.
+            # https://docs.microsoft.com/en-us/typography/opentype/spec/cmap
+            if not (platform_id == 0 or (platform_id == 3 and encoding_id in [1, 10])):
+                continue
             fp.seek(base_offset + st_offset)
             (fmttype, fmtlen, fmtlang) = cast(
                 Tuple[int, int, int], struct.unpack(">HHH", fp.read(6))
             )
             if fmttype == 0:
                 char2gid.update(
                     enumerate(
@@ -820,14 +824,16 @@
                             b = cast(Tuple[int], struct.unpack(">H", fp.read(2)))[0]
                             char2gid[c] = (b + idd) & 0xFFFF
                     else:
                         for c in range(sc, ec + 1):
                             char2gid[c] = (c + idd) & 0xFFFF
             else:
                 assert False, str(("Unhandled", fmttype))
+        if not char2gid:
+            raise TrueTypeFont.CMapNotFound
         # create unicode map
         unicode_map = FileUnicodeMap()
         for (char, gid) in char2gid.items():
             unicode_map.add_cid2unichr(gid, char)
         return unicode_map
 
 
@@ -900,16 +906,16 @@
         return self.ascent * self.vscale
 
     def get_descent(self) -> float:
         """Descent below the baseline, in text space units; always negative"""
         return self.descent * self.vscale
 
     def get_stemv(self):
-        """Width of the vertical stems in characters"""
-        return self.stemv * self.vscale
+            """Width of the vertical stems in characters"""
+            return self.stemv * self.vscale
 
     def get_width(self) -> float:
         w = self.bbox[2] - self.bbox[0]
         if w == 0:
             w = -self.default_width
         return w * self.hscale
```

### Comparing `pdfminer.aemc-20221118/pdfminer/pdfinterp.py` & `pdfminer_aemc-20231228/pdfminer/pdfinterp.py`

 * *Files identical despite different names*

### Comparing `pdfminer.aemc-20221118/pdfminer/pdfpage.py` & `pdfminer_aemc-20231228/pdfminer/pdfpage.py`

 * *Files identical despite different names*

### Comparing `pdfminer.aemc-20221118/pdfminer/pdfparser.py` & `pdfminer_aemc-20231228/pdfminer/pdfparser.py`

 * *Files identical despite different names*

### Comparing `pdfminer.aemc-20221118/pdfminer/pdftypes.py` & `pdfminer_aemc-20231228/pdfminer/pdftypes.py`

 * *Files identical despite different names*

### Comparing `pdfminer.aemc-20221118/pdfminer/psparser.py` & `pdfminer_aemc-20231228/pdfminer/psparser.py`

 * *Files identical despite different names*

### Comparing `pdfminer.aemc-20221118/pdfminer/runlength.py` & `pdfminer_aemc-20231228/pdfminer/runlength.py`

 * *Files identical despite different names*

### Comparing `pdfminer.aemc-20221118/pdfminer/utils.py` & `pdfminer_aemc-20231228/pdfminer/utils.py`

 * *Files identical despite different names*

### Comparing `pdfminer.aemc-20221118/pdfminer.aemc.egg-info/PKG-INFO` & `pdfminer_aemc-20231228/pdfminer.aemc.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,32 +1,46 @@
 Metadata-Version: 2.1
 Name: pdfminer.aemc
-Version: 20221118
+Version: 20231228
 Summary: PDF parser and analyzer
 Home-page: https://github.com/pdfminer/pdfminer.aemc
 Author: Yusuke Shinyama + Philippe Guglielmetti + Liew Chun Fui
 Author-email: wargreymon28@gmail.com
 License: MIT/X
 Keywords: pdf parser,pdf converter,layout analysis,text mining
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Topic :: Text Processing
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: charset-normalizer>=2.0.0
+Requires-Dist: cryptography>=36.0.0
+Requires-Dist: typing_extensions; python_version < "3.8"
+Requires-Dist: importlib_metadata; python_version < "3.8"
 Provides-Extra: dev
+Requires-Dist: pytest; extra == "dev"
+Requires-Dist: nox; extra == "dev"
+Requires-Dist: black; extra == "dev"
+Requires-Dist: mypy==0.931; extra == "dev"
 Provides-Extra: docs
+Requires-Dist: sphinx; extra == "docs"
+Requires-Dist: sphinx-argparse; extra == "docs"
 Provides-Extra: image
-License-File: LICENSE
+Requires-Dist: Pillow; extra == "image"
 
 pdfminer.six
 ============
 
 [![Continuous integration](https://github.com/pdfminer/pdfminer.six/actions/workflows/actions.yml/badge.svg)](https://github.com/pdfminer/pdfminer.six/actions/workflows/actions.yml)
 [![PyPI version](https://img.shields.io/pypi/v/pdfminer.six.svg)](https://pypi.python.org/pypi/pdfminer.six/)
 [![gitter](https://badges.gitter.im/pdfminer-six/Lobby.svg)](https://gitter.im/pdfminer-six/Lobby?utm_source=badge&utm_medium)
@@ -61,15 +75,15 @@
 * Table of contents extraction.
 * Tagged contents extraction.
 * Automatic layout analysis.
 
 How to use
 ----------
 
-* Install Python 3.6 or newer.
+* Install Python 3.8 or newer.
 * Install pdfminer.six.
 
   `pip install pdfminer.six`
 
 * (Optionally) install extra dependencies for extracting images.
 
   `pip install 'pdfminer.six[image]'`
```

### Comparing `pdfminer.aemc-20221118/pdfminer.aemc.egg-info/SOURCES.txt` & `pdfminer_aemc-20231228/pdfminer.aemc.egg-info/SOURCES.txt`

 * *Files 16% similar despite different names*

```diff
@@ -191,14 +191,29 @@
 pdfminer/cmap/V.pickle.gz
 pdfminer/cmap/WP-Symbol-H.pickle.gz
 pdfminer/cmap/WP-Symbol-V.pickle.gz
 pdfminer/cmap/to-unicode-Adobe-CNS1.pickle.gz
 pdfminer/cmap/to-unicode-Adobe-GB1.pickle.gz
 pdfminer/cmap/to-unicode-Adobe-Japan1.pickle.gz
 pdfminer/cmap/to-unicode-Adobe-Korea1.pickle.gz
+tests/test_converter.py
+tests/test_encodingdb.py
+tests/test_font_size.py
+tests/test_highlevel_extracttext.py
+tests/test_layout.py
+tests/test_pdfdocument.py
+tests/test_pdfencoding.py
+tests/test_pdffont.py
+tests/test_pdfminer_ccitt.py
+tests/test_pdfminer_crypto.py
+tests/test_pdfminer_psparser.py
+tests/test_pdfpage.py
+tests/test_tools_dumppdf.py
+tests/test_tools_pdf2txt.py
+tests/test_utils.py
 tools/__init__.py
 tools/conv_afm.py
 tools/conv_cmap.py
 tools/conv_glyphlist.py
 tools/dumppdf.py
 tools/pdf2txt.py
 tools/pdfdiff.py
```

### Comparing `pdfminer.aemc-20221118/setup.py` & `pdfminer_aemc-20231228/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -15,14 +15,15 @@
     version=package.__version__,
     packages=["pdfminer"],
     package_data={"pdfminer": ["cmap/*.pickle.gz", "py.typed"]},
     install_requires=[
         "charset-normalizer >= 2.0.0",
         "cryptography >= 36.0.0",
         'typing_extensions; python_version < "3.8"',
+        'importlib_metadata; python_version < "3.8"',
     ],
     extras_require={
         "dev": ["pytest", "nox", "black", "mypy == 0.931"],
         "docs": ["sphinx", "sphinx-argparse"],
         "image": ["Pillow"],
     },
     description="PDF parser and analyzer",
@@ -43,14 +44,17 @@
         "text mining",
     ],
     python_requires=">=3.8",
     classifiers=[
         "Programming Language :: Python",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
+        "Programming Language :: Python :: 3.10",
+        "Programming Language :: Python :: 3.11",
+        "Programming Language :: Python :: 3.12",
         "Programming Language :: Python :: 3 :: Only",
         "Development Status :: 5 - Production/Stable",
         "Environment :: Console",
         "Intended Audience :: Developers",
         "Intended Audience :: Science/Research",
         "License :: OSI Approved :: MIT License",
         "Topic :: Text Processing",
```

### Comparing `pdfminer.aemc-20221118/tools/conv_afm.py` & `pdfminer_aemc-20231228/tools/conv_afm.py`

 * *Files identical despite different names*

### Comparing `pdfminer.aemc-20221118/tools/conv_cmap.py` & `pdfminer_aemc-20231228/tools/conv_cmap.py`

 * *Files identical despite different names*

### Comparing `pdfminer.aemc-20221118/tools/conv_glyphlist.py` & `pdfminer_aemc-20231228/tools/conv_glyphlist.py`

 * *Files identical despite different names*

### Comparing `pdfminer.aemc-20221118/tools/dumppdf.py` & `pdfminer_aemc-20231228/tools/dumppdf.py`

 * *Files identical despite different names*

### Comparing `pdfminer.aemc-20221118/tools/pdf2txt.py` & `pdfminer_aemc-20231228/tools/pdf2txt.py`

 * *Files identical despite different names*

### Comparing `pdfminer.aemc-20221118/tools/pdfdiff.py` & `pdfminer_aemc-20231228/tools/pdfdiff.py`

 * *Files identical despite different names*

### Comparing `pdfminer.aemc-20221118/tools/pdfstats.py` & `pdfminer_aemc-20231228/tools/pdfstats.py`

 * *Files identical despite different names*

### Comparing `pdfminer.aemc-20221118/tools/prof.py` & `pdfminer_aemc-20231228/tools/prof.py`

 * *Files identical despite different names*

