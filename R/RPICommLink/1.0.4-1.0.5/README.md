# Comparing `tmp/RPICommLink-1.0.4.tar.gz` & `tmp/RPICommLink-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "RPICommLink-1.0.4.tar", last modified: Fri May  3 20:33:46 2024, max compression
+gzip compressed data, was "RPICommLink-1.0.5.tar", last modified: Sat May  4 06:27:41 2024, max compression
```

## Comparing `RPICommLink-1.0.4.tar` & `RPICommLink-1.0.5.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxrwxrwx   0        0        0        0 2024-05-03 20:33:46.260286 RPICommLink-1.0.4/
--rw-rw-rw-   0        0        0     1154 2024-05-03 20:33:46.260286 RPICommLink-1.0.4/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-05-03 20:33:46.239887 RPICommLink-1.0.4/RPICommLink/
--rw-rw-rw-   0        0        0    15143 2024-05-03 20:16:24.000000 RPICommLink-1.0.4/RPICommLink/rpicommlink.py
-drwxrwxrwx   0        0        0        0 2024-05-03 20:33:46.260286 RPICommLink-1.0.4/RPICommLink.egg-info/
--rw-rw-rw-   0        0        0     1154 2024-05-03 20:33:45.000000 RPICommLink-1.0.4/RPICommLink.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      175 2024-05-03 20:33:46.000000 RPICommLink-1.0.4/RPICommLink.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-03 20:33:45.000000 RPICommLink-1.0.4/RPICommLink.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       12 2024-05-03 20:33:45.000000 RPICommLink-1.0.4/RPICommLink.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-03 20:33:46.260286 RPICommLink-1.0.4/setup.cfg
--rw-rw-rw-   0        0        0     1487 2024-05-03 20:33:20.000000 RPICommLink-1.0.4/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-04 06:27:41.092691 RPICommLink-1.0.5/
+-rw-rw-rw-   0        0        0     1280 2024-05-04 06:27:41.091286 RPICommLink-1.0.5/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-05-04 06:27:41.059336 RPICommLink-1.0.5/RPICommLink/
+-rw-rw-rw-   0        0        0    15748 2024-05-04 06:27:14.000000 RPICommLink-1.0.5/RPICommLink/rpicommlink.py
+drwxrwxrwx   0        0        0        0 2024-05-04 06:27:41.089197 RPICommLink-1.0.5/RPICommLink.egg-info/
+-rw-rw-rw-   0        0        0     1280 2024-05-04 06:27:40.000000 RPICommLink-1.0.5/RPICommLink.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      175 2024-05-04 06:27:40.000000 RPICommLink-1.0.5/RPICommLink.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-04 06:27:40.000000 RPICommLink-1.0.5/RPICommLink.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       12 2024-05-04 06:27:40.000000 RPICommLink-1.0.5/RPICommLink.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-04 06:27:41.093019 RPICommLink-1.0.5/setup.cfg
+-rw-rw-rw-   0        0        0     1638 2024-05-04 06:27:14.000000 RPICommLink-1.0.5/setup.py
```

### Comparing `RPICommLink-1.0.4/PKG-INFO` & `RPICommLink-1.0.5/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: RPICommLink
-Version: 1.0.4
+Version: 1.0.5
 Summary: A library for communication on Raspberry Pi
 Author: adixu
 Author-email: adixu7@gmail.com
 
 RPICommLink 是一个用于在不同设备之间建立通信连接的 Python 类。提供了一系列方法使设备能够通过 TCP/IP 协议进行数据交换。灵活的通信设置可以轻松地在设备之间建立通信连接，无论是在局域网内部还是通过互联网。具备完善的错误处理机制及时发现并处理连接中断、超时等异常情况，保证通信的稳定性和可靠性。使用简单易用的接口可以方便地发送和接收数据，无需过多关注底层网络细节，让设备之间的通信变得更加简单和高效。通过 RPICommLink 类，可以实现设备之间的数据交换，为项目提供强大的通信支持。
 
 
@@ -25,8 +25,14 @@
 
 1.0.3 -修复了潜在bug，优化了获取IP的方式，现在可以不命名而使用默认设备名称了。添加了中文介绍。
 
 
 
 
 
-1.0.4 -重新了上传中文介绍
+1.0.4 -重新了上传中文介绍。
+
+
+
+
+
+1.0.5 -修复了无法在无互联网下获取IP的报错，修复了无法同时连接两个服务器的bug。
```

### Comparing `RPICommLink-1.0.4/RPICommLink/rpicommlink.py` & `RPICommLink-1.0.5/RPICommLink/rpicommlink.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import socket
+import sys
 import threading
 import time
 
 
 class RPICommLink:
     def __init__(self, rpi_port: int = 11451, password: str = '88888888'):
         """
@@ -22,15 +23,15 @@
         self.threading_now = []
         self.data_event = threading.Event()
         self.data_event.clear()
         self.rpi_port = rpi_port
         self.password = password
         self.target_name = []
         self.connect_device = []
-        self.send_server_socket = None
+        self._send_server_socket = []
 
     def open(self, device_name: str = 'default', max_connect: int = 0, ip: str = None):
         """打开_server线程的函数
 
         它使用线程来启动服务器是为了实现非阻塞式的服务器启动。如果直接调用 _server 方法而不使用线程，
         那么在服务器启动过程中，主程序会被阻塞，直到服务器关闭或者达到最大连接数为止。
 
@@ -222,22 +223,22 @@
                     if state == 'cjs8e77e':
                         print(f'\033[93mWarning:由于申请密码不正确被拒绝 \033[0m')
                         self.target_name.pop()
                         self.target_name.append(f"{device_name.decode('utf-8')}(密码错误)")
                         sock.close()
                     elif state == 'ng3mxz7g':
                         self.connect_device.append(device_name.decode('utf-8'))
