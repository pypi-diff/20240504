# Comparing `tmp/heaobject-1.5.0.tar.gz` & `tmp/heaobject-1.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "heaobject-1.5.0.tar", last modified: Wed Apr 24 17:29:04 2024, max compression
+gzip compressed data, was "heaobject-1.5.1.tar", last modified: Fri May  3 23:00:45 2024, max compression
```

## Comparing `heaobject-1.5.0.tar` & `heaobject-1.5.1.tar`

### file list

```diff
@@ -1,45 +1,45 @@
-drwxrwxrwx   0        0        0        0 2024-04-24 17:29:04.979987 heaobject-1.5.0/
--rw-rw-rw-   0        0        0    11625 2022-03-11 01:28:08.000000 heaobject-1.5.0/LICENSE
--rw-rw-rw-   0        0        0     4832 2024-04-24 17:29:04.978987 heaobject-1.5.0/PKG-INFO
--rw-rw-rw-   0        0        0     3326 2024-04-24 17:10:28.000000 heaobject-1.5.0/README.md
--rw-rw-rw-   0        0        0       42 2024-04-24 17:29:04.980988 heaobject-1.5.0/setup.cfg
--rw-rw-rw-   0        0        0     2603 2024-04-24 17:08:43.000000 heaobject-1.5.0/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-24 17:29:04.921704 heaobject-1.5.0/src/
-drwxrwxrwx   0        0        0        0 2024-04-24 17:29:04.969800 heaobject-1.5.0/src/heaobject/
--rw-rw-rw-   0        0        0     1247 2023-12-16 22:23:08.000000 heaobject-1.5.0/src/heaobject/__init__.py
--rw-rw-rw-   0        0        0     4970 2024-04-09 20:34:56.000000 heaobject-1.5.0/src/heaobject/account.py
--rw-rw-rw-   0        0        0    15629 2024-04-09 20:34:56.000000 heaobject-1.5.0/src/heaobject/activity.py
--rw-rw-rw-   0        0        0     4030 2023-12-16 22:23:08.000000 heaobject-1.5.0/src/heaobject/aws.py
--rw-rw-rw-   0        0        0     6945 2023-12-16 22:23:08.000000 heaobject-1.5.0/src/heaobject/awss3key.py
--rw-rw-rw-   0        0        0     7587 2024-04-09 20:34:56.000000 heaobject-1.5.0/src/heaobject/bucket.py
--rw-rw-rw-   0        0        0     9918 2024-04-09 20:34:56.000000 heaobject-1.5.0/src/heaobject/data.py
--rw-rw-rw-   0        0        0     2604 2023-12-16 22:23:08.000000 heaobject-1.5.0/src/heaobject/dataadapter.py
--rw-rw-rw-   0        0        0      272 2022-03-11 01:28:08.000000 heaobject-1.5.0/src/heaobject/dataelement.py
--rw-rw-rw-   0        0        0     1601 2022-03-11 01:28:08.000000 heaobject-1.5.0/src/heaobject/datamodel.py
--rw-rw-rw-   0        0        0      430 2022-03-11 01:28:08.000000 heaobject-1.5.0/src/heaobject/datapattern.py
--rw-rw-rw-   0        0        0      238 2023-12-16 22:23:08.000000 heaobject-1.5.0/src/heaobject/datatransform.py
--rw-rw-rw-   0        0        0      353 2023-12-16 22:23:08.000000 heaobject-1.5.0/src/heaobject/error.py
--rw-rw-rw-   0        0        0    22016 2024-04-09 20:34:56.000000 heaobject-1.5.0/src/heaobject/folder.py
--rw-rw-rw-   0        0        0     4662 2024-04-09 20:34:56.000000 heaobject-1.5.0/src/heaobject/keychain.py
--rw-rw-rw-   0        0        0     2859 2024-04-09 20:34:56.000000 heaobject-1.5.0/src/heaobject/mimetype.py
--rw-rw-rw-   0        0        0    14028 2024-04-24 17:07:44.000000 heaobject-1.5.0/src/heaobject/organization.py
--rw-rw-rw-   0        0        0    10911 2024-04-21 20:58:31.000000 heaobject-1.5.0/src/heaobject/person.py
--rw-rw-rw-   0        0        0     5129 2024-04-09 20:34:56.000000 heaobject-1.5.0/src/heaobject/project.py
--rw-rw-rw-   0        0        0        0 2022-03-11 01:28:08.000000 heaobject-1.5.0/src/heaobject/py.typed
--rw-rw-rw-   0        0        0      211 2024-04-09 20:34:56.000000 heaobject-1.5.0/src/heaobject/record.py
--rw-rw-rw-   0        0        0    24659 2024-04-09 20:34:56.000000 heaobject-1.5.0/src/heaobject/registry.py
--rw-rw-rw-   0        0        0    80257 2024-04-22 18:17:42.000000 heaobject-1.5.0/src/heaobject/root.py
--rw-rw-rw-   0        0        0      597 2024-04-09 20:34:56.000000 heaobject-1.5.0/src/heaobject/settings.py
--rw-rw-rw-   0        0        0       66 2024-03-26 22:41:59.000000 heaobject-1.5.0/src/heaobject/source.py
--rw-rw-rw-   0        0        0     1165 2023-12-16 22:23:08.000000 heaobject-1.5.0/src/heaobject/source2target.py
--rw-rw-rw-   0        0        0     4074 2024-04-09 20:34:56.000000 heaobject-1.5.0/src/heaobject/storage.py
--rw-rw-rw-   0        0        0    10289 2024-04-18 02:00:20.000000 heaobject-1.5.0/src/heaobject/trash.py
--rw-rw-rw-   0        0        0     1135 2024-03-26 22:41:59.000000 heaobject-1.5.0/src/heaobject/user.py
--rw-rw-rw-   0        0        0      498 2023-12-16 22:23:08.000000 heaobject-1.5.0/src/heaobject/util.py
--rw-rw-rw-   0        0        0     6618 2024-04-09 20:34:56.000000 heaobject-1.5.0/src/heaobject/volume.py
-drwxrwxrwx   0        0        0        0 2024-04-24 17:29:04.977988 heaobject-1.5.0/src/heaobject.egg-info/
--rw-rw-rw-   0        0        0     4832 2024-04-24 17:29:04.000000 heaobject-1.5.0/src/heaobject.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      995 2024-04-24 17:29:04.000000 heaobject-1.5.0/src/heaobject.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-24 17:29:04.000000 heaobject-1.5.0/src/heaobject.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      144 2024-04-24 17:29:04.000000 heaobject-1.5.0/src/heaobject.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2024-04-24 17:29:04.000000 heaobject-1.5.0/src/heaobject.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-03 23:00:45.340875 heaobject-1.5.1/
+-rw-rw-rw-   0        0        0    11625 2022-03-11 01:28:08.000000 heaobject-1.5.1/LICENSE
+-rw-rw-rw-   0        0        0     4832 2024-05-03 23:00:45.338737 heaobject-1.5.1/PKG-INFO
+-rw-rw-rw-   0        0        0     3326 2024-04-24 17:43:21.000000 heaobject-1.5.1/README.md
+-rw-rw-rw-   0        0        0       42 2024-05-03 23:00:45.340875 heaobject-1.5.1/setup.cfg
+-rw-rw-rw-   0        0        0     2603 2024-05-03 22:59:57.000000 heaobject-1.5.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-03 23:00:45.271629 heaobject-1.5.1/src/
+drwxrwxrwx   0        0        0        0 2024-05-03 23:00:45.328738 heaobject-1.5.1/src/heaobject/
+-rw-rw-rw-   0        0        0     1247 2023-12-16 22:23:08.000000 heaobject-1.5.1/src/heaobject/__init__.py
+-rw-rw-rw-   0        0        0     4970 2024-05-03 22:46:44.000000 heaobject-1.5.1/src/heaobject/account.py
+-rw-rw-rw-   0        0        0    15629 2024-04-09 20:34:56.000000 heaobject-1.5.1/src/heaobject/activity.py
+-rw-rw-rw-   0        0        0     4030 2023-12-16 22:23:08.000000 heaobject-1.5.1/src/heaobject/aws.py
+-rw-rw-rw-   0        0        0     6945 2023-12-16 22:23:08.000000 heaobject-1.5.1/src/heaobject/awss3key.py
+-rw-rw-rw-   0        0        0     7587 2024-04-09 20:34:56.000000 heaobject-1.5.1/src/heaobject/bucket.py
+-rw-rw-rw-   0        0        0     9934 2024-05-03 22:47:48.000000 heaobject-1.5.1/src/heaobject/data.py
+-rw-rw-rw-   0        0        0     2604 2023-12-16 22:23:08.000000 heaobject-1.5.1/src/heaobject/dataadapter.py
+-rw-rw-rw-   0        0        0      272 2022-03-11 01:28:08.000000 heaobject-1.5.1/src/heaobject/dataelement.py
+-rw-rw-rw-   0        0        0     1601 2022-03-11 01:28:08.000000 heaobject-1.5.1/src/heaobject/datamodel.py
+-rw-rw-rw-   0        0        0      430 2022-03-11 01:28:08.000000 heaobject-1.5.1/src/heaobject/datapattern.py
+-rw-rw-rw-   0        0        0      238 2023-12-16 22:23:08.000000 heaobject-1.5.1/src/heaobject/datatransform.py
+-rw-rw-rw-   0        0        0      353 2023-12-16 22:23:08.000000 heaobject-1.5.1/src/heaobject/error.py
+-rw-rw-rw-   0        0        0    22016 2024-04-09 20:34:56.000000 heaobject-1.5.1/src/heaobject/folder.py
+-rw-rw-rw-   0        0        0     4662 2024-04-26 23:28:37.000000 heaobject-1.5.1/src/heaobject/keychain.py
+-rw-rw-rw-   0        0        0     2859 2024-04-09 20:34:56.000000 heaobject-1.5.1/src/heaobject/mimetype.py
+-rw-rw-rw-   0        0        0    14028 2024-05-03 22:46:44.000000 heaobject-1.5.1/src/heaobject/organization.py
+-rw-rw-rw-   0        0        0    10911 2024-05-03 22:46:44.000000 heaobject-1.5.1/src/heaobject/person.py
+-rw-rw-rw-   0        0        0     5129 2024-04-09 20:34:56.000000 heaobject-1.5.1/src/heaobject/project.py
+-rw-rw-rw-   0        0        0        0 2022-03-11 01:28:08.000000 heaobject-1.5.1/src/heaobject/py.typed
+-rw-rw-rw-   0        0        0      211 2024-04-09 20:34:56.000000 heaobject-1.5.1/src/heaobject/record.py
+-rw-rw-rw-   0        0        0    24659 2024-04-09 20:34:56.000000 heaobject-1.5.1/src/heaobject/registry.py
+-rw-rw-rw-   0        0        0    80257 2024-04-24 17:43:21.000000 heaobject-1.5.1/src/heaobject/root.py
+-rw-rw-rw-   0        0        0      597 2024-04-09 20:34:56.000000 heaobject-1.5.1/src/heaobject/settings.py
+-rw-rw-rw-   0        0        0       66 2024-03-26 22:41:59.000000 heaobject-1.5.1/src/heaobject/source.py
+-rw-rw-rw-   0        0        0     1165 2023-12-16 22:23:08.000000 heaobject-1.5.1/src/heaobject/source2target.py
+-rw-rw-rw-   0        0        0     4074 2024-04-09 20:34:56.000000 heaobject-1.5.1/src/heaobject/storage.py
+-rw-rw-rw-   0        0        0    10289 2024-04-18 02:00:20.000000 heaobject-1.5.1/src/heaobject/trash.py
+-rw-rw-rw-   0        0        0     1191 2024-04-24 22:21:12.000000 heaobject-1.5.1/src/heaobject/user.py
+-rw-rw-rw-   0        0        0      498 2023-12-16 22:23:08.000000 heaobject-1.5.1/src/heaobject/util.py
+-rw-rw-rw-   0        0        0     6618 2024-05-03 22:46:44.000000 heaobject-1.5.1/src/heaobject/volume.py
+drwxrwxrwx   0        0        0        0 2024-05-03 23:00:45.337164 heaobject-1.5.1/src/heaobject.egg-info/
+-rw-rw-rw-   0        0        0     4832 2024-05-03 23:00:45.000000 heaobject-1.5.1/src/heaobject.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      995 2024-05-03 23:00:45.000000 heaobject-1.5.1/src/heaobject.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-03 23:00:45.000000 heaobject-1.5.1/src/heaobject.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      144 2024-05-03 23:00:45.000000 heaobject-1.5.1/src/heaobject.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2024-05-03 23:00:45.000000 heaobject-1.5.1/src/heaobject.egg-info/top_level.txt
```

### Comparing `heaobject-1.5.0/LICENSE` & `heaobject-1.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `heaobject-1.5.0/PKG-INFO` & `heaobject-1.5.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: heaobject
-Version: 1.5.0
+Version: 1.5.1
 Summary: Data and other classes that are passed into and out of HEA REST APIs.
 Home-page: https://risr.hci.utah.edu
 Author: Research Informatics Shared Resource, Huntsman Cancer Institute, Salt Lake City, UT
 Author-email: Andrew.Post@hci.utah.edu
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
```

