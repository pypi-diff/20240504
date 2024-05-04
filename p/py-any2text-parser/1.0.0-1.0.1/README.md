# Comparing `tmp/py_any2text_parser-1.0.0.tar.gz` & `tmp/py_any2text_parser-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py_any2text_parser-1.0.0.tar", last modified: Sat May  4 13:59:04 2024, max compression
+gzip compressed data, was "py_any2text_parser-1.0.1.tar", last modified: Sat May  4 14:06:35 2024, max compression
```

## Comparing `py_any2text_parser-1.0.0.tar` & `py_any2text_parser-1.0.1.tar`

### file list

```diff
@@ -1,19 +1,20 @@
-drwxr-xr-x   0 user       (502) staff       (20)        0 2024-05-04 13:59:04.027273 py_any2text_parser-1.0.0/
--rw-r--r--   0 user       (502) staff       (20)     1079 2024-05-04 13:59:04.027038 py_any2text_parser-1.0.0/PKG-INFO
--rw-r--r--   0 user       (502) staff       (20)      585 2024-05-04 13:38:33.000000 py_any2text_parser-1.0.0/README.md
--rw-r--r--   0 user       (502) staff       (20)      492 2024-05-04 13:58:44.000000 py_any2text_parser-1.0.0/pyproject.toml
--rw-r--r--   0 user       (502) staff       (20)       38 2024-05-04 13:59:04.027319 py_any2text_parser-1.0.0/setup.cfg
-drwxr-xr-x   0 user       (502) staff       (20)        0 2024-05-04 13:59:04.024179 py_any2text_parser-1.0.0/src/
-drwxr-xr-x   0 user       (502) staff       (20)        0 2024-05-04 13:59:04.024663 py_any2text_parser-1.0.0/src/pdf2text/
--rw-r--r--   0 user       (502) staff       (20)        0 2024-05-04 13:00:19.000000 py_any2text_parser-1.0.0/src/pdf2text/__init__.py
-drwxr-xr-x   0 user       (502) staff       (20)        0 2024-05-04 13:59:04.025890 py_any2text_parser-1.0.0/src/pdf2text/include/
--rw-r--r--   0 user       (502) staff       (20)     4364 2024-05-04 12:34:39.000000 py_any2text_parser-1.0.0/src/pdf2text/include/pdfcoordhelper.py
--rw-r--r--   0 user       (502) staff       (20)     2898 2024-05-04 13:10:36.000000 py_any2text_parser-1.0.0/src/pdf2text/include/pdfpagehelper.py
--rw-r--r--   0 user       (502) staff       (20)    10386 2024-05-04 12:53:41.000000 py_any2text_parser-1.0.0/src/pdf2text/include/pdftablehelper.py
--rw-r--r--   0 user       (502) staff       (20)    10656 2024-05-04 12:54:03.000000 py_any2text_parser-1.0.0/src/pdf2text/include/pdfunstructuredhelper.py
--rw-r--r--   0 user       (502) staff       (20)     2037 2024-05-04 13:30:35.000000 py_any2text_parser-1.0.0/src/pdf2text/pdf2text.py
-drwxr-xr-x   0 user       (502) staff       (20)        0 2024-05-04 13:59:04.026805 py_any2text_parser-1.0.0/src/py_any2text_parser.egg-info/
--rw-r--r--   0 user       (502) staff       (20)     1079 2024-05-04 13:59:04.000000 py_any2text_parser-1.0.0/src/py_any2text_parser.egg-info/PKG-INFO
--rw-r--r--   0 user       (502) staff       (20)      420 2024-05-04 13:59:04.000000 py_any2text_parser-1.0.0/src/py_any2text_parser.egg-info/SOURCES.txt
--rw-r--r--   0 user       (502) staff       (20)        1 2024-05-04 13:59:04.000000 py_any2text_parser-1.0.0/src/py_any2text_parser.egg-info/dependency_links.txt
--rw-r--r--   0 user       (502) staff       (20)        9 2024-05-04 13:59:04.000000 py_any2text_parser-1.0.0/src/py_any2text_parser.egg-info/top_level.txt
+drwxr-xr-x   0 user       (502) staff       (20)        0 2024-05-04 14:06:35.024077 py_any2text_parser-1.0.1/
+-rw-r--r--   0 user       (502) staff       (20)     1274 2024-05-04 14:06:35.023860 py_any2text_parser-1.0.1/PKG-INFO
+-rw-r--r--   0 user       (502) staff       (20)      780 2024-05-04 14:00:47.000000 py_any2text_parser-1.0.1/README.md
+-rw-r--r--   0 user       (502) staff       (20)      492 2024-05-04 14:06:08.000000 py_any2text_parser-1.0.1/pyproject.toml
+-rw-r--r--   0 user       (502) staff       (20)       38 2024-05-04 14:06:35.024128 py_any2text_parser-1.0.1/setup.cfg
+-rw-r--r--   0 user       (502) staff       (20)      622 2024-05-04 14:05:24.000000 py_any2text_parser-1.0.1/setup.py
+drwxr-xr-x   0 user       (502) staff       (20)        0 2024-05-04 14:06:35.020256 py_any2text_parser-1.0.1/src/
+drwxr-xr-x   0 user       (502) staff       (20)        0 2024-05-04 14:06:35.020859 py_any2text_parser-1.0.1/src/pdf2text/
+-rw-r--r--   0 user       (502) staff       (20)        0 2024-05-04 13:00:19.000000 py_any2text_parser-1.0.1/src/pdf2text/__init__.py
+drwxr-xr-x   0 user       (502) staff       (20)        0 2024-05-04 14:06:35.022488 py_any2text_parser-1.0.1/src/pdf2text/include/
+-rw-r--r--   0 user       (502) staff       (20)     4364 2024-05-04 12:34:39.000000 py_any2text_parser-1.0.1/src/pdf2text/include/pdfcoordhelper.py
+-rw-r--r--   0 user       (502) staff       (20)     2898 2024-05-04 13:10:36.000000 py_any2text_parser-1.0.1/src/pdf2text/include/pdfpagehelper.py
+-rw-r--r--   0 user       (502) staff       (20)    10386 2024-05-04 12:53:41.000000 py_any2text_parser-1.0.1/src/pdf2text/include/pdftablehelper.py
+-rw-r--r--   0 user       (502) staff       (20)    10656 2024-05-04 12:54:03.000000 py_any2text_parser-1.0.1/src/pdf2text/include/pdfunstructuredhelper.py
+-rw-r--r--   0 user       (502) staff       (20)     2037 2024-05-04 13:30:35.000000 py_any2text_parser-1.0.1/src/pdf2text/pdf2text.py
+drwxr-xr-x   0 user       (502) staff       (20)        0 2024-05-04 14:06:35.023508 py_any2text_parser-1.0.1/src/py_any2text_parser.egg-info/
+-rw-r--r--   0 user       (502) staff       (20)     1274 2024-05-04 14:06:35.000000 py_any2text_parser-1.0.1/src/py_any2text_parser.egg-info/PKG-INFO
+-rw-r--r--   0 user       (502) staff       (20)      429 2024-05-04 14:06:35.000000 py_any2text_parser-1.0.1/src/py_any2text_parser.egg-info/SOURCES.txt
+-rw-r--r--   0 user       (502) staff       (20)        1 2024-05-04 14:06:35.000000 py_any2text_parser-1.0.1/src/py_any2text_parser.egg-info/dependency_links.txt
+-rw-r--r--   0 user       (502) staff       (20)        9 2024-05-04 14:06:35.000000 py_any2text_parser-1.0.1/src/py_any2text_parser.egg-info/top_level.txt
```

### Comparing `py_any2text_parser-1.0.0/PKG-INFO` & `py_any2text_parser-1.0.1/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,21 +1,35 @@
 Metadata-Version: 2.1
 Name: py-any2text-parser
