# Comparing `tmp/neonize-0.0.8.tar.gz` & `tmp/neonize-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "neonize-0.0.8.tar", max compression
+gzip compressed data, was "neonize-0.0.9.tar", max compression
```

## Comparing `neonize-0.0.8.tar` & `neonize-0.0.9.tar`

### file list

```diff
@@ -1,28 +1,28 @@
--rw-r--r--   0        0        0    11357 2024-02-17 14:20:21.278089 neonize-0.0.8/LICENSE
--rw-r--r--   0        0        0     2858 2024-02-17 14:20:21.278089 neonize-0.0.8/README.md
--rw-r--r--   0        0        0      191 2024-02-17 14:20:21.290089 neonize-0.0.8/neonize/__init__.py
--rw-r--r--   0        0        0    14067 2024-02-17 14:20:21.290089 neonize-0.0.8/neonize/_binder.py
--rw-r--r--   0        0        0     3368 2024-02-17 14:20:21.290089 neonize-0.0.8/neonize/builder.py
--rw-r--r--   0        0        0    95882 2024-02-17 14:20:21.290089 neonize-0.0.8/neonize/client.py
--rw-r--r--   0        0        0       66 2024-02-17 14:20:21.290089 neonize-0.0.8/neonize/const.py
--rw-r--r--   0        0        0     1088 2024-02-17 14:20:21.290089 neonize-0.0.8/neonize/download.py
--rw-r--r--   0        0        0     6383 2024-02-17 14:20:21.290089 neonize-0.0.8/neonize/events.py
--rw-r--r--   0        0        0     2848 2024-02-17 14:20:21.290089 neonize-0.0.8/neonize/exc.py
--rw-r--r--   0        0        0    46210 2024-02-17 14:20:21.290089 neonize-0.0.8/neonize/proto/Neonize_pb2.py
--rw-r--r--   0        0        0   167316 2024-02-17 14:20:21.290089 neonize-0.0.8/neonize/proto/Neonize_pb2.pyi
--rw-r--r--   0        0        0       89 2024-02-17 14:20:21.290089 neonize-0.0.8/neonize/proto/__init__.py
--rw-r--r--   0        0        0   167844 2024-02-17 14:20:21.294089 neonize-0.0.8/neonize/proto/def_pb2.py
--rw-r--r--   0        0        0   651575 2024-02-17 14:20:21.294089 neonize-0.0.8/neonize/proto/def_pb2.pyi
--rw-r--r--   0        0        0     1593 2024-02-17 14:20:21.294089 neonize-0.0.8/neonize/types.py
--rw-r--r--   0        0        0     2736 2024-02-17 14:20:21.294089 neonize-0.0.8/neonize/utils/__init__.py
--rw-r--r--   0        0        0     2787 2024-02-17 14:20:21.294089 neonize-0.0.8/neonize/utils/calc.py
--rw-r--r--   0        0        0     4426 2024-02-17 14:20:21.294089 neonize-0.0.8/neonize/utils/enum.py
--rw-r--r--   0        0        0     9370 2024-02-17 14:20:21.294089 neonize-0.0.8/neonize/utils/ffmpeg.py
--rw-r--r--   0        0        0     3022 2024-02-17 14:20:21.294089 neonize-0.0.8/neonize/utils/iofile.py
--rw-r--r--   0        0        0     1042 2024-02-17 14:20:21.294089 neonize-0.0.8/neonize/utils/jid.py
--rw-r--r--   0        0        0      198 2024-02-17 14:20:21.294089 neonize-0.0.8/neonize/utils/log.py
--rw-r--r--   0        0        0     1185 2024-02-17 14:20:21.294089 neonize-0.0.8/neonize/utils/message.py
--rw-r--r--   0        0        0      697 2024-02-17 14:20:21.294089 neonize-0.0.8/neonize/utils/platform.py
--rw-r--r--   0        0        0      382 2024-02-17 14:20:21.294089 neonize-0.0.8/neonize/utils/thumbnail.py
--rw-r--r--   0        0        0     1103 2024-02-17 14:20:34.137954 neonize-0.0.8/pyproject.toml
--rw-r--r--   0        0        0     3745 1970-01-01 00:00:00.000000 neonize-0.0.8/PKG-INFO
+-rw-r--r--   0        0        0    11357 2024-03-03 11:29:40.668507 neonize-0.0.9/LICENSE
+-rw-r--r--   0        0        0     2858 2024-03-03 11:29:40.668507 neonize-0.0.9/README.md
+-rw-r--r--   0        0        0      191 2024-03-03 11:29:40.680507 neonize-0.0.9/neonize/__init__.py
+-rw-r--r--   0        0        0    14119 2024-03-03 11:29:40.680507 neonize-0.0.9/neonize/_binder.py
+-rw-r--r--   0        0        0     3368 2024-03-03 11:29:40.680507 neonize-0.0.9/neonize/builder.py
+-rw-r--r--   0        0        0    95882 2024-03-03 11:29:40.680507 neonize-0.0.9/neonize/client.py
+-rw-r--r--   0        0        0       66 2024-03-03 11:29:40.680507 neonize-0.0.9/neonize/const.py
+-rw-r--r--   0        0        0     1088 2024-03-03 11:29:40.680507 neonize-0.0.9/neonize/download.py
+-rw-r--r--   0        0        0     6383 2024-03-03 11:29:40.680507 neonize-0.0.9/neonize/events.py
+-rw-r--r--   0        0        0     2848 2024-03-03 11:29:40.680507 neonize-0.0.9/neonize/exc.py
+-rw-r--r--   0        0        0    46210 2024-03-03 11:29:40.680507 neonize-0.0.9/neonize/proto/Neonize_pb2.py
+-rw-r--r--   0        0        0   167316 2024-03-03 11:29:40.680507 neonize-0.0.9/neonize/proto/Neonize_pb2.pyi
+-rw-r--r--   0        0        0       89 2024-03-03 11:29:40.680507 neonize-0.0.9/neonize/proto/__init__.py
+-rw-r--r--   0        0        0   167844 2024-03-03 11:29:40.684507 neonize-0.0.9/neonize/proto/def_pb2.py
+-rw-r--r--   0        0        0   651575 2024-03-03 11:29:40.684507 neonize-0.0.9/neonize/proto/def_pb2.pyi
+-rw-r--r--   0        0        0     1593 2024-03-03 11:29:40.684507 neonize-0.0.9/neonize/types.py
+-rw-r--r--   0        0        0     2736 2024-03-03 11:29:40.684507 neonize-0.0.9/neonize/utils/__init__.py
+-rw-r--r--   0        0        0     2787 2024-03-03 11:29:40.684507 neonize-0.0.9/neonize/utils/calc.py
+-rw-r--r--   0        0        0     4426 2024-03-03 11:29:40.684507 neonize-0.0.9/neonize/utils/enum.py
+-rw-r--r--   0        0        0     9370 2024-03-03 11:29:40.684507 neonize-0.0.9/neonize/utils/ffmpeg.py
+-rw-r--r--   0        0        0     3022 2024-03-03 11:29:40.684507 neonize-0.0.9/neonize/utils/iofile.py
+-rw-r--r--   0        0        0     1042 2024-03-03 11:29:40.684507 neonize-0.0.9/neonize/utils/jid.py
+-rw-r--r--   0        0        0      198 2024-03-03 11:29:40.684507 neonize-0.0.9/neonize/utils/log.py
+-rw-r--r--   0        0        0     1185 2024-03-03 11:29:40.684507 neonize-0.0.9/neonize/utils/message.py
+-rw-r--r--   0        0        0      749 2024-03-03 11:29:40.684507 neonize-0.0.9/neonize/utils/platform.py
+-rw-r--r--   0        0        0      382 2024-03-03 11:29:40.684507 neonize-0.0.9/neonize/utils/thumbnail.py
+-rw-r--r--   0        0        0     1103 2024-03-03 11:29:52.768452 neonize-0.0.9/pyproject.toml
+-rw-r--r--   0        0        0     3745 1970-01-01 00:00:00.000000 neonize-0.0.9/PKG-INFO
```

### Comparing `neonize-0.0.8/LICENSE` & `neonize-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `neonize-0.0.8/README.md` & `neonize-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `neonize-0.0.8/neonize/_binder.py` & `neonize-0.0.9/neonize/_binder.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,14 +16,15 @@
 
 
 def load_goneonize():
     while True:
         try:
             gocode = ctypes.CDLL(f"{root_dir}/{generated_name()}")
             gocode.GetVersion.restype = ctypes.c_char_p
