# Comparing `tmp/PACMAN-charge-0.1.3.tar.gz` & `tmp/PACMAN-charge-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PACMAN-charge-0.1.3.tar", last modified: Sat May  4 13:24:03 2024, max compression
+gzip compressed data, was "PACMAN-charge-0.1.4.tar", last modified: Sat May  4 13:31:53 2024, max compression
```

## Comparing `PACMAN-charge-0.1.3.tar` & `PACMAN-charge-0.1.4.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-04 13:24:03.528351 PACMAN-charge-0.1.3/
--rwxrwxrwx   0 root         (0) root         (0)     1068 2024-03-25 02:54:44.000000 PACMAN-charge-0.1.3/LICENSE
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-04 13:24:03.358302 PACMAN-charge-0.1.3/PACMANCharge/
--rwxrwxrwx   0 root         (0) root         (0)       33 2024-04-29 12:12:36.000000 PACMAN-charge-0.1.3/PACMANCharge/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)    28392 2024-01-10 01:22:23.000000 PACMAN-charge-0.1.3/PACMANCharge/atom_init.json
--rwxrwxrwx   0 root         (0) root         (0)    26400 2024-05-04 13:21:02.000000 PACMAN-charge-0.1.3/PACMANCharge/pmcharge.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-04 13:24:03.424300 PACMAN-charge-0.1.3/PACMAN_charge.egg-info/
--rwxrwxrwx   0 root         (0) root         (0)     3306 2024-05-04 13:24:03.000000 PACMAN-charge-0.1.3/PACMAN_charge.egg-info/PKG-INFO
--rwxrwxrwx   0 root         (0) root         (0)      334 2024-05-04 13:24:03.000000 PACMAN-charge-0.1.3/PACMAN_charge.egg-info/SOURCES.txt
--rwxrwxrwx   0 root         (0) root         (0)        1 2024-05-04 13:24:03.000000 PACMAN-charge-0.1.3/PACMAN_charge.egg-info/dependency_links.txt
--rwxrwxrwx   0 root         (0) root         (0)      121 2024-05-04 13:24:03.000000 PACMAN-charge-0.1.3/PACMAN_charge.egg-info/requires.txt
--rwxrwxrwx   0 root         (0) root         (0)       18 2024-05-04 13:24:03.000000 PACMAN-charge-0.1.3/PACMAN_charge.egg-info/top_level.txt
--rwxrwxrwx   0 root         (0) root         (0)     3306 2024-05-04 13:24:03.526350 PACMAN-charge-0.1.3/PKG-INFO
--rwxrwxrwx   0 root         (0) root         (0)     2918 2024-05-01 02:30:46.000000 PACMAN-charge-0.1.3/README.md
--rwxrwxrwx   0 root         (0) root         (0)       38 2024-05-04 13:24:03.529350 PACMAN-charge-0.1.3/setup.cfg
--rwxrwxrwx   0 root         (0) root         (0)     1038 2024-05-04 13:15:18.000000 PACMAN-charge-0.1.3/setup.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-04 13:24:03.511350 PACMAN-charge-0.1.3/test/
--rwxrwxrwx   0 root         (0) root         (0)    34098 2024-05-01 02:36:11.000000 PACMAN-charge-0.1.3/test/Cu-BTC.cif
--rwxrwxrwx   0 root         (0) root         (0)        0 2024-03-25 03:31:56.000000 PACMAN-charge-0.1.3/test/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)       76 2024-05-01 02:36:03.000000 PACMAN-charge-0.1.3/test/test.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-04 13:31:53.607896 PACMAN-charge-0.1.4/
+-rwxrwxrwx   0 root         (0) root         (0)     1068 2024-03-25 02:54:44.000000 PACMAN-charge-0.1.4/LICENSE
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-04 13:31:53.472907 PACMAN-charge-0.1.4/PACMANCharge/
+-rwxrwxrwx   0 root         (0) root         (0)       33 2024-04-29 12:12:36.000000 PACMAN-charge-0.1.4/PACMANCharge/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)    28392 2024-01-10 01:22:23.000000 PACMAN-charge-0.1.4/PACMANCharge/atom_init.json
+-rwxrwxrwx   0 root         (0) root         (0)    26396 2024-05-04 13:30:46.000000 PACMAN-charge-0.1.4/PACMANCharge/pmcharge.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-04 13:31:53.552896 PACMAN-charge-0.1.4/PACMAN_charge.egg-info/
+-rwxrwxrwx   0 root         (0) root         (0)     3306 2024-05-04 13:31:53.000000 PACMAN-charge-0.1.4/PACMAN_charge.egg-info/PKG-INFO
+-rwxrwxrwx   0 root         (0) root         (0)      334 2024-05-04 13:31:53.000000 PACMAN-charge-0.1.4/PACMAN_charge.egg-info/SOURCES.txt
+-rwxrwxrwx   0 root         (0) root         (0)        1 2024-05-04 13:31:53.000000 PACMAN-charge-0.1.4/PACMAN_charge.egg-info/dependency_links.txt
+-rwxrwxrwx   0 root         (0) root         (0)      121 2024-05-04 13:31:53.000000 PACMAN-charge-0.1.4/PACMAN_charge.egg-info/requires.txt
+-rwxrwxrwx   0 root         (0) root         (0)       18 2024-05-04 13:31:53.000000 PACMAN-charge-0.1.4/PACMAN_charge.egg-info/top_level.txt
+-rwxrwxrwx   0 root         (0) root         (0)     3306 2024-05-04 13:31:53.605897 PACMAN-charge-0.1.4/PKG-INFO
+-rwxrwxrwx   0 root         (0) root         (0)     2918 2024-05-01 02:30:46.000000 PACMAN-charge-0.1.4/README.md
+-rwxrwxrwx   0 root         (0) root         (0)       38 2024-05-04 13:31:53.609896 PACMAN-charge-0.1.4/setup.cfg
+-rwxrwxrwx   0 root         (0) root         (0)     1038 2024-05-04 13:31:17.000000 PACMAN-charge-0.1.4/setup.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-04 13:31:53.591903 PACMAN-charge-0.1.4/test/
+-rwxrwxrwx   0 root         (0) root         (0)    34098 2024-05-04 13:30:14.000000 PACMAN-charge-0.1.4/test/Cu-BTC.cif
+-rwxrwxrwx   0 root         (0) root         (0)        0 2024-03-25 03:31:56.000000 PACMAN-charge-0.1.4/test/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)       76 2024-05-01 02:36:03.000000 PACMAN-charge-0.1.4/test/test.py
```

### Comparing `PACMAN-charge-0.1.3/LICENSE` & `PACMAN-charge-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `PACMAN-charge-0.1.3/PACMANCharge/atom_init.json` & `PACMAN-charge-0.1.4/PACMANCharge/atom_init.json`

 * *Files identical despite different names*

