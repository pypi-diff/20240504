# Comparing `tmp/salabim-24.0.4.post0.tar.gz` & `tmp/salabim-24.0.4.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "salabim-24.0.4.post0.tar", last modified: Fri May  3 10:15:10 2024, max compression
+gzip compressed data, was "salabim-24.0.4.post1.tar", last modified: Sat May  4 15:13:54 2024, max compression
```

## Comparing `salabim-24.0.4.post0.tar` & `salabim-24.0.4.post1.tar`

### file list

```diff
@@ -1,30 +1,31 @@
-drwxrwxrwx   0        0        0        0 2024-05-03 10:15:10.164181 salabim-24.0.4.post0/
--rw-rw-rw-   0        0        0     3036 2024-05-03 10:15:10.163172 salabim-24.0.4.post0/PKG-INFO
--rw-rw-rw-   0        0        0     2522 2024-04-28 16:58:56.000000 salabim-24.0.4.post0/README.md
--rw-rw-rw-   0        0        0      725 2024-05-03 10:15:03.000000 salabim-24.0.4.post0/pyproject.toml
-drwxrwxrwx   0        0        0        0 2024-05-03 10:15:10.140132 salabim-24.0.4.post0/salabim/
--rw-rw-rw-   0        0        0   335068 2018-11-08 08:44:44.000000 salabim-24.0.4.post0/salabim/DejaVuSansMono.ttf
--rw-rw-rw-   0        0        0     1105 2024-03-23 13:29:56.000000 salabim-24.0.4.post0/salabim/LICENSE.txt
--rw-rw-rw-   0        0        0  1330156 2023-05-08 05:21:17.000000 salabim-24.0.4.post0/salabim/calibri.ttf
--rw-rw-rw-   0        0        0   294610 2024-05-03 10:11:43.000000 salabim-24.0.4.post0/salabim/changelog.txt
--rw-rw-rw-   0        0        0   289812 2018-11-08 08:44:33.000000 salabim-24.0.4.post0/salabim/mplus-1m-regular.ttf
--rw-rw-rw-   0        0        0  1093613 2024-05-02 14:11:57.000000 salabim-24.0.4.post0/salabim/salabim.py
-drwxrwxrwx   0        0        0        0 2024-05-03 10:15:10.161666 salabim-24.0.4.post0/salabim.egg-info/
--rw-rw-rw-   0        0        0     3036 2024-05-03 10:15:10.000000 salabim-24.0.4.post0/salabim.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      559 2024-05-03 10:15:10.000000 salabim-24.0.4.post0/salabim.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-03 10:15:10.000000 salabim-24.0.4.post0/salabim.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2024-05-03 10:15:10.000000 salabim-24.0.4.post0/salabim.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-03 10:15:10.164181 salabim-24.0.4.post0/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-05-03 10:15:10.160666 salabim-24.0.4.post0/tests/
--rw-rw-rw-   0        0        0      677 2023-10-05 13:11:47.000000 salabim-24.0.4.post0/tests/test_cap_now.py
--rw-rw-rw-   0        0        0     6228 2023-05-14 06:16:09.000000 salabim-24.0.4.post0/tests/test_componentgenerator.py
--rw-rw-rw-   0        0        0     2993 2023-08-16 15:40:02.000000 salabim-24.0.4.post0/tests/test_datetime.py
--rw-rw-rw-   0        0        0     6295 2023-03-08 18:04:01.000000 salabim-24.0.4.post0/tests/test_distributions.py
--rw-rw-rw-   0        0        0     1693 2023-07-02 09:23:01.000000 salabim-24.0.4.post0/tests/test_misc.py
--rw-rw-rw-   0        0        0    21231 2023-10-05 13:15:36.000000 salabim-24.0.4.post0/tests/test_monitor.py
--rw-rw-rw-   0        0        0      654 2020-10-22 20:12:03.000000 salabim-24.0.4.post0/tests/test_process.py
--rw-rw-rw-   0        0        0     5060 2021-11-17 08:19:40.000000 salabim-24.0.4.post0/tests/test_queue.py
--rw-rw-rw-   0        0        0       74 2023-07-02 10:54:17.000000 salabim-24.0.4.post0/tests/test_salabim.py
--rw-rw-rw-   0        0        0     2677 2023-08-14 09:14:44.000000 salabim-24.0.4.post0/tests/test_state.py
--rw-rw-rw-   0        0        0      344 2023-11-29 17:46:13.000000 salabim-24.0.4.post0/tests/test_store.py
--rw-rw-rw-   0        0        0     4517 2022-04-30 07:30:12.000000 salabim-24.0.4.post0/tests/test_timeunit.py
+drwxrwxrwx   0        0        0        0 2024-05-04 15:13:54.221619 salabim-24.0.4.post1/
+-rw-rw-rw-   0        0        0     3036 2024-05-04 15:13:54.221619 salabim-24.0.4.post1/PKG-INFO
+-rw-rw-rw-   0        0        0     2522 2024-04-28 16:58:56.000000 salabim-24.0.4.post1/README.md
+-rw-rw-rw-   0        0        0      725 2024-05-04 15:13:47.000000 salabim-24.0.4.post1/pyproject.toml
+drwxrwxrwx   0        0        0        0 2024-05-04 15:13:54.188221 salabim-24.0.4.post1/salabim/
+-rw-rw-rw-   0        0        0   335068 2018-11-08 08:44:44.000000 salabim-24.0.4.post1/salabim/DejaVuSansMono.ttf
+-rw-rw-rw-   0        0        0     1105 2024-03-23 13:29:56.000000 salabim-24.0.4.post1/salabim/LICENSE.txt
+-rw-rw-rw-   0        0        0       56 2024-05-04 15:12:34.000000 salabim-24.0.4.post1/salabim/__init__.py
+-rw-rw-rw-   0        0        0  1330156 2023-05-08 05:21:17.000000 salabim-24.0.4.post1/salabim/calibri.ttf
+-rw-rw-rw-   0        0        0   294610 2024-05-04 09:33:01.000000 salabim-24.0.4.post1/salabim/changelog.txt
+-rw-rw-rw-   0        0        0   289812 2018-11-08 08:44:33.000000 salabim-24.0.4.post1/salabim/mplus-1m-regular.ttf
+-rw-rw-rw-   0        0        0  1093659 2024-05-03 14:07:01.000000 salabim-24.0.4.post1/salabim/salabim.py
+drwxrwxrwx   0        0        0        0 2024-05-04 15:13:54.220893 salabim-24.0.4.post1/salabim.egg-info/
+-rw-rw-rw-   0        0        0     3036 2024-05-04 15:13:54.000000 salabim-24.0.4.post1/salabim.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      579 2024-05-04 15:13:54.000000 salabim-24.0.4.post1/salabim.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-04 15:13:54.000000 salabim-24.0.4.post1/salabim.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2024-05-04 15:13:54.000000 salabim-24.0.4.post1/salabim.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-04 15:13:54.221619 salabim-24.0.4.post1/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-05-04 15:13:54.219205 salabim-24.0.4.post1/tests/
+-rw-rw-rw-   0        0        0      677 2023-10-05 13:11:47.000000 salabim-24.0.4.post1/tests/test_cap_now.py
+-rw-rw-rw-   0        0        0     6228 2023-05-14 06:16:09.000000 salabim-24.0.4.post1/tests/test_componentgenerator.py
+-rw-rw-rw-   0        0        0     2993 2023-08-16 15:40:02.000000 salabim-24.0.4.post1/tests/test_datetime.py
+-rw-rw-rw-   0        0        0     6295 2023-03-08 18:04:01.000000 salabim-24.0.4.post1/tests/test_distributions.py
+-rw-rw-rw-   0        0        0     1693 2023-07-02 09:23:01.000000 salabim-24.0.4.post1/tests/test_misc.py
+-rw-rw-rw-   0        0        0    21283 2024-05-03 11:37:40.000000 salabim-24.0.4.post1/tests/test_monitor.py
+-rw-rw-rw-   0        0        0      654 2020-10-22 20:12:03.000000 salabim-24.0.4.post1/tests/test_process.py
+-rw-rw-rw-   0        0        0     5060 2021-11-17 08:19:40.000000 salabim-24.0.4.post1/tests/test_queue.py
+-rw-rw-rw-   0        0        0      194 2024-05-03 14:07:30.000000 salabim-24.0.4.post1/tests/test_salabim.py
+-rw-rw-rw-   0        0        0     2677 2023-08-14 09:14:44.000000 salabim-24.0.4.post1/tests/test_state.py
+-rw-rw-rw-   0        0        0      344 2023-11-29 17:46:13.000000 salabim-24.0.4.post1/tests/test_store.py
+-rw-rw-rw-   0        0        0     4517 2022-04-30 07:30:12.000000 salabim-24.0.4.post1/tests/test_timeunit.py
```

### Comparing `salabim-24.0.4.post0/PKG-INFO` & `salabim-24.0.4.post1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: salabim
-Version: 24.0.4.post0
+Version: 24.0.4.post1
 Summary: salabim - discrete event simulation in Python
 Author-email: Ruud van der Ham <rt.van.der.ham@gmail.com>
 Project-URL: Homepage, https://salabim.org
 Project-URL: Repository, https://github.com/salabim/salabim
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3 :: Only
```

### Comparing `salabim-24.0.4.post0/README.md` & `salabim-24.0.4.post1/README.md`

 * *Files identical despite different names*

### Comparing `salabim-24.0.4.post0/pyproject.toml` & `salabim-24.0.4.post1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 [project]
 name = "salabim"
 authors = [
     {name = "Ruud van der Ham", email = "rt.van.der.ham@gmail.com"}
 ]
 description = "salabim - discrete event simulation in Python"
