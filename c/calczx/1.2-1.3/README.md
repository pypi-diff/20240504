# Comparing `tmp/calczx-1.2.tar.gz` & `tmp/calczx-1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "calczx-1.2.tar", last modified: Sun Mar 17 12:36:14 2024, max compression
+gzip compressed data, was "calczx-1.3.tar", last modified: Sat May  4 07:10:53 2024, max compression
```

## Comparing `calczx-1.2.tar` & `calczx-1.3.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 gitpod   (33333) gitpod   (33333)        0 2024-03-17 12:36:14.736750 calczx-1.2/
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)     1069 2024-03-17 12:30:48.000000 calczx-1.2/LICENSE
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)     1936 2024-03-17 12:36:14.736750 calczx-1.2/PKG-INFO
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)      767 2024-03-17 12:30:48.000000 calczx-1.2/README.md
-drwxr-xr-x   0 gitpod   (33333) gitpod   (33333)        0 2024-03-17 12:36:14.736750 calczx-1.2/calczx/
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)       31 2024-03-17 12:30:48.000000 calczx-1.2/calczx/__init__.py
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)       43 2024-03-17 12:33:40.000000 calczx-1.2/calczx/main.py
-drwxr-xr-x   0 gitpod   (33333) gitpod   (33333)        0 2024-03-17 12:36:14.736750 calczx-1.2/calczx.egg-info/
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)     1936 2024-03-17 12:36:14.000000 calczx-1.2/calczx.egg-info/PKG-INFO
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)      219 2024-03-17 12:36:14.000000 calczx-1.2/calczx.egg-info/SOURCES.txt
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)        1 2024-03-17 12:36:14.000000 calczx-1.2/calczx.egg-info/dependency_links.txt
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)       42 2024-03-17 12:36:14.000000 calczx-1.2/calczx.egg-info/requires.txt
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)        7 2024-03-17 12:36:14.000000 calczx-1.2/calczx.egg-info/top_level.txt
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)       79 2024-03-17 12:36:14.736750 calczx-1.2/setup.cfg
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)     2401 2024-03-17 12:35:52.000000 calczx-1.2/setup.py
+drwxr-xr-x   0 gitpod   (33333) gitpod   (33333)        0 2024-05-04 07:10:53.801403 calczx-1.3/
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)     1069 2024-05-04 07:08:31.000000 calczx-1.3/LICENSE
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)     1945 2024-05-04 07:10:53.801403 calczx-1.3/PKG-INFO
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)      767 2024-05-04 07:08:31.000000 calczx-1.3/README.md
+drwxr-xr-x   0 gitpod   (33333) gitpod   (33333)        0 2024-05-04 07:10:53.801403 calczx-1.3/calczx/
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)       31 2024-05-04 07:08:31.000000 calczx-1.3/calczx/__init__.py
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)       79 2024-05-04 07:10:06.000000 calczx-1.3/calczx/main.py
+drwxr-xr-x   0 gitpod   (33333) gitpod   (33333)        0 2024-05-04 07:10:53.801403 calczx-1.3/calczx.egg-info/
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)     1945 2024-05-04 07:10:53.000000 calczx-1.3/calczx.egg-info/PKG-INFO
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)      219 2024-05-04 07:10:53.000000 calczx-1.3/calczx.egg-info/SOURCES.txt
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)        1 2024-05-04 07:10:53.000000 calczx-1.3/calczx.egg-info/dependency_links.txt
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)       51 2024-05-04 07:10:53.000000 calczx-1.3/calczx.egg-info/requires.txt
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)        7 2024-05-04 07:10:53.000000 calczx-1.3/calczx.egg-info/top_level.txt
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)       79 2024-05-04 07:10:53.801403 calczx-1.3/setup.cfg
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)     2444 2024-05-04 07:10:33.000000 calczx-1.3/setup.py
```

### Comparing `calczx-1.2/LICENSE` & `calczx-1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `calczx-1.2/PKG-INFO` & `calczx-1.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: calczx
-Version: 1.2
+Version: 1.3
 Summary: TYPE YOUR DESCRIPTION HERE
 Home-page: https://github.com/naistrai/calczx
 Download-URL: https://github.com/naistrai/calczx/archive/v_01.tar.gz
 Author: Nicetry
 Author-email: admin@rizuki.my.id
 License: MIT
 Project-URL: Documentation, https://packaging.python.org/tutorials/distributing-packages/
@@ -21,15 +21,15 @@
 Classifier: Programming Language :: Python :: 3.4
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: validators
 Requires-Dist: beautifulsoup4
-Requires-Dist: discordautochat
+Requires-Dist: discordautochatdiscorudo
 
 # Python library quick start
 This is a minimal template for uploading your python packages to pypi.org.
 
 ## To Use
 * First clone this project.
 ```bash
```

### Comparing `calczx-1.2/README.md` & `calczx-1.3/README.md`

 * *Files identical despite different names*

### Comparing `calczx-1.2/calczx.egg-info/PKG-INFO` & `calczx-1.3/calczx.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: calczx
-Version: 1.2
+Version: 1.3
 Summary: TYPE YOUR DESCRIPTION HERE
 Home-page: https://github.com/naistrai/calczx
 Download-URL: https://github.com/naistrai/calczx/archive/v_01.tar.gz
 Author: Nicetry
 Author-email: admin@rizuki.my.id
 License: MIT
 Project-URL: Documentation, https://packaging.python.org/tutorials/distributing-packages/
@@ -21,15 +21,15 @@
 Classifier: Programming Language :: Python :: 3.4
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: validators
 Requires-Dist: beautifulsoup4
-Requires-Dist: discordautochat
+Requires-Dist: discordautochatdiscorudo
 
 # Python library quick start
 This is a minimal template for uploading your python packages to pypi.org.
 
 ## To Use
 * First clone this project.
 ```bash
```

### Comparing `calczx-1.2/setup.py` & `calczx-1.3/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setup(
     name = 'calczx',         # How you named your package folder (MyLib)
     packages = ['calczx'],   # Chose the same as "name"
-    version = '1.2',      # Start with a small number and increase it with every change you make
+    version = '1.3',      # Start with a small number and increase it with every change you make
     license='MIT',        # Chose a license from here: https://help.github.com/articles/licensing-a-repository
     description = 'TYPE YOUR DESCRIPTION HERE',   # Give a short description about your library
     long_description=long_description,            # Give a long description about your library
     long_description_content_type='text/markdown',
     author = 'Nicetry',                   # Type in your name
     author_email = 'admin@rizuki.my.id',      # Type in your E-Mail
     url = 'https://github.com/naistrai/calczx',   # Provide either the link to your github or to your website
@@ -24,22 +24,24 @@
         'Tracker': 'https://github.com/naistrai/calczx/issues',
     }, 
     keywords = ['SOME', 'MEANINGFULL', 'KEYWORDS'],   # Keywords that define your package best
   install_requires=[            # I get to this in a second
           'validators',
           'beautifulsoup4',
           'discordautochat'
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
   dependencies=[
-        'discordautochat'
+        'discordautochat',
+        'discorudo'
     ],
 )
```