+            print(f"{root_dir}/{generated_name()}")
             if gocode.GetVersion().decode() != importlib.metadata.version("neonize"):
                 download()
                 raise Exception("Unmatched version")
             return gocode
         except OSError as e:
             raise e
         except Exception:
```

### Comparing `neonize-0.0.8/neonize/builder.py` & `neonize-0.0.9/neonize/builder.py`

 * *Files identical despite different names*

### Comparing `neonize-0.0.8/neonize/client.py` & `neonize-0.0.9/neonize/client.py`

 * *Files identical despite different names*

### Comparing `neonize-0.0.8/neonize/download.py` & `neonize-0.0.9/neonize/download.py`

 * *Files identical despite different names*

### Comparing `neonize-0.0.8/neonize/events.py` & `neonize-0.0.9/neonize/events.py`

 * *Files identical despite different names*

### Comparing `neonize-0.0.8/neonize/exc.py` & `neonize-0.0.9/neonize/exc.py`

 * *Files identical despite different names*

### Comparing `neonize-0.0.8/neonize/proto/Neonize_pb2.py` & `neonize-0.0.9/neonize/proto/Neonize_pb2.py`

 * *Files identical despite different names*

### Comparing `neonize-0.0.8/neonize/proto/Neonize_pb2.pyi` & `neonize-0.0.9/neonize/proto/Neonize_pb2.pyi`

 * *Files identical despite different names*

### Comparing `neonize-0.0.8/neonize/proto/def_pb2.py` & `neonize-0.0.9/neonize/proto/def_pb2.py`

 * *Files identical despite different names*

### Comparing `neonize-0.0.8/neonize/proto/def_pb2.pyi` & `neonize-0.0.9/neonize/proto/def_pb2.pyi`

 * *Files identical despite different names*

### Comparing `neonize-0.0.8/neonize/types.py` & `neonize-0.0.9/neonize/types.py`

 * *Files identical despite different names*

### Comparing `neonize-0.0.8/neonize/utils/__init__.py` & `neonize-0.0.9/neonize/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `neonize-0.0.8/neonize/utils/calc.py` & `neonize-0.0.9/neonize/utils/calc.py`

 * *Files identical despite different names*

