# Comparing `tmp/pchjlib-0.0.3.6.tar.gz` & `tmp/pchjlib-0.0.3.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pchjlib-0.0.3.6.tar", last modified: Sun Mar  3 10:51:52 2024, max compression
+gzip compressed data, was "pchjlib-0.0.3.7.tar", last modified: Sat May  4 15:02:57 2024, max compression
```

## Comparing `pchjlib-0.0.3.6.tar` & `pchjlib-0.0.3.7.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2024-03-03 10:51:52.756431 pchjlib-0.0.3.6/
--rw-rw-rw-   0        0        0       10 2024-02-20 13:43:18.000000 pchjlib-0.0.3.6/COPYRIGHT.txt
--rw-rw-rw-   0        0        0     1086 2024-02-18 13:43:57.000000 pchjlib-0.0.3.6/LICENSE.txt
--rw-rw-rw-   0        0        0       59 2024-02-18 13:46:41.000000 pchjlib-0.0.3.6/MANIFEST.in
--rw-rw-rw-   0        0        0    18688 2024-03-03 10:51:52.756431 pchjlib-0.0.3.6/PKG-INFO
--rw-rw-rw-   0        0        0    16328 2024-03-03 10:50:34.000000 pchjlib-0.0.3.6/README.md
--rw-rw-rw-   0        0        0      365 2024-03-03 10:51:52.756431 pchjlib-0.0.3.6/setup.cfg
--rw-rw-rw-   0        0        0     4061 2024-03-03 10:49:19.000000 pchjlib-0.0.3.6/setup.py
-drwxrwxrwx   0        0        0        0 2024-03-03 10:51:52.749001 pchjlib-0.0.3.6/src/
-drwxrwxrwx   0        0        0        0 2024-03-03 10:51:52.756431 pchjlib-0.0.3.6/src/pchjlib.egg-info/
--rw-rw-rw-   0        0        0    18688 2024-03-03 10:51:52.000000 pchjlib-0.0.3.6/src/pchjlib.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      323 2024-03-03 10:51:52.000000 pchjlib-0.0.3.6/src/pchjlib.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-03-03 10:51:52.000000 pchjlib-0.0.3.6/src/pchjlib.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       41 2024-03-03 10:51:52.000000 pchjlib-0.0.3.6/src/pchjlib.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       12 2024-03-03 10:51:52.000000 pchjlib-0.0.3.6/src/pchjlib.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2024-03-03 10:51:52.000000 pchjlib-0.0.3.6/src/pchjlib.egg-info/top_level.txt
--rw-rw-rw-   0        0        0        2 2024-03-03 10:51:52.000000 pchjlib-0.0.3.6/src/pchjlib.egg-info/zip-safe
--rw-rw-rw-   0        0        0    46511 2024-03-03 10:48:19.000000 pchjlib-0.0.3.6/src/pchjlib.py
+drwxrwxrwx   0        0        0        0 2024-05-04 15:02:57.796834 pchjlib-0.0.3.7/
+-rw-rw-rw-   0        0        0       10 2024-02-20 13:43:18.000000 pchjlib-0.0.3.7/COPYRIGHT.txt
+-rw-rw-rw-   0        0        0     1086 2024-02-18 13:43:57.000000 pchjlib-0.0.3.7/LICENSE.txt
+-rw-rw-rw-   0        0        0       59 2024-02-18 13:46:41.000000 pchjlib-0.0.3.7/MANIFEST.in
+-rw-rw-rw-   0        0        0    17270 2024-05-04 15:02:57.796834 pchjlib-0.0.3.7/PKG-INFO
+-rw-rw-rw-   0        0        0    15737 2024-05-04 15:00:56.000000 pchjlib-0.0.3.7/README.md
+-rw-rw-rw-   0        0        0      365 2024-05-04 15:02:57.796834 pchjlib-0.0.3.7/setup.cfg
+-rw-rw-rw-   0        0        0     4061 2024-05-04 15:01:53.000000 pchjlib-0.0.3.7/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-04 15:02:57.787634 pchjlib-0.0.3.7/src/
+drwxrwxrwx   0        0        0        0 2024-05-04 15:02:57.796834 pchjlib-0.0.3.7/src/pchjlib.egg-info/
+-rw-rw-rw-   0        0        0    17270 2024-05-04 15:02:57.000000 pchjlib-0.0.3.7/src/pchjlib.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      323 2024-05-04 15:02:57.000000 pchjlib-0.0.3.7/src/pchjlib.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-04 15:02:57.000000 pchjlib-0.0.3.7/src/pchjlib.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       41 2024-05-04 15:02:57.000000 pchjlib-0.0.3.7/src/pchjlib.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       12 2024-05-04 15:02:57.000000 pchjlib-0.0.3.7/src/pchjlib.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2024-05-04 15:02:57.000000 pchjlib-0.0.3.7/src/pchjlib.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0        2 2024-05-04 15:02:57.000000 pchjlib-0.0.3.7/src/pchjlib.egg-info/zip-safe
+-rw-rw-rw-   0        0        0    46545 2024-05-04 15:01:16.000000 pchjlib-0.0.3.7/src/pchjlib.py
```

### Comparing `pchjlib-0.0.3.6/LICENSE.txt` & `pchjlib-0.0.3.7/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pchjlib-0.0.3.6/README.md` & `pchjlib-0.0.3.7/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -348,43 +348,44 @@
 - mp_loading(n):
 >> LOADING...
 ```
 
 ### Ham mo phong cay thong.
 ``` python
 - mp_christmas_tree():
