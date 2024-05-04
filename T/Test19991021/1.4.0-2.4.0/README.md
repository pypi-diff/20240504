# Comparing `tmp/Test19991021-1.4.0.tar.gz` & `tmp/Test19991021-2.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Test19991021-1.4.0.tar", last modified: Sat May  4 14:21:10 2024, max compression
+gzip compressed data, was "Test19991021-2.4.0.tar", last modified: Sat May  4 14:28:02 2024, max compression
```

## Comparing `Test19991021-1.4.0.tar` & `Test19991021-2.4.0.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2024-05-04 14:21:10.975809 Test19991021-1.4.0/
--rw-rw-rw-   0        0        0       80 2024-05-04 14:21:10.974809 Test19991021-1.4.0/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-05-04 14:21:10.966810 Test19991021-1.4.0/Test/
--rw-rw-rw-   0        0        0        0 2024-05-04 13:27:09.000000 Test19991021-1.4.0/Test/__init__.py
--rw-rw-rw-   0        0        0      104 2024-05-04 13:35:48.000000 Test19991021-1.4.0/Test/hello.py
--rw-rw-rw-   0        0        0        0 2024-05-04 13:27:19.000000 Test19991021-1.4.0/Test/main.py
-drwxrwxrwx   0        0        0        0 2024-05-04 14:21:10.973809 Test19991021-1.4.0/Test19991021.egg-info/
--rw-rw-rw-   0        0        0       80 2024-05-04 14:21:10.000000 Test19991021-1.4.0/Test19991021.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      231 2024-05-04 14:21:10.000000 Test19991021-1.4.0/Test19991021.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-04 14:21:10.000000 Test19991021-1.4.0/Test19991021.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2024-05-04 14:21:10.000000 Test19991021-1.4.0/Test19991021.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0        5 2024-05-04 14:21:10.000000 Test19991021-1.4.0/Test19991021.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-04 14:21:10.976809 Test19991021-1.4.0/setup.cfg
--rw-rw-rw-   0        0        0      291 2024-05-04 14:20:18.000000 Test19991021-1.4.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-04 14:28:02.978305 Test19991021-2.4.0/
+-rw-rw-rw-   0        0        0       80 2024-05-04 14:28:02.976303 Test19991021-2.4.0/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-05-04 14:28:02.975301 Test19991021-2.4.0/Test19991021.egg-info/
+-rw-rw-rw-   0        0        0       80 2024-05-04 14:28:02.000000 Test19991021-2.4.0/Test19991021.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      228 2024-05-04 14:28:02.000000 Test19991021-2.4.0/Test19991021.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-04 14:28:02.000000 Test19991021-2.4.0/Test19991021.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2024-05-04 14:28:02.000000 Test19991021-2.4.0/Test19991021.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0        4 2024-05-04 14:28:02.000000 Test19991021-2.4.0/Test19991021.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-04 14:28:02.973973 Test19991021-2.4.0/one/
+-rw-rw-rw-   0        0        0        0 2024-05-04 13:27:09.000000 Test19991021-2.4.0/one/__init__.py
+-rw-rw-rw-   0        0        0      104 2024-05-04 13:35:48.000000 Test19991021-2.4.0/one/hello.py
+-rw-rw-rw-   0        0        0        0 2024-05-04 13:27:19.000000 Test19991021-2.4.0/one/main.py
+-rw-rw-rw-   0        0        0       42 2024-05-04 14:28:02.978305 Test19991021-2.4.0/setup.cfg
+-rw-rw-rw-   0        0        0      291 2024-05-04 14:27:40.000000 Test19991021-2.4.0/setup.py
```

