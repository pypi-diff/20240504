# Comparing `tmp/botocore-a-la-carte-redshift-serverless-1.34.97.tar.gz` & `tmp/botocore_a_la_carte_redshift_serverless-1.34.98-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "botocore-a-la-carte-redshift-serverless-1.34.97.tar", last modified: Fri May  3 01:04:55 2024, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

