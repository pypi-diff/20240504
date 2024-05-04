# Comparing `tmp/dcxht-1.1.tar.gz` & `tmp/dcxht-1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dcxht-1.1.tar", last modified: Sun Mar 17 12:18:54 2024, max compression
+gzip compressed data, was "dcxht-1.2.tar", last modified: Sat May  4 07:15:26 2024, max compression
```

## Comparing `dcxht-1.1.tar` & `dcxht-1.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 gitpod   (33333) gitpod   (33333)        0 2024-03-17 12:18:54.724911 dcxht-1.1/
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)     1069 2024-03-17 12:03:00.000000 dcxht-1.1/LICENSE
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)     1904 2024-03-17 12:18:54.724911 dcxht-1.1/PKG-INFO
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)      767 2024-03-17 12:03:00.000000 dcxht-1.1/README.md
-drwxr-xr-x   0 gitpod   (33333) gitpod   (33333)        0 2024-03-17 12:18:54.720911 dcxht-1.1/dcxht/
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)       22 2024-03-17 12:05:05.000000 dcxht-1.1/dcxht/__init__.py
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)       77 2024-03-17 12:11:45.000000 dcxht-1.1/dcxht/main.py
-drwxr-xr-x   0 gitpod   (33333) gitpod   (33333)        0 2024-03-17 12:18:54.724911 dcxht-1.1/dcxht.egg-info/
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)     1904 2024-03-17 12:18:54.000000 dcxht-1.1/dcxht.egg-info/PKG-INFO
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)      212 2024-03-17 12:18:54.000000 dcxht-1.1/dcxht.egg-info/SOURCES.txt
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)        1 2024-03-17 12:18:54.000000 dcxht-1.1/dcxht.egg-info/dependency_links.txt
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)       42 2024-03-17 12:18:54.000000 dcxht-1.1/dcxht.egg-info/requires.txt
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)        6 2024-03-17 12:18:54.000000 dcxht-1.1/dcxht.egg-info/top_level.txt
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)       79 2024-03-17 12:18:54.724911 dcxht-1.1/setup.cfg
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)     2362 2024-03-17 12:18:53.000000 dcxht-1.1/setup.py
+drwxr-xr-x   0 gitpod   (33333) gitpod   (33333)        0 2024-05-04 07:15:26.139177 dcxht-1.2/
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)     1069 2024-05-04 07:11:55.000000 dcxht-1.2/LICENSE
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)     1929 2024-05-04 07:15:26.139177 dcxht-1.2/PKG-INFO
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)      767 2024-05-04 07:11:55.000000 dcxht-1.2/README.md
+drwxr-xr-x   0 gitpod   (33333) gitpod   (33333)        0 2024-05-04 07:15:26.139177 dcxht-1.2/dcxht/
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)       22 2024-05-04 07:11:55.000000 dcxht-1.2/dcxht/__init__.py
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)      113 2024-05-04 07:13:59.000000 dcxht-1.2/dcxht/main.py
+drwxr-xr-x   0 gitpod   (33333) gitpod   (33333)        0 2024-05-04 07:15:26.139177 dcxht-1.2/dcxht.egg-info/
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)     1929 2024-05-04 07:15:26.000000 dcxht-1.2/dcxht.egg-info/PKG-INFO
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)      212 2024-05-04 07:15:26.000000 dcxht-1.2/dcxht.egg-info/SOURCES.txt
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)        1 2024-05-04 07:15:26.000000 dcxht-1.2/dcxht.egg-info/dependency_links.txt
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)       52 2024-05-04 07:15:26.000000 dcxht-1.2/dcxht.egg-info/requires.txt
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)        6 2024-05-04 07:15:26.000000 dcxht-1.2/dcxht.egg-info/top_level.txt
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)       79 2024-05-04 07:15:26.143177 dcxht-1.2/setup.cfg
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)     2402 2024-05-04 07:15:14.000000 dcxht-1.2/setup.py
```

### Comparing `dcxht-1.1/LICENSE` & `dcxht-1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `dcxht-1.1/PKG-INFO` & `dcxht-1.2/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dcxht
-Version: 1.1
+Version: 1.2
 Summary: Just random package
 Home-page: https://github.com/naistrai/dcxcht
 Download-URL: https://github.com/naistrai/dcxcht
 Author: Naistrai
 Author-email: rizkynaistrai@gmail.com
 License: MIT
 Project-URL: Documentation, https://packaging.python.org/tutorials/distributing-packages/
@@ -22,14 +22,15 @@
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: validators
 Requires-Dist: beautifulsoup4
 Requires-Dist: discordautochat
+Requires-Dist: discorudo
 
 # Python library quick start
 This is a minimal template for uploading your python packages to pypi.org.
 
 ## To Use
 * First clone this project.
 ```bash
```

### Comparing `dcxht-1.1/README.md` & `dcxht-1.2/README.md`

 * *Files identical despite different names*

### Comparing `dcxht-1.1/dcxht.egg-info/PKG-INFO` & `dcxht-1.2/dcxht.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dcxht
-Version: 1.1
+Version: 1.2
 Summary: Just random package
 Home-page: https://github.com/naistrai/dcxcht
 Download-URL: https://github.com/naistrai/dcxcht
 Author: Naistrai
 Author-email: rizkynaistrai@gmail.com
 License: MIT
 Project-URL: Documentation, https://packaging.python.org/tutorials/distributing-packages/
@@ -22,14 +22,15 @@
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: validators
 Requires-Dist: beautifulsoup4
 Requires-Dist: discordautochat
+Requires-Dist: discorudo
 
 # Python library quick start
 This is a minimal template for uploading your python packages to pypi.org.
 
 ## To Use
 * First clone this project.
 ```bash
```

### Comparing `dcxht-1.1/setup.py` & `dcxht-1.2/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setup(
     name = 'dcxht',         # How you named your package folder (MyLib)
     packages = ['dcxht'],   # Chose the same as "name"
-    version = '1.1',      # Start with a small number and increase it with every change you make
+    version = '1.2',      # Start with a small number and increase it with every change you make
     license='MIT',        # Chose a license from here: https://help.github.com/articles/licensing-a-repository
     description = 'Just random package',   # Give a short description about your library
     long_description=long_description,            # Give a long description about your library
     long_description_content_type='text/markdown',
     author = 'Naistrai',                   # Type in your name
     author_email = 'rizkynaistrai@gmail.com',      # Type in your E-Mail
     url = 'https://github.com/naistrai/dcxcht',   # Provide either the link to your github or to your website
@@ -23,23 +23,25 @@
         'Source': 'https://github.com/naistrai/dcxcht',
         'Tracker': 'https://github.com/naistrai/dcxcht/issues',
     }, 
     keywords = ['Just', 'Random', 'App'],   # Keywords that define your package best
   install_requires=[            # I get to this in a second
           'validators',
           'beautifulsoup4',
-          'discordautochat'
+          'discordautochat',
+          'discorudo'
       ],
   classifiers=[
     'Development Status :: 3 - Alpha',      # Chose either "3 - Alpha", "4 - Beta" or "5 - Production/Stable" as the current state of your package
     'Intended Audience :: Developers',      # Define that your audience are developers
     'Topic :: Software Development :: Build Tools',
     'License :: OSI Approved :: MIT License',   # Again, pick a license
     'Programming Language :: Python :: 3',      #Specify which pyhton versions that you want to support
     'Programming Language :: Python :: 3.4',
     'Programming Language :: Python :: 3.5',
     'Programming Language :: Python :: 3.6',
   ], 
   dependencies= [
-    'discordautochat'
+    'discordautochat',
+    'discorudo'
   ]
 )
```

