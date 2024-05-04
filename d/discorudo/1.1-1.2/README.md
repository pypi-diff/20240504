# Comparing `tmp/discorudo-1.1.tar.gz` & `tmp/discorudo-1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "discorudo-1.1.tar", last modified: Wed May  1 15:06:51 2024, max compression
+gzip compressed data, was "discorudo-1.2.tar", last modified: Sat May  4 07:46:38 2024, max compression
```

## Comparing `discorudo-1.1.tar` & `discorudo-1.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 gitpod   (33333) gitpod   (33333)        0 2024-05-01 15:06:51.943893 discorudo-1.1/
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)     1049 2024-05-01 15:06:51.943893 discorudo-1.1/PKG-INFO
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)       11 2024-05-01 15:04:25.000000 discorudo-1.1/README.md
-drwxr-xr-x   0 gitpod   (33333) gitpod   (33333)        0 2024-05-01 15:06:51.943893 discorudo-1.1/discorudo/
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)       23 2024-05-01 15:00:23.000000 discorudo-1.1/discorudo/__init__.py
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)       47 2024-05-01 14:59:45.000000 discorudo-1.1/discorudo/main.py
-drwxr-xr-x   0 gitpod   (33333) gitpod   (33333)        0 2024-05-01 15:06:51.943893 discorudo-1.1/discorudo.egg-info/
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)     1049 2024-05-01 15:06:51.000000 discorudo-1.1/discorudo.egg-info/PKG-INFO
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)      222 2024-05-01 15:06:51.000000 discorudo-1.1/discorudo.egg-info/SOURCES.txt
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)        1 2024-05-01 15:06:51.000000 discorudo-1.1/discorudo.egg-info/dependency_links.txt
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)       26 2024-05-01 15:06:51.000000 discorudo-1.1/discorudo.egg-info/requires.txt
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)       10 2024-05-01 15:06:51.000000 discorudo-1.1/discorudo.egg-info/top_level.txt
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)       38 2024-05-01 15:06:51.943893 discorudo-1.1/setup.cfg
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)     2333 2024-05-01 15:05:42.000000 discorudo-1.1/setup.py
+drwxr-xr-x   0 gitpod   (33333) gitpod   (33333)        0 2024-05-04 07:46:38.793629 discorudo-1.2/
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)     1096 2024-05-04 07:46:38.793629 discorudo-1.2/PKG-INFO
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)       11 2024-05-01 15:04:25.000000 discorudo-1.2/README.md
+drwxr-xr-x   0 gitpod   (33333) gitpod   (33333)        0 2024-05-04 07:46:38.793629 discorudo-1.2/discorudo/
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)       44 2024-05-04 07:44:49.000000 discorudo-1.2/discorudo/__init__.py
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)       87 2024-05-04 07:44:36.000000 discorudo-1.2/discorudo/main.py
+drwxr-xr-x   0 gitpod   (33333) gitpod   (33333)        0 2024-05-04 07:46:38.793629 discorudo-1.2/discorudo.egg-info/
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)     1096 2024-05-04 07:46:38.000000 discorudo-1.2/discorudo.egg-info/PKG-INFO
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)      222 2024-05-04 07:46:38.000000 discorudo-1.2/discorudo.egg-info/SOURCES.txt
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)        1 2024-05-04 07:46:38.000000 discorudo-1.2/discorudo.egg-info/dependency_links.txt
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)       43 2024-05-04 07:46:38.000000 discorudo-1.2/discorudo.egg-info/requires.txt
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)       10 2024-05-04 07:46:38.000000 discorudo-1.2/discorudo.egg-info/top_level.txt
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)       38 2024-05-04 07:46:38.793629 discorudo-1.2/setup.cfg
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)     2375 2024-05-04 07:46:06.000000 discorudo-1.2/setup.py
```

### Comparing `discorudo-1.1/PKG-INFO` & `discorudo-1.2/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: discorudo
-Version: 1.1
+Version: 1.2
 Summary: Just script on to discord
 Home-page: https://github.com/rizkychi/discorudo
 Author: rizkychi
 Author-email: rizkynhae@gmail.com
 License: MIT
 Project-URL: Documentation, https://github.com/rizkychi/discorudo/
 Project-URL: Funding, https://www.paypal.me/rizkychi
@@ -19,9 +19,11 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.4
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Description-Content-Type: text/markdown
 Requires-Dist: validators
 Requires-Dist: beautifulsoup4
+Requires-Dist: numpy
+Requires-Dist: matplotlib
 
 # Discorudo
```

### Comparing `discorudo-1.1/discorudo.egg-info/PKG-INFO` & `discorudo-1.2/discorudo.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: discorudo
-Version: 1.1
+Version: 1.2
 Summary: Just script on to discord
 Home-page: https://github.com/rizkychi/discorudo
 Author: rizkychi
 Author-email: rizkynhae@gmail.com
 License: MIT
 Project-URL: Documentation, https://github.com/rizkychi/discorudo/
 Project-URL: Funding, https://www.paypal.me/rizkychi
@@ -19,9 +19,11 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.4
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Description-Content-Type: text/markdown
 Requires-Dist: validators
 Requires-Dist: beautifulsoup4
+Requires-Dist: numpy
+Requires-Dist: matplotlib
 
 # Discorudo
```

### Comparing `discorudo-1.1/setup.py` & `discorudo-1.2/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setup(
     name = 'discorudo',         # How you named your package folder (MyLib)
     packages = ['discorudo'],   # Chose the same as "name"
-    version = '1.1',      # Start with a small number and increase it with every change you make
+    version = '1.2',      # Start with a small number and increase it with every change you make
     license='MIT',        # Chose a license from here: https://help.github.com/articles/licensing-a-repository
     description = 'Just script on to discord',   # Give a short description about your library
     long_description=long_description,            # Give a long description about your library
     long_description_content_type='text/markdown',
     author = 'rizkychi',                   # Type in your name
     author_email = 'rizkynhae@gmail.com',      # Type in your E-Mail
     url = 'https://github.com/rizkychi/discorudo',   # Provide either the link to your github or to your website
@@ -23,14 +23,16 @@
         'Source': 'https://github.com/rizkychi/discorudo/',
         'Tracker': 'https://github.com/rizkychi/discorudo/issues',
     }, 
     keywords = ['discord', 'ai', 'bot', 'messages', 'chatting'],   # Keywords that define your package best
   install_requires=[            # I get to this in a second
           'validators',
           'beautifulsoup4',
+          'numpy',
+          'matplotlib'
       ],
   classifiers=[
     'Development Status :: 3 - Alpha',      # Chose either "3 - Alpha", "4 - Beta" or "5 - Production/Stable" as the current state of your package
     'Intended Audience :: Developers',      # Define that your audience are developers
     'Topic :: Software Development :: Build Tools',
     'License :: OSI Approved :: MIT License',   # Again, pick a license
     'Programming Language :: Python :: 3',      #Specify which pyhton versions that you want to support
```

