# Comparing `tmp/mikrotik-bt5-0.0.2b2.tar.gz` & `tmp/mikrotik-bt5-0.0.2b3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mikrotik-bt5-0.0.2b2.tar", last modified: Fri May  3 10:54:00 2024, max compression
+gzip compressed data, was "mikrotik-bt5-0.0.2b3.tar", last modified: Fri May  3 19:05:36 2024, max compression
```

## Comparing `mikrotik-bt5-0.0.2b2.tar` & `mikrotik-bt5-0.0.2b3.tar`

### file list

```diff
@@ -1,14 +1,15 @@
-drwxr-xr-x   0 pi        (1000) pi        (1000)        0 2024-05-03 10:54:00.425855 mikrotik-bt5-0.0.2b2/
--rw-r--r--   0 pi        (1000) pi        (1000)      868 2024-05-03 10:54:00.421855 mikrotik-bt5-0.0.2b2/PKG-INFO
--rw-r--r--   0 pi        (1000) pi        (1000)      501 2024-05-03 08:43:20.000000 mikrotik-bt5-0.0.2b2/README.md
-drwxr-xr-x   0 pi        (1000) pi        (1000)        0 2024-05-03 10:54:00.409855 mikrotik-bt5-0.0.2b2/mikrotik_bt5/
--rw-r--r--   0 pi        (1000) pi        (1000)       83 2024-05-03 10:53:42.000000 mikrotik-bt5-0.0.2b2/mikrotik_bt5/__init__.py
--rw-r--r--   0 pi        (1000) pi        (1000)     4615 2024-05-03 10:53:42.000000 mikrotik-bt5-0.0.2b2/mikrotik_bt5/client.py
-drwxr-xr-x   0 pi        (1000) pi        (1000)        0 2024-05-03 10:54:00.417855 mikrotik-bt5-0.0.2b2/mikrotik_bt5.egg-info/
--rw-r--r--   0 pi        (1000) pi        (1000)      868 2024-05-03 10:53:59.000000 mikrotik-bt5-0.0.2b2/mikrotik_bt5.egg-info/PKG-INFO
--rw-r--r--   0 pi        (1000) pi        (1000)      245 2024-05-03 10:53:59.000000 mikrotik-bt5-0.0.2b2/mikrotik_bt5.egg-info/SOURCES.txt
--rw-r--r--   0 pi        (1000) pi        (1000)        1 2024-05-03 10:53:59.000000 mikrotik-bt5-0.0.2b2/mikrotik_bt5.egg-info/dependency_links.txt
--rw-r--r--   0 pi        (1000) pi        (1000)        6 2024-05-03 10:53:59.000000 mikrotik-bt5-0.0.2b2/mikrotik_bt5.egg-info/requires.txt
--rw-r--r--   0 pi        (1000) pi        (1000)       13 2024-05-03 10:53:59.000000 mikrotik-bt5-0.0.2b2/mikrotik_bt5.egg-info/top_level.txt
--rw-r--r--   0 pi        (1000) pi        (1000)       38 2024-05-03 10:54:00.425855 mikrotik-bt5-0.0.2b2/setup.cfg
--rw-r--r--   0 pi        (1000) pi        (1000)      639 2024-05-03 10:53:47.000000 mikrotik-bt5-0.0.2b2/setup.py
+drwxr-xr-x   0 pi        (1000) pi        (1000)        0 2024-05-03 19:05:35.980290 mikrotik-bt5-0.0.2b3/
+-rw-r--r--   0 pi        (1000) pi        (1000)      868 2024-05-03 19:05:35.976290 mikrotik-bt5-0.0.2b3/PKG-INFO
+-rw-r--r--   0 pi        (1000) pi        (1000)      501 2024-05-03 08:43:20.000000 mikrotik-bt5-0.0.2b3/README.md
+drwxr-xr-x   0 pi        (1000) pi        (1000)        0 2024-05-03 19:05:35.964290 mikrotik-bt5-0.0.2b3/mikrotik_bt5/
+-rw-r--r--   0 pi        (1000) pi        (1000)       83 2024-05-03 10:53:42.000000 mikrotik-bt5-0.0.2b3/mikrotik_bt5/__init__.py
+-rw-r--r--   0 pi        (1000) pi        (1000)     4772 2024-05-03 18:57:36.000000 mikrotik-bt5-0.0.2b3/mikrotik_bt5/client.py
+-rw-r--r--   0 pi        (1000) pi        (1000)     1168 2024-05-03 18:57:52.000000 mikrotik-bt5-0.0.2b3/mikrotik_bt5/test.py
+drwxr-xr-x   0 pi        (1000) pi        (1000)        0 2024-05-03 19:05:35.976290 mikrotik-bt5-0.0.2b3/mikrotik_bt5.egg-info/
+-rw-r--r--   0 pi        (1000) pi        (1000)      868 2024-05-03 19:05:35.000000 mikrotik-bt5-0.0.2b3/mikrotik_bt5.egg-info/PKG-INFO
+-rw-r--r--   0 pi        (1000) pi        (1000)      266 2024-05-03 19:05:35.000000 mikrotik-bt5-0.0.2b3/mikrotik_bt5.egg-info/SOURCES.txt
+-rw-r--r--   0 pi        (1000) pi        (1000)        1 2024-05-03 19:05:35.000000 mikrotik-bt5-0.0.2b3/mikrotik_bt5.egg-info/dependency_links.txt
+-rw-r--r--   0 pi        (1000) pi        (1000)        6 2024-05-03 19:05:35.000000 mikrotik-bt5-0.0.2b3/mikrotik_bt5.egg-info/requires.txt
+-rw-r--r--   0 pi        (1000) pi        (1000)       13 2024-05-03 19:05:35.000000 mikrotik-bt5-0.0.2b3/mikrotik_bt5.egg-info/top_level.txt
+-rw-r--r--   0 pi        (1000) pi        (1000)       38 2024-05-03 19:05:35.980290 mikrotik-bt5-0.0.2b3/setup.cfg
+-rw-r--r--   0 pi        (1000) pi        (1000)      639 2024-05-03 19:05:20.000000 mikrotik-bt5-0.0.2b3/setup.py
```

### Comparing `mikrotik-bt5-0.0.2b2/PKG-INFO` & `mikrotik-bt5-0.0.2b3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mikrotik-bt5
-Version: 0.0.2b2
+Version: 0.0.2b3
 Summary: MikroTik BT5 scanner
 Home-page: https://github.com/Anrijs/MikroTik-BT5-Python
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
```

### Comparing `mikrotik-bt5-0.0.2b2/mikrotik_bt5/client.py` & `mikrotik-bt5-0.0.2b3/mikrotik_bt5/client.py`

 * *Files 3% similar despite different names*

```diff
@@ -34,30 +34,35 @@
             yy = self.y * self.y
             zz = self.z * self.z
 
             ms = math.sqrt(xx + yy + zz)
             return ms
 
     name: str = "MikroTik BT5"
