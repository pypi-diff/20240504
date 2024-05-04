# Comparing `tmp/mmo_tools-0.1.2.tar.gz` & `tmp/mmo_tools-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mmo_tools-0.1.2.tar", last modified: Sat May  4 13:15:19 2024, max compression
+gzip compressed data, was "mmo_tools-0.1.3.tar", last modified: Sat May  4 13:24:18 2024, max compression
```

## Comparing `mmo_tools-0.1.2.tar` & `mmo_tools-0.1.3.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2024-05-04 13:15:19.597634 mmo_tools-0.1.2/
--rw-rw-rw-   0        0        0     2385 2024-05-04 13:15:19.597634 mmo_tools-0.1.2/PKG-INFO
--rw-rw-rw-   0        0        0     1391 2024-05-04 13:14:51.000000 mmo_tools-0.1.2/README.md
--rw-rw-rw-   0        0        0       42 2024-05-04 13:15:19.597634 mmo_tools-0.1.2/setup.cfg
--rw-rw-rw-   0        0        0     1235 2024-05-04 13:15:12.000000 mmo_tools-0.1.2/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-04 13:15:19.574798 mmo_tools-0.1.2/src/
-drwxrwxrwx   0        0        0        0 2024-05-04 13:15:19.582794 mmo_tools-0.1.2/src/mmo_tools/
--rw-rw-rw-   0        0        0      183 2024-05-04 13:04:59.000000 mmo_tools-0.1.2/src/mmo_tools/__init__.py
--rw-rw-rw-   0        0        0     2643 2024-05-04 13:14:21.000000 mmo_tools-0.1.2/src/mmo_tools/core.py
--rw-rw-rw-   0        0        0     1836 2024-05-04 13:02:48.000000 mmo_tools-0.1.2/src/mmo_tools/utils.py
-drwxrwxrwx   0        0        0        0 2024-05-04 13:15:19.595789 mmo_tools-0.1.2/src/mmo_tools.egg-info/
--rw-rw-rw-   0        0        0     2385 2024-05-04 13:15:19.000000 mmo_tools-0.1.2/src/mmo_tools.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      237 2024-05-04 13:15:19.000000 mmo_tools-0.1.2/src/mmo_tools.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-04 13:15:19.000000 mmo_tools-0.1.2/src/mmo_tools.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       10 2024-05-04 13:15:19.000000 mmo_tools-0.1.2/src/mmo_tools.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-04 13:24:18.915803 mmo_tools-0.1.3/
+-rw-rw-rw-   0        0        0     2481 2024-05-04 13:24:18.915803 mmo_tools-0.1.3/PKG-INFO
+-rw-rw-rw-   0        0        0     1455 2024-05-04 13:23:51.000000 mmo_tools-0.1.3/README.md
+-rw-rw-rw-   0        0        0       42 2024-05-04 13:24:18.916805 mmo_tools-0.1.3/setup.cfg
+-rw-rw-rw-   0        0        0     1235 2024-05-04 13:24:01.000000 mmo_tools-0.1.3/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-04 13:24:18.893803 mmo_tools-0.1.3/src/
+drwxrwxrwx   0        0        0        0 2024-05-04 13:24:18.903801 mmo_tools-0.1.3/src/mmo_tools/
+-rw-rw-rw-   0        0        0      183 2024-05-04 13:04:59.000000 mmo_tools-0.1.3/src/mmo_tools/__init__.py
+-rw-rw-rw-   0        0        0     2640 2024-05-04 13:23:00.000000 mmo_tools-0.1.3/src/mmo_tools/core.py
+-rw-rw-rw-   0        0        0     1836 2024-05-04 13:02:48.000000 mmo_tools-0.1.3/src/mmo_tools/utils.py
+drwxrwxrwx   0        0        0        0 2024-05-04 13:24:18.913801 mmo_tools-0.1.3/src/mmo_tools.egg-info/
+-rw-rw-rw-   0        0        0     2481 2024-05-04 13:24:18.000000 mmo_tools-0.1.3/src/mmo_tools.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      237 2024-05-04 13:24:18.000000 mmo_tools-0.1.3/src/mmo_tools.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-04 13:24:18.000000 mmo_tools-0.1.3/src/mmo_tools.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       10 2024-05-04 13:24:18.000000 mmo_tools-0.1.3/src/mmo_tools.egg-info/top_level.txt
```

### Comparing `mmo_tools-0.1.2/PKG-INFO` & `mmo_tools-0.1.3/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,18 +1,22 @@
 Metadata-Version: 2.1
 Name: mmo_tools
-Version: 0.1.2
+Version: 0.1.3
 Summary: Thư Viện Hỗ Trợ Viết Tool Facebook Nhanh
 Home-page: UNKNOWN
 Author: Lam Dinh
 Author-email: ldl.contact.booking@gmail.com
 License: UNKNOWN
 Description: # mmo_tools
         Đây là một thư viện Python chứa các hàm tiện ích để chuyển đổi dữ liệu và cấu hình proxy .
         