-version = "24.0.4-0"
+version = "24.0.4-1"
 readme = "README.md"
 requires-python = ">=3.7"
 dependencies = [
 ]
 classifiers = [
   "Development Status :: 5 - Production/Stable",
   "License :: OSI Approved :: MIT License",
```

### Comparing `salabim-24.0.4.post0/salabim/DejaVuSansMono.ttf` & `salabim-24.0.4.post1/salabim/DejaVuSansMono.ttf`

 * *Files identical despite different names*

### Comparing `salabim-24.0.4.post0/salabim/LICENSE.txt` & `salabim-24.0.4.post1/salabim/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `salabim-24.0.4.post0/salabim/calibri.ttf` & `salabim-24.0.4.post1/salabim/calibri.ttf`

 * *Files identical despite different names*

### Comparing `salabim-24.0.4.post0/salabim/changelog.txt` & `salabim-24.0.4.post1/salabim/changelog.txt`

 * *Files identical despite different names*

### Comparing `salabim-24.0.4.post0/salabim/mplus-1m-regular.ttf` & `salabim-24.0.4.post1/salabim/mplus-1m-regular.ttf`

 * *Files identical despite different names*

### Comparing `salabim-24.0.4.post0/salabim/salabim.py` & `salabim-24.0.4.post1/salabim/salabim.py`

 * *Files 0% similar despite different names*

```diff
@@ -68327,25 +68327,28 @@
 0010ae60: 2069 6620 7365 6c66 2e69 6e63 6c75 6465   if self.include
 0010ae70: 5f70 7269 6e74 3a0a 2020 2020 2020 2020  _print:.        
 0010ae80: 2020 2020 7365 6c66 2e73 7464 6f75 742e      self.stdout.
 0010ae90: 666c 7573 6828 290a 0a0a 7265 7365 7428  flush()...reset(
 0010aea0: 290a 0a73 6574 5f65 6e76 6972 6f6e 6d65  )..set_environme
 0010aeb0: 6e74 5f61 6c69 6173 6573 2829 0a0a 6966  nt_aliases()..if
 0010aec0: 205f 5f6e 616d 655f 5f20 3d3d 2022 5f5f   __name__ == "__
-0010aed0: 6d61 696e 5f5f 223a 0a20 2020 2074 7279  main__":.    try
-0010aee0: 3a0a 2020 2020 2020 2020 696d 706f 7274  :.        import
-0010aef0: 2073 616c 6162 696d 5f65 7870 0a20 2020   salabim_exp.   
-0010af00: 2065 7863 6570 7420 4578 6365 7074 696f   except Exceptio
-0010af10: 6e20 6173 2065 3a0a 2020 2020 2020 2020  n as e:.        
-0010af20: 7072 696e 7428 2273 616c 6162 696d 5f65  print("salabim_e
-0010af30: 7870 2e70 7920 6e6f 7420 666f 756e 6420  xp.py not found 
-0010af40: 6f72 203f 2229 0a20 2020 2020 2020 2072  or ?").        r
-0010af50: 6169 7365 2065 0a0a 2020 2020 7472 793a  aise e..    try:
-0010af60: 0a20 2020 2020 2020 2073 616c 6162 696d  .        salabim
-0010af70: 5f65 7870 2e5f 5f64 6963 745f 5f5b 2265  _exp.__dict__["e
-0010af80: 7870 225d 0a20 2020 2065 7863 6570 7420  xp"].    except 
-0010af90: 4b65 7945 7272 6f72 3a0a 2020 2020 2020  KeyError:.      
-0010afa0: 2020 7072 696e 7428 2273 616c 6162 696d    print("salabim
-0010afb0: 5f65 7870 2e65 7870 2829 206e 6f74 2066  _exp.exp() not f
-0010afc0: 6f75 6e64 2229 0a20 2020 2020 2020 2071  ound").        q
-0010afd0: 7569 7428 290a 0a20 2020 2073 616c 6162  uit()..    salab
-0010afe0: 696d 5f65 7870 2e65 7870 2829 0a         im_exp.exp().
+0010aed0: 6d61 696e 5f5f 223a 0a20 2020 2073 7973  main__":.    sys
+0010aee0: 2e70 6174 682e 696e 7365 7274 2830 2c73  .path.insert(0,s
+0010aef0: 7472 2850 6174 682e 6377 6428 292f 226d  tr(Path.cwd()/"m
+0010af00: 6973 6322 2929 0a20 2020 2074 7279 3a0a  isc")).    try:.
+0010af10: 2020 2020 2020 2020 696d 706f 7274 2073          import s
+0010af20: 616c 6162 696d 5f65 7870 0a20 2020 2065  alabim_exp.    e
+0010af30: 7863 6570 7420 4578 6365 7074 696f 6e20  xcept Exception 
+0010af40: 6173 2065 3a0a 2020 2020 2020 2020 7072  as e:.        pr
+0010af50: 696e 7428 2273 616c 6162 696d 5f65 7870  int("salabim_exp
+0010af60: 2e70 7920 6e6f 7420 666f 756e 6420 6f72  .py not found or
+0010af70: 203f 2229 0a20 2020 2020 2020 2072 6169   ?").        rai
+0010af80: 7365 2065 0a0a 2020 2020 7472 793a 0a20  se e..    try:. 
+0010af90: 2020 2020 2020 2073 616c 6162 696d 5f65         salabim_e
+0010afa0: 7870 2e5f 5f64 6963 745f 5f5b 2265 7870  xp.__dict__["exp
+0010afb0: 225d 0a20 2020 2065 7863 6570 7420 4b65  "].    except Ke
+0010afc0: 7945 7272 6f72 3a0a 2020 2020 2020 2020  yError:.        
+0010afd0: 7072 696e 7428 2273 616c 6162 696d 5f65  print("salabim_e
+0010afe0: 7870 2e65 7870 2829 206e 6f74 2066 6f75  xp.exp() not fou
+0010aff0: 6e64 2229 0a20 2020 2020 2020 2071 7569  nd").        qui
+0010b000: 7428 290a 0a20 2020 2073 616c 6162 696d  t()..    salabim
+0010b010: 5f65 7870 2e65 7870 2829 0a              _exp.exp().
```

### Comparing `salabim-24.0.4.post0/salabim.egg-info/PKG-INFO` & `salabim-24.0.4.post1/salabim.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: salabim
-Version: 24.0.4.post0
+Version: 24.0.4.post1
 Summary: salabim - discrete event simulation in Python
 Author-email: Ruud van der Ham <rt.van.der.ham@gmail.com>
 Project-URL: Homepage, https://salabim.org
 Project-URL: Repository, https://github.com/salabim/salabim
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3 :: Only
```

### Comparing `salabim-24.0.4.post0/salabim.egg-info/SOURCES.txt` & `salabim-24.0.4.post1/salabim.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 README.md
 pyproject.toml
 salabim/DejaVuSansMono.ttf
 salabim/LICENSE.txt
+salabim/__init__.py
 salabim/calibri.ttf
 salabim/changelog.txt
 salabim/mplus-1m-regular.ttf
 salabim/salabim.py
 salabim.egg-info/PKG-INFO
 salabim.egg-info/SOURCES.txt
 salabim.egg-info/dependency_links.txt
```

### Comparing `salabim-24.0.4.post0/tests/test_cap_now.py` & `salabim-24.0.4.post1/tests/test_cap_now.py`

 * *Files identical despite different names*

### Comparing `salabim-24.0.4.post0/tests/test_componentgenerator.py` & `salabim-24.0.4.post1/tests/test_componentgenerator.py`

 * *Files identical despite different names*

### Comparing `salabim-24.0.4.post0/tests/test_datetime.py` & `salabim-24.0.4.post1/tests/test_datetime.py`

 * *Files identical despite different names*

### Comparing `salabim-24.0.4.post0/tests/test_distributions.py` & `salabim-24.0.4.post1/tests/test_distributions.py`

 * *Files identical despite different names*

### Comparing `salabim-24.0.4.post0/tests/test_misc.py` & `salabim-24.0.4.post1/tests/test_misc.py`

 * *Files identical despite different names*

### Comparing `salabim-24.0.4.post0/tests/test_monitor.py` & `salabim-24.0.4.post1/tests/test_monitor.py`

 * *Files 1% similar despite different names*

```diff
@@ -393,21 +393,21 @@
             self.hold(10.1, mode="ghi")
             self.release()
             self.passivate(mode="jkl")
 
     class Interrupter(sim.Component):
         def process(self):
             self.hold(6)
-            x0.interrupt()
-            x1.interrupt()
-            x2.interrupt()
+            for x in (x0,x1,x2):
+                if x.isscheduled():
+                    x.interrupt()
             self.hold(4)
-            x0.resume()
-            x1.resume()
-            x2.resume()
+            for x in (x0,x1,x2):
+                if x.isinterrupted():
+                    x.resume()
 
     def status_map(status):
         return sim.statuses().index(status)
 
     modes = "abc def ghi jkl".split()
 
     env = sim.Environment(trace=False)
@@ -421,15 +421,15 @@
     env.run(4.3)
     x0.activate()
     x1.activate()
     x2.activate()
 
     env.run(till=50)
 
-    assert x1.status.value_duration("requesting") == pytest.approx(10.1)
+    assert x1.status.value_duration("requesting") == pytest.approx(14.1)
 
     assert x0.mode.xt(force_numeric=None) == (["abc", "ghi", "jkl", "jkl"], array("d", [0.0, 4.3, 18.4, 50.0]))
     assert x0.status.xt(force_numeric=None) == (
         ["data", "scheduled", "interrupted", "scheduled", "passive", "passive"],
         array("d", [0.0, 4.3, 6.0, 10.0, 18.4, 50.0]),
     )
     assert x0.status.values() == ["data", "interrupted", "passive", "scheduled"]
```

### Comparing `salabim-24.0.4.post0/tests/test_process.py` & `salabim-24.0.4.post1/tests/test_process.py`

 * *Files identical despite different names*

### Comparing `salabim-24.0.4.post0/tests/test_queue.py` & `salabim-24.0.4.post1/tests/test_queue.py`

 * *Files identical despite different names*

### Comparing `salabim-24.0.4.post0/tests/test_state.py` & `salabim-24.0.4.post1/tests/test_state.py`

 * *Files identical despite different names*

### Comparing `salabim-24.0.4.post0/tests/test_timeunit.py` & `salabim-24.0.4.post1/tests/test_timeunit.py`

 * *Files identical despite different names*

