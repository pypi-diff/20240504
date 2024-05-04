# Comparing `tmp/easy_fossy-2.2.0.tar.gz` & `tmp/easy_fossy-2.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "easy_fossy-2.2.0.tar", max compression
+gzip compressed data, was "easy_fossy-2.3.0.tar", max compression
```

## Comparing `easy_fossy-2.2.0.tar` & `easy_fossy-2.3.0.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0    62158 2024-05-03 05:55:45.770536 easy_fossy-2.2.0/easy_fossy/__init__.py
--rw-r--r--   0        0        0    19753 2024-05-03 05:53:26.880880 easy_fossy-2.2.0/easy_fossy/models.py
--rw-r--r--   0        0        0     1089 2024-02-13 20:02:56.662156 easy_fossy-2.2.0/LICENSE
--rw-r--r--   0        0        0      612 2024-05-03 05:50:45.110121 easy_fossy-2.2.0/pyproject.toml
--rw-r--r--   0        0        0     7204 2024-05-02 21:45:14.462297 easy_fossy-2.2.0/README.md
--rw-r--r--   0        0        0     7802 1970-01-01 00:00:00.000000 easy_fossy-2.2.0/PKG-INFO
+-rw-r--r--   0        0        0    63267 2024-05-04 08:30:10.179859 easy_fossy-2.3.0/easy_fossy/__init__.py
+-rw-r--r--   0        0        0    19753 2024-05-03 05:53:26.880880 easy_fossy-2.3.0/easy_fossy/models.py
+-rw-r--r--   0        0        0     1089 2024-02-13 20:02:56.662156 easy_fossy-2.3.0/LICENSE
+-rw-r--r--   0        0        0      612 2024-05-04 07:35:27.944616 easy_fossy-2.3.0/pyproject.toml
+-rw-r--r--   0        0        0     7204 2024-05-02 21:45:14.462297 easy_fossy-2.3.0/README.md
+-rw-r--r--   0        0        0     7802 1970-01-01 00:00:00.000000 easy_fossy-2.3.0/PKG-INFO
```

### Comparing `easy_fossy-2.2.0/easy_fossy/__init__.py` & `easy_fossy-2.3.0/easy_fossy/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -40,14 +40,15 @@
     UploadType1,
     UploadType2,
     User,
     ReportFormat,
 )
 
 import requests
+import json
 import time
 import configparser
 import datetime
 import sys
 from pathlib import Path
 from typing import List
 from requests_toolbelt.multipart.encoder import MultipartEncoder
@@ -1034,26 +1035,55 @@
         visibility: Public,
     ) -> str:
         """get_upload_id_by_download_url_package_upload(file_download_url: str, file_name: str, folder_id: int, upload_desc: str, visibility: Public) -> str"""
         # files = {'file': open(file_path, 'rb')}
         if not self.check_url_exists(file_download_url):
             print(f"git url {file_download_url} is malformed")
 
-        m = MultipartEncoder(fields={"url": file_download_url, "name": file_name})
+        # m = MultipartEncoder(fields={"url": file_download_url, "name": file_name})
+        m = {
+            "location": {
+                "url": file_download_url,
+                "name": file_name,
+            },
+            "scanOptions": {
+                "analysis": {
+                    "bucket": True,
+                    "copyright_email_author": True,
+                    "ecc": True,
+                    "keyword": True,
+                    "mime": True,
+                    "monk": True,
+                    "nomos": True,
+                    "ojo": True,
+                    "package": True,
+                    "reso": True,
+                    "heritage": False,
+                },
+                "decider": {
+                    "nomos_monk": True,
+                    "bulk_reused": True,
+                    "new_scanner": True,
+                    "ojo_decider": True,
+                },
+            },
+        }
         headers = {
             # "accept": "application/json",
             "folderId": str(folder_id),
             "groupName": self.group_name,
             "uploadType": "url",
             "uploadDescription": upload_desc,
             "public": visibility.name,
-            "Content-Type": m.content_type,
+            "Content-Type": "application/json",
             "Authorization": self.bearer_token,
         }
-        response = requests.post(self.url + str("uploads"), data=m, headers=headers)
+        response = requests.post(
+            self.url + str("uploads"), data=json.dumps(m), headers=headers
+        )
 
         timeout = 20
         timewait = 0.2
         timer = 0
 
         while response.status_code != 201:
 
@@ -1066,15 +1096,18 @@
                 break
             if response.status_code == 201:
                 break
 
         match response.json():
             case {**info}:
                 report_info = Info(**info)
-                print(f"upload id is {report_info.message}")
+                if isinstance(report_info.message, str):
+                    print(f"Error while getting upload id: {report_info.message}")
+                    sys.exit(1)
+                # print(f"upload id is {report_info.message}")
                 return report_info.message
             case _:
                 print(response.text)
 
     # get_upload_id_by_download_url_package_upload(
     #     file_download_url='https://github.com/dineshr93/pageres/archive/refs/heads/master.zip', file_name='pageres', folder_id=1, upload_desc='commons-io-2.11.0', visibility=Public.public)
```

### Comparing `easy_fossy-2.2.0/easy_fossy/models.py` & `easy_fossy-2.3.0/easy_fossy/models.py`

 * *Files identical despite different names*

### Comparing `easy_fossy-2.2.0/LICENSE` & `easy_fossy-2.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `easy_fossy-2.2.0/pyproject.toml` & `easy_fossy-2.3.0/pyproject.toml`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "easy_fossy"
-version = "2.2.0"
+version = "2.3.0"
 description = "fossology API wrapper in python 3.10"
 authors = ["dinesh_ravi"]
 license = "MIT License"
 readme = "README.md"
 
 [tool.poetry.scripts]
 easy_fossy = 'easy_fossy:easy_fossy'
```

### Comparing `easy_fossy-2.2.0/README.md` & `easy_fossy-2.3.0/README.md`

 * *Files identical despite different names*

### Comparing `easy_fossy-2.2.0/PKG-INFO` & `easy_fossy-2.3.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: easy_fossy
-Version: 2.2.0
+Version: 2.3.0
 Summary: fossology API wrapper in python 3.10
 License: MIT
 Author: dinesh_ravi
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
```

