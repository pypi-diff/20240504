# Comparing `tmp/PACMAN-charge-0.1.4.tar.gz` & `tmp/PACMAN-charge-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PACMAN-charge-0.1.4.tar", last modified: Sat May  4 13:31:53 2024, max compression
+gzip compressed data, was "PACMAN-charge-0.1.5.tar", last modified: Sat May  4 13:44:52 2024, max compression
```

## Comparing `PACMAN-charge-0.1.4.tar` & `PACMAN-charge-0.1.5.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-04 13:31:53.607896 PACMAN-charge-0.1.4/
--rwxrwxrwx   0 root         (0) root         (0)     1068 2024-03-25 02:54:44.000000 PACMAN-charge-0.1.4/LICENSE
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-04 13:31:53.472907 PACMAN-charge-0.1.4/PACMANCharge/
--rwxrwxrwx   0 root         (0) root         (0)       33 2024-04-29 12:12:36.000000 PACMAN-charge-0.1.4/PACMANCharge/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)    28392 2024-01-10 01:22:23.000000 PACMAN-charge-0.1.4/PACMANCharge/atom_init.json
--rwxrwxrwx   0 root         (0) root         (0)    26396 2024-05-04 13:30:46.000000 PACMAN-charge-0.1.4/PACMANCharge/pmcharge.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-04 13:31:53.552896 PACMAN-charge-0.1.4/PACMAN_charge.egg-info/
--rwxrwxrwx   0 root         (0) root         (0)     3306 2024-05-04 13:31:53.000000 PACMAN-charge-0.1.4/PACMAN_charge.egg-info/PKG-INFO
--rwxrwxrwx   0 root         (0) root         (0)      334 2024-05-04 13:31:53.000000 PACMAN-charge-0.1.4/PACMAN_charge.egg-info/SOURCES.txt
--rwxrwxrwx   0 root         (0) root         (0)        1 2024-05-04 13:31:53.000000 PACMAN-charge-0.1.4/PACMAN_charge.egg-info/dependency_links.txt
--rwxrwxrwx   0 root         (0) root         (0)      121 2024-05-04 13:31:53.000000 PACMAN-charge-0.1.4/PACMAN_charge.egg-info/requires.txt
--rwxrwxrwx   0 root         (0) root         (0)       18 2024-05-04 13:31:53.000000 PACMAN-charge-0.1.4/PACMAN_charge.egg-info/top_level.txt
--rwxrwxrwx   0 root         (0) root         (0)     3306 2024-05-04 13:31:53.605897 PACMAN-charge-0.1.4/PKG-INFO
--rwxrwxrwx   0 root         (0) root         (0)     2918 2024-05-01 02:30:46.000000 PACMAN-charge-0.1.4/README.md
--rwxrwxrwx   0 root         (0) root         (0)       38 2024-05-04 13:31:53.609896 PACMAN-charge-0.1.4/setup.cfg
--rwxrwxrwx   0 root         (0) root         (0)     1038 2024-05-04 13:31:17.000000 PACMAN-charge-0.1.4/setup.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-04 13:31:53.591903 PACMAN-charge-0.1.4/test/
--rwxrwxrwx   0 root         (0) root         (0)    34098 2024-05-04 13:30:14.000000 PACMAN-charge-0.1.4/test/Cu-BTC.cif
--rwxrwxrwx   0 root         (0) root         (0)        0 2024-03-25 03:31:56.000000 PACMAN-charge-0.1.4/test/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)       76 2024-05-01 02:36:03.000000 PACMAN-charge-0.1.4/test/test.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-04 13:44:52.326818 PACMAN-charge-0.1.5/
+-rwxrwxrwx   0 root         (0) root         (0)     1068 2024-03-25 02:54:44.000000 PACMAN-charge-0.1.5/LICENSE
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-04 13:44:52.203024 PACMAN-charge-0.1.5/PACMANCharge/
+-rwxrwxrwx   0 root         (0) root         (0)       33 2024-04-29 12:12:36.000000 PACMAN-charge-0.1.5/PACMANCharge/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)    28392 2024-01-10 01:22:23.000000 PACMAN-charge-0.1.5/PACMANCharge/atom_init.json
+-rwxrwxrwx   0 root         (0) root         (0)    26468 2024-05-04 13:44:35.000000 PACMAN-charge-0.1.5/PACMANCharge/pmcharge.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-04 13:44:52.269025 PACMAN-charge-0.1.5/PACMAN_charge.egg-info/
+-rwxrwxrwx   0 root         (0) root         (0)     3306 2024-05-04 13:44:51.000000 PACMAN-charge-0.1.5/PACMAN_charge.egg-info/PKG-INFO
+-rwxrwxrwx   0 root         (0) root         (0)      334 2024-05-04 13:44:52.000000 PACMAN-charge-0.1.5/PACMAN_charge.egg-info/SOURCES.txt
+-rwxrwxrwx   0 root         (0) root         (0)        1 2024-05-04 13:44:52.000000 PACMAN-charge-0.1.5/PACMAN_charge.egg-info/dependency_links.txt
+-rwxrwxrwx   0 root         (0) root         (0)      121 2024-05-04 13:44:52.000000 PACMAN-charge-0.1.5/PACMAN_charge.egg-info/requires.txt
+-rwxrwxrwx   0 root         (0) root         (0)       18 2024-05-04 13:44:52.000000 PACMAN-charge-0.1.5/PACMAN_charge.egg-info/top_level.txt
+-rwxrwxrwx   0 root         (0) root         (0)     3306 2024-05-04 13:44:52.324819 PACMAN-charge-0.1.5/PKG-INFO
+-rwxrwxrwx   0 root         (0) root         (0)     2918 2024-05-01 02:30:46.000000 PACMAN-charge-0.1.5/README.md
+-rwxrwxrwx   0 root         (0) root         (0)       38 2024-05-04 13:44:52.326818 PACMAN-charge-0.1.5/setup.cfg
+-rwxrwxrwx   0 root         (0) root         (0)     1038 2024-05-04 13:44:39.000000 PACMAN-charge-0.1.5/setup.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-04 13:44:52.309025 PACMAN-charge-0.1.5/test/
+-rwxrwxrwx   0 root         (0) root         (0)    34098 2024-05-04 13:39:15.000000 PACMAN-charge-0.1.5/test/Cu-BTC.cif
+-rwxrwxrwx   0 root         (0) root         (0)        0 2024-03-25 03:31:56.000000 PACMAN-charge-0.1.5/test/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)       76 2024-05-01 02:36:03.000000 PACMAN-charge-0.1.5/test/test.py
```

### Comparing `PACMAN-charge-0.1.4/LICENSE` & `PACMAN-charge-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `PACMAN-charge-0.1.4/PACMANCharge/atom_init.json` & `PACMAN-charge-0.1.5/PACMANCharge/atom_init.json`

 * *Files identical despite different names*

