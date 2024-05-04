# Comparing `tmp/sparrow_parse-0.1.8.tar.gz` & `tmp/sparrow_parse-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sparrow_parse-0.1.8.tar", max compression
+gzip compressed data, was "sparrow_parse-0.1.9.tar", max compression
```

## Comparing `sparrow_parse-0.1.8.tar` & `sparrow_parse-0.1.9.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     2364 2024-04-29 18:20:58.943665 sparrow_parse-0.1.8/README.md
--rw-r--r--   0        0        0      890 2024-04-29 18:21:33.497508 sparrow_parse-0.1.8/pyproject.toml
--rw-r--r--   0        0        0       21 2024-04-29 18:21:33.499724 sparrow_parse-0.1.8/sparrow_parse/__init__.py
--rw-r--r--   0        0        0      153 2024-04-26 13:21:19.954203 sparrow_parse-0.1.8/sparrow_parse/__main__.py
--rw-r--r--   0        0        0        0 2024-04-26 13:23:26.975618 sparrow_parse-0.1.8/sparrow_parse/pdf/__init__.py
--rw-r--r--   0        0        0      159 2024-04-29 11:29:52.002669 sparrow_parse-0.1.8/sparrow_parse/pdf/pdf_processor.py
--rw-r--r--   0        0        0     3250 1970-01-01 00:00:00.000000 sparrow_parse-0.1.8/PKG-INFO
+-rw-r--r--   0        0        0     2417 2024-04-29 18:22:48.987861 sparrow_parse-0.1.9/README.md
+-rw-r--r--   0        0        0     1030 2024-05-04 07:56:39.762943 sparrow_parse-0.1.9/pyproject.toml
+-rw-r--r--   0        0        0       21 2024-05-04 07:56:39.768812 sparrow_parse-0.1.9/sparrow_parse/__init__.py
+-rw-r--r--   0        0        0      153 2024-04-26 13:21:19.954203 sparrow_parse-0.1.9/sparrow_parse/__main__.py
+-rw-r--r--   0        0        0        0 2024-04-26 13:23:26.975618 sparrow_parse-0.1.9/sparrow_parse/extractor/__init__.py
+-rw-r--r--   0        0        0     5621 2024-05-04 07:56:39.765937 sparrow_parse-0.1.9/sparrow_parse/extractor/file_processor.py
+-rw-r--r--   0        0        0     3428 1970-01-01 00:00:00.000000 sparrow_parse-0.1.9/PKG-INFO
```

### Comparing `sparrow_parse-0.1.8/README.md` & `sparrow_parse-0.1.9/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -24,16 +24,22 @@
 processor = PDFProcessor()
 result = processor.process_file(file_path, strategy, model_name)
 ```
 
 Build for development
 
 ```
+poetry build
+```
+
+Publish to PyPi
 
 ```
+poetry publish
+```
 
 ## Commercial usage
 
 Sparrow is available under the GPL 3.0 license, promoting freedom to use, modify, and distribute the software while ensuring any modifications remain open source under the same license. This aligns with our commitment to supporting the open-source community and fostering collaboration.
 
 Additionally, we recognize the diverse needs of organizations, including small to medium-sized enterprises (SMEs). Therefore, Sparrow is also offered for free commercial use to organizations with gross revenue below $5 million USD in the past 12 months, enabling them to leverage Sparrow without the financial burden often associated with high-quality software solutions.
```

### Comparing `sparrow_parse-0.1.8/pyproject.toml` & `sparrow_parse-0.1.9/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "sparrow-parse"
-version = "0.1.8"
+version = "0.1.9"
 description = "Sparrow Parse is a Python package for parsing and extracting information from documents."
 authors = ["Andrej Baranovskij <andrejus.baranovskis@gmail.com>"]
 license = "GPL-3.0"
 readme = "README.md"
 homepage = "https://github.com/katanaml/sparrow/tree/main/sparrow-data/parse"
 repository = "https://github.com/katanaml/sparrow"
 keywords = ["llm", "rag", "vision"]
@@ -16,16 +16,19 @@
 ]
 include = [
     "LICENSE",
 ]
 
 
 [tool.poetry.dependencies]
-python = "^3.10"
-requests = "^2.31.0"
+python = ">=3.9,<3.12"
+torch = {version = "2.2.2", source = "pypi"}
+unstructured = {version = "0.13.6", extras = ["all-docs"]}
+unstructured-inference = "0.7.29"
+rich = "^13.7.1"
 
 
 [tool.poetry.scripts]
 sparrow-parse = 'sparrow_parse:main'
 
 
 [build-system]
```

### Comparing `sparrow_parse-0.1.8/PKG-INFO` & `sparrow_parse-0.1.9/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,25 +1,28 @@
 Metadata-Version: 2.1
 Name: sparrow-parse
-Version: 0.1.8
+Version: 0.1.9
 Summary: Sparrow Parse is a Python package for parsing and extracting information from documents.
 Home-page: https://github.com/katanaml/sparrow/tree/main/sparrow-data/parse
 License: GPL-3.0
 Keywords: llm,rag,vision
 Author: Andrej Baranovskij
 Author-email: andrejus.baranovskis@gmail.com
-Requires-Python: >=3.10,<4.0
+Requires-Python: >=3.9,<3.12
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Software Development
-Requires-Dist: requests (>=2.31.0,<3.0.0)
+Requires-Dist: rich (>=13.7.1,<14.0.0)
+Requires-Dist: torch (==2.2.2)
+Requires-Dist: unstructured-inference (==0.7.29)
+Requires-Dist: unstructured[all-docs] (==0.13.6)
 Project-URL: Repository, https://github.com/katanaml/sparrow
 Description-Content-Type: text/markdown
 
 # Sparrow Parse
 
 ## Description
 
@@ -45,16 +48,22 @@
 processor = PDFProcessor()
 result = processor.process_file(file_path, strategy, model_name)
 ```
 
 Build for development
 
 ```
+poetry build
+```
+
+Publish to PyPi
 
 ```
+poetry publish
+```
 
 ## Commercial usage
 
 Sparrow is available under the GPL 3.0 license, promoting freedom to use, modify, and distribute the software while ensuring any modifications remain open source under the same license. This aligns with our commitment to supporting the open-source community and fostering collaboration.
 
 Additionally, we recognize the diverse needs of organizations, including small to medium-sized enterprises (SMEs). Therefore, Sparrow is also offered for free commercial use to organizations with gross revenue below $5 million USD in the past 12 months, enabling them to leverage Sparrow without the financial burden often associated with high-quality software solutions.
```

