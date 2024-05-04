# Comparing `tmp/amino.light.py-0.1.8.tar.gz` & `tmp/amino.light.py-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "amino.light.py-0.1.8.tar", last modified: Sun Apr 28 16:42:02 2024, max compression
+gzip compressed data, was "amino.light.py-0.1.9.tar", last modified: Sat May  4 09:48:32 2024, max compression
```

## Comparing `amino.light.py-0.1.8.tar` & `amino.light.py-0.1.9.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxrwxrwx   0        0        0        0 2024-04-28 16:42:02.510152 amino.light.py-0.1.8/
-drwxrwxrwx   0        0        0        0 2024-04-28 16:42:02.463288 amino.light.py-0.1.8/AminoLightPy/
--rw-rw-rw-   0        0        0      297 2024-04-19 03:59:31.000000 amino.light.py-0.1.8/AminoLightPy/__init__.py
--rw-rw-rw-   0        0        0    14819 2024-04-24 14:56:57.000000 amino.light.py-0.1.8/AminoLightPy/acm.py
--rw-rw-rw-   0        0        0    16533 2024-04-28 15:38:37.000000 amino.light.py-0.1.8/AminoLightPy/amino_socket.py
--rw-rw-rw-   0        0        0    74156 2024-04-28 15:28:46.000000 amino.light.py-0.1.8/AminoLightPy/client.py
--rw-rw-rw-   0        0        0     2704 2024-04-24 14:56:35.000000 amino.light.py-0.1.8/AminoLightPy/constants.py
-drwxrwxrwx   0        0        0        0 2024-04-28 16:42:02.478911 amino.light.py-0.1.8/AminoLightPy/lib/
--rw-rw-rw-   0        0        0        0 2024-04-19 03:59:31.000000 amino.light.py-0.1.8/AminoLightPy/lib/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-28 16:42:02.478911 amino.light.py-0.1.8/AminoLightPy/lib/util/
--rw-rw-rw-   0        0        0       75 2024-04-19 03:26:32.000000 amino.light.py-0.1.8/AminoLightPy/lib/util/__init__.py
--rw-rw-rw-   0        0        0    32832 2024-04-24 14:57:25.000000 amino.light.py-0.1.8/AminoLightPy/lib/util/exceptions.py
--rw-rw-rw-   0        0        0     1846 2024-04-24 14:57:20.000000 amino.light.py-0.1.8/AminoLightPy/lib/util/helpers.py
--rw-rw-rw-   0        0        0    94997 2024-04-28 16:41:32.000000 amino.light.py-0.1.8/AminoLightPy/lib/util/objects.py
--rw-rw-rw-   0        0        0      270 2024-04-28 16:03:50.000000 amino.light.py-0.1.8/AminoLightPy/managers.py
--rw-rw-rw-   0        0        0    67523 2024-04-23 09:48:37.000000 amino.light.py-0.1.8/AminoLightPy/sub_client.py
--rw-rw-rw-   0        0        0     1089 2024-04-06 02:55:57.000000 amino.light.py-0.1.8/LICENSE
--rw-rw-rw-   0        0        0     3630 2024-04-28 16:42:02.510152 amino.light.py-0.1.8/PKG-INFO
--rw-rw-rw-   0        0        0     2834 2024-04-19 02:52:28.000000 amino.light.py-0.1.8/README.md
-drwxrwxrwx   0        0        0        0 2024-04-28 16:42:02.510152 amino.light.py-0.1.8/amino.light.py.egg-info/
--rw-rw-rw-   0        0        0     3630 2024-04-28 16:42:02.000000 amino.light.py-0.1.8/amino.light.py.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      565 2024-04-28 16:42:02.000000 amino.light.py-0.1.8/amino.light.py.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-28 16:42:02.000000 amino.light.py-0.1.8/amino.light.py.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       26 2024-04-28 16:42:02.000000 amino.light.py-0.1.8/amino.light.py.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2024-04-28 16:42:02.000000 amino.light.py-0.1.8/amino.light.py.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-28 16:42:02.525772 amino.light.py-0.1.8/setup.cfg
--rw-rw-rw-   0        0        0     1298 2024-04-28 16:41:53.000000 amino.light.py-0.1.8/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-04 09:48:32.050848 amino.light.py-0.1.9/
+drwxrwxrwx   0        0        0        0 2024-05-04 09:48:31.913033 amino.light.py-0.1.9/AminoLightPy/
+-rw-rw-rw-   0        0        0      297 2024-05-04 09:47:40.000000 amino.light.py-0.1.9/AminoLightPy/__init__.py
+-rw-rw-rw-   0        0        0    14819 2024-04-24 14:56:57.000000 amino.light.py-0.1.9/AminoLightPy/acm.py
+-rw-rw-rw-   0        0        0    16533 2024-04-28 15:38:37.000000 amino.light.py-0.1.9/AminoLightPy/amino_socket.py
+-rw-rw-rw-   0        0        0    74754 2024-04-30 14:32:26.000000 amino.light.py-0.1.9/AminoLightPy/client.py
+-rw-rw-rw-   0        0        0     2704 2024-04-24 14:56:35.000000 amino.light.py-0.1.9/AminoLightPy/constants.py
+drwxrwxrwx   0        0        0        0 2024-05-04 09:48:31.920015 amino.light.py-0.1.9/AminoLightPy/lib/
+-rw-rw-rw-   0        0        0        0 2024-04-19 03:59:31.000000 amino.light.py-0.1.9/AminoLightPy/lib/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-04 09:48:31.932847 amino.light.py-0.1.9/AminoLightPy/lib/util/
+-rw-rw-rw-   0        0        0       75 2024-04-19 03:26:32.000000 amino.light.py-0.1.9/AminoLightPy/lib/util/__init__.py
+-rw-rw-rw-   0        0        0    32832 2024-04-24 14:57:25.000000 amino.light.py-0.1.9/AminoLightPy/lib/util/exceptions.py
+-rw-rw-rw-   0        0        0     1846 2024-04-24 14:57:20.000000 amino.light.py-0.1.9/AminoLightPy/lib/util/helpers.py
+-rw-rw-rw-   0        0        0    94997 2024-04-28 16:41:32.000000 amino.light.py-0.1.9/AminoLightPy/lib/util/objects.py
+-rw-rw-rw-   0        0        0      894 2024-04-30 14:33:17.000000 amino.light.py-0.1.9/AminoLightPy/managers.py
+-rw-rw-rw-   0        0        0    67523 2024-04-23 09:48:37.000000 amino.light.py-0.1.9/AminoLightPy/sub_client.py
+-rw-rw-rw-   0        0        0     1089 2024-04-06 02:55:57.000000 amino.light.py-0.1.9/LICENSE
+-rw-rw-rw-   0        0        0     3630 2024-05-04 09:48:32.049847 amino.light.py-0.1.9/PKG-INFO
+-rw-rw-rw-   0        0        0     2834 2024-04-19 02:52:28.000000 amino.light.py-0.1.9/README.md
+drwxrwxrwx   0        0        0        0 2024-05-04 09:48:32.047857 amino.light.py-0.1.9/amino.light.py.egg-info/
+-rw-rw-rw-   0        0        0     3630 2024-05-04 09:48:30.000000 amino.light.py-0.1.9/amino.light.py.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      565 2024-05-04 09:48:30.000000 amino.light.py-0.1.9/amino.light.py.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-04 09:48:30.000000 amino.light.py-0.1.9/amino.light.py.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       26 2024-05-04 09:48:30.000000 amino.light.py-0.1.9/amino.light.py.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2024-05-04 09:48:30.000000 amino.light.py-0.1.9/amino.light.py.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-04 09:48:32.053849 amino.light.py-0.1.9/setup.cfg
+-rw-rw-rw-   0        0        0     1298 2024-05-04 09:47:20.000000 amino.light.py-0.1.9/setup.py
```

### Comparing `amino.light.py-0.1.8/AminoLightPy/acm.py` & `amino.light.py-0.1.9/AminoLightPy/acm.py`

 * *Files identical despite different names*

### Comparing `amino.light.py-0.1.8/AminoLightPy/amino_socket.py` & `amino.light.py-0.1.9/AminoLightPy/amino_socket.py`

 * *Files identical despite different names*

### Comparing `amino.light.py-0.1.8/AminoLightPy/client.py` & `amino.light.py-0.1.9/AminoLightPy/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 # pylint: disable=invalid-name
 # pylint: disable=too-many-lines
 
 from uuid import uuid4
 from typing import BinaryIO, Union