+    address: str | None = None
     version: int | None = None
     udata: int | None = None
     salt: int | None = None
     acceleration: Acceleration | None = None
     temperature: float | None = None
     uptime: int | None = None
     flags: int | None = None
     battery: int | None = None
+    rssi: int | None = None
 
     def __init__(self, device = None, ad_data = None):
         super().__init__(BeaconType.MIKROTIK.value)
 
         if device and ad_data and MikrotikBT5.MIKROTIK_ID in ad_data.manufacturer_data:
             if device.name:
                 self.name = device.name
 
+            self.address = device.address
+            self.rssi = getattr(ad_data, 'rssi', None)
+
             raw_bytes = ad_data.manufacturer_data[MikrotikBT5.MIKROTIK_ID]
 
             version = int(raw_bytes[0])
             value_fmt = None
 
             if version == 0:
                 value_fmt = "<BBHhhhbIBB"
```

### Comparing `mikrotik-bt5-0.0.2b2/mikrotik_bt5.egg-info/PKG-INFO` & `mikrotik-bt5-0.0.2b3/mikrotik_bt5.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mikrotik-bt5
-Version: 0.0.2b2
+Version: 0.0.2b3
 Summary: MikroTik BT5 scanner
 Home-page: https://github.com/Anrijs/MikroTik-BT5-Python
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
```

### Comparing `mikrotik-bt5-0.0.2b2/setup.py` & `mikrotik-bt5-0.0.2b3/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="mikrotik-bt5",
-    version="0.0.2b2",
+    version="0.0.2b3",
     description="MikroTik BT5 scanner",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/Anrijs/MikroTik-BT5-Python",
     packages=setuptools.find_packages(),
     classifiers=[
         'Programming Language :: Python',
```

