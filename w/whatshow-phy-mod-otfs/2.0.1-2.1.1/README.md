# Comparing `tmp/whatshow_phy_mod_otfs-2.0.1.tar.gz` & `tmp/whatshow_phy_mod_otfs-2.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "whatshow_phy_mod_otfs-2.0.1.tar", last modified: Sat Apr 27 11:29:47 2024, max compression
+gzip compressed data, was "whatshow_phy_mod_otfs-2.1.1.tar", last modified: Sat May  4 06:55:03 2024, max compression
```

## Comparing `whatshow_phy_mod_otfs-2.0.1.tar` & `whatshow_phy_mod_otfs-2.1.1.tar`

### file list

```diff
@@ -1,15 +1,16 @@
-drwxrwxrwx   0        0        0        0 2024-04-27 11:29:47.860392 whatshow_phy_mod_otfs-2.0.1/
--rw-rw-rw-   0        0        0    12548 2024-04-27 11:29:47.858391 whatshow_phy_mod_otfs-2.0.1/PKG-INFO
--rw-rw-rw-   0        0        0    12432 2024-04-27 11:29:47.000000 whatshow_phy_mod_otfs-2.0.1/README.md
--rw-rw-rw-   0        0        0       42 2024-04-27 11:29:47.860392 whatshow_phy_mod_otfs-2.0.1/setup.cfg
--rw-rw-rw-   0        0        0      408 2024-04-27 11:29:47.000000 whatshow_phy_mod_otfs-2.0.1/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-27 11:29:47.833670 whatshow_phy_mod_otfs-2.0.1/whatshow_phy_mod_otfs/
--rw-rw-rw-   0        0        0    19980 2024-04-27 11:29:47.000000 whatshow_phy_mod_otfs-2.0.1/whatshow_phy_mod_otfs/OTFS.py
--rw-rw-rw-   0        0        0    27830 2024-04-27 11:29:47.000000 whatshow_phy_mod_otfs-2.0.1/whatshow_phy_mod_otfs/OTFSResGrid.py
--rw-rw-rw-   0        0        0      100 2024-04-27 11:29:47.000000 whatshow_phy_mod_otfs-2.0.1/whatshow_phy_mod_otfs/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-27 11:29:47.856212 whatshow_phy_mod_otfs-2.0.1/whatshow_phy_mod_otfs.egg-info/
--rw-rw-rw-   0        0        0    12548 2024-04-27 11:29:47.000000 whatshow_phy_mod_otfs-2.0.1/whatshow_phy_mod_otfs.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      343 2024-04-27 11:29:47.000000 whatshow_phy_mod_otfs-2.0.1/whatshow_phy_mod_otfs.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-27 11:29:47.000000 whatshow_phy_mod_otfs-2.0.1/whatshow_phy_mod_otfs.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       14 2024-04-27 11:29:47.000000 whatshow_phy_mod_otfs-2.0.1/whatshow_phy_mod_otfs.egg-info/requires.txt
--rw-rw-rw-   0        0        0       22 2024-04-27 11:29:47.000000 whatshow_phy_mod_otfs-2.0.1/whatshow_phy_mod_otfs.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-04 06:55:03.186038 whatshow_phy_mod_otfs-2.1.1/
+-rw-rw-rw-   0        0        0    13032 2024-05-04 06:55:03.183699 whatshow_phy_mod_otfs-2.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0    12916 2024-05-04 06:54:49.000000 whatshow_phy_mod_otfs-2.1.1/README.md
+-rw-rw-rw-   0        0        0       42 2024-05-04 06:55:03.186038 whatshow_phy_mod_otfs-2.1.1/setup.cfg
+-rw-rw-rw-   0        0        0      408 2024-05-04 06:54:49.000000 whatshow_phy_mod_otfs-2.1.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-04 06:55:03.161924 whatshow_phy_mod_otfs-2.1.1/whatshow_phy_mod_otfs/
+-rw-rw-rw-   0        0        0    26618 2024-05-04 06:54:49.000000 whatshow_phy_mod_otfs-2.1.1/whatshow_phy_mod_otfs/OTFS.py
+-rw-rw-rw-   0        0        0    15905 2024-05-04 06:54:49.000000 whatshow_phy_mod_otfs-2.1.1/whatshow_phy_mod_otfs/OTFSDetector.py
+-rw-rw-rw-   0        0        0    27873 2024-05-04 06:54:49.000000 whatshow_phy_mod_otfs-2.1.1/whatshow_phy_mod_otfs/OTFSResGrid.py
+-rw-rw-rw-   0        0        0      100 2024-05-04 06:54:49.000000 whatshow_phy_mod_otfs-2.1.1/whatshow_phy_mod_otfs/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-04 06:55:03.180700 whatshow_phy_mod_otfs-2.1.1/whatshow_phy_mod_otfs.egg-info/
+-rw-rw-rw-   0        0        0    13032 2024-05-04 06:55:02.000000 whatshow_phy_mod_otfs-2.1.1/whatshow_phy_mod_otfs.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      381 2024-05-04 06:55:02.000000 whatshow_phy_mod_otfs-2.1.1/whatshow_phy_mod_otfs.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-04 06:55:02.000000 whatshow_phy_mod_otfs-2.1.1/whatshow_phy_mod_otfs.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       14 2024-05-04 06:55:02.000000 whatshow_phy_mod_otfs-2.1.1/whatshow_phy_mod_otfs.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       22 2024-05-04 06:55:02.000000 whatshow_phy_mod_otfs-2.1.1/whatshow_phy_mod_otfs.egg-info/top_level.txt
```

### Comparing `whatshow_phy_mod_otfs-2.0.1/PKG-INFO` & `whatshow_phy_mod_otfs-2.1.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: whatshow_phy_mod_otfs
-Version: 2.0.1
+Version: 2.1.1
 Description-Content-Type: text/markdown
 
 # OTFS Modulation
