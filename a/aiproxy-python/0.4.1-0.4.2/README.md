# Comparing `tmp/aiproxy_python-0.4.1-py3-none-any.whl.zip` & `tmp/aiproxy_python-0.4.2-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,18 +1,18 @@
-Zip file size: 30166 bytes, number of entries: 16
--rw-r--r--  2.0 unx      540 b- defN 24-May-02 07:38 aiproxy/__init__.py
+Zip file size: 30353 bytes, number of entries: 16
+-rw-r--r--  2.0 unx      540 b- defN 24-May-03 22:58 aiproxy/__init__.py
 -rw-r--r--  2.0 unx     2414 b- defN 24-May-02 07:38 aiproxy/__main__.py
 -rw-r--r--  2.0 unx     7728 b- defN 24-May-01 13:52 aiproxy/accesslog.py
 -rw-r--r--  2.0 unx     7318 b- defN 24-May-02 06:49 aiproxy/anthropic_claude.py
 -rw-r--r--  2.0 unx     1337 b- defN 23-Dec-08 14:24 aiproxy/azurequeueclient.py
--rw-r--r--  2.0 unx    11199 b- defN 24-May-02 07:38 aiproxy/chatgpt.py
+-rw-r--r--  2.0 unx    13037 b- defN 24-May-03 22:49 aiproxy/chatgpt.py
 -rw-r--r--  2.0 unx    16284 b- defN 23-Dec-11 15:51 aiproxy/claude2.py
 -rw-r--r--  2.0 unx    11392 b- defN 24-May-02 06:49 aiproxy/gemini.py
--rw-r--r--  2.0 unx    21761 b- defN 24-May-02 05:47 aiproxy/httpx_proxy.py
+-rw-r--r--  2.0 unx    21761 b- defN 24-May-03 22:46 aiproxy/httpx_proxy.py
 -rw-r--r--  2.0 unx     2165 b- defN 24-Apr-02 01:14 aiproxy/proxy.py
 -rw-r--r--  2.0 unx      731 b- defN 24-May-01 13:52 aiproxy/queueclient.py
--rw-r--r--  2.0 unx    11324 b- defN 24-May-02 07:39 aiproxy_python-0.4.1.dist-info/LICENSE
--rw-r--r--  2.0 unx    14231 b- defN 24-May-02 07:39 aiproxy_python-0.4.1.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-May-02 07:39 aiproxy_python-0.4.1.dist-info/WHEEL
--rw-r--r--  2.0 unx        8 b- defN 24-May-02 07:39 aiproxy_python-0.4.1.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     1276 b- defN 24-May-02 07:39 aiproxy_python-0.4.1.dist-info/RECORD
-16 files, 109800 bytes uncompressed, 28090 bytes compressed:  74.4%
+-rw-r--r--  2.0 unx    11324 b- defN 24-May-03 22:58 aiproxy_python-0.4.2.dist-info/LICENSE
+-rw-r--r--  2.0 unx    14231 b- defN 24-May-03 22:58 aiproxy_python-0.4.2.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-May-03 22:58 aiproxy_python-0.4.2.dist-info/WHEEL
+-rw-r--r--  2.0 unx        8 b- defN 24-May-03 22:58 aiproxy_python-0.4.2.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     1276 b- defN 24-May-03 22:58 aiproxy_python-0.4.2.dist-info/RECORD
+16 files, 111638 bytes uncompressed, 28277 bytes compressed:  74.7%
```

## zipnote {}

```diff
@@ -27,23 +27,23 @@
 
 Filename: aiproxy/proxy.py
 Comment: 
 
 Filename: aiproxy/queueclient.py
 Comment: 
 
-Filename: aiproxy_python-0.4.1.dist-info/LICENSE
+Filename: aiproxy_python-0.4.2.dist-info/LICENSE
 Comment: 
 
-Filename: aiproxy_python-0.4.1.dist-info/METADATA
+Filename: aiproxy_python-0.4.2.dist-info/METADATA
 Comment: 
 
-Filename: aiproxy_python-0.4.1.dist-info/WHEEL
+Filename: aiproxy_python-0.4.2.dist-info/WHEEL
 Comment: 
 
-Filename: aiproxy_python-0.4.1.dist-info/top_level.txt
+Filename: aiproxy_python-0.4.2.dist-info/top_level.txt
 Comment: 
 
-Filename: aiproxy_python-0.4.1.dist-info/RECORD
+Filename: aiproxy_python-0.4.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## aiproxy/__init__.py

```diff
@@ -1,8 +1,8 @@
-__version__ = "0.4.1"
+__version__ = "0.4.2"
 
 import logging
 
 logger = logging.getLogger("aiproxy")
 logger.setLevel(logging.INFO)
 log_format = logging.Formatter("[%(levelname)s] %(asctime)s : %(message)s")
 streamHandler = logging.StreamHandler()
```

## aiproxy/chatgpt.py

