# Comparing `tmp/resszo-0.1.tar.gz` & `tmp/resszo-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "resszo-0.1.tar", last modified: Wed May  1 15:32:00 2024, max compression
+gzip compressed data, was "resszo-0.2.tar", last modified: Sat May  4 06:51:19 2024, max compression
```

## Comparing `resszo-0.1.tar` & `resszo-0.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 gitpod   (33333) gitpod   (33333)        0 2024-05-01 15:32:00.028802 resszo-0.1/
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)     1069 2024-05-01 15:24:31.000000 resszo-0.1/LICENSE
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)     1810 2024-05-01 15:32:00.028802 resszo-0.1/PKG-INFO
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)      767 2024-05-01 15:24:31.000000 resszo-0.1/README.md
-drwxr-xr-x   0 gitpod   (33333) gitpod   (33333)        0 2024-05-01 15:32:00.024802 resszo-0.1/resszo/
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)       31 2024-05-01 15:30:21.000000 resszo-0.1/resszo/__init__.py
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)       36 2024-05-01 15:29:17.000000 resszo-0.1/resszo/main.py
-drwxr-xr-x   0 gitpod   (33333) gitpod   (33333)        0 2024-05-01 15:32:00.028802 resszo-0.1/resszo.egg-info/
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)     1810 2024-05-01 15:31:59.000000 resszo-0.1/resszo.egg-info/PKG-INFO
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)      219 2024-05-01 15:31:59.000000 resszo-0.1/resszo.egg-info/SOURCES.txt
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)        1 2024-05-01 15:31:59.000000 resszo-0.1/resszo.egg-info/dependency_links.txt
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)       36 2024-05-01 15:31:59.000000 resszo-0.1/resszo.egg-info/requires.txt
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)        7 2024-05-01 15:31:59.000000 resszo-0.1/resszo.egg-info/top_level.txt
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)       79 2024-05-01 15:32:00.028802 resszo-0.1/setup.cfg
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)     2292 2024-05-01 15:31:35.000000 resszo-0.1/setup.py
+drwxr-xr-x   0 gitpod   (33333) gitpod   (33333)        0 2024-05-04 06:51:19.799862 resszo-0.2/
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)     1069 2024-05-01 15:24:31.000000 resszo-0.2/LICENSE
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)     1858 2024-05-04 06:51:19.799862 resszo-0.2/PKG-INFO
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)      767 2024-05-01 15:24:31.000000 resszo-0.2/README.md
+drwxr-xr-x   0 gitpod   (33333) gitpod   (33333)        0 2024-05-04 06:51:19.799862 resszo-0.2/resszo/
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)       31 2024-05-01 15:30:21.000000 resszo-0.2/resszo/__init__.py
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)       36 2024-05-01 15:29:17.000000 resszo-0.2/resszo/main.py
+drwxr-xr-x   0 gitpod   (33333) gitpod   (33333)        0 2024-05-04 06:51:19.799862 resszo-0.2/resszo.egg-info/
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)     1858 2024-05-04 06:51:19.000000 resszo-0.2/resszo.egg-info/PKG-INFO
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)      219 2024-05-04 06:51:19.000000 resszo-0.2/resszo.egg-info/SOURCES.txt
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)        1 2024-05-04 06:51:19.000000 resszo-0.2/resszo.egg-info/dependency_links.txt
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)       52 2024-05-04 06:51:19.000000 resszo-0.2/resszo.egg-info/requires.txt
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)        7 2024-05-04 06:51:19.000000 resszo-0.2/resszo.egg-info/top_level.txt
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)       79 2024-05-04 06:51:19.799862 resszo-0.2/setup.cfg
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)     2402 2024-05-04 06:51:17.000000 resszo-0.2/setup.py
```

### Comparing `resszo-0.1/LICENSE` & `resszo-0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `resszo-0.1/PKG-INFO` & `resszo-0.2/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,34 +1,35 @@
 Metadata-Version: 2.1
 Name: resszo
-Version: 0.1
+Version: 0.2
 Summary: TYPE YOUR DESCRIPTION HERE
-Home-page: https://github.com/user/resszo
-Author: YOUR NAME
-Author-email: your.email@domain.com
+Home-page: https://github.com/naistrai/resszo
+Author: Naistrai
+Author-email: rizkynaistrai@gmail.com
 License: MIT
-Project-URL: Documentation, https://github.com/pypa/resszo/
+Project-URL: Documentation, https://github.com/naistrai/resszo/
 Project-URL: Funding, https://donate.pypi.org
 Project-URL: Say Thanks!, http://saythanks.io/to/example
-Project-URL: Source, https://github.com/pypa/resszo/
-Project-URL: Tracker, https://github.com/pypa/resszo/issues
+Project-URL: Source, https://github.com/naistrai/resszo/
+Project-URL: Tracker, https://github.com/naistrai/resszo/issues
 Keywords: SOME,MEANINGFULL,KEYWORDS
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.4
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: validators
 Requires-Dist: beautifulsoup4
 Requires-Dist: discorudo
+Requires-Dist: discordautochat
 
 # Python library quick start
 This is a minimal template for uploading your python packages to pypi.org.
 
 ## To Use
 * First clone this project.
 ```bash
