# Comparing `tmp/chord_reviews-0.2.0.tar.gz` & `tmp/chord_reviews-0.2.1-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chord_reviews-0.2.0.tar", last modified: Sat May  4 14:10:22 2024, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