```diff
@@ -287,7 +287,54 @@
     async def parse_request(self, fastapi_request: Request, session: SessionInfo):
         await super().parse_request(fastapi_request, session)
         session.stream = session.request_json.get("stream") is True
 
     def prepare_httpx_request_headers(self, session: SessionInfo):
         super().prepare_httpx_request_headers(session)
         session.request_headers["authorization"] = f"Bearer {self.api_key}"
+
+
+# Reverse proxy application for Azure OpenAI Service API
+class AzureOpenAIProxy(ChatGPTProxy):
+    def __init__(
+        self,
+        *,
+        api_key: str = None,
+        resource_name: str = None,
+        deployment_id: str = None,
+        api_version: str = None,
+        timeout=60.0,
+        request_filters: List[RequestFilterBase] = None,
+        response_filters: List[ResponseFilterBase] = None,
+        request_item_class: type = ChatGPTRequestItem,
+        response_item_class: type = ChatGPTResponseItem,
+        stream_response_item_class: type = ChatGPTStreamResponseItem,
+        error_item_class: type = ChatGPTErrorItem,
+        access_logger_queue: QueueClientBase
+    ):
+        super().__init__(
+            api_key=api_key,
+            timeout=timeout,
+            request_filters=request_filters,
+            response_filters=response_filters,
+            request_item_class=request_item_class,
+            response_item_class=response_item_class,
+            stream_response_item_class=stream_response_item_class,
+            error_item_class=error_item_class,
+            access_logger_queue=access_logger_queue
+        )
+
+        self.api_base_url = "https://{resource_name}.openai.azure.com/openai/deployments/{deployment_id}/chat/completions?api-version={api_version}"
+        self.resource_name = resource_name
+        self.deployment_id = deployment_id
+        self.api_version = api_version
+
+    def prepare_httpx_request_headers(self, session: SessionInfo):
+        super().prepare_httpx_request_headers(session)
+        session.request_headers["api-key"] = self.api_key
+
+    def make_url(self, session: SessionInfo):
+        return self.api_base_url.format(
+            resource_name=self.resource_name,
+            deployment_id=self.deployment_id,
+            api_version=self.api_version
+        )
```

## Comparing `aiproxy_python-0.4.1.dist-info/LICENSE` & `aiproxy_python-0.4.2.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `aiproxy_python-0.4.1.dist-info/METADATA` & `aiproxy_python-0.4.2.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aiproxy-python
-Version: 0.4.1
+Version: 0.4.2
 Summary: 🦉AIProxy is a reverse proxy for ChatGPT API that provides monitoring, logging, and filtering requests and responses.
 Home-page: https://github.com/uezo/aiproxy
 Author: uezo
 Author-email: uezo@uezo.net
 Maintainer: uezo
 Maintainer-email: uezo@uezo.net
 License: Apache v2
```

## Comparing `aiproxy_python-0.4.1.dist-info/RECORD` & `aiproxy_python-0.4.2.dist-info/RECORD`

 * *Files 10% similar despite different names*

```diff
@@ -1,16 +1,16 @@
-aiproxy/__init__.py,sha256=lg46FR7Z2ItcRSIkGwaL1ZUBBbCKWp3bMtLtpkTdxIs,540
+aiproxy/__init__.py,sha256=2Ie1ECHoAH_8EibDC6CPO93hVnAybJvArevl4UF-HtY,540
 aiproxy/__main__.py,sha256=YhGpey2hGBaMaNjrB5tKITdaY2wXFOQaUvnn6m1Z09g,2414
 aiproxy/accesslog.py,sha256=YmpQpOR9vYDkTq32PqiEsIlzxb7rnIetrGd7SJR38tU,7728
 aiproxy/anthropic_claude.py,sha256=4zuX-7Bh3R3BRw6eXJXObr0cPkvjk3nRcHz0UNqm0C4,7318
 aiproxy/azurequeueclient.py,sha256=uhQNH4ZSlUcFppE2_IB7HG0Hsvf2ZqGgrrJ1D1Pheqk,1337
-aiproxy/chatgpt.py,sha256=LWCh-0K1rcahUnrAitXM9YCbIs2Y6I13WHipFEkhUh4,11199
+aiproxy/chatgpt.py,sha256=6DFfzCDuFslL98Srh-kyoMN7ssl2PlXwE2L3CwkLqyM,13037
 aiproxy/claude2.py,sha256=MIhInTap6BQ_8pfKsSt5gCzgRObiaviSHgVaIh35iYU,16284
 aiproxy/gemini.py,sha256=KQImlmeXdwffMfpv_UR2mDozDb9C8YZB9W2fKZ1G_T8,11392
 aiproxy/httpx_proxy.py,sha256=2ptvCeX7cam6_6WHOn2mNHo9YhlG1vIQ-S2yi8hrhI8,21761
 aiproxy/proxy.py,sha256=nUMqvcH0wQQu6OsJpQTNMmIuZ0jVpzzjmOoTMCnUPRk,2165
 aiproxy/queueclient.py,sha256=TKPYRWWmKX-3e0FnMkkiuQOKvjxI-ak8-Q6XrZIJ19Y,731
-aiproxy_python-0.4.1.dist-info/LICENSE,sha256=UOZ1F5fFDe3XXvG4oNnkL1-Ecun7zpHzRxjp-XsMeAo,11324
-aiproxy_python-0.4.1.dist-info/METADATA,sha256=r_vAXc1yPO9UuaFB0mC-3hPFWORTHeGcSiDzxz7ZIMU,14231
-aiproxy_python-0.4.1.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
-aiproxy_python-0.4.1.dist-info/top_level.txt,sha256=QdyikybYJCoUrciRj-u1dOhyN3X7K49bma7UAjrvnmo,8
-aiproxy_python-0.4.1.dist-info/RECORD,,
+aiproxy_python-0.4.2.dist-info/LICENSE,sha256=UOZ1F5fFDe3XXvG4oNnkL1-Ecun7zpHzRxjp-XsMeAo,11324
+aiproxy_python-0.4.2.dist-info/METADATA,sha256=InF3TtEKc-EQR659cDyQs9amEucJcpQLft94jSMBHzQ,14231
+aiproxy_python-0.4.2.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
+aiproxy_python-0.4.2.dist-info/top_level.txt,sha256=QdyikybYJCoUrciRj-u1dOhyN3X7K49bma7UAjrvnmo,8
+aiproxy_python-0.4.2.dist-info/RECORD,,
```

