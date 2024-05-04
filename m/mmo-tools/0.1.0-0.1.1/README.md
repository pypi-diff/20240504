# Comparing `tmp/mmo_tools-0.1.0.tar.gz` & `tmp/mmo_tools-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mmo_tools-0.1.0.tar", last modified: Sat May  4 12:39:43 2024, max compression
+gzip compressed data, was "mmo_tools-0.1.1.tar", last modified: Sat May  4 13:03:28 2024, max compression
```

## Comparing `mmo_tools-0.1.0.tar` & `mmo_tools-0.1.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2024-05-04 12:39:43.442509 mmo_tools-0.1.0/
--rw-rw-rw-   0        0        0     1836 2024-05-04 12:39:43.441514 mmo_tools-0.1.0/PKG-INFO
--rw-rw-rw-   0        0        0      978 2024-05-04 12:39:31.000000 mmo_tools-0.1.0/README.md
--rw-rw-rw-   0        0        0       42 2024-05-04 12:39:43.442509 mmo_tools-0.1.0/setup.cfg
--rw-rw-rw-   0        0        0     1235 2024-05-04 12:39:22.000000 mmo_tools-0.1.0/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-04 12:39:43.420723 mmo_tools-0.1.0/src/
-drwxrwxrwx   0        0        0        0 2024-05-04 12:39:43.423723 mmo_tools-0.1.0/src/mmo_tools/
--rw-rw-rw-   0        0        0      209 2024-05-04 11:18:50.000000 mmo_tools-0.1.0/src/mmo_tools/__init__.py
--rw-rw-rw-   0        0        0     2513 2024-05-04 12:06:32.000000 mmo_tools-0.1.0/src/mmo_tools/core.py
--rw-rw-rw-   0        0        0     1803 2024-05-04 11:33:36.000000 mmo_tools-0.1.0/src/mmo_tools/utils.py
-drwxrwxrwx   0        0        0        0 2024-05-04 12:39:43.441514 mmo_tools-0.1.0/src/mmo_tools.egg-info/
--rw-rw-rw-   0        0        0     1836 2024-05-04 12:39:43.000000 mmo_tools-0.1.0/src/mmo_tools.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      237 2024-05-04 12:39:43.000000 mmo_tools-0.1.0/src/mmo_tools.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-04 12:39:43.000000 mmo_tools-0.1.0/src/mmo_tools.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       10 2024-05-04 12:39:43.000000 mmo_tools-0.1.0/src/mmo_tools.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-04 13:03:28.717174 mmo_tools-0.1.1/
+-rw-rw-rw-   0        0        0     1723 2024-05-04 13:03:28.715170 mmo_tools-0.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0      889 2024-05-04 12:47:45.000000 mmo_tools-0.1.1/README.md
+-rw-rw-rw-   0        0        0       42 2024-05-04 13:03:28.717174 mmo_tools-0.1.1/setup.cfg
+-rw-rw-rw-   0        0        0     1235 2024-05-04 13:01:15.000000 mmo_tools-0.1.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-04 13:03:28.694172 mmo_tools-0.1.1/src/
+drwxrwxrwx   0        0        0        0 2024-05-04 13:03:28.709169 mmo_tools-0.1.1/src/mmo_tools/
+-rw-rw-rw-   0        0        0      160 2024-05-04 13:02:54.000000 mmo_tools-0.1.1/src/mmo_tools/__init__.py
+-rw-rw-rw-   0        0        0     2638 2024-05-04 12:56:59.000000 mmo_tools-0.1.1/src/mmo_tools/core.py
+-rw-rw-rw-   0        0        0     1836 2024-05-04 13:02:48.000000 mmo_tools-0.1.1/src/mmo_tools/utils.py
+drwxrwxrwx   0        0        0        0 2024-05-04 13:03:28.714171 mmo_tools-0.1.1/src/mmo_tools.egg-info/
+-rw-rw-rw-   0        0        0     1723 2024-05-04 13:03:28.000000 mmo_tools-0.1.1/src/mmo_tools.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      237 2024-05-04 13:03:28.000000 mmo_tools-0.1.1/src/mmo_tools.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-04 13:03:28.000000 mmo_tools-0.1.1/src/mmo_tools.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       10 2024-05-04 13:03:28.000000 mmo_tools-0.1.1/src/mmo_tools.egg-info/top_level.txt
```

### Comparing `mmo_tools-0.1.0/PKG-INFO` & `mmo_tools-0.1.1/src/mmo_tools.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,32 +1,29 @@
 Metadata-Version: 2.1
