# Comparing `tmp/EnglishLanguageAPI-0.0.2.tar.gz` & `tmp/englishlanguageapi-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "EnglishLanguageAPI-0.0.2.tar", last modified: Mon Jan 16 09:19:06 2023, max compression
+gzip compressed data, was "englishlanguageapi-1.0.0.tar", last modified: Fri May  3 23:52:28 2024, max compression
```

## Comparing `EnglishLanguageAPI-0.0.2.tar` & `englishlanguageapi-1.0.0.tar`

### file list

```diff
@@ -1,14 +1,16 @@
-drwxr-xr-x   0 guyyatsu  (1000) guyyatsu  (1000)        0 2023-01-16 09:19:06.115582 EnglishLanguageAPI-0.0.2/
--rw-r--r--   0 guyyatsu  (1000) guyyatsu  (1000)     8102 2023-01-16 09:19:06.112254 EnglishLanguageAPI-0.0.2/PKG-INFO
--rw-r--r--   0 guyyatsu  (1000) guyyatsu  (1000)      681 2023-01-16 09:18:05.000000 EnglishLanguageAPI-0.0.2/pyproject.toml
--rw-r--r--   0 guyyatsu  (1000) guyyatsu  (1000)       38 2023-01-16 09:19:06.115582 EnglishLanguageAPI-0.0.2/setup.cfg
-drwxr-xr-x   0 guyyatsu  (1000) guyyatsu  (1000)        0 2023-01-16 09:19:06.075646 EnglishLanguageAPI-0.0.2/src/
-drwxr-xr-x   0 guyyatsu  (1000) guyyatsu  (1000)        0 2023-01-16 09:19:06.085630 EnglishLanguageAPI-0.0.2/src/EnglishLanguageAPI/
--rw-r--r--   0 guyyatsu  (1000) guyyatsu  (1000)     7798 2023-01-16 09:03:50.000000 EnglishLanguageAPI-0.0.2/src/EnglishLanguageAPI/EnglishLanguageAPI.py
--rw-r--r--   0 guyyatsu  (1000) guyyatsu  (1000)       34 2023-01-16 09:11:42.000000 EnglishLanguageAPI-0.0.2/src/EnglishLanguageAPI/__init__.py
-drwxr-xr-x   0 guyyatsu  (1000) guyyatsu  (1000)        0 2023-01-16 09:19:06.105598 EnglishLanguageAPI-0.0.2/src/EnglishLanguageAPI.egg-info/
--rw-r--r--   0 guyyatsu  (1000) guyyatsu  (1000)     8102 2023-01-16 09:19:05.000000 EnglishLanguageAPI-0.0.2/src/EnglishLanguageAPI.egg-info/PKG-INFO
--rw-r--r--   0 guyyatsu  (1000) guyyatsu  (1000)      323 2023-01-16 09:19:05.000000 EnglishLanguageAPI-0.0.2/src/EnglishLanguageAPI.egg-info/SOURCES.txt
--rw-r--r--   0 guyyatsu  (1000) guyyatsu  (1000)        1 2023-01-16 09:19:05.000000 EnglishLanguageAPI-0.0.2/src/EnglishLanguageAPI.egg-info/dependency_links.txt
--rw-r--r--   0 guyyatsu  (1000) guyyatsu  (1000)        4 2023-01-16 09:19:05.000000 EnglishLanguageAPI-0.0.2/src/EnglishLanguageAPI.egg-info/requires.txt
--rw-r--r--   0 guyyatsu  (1000) guyyatsu  (1000)       19 2023-01-16 09:19:05.000000 EnglishLanguageAPI-0.0.2/src/EnglishLanguageAPI.egg-info/top_level.txt
+drwxr-xr-x   0 guyyatsu  (1000) guyyatsu  (1000)        0 2024-05-03 23:52:28.773885 englishlanguageapi-1.0.0/
+-rw-r--r--   0 guyyatsu  (1000) guyyatsu  (1000)     1812 2024-05-03 23:52:28.770552 englishlanguageapi-1.0.0/PKG-INFO
+-rw-r--r--   0 guyyatsu  (1000) guyyatsu  (1000)      660 2024-05-03 23:50:09.000000 englishlanguageapi-1.0.0/pyproject.toml
+-rw-r--r--   0 guyyatsu  (1000) guyyatsu  (1000)     1244 2024-05-03 23:47:07.000000 englishlanguageapi-1.0.0/readme.md
+-rw-r--r--   0 guyyatsu  (1000) guyyatsu  (1000)       38 2024-05-03 23:52:28.773885 englishlanguageapi-1.0.0/setup.cfg
+drwxr-xr-x   0 guyyatsu  (1000) guyyatsu  (1000)        0 2024-05-03 23:52:28.687218 englishlanguageapi-1.0.0/src/
+drwxr-xr-x   0 guyyatsu  (1000) guyyatsu  (1000)        0 2024-05-03 23:52:28.713885 englishlanguageapi-1.0.0/src/EnglishLanguageAPI/
+drwxr-xr-x   0 guyyatsu  (1000) guyyatsu  (1000)        0 2024-05-03 23:52:28.757218 englishlanguageapi-1.0.0/src/EnglishLanguageAPI/API/
+-rw-r--r--   0 guyyatsu  (1000) guyyatsu  (1000)     2581 2024-05-03 20:42:49.000000 englishlanguageapi-1.0.0/src/EnglishLanguageAPI/API/__init__.py
+-rw-r--r--   0 guyyatsu  (1000) guyyatsu  (1000)     4909 2024-05-03 22:36:07.000000 englishlanguageapi-1.0.0/src/EnglishLanguageAPI/__init__.py
+drwxr-xr-x   0 guyyatsu  (1000) guyyatsu  (1000)        0 2024-05-03 23:52:28.760552 englishlanguageapi-1.0.0/src/EnglishLanguageAPI.egg-info/
+-rw-r--r--   0 guyyatsu  (1000) guyyatsu  (1000)     1812 2024-05-03 23:52:28.000000 englishlanguageapi-1.0.0/src/EnglishLanguageAPI.egg-info/PKG-INFO
+-rw-r--r--   0 guyyatsu  (1000) guyyatsu  (1000)      327 2024-05-03 23:52:28.000000 englishlanguageapi-1.0.0/src/EnglishLanguageAPI.egg-info/SOURCES.txt
+-rw-r--r--   0 guyyatsu  (1000) guyyatsu  (1000)        1 2024-05-03 23:52:28.000000 englishlanguageapi-1.0.0/src/EnglishLanguageAPI.egg-info/dependency_links.txt
+-rw-r--r--   0 guyyatsu  (1000) guyyatsu  (1000)       13 2024-05-03 23:52:28.000000 englishlanguageapi-1.0.0/src/EnglishLanguageAPI.egg-info/requires.txt
+-rw-r--r--   0 guyyatsu  (1000) guyyatsu  (1000)       19 2024-05-03 23:52:28.000000 englishlanguageapi-1.0.0/src/EnglishLanguageAPI.egg-info/top_level.txt
```

