# Comparing `tmp/sphinxext-photofinish-0.1.8.tar.gz` & `tmp/sphinxext-photofinish-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/sphinxext-photofinish-0.1.8.tar", last modified: Sun Oct 17 18:45:55 2021, max compression
+gzip compressed data, was "dist/sphinxext-photofinish-0.1.9.tar", last modified: Sun Aug 28 06:08:30 2022, max compression
```

## Comparing `sphinxext-photofinish-0.1.8.tar` & `sphinxext-photofinish-0.1.9.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-17 18:45:55.000000 sphinxext-photofinish-0.1.8/
--rw-r--r--   0 runner    (1001) docker     (121)     1057 2021-10-17 18:45:43.000000 sphinxext-photofinish-0.1.8/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (121)     2231 2021-10-17 18:45:55.000000 sphinxext-photofinish-0.1.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1162 2021-10-17 18:45:43.000000 sphinxext-photofinish-0.1.8/README.md
--rw-r--r--   0 runner    (1001) docker     (121)       38 2021-10-17 18:45:55.000000 sphinxext-photofinish-0.1.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1558 2021-10-17 18:45:43.000000 sphinxext-photofinish-0.1.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-17 18:45:55.000000 sphinxext-photofinish-0.1.8/sphinxext/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-17 18:45:55.000000 sphinxext-photofinish-0.1.8/sphinxext/photofinish/
--rw-r--r--   0 runner    (1001) docker     (121)    15463 2021-10-17 18:45:43.000000 sphinxext-photofinish-0.1.8/sphinxext/photofinish/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    11044 2021-10-17 18:45:43.000000 sphinxext-photofinish-0.1.8/sphinxext/photofinish/svgtopng.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-17 18:45:55.000000 sphinxext-photofinish-0.1.8/sphinxext_photofinish.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     2231 2021-10-17 18:45:55.000000 sphinxext-photofinish-0.1.8/sphinxext_photofinish.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      321 2021-10-17 18:45:55.000000 sphinxext-photofinish-0.1.8/sphinxext_photofinish.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-10-17 18:45:55.000000 sphinxext-photofinish-0.1.8/sphinxext_photofinish.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       40 2021-10-17 18:45:55.000000 sphinxext-photofinish-0.1.8/sphinxext_photofinish.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       22 2021-10-17 18:45:55.000000 sphinxext-photofinish-0.1.8/sphinxext_photofinish.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-28 06:08:30.000000 sphinxext-photofinish-0.1.9/
+-rw-r--r--   0 runner    (1001) docker     (121)     1057 2022-08-28 06:08:21.000000 sphinxext-photofinish-0.1.9/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (121)     2309 2022-08-28 06:08:30.000000 sphinxext-photofinish-0.1.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     1276 2022-08-28 06:08:21.000000 sphinxext-photofinish-0.1.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (121)       38 2022-08-28 06:08:30.000000 sphinxext-photofinish-0.1.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)     1616 2022-08-28 06:08:21.000000 sphinxext-photofinish-0.1.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-28 06:08:30.000000 sphinxext-photofinish-0.1.9/sphinxext/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-28 06:08:30.000000 sphinxext-photofinish-0.1.9/sphinxext/photofinish/
+-rw-r--r--   0 runner    (1001) docker     (121)    16182 2022-08-28 06:08:21.000000 sphinxext-photofinish-0.1.9/sphinxext/photofinish/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    11044 2022-08-28 06:08:21.000000 sphinxext-photofinish-0.1.9/sphinxext/photofinish/svgtopng.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-28 06:08:30.000000 sphinxext-photofinish-0.1.9/sphinxext_photofinish.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)     2309 2022-08-28 06:08:30.000000 sphinxext-photofinish-0.1.9/sphinxext_photofinish.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)      321 2022-08-28 06:08:30.000000 sphinxext-photofinish-0.1.9/sphinxext_photofinish.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-08-28 06:08:30.000000 sphinxext-photofinish-0.1.9/sphinxext_photofinish.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       56 2022-08-28 06:08:30.000000 sphinxext-photofinish-0.1.9/sphinxext_photofinish.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       22 2022-08-28 06:08:30.000000 sphinxext-photofinish-0.1.9/sphinxext_photofinish.egg-info/top_level.txt
```

### Comparing `sphinxext-photofinish-0.1.8/LICENSE.md` & `sphinxext-photofinish-0.1.9/LICENSE.md`

 * *Files identical despite different names*

### Comparing `sphinxext-photofinish-0.1.8/PKG-INFO` & `sphinxext-photofinish-0.1.9/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,14 @@
 Metadata-Version: 2.1
 Name: sphinxext-photofinish
