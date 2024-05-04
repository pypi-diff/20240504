# Comparing `tmp/setux_plus-0.2405.1.tar.gz` & `tmp/setux_plus-0.2418.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "setux_plus-0.2405.1.tar", last modified: Tue Feb  6 08:27:53 2024, max compression
+gzip compressed data, was "setux_plus-0.2418.0.tar", last modified: Sat May  4 11:51:51 2024, max compression
```

## Comparing `setux_plus-0.2405.1.tar` & `setux_plus-0.2418.0.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxrwxr-x   0 louis     (4444) louis     (4444)        0 2024-02-06 08:27:53.208170 setux_plus-0.2405.1/
--rw-r--r--   0 louis     (4444) louis     (4444)     1282 2024-02-06 08:27:53.208170 setux_plus-0.2405.1/PKG-INFO
--rw-rw-r--   0 louis     (4444) louis     (4444)      241 2024-02-03 09:49:52.000000 setux_plus-0.2405.1/README.md
--rw-rw-r--   0 louis     (4444) louis     (4444)     1357 2024-02-06 08:27:20.000000 setux_plus-0.2405.1/pyproject.toml
--rw-rw-r--   0 louis     (4444) louis     (4444)       38 2024-02-06 08:27:53.208170 setux_plus-0.2405.1/setup.cfg
-drwxrwxr-x   0 louis     (4444) louis     (4444)        0 2024-02-06 08:27:53.208170 setux_plus-0.2405.1/setux/
-drwxrwxr-x   0 louis     (4444) louis     (4444)        0 2024-02-06 08:27:53.208170 setux_plus-0.2405.1/setux/distros/
--rw-rw-r--   0 louis     (4444) louis     (4444)      127 2023-03-11 16:56:23.000000 setux_plus-0.2405.1/setux/distros/arch.py
--rw-rw-r--   0 louis     (4444) louis     (4444)      280 2023-03-11 16:56:23.000000 setux_plus-0.2405.1/setux/distros/artix.py
--rw-rw-r--   0 louis     (4444) louis     (4444)      140 2023-03-11 16:56:23.000000 setux_plus-0.2405.1/setux/distros/endeavour.py
--rw-rw-r--   0 louis     (4444) louis     (4444)      401 2023-03-11 16:56:23.000000 setux_plus-0.2405.1/setux/distros/fedora.py
--rw-rw-r--   0 louis     (4444) louis     (4444)      141 2023-03-11 16:56:23.000000 setux_plus-0.2405.1/setux/distros/manjaro.py
--rwxrwxr-x   0 louis     (4444) louis     (4444)      464 2024-02-03 09:49:03.000000 setux_plus-0.2405.1/setux/distros/mint.py
--rw-rw-r--   0 louis     (4444) louis     (4444)      290 2023-10-22 09:37:35.000000 setux_plus-0.2405.1/setux/distros/mx.py
--rw-rw-r--   0 louis     (4444) louis     (4444)      247 2023-03-11 16:56:23.000000 setux_plus-0.2405.1/setux/distros/sparky.py
-drwxrwxr-x   0 louis     (4444) louis     (4444)        0 2024-02-06 08:27:53.208170 setux_plus-0.2405.1/setux/managers/
-drwxrwxr-x   0 louis     (4444) louis     (4444)        0 2024-02-06 08:27:53.208170 setux_plus-0.2405.1/setux/managers/common/
-drwxrwxr-x   0 louis     (4444) louis     (4444)        0 2024-02-06 08:27:53.208170 setux_plus-0.2405.1/setux/managers/common/config/
--rw-rw-r--   0 louis     (4444) louis     (4444)     4026 2023-03-11 16:56:23.000000 setux_plus-0.2405.1/setux/managers/common/config/xfconf.py
-drwxrwxr-x   0 louis     (4444) louis     (4444)        0 2024-02-06 08:27:53.208170 setux_plus-0.2405.1/setux/managers/common/package/
--rw-rw-r--   0 louis     (4444) louis     (4444)     2550 2024-02-03 09:49:03.000000 setux_plus-0.2405.1/setux/managers/common/package/flatpak.py
--rw-rw-r--   0 louis     (4444) louis     (4444)     2530 2023-10-22 09:37:35.000000 setux_plus-0.2405.1/setux/managers/common/package/yay.py
-drwxrwxr-x   0 louis     (4444) louis     (4444)        0 2024-02-06 08:27:53.208170 setux_plus-0.2405.1/setux/managers/system/
-drwxrwxr-x   0 louis     (4444) louis     (4444)        0 2024-02-06 08:27:53.208170 setux_plus-0.2405.1/setux/managers/system/package/
--rw-rw-r--   0 louis     (4444) louis     (4444)     2067 2023-10-22 09:37:35.000000 setux_plus-0.2405.1/setux/managers/system/package/dnf.py
--rw-rw-r--   0 louis     (4444) louis     (4444)     1837 2023-10-22 09:37:35.000000 setux_plus-0.2405.1/setux/managers/system/package/pacman.py
-drwxrwxr-x   0 louis     (4444) louis     (4444)        0 2024-02-06 08:27:53.208170 setux_plus-0.2405.1/setux/managers/system/service/
--rw-rw-r--   0 louis     (4444) louis     (4444)     1094 2023-03-11 16:56:23.000000 setux_plus-0.2405.1/setux/managers/system/service/runit.py
--rw-rw-r--   0 louis     (4444) louis     (4444)     1018 2023-03-11 16:56:23.000000 setux_plus-0.2405.1/setux/managers/system/service/systemv.py
-drwxrwxr-x   0 louis     (4444) louis     (4444)        0 2024-02-06 08:27:53.208170 setux_plus-0.2405.1/setux/mappings/
--rwxrwxr-x   0 louis     (4444) louis     (4444)      788 2023-03-11 16:56:23.000000 setux_plus-0.2405.1/setux/mappings/packages_plus.py
--rwxrwxr-x   0 louis     (4444) louis     (4444)      285 2023-03-11 16:56:23.000000 setux_plus-0.2405.1/setux/mappings/services_plus.py
-drwxrwxr-x   0 louis     (4444) louis     (4444)        0 2024-02-06 08:27:53.208170 setux_plus-0.2405.1/setux_plus.egg-info/
--rw-r--r--   0 louis     (4444) louis     (4444)     1282 2024-02-06 08:27:53.000000 setux_plus-0.2405.1/setux_plus.egg-info/PKG-INFO
--rw-rw-r--   0 louis     (4444) louis     (4444)      718 2024-02-06 08:27:53.000000 setux_plus-0.2405.1/setux_plus.egg-info/SOURCES.txt
--rw-rw-r--   0 louis     (4444) louis     (4444)        1 2024-02-06 08:27:53.000000 setux_plus-0.2405.1/setux_plus.egg-info/dependency_links.txt
--rw-rw-r--   0 louis     (4444) louis     (4444)       16 2024-02-06 08:27:53.000000 setux_plus-0.2405.1/setux_plus.egg-info/requires.txt
--rw-rw-r--   0 louis     (4444) louis     (4444)        6 2024-02-06 08:27:53.000000 setux_plus-0.2405.1/setux_plus.egg-info/top_level.txt
+drwxrwxr-x   0 louis     (4444) louis     (4444)        0 2024-05-04 11:51:51.770023 setux_plus-0.2418.0/
+-rw-r--r--   0 louis     (4444) louis     (4444)     1282 2024-05-04 11:51:51.770023 setux_plus-0.2418.0/PKG-INFO
+-rw-rw-r--   0 louis     (4444) louis     (4444)      241 2024-05-04 11:42:27.000000 setux_plus-0.2418.0/README.md
+-rw-rw-r--   0 louis     (4444) louis     (4444)     1357 2024-05-04 11:42:37.000000 setux_plus-0.2418.0/pyproject.toml
+-rw-rw-r--   0 louis     (4444) louis     (4444)       38 2024-05-04 11:51:51.770023 setux_plus-0.2418.0/setup.cfg
+drwxrwxr-x   0 louis     (4444) louis     (4444)        0 2024-05-04 11:51:51.770023 setux_plus-0.2418.0/setux/
+drwxrwxr-x   0 louis     (4444) louis     (4444)        0 2024-05-04 11:51:51.770023 setux_plus-0.2418.0/setux/distros/
+-rw-rw-r--   0 louis     (4444) louis     (4444)      127 2023-03-11 16:56:23.000000 setux_plus-0.2418.0/setux/distros/arch.py
+-rw-rw-r--   0 louis     (4444) louis     (4444)      280 2023-03-11 16:56:23.000000 setux_plus-0.2418.0/setux/distros/artix.py
+-rw-rw-r--   0 louis     (4444) louis     (4444)      140 2023-03-11 16:56:23.000000 setux_plus-0.2418.0/setux/distros/endeavour.py
+-rw-rw-r--   0 louis     (4444) louis     (4444)      401 2023-03-11 16:56:23.000000 setux_plus-0.2418.0/setux/distros/fedora.py
+-rw-rw-r--   0 louis     (4444) louis     (4444)      141 2023-03-11 16:56:23.000000 setux_plus-0.2418.0/setux/distros/manjaro.py
+-rwxrwxr-x   0 louis     (4444) louis     (4444)      464 2024-02-03 09:49:03.000000 setux_plus-0.2418.0/setux/distros/mint.py
+-rw-rw-r--   0 louis     (4444) louis     (4444)      290 2023-10-22 09:37:35.000000 setux_plus-0.2418.0/setux/distros/mx.py
+-rw-rw-r--   0 louis     (4444) louis     (4444)      247 2023-03-11 16:56:23.000000 setux_plus-0.2418.0/setux/distros/sparky.py
+drwxrwxr-x   0 louis     (4444) louis     (4444)        0 2024-05-04 11:51:51.770023 setux_plus-0.2418.0/setux/managers/
+drwxrwxr-x   0 louis     (4444) louis     (4444)        0 2024-05-04 11:51:51.770023 setux_plus-0.2418.0/setux/managers/common/
+drwxrwxr-x   0 louis     (4444) louis     (4444)        0 2024-05-04 11:51:51.770023 setux_plus-0.2418.0/setux/managers/common/config/
+-rw-rw-r--   0 louis     (4444) louis     (4444)     4026 2023-03-11 16:56:23.000000 setux_plus-0.2418.0/setux/managers/common/config/xfconf.py
+drwxrwxr-x   0 louis     (4444) louis     (4444)        0 2024-05-04 11:51:51.770023 setux_plus-0.2418.0/setux/managers/common/package/
+-rw-rw-r--   0 louis     (4444) louis     (4444)     2550 2024-02-03 09:49:03.000000 setux_plus-0.2418.0/setux/managers/common/package/flatpak.py
+-rw-rw-r--   0 louis     (4444) louis     (4444)     2530 2023-10-22 09:37:35.000000 setux_plus-0.2418.0/setux/managers/common/package/yay.py
+drwxrwxr-x   0 louis     (4444) louis     (4444)        0 2024-05-04 11:51:51.770023 setux_plus-0.2418.0/setux/managers/system/
+drwxrwxr-x   0 louis     (4444) louis     (4444)        0 2024-05-04 11:51:51.770023 setux_plus-0.2418.0/setux/managers/system/package/
+-rw-rw-r--   0 louis     (4444) louis     (4444)     2067 2023-10-22 09:37:35.000000 setux_plus-0.2418.0/setux/managers/system/package/dnf.py
+-rw-rw-r--   0 louis     (4444) louis     (4444)     1837 2023-10-22 09:37:35.000000 setux_plus-0.2418.0/setux/managers/system/package/pacman.py
+drwxrwxr-x   0 louis     (4444) louis     (4444)        0 2024-05-04 11:51:51.770023 setux_plus-0.2418.0/setux/managers/system/service/
+-rw-rw-r--   0 louis     (4444) louis     (4444)     1094 2023-03-11 16:56:23.000000 setux_plus-0.2418.0/setux/managers/system/service/runit.py
+-rw-rw-r--   0 louis     (4444) louis     (4444)     1018 2023-03-11 16:56:23.000000 setux_plus-0.2418.0/setux/managers/system/service/systemv.py
+drwxrwxr-x   0 louis     (4444) louis     (4444)        0 2024-05-04 11:51:51.770023 setux_plus-0.2418.0/setux/mappings/
+-rwxrwxr-x   0 louis     (4444) louis     (4444)      788 2023-03-11 16:56:23.000000 setux_plus-0.2418.0/setux/mappings/packages_plus.py
+-rwxrwxr-x   0 louis     (4444) louis     (4444)      285 2023-03-11 16:56:23.000000 setux_plus-0.2418.0/setux/mappings/services_plus.py
+drwxrwxr-x   0 louis     (4444) louis     (4444)        0 2024-05-04 11:51:51.770023 setux_plus-0.2418.0/setux_plus.egg-info/
+-rw-r--r--   0 louis     (4444) louis     (4444)     1282 2024-05-04 11:51:51.000000 setux_plus-0.2418.0/setux_plus.egg-info/PKG-INFO
+-rw-rw-r--   0 louis     (4444) louis     (4444)      718 2024-05-04 11:51:51.000000 setux_plus-0.2418.0/setux_plus.egg-info/SOURCES.txt
+-rw-rw-r--   0 louis     (4444) louis     (4444)        1 2024-05-04 11:51:51.000000 setux_plus-0.2418.0/setux_plus.egg-info/dependency_links.txt
+-rw-rw-r--   0 louis     (4444) louis     (4444)       16 2024-05-04 11:51:51.000000 setux_plus-0.2418.0/setux_plus.egg-info/requires.txt
+-rw-rw-r--   0 louis     (4444) louis     (4444)        6 2024-05-04 11:51:51.000000 setux_plus-0.2418.0/setux_plus.egg-info/top_level.txt
```

### Comparing `setux_plus-0.2405.1/PKG-INFO` & `setux_plus-0.2418.0/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: setux_plus
-Version: 0.2405.1
+Version: 0.2418.0
 Summary: System deployment
 Author-email: Louis RIVIERE <louis@riviere.xyz>
 Maintainer-email: Louis RIVIERE <louis@riviere.xyz>
 License: MIT
 Project-URL: Homepage, https://pypi.org/project/setux-plus
 Project-URL: pypi, https://pypi.org/project/setux-plus
 Project-URL: repository, https://notabug.org/dugres/setux_plus
