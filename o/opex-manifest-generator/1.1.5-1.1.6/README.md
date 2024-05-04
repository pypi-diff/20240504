# Comparing `tmp/opex_manifest_generator-1.1.5.tar.gz` & `tmp/opex_manifest_generator-1.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "opex_manifest_generator-1.1.5.tar", last modified: Sun Apr 21 18:50:39 2024, max compression
+gzip compressed data, was "opex_manifest_generator-1.1.6.tar", last modified: Sat May  4 20:41:59 2024, max compression
```

## Comparing `opex_manifest_generator-1.1.5.tar` & `opex_manifest_generator-1.1.6.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxrwxrwx   0        0        0        0 2024-04-21 18:50:39.880282 opex_manifest_generator-1.1.5/
--rw-rw-rw-   0        0        0      124 2024-04-12 13:39:12.000000 opex_manifest_generator-1.1.5/.gitignore
--rw-rw-rw-   0        0        0    11558 2024-02-18 12:39:01.000000 opex_manifest_generator-1.1.5/LICENSE.md
--rw-rw-rw-   0        0        0      701 2024-04-21 18:50:39.880282 opex_manifest_generator-1.1.5/PKG-INFO
--rw-rw-rw-   0        0        0    21573 2024-04-21 18:27:56.000000 opex_manifest_generator-1.1.5/README.md
-drwxrwxrwx   0        0        0        0 2024-04-21 18:50:39.409942 opex_manifest_generator-1.1.5/assets/
--rw-rw-rw-   0        0        0     8271 2024-04-12 14:39:11.000000 opex_manifest_generator-1.1.5/assets/Column Headers.png
--rw-rw-rw-   0        0        0    27359 2024-04-12 14:49:33.000000 opex_manifest_generator-1.1.5/assets/FullName Column.png
--rw-rw-rw-   0        0        0    16064 2024-04-12 14:57:04.000000 opex_manifest_generator-1.1.5/assets/Hash Headers.png
--rw-rw-rw-   0        0        0     4920 2024-04-12 14:58:52.000000 opex_manifest_generator-1.1.5/assets/Identifiers Headers.png
--rw-rw-rw-   0        0        0     2602 2024-04-12 15:01:06.000000 opex_manifest_generator-1.1.5/assets/XML Headers.png
-drwxrwxrwx   0        0        0        0 2024-04-21 18:50:39.499178 opex_manifest_generator-1.1.5/opex_manifest_generator/
--rw-rw-rw-   0        0        0      476 2024-04-21 18:41:39.000000 opex_manifest_generator-1.1.5/opex_manifest_generator/__init__.py
--rw-rw-rw-   0        0        0     6046 2024-04-21 18:36:34.000000 opex_manifest_generator-1.1.5/opex_manifest_generator/cli.py
--rw-rw-rw-   0        0        0      676 2024-04-04 09:48:17.000000 opex_manifest_generator-1.1.5/opex_manifest_generator/common.py
--rw-rw-rw-   0        0        0      966 2024-02-18 22:01:42.000000 opex_manifest_generator-1.1.5/opex_manifest_generator/hash.py
-drwxrwxrwx   0        0        0        0 2024-04-21 18:50:39.717914 opex_manifest_generator-1.1.5/opex_manifest_generator/metadata/
--rw-rw-rw-   0        0        0      775 2023-12-13 09:26:40.000000 opex_manifest_generator-1.1.5/opex_manifest_generator/metadata/DublinCore Template.xml
--rw-rw-rw-   0        0        0     2268 2023-12-13 09:26:40.000000 opex_manifest_generator-1.1.5/opex_manifest_generator/metadata/EAD Template.xml
--rw-rw-rw-   0        0        0      483 2023-12-13 09:26:40.000000 opex_manifest_generator-1.1.5/opex_manifest_generator/metadata/GDPR Template.xml
--rw-rw-rw-   0        0        0     2701 2023-12-13 09:26:40.000000 opex_manifest_generator-1.1.5/opex_manifest_generator/metadata/MODS Template.xml
--rw-rw-rw-   0        0        0    28748 2024-04-18 10:19:35.000000 opex_manifest_generator-1.1.5/opex_manifest_generator/opex_manifest.py
-drwxrwxrwx   0        0        0        0 2024-04-21 18:50:39.775124 opex_manifest_generator-1.1.5/opex_manifest_generator/samples/
--rw-rw-rw-   0        0        0      389 2023-02-23 12:37:11.000000 opex_manifest_generator-1.1.5/opex_manifest_generator/samples/Opex.xml
--rw-rw-rw-   0        0        0    24938 2024-04-12 14:50:52.000000 opex_manifest_generator-1.1.5/opex_manifest_generator/samples/opex_manifest_generator_AutoClass.xlsx
-drwxrwxrwx   0        0        0        0 2024-04-21 18:50:39.872280 opex_manifest_generator-1.1.5/opex_manifest_generator/samples/spreads/
--rw-rw-rw-   0        0        0    22794 2024-04-04 14:48:01.000000 opex_manifest_generator-1.1.5/opex_manifest_generator/samples/spreads/dctemplate.xlsx
--rw-rw-rw-   0        0        0    19299 2024-04-04 14:45:30.000000 opex_manifest_generator-1.1.5/opex_manifest_generator/samples/spreads/eadtemplate.xlsx
--rw-rw-rw-   0        0        0    18662 2024-04-04 14:51:01.000000 opex_manifest_generator-1.1.5/opex_manifest_generator/samples/spreads/gdprtemplate.xlsx
--rw-rw-rw-   0        0        0    19509 2024-04-04 14:46:22.000000 opex_manifest_generator-1.1.5/opex_manifest_generator/samples/spreads/modstemplate.xlsx
--rw-rw-rw-   0        0        0       58 2024-02-20 15:05:15.000000 opex_manifest_generator-1.1.5/opex_manifest_generator/test_cli.py
-drwxrwxrwx   0        0        0        0 2024-04-21 18:50:39.872280 opex_manifest_generator-1.1.5/opex_manifest_generator.egg-info/
--rw-rw-rw-   0        0        0      701 2024-04-21 18:50:38.000000 opex_manifest_generator-1.1.5/opex_manifest_generator.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1221 2024-04-21 18:50:39.000000 opex_manifest_generator-1.1.5/opex_manifest_generator.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-21 18:50:38.000000 opex_manifest_generator-1.1.5/opex_manifest_generator.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       70 2024-04-21 18:50:38.000000 opex_manifest_generator-1.1.5/opex_manifest_generator.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       51 2024-04-21 18:50:38.000000 opex_manifest_generator-1.1.5/opex_manifest_generator.egg-info/requires.txt
--rw-rw-rw-   0        0        0       24 2024-04-21 18:50:38.000000 opex_manifest_generator-1.1.5/opex_manifest_generator.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      940 2024-04-21 18:48:58.000000 opex_manifest_generator-1.1.5/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-04-21 18:50:39.888287 opex_manifest_generator-1.1.5/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-05-04 20:41:59.872850 opex_manifest_generator-1.1.6/
+-rw-rw-rw-   0        0        0      124 2024-04-12 13:39:12.000000 opex_manifest_generator-1.1.6/.gitignore
+-rw-rw-rw-   0        0        0    11558 2024-02-18 12:39:01.000000 opex_manifest_generator-1.1.6/LICENSE.md
+-rw-rw-rw-   0        0        0      701 2024-05-04 20:41:59.860877 opex_manifest_generator-1.1.6/PKG-INFO
+-rw-rw-rw-   0        0        0    21573 2024-04-21 18:27:56.000000 opex_manifest_generator-1.1.6/README.md
+drwxrwxrwx   0        0        0        0 2024-05-04 20:41:59.417107 opex_manifest_generator-1.1.6/assets/
+-rw-rw-rw-   0        0        0     8271 2024-04-12 14:39:11.000000 opex_manifest_generator-1.1.6/assets/Column Headers.png
+-rw-rw-rw-   0        0        0    27359 2024-04-12 14:49:33.000000 opex_manifest_generator-1.1.6/assets/FullName Column.png
+-rw-rw-rw-   0        0        0    16064 2024-04-12 14:57:04.000000 opex_manifest_generator-1.1.6/assets/Hash Headers.png
+-rw-rw-rw-   0        0        0     4920 2024-04-12 14:58:52.000000 opex_manifest_generator-1.1.6/assets/Identifiers Headers.png
+-rw-rw-rw-   0        0        0     2602 2024-04-12 15:01:06.000000 opex_manifest_generator-1.1.6/assets/XML Headers.png
+drwxrwxrwx   0        0        0        0 2024-05-04 20:41:59.482435 opex_manifest_generator-1.1.6/opex_manifest_generator/
+-rw-rw-rw-   0        0        0      476 2024-04-21 18:41:39.000000 opex_manifest_generator-1.1.6/opex_manifest_generator/__init__.py
+-rw-rw-rw-   0        0        0     6046 2024-04-21 18:36:34.000000 opex_manifest_generator-1.1.6/opex_manifest_generator/cli.py
+-rw-rw-rw-   0        0        0      676 2024-04-04 09:48:17.000000 opex_manifest_generator-1.1.6/opex_manifest_generator/common.py
+-rw-rw-rw-   0        0        0      966 2024-02-18 22:01:42.000000 opex_manifest_generator-1.1.6/opex_manifest_generator/hash.py
+drwxrwxrwx   0        0        0        0 2024-05-04 20:41:59.694088 opex_manifest_generator-1.1.6/opex_manifest_generator/metadata/
+-rw-rw-rw-   0        0        0      775 2023-12-13 09:26:40.000000 opex_manifest_generator-1.1.6/opex_manifest_generator/metadata/DublinCore Template.xml
+-rw-rw-rw-   0        0        0     2268 2023-12-13 09:26:40.000000 opex_manifest_generator-1.1.6/opex_manifest_generator/metadata/EAD Template.xml
+-rw-rw-rw-   0        0        0      483 2023-12-13 09:26:40.000000 opex_manifest_generator-1.1.6/opex_manifest_generator/metadata/GDPR Template.xml
+-rw-rw-rw-   0        0        0     2701 2023-12-13 09:26:40.000000 opex_manifest_generator-1.1.6/opex_manifest_generator/metadata/MODS Template.xml
+-rw-rw-rw-   0        0        0    28824 2024-05-04 20:39:09.000000 opex_manifest_generator-1.1.6/opex_manifest_generator/opex_manifest.py
+drwxrwxrwx   0        0        0        0 2024-05-04 20:41:59.742864 opex_manifest_generator-1.1.6/opex_manifest_generator/samples/
+-rw-rw-rw-   0        0        0      389 2023-02-23 12:37:11.000000 opex_manifest_generator-1.1.6/opex_manifest_generator/samples/Opex.xml
+-rw-rw-rw-   0        0        0    24938 2024-04-12 14:50:52.000000 opex_manifest_generator-1.1.6/opex_manifest_generator/samples/opex_manifest_generator_AutoClass.xlsx
+drwxrwxrwx   0        0        0        0 2024-05-04 20:41:59.849778 opex_manifest_generator-1.1.6/opex_manifest_generator/samples/spreads/
+-rw-rw-rw-   0        0        0    22794 2024-04-04 14:48:01.000000 opex_manifest_generator-1.1.6/opex_manifest_generator/samples/spreads/dctemplate.xlsx
+-rw-rw-rw-   0        0        0    19299 2024-04-04 14:45:30.000000 opex_manifest_generator-1.1.6/opex_manifest_generator/samples/spreads/eadtemplate.xlsx
+-rw-rw-rw-   0        0        0    18662 2024-04-04 14:51:01.000000 opex_manifest_generator-1.1.6/opex_manifest_generator/samples/spreads/gdprtemplate.xlsx
+-rw-rw-rw-   0        0        0    19509 2024-04-04 14:46:22.000000 opex_manifest_generator-1.1.6/opex_manifest_generator/samples/spreads/modstemplate.xlsx
+-rw-rw-rw-   0        0        0       58 2024-02-20 15:05:15.000000 opex_manifest_generator-1.1.6/opex_manifest_generator/test_cli.py
+drwxrwxrwx   0        0        0        0 2024-05-04 20:41:59.856500 opex_manifest_generator-1.1.6/opex_manifest_generator.egg-info/
+-rw-rw-rw-   0        0        0      701 2024-05-04 20:41:58.000000 opex_manifest_generator-1.1.6/opex_manifest_generator.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1221 2024-05-04 20:41:59.000000 opex_manifest_generator-1.1.6/opex_manifest_generator.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-04 20:41:58.000000 opex_manifest_generator-1.1.6/opex_manifest_generator.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       70 2024-05-04 20:41:58.000000 opex_manifest_generator-1.1.6/opex_manifest_generator.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       51 2024-05-04 20:41:58.000000 opex_manifest_generator-1.1.6/opex_manifest_generator.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       24 2024-05-04 20:41:58.000000 opex_manifest_generator-1.1.6/opex_manifest_generator.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      940 2024-05-04 20:40:54.000000 opex_manifest_generator-1.1.6/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-05-04 20:41:59.874874 opex_manifest_generator-1.1.6/setup.cfg
```

### Comparing `opex_manifest_generator-1.1.5/LICENSE.md` & `opex_manifest_generator-1.1.6/LICENSE.md`

 * *Files identical despite different names*

### Comparing `opex_manifest_generator-1.1.5/PKG-INFO` & `opex_manifest_generator-1.1.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: opex_manifest_generator
-Version: 1.1.5
+Version: 1.1.6
 Summary: Opex Manifest Generator Tool for use with Opex / Preservica
 Author-email: Christopher Prince <c.pj.prince@gmail.com>
 Project-URL: Homepage, https://github.com/CPJPRINCE/opex_manifest_generator
 Project-URL: Issues, https://github.com/CPJPRINCE/opex_manifest_generator/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

