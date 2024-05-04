# Comparing `tmp/sphinxcontrib_lightbox2-0.1.0.tar.gz` & `tmp/sphinxcontrib_lightbox2-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sphinxcontrib_lightbox2-0.1.0.tar", max compression
+gzip compressed data, was "sphinxcontrib_lightbox2-0.1.1.tar", max compression
```

## Comparing `sphinxcontrib_lightbox2-0.1.0.tar` & `sphinxcontrib_lightbox2-0.1.1.tar`

### file list

```diff
@@ -1,11 +1,12 @@
--rw-r--r--   0        0        0      562 2024-05-04 16:06:11.953643 sphinxcontrib_lightbox2-0.1.0/README.md
--rw-r--r--   0        0        0      724 2024-05-04 13:26:50.833987 sphinxcontrib_lightbox2-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     4597 2024-05-04 17:31:43.692509 sphinxcontrib_lightbox2-0.1.0/sphinxcontrib/lightbox2/__init__.py
--rw-r--r--   0        0        0     2532 2024-05-03 18:20:15.129334 sphinxcontrib_lightbox2-0.1.0/sphinxcontrib/lightbox2/assets/css/lightbox.min.css
--rw-r--r--   0        0        0      280 2023-02-21 22:34:02.000000 sphinxcontrib_lightbox2-0.1.0/sphinxcontrib/lightbox2/assets/images/close.png
--rw-r--r--   0        0        0     8476 2023-02-21 22:34:02.000000 sphinxcontrib_lightbox2-0.1.0/sphinxcontrib/lightbox2/assets/images/loading.gif
--rw-r--r--   0        0        0     1350 2023-02-21 22:34:02.000000 sphinxcontrib_lightbox2-0.1.0/sphinxcontrib/lightbox2/assets/images/next.png
--rw-r--r--   0        0        0     1360 2023-02-21 22:34:02.000000 sphinxcontrib_lightbox2-0.1.0/sphinxcontrib/lightbox2/assets/images/prev.png
--rw-r--r--   0        0        0   100774 2024-05-04 16:42:54.313868 sphinxcontrib_lightbox2-0.1.0/sphinxcontrib/lightbox2/assets/js/lightbox-plus-jquery.min.js
--rw-r--r--   0        0        0   147284 2024-05-04 16:42:57.919909 sphinxcontrib_lightbox2-0.1.0/sphinxcontrib/lightbox2/assets/js/lightbox-plus-jquery.min.map
--rw-r--r--   0        0        0     1146 1970-01-01 00:00:00.000000 sphinxcontrib_lightbox2-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0      667 2024-05-04 18:47:26.840399 sphinxcontrib_lightbox2-0.1.1/README.md
+-rw-r--r--   0        0        0     1289 2024-05-04 18:47:26.840399 sphinxcontrib_lightbox2-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     4591 2024-05-04 18:47:26.840399 sphinxcontrib_lightbox2-0.1.1/sphinxcontrib/lightbox2/__init__.py
+-rw-r--r--   0        0        0     2532 2024-05-04 18:47:26.840399 sphinxcontrib_lightbox2-0.1.1/sphinxcontrib/lightbox2/assets/css/lightbox.min.css
+-rw-r--r--   0        0        0      280 2024-05-04 18:47:26.840399 sphinxcontrib_lightbox2-0.1.1/sphinxcontrib/lightbox2/assets/images/close.png
+-rw-r--r--   0        0        0     8476 2024-05-04 18:47:26.840399 sphinxcontrib_lightbox2-0.1.1/sphinxcontrib/lightbox2/assets/images/loading.gif
+-rw-r--r--   0        0        0     1350 2024-05-04 18:47:26.840399 sphinxcontrib_lightbox2-0.1.1/sphinxcontrib/lightbox2/assets/images/next.png
+-rw-r--r--   0        0        0     1360 2024-05-04 18:47:26.840399 sphinxcontrib_lightbox2-0.1.1/sphinxcontrib/lightbox2/assets/images/prev.png
+-rw-r--r--   0        0        0   100774 2024-05-04 18:47:26.840399 sphinxcontrib_lightbox2-0.1.1/sphinxcontrib/lightbox2/assets/js/lightbox-plus-jquery.min.js
+-rw-r--r--   0        0        0   147284 2024-05-04 18:47:26.844399 sphinxcontrib_lightbox2-0.1.1/sphinxcontrib/lightbox2/assets/js/lightbox-plus-jquery.min.map
+-rw-r--r--   0        0        0        0 2024-05-04 18:47:26.844399 sphinxcontrib_lightbox2-0.1.1/sphinxcontrib/lightbox2/py.typed
+-rw-r--r--   0        0        0     1327 1970-01-01 00:00:00.000000 sphinxcontrib_lightbox2-0.1.1/PKG-INFO
```

### Comparing `sphinxcontrib_lightbox2-0.1.0/README.md` & `sphinxcontrib_lightbox2-0.1.1/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -1,11 +1,17 @@
 # sphinxcontrib-lightbox2
 
 Sphinx extension to add [lightbox2](https://lokeshdhakar.com/projects/lightbox2/) to each figure and image added in HTML.
 
+---
+
+**[Read the documentation on ReadTheDocs!](https://sphinxcontrib-lightbox2.readthedocs.io/)**
+
+---
+
 Usually Sphinx themes limit their content width to a limit to improve readability. This creates a problem for large
 images and diagrams which might be needed in technical documentation.
 
 ## Installation
 
 Install the package using
```

### Comparing `sphinxcontrib_lightbox2-0.1.0/sphinxcontrib/lightbox2/__init__.py` & `sphinxcontrib_lightbox2-0.1.1/sphinxcontrib/lightbox2/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 import importlib.metadata
 import pathlib
-from docutils import nodes
-import urllib.parse
 import posixpath
+import urllib.parse
+
+from docutils import nodes
 from sphinx.application import Sphinx
 from sphinx.environment import BuildEnvironment
 from sphinx.util import display, osutil
 from sphinx.util.typing import ExtensionMetadata
-from sphinx.builders.html import StandaloneHTMLBuilder
 from sphinx.writers.html5 import HTML5Translator
 
 try:
-    import sphinxcontrib.plantuml
+    import sphinxcontrib.plantuml  # type: ignore
 
     __PLANTUML_AVAILABLE__ = True
 
 except ImportError:
     __PLANTUML_AVAILABLE__ = False
 
 try:
@@ -33,22 +33,22 @@
     pathlib.Path("assets/images/loading.gif"),
     pathlib.Path("assets/js/lightbox-plus-jquery.min.js"),
     pathlib.Path("assets/js/lightbox-plus-jquery.min.map"),
     pathlib.Path("assets/css/lightbox.min.css"),
 )
 
 
-def start_lightbox_anchor(self: HTML5Translator, uri: str):
+def start_lightbox_anchor(self: HTML5Translator, uri: str) -> None:
     """
     Write the start of a lightbox anchor to the body
     """
     self.body.append(f"""<a href="{uri}" data-lightbox="image-set">\n""")
 
 
-def end_lightbox_anchor(self: HTML5Translator, node: nodes.Element):
+def end_lightbox_anchor(self: HTML5Translator, node: nodes.Element) -> None:
     self.body.append("</a>\n")
 
 
 def install_static_files(app: Sphinx, env: BuildEnvironment) -> None:
     static_dir = pathlib.Path(app.builder.outdir) / app.config.html_static_path[0]
     dest_path = pathlib.Path(static_dir)
 
@@ -57,24 +57,24 @@
         "Copying static files for sphinxcontrib-lightbox2...",
         "brown",
         len(STATIC_FILES),
     ):
         dest_file_path = dest_path / source_file_path.relative_to(*source_file_path.parts[:1])
         osutil.ensuredir(dest_file_path.parent)
 
