# Comparing `tmp/http-rpc-20240120.tar.gz` & `tmp/http_rpc-20240504.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "http-rpc-20240120.tar", last modified: Sat Jan 20 06:26:25 2024, max compression
+gzip compressed data, was "http_rpc-20240504.tar", last modified: Sat May  4 16:44:16 2024, max compression
```

## Comparing `http-rpc-20240120.tar` & `http_rpc-20240504.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-20 06:26:25.033064 http-rpc-20240120/
--rw-r--r--   0 root         (0) root         (0)     1211 2024-01-06 09:08:43.000000 http-rpc-20240120/LICENSE
--rw-r--r--   0 root         (0) root         (0)      288 2024-01-20 06:26:25.033064 http-rpc-20240120/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       93 2024-01-06 09:08:43.000000 http-rpc-20240120/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-20 06:26:25.032064 http-rpc-20240120/bin/
--rwxr-xr-x   0 root         (0) root         (0)      288 2024-01-20 06:23:44.000000 http-rpc-20240120/bin/httprpc-self-signed
--rwxr-xr-x   0 root         (0) root         (0)     1233 2024-01-06 09:08:43.000000 http-rpc-20240120/bin/httprpc-sign-cert
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-20 06:26:25.032064 http-rpc-20240120/http_rpc.egg-info/
--rw-r--r--   0 root         (0) root         (0)      288 2024-01-20 06:26:25.000000 http-rpc-20240120/http_rpc.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      211 2024-01-20 06:26:25.000000 http-rpc-20240120/http_rpc.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-01-20 06:26:25.000000 http-rpc-20240120/http_rpc.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        8 2024-01-20 06:26:25.000000 http-rpc-20240120/http_rpc.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     9178 2024-01-20 06:25:17.000000 http-rpc-20240120/httprpc.py
--rw-r--r--   0 root         (0) root         (0)       38 2024-01-20 06:26:25.033064 http-rpc-20240120/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      459 2024-01-06 09:18:13.000000 http-rpc-20240120/setup.py
+drwxr-xr-x   0 bhupendra.singh   (502) staff       (20)        0 2024-05-04 16:44:16.159116 http_rpc-20240504/
+-rw-r--r--   0 bhupendra.singh   (502) staff       (20)     1211 2024-01-04 04:00:55.000000 http_rpc-20240504/LICENSE
+-rw-r--r--   0 bhupendra.singh   (502) staff       (20)      288 2024-05-04 16:44:16.158651 http_rpc-20240504/PKG-INFO
+-rw-r--r--   0 bhupendra.singh   (502) staff       (20)       93 2024-01-04 04:00:55.000000 http_rpc-20240504/README.md
+drwxr-xr-x   0 bhupendra.singh   (502) staff       (20)        0 2024-05-04 16:44:16.156914 http_rpc-20240504/bin/
+-rwxr-xr-x   0 bhupendra.singh   (502) staff       (20)      253 2024-05-04 10:47:45.000000 http_rpc-20240504/bin/httprpc-self-signed
+-rwxr-xr-x   0 bhupendra.singh   (502) staff       (20)     1233 2024-01-04 04:00:55.000000 http_rpc-20240504/bin/httprpc-sign-cert
+drwxr-xr-x   0 bhupendra.singh   (502) staff       (20)        0 2024-05-04 16:44:16.158289 http_rpc-20240504/http_rpc.egg-info/
+-rw-r--r--   0 bhupendra.singh   (502) staff       (20)      288 2024-05-04 16:44:16.000000 http_rpc-20240504/http_rpc.egg-info/PKG-INFO
+-rw-r--r--   0 bhupendra.singh   (502) staff       (20)      211 2024-05-04 16:44:16.000000 http_rpc-20240504/http_rpc.egg-info/SOURCES.txt
+-rw-r--r--   0 bhupendra.singh   (502) staff       (20)        1 2024-05-04 16:44:16.000000 http_rpc-20240504/http_rpc.egg-info/dependency_links.txt
+-rw-r--r--   0 bhupendra.singh   (502) staff       (20)        8 2024-05-04 16:44:16.000000 http_rpc-20240504/http_rpc.egg-info/top_level.txt
+-rw-r--r--   0 bhupendra.singh   (502) staff       (20)     9344 2024-05-04 16:36:37.000000 http_rpc-20240504/httprpc.py
+-rw-r--r--   0 bhupendra.singh   (502) staff       (20)       38 2024-05-04 16:44:16.159164 http_rpc-20240504/setup.cfg
+-rw-r--r--   0 bhupendra.singh   (502) staff       (20)      459 2024-05-04 10:45:28.000000 http_rpc-20240504/setup.py
```

### Comparing `http-rpc-20240120/LICENSE` & `http_rpc-20240504/LICENSE`

 * *Files identical despite different names*

### Comparing `http-rpc-20240120/bin/httprpc-sign-cert` & `http_rpc-20240504/bin/httprpc-sign-cert`

 * *Files identical despite different names*

### Comparing `http-rpc-20240120/httprpc.py` & `http_rpc-20240504/httprpc.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,39 +1,29 @@
-import sys
 import ssl
 import gzip
 import time
 import json
 import pickle
 import asyncio
