# Comparing `tmp/ACME oneM2M CSE-0.3.0.tar.gz` & `tmp/ACME_oneM2M_CSE-2024.4.8-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/ACME oneM2M CSE-0.3.0.tar", last modified: Thu May  7 11:41:19 2020, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

