# Comparing `tmp/PACMAN-charge-0.1.5.tar.gz` & `tmp/PACMAN-charge-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PACMAN-charge-0.1.5.tar", last modified: Sat May  4 13:44:52 2024, max compression
+gzip compressed data, was "PACMAN-charge-0.1.6.tar", last modified: Sat May  4 13:48:24 2024, max compression
```

## Comparing `PACMAN-charge-0.1.5.tar` & `PACMAN-charge-0.1.6.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-04 13:44:52.326818 PACMAN-charge-0.1.5/
--rwxrwxrwx   0 root         (0) root         (0)     1068 2024-03-25 02:54:44.000000 PACMAN-charge-0.1.5/LICENSE
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-04 13:44:52.203024 PACMAN-charge-0.1.5/PACMANCharge/
--rwxrwxrwx   0 root         (0) root         (0)       33 2024-04-29 12:12:36.000000 PACMAN-charge-0.1.5/PACMANCharge/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)    28392 2024-01-10 01:22:23.000000 PACMAN-charge-0.1.5/PACMANCharge/atom_init.json
--rwxrwxrwx   0 root         (0) root         (0)    26468 2024-05-04 13:44:35.000000 PACMAN-charge-0.1.5/PACMANCharge/pmcharge.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-04 13:44:52.269025 PACMAN-charge-0.1.5/PACMAN_charge.egg-info/
--rwxrwxrwx   0 root         (0) root         (0)     3306 2024-05-04 13:44:51.000000 PACMAN-charge-0.1.5/PACMAN_charge.egg-info/PKG-INFO
--rwxrwxrwx   0 root         (0) root         (0)      334 2024-05-04 13:44:52.000000 PACMAN-charge-0.1.5/PACMAN_charge.egg-info/SOURCES.txt
--rwxrwxrwx   0 root         (0) root         (0)        1 2024-05-04 13:44:52.000000 PACMAN-charge-0.1.5/PACMAN_charge.egg-info/dependency_links.txt
--rwxrwxrwx   0 root         (0) root         (0)      121 2024-05-04 13:44:52.000000 PACMAN-charge-0.1.5/PACMAN_charge.egg-info/requires.txt
--rwxrwxrwx   0 root         (0) root         (0)       18 2024-05-04 13:44:52.000000 PACMAN-charge-0.1.5/PACMAN_charge.egg-info/top_level.txt
--rwxrwxrwx   0 root         (0) root         (0)     3306 2024-05-04 13:44:52.324819 PACMAN-charge-0.1.5/PKG-INFO
--rwxrwxrwx   0 root         (0) root         (0)     2918 2024-05-01 02:30:46.000000 PACMAN-charge-0.1.5/README.md
--rwxrwxrwx   0 root         (0) root         (0)       38 2024-05-04 13:44:52.326818 PACMAN-charge-0.1.5/setup.cfg
--rwxrwxrwx   0 root         (0) root         (0)     1038 2024-05-04 13:44:39.000000 PACMAN-charge-0.1.5/setup.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-04 13:44:52.309025 PACMAN-charge-0.1.5/test/
--rwxrwxrwx   0 root         (0) root         (0)    34098 2024-05-04 13:39:15.000000 PACMAN-charge-0.1.5/test/Cu-BTC.cif
--rwxrwxrwx   0 root         (0) root         (0)        0 2024-03-25 03:31:56.000000 PACMAN-charge-0.1.5/test/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)       76 2024-05-01 02:36:03.000000 PACMAN-charge-0.1.5/test/test.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-04 13:48:24.346207 PACMAN-charge-0.1.6/
+-rwxrwxrwx   0 root         (0) root         (0)     1068 2024-03-25 02:54:44.000000 PACMAN-charge-0.1.6/LICENSE
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-04 13:48:24.219205 PACMAN-charge-0.1.6/PACMANCharge/
+-rwxrwxrwx   0 root         (0) root         (0)       33 2024-04-29 12:12:36.000000 PACMAN-charge-0.1.6/PACMANCharge/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)    28392 2024-01-10 01:22:23.000000 PACMAN-charge-0.1.6/PACMANCharge/atom_init.json
+-rwxrwxrwx   0 root         (0) root         (0)    26468 2024-05-04 13:45:43.000000 PACMAN-charge-0.1.6/PACMANCharge/pmcharge.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-04 13:48:24.288206 PACMAN-charge-0.1.6/PACMAN_charge.egg-info/
+-rwxrwxrwx   0 root         (0) root         (0)     3306 2024-05-04 13:48:24.000000 PACMAN-charge-0.1.6/PACMAN_charge.egg-info/PKG-INFO
+-rwxrwxrwx   0 root         (0) root         (0)      334 2024-05-04 13:48:24.000000 PACMAN-charge-0.1.6/PACMAN_charge.egg-info/SOURCES.txt
+-rwxrwxrwx   0 root         (0) root         (0)        1 2024-05-04 13:48:24.000000 PACMAN-charge-0.1.6/PACMAN_charge.egg-info/dependency_links.txt
+-rwxrwxrwx   0 root         (0) root         (0)      121 2024-05-04 13:48:24.000000 PACMAN-charge-0.1.6/PACMAN_charge.egg-info/requires.txt
+-rwxrwxrwx   0 root         (0) root         (0)       18 2024-05-04 13:48:24.000000 PACMAN-charge-0.1.6/PACMAN_charge.egg-info/top_level.txt
+-rwxrwxrwx   0 root         (0) root         (0)     3306 2024-05-04 13:48:24.344208 PACMAN-charge-0.1.6/PKG-INFO
+-rwxrwxrwx   0 root         (0) root         (0)     2918 2024-05-01 02:30:46.000000 PACMAN-charge-0.1.6/README.md
+-rwxrwxrwx   0 root         (0) root         (0)       38 2024-05-04 13:48:24.346207 PACMAN-charge-0.1.6/setup.cfg
+-rwxrwxrwx   0 root         (0) root         (0)     1038 2024-05-04 13:48:17.000000 PACMAN-charge-0.1.6/setup.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-04 13:48:24.328205 PACMAN-charge-0.1.6/test/
+-rwxrwxrwx   0 root         (0) root         (0)    34098 2024-05-04 13:47:28.000000 PACMAN-charge-0.1.6/test/Cu-BTC.cif
+-rwxrwxrwx   0 root         (0) root         (0)        0 2024-03-25 03:31:56.000000 PACMAN-charge-0.1.6/test/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)      151 2024-05-04 13:47:26.000000 PACMAN-charge-0.1.6/test/test.py
```

### Comparing `PACMAN-charge-0.1.5/LICENSE` & `PACMAN-charge-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `PACMAN-charge-0.1.5/PACMANCharge/atom_init.json` & `PACMAN-charge-0.1.6/PACMANCharge/atom_init.json`

 * *Files identical despite different names*