+        ## service
+        - **convert_data**
+        - **headers**
+        - **checklive**
         ## funciton
         
         ### `convert_data`
         - Chuyển đổi dữ liệu từ tệp đầu vào thành danh sách các đối tượng từ điển.
         - **input**: path file input (str).
         - **result**: dict (`[{},{}`]).
         ### `headers`
```

### Comparing `mmo_tools-0.1.2/README.md` & `mmo_tools-0.1.3/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,14 @@
 # mmo_tools
 Đây là một thư viện Python chứa các hàm tiện ích để chuyển đổi dữ liệu và cấu hình proxy .
 
+## service
+- **convert_data**
+- **headers**
+- **checklive**
 ## funciton
 
 ### `convert_data`
 - Chuyển đổi dữ liệu từ tệp đầu vào thành danh sách các đối tượng từ điển.
 - **input**: path file input (str).
 - **result**: dict (`[{},{}`]).
 ### `headers`
```

### Comparing `mmo_tools-0.1.2/setup.py` & `mmo_tools-0.1.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
   'Operating System :: Microsoft :: Windows :: Windows 10',
   'License :: OSI Approved :: MIT License',
   'Programming Language :: Python :: 3'
 ]
  
 setup(
     name='mmo_tools',  # Tên thư viện của bạn
-    version='0.1.2',  # Phiên bản đầu tiên
+    version='0.1.3',  # Phiên bản đầu tiên
     packages=find_packages('src'),  # Tìm tất cả các packages trong thư mục src
     package_dir={'': 'src'},  # Chỉ định thư mục chứa các packages
     author='Lam Dinh',
     author_email='ldl.contact.booking@gmail.com',
     description='Thư Viện Hỗ Trợ Viết Tool Facebook Nhanh',
     long_description=open('README.md','r',encoding='utf-8').read(),  # Đọc nội dung README nếu có
     long_description_content_type='text/markdown',  # Định dạng của long description
```

### Comparing `mmo_tools-0.1.2/src/mmo_tools/core.py` & `mmo_tools-0.1.3/src/mmo_tools/core.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,15 +21,15 @@
         password = utils.type_pw(value=r , valueid=user)
         if password: rp.update({"password":password})
         
         for rtip in r.split("|"):
             if "NA" in rtip and ":" in rtip:rp.update({"fb_dtsg":rtip.strip("\n")})
             if ("c_user" in rtip) or ("i_user" in rtip):rp.update({"cookie":rtip.strip("\n")})
             if ("Mozilla" in rtip) or ("Chrome" in rtip) or ("Safari" in rtip) or ("AppleWebKit" in rtip):rp.update({"user-agent":rtip.strip("\n")})
-            if (len(rtip) > 150 ) and ('=' not in rtip) :rtip.update({'access_token':rtip.strip('\n')})
+            if (len(rtip) > 150) and ('=' not in rtip) :rp.update({'access_token':rtip.strip('\n')})
             if (len(rtip.split(':')) in [2,4]) or ('http://' in rtip):rp.update({'proxy':rtip.strip('\n')}) 
             if ("c_user" not in rtip) and (len(rtip) >= 32 and len(rtip) <= 40) and ("@" not in rtip):rp.update({'code':rtip.strip('\n')})
             try:
                 email = re.search(r'@(.*)\.',rtip.strip("\n"))[1]
                 if utils.type_emailr(email):
                     rp.update({'email':rtip.strip('\n')})
                     pass_mail = utils.type_pwemail(value=r , valuemail=rtip.strip("\n"))
```

### Comparing `mmo_tools-0.1.2/src/mmo_tools/utils.py` & `mmo_tools-0.1.3/src/mmo_tools/utils.py`

 * *Files identical despite different names*

### Comparing `mmo_tools-0.1.2/src/mmo_tools.egg-info/PKG-INFO` & `mmo_tools-0.1.3/src/mmo_tools.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,18 +1,22 @@
 Metadata-Version: 2.1
 Name: mmo-tools
-Version: 0.1.2
+Version: 0.1.3
 Summary: Thư Viện Hỗ Trợ Viết Tool Facebook Nhanh
 Home-page: UNKNOWN
 Author: Lam Dinh
 Author-email: ldl.contact.booking@gmail.com
 License: UNKNOWN
 Description: # mmo_tools
         Đây là một thư viện Python chứa các hàm tiện ích để chuyển đổi dữ liệu và cấu hình proxy .
         
+        ## service
+        - **convert_data**
+        - **headers**
+        - **checklive**
         ## funciton
         
         ### `convert_data`
         - Chuyển đổi dữ liệu từ tệp đầu vào thành danh sách các đối tượng từ điển.
         - **input**: path file input (str).
         - **result**: dict (`[{},{}`]).
         ### `headers`
```

