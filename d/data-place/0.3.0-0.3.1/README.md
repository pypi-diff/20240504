# Comparing `tmp/data-place-0.3.0.tar.gz` & `tmp/data-place-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "data-place-0.3.0.tar", last modified: Fri May  3 15:20:26 2024, max compression
+gzip compressed data, was "data-place-0.3.1.tar", last modified: Fri May  3 15:37:12 2024, max compression
```

## Comparing `data-place-0.3.0.tar` & `data-place-0.3.1.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxrwx   0        0        0        0 2024-05-03 15:20:26.633219 data-place-0.3.0/
--rw-rw-rw-   0        0        0       44 2024-05-03 15:20:26.000000 data-place-0.3.0/MANIFEST.in
--rw-rw-rw-   0        0        0     6073 2024-05-03 15:20:26.631885 data-place-0.3.0/PKG-INFO
--rw-rw-rw-   0        0        0     5156 2024-01-27 16:23:24.000000 data-place-0.3.0/README.md
--rw-rw-rw-   0        0        0     9793 2024-04-19 12:34:18.000000 data-place-0.3.0/build.py
-drwxrwxrwx   0        0        0        0 2024-05-03 15:20:26.631885 data-place-0.3.0/data_place.egg-info/
--rw-rw-rw-   0        0        0     6073 2024-05-03 15:20:26.000000 data-place-0.3.0/data_place.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      403 2024-05-03 15:20:26.000000 data-place-0.3.0/data_place.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-03 15:20:26.000000 data-place-0.3.0/data_place.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       18 2024-05-03 15:20:26.000000 data-place-0.3.0/data_place.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2024-05-03 15:20:26.000000 data-place-0.3.0/data_place.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-05-03 15:20:26.630886 data-place-0.3.0/dataplace/
--rw-rw-rw-   0        0        0      269 2024-01-20 13:15:44.000000 data-place-0.3.0/dataplace/__init__.py
--rw-rw-rw-   0        0        0     1686 2024-05-03 15:13:02.000000 data-place-0.3.0/dataplace/base.py
--rw-rw-rw-   0        0        0     2304 2024-01-27 08:30:20.000000 data-place-0.3.0/dataplace/callback.py
--rw-rw-rw-   0        0        0     3178 2024-05-03 10:26:32.000000 data-place-0.3.0/dataplace/control.py
--rw-rw-rw-   0        0        0     3556 2024-02-11 17:10:37.000000 data-place-0.3.0/dataplace/handler.py
--rw-rw-rw-   0        0        0     2771 2024-01-25 20:35:44.000000 data-place-0.3.0/dataplace/io.py
--rw-rw-rw-   0        0        0     8742 2024-05-03 15:20:22.000000 data-place-0.3.0/dataplace/receive.py
--rw-rw-rw-   0        0        0    11010 2024-05-03 15:20:22.000000 data-place-0.3.0/dataplace/send.py
--rw-rw-rw-   0        0        0     7260 2024-04-27 12:38:35.000000 data-place-0.3.0/dataplace/store.py
--rw-rw-rw-   0        0        0       10 2024-01-20 13:15:44.000000 data-place-0.3.0/requirements.txt
--rw-rw-rw-   0        0        0       42 2024-05-03 15:20:26.633219 data-place-0.3.0/setup.cfg
--rw-rw-rw-   0        0        0     1615 2024-05-03 15:20:22.000000 data-place-0.3.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-03 15:37:12.452220 data-place-0.3.1/
+-rw-rw-rw-   0        0        0       44 2024-05-03 15:37:12.000000 data-place-0.3.1/MANIFEST.in
+-rw-rw-rw-   0        0        0     6073 2024-05-03 15:37:12.450587 data-place-0.3.1/PKG-INFO
+-rw-rw-rw-   0        0        0     5156 2024-01-27 16:23:24.000000 data-place-0.3.1/README.md
+-rw-rw-rw-   0        0        0     9793 2024-04-19 12:34:18.000000 data-place-0.3.1/build.py
+drwxrwxrwx   0        0        0        0 2024-05-03 15:37:12.449587 data-place-0.3.1/data_place.egg-info/
+-rw-rw-rw-   0        0        0     6073 2024-05-03 15:37:12.000000 data-place-0.3.1/data_place.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      403 2024-05-03 15:37:12.000000 data-place-0.3.1/data_place.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-03 15:37:12.000000 data-place-0.3.1/data_place.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       18 2024-05-03 15:37:12.000000 data-place-0.3.1/data_place.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2024-05-03 15:37:12.000000 data-place-0.3.1/data_place.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-03 15:37:12.448606 data-place-0.3.1/dataplace/
+-rw-rw-rw-   0        0        0      269 2024-01-20 13:15:44.000000 data-place-0.3.1/dataplace/__init__.py
+-rw-rw-rw-   0        0        0     1963 2024-05-03 15:37:10.000000 data-place-0.3.1/dataplace/base.py
+-rw-rw-rw-   0        0        0     2304 2024-01-27 08:30:20.000000 data-place-0.3.1/dataplace/callback.py
+-rw-rw-rw-   0        0        0     3178 2024-05-03 10:26:32.000000 data-place-0.3.1/dataplace/control.py
+-rw-rw-rw-   0        0        0     3556 2024-02-11 17:10:37.000000 data-place-0.3.1/dataplace/handler.py
+-rw-rw-rw-   0        0        0     2771 2024-01-25 20:35:44.000000 data-place-0.3.1/dataplace/io.py
+-rw-rw-rw-   0        0        0     8742 2024-05-03 15:20:22.000000 data-place-0.3.1/dataplace/receive.py
+-rw-rw-rw-   0        0        0    11010 2024-05-03 15:20:22.000000 data-place-0.3.1/dataplace/send.py
+-rw-rw-rw-   0        0        0     7260 2024-04-27 12:38:35.000000 data-place-0.3.1/dataplace/store.py
+-rw-rw-rw-   0        0        0       10 2024-01-20 13:15:44.000000 data-place-0.3.1/requirements.txt
+-rw-rw-rw-   0        0        0       42 2024-05-03 15:37:12.452220 data-place-0.3.1/setup.cfg
+-rw-rw-rw-   0        0        0     1615 2024-05-03 15:37:10.000000 data-place-0.3.1/setup.py
```

### Comparing `data-place-0.3.0/PKG-INFO` & `data-place-0.3.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: data-place
-Version: 0.3.0
+Version: 0.3.1
 Summary: A powerfull and flexible framework for designing async socket based data streaming and distribution systems, with automated parsing, dynamic data store and high-level control hooks.
 Home-page: https://github.com/Shahaf-F-S/data-place
 Author: Shahaf Frank-Shapir
 Author-email: shahaffrs@gmail.com
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `data-place-0.3.0/README.md` & `data-place-0.3.1/README.md`

 * *Files identical despite different names*