### Comparing `PACMAN-charge-0.1.4/PACMANCharge/pmcharge.py` & `PACMAN-charge-0.1.5/PACMANCharge/pmcharge.py`

 * *Files 0% similar despite different names*

```diff
@@ -403,14 +403,15 @@
                                      nn.BatchNorm1d(512),
                                      nn.LeakyReLU(0.2))
         self.conv = nn.Sequential(nn.Conv1d(64,512,3,stride=1,padding=0),nn.BatchNorm1d(512),nn.LeakyReLU(0.2),
                                    nn.Conv1d(512,512,3,stride=1,padding=0),nn.BatchNorm1d(512),nn.LeakyReLU(0.2),
                                    nn.Conv1d(512,256,3,stride=1,padding=1),nn.LeakyReLU(0.2),
                                    nn.Conv1d(256,256,3,stride=1,padding=1),nn.LeakyReLU(0.2),
                                    nn.Conv1d(256,1,kernel_size=4,stride=1,padding=0))
+        self.cell_embedding = nn.Sequential(nn.Linear(9,128)) # remove
     def forward(self,atom_fea,nbr_fea,nbr_fea_idx1,nbr_fea_idx2,num_nbrs,atom_idx,structure_feature):
         nbr_fea_idx1 = nbr_fea_idx1.cuda() if torch.cuda.is_available() else nbr_fea_idx1
         nbr_fea_idx2 = nbr_fea_idx2.cuda() if torch.cuda.is_available() else nbr_fea_idx2
         num_nbrs = num_nbrs.cuda() if torch.cuda.is_available() else num_nbrs
         atom_idx = atom_idx.cuda() if torch.cuda.is_available() else atom_idx
         atom_fea = atom_fea.cuda() if torch.cuda.is_available() else atom_fea
         nbr_fea = nbr_fea.cuda() if torch.cuda.is_available() else nbr_fea
```

### Comparing `PACMAN-charge-0.1.4/PACMAN_charge.egg-info/PKG-INFO` & `PACMAN-charge-0.1.5/PACMAN_charge.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PACMAN-charge
-Version: 0.1.4
+Version: 0.1.5
 Summary: Partial Atomic Charges for Porous Materials based on Graph Convolutional Neural Network (PACMAN)
 Home-page: https://github.com/sxm13/PACMAN
 Author: Guobin Zhao
 Author-email: sxmzhaogb@gmai.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `PACMAN-charge-0.1.4/PKG-INFO` & `PACMAN-charge-0.1.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PACMAN-charge
-Version: 0.1.4
+Version: 0.1.5
 Summary: Partial Atomic Charges for Porous Materials based on Graph Convolutional Neural Network (PACMAN)
 Home-page: https://github.com/sxm13/PACMAN
 Author: Guobin Zhao
 Author-email: sxmzhaogb@gmai.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `PACMAN-charge-0.1.4/README.md` & `PACMAN-charge-0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `PACMAN-charge-0.1.4/setup.py` & `PACMAN-charge-0.1.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import requests
 from setuptools import setup, find_packages
 
 setup(
     name="PACMAN-charge",
-    version="0.1.4",
+    version="0.1.5",
     packages=find_packages(),
     description="Partial Atomic Charges for Porous Materials based on Graph Convolutional Neural Network (PACMAN)",
     author="Guobin Zhao",
     author_email="sxmzhaogb@gmai.com",
     url="https://github.com/sxm13/PACMAN",
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
```

### Comparing `PACMAN-charge-0.1.4/test/Cu-BTC.cif` & `PACMAN-charge-0.1.5/test/Cu-BTC.cif`

 * *Files identical despite different names*