### Comparing `opex_manifest_generator-1.1.5/README.md` & `opex_manifest_generator-1.1.6/README.md`

 * *Files identical despite different names*

### Comparing `opex_manifest_generator-1.1.5/assets/Column Headers.png` & `opex_manifest_generator-1.1.6/assets/Column Headers.png`

 * *Files identical despite different names*

### Comparing `opex_manifest_generator-1.1.5/assets/FullName Column.png` & `opex_manifest_generator-1.1.6/assets/FullName Column.png`

 * *Files identical despite different names*

### Comparing `opex_manifest_generator-1.1.5/assets/Hash Headers.png` & `opex_manifest_generator-1.1.6/assets/Hash Headers.png`

 * *Files identical despite different names*

### Comparing `opex_manifest_generator-1.1.5/assets/Identifiers Headers.png` & `opex_manifest_generator-1.1.6/assets/Identifiers Headers.png`

 * *Files identical despite different names*

### Comparing `opex_manifest_generator-1.1.5/assets/XML Headers.png` & `opex_manifest_generator-1.1.6/assets/XML Headers.png`

 * *Files identical despite different names*

### Comparing `opex_manifest_generator-1.1.5/opex_manifest_generator/cli.py` & `opex_manifest_generator-1.1.6/opex_manifest_generator/cli.py`

 * *Files identical despite different names*