### Comparing `PACMAN-charge-0.1.5/PACMANCharge/pmcharge.py` & `PACMAN-charge-0.1.6/PACMANCharge/pmcharge.py`

 * *Files 0% similar despite different names*

```diff
@@ -22,16 +22,16 @@
 files_to_download = {
                     'mof-cm5.pth': 'https://raw.githubusercontent.com/sxm13/PACMAN/main/pth/best_cm5/cm5.pth',
                     'mof-cm5.pkl': 'https://raw.githubusercontent.com/sxm13/PACMAN/main/pth/best_cm5/normalizer-cm5.pkl',
                     'mof-bader.pth': 'https://raw.githubusercontent.com/sxm13/PACMAN/main/pth/best_bader/bader.pth',
                     'mof-bader.pkl': 'https://raw.githubusercontent.com/sxm13/PACMAN/main/pth/best_bader/normalizer-bader.pkl',
                     'mof-ddec.pth': 'https://raw.githubusercontent.com/sxm13/PACMAN/main/pth/best_ddec/ddec.pth',
                     'mof-ddec.pkl': 'https://raw.githubusercontent.com/sxm13/PACMAN/main/pth/best_ddec/normalizer-ddec.pkl',
-                    'cof.pth': 'https://raw.githubusercontent.com/sxm13/PACMAN/main/pth/best_ddec_COF/ddec.pth',
-                    'cof.pkl': 'https://raw.githubusercontent.com/sxm13/PACMAN/main/pth/best_ddec_COF/normalizer-ddec.pkl',
+                    'cof.pth': 'https://raw.githubusercontent.com/sxm13/PACMAN/main/pth/best_ddec_cof/ddec.pth',
+                    'cof.pkl': 'https://raw.githubusercontent.com/sxm13/PACMAN/main/pth/best_ddec_cof/normalizer-ddec.pkl',
                     }
 
 for file_name, url in files_to_download.items():
     file_path = os.path.join(package_directory, file_name)
     if not os.path.exists(file_path):
         response = requests.get(url)
         if response.status_code == 200:
```

### Comparing `PACMAN-charge-0.1.5/PACMAN_charge.egg-info/PKG-INFO` & `PACMAN-charge-0.1.6/PACMAN_charge.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PACMAN-charge
-Version: 0.1.5
+Version: 0.1.6
 Summary: Partial Atomic Charges for Porous Materials based on Graph Convolutional Neural Network (PACMAN)
 Home-page: https://github.com/sxm13/PACMAN
 Author: Guobin Zhao
 Author-email: sxmzhaogb@gmai.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `PACMAN-charge-0.1.5/PKG-INFO` & `PACMAN-charge-0.1.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PACMAN-charge
-Version: 0.1.5
+Version: 0.1.6
 Summary: Partial Atomic Charges for Porous Materials based on Graph Convolutional Neural Network (PACMAN)
 Home-page: https://github.com/sxm13/PACMAN
 Author: Guobin Zhao
 Author-email: sxmzhaogb@gmai.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `PACMAN-charge-0.1.5/README.md` & `PACMAN-charge-0.1.6/README.md`

 * *Files identical despite different names*

### Comparing `PACMAN-charge-0.1.5/setup.py` & `PACMAN-charge-0.1.6/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import requests
 from setuptools import setup, find_packages
 
 setup(
     name="PACMAN-charge",
-    version="0.1.5",
+    version="0.1.6",
     packages=find_packages(),
     description="Partial Atomic Charges for Porous Materials based on Graph Convolutional Neural Network (PACMAN)",
     author="Guobin Zhao",
     author_email="sxmzhaogb@gmai.com",
     url="https://github.com/sxm13/PACMAN",
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
```

### Comparing `PACMAN-charge-0.1.5/test/Cu-BTC.cif` & `PACMAN-charge-0.1.6/test/Cu-BTC.cif`

 * *Files identical despite different names*

