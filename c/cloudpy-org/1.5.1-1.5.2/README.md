# Comparing `tmp/cloudpy_org-1.5.1.tar.gz` & `tmp/cloudpy_org-1.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\cloudpy_org-1.5.1.tar", last modified: Wed May  1 08:59:29 2024, max compression
+gzip compressed data, was "dist\cloudpy_org-1.5.2.tar", last modified: Sat May  4 09:21:40 2024, max compression
```

## Comparing `cloudpy_org-1.5.1.tar` & `cloudpy_org-1.5.2.tar`

### file list

```diff
@@ -1,19 +1,20 @@
-drwxrwxrwx   0        0        0        0 2024-05-01 08:59:29.608911 cloudpy_org-1.5.1/
--rw-rw-rw-   0        0        0      935 2024-05-01 08:59:29.608262 cloudpy_org-1.5.1/PKG-INFO
--rw-rw-rw-   0        0        0      454 2023-04-14 05:11:55.000000 cloudpy_org-1.5.1/README.md
-drwxrwxrwx   0        0        0        0 2024-05-01 08:59:29.474939 cloudpy_org-1.5.1/cloudpy_org/
--rw-rw-rw-   0        0        0     3169 2024-05-01 08:55:23.000000 cloudpy_org-1.5.1/cloudpy_org/__init__.py
--rw-rw-rw-   0        0        0    32752 2024-05-01 08:48:41.000000 cloudpy_org-1.5.1/cloudpy_org/aws.py
--rw-rw-rw-   0        0        0    23305 2024-05-01 08:48:51.000000 cloudpy_org-1.5.1/cloudpy_org/client_usage.py
--rw-rw-rw-   0        0        0    13614 2024-05-01 08:49:05.000000 cloudpy_org-1.5.1/cloudpy_org/docs.py
--rw-rw-rw-   0        0        0     3924 2024-05-01 08:43:26.000000 cloudpy_org-1.5.1/cloudpy_org/imgedit.py
--rw-rw-rw-   0        0        0    49731 2024-05-01 08:49:21.000000 cloudpy_org-1.5.1/cloudpy_org/tools.py
--rw-rw-rw-   0        0        0     4998 2024-05-01 08:49:29.000000 cloudpy_org-1.5.1/cloudpy_org/web.py
-drwxrwxrwx   0        0        0        0 2024-05-01 08:59:29.585321 cloudpy_org-1.5.1/cloudpy_org.egg-info/
--rw-rw-rw-   0        0        0      935 2024-05-01 08:59:27.000000 cloudpy_org-1.5.1/cloudpy_org.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      346 2024-05-01 08:59:28.000000 cloudpy_org-1.5.1/cloudpy_org.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-01 08:59:27.000000 cloudpy_org-1.5.1/cloudpy_org.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       63 2024-05-01 08:59:27.000000 cloudpy_org-1.5.1/cloudpy_org.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2024-05-01 08:59:27.000000 cloudpy_org-1.5.1/cloudpy_org.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-01 08:59:29.608911 cloudpy_org-1.5.1/setup.cfg
--rw-rw-rw-   0        0        0     1324 2024-05-01 08:58:57.000000 cloudpy_org-1.5.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-04 09:21:40.960820 cloudpy_org-1.5.2/
+-rw-rw-rw-   0        0        0      935 2024-05-04 09:21:40.960043 cloudpy_org-1.5.2/PKG-INFO
+-rw-rw-rw-   0        0        0      454 2023-04-14 05:11:55.000000 cloudpy_org-1.5.2/README.md
+drwxrwxrwx   0        0        0        0 2024-05-04 09:21:40.814471 cloudpy_org-1.5.2/cloudpy_org/
+-rw-rw-rw-   0        0        0     3233 2024-05-04 09:15:13.000000 cloudpy_org-1.5.2/cloudpy_org/__init__.py
+-rw-rw-rw-   0        0        0    32752 2024-05-01 08:48:41.000000 cloudpy_org-1.5.2/cloudpy_org/aws.py
+-rw-rw-rw-   0        0        0    23305 2024-05-01 08:48:51.000000 cloudpy_org-1.5.2/cloudpy_org/client_usage.py
+-rw-rw-rw-   0        0        0    13614 2024-05-01 08:49:05.000000 cloudpy_org-1.5.2/cloudpy_org/docs.py
+-rw-rw-rw-   0        0        0     3924 2024-05-01 08:43:26.000000 cloudpy_org-1.5.2/cloudpy_org/imgedit.py
+-rw-rw-rw-   0        0        0    49731 2024-05-01 08:49:21.000000 cloudpy_org-1.5.2/cloudpy_org/tools.py
+-rw-rw-rw-   0        0        0     4998 2024-05-01 08:49:29.000000 cloudpy_org-1.5.2/cloudpy_org/web.py
+-rw-rw-rw-   0        0        0     7083 2024-05-04 09:14:52.000000 cloudpy_org-1.5.2/cloudpy_org/web_client_usage.py
+drwxrwxrwx   0        0        0        0 2024-05-04 09:21:40.935074 cloudpy_org-1.5.2/cloudpy_org.egg-info/
+-rw-rw-rw-   0        0        0      935 2024-05-04 09:21:39.000000 cloudpy_org-1.5.2/cloudpy_org.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      378 2024-05-04 09:21:39.000000 cloudpy_org-1.5.2/cloudpy_org.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-04 09:21:39.000000 cloudpy_org-1.5.2/cloudpy_org.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       63 2024-05-04 09:21:39.000000 cloudpy_org-1.5.2/cloudpy_org.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2024-05-04 09:21:39.000000 cloudpy_org-1.5.2/cloudpy_org.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-04 09:21:40.961319 cloudpy_org-1.5.2/setup.cfg
+-rw-rw-rw-   0        0        0     1324 2024-05-04 09:15:33.000000 cloudpy_org-1.5.2/setup.py
```

### Comparing `cloudpy_org-1.5.1/PKG-INFO` & `cloudpy_org-1.5.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cloudpy_org
-Version: 1.5.1
+Version: 1.5.2
 Summary: Cloud data pipeline organization and automation library. Includes AWS framework manager API.
 Home-page: https://www.cloudpy.org/
 Author: cloudpy.org
 Author-email: admin@cloudpy.org
 License: MIT
 Description: A library to programmatically create, interact, encrypt and automate your data pipelines making it simple to scale to the most popular cloud plattforms.
 Platform: UNKNOWN