### Comparing `opex_manifest_generator-1.1.5/opex_manifest_generator/common.py` & `opex_manifest_generator-1.1.6/opex_manifest_generator/common.py`

 * *Files identical despite different names*

### Comparing `opex_manifest_generator-1.1.5/opex_manifest_generator/hash.py` & `opex_manifest_generator-1.1.6/opex_manifest_generator/hash.py`

 * *Files identical despite different names*

### Comparing `opex_manifest_generator-1.1.5/opex_manifest_generator/metadata/DublinCore Template.xml` & `opex_manifest_generator-1.1.6/opex_manifest_generator/metadata/DublinCore Template.xml`

 * *Files identical despite different names*

### Comparing `opex_manifest_generator-1.1.5/opex_manifest_generator/metadata/EAD Template.xml` & `opex_manifest_generator-1.1.6/opex_manifest_generator/metadata/EAD Template.xml`

 * *Files identical despite different names*

### Comparing `opex_manifest_generator-1.1.5/opex_manifest_generator/metadata/MODS Template.xml` & `opex_manifest_generator-1.1.6/opex_manifest_generator/metadata/MODS Template.xml`

 * *Files identical despite different names*

### Comparing `opex_manifest_generator-1.1.5/opex_manifest_generator/opex_manifest.py` & `opex_manifest_generator-1.1.6/opex_manifest_generator/opex_manifest.py`

 * *Files 0% similar despite different names*

