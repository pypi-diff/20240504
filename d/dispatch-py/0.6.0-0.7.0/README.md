# Comparing `tmp/dispatch_py-0.6.0.tar.gz` & `tmp/dispatch_py-0.7.0-cp311-cp311-manylinux_2_17_s390x.manylinux2014_s390x.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dispatch_py-0.6.0.tar", last modified: Tue Apr 23 01:46:46 2024, max compression
+Zip archive data, at least v2.0 to extract, compression method=store
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

