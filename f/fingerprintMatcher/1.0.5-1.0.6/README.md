# Comparing `tmp/fingerprintMatcher-1.0.5.tar.gz` & `tmp/fingerprintMatcher-1.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fingerprintMatcher-1.0.5.tar", last modified: Mon Apr 15 06:24:06 2024, max compression
+gzip compressed data, was "fingerprintMatcher-1.0.6.tar", last modified: Sat May  4 09:17:34 2024, max compression
```

## Comparing `fingerprintMatcher-1.0.5.tar` & `fingerprintMatcher-1.0.6.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxrwx   0        0        0        0 2024-04-15 06:24:06.152633 fingerprintMatcher-1.0.5/
--rw-rw-rw-   0        0        0     2572 2024-04-15 06:24:06.141375 fingerprintMatcher-1.0.5/PKG-INFO
--rw-rw-rw-   0        0        0     1705 2024-04-14 12:03:30.000000 fingerprintMatcher-1.0.5/README.md
-drwxrwxrwx   0        0        0        0 2024-04-15 06:24:06.141375 fingerprintMatcher-1.0.5/fingerprintMatcher.egg-info/
--rw-rw-rw-   0        0        0     2572 2024-04-15 06:24:06.000000 fingerprintMatcher-1.0.5/fingerprintMatcher.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      249 2024-04-15 06:24:06.000000 fingerprintMatcher-1.0.5/fingerprintMatcher.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-15 06:24:06.000000 fingerprintMatcher-1.0.5/fingerprintMatcher.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       43 2024-04-15 06:24:06.000000 fingerprintMatcher-1.0.5/fingerprintMatcher.egg-info/requires.txt
--rw-rw-rw-   0        0        0       19 2024-04-15 06:24:06.000000 fingerprintMatcher-1.0.5/fingerprintMatcher.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     3643 2024-04-14 10:59:09.000000 fingerprintMatcher-1.0.5/fingerprintmatcher.py
--rw-rw-rw-   0        0        0       42 2024-04-15 06:24:06.152633 fingerprintMatcher-1.0.5/setup.cfg
--rw-rw-rw-   0        0        0     1161 2024-04-15 06:24:02.000000 fingerprintMatcher-1.0.5/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-04 09:17:34.358283 fingerprintMatcher-1.0.6/
+-rw-rw-rw-   0        0        0     2572 2024-05-04 09:17:34.351624 fingerprintMatcher-1.0.6/PKG-INFO
+-rw-rw-rw-   0        0        0     1705 2024-04-14 12:03:30.000000 fingerprintMatcher-1.0.6/README.md
+drwxrwxrwx   0        0        0        0 2024-05-04 09:17:34.351624 fingerprintMatcher-1.0.6/fingerprintMatcher.egg-info/
+-rw-rw-rw-   0        0        0     2572 2024-05-04 09:17:34.000000 fingerprintMatcher-1.0.6/fingerprintMatcher.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      249 2024-05-04 09:17:34.000000 fingerprintMatcher-1.0.6/fingerprintMatcher.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-04 09:17:34.000000 fingerprintMatcher-1.0.6/fingerprintMatcher.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       43 2024-05-04 09:17:34.000000 fingerprintMatcher-1.0.6/fingerprintMatcher.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       19 2024-05-04 09:17:34.000000 fingerprintMatcher-1.0.6/fingerprintMatcher.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     3650 2024-05-04 09:12:12.000000 fingerprintMatcher-1.0.6/fingerprintmatcher.py
+-rw-rw-rw-   0        0        0       42 2024-05-04 09:17:34.358283 fingerprintMatcher-1.0.6/setup.cfg
+-rw-rw-rw-   0        0        0     1161 2024-05-04 09:17:25.000000 fingerprintMatcher-1.0.6/setup.py
```

### Comparing `fingerprintMatcher-1.0.5/PKG-INFO` & `fingerprintMatcher-1.0.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fingerprintMatcher
-Version: 1.0.5
+Version: 1.0.6
 Summary: The FingerprintMatcher Python package provides a comprehensive toolkit for fingerprint matching and recognition tasks. With its intuitive interface and powerful functionality, this package enables users to compare fingerprint images, match them against a database of known fingerprints, and determine their similarity with high accuracy.
 Home-page: https://github.com/Tharunk07/fingerprintMatcher
 Author: Tharun K
 Author-email: tharunkkumarasamy@gmail.com
 Project-URL: Bug Tracker, https://github.com/Tharunk07/fingerprintMatcher/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `fingerprintMatcher-1.0.5/README.md` & `fingerprintMatcher-1.0.6/README.md`

 * *Files identical despite different names*

### Comparing `fingerprintMatcher-1.0.5/fingerprintMatcher.egg-info/PKG-INFO` & `fingerprintMatcher-1.0.6/fingerprintMatcher.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fingerprintMatcher
-Version: 1.0.5
+Version: 1.0.6
 Summary: The FingerprintMatcher Python package provides a comprehensive toolkit for fingerprint matching and recognition tasks. With its intuitive interface and powerful functionality, this package enables users to compare fingerprint images, match them against a database of known fingerprints, and determine their similarity with high accuracy.
 Home-page: https://github.com/Tharunk07/fingerprintMatcher
 Author: Tharun K
 Author-email: tharunkkumarasamy@gmail.com
 Project-URL: Bug Tracker, https://github.com/Tharunk07/fingerprintMatcher/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `fingerprintMatcher-1.0.5/fingerprintmatcher.py` & `fingerprintMatcher-1.0.6/fingerprintmatcher.py`

 * *Files 1% similar despite different names*

```diff
@@ -80,15 +80,15 @@
                 if p.distance < 0.1 * q.distance:
                     match_points.append(p)
 
             keypoints_count = min(len(keypoints_1), len(keypoints_2))
             match_ratio = len(match_points) / keypoints_count
 
             if match_ratio > 0.95:
-                print(f"The image is matched with {file}")
+                print(f"The image is matched with file : {file}")
                 print("percentage(%) of match: ", len(match_points) / keypoints_count * 100)
                 result = cv2.drawMatches(test_original, keypoints_1, fingerprint_database_image, keypoints_2, match_points, None)
                 result = cv2.resize(result, None, fx=1, fy=1)
                 cv2.imshow("result", result)
                 cv2.waitKey(1000)
                 cv2.destroyAllWindows()
                 match_found = True
```

### Comparing `fingerprintMatcher-1.0.5/setup.py` & `fingerprintMatcher-1.0.6/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name='fingerprintMatcher',
-    version='1.0.5',
+    version='1.0.6',
     author='Tharun K',
     author_email='tharunkkumarasamy@gmail.com',
     description='The FingerprintMatcher Python package provides a comprehensive toolkit for fingerprint matching and recognition tasks. With its intuitive interface and powerful functionality, this package enables users to compare fingerprint images, match them against a database of known fingerprints, and determine their similarity with high accuracy.',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/Tharunk07/fingerprintMatcher',
     project_urls={
```