```diff
@@ -425,16 +425,18 @@
         self.OMG = OMG
         self.root = self.OMG.root
         self.opexns = self.OMG.opexns
         if folder_path.startswith(u'\\\\?\\'):
             self.folder_path = folder_path.replace(u'\\\\?\\',"")
         else:
             self.folder_path = folder_path
-        if self.OMG.input or not self.OMG.autoclass_flag in {"g","generic"} or self.OMG.ignore_flag or self.OMG.remove_flag or self.OMG.sourceid_flag or self.OMG.title_flag or self.OMG.description_flag or self.OMG.security_flag:
-            self.index = self.OMG.index_df_lookup(self.folder_path)
+        if self.OMG.autoclass_flag is None:
+            pass
+        elif self.OMG.input or not self.OMG.autoclass_flag in {"g","generic","none"} or self.OMG.ignore_flag or self.OMG.remove_flag or self.OMG.sourceid_flag or self.OMG.title_flag or self.OMG.description_flag or self.OMG.security_flag:
+                self.index = self.OMG.index_df_lookup(self.folder_path)
         if self.OMG.ignore_flag or self.OMG.remove_flag:
             if self.OMG.ignore_flag:
                 self.ignore = self.OMG.ignore_df_lookup(self.index)
                 if self.ignore:
                     return
             if self.OMG.remove_flag:
                 self.removal = self.OMG.remove_df_lookup(self.folder_path, self.index)
```

