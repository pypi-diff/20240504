# Comparing `tmp/ssm_svg-0.0.7.tar.gz` & `tmp/ssm_svg-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ssm_svg-0.0.7.tar", last modified: Fri May  3 05:36:35 2024, max compression
+gzip compressed data, was "ssm_svg-0.0.8.tar", last modified: Fri May  3 16:06:32 2024, max compression
```

## Comparing `ssm_svg-0.0.7.tar` & `ssm_svg-0.0.8.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 05:36:35.721920 ssm_svg-0.0.7/
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-05-03 05:36:24.000000 ssm_svg-0.0.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     4651 2024-05-03 05:36:35.721920 ssm_svg-0.0.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4217 2024-05-03 05:36:24.000000 ssm_svg-0.0.7/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-03 05:36:35.721920 ssm_svg-0.0.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      921 2024-05-03 05:36:24.000000 ssm_svg-0.0.7/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 05:36:35.717920 ssm_svg-0.0.7/ssm/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 05:36:24.000000 ssm_svg-0.0.7/ssm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       62 2024-05-03 05:36:24.000000 ssm_svg-0.0.7/ssm/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)       63 2024-05-03 05:36:24.000000 ssm_svg-0.0.7/ssm/__version__.py
--rw-r--r--   0 runner    (1001) docker     (127)    16283 2024-05-03 05:36:24.000000 ssm_svg-0.0.7/ssm/ssm.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 05:36:35.721920 ssm_svg-0.0.7/ssm_svg.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4651 2024-05-03 05:36:35.000000 ssm_svg-0.0.7/ssm_svg.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      294 2024-05-03 05:36:35.000000 ssm_svg-0.0.7/ssm_svg.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-03 05:36:35.000000 ssm_svg-0.0.7/ssm_svg.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       37 2024-05-03 05:36:35.000000 ssm_svg-0.0.7/ssm_svg.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-03 05:36:35.000000 ssm_svg-0.0.7/ssm_svg.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        4 2024-05-03 05:36:35.000000 ssm_svg-0.0.7/ssm_svg.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 05:36:35.721920 ssm_svg-0.0.7/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     7499 2024-05-03 05:36:24.000000 ssm_svg-0.0.7/tests/test_ssm.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 16:06:32.711890 ssm_svg-0.0.8/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-05-03 16:06:25.000000 ssm_svg-0.0.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     4687 2024-05-03 16:06:32.711890 ssm_svg-0.0.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4253 2024-05-03 16:06:25.000000 ssm_svg-0.0.8/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-03 16:06:32.711890 ssm_svg-0.0.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      921 2024-05-03 16:06:25.000000 ssm_svg-0.0.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 16:06:32.707890 ssm_svg-0.0.8/ssm/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 16:06:25.000000 ssm_svg-0.0.8/ssm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-05-03 16:06:25.000000 ssm_svg-0.0.8/ssm/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       63 2024-05-03 16:06:25.000000 ssm_svg-0.0.8/ssm/__version__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16283 2024-05-03 16:06:25.000000 ssm_svg-0.0.8/ssm/ssm.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 16:06:32.711890 ssm_svg-0.0.8/ssm_svg.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4687 2024-05-03 16:06:32.000000 ssm_svg-0.0.8/ssm_svg.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      294 2024-05-03 16:06:32.000000 ssm_svg-0.0.8/ssm_svg.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-03 16:06:32.000000 ssm_svg-0.0.8/ssm_svg.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-05-03 16:06:32.000000 ssm_svg-0.0.8/ssm_svg.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-03 16:06:32.000000 ssm_svg-0.0.8/ssm_svg.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        4 2024-05-03 16:06:32.000000 ssm_svg-0.0.8/ssm_svg.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 16:06:32.707890 ssm_svg-0.0.8/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     7499 2024-05-03 16:06:25.000000 ssm_svg-0.0.8/tests/test_ssm.py
```

### Comparing `ssm_svg-0.0.7/LICENSE` & `ssm_svg-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `ssm_svg-0.0.7/PKG-INFO` & `ssm_svg-0.0.8/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ssm-svg
-Version: 0.0.7
+Version: 0.0.8
 Summary: SVG spritesheet maker
 Home-page: https://github.com/obeezzy/ssm
 Author: Chronic Coder
 Author-email: efeoghene.obebeduo@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -14,15 +14,15 @@
 Requires-Dist: lxml
 
 # ssm
 
 SVG spritesheet maker
 
 [![CI](https://github.com/obeezzy/ssm/actions/workflows/main.yml/badge.svg)](https://github.com/obeezzy/ssm/actions/workflows/main.yml)
-[![Deployment to PyPI](https://github.com/obeezzy/ssm/actions/workflows/deploy.yml/badge.svg?branch=v0.0.7)](https://github.com/obeezzy/ssm/actions/workflows/deploy.yml)
+[![Deployment to PyPI](https://github.com/obeezzy/ssm/actions/workflows/deploy.yml/badge.svg?branch=v0.0.8)](https://github.com/obeezzy/ssm/actions/workflows/deploy.yml)
 
 __ssm__ is a command-line tool for creating and managing SVG spritesheets. It has 5 main functions:
 
 * __create__: For creating spritesheets from a list of SVG sprites (i.e. SVG icons etc.).
 * __list__: For listing the SVG sprites stored in a spritesheet.
 * __add__: For adding SVG sprites to an existing spritesheet.
 * __remove__: For removing SVG sprites from an existing spritesheet.
@@ -48,38 +48,38 @@
   <defs>
     <symbol id="search" viewBox="0 0 24 24">...</symbol>
     <symbol id="menu" viewBox="0 0 24 24">...</symbol>
   </defs>
 </svg>
 ```
 
