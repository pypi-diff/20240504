# Comparing `tmp/SparkleLogging-1.0.6.tar.gz` & `tmp/SparkleLogging-1.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "SparkleLogging-1.0.6.tar", last modified: Fri May  3 03:56:55 2024, max compression
+gzip compressed data, was "SparkleLogging-1.0.7.tar", last modified: Fri May  3 04:40:47 2024, max compression
```

## Comparing `SparkleLogging-1.0.6.tar` & `SparkleLogging-1.0.7.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxrwx   0        0        0        0 2024-05-03 03:56:55.313408 SparkleLogging-1.0.6/
--rw-rw-rw-   0        0        0     3015 2024-05-03 03:56:55.312411 SparkleLogging-1.0.6/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-05-03 03:56:55.207569 SparkleLogging-1.0.6/SparkleLogging/
--rw-rw-rw-   0        0        0        0 2024-05-01 12:32:10.000000 SparkleLogging-1.0.6/SparkleLogging/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-03 03:56:55.307422 SparkleLogging-1.0.6/SparkleLogging/plugins/
--rw-rw-rw-   0        0        0      450 2024-02-21 07:45:12.000000 SparkleLogging-1.0.6/SparkleLogging/plugins/DecoratorsTools.py
--rw-rw-rw-   0        0        0     1160 2024-02-20 08:39:34.000000 SparkleLogging-1.0.6/SparkleLogging/plugins/HttpHander.py
--rw-rw-rw-   0        0        0        0 2024-02-20 09:06:56.000000 SparkleLogging-1.0.6/SparkleLogging/plugins/__init__.py
--rw-rw-rw-   0        0        0      954 2024-02-18 04:21:24.000000 SparkleLogging-1.0.6/SparkleLogging/plugins/websocketHander.py
-drwxrwxrwx   0        0        0        0 2024-05-03 03:56:55.310415 SparkleLogging-1.0.6/SparkleLogging/utils/
--rw-rw-rw-   0        0        0        0 2024-04-30 09:33:18.000000 SparkleLogging-1.0.6/SparkleLogging/utils/__init__.py
--rw-rw-rw-   0        0        0      500 2024-05-03 03:54:03.000000 SparkleLogging-1.0.6/SparkleLogging/utils/core.py
--rw-rw-rw-   0        0        0     4725 2024-05-03 03:53:37.000000 SparkleLogging-1.0.6/SparkleLogging/utils/getLog.py
--rw-rw-rw-   0        0        0      372 2024-05-01 05:44:51.000000 SparkleLogging-1.0.6/SparkleLogging/utils/plugins_for_core.py
-drwxrwxrwx   0        0        0        0 2024-05-03 03:56:55.311414 SparkleLogging-1.0.6/SparkleLogging.egg-info/
--rw-rw-rw-   0        0        0     3015 2024-05-03 03:56:54.000000 SparkleLogging-1.0.6/SparkleLogging.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      514 2024-05-03 03:56:55.000000 SparkleLogging-1.0.6/SparkleLogging.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-03 03:56:54.000000 SparkleLogging-1.0.6/SparkleLogging.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       35 2024-05-03 03:56:54.000000 SparkleLogging-1.0.6/SparkleLogging.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2024-05-03 03:56:54.000000 SparkleLogging-1.0.6/SparkleLogging.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-03 03:56:55.313408 SparkleLogging-1.0.6/setup.cfg
--rw-rw-rw-   0        0        0      724 2024-05-03 03:56:41.000000 SparkleLogging-1.0.6/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-03 04:40:47.049697 SparkleLogging-1.0.7/
+-rw-rw-rw-   0        0        0     3015 2024-05-03 04:40:47.047700 SparkleLogging-1.0.7/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-05-03 04:40:47.018613 SparkleLogging-1.0.7/SparkleLogging/
+-rw-rw-rw-   0        0        0        0 2024-05-03 04:38:26.000000 SparkleLogging-1.0.7/SparkleLogging/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-03 04:40:47.043708 SparkleLogging-1.0.7/SparkleLogging/plugins/
+-rw-rw-rw-   0        0        0      450 2024-05-03 04:38:26.000000 SparkleLogging-1.0.7/SparkleLogging/plugins/DecoratorsTools.py
+-rw-rw-rw-   0        0        0     1160 2024-05-03 04:38:26.000000 SparkleLogging-1.0.7/SparkleLogging/plugins/HttpHander.py
+-rw-rw-rw-   0        0        0        0 2024-05-03 04:38:26.000000 SparkleLogging-1.0.7/SparkleLogging/plugins/__init__.py
+-rw-rw-rw-   0        0        0      954 2024-05-03 04:38:26.000000 SparkleLogging-1.0.7/SparkleLogging/plugins/websocketHander.py
+drwxrwxrwx   0        0        0        0 2024-05-03 04:40:47.046704 SparkleLogging-1.0.7/SparkleLogging/utils/
+-rw-rw-rw-   0        0        0        0 2024-05-03 04:38:26.000000 SparkleLogging-1.0.7/SparkleLogging/utils/__init__.py
+-rw-rw-rw-   0        0        0      500 2024-05-03 04:38:26.000000 SparkleLogging-1.0.7/SparkleLogging/utils/core.py
+-rw-rw-rw-   0        0        0     4696 2024-05-03 04:38:26.000000 SparkleLogging-1.0.7/SparkleLogging/utils/getLog.py
+-rw-rw-rw-   0        0        0      372 2024-05-03 04:38:26.000000 SparkleLogging-1.0.7/SparkleLogging/utils/plugins_for_core.py
+drwxrwxrwx   0        0        0        0 2024-05-03 04:40:47.047700 SparkleLogging-1.0.7/SparkleLogging.egg-info/
+-rw-rw-rw-   0        0        0     3015 2024-05-03 04:40:46.000000 SparkleLogging-1.0.7/SparkleLogging.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      514 2024-05-03 04:40:46.000000 SparkleLogging-1.0.7/SparkleLogging.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-03 04:40:46.000000 SparkleLogging-1.0.7/SparkleLogging.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       35 2024-05-03 04:40:46.000000 SparkleLogging-1.0.7/SparkleLogging.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2024-05-03 04:40:46.000000 SparkleLogging-1.0.7/SparkleLogging.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-03 04:40:47.049697 SparkleLogging-1.0.7/setup.cfg
+-rw-rw-rw-   0        0        0      724 2024-05-03 04:40:14.000000 SparkleLogging-1.0.7/setup.py
```

### Comparing `SparkleLogging-1.0.6/PKG-INFO` & `SparkleLogging-1.0.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SparkleLogging
-Version: 1.0.6
+Version: 1.0.7
 Summary: A logging library for Python
 Home-page: https://github.com/KOKOMI12345/SparkleLogging
 Author: 花火official
 Author-email: 3072252442@qq.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `SparkleLogging-1.0.6/SparkleLogging/plugins/HttpHander.py` & `SparkleLogging-1.0.7/SparkleLogging/plugins/HttpHander.py`

 * *Files identical despite different names*

