# Comparing `tmp/coverage-7.5.0.tar.gz` & `tmp/coverage-7.5.1-cp310-cp310-win32.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "coverage-7.5.0.tar", last modified: Tue Apr 23 17:16:04 2024, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