-                      * 
-                    * * * 
-                  * * * * * 
-                * * * * * * * 
-              * * * * * * * * * 
-            * * * * * * * * * * * 
-          * * * * * * * * * * * * * 
-                      * 
-                      * 
-                      * 
+- Nhap chieu cao cay thong: 8
+        *
+       * *
+      * * *
+     * * * *
+    * * * * *
+   * * * * * *
+  * * * * * * *
+ * * * * * * * *
+        ▮
+        ▮
 ```
 
 # Ham ho tro tinh toan dac biet:
 ### Ham tinh toan cac cong thuc vat ly.
 ``` python
 - tinh_toan_vat_ly_8().
 >> Mot bang lua chon cac cong thuc vat ly 8 chuong trinh GDPT 2018 sach CTST HK1;
 >>
-    ————————————————————————————————————————————————————————————————————————————————————
-  |                 >>>>> NHAP TEN CONG THUC BAN MUON DE ADMIN TINH <<<<<               |
-  |                         ~~~ ! Luu y: Nhap theo yeu cau ! ~~~                        |
-  |                                                                                     |
-  |        --> 1. Cong thuc tinh: Khoi luong rieng      (ki hieu D, Kg/m^3)             |
-  |        --> 2. Cong thuc tinh: Trong luong rieng     (ki hieu d, don vi N/m^3)       |
-  |        --> 3. Cong thuc tinh: Luc day Archimedes    (ki hieu Fa, don vi N)          |
-  |        --> 4. Cong thuc tinh: Trong luong           (ki hieu P, don vi N)           |
-  |        --> 5. Cong thuc tinh: Ap suat chat ran      (ki hieu p, N/m^2)              |
-  |        --> 6. Cong thuc tinh: Ap suat chat long     (ki hieu p, N/m^2)              |
-    ———————————————————————————————————————————————————————————————————————————————————-
+
+                   >>>>> NHAP TEN CONG THUC BAN MUON DE ADMIN TINH <<<<<               
+                           ~~~ ! Luu y: Nhap theo yeu cau ! ~~~                        
+                                                                                       
+          --> 1. Cong thuc tinh: Khoi luong rieng      (ki hieu D, Kg/m^3)             
+          --> 2. Cong thuc tinh: Trong luong rieng     (ki hieu d, don vi N/m^3)       
+          --> 3. Cong thuc tinh: Luc day Archimedes    (ki hieu Fa, don vi N)         
+          --> 4. Cong thuc tinh: Trong luong           (ki hieu P, don vi N)           
+          --> 5. Cong thuc tinh: Ap suat chat ran      (ki hieu p, N/m^2)             
+          --> 6. Cong thuc tinh: Ap suat chat long     (ki hieu p, N/m^2)              
+
       AD: Nhap cong thuc ban chon de AD tinh: 4
   - Nhap khoi luong cua vat (kg): 3.4
       AD: Dang tinh toan [■■■■■■■■■■■■■■■■■■■■■■■■■■■■■] 100%
       AD: Trong luong cua chat do la:  33.32 N 
 ```
 
 ### Ham tinh toan tien dien a la chi so cu, b la chi so moi (b > a).
@@ -441,14 +442,17 @@
 ``` python
 - one_two_three().
 >> Nhung su lua chon de ban choi keo bua bao voi A.I;
 ```
 
 # NHUNG BAN CAP NHAT
 
+### 0.0.3.7 - (4/5/2024).
+- ***Cap nhat "mp_christmas_tree".***
+
 ### 0.0.3.6 - (03/03/2024).
 - ***Thu nghiem.***
 
 ### 0.0.3.5 - (01/03/2024).
 - ***Thu nghiem.***
 
 ### 0.0.3.4 - (26/02/2024).
```

