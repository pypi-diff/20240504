# Comparing `tmp/qh3-1.0.4.tar.gz` & `tmp/qh3-1.0.5-pp38-pypy38_pp73-musllinux_1_1_aarch64.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

