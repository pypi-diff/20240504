# Comparing `tmp/asyncAminoLab-1.0.tar.gz` & `tmp/asyncAminoLab-1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "asyncAminoLab-1.0.tar", last modified: Sat May  4 11:26:18 2024, max compression
+gzip compressed data, was "asyncAminoLab-1.1.tar", last modified: Sat May  4 11:53:08 2024, max compression
```

## Comparing `asyncAminoLab-1.0.tar` & `asyncAminoLab-1.1.tar`

### file list

```diff
@@ -1,10 +1,10 @@
-drwx------   0 u0_a406  (10406) u0_a406  (10406)        0 2024-05-04 11:26:18.453859 asyncAminoLab-1.0/
--rw-r--r--   0 u0_a406  (10406) u0_a406  (10406)      468 2024-05-04 11:26:18.449859 asyncAminoLab-1.0/PKG-INFO
-drwx------   0 u0_a406  (10406) u0_a406  (10406)        0 2024-05-04 11:26:18.449859 asyncAminoLab-1.0/asyncAminoLab.egg-info/
--rw-r--r--   0 u0_a406  (10406) u0_a406  (10406)      468 2024-05-04 11:26:18.000000 asyncAminoLab-1.0/asyncAminoLab.egg-info/PKG-INFO
--rw-------   0 u0_a406  (10406) u0_a406  (10406)      192 2024-05-04 11:26:18.000000 asyncAminoLab-1.0/asyncAminoLab.egg-info/SOURCES.txt
--rw-------   0 u0_a406  (10406) u0_a406  (10406)        1 2024-05-04 11:26:18.000000 asyncAminoLab-1.0/asyncAminoLab.egg-info/dependency_links.txt
--rw-------   0 u0_a406  (10406) u0_a406  (10406)       19 2024-05-04 11:26:18.000000 asyncAminoLab-1.0/asyncAminoLab.egg-info/requires.txt
--rw-------   0 u0_a406  (10406) u0_a406  (10406)        9 2024-05-04 11:26:18.000000 asyncAminoLab-1.0/asyncAminoLab.egg-info/top_level.txt
--rw-------   0 u0_a406  (10406) u0_a406  (10406)       38 2024-05-04 11:26:18.453859 asyncAminoLab-1.0/setup.cfg
--rw-------   0 u0_a406  (10406) u0_a406  (10406)      773 2024-05-04 11:25:43.000000 asyncAminoLab-1.0/setup.py
+drwx------   0 u0_a406  (10406) u0_a406  (10406)        0 2024-05-04 11:53:08.373875 asyncAminoLab-1.1/
+-rw-r--r--   0 u0_a406  (10406) u0_a406  (10406)      607 2024-05-04 11:53:08.373875 asyncAminoLab-1.1/PKG-INFO
+drwx------   0 u0_a406  (10406) u0_a406  (10406)        0 2024-05-04 11:53:08.369875 asyncAminoLab-1.1/asyncAminoLab.egg-info/
+-rw-r--r--   0 u0_a406  (10406) u0_a406  (10406)      607 2024-05-04 11:53:08.000000 asyncAminoLab-1.1/asyncAminoLab.egg-info/PKG-INFO
+-rw-------   0 u0_a406  (10406) u0_a406  (10406)      192 2024-05-04 11:53:08.000000 asyncAminoLab-1.1/asyncAminoLab.egg-info/SOURCES.txt
+-rw-------   0 u0_a406  (10406) u0_a406  (10406)        1 2024-05-04 11:53:08.000000 asyncAminoLab-1.1/asyncAminoLab.egg-info/dependency_links.txt
+-rw-------   0 u0_a406  (10406) u0_a406  (10406)       16 2024-05-04 11:53:08.000000 asyncAminoLab-1.1/asyncAminoLab.egg-info/requires.txt
+-rw-------   0 u0_a406  (10406) u0_a406  (10406)        1 2024-05-04 11:53:08.000000 asyncAminoLab-1.1/asyncAminoLab.egg-info/top_level.txt
+-rw-------   0 u0_a406  (10406) u0_a406  (10406)       38 2024-05-04 11:53:08.373875 asyncAminoLab-1.1/setup.cfg
+-rw-------   0 u0_a406  (10406) u0_a406  (10406)      957 2024-05-04 11:50:53.000000 asyncAminoLab-1.1/setup.py
```

### Comparing `asyncAminoLab-1.0/setup.py` & `asyncAminoLab-1.1/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,29 +1,35 @@
 from setuptools import setup, find_packages
 setup(name='asyncAminoLab',
-      version='1.0',
+      version='1.1',
       url = 'https://github.com/l0v3m0n3y/AminoLab',
     download_url = 'https://github.com/l0v3m0n3y/AminoLab/archive/refs/heads/main.zip',
       description='async libary for aminoapps.com. ton wallet: UQAeAZH2DkWqsU8zLtdpx9ELkM0agCtCoi8myYkPOJ-9ObNS',
-      packages=['AminoLab'],
       author_email="pepsiritp@gmail.com",
+      long_description = """# AminoLab
+AminoLab Api For AminoApps using aminoapps.com/api
+
+### Installing
+`pip install AminoLab`""",
+    long_description_content_type ='text/markdown',
       keywords = [
         'aminoapps',
         'amino-py',
         'amino',
         'amino-bot',
         'narvii',
         'api',
         'python',
         'python3',
         'python3.x',
         'botamino',
         'AminoLab'
     ],
     install_requires = [
-        'setuptools',
         'aiohttp',
+        'asyncio'
     ],
     setup_requires = [
         'wheel'
-    ]
+    ],
+    packages = find_packages()
 )
```