### Comparing `SparkleLogging-1.0.6/SparkleLogging/plugins/websocketHander.py` & `SparkleLogging-1.0.7/SparkleLogging/plugins/websocketHander.py`

 * *Files identical despite different names*

### Comparing `SparkleLogging-1.0.6/SparkleLogging/utils/getLog.py` & `SparkleLogging-1.0.7/SparkleLogging/utils/getLog.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,18 +3,18 @@
 # 建议不要改这个地方
 DEFAUIT_FOMATTER = logging.Formatter(
     fmt='[%(asctime)s.%(msecs)d| %(levelname)-8s |%(threadName)s|%(name)s.%(funcName)s|%(filename)s:%(lineno)d]: %(message)s',
     datefmt='%Y-%m-%d %H:%M:%S'
 )
 
 class LogManager:
-    def __init__(self) -> None:
-        self.public_formatter = DEFAUIT_FOMATTER
+    public_formatter = DEFAUIT_FOMATTER
 
-    def GetLogger(self, log_name: str = "default",
+    @classmethod
+    def GetLogger(cls, log_name: str = "default",
                   setConsoleLevel: int = logging.DEBUG,
                   setFileLevel: int = logging.INFO,
                   setWebsocketLevel: int = logging.INFO,
                   setHTTPLevel: int = logging.INFO,
                   out_to_console: bool = True,
                   web_log_mode: bool = False,
                   WSpost_url: str = "",
@@ -58,15 +58,15 @@
 
             logger.setLevel(setConsoleLevel)
             logger.addHandler(console_handler)
 
         
         file_handler = TimedRotatingFileHandler(f'./logs/{log_name}/{log_name}.log',encoding="utf-8", when='midnight', interval=1, backupCount=7)
         file_handler.setLevel(setFileLevel)
-        file_handler.setFormatter(self.public_formatter)
+        file_handler.setFormatter(cls.public_formatter)
 
         if custom_formatter:
             file_handler.setFormatter(custom_formatter)
 
         # 检查代码是否在异步环境中运行
         if asyncio.iscoroutinefunction(logging.Handler.emit):
             queue = asyncio.Queue()
@@ -76,32 +76,32 @@
             asyncio.ensure_future(queue_listener.start())
         else:
             logger.addHandler(file_handler)
 
         if web_log_mode and WSpost_url:
             websocket_handler = WebsocketHandler(WSpost_url)
             websocket_handler.setLevel(setWebsocketLevel)
-            formatter = self.public_formatter
+            formatter = cls.public_formatter
             if custom_formatter:
                 formatter = custom_formatter
             websocket_handler.setFormatter(formatter)
             logger.addHandler(websocket_handler)
 
         if http_mode and HTTPpost_url:
             # 检查代码是否在异步环境中运行
             if asyncio.iscoroutinefunction(logging.Handler.emit):
                 async_http_hander = AsyncHTTPhandler(HTTPpost_url)
                 async_http_hander.setLevel(setHTTPLevel)
-                formatter = self.public_formatter
+                formatter = cls.public_formatter
                 if custom_formatter:
                     formatter = custom_formatter
                 async_http_hander.setFormatter(formatter)
                 logger.addHandler(async_http_hander)
             http_handler = HTTPhandler(HTTPpost_url)
             http_handler.setLevel(setHTTPLevel)
-            formatter = self.public_formatter
+            formatter = cls.public_formatter
             if custom_formatter:
                 formatter = custom_formatter
             http_handler.setFormatter(formatter)
             logger.addHandler(http_handler)
 
         return logger
```

### Comparing `SparkleLogging-1.0.6/SparkleLogging.egg-info/PKG-INFO` & `SparkleLogging-1.0.7/SparkleLogging.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SparkleLogging
-Version: 1.0.6
+Version: 1.0.7
 Summary: A logging library for Python
 Home-page: https://github.com/KOKOMI12345/SparkleLogging
 Author: 花火official
 Author-email: 3072252442@qq.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `SparkleLogging-1.0.6/SparkleLogging.egg-info/SOURCES.txt` & `SparkleLogging-1.0.7/SparkleLogging.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `SparkleLogging-1.0.6/setup.py` & `SparkleLogging-1.0.7/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='SparkleLogging',
-    version='1.0.6',
+    version='1.0.7',
     packages=find_packages(),
     author='花火official',
     author_email='3072252442@qq.com',
     description='A logging library for Python',
     long_description=open('Readme.md','r',encoding='utf-8').read(),
     long_description_content_type='text/markdown',
     url='https://github.com/KOKOMI12345/SparkleLogging',
```

