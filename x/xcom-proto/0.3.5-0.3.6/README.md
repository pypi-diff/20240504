# Comparing `tmp/xcom_proto-0.3.5.tar.gz` & `tmp/xcom_proto-0.3.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xcom_proto-0.3.5.tar", max compression
+gzip compressed data, was "xcom_proto-0.3.6.tar", max compression
```

## Comparing `xcom_proto-0.3.5.tar` & `xcom_proto-0.3.6.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0    35149 2021-05-28 08:45:09.224099 xcom_proto-0.3.5/LICENSE
--rw-r--r--   0        0        0     6253 2024-02-20 12:29:52.524605 xcom_proto-0.3.5/README.md
--rw-r--r--   0        0        0      557 2024-04-24 13:43:16.528317 xcom_proto-0.3.5/pyproject.toml
--rw-r--r--   0        0        0     2129 2024-02-20 14:54:25.383464 xcom_proto-0.3.5/xcom_proto/XcomAbs.py
--rw-r--r--   0        0        0     4241 2024-02-20 14:57:20.703484 xcom_proto-0.3.5/xcom_proto/XcomLAN.py
--rw-r--r--   0        0        0     1219 2024-04-24 13:23:19.767515 xcom_proto-0.3.5/xcom_proto/XcomRS232.py
--rwxr-xr-x   0        0        0      151 2023-12-01 12:44:46.219550 xcom_proto-0.3.5/xcom_proto/__init__.py
--rw-r--r--   0        0        0     8766 2024-01-31 15:29:29.574821 xcom_proto-0.3.5/xcom_proto/parameters.py
--rw-r--r--   0        0        0     7559 2024-04-24 13:35:45.098869 xcom_proto-0.3.5/xcom_proto/protocol.py
--rw-r--r--   0        0        0     7003 1970-01-01 00:00:00.000000 xcom_proto-0.3.5/PKG-INFO
+-rw-r--r--   0        0        0    35149 2021-05-28 08:45:09.224099 xcom_proto-0.3.6/LICENSE
+-rw-r--r--   0        0        0     6661 2024-05-04 16:44:24.708635 xcom_proto-0.3.6/README.md
+-rw-r--r--   0        0        0      557 2024-05-04 16:35:06.271261 xcom_proto-0.3.6/pyproject.toml
+-rw-r--r--   0        0        0     2129 2024-02-20 14:54:25.383464 xcom_proto-0.3.6/xcom_proto/XcomAbs.py
+-rw-r--r--   0        0        0     4241 2024-02-20 14:57:20.703484 xcom_proto-0.3.6/xcom_proto/XcomLAN.py
+-rw-r--r--   0        0        0     1219 2024-04-24 13:23:19.767515 xcom_proto-0.3.6/xcom_proto/XcomRS232.py
+-rwxr-xr-x   0        0        0      151 2023-12-01 12:44:46.219550 xcom_proto-0.3.6/xcom_proto/__init__.py
+-rw-r--r--   0        0        0     8922 2024-05-04 16:37:15.770370 xcom_proto-0.3.6/xcom_proto/parameters.py
+-rw-r--r--   0        0        0     7492 2024-05-04 16:32:18.155225 xcom_proto-0.3.6/xcom_proto/protocol.py
+-rw-r--r--   0        0        0     7411 1970-01-01 00:00:00.000000 xcom_proto-0.3.6/PKG-INFO
```

### Comparing `xcom_proto-0.3.5/LICENSE` & `xcom_proto-0.3.6/LICENSE`

 * *Files identical despite different names*

### Comparing `xcom_proto-0.3.5/README.md` & `xcom_proto-0.3.6/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -109,15 +109,15 @@
     boostValue = xcom.getValue(param.SMART_BOOST_LIMIT)
     # same as above
 ```
 
 ### Writing values
 
 **IMPORTANT**:
-`setValue()` has an optional named parameter `propertyID` which you can pass either:
+`setValue()` and `setValueByID()` have an optional named parameter `propertyID` which you can pass either:
 
 - `XcomC.QSP_UNSAVED_VALUE`: writes value into RAM only (default when not specified)
 - `XcomC.QSP_VALUE`: writes value into flash memory; **you should write into flash only if you *really* need it, write cycles are limited!**
 
 ```python
 from xcom_proto import XcomP as param
 from xcom_proto import XcomC
