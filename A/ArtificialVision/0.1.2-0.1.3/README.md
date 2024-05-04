# Comparing `tmp/ArtificialVision-0.1.2.tar.gz` & `tmp/ArtificialVision-0.1.3-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/Users/hwk06023/Desktop/Git/ArtificialVision/dist/.tmp-lv_ru9pu/ArtificialVision-0.1.2.tar", last modified: Sun Feb 25 08:27:02 2024, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

