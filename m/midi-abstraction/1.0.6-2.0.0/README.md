# Comparing `tmp/midi-abstraction-1.0.6.tar.gz` & `tmp/midi-abstraction-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "midi-abstraction-1.0.6.tar", last modified: Tue May 31 20:57:19 2022, max compression
+gzip compressed data, was "midi-abstraction-2.0.0.tar", last modified: Sat May  4 06:27:35 2024, max compression
```

## Comparing `midi-abstraction-1.0.6.tar` & `midi-abstraction-2.0.0.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 cyberrumor  (1000) cyberrumor  (1000)        0 2022-05-31 20:57:19.966338 midi-abstraction-1.0.6/
--rw-r--r--   0 cyberrumor  (1000) cyberrumor  (1000)    35149 2022-05-24 18:08:34.000000 midi-abstraction-1.0.6/LICENSE
--rw-r--r--   0 cyberrumor  (1000) cyberrumor  (1000)     2687 2022-05-31 20:57:19.966338 midi-abstraction-1.0.6/PKG-INFO
--rwxr-xr-x   0 cyberrumor  (1000) cyberrumor  (1000)     2140 2022-05-24 18:08:34.000000 midi-abstraction-1.0.6/README.md
-drwxr-xr-x   0 cyberrumor  (1000) cyberrumor  (1000)        0 2022-05-31 20:57:19.965338 midi-abstraction-1.0.6/midi_abstraction/
--rwxr-xr-x   0 cyberrumor  (1000) cyberrumor  (1000)       48 2022-05-24 18:08:34.000000 midi-abstraction-1.0.6/midi_abstraction/__init__.py
--rwxr-xr-x   0 cyberrumor  (1000) cyberrumor  (1000)    15551 2022-05-31 20:49:35.000000 midi-abstraction-1.0.6/midi_abstraction/midi_abstraction.py
-drwxr-xr-x   0 cyberrumor  (1000) cyberrumor  (1000)        0 2022-05-31 20:57:19.966338 midi-abstraction-1.0.6/midi_abstraction.egg-info/
--rw-r--r--   0 cyberrumor  (1000) cyberrumor  (1000)     2687 2022-05-31 20:57:19.000000 midi-abstraction-1.0.6/midi_abstraction.egg-info/PKG-INFO
--rw-r--r--   0 cyberrumor  (1000) cyberrumor  (1000)      252 2022-05-31 20:57:19.000000 midi-abstraction-1.0.6/midi_abstraction.egg-info/SOURCES.txt
--rw-r--r--   0 cyberrumor  (1000) cyberrumor  (1000)        1 2022-05-31 20:57:19.000000 midi-abstraction-1.0.6/midi_abstraction.egg-info/dependency_links.txt
--rw-r--r--   0 cyberrumor  (1000) cyberrumor  (1000)       17 2022-05-31 20:57:19.000000 midi-abstraction-1.0.6/midi_abstraction.egg-info/top_level.txt
--rw-r--r--   0 cyberrumor  (1000) cyberrumor  (1000)       38 2022-05-31 20:57:19.966338 midi-abstraction-1.0.6/setup.cfg
--rwxr-xr-x   0 cyberrumor  (1000) cyberrumor  (1000)      729 2022-05-31 20:57:04.000000 midi-abstraction-1.0.6/setup.py
+drwxr-xr-x   0 cyberrumor  (1000) wheel      (998)        0 2024-05-04 06:27:35.254342 midi-abstraction-2.0.0/
+-rw-r--r--   0 cyberrumor  (1000) wheel      (998)    35149 2024-04-30 01:45:13.000000 midi-abstraction-2.0.0/LICENSE
+-rw-r--r--   0 cyberrumor  (1000) wheel      (998)     1781 2024-05-04 06:27:35.254342 midi-abstraction-2.0.0/PKG-INFO
+-rwxr-xr-x   0 cyberrumor  (1000) wheel      (998)     1270 2024-05-04 05:46:43.000000 midi-abstraction-2.0.0/README.md
+drwxr-xr-x   0 cyberrumor  (1000) wheel      (998)        0 2024-05-04 06:27:35.251008 midi-abstraction-2.0.0/midi_abstraction/
+-rwxr-xr-x   0 cyberrumor  (1000) wheel      (998)       32 2024-05-04 00:54:44.000000 midi-abstraction-2.0.0/midi_abstraction/__init__.py
+-rwxr-xr-x   0 cyberrumor  (1000) wheel      (998)    15131 2024-05-04 05:17:50.000000 midi-abstraction-2.0.0/midi_abstraction/midi_abstraction.py
+drwxr-xr-x   0 cyberrumor  (1000) wheel      (998)        0 2024-05-04 06:27:35.254342 midi-abstraction-2.0.0/midi_abstraction.egg-info/
+-rw-r--r--   0 cyberrumor  (1000) wheel      (998)     1781 2024-05-04 06:27:35.000000 midi-abstraction-2.0.0/midi_abstraction.egg-info/PKG-INFO
+-rw-r--r--   0 cyberrumor  (1000) wheel      (998)      252 2024-05-04 06:27:35.000000 midi-abstraction-2.0.0/midi_abstraction.egg-info/SOURCES.txt
+-rw-r--r--   0 cyberrumor  (1000) wheel      (998)        1 2024-05-04 06:27:35.000000 midi-abstraction-2.0.0/midi_abstraction.egg-info/dependency_links.txt
+-rw-r--r--   0 cyberrumor  (1000) wheel      (998)       17 2024-05-04 06:27:35.000000 midi-abstraction-2.0.0/midi_abstraction.egg-info/top_level.txt
+-rw-r--r--   0 cyberrumor  (1000) wheel      (998)       38 2024-05-04 06:27:35.254342 midi-abstraction-2.0.0/setup.cfg
+-rwxr-xr-x   0 cyberrumor  (1000) wheel      (998)      787 2024-05-04 06:25:01.000000 midi-abstraction-2.0.0/setup.py
```

### Comparing `midi-abstraction-1.0.6/LICENSE` & `midi-abstraction-2.0.0/LICENSE`

 * *Files identical despite different names*

