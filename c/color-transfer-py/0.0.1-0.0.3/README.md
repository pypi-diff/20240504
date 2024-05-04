# Comparing `tmp/color_transfer_py-0.0.1.tar.gz` & `tmp/color_transfer_py-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "color_transfer_py-0.0.1.tar", last modified: Sat May  4 14:09:54 2024, max compression
+gzip compressed data, was "color_transfer_py-0.0.3.tar", last modified: Sat May  4 14:59:12 2024, max compression
```

## Comparing `color_transfer_py-0.0.1.tar` & `color_transfer_py-0.0.3.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2024-05-04 14:09:54.627063 color_transfer_py-0.0.1/
--rw-rw-rw-   0        0        0     1085 2024-05-04 12:51:43.000000 color_transfer_py-0.0.1/LICENSE.txt
--rw-rw-rw-   0        0        0     2139 2024-05-04 14:09:54.625970 color_transfer_py-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0     1560 2024-05-04 13:24:29.000000 color_transfer_py-0.0.1/README.md
-drwxrwxrwx   0        0        0        0 2024-05-04 14:09:54.624970 color_transfer_py-0.0.1/color_transfer_py.egg-info/
--rw-rw-rw-   0        0        0     2139 2024-05-04 14:09:54.000000 color_transfer_py-0.0.1/color_transfer_py.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      249 2024-05-04 14:09:54.000000 color_transfer_py-0.0.1/color_transfer_py.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-04 14:09:54.000000 color_transfer_py-0.0.1/color_transfer_py.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       35 2024-05-04 14:09:54.000000 color_transfer_py-0.0.1/color_transfer_py.egg-info/requires.txt
--rw-rw-rw-   0        0        0        1 2024-05-04 14:09:54.000000 color_transfer_py-0.0.1/color_transfer_py.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      202 2024-05-04 12:50:39.000000 color_transfer_py-0.0.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-05-04 14:09:54.627063 color_transfer_py-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0      997 2024-05-04 14:07:51.000000 color_transfer_py-0.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-04 14:59:12.595951 color_transfer_py-0.0.3/
+-rw-rw-rw-   0        0        0     1085 2024-05-04 12:51:43.000000 color_transfer_py-0.0.3/LICENSE.txt
+-rw-rw-rw-   0        0        0     2142 2024-05-04 14:59:12.595951 color_transfer_py-0.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0     1560 2024-05-04 13:24:29.000000 color_transfer_py-0.0.3/README.md
+drwxrwxrwx   0        0        0        0 2024-05-04 14:59:12.595951 color_transfer_py-0.0.3/color_transfer_py.egg-info/
+-rw-rw-rw-   0        0        0     2142 2024-05-04 14:59:12.000000 color_transfer_py-0.0.3/color_transfer_py.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      249 2024-05-04 14:59:12.000000 color_transfer_py-0.0.3/color_transfer_py.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-04 14:59:12.000000 color_transfer_py-0.0.3/color_transfer_py.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       38 2024-05-04 14:59:12.000000 color_transfer_py-0.0.3/color_transfer_py.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        1 2024-05-04 14:59:12.000000 color_transfer_py-0.0.3/color_transfer_py.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      202 2024-05-04 12:50:39.000000 color_transfer_py-0.0.3/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-05-04 14:59:12.595951 color_transfer_py-0.0.3/setup.cfg
+-rw-rw-rw-   0        0        0     1003 2024-05-04 14:58:01.000000 color_transfer_py-0.0.3/setup.py
```

### Comparing `color_transfer_py-0.0.1/LICENSE.txt` & `color_transfer_py-0.0.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `color_transfer_py-0.0.1/PKG-INFO` & `color_transfer_py-0.0.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: color_transfer_py
-Version: 0.0.1
+Version: 0.0.3
 Summary: Color transfer between images
 Home-page: https://github.com/ptran1203/color_transfer
 Author: Phat Tran
 Author-email: phatth1203@gmail.com
 Project-URL: Bug Tracker, https://github.com/ptran1203/color_transfer/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
-Requires-Dist: opencv-python==4.7.0
+Requires-Dist: opencv-python>=4.7.0.72
 Requires-Dist: torch>=1.13.0
 
 # Color transfer between images
 
 - Paper: [Color Transfer between Images](https://www.cs.tau.ac.il/~turkel/imagepapers/ColorTransfer.pdf) by Erik Reinhard, Michael Ashikhmin, Bruce Gooch and Peter Shirley.
 - This is the re-implementation based on: https://github.com/chia56028/Color-Transfer-between-Images.
 - The transfer process performed in numpy array instead of looping over pixel to improve performance.
```

### Comparing `color_transfer_py-0.0.1/README.md` & `color_transfer_py-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `color_transfer_py-0.0.1/color_transfer_py.egg-info/PKG-INFO` & `color_transfer_py-0.0.3/color_transfer_py.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: color_transfer_py
-Version: 0.0.1
+Version: 0.0.3
 Summary: Color transfer between images
 Home-page: https://github.com/ptran1203/color_transfer
 Author: Phat Tran
 Author-email: phatth1203@gmail.com
 Project-URL: Bug Tracker, https://github.com/ptran1203/color_transfer/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
-Requires-Dist: opencv-python==4.7.0
+Requires-Dist: opencv-python>=4.7.0.72
 Requires-Dist: torch>=1.13.0
 
 # Color transfer between images
 
 - Paper: [Color Transfer between Images](https://www.cs.tau.ac.il/~turkel/imagepapers/ColorTransfer.pdf) by Erik Reinhard, Michael Ashikhmin, Bruce Gooch and Peter Shirley.
 - This is the re-implementation based on: https://github.com/chia56028/Color-Transfer-between-Images.
 - The transfer process performed in numpy array instead of looping over pixel to improve performance.
```

### Comparing `color_transfer_py-0.0.1/setup.py` & `color_transfer_py-0.0.3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding = "utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name = "color_transfer_py",
-    version = "0.0.1",
+    version = "0.0.3",
     author = "Phat Tran",
     author_email = "phatth1203@gmail.com",
     description = "Color transfer between images",
     long_description = long_description,
     long_description_content_type = "text/markdown",
     url = "https://github.com/ptran1203/color_transfer",
     project_urls = {
@@ -18,11 +18,11 @@
     classifiers = [
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
     # package_dir = {"": "."},
     packages=setuptools.find_packages(),
-    install_requires=['opencv-python==4.7.0', 'torch>=1.13.0'],
+    install_requires=['opencv-python>=4.7.0.72', 'torch>=1.13.0'],
     setup_requires=['pytest-runner==5.3.1'],
-    tests_require=['pytest==6.2.5', 'opencv-python==4.7.0'],
+    tests_require=['pytest==6.2.5', 'opencv-python>=4.7.0.72'],
 )
```

