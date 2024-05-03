# Comparing `tmp/scrapkit-1.7.tar.gz` & `tmp/scrapkit-2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scrapkit-1.7.tar", last modified: Wed May  1 15:43:21 2024, max compression
+gzip compressed data, was "scrapkit-2.0.tar", last modified: Fri May  3 00:43:08 2024, max compression
```

## Comparing `scrapkit-1.7.tar` & `scrapkit-2.0.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2024-05-01 15:43:21.156507 scrapkit-1.7/
--rw-rw-rw-   0        0        0     1709 2024-05-01 15:43:21.148512 scrapkit-1.7/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-05-01 15:43:21.109534 scrapkit-1.7/scrapkit/
--rw-rw-rw-   0        0        0      300 2024-05-01 15:40:58.000000 scrapkit-1.7/scrapkit/__init__.py
--rw-rw-rw-   0        0        0     3710 2024-05-01 15:41:04.000000 scrapkit-1.7/scrapkit/main.py
-drwxrwxrwx   0        0        0        0 2024-05-01 15:43:21.144515 scrapkit-1.7/scrapkit.egg-info/
--rw-rw-rw-   0        0        0     1709 2024-05-01 15:43:20.000000 scrapkit-1.7/scrapkit.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      205 2024-05-01 15:43:21.000000 scrapkit-1.7/scrapkit.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-01 15:43:20.000000 scrapkit-1.7/scrapkit.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       28 2024-05-01 15:43:20.000000 scrapkit-1.7/scrapkit.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2024-05-01 15:43:20.000000 scrapkit-1.7/scrapkit.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-01 15:43:21.157510 scrapkit-1.7/setup.cfg
--rw-rw-rw-   0        0        0      456 2024-05-01 15:43:09.000000 scrapkit-1.7/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-03 00:43:08.532441 scrapkit-2.0/
+-rw-rw-rw-   0        0        0     2066 2024-05-03 00:43:08.529443 scrapkit-2.0/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-05-03 00:43:08.479472 scrapkit-2.0/scrapkit/
+-rw-rw-rw-   0        0        0      597 2024-05-03 00:24:13.000000 scrapkit-2.0/scrapkit/__init__.py
+-rw-rw-rw-   0        0        0     5819 2024-05-03 00:25:12.000000 scrapkit-2.0/scrapkit/main.py
+drwxrwxrwx   0        0        0        0 2024-05-03 00:43:08.527442 scrapkit-2.0/scrapkit.egg-info/
+-rw-rw-rw-   0        0        0     2066 2024-05-03 00:43:08.000000 scrapkit-2.0/scrapkit.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      205 2024-05-03 00:43:08.000000 scrapkit-2.0/scrapkit.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-03 00:43:08.000000 scrapkit-2.0/scrapkit.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       28 2024-05-03 00:43:08.000000 scrapkit-2.0/scrapkit.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2024-05-03 00:43:08.000000 scrapkit-2.0/scrapkit.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-03 00:43:08.533439 scrapkit-2.0/setup.cfg
+-rw-rw-rw-   0        0        0      457 2024-05-03 00:42:49.000000 scrapkit-2.0/setup.py
```