-Create spritesheet and overwrite existing file:
+Create spritesheet and overwrite existing file (with the `-F` option):
 
 ```bash
 $ ssm create -f icons.svg search.svg menu.svg -F
 ```
 
 Create spritesheet containing `search.svg` and `menu.svg`, with custom ID `hamburger-icon` for `menu.svg` (instead of defaulting to its file name):
 
 ```bash
-$ ssm create -f icons.svg search.svg hamburger-icon=menu.svg
+$ ssm create -f icons.svg search.svg hamburger-icon=menu.svg -F
 $ cat icons.svg
 <svg xmlns="http://www.w3.org/2000/svg">
   <defs>
     <symbol id="search" viewBox="0 0 24 24">...</symbol>
     <symbol id="hamburger-icon" viewBox="0 0 24 24">...</symbol>
   </defs>
 </svg>
 ```
 
 List IDs of sprites in spritesheet:
 
 ```bash
 $ ssm list -f icons.svg
-menu
+hamburger-icon
 search
 ```
 
 Add `facebook.svg` and `instagram.svg` to spritesheet:
 
 ```bash
 $ ssm add -f icons.svg facebook.svg instagram.svg
```

### Comparing `ssm_svg-0.0.7/README.md` & `ssm_svg-0.0.8/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # ssm
 
 SVG spritesheet maker
 
 [![CI](https://github.com/obeezzy/ssm/actions/workflows/main.yml/badge.svg)](https://github.com/obeezzy/ssm/actions/workflows/main.yml)
-[![Deployment to PyPI](https://github.com/obeezzy/ssm/actions/workflows/deploy.yml/badge.svg?branch=v0.0.7)](https://github.com/obeezzy/ssm/actions/workflows/deploy.yml)
+[![Deployment to PyPI](https://github.com/obeezzy/ssm/actions/workflows/deploy.yml/badge.svg?branch=v0.0.8)](https://github.com/obeezzy/ssm/actions/workflows/deploy.yml)
 
 __ssm__ is a command-line tool for creating and managing SVG spritesheets. It has 5 main functions:
 
 * __create__: For creating spritesheets from a list of SVG sprites (i.e. SVG icons etc.).
 * __list__: For listing the SVG sprites stored in a spritesheet.
 * __add__: For adding SVG sprites to an existing spritesheet.
 * __remove__: For removing SVG sprites from an existing spritesheet.
@@ -33,38 +33,38 @@
   <defs>
     <symbol id="search" viewBox="0 0 24 24">...</symbol>
     <symbol id="menu" viewBox="0 0 24 24">...</symbol>
   </defs>
 </svg>
 ```
 
-Create spritesheet and overwrite existing file:
+Create spritesheet and overwrite existing file (with the `-F` option):
 
 ```bash
 $ ssm create -f icons.svg search.svg menu.svg -F
 ```
 
 Create spritesheet containing `search.svg` and `menu.svg`, with custom ID `hamburger-icon` for `menu.svg` (instead of defaulting to its file name):
 
 ```bash
-$ ssm create -f icons.svg search.svg hamburger-icon=menu.svg
+$ ssm create -f icons.svg search.svg hamburger-icon=menu.svg -F
 $ cat icons.svg
 <svg xmlns="http://www.w3.org/2000/svg">
   <defs>
     <symbol id="search" viewBox="0 0 24 24">...</symbol>
     <symbol id="hamburger-icon" viewBox="0 0 24 24">...</symbol>
   </defs>
 </svg>
 ```
 
 List IDs of sprites in spritesheet:
 
 ```bash
 $ ssm list -f icons.svg
-menu
+hamburger-icon
 search
 ```
 
 Add `facebook.svg` and `instagram.svg` to spritesheet:
 
 ```bash
 $ ssm add -f icons.svg facebook.svg instagram.svg
```

### Comparing `ssm_svg-0.0.7/setup.py` & `ssm_svg-0.0.8/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 # The text of the README file
 README = (ROOT_DIR / "README.md").read_text()
 
 # This call to setup() does all the work
 setup(
     name="ssm-svg",
-    version="0.0.7",
+    version="0.0.8",
     description="SVG spritesheet maker",
     long_description=README,
     long_description_content_type="text/markdown",
     url="https://github.com/obeezzy/ssm",
     author="Chronic Coder",
     author_email="efeoghene.obebeduo@gmail.com",
     license="MIT",
```

### Comparing `ssm_svg-0.0.7/ssm/ssm.py` & `ssm_svg-0.0.8/ssm/ssm.py`

 * *Files identical despite different names*

### Comparing `ssm_svg-0.0.7/ssm_svg.egg-info/PKG-INFO` & `ssm_svg-0.0.8/ssm_svg.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ssm-svg
-Version: 0.0.7
+Version: 0.0.8
 Summary: SVG spritesheet maker
 Home-page: https://github.com/obeezzy/ssm
 Author: Chronic Coder
 Author-email: efeoghene.obebeduo@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -14,15 +14,15 @@
 Requires-Dist: lxml
 
 # ssm
 
 SVG spritesheet maker
 
 [![CI](https://github.com/obeezzy/ssm/actions/workflows/main.yml/badge.svg)](https://github.com/obeezzy/ssm/actions/workflows/main.yml)
-[![Deployment to PyPI](https://github.com/obeezzy/ssm/actions/workflows/deploy.yml/badge.svg?branch=v0.0.7)](https://github.com/obeezzy/ssm/actions/workflows/deploy.yml)
+[![Deployment to PyPI](https://github.com/obeezzy/ssm/actions/workflows/deploy.yml/badge.svg?branch=v0.0.8)](https://github.com/obeezzy/ssm/actions/workflows/deploy.yml)
 
 __ssm__ is a command-line tool for creating and managing SVG spritesheets. It has 5 main functions:
 
 * __create__: For creating spritesheets from a list of SVG sprites (i.e. SVG icons etc.).
 * __list__: For listing the SVG sprites stored in a spritesheet.
 * __add__: For adding SVG sprites to an existing spritesheet.
 * __remove__: For removing SVG sprites from an existing spritesheet.
@@ -48,38 +48,38 @@
   <defs>
     <symbol id="search" viewBox="0 0 24 24">...</symbol>
     <symbol id="menu" viewBox="0 0 24 24">...</symbol>
   </defs>
 </svg>
 ```
 
-Create spritesheet and overwrite existing file:
+Create spritesheet and overwrite existing file (with the `-F` option):
 
 ```bash
 $ ssm create -f icons.svg search.svg menu.svg -F
 ```
 
 Create spritesheet containing `search.svg` and `menu.svg`, with custom ID `hamburger-icon` for `menu.svg` (instead of defaulting to its file name):
 
 ```bash
-$ ssm create -f icons.svg search.svg hamburger-icon=menu.svg
+$ ssm create -f icons.svg search.svg hamburger-icon=menu.svg -F
 $ cat icons.svg
 <svg xmlns="http://www.w3.org/2000/svg">
   <defs>
     <symbol id="search" viewBox="0 0 24 24">...</symbol>
     <symbol id="hamburger-icon" viewBox="0 0 24 24">...</symbol>
   </defs>
 </svg>
 ```
 
 List IDs of sprites in spritesheet:
 
 ```bash
 $ ssm list -f icons.svg
-menu
+hamburger-icon
 search
 ```
 
 Add `facebook.svg` and `instagram.svg` to spritesheet:
 
 ```bash
 $ ssm add -f icons.svg facebook.svg instagram.svg
```

### Comparing `ssm_svg-0.0.7/tests/test_ssm.py` & `ssm_svg-0.0.8/tests/test_ssm.py`

 * *Files identical despite different names*