### Comparing `heaobject-1.5.0/README.md` & `heaobject-1.5.1/README.md`

 * *Files identical despite different names*

### Comparing `heaobject-1.5.0/setup.py` & `heaobject-1.5.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 from os import path
 
 this_directory = path.abspath(path.dirname(__file__))
 with open(path.join(this_directory, 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
 
 setuptools.setup(name='heaobject',
-                 version='1.5.0',
+                 version='1.5.1',
                  description='Data and other classes that are passed into and out of HEA REST APIs.',
                  long_description=long_description,
                  long_description_content_type='text/markdown',
                  url='https://risr.hci.utah.edu',
                  author='Research Informatics Shared Resource, Huntsman Cancer Institute, Salt Lake City, UT',
                  author_email='Andrew.Post@hci.utah.edu',
                  python_requires='>=3.10',
```

### Comparing `heaobject-1.5.0/src/heaobject/__init__.py` & `heaobject-1.5.1/src/heaobject/__init__.py`

 * *Files identical despite different names*

### Comparing `heaobject-1.5.0/src/heaobject/account.py` & `heaobject-1.5.1/src/heaobject/account.py`

 * *Files identical despite different names*

### Comparing `heaobject-1.5.0/src/heaobject/activity.py` & `heaobject-1.5.1/src/heaobject/activity.py`

 * *Files identical despite different names*

### Comparing `heaobject-1.5.0/src/heaobject/aws.py` & `heaobject-1.5.1/src/heaobject/aws.py`

 * *Files identical despite different names*

### Comparing `heaobject-1.5.0/src/heaobject/awss3key.py` & `heaobject-1.5.1/src/heaobject/awss3key.py`

 * *Files identical despite different names*

### Comparing `heaobject-1.5.0/src/heaobject/bucket.py` & `heaobject-1.5.1/src/heaobject/bucket.py`

 * *Files identical despite different names*

### Comparing `heaobject-1.5.0/src/heaobject/data.py` & `heaobject-1.5.1/src/heaobject/data.py`

 * *Files 0% similar despite different names*

```diff
@@ -168,15 +168,15 @@
         """
         key = self.key
         if key is not None and is_folder(key):
             key = key.strip('/')
         if key is not None:
             return key.rsplit('/', maxsplit=1)[-1]
         else:
-            return None
+            return super().display_name
 
     @display_name.setter
     def display_name(self, display_name: str):
         if display_name is not None:
             if '/' in display_name:
                 raise ValueError(f'display_name {display_name} cannot contain slashes')
             try:
```

### Comparing `heaobject-1.5.0/src/heaobject/dataadapter.py` & `heaobject-1.5.1/src/heaobject/dataadapter.py`

 * *Files identical despite different names*

### Comparing `heaobject-1.5.0/src/heaobject/datamodel.py` & `heaobject-1.5.1/src/heaobject/datamodel.py`

 * *Files identical despite different names*

### Comparing `heaobject-1.5.0/src/heaobject/folder.py` & `heaobject-1.5.1/src/heaobject/folder.py`

 * *Files identical despite different names*

### Comparing `heaobject-1.5.0/src/heaobject/keychain.py` & `heaobject-1.5.1/src/heaobject/keychain.py`

 * *Files identical despite different names*

### Comparing `heaobject-1.5.0/src/heaobject/mimetype.py` & `heaobject-1.5.1/src/heaobject/mimetype.py`

 * *Files identical despite different names*

### Comparing `heaobject-1.5.0/src/heaobject/organization.py` & `heaobject-1.5.1/src/heaobject/organization.py`

 * *Files identical despite different names*

### Comparing `heaobject-1.5.0/src/heaobject/person.py` & `heaobject-1.5.1/src/heaobject/person.py`

 * *Files identical despite different names*

### Comparing `heaobject-1.5.0/src/heaobject/project.py` & `heaobject-1.5.1/src/heaobject/project.py`

 * *Files identical despite different names*

### Comparing `heaobject-1.5.0/src/heaobject/registry.py` & `heaobject-1.5.1/src/heaobject/registry.py`

 * *Files identical despite different names*

### Comparing `heaobject-1.5.0/src/heaobject/root.py` & `heaobject-1.5.1/src/heaobject/root.py`

 * *Files identical despite different names*

### Comparing `heaobject-1.5.0/src/heaobject/settings.py` & `heaobject-1.5.1/src/heaobject/settings.py`

 * *Files identical despite different names*

### Comparing `heaobject-1.5.0/src/heaobject/source2target.py` & `heaobject-1.5.1/src/heaobject/source2target.py`

 * *Files identical despite different names*

### Comparing `heaobject-1.5.0/src/heaobject/storage.py` & `heaobject-1.5.1/src/heaobject/storage.py`

 * *Files identical despite different names*

### Comparing `heaobject-1.5.0/src/heaobject/trash.py` & `heaobject-1.5.1/src/heaobject/trash.py`

 * *Files identical despite different names*

### Comparing `heaobject-1.5.0/src/heaobject/user.py` & `heaobject-1.5.1/src/heaobject/user.py`

 * *Files 5% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 """
 
 NONE_USER = 'system|none'
 ALL_USERS = 'system|all'
 TEST_USER = 'system|test'
 SOURCE_USER = 'system|source'
 AWS_USER = 'system|aws'
+CREDENTIALS_MANAGER_USER = 'system|credentialsmanager'
 
 
 def is_system_user(id_: str) -> bool:
     """
     Returns whether the given ID is a system user or not.
 
     :param id_: The user ID to check.
```

### Comparing `heaobject-1.5.0/src/heaobject/volume.py` & `heaobject-1.5.1/src/heaobject/volume.py`

 * *Files identical despite different names*

### Comparing `heaobject-1.5.0/src/heaobject.egg-info/PKG-INFO` & `heaobject-1.5.1/src/heaobject.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: heaobject
-Version: 1.5.0
+Version: 1.5.1
 Summary: Data and other classes that are passed into and out of HEA REST APIs.
 Home-page: https://risr.hci.utah.edu
 Author: Research Informatics Shared Resource, Huntsman Cancer Institute, Salt Lake City, UT
 Author-email: Andrew.Post@hci.utah.edu
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
```

### Comparing `heaobject-1.5.0/src/heaobject.egg-info/SOURCES.txt` & `heaobject-1.5.1/src/heaobject.egg-info/SOURCES.txt`

 * *Files identical despite different names*