-Name: mmo_tools
-Version: 0.1.0
+Name: mmo-tools
+Version: 0.1.1
 Summary: Thư Viện Hỗ Trợ Viết Tool Facebook Nhanh
 Home-page: UNKNOWN
 Author: Lam Dinh
 Author-email: ldl.contact.booking@gmail.com
 License: UNKNOWN
 Description: # mmo_tools
-        ©dinhlam
         Đây là một thư viện Python chứa các hàm tiện ích để chuyển đổi dữ liệu và cấu hình proxy .
         
         ## func
         
         ### `convert_data(file)`
         - Chuyển đổi dữ liệu từ tệp đầu vào thành danh sách các đối tượng từ điển.
         - **input**: path file input (str).
         - **result**: dict (`[{},{}`]).
         
         #### example
         ```python
         import os , sys
-        from lam_tools import convert_data
-        
-        sys.path.append(os.path.join(os.path.dirname(__file__), 'src'))
+        from mmo_tools import *
         # Giả sử file_path là đường dẫn tới tệp dữ liệu
         file_path = 'data/mmo_tools.txt'
         
         # Chuyển đổi dữ liệu từ tệp
         data = convert_data(file_path)
         
         print(data)  # [{'key': 'value'}, {'key2': 'value2'}]
```

### Comparing `mmo_tools-0.1.0/README.md` & `mmo_tools-0.1.1/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -1,24 +1,21 @@
 # mmo_tools
-©dinhlam
 Đây là một thư viện Python chứa các hàm tiện ích để chuyển đổi dữ liệu và cấu hình proxy .
 
 ## func
 
 ### `convert_data(file)`
 - Chuyển đổi dữ liệu từ tệp đầu vào thành danh sách các đối tượng từ điển.
 - **input**: path file input (str).
 - **result**: dict (`[{},{}`]).
 
 #### example
 ```python
 import os , sys
-from lam_tools import convert_data
-
-sys.path.append(os.path.join(os.path.dirname(__file__), 'src'))
+from mmo_tools import *
 # Giả sử file_path là đường dẫn tới tệp dữ liệu
 file_path = 'data/mmo_tools.txt'
 
 # Chuyển đổi dữ liệu từ tệp
 data = convert_data(file_path)
 
 print(data)  # [{'key': 'value'}, {'key2': 'value2'}]
```

