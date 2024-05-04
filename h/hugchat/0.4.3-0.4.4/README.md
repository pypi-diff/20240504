# Comparing `tmp/hugchat-0.4.3.tar.gz` & `tmp/hugchat-0.4.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hugchat-0.4.3.tar", last modified: Wed Apr 24 07:29:40 2024, max compression
+gzip compressed data, was "hugchat-0.4.4.tar", last modified: Fri May  3 15:37:32 2024, max compression
```

## Comparing `hugchat-0.4.3.tar` & `hugchat-0.4.4.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 07:29:40.126153 hugchat-0.4.3/
--rw-r--r--   0 runner    (1001) docker     (127)    34523 2024-04-24 07:29:35.000000 hugchat-0.4.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     6804 2024-04-24 07:29:40.122153 hugchat-0.4.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5729 2024-04-24 07:29:35.000000 hugchat-0.4.3/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-24 07:29:40.126153 hugchat-0.4.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1435 2024-04-24 07:29:35.000000 hugchat-0.4.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 07:29:40.122153 hugchat-0.4.3/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 07:29:40.122153 hugchat-0.4.3/src/hugchat/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 07:29:35.000000 hugchat-0.4.3/src/hugchat/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10354 2024-04-24 07:29:35.000000 hugchat-0.4.3/src/hugchat/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)      853 2024-04-24 07:29:35.000000 hugchat-0.4.3/src/hugchat/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)    30223 2024-04-24 07:29:35.000000 hugchat-0.4.3/src/hugchat/hugchat.py
--rw-r--r--   0 runner    (1001) docker     (127)     8643 2024-04-24 07:29:35.000000 hugchat-0.4.3/src/hugchat/login.py
--rw-r--r--   0 runner    (1001) docker     (127)     7570 2024-04-24 07:29:35.000000 hugchat-0.4.3/src/hugchat/message.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 07:29:40.122153 hugchat-0.4.3/src/hugchat/types/
--rw-r--r--   0 runner    (1001) docker     (127)      177 2024-04-24 07:29:35.000000 hugchat-0.4.3/src/hugchat/types/assistant.py
--rw-r--r--   0 runner    (1001) docker     (127)     1004 2024-04-24 07:29:35.000000 hugchat-0.4.3/src/hugchat/types/message.py
--rw-r--r--   0 runner    (1001) docker     (127)      988 2024-04-24 07:29:35.000000 hugchat-0.4.3/src/hugchat/types/model.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 07:29:40.122153 hugchat-0.4.3/src/hugchat.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     6804 2024-04-24 07:29:40.000000 hugchat-0.4.3/src/hugchat.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      423 2024-04-24 07:29:40.000000 hugchat-0.4.3/src/hugchat.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-24 07:29:40.000000 hugchat-0.4.3/src/hugchat.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       27 2024-04-24 07:29:40.000000 hugchat-0.4.3/src/hugchat.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-24 07:29:40.000000 hugchat-0.4.3/src/hugchat.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 15:37:32.706865 hugchat-0.4.4/
+-rw-r--r--   0 runner    (1001) docker     (127)    34523 2024-05-03 15:37:28.000000 hugchat-0.4.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     6804 2024-05-03 15:37:32.706865 hugchat-0.4.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5729 2024-05-03 15:37:28.000000 hugchat-0.4.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-03 15:37:32.706865 hugchat-0.4.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1435 2024-05-03 15:37:28.000000 hugchat-0.4.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 15:37:32.702865 hugchat-0.4.4/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 15:37:32.702865 hugchat-0.4.4/src/hugchat/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 15:37:28.000000 hugchat-0.4.4/src/hugchat/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10354 2024-05-03 15:37:28.000000 hugchat-0.4.4/src/hugchat/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)      853 2024-05-03 15:37:28.000000 hugchat-0.4.4/src/hugchat/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30223 2024-05-03 15:37:28.000000 hugchat-0.4.4/src/hugchat/hugchat.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8696 2024-05-03 15:37:28.000000 hugchat-0.4.4/src/hugchat/login.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7570 2024-05-03 15:37:28.000000 hugchat-0.4.4/src/hugchat/message.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 15:37:32.706865 hugchat-0.4.4/src/hugchat/types/
+-rw-r--r--   0 runner    (1001) docker     (127)      177 2024-05-03 15:37:28.000000 hugchat-0.4.4/src/hugchat/types/assistant.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1004 2024-05-03 15:37:28.000000 hugchat-0.4.4/src/hugchat/types/message.py
+-rw-r--r--   0 runner    (1001) docker     (127)      988 2024-05-03 15:37:28.000000 hugchat-0.4.4/src/hugchat/types/model.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 15:37:32.706865 hugchat-0.4.4/src/hugchat.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6804 2024-05-03 15:37:32.000000 hugchat-0.4.4/src/hugchat.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      423 2024-05-03 15:37:32.000000 hugchat-0.4.4/src/hugchat.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-03 15:37:32.000000 hugchat-0.4.4/src/hugchat.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-05-03 15:37:32.000000 hugchat-0.4.4/src/hugchat.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-03 15:37:32.000000 hugchat-0.4.4/src/hugchat.egg-info/top_level.txt
```

### Comparing `hugchat-0.4.3/LICENSE` & `hugchat-0.4.4/LICENSE`

 * *Files identical despite different names*

### Comparing `hugchat-0.4.3/PKG-INFO` & `hugchat-0.4.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hugchat
-Version: 0.4.3
+Version: 0.4.4
 Summary: A huggingchat python api.
 Home-page: https://github.com/Soulter/hugging-chat-api
 Author: Soulter
 Author-email: 905617992@qq.com
 License: GNU Affero General Public License v3.0
 Project-URL: Bug Report, https://github.com/Soulter/hugging-chat-api/issues
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

