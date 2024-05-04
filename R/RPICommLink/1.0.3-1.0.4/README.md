# Comparing `tmp/RPICommLink-1.0.3.tar.gz` & `tmp/RPICommLink-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "RPICommLink-1.0.3.tar", last modified: Fri May  3 20:19:42 2024, max compression
+gzip compressed data, was "RPICommLink-1.0.4.tar", last modified: Fri May  3 20:33:46 2024, max compression
```

## Comparing `RPICommLink-1.0.3.tar` & `RPICommLink-1.0.4.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxrwxrwx   0        0        0        0 2024-05-03 20:19:42.929302 RPICommLink-1.0.3/
--rw-rw-rw-   0        0        0     1088 2024-05-03 20:19:42.929302 RPICommLink-1.0.3/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-05-03 20:19:42.909289 RPICommLink-1.0.3/RPICommLink/
--rw-rw-rw-   0        0        0    15143 2024-05-03 20:16:24.000000 RPICommLink-1.0.3/RPICommLink/rpicommlink.py
-drwxrwxrwx   0        0        0        0 2024-05-03 20:19:42.929302 RPICommLink-1.0.3/RPICommLink.egg-info/
--rw-rw-rw-   0        0        0     1088 2024-05-03 20:19:42.000000 RPICommLink-1.0.3/RPICommLink.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      175 2024-05-03 20:19:42.000000 RPICommLink-1.0.3/RPICommLink.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-03 20:19:42.000000 RPICommLink-1.0.3/RPICommLink.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       12 2024-05-03 20:19:42.000000 RPICommLink-1.0.3/RPICommLink.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-03 20:19:42.929302 RPICommLink-1.0.3/setup.cfg
--rw-rw-rw-   0        0        0     1396 2024-05-03 20:17:21.000000 RPICommLink-1.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-03 20:33:46.260286 RPICommLink-1.0.4/
+-rw-rw-rw-   0        0        0     1154 2024-05-03 20:33:46.260286 RPICommLink-1.0.4/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-05-03 20:33:46.239887 RPICommLink-1.0.4/RPICommLink/
+-rw-rw-rw-   0        0        0    15143 2024-05-03 20:16:24.000000 RPICommLink-1.0.4/RPICommLink/rpicommlink.py
+drwxrwxrwx   0        0        0        0 2024-05-03 20:33:46.260286 RPICommLink-1.0.4/RPICommLink.egg-info/
+-rw-rw-rw-   0        0        0     1154 2024-05-03 20:33:45.000000 RPICommLink-1.0.4/RPICommLink.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      175 2024-05-03 20:33:46.000000 RPICommLink-1.0.4/RPICommLink.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-03 20:33:45.000000 RPICommLink-1.0.4/RPICommLink.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       12 2024-05-03 20:33:45.000000 RPICommLink-1.0.4/RPICommLink.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-03 20:33:46.260286 RPICommLink-1.0.4/setup.cfg
+-rw-rw-rw-   0        0        0     1487 2024-05-03 20:33:20.000000 RPICommLink-1.0.4/setup.py
```

### Comparing `RPICommLink-1.0.3/PKG-INFO` & `RPICommLink-1.0.4/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,16 +1,32 @@
 Metadata-Version: 2.1
 Name: RPICommLink
-Version: 1.0.3
+Version: 1.0.4
 Summary: A library for communication on Raspberry Pi
 Author: adixu
 Author-email: adixu7@gmail.com
 
 RPICommLink 是一个用于在不同设备之间建立通信连接的 Python 类。提供了一系列方法使设备能够通过 TCP/IP 协议进行数据交换。灵活的通信设置可以轻松地在设备之间建立通信连接，无论是在局域网内部还是通过互联网。具备完善的错误处理机制及时发现并处理连接中断、超时等异常情况，保证通信的稳定性和可靠性。使用简单易用的接口可以方便地发送和接收数据，无需过多关注底层网络细节，让设备之间的通信变得更加简单和高效。通过 RPICommLink 类，可以实现设备之间的数据交换，为项目提供强大的通信支持。
 
 
 
 
 
 历代版本更新：