-Version: 0.1.8
+Version: 0.1.9
 Summary: Sphinx Extension that creates responsive images.
 Home-page: https://github.com/wpilibsuite/sphinxext-photofinish
 Author: WPILib
 Author-email: developers@wpilib.org
-License: UNKNOWN
-Platform: UNKNOWN
 Classifier: Environment :: Plugins
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Sphinx :: Extension
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
@@ -55,8 +53,8 @@
 
 `max_viewport_width` - This is maximum "viewable" size of images in your documentation. Typically, it's set to the width of your body. Responsive images are generated up to double of this value. Default is 1000.
 
 `width_min` - Minimum width of images to generate. Default is 500.
 
 `width_step` - The resolution to iterate over for generating images. EX: 500, 800, 1100. Default is 300.
 
-
+`photofinish_ci_only` - Should this extension only run if the `CI` environment variable is set? Default is False.
```

### Comparing `sphinxext-photofinish-0.1.8/README.md` & `sphinxext-photofinish-0.1.9/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -25,7 +25,9 @@
 Photofinish adds several `conf.py` options that you can optionally configure:
 
 `max_viewport_width` - This is maximum "viewable" size of images in your documentation. Typically, it's set to the width of your body. Responsive images are generated up to double of this value. Default is 1000.
 
 `width_min` - Minimum width of images to generate. Default is 500.
 
 `width_step` - The resolution to iterate over for generating images. EX: 500, 800, 1100. Default is 300.
+
+`photofinish_ci_only` - Should this extension only run if the `CI` environment variable is set? Default is False.
```

### Comparing `sphinxext-photofinish-0.1.8/setup.py` & `sphinxext-photofinish-0.1.9/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -19,15 +19,20 @@
     author="WPILib",
     author_email="developers@wpilib.org",
     description="Sphinx Extension that creates responsive images.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/wpilibsuite/sphinxext-photofinish",
     packages=["sphinxext/photofinish"],
-    install_requires=["sphinx>=2.0", "beautifulsoup4>=4", "pillow>=8"],
+    install_requires=[
+        "sphinx>=2.0",
+        "beautifulsoup4>=4",
+        "pillow>=8",
+        "tinycss2>=1.1.1",
+    ],
     classifiers=[
         "Environment :: Plugins",
         "Environment :: Web Environment",
         "Framework :: Sphinx :: Extension",
         "Intended Audience :: Developers",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

### Comparing `sphinxext-photofinish-0.1.8/sphinxext/photofinish/__init__.py` & `sphinxext-photofinish-0.1.9/sphinxext/photofinish/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -19,14 +19,17 @@
 ## Re 3. `pillow_avif` conveniently packages its own libavif and seems to have
 # full wheels for a few OSes so I went for this as my first (and only) try.
 ## Re 4. `rav1e` is not prepackaged and can't be installed on RTD
 from dataclasses import dataclass
 from os import PathLike
 from pathlib import Path
 import tempfile
+from turtle import st
+import tinycss2
+import tinycss2.ast
 from typing import Any, Callable, Dict, Optional, Set
 
 from bs4 import BeautifulSoup, Tag
 from docutils.nodes import Node
 from docutils.writers.html5_polyglot import HTMLTranslator
 from PIL import Image
 from PIL.PngImagePlugin import PngImageFile, PngInfo
@@ -99,24 +102,49 @@
         re.sub(CRITICAL_PATH_CHAR_RE, "_", img_src_path.stem) + img_src_path.suffix
     )
     ensuredir(imagedir)
 
     soup_img: Tag = BeautifulSoup(img_tag_str, features="html.parser").img
     soup_picture: Tag = BeautifulSoup().new_tag("picture")
 
