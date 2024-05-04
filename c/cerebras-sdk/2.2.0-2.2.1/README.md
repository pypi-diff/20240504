# Comparing `tmp/cerebras_sdk-2.2.0-cp38-none-manylinux2014_x86_64.whl.zip` & `tmp/cerebras_sdk-2.2.1-cp38-none-manylinux2014_x86_64.whl.zip`

## zipinfo {}

```diff
@@ -1,14 +1,14 @@
-Zip file size: 24718 bytes, number of entries: 12
--rw-r--r--  2.0 unx        0 b- defN 24-Mar-30 23:18 cerebras/sdk/__init__.py
--rw-r--r--  2.0 unx      201 b- defN 24-Mar-30 22:04 cerebras/sdk/client/__init__.py
--rw-r--r--  2.0 unx       49 b- defN 24-Mar-30 23:18 cerebras/sdk/client/_version.py
--rw-r--r--  2.0 unx    10548 b- defN 24-Mar-30 22:04 cerebras/sdk/client/debug_util.py
--rw-r--r--  2.0 unx    53757 b- defN 24-Mar-30 22:04 cerebras/sdk/client/sdk_appliance_client.py
--rw-r--r--  2.0 unx     5714 b- defN 24-Mar-30 22:04 cerebras/sdk/client/sdk_appliance_utils.py
--rw-r--r--  2.0 unx    12018 b- defN 24-Mar-30 22:04 cerebras/sdk/client/sdk_utils.py
--rw-r--r--  2.0 unx     1530 b- defN 24-Mar-30 23:18 cerebras_sdk-2.2.0.dist-info/LICENSE
--rw-r--r--  2.0 unx     1559 b- defN 24-Mar-30 23:18 cerebras_sdk-2.2.0.dist-info/METADATA
--rw-r--r--  2.0 unx      110 b- defN 24-Mar-30 23:18 cerebras_sdk-2.2.0.dist-info/WHEEL
--rw-r--r--  2.0 unx        9 b- defN 24-Mar-30 23:18 cerebras_sdk-2.2.0.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     1043 b- defN 24-Mar-30 23:18 cerebras_sdk-2.2.0.dist-info/RECORD
-12 files, 86538 bytes uncompressed, 22944 bytes compressed:  73.5%
+Zip file size: 24715 bytes, number of entries: 12
+-rw-r--r--  2.0 unx        0 b- defN 24-Apr-29 23:36 cerebras/sdk/__init__.py
+-rw-r--r--  2.0 unx      201 b- defN 24-Apr-29 22:18 cerebras/sdk/client/__init__.py
+-rw-r--r--  2.0 unx       49 b- defN 24-Apr-29 23:36 cerebras/sdk/client/_version.py
+-rw-r--r--  2.0 unx    10548 b- defN 24-Apr-29 22:18 cerebras/sdk/client/debug_util.py
+-rw-r--r--  2.0 unx    53757 b- defN 24-Apr-29 22:18 cerebras/sdk/client/sdk_appliance_client.py
+-rw-r--r--  2.0 unx     5714 b- defN 24-Apr-29 22:18 cerebras/sdk/client/sdk_appliance_utils.py
+-rw-r--r--  2.0 unx    12018 b- defN 24-Apr-29 22:18 cerebras/sdk/client/sdk_utils.py
+-rw-r--r--  2.0 unx     1530 b- defN 24-Apr-29 23:36 cerebras_sdk-2.2.1.dist-info/LICENSE
+-rw-r--r--  2.0 unx     1559 b- defN 24-Apr-29 23:36 cerebras_sdk-2.2.1.dist-info/METADATA
+-rw-r--r--  2.0 unx      110 b- defN 24-Apr-29 23:36 cerebras_sdk-2.2.1.dist-info/WHEEL
+-rw-r--r--  2.0 unx        9 b- defN 24-Apr-29 23:36 cerebras_sdk-2.2.1.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx     1043 b- defN 24-Apr-29 23:36 cerebras_sdk-2.2.1.dist-info/RECORD
+12 files, 86538 bytes uncompressed, 22941 bytes compressed:  73.5%
```

## zipnote {}