-        source_file_path = pathlib.Path(__file__).parent / source_file_path
-        osutil.copyfile(source_file_path, dest_file_path)
+        abs_source_file_path = pathlib.Path(__file__).parent / source_file_path
+        osutil.copyfile(abs_source_file_path, dest_file_path)
 
         if dest_file_path.suffix == ".js":
             app.add_js_file(str(dest_file_path.relative_to(static_dir)))
         elif dest_file_path.suffix == ".css":
             app.add_css_file(str(dest_file_path.relative_to(static_dir)))
 
 
-def html_visit_plantuml(self: HTML5Translator, node: nodes.Element):
+def html_visit_plantuml(self: HTML5Translator, node: nodes.Element) -> None:
 
     if "html_format" in node:
         fmt = node["html_format"]
     else:
         fmt = self.builder.config.plantuml_output_format
 
     with sphinxcontrib.plantuml._prepare_html_render(self, fmt, node) as (fileformats, _):
```

### Comparing `sphinxcontrib_lightbox2-0.1.0/sphinxcontrib/lightbox2/assets/css/lightbox.min.css` & `sphinxcontrib_lightbox2-0.1.1/sphinxcontrib/lightbox2/assets/css/lightbox.min.css`

 * *Files identical despite different names*

### Comparing `sphinxcontrib_lightbox2-0.1.0/sphinxcontrib/lightbox2/assets/images/loading.gif` & `sphinxcontrib_lightbox2-0.1.1/sphinxcontrib/lightbox2/assets/images/loading.gif`

 * *Files identical despite different names*

### Comparing `sphinxcontrib_lightbox2-0.1.0/sphinxcontrib/lightbox2/assets/images/next.png` & `sphinxcontrib_lightbox2-0.1.1/sphinxcontrib/lightbox2/assets/images/next.png`

 * *Files identical despite different names*

### Comparing `sphinxcontrib_lightbox2-0.1.0/sphinxcontrib/lightbox2/assets/images/prev.png` & `sphinxcontrib_lightbox2-0.1.1/sphinxcontrib/lightbox2/assets/images/prev.png`

 * *Files identical despite different names*

### Comparing `sphinxcontrib_lightbox2-0.1.0/sphinxcontrib/lightbox2/assets/js/lightbox-plus-jquery.min.js` & `sphinxcontrib_lightbox2-0.1.1/sphinxcontrib/lightbox2/assets/js/lightbox-plus-jquery.min.js`

 * *Files identical despite different names*

### Comparing `sphinxcontrib_lightbox2-0.1.0/sphinxcontrib/lightbox2/assets/js/lightbox-plus-jquery.min.map` & `sphinxcontrib_lightbox2-0.1.1/sphinxcontrib/lightbox2/assets/js/lightbox-plus-jquery.min.map`

 * *Files identical despite different names*

### Comparing `sphinxcontrib_lightbox2-0.1.0/PKG-INFO` & `sphinxcontrib_lightbox2-0.1.1/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,27 +1,34 @@
 Metadata-Version: 2.1
 Name: sphinxcontrib-lightbox2
-Version: 0.1.0
+Version: 0.1.1
 Summary: Sphinx extension to add lightbox2 to each figure and image added in HTML
 License: MIT
 Author: Jonas Ehrlich
 Author-email: jonas.ehrlich@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: sphinx (>=7.3.7,<8.0.0)
+Project-URL: Documentation, https://sphinxcontrib-lightbox2.readthedocs.io/
 Description-Content-Type: text/markdown
 
 # sphinxcontrib-lightbox2
 
 Sphinx extension to add [lightbox2](https://lokeshdhakar.com/projects/lightbox2/) to each figure and image added in HTML.
 
+---
+
+**[Read the documentation on ReadTheDocs!](https://sphinxcontrib-lightbox2.readthedocs.io/)**
+
+---
+
 Usually Sphinx themes limit their content width to a limit to improve readability. This creates a problem for large
 images and diagrams which might be needed in technical documentation.
 
 ## Installation
 
 Install the package using
```