-    # Move height / width from <img/> to <picture/>. The img tag will hold the actual
-    # resolution of the image file and its parent, picture, will hold
-    # the desired size constraints.
-    if "height" in soup_img.attrs:
-        soup_picture.attrs["height"] = soup_img.attrs["height"]
-        del soup_img.attrs["height"]
-
-    if "width" in soup_img.attrs:
-        soup_picture.attrs["width"] = soup_img.attrs["width"]
-        del soup_img.attrs["width"]
+    # Move height / width from img attributes to img style attributes.
+    # The img tag will hold the actual resolution of the image file and its style
+    # will hold the desired size constraints.
+
+    if "style" in soup_img.attrs:
+        styles = tinycss2.parse_declaration_list(
+            soup_img["style"], skip_comments=True, skip_whitespace=True
+        )
+    else:
+        styles = []
+
+    for attr in ("height", "width"):
+        if attr in soup_img.attrs:
+            styles = [s for s in styles if s.lower_name != attr]
+
+            attr_value = soup_img[attr]
+
+            try:
+                float(attr_value)
+                attr_value += "px"
+            except ValueError:
+                pass
+
+            styles.append(
+                tinycss2.ast.Declaration(
+                    line=None,
+                    column=None,
+                    name=attr,
+                    lower_name=attr.lower(),
+                    value=[tinycss2.parse_one_component_value(attr_value)],
+                    important=False,
+                )
+            )
+
+    soup_img["style"] = tinycss2.serialize(styles)
 
     # Lazy + async load by default
     # There is an open docutils feature request
     # (https://sourceforge.net/p/docutils/feature-requests/78/)
     # adding support for lazy loading that will probably target
     # docutils 0.18. lazy loading can probably be removed from
     # here at that point unless we'd like to continue
@@ -371,15 +399,15 @@
     app.builder.copy_image_files = new_copy_image_files
 
 
 def setup(app: Sphinx) -> Dict[str, Any]:
     app.add_config_value("max_viewport_width", 1000, "html")
     app.add_config_value("width_min", 500, "html")
     app.add_config_value("width_step", 300, "html")
-    app.add_config_value("photofinish_ci_only", True, "html")
+    app.add_config_value("photofinish_ci_only", False, "html")
     app.connect("builder-inited", builder_init, 1e99)
 
     return {
         "parallel_read_safe": True,
         "parallel_write_safe": False,
     }
```

### Comparing `sphinxext-photofinish-0.1.8/sphinxext/photofinish/svgtopng.py` & `sphinxext-photofinish-0.1.9/sphinxext/photofinish/svgtopng.py`

 * *Files identical despite different names*

### Comparing `sphinxext-photofinish-0.1.8/sphinxext_photofinish.egg-info/PKG-INFO` & `sphinxext-photofinish-0.1.9/sphinxext_photofinish.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,14 @@
 Metadata-Version: 2.1
 Name: sphinxext-photofinish
-Version: 0.1.8
+Version: 0.1.9
 Summary: Sphinx Extension that creates responsive images.
 Home-page: https://github.com/wpilibsuite/sphinxext-photofinish
 Author: WPILib
 Author-email: developers@wpilib.org
-License: UNKNOWN
-Platform: UNKNOWN
 Classifier: Environment :: Plugins
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Sphinx :: Extension
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
@@ -55,8 +53,8 @@
 
 `max_viewport_width` - This is maximum "viewable" size of images in your documentation. Typically, it's set to the width of your body. Responsive images are generated up to double of this value. Default is 1000.
 
 `width_min` - Minimum width of images to generate. Default is 500.
 
 `width_step` - The resolution to iterate over for generating images. EX: 500, 800, 1100. Default is 300.
 
-
+`photofinish_ci_only` - Should this extension only run if the `CI` environment variable is set? Default is False.
```