+
+
+
+
+
 1.0.2 -优化了函数的命名，发送模块不再进行死循环。
+
+
+
+
+
 1.0.3 -修复了潜在bug，优化了获取IP的方式，现在可以不命名而使用默认设备名称了。添加了中文介绍。
+
+
+
+
+
+1.0.4 -重新了上传中文介绍
```

### Comparing `RPICommLink-1.0.3/RPICommLink/rpicommlink.py` & `RPICommLink-1.0.4/RPICommLink/rpicommlink.py`

 * *Files identical despite different names*

### Comparing `RPICommLink-1.0.3/RPICommLink.egg-info/PKG-INFO` & `RPICommLink-1.0.4/RPICommLink.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,16 +1,32 @@
 Metadata-Version: 2.1
 Name: RPICommLink
-Version: 1.0.3
+Version: 1.0.4
 Summary: A library for communication on Raspberry Pi
 Author: adixu
 Author-email: adixu7@gmail.com
 
 RPICommLink 是一个用于在不同设备之间建立通信连接的 Python 类。提供了一系列方法使设备能够通过 TCP/IP 协议进行数据交换。灵活的通信设置可以轻松地在设备之间建立通信连接，无论是在局域网内部还是通过互联网。具备完善的错误处理机制及时发现并处理连接中断、超时等异常情况，保证通信的稳定性和可靠性。使用简单易用的接口可以方便地发送和接收数据，无需过多关注底层网络细节，让设备之间的通信变得更加简单和高效。通过 RPICommLink 类，可以实现设备之间的数据交换，为项目提供强大的通信支持。
 
 
 
 
 
 历代版本更新：
+
+
+
+
+
 1.0.2 -优化了函数的命名，发送模块不再进行死循环。
+
+
+
+
+
 1.0.3 -修复了潜在bug，优化了获取IP的方式，现在可以不命名而使用默认设备名称了。添加了中文介绍。
+
+
+
+
+
+1.0.4 -重新了上传中文介绍
```

### Comparing `RPICommLink-1.0.3/setup.py` & `RPICommLink-1.0.4/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 from setuptools import setup
 
 setup(
     name='RPICommLink',
-    version='1.0.3',
+    version='1.0.4',
     author='adixu',
     author_email='adixu7@gmail.com',
     description='A library for communication on Raspberry Pi',
     long_description="RPICommLink 是一个用于在不同设备之间建立通信连接的 Python 类。提供了一系列方法使设备能够通过 TCP/IP 协议进行数据交换。"
                      "灵活的通信设置可以轻松地在设备之间建立通信连接，无论是在局域网内部还是通过互联网。"
                      "具备完善的错误处理机制及时发现并处理连接中断、超时等异常情况，保证通信的稳定性和可靠性。"
                      "使用简单易用的接口可以方便地发送和接收数据，无需过多关注底层网络细节，让设备之间的通信变得更加简单和高效。"
                      "通过 RPICommLink 类，可以实现设备之间的数据交换，为项目提供强大的通信支持。"
                      "\n\n\n\n\n\n历代版本更新："
-                     "\n1.0.2 -优化了函数的命名，发送模块不再进行死循环。"
-                     "\n1.0.3 -修复了潜在bug，优化了获取IP的方式，现在可以不命名而使用默认设备名称了。添加了中文介绍。",
+                     "\n\n\n\n\n\n1.0.2 -优化了函数的命名，发送模块不再进行死循环。"
+                     "\n\n\n\n\n\n1.0.3 -修复了潜在bug，优化了获取IP的方式，现在可以不命名而使用默认设备名称了。添加了中文介绍。"
+                     "\n\n\n\n\n\n1.0.4 -重新了上传中文介绍",
     packages=['RPICommLink'],
     install_requires=[],
 )
```

