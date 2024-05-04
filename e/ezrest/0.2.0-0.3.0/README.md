# Comparing `tmp/ezrest-0.2.0.tar.gz` & `tmp/ezrest-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ezrest-0.2.0.tar", last modified: Sun Apr 21 22:00:20 2024, max compression
+gzip compressed data, was "ezrest-0.3.0.tar", last modified: Sat May  4 17:48:31 2024, max compression
```

## Comparing `ezrest-0.2.0.tar` & `ezrest-0.3.0.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxr-x   0 mrf0x     (1000) mrf0x     (1000)        0 2024-04-21 22:00:20.858135 ezrest-0.2.0/
--rw-rw-r--   0 mrf0x     (1000) mrf0x     (1000)     1071 2024-04-08 18:35:44.000000 ezrest-0.2.0/LICENSE
--rw-r--r--   0 mrf0x     (1000) mrf0x     (1000)     4147 2024-04-21 22:00:20.858135 ezrest-0.2.0/PKG-INFO
-drwxrwxr-x   0 mrf0x     (1000) mrf0x     (1000)        0 2024-04-21 22:00:20.854135 ezrest-0.2.0/docs/
--rw-rw-r--   0 mrf0x     (1000) mrf0x     (1000)     1738 2024-04-21 21:39:54.000000 ezrest-0.2.0/docs/README.md
-drwxrwxr-x   0 mrf0x     (1000) mrf0x     (1000)        0 2024-04-21 22:00:20.854135 ezrest-0.2.0/ezrest/
--rw-rw-r--   0 mrf0x     (1000) mrf0x     (1000)       22 2024-04-21 21:39:57.000000 ezrest-0.2.0/ezrest/__init__.py
--rw-rw-r--   0 mrf0x     (1000) mrf0x     (1000)     5360 2024-04-21 18:13:33.000000 ezrest-0.2.0/ezrest/objects.py
--rw-rw-r--   0 mrf0x     (1000) mrf0x     (1000)     9774 2024-04-21 17:03:21.000000 ezrest-0.2.0/ezrest/requests.py
-drwxrwxr-x   0 mrf0x     (1000) mrf0x     (1000)        0 2024-04-21 22:00:20.858135 ezrest-0.2.0/ezrest.egg-info/
--rw-r--r--   0 mrf0x     (1000) mrf0x     (1000)     4147 2024-04-21 22:00:20.000000 ezrest-0.2.0/ezrest.egg-info/PKG-INFO
--rw-rw-r--   0 mrf0x     (1000) mrf0x     (1000)      242 2024-04-21 22:00:20.000000 ezrest-0.2.0/ezrest.egg-info/SOURCES.txt
--rw-rw-r--   0 mrf0x     (1000) mrf0x     (1000)        1 2024-04-21 22:00:20.000000 ezrest-0.2.0/ezrest.egg-info/dependency_links.txt
--rw-rw-r--   0 mrf0x     (1000) mrf0x     (1000)       68 2024-04-21 22:00:20.000000 ezrest-0.2.0/ezrest.egg-info/requires.txt
--rw-rw-r--   0 mrf0x     (1000) mrf0x     (1000)        7 2024-04-21 22:00:20.000000 ezrest-0.2.0/ezrest.egg-info/top_level.txt
--rw-rw-r--   0 mrf0x     (1000) mrf0x     (1000)     1592 2024-04-20 19:15:51.000000 ezrest-0.2.0/pyproject.toml
--rw-rw-r--   0 mrf0x     (1000) mrf0x     (1000)       38 2024-04-21 22:00:20.858135 ezrest-0.2.0/setup.cfg
+drwxrwxr-x   0 mrf0x     (1000) mrf0x     (1000)        0 2024-05-04 17:48:31.806985 ezrest-0.3.0/
+-rw-rw-r--   0 mrf0x     (1000) mrf0x     (1000)     1071 2024-04-08 18:35:44.000000 ezrest-0.3.0/LICENSE
+-rw-r--r--   0 mrf0x     (1000) mrf0x     (1000)     4147 2024-05-04 17:48:31.806985 ezrest-0.3.0/PKG-INFO
+drwxrwxr-x   0 mrf0x     (1000) mrf0x     (1000)        0 2024-05-04 17:48:31.802985 ezrest-0.3.0/docs/
+-rw-rw-r--   0 mrf0x     (1000) mrf0x     (1000)     1738 2024-05-04 17:33:00.000000 ezrest-0.3.0/docs/README.md
+drwxrwxr-x   0 mrf0x     (1000) mrf0x     (1000)        0 2024-05-04 17:48:31.802985 ezrest-0.3.0/ezrest/
+-rw-rw-r--   0 mrf0x     (1000) mrf0x     (1000)       22 2024-05-04 17:33:03.000000 ezrest-0.3.0/ezrest/__init__.py
+-rw-rw-r--   0 mrf0x     (1000) mrf0x     (1000)     5360 2024-04-21 18:13:33.000000 ezrest-0.3.0/ezrest/objects.py
+-rw-rw-r--   0 mrf0x     (1000) mrf0x     (1000)    10819 2024-05-04 17:24:57.000000 ezrest-0.3.0/ezrest/requests.py
+drwxrwxr-x   0 mrf0x     (1000) mrf0x     (1000)        0 2024-05-04 17:48:31.802985 ezrest-0.3.0/ezrest.egg-info/
+-rw-r--r--   0 mrf0x     (1000) mrf0x     (1000)     4147 2024-05-04 17:48:31.000000 ezrest-0.3.0/ezrest.egg-info/PKG-INFO
+-rw-rw-r--   0 mrf0x     (1000) mrf0x     (1000)      242 2024-05-04 17:48:31.000000 ezrest-0.3.0/ezrest.egg-info/SOURCES.txt
+-rw-rw-r--   0 mrf0x     (1000) mrf0x     (1000)        1 2024-05-04 17:48:31.000000 ezrest-0.3.0/ezrest.egg-info/dependency_links.txt
+-rw-rw-r--   0 mrf0x     (1000) mrf0x     (1000)       68 2024-05-04 17:48:31.000000 ezrest-0.3.0/ezrest.egg-info/requires.txt
+-rw-rw-r--   0 mrf0x     (1000) mrf0x     (1000)        7 2024-05-04 17:48:31.000000 ezrest-0.3.0/ezrest.egg-info/top_level.txt
+-rw-rw-r--   0 mrf0x     (1000) mrf0x     (1000)     1592 2024-04-20 19:15:51.000000 ezrest-0.3.0/pyproject.toml
+-rw-rw-r--   0 mrf0x     (1000) mrf0x     (1000)       38 2024-05-04 17:48:31.806985 ezrest-0.3.0/setup.cfg
```

### Comparing `ezrest-0.2.0/LICENSE` & `ezrest-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ezrest-0.2.0/PKG-INFO` & `ezrest-0.3.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ezrest
-Version: 0.2.0
+Version: 0.3.0
 Summary: Modular Python framework for implementing REST API clients
 Author: Jacek Lewański
 License: MIT License
         
         Copyright (c) 2024 Jacek Lewański
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -66,15 +66,15 @@
 ## Installation
 
 **Requirements:** Python 3.8+
 
 ```bash
 pip install ezrest
 # Or by providing specific version:
-pip install ezrest==0.2.0
+pip install ezrest==0.3.0
 ```
 
 ## Usage <!-- {docsify-ignore} -->
 
 Please refer to the [documentation pages](https://nullJaX.github.io/ezrest/#/modules) on how to use this module.
 
 ## Contributing
```

### Comparing `ezrest-0.2.0/docs/README.md` & `ezrest-0.3.0/docs/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 ## Installation
 
 **Requirements:** Python 3.8+
 
 ```bash
 pip install ezrest
 # Or by providing specific version:
-pip install ezrest==0.2.0
+pip install ezrest==0.3.0
 ```
 
 ## Usage <!-- {docsify-ignore} -->
 
 Please refer to the [documentation pages](https://nullJaX.github.io/ezrest/#/modules) on how to use this module.
 
 ## Contributing
```

### Comparing `ezrest-0.2.0/ezrest/objects.py` & `ezrest-0.3.0/ezrest/objects.py`

 * *Files identical despite different names*

### Comparing `ezrest-0.2.0/ezrest/requests.py` & `ezrest-0.3.0/ezrest/requests.py`

 * *Files 10% similar despite different names*

```diff
@@ -25,45 +25,45 @@
     NOTE: To keep your code simple and maintainable, the implementations of
     this class should not define how the resources are converted from and into
     objects/dataclasses. The intended scope of a connector is to provide
     unified interface between client and a server on a request-response level,
     possibly with authentication scheme and error handling.
     """
 
-    def post(self, url: str, *args, **kwargs) -> _ResponseType:
+    def post(self, url: str, **kwargs) -> _ResponseType:
         """Performs HTTP POST request"""
         raise NotImplementedError()
 
-    def get(self, url: str, *args, **kwargs) -> _ResponseType:
+    def get(self, url: str, **kwargs) -> _ResponseType:
         """Performs HTTP GET request"""
         raise NotImplementedError()
 
-    def put(self, url: str, *args, **kwargs) -> _ResponseType:
+    def put(self, url: str, **kwargs) -> _ResponseType:
         """Performs HTTP PUT request"""
         raise NotImplementedError()
 
-    def patch(self, url: str, *args, **kwargs) -> _ResponseType:
+    def patch(self, url: str, **kwargs) -> _ResponseType:
         """Performs HTTP PATCH request"""
         raise NotImplementedError()
 
-    def delete(self, url: str, *args, **kwargs) -> _ResponseType:
+    def delete(self, url: str, **kwargs) -> _ResponseType:
         """Performs HTTP DELETE request"""
         raise NotImplementedError()
 
-    def list(self, url: str, *args, **kwargs) -> Iterator[_ResponseType]:
+    def list(self, url: str, **kwargs) -> Iterator[_ResponseType]:
         """
         Yields items/resources one-by-one for endpoints returning collections
         and/or paginated responses.
 
         Example:
 
-        def list(self, url: str, *args, **kwargs) -> Iterator[ResponseType]:
+        def list(self, url: str, **kwargs) -> Iterator[ResponseType]:
             next_url: str = url
             while next_url:
-                response = self.get(url, *args, **kwargs).json()
+                response = self.get(url, **kwargs).json()
                 for item in response.get("items", []):
                     yield item
                 next_url = response.get("next")
         """
         raise NotImplementedError()
 
 
@@ -86,45 +86,45 @@
     NOTE: To keep your code simple and maintainable, the implementations of
     this class should not define how the resources are converted from and into
     objects/dataclasses. The intended scope of a connector is to provide
     unified interface between client and a server on a request-response level,
     possibly with authentication scheme and error handling.
     """
 
-    async def post(self, url: str, *args, **kwargs) -> _ResponseType:
+    async def post(self, url: str, **kwargs) -> _ResponseType:
         """Performs HTTP POST request"""
         raise NotImplementedError()
 
-    async def get(self, url: str, *args, **kwargs) -> _ResponseType:
+    async def get(self, url: str, **kwargs) -> _ResponseType:
         """Performs HTTP GET request"""
         raise NotImplementedError()
 
-    async def put(self, url: str, *args, **kwargs) -> _ResponseType:
+    async def put(self, url: str, **kwargs) -> _ResponseType:
         """Performs HTTP PUT request"""
         raise NotImplementedError()
 
-    async def patch(self, url: str, *args, **kwargs) -> _ResponseType:
+    async def patch(self, url: str, **kwargs) -> _ResponseType:
         """Performs HTTP PATCH request"""
         raise NotImplementedError()
 
-    async def delete(self, url: str, *args, **kwargs) -> _ResponseType:
+    async def delete(self, url: str, **kwargs) -> _ResponseType:
         """Performs HTTP DELETE request"""
         raise NotImplementedError()
 
-    async def list(self, url: str, *args, **kwargs) -> AsyncIterator[_ResponseType]:
+    async def list(self, url: str, **kwargs) -> AsyncIterator[_ResponseType]:
         """
         Yields items/resources one-by-one for endpoints returning collections
         and/or paginated responses.
 
         Example:
 
-        async def list(self, url: str, *args, **kwargs) -> AsyncIterator[ResponseType]:
+        async def list(self, url: str, **kwargs) -> AsyncIterator[ResponseType]:
             next_url: str = url
             while next_url:
-                response = await self.get(url, *args, **kwargs).json()
+                response = await self.get(url, **kwargs).json()
                 for item in response.get("items", []):
                     yield item
                 next_url = response.get("next")
         """
         raise NotImplementedError()
         yield None  # pragma: no cover # supresses mypy error
 
@@ -145,31 +145,38 @@
     The (Async)Endpoint usage is explained in the following snippet.
     There is no significant difference between synchronous and asynchronous
     version other than the class names used. Each example will generate a
     copy of the (Async)Endpoint with modified URL, but the (Async)Connector
     instance will be shared with the newly created (Async)Endpoint. On each
     (Async)Endpoint one can call methods implemented in the (Async)Connector.
     Note, however, that these methods don't accept URL as the first argument,
-    it is automatically injected. The rest of the arguments are passed through
-    without any modifications.
+    it is automatically injected.
+
+    In case of the endpoints that require multiple identifiers (or other
+    dynamic path contents) to be specified, one can use url_inject positional
+    arguments - the code will use standard str.format() method to inject
+    arguments to the URL before executing the request. The rest of the
+    arguments are passed through without any modifications.
 
     Examples:
 
     base_url = 'http://x.com/'
 
     connector = Connector[Dict[str, Any]] ()
 
     api_root = Endpoint[Dict[str, Any]](base_url, connector)
 
-    api_root                # http://x.com/
-    api_root.posts          # http://x.com/posts
-    api_root.comments[3]    # http://x.com/comments/3
-    api_root["comments"][3] # http://x.com/comments/3
+    api_root                                        # http://x.com/
+    api_root.posts                                  # http://x.com/posts
+    api_root.comments[3]                            # http://x.com/comments/3
+    api_root["comments"][3]                         # http://x.com/comments/3
+    api_root.comments.3                             # Not allowed, 3 is not a string type
 
-    api_root.comments.3     # Not allowed, 3 is not a string type
+    endpoint = api_root.posts["{}"].comments["{}"]  # Prepares URL for injection: http://x.com/posts/{}/comments/{}
+    endpoint.get(5, 3, ...)                         # Performs GET request, injecting 5 and 3 as identifiers: http://x.com/posts/5/comments/3
     """
 
     url: str
     """URL of the current endpoint"""
 
     connector: _ConnectorType
     """Connector instance that is used to perform requests"""
@@ -205,37 +212,44 @@
         """
         Generates new URL with the name of the resource appended at the end
         """
         return f"{self.url}/{str(name)}"
 
     __getattr__ = __getitem__ = _generate_endpoint
 
-    def post(self, *args, **kwargs):
-        """Executes HTTP POST request via connector"""
-        return self.connector.post(self.url, *args, **kwargs)
-
-    def get(self, *args, **kwargs):
-        """Executes HTTP GET request via connector"""
-        return self.connector.get(self.url, *args, **kwargs)
-
-    def put(self, *args, **kwargs):
-        """Executes HTTP PUT request via connector"""
-        return self.connector.put(self.url, *args, **kwargs)
-
-    def patch(self, *args, **kwargs):
-        """Executes HTTP PATCH request via connector"""
-        return self.connector.patch(self.url, *args, **kwargs)
-
-    def delete(self, *args, **kwargs):
-        """Executes HTTP DELETE request via connector"""
-        return self.connector.delete(self.url, *args, **kwargs)
-
-    def list(self, *args, **kwargs):
-        """Runs connector's list method to retrieve items one-by-one"""
-        return self.connector.list(self.url, *args, **kwargs)
+    def _compile_url(self, *url_inject) -> str:
+        return self.url.format(*url_inject)
+
+    def _request(self, method: str, *url_inject, **kwargs):
+        """Executes HTTP request via connector and injects URL arguments"""
+        return getattr(self.connector, method)(self._compile_url(*url_inject), **kwargs)
+
+    def post(self, *url_inject, **kwargs):
+        """Executes HTTP POST request via connector and injects URL arguments"""
+        return self._request("post", *url_inject, **kwargs)
+
+    def get(self, *url_inject, **kwargs):
+        """Executes HTTP GET request via connector and injects URL arguments"""
+        return self._request("get", *url_inject, **kwargs)
+
+    def put(self, *url_inject, **kwargs):
+        """Executes HTTP PUT request via connector and injects URL arguments"""
+        return self._request("put", *url_inject, **kwargs)
+
+    def patch(self, *url_inject, **kwargs):
+        """Executes HTTP PATCH request via connector and injects URL arguments"""
+        return self._request("patch", *url_inject, **kwargs)
+
+    def delete(self, *url_inject, **kwargs):
+        """Executes HTTP DELETE request via connector and injects URL arguments"""
+        return self._request("delete", *url_inject, **kwargs)
+
+    def list(self, *url_inject, **kwargs):
+        """Runs connector's list method to retrieve items one-by-one and injects URL arguments"""
+        return self._request("list", *url_inject, **kwargs)
 
 
 # Type aliases that are more convenient to use.
 # If the response type is Dict[str, Any],
 # instantiation will look like this:
 #
 # endpoint = endpoint = Endpoint[Dict[str, Any]](url, Connector())
```

### Comparing `ezrest-0.2.0/ezrest.egg-info/PKG-INFO` & `ezrest-0.3.0/ezrest.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ezrest
-Version: 0.2.0
+Version: 0.3.0
 Summary: Modular Python framework for implementing REST API clients
 Author: Jacek Lewański
 License: MIT License
         
         Copyright (c) 2024 Jacek Lewański
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -66,15 +66,15 @@
 ## Installation
 
 **Requirements:** Python 3.8+
 
 ```bash
 pip install ezrest
 # Or by providing specific version:
-pip install ezrest==0.2.0
+pip install ezrest==0.3.0
 ```
 
 ## Usage <!-- {docsify-ignore} -->
 
 Please refer to the [documentation pages](https://nullJaX.github.io/ezrest/#/modules) on how to use this module.
 
 ## Contributing
```

### Comparing `ezrest-0.2.0/pyproject.toml` & `ezrest-0.3.0/pyproject.toml`

 * *Files identical despite different names*