@@ -129,17 +129,25 @@
 xcom = XcomLANUDP("192.168.178.110")
 # OR overwriting ports
 xcom = XcomLANUDP("192.168.178.110", dstPort=4002, srcPort=4001)
 
 xcom.setValue(param.SMART_BOOST_LIMIT, 100) # writes into RAM
 xcom.setValue(param.FORCE_NEW_CYCLE, 1, propertyID=XcomC.QSP_VALUE) # writes into flash memory
 
-# using custom dstAddr (can also be used for setValueByID())
+# using custom dstAddr
 xcom.setValue(param.BATTERY_CHARGE_CURR, 2, dstAddr=101) # writes into RAM
 xcom.setValue(param.BATTERY_CHARGE_CURR, 2, dstAddr=101, propertyID=XcomC.QSP_VALUE) # writes into flash memory
+
+# using custom value by ID
+xcom.setValueByID(1107, XcomC.TYPE_FLOAT, 30) # writes into RAM
+xcom.setValueByID(1107, XcomC.TYPE_FLOAT, 30, propertyID=XcomC.QSP_VALUE) # writes into flash memory
+
+# using custom value by ID and dstAddr
+xcom.setValueByID(1107, XcomC.TYPE_FLOAT, 30, dstAddr=101) # writes into RAM
+xcom.setValueByID(1107, XcomC.TYPE_FLOAT, 30, dstAddr=101, propertyID=XcomC.QSP_VALUE) # writes into flash memory
 ```
 
 #### XcomLAN TCP
 
 ```python
 from xcom_proto import XcomP as param
 from xcom_proto import XcomC
```

### Comparing `xcom_proto-0.3.5/pyproject.toml` & `xcom_proto-0.3.6/pyproject.toml`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "xcom_proto"
-version = "0.3.5"
+version = "0.3.6"
 description = "Python library implementing Studer-Innotec Xcom protocol used by Xcom-232i and Xcom-LAN"
 authors = ["zocker_160 <zocker1600@posteo.net>"]
 license = "GPL-3.0-or-later"
 readme = "README.md"
 homepage = "https://github.com/zocker-160/xcom-protocol"
 repository = "https://github.com/zocker-160/xcom-protocol"
```

### Comparing `xcom_proto-0.3.5/xcom_proto/XcomAbs.py` & `xcom_proto-0.3.6/xcom_proto/XcomAbs.py`

 * *Files identical despite different names*

### Comparing `xcom_proto-0.3.5/xcom_proto/XcomLAN.py` & `xcom_proto-0.3.6/xcom_proto/XcomLAN.py`

 * *Files identical despite different names*

### Comparing `xcom_proto-0.3.5/xcom_proto/XcomRS232.py` & `xcom_proto-0.3.6/xcom_proto/XcomRS232.py`

 * *Files identical despite different names*

### Comparing `xcom_proto-0.3.5/xcom_proto/parameters.py` & `xcom_proto-0.3.6/xcom_proto/parameters.py`

 * *Files 2% similar despite different names*

```diff
@@ -166,16 +166,18 @@
 }
 
 ### main parameters
 
 class Dataset:
 
     # Xtender parameters (Writable)
+    MAX_CURR_AC_SOURCE = Datapoint(1107, "MAX_CURR_AC_SOURCE", TYPE_FLOAT)
     SMART_BOOST_ALLOWED = Datapoint(1126, "SMART_BOOST_ALLOWED", TYPE_BOOL)
     BATTERY_CHARGE_CURR = Datapoint(1138, "BATTERY_CHARGE_CURR", TYPE_FLOAT)
+    MAX_GRID_FEEDING_CURR = Datapoint(1523, "MAX_GRID_FEEDING_CURR", TYPE_FLOAT)
     SMART_BOOST_LIMIT = Datapoint(1607, "SMART_BOOST_LIMIT", TYPE_FLOAT)
 
     PARAMS_SAVED_IN_FLASH = Datapoint(1550, "PARAMS_SAVED_IN_FLASH", TYPE_BOOL)
 
     # RCC / Xcom-232i parameters (Not SCOM accessible, do not use)
     USER_LEVEL = Datapoint(5012, "USER_LEVEL", TYPE_SHORT_ENUM)
```

