# Comparing `tmp/hat_asn1-0.6.6-cp310.cp311-none-any.whl.zip` & `tmp/hat_asn1-0.6.7-cp310.cp311.cp312-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,13 +1,11 @@
-Zip file size: 22864 bytes, number of entries: 11
--rw-r--r--  2.0 unx     8643 b- defN 23-Jun-25 12:49 hat/asn1/__init__.py
--rw-r--r--  2.0 unx    23029 b- defN 23-Jun-25 12:50 hat/asn1/ber.py
--rw-r--r--  2.0 unx     8777 b- defN 23-Jun-25 13:11 hat/asn1/common.py
--rw-r--r--  2.0 unx     4593 b- defN 23-Jun-25 13:11 hat/asn1/doc.py
--rw-r--r--  2.0 unx    41422 b- defN 23-Jun-25 13:12 hat/asn1/parser.py
--rw-r--r--  2.0 unx    11358 b- defN 23-Jun-25 13:12 hat_asn1-0.6.6.dist-info/LICENSE
--rw-r--r--  2.0 unx     2331 b- defN 23-Jun-25 13:12 hat_asn1-0.6.6.dist-info/METADATA
--rw-r--r--  2.0 unx      114 b- defN 23-Jun-25 13:12 hat_asn1-0.6.6.dist-info/WHEEL
--rw-r--r--  2.0 unx        4 b- defN 23-Jun-25 13:12 hat_asn1-0.6.6.dist-info/top_level.txt
--rw-r--r--  2.0 unx        1 b- defN 23-Jun-25 13:12 hat_asn1-0.6.6.dist-info/zip-safe
--rw-rw-r--  2.0 unx      852 b- defN 23-Jun-25 13:12 hat_asn1-0.6.6.dist-info/RECORD
-11 files, 101124 bytes uncompressed, 21440 bytes compressed:  78.8%
+Zip file size: 22521 bytes, number of entries: 9
+?rw-------  2.0 unx    41422 b- defN 24-May-04 20:54 hat/asn1/parser.py
+?rw-------  2.0 unx     8777 b- defN 24-May-04 20:54 hat/asn1/common.py
+?rw-------  2.0 unx    23029 b- defN 24-May-04 20:54 hat/asn1/ber.py
+?rw-------  2.0 unx     4593 b- defN 24-May-04 20:54 hat/asn1/doc.py
+?rw-------  2.0 unx     8643 b- defN 24-May-04 20:54 hat/asn1/__init__.py
+?rw-------  2.0 unx    11358 b- defN 24-May-04 20:54 hat_asn1-0.6.7.dist-info/LICENSE
+?rw-------  2.0 unx     2588 b- defN 24-May-04 20:54 hat_asn1-0.6.7.dist-info/METADATA
+?rw-------  2.0 unx      118 b- defN 24-May-04 20:54 hat_asn1-0.6.7.dist-info/WHEEL
+?rw-------  2.0 unx      673 b- defN 24-May-04 20:54 hat_asn1-0.6.7.dist-info/RECORD
+9 files, 101201 bytes uncompressed, 21391 bytes compressed:  78.9%
```

## zipnote {}

```diff
@@ -1,34 +1,28 @@
-Filename: hat/asn1/__init__.py
-Comment: 
-
-Filename: hat/asn1/ber.py
+Filename: hat/asn1/parser.py
 Comment: 
 
 Filename: hat/asn1/common.py
 Comment: 
 
-Filename: hat/asn1/doc.py
-Comment: 
-
-Filename: hat/asn1/parser.py
+Filename: hat/asn1/ber.py
 Comment: 
 
-Filename: hat_asn1-0.6.6.dist-info/LICENSE
+Filename: hat/asn1/doc.py
 Comment: 
 
-Filename: hat_asn1-0.6.6.dist-info/METADATA
+Filename: hat/asn1/__init__.py
 Comment: 
 
-Filename: hat_asn1-0.6.6.dist-info/WHEEL
+Filename: hat_asn1-0.6.7.dist-info/LICENSE
 Comment: 
 
-Filename: hat_asn1-0.6.6.dist-info/top_level.txt
+Filename: hat_asn1-0.6.7.dist-info/METADATA
 Comment: 
 
-Filename: hat_asn1-0.6.6.dist-info/zip-safe
+Filename: hat_asn1-0.6.7.dist-info/WHEEL
 Comment: 
 
-Filename: hat_asn1-0.6.6.dist-info/RECORD
+Filename: hat_asn1-0.6.7.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `hat_asn1-0.6.6.dist-info/LICENSE` & `hat_asn1-0.6.7.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `hat_asn1-0.6.6.dist-info/METADATA` & `hat_asn1-0.6.7.dist-info/METADATA`

 * *Files 14% similar despite different names*

```diff
@@ -1,21 +1,24 @@
 Metadata-Version: 2.1
 Name: hat-asn1
-Version: 0.6.6
+Version: 0.6.7
 Summary: Hat ASN.1 parser and encoder
-Home-page: https://github.com/hat-open/hat-asn1
+Description-Content-Type: text/x-rst
 License: Apache-2.0
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
+Provides-Extra: dev
+Requires-Dist: hat-json ~=0.5.27
+Requires-Dist: hat-peg ~=0.5.7
+Requires-Dist: hat-util ~=0.6.13
+Requires-Dist: hat-doit ~=0.15.13; extra == 'dev'
 Requires-Python: >=3.10
-Description-Content-Type: text/x-rst
-License-File: LICENSE
-Requires-Dist: hat-json (~=0.5.19)
-Requires-Dist: hat-peg (~=0.5.7)
-Requires-Dist: hat-util (~=0.6.10)
+Project-URL: Homepage, http://hat-open.com
+Project-URL: Repository, https://github.com/hat-open/hat-asn1.git
+Project-URL: Documentation, http://hat-asn1.hat-open.com
 
 .. _online documentation: https://hat-asn1.hat-open.com
 .. _git repository: https://github.com/hat-open/hat-asn1.git
 .. _PyPI project: https://pypi.org/project/hat-asn1
 .. _pydoit: https://pydoit.org
 .. _Hat Open: https://hat-open.com
 .. _Končar Digital: https://www.koncar.hr/en
@@ -43,20 +46,25 @@
 
     $ pip install hat-asn1
 
 
 Build
 -----
 
-Build tool used for `hat-asn1` is `pydoit`_. It can be installed together
-with other python dependencies by running::
+To install editable installation, together with python development
+dependencies, run::
+
+    $ pip install -e '.[dev]'
+
+To install only python development dependencies, run::
 
-    $ pip install -r requirements.pip.dev.txt
+    $ pip install -r requirements.pip.txt
 
-For listing available doit tasks, use::
+Build tool used for `hat-asn1` is `pydoit`_. For listing available doit tasks,
+use::
 
     $ doit list
 
 Default task::
 
     $ doit
 
@@ -74,15 +82,15 @@
 Development of Hat Open and associated repositories is sponsored by
 `Končar Digital`_.
 
 
 License
 -------
 
-Copyright 2020-2023 Hat Open AUTHORS
+Copyright 2020-2024 Hat Open AUTHORS
 
 Licensed under the Apache License, Version 2.0 (the "License");
 you may not use this file except in compliance with the License.
 You may obtain a copy of the License at
 
     http://www.apache.org/licenses/LICENSE-2.0
```