### Comparing `opex_manifest_generator-1.1.5/opex_manifest_generator/samples/opex_manifest_generator_AutoClass.xlsx` & `opex_manifest_generator-1.1.6/opex_manifest_generator/samples/opex_manifest_generator_AutoClass.xlsx`

 * *Files identical despite different names*

### Comparing `opex_manifest_generator-1.1.5/opex_manifest_generator/samples/spreads/dctemplate.xlsx` & `opex_manifest_generator-1.1.6/opex_manifest_generator/samples/spreads/dctemplate.xlsx`

 * *Files identical despite different names*

### Comparing `opex_manifest_generator-1.1.5/opex_manifest_generator/samples/spreads/eadtemplate.xlsx` & `opex_manifest_generator-1.1.6/opex_manifest_generator/samples/spreads/eadtemplate.xlsx`

 * *Files identical despite different names*

### Comparing `opex_manifest_generator-1.1.5/opex_manifest_generator/samples/spreads/gdprtemplate.xlsx` & `opex_manifest_generator-1.1.6/opex_manifest_generator/samples/spreads/gdprtemplate.xlsx`

 * *Files identical despite different names*

### Comparing `opex_manifest_generator-1.1.5/opex_manifest_generator/samples/spreads/modstemplate.xlsx` & `opex_manifest_generator-1.1.6/opex_manifest_generator/samples/spreads/modstemplate.xlsx`

 * *Files identical despite different names*

### Comparing `opex_manifest_generator-1.1.5/opex_manifest_generator.egg-info/PKG-INFO` & `opex_manifest_generator-1.1.6/opex_manifest_generator.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: opex_manifest_generator
-Version: 1.1.5
+Version: 1.1.6
 Summary: Opex Manifest Generator Tool for use with Opex / Preservica
 Author-email: Christopher Prince <c.pj.prince@gmail.com>
 Project-URL: Homepage, https://github.com/CPJPRINCE/opex_manifest_generator
 Project-URL: Issues, https://github.com/CPJPRINCE/opex_manifest_generator/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

### Comparing `opex_manifest_generator-1.1.5/opex_manifest_generator.egg-info/SOURCES.txt` & `opex_manifest_generator-1.1.6/opex_manifest_generator.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `opex_manifest_generator-1.1.5/pyproject.toml` & `opex_manifest_generator-1.1.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 00000030: 746f 6f6c 732d 7363 6d22 5d0d 0a62 7569  tools-scm"]..bui
 00000040: 6c64 2d62 6163 6b65 6e64 203d 2022 7365  ld-backend = "se
 00000050: 7475 7074 6f6f 6c73 2e62 7569 6c64 5f6d  tuptools.build_m
 00000060: 6574 6122 0d0a 0d0a 5b70 726f 6a65 6374  eta"....[project
 00000070: 5d0d 0a6e 616d 6520 3d20 226f 7065 785f  ]..name = "opex_
 00000080: 6d61 6e69 6665 7374 5f67 656e 6572 6174  manifest_generat
 00000090: 6f72 220d 0a76 6572 7369 6f6e 203d 2022  or"..version = "
-000000a0: 312e 312e 3522 0d0a 6175 7468 6f72 7320  1.1.5"..authors 
+000000a0: 312e 312e 3622 0d0a 6175 7468 6f72 7320  1.1.6"..authors 
 000000b0: 3d20 5b0d 0a20 2020 207b 6e61 6d65 3d22  = [..    {name="
 000000c0: 4368 7269 7374 6f70 6865 7220 5072 696e  Christopher Prin
 000000d0: 6365 222c 2065 6d61 696c 3d22 632e 706a  ce", email="c.pj
 000000e0: 2e70 7269 6e63 6540 676d 6169 6c2e 636f  .prince@gmail.co
 000000f0: 6d22 7d0d 0a20 2020 205d 0d0a 6465 7363  m"}..    ]..desc
 00000100: 7269 7074 696f 6e20 3d20 224f 7065 7820  ription = "Opex 
 00000110: 4d61 6e69 6665 7374 2047 656e 6572 6174  Manifest Generat
```

