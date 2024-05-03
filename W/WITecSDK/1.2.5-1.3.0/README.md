# Comparing `tmp/witecsdk-1.2.5.tar.gz` & `tmp/WITecSDK-1.3.0-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "witecsdk-1.2.5.tar", last modified: Tue Apr 30 10:51:23 2024, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

