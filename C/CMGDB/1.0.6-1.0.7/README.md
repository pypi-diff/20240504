# Comparing `tmp/CMGDB-1.0.6.tar.gz` & `tmp/CMGDB-1.0.7-pp310-pypy310_pp73-manylinux_2_17_i686.manylinux2014_i686.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "CMGDB-1.0.6.tar", last modified: Thu Jan 11 01:09:28 2024, max compression
+Zip archive data, at least v2.0 to extract, compression method=store
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

