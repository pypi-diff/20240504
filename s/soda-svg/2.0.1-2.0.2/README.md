# Comparing `tmp/soda_svg-2.0.1.tar.gz` & `tmp/soda_svg-2.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "soda_svg-2.0.1.tar", max compression
+gzip compressed data, was "soda_svg-2.0.2.tar", max compression
```

## Comparing `soda_svg-2.0.1.tar` & `soda_svg-2.0.2.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0     1073 2024-05-04 19:22:52.017212 soda_svg-2.0.1/LICENSE
--rw-r--r--   0        0        0    13304 2024-05-04 19:22:52.017212 soda_svg-2.0.1/README.md
--rw-r--r--   0        0        0      633 2024-05-04 19:22:52.017212 soda_svg-2.0.1/pyproject.toml
--rw-r--r--   0        0        0      317 2024-05-04 19:22:52.017212 soda_svg-2.0.1/soda/__init__.py
--rw-r--r--   0        0        0      123 2024-05-04 19:22:52.021212 soda_svg-2.0.1/soda/config_mod.py
--rw-r--r--   0        0        0     2489 2024-05-04 19:22:52.021212 soda_svg-2.0.1/soda/custom_tags.py
--rw-r--r--   0        0        0     7357 2024-05-04 19:22:52.021212 soda_svg-2.0.1/soda/paths.py
--rw-r--r--   0        0        0    11689 2024-05-04 19:22:52.021212 soda_svg-2.0.1/soda/point.py
--rw-r--r--   0        0        0        0 2024-05-04 19:22:52.021212 soda_svg-2.0.1/soda/py.typed
--rw-r--r--   0        0        0    11663 2024-05-04 19:22:52.021212 soda_svg-2.0.1/soda/tags.py
--rw-r--r--   0        0        0     1838 2024-05-04 19:22:52.021212 soda_svg-2.0.1/soda/utils.py
--rw-r--r--   0        0        0     1672 2024-05-04 19:22:52.021212 soda_svg-2.0.1/soda/xml_parse.py
--rw-r--r--   0        0        0    14127 1970-01-01 00:00:00.000000 soda_svg-2.0.1/PKG-INFO
+-rw-r--r--   0        0        0     1073 2024-05-04 19:51:19.550289 soda_svg-2.0.2/LICENSE
+-rw-r--r--   0        0        0    13304 2024-05-04 19:51:19.550289 soda_svg-2.0.2/README.md
+-rw-r--r--   0        0        0      633 2024-05-04 19:51:19.550289 soda_svg-2.0.2/pyproject.toml
+-rw-r--r--   0        0        0      317 2024-05-04 19:51:19.550289 soda_svg-2.0.2/soda/__init__.py
+-rw-r--r--   0        0        0      123 2024-05-04 19:51:19.550289 soda_svg-2.0.2/soda/config_mod.py
+-rw-r--r--   0        0        0     2489 2024-05-04 19:51:19.550289 soda_svg-2.0.2/soda/custom_tags.py
+-rw-r--r--   0        0        0     7357 2024-05-04 19:51:19.550289 soda_svg-2.0.2/soda/paths.py
+-rw-r--r--   0        0        0    11689 2024-05-04 19:51:19.550289 soda_svg-2.0.2/soda/point.py
+-rw-r--r--   0        0        0        0 2024-05-04 19:51:19.550289 soda_svg-2.0.2/soda/py.typed
+-rw-r--r--   0        0        0    11663 2024-05-04 19:51:19.554288 soda_svg-2.0.2/soda/tags.py
+-rw-r--r--   0        0        0     1838 2024-05-04 19:51:19.554288 soda_svg-2.0.2/soda/utils.py
+-rw-r--r--   0        0        0     1748 2024-05-04 19:51:19.554288 soda_svg-2.0.2/soda/xml_parse.py
+-rw-r--r--   0        0        0    14127 1970-01-01 00:00:00.000000 soda_svg-2.0.2/PKG-INFO
```

### Comparing `soda_svg-2.0.1/LICENSE` & `soda_svg-2.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `soda_svg-2.0.1/README.md` & `soda_svg-2.0.2/README.md`

 * *Files identical despite different names*

### Comparing `soda_svg-2.0.1/pyproject.toml` & `soda_svg-2.0.2/pyproject.toml`

 * *Files 22% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool.poetry]
 name = "soda-svg"
 packages = [{include = "soda"}]
-version = "2.0.1"
+version = "2.0.2"
 description = "Fast SVG generation tool"
 authors = ["Dmitry Gritsenko <soda@evtn.ru>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/evtn/soda"
 homepage = "https://github.com/evtn/soda"
 keywords = ["soda", "svg", "xml"]
```

### Comparing `soda_svg-2.0.1/soda/custom_tags.py` & `soda_svg-2.0.2/soda/custom_tags.py`

 * *Files identical despite different names*

### Comparing `soda_svg-2.0.1/soda/paths.py` & `soda_svg-2.0.2/soda/paths.py`

 * *Files identical despite different names*

### Comparing `soda_svg-2.0.1/soda/point.py` & `soda_svg-2.0.2/soda/point.py`

 * *Files identical despite different names*

### Comparing `soda_svg-2.0.1/soda/tags.py` & `soda_svg-2.0.2/soda/tags.py`

 * *Files identical despite different names*

### Comparing `soda_svg-2.0.1/soda/utils.py` & `soda_svg-2.0.2/soda/utils.py`

 * *Files identical despite different names*

### Comparing `soda_svg-2.0.1/soda/xml_parse.py` & `soda_svg-2.0.2/soda/xml_parse.py`

 * *Files 9% similar despite different names*

```diff
@@ -40,17 +40,20 @@
         yield element_to_tag(child)
         tail = str_to_tag(child.tail)
         if tail:
             yield tail
 
 
 def element_to_tag(element: etree._Element) -> Tag:
-    if not isinstance(element.tag, str):
+    if isinstance(element.tag, etree._Comment):
         return XMLComment(element.tag.text)
 
+    if not isinstance(element.tag, str):
+        return Literal("")
+
     tag_name = element.tag.split("}")[-1]
     raw_attributes = element.attrib
 
     reverse_nsmap = {v: k for k, v in element.nsmap.items()}
 
     attributes: dict[str, str] = {}
```

### Comparing `soda_svg-2.0.1/PKG-INFO` & `soda_svg-2.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: soda-svg
-Version: 2.0.1
+Version: 2.0.2
 Summary: Fast SVG generation tool
 Home-page: https://github.com/evtn/soda
 License: MIT
 Keywords: soda,svg,xml
 Author: Dmitry Gritsenko
 Author-email: soda@evtn.ru
 Requires-Python: >=3.8,<3.13
```

