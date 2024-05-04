# Comparing `tmp/cmgdb-1.0.7.tar.gz` & `tmp/CMGDB-1.0.8-cp38-cp38-macosx_11_0_arm64.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cmgdb-1.0.7.tar", last modified: Fri May  3 21:05:41 2024, max compression
+Zip archive data, at least v2.0 to extract, compression method=store
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