### Comparing `neonize-0.0.8/neonize/utils/enum.py` & `neonize-0.0.9/neonize/utils/enum.py`

 * *Files identical despite different names*

### Comparing `neonize-0.0.8/neonize/utils/ffmpeg.py` & `neonize-0.0.9/neonize/utils/ffmpeg.py`

 * *Files identical despite different names*

### Comparing `neonize-0.0.8/neonize/utils/iofile.py` & `neonize-0.0.9/neonize/utils/iofile.py`

 * *Files identical despite different names*

### Comparing `neonize-0.0.8/neonize/utils/jid.py` & `neonize-0.0.9/neonize/utils/jid.py`

 * *Files identical despite different names*

### Comparing `neonize-0.0.8/neonize/utils/message.py` & `neonize-0.0.9/neonize/utils/message.py`

 * *Files identical despite different names*

### Comparing `neonize-0.0.8/neonize/utils/platform.py` & `neonize-0.0.9/neonize/utils/platform.py`

 * *Files 11% similar despite different names*

```diff
@@ -17,10 +17,12 @@
     if os_name == "windows":
         ext = "dll"
     elif os_name == "linux":
         is_android = "android" in os.popen("uname -a").read().strip().lower()
         if is_android:
             os_name = "android"
         ext = "so"
+    elif os_name == "darwin":
+        ext = "dylib"
     else:
         ext = "so"
     return f"neonize-{os_name}-{arch_name}.{ext}"
```

### Comparing `neonize-0.0.8/pyproject.toml` & `neonize-0.0.9/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "neonize"
-version = "0.0.8"
+version = "0.0.9"
 description = "whatsmeow binder for python"
 authors = ["krypton-byte <rosid6434@gmail.com>"]
 license = "Apache-2.0"
 readme = "README.md"
 exclude = [
     "docs/",
     "goneonize/"
```

### Comparing `neonize-0.0.8/PKG-INFO` & `neonize-0.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neonize
-Version: 0.0.8
+Version: 0.0.9
 Summary: whatsmeow binder for python
 License: Apache-2.0
 Author: krypton-byte
 Author-email: rosid6434@gmail.com
 Requires-Python: >=3.10
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: neonize Version: 0.0.8 Summary: whatsmeow binder
+Metadata-Version: 2.1 Name: neonize Version: 0.0.9 Summary: whatsmeow binder
 for python License: Apache-2.0 Author: krypton-byte Author-email:
 rosid6434@gmail.com Requires-Python: >=3.10 Classifier: License :: OSI Approved
 :: Apache Software License Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
 Language :: Python :: 3.11 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: linkpreview (>=0.8.3,<0.9.0) Requires-Dist: phonenumbers
 (>=8.13.27,<9.0.0) Requires-Dist: pillow (>=10.1.0,<11.0.0) Requires-Dist:
```

