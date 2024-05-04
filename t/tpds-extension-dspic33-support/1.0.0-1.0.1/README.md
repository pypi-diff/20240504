# Comparing `tmp/tpds_extension_dspic33_support-1.0.0-py3-none-any.whl.zip` & `tmp/tpds_extension_dspic33_support-1.0.1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,12 +1,12 @@
-Zip file size: 833164 bytes, number of entries: 10
--rw-r--r--  2.0 unx       80 b- defN 24-Mar-09 17:13 tpds_extension/dspic33_support/extension.yaml
--rw-r--r--  2.0 unx       38 b- defN 24-Mar-09 17:13 tpds_extension/dspic33_support/setup.py
--rw-r--r--  2.0 unx       21 b- defN 24-Mar-09 17:13 tpds_extension/dspic33_support/version.py
--rw-r--r--  2.0 unx      264 b- defN 24-Mar-09 17:13 tpds_extension/dspic33_support/backend/__init__.py
--rw-r--r--  2.0 unx      543 b- defN 24-Mar-09 17:13 tpds_extension/dspic33_support/backend/boards/DM240001-2.yaml
--rw-r--r--  2.0 unx   830029 b- defN 24-Mar-09 17:13 tpds_extension/dspic33_support/backend/boards/DM240001-2/DM240001-2.png
--rw-r--r--  2.0 unx      800 b- defN 24-Mar-09 17:13 tpds_extension_dspic33_support-1.0.0.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-Mar-09 17:13 tpds_extension_dspic33_support-1.0.0.dist-info/WHEEL
--rw-r--r--  2.0 unx       15 b- defN 24-Mar-09 17:13 tpds_extension_dspic33_support-1.0.0.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     1032 b- defN 24-Mar-09 17:13 tpds_extension_dspic33_support-1.0.0.dist-info/RECORD
-10 files, 832914 bytes uncompressed, 831328 bytes compressed:  0.2%
+Zip file size: 833558 bytes, number of entries: 10
+-rw-r--r--  2.0 unx       75 b- defN 24-May-04 12:21 tpds_extension/dspic33_support/extension.yaml
+-rw-r--r--  2.0 unx       38 b- defN 24-May-04 12:21 tpds_extension/dspic33_support/setup.py
+-rw-r--r--  2.0 unx       21 b- defN 24-May-04 12:21 tpds_extension/dspic33_support/version.py
+-rw-r--r--  2.0 unx      264 b- defN 24-May-04 12:21 tpds_extension/dspic33_support/backend/__init__.py
+-rw-r--r--  2.0 unx      543 b- defN 24-May-04 12:21 tpds_extension/dspic33_support/backend/boards/DM240001-2.yaml
+-rw-r--r--  2.0 unx   830029 b- defN 24-May-04 12:21 tpds_extension/dspic33_support/backend/boards/DM240001-2/DM240001-2.png
+-rw-r--r--  2.0 unx     1510 b- defN 24-May-04 12:21 tpds_extension_dspic33_support-1.0.1.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-May-04 12:21 tpds_extension_dspic33_support-1.0.1.dist-info/WHEEL
+-rw-r--r--  2.0 unx       15 b- defN 24-May-04 12:21 tpds_extension_dspic33_support-1.0.1.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     1033 b- defN 24-May-04 12:21 tpds_extension_dspic33_support-1.0.1.dist-info/RECORD
+10 files, 833620 bytes uncompressed, 831722 bytes compressed:  0.2%
```

## zipnote {}

```diff
@@ -12,20 +12,20 @@
 
 Filename: tpds_extension/dspic33_support/backend/boards/DM240001-2.yaml
 Comment: 
 
 Filename: tpds_extension/dspic33_support/backend/boards/DM240001-2/DM240001-2.png
 Comment: 
 
-Filename: tpds_extension_dspic33_support-1.0.0.dist-info/METADATA
+Filename: tpds_extension_dspic33_support-1.0.1.dist-info/METADATA
 Comment: 
 
-Filename: tpds_extension_dspic33_support-1.0.0.dist-info/WHEEL
+Filename: tpds_extension_dspic33_support-1.0.1.dist-info/WHEEL
 Comment: 
 
-Filename: tpds_extension_dspic33_support-1.0.0.dist-info/top_level.txt
+Filename: tpds_extension_dspic33_support-1.0.1.dist-info/top_level.txt
 Comment: 
 
-Filename: tpds_extension_dspic33_support-1.0.0.dist-info/RECORD
+Filename: tpds_extension_dspic33_support-1.0.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## tpds_extension/dspic33_support/extension.yaml

```diff
@@ -1,7 +1,7 @@
-name: tpds_dspic33_support
+name: dspic33_support
 
 backend:
   path: "backend"
   routers:
     - router
```

## tpds_extension/dspic33_support/version.py

```diff
@@ -1 +1 @@
-__version__ = '1.0.0'
+__version__ = '1.0.1'
```