-Version: 1.0.0
+Version: 1.0.1
 Summary: Any2Text - any format to text using Unstructured.io
 Author-email: Vanson Leung <vanson@vanportdev.com>
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.9
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 
-# any2text-parser
+# py-any2text-parser
+
+## install
+
+`pip install py-any2text-parser`
+
+## usage
+
+```
+
+```
+
+
+
+# developer only below:
 
 ## initialize
 
 ```shell
 python3 -m venv ./venv
 source venv/bin/activate
 pip install -r requirements.txt
@@ -41,7 +55,15 @@
     meta_data_mapping = {
         "document_category": "DEF",
     }
   )
   
   print(text_data, text)
 ```
+
+## develop - upload to pypi
+
+```
+pip install twine build
+python3 -m build
+twine upload dist/*
+```
```

### Comparing `py_any2text_parser-1.0.0/README.md` & `py_any2text_parser-1.0.1/README.md`

 * *Files 27% similar despite different names*

```diff
@@ -1,8 +1,22 @@
-# any2text-parser
+# py-any2text-parser
+
+## install
+
+`pip install py-any2text-parser`
+
+## usage
+
+```
+
+```
+
+
+
+# developer only below:
 
 ## initialize
 
 ```shell
 python3 -m venv ./venv
 source venv/bin/activate
 pip install -r requirements.txt
@@ -28,7 +42,15 @@
     meta_data_mapping = {
         "document_category": "DEF",
     }
   )
   
   print(text_data, text)
 ```