### Comparing `PACMAN-charge-0.1.3/PACMANCharge/pmcharge.py` & `PACMAN-charge-0.1.4/PACMANCharge/pmcharge.py`

 * *Files 0% similar despite different names*

```diff
@@ -395,15 +395,15 @@
     def __init__(self,orig_atom_fea_len,nbr_fea_len,atom_fea_len,n_conv,n_feature):    
         super(SemiFullGN, self).__init__()
         self.node_embedding = nn.Linear(orig_atom_fea_len,atom_fea_len)
         self.edge_embedding = nn.Linear(nbr_fea_len,atom_fea_len)
         self.convs = nn.ModuleList([ConvLayer(atom_fea_len=atom_fea_len,nbr_fea_len=atom_fea_len) for _ in range(n_conv)])
         self.feature_embedding = nn.Sequential(nn.Linear(n_feature,512))
         self.atom_nbr_fea_embedding = nn.Sequential(nn.Linear(2*atom_fea_len,128))
-        self.phi_pos = nn.Sequential(nn.Linear(512+128+128,512),
+        self.phi_pos = nn.Sequential(nn.Linear(512+128,512),
                                      nn.BatchNorm1d(512),
                                      nn.LeakyReLU(0.2))
         self.conv = nn.Sequential(nn.Conv1d(64,512,3,stride=1,padding=0),nn.BatchNorm1d(512),nn.LeakyReLU(0.2),
                                    nn.Conv1d(512,512,3,stride=1,padding=0),nn.BatchNorm1d(512),nn.LeakyReLU(0.2),
                                    nn.Conv1d(512,256,3,stride=1,padding=1),nn.LeakyReLU(0.2),
                                    nn.Conv1d(256,256,3,stride=1,padding=1),nn.LeakyReLU(0.2),
                                    nn.Conv1d(256,1,kernel_size=4,stride=1,padding=0))
```

### Comparing `PACMAN-charge-0.1.3/PACMAN_charge.egg-info/PKG-INFO` & `PACMAN-charge-0.1.4/PACMAN_charge.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PACMAN-charge
-Version: 0.1.3
+Version: 0.1.4
 Summary: Partial Atomic Charges for Porous Materials based on Graph Convolutional Neural Network (PACMAN)
 Home-page: https://github.com/sxm13/PACMAN
 Author: Guobin Zhao
 Author-email: sxmzhaogb@gmai.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `PACMAN-charge-0.1.3/PKG-INFO` & `PACMAN-charge-0.1.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PACMAN-charge
-Version: 0.1.3
+Version: 0.1.4
 Summary: Partial Atomic Charges for Porous Materials based on Graph Convolutional Neural Network (PACMAN)
 Home-page: https://github.com/sxm13/PACMAN
 Author: Guobin Zhao
 Author-email: sxmzhaogb@gmai.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `PACMAN-charge-0.1.3/README.md` & `PACMAN-charge-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `PACMAN-charge-0.1.3/setup.py` & `PACMAN-charge-0.1.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import requests
 from setuptools import setup, find_packages
 
 setup(
     name="PACMAN-charge",
-    version="0.1.3",
+    version="0.1.4",
     packages=find_packages(),
     description="Partial Atomic Charges for Porous Materials based on Graph Convolutional Neural Network (PACMAN)",
     author="Guobin Zhao",
     author_email="sxmzhaogb@gmai.com",
     url="https://github.com/sxm13/PACMAN",
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
```

### Comparing `PACMAN-charge-0.1.3/test/Cu-BTC.cif` & `PACMAN-charge-0.1.4/test/Cu-BTC.cif`

 * *Files identical despite different names*

