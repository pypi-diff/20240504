# Comparing `tmp/kuzu-0.4.0.tar.gz` & `tmp/kuzu-0.4.1.dev1-cp312-cp312-macosx_11_0_arm64.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kuzu-0.4.0.tar", last modified: Thu May  2 19:55:22 2024, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