+from .managers import Typing, Recording
 
 from .constants import api, upload_media, AminoSession
 from .amino_socket import Callbacks, SocketHandler, SocketRequests
 from .lib.util import exceptions, objects, helpers, self_deviceId
 
 
 #@dorthegra/IDörthe#8835 thanks for support!
@@ -2141,7 +2142,25 @@
         if not getNotifications:
             data["notificationStatus"] = 2
         else:
             data["privacyMode"] = 1
 
         response = self.session.post(f"{api}/g/s/account/visit-settings", json=data)
         return response.json()
+
+    def typing(self, chatId: str, comId: int = None) -> Typing:
+        """
+        Start typing message in context manager.
+
+        **Returns**
+            - **Success** : :meth:`class <Typing>`
+        """
+        return Typing(self, chatId=chatId, comId=comId)
+
+    def recording(self, chatId: str, comId: int = None) -> Recording:
+        """
+        Start recording in context manager.
+
+        **Returns**
+            - **Success** : :meth:`class <Recording>`
+        """
+        return Recording(self, chatId=chatId, comId=comId)
```

### Comparing `amino.light.py-0.1.8/AminoLightPy/constants.py` & `amino.light.py-0.1.9/AminoLightPy/constants.py`

 * *Files identical despite different names*

### Comparing `amino.light.py-0.1.8/AminoLightPy/lib/util/exceptions.py` & `amino.light.py-0.1.9/AminoLightPy/lib/util/exceptions.py`

 * *Files identical despite different names*

### Comparing `amino.light.py-0.1.8/AminoLightPy/lib/util/helpers.py` & `amino.light.py-0.1.9/AminoLightPy/lib/util/helpers.py`

 * *Files identical despite different names*

### Comparing `amino.light.py-0.1.8/AminoLightPy/lib/util/objects.py` & `amino.light.py-0.1.9/AminoLightPy/lib/util/objects.py`

 * *Files identical despite different names*

### Comparing `amino.light.py-0.1.8/AminoLightPy/sub_client.py` & `amino.light.py-0.1.9/AminoLightPy/sub_client.py`

 * *Files identical despite different names*

### Comparing `amino.light.py-0.1.8/LICENSE` & `amino.light.py-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `amino.light.py-0.1.8/PKG-INFO` & `amino.light.py-0.1.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: amino.light.py
-Version: 0.1.8
+Version: 0.1.9
 Summary: Best Amino.py alternative
 Home-page: https://github.com/AugustLigh/AminoLightPy
 Author: AugustLight
 License: MIT
 Keywords: amino,aminoapps,amino.fix,amino.light,amino.ligt.py,AminoLightPy,amino-bot,narvii,medialab,api,python,python3,python3.x,minori,august,augustlight,aminolightpy,amino.py
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: amino.light.py Version: 0.1.8 Summary: Best
+Metadata-Version: 2.1 Name: amino.light.py Version: 0.1.9 Summary: Best
 Amino.py alternative Home-page: https://github.com/AugustLigh/AminoLightPy
 Author: AugustLight License: MIT Keywords:
 amino,aminoapps,amino.fix,amino.light,amino.ligt.py,AminoLightPy,amino-
 bot,narvii,medialab,api,python,python3,python3.x,minori,august,augustlight,aminolightpy,amino.py
 Classifier: Intended Audience :: Developers Classifier: License :: OSI Approved
 :: MIT License Classifier: Programming Language :: Python :: 3.9 Classifier:
 Programming Language :: Python :: 3.10 Classifier: Programming Language ::
```