### Comparing `pchjlib-0.0.3.6/setup.py` & `pchjlib-0.0.3.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -28,15 +28,15 @@
 from setuptools import setup
 
 
 desc = open(r"C:\Users\LAPTOP DELL\Desktop\pchjlib_admin\README.md").read()
 
 setup(
     name="pchjlib",
-    version="0.0.3.6",
+    version="0.0.3.7",
     author="Joesifer",
     description="Thư viện này có thể thực hiện các phép tính, thuật toán, xử lí chuỗi, mảng, . . .",
     long_description=desc,
     long_description_content_type="text/markdown",
     license="MIT License",
     keywords="pchjlib",
     classifiers=[
```

### Comparing `pchjlib-0.0.3.6/src/pchjlib.py` & `pchjlib-0.0.3.7/src/pchjlib.py`

 * *Files 2% similar despite different names*

```diff
@@ -30,15 +30,15 @@
 
 Tác giả
 ---------------------------------------------------------
 - Joesifer.
 
 Phiên bản
 ---------------------------------------------------------
-- 0.0.3.6.
+- 0.0.3.7.
 
 Ngày đăng
 ---------------------------------------------------------
 - ngày 14 tháng Hai, năm 2024.
 
 Bản quyền
 ---------------------------------------------------------
@@ -972,24 +972,28 @@
             time.sleep(0.4)
         sys.stdout.write("\b\b\b   \b\b\b")
         sys.stdout.flush()
 
 
 # Ham mo phong cay thong
 def mp_christmas_tree():
-    n = 9  # De tao cay thong dep thi cho n = 9
-    for i in range(1, n + 1):
-        for __ in range(n - i + 5):
-            print(" ", end=" ")
-        for _ in range(2 * i - 5):
-            print("*", end=" ")
-        print()
-    for i in range(3):
-        print("                     ", end="")
-        print(" * ")
+    n = int(input("- Nhập chiều cao cây thông: "))
+    tree, dem = [], n
+    for i in range(n):
+        tree.append("* " * (i + 1) + " " * (i + 1))
+
+    for i in range(n):
+        tree[i] = " " * dem + tree[i]
+        dem -= 1
+
+    for i in range(n // 3):
+        tree.append(" " * n + "▮")
+
+    for i in range(len(tree)):
+        print(tree[i])
 
 
 # # Ham ho tro tinh toan dac biet
 # Ham tinh toan cac cong thuc vat ly
 def tinh_toan_vat_ly_8():
     print(
         "\n",
```