-[![PyPi](https://img.shields.io/badge/PyPi-2.0.1-blue)](https://pypi.org/project/whatshow-phy-mod-otfs/) [![MathWorks](https://img.shields.io/badge/MathWorks-2.0.1-red)](https://mathworks.com/matlabcentral/fileexchange/161136-whatshow_phy_mod_otfs)
+[![PyPi](https://img.shields.io/badge/PyPi-2.1.1-blue)](https://pypi.org/project/whatshow-phy-mod-otfs/) [![MathWorks](https://img.shields.io/badge/MathWorks-2.1.1-red)](https://mathworks.com/matlabcentral/fileexchange/161136-whatshow_phy_mod_otfs)
 
 This repository is a fundamental toolbox of OTFS modulation crossing `matlab` and `python`. This repositiory is based on papers below:
 > Raviteja, P., Phan, K. T., Hong, Y., & Viterbo, E. (2018). Interference cancellation and iterative detection for orthogonal time frequency space modulation. *IEEE transactions on wireless communications, 17(10)*, 6501-6515.
 
 > Raviteja, P., Phan, K. T., & Hong, Y. (2019). Embedded pilot-aided channel estimation for OTFS in delayâ€“Doppler channels. *IEEE transactions on vehicular technology, 68(5)*, 4906-4917.
 
 ## How to use
@@ -61,26 +61,26 @@
         rg.setGuard(guard_delay_num_neg, guard_delay_num_pos, 'guard_doppl_full', true);
         rg.setGuard(guard_delay_num_neg, guard_delay_num_pos, guard_doppl_full=True);
         ```
     * map(): `symbols` is mandatory, `pilots_pow` and `pilots_pow` must use one if you want to use pilots. Other parameters define the length of pilots and the guards area around the pilots. If the guard area is oversize, you are suggested to use full guard on that axis so that the channel estimation result will be more accurate.<br>
         `@symbols`: OTFS symbols<br>
         `@pilots(opt)`: a vector of your pilots (if given `pilots_pow` won't be used)<br>
         `@pilots_pow(opt)`: pilot power to generate random pilots
-    * setAreaCE(): set the channel estimation area manually. **You should only call this function when you disagree with our channel estimation area.**
+    * setAreaCE(): set the channel estimation area manually. **You should only call this function when you disagree with our channel estimation area.**<br>
         `@ce_l_beg`: CE delay beginning<br>
         `@ce_l_end`: CE delay ending<br>
         `@ce_k_beg`: CE Doppler beginning<br>
         `@ce_k_end`: CE Doppler ending<br>
     * demap()<br>
         `@isData(opt)`: whether give the data (true by default)<br>
         `@isCE(opt)`: whether give the channel estimation result(true by default)<br>
         `@threshold(opt)`: the threshold to estimate the channel
         ```c, matlab, python
         [y, his_est, lis_est, kis_est] = rg_rx.demap("threshold", 1e-10);
-        y, his_est, lis_est, kis_est = rg_rx.demap("threshold", 1e-10);
+        y, his_est, lis_est, kis_est = rg_rx.demap(threshold=1e-10);
         ```
     * clone(): clone this resource grid
     * isZP(): return zero padding length
     * isPG(): check whether use pilots & guards
     * Check whether your coordinate is in a certain area<br>
         `@pos_doppl`: the position on the Doppler axis. Not given means the position is for a Doppler-delay vector <br>
         `@pos_delay`: the position on the delay axis for matrix or th position on the Doppler-delay axis for the vector
@@ -132,18 +132,23 @@
         rg.getContent(isVector=True);
         ```
     * getContentCE(): get the channel estimation area content (return a matrix)
     * getContentNoCE(): get the content except CE area (return a vector)
     * getContentZeroPG(): get the content of zero PG area (return a vector)
     * getContentZeroCE(): get the content of zero CE area (return a vector)
 * OTFS: this class provides the entire process of OTFS from Tx to Rx
-    * OTFS()
+    * OTFS()<br>
         `@batch_size(opt)`: the batch size (only used in python)
+    * Pulse settings: if you want to input delay-Doppler domain matrix directly into `OTFS`, you need to set the pulse type before `modulate`.
+        ```c, matlab, python
+        otfs.setPulse2Ideal();  // use ideal pulses
+        otfs.setPulse2Recta();  // use rectangular pulses
+        ```
     * modulate():modulate (use fast method by default)<br>
-        `@rg`: an OTFS resource grid<br>
+        `@in1`: an OTFS resource grid or a 2D matrix [(batch_size), Doppler, delay]<br>
         `@isFast(opt)`: DD domain -> TD domain (no X_TF)
         ```c, matlab, python
         // fast modulate
         otfs.modulate(rg);
         // slow modulate
         otfs.modulate(rg, "isFast", false);
         otfs.modulate(rg, isFast=False);
@@ -178,15 +183,16 @@
         `@No`: linear noise power (a scalar) or a given noise vector
         ```c, matlab, python
         otfs.passChannel(No);
         ```
     * demodulate(): demodulate (use fast method by default)<br>
         `@isFast(opt)`: TD domain -> DD domain (no Y_TF) 
         ```c, matlab, python
-        rg = otfs.demodulate();
+        rg = otfs.demodulate(); // if the modulation uses a resource grid
+        Y_DD = otfs.demodulate(); // if the modulation uses a delay-Doppler domain matrix
         ```
     * getChannel(): return the channel on delay Doppler domain. If not given `his`, `lis`, `kis`, use the current channel.<br>
         `@his`: the channel gains<br>
         `@lis`: the channel delays<br>
         `@kis`: the channel Dopplers<br>
         `@data_only(opt)`: whether the channel is only for data (by default true). If you want to get the entire H_DD when using pilos and/or guards, you should manullay set it to false.
         ```c, matlab, python
```

### Comparing `whatshow_phy_mod_otfs-2.0.1/README.md` & `whatshow_phy_mod_otfs-2.1.1/whatshow_phy_mod_otfs.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,19 @@
+Metadata-Version: 2.1
+Name: whatshow-phy-mod-otfs
+Version: 2.1.1
+Description-Content-Type: text/markdown
+
 # OTFS Modulation
-[![PyPi](https://img.shields.io/badge/PyPi-2.0.1-blue)](https://pypi.org/project/whatshow-phy-mod-otfs/) [![MathWorks](https://img.shields.io/badge/MathWorks-2.0.1-red)](https://mathworks.com/matlabcentral/fileexchange/161136-whatshow_phy_mod_otfs)
+[![PyPi](https://img.shields.io/badge/PyPi-2.1.1-blue)](https://pypi.org/project/whatshow-phy-mod-otfs/) [![MathWorks](https://img.shields.io/badge/MathWorks-2.1.1-red)](https://mathworks.com/matlabcentral/fileexchange/161136-whatshow_phy_mod_otfs)
 
 This repository is a fundamental toolbox of OTFS modulation crossing `matlab` and `python`. This repositiory is based on papers below:
 > Raviteja, P., Phan, K. T., Hong, Y., & Viterbo, E. (2018). Interference cancellation and iterative detection for orthogonal time frequency space modulation. *IEEE transactions on wireless communications, 17(10)*, 6501-6515.
 
-> Raviteja, P., Phan, K. T., & Hong, Y. (2019). Embedded pilot-aided channel estimation for OTFS in delay–Doppler channels. *IEEE transactions on vehicular technology, 68(5)*, 4906-4917.
+> Raviteja, P., Phan, K. T., & Hong, Y. (2019). Embedded pilot-aided channel estimation for OTFS in delayâ€“Doppler channels. *IEEE transactions on vehicular technology, 68(5)*, 4906-4917.
 
 ## How to use
 All codes are uniform in matlab and python in three class.
 ![system_model](https://github.com/whatshow/Phy_Mod_OTFS/blob/main/Img/system_model.jpg)
 * OTFSResGrid: this class provides the resource grid
     * OTFSResGrid()<br>
         `@in1`: 1st input, a scalar for subcarrier number or the content directly<br>
@@ -56,26 +61,26 @@
         rg.setGuard(guard_delay_num_neg, guard_delay_num_pos, 'guard_doppl_full', true);
         rg.setGuard(guard_delay_num_neg, guard_delay_num_pos, guard_doppl_full=True);
         ```
     * map(): `symbols` is mandatory, `pilots_pow` and `pilots_pow` must use one if you want to use pilots. Other parameters define the length of pilots and the guards area around the pilots. If the guard area is oversize, you are suggested to use full guard on that axis so that the channel estimation result will be more accurate.<br>
         `@symbols`: OTFS symbols<br>
         `@pilots(opt)`: a vector of your pilots (if given `pilots_pow` won't be used)<br>
         `@pilots_pow(opt)`: pilot power to generate random pilots
-    * setAreaCE(): set the channel estimation area manually. **You should only call this function when you disagree with our channel estimation area.**
+    * setAreaCE(): set the channel estimation area manually. **You should only call this function when you disagree with our channel estimation area.**<br>
         `@ce_l_beg`: CE delay beginning<br>
         `@ce_l_end`: CE delay ending<br>
         `@ce_k_beg`: CE Doppler beginning<br>
         `@ce_k_end`: CE Doppler ending<br>
     * demap()<br>
         `@isData(opt)`: whether give the data (true by default)<br>
         `@isCE(opt)`: whether give the channel estimation result(true by default)<br>
         `@threshold(opt)`: the threshold to estimate the channel
         ```c, matlab, python
         [y, his_est, lis_est, kis_est] = rg_rx.demap("threshold", 1e-10);
-        y, his_est, lis_est, kis_est = rg_rx.demap("threshold", 1e-10);
+        y, his_est, lis_est, kis_est = rg_rx.demap(threshold=1e-10);
         ```
     * clone(): clone this resource grid
     * isZP(): return zero padding length
     * isPG(): check whether use pilots & guards
     * Check whether your coordinate is in a certain area<br>
         `@pos_doppl`: the position on the Doppler axis. Not given means the position is for a Doppler-delay vector <br>
         `@pos_delay`: the position on the delay axis for matrix or th position on the Doppler-delay axis for the vector
@@ -127,18 +132,23 @@
         rg.getContent(isVector=True);
         ```
     * getContentCE(): get the channel estimation area content (return a matrix)
     * getContentNoCE(): get the content except CE area (return a vector)
     * getContentZeroPG(): get the content of zero PG area (return a vector)
     * getContentZeroCE(): get the content of zero CE area (return a vector)
 * OTFS: this class provides the entire process of OTFS from Tx to Rx
-    * OTFS()
+    * OTFS()<br>
         `@batch_size(opt)`: the batch size (only used in python)
+    * Pulse settings: if you want to input delay-Doppler domain matrix directly into `OTFS`, you need to set the pulse type before `modulate`.
+        ```c, matlab, python
+        otfs.setPulse2Ideal();  // use ideal pulses
+        otfs.setPulse2Recta();  // use rectangular pulses
+        ```
     * modulate():modulate (use fast method by default)<br>
-        `@rg`: an OTFS resource grid<br>
+        `@in1`: an OTFS resource grid or a 2D matrix [(batch_size), Doppler, delay]<br>
         `@isFast(opt)`: DD domain -> TD domain (no X_TF)
         ```c, matlab, python
         // fast modulate
         otfs.modulate(rg);
         // slow modulate
         otfs.modulate(rg, "isFast", false);
         otfs.modulate(rg, isFast=False);
@@ -173,15 +183,16 @@
         `@No`: linear noise power (a scalar) or a given noise vector
         ```c, matlab, python
         otfs.passChannel(No);
         ```
     * demodulate(): demodulate (use fast method by default)<br>
         `@isFast(opt)`: TD domain -> DD domain (no Y_TF) 
         ```c, matlab, python
-        rg = otfs.demodulate();
+        rg = otfs.demodulate(); // if the modulation uses a resource grid
+        Y_DD = otfs.demodulate(); // if the modulation uses a delay-Doppler domain matrix
         ```
     * getChannel(): return the channel on delay Doppler domain. If not given `his`, `lis`, `kis`, use the current channel.<br>
         `@his`: the channel gains<br>
         `@lis`: the channel delays<br>
         `@kis`: the channel Dopplers<br>
         `@data_only(opt)`: whether the channel is only for data (by default true). If you want to get the entire H_DD when using pilos and/or guards, you should manullay set it to false.
         ```c, matlab, python
```

### Comparing `whatshow_phy_mod_otfs-2.0.1/whatshow_phy_mod_otfs/OTFSResGrid.py` & `whatshow_phy_mod_otfs-2.1.1/whatshow_phy_mod_otfs/OTFSResGrid.py`

 * *Files 1% similar despite different names*

```diff
@@ -345,16 +345,15 @@
     '''
     get content
     @isVector: if true, the returned result is a vector
     '''
     def getContent(self, *, isVector=False):
         # return
         if isVector:
-            content = self.content.copy();
-            content = self.reshape(content, self.nSubcarNum*self.nTimeslotNum);
+            content = self.reshape(self.content, self.nSubcarNum*self.nTimeslotNum);
         else:
             content = self.content;
         return content;
 
     '''
     get content - CE (return a matrix)
     '''
@@ -440,25 +439,24 @@
             if self.pl1 + self.pl_len - 1 >= self.nSubcarNum:
                 raise Exception("Pilot length on the Doppler axis overflows.");
     
     '''
     calculate PG & CE area
     '''
     def calcAreaPGCE(self):
-        # overflow check
-        if self.pl1 - self.gl_len_neg < 0:
-            raise Exception("The guard (neg) on delay axis overflows.");
-        if (self.pl1+self.pl_len-1) + self.gl_len_pos >= self.nSubcarNum:
-            raise Exception("The guard (pos) on delay axis overflows.");
-        if self.pk1 - self.gk_len_neg < 0:
-            raise Exception("The guard (neg) on Doppler axis overflows.");
-        if (self.pk1+self.pk_len-1) + self.gk_len_pos >= self.nTimeslotNum:
-            raise Exception("The guard (pos) on Doppler axis overflows.");
-        # calculate area
         if self.pl_len > 0 and self.pk_len > 0:
+            # overflow check
+            if self.pl1 - self.gl_len_neg < 0:
+                raise Exception("The guard (neg) on delay axis overflows.");
+            if (self.pl1+self.pl_len-1) + self.gl_len_pos >= self.nSubcarNum:
+                raise Exception("The guard (pos) on delay axis overflows.");
+            if self.pk1 - self.gk_len_neg < 0:
+                raise Exception("The guard (neg) on Doppler axis overflows.");
+            if (self.pk1+self.pk_len-1) + self.gk_len_pos >= self.nTimeslotNum:
+                raise Exception("The guard (pos) on Doppler axis overflows.");
             # calculate PG area
             if self.pilot_type == self.PILOT_TYPE_EM:
                 # PG area only exist when using embedded pilots
                 self.pg_num = ((self.pl_len+self.gl_len_neg+self.gl_len_pos)*(self.pk_len+self.gk_len_neg+self.gk_len_pos)).astype(int);
                 self.pg_delay_beg = (self.pl1 - self.gl_len_neg).astype(int);
                 self.pg_delay_end = (self.pl1 + self.pl_len - 1 + self.gl_len_pos).astype(int);
                 self.pg_doppl_beg = (self.pk1 - self.gk_len_neg).astype(int);
@@ -521,20 +519,21 @@
         # input check - pilots
         if self.p_len > 0:
             if self.p_len != self.pl_len*self.pk_len:
                 raise Exception("The manual pilot input do not have the required number.");
             elif self.p_len > self.nTimeslotNum*self.nSubcarNum:
                 raise Exception("The manual pilot input overflows (over the OTFS frame size).");
         # input check - pilot power
-        if self.p_len == 0 and pilots_pow == None:
+        if self.p_len == 0 and pilots_pow == None and self.pk_len>0 and self.pl_len>0:
             raise Exception("The pilots (linear) power is required while no manual pilot input.");
         # initiate pilots if empty
         if self.p_len == 0:
             self.p_len = self.pl_len*self.pk_len;
-            self.pilots = sqrt(pilots_pow/2)*(1+1j)*np.ones(self.p_len);
+            if self.p_len > 0:
+                self.pilots = sqrt(pilots_pow/2)*(1+1j)*np.ones(self.p_len);
         # allocate pilots
         if self.p_len != 0:
             # allocate pilots
             if self.batch_size == self.BATCH_SIZE_NO:
                 self.content[self.pk1:self.pk1+self.pk_len, self.pl1:self.pl1+self.pl_len] = self.content[self.pk1:self.pk1+self.pk_len, self.pl1:self.pl1+self.pl_len] + self.reshape(self.pilots, self.pk_len, self.pl_len);
             else:
                 pilots = np.tile(np.reshape(self.pilots, (self.pk_len, self.pl_len)), (self.batch_size, 1, 1));
```

### Comparing `whatshow_phy_mod_otfs-2.0.1/whatshow_phy_mod_otfs.egg-info/PKG-INFO` & `whatshow_phy_mod_otfs-2.1.1/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,19 +1,14 @@
-Metadata-Version: 2.1
-Name: whatshow-phy-mod-otfs
-Version: 2.0.1
-Description-Content-Type: text/markdown
-
 # OTFS Modulation
-[![PyPi](https://img.shields.io/badge/PyPi-2.0.1-blue)](https://pypi.org/project/whatshow-phy-mod-otfs/) [![MathWorks](https://img.shields.io/badge/MathWorks-2.0.1-red)](https://mathworks.com/matlabcentral/fileexchange/161136-whatshow_phy_mod_otfs)
+[![PyPi](https://img.shields.io/badge/PyPi-2.1.1-blue)](https://pypi.org/project/whatshow-phy-mod-otfs/) [![MathWorks](https://img.shields.io/badge/MathWorks-2.1.1-red)](https://mathworks.com/matlabcentral/fileexchange/161136-whatshow_phy_mod_otfs)
 
 This repository is a fundamental toolbox of OTFS modulation crossing `matlab` and `python`. This repositiory is based on papers below:
 > Raviteja, P., Phan, K. T., Hong, Y., & Viterbo, E. (2018). Interference cancellation and iterative detection for orthogonal time frequency space modulation. *IEEE transactions on wireless communications, 17(10)*, 6501-6515.
 
-> Raviteja, P., Phan, K. T., & Hong, Y. (2019). Embedded pilot-aided channel estimation for OTFS in delayâ€“Doppler channels. *IEEE transactions on vehicular technology, 68(5)*, 4906-4917.
+> Raviteja, P., Phan, K. T., & Hong, Y. (2019). Embedded pilot-aided channel estimation for OTFS in delay–Doppler channels. *IEEE transactions on vehicular technology, 68(5)*, 4906-4917.
 
 ## How to use
 All codes are uniform in matlab and python in three class.
 ![system_model](https://github.com/whatshow/Phy_Mod_OTFS/blob/main/Img/system_model.jpg)
 * OTFSResGrid: this class provides the resource grid
     * OTFSResGrid()<br>
         `@in1`: 1st input, a scalar for subcarrier number or the content directly<br>
@@ -61,26 +56,26 @@
         rg.setGuard(guard_delay_num_neg, guard_delay_num_pos, 'guard_doppl_full', true);
         rg.setGuard(guard_delay_num_neg, guard_delay_num_pos, guard_doppl_full=True);
         ```
     * map(): `symbols` is mandatory, `pilots_pow` and `pilots_pow` must use one if you want to use pilots. Other parameters define the length of pilots and the guards area around the pilots. If the guard area is oversize, you are suggested to use full guard on that axis so that the channel estimation result will be more accurate.<br>
         `@symbols`: OTFS symbols<br>
         `@pilots(opt)`: a vector of your pilots (if given `pilots_pow` won't be used)<br>
         `@pilots_pow(opt)`: pilot power to generate random pilots
-    * setAreaCE(): set the channel estimation area manually. **You should only call this function when you disagree with our channel estimation area.**
+    * setAreaCE(): set the channel estimation area manually. **You should only call this function when you disagree with our channel estimation area.**<br>
         `@ce_l_beg`: CE delay beginning<br>
         `@ce_l_end`: CE delay ending<br>
         `@ce_k_beg`: CE Doppler beginning<br>
         `@ce_k_end`: CE Doppler ending<br>
     * demap()<br>
         `@isData(opt)`: whether give the data (true by default)<br>
         `@isCE(opt)`: whether give the channel estimation result(true by default)<br>
         `@threshold(opt)`: the threshold to estimate the channel
         ```c, matlab, python
         [y, his_est, lis_est, kis_est] = rg_rx.demap("threshold", 1e-10);
-        y, his_est, lis_est, kis_est = rg_rx.demap("threshold", 1e-10);
+        y, his_est, lis_est, kis_est = rg_rx.demap(threshold=1e-10);
         ```
     * clone(): clone this resource grid
     * isZP(): return zero padding length
     * isPG(): check whether use pilots & guards
     * Check whether your coordinate is in a certain area<br>
         `@pos_doppl`: the position on the Doppler axis. Not given means the position is for a Doppler-delay vector <br>
         `@pos_delay`: the position on the delay axis for matrix or th position on the Doppler-delay axis for the vector
@@ -132,18 +127,23 @@
         rg.getContent(isVector=True);
         ```
     * getContentCE(): get the channel estimation area content (return a matrix)
     * getContentNoCE(): get the content except CE area (return a vector)
     * getContentZeroPG(): get the content of zero PG area (return a vector)
     * getContentZeroCE(): get the content of zero CE area (return a vector)
 * OTFS: this class provides the entire process of OTFS from Tx to Rx
-    * OTFS()
+    * OTFS()<br>
         `@batch_size(opt)`: the batch size (only used in python)
+    * Pulse settings: if you want to input delay-Doppler domain matrix directly into `OTFS`, you need to set the pulse type before `modulate`.
+        ```c, matlab, python
+        otfs.setPulse2Ideal();  // use ideal pulses
+        otfs.setPulse2Recta();  // use rectangular pulses
+        ```
     * modulate():modulate (use fast method by default)<br>
-        `@rg`: an OTFS resource grid<br>
+        `@in1`: an OTFS resource grid or a 2D matrix [(batch_size), Doppler, delay]<br>
         `@isFast(opt)`: DD domain -> TD domain (no X_TF)
         ```c, matlab, python
         // fast modulate
         otfs.modulate(rg);
         // slow modulate
         otfs.modulate(rg, "isFast", false);
         otfs.modulate(rg, isFast=False);
@@ -178,15 +178,16 @@
         `@No`: linear noise power (a scalar) or a given noise vector
         ```c, matlab, python
         otfs.passChannel(No);
         ```
     * demodulate(): demodulate (use fast method by default)<br>
         `@isFast(opt)`: TD domain -> DD domain (no Y_TF) 
         ```c, matlab, python
-        rg = otfs.demodulate();
+        rg = otfs.demodulate(); // if the modulation uses a resource grid
+        Y_DD = otfs.demodulate(); // if the modulation uses a delay-Doppler domain matrix
         ```
     * getChannel(): return the channel on delay Doppler domain. If not given `his`, `lis`, `kis`, use the current channel.<br>
         `@his`: the channel gains<br>
         `@lis`: the channel delays<br>
         `@kis`: the channel Dopplers<br>
         `@data_only(opt)`: whether the channel is only for data (by default true). If you want to get the entire H_DD when using pilos and/or guards, you should manullay set it to false.
         ```c, matlab, python
```