```

### Comparing `cloudpy_org-1.5.1/cloudpy_org/__init__.py` & `cloudpy_org-1.5.2/cloudpy_org/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -24,15 +24,16 @@
  'eu-west-1': {'long_name': 'Europe (Ireland)', 'code': 'euw1'},
  'eu-west-2': {'long_name': 'Europe (London)', 'code': 'euw2'},
  'eu-west-3': {'long_name': 'Europe (Paris)', 'code': 'euw3'},
  'eu-north-1': {'long_name': 'Europe (Stockholm)', 'code': 'eun1'},
  'sa-east-1': {'long_name': 'South America (São Paulo)', 'code': 'sae1'}}
 subscription_url = 'https://www.cloudpy.org'
 msh = 'secure'
-cloudpy_org_version='1.5.1'
+cloudpy_org_version='1.5.2'
 gsep = {'user_email_sep': '-0-', '@': '-1-', '.': '-2-'}
 from cloudpy_org.tools import processing_tools,unique_id
 from cloudpy_org.docs import auto_document,convert_jupiter_notebook_to_html,documentation_from_folder
 from cloudpy_org.aws import aws_framework_manager,aws_framework_manager_client,gen_aws_auth_token,gen_new_service_token,configure_aws,get_my_aws_service_token,authenticate_with_token,delete_biscuit,co_token_auth
 from cloudpy_org.web import flask_website
 from cloudpy_org.imgedit import colors
-from cloudpy_org.client_usage import cloudpy_org_aws_framework_client
+from cloudpy_org.client_usage import cloudpy_org_aws_framework_client
+from cloudpy_org.web_client_usage import cloudpy_org_web_client
```

### Comparing `cloudpy_org-1.5.1/cloudpy_org/aws.py` & `cloudpy_org-1.5.2/cloudpy_org/aws.py`

 * *Files identical despite different names*

### Comparing `cloudpy_org-1.5.1/cloudpy_org/client_usage.py` & `cloudpy_org-1.5.2/cloudpy_org/client_usage.py`

 * *Files identical despite different names*

### Comparing `cloudpy_org-1.5.1/cloudpy_org/docs.py` & `cloudpy_org-1.5.2/cloudpy_org/docs.py`

 * *Files identical despite different names*

### Comparing `cloudpy_org-1.5.1/cloudpy_org/imgedit.py` & `cloudpy_org-1.5.2/cloudpy_org/imgedit.py`

 * *Files identical despite different names*

### Comparing `cloudpy_org-1.5.1/cloudpy_org/tools.py` & `cloudpy_org-1.5.2/cloudpy_org/tools.py`

 * *Files identical despite different names*

### Comparing `cloudpy_org-1.5.1/cloudpy_org/web.py` & `cloudpy_org-1.5.2/cloudpy_org/web.py`

 * *Files identical despite different names*

### Comparing `cloudpy_org-1.5.1/cloudpy_org.egg-info/PKG-INFO` & `cloudpy_org-1.5.2/cloudpy_org.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cloudpy-org
-Version: 1.5.1
+Version: 1.5.2
 Summary: Cloud data pipeline organization and automation library. Includes AWS framework manager API.
 Home-page: https://www.cloudpy.org/
 Author: cloudpy.org
 Author-email: admin@cloudpy.org
 License: MIT
 Description: A library to programmatically create, interact, encrypt and automate your data pipelines making it simple to scale to the most popular cloud plattforms.
 Platform: UNKNOWN
```

### Comparing `cloudpy_org-1.5.1/setup.py` & `cloudpy_org-1.5.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from os import path
 
 
 long_description = 'A library to programmatically create, interact, encrypt and automate your data pipelines making it simple to scale to the most popular cloud plattforms.'
 
 setup(
     name="cloudpy_org",
-    version="1.5.1",
+    version="1.5.2",
     description="Cloud data pipeline organization and automation library. Includes AWS framework manager API.",
     long_description_content_type="text/markdown",
     long_description=long_description,
     url="https://www.cloudpy.org/",
     author="cloudpy.org",
     author_email="admin@cloudpy.org",
     license="MIT",
```