+import logging
+import argparse
 import traceback
+import importlib
 import urllib.parse
-import logging
 from logging import critical as log
 
 
 class Server():
     async def _handler(self, reader, writer):
         peer = None
         count = 1
 
         while True:
-            try:
-                peer = writer.get_extra_info('socket').getpeername()
-                ctx = dict(ip=peer[0])
-
-                cert = writer.get_extra_info('peercert')
-                subject = cert['subject'][0][0][1]
-                ip_list = [y for x, y in cert['subjectAltName']
-                           if 'IP Address' == x]
-
-                if peer[0] in ip_list:
-                    ctx['subject'] = subject
-            except Exception:
-                pass
+            cert = writer.get_extra_info('peercert')
+            peer = writer.get_extra_info('socket').getpeername()
 
             try:
                 line = await reader.readline()
                 p = line.decode().split()[1].strip('/').split('/')
 
                 method = p[0]
                 params = {k.lower(): urllib.parse.unquote(v)
@@ -74,15 +64,23 @@
                     else:
                         params['octets'] = octets
 
             except Exception:
                 return writer.close()
 
             try:
-                octets = await self.methods[method](ctx, **params)
+                if cert and method:
+                    octets = await getattr(self.app, method)(cert, **params)
+                elif cert:
+                    octets = await mtls_echo(cert, **params)
+                elif method:
+                    octets = await getattr(self.app, method)(**params)
+                else:
+                    octets = await tls_echo(**params)
+
                 status = content_type = None
 
                 if type(octets) is bytes:
                     content_type = 'application/octet-stream'
 
                 elif type(octets) is str:
                     octets = octets.encode()
@@ -118,35 +116,33 @@
                 return writer.close()
 
             log(f'{peer} count({count}) status({status}) '
                 f'in_len({length}) out_len({len(octets)}) '
                 f'{method}({", ".join(params.keys())})')
             count += 1
 
-    async def run(self, ip, port, methods, cert=None, cacert=None):
-        self.methods = methods
+    async def run(self, ip, port, app, cert, cacert=None):
+        self.app = app
 
-        ctx = None
-        if cert:
-            if not cacert:
-                cacert = cert
-
-            ctx = ssl.create_default_context(
-                cafile=cacert, purpose=ssl.Purpose.CLIENT_AUTH)
-            ctx.load_cert_chain(cert, cert)
-            ctx.verify_mode = ssl.CERT_OPTIONAL
-            ctx.check_hostname = True
+        if not cacert:
+            cacert = cert
+
+        ctx = ssl.create_default_context(
+            cafile=cacert, purpose=ssl.Purpose.CLIENT_AUTH)
+        ctx.load_cert_chain(cert, cert)
+        ctx.verify_mode = ssl.CERT_OPTIONAL
+        ctx.check_hostname = True
 
         srv = await asyncio.start_server(self._handler, ip, port, ssl=ctx)
         async with srv:
             return await srv.serve_forever()
 
 
-def run(port, handlers, cert=None, cacert=None, ip=None):
-    asyncio.run(Server().run(ip, port, handlers, cert, cacert))
+def run(port, app, cert=None, cacert=None, ip=None):
+    asyncio.run(Server().run(ip, port, app, cert, cacert))
 
 
 class Client():
     def __init__(self, cacert, cert, servers):
         servers = [s.split(':') for s in servers.split(',')]
 
         self.SSL = ssl.create_default_context(
@@ -237,25 +233,34 @@
         for server, (reader, writer) in self.conns.items():
             try:
                 writer.close()
             except Exception:
                 pass
 
 
-async def echo(ctx, obj):
-    return dict(obj=obj, ctx=ctx, time=time.time())
+async def tls_echo(obj):
+    return dict(obj=obj, time=time.time())
+
+
+async def mtls_echo(cert, obj):
+    res = await tls_echo(obj)
+    res['cert'] = cert
+    return res
 
 
 if __name__ == '__main__':
     logging.basicConfig(format='%(asctime)s %(process)d : %(message)s')
 
-    port = int(sys.argv[1])
-    cert = sys.argv[2] if len(sys.argv) > 2 else None
-    proto = 'https' if cert else 'http'
+    G = argparse.ArgumentParser()
+    G.add_argument('--app', help='application module')
+    G.add_argument('--port', type=int, help='port number for server')
+    G.add_argument('--cert', help='certificate path')
+    G.add_argument('--cacert', help='ca certificate path')
+    G = G.parse_args()
 
     log('''echo '{"value": [1, 2, 3, 4]}' | gzip - | '''
-        f'curl -kv --compressed {proto}://localhost:{port}/echo '
+        f'curl -kv --compressed https://localhost:{G.port} '
         '--data-binary @- '
         '-H "content-type: application/json" '
         '-H "content-encoding: gzip"')
 
-    run(port, dict(echo=echo), cert)
+    run(G.port, importlib.import_module(G.app), G.cert, G.cacert)
```

