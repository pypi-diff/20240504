# Comparing `tmp/TrainingAnimation-0.0.10.tar.gz` & `tmp/TrainingAnimation-0.0.11.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "TrainingAnimation-0.0.10.tar", last modified: Sat May  4 12:17:28 2024, max compression
+gzip compressed data, was "TrainingAnimation-0.0.11.tar", last modified: Sat May  4 12:24:27 2024, max compression
```

## Comparing `TrainingAnimation-0.0.10.tar` & `TrainingAnimation-0.0.11.tar`

### file list

```diff
@@ -1,15 +1,12 @@
-drwxrwxrwx   0        0        0        0 2024-05-04 12:17:28.871126 TrainingAnimation-0.0.10/
--rw-rw-rw-   0        0        0        3 2024-05-04 12:05:08.000000 TrainingAnimation-0.0.10/LICENSE
--rw-rw-rw-   0        0        0      245 2024-05-04 12:17:28.871126 TrainingAnimation-0.0.10/PKG-INFO
--rw-rw-rw-   0        0        0        6 2024-05-04 12:04:55.000000 TrainingAnimation-0.0.10/README.md
-drwxrwxrwx   0        0        0        0 2024-05-04 12:17:28.861121 TrainingAnimation-0.0.10/TrainingAnimation/
--rw-rw-rw-   0        0        0        0 2024-05-04 12:04:37.000000 TrainingAnimation-0.0.10/TrainingAnimation/__init__.py
--rw-rw-rw-   0        0        0      651 2024-05-04 12:01:08.000000 TrainingAnimation-0.0.10/TrainingAnimation/progress.py
-drwxrwxrwx   0        0        0        0 2024-05-04 12:17:28.870126 TrainingAnimation-0.0.10/TrainingAnimation.egg-info/
--rw-rw-rw-   0        0        0      245 2024-05-04 12:17:28.000000 TrainingAnimation-0.0.10/TrainingAnimation.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      290 2024-05-04 12:17:28.000000 TrainingAnimation-0.0.10/TrainingAnimation.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-04 12:17:28.000000 TrainingAnimation-0.0.10/TrainingAnimation.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       14 2024-05-04 12:17:28.000000 TrainingAnimation-0.0.10/TrainingAnimation.egg-info/requires.txt
--rw-rw-rw-   0        0        0       18 2024-05-04 12:17:28.000000 TrainingAnimation-0.0.10/TrainingAnimation.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-04 12:17:28.871126 TrainingAnimation-0.0.10/setup.cfg
--rw-rw-rw-   0        0        0      366 2024-05-04 12:17:25.000000 TrainingAnimation-0.0.10/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-04 12:24:27.826328 TrainingAnimation-0.0.11/
+-rw-rw-rw-   0        0        0        3 2024-05-04 12:05:08.000000 TrainingAnimation-0.0.11/LICENSE
+-rw-rw-rw-   0        0        0      245 2024-05-04 12:24:27.825329 TrainingAnimation-0.0.11/PKG-INFO
+-rw-rw-rw-   0        0        0        6 2024-05-04 12:04:55.000000 TrainingAnimation-0.0.11/README.md
+drwxrwxrwx   0        0        0        0 2024-05-04 12:24:27.825329 TrainingAnimation-0.0.11/TrainingAnimation.egg-info/
+-rw-rw-rw-   0        0        0      245 2024-05-04 12:24:27.000000 TrainingAnimation-0.0.11/TrainingAnimation.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      230 2024-05-04 12:24:27.000000 TrainingAnimation-0.0.11/TrainingAnimation.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-04 12:24:27.000000 TrainingAnimation-0.0.11/TrainingAnimation.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       14 2024-05-04 12:24:27.000000 TrainingAnimation-0.0.11/TrainingAnimation.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        1 2024-05-04 12:24:27.000000 TrainingAnimation-0.0.11/TrainingAnimation.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-04 12:24:27.826328 TrainingAnimation-0.0.11/setup.cfg
+-rw-rw-rw-   0        0        0      366 2024-05-04 12:24:22.000000 TrainingAnimation-0.0.11/setup.py
```

