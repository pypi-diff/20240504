# Comparing `tmp/siglyser-0.112.tar.gz` & `tmp/siglyser-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "siglyser-0.112.tar", last modified: Mon Apr 22 15:33:51 2024, max compression
+gzip compressed data, was "siglyser-0.2.tar", last modified: Sat May  4 12:37:29 2024, max compression
```

## Comparing `siglyser-0.112.tar` & `siglyser-0.2.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2024-04-22 15:33:51.827218 siglyser-0.112/
--rw-rw-rw-   0        0        0      243 2024-04-22 15:33:51.827218 siglyser-0.112/PKG-INFO
--rw-rw-rw-   0        0        0      143 2024-04-17 15:48:54.000000 siglyser-0.112/README.md
--rw-rw-rw-   0        0        0       42 2024-04-22 15:33:51.827218 siglyser-0.112/setup.cfg
--rw-rw-rw-   0        0        0      359 2024-04-22 15:33:01.000000 siglyser-0.112/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-22 15:33:51.795852 siglyser-0.112/siglyser/
--rw-rw-rw-   0        0        0       53 2024-04-17 16:48:28.000000 siglyser-0.112/siglyser/__init__.py
--rw-rw-rw-   0        0        0     3506 2024-04-20 13:45:38.000000 siglyser-0.112/siglyser/main.py
-drwxrwxrwx   0        0        0        0 2024-04-22 15:33:51.827218 siglyser-0.112/siglyser.egg-info/
--rw-rw-rw-   0        0        0      243 2024-04-22 15:33:51.000000 siglyser-0.112/siglyser.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      184 2024-04-22 15:33:51.000000 siglyser-0.112/siglyser.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-22 15:33:51.000000 siglyser-0.112/siglyser.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2024-04-22 15:33:51.000000 siglyser-0.112/siglyser.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-04 12:37:29.458494 siglyser-0.2/
+-rw-rw-rw-   0        0        0      241 2024-05-04 12:37:29.457613 siglyser-0.2/PKG-INFO
+-rw-rw-rw-   0        0        0      143 2024-04-17 15:48:54.000000 siglyser-0.2/README.md
+-rw-rw-rw-   0        0        0       42 2024-05-04 12:37:29.458494 siglyser-0.2/setup.cfg
+-rw-rw-rw-   0        0        0      357 2024-05-04 12:35:13.000000 siglyser-0.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-04 12:37:29.415681 siglyser-0.2/siglyser/
+-rw-rw-rw-   0        0        0       53 2024-04-17 16:48:28.000000 siglyser-0.2/siglyser/__init__.py
+-rw-rw-rw-   0        0        0     3572 2024-05-04 12:35:47.000000 siglyser-0.2/siglyser/main.py
+drwxrwxrwx   0        0        0        0 2024-05-04 12:37:29.455096 siglyser-0.2/siglyser.egg-info/
+-rw-rw-rw-   0        0        0      241 2024-05-04 12:37:29.000000 siglyser-0.2/siglyser.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      184 2024-05-04 12:37:29.000000 siglyser-0.2/siglyser.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-04 12:37:29.000000 siglyser-0.2/siglyser.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2024-05-04 12:37:29.000000 siglyser-0.2/siglyser.egg-info/top_level.txt
```

### Comparing `siglyser-0.112/siglyser/main.py` & `siglyser-0.2/siglyser/main.py`

 * *Files 7% similar despite different names*

```diff
@@ -10,14 +10,17 @@
 
 
 def calc_fft(time_sec, vibr):
     """
     Inputs:
     time_sec: time in second
     vibr: vibration signal corresponding to time data.
+    Outputs:
+    frequency in Hz
+    vibration fft in base units.
     """
     datalength_fft = len(time_sec)
     datalengthby2 = int(datalength_fft/2)
     timeavgcalc = np.array([], dtype = float64)
     time_sec_i = time_sec[1:]
     time_sec_i_1 = time_sec[:-1]
     timeavgcalc = time_sec_i - time_sec_i_1
```