-                        self.send_server_socket = sock
+                        self._send_server_socket.append(sock)
                     elif state == 'ny6cz4ln':
                         print(f'\033[91mError:已达到服务器的设备连接上限 \033[0m')
             return
         except Exception:
             return None
 
-    def connect(self, target_name: str= 'default', subnet_ip: str = None):
+    def connect(self, target_name: str = 'default', subnet_ip: str = None):
         """连接到服务器并尝试与指定设备建立连接的函数。
 
         如果无法构建局域网，请自行修改。
 
         获取本地主机的 IP 地址并构建局域网的子网。
         用线程遍历子网中的所有可能 IP 地址，并尝试连接到每个 IP 地址的指定端口。
         在连接成功时，发送密码给服务器端，并接收服务器返回的设备名称和状态。
@@ -278,28 +279,43 @@
                 print(f'\033[93mError:没有找到{target_name}设备或密码不正确 \033[0m')
 
     def send(self, msg: str):
         """向服务器发送消息的函数
 
         :param msg:发送的信息
         """
-        try:
-            self.send_server_socket.send(msg.encode('utf-8'))
-        except Exception:
-            print('\033[91mError:发送失败！请确认是否有连接服务器 \033[0m')
+        for sock in self._send_server_socket:
+            try:
+                sock.send(msg.encode('utf-8'))
+            except Exception:
+                print('\033[91mError:一个服务器发送失败！请确认是否有连接服务器 \033[0m')
+                self._send_server_socket.remove(sock)
+                if len(self._send_server_socket) == 0:
+                    print('\033[91mError:无服务器连接 \033[0m')
+                    sys.exit()
+
 
 def get_host_ip():
     """
     查询本机IP地址
     :return:本机IP地址
     """
     try:
         sock = socket.socket(socket.AF_INET, socket.SOCK_DGRAM)
         sock.connect(('8.8.8.8', 80))
         ip = sock.getsockname()[0]
         sock.close()
-        return ip
+        if ip is not None:
+            return ip
+        else:
+            ip = socket.gethostbyname(socket.gethostname())
+        if ip != '127.0.0.1':
+            return ip
+        else:
+            print(f'\033[93mWarning：无法通过互联网或自身获取IP，请自行设置IP \033[0m')
+            sys.exit()
     except Exception as e:
         print(e)
 
+
 if __name__ == "__main__":
     pass
```

### Comparing `RPICommLink-1.0.4/RPICommLink.egg-info/PKG-INFO` & `RPICommLink-1.0.5/RPICommLink.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: RPICommLink
-Version: 1.0.4
+Version: 1.0.5
 Summary: A library for communication on Raspberry Pi
 Author: adixu
 Author-email: adixu7@gmail.com
 
 RPICommLink 是一个用于在不同设备之间建立通信连接的 Python 类。提供了一系列方法使设备能够通过 TCP/IP 协议进行数据交换。灵活的通信设置可以轻松地在设备之间建立通信连接，无论是在局域网内部还是通过互联网。具备完善的错误处理机制及时发现并处理连接中断、超时等异常情况，保证通信的稳定性和可靠性。使用简单易用的接口可以方便地发送和接收数据，无需过多关注底层网络细节，让设备之间的通信变得更加简单和高效。通过 RPICommLink 类，可以实现设备之间的数据交换，为项目提供强大的通信支持。
 
 
@@ -25,8 +25,14 @@
 
 1.0.3 -修复了潜在bug，优化了获取IP的方式，现在可以不命名而使用默认设备名称了。添加了中文介绍。
 
 
 
 
 
-1.0.4 -重新了上传中文介绍
+1.0.4 -重新了上传中文介绍。
+
+
+
+
+
+1.0.5 -修复了无法在无互联网下获取IP的报错，修复了无法同时连接两个服务器的bug。
```

### Comparing `RPICommLink-1.0.4/setup.py` & `RPICommLink-1.0.5/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 from setuptools import setup
 
 setup(
     name='RPICommLink',
-    version='1.0.4',
+    version='1.0.5',
     author='adixu',
     author_email='adixu7@gmail.com',
     description='A library for communication on Raspberry Pi',
     long_description="RPICommLink 是一个用于在不同设备之间建立通信连接的 Python 类。提供了一系列方法使设备能够通过 TCP/IP 协议进行数据交换。"
                      "灵活的通信设置可以轻松地在设备之间建立通信连接，无论是在局域网内部还是通过互联网。"
                      "具备完善的错误处理机制及时发现并处理连接中断、超时等异常情况，保证通信的稳定性和可靠性。"
                      "使用简单易用的接口可以方便地发送和接收数据，无需过多关注底层网络细节，让设备之间的通信变得更加简单和高效。"
                      "通过 RPICommLink 类，可以实现设备之间的数据交换，为项目提供强大的通信支持。"
                      "\n\n\n\n\n\n历代版本更新："
                      "\n\n\n\n\n\n1.0.2 -优化了函数的命名，发送模块不再进行死循环。"
                      "\n\n\n\n\n\n1.0.3 -修复了潜在bug，优化了获取IP的方式，现在可以不命名而使用默认设备名称了。添加了中文介绍。"
-                     "\n\n\n\n\n\n1.0.4 -重新了上传中文介绍",
+                     "\n\n\n\n\n\n1.0.4 -重新了上传中文介绍。"
+                     "\n\n\n\n\n\n1.0.5 -修复了无法在无互联网下获取IP的报错，修复了无法同时连接两个服务器的bug。",
     packages=['RPICommLink'],
     install_requires=[],
 )
```

