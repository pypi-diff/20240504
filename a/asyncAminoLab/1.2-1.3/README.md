# Comparing `tmp/asyncAminoLab-1.2.tar.gz` & `tmp/asyncAminoLab-1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "asyncAminoLab-1.2.tar", last modified: Sat May  4 12:26:54 2024, max compression
+gzip compressed data, was "asyncAminoLab-1.3.tar", last modified: Sat May  4 12:34:37 2024, max compression
```

## Comparing `asyncAminoLab-1.2.tar` & `asyncAminoLab-1.3.tar`

### file list

```diff
@@ -1,10 +1,10 @@
-drwx------   0 u0_a406  (10406) u0_a406  (10406)        0 2024-05-04 12:26:54.969968 asyncAminoLab-1.2/
--rw-r--r--   0 u0_a406  (10406) u0_a406  (10406)      584 2024-05-04 12:26:54.965968 asyncAminoLab-1.2/PKG-INFO
-drwx------   0 u0_a406  (10406) u0_a406  (10406)        0 2024-05-04 12:26:54.965968 asyncAminoLab-1.2/asyncAminoLab.egg-info/
--rw-r--r--   0 u0_a406  (10406) u0_a406  (10406)      584 2024-05-04 12:26:54.000000 asyncAminoLab-1.2/asyncAminoLab.egg-info/PKG-INFO
--rw-------   0 u0_a406  (10406) u0_a406  (10406)      192 2024-05-04 12:26:54.000000 asyncAminoLab-1.2/asyncAminoLab.egg-info/SOURCES.txt
--rw-------   0 u0_a406  (10406) u0_a406  (10406)        1 2024-05-04 12:26:54.000000 asyncAminoLab-1.2/asyncAminoLab.egg-info/dependency_links.txt
--rw-------   0 u0_a406  (10406) u0_a406  (10406)        8 2024-05-04 12:26:54.000000 asyncAminoLab-1.2/asyncAminoLab.egg-info/requires.txt
--rw-------   0 u0_a406  (10406) u0_a406  (10406)        1 2024-05-04 12:26:54.000000 asyncAminoLab-1.2/asyncAminoLab.egg-info/top_level.txt
--rw-------   0 u0_a406  (10406) u0_a406  (10406)       38 2024-05-04 12:26:54.969968 asyncAminoLab-1.2/setup.cfg
--rw-------   0 u0_a406  (10406) u0_a406  (10406)      938 2024-05-04 12:26:08.000000 asyncAminoLab-1.2/setup.py
+drwx------   0 u0_a406  (10406) u0_a406  (10406)        0 2024-05-04 12:34:37.605968 asyncAminoLab-1.3/
+-rw-r--r--   0 u0_a406  (10406) u0_a406  (10406)      589 2024-05-04 12:34:37.605968 asyncAminoLab-1.3/PKG-INFO
+drwx------   0 u0_a406  (10406) u0_a406  (10406)        0 2024-05-04 12:34:37.601968 asyncAminoLab-1.3/asyncAminoLab.egg-info/
+-rw-r--r--   0 u0_a406  (10406) u0_a406  (10406)      589 2024-05-04 12:34:37.000000 asyncAminoLab-1.3/asyncAminoLab.egg-info/PKG-INFO
+-rw-------   0 u0_a406  (10406) u0_a406  (10406)      192 2024-05-04 12:34:37.000000 asyncAminoLab-1.3/asyncAminoLab.egg-info/SOURCES.txt
+-rw-------   0 u0_a406  (10406) u0_a406  (10406)        1 2024-05-04 12:34:37.000000 asyncAminoLab-1.3/asyncAminoLab.egg-info/dependency_links.txt
+-rw-------   0 u0_a406  (10406) u0_a406  (10406)        8 2024-05-04 12:34:37.000000 asyncAminoLab-1.3/asyncAminoLab.egg-info/requires.txt
+-rw-------   0 u0_a406  (10406) u0_a406  (10406)        1 2024-05-04 12:34:37.000000 asyncAminoLab-1.3/asyncAminoLab.egg-info/top_level.txt
+-rw-------   0 u0_a406  (10406) u0_a406  (10406)       38 2024-05-04 12:34:37.605968 asyncAminoLab-1.3/setup.cfg
+-rw-------   0 u0_a406  (10406) u0_a406  (10406)      943 2024-05-04 12:33:03.000000 asyncAminoLab-1.3/setup.py
```

### Comparing `asyncAminoLab-1.2/PKG-INFO` & `asyncAminoLab-1.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: asyncAminoLab
-Version: 1.2
+Version: 1.3
 Summary: async libary for aminoapps.com. ton wallet: UQAeAZH2DkWqsU8zLtdpx9ELkM0agCtCoi8myYkPOJ-9ObNS
 Home-page: https://github.com/l0v3m0n3y/AminoLab
 Download-URL: https://github.com/l0v3m0n3y/AminoLab/archive/refs/heads/main.zip
 Author-email: pepsiritp@gmail.com
 Keywords: aminoapps,amino-py,amino,amino-bot,narvii,api,python,python3,python3.x,botamino,AminoLab
 Description-Content-Type: text/markdown
 Requires-Dist: aiohttp
 
 # AminoLab
 AminoLab Api For AminoApps using aminoapps.com/api
 
 ### Installing
-`pip install AminoLab`
+`pip install asyncAminoLab`
```

### Comparing `asyncAminoLab-1.2/asyncAminoLab.egg-info/PKG-INFO` & `asyncAminoLab-1.3/asyncAminoLab.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: asyncAminoLab
-Version: 1.2
+Version: 1.3
 Summary: async libary for aminoapps.com. ton wallet: UQAeAZH2DkWqsU8zLtdpx9ELkM0agCtCoi8myYkPOJ-9ObNS
 Home-page: https://github.com/l0v3m0n3y/AminoLab
 Download-URL: https://github.com/l0v3m0n3y/AminoLab/archive/refs/heads/main.zip
 Author-email: pepsiritp@gmail.com
 Keywords: aminoapps,amino-py,amino,amino-bot,narvii,api,python,python3,python3.x,botamino,AminoLab
 Description-Content-Type: text/markdown
 Requires-Dist: aiohttp
 
 # AminoLab
 AminoLab Api For AminoApps using aminoapps.com/api
 
 ### Installing
-`pip install AminoLab`
+`pip install asyncAminoLab`
```

### Comparing `asyncAminoLab-1.2/setup.py` & `asyncAminoLab-1.3/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 from setuptools import setup, find_packages
 setup(name='asyncAminoLab',
-      version='1.2',
+      version='1.3',
       url = 'https://github.com/l0v3m0n3y/AminoLab',
     download_url = 'https://github.com/l0v3m0n3y/AminoLab/archive/refs/heads/main.zip',
       description='async libary for aminoapps.com. ton wallet: UQAeAZH2DkWqsU8zLtdpx9ELkM0agCtCoi8myYkPOJ-9ObNS',
       author_email="pepsiritp@gmail.com",
       long_description = """# AminoLab
 AminoLab Api For AminoApps using aminoapps.com/api
 
 ### Installing
-`pip install AminoLab`""",
+`pip install asyncAminoLab`""",
     long_description_content_type ='text/markdown',
       keywords = [
         'aminoapps',
         'amino-py',
         'amino',
         'amino-bot',
         'narvii',
```