### Comparing `amino.light.py-0.1.8/README.md` & `amino.light.py-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `amino.light.py-0.1.8/amino.light.py.egg-info/PKG-INFO` & `amino.light.py-0.1.9/amino.light.py.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: amino.light.py
-Version: 0.1.8
+Version: 0.1.9
 Summary: Best Amino.py alternative
 Home-page: https://github.com/AugustLigh/AminoLightPy
 Author: AugustLight
 License: MIT
 Keywords: amino,aminoapps,amino.fix,amino.light,amino.ligt.py,AminoLightPy,amino-bot,narvii,medialab,api,python,python3,python3.x,minori,august,augustlight,aminolightpy,amino.py
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: amino.light.py Version: 0.1.8 Summary: Best
+Metadata-Version: 2.1 Name: amino.light.py Version: 0.1.9 Summary: Best
 Amino.py alternative Home-page: https://github.com/AugustLigh/AminoLightPy
 Author: AugustLight License: MIT Keywords:
 amino,aminoapps,amino.fix,amino.light,amino.ligt.py,AminoLightPy,amino-
 bot,narvii,medialab,api,python,python3,python3.x,minori,august,augustlight,aminolightpy,amino.py
 Classifier: Intended Audience :: Developers Classifier: License :: OSI Approved
 :: MIT License Classifier: Programming Language :: Python :: 3.9 Classifier:
 Programming Language :: Python :: 3.10 Classifier: Programming Language ::
```

### Comparing `amino.light.py-0.1.8/amino.light.py.egg-info/SOURCES.txt` & `amino.light.py-0.1.9/amino.light.py.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `amino.light.py-0.1.8/setup.py` & `amino.light.py-0.1.9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -24,15 +24,15 @@
     "augustlight",
     "aminolightpy",
     "amino.py"
 ]
 
 setup(
     name="amino.light.py",
-    version="0.1.8",
+    version="0.1.9",
     url="https://github.com/AugustLigh/AminoLightPy",
     license="MIT",
     description="Best Amino.py alternative",
     author="AugustLight",
     packages=find_packages(),
     install_requires=["requests", "websocket-client"],
     long_description=long_description,
```