```

### Comparing `resszo-0.1/README.md` & `resszo-0.2/README.md`

 * *Files identical despite different names*

### Comparing `resszo-0.1/resszo.egg-info/PKG-INFO` & `resszo-0.2/resszo.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,34 +1,35 @@
 Metadata-Version: 2.1
 Name: resszo
-Version: 0.1
+Version: 0.2
 Summary: TYPE YOUR DESCRIPTION HERE
-Home-page: https://github.com/user/resszo
-Author: YOUR NAME
-Author-email: your.email@domain.com
+Home-page: https://github.com/naistrai/resszo
+Author: Naistrai
+Author-email: rizkynaistrai@gmail.com
 License: MIT
-Project-URL: Documentation, https://github.com/pypa/resszo/
+Project-URL: Documentation, https://github.com/naistrai/resszo/
 Project-URL: Funding, https://donate.pypi.org
 Project-URL: Say Thanks!, http://saythanks.io/to/example
-Project-URL: Source, https://github.com/pypa/resszo/
-Project-URL: Tracker, https://github.com/pypa/resszo/issues
+Project-URL: Source, https://github.com/naistrai/resszo/
+Project-URL: Tracker, https://github.com/naistrai/resszo/issues
 Keywords: SOME,MEANINGFULL,KEYWORDS
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.4
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: validators
 Requires-Dist: beautifulsoup4
 Requires-Dist: discorudo
+Requires-Dist: discordautochat
 
 # Python library quick start
 This is a minimal template for uploading your python packages to pypi.org.
 
 ## To Use
 * First clone this project.
 ```bash
```

### Comparing `resszo-0.1/setup.py` & `resszo-0.2/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -3,40 +3,45 @@
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setup(
     name = 'resszo',         # How you named your package folder (MyLib)
     packages = ['resszo'],   # Chose the same as "name"
-    version = '0.1',      # Start with a small number and increase it with every change you make
+    version = '0.2',      # Start with a small number and increase it with every change you make
     license='MIT',        # Chose a license from here: https://help.github.com/articles/licensing-a-repository
     description = 'TYPE YOUR DESCRIPTION HERE',   # Give a short description about your library
     long_description=long_description,            # Give a long description about your library
     long_description_content_type='text/markdown',
-    author = 'YOUR NAME',                   # Type in your name
-    author_email = 'your.email@domain.com',      # Type in your E-Mail
-    url = 'https://github.com/user/resszo',   # Provide either the link to your github or to your website
-    # download_url = 'https://github.com/user/resszo/archive/v_01.tar.gz',    # I explain this later on
+    author = 'Naistrai',                   # Type in your name
+    author_email = 'rizkynaistrai@gmail.com',      # Type in your E-Mail
+    url = 'https://github.com/naistrai/resszo',   # Provide either the link to your github or to your website
+    # download_url = 'https://github.com/naistrai/resszo/archive/v_01.tar.gz',    # I explain this later on
     project_urls={
-        'Documentation': 'https://github.com/pypa/resszo/',
+        'Documentation': 'https://github.com/naistrai/resszo/',
         'Funding': 'https://donate.pypi.org',
         'Say Thanks!': 'http://saythanks.io/to/example',
-        'Source': 'https://github.com/pypa/resszo/',
-        'Tracker': 'https://github.com/pypa/resszo/issues',
+        'Source': 'https://github.com/naistrai/resszo/',
+        'Tracker': 'https://github.com/naistrai/resszo/issues',
     }, 
     keywords = ['SOME', 'MEANINGFULL', 'KEYWORDS'],   # Keywords that define your package best
   install_requires=[            # I get to this in a second
           'validators',
           'beautifulsoup4',
-          'discorudo'
+          'discorudo',
+          'discordautochat'
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
-  ], 
+  ],
+  dependencies=[
+    'discordautochat',
+    'discorudo'
+  ],
 )
```