### Comparing `data-place-0.3.0/build.py` & `data-place-0.3.1/build.py`

 * *Files identical despite different names*

### Comparing `data-place-0.3.0/data_place.egg-info/PKG-INFO` & `data-place-0.3.1/data_place.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: data-place
-Version: 0.3.0
+Version: 0.3.1
 Summary: A powerfull and flexible framework for designing async socket based data streaming and distribution systems, with automated parsing, dynamic data store and high-level control hooks.
 Home-page: https://github.com/Shahaf-F-S/data-place
 Author: Shahaf Frank-Shapir
 Author-email: shahaffrs@gmail.com
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `data-place-0.3.0/dataplace/base.py` & `data-place-0.3.1/dataplace/base.py`

 * *Files 18% similar despite different names*

```diff
@@ -26,14 +26,15 @@
         if callbacks is None:
             callbacks = []
 
         if controllers is None:
             controllers = []
 
         self._connected = False
+        self._closed = False
 
         super().__init__(
             callbacks=callbacks,
             controllers=controllers,
             paused=paused,
             running=running,
             enabled=enabled,
@@ -42,14 +43,19 @@
         )
 
     @property
     def connected(self) -> bool:
 
         return self._connected
 
+    @property
+    def closed(self) -> bool:
+
+        return self._closed
+
     async def send(self, **kwargs) -> None:
 
         pass
 
     async def handle(self, **kwargs) -> None:
 
         pass
@@ -64,17 +70,27 @@
         pass
 
     @abstractmethod
     async def close(self) -> None:
 
         pass
 
+    async def _close(self) -> None:
+
+        await self.close()
+
+        self._closed = True
+
     async def _connect(self) -> None:
 
         await self.connect()
 
         self._connected = True
 
+    async def stop(self) -> None:
+
+        await self._close()
+
     async def start(self) -> None:
 
         if not self.connected:
             await self._connect()
```

### Comparing `data-place-0.3.0/dataplace/callback.py` & `data-place-0.3.1/dataplace/callback.py`

 * *Files identical despite different names*

### Comparing `data-place-0.3.0/dataplace/control.py` & `data-place-0.3.1/dataplace/control.py`

 * *Files identical despite different names*

### Comparing `data-place-0.3.0/dataplace/handler.py` & `data-place-0.3.1/dataplace/handler.py`

 * *Files identical despite different names*

### Comparing `data-place-0.3.0/dataplace/io.py` & `data-place-0.3.1/dataplace/io.py`

 * *Files identical despite different names*

### Comparing `data-place-0.3.0/dataplace/receive.py` & `data-place-0.3.1/dataplace/receive.py`

 * *Files identical despite different names*

### Comparing `data-place-0.3.0/dataplace/send.py` & `data-place-0.3.1/dataplace/send.py`

 * *Files identical despite different names*

### Comparing `data-place-0.3.0/dataplace/store.py` & `data-place-0.3.1/dataplace/store.py`

 * *Files identical despite different names*

### Comparing `data-place-0.3.0/setup.py` & `data-place-0.3.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -18,15 +18,15 @@
             "__pycache__",
             "*.pyc"
         ],
         include=[],
         requirements="requirements.txt",
         dev_requirements="requirements-dev.txt",
         name='data-place',
-        version='0.3.0',
+        version='0.3.1',
         description=(
             "A powerfull and flexible framework for designing async "
             "socket based data streaming and distribution systems, "
             "with automated parsing, dynamic data store and "
             "high-level control hooks."
         ),
         license='MIT',
```