### Comparing `xcom_proto-0.3.5/xcom_proto/protocol.py` & `xcom_proto-0.3.6/xcom_proto/protocol.py`

 * *Files 1% similar despite different names*

```diff
@@ -142,21 +142,19 @@
 
     start_byte: bytes = b'\xAA'
     header: Header
     frame_data: Frame
 
     @staticmethod
     def seekPackageStart(f: BufferedReader) -> bool:
-        while True:
-            byte = f.read(1)
-            if not byte:
-                return False
-            if byte == Package.start_byte:
-                f.seek(-1, 1)
+        while b := f.read(1):
+            if b == Package.start_byte:
                 return True
+        else:
+            return False
 
     @staticmethod
     def parse(f: BufferedReader):
         if not Package.seekPackageStart(f):
             raise AssertionError("empty or invalid package: package start byte not found")
 
         h_raw = f.read(Header.length)
```

### Comparing `xcom_proto-0.3.5/PKG-INFO` & `xcom_proto-0.3.6/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xcom-proto
-Version: 0.3.5
+Version: 0.3.6
 Summary: Python library implementing Studer-Innotec Xcom protocol used by Xcom-232i and Xcom-LAN
 Home-page: https://github.com/zocker-160/xcom-protocol
 License: GPL-3.0-or-later
 Author: zocker_160
 Author-email: zocker1600@posteo.net
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
@@ -127,15 +127,15 @@
     boostValue = xcom.getValue(param.SMART_BOOST_LIMIT)
     # same as above
 ```
 
 ### Writing values
 
 **IMPORTANT**:
-`setValue()` has an optional named parameter `propertyID` which you can pass either:
+`setValue()` and `setValueByID()` have an optional named parameter `propertyID` which you can pass either:
 
 - `XcomC.QSP_UNSAVED_VALUE`: writes value into RAM only (default when not specified)
 - `XcomC.QSP_VALUE`: writes value into flash memory; **you should write into flash only if you *really* need it, write cycles are limited!**
 
 ```python
 from xcom_proto import XcomP as param
 from xcom_proto import XcomC
@@ -147,17 +147,25 @@
 xcom = XcomLANUDP("192.168.178.110")
 # OR overwriting ports
 xcom = XcomLANUDP("192.168.178.110", dstPort=4002, srcPort=4001)
 
 xcom.setValue(param.SMART_BOOST_LIMIT, 100) # writes into RAM
 xcom.setValue(param.FORCE_NEW_CYCLE, 1, propertyID=XcomC.QSP_VALUE) # writes into flash memory
 
-# using custom dstAddr (can also be used for setValueByID())
+# using custom dstAddr
 xcom.setValue(param.BATTERY_CHARGE_CURR, 2, dstAddr=101) # writes into RAM
 xcom.setValue(param.BATTERY_CHARGE_CURR, 2, dstAddr=101, propertyID=XcomC.QSP_VALUE) # writes into flash memory
+
+# using custom value by ID
+xcom.setValueByID(1107, XcomC.TYPE_FLOAT, 30) # writes into RAM
+xcom.setValueByID(1107, XcomC.TYPE_FLOAT, 30, propertyID=XcomC.QSP_VALUE) # writes into flash memory
+
+# using custom value by ID and dstAddr
+xcom.setValueByID(1107, XcomC.TYPE_FLOAT, 30, dstAddr=101) # writes into RAM
+xcom.setValueByID(1107, XcomC.TYPE_FLOAT, 30, dstAddr=101, propertyID=XcomC.QSP_VALUE) # writes into flash memory
 ```
 
 #### XcomLAN TCP
 
 ```python
 from xcom_proto import XcomP as param
 from xcom_proto import XcomC
```