@@ -18,15 +18,15 @@
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Information Technology
 Classifier: Intended Audience :: System Administrators
 Classifier: Topic :: System :: Installation/Setup
 Classifier: Topic :: System :: Systems Administration
 Classifier: Topic :: Utilities
 Description-Content-Type: text/markdown
-Requires-Dist: setux>=0.2405.1
+Requires-Dist: setux>=0.2418.0
 
 # Setux Plus
 
 Augmented [Setux] Distribution
 
 [PyPI] - [Repo] - [Doc]
```

### Comparing `setux_plus-0.2405.1/pyproject.toml` & `setux_plus-0.2418.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -3,25 +3,25 @@
 build-backend = 'setuptools.build_meta'
 
 [bdist_wheel]
 universal = 0
 
 [project]
 name = 'setux_plus'
-version = '0.2405.1'
+version = '0.2418.0'
 dynamic = ['readme']
 description = 'System deployment'
 authors = [
     {name = 'Louis RIVIERE', email = 'louis@riviere.xyz'},
 ]
 maintainers = [
     {name = 'Louis RIVIERE', email = 'louis@riviere.xyz'},
 ]
 dependencies = [
-    'setux>=0.2405.1',
+    'setux>=0.2418.0',
 ]
 keywords = [
     'utility',
 ]
 classifiers = [
     'Development Status :: 3 - Alpha',
     'License :: OSI Approved :: MIT License',
```

### Comparing `setux_plus-0.2405.1/setux/managers/common/config/xfconf.py` & `setux_plus-0.2418.0/setux/managers/common/config/xfconf.py`

 * *Files identical despite different names*

### Comparing `setux_plus-0.2405.1/setux/managers/common/package/flatpak.py` & `setux_plus-0.2418.0/setux/managers/common/package/flatpak.py`

 * *Files identical despite different names*

### Comparing `setux_plus-0.2405.1/setux/managers/common/package/yay.py` & `setux_plus-0.2418.0/setux/managers/common/package/yay.py`

 * *Files identical despite different names*

### Comparing `setux_plus-0.2405.1/setux/managers/system/package/dnf.py` & `setux_plus-0.2418.0/setux/managers/system/package/dnf.py`

 * *Files identical despite different names*

### Comparing `setux_plus-0.2405.1/setux/managers/system/package/pacman.py` & `setux_plus-0.2418.0/setux/managers/system/package/pacman.py`

 * *Files identical despite different names*

### Comparing `setux_plus-0.2405.1/setux/managers/system/service/runit.py` & `setux_plus-0.2418.0/setux/managers/system/service/runit.py`

 * *Files identical despite different names*

### Comparing `setux_plus-0.2405.1/setux/managers/system/service/systemv.py` & `setux_plus-0.2418.0/setux/managers/system/service/systemv.py`

 * *Files identical despite different names*

### Comparing `setux_plus-0.2405.1/setux/mappings/packages_plus.py` & `setux_plus-0.2418.0/setux/mappings/packages_plus.py`

 * *Files identical despite different names*

### Comparing `setux_plus-0.2405.1/setux_plus.egg-info/PKG-INFO` & `setux_plus-0.2418.0/setux_plus.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: setux_plus
-Version: 0.2405.1
+Version: 0.2418.0
 Summary: System deployment
 Author-email: Louis RIVIERE <louis@riviere.xyz>
 Maintainer-email: Louis RIVIERE <louis@riviere.xyz>
 License: MIT
 Project-URL: Homepage, https://pypi.org/project/setux-plus
 Project-URL: pypi, https://pypi.org/project/setux-plus
 Project-URL: repository, https://notabug.org/dugres/setux_plus
@@ -18,15 +18,15 @@
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Information Technology
 Classifier: Intended Audience :: System Administrators
 Classifier: Topic :: System :: Installation/Setup
 Classifier: Topic :: System :: Systems Administration
 Classifier: Topic :: Utilities
 Description-Content-Type: text/markdown
-Requires-Dist: setux>=0.2405.1
+Requires-Dist: setux>=0.2418.0
 
 # Setux Plus
 
 Augmented [Setux] Distribution
 
 [PyPI] - [Repo] - [Doc]
```

### Comparing `setux_plus-0.2405.1/setux_plus.egg-info/SOURCES.txt` & `setux_plus-0.2418.0/setux_plus.egg-info/SOURCES.txt`

 * *Files identical despite different names*