+
+## develop - upload to pypi
+
+```
+pip install twine build
+python3 -m build
+twine upload dist/*
+```
```

### Comparing `py_any2text_parser-1.0.0/src/pdf2text/include/pdfcoordhelper.py` & `py_any2text_parser-1.0.1/src/pdf2text/include/pdfcoordhelper.py`

 * *Files identical despite different names*

### Comparing `py_any2text_parser-1.0.0/src/pdf2text/include/pdfpagehelper.py` & `py_any2text_parser-1.0.1/src/pdf2text/include/pdfpagehelper.py`

 * *Files identical despite different names*

### Comparing `py_any2text_parser-1.0.0/src/pdf2text/include/pdftablehelper.py` & `py_any2text_parser-1.0.1/src/pdf2text/include/pdftablehelper.py`

 * *Files identical despite different names*

### Comparing `py_any2text_parser-1.0.0/src/pdf2text/include/pdfunstructuredhelper.py` & `py_any2text_parser-1.0.1/src/pdf2text/include/pdfunstructuredhelper.py`

 * *Files identical despite different names*

### Comparing `py_any2text_parser-1.0.0/src/pdf2text/pdf2text.py` & `py_any2text_parser-1.0.1/src/pdf2text/pdf2text.py`

 * *Files identical despite different names*

### Comparing `py_any2text_parser-1.0.0/src/py_any2text_parser.egg-info/PKG-INFO` & `py_any2text_parser-1.0.1/src/py_any2text_parser.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,21 +1,35 @@
 Metadata-Version: 2.1
 Name: py-any2text-parser
-Version: 1.0.0
+Version: 1.0.1
 Summary: Any2Text - any format to text using Unstructured.io
 Author-email: Vanson Leung <vanson@vanportdev.com>
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.9
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 
-# any2text-parser
+# py-any2text-parser
+
+## install
+
+`pip install py-any2text-parser`
+
+## usage
+
+```
+
+```
+
+
+
+# developer only below:
 
 ## initialize
 
 ```shell
 python3 -m venv ./venv
 source venv/bin/activate
 pip install -r requirements.txt
@@ -41,7 +55,15 @@
     meta_data_mapping = {
         "document_category": "DEF",
     }
   )
   
   print(text_data, text)
 ```
+
+## develop - upload to pypi
+
+```
+pip install twine build
+python3 -m build
+twine upload dist/*
+```
```

