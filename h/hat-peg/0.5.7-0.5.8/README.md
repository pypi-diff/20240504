# Comparing `tmp/hat_peg-0.5.7-cp310.cp311-none-any.whl.zip` & `tmp/hat_peg-0.5.8-cp310.cp311.cp312-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,7 @@
-Zip file size: 10899 bytes, number of entries: 7
--rw-r--r--  2.0 unx    18746 b- defN 23-Jun-23 20:29 hat/peg.py
--rw-r--r--  2.0 unx    11358 b- defN 23-Jun-23 20:43 hat_peg-0.5.7.dist-info/LICENSE
--rw-r--r--  2.0 unx     2248 b- defN 23-Jun-23 20:43 hat_peg-0.5.7.dist-info/METADATA
--rw-r--r--  2.0 unx      114 b- defN 23-Jun-23 20:43 hat_peg-0.5.7.dist-info/WHEEL
--rw-r--r--  2.0 unx        4 b- defN 23-Jun-23 20:43 hat_peg-0.5.7.dist-info/top_level.txt
--rw-r--r--  2.0 unx        1 b- defN 23-Jun-23 20:43 hat_peg-0.5.7.dist-info/zip-safe
--rw-rw-r--  2.0 unx      541 b- defN 23-Jun-23 20:43 hat_peg-0.5.7.dist-info/RECORD
-7 files, 33012 bytes uncompressed, 9943 bytes compressed:  69.9%
+Zip file size: 10563 bytes, number of entries: 5
+?rw-------  2.0 unx    18719 b- defN 24-May-04 20:56 hat/peg.py
+?rw-------  2.0 unx    11358 b- defN 24-May-04 20:56 hat_peg-0.5.8.dist-info/LICENSE
+?rw-------  2.0 unx     2508 b- defN 24-May-04 20:56 hat_peg-0.5.8.dist-info/METADATA
+?rw-------  2.0 unx      118 b- defN 24-May-04 20:56 hat_peg-0.5.8.dist-info/WHEEL
+?rw-------  2.0 unx      364 b- defN 24-May-04 20:56 hat_peg-0.5.8.dist-info/RECORD
+5 files, 33067 bytes uncompressed, 9897 bytes compressed:  70.1%
```

## zipnote {}

```diff
@@ -1,22 +1,16 @@
 Filename: hat/peg.py
 Comment: 
 
-Filename: hat_peg-0.5.7.dist-info/LICENSE
+Filename: hat_peg-0.5.8.dist-info/LICENSE
 Comment: 
 
-Filename: hat_peg-0.5.7.dist-info/METADATA
+Filename: hat_peg-0.5.8.dist-info/METADATA
 Comment: 
 
-Filename: hat_peg-0.5.7.dist-info/WHEEL
+Filename: hat_peg-0.5.8.dist-info/WHEEL
 Comment: 
 
-Filename: hat_peg-0.5.7.dist-info/top_level.txt
-Comment: 
-
-Filename: hat_peg-0.5.7.dist-info/zip-safe
-Comment: 
-
-Filename: hat_peg-0.5.7.dist-info/RECORD
+Filename: hat_peg-0.5.8.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## hat/peg.py

```diff
@@ -159,15 +159,15 @@
 
 
 class Literal(typing.NamedTuple):
     value: str
 
 
 class Class(typing.NamedTuple):
-    values: typing.List[typing.Union[str, typing.Tuple[str, str]]]
+    values: list[str | tuple[str, str]]
 
 
 class Dot(typing.NamedTuple):
     pass
 
 
 Expression: typing.TypeAlias = (Sequence | Choice | Not | And | OneOrMore |
```

## Comparing `hat_peg-0.5.7.dist-info/LICENSE` & `hat_peg-0.5.8.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `hat_peg-0.5.7.dist-info/METADATA` & `hat_peg-0.5.8.dist-info/METADATA`

 * *Files 16% similar despite different names*

```diff
@@ -1,19 +1,22 @@
 Metadata-Version: 2.1
 Name: hat-peg
-Version: 0.5.7
+Version: 0.5.8
 Summary: Hat PEG parser
-Home-page: https://github.com/hat-open/hat-peg
+Description-Content-Type: text/x-rst
 License: Apache-2.0
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
+Provides-Extra: dev
+Requires-Dist: hat-util ~=0.6.10
+Requires-Dist: hat-doit ~=0.15.13; extra == 'dev'
 Requires-Python: >=3.10
-Description-Content-Type: text/x-rst
-License-File: LICENSE
-Requires-Dist: hat-util (~=0.6.10)
+Project-URL: Homepage, http://hat-open.com
+Project-URL: Repository, https://github.com/hat-open/hat-peg.git
+Project-URL: Documentation, http://hat-peg.hat-open.com
 
 .. _online documentation: https://hat-peg.hat-open.com
 .. _git repository: https://github.com/hat-open/hat-peg.git
 .. _PyPI project: https://pypi.org/project/hat-peg
 .. _pydoit: https://pydoit.org
 .. _Hat Open: https://hat-open.com
 .. _Končar Digital: https://www.koncar.hr/en
@@ -41,20 +44,25 @@
 
     $ pip install hat-peg
 
 
 Build
 -----
 
-Build tool used for `hat-peg` is `pydoit`_. It can be installed together
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
+Build tool used for `hat-peg` is `pydoit`_. For listing available doit tasks,
+use::
 
     $ doit list
 
 Default task::
 
     $ doit
```