### Comparing `hugchat-0.4.3/README.md` & `hugchat-0.4.4/README.md`

 * *Files identical despite different names*

### Comparing `hugchat-0.4.3/setup.py` & `hugchat-0.4.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import find_namespace_packages
 from setuptools import setup
 
 setup(
     name="hugchat",
-    version="0.4.3",
+    version="0.4.4",
     description="A huggingchat python api.",
     long_description=open("README.md", "rt", encoding="utf-8").read(),
     long_description_content_type="text/markdown",
     url="https://github.com/Soulter/hugging-chat-api",
     project_urls={
         "Bug Report": "https://github.com/Soulter/hugging-chat-api/issues"
     },
```

### Comparing `hugchat-0.4.3/src/hugchat/cli.py` & `hugchat-0.4.4/src/hugchat/cli.py`

 * *Files identical despite different names*

### Comparing `hugchat-0.4.3/src/hugchat/exceptions.py` & `hugchat-0.4.4/src/hugchat/exceptions.py`

 * *Files identical despite different names*

### Comparing `hugchat-0.4.3/src/hugchat/hugchat.py` & `hugchat-0.4.4/src/hugchat/hugchat.py`

 * *Files identical despite different names*

### Comparing `hugchat-0.4.3/src/hugchat/login.py` & `hugchat-0.4.4/src/hugchat/login.py`

 * *Files 2% similar despite different names*

```diff
@@ -149,15 +149,16 @@
             raise Exception("wrong username or password")
 
     def _get_auth_url(self):
         url = "https://huggingface.co/chat/login"
         headers = {
             "Referer": "https://huggingface.co/chat/login",
             "User-Agent": self.headers["User-Agent"],
-            "Content-Type": "application/x-www-form-urlencoded"
+            "Content-Type": "application/x-www-form-urlencoded",
+            "Origin": "https://huggingface.co/chat"
         }
         res = self._request_post(url, headers=headers, allow_redirects=False)
         if res.status_code == 200:
             # location = res.headers.get("Location", None)
             location = res.json()["location"]
             if location:
                 return location
```

### Comparing `hugchat-0.4.3/src/hugchat/message.py` & `hugchat-0.4.4/src/hugchat/message.py`

 * *Files identical despite different names*

### Comparing `hugchat-0.4.3/src/hugchat/types/message.py` & `hugchat-0.4.4/src/hugchat/types/message.py`

 * *Files identical despite different names*

### Comparing `hugchat-0.4.3/src/hugchat/types/model.py` & `hugchat-0.4.4/src/hugchat/types/model.py`

 * *Files identical despite different names*

### Comparing `hugchat-0.4.3/src/hugchat.egg-info/PKG-INFO` & `hugchat-0.4.4/src/hugchat.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hugchat
-Version: 0.4.3
+Version: 0.4.4
 Summary: A huggingchat python api.
 Home-page: https://github.com/Soulter/hugging-chat-api
 Author: Soulter
 Author-email: 905617992@qq.com
 License: GNU Affero General Public License v3.0
 Project-URL: Bug Report, https://github.com/Soulter/hugging-chat-api/issues
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