```diff
@@ -15,23 +15,23 @@
 
 Filename: cerebras/sdk/client/sdk_appliance_utils.py
 Comment: 
 
 Filename: cerebras/sdk/client/sdk_utils.py
 Comment: 
 
-Filename: cerebras_sdk-2.2.0.dist-info/LICENSE
+Filename: cerebras_sdk-2.2.1.dist-info/LICENSE
 Comment: 
 
-Filename: cerebras_sdk-2.2.0.dist-info/METADATA
+Filename: cerebras_sdk-2.2.1.dist-info/METADATA
 Comment: 
 
-Filename: cerebras_sdk-2.2.0.dist-info/WHEEL
+Filename: cerebras_sdk-2.2.1.dist-info/WHEEL
 Comment: 
 
-Filename: cerebras_sdk-2.2.0.dist-info/top_level.txt
+Filename: cerebras_sdk-2.2.1.dist-info/top_level.txt
 Comment: 
 
-Filename: cerebras_sdk-2.2.0.dist-info/RECORD
+Filename: cerebras_sdk-2.2.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## cerebras/sdk/client/_version.py

```diff
@@ -1,2 +1,2 @@
-__version__ = '2.2.0'
-__githash__ = '43cf2d30ea'
+__version__ = '2.2.1'
+__githash__ = 'e594da27f6'
```

## Comparing `cerebras_sdk-2.2.0.dist-info/LICENSE` & `cerebras_sdk-2.2.1.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `cerebras_sdk-2.2.0.dist-info/METADATA` & `cerebras_sdk-2.2.1.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cerebras-sdk
-Version: 2.2.0
+Version: 2.2.1
 Summary: Cerebras Wafer Scale Cluster SDK
 Home-page: https://cerebras.net/
 Author: Cerebras Systems
 Author-email: support@cerebras.net
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
@@ -12,15 +12,15 @@
 Classifier: Topic :: Software Development
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: System :: Hardware
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: cerebras-appliance (==2.2.0)
+Requires-Dist: cerebras-appliance (==2.2.1)
 
 # cerebras_sdk
 
 [![PyPI Version](https://img.shields.io/pypi/v/cerebras_sdk)](https://pypi.org/project/cerebras_sdk/)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/cerebras_sdk)](https://pypi.org/project/cerebras_sdk/)
 [![Discord](https://img.shields.io/discord/1085960591052644463)](https://discord.gg/ZqvYS2e2rY)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/cerebras_sdk)](https://pypi.org/project/cerebras_sdk/#files)
```

## Comparing `cerebras_sdk-2.2.0.dist-info/RECORD` & `cerebras_sdk-2.2.1.dist-info/RECORD`

 * *Files 16% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 cerebras/sdk/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 cerebras/sdk/client/__init__.py,sha256=NUgVWGiuK9fWAG-0OV0DiiHX--t82iCyrduK7ZNyLx8,201
-cerebras/sdk/client/_version.py,sha256=fAiIogmnrXOTXSiCfTcKwkJukQPQe8e3VSUNkEy1kfw,49
+cerebras/sdk/client/_version.py,sha256=YH37mYIccP8GNc6RIHL_4iGl10n2Sh4H3PL6Qyz8-8M,49
 cerebras/sdk/client/debug_util.py,sha256=JqAwSA6M3_p18D5DcDpRLOm3PaKsrJ_Sr9T8ni4S2GA,10548
 cerebras/sdk/client/sdk_appliance_client.py,sha256=MCgaUGhf-1BG3yAaqvxYvOYxDkPj_XMdcp3hPucT2cU,53757
 cerebras/sdk/client/sdk_appliance_utils.py,sha256=uWqEnt_r6AhlV01gEh8BfkRcHkFpnlXsPIPO6SwhYls,5714
 cerebras/sdk/client/sdk_utils.py,sha256=dlkbe9SSgm8ko0UABiZdmpSvo5SQKWSF0hlYGHbBE9E,12018
-cerebras_sdk-2.2.0.dist-info/LICENSE,sha256=KsAlK4tDuwDdMsNJfq1HYb1m7yfRHhF4JcEApxbj0l4,1530
-cerebras_sdk-2.2.0.dist-info/METADATA,sha256=kkXbZJRulztYXtgE502lpw18UpkNLhzcrVbVjPCQRdA,1559
-cerebras_sdk-2.2.0.dist-info/WHEEL,sha256=e5Y3DPYAs-Xadt9xFueu4oLULkV7c1JHxqudwfakJ68,110
-cerebras_sdk-2.2.0.dist-info/top_level.txt,sha256=vMbKLmum4dNIcI_PLO1-YsOVnsjCff3jP2_OJSF3FLE,9
-cerebras_sdk-2.2.0.dist-info/RECORD,,
+cerebras_sdk-2.2.1.dist-info/LICENSE,sha256=KsAlK4tDuwDdMsNJfq1HYb1m7yfRHhF4JcEApxbj0l4,1530
+cerebras_sdk-2.2.1.dist-info/METADATA,sha256=Z4sd-ARiyA1xRZiS-8yvzS5ySQHTvG1lsXCr0WWe_zg,1559
+cerebras_sdk-2.2.1.dist-info/WHEEL,sha256=e5Y3DPYAs-Xadt9xFueu4oLULkV7c1JHxqudwfakJ68,110
+cerebras_sdk-2.2.1.dist-info/top_level.txt,sha256=vMbKLmum4dNIcI_PLO1-YsOVnsjCff3jP2_OJSF3FLE,9
+cerebras_sdk-2.2.1.dist-info/RECORD,,
```