### Comparing `mmo_tools-0.1.0/setup.py` & `mmo_tools-0.1.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
   'Operating System :: Microsoft :: Windows :: Windows 10',
   'License :: OSI Approved :: MIT License',
   'Programming Language :: Python :: 3'
 ]
  
 setup(
     name='mmo_tools',  # Tên thư viện của bạn
-    version='0.1.0',  # Phiên bản đầu tiên
+    version='0.1.1',  # Phiên bản đầu tiên
     packages=find_packages('src'),  # Tìm tất cả các packages trong thư mục src
     package_dir={'': 'src'},  # Chỉ định thư mục chứa các packages
     author='Lam Dinh',
     author_email='ldl.contact.booking@gmail.com',
     description='Thư Viện Hỗ Trợ Viết Tool Facebook Nhanh',
     long_description=open('README.md','r',encoding='utf-8').read(),  # Đọc nội dung README nếu có
     long_description_content_type='text/markdown',  # Định dạng của long description
```

### Comparing `mmo_tools-0.1.0/src/mmo_tools/core.py` & `mmo_tools-0.1.1/src/mmo_tools/core.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from . import utils
-import os , re
+import os , re , requests
+
 def convert_data(file) -> str:
    
     try:
         data_r =  open(file , "r",encoding="UTF-8").readlines()
     except Exception as error:
         return error
     data   = []
@@ -21,15 +22,15 @@
         if password: rp.update({"password":password})
         
         for rtip in r.split("|"):
             if "NA" in rtip and ":" in rtip:rp.update({"fb_dtsg":rtip.strip("\n")})
             if ("c_user" in rtip) or ("i_user" in rtip):rp.update({"cookie":rtip.strip("\n")})
             if ("Mozilla" in rtip) or ("Chrome" in rtip) or ("Safari" in rtip) or ("AppleWebKit" in rtip):rp.update({"user-agent":rtip.strip("\n")})
             if (len(rtip) > 150 ) and ('=' not in rtip) :rtip.update({'access_token':rtip.strip('\n')})
-            if (len(rtip.split(':')) in [2,4]) or ('http://' in rtip):rp.update({'proxy':rtip.strip('\n')}) # http://danhnguyen:tothemoon@45.43.190.197:6715
+            if (len(rtip.split(':')) in [2,4]) or ('http://' in rtip):rp.update({'proxy':rtip.strip('\n')}) 
             if ("c_user" not in rtip) and (len(rtip) >= 32 and len(rtip) <= 40) and ("@" not in rtip):rp.update({'code':rtip.strip('\n')})
             try:
                 email = re.search(r'@(.*)\.',rtip.strip("\n"))[1]
                 if utils.type_emailr(email):
                     rp.update({'email':rtip.strip('\n')})
                     pass_mail = utils.type_pwemail(value=r , valuemail=rtip.strip("\n"))
                     if pass_mail:rp.update({'passemail':pass_mail})
@@ -54,7 +55,11 @@
         ip , port , user , pass_proxy = map(str,proxy.split(":"))
         https = {
             "https":f"http://{user}:{pass_proxy}@{ip}:{ port}",
             "http":f"http://{user}:{pass_proxy}@{ip}:{ port}"
             }
     return https
 
+def checklive(fbid):
+    if len(requests.get(f'https://graph.facebook.com/{fbid}/picture?redirect=0').json()['data']['url']) >= 150: return 1
+    return 0
+
```

### Comparing `mmo_tools-0.1.0/src/mmo_tools/utils.py` & `mmo_tools-0.1.1/src/mmo_tools/utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,10 @@
 
+from datetime import datetime
+
 def type_pw(value,valueid):
     value =  value + "|"
     for index , x in enumerate(value.split("|")):
         try:
             if valueid == x and len(value.split("|")) >  1:
                 return value.split("|")[index + 1]
         except:pass
```

### Comparing `mmo_tools-0.1.0/src/mmo_tools.egg-info/PKG-INFO` & `mmo_tools-0.1.1/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,32 +1,29 @@
 Metadata-Version: 2.1
-Name: mmo-tools
-Version: 0.1.0
+Name: mmo_tools
+Version: 0.1.1
 Summary: Thư Viện Hỗ Trợ Viết Tool Facebook Nhanh
 Home-page: UNKNOWN
 Author: Lam Dinh
 Author-email: ldl.contact.booking@gmail.com
 License: UNKNOWN
 Description: # mmo_tools
-        ©dinhlam
         Đây là một thư viện Python chứa các hàm tiện ích để chuyển đổi dữ liệu và cấu hình proxy .
         
         ## func
         
         ### `convert_data(file)`
         - Chuyển đổi dữ liệu từ tệp đầu vào thành danh sách các đối tượng từ điển.
         - **input**: path file input (str).
         - **result**: dict (`[{},{}`]).
         
         #### example
         ```python
         import os , sys
-        from lam_tools import convert_data
-        
-        sys.path.append(os.path.join(os.path.dirname(__file__), 'src'))
+        from mmo_tools import *
         # Giả sử file_path là đường dẫn tới tệp dữ liệu
         file_path = 'data/mmo_tools.txt'
         
         # Chuyển đổi dữ liệu từ tệp
         data = convert_data(file_path)
         
         print(data)  # [{'key': 'value'}, {'key2': 'value2'}]
```

