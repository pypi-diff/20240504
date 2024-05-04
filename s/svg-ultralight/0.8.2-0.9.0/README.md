# Comparing `tmp/svg_ultralight-0.8.2.tar.gz` & `tmp/svg_ultralight-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\svg_ultralight-0.8.2.tar", last modified: Sat May 22 21:23:36 2021, max compression
+gzip compressed data, was "svg_ultralight-0.9.0.tar", last modified: Tue Nov 15 15:29:08 2022, max compression
```

## Comparing `svg_ultralight-0.8.2.tar` & `svg_ultralight-0.9.0.tar`

### file list

```diff
@@ -1,31 +1,32 @@
-drwxrwxrwx   0        0        0        0 2021-05-22 21:23:36.651883 svg_ultralight-0.8.2/
--rw-rw-rw-   0        0        0     1095 2021-05-22 16:11:52.000000 svg_ultralight-0.8.2/LICENSE.txt
--rw-rw-rw-   0        0        0       19 2021-05-22 16:11:52.000000 svg_ultralight-0.8.2/MANIFEST.in
--rw-rw-rw-   0        0        0    10794 2021-05-22 21:23:36.651883 svg_ultralight-0.8.2/PKG-INFO
--rw-rw-rw-   0        0        0     8643 2021-05-22 16:11:52.000000 svg_ultralight-0.8.2/README.md
--rw-rw-rw-   0        0        0       42 2021-05-22 21:23:36.652889 svg_ultralight-0.8.2/setup.cfg
--rw-rw-rw-   0        0        0      922 2021-05-22 21:22:58.000000 svg_ultralight-0.8.2/setup.py
-drwxrwxrwx   0        0        0        0 2021-05-22 21:23:36.616881 svg_ultralight-0.8.2/svg_ultralight/
--rw-rw-rw-   0        0        0      133 2021-05-22 16:11:52.000000 svg_ultralight-0.8.2/svg_ultralight/__init__.py
--rw-rw-rw-   0        0        0      742 2021-05-22 16:11:52.000000 svg_ultralight-0.8.2/svg_ultralight/animate.py
-drwxrwxrwx   0        0        0        0 2021-05-22 21:23:36.640880 svg_ultralight-0.8.2/svg_ultralight/constructors/
--rw-rw-rw-   0        0        0      130 2021-05-22 16:11:52.000000 svg_ultralight-0.8.2/svg_ultralight/constructors/__init__.py
--rw-rw-rw-   0        0        0     3142 2021-05-22 21:22:58.000000 svg_ultralight-0.8.2/svg_ultralight/constructors/new_element.py
--rw-rw-rw-   0        0        0      801 2021-05-22 21:22:58.000000 svg_ultralight-0.8.2/svg_ultralight/nsmap.py
--rw-rw-rw-   0        0        0        0 2021-05-22 16:11:52.000000 svg_ultralight-0.8.2/svg_ultralight/py.typed
--rw-rw-rw-   0        0        0    11065 2021-05-22 21:22:58.000000 svg_ultralight-0.8.2/svg_ultralight/query.py
--rw-rw-rw-   0        0        0     4144 2021-05-22 16:11:52.000000 svg_ultralight-0.8.2/svg_ultralight/string_conversion.py
-drwxrwxrwx   0        0        0        0 2021-05-22 21:23:36.643881 svg_ultralight-0.8.2/svg_ultralight/strings/
--rw-rw-rw-   0        0        0       26 2021-05-22 16:11:52.000000 svg_ultralight-0.8.2/svg_ultralight/strings/__init__.py
--rw-rw-rw-   0        0        0     1200 2021-05-22 16:11:52.000000 svg_ultralight-0.8.2/svg_ultralight/strings/svg_strings.py
--rw-rw-rw-   0        0        0     9278 2021-05-22 21:22:58.000000 svg_ultralight-0.8.2/svg_ultralight/svg_ultralight.py
-drwxrwxrwx   0        0        0        0 2021-05-22 21:23:36.637881 svg_ultralight-0.8.2/svg_ultralight.egg-info/
--rw-rw-rw-   0        0        0    10794 2021-05-22 21:23:36.000000 svg_ultralight-0.8.2/svg_ultralight.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      655 2021-05-22 21:23:36.000000 svg_ultralight-0.8.2/svg_ultralight.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2021-05-22 21:23:36.000000 svg_ultralight-0.8.2/svg_ultralight.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        5 2021-05-22 21:23:36.000000 svg_ultralight-0.8.2/svg_ultralight.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2021-05-22 21:23:36.000000 svg_ultralight-0.8.2/svg_ultralight.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2021-05-22 21:23:36.649882 svg_ultralight-0.8.2/test/
--rw-rw-rw-   0        0        0     2797 2021-05-22 16:11:52.000000 svg_ultralight-0.8.2/test/test_new_element.py
--rw-rw-rw-   0        0        0     3054 2021-05-22 21:22:58.000000 svg_ultralight-0.8.2/test/test_queries.py
--rw-rw-rw-   0        0        0     6676 2021-05-22 16:11:52.000000 svg_ultralight-0.8.2/test/test_svg_ultralight.py
+drwxrwxrwx   0        0        0        0 2022-11-15 15:29:08.328832 svg_ultralight-0.9.0/
+-rw-rw-rw-   0        0        0     1095 2022-11-14 14:16:58.000000 svg_ultralight-0.9.0/LICENSE.txt
+-rw-rw-rw-   0        0        0       19 2022-11-14 14:16:58.000000 svg_ultralight-0.9.0/MANIFEST.in
+-rw-rw-rw-   0        0        0     8839 2022-11-15 15:29:08.327839 svg_ultralight-0.9.0/PKG-INFO
+-rw-rw-rw-   0        0        0     8383 2022-11-15 15:15:39.000000 svg_ultralight-0.9.0/README.md
+-rw-rw-rw-   0        0        0       95 2022-11-15 15:15:39.000000 svg_ultralight-0.9.0/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2022-11-15 15:29:08.329518 svg_ultralight-0.9.0/setup.cfg
+-rw-rw-rw-   0        0        0      786 2022-11-15 15:15:39.000000 svg_ultralight-0.9.0/setup.py
+drwxrwxrwx   0        0        0        0 2022-11-15 15:29:08.259079 svg_ultralight-0.9.0/svg_ultralight/
+-rw-rw-rw-   0        0        0      137 2022-11-15 15:15:39.000000 svg_ultralight-0.9.0/svg_ultralight/__init__.py
+-rw-rw-rw-   0        0        0     1052 2022-11-15 15:15:39.000000 svg_ultralight-0.9.0/svg_ultralight/animate.py
+drwxrwxrwx   0        0        0        0 2022-11-15 15:29:08.293355 svg_ultralight-0.9.0/svg_ultralight/constructors/
+-rw-rw-rw-   0        0        0      157 2022-11-15 15:15:39.000000 svg_ultralight-0.9.0/svg_ultralight/constructors/__init__.py
+-rw-rw-rw-   0        0        0     3137 2022-11-15 15:15:39.000000 svg_ultralight-0.9.0/svg_ultralight/constructors/new_element.py
+-rw-rw-rw-   0        0        0     9682 2022-11-15 15:15:39.000000 svg_ultralight-0.9.0/svg_ultralight/main.py
+-rw-rw-rw-   0        0        0      801 2022-11-15 00:46:08.000000 svg_ultralight-0.9.0/svg_ultralight/nsmap.py
+-rw-rw-rw-   0        0        0        0 2022-11-15 09:03:25.000000 svg_ultralight-0.9.0/svg_ultralight/py.typed
+-rw-rw-rw-   0        0        0    13419 2022-11-15 15:15:39.000000 svg_ultralight-0.9.0/svg_ultralight/query.py
+-rw-rw-rw-   0        0        0     4204 2022-11-15 15:15:39.000000 svg_ultralight-0.9.0/svg_ultralight/string_conversion.py
+drwxrwxrwx   0        0        0        0 2022-11-15 15:29:08.300977 svg_ultralight-0.9.0/svg_ultralight/strings/
+-rw-rw-rw-   0        0        0       26 2022-11-14 14:16:58.000000 svg_ultralight-0.9.0/svg_ultralight/strings/__init__.py
+-rw-rw-rw-   0        0        0     1255 2022-11-15 15:15:39.000000 svg_ultralight-0.9.0/svg_ultralight/strings/svg_strings.py
+drwxrwxrwx   0        0        0        0 2022-11-15 15:29:08.281381 svg_ultralight-0.9.0/svg_ultralight.egg-info/
+-rw-rw-rw-   0        0        0     8839 2022-11-15 15:29:08.000000 svg_ultralight-0.9.0/svg_ultralight.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      660 2022-11-15 15:29:08.000000 svg_ultralight-0.9.0/svg_ultralight.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2022-11-15 15:29:08.000000 svg_ultralight-0.9.0/svg_ultralight.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        5 2022-11-15 15:29:08.000000 svg_ultralight-0.9.0/svg_ultralight.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2022-11-15 15:29:08.000000 svg_ultralight-0.9.0/svg_ultralight.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2022-11-15 15:29:08.319173 svg_ultralight-0.9.0/test/
+-rw-rw-rw-   0        0        0     2373 2022-11-15 15:15:39.000000 svg_ultralight-0.9.0/test/test_new_element.py
+-rw-rw-rw-   0        0        0     3825 2022-11-15 15:15:39.000000 svg_ultralight-0.9.0/test/test_queries.py
+-rw-rw-rw-   0        0        0     6624 2022-11-15 15:15:39.000000 svg_ultralight-0.9.0/test/test_svg_ultralight.py
```

### Comparing `svg_ultralight-0.8.2/LICENSE.txt` & `svg_ultralight-0.9.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `svg_ultralight-0.8.2/README.md` & `svg_ultralight-0.9.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -17,37 +17,32 @@
     height_: Optional[float],
     pad_: float = 0
     dpu_: float = 1
     nsmap: Optional[Dict[str, str]] = None (svg_ultralight.NSMAP if None)
     **attributes: Union[float, str],
     -> etree.Element
 
-Create an svg root element from viewBox style arguments and provide the necessary svg-specific attributes and
-namespaces. This is your window onto the scene.
+Create an svg root element from viewBox style arguments and provide the necessary svg-specific attributes and namespaces. This is your window onto the scene.
 
 Three ways to call:
 
-1. The trailing-underscore arguments are the same you'd use to create a `rect` element (plus `pad_` and `dpu_`).
-`new_svg_root` will infer `viewBox`, `width`, and `height` svg attributes from these values.
+1. The trailing-underscore arguments are the same you'd use to create a `rect` element (plus `pad_` and `dpu_`).  `new_svg_root` will infer `viewBox`, `width`, and `height` svg attributes from these values.
 2. Use the svg attributes you already know: `viewBox`, `width`, `height`, etc. These will be written to the xml file.
 3. Of course, you can combine 1. and 2. if you know what you're doing.
 
 See `namespaces` below.
 
 * `x_`: x value in upper-left corner
 * `y_`: y value in upper-left corner
 * `width_`: width of viewBox
 * `height_`: height of viewBox
 * `pad_`: the one small convenience I've provided. Optionally increase viewBox by `pad` in all directions.
 * `dpu_`: pixels per viewBox unit for output png images.
-* `nsmap`: namespaces. (defaults to svg_ultralight.NSMAP). Available as an argument should you wish to add additional
-namespaces. To do this, add items to NSMAP then call with `nsmap=NSMAP`.
-* `**attributes`: the trailing-underscore arguments are an *optional* shortcut for creating a scene. The entire svg
-interface is available to you through kwargs. See `A few helpers` below for details on attribute-name translation
-between Python and xml (the short version: `this_name` becomes `this-name` and `this_` becomes `this`)
+* `nsmap`: namespaces. (defaults to svg_ultralight.NSMAP). Available as an argument should you wish to add additional namespaces. To do this, add items to NSMAP then call with `nsmap=NSMAP`.
+* `**attributes`: the trailing-underscore arguments are an *optional* shortcut for creating a scene. The entire svg interface is available to you through kwargs. See `A few helpers` below for details on attribute-name translation between Python and xml (the short version: `this_name` becomes `this-name` and `this_` becomes `this`)
 
 ### namespaces (svg_ultralight.NSMAP)
 
 `new_svg_root` will create a root with several available namespaces.
 
 * `"dc": "http://purl.org/dc/elements/1.1/"`
 * `"cc": "http://creativecommons.org/ns#"`
@@ -162,48 +157,35 @@
 As above, but creates a subelement.
 
     >>> parent = etree.Element('g')
     >>> _ = new_sub_element('rect')
     >>> etree.tostring(parent)
     b'<g><rect/></g>'
     
-### update_element and deepcopy_element
+### update_element
 
-These are two more ways to add params with the above-described name and type conversion. Again unnecessary, but
-potentially helpful. Easily understood from the code or docstrings.
+Another way to add params through the new_element name / float translator. Again unnecessary, but potentially helpful. Easily understood from the code or docstrings.
     
 ## Extras:
 
 ### query.map_ids_to_bounding_boxes
 
-Python cannot parse an svg file. Python can *create* an svg file, and Inkscape can parse (and inspect) it. Inkscape has
-a command-line interface capable of reading an svg file and returning some limited information. This is the only way I
-know for a Python program to:
+Python cannot parse an svg file. Python can *create* an svg file, and Inkscape can parse (and inspect) it. Inkscape has a command-line interface capable of reading an svg file and returning some limited information. This is the only way I know for a Python program to:
 
 1. create an svg file (optionally without writing to filesystem)
 2. query the svg file for bounding-box information
 3. create an adjusted svg file.
 
 This would be necessary for, e.g., algorithmically fitting text in a box.
 
     from svg_ultralight.queries import map_ids_to_bounding_boxes
 
-You can get a tiny bit more sophisticated with Inkscape bounding-box queries, but not much. This will give you pretty
-much all you can get out of it.
-
-### query.get_bounding_box
-
-Get the bounding box around an svg element. Works with group elements.
-
-Internally, this just creates an svg file around your element then calls `map_ids_to_bounding_boxes`.
-
-    from svg_ultralight.queries import get_bounding_box
+You can get a tiny bit more sophisticated with Inkscape bounding-box queries, but not much. This will give you pretty much all you can get out of it.
 
 ### animate.write_gif
 
-Create an animated gif from a sequence of png filenames. This is a Pillow one-liner, but it's convenient for me to have
-it, so it might be convenient for you.
+Create an animated gif from a sequence of png filenames. This is a Pillow one-liner, but it's convenient for me to have it, so it might be convenient for you. Requires pillow, which is not a project dependency.
 
     from svg_ultralight.animate import write_gif
     
 [Full Documentation and Tutorial](https://shayallenhill.com/svg-with-css-in-python/)
```

### Comparing `svg_ultralight-0.8.2/setup.py` & `svg_ultralight-0.9.0/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,27 +1,23 @@
 import setuptools
 
 with open("README.md") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="svg_ultralight",
-    version="0.8.2",
+    version="0.9.0",
     author="Shay Hill",
     author_email="shay_public@hotmail.com",
     description="Write SVG files with Python.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/ShayHill/svg_ultralight",
     package_data={"svg_ultralight": ["py.typed"]},
     packages=setuptools.find_packages(),
-    # package_dir={
-    #     "svg_ultralight": "svg_ultralight",
-    #     "svg_ultralight.constructors": "constructors",
-    # },
     install_requires=["lxml"],
     tests_require=["pytest"],
     python_requires=">=3.6",
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
```

### Comparing `svg_ultralight-0.8.2/svg_ultralight/constructors/new_element.py` & `svg_ultralight-0.9.0/svg_ultralight/constructors/new_element.py`

 * *Files 20% similar despite different names*

```diff
@@ -8,23 +8,24 @@
 This is principally to allow passing values, rather than strings, as svg element
 parameters.
 
 Will translate ``stroke_width=10`` to ``stroke-width="10"``
 """
 
 import copy
-from typing import Union
+from typing import TypeAlias, Union
 
-from lxml import etree  # type: ignore
+from lxml import etree
 
-from ..string_conversion import set_attributes
+from svg_ultralight.string_conversion import set_attributes
 
+_Element: TypeAlias = etree._Element  # type: ignore
 
-def new_element(tag: str, **attributes: Union[str, float]) -> etree.Element:
-    # noinspection PyShadowingNames
+
+def new_element(tag: str, **attributes: Union[str, float]) -> _Element:
     """
     Create an etree.Element, make every kwarg value a string.
 
     :param tag: element tag
     :param attributes: element attribute names and values
     :returns: new ``tag`` element
 
@@ -53,17 +54,16 @@
     """
     elem = etree.Element(tag)
     set_attributes(elem, **attributes)
     return elem
 
 
 def new_sub_element(
-    parent: etree.Element, tag: str, **attributes: Union[str, float]
-) -> etree.Element:
-    # noinspection PyShadowingNames
+    parent: _Element, tag: str, **attributes: Union[str, float]
+) -> _Element:
     """
     Create an etree.SubElement, make every kwarg value a string.
 
     :param parent: parent element
     :param tag: element tag
     :param attributes: element attribute names and values
     :returns: new ``tag`` element
@@ -74,40 +74,33 @@
         b'<g><rect/></g>'
     """
     elem = etree.SubElement(parent, tag)
     set_attributes(elem, **attributes)
     return elem
 
 
-def update_element(
-    elem: etree.Element, **attributes: Union[str, float]
-) -> etree.Element:
+def update_element(elem: _Element, **attributes: Union[str, float]) -> _Element:
     """
     Update an existing etree.Element with additional params.
 
     :param elem: at etree element
     :param attributes: element attribute names and values
     """
     set_attributes(elem, **attributes)
     return elem
 
 
-def deepcopy_element(
-    elem: etree.Element, **attributes: Union[str, float]
-) -> etree.Element:
+def deepcopy_element(elem: _Element, **attributes: str | float) -> _Element:
     """
     Create a deepcopy of an element. Optionally pass additional params.
 
-    :param elem: at etree element
+    :param elem: at etree element or list of elements
     :param attributes: element attribute names and values
+    :returns: a deepcopy of the element with updated attributes
     """
-    if isinstance(elem, list):
-        return [deepcopy_element(x, **attributes) for x in elem]
+    raise DeprecationWarning(
+        "deepcopy_element is deprecated. "
+        + "Use copy.deepcopy from the standard library instead."
+    )
     elem = copy.deepcopy(elem)
-    update_element(elem, **attributes)
+    _ = update_element(elem, **attributes)
     return elem
-
-
-if __name__ == "__main__":
-    import doctest
-
-    doctest.testmod()
```

### Comparing `svg_ultralight-0.8.2/svg_ultralight/nsmap.py` & `svg_ultralight-0.9.0/svg_ultralight/nsmap.py`

 * *Files identical despite different names*

### Comparing `svg_ultralight-0.8.2/svg_ultralight/query.py` & `svg_ultralight-0.9.0/svg_ultralight/query.py`

 * *Files 15% similar despite different names*

```diff
@@ -11,31 +11,47 @@
 business card). Getting bounding boxes from Inkscape is not exceptionally fast.
 """
 
 from __future__ import annotations
 
 import os
 import re
+import uuid
 from dataclasses import dataclass
+from pathlib import Path
 from subprocess import PIPE, Popen
 from tempfile import NamedTemporaryFile
-from typing import Dict
+from typing import TypeAlias
+from copy import deepcopy
 
-from lxml import etree  # type: ignore
+from lxml import etree
 
-from svg_ultralight import write_svg
-from .constructors import deepcopy_element
-from .strings import format_number
-from .svg_ultralight import new_svg_root
+from svg_ultralight.main import new_svg_root, write_svg
+from svg_ultralight.strings import format_number
+
+_Element: TypeAlias = etree._Element  # type: ignore
 
 
 @dataclass
 class BoundingBox:
-    """
-    Mutable bounding box object for svg_ultralight.
+    """Mutable bounding box object for svg_ultralight.
+
+    :param x: left x value
+    :param y: top y value
+    :param width: width of the bounding box
+    :param height: height of the bounding box
+
+    The below optional parameters, in addition to the required parameters, capture
+    the entire state of a BoundingBox instance.  They could be used to make a copy or
+    to initialize a transformed box with the same transform_string as another box.
+    Under most circumstances, they will not be used.
+
+    :param scale: scale of the bounding box
+    :param translation_x: x translation of the bounding box
+    :param translation_y: y translation of the bounding box
 
     Functions that return a bounding box will return a BoundingBox instance. This
     instance can be transformed (uniform scale and translate only). Transformations
     will be combined and scored to be passed to new_element as a transform value.
 
     Define the bbox with x=, y=, width=, height=
 
@@ -73,34 +89,25 @@
         # stack a on top of b
         bbox_a.y2 = bbox_b.y
 
         update_element(elem_a, transform=bbox_a.transform_string)
         update_element(elem_b, transform=bbox_b.transform_string)
     """
 
-    def __init__(self, x: float, y: float, width: float, height: float) -> None:
-        """
-        Pass input values to private members. Initialize the transformation variables
-
-        These private members will store the untransformed bbox position and size.
-        """
-        self._x = x
-        self._y = y
-        self._width = width
-        self._height = height
-
-        # transformation values
-        self._scale: float = 1
-        self._translation_x: float = 0
-        self._translation_y: float = 0
+    _x: float
+    _y: float
+    _width: float
+    _height: float
+    _scale: float = 1.0
+    _translation_x: float = 0.0
+    _translation_y: float = 0.0
 
     @property
     def scale(self) -> float:
-        """
-        Read-only scale.
+        """Read-only scale.
 
         self.scale is publicly visible, because it's convenient to fit a (usually
         text) element somewhere then scale other elements to the same size--even
         though element width and height may be different. This is a read-only
         attribute, because writing it would cause too many errors of intuition (would
         the scaled element stay anchored to x and y?).
 
@@ -110,214 +117,244 @@
         This is consistent with setting width any other way: the element will still
         be anchored at self.x and self.y.
         """
         return self._scale
 
     @property
     def x(self) -> float:
-        """
-        x left value of bounding box
-        """
+        """x left value of bounding box"""
         return (self._translation_x + self._x) * self._scale
 
     @x.setter
-    def x(self, x) -> None:
-        """
-        Update transform values (do not alter self._x)
-        """
+    def x(self, x: float) -> None:
+        """Update transform values (do not alter self._x)"""
         self._add_transform(1, x - self.x, 0)
 
     @property
     def y(self) -> float:
-        """
-        y top value of bounding box
-        """
+        """y top value of bounding box"""
         return (self._translation_y + self._y) * self._scale
 
     @y.setter
-    def y(self, y) -> None:
-        """
-        Update transform values (do not alter self._y)
-        """
+    def y(self, y: float) -> None:
+        """Update transform values (do not alter self._y)"""
         self._add_transform(1, 0, y - self.y)
 
     @property
     def x2(self) -> float:
-        """
-        x right value of bounding box
-        """
+        """x right value of bounding box"""
         return self.x + self.width
 
     @x2.setter
-    def x2(self, x2) -> None:
-        """
-        Update transform values (do not alter self._x)
-        """
+    def x2(self, x2: float) -> None:
+        """Update transform values (do not alter self._x)"""
         self.x = x2 - self.width
 
     @property
     def y2(self) -> float:
-        """
-        y bottom value of bounding box
-        """
+        """y bottom value of bounding box"""
         return self.y + self.height
 
     @y2.setter
-    def y2(self, y2) -> None:
-        """
-        Update transform values (do not alter self._y)
-        """
+    def y2(self, y2: float) -> None:
+        """Update transform values (do not alter self._y)"""
         self.y = y2 - self.height
 
     @property
     def width(self) -> float:
-        """
-        Width of transformed bounding box
-        """
+        """Width of transformed bounding box"""
         return self._width * self._scale
 
     @width.setter
     def width(self, width: float) -> None:
-        """
-        Update transform values, Do not alter self._width.
+        """Update transform values, Do not alter self._width.
 
         Here transformed x and y value will be preserved. That is, the bounding box
         is scaled, but still anchored at (transformed) self.x and self.y
         """
         current_x = self.x
         current_y = self.y
         self._scale *= width / self.width
         self.x = current_x
         self.y = current_y
 
     @property
     def height(self) -> float:
-        """
-        Height of transformed bounding box
-        """
+        """Height of transformed bounding box"""
         return self._height * self._scale
 
     @height.setter
     def height(self, height: float) -> None:
-        """
-        Update transform values, Do not alter self._height.
+        """Update transform values, Do not alter self._height.
 
         Here transformed x and y value will be preserved. That is, the bounding box
         is scaled, but still anchored at (transformed) self.x and self.y
         """
         self.width = height * self.width / self.height
 
-    def _asdict(self):
-        """
-        For passing transformed bounding box values into a rect element or another bbox
-
-        I would make this a public (no underscore) property (no parenthesis). Keeping
-        it this way to mirror the ``_asdict`` method of namedtuple.
-        """
-        return {x: getattr(self, x) for x in ("x", "y", "width", "height")}
-
     def _add_transform(self, scale: float, translation_x: float, translation_y: float):
-        """
-        Transform the bounding box by updating the transformation attributes
+        """Transform the bounding box by updating the transformation attributes
 
         Transformation attributes are _translation_x, _translation_y, and _scale
         """
         self._translation_x += translation_x / self._scale
         self._translation_y += translation_y / self._scale
         self._scale *= scale
 
     @property
     def transform_string(self) -> str:
-        """
-        Transformation property string value for svg element.
+        """Transformation property string value for svg element.
 
         :return: string value for an svg transform attribute.
 
         Use with
         ``update_element(elem, transform=bbox.transform_string)``
         """
         transformation_values = (
             format_number(x)
             for x in (self._scale, self._translation_x, self._translation_y)
         )
         return "scale({}) translate({} {})".format(*transformation_values)
 
-    def merge(self, *others) -> BoundingBox:
-        """
-        Create a bounding box around all other bounding boxes.
+    def merge(self, *others: BoundingBox) -> BoundingBox:
+        """Create a bounding box around all other bounding boxes.
 
         :param others: one or more bounding boxes to merge with self
         :return: a bounding box around self and other bounding boxes
         """
-        bboxes = (self,) + others
+        raise DeprecationWarning(
+            "Method a.merge(b, c) is deprecated. "
+            + "Use classmethod BoundingBox.merged(a, b, c) instead."
+        )
+        return BoundingBox.merged(self, *others)
+
+    @classmethod
+    def merged(cls, *bboxes: BoundingBox) -> BoundingBox:
+        """Create a bounding box around all other bounding boxes.
+
+        This can be used to repace a bounding box after the element it bounds has
+        been transformed with instance.transform_string.
+
+        :param others: one or more bounding boxes
+        :return: a bounding box encompasing all bboxes args
+        """
+        if not bboxes:
+            raise ValueError("At least one bounding box is required")
         min_x = min(x.x for x in bboxes)
         max_x = max(x.x + x.width for x in bboxes)
         min_y = min(x.y for x in bboxes)
         max_y = max(x.y + x.height for x in bboxes)
         return BoundingBox(min_x, min_y, max_x - min_x, max_y - min_y)
 
 
-def map_ids_to_bounding_boxes(
-    inkscape: str,
-    xml: etree.Element,
-) -> Dict[str, BoundingBox]:
-    # noinspection SpellCheckingInspection
+def _fill_ids(*elem_args: _Element) -> None:
+    """Set the id attribute of an element and all its children. Keep existing ids.
+
+    :param elem: an etree element, accepts multiple arguments
     """
-    Query an svg file for bounding-box dimensions
+    if not elem_args:
+        return
+    elem = elem_args[0]
+    for child in elem:
+        _ = _fill_ids(child)
+    if elem.get("id") is None:
+        elem.set("id", f"svg_ul-{uuid.uuid4()}")
+    _fill_ids(*elem_args[1:])
+
+
+def _normalize_views(elem: _Element) -> None:
+    """Create a square viewbox for any element with an svg tag.
+
+    :param elem: an etree element
+
+    This prevents the bounding boxes from being distorted. Only do this to copies,
+    because there's no way to undo it.
+    """
+    for child in elem:
+        _ = _normalize_views(child)
+    if str(elem.tag).endswith("svg"):
+        elem.set("viewBox", "0 0 1 1")
+        elem.set("width", "1")
+        elem.set("height", "1")
+
+
+def _envelop_copies(*elem_args: _Element) -> _Element:
+    """An svg root element containing all elem_args.
+
+    :param elem_args: one or more etree elements
+    :return: an etree element enveloping copies of elem_args with all views normalized
+    """
+    envelope = new_svg_root(0, 0, 1, 1, id_=f"envelope_{uuid.uuid4()}")
+    envelope.extend(deepcopy(e) for e in elem_args)
+    _normalize_views(envelope)
+    return envelope
+
+
+def map_ids_to_bounding_boxes(
+    inkscape: str | Path, *elem_args: _Element
+) -> dict[str, BoundingBox]:
+    """Query an svg file for bounding-box dimensions
 
     :param inkscape: path to an inkscape executable on your local file system
         IMPORTANT: path cannot end with ``.exe``.
         Use something like ``"C:\\Program Files\\Inkscape\\inkscape"``
-
-    PROVIDE ONE OF:
-    :param xml: xml element (written to a temporary file then queried)
-
+    :param elem_args: xml element (written to a temporary file then queried)
     :return: svg element ids (and a bounding box for the entire svg file as ``svg``)
         mapped to (x, y, width, height)
+    :effects: adds an id attribute to any element without one. These will all have
+        the prefix svg_ul-, so you can find and remove them later if desired.
 
     Bounding boxes are relative to svg viewbox. If viewbox x == -10,
-    all bounding-box x values will be offset -10.
+    all bounding-box x values will be offset -10. So, everything is wrapped in a root
+    element with a "normalized" viewbox, (viewbox=(0, 0, 1, 1)) then any child root
+    elements ("child root elements" sounds wrong, but it works) viewboxes are
+    normalized as well. This works even with a root element around a root element, so
+    input elem_args can be root elements or "normal" elements like "rect", "circle",
+    or "text" or a mixture of both.
 
     The ``inkscape --query-all svg`` call will return a tuple:
 
     (b'svg1,x,y,width,height\\r\\elem1,x,y,width,height\\r\\n', None)
     where x, y, width, and height are strings of numbers.
 
     This calls the command and formats the output into a dictionary.
 
     dpu_ arguments to new_svg_root transform the bounding boxes in non-useful ways.
     This copies all elements except the root element in to a (0, 0, 1, 1) root. This
     will put the boxes where you'd expect them to be, no matter what root you use.
     """
-    xml_prime = new_svg_root(0, 0, 1, 1)
-    xml_prime.extend((deepcopy_element(x) for x in xml))
+    _fill_ids(*elem_args)
+    envelope = _envelop_copies(*elem_args)
+
     with NamedTemporaryFile(mode="wb", delete=False, suffix=".svg") as svg_file:
-        svg = write_svg(svg_file, xml_prime)
+        svg = write_svg(svg_file, envelope)
 
     bb_process = Popen(f'"{inkscape}" --query-all {svg}', stdout=PIPE)
     bb_data = str(bb_process.communicate()[0])[2:-1]
     bb_strings = re.split(r"[\\r]*\\n", bb_data)[:-1]
     os.unlink(svg_file.name)
 
-    id2bbox = {}
+    id2bbox: dict[str, BoundingBox] = {}
     for id_, *bounds in (x.split(",") for x in bb_strings):
         id2bbox[id_] = BoundingBox(*(float(x) for x in bounds))
     return id2bbox
 
 
-def get_bounding_box(inkscape: str, elem: etree.Element) -> BoundingBox:
-    """
-    Get bounding box around a single element.
+def get_bounding_box(inkscape: str | Path, elem: _Element) -> BoundingBox:
+    """Get bounding box around a single element.
 
     :param inkscape: path to an inkscape executable on your local file system
         IMPORTANT: path cannot end with ``.exe``.
         Use something like ``"C:\\Program Files\\Inkscape\\inkscape"``
-    :param elem: xml element
+    :param elem_args: xml elements
     :return: a BoundingBox instance around elem.
 
     This will work most of the time, but if you're missing an nsmap, you'll need to
     create an entire xml file with a custom nsmap (using
     `svg_ultralight.new_svg_root`) then call `map_ids_to_bounding_boxes` directly.
     """
-    temp_screen = new_svg_root(0, 0, 1, 1)
-    temp_screen.append(deepcopy_element(elem))
-    return list(map_ids_to_bounding_boxes(inkscape, xml=temp_screen).values())[1]
+    raise DeprecationWarning(
+        "get_bounding_box is deprecated. "
+        + "Use map_ids_to_bounding_boxes(elem)[id] instead."
+    )
+    id2bbox = map_ids_to_bounding_boxes(inkscape, elem)
+    return id2bbox[elem.attrib["id"]]
```

### Comparing `svg_ultralight-0.8.2/svg_ultralight/string_conversion.py` & `svg_ultralight-0.9.0/svg_ultralight/string_conversion.py`

 * *Files 10% similar despite different names*

```diff
@@ -15,245 +15,249 @@
 000000e0: 6c6f 6174 7320 746f 2073 6978 2064 6967  loats to six dig
 000000f0: 6974 7320 6166 7465 7220 7468 6520 6465  its after the de
 00000100: 6369 6d61 6c0d 0a2a 2052 6f75 6e64 696e  cimal..* Roundin
 00000110: 6720 7669 6577 426f 7820 6469 6d65 6e73  g viewBox dimens
 00000120: 696f 6e73 2074 6f20 696e 7473 0d0a 2222  ions to ints..""
 00000130: 220d 0a66 726f 6d20 656e 756d 2069 6d70  "..from enum imp
 00000140: 6f72 7420 456e 756d 0d0a 6672 6f6d 2074  ort Enum..from t
-00000150: 7970 696e 6720 696d 706f 7274 2055 6e69  yping import Uni
-00000160: 6f6e 0d0a 0d0a 6672 6f6d 206c 786d 6c20  on....from lxml 
-00000170: 696d 706f 7274 2065 7472 6565 0d0a 6672  import etree..fr
-00000180: 6f6d 202e 6e73 6d61 7020 696d 706f 7274  om .nsmap import
-00000190: 204e 534d 4150 0d0a 0d0a 0d0a 6465 6620   NSMAP......def 
-000001a0: 666f 726d 6174 5f6e 756d 6265 7228 6e75  format_number(nu
-000001b0: 6d3a 2066 6c6f 6174 2920 2d3e 2073 7472  m: float) -> str
-000001c0: 3a0d 0a20 2020 2022 2222 0d0a 2020 2020  :..    """..    
-000001d0: 466f 726d 6174 2073 7472 696e 6773 2061  Format strings a
-000001e0: 7420 6c69 6d69 7465 6420 7072 6563 6973  t limited precis
-000001f0: 696f 6e0d 0a0d 0a20 2020 203a 7061 7261  ion....    :para
-00000200: 6d20 6e75 6d3a 2061 6e79 7468 696e 6720  m num: anything 
-00000210: 7468 6174 2063 616e 2070 7269 6e74 2061  that can print a
-00000220: 7320 6120 666c 6f61 742e 0d0a 2020 2020  s a float...    
-00000230: 3a72 6574 7572 6e3a 2073 7472 0d0a 0d0a  :return: str....
-00000240: 2020 2020 4927 7665 2072 6561 6420 6172      I've read ar
-00000250: 7469 636c 6573 2074 6861 7420 7265 636f  ticles that reco
-00000260: 6d6d 656e 6420 6e6f 206d 6f72 6520 7468  mmend no more th
-00000270: 616e 2066 6f75 7220 6469 6769 7473 2062  an four digits b
-00000280: 6566 6f72 6520 616e 6420 7477 6f20 6469  efore and two di
-00000290: 6769 7473 0d0a 2020 2020 6166 7465 7220  gits..    after 
-000002a0: 7468 6520 6465 6369 6d61 6c20 706f 696e  the decimal poin
-000002b0: 7420 746f 2065 6e73 7572 6520 676f 6f64  t to ensure good
-000002c0: 2073 7667 2072 656e 6465 7269 6e67 2e20   svg rendering. 
-000002d0: 4927 6d20 6265 696e 6720 6765 6e65 726f  I'm being genero
-000002e0: 7573 2061 6e64 0d0a 2020 2020 6769 7669  us and..    givi
-000002f0: 6e67 2073 6978 2e20 4d6f 7374 6c79 2074  ng six. Mostly t
-00000300: 6f20 656c 696d 696e 6174 6520 6578 706f  o eliminate expo
-00000310: 6e65 6e74 6961 6c20 6e6f 7461 7469 6f6e  nential notation
-00000320: 2c20 6275 7420 4927 6d20 2272 7374 7269  , but I'm "rstri
-00000330: 7070 696e 6722 2074 6865 0d0a 2020 2020  pping" the..    
-00000340: 7374 7269 6e67 7320 746f 2072 6564 7563  strings to reduc
-00000350: 6520 6669 6c65 7369 7a65 2061 6e64 2069  e filesize and i
-00000360: 6e63 7265 6173 6520 7265 6164 6162 696c  ncrease readabil
-00000370: 6974 790d 0a20 2020 2022 2222 0d0a 2020  ity..    """..  
-00000380: 2020 7265 7475 726e 2066 227b 6e75 6d3a    return f"{num:
-00000390: 302e 3666 7d22 2e72 7374 7269 7028 2230  0.6f}".rstrip("0
-000003a0: 2229 2e72 7374 7269 7028 222e 2229 0d0a  ").rstrip(".")..
-000003b0: 0d0a 0d0a 6465 6620 7365 745f 6174 7472  ....def set_attr
-000003c0: 6962 7574 6573 2865 6c65 6d3a 2065 7472  ibutes(elem: etr
-000003d0: 6565 2e45 6c65 6d65 6e74 2c20 2a2a 6174  ee.Element, **at
-000003e0: 7472 6962 7574 6573 3a20 556e 696f 6e5b  tributes: Union[
-000003f0: 7374 722c 2066 6c6f 6174 5d29 202d 3e20  str, float]) -> 
-00000400: 4e6f 6e65 3a0d 0a20 2020 2022 2222 0d0a  None:..    """..
-00000410: 2020 2020 5365 7420 6e61 6d65 3a20 7661      Set name: va
-00000420: 6c75 6520 6974 656d 7320 6173 2065 6c65  lue items as ele
-00000430: 6d65 6e74 2061 7474 7269 6275 7465 732e  ment attributes.
-00000440: 204d 616b 6520 6576 6572 7920 7661 6c75   Make every valu
-00000450: 6520 6120 7374 7269 6e67 2e0d 0a0d 0a20  e a string..... 
-00000460: 2020 203a 7061 7261 6d20 656c 656d 3a20     :param elem: 
-00000470: 656c 656d 656e 7420 746f 2072 6563 6569  element to recei
-00000480: 7665 2065 6c65 6d65 6e74 2e73 6574 286b  ve element.set(k
-00000490: 6579 776f 7264 2c20 7374 7228 7661 6c75  eyword, str(valu
-000004a0: 6529 2920 6361 6c6c 730d 0a20 2020 203a  e)) calls..    :
-000004b0: 7061 7261 6d20 6174 7472 6962 7574 6573  param attributes
-000004c0: 3a20 656c 656d 656e 7420 6174 7472 6962  : element attrib
-000004d0: 7574 6520 6e61 6d65 7320 616e 6420 7661  ute names and va
-000004e0: 6c75 6573 2e20 4b6e 6f77 7320 7768 6174  lues. Knows what
-000004f0: 2074 6f20 646f 2077 6974 6820 2774 6578   to do with 'tex
-00000500: 7427 0d0a 2020 2020 2020 2020 6b65 7977  t'..        keyw
-00000510: 6f72 642e 5620 3a65 6666 6563 7473 3a20  ord.V :effects: 
-00000520: 7570 6461 7465 7320 6060 656c 656d 6060  updates ``elem``
-00000530: 0d0a 0d0a 2020 2020 5468 6973 2069 7320  ....    This is 
-00000540: 6a75 7374 2074 6f20 7361 7665 2061 206c  just to save a l
-00000550: 6f74 206f 6620 7479 7069 6e67 2e20 6574  ot of typing. et
-00000560: 7265 652e 456c 656d 656e 7473 2077 696c  ree.Elements wil
-00000570: 6c20 6f6e 6c79 2061 6363 6570 7420 7374  l only accept st
-00000580: 7269 6e67 0d0a 2020 2020 7661 6c75 6573  ring..    values
-00000590: 2e20 5461 6b65 7320 6561 6368 2069 6e20  . Takes each in 
-000005a0: 7061 7261 6d73 2e76 616c 7565 7328 292c  params.values(),
-000005b0: 2061 6e64 2070 6173 7365 7320 6974 2074   and passes it t
-000005c0: 6f20 6574 7265 652e 456c 656d 656e 7420  o etree.Element 
-000005d0: 6173 2061 0d0a 2020 2020 7374 7269 6e67  as a..    string
-000005e0: 2e20 5769 6c6c 2061 6c73 6f20 7265 706c  . Will also repl
-000005f0: 6163 6520 605f 6020 7769 7468 2060 2d60  ace `_` with `-`
-00000600: 2074 6f20 7472 616e 736c 6174 6520 7661   to translate va
-00000610: 6c69 6420 5079 7468 6f6e 2076 6172 6961  lid Python varia
-00000620: 626c 6520 6e61 6d65 730d 0a20 2020 2066  ble names..    f
-00000630: 6f72 2078 6d6c 2070 6172 616d 6574 6572  or xml parameter
-00000640: 206e 616d 6573 2e0d 0a0d 0a20 2020 2049   names.....    I
-00000650: 6e76 616c 6964 206e 616d 6573 2028 6120  nvalid names (a 
-00000660: 706f 7075 6c61 7220 6f6e 6520 7769 6c6c  popular one will
-00000670: 2062 6520 2763 6c61 7373 2729 2063 616e   be 'class') can
-00000680: 2062 6520 7061 7373 6564 2077 6974 6820   be passed with 
-00000690: 6120 7472 6169 6c69 6e67 0d0a 2020 2020  a trailing..    
-000006a0: 756e 6465 7273 636f 7265 2028 652e 672e  underscore (e.g.
-000006b0: 2c20 636c 6173 735f 3d27 626f 6479 5f74  , class_='body_t
-000006c0: 6578 7427 292e 0d0a 0d0a 2020 2020 5468  ext').....    Th
-000006d0: 6174 2773 2061 6c6d 6f73 7420 616c 6c2e  at's almost all.
-000006e0: 2054 6865 2066 756e 6374 696f 6e20 7769   The function wi
-000006f0: 6c6c 2061 6c73 6f20 6861 6e64 6c65 2074  ll also handle t
-00000700: 6865 2027 7465 7874 2720 6b65 7977 6f72  he 'text' keywor
-00000710: 642c 2070 6c61 6369 6e67 2074 6865 0d0a  d, placing the..
-00000720: 2020 2020 7661 6c75 6520 6265 7477 6565      value betwee
-00000730: 6e20 656c 656d 656e 7420 7461 6773 2e0d  n element tags..
-00000740: 0a0d 0a20 2020 2046 6f72 6d61 7420 666c  ...    Format fl
-00000750: 6f61 7473 2074 6872 6f75 6768 2066 277b  oats through f'{
-00000760: 7661 6c75 653a 667d 2074 6f20 6176 6f69  value:f} to avoi
-00000770: 6420 6578 706f 6e65 6e74 6961 6c20 7265  d exponential re
-00000780: 7072 6573 656e 7461 7469 6f6e 0d0a 2020  presentation..  
-00000790: 2020 2865 2e67 2e2c 2031 3065 2d30 3629    (e.g., 10e-06)
-000007a0: 2077 6869 6368 2073 7667 2070 6172 7365   which svg parse
-000007b0: 7273 2077 6f6e 2774 2075 6e64 6572 7374  rs won't underst
-000007c0: 616e 642e 0d0a 2020 2020 2222 220d 0a20  and...    """.. 
-000007d0: 2020 2064 6f74 7320 3d20 7b22 7465 7874     dots = {"text
-000007e0: 227d 0d0a 2020 2020 666f 7220 646f 7420  "}..    for dot 
-000007f0: 696e 2064 6f74 7320 2620 7365 7428 6174  in dots & set(at
-00000800: 7472 6962 7574 6573 293a 0d0a 2020 2020  tributes):..    
-00000810: 2020 2020 7365 7461 7474 7228 656c 656d      setattr(elem
-00000820: 2c20 646f 742c 2061 7474 7269 6275 7465  , dot, attribute
-00000830: 732e 706f 7028 646f 7429 290d 0a0d 0a20  s.pop(dot)).... 
-00000840: 2020 2066 6f72 206b 2c20 7620 696e 2061     for k, v in a
-00000850: 7474 7269 6275 7465 732e 6974 656d 7328  ttributes.items(
-00000860: 293a 0d0a 2020 2020 2020 2020 6966 2022  ):..        if "
-00000870: 3a22 2069 6e20 6b3a 0d0a 2020 2020 2020  :" in k:..      
-00000880: 2020 2020 2020 6e61 6d65 7370 6163 652c        namespace,
-00000890: 2074 6167 203d 206b 2e73 706c 6974 2822   tag = k.split("
-000008a0: 3a22 290d 0a20 2020 2020 2020 2020 2020  :")..           
-000008b0: 206b 203d 2065 7472 6565 2e51 4e61 6d65   k = etree.QName
-000008c0: 284e 534d 4150 5b6e 616d 6573 7061 6365  (NSMAP[namespace
-000008d0: 5d2c 2074 6167 290d 0a20 2020 2020 2020  ], tag)..       
-000008e0: 2065 6c73 653a 0d0a 2020 2020 2020 2020   else:..        
-000008f0: 2020 2020 6b20 3d20 6b2e 7273 7472 6970      k = k.rstrip
-00000900: 2822 5f22 292e 7265 706c 6163 6528 225f  ("_").replace("_
-00000910: 222c 2022 2d22 290d 0a20 2020 2020 2020  ", "-")..       
-00000920: 2074 7279 3a0d 0a20 2020 2020 2020 2020   try:..         
-00000930: 2020 2076 616c 203d 2066 6f72 6d61 745f     val = format_
-00000940: 6e75 6d62 6572 2876 290d 0a20 2020 2020  number(v)..     
-00000950: 2020 2065 7863 6570 7420 5661 6c75 6545     except ValueE
-00000960: 7272 6f72 3a0d 0a20 2020 2020 2020 2020  rror:..         
-00000970: 2020 2076 616c 203d 2073 7472 2876 290d     val = str(v).
-00000980: 0a20 2020 2020 2020 2065 6c65 6d2e 7365  .        elem.se
-00000990: 7428 6b2c 2076 616c 290d 0a0d 0a0d 0a63  t(k, val)......c
-000009a0: 6c61 7373 205f 546f 7374 7269 6e67 4465  lass _TostringDe
-000009b0: 6661 756c 7473 2845 6e75 6d29 3a0d 0a20  faults(Enum):.. 
-000009c0: 2020 2022 2222 4465 6661 756c 7420 7661     """Default va
-000009d0: 6c75 6573 2066 6f72 2061 6e20 7376 6720  lues for an svg 
-000009e0: 786d 6c5f 6865 6164 6572 2222 220d 0a0d  xml_header"""...
-000009f0: 0a20 2020 2064 6f63 7479 7065 3a20 7374  .    doctype: st
-00000a00: 7220 3d20 280d 0a20 2020 2020 2020 2027  r = (..        '
-00000a10: 3c21 444f 4354 5950 4520 7376 6720 5055  <!DOCTYPE svg PU
-00000a20: 424c 4943 2022 2d2f 2f57 3343 2f2f 4454  BLIC "-//W3C//DT
-00000a30: 4420 5356 4720 312e 312f 2f45 4e22 5c6e  D SVG 1.1//EN"\n
-00000a40: 270d 0a20 2020 2020 2020 2027 2268 7474  '..        '"htt
-00000a50: 703a 2f2f 7777 772e 7733 2e6f 7267 2f47  p://www.w3.org/G
-00000a60: 7261 7068 6963 732f 5356 472f 312e 312f  raphics/SVG/1.1/
-00000a70: 4454 442f 7376 6731 312e 6474 6422 3e27  DTD/svg11.dtd">'
-00000a80: 0d0a 2020 2020 290d 0a20 2020 2065 6e63  ..    )..    enc
-00000a90: 6f64 696e 673a 2073 7472 203d 2022 5554  oding: str = "UT
-00000aa0: 462d 3822 0d0a 0d0a 0d0a 6465 6620 7376  F-8"......def sv
-00000ab0: 675f 746f 7374 7269 6e67 2878 6d6c 3a20  g_tostring(xml: 
-00000ac0: 6574 7265 652e 456c 656d 656e 742c 202a  etree.Element, *
-00000ad0: 2a74 6f73 7472 696e 675f 6b77 6172 6773  *tostring_kwargs
-00000ae0: 2920 2d3e 2062 7974 6561 7272 6179 3a0d  ) -> bytearray:.
-00000af0: 0a20 2020 2022 2222 0d0a 2020 2020 436f  .    """..    Co
-00000b00: 6e74 656e 7473 206f 6620 7376 6720 6669  ntents of svg fi
-00000b10: 6c65 2077 6974 6820 6f70 7469 6f6e 616c  le with optional
-00000b20: 2078 6d6c 2064 6563 6c61 7261 7469 6f6e   xml declaration
-00000b30: 2e0d 0a0d 0a20 2020 203a 7061 7261 6d20  .....    :param 
-00000b40: 786d 6c3a 2072 6f6f 7420 6e6f 6465 206f  xml: root node o
-00000b50: 6620 796f 7572 2073 7667 2067 656f 6d65  f your svg geome
-00000b60: 7472 790d 0a20 2020 203a 7061 7261 6d20  try..    :param 
-00000b70: 746f 7374 7269 6e67 5f6b 7761 7267 733a  tostring_kwargs:
-00000b80: 206b 6579 776f 7264 2061 7267 756d 656e   keyword argumen
-00000b90: 7473 2074 6f20 6574 7265 652e 746f 7374  ts to etree.tost
-00000ba0: 7269 6e67 2e20 786d 6c5f 6865 6164 6572  ring. xml_header
-00000bb0: 3d54 7275 6520 666f 720d 0a20 2020 2020  =True for..     
-00000bc0: 2020 2073 656e 7369 626c 6520 6465 6661     sensible defa
-00000bd0: 756c 7420 7661 6c75 6573 2e20 5365 6520  ult values. See 
-00000be0: 6265 6c6f 772e 0d0a 0d0a 2020 2020 4675  below.....    Fu
-00000bf0: 7274 6865 7220 646f 6375 6d65 6e74 6174  rther documentat
-00000c00: 696f 6e20 696e 2077 7269 7465 5f73 7667  ion in write_svg
-00000c10: 2064 6f63 7374 7269 6e67 2e0d 0a20 2020   docstring...   
-00000c20: 2022 2222 0d0a 2020 2020 746f 7374 7269   """..    tostri
-00000c30: 6e67 5f6b 7761 7267 735b 2270 7265 7474  ng_kwargs["prett
-00000c40: 795f 7072 696e 7422 5d20 3d20 746f 7374  y_print"] = tost
-00000c50: 7269 6e67 5f6b 7761 7267 732e 6765 7428  ring_kwargs.get(
-00000c60: 2270 7265 7474 795f 7072 696e 7422 2c20  "pretty_print", 
-00000c70: 5472 7565 290d 0a20 2020 2069 6620 746f  True)..    if to
-00000c80: 7374 7269 6e67 5f6b 7761 7267 732e 6765  string_kwargs.ge
-00000c90: 7428 2278 6d6c 5f64 6563 6c61 7261 7469  t("xml_declarati
-00000ca0: 6f6e 2229 3a0d 0a20 2020 2020 2020 2066  on"):..        f
-00000cb0: 6f72 2064 6566 6175 6c74 2069 6e20 5f54  or default in _T
-00000cc0: 6f73 7472 696e 6744 6566 6175 6c74 733a  ostringDefaults:
-00000cd0: 0d0a 2020 2020 2020 2020 2020 2020 7661  ..            va
-00000ce0: 6c75 6520 3d20 746f 7374 7269 6e67 5f6b  lue = tostring_k
-00000cf0: 7761 7267 732e 6765 7428 6465 6661 756c  wargs.get(defaul
-00000d00: 742e 6e61 6d65 2c20 6465 6661 756c 742e  t.name, default.
-00000d10: 7661 6c75 6529 0d0a 2020 2020 2020 2020  value)..        
-00000d20: 2020 2020 746f 7374 7269 6e67 5f6b 7761      tostring_kwa
-00000d30: 7267 735b 6465 6661 756c 742e 6e61 6d65  rgs[default.name
-00000d40: 5d20 3d20 7661 6c75 650d 0a20 2020 2073  ] = value..    s
-00000d50: 7667 5f63 6f6e 7465 6e74 7320 3d20 6574  vg_contents = et
-00000d60: 7265 652e 746f 7374 7269 6e67 2865 7472  ree.tostring(etr
-00000d70: 6565 2e45 6c65 6d65 6e74 5472 6565 2878  ee.ElementTree(x
-00000d80: 6d6c 292c 202a 2a74 6f73 7472 696e 675f  ml), **tostring_
-00000d90: 6b77 6172 6773 290d 0a20 2020 2072 6574  kwargs)..    ret
-00000da0: 7572 6e20 7376 675f 636f 6e74 656e 7473  urn svg_contents
-00000db0: 0d0a 0d0a 0d0a 6465 6620 6765 745f 7669  ......def get_vi
-00000dc0: 6577 426f 785f 7374 7228 0d0a 2020 2020  ewBox_str(..    
-00000dd0: 783a 2066 6c6f 6174 2c20 793a 2066 6c6f  x: float, y: flo
-00000de0: 6174 2c20 7769 6474 683a 2066 6c6f 6174  at, width: float
-00000df0: 2c20 6865 6967 6874 3a20 666c 6f61 742c  , height: float,
-00000e00: 2070 6164 3a20 666c 6f61 7420 3d20 300d   pad: float = 0.
-00000e10: 0a29 202d 3e20 7374 723a 0d0a 2020 2020  .) -> str:..    
-00000e20: 2222 220d 0a20 2020 2052 6f75 6e64 2061  """..    Round a
-00000e30: 7267 756d 656e 7473 2074 6f20 696e 7473  rguments to ints
-00000e40: 2061 6e64 2063 7265 6174 6520 6120 7370   and create a sp
-00000e50: 6163 652d 6465 6c69 6d69 7465 6420 7374  ace-delimited st
-00000e60: 7269 6e67 2e0d 0a0d 0a20 2020 203a 7061  ring.....    :pa
-00000e70: 7261 6d20 783a 2078 2076 616c 7565 2069  ram x: x value i
-00000e80: 6e20 7570 7065 722d 6c65 6674 2063 6f72  n upper-left cor
-00000e90: 6e65 720d 0a20 2020 203a 7061 7261 6d20  ner..    :param 
-00000ea0: 793a 2079 2076 616c 7565 2069 6e20 7570  y: y value in up
-00000eb0: 7065 722d 6c65 6674 2063 6f72 6e65 720d  per-left corner.
-00000ec0: 0a20 2020 203a 7061 7261 6d20 7769 6474  .    :param widt
-00000ed0: 683a 2077 6964 7468 206f 6620 7669 6577  h: width of view
-00000ee0: 426f 780d 0a20 2020 203a 7061 7261 6d20  Box..    :param 
-00000ef0: 6865 6967 6874 3a20 6865 6967 6874 206f  height: height o
-00000f00: 6620 7669 6577 426f 780d 0a20 2020 203a  f viewBox..    :
-00000f10: 7061 7261 6d20 7061 643a 206f 7074 696f  param pad: optio
-00000f20: 6e61 6c6c 7920 696e 6372 6561 7365 2076  nally increase v
-00000f30: 6965 7742 6f78 2062 7920 7061 6420 696e  iewBox by pad in
-00000f40: 2061 6c6c 2064 6972 6563 7469 6f6e 730d   all directions.
-00000f50: 0a20 2020 203a 7265 7475 726e 3a20 7370  .    :return: sp
-00000f60: 6163 652d 6465 6c69 6d69 7465 6420 7374  ace-delimited st
-00000f70: 7269 6e67 2022 7820 7920 7769 6474 6820  ring "x y width 
-00000f80: 6865 6967 6874 220d 0a20 2020 2022 2222  height"..    """
-00000f90: 0d0a 2020 2020 6469 6d73 203d 205b 0d0a  ..    dims = [..
-00000fa0: 2020 2020 2020 2020 666f 726d 6174 5f6e          format_n
-00000fb0: 756d 6265 7228 6120 2b20 6229 0d0a 2020  umber(a + b)..  
-00000fc0: 2020 2020 2020 666f 7220 612c 2062 2069        for a, b i
-00000fd0: 6e20 7a69 7028 2878 2c20 792c 2077 6964  n zip((x, y, wid
-00000fe0: 7468 2c20 6865 6967 6874 292c 2028 2d70  th, height), (-p
-00000ff0: 6164 2c20 2d70 6164 2c20 7061 6420 2a20  ad, -pad, pad * 
-00001000: 322c 2070 6164 202a 2032 2929 0d0a 2020  2, pad * 2))..  
-00001010: 2020 5d0d 0a20 2020 2072 6574 7572 6e20    ]..    return 
-00001020: 2220 222e 6a6f 696e 2864 696d 7329 0d0a  " ".join(dims)..
+00000150: 7970 696e 6720 696d 706f 7274 2054 7970  yping import Typ
+00000160: 6541 6c69 6173 2c20 556e 696f 6e0d 0a0d  eAlias, Union...
+00000170: 0a66 726f 6d20 6c78 6d6c 2069 6d70 6f72  .from lxml impor
+00000180: 7420 6574 7265 650d 0a0d 0a66 726f 6d20  t etree....from 
+00000190: 7376 675f 756c 7472 616c 6967 6874 2e6e  svg_ultralight.n
+000001a0: 736d 6170 2069 6d70 6f72 7420 4e53 4d41  smap import NSMA
+000001b0: 500d 0a0d 0a5f 456c 656d 656e 743a 2054  P...._Element: T
+000001c0: 7970 6541 6c69 6173 203d 2065 7472 6565  ypeAlias = etree
+000001d0: 2e5f 456c 656d 656e 7420 2023 2074 7970  ._Element  # typ
+000001e0: 653a 2069 676e 6f72 650d 0a0d 0a0d 0a64  e: ignore......d
+000001f0: 6566 2066 6f72 6d61 745f 6e75 6d62 6572  ef format_number
+00000200: 286e 756d 3a20 666c 6f61 7429 202d 3e20  (num: float) -> 
+00000210: 7374 723a 0d0a 2020 2020 2222 220d 0a20  str:..    """.. 
+00000220: 2020 2046 6f72 6d61 7420 7374 7269 6e67     Format string
+00000230: 7320 6174 206c 696d 6974 6564 2070 7265  s at limited pre
+00000240: 6369 7369 6f6e 0d0a 0d0a 2020 2020 3a70  cision....    :p
+00000250: 6172 616d 206e 756d 3a20 616e 7974 6869  aram num: anythi
+00000260: 6e67 2074 6861 7420 6361 6e20 7072 696e  ng that can prin
+00000270: 7420 6173 2061 2066 6c6f 6174 2e0d 0a20  t as a float... 
+00000280: 2020 203a 7265 7475 726e 3a20 7374 720d     :return: str.
+00000290: 0a0d 0a20 2020 2049 2776 6520 7265 6164  ...    I've read
+000002a0: 2061 7274 6963 6c65 7320 7468 6174 2072   articles that r
+000002b0: 6563 6f6d 6d65 6e64 206e 6f20 6d6f 7265  ecommend no more
+000002c0: 2074 6861 6e20 666f 7572 2064 6967 6974   than four digit
+000002d0: 7320 6265 666f 7265 2061 6e64 2074 776f  s before and two
+000002e0: 2064 6967 6974 730d 0a20 2020 2061 6674   digits..    aft
+000002f0: 6572 2074 6865 2064 6563 696d 616c 2070  er the decimal p
+00000300: 6f69 6e74 2074 6f20 656e 7375 7265 2067  oint to ensure g
+00000310: 6f6f 6420 7376 6720 7265 6e64 6572 696e  ood svg renderin
+00000320: 672e 2049 276d 2062 6569 6e67 2067 656e  g. I'm being gen
+00000330: 6572 6f75 7320 616e 640d 0a20 2020 2067  erous and..    g
+00000340: 6976 696e 6720 7369 782e 204d 6f73 746c  iving six. Mostl
+00000350: 7920 746f 2065 6c69 6d69 6e61 7465 2065  y to eliminate e
+00000360: 7870 6f6e 656e 7469 616c 206e 6f74 6174  xponential notat
+00000370: 696f 6e2c 2062 7574 2049 276d 2022 7273  ion, but I'm "rs
+00000380: 7472 6970 7069 6e67 2220 7468 650d 0a20  tripping" the.. 
+00000390: 2020 2073 7472 696e 6773 2074 6f20 7265     strings to re
+000003a0: 6475 6365 2066 696c 6573 697a 6520 616e  duce filesize an
+000003b0: 6420 696e 6372 6561 7365 2072 6561 6461  d increase reada
+000003c0: 6269 6c69 7479 0d0a 2020 2020 2222 220d  bility..    """.
+000003d0: 0a20 2020 2072 6574 7572 6e20 6622 7b6e  .    return f"{n
+000003e0: 756d 3a30 2e36 667d 222e 7273 7472 6970  um:0.6f}".rstrip
+000003f0: 2822 3022 292e 7273 7472 6970 2822 2e22  ("0").rstrip("."
+00000400: 290d 0a0d 0a0d 0a64 6566 2073 6574 5f61  )......def set_a
+00000410: 7474 7269 6275 7465 7328 656c 656d 3a20  ttributes(elem: 
+00000420: 5f45 6c65 6d65 6e74 2c20 2a2a 6174 7472  _Element, **attr
+00000430: 6962 7574 6573 3a20 556e 696f 6e5b 7374  ibutes: Union[st
+00000440: 722c 2066 6c6f 6174 5d29 202d 3e20 4e6f  r, float]) -> No
+00000450: 6e65 3a0d 0a20 2020 2022 2222 0d0a 2020  ne:..    """..  
+00000460: 2020 5365 7420 6e61 6d65 3a20 7661 6c75    Set name: valu
+00000470: 6520 6974 656d 7320 6173 2065 6c65 6d65  e items as eleme
+00000480: 6e74 2061 7474 7269 6275 7465 732e 204d  nt attributes. M
+00000490: 616b 6520 6576 6572 7920 7661 6c75 6520  ake every value 
+000004a0: 6120 7374 7269 6e67 2e0d 0a0d 0a20 2020  a string.....   
+000004b0: 203a 7061 7261 6d20 656c 656d 3a20 656c   :param elem: el
+000004c0: 656d 656e 7420 746f 2072 6563 6569 7665  ement to receive
+000004d0: 2065 6c65 6d65 6e74 2e73 6574 286b 6579   element.set(key
+000004e0: 776f 7264 2c20 7374 7228 7661 6c75 6529  word, str(value)
+000004f0: 2920 6361 6c6c 730d 0a20 2020 203a 7061  ) calls..    :pa
+00000500: 7261 6d20 6174 7472 6962 7574 6573 3a20  ram attributes: 
+00000510: 656c 656d 656e 7420 6174 7472 6962 7574  element attribut
+00000520: 6520 6e61 6d65 7320 616e 6420 7661 6c75  e names and valu
+00000530: 6573 2e20 4b6e 6f77 7320 7768 6174 2074  es. Knows what t
+00000540: 6f20 646f 2077 6974 6820 2774 6578 7427  o do with 'text'
+00000550: 0d0a 2020 2020 2020 2020 6b65 7977 6f72  ..        keywor
+00000560: 642e 5620 3a65 6666 6563 7473 3a20 7570  d.V :effects: up
+00000570: 6461 7465 7320 6060 656c 656d 6060 0d0a  dates ``elem``..
+00000580: 0d0a 2020 2020 5468 6973 2069 7320 6a75  ..    This is ju
+00000590: 7374 2074 6f20 7361 7665 2061 206c 6f74  st to save a lot
+000005a0: 206f 6620 7479 7069 6e67 2e20 6574 7265   of typing. etre
+000005b0: 652e 456c 656d 656e 7473 2077 696c 6c20  e.Elements will 
+000005c0: 6f6e 6c79 2061 6363 6570 7420 7374 7269  only accept stri
+000005d0: 6e67 0d0a 2020 2020 7661 6c75 6573 2e20  ng..    values. 
+000005e0: 5461 6b65 7320 6561 6368 2069 6e20 7061  Takes each in pa
+000005f0: 7261 6d73 2e76 616c 7565 7328 292c 2061  rams.values(), a
+00000600: 6e64 2070 6173 7365 7320 6974 2074 6f20  nd passes it to 
+00000610: 6574 7265 652e 456c 656d 656e 7420 6173  etree.Element as
+00000620: 2061 0d0a 2020 2020 7374 7269 6e67 2e20   a..    string. 
+00000630: 5769 6c6c 2061 6c73 6f20 7265 706c 6163  Will also replac
+00000640: 6520 605f 6020 7769 7468 2060 2d60 2074  e `_` with `-` t
+00000650: 6f20 7472 616e 736c 6174 6520 7661 6c69  o translate vali
+00000660: 6420 5079 7468 6f6e 2076 6172 6961 626c  d Python variabl
+00000670: 6520 6e61 6d65 730d 0a20 2020 2066 6f72  e names..    for
+00000680: 2078 6d6c 2070 6172 616d 6574 6572 206e   xml parameter n
+00000690: 616d 6573 2e0d 0a0d 0a20 2020 2049 6e76  ames.....    Inv
+000006a0: 616c 6964 206e 616d 6573 2028 6120 706f  alid names (a po
+000006b0: 7075 6c61 7220 6f6e 6520 7769 6c6c 2062  pular one will b
+000006c0: 6520 2763 6c61 7373 2729 2063 616e 2062  e 'class') can b
+000006d0: 6520 7061 7373 6564 2077 6974 6820 6120  e passed with a 
+000006e0: 7472 6169 6c69 6e67 0d0a 2020 2020 756e  trailing..    un
+000006f0: 6465 7273 636f 7265 2028 652e 672e 2c20  derscore (e.g., 
+00000700: 636c 6173 735f 3d27 626f 6479 5f74 6578  class_='body_tex
+00000710: 7427 292e 0d0a 0d0a 2020 2020 5468 6174  t').....    That
+00000720: 2773 2061 6c6d 6f73 7420 616c 6c2e 2054  's almost all. T
+00000730: 6865 2066 756e 6374 696f 6e20 7769 6c6c  he function will
+00000740: 2061 6c73 6f20 6861 6e64 6c65 2074 6865   also handle the
+00000750: 2027 7465 7874 2720 6b65 7977 6f72 642c   'text' keyword,
+00000760: 2070 6c61 6369 6e67 2074 6865 0d0a 2020   placing the..  
+00000770: 2020 7661 6c75 6520 6265 7477 6565 6e20    value between 
+00000780: 656c 656d 656e 7420 7461 6773 2e0d 0a0d  element tags....
+00000790: 0a20 2020 2046 6f72 6d61 7420 666c 6f61  .    Format floa
+000007a0: 7473 2074 6872 6f75 6768 2066 277b 7661  ts through f'{va
+000007b0: 6c75 653a 667d 2074 6f20 6176 6f69 6420  lue:f} to avoid 
+000007c0: 6578 706f 6e65 6e74 6961 6c20 7265 7072  exponential repr
+000007d0: 6573 656e 7461 7469 6f6e 0d0a 2020 2020  esentation..    
+000007e0: 2865 2e67 2e2c 2031 3065 2d30 3629 2077  (e.g., 10e-06) w
+000007f0: 6869 6368 2073 7667 2070 6172 7365 7273  hich svg parsers
+00000800: 2077 6f6e 2774 2075 6e64 6572 7374 616e   won't understan
+00000810: 642e 0d0a 2020 2020 2222 220d 0a20 2020  d...    """..   
+00000820: 2064 6f74 7320 3d20 7b22 7465 7874 227d   dots = {"text"}
+00000830: 0d0a 2020 2020 666f 7220 646f 7420 696e  ..    for dot in
+00000840: 2064 6f74 7320 2620 7365 7428 6174 7472   dots & set(attr
+00000850: 6962 7574 6573 293a 0d0a 2020 2020 2020  ibutes):..      
+00000860: 2020 7365 7461 7474 7228 656c 656d 2c20    setattr(elem, 
+00000870: 646f 742c 2061 7474 7269 6275 7465 732e  dot, attributes.
+00000880: 706f 7028 646f 7429 290d 0a0d 0a20 2020  pop(dot))....   
+00000890: 2066 6f72 206b 2c20 7620 696e 2061 7474   for k, v in att
+000008a0: 7269 6275 7465 732e 6974 656d 7328 293a  ributes.items():
+000008b0: 0d0a 2020 2020 2020 2020 6966 2022 3a22  ..        if ":"
+000008c0: 2069 6e20 6b3a 0d0a 2020 2020 2020 2020   in k:..        
+000008d0: 2020 2020 6e61 6d65 7370 6163 652c 2074      namespace, t
+000008e0: 6167 203d 206b 2e73 706c 6974 2822 3a22  ag = k.split(":"
+000008f0: 290d 0a20 2020 2020 2020 2020 2020 206b  )..            k
+00000900: 203d 2065 7472 6565 2e51 4e61 6d65 284e   = etree.QName(N
+00000910: 534d 4150 5b6e 616d 6573 7061 6365 5d2c  SMAP[namespace],
+00000920: 2074 6167 290d 0a20 2020 2020 2020 2065   tag)..        e
+00000930: 6c73 653a 0d0a 2020 2020 2020 2020 2020  lse:..          
+00000940: 2020 6b20 3d20 6b2e 7273 7472 6970 2822    k = k.rstrip("
+00000950: 5f22 292e 7265 706c 6163 6528 225f 222c  _").replace("_",
+00000960: 2022 2d22 290d 0a20 2020 2020 2020 2074   "-")..        t
+00000970: 7279 3a0d 0a20 2020 2020 2020 2020 2020  ry:..           
+00000980: 2076 616c 203d 2066 6f72 6d61 745f 6e75   val = format_nu
+00000990: 6d62 6572 2866 6c6f 6174 2876 2929 0d0a  mber(float(v))..
+000009a0: 2020 2020 2020 2020 6578 6365 7074 2056          except V
+000009b0: 616c 7565 4572 726f 723a 0d0a 2020 2020  alueError:..    
+000009c0: 2020 2020 2020 2020 7661 6c20 3d20 7374          val = st
+000009d0: 7228 7629 0d0a 2020 2020 2020 2020 656c  r(v)..        el
+000009e0: 656d 2e73 6574 286b 2c20 7661 6c29 0d0a  em.set(k, val)..
+000009f0: 0d0a 0d0a 636c 6173 7320 5f54 6f73 7472  ....class _Tostr
+00000a00: 696e 6744 6566 6175 6c74 7328 456e 756d  ingDefaults(Enum
+00000a10: 293a 0d0a 2020 2020 2222 2244 6566 6175  ):..    """Defau
+00000a20: 6c74 2076 616c 7565 7320 666f 7220 616e  lt values for an
+00000a30: 2073 7667 2078 6d6c 5f68 6561 6465 7222   svg xml_header"
+00000a40: 2222 0d0a 0d0a 2020 2020 646f 6374 7970  ""....    doctyp
+00000a50: 6520 3d20 280d 0a20 2020 2020 2020 2027  e = (..        '
+00000a60: 3c21 444f 4354 5950 4520 7376 6720 5055  <!DOCTYPE svg PU
+00000a70: 424c 4943 2022 2d2f 2f57 3343 2f2f 4454  BLIC "-//W3C//DT
+00000a80: 4420 5356 4720 312e 312f 2f45 4e22 5c6e  D SVG 1.1//EN"\n
+00000a90: 270d 0a20 2020 2020 2020 202b 2027 2268  '..        + '"h
+00000aa0: 7474 703a 2f2f 7777 772e 7733 2e6f 7267  ttp://www.w3.org
+00000ab0: 2f47 7261 7068 6963 732f 5356 472f 312e  /Graphics/SVG/1.
+00000ac0: 312f 4454 442f 7376 6731 312e 6474 6422  1/DTD/svg11.dtd"
+00000ad0: 3e27 0d0a 2020 2020 290d 0a20 2020 2065  >'..    )..    e
+00000ae0: 6e63 6f64 696e 6720 3d20 2255 5446 2d38  ncoding = "UTF-8
+00000af0: 220d 0a0d 0a0d 0a64 6566 2073 7667 5f74  "......def svg_t
+00000b00: 6f73 7472 696e 6728 786d 6c3a 205f 456c  ostring(xml: _El
+00000b10: 656d 656e 742c 202a 2a74 6f73 7472 696e  ement, **tostrin
+00000b20: 675f 6b77 6172 6773 3a20 7374 7220 7c20  g_kwargs: str | 
+00000b30: 626f 6f6c 2920 2d3e 2062 7974 6573 3a0d  bool) -> bytes:.
+00000b40: 0a20 2020 2022 2222 0d0a 2020 2020 436f  .    """..    Co
+00000b50: 6e74 656e 7473 206f 6620 7376 6720 6669  ntents of svg fi
+00000b60: 6c65 2077 6974 6820 6f70 7469 6f6e 616c  le with optional
+00000b70: 2078 6d6c 2064 6563 6c61 7261 7469 6f6e   xml declaration
+00000b80: 2e0d 0a0d 0a20 2020 203a 7061 7261 6d20  .....    :param 
+00000b90: 786d 6c3a 2072 6f6f 7420 6e6f 6465 206f  xml: root node o
+00000ba0: 6620 796f 7572 2073 7667 2067 656f 6d65  f your svg geome
+00000bb0: 7472 790d 0a20 2020 203a 7061 7261 6d20  try..    :param 
+00000bc0: 746f 7374 7269 6e67 5f6b 7761 7267 733a  tostring_kwargs:
+00000bd0: 206b 6579 776f 7264 2061 7267 756d 656e   keyword argumen
+00000be0: 7473 2074 6f20 6574 7265 652e 746f 7374  ts to etree.tost
+00000bf0: 7269 6e67 2e0d 0a20 2020 2020 2020 2070  ring...        p
+00000c00: 6173 7320 786d 6c5f 6865 6164 6572 3d54  ass xml_header=T
+00000c10: 7275 6520 666f 7220 7365 6e73 6962 6c65  rue for sensible
+00000c20: 2064 6566 6175 6c74 732c 2073 6565 2066   defaults, see f
+00000c30: 7572 7468 6572 2064 6f63 756d 656e 7461  urther documenta
+00000c40: 7469 6f6e 206f 6e20 786d 6c0d 0a20 2020  tion on xml..   
+00000c50: 2020 2020 2068 6561 6465 7220 696e 2077       header in w
+00000c60: 7269 7465 5f73 7667 2064 6f63 7374 7269  rite_svg docstri
+00000c70: 6e67 2e0d 0a20 2020 2022 2222 0d0a 2020  ng...    """..  
+00000c80: 2020 746f 7374 7269 6e67 5f6b 7761 7267    tostring_kwarg
+00000c90: 735b 2270 7265 7474 795f 7072 696e 7422  s["pretty_print"
+00000ca0: 5d20 3d20 746f 7374 7269 6e67 5f6b 7761  ] = tostring_kwa
+00000cb0: 7267 732e 6765 7428 2270 7265 7474 795f  rgs.get("pretty_
+00000cc0: 7072 696e 7422 2c20 5472 7565 290d 0a20  print", True).. 
+00000cd0: 2020 2069 6620 746f 7374 7269 6e67 5f6b     if tostring_k
+00000ce0: 7761 7267 732e 6765 7428 2278 6d6c 5f64  wargs.get("xml_d
+00000cf0: 6563 6c61 7261 7469 6f6e 2229 3a0d 0a20  eclaration"):.. 
+00000d00: 2020 2020 2020 2066 6f72 2064 6566 6175         for defau
+00000d10: 6c74 2069 6e20 5f54 6f73 7472 696e 6744  lt in _TostringD
+00000d20: 6566 6175 6c74 733a 0d0a 2020 2020 2020  efaults:..      
+00000d30: 2020 2020 2020 7661 6c75 6520 3d20 746f        value = to
+00000d40: 7374 7269 6e67 5f6b 7761 7267 732e 6765  string_kwargs.ge
+00000d50: 7428 6465 6661 756c 742e 6e61 6d65 2c20  t(default.name, 
+00000d60: 6465 6661 756c 742e 7661 6c75 6529 0d0a  default.value)..
+00000d70: 2020 2020 2020 2020 2020 2020 746f 7374              tost
+00000d80: 7269 6e67 5f6b 7761 7267 735b 6465 6661  ring_kwargs[defa
+00000d90: 756c 742e 6e61 6d65 5d20 3d20 7661 6c75  ult.name] = valu
+00000da0: 650d 0a20 2020 2073 7667 5f63 6f6e 7465  e..    svg_conte
+00000db0: 6e74 7320 3d20 6574 7265 652e 746f 7374  nts = etree.tost
+00000dc0: 7269 6e67 2865 7472 6565 2e45 6c65 6d65  ring(etree.Eleme
+00000dd0: 6e74 5472 6565 2878 6d6c 292c 202a 2a74  ntTree(xml), **t
+00000de0: 6f73 7472 696e 675f 6b77 6172 6773 290d  ostring_kwargs).
+00000df0: 0a20 2020 2072 6574 7572 6e20 7376 675f  .    return svg_
+00000e00: 636f 6e74 656e 7473 0d0a 0d0a 0d0a 6465  contents......de
+00000e10: 6620 6765 745f 7669 6577 426f 785f 7374  f get_viewBox_st
+00000e20: 7228 0d0a 2020 2020 783a 2066 6c6f 6174  r(..    x: float
+00000e30: 2c20 793a 2066 6c6f 6174 2c20 7769 6474  , y: float, widt
+00000e40: 683a 2066 6c6f 6174 2c20 6865 6967 6874  h: float, height
+00000e50: 3a20 666c 6f61 742c 2070 6164 3a20 666c  : float, pad: fl
+00000e60: 6f61 7420 3d20 300d 0a29 202d 3e20 7374  oat = 0..) -> st
+00000e70: 723a 0d0a 2020 2020 2222 220d 0a20 2020  r:..    """..   
+00000e80: 2043 7265 6174 6520 6120 7370 6163 652d   Create a space-
+00000e90: 6465 6c69 6d69 7465 6420 7374 7269 6e67  delimited string
+00000ea0: 2e0d 0a0d 0a20 2020 203a 7061 7261 6d20  .....    :param 
+00000eb0: 783a 2078 2076 616c 7565 2069 6e20 7570  x: x value in up
+00000ec0: 7065 722d 6c65 6674 2063 6f72 6e65 720d  per-left corner.
+00000ed0: 0a20 2020 203a 7061 7261 6d20 793a 2079  .    :param y: y
+00000ee0: 2076 616c 7565 2069 6e20 7570 7065 722d   value in upper-
+00000ef0: 6c65 6674 2063 6f72 6e65 720d 0a20 2020  left corner..   
+00000f00: 203a 7061 7261 6d20 7769 6474 683a 2077   :param width: w
+00000f10: 6964 7468 206f 6620 7669 6577 426f 780d  idth of viewBox.
+00000f20: 0a20 2020 203a 7061 7261 6d20 6865 6967  .    :param heig
+00000f30: 6874 3a20 6865 6967 6874 206f 6620 7669  ht: height of vi
+00000f40: 6577 426f 780d 0a20 2020 203a 7061 7261  ewBox..    :para
+00000f50: 6d20 7061 643a 206f 7074 696f 6e61 6c6c  m pad: optionall
+00000f60: 7920 696e 6372 6561 7365 2076 6965 7742  y increase viewB
+00000f70: 6f78 2062 7920 7061 6420 696e 2061 6c6c  ox by pad in all
+00000f80: 2064 6972 6563 7469 6f6e 730d 0a20 2020   directions..   
+00000f90: 203a 7265 7475 726e 3a20 7370 6163 652d   :return: space-
+00000fa0: 6465 6c69 6d69 7465 6420 7374 7269 6e67  delimited string
+00000fb0: 2022 7820 7920 7769 6474 6820 6865 6967   "x y width heig
+00000fc0: 6874 220d 0a20 2020 2022 2222 0d0a 2020  ht"..    """..  
+00000fd0: 2020 6469 6d73 203d 205b 0d0a 2020 2020    dims = [..    
+00000fe0: 2020 2020 666f 726d 6174 5f6e 756d 6265      format_numbe
+00000ff0: 7228 6120 2b20 6229 0d0a 2020 2020 2020  r(a + b)..      
+00001000: 2020 666f 7220 612c 2062 2069 6e20 7a69    for a, b in zi
+00001010: 7028 2878 2c20 792c 2077 6964 7468 2c20  p((x, y, width, 
+00001020: 6865 6967 6874 292c 2028 2d70 6164 2c20  height), (-pad, 
+00001030: 2d70 6164 2c20 7061 6420 2a20 322c 2070  -pad, pad * 2, p
+00001040: 6164 202a 2032 2929 0d0a 2020 2020 5d0d  ad * 2))..    ].
+00001050: 0a20 2020 2072 6574 7572 6e20 2220 222e  .    return " ".
+00001060: 6a6f 696e 2864 696d 7329 0d0a            join(dims)..
```

### Comparing `svg_ultralight-0.8.2/svg_ultralight/strings/svg_strings.py` & `svg_ultralight-0.9.0/svg_ultralight/strings/svg_strings.py`

 * *Files 12% similar despite different names*

```diff
@@ -5,20 +5,20 @@
 :author: Shay Hill
 :created: 10/30/2020
 
 The `string_conversion` module will format floats or strings. Some other formatters can
 make things easier.
 """
 
-from typing import Iterable, Tuple
+from typing import Iterable
 
-from ..string_conversion import format_number
+from svg_ultralight.string_conversion import format_number
 
 
-def svg_color_tuple(rgb_floats):
+def svg_color_tuple(rgb_floats: tuple[float, float, float]) -> str:
     """
     Turn an rgb tuple (0-255, 0-255, 0-255) into an svg color definition.
 
     :param rgb_floats: (0-255, 0-255, 0-255)
     :return: "rgb(128,128,128)"
     """
     r, g, b = (round(x) for x in rgb_floats)
@@ -31,16 +31,16 @@
 
     :param floats: and number of floats
     :return: each float rounded to an int, space delimited
     """
     return " ".join(str(round(x)) for x in floats)
 
 
-def svg_float_tuples(tuples: Iterable[Tuple[float, float]]) -> str:
+def svg_float_tuples(tuples: Iterable[tuple[float, float]]) -> str:
     """
     Space-delimited tuples
 
     :param tuples: [(a, b), (c, d)]
     :return: "a,b c,d"
     """
-    tuples = [",".join(format_number(x) for x in y) for y in tuples]
-    return " ".join(tuples)
+    tuple_strings = [",".join(format_number(n) for n in t) for t in tuples]
+    return " ".join(tuple_strings)
```

### Comparing `svg_ultralight-0.8.2/svg_ultralight/svg_ultralight.py` & `svg_ultralight-0.9.0/svg_ultralight/main.py`

 * *Files 3% similar despite different names*

```diff
@@ -33,548 +33,574 @@
 00000200: 0d0a 0d0a 696d 706f 7274 206f 730d 0a69  ....import os..i
 00000210: 6d70 6f72 7420 7375 6270 726f 6365 7373  mport subprocess
 00000220: 0d0a 6672 6f6d 2070 6174 686c 6962 2069  ..from pathlib i
 00000230: 6d70 6f72 7420 5061 7468 0d0a 6672 6f6d  mport Path..from
 00000240: 2074 656d 7066 696c 6520 696d 706f 7274   tempfile import
 00000250: 204e 616d 6564 5465 6d70 6f72 6172 7946   NamedTemporaryF
 00000260: 696c 650d 0a66 726f 6d20 7479 7069 6e67  ile..from typing
-00000270: 2069 6d70 6f72 7420 4469 6374 2c20 494f   import Dict, IO
-00000280: 2c20 4f70 7469 6f6e 616c 2c20 556e 696f  , Optional, Unio
-00000290: 6e0d 0a0d 0a66 726f 6d20 6c78 6d6c 2069  n....from lxml i
-000002a0: 6d70 6f72 7420 6574 7265 6520 2023 2074  mport etree  # t
-000002b0: 7970 653a 2069 676e 6f72 650d 0a0d 0a66  ype: ignore....f
-000002c0: 726f 6d20 2e63 6f6e 7374 7275 6374 6f72  rom .constructor
-000002d0: 7320 696d 706f 7274 2075 7064 6174 655f  s import update_
-000002e0: 656c 656d 656e 740d 0a66 726f 6d20 2e6e  element..from .n
-000002f0: 736d 6170 2069 6d70 6f72 7420 4e53 4d41  smap import NSMA
-00000300: 500d 0a66 726f 6d20 2e73 7472 696e 675f  P..from .string_
-00000310: 636f 6e76 6572 7369 6f6e 2069 6d70 6f72  conversion impor
-00000320: 7420 666f 726d 6174 5f6e 756d 6265 722c  t format_number,
-00000330: 2067 6574 5f76 6965 7742 6f78 5f73 7472   get_viewBox_str
-00000340: 2c20 7376 675f 746f 7374 7269 6e67 0d0a  , svg_tostring..
-00000350: 0d0a 0d0a 6465 6620 6e65 775f 7376 675f  ....def new_svg_
-00000360: 726f 6f74 280d 0a20 2020 2078 5f3a 204f  root(..    x_: O
-00000370: 7074 696f 6e61 6c5b 666c 6f61 745d 203d  ptional[float] =
-00000380: 204e 6f6e 652c 0d0a 2020 2020 795f 3a20   None,..    y_: 
-00000390: 4f70 7469 6f6e 616c 5b66 6c6f 6174 5d20  Optional[float] 
-000003a0: 3d20 4e6f 6e65 2c0d 0a20 2020 2077 6964  = None,..    wid
-000003b0: 7468 5f3a 204f 7074 696f 6e61 6c5b 666c  th_: Optional[fl
-000003c0: 6f61 745d 203d 204e 6f6e 652c 0d0a 2020  oat] = None,..  
-000003d0: 2020 6865 6967 6874 5f3a 204f 7074 696f    height_: Optio
-000003e0: 6e61 6c5b 666c 6f61 745d 203d 204e 6f6e  nal[float] = Non
-000003f0: 652c 0d0a 2020 2020 7061 645f 3a20 666c  e,..    pad_: fl
-00000400: 6f61 7420 3d20 302c 0d0a 2020 2020 6470  oat = 0,..    dp
-00000410: 755f 3a20 666c 6f61 7420 3d20 312c 0d0a  u_: float = 1,..
-00000420: 2020 2020 6e73 6d61 703a 204f 7074 696f      nsmap: Optio
-00000430: 6e61 6c5b 4469 6374 5b55 6e69 6f6e 5b73  nal[Dict[Union[s
-00000440: 7472 2c20 4e6f 6e65 5d2c 2073 7472 5d5d  tr, None], str]]
-00000450: 203d 204e 6f6e 652c 0d0a 2020 2020 2a2a   = None,..    **
-00000460: 6174 7472 6962 7574 6573 3a20 556e 696f  attributes: Unio
-00000470: 6e5b 666c 6f61 742c 2073 7472 5d2c 0d0a  n[float, str],..
-00000480: 2920 2d3e 2065 7472 6565 2e45 6c65 6d65  ) -> etree.Eleme
-00000490: 6e74 3a0d 0a20 2020 2022 2222 0d0a 2020  nt:..    """..  
-000004a0: 2020 4372 6561 7465 2061 6e20 7376 6720    Create an svg 
-000004b0: 726f 6f74 2065 6c65 6d65 6e74 2066 726f  root element fro
-000004c0: 6d20 7669 6577 426f 7820 7374 796c 6520  m viewBox style 
-000004d0: 7061 7261 6d65 7465 7273 2e0d 0a0d 0a20  parameters..... 
-000004e0: 2020 203a 7061 7261 6d20 785f 3a20 7820     :param x_: x 
-000004f0: 7661 6c75 6520 696e 2075 7070 6572 2d6c  value in upper-l
-00000500: 6566 7420 636f 726e 6572 0d0a 2020 2020  eft corner..    
-00000510: 3a70 6172 616d 2079 5f3a 2079 2076 616c  :param y_: y val
-00000520: 7565 2069 6e20 7570 7065 722d 6c65 6674  ue in upper-left
-00000530: 2063 6f72 6e65 720d 0a20 2020 203a 7061   corner..    :pa
-00000540: 7261 6d20 7769 6474 685f 3a20 7769 6474  ram width_: widt
-00000550: 6820 6f66 2076 6965 7742 6f78 0d0a 2020  h of viewBox..  
-00000560: 2020 3a70 6172 616d 2068 6569 6768 745f    :param height_
-00000570: 3a20 6865 6967 6874 206f 6620 7669 6577  : height of view
-00000580: 426f 780d 0a20 2020 203a 7061 7261 6d20  Box..    :param 
-00000590: 7061 645f 3a20 6f70 7469 6f6e 616c 6c79  pad_: optionally
-000005a0: 2069 6e63 7265 6173 6520 7669 6577 426f   increase viewBo
-000005b0: 7820 6279 2070 6164 2069 6e20 616c 6c20  x by pad in all 
-000005c0: 6469 7265 6374 696f 6e73 0d0a 2020 2020  directions..    
-000005d0: 3a70 6172 616d 2064 7075 5f3a 206f 7074  :param dpu_: opt
-000005e0: 696f 6e61 6c6c 7920 7363 616c 6520 696d  ionally scale im
-000005f0: 6167 6520 2870 6978 656c 7320 7065 7220  age (pixels per 
-00000600: 756e 6974 206f 6620 626f 756e 6469 6e67  unit of bounding
-00000610: 2062 6f78 290d 0a20 2020 203a 7061 7261   box)..    :para
-00000620: 6d20 6e73 6d61 703a 206f 7074 696f 6e61  m nsmap: optiona
-00000630: 6c6c 7920 7061 7373 2061 206e 616d 6573  lly pass a names
-00000640: 7061 6365 206d 6170 206f 6620 796f 7572  pace map of your
-00000650: 2063 686f 6f73 696e 670d 0a20 2020 203a   choosing..    :
-00000660: 7061 7261 6d20 6174 7472 6962 7574 6573  param attributes
-00000670: 3a20 656c 656d 656e 7420 6174 7472 6962  : element attrib
-00000680: 7574 6520 6e61 6d65 7320 616e 6420 7661  ute names and va
-00000690: 6c75 6573 0d0a 2020 2020 3a72 6574 7572  lues..    :retur
-000006a0: 6e3a 2072 6f6f 7420 7376 6720 656c 656d  n: root svg elem
-000006b0: 656e 740d 0a0d 0a20 2020 2041 6c6c 2076  ent....    All v
-000006c0: 6965 7742 6f78 2d73 7479 6c65 2028 7472  iewBox-style (tr
-000006d0: 6169 6c69 6e67 2075 6e64 6572 7363 6f72  ailing underscor
-000006e0: 6529 2070 6172 616d 6574 6572 7320 6172  e) parameters ar
-000006f0: 6520 6f70 7469 6f6e 616c 2e20 416e 7920  e optional. Any 
-00000700: 6b77 6172 6773 2077 696c 6c0d 0a20 2020  kwargs will..   
-00000710: 2062 6520 7061 7373 6564 2074 6f20 6060   be passed to ``
-00000720: 6574 7265 652e 456c 656d 656e 7460 6020  etree.Element`` 
-00000730: 6173 2065 6c65 6d65 6e74 2070 6172 616d  as element param
-00000740: 6574 6572 732e 0d0a 2020 2020 2222 220d  eters...    """.
-00000750: 0a20 2020 2069 6620 6e73 6d61 7020 6973  .    if nsmap is
-00000760: 204e 6f6e 653a 0d0a 2020 2020 2020 2020   None:..        
-00000770: 6e73 6d61 7020 3d20 4e53 4d41 500d 0a20  nsmap = NSMAP.. 
-00000780: 2020 2069 6620 4e6f 6e65 206e 6f74 2069     if None not i
-00000790: 6e20 2878 5f2c 2079 5f2c 2077 6964 7468  n (x_, y_, width
-000007a0: 5f2c 2068 6569 6768 745f 293a 0d0a 2020  _, height_):..  
-000007b0: 2020 2020 2020 7669 6577 5f62 6f78 203d        view_box =
-000007c0: 2067 6574 5f76 6965 7742 6f78 5f73 7472   get_viewBox_str
-000007d0: 2878 5f2c 2079 5f2c 2077 6964 7468 5f2c  (x_, y_, width_,
-000007e0: 2068 6569 6768 745f 2c20 7061 645f 290d   height_, pad_).
-000007f0: 0a20 2020 2020 2020 2070 6978 656c 5f77  .        pixel_w
-00000800: 6964 7468 203d 2066 6f72 6d61 745f 6e75  idth = format_nu
-00000810: 6d62 6572 2828 7769 6474 685f 202b 2070  mber((width_ + p
-00000820: 6164 5f20 2a20 3229 202a 2064 7075 5f29  ad_ * 2) * dpu_)
-00000830: 0d0a 2020 2020 2020 2020 7069 7865 6c5f  ..        pixel_
-00000840: 6865 6967 6874 203d 2066 6f72 6d61 745f  height = format_
-00000850: 6e75 6d62 6572 2828 6865 6967 6874 5f20  number((height_ 
-00000860: 2b20 7061 645f 202a 2032 2920 2a20 6470  + pad_ * 2) * dp
-00000870: 755f 290d 0a20 2020 2020 2020 2061 7474  u_)..        att
-00000880: 7269 6275 7465 735b 2276 6965 7742 6f78  ributes["viewBox
-00000890: 225d 203d 2061 7474 7269 6275 7465 732e  "] = attributes.
-000008a0: 6765 7428 2276 6965 7742 6f78 222c 2076  get("viewBox", v
-000008b0: 6965 775f 626f 7829 0d0a 2020 2020 2020  iew_box)..      
-000008c0: 2020 6174 7472 6962 7574 6573 5b22 7769    attributes["wi
-000008d0: 6474 6822 5d20 3d20 6174 7472 6962 7574  dth"] = attribut
-000008e0: 6573 2e67 6574 2822 7769 6474 6822 2c20  es.get("width", 
-000008f0: 7069 7865 6c5f 7769 6474 6829 0d0a 2020  pixel_width)..  
-00000900: 2020 2020 2020 6174 7472 6962 7574 6573        attributes
-00000910: 5b22 6865 6967 6874 225d 203d 2061 7474  ["height"] = att
-00000920: 7269 6275 7465 732e 6765 7428 2268 6569  ributes.get("hei
-00000930: 6768 7422 2c20 7069 7865 6c5f 6865 6967  ght", pixel_heig
-00000940: 6874 290d 0a20 2020 2023 2063 616e 206f  ht)..    # can o
-00000950: 6e6c 7920 7061 7373 206e 736d 6170 206f  nly pass nsmap o
-00000960: 6e20 696e 7374 616e 6365 2063 7265 6174  n instance creat
-00000970: 696f 6e0d 0a20 2020 2073 7667 5f72 6f6f  ion..    svg_roo
-00000980: 7420 3d20 6574 7265 652e 456c 656d 656e  t = etree.Elemen
-00000990: 7428 6622 7b7b 7b6e 736d 6170 5b4e 6f6e  t(f"{{{nsmap[Non
-000009a0: 655d 7d7d 7d73 7667 222c 206e 736d 6170  e]}}}svg", nsmap
-000009b0: 3d6e 736d 6170 290d 0a20 2020 2072 6574  =nsmap)..    ret
-000009c0: 7572 6e20 7570 6461 7465 5f65 6c65 6d65  urn update_eleme
-000009d0: 6e74 2873 7667 5f72 6f6f 742c 202a 2a61  nt(svg_root, **a
-000009e0: 7474 7269 6275 7465 7329 0d0a 0d0a 0d0a  ttributes)......
-000009f0: 6465 6620 7772 6974 655f 7376 6728 0d0a  def write_svg(..
-00000a00: 2020 2020 7376 673a 2055 6e69 6f6e 5b73      svg: Union[s
-00000a10: 7472 2c20 494f 5b62 7974 6573 5d5d 2c0d  tr, IO[bytes]],.
-00000a20: 0a20 2020 2078 6d6c 3a20 6574 7265 652e  .    xml: etree.
-00000a30: 456c 656d 656e 742c 0d0a 2020 2020 7374  Element,..    st
-00000a40: 796c 6573 6865 6574 3a20 4f70 7469 6f6e  ylesheet: Option
-00000a50: 616c 5b73 7472 5d20 3d20 4e6f 6e65 2c0d  al[str] = None,.
-00000a60: 0a20 2020 2064 6f5f 6c69 6e6b 5f63 7373  .    do_link_css
-00000a70: 3a20 626f 6f6c 203d 2046 616c 7365 2c0d  : bool = False,.
-00000a80: 0a20 2020 202a 2a74 6f73 7472 696e 675f  .    **tostring_
-00000a90: 6b77 6172 6773 2c0d 0a29 202d 3e20 7374  kwargs,..) -> st
-00000aa0: 723a 0d0a 2020 2020 2222 220d 0a20 2020  r:..    """..   
-00000ab0: 2057 7269 7465 2061 6e20 786d 6c20 656c   Write an xml el
-00000ac0: 656d 656e 7420 6173 2061 6e20 7376 6720  ement as an svg 
-00000ad0: 6669 6c65 2e0d 0a0d 0a20 2020 203a 7061  file.....    :pa
-00000ae0: 7261 6d20 7376 673a 206f 7065 6e20 6269  ram svg: open bi
-00000af0: 6e61 7279 2066 696c 6520 6f62 6a65 6374  nary file object
-00000b00: 206f 7220 7061 7468 2074 6f20 6f75 7470   or path to outp
-00000b10: 7574 2066 696c 6520 2869 6e63 6c75 6465  ut file (include
-00000b20: 2065 7874 656e 7369 6f6e 202e 7376 6729   extension .svg)
-00000b30: 0d0a 2020 2020 3a70 6172 616d 2078 6d6c  ..    :param xml
-00000b40: 3a20 726f 6f74 206e 6f64 6520 6f66 2079  : root node of y
-00000b50: 6f75 7220 7376 6720 6765 6f6d 6574 7279  our svg geometry
-00000b60: 0d0a 2020 2020 3a70 6172 616d 2073 7479  ..    :param sty
-00000b70: 6c65 7368 6565 743a 206f 7074 696f 6e61  lesheet: optiona
-00000b80: 6c20 7061 7468 2074 6f20 6373 7320 7374  l path to css st
-00000b90: 796c 6573 6865 6574 0d0a 2020 2020 3a70  ylesheet..    :p
-00000ba0: 6172 616d 2064 6f5f 6c69 6e6b 5f63 7373  aram do_link_css
-00000bb0: 3a20 6c69 6e6b 2074 6f20 7374 796c 6573  : link to styles
-00000bc0: 6865 6574 2c20 656c 7365 2028 6465 6661  heet, else (defa
-00000bd0: 756c 7429 2077 7269 7465 2063 6f6e 7465  ult) write conte
-00000be0: 6e74 7320 6f66 2073 7479 6c65 7368 6565  nts of styleshee
-00000bf0: 740d 0a20 2020 2020 2020 2069 6e74 6f20  t..        into 
-00000c00: 7376 6720 2869 676e 6f72 6564 2069 6620  svg (ignored if 
-00000c10: 7374 796c 6573 6865 6574 2069 7320 4e6f  stylesheet is No
-00000c20: 6e65 290d 0a20 2020 203a 7061 7261 6d20  ne)..    :param 
-00000c30: 746f 7374 7269 6e67 5f6b 7761 7267 733a  tostring_kwargs:
-00000c40: 206b 6579 776f 7264 2061 7267 756d 656e   keyword argumen
-00000c50: 7473 2074 6f20 6574 7265 652e 746f 7374  ts to etree.tost
-00000c60: 7269 6e67 2e20 786d 6c5f 6865 6164 6572  ring. xml_header
-00000c70: 3d54 7275 6520 666f 720d 0a20 2020 2020  =True for..     
-00000c80: 2020 2073 656e 7369 626c 6520 6465 6661     sensible defa
-00000c90: 756c 7420 7661 6c75 6573 2e20 5365 6520  ult values. See 
-00000ca0: 6265 6c6f 772e 0d0a 2020 2020 3a72 6574  below...    :ret
-00000cb0: 7572 6e3a 2073 7667 2066 696c 656e 616d  urn: svg filenam
-00000cc0: 650d 0a20 2020 203a 6566 6665 6374 733a  e..    :effects:
-00000cd0: 2063 7265 6174 6573 2073 7667 2066 696c   creates svg fil
-00000ce0: 6520 6174 2060 6073 7667 6060 0d0a 0d0a  e at ``svg``....
-00000cf0: 2020 2020 4974 2773 206f 6674 656e 2075      It's often u
-00000d00: 7365 6675 6c20 746f 2077 7269 7465 2061  seful to write a
-00000d10: 2074 656d 706f 7261 7279 2073 7667 2066   temporary svg f
-00000d20: 696c 652c 2073 6f20 6120 7465 6d70 6669  ile, so a tempfi
-00000d30: 6c65 2e4e 616d 6564 5465 6d70 6f72 6172  le.NamedTemporar
-00000d40: 7946 696c 650d 0a20 2020 206f 626a 6563  yFile..    objec
-00000d50: 7420 286f 7220 616e 7920 6f70 656e 2062  t (or any open b
-00000d60: 696e 6172 7920 6669 6c65 206f 626a 6563  inary file objec
-00000d70: 7420 6361 6e20 6265 2070 6173 7365 6420  t can be passed 
-00000d80: 696e 7374 6561 6420 6f66 2061 6e20 7376  instead of an sv
-00000d90: 6720 6669 6c65 6e61 6d65 292e 0d0a 0d0a  g filename).....
-00000da0: 2020 2020 596f 7520 6d61 7920 6e65 7665      You may neve
-00000db0: 7220 6e65 6564 2061 6e20 786d 6c5f 6865  r need an xml_he
-00000dc0: 6164 6572 2e20 496e 6b73 6361 7065 2064  ader. Inkscape d
-00000dd0: 6f65 736e 2774 206e 6565 6420 6974 2c20  oesn't need it, 
-00000de0: 796f 7572 2062 726f 7773 6572 2064 6f65  your browser doe
-00000df0: 736e 2774 0d0a 2020 2020 6e65 6564 2069  sn't..    need i
-00000e00: 742c 2061 6e64 2069 7427 7320 666f 7262  t, and it's forb
-00000e10: 6964 6465 6e20 6966 2079 6f75 2764 206c  idden if you'd l
-00000e20: 696b 6520 746f 2022 696e 6c69 6e65 2220  ike to "inline" 
-00000e30: 796f 7572 2073 7667 2069 6e20 616e 2068  your svg in an h
-00000e40: 746d 6c20 6669 6c65 2e0d 0a20 2020 2054  tml file...    T
-00000e50: 6865 206d 6f73 7420 7072 6573 7369 6e67  he most pressing
-00000e60: 206e 6565 6420 6d69 6768 7420 6265 2074   need might be t
-00000e70: 6f20 7365 7420 616e 2065 6e63 6f64 696e  o set an encodin
-00000e80: 672e 2049 6620 796f 7520 7061 7373 0d0a  g. If you pass..
-00000e90: 2020 2020 6060 786d 6c5f 6465 636c 6172      ``xml_declar
-00000ea0: 6174 696f 6e3d 5472 7565 6060 2061 7320  ation=True`` as 
-00000eb0: 6120 746f 7374 7269 6e67 5f6b 7761 7267  a tostring_kwarg
-00000ec0: 2c20 7468 6973 2066 756e 6374 696f 6e20  , this function 
-00000ed0: 7769 6c6c 2061 7474 656d 7074 2074 6f20  will attempt to 
-00000ee0: 7061 7373 0d0a 2020 2020 7468 6520 666f  pass..    the fo
-00000ef0: 6c6c 6f77 696e 6720 6465 6661 756c 7473  llowing defaults
-00000f00: 2074 6f20 6060 6c78 6d6c 2e65 7472 6565   to ``lxml.etree
-00000f10: 2e74 6f73 7472 696e 6760 603a 0d0a 0d0a  .tostring``:....
-00000f20: 2020 2020 2a20 646f 6374 7970 653a 2073      * doctype: s
-00000f30: 7472 203d 2028 0d0a 2020 2020 2020 2020  tr = (..        
-00000f40: 273c 2144 4f43 5459 5045 2073 7667 2050  '<!DOCTYPE svg P
-00000f50: 5542 4c49 4320 222d 2f2f 5733 432f 2f44  UBLIC "-//W3C//D
-00000f60: 5444 2053 5647 2031 2e31 2f2f 454e 225c  TD SVG 1.1//EN"\
-00000f70: 6e27 0d0a 2020 2020 2020 2020 2722 6874  n'..        '"ht
-00000f80: 7470 3a2f 2f77 7777 2e77 332e 6f72 672f  tp://www.w3.org/
-00000f90: 4772 6170 6869 6373 2f53 5647 2f31 2e31  Graphics/SVG/1.1
-00000fa0: 2f44 5444 2f73 7667 3131 2e64 7464 223e  /DTD/svg11.dtd">
-00000fb0: 270d 0a20 2020 2029 0d0a 2020 2020 2a20  '..    )..    * 
-00000fc0: 656e 636f 6469 6e67 203d 2022 5554 462d  encoding = "UTF-
-00000fd0: 3822 0d0a 0d0a 2020 2020 416c 7761 7973  8"....    Always
-00000fe0: 2c20 7468 6973 2066 756e 6374 696f 6e20  , this function 
-00000ff0: 7769 6c6c 2064 6566 6175 6c74 2074 6f20  will default to 
-00001000: 6060 7072 6574 7479 5f70 7269 6e74 3d54  ``pretty_print=T
-00001010: 7275 6560 600d 0a0d 0a20 2020 2054 6865  rue``....    The
-00001020: 7365 2063 616e 2062 6520 6f76 6572 7269  se can be overri
-00001030: 6464 656e 2062 7920 746f 7374 7269 6e67  dden by tostring
-00001040: 5f6b 7761 7267 732e 0d0a 0d0a 2020 2020  _kwargs.....    
-00001050: 652e 672e 2c20 6060 7772 6974 655f 7376  e.g., ``write_sv
-00001060: 6728 2e2e 2e2c 2078 6d6c 5f64 6563 6c61  g(..., xml_decla
-00001070: 7261 7469 6f6e 3d54 7275 652c 2064 6f63  ration=True, doc
-00001080: 7479 7065 3d4e 6f6e 6560 6029 0d0a 2020  type=None``)..  
-00001090: 2020 652e 672e 2c20 6060 7772 6974 655f    e.g., ``write_
-000010a0: 7376 6728 2e2e 2e2c 2078 6d6c 5f64 6563  svg(..., xml_dec
-000010b0: 6c61 7261 7469 6f6e 3d54 7275 652c 2065  laration=True, e
-000010c0: 6e63 6f64 696e 673d 2761 7363 6969 2729  ncoding='ascii')
-000010d0: 6060 0d0a 0d0a 2020 2020 6060 6c78 6d6c  ``....    ``lxml
-000010e0: 2e65 7472 6565 2e74 6f73 7472 696e 6760  .etree.tostring`
-000010f0: 6020 6973 2064 6f63 756d 656e 7465 6420  ` is documented 
-00001100: 6865 7265 3a20 6874 7470 733a 2f2f 6c78  here: https://lx
-00001110: 6d6c 2e64 652f 6170 692f 696e 6465 782e  ml.de/api/index.
-00001120: 6874 6d6c 2c0d 0a20 2020 2062 7574 2049  html,..    but I
-00001130: 206b 6e6f 7720 7468 6174 2074 6f20 6265   know that to be
-00001140: 2069 6e63 6f6d 706c 6574 6520 6173 206f   incomplete as o
-00001150: 6620 3230 3230 2046 6562 2030 312c 2061  f 2020 Feb 01, a
-00001160: 7320 6974 2064 6f65 7320 6e6f 7420 646f  s it does not do
-00001170: 6375 6d65 6e74 2074 6865 0d0a 2020 2020  cument the..    
-00001180: 2870 6572 6861 7073 2069 6d70 6f72 7461  (perhaps importa
-00001190: 6e74 2074 6f20 796f 7529 2027 656e 636f  nt to you) 'enco
-000011a0: 6469 6e67 2720 6b77 6172 672e 0d0a 2020  ding' kwarg...  
-000011b0: 2020 2222 220d 0a20 2020 2069 6620 7374    """..    if st
-000011c0: 796c 6573 6865 6574 2069 7320 6e6f 7420  ylesheet is not 
-000011d0: 4e6f 6e65 3a0d 0a20 2020 2020 2020 2069  None:..        i
-000011e0: 6620 646f 5f6c 696e 6b5f 6373 7320 6973  f do_link_css is
-000011f0: 2054 7275 653a 0d0a 2020 2020 2020 2020   True:..        
-00001200: 2020 2020 7265 6c61 7469 7665 5f63 7373      relative_css
-00001210: 5f70 6174 6820 3d20 5061 7468 2873 7479  _path = Path(sty
-00001220: 6c65 7368 6565 7429 2e72 656c 6174 6976  lesheet).relativ
-00001230: 655f 746f 2850 6174 6828 7376 6729 2e70  e_to(Path(svg).p
-00001240: 6172 656e 7429 0d0a 2020 2020 2020 2020  arent)..        
-00001250: 2020 2020 6c69 6e6b 203d 2065 7472 6565      link = etree
-00001260: 2e50 4928 0d0a 2020 2020 2020 2020 2020  .PI(..          
-00001270: 2020 2020 2020 2278 6d6c 2d73 7479 6c65        "xml-style
-00001280: 7368 6565 7422 2c20 6627 6872 6566 3d22  sheet", f'href="
-00001290: 7b72 656c 6174 6976 655f 6373 735f 7061  {relative_css_pa
-000012a0: 7468 7d22 2074 7970 653d 2274 6578 742f  th}" type="text/
-000012b0: 6373 7322 270d 0a20 2020 2020 2020 2020  css"'..         
-000012c0: 2020 2029 0d0a 2020 2020 2020 2020 2020     )..          
-000012d0: 2020 786d 6c2e 6164 6470 7265 7669 6f75    xml.addpreviou
-000012e0: 7328 6c69 6e6b 290d 0a20 2020 2020 2020  s(link)..       
-000012f0: 2065 6c73 653a 0d0a 2020 2020 2020 2020   else:..        
-00001300: 2020 2020 7374 796c 6520 3d20 6574 7265      style = etre
-00001310: 652e 456c 656d 656e 7428 2273 7479 6c65  e.Element("style
-00001320: 222c 2074 7970 653d 2274 6578 742f 6373  ", type="text/cs
-00001330: 7322 290d 0a20 2020 2020 2020 2020 2020  s")..           
-00001340: 2077 6974 6820 6f70 656e 2873 7479 6c65   with open(style
-00001350: 7368 6565 7429 2061 7320 6373 735f 6669  sheet) as css_fi
-00001360: 6c65 3a0d 0a20 2020 2020 2020 2020 2020  le:..           
-00001370: 2020 2020 2073 7479 6c65 2e74 6578 7420       style.text 
-00001380: 3d20 6574 7265 652e 4344 4154 4128 225c  = etree.CDATA("\
-00001390: 6e22 202b 2022 222e 6a6f 696e 2863 7373  n" + "".join(css
-000013a0: 5f66 696c 652e 7265 6164 6c69 6e65 7328  _file.readlines(
-000013b0: 2929 202b 2022 5c6e 2229 0d0a 2020 2020  )) + "\n")..    
-000013c0: 2020 2020 2020 2020 786d 6c2e 696e 7365          xml.inse
-000013d0: 7274 2830 2c20 7374 796c 6529 0d0a 0d0a  rt(0, style)....
-000013e0: 2020 2020 7376 675f 636f 6e74 656e 7473      svg_contents
-000013f0: 203d 2073 7667 5f74 6f73 7472 696e 6728   = svg_tostring(
-00001400: 786d 6c2c 202a 2a74 6f73 7472 696e 675f  xml, **tostring_
-00001410: 6b77 6172 6773 290d 0a0d 0a20 2020 2074  kwargs)....    t
-00001420: 7279 3a0d 0a20 2020 2020 2020 2073 7667  ry:..        svg
-00001430: 2e77 7269 7465 2873 7667 5f63 6f6e 7465  .write(svg_conte
-00001440: 6e74 7329 0d0a 2020 2020 2020 2020 7265  nts)..        re
-00001450: 7475 726e 2073 7667 2e6e 616d 650d 0a20  turn svg.name.. 
-00001460: 2020 2065 7863 6570 7420 4174 7472 6962     except Attrib
-00001470: 7574 6545 7272 6f72 3a0d 0a20 2020 2020  uteError:..     
-00001480: 2020 2077 6974 6820 6f70 656e 2873 7667     with open(svg
-00001490: 2c20 2277 6222 2920 6173 2073 7667 5f66  , "wb") as svg_f
-000014a0: 696c 653a 0d0a 2020 2020 2020 2020 2020  ile:..          
-000014b0: 2020 7376 675f 6669 6c65 2e77 7269 7465    svg_file.write
-000014c0: 2873 7667 5f63 6f6e 7465 6e74 7329 0d0a  (svg_contents)..
-000014d0: 2020 2020 2020 2020 7265 7475 726e 2073          return s
-000014e0: 7667 0d0a 0d0a 0d0a 6465 6620 7772 6974  vg......def writ
-000014f0: 655f 706e 675f 6672 6f6d 5f73 7667 2869  e_png_from_svg(i
-00001500: 6e6b 7363 6170 653a 2073 7472 2c20 7376  nkscape: str, sv
-00001510: 673a 2073 7472 2c20 706e 673a 204f 7074  g: str, png: Opt
-00001520: 696f 6e61 6c5b 7374 725d 203d 204e 6f6e  ional[str] = Non
-00001530: 6529 202d 3e20 7374 723a 0d0a 2020 2020  e) -> str:..    
-00001540: 2222 220d 0a20 2020 2043 6f6e 7665 7274  """..    Convert
-00001550: 2061 6e20 7376 6720 6669 6c65 2074 6f20   an svg file to 
-00001560: 6120 706e 670d 0a0d 0a20 2020 203a 7061  a png....    :pa
-00001570: 7261 6d20 696e 6b73 6361 7065 3a20 7061  ram inkscape: pa
-00001580: 7468 2074 6f20 696e 6b73 6361 7065 2065  th to inkscape e
-00001590: 7865 6375 7461 626c 6520 2877 6974 686f  xecutable (witho
-000015a0: 7574 202e 6578 6520 6578 7465 6e73 696f  ut .exe extensio
-000015b0: 6e21 290d 0a20 2020 203a 7061 7261 6d20  n!)..    :param 
-000015c0: 7376 673a 2070 6174 6820 746f 2073 7667  svg: path to svg
-000015d0: 2066 696c 650d 0a20 2020 203a 7061 7261   file..    :para
-000015e0: 6d20 706e 673a 206f 7074 696f 6e61 6c20  m png: optional 
-000015f0: 7061 7468 2074 6f20 706e 6720 6f75 7470  path to png outp
-00001600: 7574 2066 696c 650d 0a20 2020 203a 7265  ut file..    :re
-00001610: 7475 726e 3a20 706e 6720 6669 6c65 6e61  turn: png filena
-00001620: 6d65 0d0a 2020 2020 3a65 6666 6563 7473  me..    :effects
-00001630: 3a20 6372 6561 7465 7320 6120 6e65 7720  : creates a new 
-00001640: 706e 6720 6672 6f6d 2073 7667 2066 696c  png from svg fil
-00001650: 656e 616d 650d 0a0d 0a20 2020 2049 6620  ename....    If 
-00001660: 6e6f 206f 7574 7075 7420 706e 6720 7061  no output png pa
-00001670: 7468 2069 7320 6769 7665 6e2c 2074 6865  th is given, the
-00001680: 206f 7574 7075 7420 7061 7468 2077 696c   output path wil
-00001690: 6c20 6265 2069 6e66 6572 7265 6420 6672  l be inferred fr
-000016a0: 6f6d 2074 6865 2060 6073 7667 6060 0d0a  om the ``svg``..
-000016b0: 2020 2020 6669 6c65 6e61 6d65 2e0d 0a20      filename... 
-000016c0: 2020 2022 2222 0d0a 2020 2020 6966 2070     """..    if p
-000016d0: 6e67 2069 7320 4e6f 6e65 3a0d 0a20 2020  ng is None:..   
-000016e0: 2020 2020 2070 6e67 203d 2073 7472 2850       png = str(P
-000016f0: 6174 6828 7376 6729 2e77 6974 685f 7375  ath(svg).with_su
-00001700: 6666 6978 2822 2e70 6e67 2229 290d 0a0d  ffix(".png"))...
-00001710: 0a20 2020 2023 2069 6e6b 7363 6170 6520  .    # inkscape 
-00001720: 7665 7273 696f 6e73 203e 3d20 312e 300d  versions >= 1.0.
-00001730: 0a20 2020 206f 7074 696f 6e73 203d 205b  .    options = [
-00001740: 6627 227b 7376 677d 2227 2c20 222d 2d65  f'"{svg}"', "--e
-00001750: 7870 6f72 742d 7479 7065 3d70 6e67 222c  xport-type=png",
-00001760: 2066 272d 2d65 7870 6f72 742d 6669 6c65   f'--export-file
-00001770: 6e61 6d65 3d22 7b70 6e67 7d22 275d 0d0a  name="{png}"']..
-00001780: 2020 2020 7265 7475 726e 5f63 6f64 6520      return_code 
-00001790: 3d20 7375 6270 726f 6365 7373 2e63 616c  = subprocess.cal
-000017a0: 6c28 6627 227b 696e 6b73 6361 7065 7d22  l(f'"{inkscape}"
-000017b0: 2027 202b 2022 2022 2e6a 6f69 6e28 6f70   ' + " ".join(op
-000017c0: 7469 6f6e 7329 290d 0a20 2020 2069 6620  tions))..    if 
-000017d0: 7265 7475 726e 5f63 6f64 6520 3d3d 2030  return_code == 0
-000017e0: 3a0d 0a20 2020 2020 2020 2072 6574 7572  :..        retur
-000017f0: 6e20 706e 670d 0a0d 0a20 2020 2023 2069  n png....    # i
-00001800: 6e6b 7363 6170 6520 7665 7273 696f 6e73  nkscape versions
-00001810: 203c 2031 2e30 0d0a 2020 2020 7265 7475   < 1.0..    retu
-00001820: 726e 5f63 6f64 6520 3d20 7375 6270 726f  rn_code = subpro
-00001830: 6365 7373 2e63 616c 6c28 6627 227b 696e  cess.call(f'"{in
-00001840: 6b73 6361 7065 7d22 202d 6620 227b 7376  kscape}" -f "{sv
-00001850: 677d 2220 2d65 2022 7b70 6e67 7d22 2729  g}" -e "{png}"')
-00001860: 0d0a 2020 2020 6966 2072 6574 7572 6e5f  ..    if return_
-00001870: 636f 6465 203d 3d20 303a 0d0a 2020 2020  code == 0:..    
-00001880: 2020 2020 7265 7475 726e 2070 6e67 0d0a      return png..
-00001890: 0d0a 2020 2020 7261 6973 6520 5661 6c75  ..    raise Valu
-000018a0: 6545 7272 6f72 2866 2266 6169 6c65 6420  eError(f"failed 
-000018b0: 746f 2077 7269 7465 207b 706e 677d 2229  to write {png}")
-000018c0: 0d0a 0d0a 0d0a 6465 6620 7772 6974 655f  ......def write_
-000018d0: 706e 6728 0d0a 2020 2020 696e 6b73 6361  png(..    inksca
-000018e0: 7065 3a20 7374 722c 0d0a 2020 2020 706e  pe: str,..    pn
-000018f0: 673a 2073 7472 2c0d 0a20 2020 2078 6d6c  g: str,..    xml
-00001900: 3a20 6574 7265 652e 456c 656d 656e 742c  : etree.Element,
-00001910: 0d0a 2020 2020 7374 796c 6573 6865 6574  ..    stylesheet
-00001920: 3a20 4f70 7469 6f6e 616c 5b73 7472 5d20  : Optional[str] 
-00001930: 3d20 4e6f 6e65 2c0d 0a29 202d 3e20 7374  = None,..) -> st
-00001940: 723a 0d0a 2020 2020 2222 220d 0a20 2020  r:..    """..   
-00001950: 2043 7265 6174 6520 6120 706e 6720 6669   Create a png fi
-00001960: 6c65 2077 6974 686f 7574 2077 7269 7469  le without writi
-00001970: 6e67 2061 6e20 696e 7465 726d 6564 6961  ng an intermedia
-00001980: 7465 2073 7667 2066 696c 652e 0d0a 0d0a  te svg file.....
-00001990: 2020 2020 3a70 6172 616d 2069 6e6b 7363      :param inksc
-000019a0: 6170 653a 2070 6174 6820 746f 2069 6e6b  ape: path to ink
-000019b0: 7363 6170 6520 6578 6563 7574 6162 6c65  scape executable
-000019c0: 2028 7769 7468 6f75 7420 2e65 7865 2065   (without .exe e
-000019d0: 7874 656e 7369 6f6e 2129 0d0a 2020 2020  xtension!)..    
-000019e0: 3a70 6172 616d 2070 6e67 3a20 7061 7468  :param png: path
-000019f0: 2074 6f20 6f75 7470 7574 2070 6e67 2066   to output png f
-00001a00: 696c 650d 0a20 2020 203a 7061 7261 6d20  ile..    :param 
-00001a10: 786d 6c3a 2072 6f6f 7420 6e6f 6465 206f  xml: root node o
-00001a20: 6620 796f 7572 2073 7667 2067 656f 6d65  f your svg geome
-00001a30: 7472 790d 0a20 2020 203a 7061 7261 6d20  try..    :param 
-00001a40: 7374 796c 6573 6865 6574 3a20 6f70 7469  stylesheet: opti
-00001a50: 6f6e 616c 2070 6174 6820 746f 2063 7373  onal path to css
-00001a60: 2073 7479 6c65 7368 6565 740d 0a20 2020   stylesheet..   
-00001a70: 203a 7265 7475 726e 3a20 706e 6720 6669   :return: png fi
-00001a80: 6c65 6e61 6d65 2028 7468 6520 7361 6d65  lename (the same
-00001a90: 2079 6f75 2069 6e70 7574 2061 7320 6060   you input as ``
-00001aa0: 706e 6760 6029 0d0a 2020 2020 3a65 6666  png``)..    :eff
-00001ab0: 6563 7473 3a20 6372 6561 7465 7320 6120  ects: creates a 
-00001ac0: 6e65 7720 706e 6720 6669 6c65 0d0a 0d0a  new png file....
-00001ad0: 2020 2020 5468 6973 206a 7573 7420 6372      This just cr
-00001ae0: 6561 7465 7320 6120 7465 6d70 6669 6c65  eates a tempfile
-00001af0: 2c20 7772 6974 6573 2074 6865 2073 7667  , writes the svg
-00001b00: 2074 6f20 7468 6520 7465 6d70 6669 6c65   to the tempfile
-00001b10: 2c20 7468 656e 2063 616c 6c73 0d0a 2020  , then calls..  
-00001b20: 2020 6060 7772 6974 655f 706e 675f 6672    ``write_png_fr
-00001b30: 6f6d 5f73 7667 6060 2077 6974 6820 7468  om_svg`` with th
-00001b40: 6520 7465 6d70 6669 6c65 2e20 5468 6973  e tempfile. This
-00001b50: 2069 736e 2774 2066 6173 7465 7220 2869   isn't faster (i
-00001b60: 7420 6d69 6768 7420 6265 2073 6c69 6768  t might be sligh
-00001b70: 746c 790d 0a20 2020 2073 6c6f 7765 7229  tly..    slower)
-00001b80: 2c20 6275 7420 6974 206b 6565 7073 2074  , but it keeps t
-00001b90: 6865 2066 696c 6573 7973 7465 6d20 636c  he filesystem cl
-00001ba0: 6561 6e20 7768 656e 2079 6f75 206f 6e6c  ean when you onl
-00001bb0: 7920 7761 6e74 2074 6865 2070 6e67 2e0d  y want the png..
-00001bc0: 0a20 2020 2022 2222 0d0a 2020 2020 7769  .    """..    wi
-00001bd0: 7468 204e 616d 6564 5465 6d70 6f72 6172  th NamedTemporar
-00001be0: 7946 696c 6528 6d6f 6465 3d22 7762 222c  yFile(mode="wb",
-00001bf0: 2064 656c 6574 653d 4661 6c73 6529 2061   delete=False) a
-00001c00: 7320 7376 675f 6669 6c65 3a0d 0a20 2020  s svg_file:..   
-00001c10: 2020 2020 2073 7667 203d 2077 7269 7465       svg = write
-00001c20: 5f73 7667 2873 7667 5f66 696c 652c 2078  _svg(svg_file, x
-00001c30: 6d6c 2c20 7374 796c 6573 6865 6574 290d  ml, stylesheet).
-00001c40: 0a20 2020 2077 7269 7465 5f70 6e67 5f66  .    write_png_f
-00001c50: 726f 6d5f 7376 6728 696e 6b73 6361 7065  rom_svg(inkscape
-00001c60: 2c20 7376 672c 2070 6e67 290d 0a20 2020  , svg, png)..   
-00001c70: 206f 732e 756e 6c69 6e6b 2873 7667 290d   os.unlink(svg).
-00001c80: 0a20 2020 2072 6574 7572 6e20 706e 670d  .    return png.
-00001c90: 0a0d 0a0d 0a64 6566 2077 7269 7465 5f70  .....def write_p
-00001ca0: 6466 5f66 726f 6d5f 7376 6728 696e 6b73  df_from_svg(inks
-00001cb0: 6361 7065 3a20 7374 722c 2073 7667 3a20  cape: str, svg: 
-00001cc0: 7374 722c 2070 6466 3a20 4f70 7469 6f6e  str, pdf: Option
-00001cd0: 616c 5b73 7472 5d20 3d20 4e6f 6e65 2920  al[str] = None) 
-00001ce0: 2d3e 2073 7472 3a0d 0a20 2020 2022 2222  -> str:..    """
-00001cf0: 0d0a 2020 2020 436f 6e76 6572 7420 616e  ..    Convert an
-00001d00: 2073 7667 2066 696c 6520 746f 2061 2070   svg file to a p
-00001d10: 6466 0d0a 0d0a 2020 2020 3a70 6172 616d  df....    :param
-00001d20: 2069 6e6b 7363 6170 653a 2070 6174 6820   inkscape: path 
-00001d30: 746f 2069 6e6b 7363 6170 6520 6578 6563  to inkscape exec
-00001d40: 7574 6162 6c65 2028 7769 7468 6f75 7420  utable (without 
-00001d50: 2e65 7865 2065 7874 656e 7369 6f6e 2129  .exe extension!)
-00001d60: 0d0a 2020 2020 3a70 6172 616d 2073 7667  ..    :param svg
-00001d70: 3a20 7061 7468 2074 6f20 7376 6720 6669  : path to svg fi
-00001d80: 6c65 0d0a 2020 2020 3a70 6172 616d 2070  le..    :param p
-00001d90: 6466 3a20 6f70 7469 6f6e 616c 2070 6174  df: optional pat
-00001da0: 6820 746f 2070 6e67 206f 7574 7075 7420  h to png output 
-00001db0: 6669 6c65 0d0a 2020 2020 3a72 6574 7572  file..    :retur
-00001dc0: 6e3a 2070 6466 2066 696c 656e 616d 650d  n: pdf filename.
-00001dd0: 0a20 2020 203a 6566 6665 6374 733a 2063  .    :effects: c
-00001de0: 7265 6174 6573 2061 206e 6577 2070 6664  reates a new pfd
-00001df0: 2066 726f 6d20 7376 6720 6669 6c65 6e61   from svg filena
-00001e00: 6d65 0d0a 0d0a 2020 2020 4966 206e 6f20  me....    If no 
-00001e10: 6f75 7470 7574 2070 6e67 2070 6174 6820  output png path 
-00001e20: 6973 2067 6976 656e 2c20 7468 6520 6f75  is given, the ou
-00001e30: 7470 7574 2070 6174 6820 7769 6c6c 2062  tput path will b
-00001e40: 6520 696e 6665 7272 6564 2066 726f 6d20  e inferred from 
-00001e50: 7468 6520 6060 7376 6760 600d 0a20 2020  the ``svg``..   
-00001e60: 2066 696c 656e 616d 652e 0d0a 2020 2020   filename...    
-00001e70: 2222 220d 0a20 2020 2069 6620 7064 6620  """..    if pdf 
-00001e80: 6973 204e 6f6e 653a 0d0a 2020 2020 2020  is None:..      
-00001e90: 2020 7064 6620 3d20 7374 7228 5061 7468    pdf = str(Path
-00001ea0: 2873 7667 292e 7769 7468 5f73 7566 6669  (svg).with_suffi
-00001eb0: 7828 222e 7064 6622 2929 0d0a 0d0a 2020  x(".pdf"))....  
-00001ec0: 2020 2320 696e 6b73 6361 7065 2076 6572    # inkscape ver
-00001ed0: 7369 6f6e 7320 3e3d 2031 2e30 0d0a 2020  sions >= 1.0..  
-00001ee0: 2020 6f70 7469 6f6e 7320 3d20 5b66 2722    options = [f'"
-00001ef0: 7b73 7667 7d22 272c 2022 2d2d 6578 706f  {svg}"', "--expo
-00001f00: 7274 2d74 7970 653d 7064 6622 2c20 6627  rt-type=pdf", f'
-00001f10: 2d2d 6578 706f 7274 2d66 696c 656e 616d  --export-filenam
-00001f20: 653d 227b 7064 667d 2227 5d0d 0a20 2020  e="{pdf}"']..   
-00001f30: 2072 6574 7572 6e5f 636f 6465 203d 2073   return_code = s
-00001f40: 7562 7072 6f63 6573 732e 6361 6c6c 2866  ubprocess.call(f
-00001f50: 2722 7b69 6e6b 7363 6170 657d 2220 2720  '"{inkscape}" ' 
-00001f60: 2b20 2220 222e 6a6f 696e 286f 7074 696f  + " ".join(optio
-00001f70: 6e73 2929 0d0a 2020 2020 6966 2072 6574  ns))..    if ret
-00001f80: 7572 6e5f 636f 6465 203d 3d20 303a 0d0a  urn_code == 0:..
-00001f90: 2020 2020 2020 2020 7265 7475 726e 2070          return p
-00001fa0: 6466 0d0a 0d0a 2020 2020 2320 696e 6b73  df....    # inks
-00001fb0: 6361 7065 2076 6572 7369 6f6e 7320 3c20  cape versions < 
-00001fc0: 312e 300d 0a20 2020 2072 6574 7572 6e5f  1.0..    return_
-00001fd0: 636f 6465 203d 2073 7562 7072 6f63 6573  code = subproces
-00001fe0: 732e 6361 6c6c 2866 2722 7b69 6e6b 7363  s.call(f'"{inksc
-00001ff0: 6170 657d 2220 2d66 2022 7b73 7667 7d22  ape}" -f "{svg}"
-00002000: 202d 6520 227b 7064 667d 2227 290d 0a20   -e "{pdf}"').. 
-00002010: 2020 2069 6620 7265 7475 726e 5f63 6f64     if return_cod
-00002020: 6520 3d3d 2030 3a0d 0a20 2020 2020 2020  e == 0:..       
-00002030: 2072 6574 7572 6e20 7064 660d 0a0d 0a20   return pdf.... 
-00002040: 2020 2072 6169 7365 2056 616c 7565 4572     raise ValueEr
-00002050: 726f 7228 6622 6661 696c 6564 2074 6f20  ror(f"failed to 
-00002060: 7772 6974 6520 7b70 6466 7d22 290d 0a0d  write {pdf}")...
-00002070: 0a0d 0a64 6566 2077 7269 7465 5f70 6466  ...def write_pdf
-00002080: 280d 0a20 2020 2069 6e6b 7363 6170 653a  (..    inkscape:
-00002090: 2073 7472 2c0d 0a20 2020 2070 6466 3a20   str,..    pdf: 
-000020a0: 7374 722c 0d0a 2020 2020 786d 6c3a 2065  str,..    xml: e
-000020b0: 7472 6565 2e45 6c65 6d65 6e74 2c0d 0a20  tree.Element,.. 
-000020c0: 2020 2073 7479 6c65 7368 6565 743a 204f     stylesheet: O
-000020d0: 7074 696f 6e61 6c5b 7374 725d 203d 204e  ptional[str] = N
-000020e0: 6f6e 652c 0d0a 2920 2d3e 2073 7472 3a0d  one,..) -> str:.
-000020f0: 0a20 2020 2022 2222 0d0a 2020 2020 4372  .    """..    Cr
-00002100: 6561 7465 2061 2070 6466 2066 696c 6520  eate a pdf file 
-00002110: 7769 7468 6f75 7420 7772 6974 696e 6720  without writing 
-00002120: 616e 2069 6e74 6572 6d65 6469 6174 6520  an intermediate 
-00002130: 7376 6720 6669 6c65 2e0d 0a0d 0a20 2020  svg file.....   
-00002140: 203a 7061 7261 6d20 696e 6b73 6361 7065   :param inkscape
-00002150: 3a20 7061 7468 2074 6f20 696e 6b73 6361  : path to inksca
-00002160: 7065 2065 7865 6375 7461 626c 6520 2877  pe executable (w
-00002170: 6974 686f 7574 202e 6578 6520 6578 7465  ithout .exe exte
-00002180: 6e73 696f 6e21 290d 0a20 2020 203a 7061  nsion!)..    :pa
-00002190: 7261 6d20 7064 663a 2070 6174 6820 746f  ram pdf: path to
-000021a0: 206f 7574 7075 7420 7064 6620 6669 6c65   output pdf file
-000021b0: 0d0a 2020 2020 3a70 6172 616d 2078 6d6c  ..    :param xml
-000021c0: 3a20 726f 6f74 206e 6f64 6520 6f66 2079  : root node of y
-000021d0: 6f75 7220 7376 6720 6765 6f6d 6574 7279  our svg geometry
-000021e0: 0d0a 2020 2020 3a70 6172 616d 2073 7479  ..    :param sty
-000021f0: 6c65 7368 6565 743a 206f 7074 696f 6e61  lesheet: optiona
-00002200: 6c20 7061 7468 2074 6f20 6373 7320 7374  l path to css st
-00002210: 796c 6573 6865 6574 0d0a 2020 2020 3a72  ylesheet..    :r
-00002220: 6574 7572 6e3a 2070 6466 2066 696c 656e  eturn: pdf filen
-00002230: 616d 6520 2874 6865 2073 616d 6520 796f  ame (the same yo
-00002240: 7520 696e 7075 7420 6173 2060 6070 6466  u input as ``pdf
-00002250: 6060 290d 0a20 2020 203a 6566 6665 6374  ``)..    :effect
-00002260: 733a 2063 7265 6174 6573 2061 206e 6577  s: creates a new
-00002270: 2070 6466 2066 696c 650d 0a0d 0a20 2020   pdf file....   
-00002280: 2054 6869 7320 6a75 7374 2063 7265 6174   This just creat
-00002290: 6573 2061 2074 656d 7066 696c 652c 2077  es a tempfile, w
-000022a0: 7269 7465 7320 7468 6520 7376 6720 746f  rites the svg to
-000022b0: 2074 6865 2074 656d 7066 696c 652c 2074   the tempfile, t
-000022c0: 6865 6e20 6361 6c6c 730d 0a20 2020 2060  hen calls..    `
-000022d0: 6077 7269 7465 5f70 6466 5f66 726f 6d5f  `write_pdf_from_
-000022e0: 7376 6760 6020 7769 7468 2074 6865 2074  svg`` with the t
-000022f0: 656d 7066 696c 652e 2054 6869 7320 6973  empfile. This is
-00002300: 6e27 7420 6661 7374 6572 2028 6974 206d  n't faster (it m
-00002310: 6967 6874 2062 6520 736c 6967 6874 6c79  ight be slightly
-00002320: 0d0a 2020 2020 736c 6f77 6572 292c 2062  ..    slower), b
-00002330: 7574 2069 7420 6b65 6570 7320 7468 6520  ut it keeps the 
-00002340: 6669 6c65 7379 7374 656d 2063 6c65 616e  filesystem clean
-00002350: 2077 6865 6e20 796f 7520 6f6e 6c79 2077   when you only w
-00002360: 616e 7420 7468 6520 7064 662e 0d0a 2020  ant the pdf...  
-00002370: 2020 2222 220d 0a20 2020 2077 6974 6820    """..    with 
-00002380: 4e61 6d65 6454 656d 706f 7261 7279 4669  NamedTemporaryFi
-00002390: 6c65 286d 6f64 653d 2277 6222 2c20 6465  le(mode="wb", de
-000023a0: 6c65 7465 3d46 616c 7365 2920 6173 2073  lete=False) as s
-000023b0: 7667 5f66 696c 653a 0d0a 2020 2020 2020  vg_file:..      
-000023c0: 2020 7376 6720 3d20 7772 6974 655f 7376    svg = write_sv
-000023d0: 6728 7376 675f 6669 6c65 2c20 786d 6c2c  g(svg_file, xml,
-000023e0: 2073 7479 6c65 7368 6565 7429 0d0a 2020   stylesheet)..  
-000023f0: 2020 7772 6974 655f 7064 665f 6672 6f6d    write_pdf_from
-00002400: 5f73 7667 2869 6e6b 7363 6170 652c 2073  _svg(inkscape, s
-00002410: 7667 2c20 7064 6629 0d0a 2020 2020 6f73  vg, pdf)..    os
-00002420: 2e75 6e6c 696e 6b28 7376 6729 0d0a 2020  .unlink(svg)..  
-00002430: 2020 7265 7475 726e 2070 6466 0d0a         return pdf..
+00000270: 2069 6d70 6f72 7420 494f 2c20 4469 6374   import IO, Dict
+00000280: 2c20 4f70 7469 6f6e 616c 2c20 5479 7065  , Optional, Type
+00000290: 416c 6961 732c 2055 6e69 6f6e 2c20 6361  Alias, Union, ca
+000002a0: 7374 0d0a 0d0a 6672 6f6d 206c 786d 6c20  st....from lxml 
+000002b0: 696d 706f 7274 2065 7472 6565 0d0a 0d0a  import etree....
+000002c0: 6672 6f6d 2073 7667 5f75 6c74 7261 6c69  from svg_ultrali
+000002d0: 6768 742e 636f 6e73 7472 7563 746f 7273  ght.constructors
+000002e0: 2069 6d70 6f72 7420 7570 6461 7465 5f65   import update_e
+000002f0: 6c65 6d65 6e74 0d0a 6672 6f6d 2073 7667  lement..from svg
+00000300: 5f75 6c74 7261 6c69 6768 742e 6e73 6d61  _ultralight.nsma
+00000310: 7020 696d 706f 7274 204e 534d 4150 0d0a  p import NSMAP..
+00000320: 6672 6f6d 2073 7667 5f75 6c74 7261 6c69  from svg_ultrali
+00000330: 6768 742e 7374 7269 6e67 5f63 6f6e 7665  ght.string_conve
+00000340: 7273 696f 6e20 696d 706f 7274 2028 0d0a  rsion import (..
+00000350: 2020 2020 666f 726d 6174 5f6e 756d 6265      format_numbe
+00000360: 722c 0d0a 2020 2020 6765 745f 7669 6577  r,..    get_view
+00000370: 426f 785f 7374 722c 0d0a 2020 2020 7376  Box_str,..    sv
+00000380: 675f 746f 7374 7269 6e67 2c0d 0a29 0d0a  g_tostring,..)..
+00000390: 0d0a 5f45 6c65 6d65 6e74 3a20 5479 7065  .._Element: Type
+000003a0: 416c 6961 7320 3d20 6574 7265 652e 5f45  Alias = etree._E
+000003b0: 6c65 6d65 6e74 2020 2320 7479 7065 3a20  lement  # type: 
+000003c0: 6967 6e6f 7265 0d0a 0d0a 0d0a 6465 6620  ignore......def 
+000003d0: 6e65 775f 7376 675f 726f 6f74 280d 0a20  new_svg_root(.. 
+000003e0: 2020 2078 5f3a 204f 7074 696f 6e61 6c5b     x_: Optional[
+000003f0: 666c 6f61 745d 203d 204e 6f6e 652c 0d0a  float] = None,..
+00000400: 2020 2020 795f 3a20 4f70 7469 6f6e 616c      y_: Optional
+00000410: 5b66 6c6f 6174 5d20 3d20 4e6f 6e65 2c0d  [float] = None,.
+00000420: 0a20 2020 2077 6964 7468 5f3a 204f 7074  .    width_: Opt
+00000430: 696f 6e61 6c5b 666c 6f61 745d 203d 204e  ional[float] = N
+00000440: 6f6e 652c 0d0a 2020 2020 6865 6967 6874  one,..    height
+00000450: 5f3a 204f 7074 696f 6e61 6c5b 666c 6f61  _: Optional[floa
+00000460: 745d 203d 204e 6f6e 652c 0d0a 2020 2020  t] = None,..    
+00000470: 7061 645f 3a20 666c 6f61 7420 3d20 302c  pad_: float = 0,
+00000480: 0d0a 2020 2020 6470 755f 3a20 666c 6f61  ..    dpu_: floa
+00000490: 7420 3d20 312c 0d0a 2020 2020 6e73 6d61  t = 1,..    nsma
+000004a0: 703a 204f 7074 696f 6e61 6c5b 4469 6374  p: Optional[Dict
+000004b0: 5b55 6e69 6f6e 5b73 7472 2c20 4e6f 6e65  [Union[str, None
+000004c0: 5d2c 2073 7472 5d5d 203d 204e 6f6e 652c  ], str]] = None,
+000004d0: 0d0a 2020 2020 2a2a 6174 7472 6962 7574  ..    **attribut
+000004e0: 6573 3a20 556e 696f 6e5b 666c 6f61 742c  es: Union[float,
+000004f0: 2073 7472 5d2c 0d0a 2920 2d3e 205f 456c   str],..) -> _El
+00000500: 656d 656e 743a 0d0a 2020 2020 2222 220d  ement:..    """.
+00000510: 0a20 2020 2043 7265 6174 6520 616e 2073  .    Create an s
+00000520: 7667 2072 6f6f 7420 656c 656d 656e 7420  vg root element 
+00000530: 6672 6f6d 2076 6965 7742 6f78 2073 7479  from viewBox sty
+00000540: 6c65 2070 6172 616d 6574 6572 732e 0d0a  le parameters...
+00000550: 0d0a 2020 2020 3a70 6172 616d 2078 5f3a  ..    :param x_:
+00000560: 2078 2076 616c 7565 2069 6e20 7570 7065   x value in uppe
+00000570: 722d 6c65 6674 2063 6f72 6e65 720d 0a20  r-left corner.. 
+00000580: 2020 203a 7061 7261 6d20 795f 3a20 7920     :param y_: y 
+00000590: 7661 6c75 6520 696e 2075 7070 6572 2d6c  value in upper-l
+000005a0: 6566 7420 636f 726e 6572 0d0a 2020 2020  eft corner..    
+000005b0: 3a70 6172 616d 2077 6964 7468 5f3a 2077  :param width_: w
+000005c0: 6964 7468 206f 6620 7669 6577 426f 780d  idth of viewBox.
+000005d0: 0a20 2020 203a 7061 7261 6d20 6865 6967  .    :param heig
+000005e0: 6874 5f3a 2068 6569 6768 7420 6f66 2076  ht_: height of v
+000005f0: 6965 7742 6f78 0d0a 2020 2020 3a70 6172  iewBox..    :par
+00000600: 616d 2070 6164 5f3a 206f 7074 696f 6e61  am pad_: optiona
+00000610: 6c6c 7920 696e 6372 6561 7365 2076 6965  lly increase vie
+00000620: 7742 6f78 2062 7920 7061 6420 696e 2061  wBox by pad in a
+00000630: 6c6c 2064 6972 6563 7469 6f6e 730d 0a20  ll directions.. 
+00000640: 2020 203a 7061 7261 6d20 6470 755f 3a20     :param dpu_: 
+00000650: 6f70 7469 6f6e 616c 6c79 2073 6361 6c65  optionally scale
+00000660: 2069 6d61 6765 2028 7069 7865 6c73 2070   image (pixels p
+00000670: 6572 2075 6e69 7420 6f66 2062 6f75 6e64  er unit of bound
+00000680: 696e 6720 626f 7829 0d0a 2020 2020 3a70  ing box)..    :p
+00000690: 6172 616d 206e 736d 6170 3a20 6f70 7469  aram nsmap: opti
+000006a0: 6f6e 616c 6c79 2070 6173 7320 6120 6e61  onally pass a na
+000006b0: 6d65 7370 6163 6520 6d61 7020 6f66 2079  mespace map of y
+000006c0: 6f75 7220 6368 6f6f 7369 6e67 0d0a 2020  our choosing..  
+000006d0: 2020 3a70 6172 616d 2061 7474 7269 6275    :param attribu
+000006e0: 7465 733a 2065 6c65 6d65 6e74 2061 7474  tes: element att
+000006f0: 7269 6275 7465 206e 616d 6573 2061 6e64  ribute names and
+00000700: 2076 616c 7565 730d 0a20 2020 203a 7265   values..    :re
+00000710: 7475 726e 3a20 726f 6f74 2073 7667 2065  turn: root svg e
+00000720: 6c65 6d65 6e74 0d0a 0d0a 2020 2020 416c  lement....    Al
+00000730: 6c20 7669 6577 426f 782d 7374 796c 6520  l viewBox-style 
+00000740: 2874 7261 696c 696e 6720 756e 6465 7273  (trailing unders
+00000750: 636f 7265 2920 7061 7261 6d65 7465 7273  core) parameters
+00000760: 2061 7265 206f 7074 696f 6e61 6c2e 2041   are optional. A
+00000770: 6e79 206b 7761 7267 7320 7769 6c6c 0d0a  ny kwargs will..
+00000780: 2020 2020 6265 2070 6173 7365 6420 746f      be passed to
+00000790: 2060 6065 7472 6565 2e45 6c65 6d65 6e74   ``etree.Element
+000007a0: 6060 2061 7320 656c 656d 656e 7420 7061  `` as element pa
+000007b0: 7261 6d65 7465 7273 2e0d 0a20 2020 2022  rameters...    "
+000007c0: 2222 0d0a 2020 2020 6966 206e 736d 6170  ""..    if nsmap
+000007d0: 2069 7320 4e6f 6e65 3a0d 0a20 2020 2020   is None:..     
+000007e0: 2020 206e 736d 6170 203d 204e 534d 4150     nsmap = NSMAP
+000007f0: 0d0a 2020 2020 6966 204e 6f6e 6520 6e6f  ..    if None no
+00000800: 7420 696e 2028 785f 2c20 795f 2c20 7769  t in (x_, y_, wi
+00000810: 6474 685f 2c20 6865 6967 6874 5f29 3a0d  dth_, height_):.
+00000820: 0a20 2020 2020 2020 2061 7373 6572 7420  .        assert 
+00000830: 785f 2069 7320 6e6f 7420 4e6f 6e65 0d0a  x_ is not None..
+00000840: 2020 2020 2020 2020 6173 7365 7274 2079          assert y
+00000850: 5f20 6973 206e 6f74 204e 6f6e 650d 0a20  _ is not None.. 
+00000860: 2020 2020 2020 2061 7373 6572 7420 7769         assert wi
+00000870: 6474 685f 2069 7320 6e6f 7420 4e6f 6e65  dth_ is not None
+00000880: 0d0a 2020 2020 2020 2020 6173 7365 7274  ..        assert
+00000890: 2068 6569 6768 745f 2069 7320 6e6f 7420   height_ is not 
+000008a0: 4e6f 6e65 0d0a 2020 2020 2020 2020 7669  None..        vi
+000008b0: 6577 5f62 6f78 203d 2067 6574 5f76 6965  ew_box = get_vie
+000008c0: 7742 6f78 5f73 7472 2878 5f2c 2079 5f2c  wBox_str(x_, y_,
+000008d0: 2077 6964 7468 5f2c 2068 6569 6768 745f   width_, height_
+000008e0: 2c20 7061 645f 290d 0a20 2020 2020 2020  , pad_)..       
+000008f0: 2070 6978 656c 5f77 6964 7468 203d 2066   pixel_width = f
+00000900: 6f72 6d61 745f 6e75 6d62 6572 2828 7769  ormat_number((wi
+00000910: 6474 685f 202b 2070 6164 5f20 2a20 3229  dth_ + pad_ * 2)
+00000920: 202a 2064 7075 5f29 0d0a 2020 2020 2020   * dpu_)..      
+00000930: 2020 7069 7865 6c5f 6865 6967 6874 203d    pixel_height =
+00000940: 2066 6f72 6d61 745f 6e75 6d62 6572 2828   format_number((
+00000950: 6865 6967 6874 5f20 2b20 7061 645f 202a  height_ + pad_ *
+00000960: 2032 2920 2a20 6470 755f 290d 0a20 2020   2) * dpu_)..   
+00000970: 2020 2020 2061 7474 7269 6275 7465 735b       attributes[
+00000980: 2276 6965 7742 6f78 225d 203d 2061 7474  "viewBox"] = att
+00000990: 7269 6275 7465 732e 6765 7428 2276 6965  ributes.get("vie
+000009a0: 7742 6f78 222c 2076 6965 775f 626f 7829  wBox", view_box)
+000009b0: 0d0a 2020 2020 2020 2020 6174 7472 6962  ..        attrib
+000009c0: 7574 6573 5b22 7769 6474 6822 5d20 3d20  utes["width"] = 
+000009d0: 6174 7472 6962 7574 6573 2e67 6574 2822  attributes.get("
+000009e0: 7769 6474 6822 2c20 7069 7865 6c5f 7769  width", pixel_wi
+000009f0: 6474 6829 0d0a 2020 2020 2020 2020 6174  dth)..        at
+00000a00: 7472 6962 7574 6573 5b22 6865 6967 6874  tributes["height
+00000a10: 225d 203d 2061 7474 7269 6275 7465 732e  "] = attributes.
+00000a20: 6765 7428 2268 6569 6768 7422 2c20 7069  get("height", pi
+00000a30: 7865 6c5f 6865 6967 6874 290d 0a20 2020  xel_height)..   
+00000a40: 2023 2063 616e 206f 6e6c 7920 7061 7373   # can only pass
+00000a50: 206e 736d 6170 206f 6e20 696e 7374 616e   nsmap on instan
+00000a60: 6365 2063 7265 6174 696f 6e0d 0a20 2020  ce creation..   
+00000a70: 2073 7667 5f72 6f6f 7420 3d20 6574 7265   svg_root = etre
+00000a80: 652e 456c 656d 656e 7428 6622 7b7b 7b6e  e.Element(f"{{{n
+00000a90: 736d 6170 5b4e 6f6e 655d 7d7d 7d73 7667  smap[None]}}}svg
+00000aa0: 222c 206e 736d 6170 3d6e 736d 6170 290d  ", nsmap=nsmap).
+00000ab0: 0a20 2020 2072 6574 7572 6e20 7570 6461  .    return upda
+00000ac0: 7465 5f65 6c65 6d65 6e74 2873 7667 5f72  te_element(svg_r
+00000ad0: 6f6f 742c 202a 2a61 7474 7269 6275 7465  oot, **attribute
+00000ae0: 7329 0d0a 0d0a 0d0a 6465 6620 7772 6974  s)......def writ
+00000af0: 655f 7376 6728 0d0a 2020 2020 7376 673a  e_svg(..    svg:
+00000b00: 2050 6174 6820 7c20 7374 7220 7c20 494f   Path | str | IO
+00000b10: 5b62 7974 6573 5d2c 0d0a 2020 2020 786d  [bytes],..    xm
+00000b20: 6c3a 205f 456c 656d 656e 742c 0d0a 2020  l: _Element,..  
+00000b30: 2020 7374 796c 6573 6865 6574 3a20 4f70    stylesheet: Op
+00000b40: 7469 6f6e 616c 5b73 7472 5d20 3d20 4e6f  tional[str] = No
+00000b50: 6e65 2c0d 0a20 2020 2064 6f5f 6c69 6e6b  ne,..    do_link
+00000b60: 5f63 7373 3a20 626f 6f6c 203d 2046 616c  _css: bool = Fal
+00000b70: 7365 2c0d 0a20 2020 202a 2a74 6f73 7472  se,..    **tostr
+00000b80: 696e 675f 6b77 6172 6773 3a20 7374 7220  ing_kwargs: str 
+00000b90: 7c20 626f 6f6c 2c0d 0a29 202d 3e20 7374  | bool,..) -> st
+00000ba0: 723a 0d0a 2020 2020 2222 220d 0a20 2020  r:..    """..   
+00000bb0: 2057 7269 7465 2061 6e20 786d 6c20 656c   Write an xml el
+00000bc0: 656d 656e 7420 6173 2061 6e20 7376 6720  ement as an svg 
+00000bd0: 6669 6c65 2e0d 0a0d 0a20 2020 203a 7061  file.....    :pa
+00000be0: 7261 6d20 7376 673a 206f 7065 6e20 6269  ram svg: open bi
+00000bf0: 6e61 7279 2066 696c 6520 6f62 6a65 6374  nary file object
+00000c00: 206f 7220 7061 7468 2074 6f20 6f75 7470   or path to outp
+00000c10: 7574 2066 696c 6520 2869 6e63 6c75 6465  ut file (include
+00000c20: 2065 7874 656e 7369 6f6e 202e 7376 6729   extension .svg)
+00000c30: 0d0a 2020 2020 3a70 6172 616d 2078 6d6c  ..    :param xml
+00000c40: 3a20 726f 6f74 206e 6f64 6520 6f66 2079  : root node of y
+00000c50: 6f75 7220 7376 6720 6765 6f6d 6574 7279  our svg geometry
+00000c60: 0d0a 2020 2020 3a70 6172 616d 2073 7479  ..    :param sty
+00000c70: 6c65 7368 6565 743a 206f 7074 696f 6e61  lesheet: optiona
+00000c80: 6c20 7061 7468 2074 6f20 6373 7320 7374  l path to css st
+00000c90: 796c 6573 6865 6574 0d0a 2020 2020 3a70  ylesheet..    :p
+00000ca0: 6172 616d 2064 6f5f 6c69 6e6b 5f63 7373  aram do_link_css
+00000cb0: 3a20 6c69 6e6b 2074 6f20 7374 796c 6573  : link to styles
+00000cc0: 6865 6574 2c20 656c 7365 2028 6465 6661  heet, else (defa
+00000cd0: 756c 7429 2077 7269 7465 2063 6f6e 7465  ult) write conte
+00000ce0: 6e74 7320 6f66 2073 7479 6c65 7368 6565  nts of styleshee
+00000cf0: 740d 0a20 2020 2020 2020 2069 6e74 6f20  t..        into 
+00000d00: 7376 6720 2869 676e 6f72 6564 2069 6620  svg (ignored if 
+00000d10: 7374 796c 6573 6865 6574 2069 7320 4e6f  stylesheet is No
+00000d20: 6e65 290d 0a20 2020 203a 7061 7261 6d20  ne)..    :param 
+00000d30: 746f 7374 7269 6e67 5f6b 7761 7267 733a  tostring_kwargs:
+00000d40: 206b 6579 776f 7264 2061 7267 756d 656e   keyword argumen
+00000d50: 7473 2074 6f20 6574 7265 652e 746f 7374  ts to etree.tost
+00000d60: 7269 6e67 2e20 786d 6c5f 6865 6164 6572  ring. xml_header
+00000d70: 3d54 7275 6520 666f 720d 0a20 2020 2020  =True for..     
+00000d80: 2020 2073 656e 7369 626c 6520 6465 6661     sensible defa
+00000d90: 756c 7420 7661 6c75 6573 2e20 5365 6520  ult values. See 
+00000da0: 6265 6c6f 772e 0d0a 2020 2020 3a72 6574  below...    :ret
+00000db0: 7572 6e3a 2073 7667 2066 696c 656e 616d  urn: svg filenam
+00000dc0: 650d 0a20 2020 203a 6566 6665 6374 733a  e..    :effects:
+00000dd0: 2063 7265 6174 6573 2073 7667 2066 696c   creates svg fil
+00000de0: 6520 6174 2060 6073 7667 6060 0d0a 0d0a  e at ``svg``....
+00000df0: 2020 2020 4974 2773 206f 6674 656e 2075      It's often u
+00000e00: 7365 6675 6c20 746f 2077 7269 7465 2061  seful to write a
+00000e10: 2074 656d 706f 7261 7279 2073 7667 2066   temporary svg f
+00000e20: 696c 652c 2073 6f20 6120 7465 6d70 6669  ile, so a tempfi
+00000e30: 6c65 2e4e 616d 6564 5465 6d70 6f72 6172  le.NamedTemporar
+00000e40: 7946 696c 650d 0a20 2020 206f 626a 6563  yFile..    objec
+00000e50: 7420 286f 7220 616e 7920 6f70 656e 2062  t (or any open b
+00000e60: 696e 6172 7920 6669 6c65 206f 626a 6563  inary file objec
+00000e70: 7420 6361 6e20 6265 2070 6173 7365 6420  t can be passed 
+00000e80: 696e 7374 6561 6420 6f66 2061 6e20 7376  instead of an sv
+00000e90: 6720 6669 6c65 6e61 6d65 292e 0d0a 0d0a  g filename).....
+00000ea0: 2020 2020 596f 7520 6d61 7920 6e65 7665      You may neve
+00000eb0: 7220 6e65 6564 2061 6e20 786d 6c5f 6865  r need an xml_he
+00000ec0: 6164 6572 2e20 496e 6b73 6361 7065 2064  ader. Inkscape d
+00000ed0: 6f65 736e 2774 206e 6565 6420 6974 2c20  oesn't need it, 
+00000ee0: 796f 7572 2062 726f 7773 6572 2064 6f65  your browser doe
+00000ef0: 736e 2774 0d0a 2020 2020 6e65 6564 2069  sn't..    need i
+00000f00: 742c 2061 6e64 2069 7427 7320 666f 7262  t, and it's forb
+00000f10: 6964 6465 6e20 6966 2079 6f75 2764 206c  idden if you'd l
+00000f20: 696b 6520 746f 2022 696e 6c69 6e65 2220  ike to "inline" 
+00000f30: 796f 7572 2073 7667 2069 6e20 616e 2068  your svg in an h
+00000f40: 746d 6c20 6669 6c65 2e0d 0a20 2020 2054  tml file...    T
+00000f50: 6865 206d 6f73 7420 7072 6573 7369 6e67  he most pressing
+00000f60: 206e 6565 6420 6d69 6768 7420 6265 2074   need might be t
+00000f70: 6f20 7365 7420 616e 2065 6e63 6f64 696e  o set an encodin
+00000f80: 672e 2049 6620 796f 7520 7061 7373 0d0a  g. If you pass..
+00000f90: 2020 2020 6060 786d 6c5f 6465 636c 6172      ``xml_declar
+00000fa0: 6174 696f 6e3d 5472 7565 6060 2061 7320  ation=True`` as 
+00000fb0: 6120 746f 7374 7269 6e67 5f6b 7761 7267  a tostring_kwarg
+00000fc0: 2c20 7468 6973 2066 756e 6374 696f 6e20  , this function 
+00000fd0: 7769 6c6c 2061 7474 656d 7074 2074 6f20  will attempt to 
+00000fe0: 7061 7373 0d0a 2020 2020 7468 6520 666f  pass..    the fo
+00000ff0: 6c6c 6f77 696e 6720 6465 6661 756c 7473  llowing defaults
+00001000: 2074 6f20 6060 6c78 6d6c 2e65 7472 6565   to ``lxml.etree
+00001010: 2e74 6f73 7472 696e 6760 603a 0d0a 0d0a  .tostring``:....
+00001020: 2020 2020 2a20 646f 6374 7970 653a 2073      * doctype: s
+00001030: 7472 203d 2028 0d0a 2020 2020 2020 2020  tr = (..        
+00001040: 273c 2144 4f43 5459 5045 2073 7667 2050  '<!DOCTYPE svg P
+00001050: 5542 4c49 4320 222d 2f2f 5733 432f 2f44  UBLIC "-//W3C//D
+00001060: 5444 2053 5647 2031 2e31 2f2f 454e 225c  TD SVG 1.1//EN"\
+00001070: 6e27 0d0a 2020 2020 2020 2020 2722 6874  n'..        '"ht
+00001080: 7470 3a2f 2f77 7777 2e77 332e 6f72 672f  tp://www.w3.org/
+00001090: 4772 6170 6869 6373 2f53 5647 2f31 2e31  Graphics/SVG/1.1
+000010a0: 2f44 5444 2f73 7667 3131 2e64 7464 223e  /DTD/svg11.dtd">
+000010b0: 270d 0a20 2020 2029 0d0a 2020 2020 2a20  '..    )..    * 
+000010c0: 656e 636f 6469 6e67 203d 2022 5554 462d  encoding = "UTF-
+000010d0: 3822 0d0a 0d0a 2020 2020 416c 7761 7973  8"....    Always
+000010e0: 2c20 7468 6973 2066 756e 6374 696f 6e20  , this function 
+000010f0: 7769 6c6c 2064 6566 6175 6c74 2074 6f20  will default to 
+00001100: 6060 7072 6574 7479 5f70 7269 6e74 3d54  ``pretty_print=T
+00001110: 7275 6560 600d 0a0d 0a20 2020 2054 6865  rue``....    The
+00001120: 7365 2063 616e 2062 6520 6f76 6572 7269  se can be overri
+00001130: 6464 656e 2062 7920 746f 7374 7269 6e67  dden by tostring
+00001140: 5f6b 7761 7267 732e 0d0a 0d0a 2020 2020  _kwargs.....    
+00001150: 652e 672e 2c20 6060 7772 6974 655f 7376  e.g., ``write_sv
+00001160: 6728 2e2e 2e2c 2078 6d6c 5f64 6563 6c61  g(..., xml_decla
+00001170: 7261 7469 6f6e 3d54 7275 652c 2064 6f63  ration=True, doc
+00001180: 7479 7065 3d4e 6f6e 6560 6029 0d0a 2020  type=None``)..  
+00001190: 2020 652e 672e 2c20 6060 7772 6974 655f    e.g., ``write_
+000011a0: 7376 6728 2e2e 2e2c 2078 6d6c 5f64 6563  svg(..., xml_dec
+000011b0: 6c61 7261 7469 6f6e 3d54 7275 652c 2065  laration=True, e
+000011c0: 6e63 6f64 696e 673d 2761 7363 6969 2729  ncoding='ascii')
+000011d0: 6060 0d0a 0d0a 2020 2020 6060 6c78 6d6c  ``....    ``lxml
+000011e0: 2e65 7472 6565 2e74 6f73 7472 696e 6760  .etree.tostring`
+000011f0: 6020 6973 2064 6f63 756d 656e 7465 6420  ` is documented 
+00001200: 6865 7265 3a20 6874 7470 733a 2f2f 6c78  here: https://lx
+00001210: 6d6c 2e64 652f 6170 692f 696e 6465 782e  ml.de/api/index.
+00001220: 6874 6d6c 2c0d 0a20 2020 2062 7574 2049  html,..    but I
+00001230: 206b 6e6f 7720 7468 6174 2074 6f20 6265   know that to be
+00001240: 2069 6e63 6f6d 706c 6574 6520 6173 206f   incomplete as o
+00001250: 6620 3230 3230 2046 6562 2030 312c 2061  f 2020 Feb 01, a
+00001260: 7320 6974 2064 6f65 7320 6e6f 7420 646f  s it does not do
+00001270: 6375 6d65 6e74 2074 6865 0d0a 2020 2020  cument the..    
+00001280: 2870 6572 6861 7073 2069 6d70 6f72 7461  (perhaps importa
+00001290: 6e74 2074 6f20 796f 7529 2027 656e 636f  nt to you) 'enco
+000012a0: 6469 6e67 2720 6b77 6172 672e 0d0a 2020  ding' kwarg...  
+000012b0: 2020 2222 220d 0a20 2020 2069 6620 7374    """..    if st
+000012c0: 796c 6573 6865 6574 2069 7320 6e6f 7420  ylesheet is not 
+000012d0: 4e6f 6e65 3a0d 0a20 2020 2020 2020 2069  None:..        i
+000012e0: 6620 646f 5f6c 696e 6b5f 6373 7320 6973  f do_link_css is
+000012f0: 2054 7275 653a 0d0a 2020 2020 2020 2020   True:..        
+00001300: 2020 2020 7061 7265 6e74 203d 2050 6174      parent = Pat
+00001310: 6828 7374 7228 7376 6729 292e 7061 7265  h(str(svg)).pare
+00001320: 6e74 0d0a 2020 2020 2020 2020 2020 2020  nt..            
+00001330: 7265 6c61 7469 7665 5f63 7373 5f70 6174  relative_css_pat
+00001340: 6820 3d20 5061 7468 2873 7479 6c65 7368  h = Path(stylesh
+00001350: 6565 7429 2e72 656c 6174 6976 655f 746f  eet).relative_to
+00001360: 2870 6172 656e 7429 0d0a 2020 2020 2020  (parent)..      
+00001370: 2020 2020 2020 6c69 6e6b 203d 2065 7472        link = etr
+00001380: 6565 2e50 4928 0d0a 2020 2020 2020 2020  ee.PI(..        
+00001390: 2020 2020 2020 2020 2278 6d6c 2d73 7479          "xml-sty
+000013a0: 6c65 7368 6565 7422 2c20 6627 6872 6566  lesheet", f'href
+000013b0: 3d22 7b72 656c 6174 6976 655f 6373 735f  ="{relative_css_
+000013c0: 7061 7468 7d22 2074 7970 653d 2274 6578  path}" type="tex
+000013d0: 742f 6373 7322 270d 0a20 2020 2020 2020  t/css"'..       
+000013e0: 2020 2020 2029 0d0a 2020 2020 2020 2020       )..        
+000013f0: 2020 2020 786d 6c2e 6164 6470 7265 7669      xml.addprevi
+00001400: 6f75 7328 6c69 6e6b 290d 0a20 2020 2020  ous(link)..     
+00001410: 2020 2065 6c73 653a 0d0a 2020 2020 2020     else:..      
+00001420: 2020 2020 2020 7374 796c 6520 3d20 6574        style = et
+00001430: 7265 652e 456c 656d 656e 7428 2273 7479  ree.Element("sty
+00001440: 6c65 222c 2074 7970 653d 2274 6578 742f  le", type="text/
+00001450: 6373 7322 290d 0a20 2020 2020 2020 2020  css")..         
+00001460: 2020 2077 6974 6820 6f70 656e 2873 7479     with open(sty
+00001470: 6c65 7368 6565 7429 2061 7320 6373 735f  lesheet) as css_
+00001480: 6669 6c65 3a0d 0a20 2020 2020 2020 2020  file:..         
+00001490: 2020 2020 2020 2073 7479 6c65 2e74 6578         style.tex
+000014a0: 7420 3d20 6574 7265 652e 4344 4154 4128  t = etree.CDATA(
+000014b0: 225c 6e22 202b 2022 222e 6a6f 696e 2863  "\n" + "".join(c
+000014c0: 7373 5f66 696c 652e 7265 6164 6c69 6e65  ss_file.readline
+000014d0: 7328 2929 202b 2022 5c6e 2229 0d0a 2020  s()) + "\n")..  
+000014e0: 2020 2020 2020 2020 2020 786d 6c2e 696e            xml.in
+000014f0: 7365 7274 2830 2c20 7374 796c 6529 0d0a  sert(0, style)..
+00001500: 0d0a 2020 2020 7376 675f 636f 6e74 656e  ..    svg_conten
+00001510: 7473 203d 2073 7667 5f74 6f73 7472 696e  ts = svg_tostrin
+00001520: 6728 786d 6c2c 202a 2a74 6f73 7472 696e  g(xml, **tostrin
+00001530: 675f 6b77 6172 6773 290d 0a0d 0a20 2020  g_kwargs)....   
+00001540: 2074 7279 3a0d 0a20 2020 2020 2020 2073   try:..        s
+00001550: 7667 5f66 696c 6520 3d20 6361 7374 2849  vg_file = cast(I
+00001560: 4f5b 6279 7465 735d 2c20 7376 6729 0d0a  O[bytes], svg)..
+00001570: 2020 2020 2020 2020 5f20 3d20 7376 675f          _ = svg_
+00001580: 6669 6c65 2e77 7269 7465 2873 7667 5f63  file.write(svg_c
+00001590: 6f6e 7465 6e74 7329 0d0a 2020 2020 2020  ontents)..      
+000015a0: 2020 7265 7475 726e 2073 7667 5f66 696c    return svg_fil
+000015b0: 652e 6e61 6d65 0d0a 2020 2020 6578 6365  e.name..    exce
+000015c0: 7074 2041 7474 7269 6275 7465 4572 726f  pt AttributeErro
+000015d0: 723a 0d0a 2020 2020 2020 2020 7376 675f  r:..        svg_
+000015e0: 6669 6c65 6e61 6d65 203d 2063 6173 7428  filename = cast(
+000015f0: 7374 722c 2073 7667 290d 0a20 2020 2020  str, svg)..     
+00001600: 2020 2077 6974 6820 6f70 656e 2873 7667     with open(svg
+00001610: 5f66 696c 656e 616d 652c 2022 7762 2229  _filename, "wb")
+00001620: 2061 7320 7376 675f 6669 6c65 3a0d 0a20   as svg_file:.. 
+00001630: 2020 2020 2020 2020 2020 205f 203d 2073             _ = s
+00001640: 7667 5f66 696c 652e 7772 6974 6528 7376  vg_file.write(sv
+00001650: 675f 636f 6e74 656e 7473 290d 0a20 2020  g_contents)..   
+00001660: 2020 2020 2072 6574 7572 6e20 7376 675f       return svg_
+00001670: 6669 6c65 6e61 6d65 0d0a 0d0a 0d0a 6465  filename......de
+00001680: 6620 7772 6974 655f 706e 675f 6672 6f6d  f write_png_from
+00001690: 5f73 7667 2869 6e6b 7363 6170 653a 2073  _svg(inkscape: s
+000016a0: 7472 2c20 7376 673a 2073 7472 2c20 706e  tr, svg: str, pn
+000016b0: 673a 204f 7074 696f 6e61 6c5b 7374 725d  g: Optional[str]
+000016c0: 203d 204e 6f6e 6529 202d 3e20 7374 723a   = None) -> str:
+000016d0: 0d0a 2020 2020 2222 220d 0a20 2020 2043  ..    """..    C
+000016e0: 6f6e 7665 7274 2061 6e20 7376 6720 6669  onvert an svg fi
+000016f0: 6c65 2074 6f20 6120 706e 670d 0a0d 0a20  le to a png.... 
+00001700: 2020 203a 7061 7261 6d20 696e 6b73 6361     :param inksca
+00001710: 7065 3a20 7061 7468 2074 6f20 696e 6b73  pe: path to inks
+00001720: 6361 7065 2065 7865 6375 7461 626c 6520  cape executable 
+00001730: 2877 6974 686f 7574 202e 6578 6520 6578  (without .exe ex
+00001740: 7465 6e73 696f 6e21 290d 0a20 2020 203a  tension!)..    :
+00001750: 7061 7261 6d20 7376 673a 2070 6174 6820  param svg: path 
+00001760: 746f 2073 7667 2066 696c 650d 0a20 2020  to svg file..   
+00001770: 203a 7061 7261 6d20 706e 673a 206f 7074   :param png: opt
+00001780: 696f 6e61 6c20 7061 7468 2074 6f20 706e  ional path to pn
+00001790: 6720 6f75 7470 7574 2066 696c 650d 0a20  g output file.. 
+000017a0: 2020 203a 7265 7475 726e 3a20 706e 6720     :return: png 
+000017b0: 6669 6c65 6e61 6d65 0d0a 2020 2020 3a65  filename..    :e
+000017c0: 6666 6563 7473 3a20 6372 6561 7465 7320  ffects: creates 
+000017d0: 6120 6e65 7720 706e 6720 6672 6f6d 2073  a new png from s
+000017e0: 7667 2066 696c 656e 616d 650d 0a0d 0a20  vg filename.... 
+000017f0: 2020 2049 6620 6e6f 206f 7574 7075 7420     If no output 
+00001800: 706e 6720 7061 7468 2069 7320 6769 7665  png path is give
+00001810: 6e2c 2074 6865 206f 7574 7075 7420 7061  n, the output pa
+00001820: 7468 2077 696c 6c20 6265 2069 6e66 6572  th will be infer
+00001830: 7265 6420 6672 6f6d 2074 6865 2060 6073  red from the ``s
+00001840: 7667 6060 0d0a 2020 2020 6669 6c65 6e61  vg``..    filena
+00001850: 6d65 2e0d 0a20 2020 2022 2222 0d0a 2020  me...    """..  
+00001860: 2020 6966 2070 6e67 2069 7320 4e6f 6e65    if png is None
+00001870: 3a0d 0a20 2020 2020 2020 2070 6e67 203d  :..        png =
+00001880: 2073 7472 2850 6174 6828 7376 6729 2e77   str(Path(svg).w
+00001890: 6974 685f 7375 6666 6978 2822 2e70 6e67  ith_suffix(".png
+000018a0: 2229 290d 0a0d 0a20 2020 2023 2069 6e6b  "))....    # ink
+000018b0: 7363 6170 6520 7665 7273 696f 6e73 203e  scape versions >
+000018c0: 3d20 312e 300d 0a20 2020 206f 7074 696f  = 1.0..    optio
+000018d0: 6e73 203d 205b 6627 227b 7376 677d 2227  ns = [f'"{svg}"'
+000018e0: 2c20 222d 2d65 7870 6f72 742d 7479 7065  , "--export-type
+000018f0: 3d70 6e67 222c 2066 272d 2d65 7870 6f72  =png", f'--expor
+00001900: 742d 6669 6c65 6e61 6d65 3d22 7b70 6e67  t-filename="{png
+00001910: 7d22 275d 0d0a 2020 2020 7265 7475 726e  }"']..    return
+00001920: 5f63 6f64 6520 3d20 7375 6270 726f 6365  _code = subproce
+00001930: 7373 2e63 616c 6c28 6627 227b 696e 6b73  ss.call(f'"{inks
+00001940: 6361 7065 7d22 2027 202b 2022 2022 2e6a  cape}" ' + " ".j
+00001950: 6f69 6e28 6f70 7469 6f6e 7329 290d 0a20  oin(options)).. 
+00001960: 2020 2069 6620 7265 7475 726e 5f63 6f64     if return_cod
+00001970: 6520 3d3d 2030 3a0d 0a20 2020 2020 2020  e == 0:..       
+00001980: 2072 6574 7572 6e20 706e 670d 0a0d 0a20   return png.... 
+00001990: 2020 2023 2069 6e6b 7363 6170 6520 7665     # inkscape ve
+000019a0: 7273 696f 6e73 203c 2031 2e30 0d0a 2020  rsions < 1.0..  
+000019b0: 2020 7265 7475 726e 5f63 6f64 6520 3d20    return_code = 
+000019c0: 7375 6270 726f 6365 7373 2e63 616c 6c28  subprocess.call(
+000019d0: 6627 227b 696e 6b73 6361 7065 7d22 202d  f'"{inkscape}" -
+000019e0: 6620 227b 7376 677d 2220 2d65 2022 7b70  f "{svg}" -e "{p
+000019f0: 6e67 7d22 2729 0d0a 2020 2020 6966 2072  ng}"')..    if r
+00001a00: 6574 7572 6e5f 636f 6465 203d 3d20 303a  eturn_code == 0:
+00001a10: 0d0a 2020 2020 2020 2020 7265 7475 726e  ..        return
+00001a20: 2070 6e67 0d0a 0d0a 2020 2020 7261 6973   png....    rais
+00001a30: 6520 5661 6c75 6545 7272 6f72 2866 2266  e ValueError(f"f
+00001a40: 6169 6c65 6420 746f 2077 7269 7465 207b  ailed to write {
+00001a50: 706e 677d 2229 0d0a 0d0a 0d0a 6465 6620  png}")......def 
+00001a60: 7772 6974 655f 706e 6728 0d0a 2020 2020  write_png(..    
+00001a70: 696e 6b73 6361 7065 3a20 7374 722c 0d0a  inkscape: str,..
+00001a80: 2020 2020 706e 673a 2073 7472 2c0d 0a20      png: str,.. 
+00001a90: 2020 2078 6d6c 3a20 5f45 6c65 6d65 6e74     xml: _Element
+00001aa0: 2c0d 0a20 2020 2073 7479 6c65 7368 6565  ,..    styleshee
+00001ab0: 743a 204f 7074 696f 6e61 6c5b 7374 725d  t: Optional[str]
+00001ac0: 203d 204e 6f6e 652c 0d0a 2920 2d3e 2073   = None,..) -> s
+00001ad0: 7472 3a0d 0a20 2020 2022 2222 0d0a 2020  tr:..    """..  
+00001ae0: 2020 4372 6561 7465 2061 2070 6e67 2066    Create a png f
+00001af0: 696c 6520 7769 7468 6f75 7420 7772 6974  ile without writ
+00001b00: 696e 6720 616e 2069 6e74 6572 6d65 6469  ing an intermedi
+00001b10: 6174 6520 7376 6720 6669 6c65 2e0d 0a0d  ate svg file....
+00001b20: 0a20 2020 203a 7061 7261 6d20 696e 6b73  .    :param inks
+00001b30: 6361 7065 3a20 7061 7468 2074 6f20 696e  cape: path to in
+00001b40: 6b73 6361 7065 2065 7865 6375 7461 626c  kscape executabl
+00001b50: 6520 2877 6974 686f 7574 202e 6578 6520  e (without .exe 
+00001b60: 6578 7465 6e73 696f 6e21 290d 0a20 2020  extension!)..   
+00001b70: 203a 7061 7261 6d20 706e 673a 2070 6174   :param png: pat
+00001b80: 6820 746f 206f 7574 7075 7420 706e 6720  h to output png 
+00001b90: 6669 6c65 0d0a 2020 2020 3a70 6172 616d  file..    :param
+00001ba0: 2078 6d6c 3a20 726f 6f74 206e 6f64 6520   xml: root node 
+00001bb0: 6f66 2079 6f75 7220 7376 6720 6765 6f6d  of your svg geom
+00001bc0: 6574 7279 0d0a 2020 2020 3a70 6172 616d  etry..    :param
+00001bd0: 2073 7479 6c65 7368 6565 743a 206f 7074   stylesheet: opt
+00001be0: 696f 6e61 6c20 7061 7468 2074 6f20 6373  ional path to cs
+00001bf0: 7320 7374 796c 6573 6865 6574 0d0a 2020  s stylesheet..  
+00001c00: 2020 3a72 6574 7572 6e3a 2070 6e67 2066    :return: png f
+00001c10: 696c 656e 616d 6520 2874 6865 2073 616d  ilename (the sam
+00001c20: 6520 796f 7520 696e 7075 7420 6173 2060  e you input as `
+00001c30: 6070 6e67 6060 290d 0a20 2020 203a 6566  `png``)..    :ef
+00001c40: 6665 6374 733a 2063 7265 6174 6573 2061  fects: creates a
+00001c50: 206e 6577 2070 6e67 2066 696c 650d 0a0d   new png file...
+00001c60: 0a20 2020 2054 6869 7320 6a75 7374 2063  .    This just c
+00001c70: 7265 6174 6573 2061 2074 656d 7066 696c  reates a tempfil
+00001c80: 652c 2077 7269 7465 7320 7468 6520 7376  e, writes the sv
+00001c90: 6720 746f 2074 6865 2074 656d 7066 696c  g to the tempfil
+00001ca0: 652c 2074 6865 6e20 6361 6c6c 730d 0a20  e, then calls.. 
+00001cb0: 2020 2060 6077 7269 7465 5f70 6e67 5f66     ``write_png_f
+00001cc0: 726f 6d5f 7376 6760 6020 7769 7468 2074  rom_svg`` with t
+00001cd0: 6865 2074 656d 7066 696c 652e 2054 6869  he tempfile. Thi
+00001ce0: 7320 6973 6e27 7420 6661 7374 6572 2028  s isn't faster (
+00001cf0: 6974 206d 6967 6874 2062 6520 736c 6967  it might be slig
+00001d00: 6874 6c79 0d0a 2020 2020 736c 6f77 6572  htly..    slower
+00001d10: 292c 2062 7574 2069 7420 6b65 6570 7320  ), but it keeps 
+00001d20: 7468 6520 6669 6c65 7379 7374 656d 2063  the filesystem c
+00001d30: 6c65 616e 2077 6865 6e20 796f 7520 6f6e  lean when you on
+00001d40: 6c79 2077 616e 7420 7468 6520 706e 672e  ly want the png.
+00001d50: 0d0a 2020 2020 2222 220d 0a20 2020 2077  ..    """..    w
+00001d60: 6974 6820 4e61 6d65 6454 656d 706f 7261  ith NamedTempora
+00001d70: 7279 4669 6c65 286d 6f64 653d 2277 6222  ryFile(mode="wb"
+00001d80: 2c20 6465 6c65 7465 3d46 616c 7365 2920  , delete=False) 
+00001d90: 6173 2073 7667 5f66 696c 653a 0d0a 2020  as svg_file:..  
+00001da0: 2020 2020 2020 7376 6720 3d20 7772 6974        svg = writ
+00001db0: 655f 7376 6728 7376 675f 6669 6c65 2c20  e_svg(svg_file, 
+00001dc0: 786d 6c2c 2073 7479 6c65 7368 6565 7429  xml, stylesheet)
+00001dd0: 0d0a 2020 2020 5f20 3d20 7772 6974 655f  ..    _ = write_
+00001de0: 706e 675f 6672 6f6d 5f73 7667 2869 6e6b  png_from_svg(ink
+00001df0: 7363 6170 652c 2073 7667 2c20 706e 6729  scape, svg, png)
+00001e00: 0d0a 2020 2020 6f73 2e75 6e6c 696e 6b28  ..    os.unlink(
+00001e10: 7376 6729 0d0a 2020 2020 7265 7475 726e  svg)..    return
+00001e20: 2070 6e67 0d0a 0d0a 0d0a 6465 6620 7772   png......def wr
+00001e30: 6974 655f 7064 665f 6672 6f6d 5f73 7667  ite_pdf_from_svg
+00001e40: 2869 6e6b 7363 6170 653a 2073 7472 2c20  (inkscape: str, 
+00001e50: 7376 673a 2073 7472 2c20 7064 663a 204f  svg: str, pdf: O
+00001e60: 7074 696f 6e61 6c5b 7374 725d 203d 204e  ptional[str] = N
+00001e70: 6f6e 6529 202d 3e20 7374 723a 0d0a 2020  one) -> str:..  
+00001e80: 2020 2222 220d 0a20 2020 2043 6f6e 7665    """..    Conve
+00001e90: 7274 2061 6e20 7376 6720 6669 6c65 2074  rt an svg file t
+00001ea0: 6f20 6120 7064 660d 0a0d 0a20 2020 203a  o a pdf....    :
+00001eb0: 7061 7261 6d20 696e 6b73 6361 7065 3a20  param inkscape: 
+00001ec0: 7061 7468 2074 6f20 696e 6b73 6361 7065  path to inkscape
+00001ed0: 2065 7865 6375 7461 626c 6520 2877 6974   executable (wit
+00001ee0: 686f 7574 202e 6578 6520 6578 7465 6e73  hout .exe extens
+00001ef0: 696f 6e21 290d 0a20 2020 203a 7061 7261  ion!)..    :para
+00001f00: 6d20 7376 673a 2070 6174 6820 746f 2073  m svg: path to s
+00001f10: 7667 2066 696c 650d 0a20 2020 203a 7061  vg file..    :pa
+00001f20: 7261 6d20 7064 663a 206f 7074 696f 6e61  ram pdf: optiona
+00001f30: 6c20 7061 7468 2074 6f20 706e 6720 6f75  l path to png ou
+00001f40: 7470 7574 2066 696c 650d 0a20 2020 203a  tput file..    :
+00001f50: 7265 7475 726e 3a20 7064 6620 6669 6c65  return: pdf file
+00001f60: 6e61 6d65 0d0a 2020 2020 3a65 6666 6563  name..    :effec
+00001f70: 7473 3a20 6372 6561 7465 7320 6120 6e65  ts: creates a ne
+00001f80: 7720 7066 6420 6672 6f6d 2073 7667 2066  w pfd from svg f
+00001f90: 696c 656e 616d 650d 0a0d 0a20 2020 2049  ilename....    I
+00001fa0: 6620 6e6f 206f 7574 7075 7420 706e 6720  f no output png 
+00001fb0: 7061 7468 2069 7320 6769 7665 6e2c 2074  path is given, t
+00001fc0: 6865 206f 7574 7075 7420 7061 7468 2077  he output path w
+00001fd0: 696c 6c20 6265 2069 6e66 6572 7265 6420  ill be inferred 
+00001fe0: 6672 6f6d 2074 6865 2060 6073 7667 6060  from the ``svg``
+00001ff0: 0d0a 2020 2020 6669 6c65 6e61 6d65 2e0d  ..    filename..
+00002000: 0a20 2020 2022 2222 0d0a 2020 2020 6966  .    """..    if
+00002010: 2070 6466 2069 7320 4e6f 6e65 3a0d 0a20   pdf is None:.. 
+00002020: 2020 2020 2020 2070 6466 203d 2073 7472         pdf = str
+00002030: 2850 6174 6828 7376 6729 2e77 6974 685f  (Path(svg).with_
+00002040: 7375 6666 6978 2822 2e70 6466 2229 290d  suffix(".pdf")).
+00002050: 0a0d 0a20 2020 2023 2069 6e6b 7363 6170  ...    # inkscap
+00002060: 6520 7665 7273 696f 6e73 203e 3d20 312e  e versions >= 1.
+00002070: 300d 0a20 2020 206f 7074 696f 6e73 203d  0..    options =
+00002080: 205b 6627 227b 7376 677d 2227 2c20 222d   [f'"{svg}"', "-
+00002090: 2d65 7870 6f72 742d 7479 7065 3d70 6466  -export-type=pdf
+000020a0: 222c 2066 272d 2d65 7870 6f72 742d 6669  ", f'--export-fi
+000020b0: 6c65 6e61 6d65 3d22 7b70 6466 7d22 275d  lename="{pdf}"']
+000020c0: 0d0a 2020 2020 7265 7475 726e 5f63 6f64  ..    return_cod
+000020d0: 6520 3d20 7375 6270 726f 6365 7373 2e63  e = subprocess.c
+000020e0: 616c 6c28 6627 227b 696e 6b73 6361 7065  all(f'"{inkscape
+000020f0: 7d22 2027 202b 2022 2022 2e6a 6f69 6e28  }" ' + " ".join(
+00002100: 6f70 7469 6f6e 7329 290d 0a20 2020 2069  options))..    i
+00002110: 6620 7265 7475 726e 5f63 6f64 6520 3d3d  f return_code ==
+00002120: 2030 3a0d 0a20 2020 2020 2020 2072 6574   0:..        ret
+00002130: 7572 6e20 7064 660d 0a0d 0a20 2020 2023  urn pdf....    #
+00002140: 2069 6e6b 7363 6170 6520 7665 7273 696f   inkscape versio
+00002150: 6e73 203c 2031 2e30 0d0a 2020 2020 7265  ns < 1.0..    re
+00002160: 7475 726e 5f63 6f64 6520 3d20 7375 6270  turn_code = subp
+00002170: 726f 6365 7373 2e63 616c 6c28 6627 227b  rocess.call(f'"{
+00002180: 696e 6b73 6361 7065 7d22 202d 6620 227b  inkscape}" -f "{
+00002190: 7376 677d 2220 2d65 2022 7b70 6466 7d22  svg}" -e "{pdf}"
+000021a0: 2729 0d0a 2020 2020 6966 2072 6574 7572  ')..    if retur
+000021b0: 6e5f 636f 6465 203d 3d20 303a 0d0a 2020  n_code == 0:..  
+000021c0: 2020 2020 2020 7265 7475 726e 2070 6466        return pdf
+000021d0: 0d0a 0d0a 2020 2020 7261 6973 6520 5661  ....    raise Va
+000021e0: 6c75 6545 7272 6f72 2866 2266 6169 6c65  lueError(f"faile
+000021f0: 6420 746f 2077 7269 7465 207b 7064 667d  d to write {pdf}
+00002200: 2229 0d0a 0d0a 0d0a 6465 6620 7772 6974  ")......def writ
+00002210: 655f 7064 6628 0d0a 2020 2020 696e 6b73  e_pdf(..    inks
+00002220: 6361 7065 3a20 7374 722c 0d0a 2020 2020  cape: str,..    
+00002230: 7064 663a 2073 7472 2c0d 0a20 2020 2078  pdf: str,..    x
+00002240: 6d6c 3a20 5f45 6c65 6d65 6e74 2c0d 0a20  ml: _Element,.. 
+00002250: 2020 2073 7479 6c65 7368 6565 743a 204f     stylesheet: O
+00002260: 7074 696f 6e61 6c5b 7374 725d 203d 204e  ptional[str] = N
+00002270: 6f6e 652c 0d0a 2920 2d3e 2073 7472 3a0d  one,..) -> str:.
+00002280: 0a20 2020 2022 2222 0d0a 2020 2020 4372  .    """..    Cr
+00002290: 6561 7465 2061 2070 6466 2066 696c 6520  eate a pdf file 
+000022a0: 7769 7468 6f75 7420 7772 6974 696e 6720  without writing 
+000022b0: 616e 2069 6e74 6572 6d65 6469 6174 6520  an intermediate 
+000022c0: 7376 6720 6669 6c65 2e0d 0a0d 0a20 2020  svg file.....   
+000022d0: 203a 7061 7261 6d20 696e 6b73 6361 7065   :param inkscape
+000022e0: 3a20 7061 7468 2074 6f20 696e 6b73 6361  : path to inksca
+000022f0: 7065 2065 7865 6375 7461 626c 6520 2877  pe executable (w
+00002300: 6974 686f 7574 202e 6578 6520 6578 7465  ithout .exe exte
+00002310: 6e73 696f 6e21 290d 0a20 2020 203a 7061  nsion!)..    :pa
+00002320: 7261 6d20 7064 663a 2070 6174 6820 746f  ram pdf: path to
+00002330: 206f 7574 7075 7420 7064 6620 6669 6c65   output pdf file
+00002340: 0d0a 2020 2020 3a70 6172 616d 2078 6d6c  ..    :param xml
+00002350: 3a20 726f 6f74 206e 6f64 6520 6f66 2079  : root node of y
+00002360: 6f75 7220 7376 6720 6765 6f6d 6574 7279  our svg geometry
+00002370: 0d0a 2020 2020 3a70 6172 616d 2073 7479  ..    :param sty
+00002380: 6c65 7368 6565 743a 206f 7074 696f 6e61  lesheet: optiona
+00002390: 6c20 7061 7468 2074 6f20 6373 7320 7374  l path to css st
+000023a0: 796c 6573 6865 6574 0d0a 2020 2020 3a72  ylesheet..    :r
+000023b0: 6574 7572 6e3a 2070 6466 2066 696c 656e  eturn: pdf filen
+000023c0: 616d 6520 2874 6865 2073 616d 6520 796f  ame (the same yo
+000023d0: 7520 696e 7075 7420 6173 2060 6070 6466  u input as ``pdf
+000023e0: 6060 290d 0a20 2020 203a 6566 6665 6374  ``)..    :effect
+000023f0: 733a 2063 7265 6174 6573 2061 206e 6577  s: creates a new
+00002400: 2070 6466 2066 696c 650d 0a0d 0a20 2020   pdf file....   
+00002410: 2054 6869 7320 6a75 7374 2063 7265 6174   This just creat
+00002420: 6573 2061 2074 656d 7066 696c 652c 2077  es a tempfile, w
+00002430: 7269 7465 7320 7468 6520 7376 6720 746f  rites the svg to
+00002440: 2074 6865 2074 656d 7066 696c 652c 2074   the tempfile, t
+00002450: 6865 6e20 6361 6c6c 730d 0a20 2020 2060  hen calls..    `
+00002460: 6077 7269 7465 5f70 6466 5f66 726f 6d5f  `write_pdf_from_
+00002470: 7376 6760 6020 7769 7468 2074 6865 2074  svg`` with the t
+00002480: 656d 7066 696c 652e 2054 6869 7320 6973  empfile. This is
+00002490: 6e27 7420 6661 7374 6572 2028 6974 206d  n't faster (it m
+000024a0: 6967 6874 2062 6520 736c 6967 6874 6c79  ight be slightly
+000024b0: 0d0a 2020 2020 736c 6f77 6572 292c 2062  ..    slower), b
+000024c0: 7574 2069 7420 6b65 6570 7320 7468 6520  ut it keeps the 
+000024d0: 6669 6c65 7379 7374 656d 2063 6c65 616e  filesystem clean
+000024e0: 2077 6865 6e20 796f 7520 6f6e 6c79 2077   when you only w
+000024f0: 616e 7420 7468 6520 7064 662e 0d0a 2020  ant the pdf...  
+00002500: 2020 2222 220d 0a20 2020 2077 6974 6820    """..    with 
+00002510: 4e61 6d65 6454 656d 706f 7261 7279 4669  NamedTemporaryFi
+00002520: 6c65 286d 6f64 653d 2277 6222 2c20 6465  le(mode="wb", de
+00002530: 6c65 7465 3d46 616c 7365 2920 6173 2073  lete=False) as s
+00002540: 7667 5f66 696c 653a 0d0a 2020 2020 2020  vg_file:..      
+00002550: 2020 7376 6720 3d20 7772 6974 655f 7376    svg = write_sv
+00002560: 6728 7376 675f 6669 6c65 2c20 786d 6c2c  g(svg_file, xml,
+00002570: 2073 7479 6c65 7368 6565 7429 0d0a 2020   stylesheet)..  
+00002580: 2020 5f20 3d20 7772 6974 655f 7064 665f    _ = write_pdf_
+00002590: 6672 6f6d 5f73 7667 2869 6e6b 7363 6170  from_svg(inkscap
+000025a0: 652c 2073 7667 2c20 7064 6629 0d0a 2020  e, svg, pdf)..  
+000025b0: 2020 6f73 2e75 6e6c 696e 6b28 7376 6729    os.unlink(svg)
+000025c0: 0d0a 2020 2020 7265 7475 726e 2070 6466  ..    return pdf
+000025d0: 0d0a                                     ..
```

### Comparing `svg_ultralight-0.8.2/svg_ultralight.egg-info/SOURCES.txt` & `svg_ultralight-0.9.0/svg_ultralight.egg-info/SOURCES.txt`

 * *Files 16% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 LICENSE.txt
 MANIFEST.in
 README.md
+pyproject.toml
 setup.py
 svg_ultralight/__init__.py
 svg_ultralight/animate.py
+svg_ultralight/main.py
 svg_ultralight/nsmap.py
 svg_ultralight/py.typed
 svg_ultralight/query.py
 svg_ultralight/string_conversion.py
-svg_ultralight/svg_ultralight.py
 svg_ultralight.egg-info/PKG-INFO
 svg_ultralight.egg-info/SOURCES.txt
 svg_ultralight.egg-info/dependency_links.txt
 svg_ultralight.egg-info/requires.txt
 svg_ultralight.egg-info/top_level.txt
 svg_ultralight/constructors/__init__.py
 svg_ultralight/constructors/new_element.py
```

### Comparing `svg_ultralight-0.8.2/test/test_new_element.py` & `svg_ultralight-0.9.0/test/test_new_element.py`

 * *Files 12% similar despite different names*

```diff
@@ -2,80 +2,61 @@
 # _*_ coding: utf-8 _*_
 """Test functions in constructors.new_element
 
 :author: Shay Hill
 :created: 1/31/2020
 """
 
-from lxml import etree  # type: ignore
+from lxml import etree
 
-from svg_ultralight.constructors.new_element import (
-    deepcopy_element,
-    new_element,
-    new_sub_element,
-    update_element,
-)
+from svg_ultralight import constructors
 
 
 class TestNewElement:
     def test_params(self) -> None:
         """Replace _ with -. Pass params.values() as strings"""
-        elem = new_element("line", x=10, y1=80, stroke_width="2")
+        elem = constructors.new_element("line", x=10, y1=80, stroke_width="2")
         assert etree.tostring(elem) == b'<line x="10" y1="80" stroke-width="2"/>'
 
     def test_qualified_name_string_conversion(self) -> None:
         """If a keyword argument has :, convert to qname"""
-        elem = new_element("line", **{"xlink:href": 10})
+        elem = constructors.new_element("line", **{"xlink:href": 10})
         assert (
             etree.tostring(elem)
             == b'<line xmlns:ns0="http://www.w3.org/1999/xlink" ns0:href="10"/>'
         )
 
     def test_trailing_underscore(self) -> None:
         """Remove trailing _ from params"""
-        elem = new_element("line", x=10, y1=80, in_="SourceAlpha")
+        elem = constructors.new_element("line", x=10, y1=80, in_="SourceAlpha")
         assert etree.tostring(elem) == b'<line x="10" y1="80" in="SourceAlpha"/>'
 
     def test_param_text(self) -> None:
         """Insert text between tags with parameters"""
-        elem = new_element("text", x=120, y=12, text="text here")
+        elem = constructors.new_element("text", x=120, y=12, text="text here")
         assert etree.tostring(elem) == b'<text x="120" y="12">text here</text>'
 
     def test_text(self) -> None:
         """Insert text between tags"""
-        elem = new_element("text", text="text here")
+        elem = constructors.new_element("text", text="text here")
         assert etree.tostring(elem) == b"<text>text here</text>"
 
     def test_float(self) -> None:
         """Floats at 0.6f precision"""
-        elem = new_element("text", x=1/3)
+        elem = constructors.new_element("text", x=1 / 3)
         assert etree.tostring(elem) == b'<text x="0.333333"/>'
 
 
 class TestNewSubElement:
     def test_sub_element(self) -> None:
         """New element is a sub-element of parent"""
-        parent = new_element("g")
-        _ = new_sub_element(parent, "rect")
+        parent = constructors.new_element("g")
+        _ = constructors.new_sub_element(parent, "rect")
         assert etree.tostring(parent) == b"<g><rect/></g>"
 
 
 class TestUpdateElement:
     def test_new_params(self) -> None:
         """New params added"""
-        elem = new_element("line", x=10, y1=80)
-        update_element(elem, stroke_width=2)
+        elem = constructors.new_element("line", x=10, y1=80)
+        _ = constructors.update_element(elem, stroke_width=2)
         assert etree.tostring(elem) == b'<line x="10" y1="80" stroke-width="2"/>'
-
-
-class TestDeepcopyElement:
-    def test_is_copy(self) -> None:
-        """"""
-        group = new_element("g")
-        line = new_sub_element(group, "line", x=10, y1=80)
-        group_copy = deepcopy_element(group, stroke="black")
-        assert (
-            etree.tostring(group_copy)
-            == b'<g stroke="black"><line x="10" y1="80"/></g>'
-        )
-        assert line in group
-        assert line not in group_copy
```

### Comparing `svg_ultralight-0.8.2/test/test_queries.py` & `svg_ultralight-0.9.0/test/test_queries.py`

 * *Files 24% similar despite different names*

```diff
@@ -6,28 +6,42 @@
 :created: 7/25/2020
 
 A quick test. Won't be able to run it till you change INKSCAPE to the correct path on
 your system.
 """
 
 import math
+import pytest
 
 from svg_ultralight import new_svg_root
-from svg_ultralight.constructors import new_element, new_sub_element
+from svg_ultralight.constructors import new_sub_element
 from svg_ultralight.query import (
     BoundingBox,
     get_bounding_box,
     map_ids_to_bounding_boxes,
 )
 
 INKSCAPE = r"C:\Program Files\Inkscape\bin\inkscape"
 
 
-aaa = BoundingBox(-2, -4, 10, 20)
-bbb = BoundingBox(3, 4, 10, 20)
+class TestMergeBoundingBoxes:
+    def test_merge_deprecation_warning(self):
+        bbox_a = BoundingBox(-2, -4, 10, 20)
+        bbox_b = BoundingBox(0, 0, 10, 10)
+        with pytest.raises(DeprecationWarning):
+            _ = bbox_a.merge(bbox_b)
+
+    def test_new_merged_bbox(self):
+        bbox_a = BoundingBox(-2, -4, 10, 20)
+        bbox_b = BoundingBox(0, 0, 10, 10)
+        merged = BoundingBox.merged(bbox_a, bbox_b)
+        assert merged.x == -2
+        assert merged.y == -4
+        assert merged.width == 12
+        assert merged.height == 20
 
 
 class TestTransformBoundingBoxes:
     def test_transforms_commutative(self):
         """
         Scale then transform = transform then scale
         """
@@ -44,54 +58,52 @@
 
 
 class TestMapIdsToBoundingBoxes:
     def test_gets_bboxes(self) -> None:
         """
         Run with a temporary file.
         """
-        expected = {
-            "svg4": BoundingBox(x=0.0, y=0.0, width=16.0, height=32.0),
-            "rect1": BoundingBox(x=0.0, y=0.0, width=16.0, height=9.0),
-            "rect2": BoundingBox(x=0.0, y=0.0, width=8.0, height=32.0),
-        }
+        xml = new_svg_root(10, 20, 160, 19, id="svg1")
+        _ = new_sub_element(xml, "rect", id="rect1", x=0, y=0, width=16, height=9)
+        _ = new_sub_element(xml, "rect", id="rect2", x=0, y=0, width=8, height=32)
+        result = map_ids_to_bounding_boxes(INKSCAPE, xml)
+        assert result["rect1"] == BoundingBox(0.0, 0.0, 16.0, 9.0)
+        assert result["rect2"] == BoundingBox(0.0, 0.0, 8.0, 32.0)
 
+    def test_adds_missing_ids(self) -> None:
+        """Returns a dict with an entry for each element plus an envelope entry."""
         xml = new_svg_root(10, 20, 160, 19, id="svg1")
-        new_sub_element(xml, "rect", id="rect1", x=0, y=0, width=16, height=9)
-        new_sub_element(xml, "rect", id="rect2", x=0, y=0, width=8, height=32)
+        rect1 = new_sub_element(xml, "rect", x=0, y=0, width=16, height=9)
+        rect2 = new_sub_element(xml, "rect", x=0, y=0, width=8, height=32)
+        rect3 = new_sub_element(xml, "rect", x=0, y=0, width=12, height=18)
         result = map_ids_to_bounding_boxes(INKSCAPE, xml)
-        assert result == expected
+        assert xml.get("id") in result.keys()
+        assert rect1.get("id") in result.keys()
+        assert rect2.get("id") in result.keys()
+        assert rect3.get("id") in result.keys()
 
 
 class TestGetBBox:
-    def test_single(self) -> None:
-        """
-        Return bounding box around entire group.
-        :return:
-        """
-        rect = new_element("rect", id="rect1", x=0, y=0, width=16, height=9)
-        result = get_bounding_box(INKSCAPE, rect)
-        assert result == BoundingBox(0, 0, 16, 9)
-
-    def test_grouped(self) -> None:
+    def test_raises_deprecation_warning(self) -> None:
         """
         Return bounding box around entire group.
         :return:
         """
         xml = new_svg_root(10, 20, 160, 19, id="svg1")
         group = new_sub_element(xml, "g", id="grouped elements")
-        new_sub_element(group, "rect", id="rect1", x=0, y=0, width=16, height=9)
-        new_sub_element(group, "rect", id="rect2", x=1, y=1, width=8, height=32)
-        result = get_bounding_box(INKSCAPE, group)
-        assert result == BoundingBox(0, 0, 16, 33)
+        _ = new_sub_element(group, "rect", id="rect1", x=0, y=0, width=16, height=9)
+        _ = new_sub_element(group, "rect", id="rect2", x=1, y=1, width=8, height=32)
+        with pytest.raises(DeprecationWarning):
+            _ = get_bounding_box(INKSCAPE, group)
 
 
 class TestAlterBoundingBox:
     def test_reverse_width(self) -> None:
-        """ adjust width one way then the other returns to original box """
+        """adjust width one way then the other returns to original box"""
         bbox = BoundingBox(10, 20, 30, 40)
         bbox.x = 100
         bbox.y = 200
         bbox.height = 200
         bbox.height = 40
         assert math.isclose(bbox.scale, 1)
-        assert math.isclose(bbox._translation_x, 90)
-        assert math.isclose(bbox._translation_y, 180)
+        assert math.isclose(bbox._translation_x, 90)  # type: ignore
+        assert math.isclose(bbox._translation_y, 180)  # type: ignore
```

### Comparing `svg_ultralight-0.8.2/test/test_svg_ultralight.py` & `svg_ultralight-0.9.0/test/test_svg_ultralight.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,400 +19,396 @@
 00000120: 6d20 7061 7468 6c69 6220 696d 706f 7274  m pathlib import
 00000130: 2050 6174 680d 0a0d 0a69 6d70 6f72 7420   Path....import 
 00000140: 7079 7465 7374 0d0a 6672 6f6d 206c 786d  pytest..from lxm
 00000150: 6c20 696d 706f 7274 2065 7472 6565 0d0a  l import etree..
 00000160: 0d0a 2320 6e6f 696e 7370 6563 7469 6f6e  ..# noinspection
 00000170: 2050 7950 726f 7465 6374 6564 4d65 6d62   PyProtectedMemb
 00000180: 6572 0d0a 6672 6f6d 2073 7667 5f75 6c74  er..from svg_ult
-00000190: 7261 6c69 6768 742e 7376 675f 756c 7472  ralight.svg_ultr
-000001a0: 616c 6967 6874 2069 6d70 6f72 7420 6e65  alight import ne
-000001b0: 775f 7376 675f 726f 6f74 2c20 7772 6974  w_svg_root, writ
-000001c0: 655f 7376 670d 0a66 726f 6d20 7376 675f  e_svg..from svg_
-000001d0: 756c 7472 616c 6967 6874 2069 6d70 6f72  ultralight impor
-000001e0: 7420 4e53 4d41 500d 0a66 726f 6d20 7376  t NSMAP..from sv
-000001f0: 675f 756c 7472 616c 6967 6874 2e73 7472  g_ultralight.str
-00000200: 696e 675f 636f 6e76 6572 7369 6f6e 2069  ing_conversion i
-00000210: 6d70 6f72 7420 7376 675f 746f 7374 7269  mport svg_tostri
-00000220: 6e67 0d0a 0d0a 0d0a 4070 7974 6573 742e  ng......@pytest.
-00000230: 6669 7874 7572 650d 0a64 6566 2063 7373  fixture..def css
-00000240: 5f73 6f75 7263 6528 293a 0d0a 2020 2020  _source():..    
-00000250: 2222 2254 656d 706f 7261 7279 2063 7373  """Temporary css
-00000260: 2066 696c 6520 6f62 6a65 6374 2077 6974   file object wit
-00000270: 6820 6d65 616e 696e 676c 6573 7320 636f  h meaningless co
-00000280: 6e74 656e 7473 2e22 2222 0d0a 2020 2020  ntents."""..    
-00000290: 7769 7468 2074 656d 7066 696c 652e 4e61  with tempfile.Na
-000002a0: 6d65 6454 656d 706f 7261 7279 4669 6c65  medTemporaryFile
-000002b0: 286d 6f64 653d 2277 222c 2064 656c 6574  (mode="w", delet
-000002c0: 653d 4661 6c73 6529 2061 7320 6373 735f  e=False) as css_
-000002d0: 736f 7572 6365 3a0d 0a20 2020 2020 2020  source:..       
-000002e0: 2063 7373 5f73 6f75 7263 652e 7772 6974   css_source.writ
-000002f0: 6528 222f 2a2a 2063 7373 2066 6f72 206d  e("/** css for m
-00000300: 7920 7072 6f6a 6563 7420 2a2a 2f22 290d  y project **/").
-00000310: 0a20 2020 2079 6965 6c64 2063 7373 5f73  .    yield css_s
-00000320: 6f75 7263 652e 6e61 6d65 0d0a 2020 2020  ource.name..    
-00000330: 6f73 2e75 6e6c 696e 6b28 6373 735f 736f  os.unlink(css_so
-00000340: 7572 6365 2e6e 616d 6529 0d0a 0d0a 0d0a  urce.name)......
-00000350: 4070 7974 6573 742e 6669 7874 7572 650d  @pytest.fixture.
-00000360: 0a64 6566 2074 656d 705f 6669 6c65 6e61  .def temp_filena
-00000370: 6d65 286d 6f64 653d 2277 2229 3a0d 0a20  me(mode="w"):.. 
-00000380: 2020 2022 2222 5465 6d70 6f72 6172 7920     """Temporary 
-00000390: 6669 6c65 206f 626a 6563 7420 746f 2063  file object to c
-000003a0: 6170 7475 7265 2074 6573 7420 6f75 7470  apture test outp
-000003b0: 7574 2e22 2222 0d0a 2020 2020 7376 675f  ut."""..    svg_
-000003c0: 6f75 7470 7574 203d 2074 656d 7066 696c  output = tempfil
-000003d0: 652e 4e61 6d65 6454 656d 706f 7261 7279  e.NamedTemporary
-000003e0: 4669 6c65 286d 6f64 653d 6d6f 6465 2c20  File(mode=mode, 
-000003f0: 6465 6c65 7465 3d46 616c 7365 290d 0a20  delete=False).. 
-00000400: 2020 2073 7667 5f6f 7574 7075 742e 636c     svg_output.cl
-00000410: 6f73 6528 290d 0a20 2020 2079 6965 6c64  ose()..    yield
-00000420: 2073 7667 5f6f 7574 7075 742e 6e61 6d65   svg_output.name
-00000430: 0d0a 2020 2020 6f73 2e75 6e6c 696e 6b28  ..    os.unlink(
-00000440: 7376 675f 6f75 7470 7574 2e6e 616d 6529  svg_output.name)
-00000450: 0d0a 0d0a 0d0a 636c 6173 7320 5465 7374  ......class Test
-00000460: 5772 6974 6553 7667 3a0d 0a20 2020 2064  WriteSvg:..    d
-00000470: 6566 2074 6573 745f 6c69 6e6b 6564 2873  ef test_linked(s
-00000480: 656c 662c 2063 7373 5f73 6f75 7263 652c  elf, css_source,
-00000490: 2074 656d 705f 6669 6c65 6e61 6d65 2920   temp_filename) 
-000004a0: 2d3e 204e 6f6e 653a 0d0a 2020 2020 2020  -> None:..      
-000004b0: 2020 2222 2249 6e73 6572 7420 7374 796c    """Insert styl
-000004c0: 6573 6865 6574 2072 6566 6572 656e 6365  esheet reference
-000004d0: 2222 220d 0a20 2020 2020 2020 2062 6c61  """..        bla
-000004e0: 6e6b 203d 2065 7472 6565 2e45 6c65 6d65  nk = etree.Eleme
-000004f0: 6e74 2822 626c 616e 6b22 290d 0a20 2020  nt("blank")..   
-00000500: 2020 2020 2077 7269 7465 5f73 7667 280d       write_svg(.
-00000510: 0a20 2020 2020 2020 2020 2020 2074 656d  .            tem
-00000520: 705f 6669 6c65 6e61 6d65 2c20 626c 616e  p_filename, blan
-00000530: 6b2c 2063 7373 5f73 6f75 7263 652c 2064  k, css_source, d
-00000540: 6f5f 6c69 6e6b 5f63 7373 3d54 7275 652c  o_link_css=True,
-00000550: 2078 6d6c 5f64 6563 6c61 7261 7469 6f6e   xml_declaration
-00000560: 3d54 7275 652c 0d0a 2020 2020 2020 2020  =True,..        
-00000570: 290d 0a20 2020 2020 2020 2077 6974 6820  )..        with 
-00000580: 6f70 656e 2874 656d 705f 6669 6c65 6e61  open(temp_filena
-00000590: 6d65 2c20 2272 6222 2920 6173 2073 7667  me, "rb") as svg
-000005a0: 5f62 696e 6172 793a 0d0a 2020 2020 2020  _binary:..      
-000005b0: 2020 2020 2020 7376 675f 6c69 6e65 7320        svg_lines 
-000005c0: 3d20 5b78 2e64 6563 6f64 6528 2920 666f  = [x.decode() fo
-000005d0: 7220 7820 696e 2073 7667 5f62 696e 6172  r x in svg_binar
-000005e0: 792e 7265 6164 6c69 6e65 7328 295d 0d0a  y.readlines()]..
-000005f0: 0d0a 2020 2020 2020 2020 7265 6c61 7469  ..        relati
-00000600: 7665 5f63 7373 5f70 6174 6820 3d20 5061  ve_css_path = Pa
-00000610: 7468 2863 7373 5f73 6f75 7263 6529 2e72  th(css_source).r
-00000620: 656c 6174 6976 655f 746f 2850 6174 6828  elative_to(Path(
-00000630: 7465 6d70 5f66 696c 656e 616d 6529 2e70  temp_filename).p
-00000640: 6172 656e 7429 0d0a 2020 2020 2020 2020  arent)..        
-00000650: 6173 7365 7274 2073 7667 5f6c 696e 6573  assert svg_lines
-00000660: 203d 3d20 5b0d 0a20 2020 2020 2020 2020   == [..         
-00000670: 2020 2022 3c3f 786d 6c20 7665 7273 696f     "<?xml versio
-00000680: 6e3d 2731 2e30 2720 656e 636f 6469 6e67  n='1.0' encoding
-00000690: 3d27 5554 462d 3827 3f3e 5c6e 222c 0d0a  ='UTF-8'?>\n",..
-000006a0: 2020 2020 2020 2020 2020 2020 273c 2144              '<!D
-000006b0: 4f43 5459 5045 2073 7667 2050 5542 4c49  OCTYPE svg PUBLI
-000006c0: 4320 222d 2f2f 5733 432f 2f44 5444 2053  C "-//W3C//DTD S
-000006d0: 5647 2031 2e31 2f2f 454e 225c 6e27 2c0d  VG 1.1//EN"\n',.
-000006e0: 0a20 2020 2020 2020 2020 2020 2027 2268  .            '"h
-000006f0: 7474 703a 2f2f 7777 772e 7733 2e6f 7267  ttp://www.w3.org
-00000700: 2f47 7261 7068 6963 732f 5356 472f 312e  /Graphics/SVG/1.
-00000710: 312f 4454 442f 7376 6731 312e 6474 6422  1/DTD/svg11.dtd"
-00000720: 3e5c 6e27 2c0d 0a20 2020 2020 2020 2020  >\n',..         
-00000730: 2020 2066 273c 3f78 6d6c 2d73 7479 6c65     f'<?xml-style
-00000740: 7368 6565 7420 6872 6566 3d22 7b72 656c  sheet href="{rel
-00000750: 6174 6976 655f 6373 735f 7061 7468 7d22  ative_css_path}"
-00000760: 2074 7970 653d 2274 6578 742f 6373 7322   type="text/css"
-00000770: 3f3e 5c6e 272c 0d0a 2020 2020 2020 2020  ?>\n',..        
-00000780: 2020 2020 223c 626c 616e 6b2f 3e5c 6e22      "<blank/>\n"
-00000790: 2c0d 0a20 2020 2020 2020 205d 0d0a 0d0a  ,..        ]....
-000007a0: 2020 2020 6465 6620 7465 7374 5f6e 6f74      def test_not
-000007b0: 5f6c 696e 6b65 6428 7365 6c66 2c20 6373  _linked(self, cs
-000007c0: 735f 736f 7572 6365 2c20 7465 6d70 5f66  s_source, temp_f
-000007d0: 696c 656e 616d 6529 202d 3e20 4e6f 6e65  ilename) -> None
-000007e0: 3a0d 0a20 2020 2020 2020 2022 2222 436f  :..        """Co
-000007f0: 7079 2063 7373 5f73 6f75 7263 6520 636f  py css_source co
-00000800: 6e74 656e 7473 2069 6e74 6f20 7376 6720  ntents into svg 
-00000810: 6669 6c65 2222 220d 0a20 2020 2020 2020  file"""..       
-00000820: 2062 6c61 6e6b 203d 2065 7472 6565 2e45   blank = etree.E
-00000830: 6c65 6d65 6e74 2822 626c 616e 6b22 290d  lement("blank").
-00000840: 0a20 2020 2020 2020 2077 7269 7465 5f73  .        write_s
-00000850: 7667 2874 656d 705f 6669 6c65 6e61 6d65  vg(temp_filename
-00000860: 2c20 626c 616e 6b2c 2063 7373 5f73 6f75  , blank, css_sou
-00000870: 7263 6529 0d0a 2020 2020 2020 2020 7769  rce)..        wi
-00000880: 7468 206f 7065 6e28 7465 6d70 5f66 696c  th open(temp_fil
-00000890: 656e 616d 652c 2022 7262 2229 2061 7320  ename, "rb") as 
-000008a0: 7376 675f 6269 6e61 7279 3a0d 0a20 2020  svg_binary:..   
-000008b0: 2020 2020 2020 2020 2073 7667 5f6c 696e           svg_lin
-000008c0: 6573 203d 205b 782e 6465 636f 6465 2829  es = [x.decode()
-000008d0: 2066 6f72 2078 2069 6e20 7376 675f 6269   for x in svg_bi
-000008e0: 6e61 7279 2e72 6561 646c 696e 6573 2829  nary.readlines()
-000008f0: 5d0d 0a0d 0a20 2020 2020 2020 2061 7373  ]....        ass
-00000900: 6572 7420 7376 675f 6c69 6e65 7320 3d3d  ert svg_lines ==
-00000910: 205b 0d0a 2020 2020 2020 2020 2020 2020   [..            
-00000920: 223c 626c 616e 6b3e 5c6e 222c 0d0a 2020  "<blank>\n",..  
-00000930: 2020 2020 2020 2020 2020 2720 203c 7374            '  <st
-00000940: 796c 6520 7479 7065 3d22 7465 7874 2f63  yle type="text/c
-00000950: 7373 223e 3c21 5b43 4441 5441 5b5c 6e27  ss"><![CDATA[\n'
-00000960: 2c0d 0a20 2020 2020 2020 2020 2020 2022  ,..            "
-00000970: 2f2a 2a20 6373 7320 666f 7220 6d79 2070  /** css for my p
-00000980: 726f 6a65 6374 202a 2a2f 5c6e 222c 0d0a  roject **/\n",..
-00000990: 2020 2020 2020 2020 2020 2020 225d 5d3e              "]]>
-000009a0: 3c2f 7374 796c 653e 5c6e 222c 0d0a 2020  </style>\n",..  
-000009b0: 2020 2020 2020 2020 2020 223c 2f62 6c61            "</bla
-000009c0: 6e6b 3e5c 6e22 2c0d 0a20 2020 2020 2020  nk>\n",..       
-000009d0: 205d 0d0a 0d0a 2020 2020 6465 6620 7465   ]....    def te
-000009e0: 7374 5f63 7373 5f6e 6f6e 6528 7365 6c66  st_css_none(self
-000009f0: 2c20 7465 6d70 5f66 696c 656e 616d 6529  , temp_filename)
-00000a00: 202d 3e20 4e6f 6e65 3a0d 0a20 2020 2020   -> None:..     
-00000a10: 2020 2022 2222 446f 206e 6f74 206c 696e     """Do not lin
-00000a20: 6b20 6f72 2063 6f70 7920 696e 2063 7373  k or copy in css
-00000a30: 2069 6620 6e6f 2063 7373 5f73 6f75 7263   if no css_sourc
-00000a40: 6520 6973 2070 6173 7365 642e 2222 220d  e is passed.""".
-00000a50: 0a20 2020 2020 2020 2062 6c61 6e6b 203d  .        blank =
-00000a60: 2065 7472 6565 2e45 6c65 6d65 6e74 2822   etree.Element("
-00000a70: 626c 616e 6b22 290d 0a20 2020 2020 2020  blank")..       
-00000a80: 2077 7269 7465 5f73 7667 2874 656d 705f   write_svg(temp_
-00000a90: 6669 6c65 6e61 6d65 2c20 626c 616e 6b2c  filename, blank,
-00000aa0: 2064 6f5f 6c69 6e6b 5f63 7373 3d54 7275   do_link_css=Tru
-00000ab0: 6529 0d0a 2020 2020 2020 2020 7769 7468  e)..        with
-00000ac0: 206f 7065 6e28 7465 6d70 5f66 696c 656e   open(temp_filen
-00000ad0: 616d 652c 2022 7262 2229 2061 7320 7376  ame, "rb") as sv
-00000ae0: 675f 6269 6e61 7279 3a0d 0a20 2020 2020  g_binary:..     
-00000af0: 2020 2020 2020 2073 7667 5f6c 696e 6573         svg_lines
-00000b00: 203d 205b 782e 6465 636f 6465 2829 2066   = [x.decode() f
-00000b10: 6f72 2078 2069 6e20 7376 675f 6269 6e61  or x in svg_bina
-00000b20: 7279 2e72 6561 646c 696e 6573 2829 5d0d  ry.readlines()].
-00000b30: 0a0d 0a20 2020 2020 2020 2061 7373 6572  ...        asser
-00000b40: 7420 7376 675f 6c69 6e65 7320 3d3d 205b  t svg_lines == [
-00000b50: 0d0a 2020 2020 2020 2020 2020 2020 223c  ..            "<
-00000b60: 626c 616e 6b2f 3e5c 6e22 2c0d 0a20 2020  blank/>\n",..   
-00000b70: 2020 2020 205d 0d0a 0d0a 2020 2020 2020       ]....      
-00000b80: 2020 2320 7465 7374 2077 6974 6820 646f    # test with do
-00000b90: 5f6c 696e 6b5f 6373 7320 3d20 4661 6c73  _link_css = Fals
-00000ba0: 650d 0a20 2020 2020 2020 2077 7269 7465  e..        write
-00000bb0: 5f73 7667 2874 656d 705f 6669 6c65 6e61  _svg(temp_filena
-00000bc0: 6d65 2c20 626c 616e 6b29 0d0a 2020 2020  me, blank)..    
-00000bd0: 2020 2020 7769 7468 206f 7065 6e28 7465      with open(te
-00000be0: 6d70 5f66 696c 656e 616d 652c 2022 7262  mp_filename, "rb
-00000bf0: 2229 2061 7320 7376 675f 6269 6e61 7279  ") as svg_binary
-00000c00: 3a0d 0a20 2020 2020 2020 2020 2020 2073  :..            s
-00000c10: 7667 5f6c 696e 6573 5f66 616c 7365 203d  vg_lines_false =
-00000c20: 205b 782e 6465 636f 6465 2829 2066 6f72   [x.decode() for
-00000c30: 2078 2069 6e20 7376 675f 6269 6e61 7279   x in svg_binary
-00000c40: 2e72 6561 646c 696e 6573 2829 5d0d 0a20  .readlines()].. 
-00000c50: 2020 2020 2020 2061 7373 6572 7420 7376         assert sv
-00000c60: 675f 6c69 6e65 735f 6661 6c73 6520 3d3d  g_lines_false ==
-00000c70: 2073 7667 5f6c 696e 6573 0d0a 0d0a 0d0a   svg_lines......
-00000c80: 6465 6620 7376 675f 726f 6f74 282a 2a6b  def svg_root(**k
-00000c90: 7761 7267 7329 202d 3e20 6574 7265 652e  wargs) -> etree.
-00000ca0: 456c 656d 656e 743a 0d0a 2020 2020 2222  Element:..    ""
-00000cb0: 220d 0a20 2020 2043 7265 6174 6520 616e  "..    Create an
-00000cc0: 2073 7667 2072 6f6f 7420 6672 6f6d 2061   svg root from a
-00000cd0: 7474 7269 6275 7465 206b 7761 7267 730d  ttribute kwargs.
-00000ce0: 0a0d 0a20 2020 203a 7061 7261 6d20 6b77  ...    :param kw
-00000cf0: 6172 6773 3a20 6578 6163 7420 7376 6720  args: exact svg 
-00000d00: 6174 7472 6962 7574 6520 6e61 6d65 730d  attribute names.
-00000d10: 0a20 2020 203a 7265 7475 726e 3a20 6120  .    :return: a 
-00000d20: 7661 6c69 6420 726f 6f74 2074 6f20 7465  valid root to te
-00000d30: 7374 2061 6761 696e 7374 0d0a 0d0a 2020  st against....  
-00000d40: 2020 5468 6520 7072 6f63 6573 7320 6973    The process is
-00000d50: 2074 6869 733a 0d0a 2020 2020 2a20 6372   this:..    * cr
-00000d60: 6561 7465 2061 2072 6f6f 7420 6865 7265  eate a root here
-00000d70: 2077 6974 6820 6578 706c 6963 6974 2061   with explicit a
-00000d80: 7474 7269 6275 7465 730d 0a20 2020 202a  ttributes..    *
-00000d90: 2063 7265 6174 6520 6120 726f 6f74 2077   create a root w
-00000da0: 6974 6820 6120 6675 6e63 7469 6f6e 2074  ith a function t
-00000db0: 6861 7420 696e 6665 7273 2065 7870 6c69  hat infers expli
-00000dc0: 6369 7420 6174 7472 6962 7574 6573 0d0a  cit attributes..
-00000dd0: 2020 2020 2a20 636f 6d70 6172 6520 7265      * compare re
-00000de0: 7375 6c74 730d 0a20 2020 2022 2222 0d0a  sults..    """..
-00000df0: 2020 2020 6e61 6d65 7370 6163 6520 3d20      namespace = 
-00000e00: 7475 706c 6528 4e53 4d41 502e 6974 656d  tuple(NSMAP.item
-00000e10: 7328 2929 0d0a 2020 2020 786d 6c6e 7320  s())..    xmlns 
-00000e20: 3d20 5b66 2778 6d6c 6e73 3d22 7b6e 616d  = [f'xmlns="{nam
-00000e30: 6573 7061 6365 5b30 5d5b 315d 7d22 275d  espace[0][1]}"']
-00000e40: 0d0a 2020 2020 786d 6c6e 7320 2b3d 205b  ..    xmlns += [
-00000e50: 6627 786d 6c6e 733a 7b6b 7d3d 227b 767d  f'xmlns:{k}="{v}
-00000e60: 2227 2066 6f72 206b 2c20 7620 696e 206e  "' for k, v in n
-00000e70: 616d 6573 7061 6365 5b31 3a5d 5d0d 0a20  amespace[1:]].. 
-00000e80: 2020 2061 7474 7269 6275 7465 7320 3d20     attributes = 
-00000e90: 2720 272e 6a6f 696e 285b 6627 7b6b 7d3d  ' '.join([f'{k}=
-00000ea0: 227b 767d 2227 2066 6f72 206b 2c20 7620  "{v}"' for k, v 
-00000eb0: 696e 206b 7761 7267 732e 6974 656d 7328  in kwargs.items(
-00000ec0: 295d 290d 0a20 2020 2072 6574 7572 6e20  )])..    return 
-00000ed0: 6574 7265 652e 6672 6f6d 7374 7269 6e67  etree.fromstring
-00000ee0: 2866 273c 7376 6720 7b22 2022 2e6a 6f69  (f'<svg {" ".joi
-00000ef0: 6e28 786d 6c6e 7329 7d20 7b61 7474 7269  n(xmlns)} {attri
-00000f00: 6275 7465 737d 2f3e 272e 656e 636f 6465  butes}/>'.encode
-00000f10: 2829 290d 0a0d 0a0d 0a63 6c61 7373 2054  ())......class T
-00000f20: 6573 744e 6577 5376 6752 6f6f 743a 0d0a  estNewSvgRoot:..
-00000f30: 2020 2020 6465 6620 7465 7374 5f6e 736d      def test_nsm
-00000f40: 6170 2873 656c 6629 202d 3e20 4e6f 6e65  ap(self) -> None
-00000f50: 3a0d 0a20 2020 2020 2020 2022 2222 204e  :..        """ N
-00000f60: 534d 4150 2070 6173 7365 6420 6279 2064  SMAP passed by d
-00000f70: 6566 6175 6c74 2061 6e64 2070 6172 7365  efault and parse
-00000f80: 6162 6c65 2062 7920 6c78 6d6c 2022 2222  able by lxml """
-00000f90: 0d0a 2020 2020 2020 2020 7265 7375 6c74  ..        result
-00000fa0: 203d 206e 6577 5f73 7667 5f72 6f6f 7428   = new_svg_root(
-00000fb0: 290d 0a20 2020 2020 2020 2061 7373 6572  )..        asser
-00000fc0: 7420 7265 7375 6c74 2e6e 736d 6170 203d  t result.nsmap =
-00000fd0: 3d20 4e53 4d41 500d 0a0d 0a20 2020 2064  = NSMAP....    d
-00000fe0: 6566 2074 6573 745f 6172 6773 5f70 6173  ef test_args_pas
-00000ff0: 7328 7365 6c66 2920 2d3e 204e 6f6e 653a  s(self) -> None:
-00001000: 0d0a 2020 2020 2020 2020 2222 2241 7267  ..        """Arg
-00001010: 756d 656e 7473 2061 6e64 2078 6d6c 6e73  uments and xmlns
-00001020: 2061 7070 6561 7220 696e 2065 6c65 6d65   appear in eleme
-00001030: 6e74 2e0d 0a0d 0a20 2020 2020 2020 2042  nt.....        B
-00001040: 7569 6c64 2074 6865 2073 7667 2065 6c65  uild the svg ele
-00001050: 6d65 6e74 206e 616d 6573 7061 6365 2066  ment namespace f
-00001060: 726f 6d20 4e53 4d41 5020 616e 6420 636f  rom NSMAP and co
-00001070: 6d70 6172 6520 746f 206f 7574 7075 7422  mpare to output"
-00001080: 2222 0d0a 2020 2020 2020 2020 6578 7065  ""..        expe
-00001090: 6374 203d 2073 7667 5f72 6f6f 7428 0d0a  ct = svg_root(..
-000010a0: 2020 2020 2020 2020 2020 2020 2a2a 7b22              **{"
-000010b0: 7669 6577 426f 7822 3a20 2230 2031 2032  viewBox": "0 1 2
-000010c0: 2033 222c 2022 7769 6474 6822 3a20 2232   3", "width": "2
-000010d0: 222c 2022 6865 6967 6874 223a 2022 3322  ", "height": "3"
-000010e0: 7d0d 0a20 2020 2020 2020 2029 0d0a 2020  }..        )..  
-000010f0: 2020 2020 2020 7265 7375 6c74 203d 206e        result = n
-00001100: 6577 5f73 7667 5f72 6f6f 7428 302c 2031  ew_svg_root(0, 1
-00001110: 2c20 322c 2033 290d 0a20 2020 2020 2020  , 2, 3)..       
-00001120: 2061 7373 6572 7420 7265 7375 6c74 2e61   assert result.a
-00001130: 7474 7269 6220 3d3d 2065 7870 6563 742e  ttrib == expect.
-00001140: 6174 7472 6962 0d0a 0d0a 2020 2020 6465  attrib....    de
-00001150: 6620 7465 7374 5f61 6464 6974 696f 6e61  f test_additiona
-00001160: 6c5f 7061 7261 6d73 2873 656c 6629 202d  l_params(self) -
-00001170: 3e20 4e6f 6e65 3a0d 0a20 2020 2020 2020  > None:..       
-00001180: 2022 2222 5061 7373 2061 6464 6974 696f   """Pass additio
-00001190: 6e61 6c20 7061 7261 6d73 2222 220d 0a20  nal params""".. 
-000011a0: 2020 2020 2020 2065 7870 6563 7420 3d20         expect = 
-000011b0: 7376 675f 726f 6f74 280d 0a20 2020 2020  svg_root(..     
-000011c0: 2020 2020 2020 202a 2a7b 2261 7474 7222         **{"attr"
-000011d0: 3a20 2276 616c 7565 222c 2022 7669 6577  : "value", "view
-000011e0: 426f 7822 3a20 2230 2031 2032 2033 222c  Box": "0 1 2 3",
-000011f0: 2022 7769 6474 6822 3a20 2232 222c 2022   "width": "2", "
-00001200: 6865 6967 6874 223a 2022 3322 7d0d 0a20  height": "3"}.. 
-00001210: 2020 2020 2020 2029 0d0a 2020 2020 2020         )..      
-00001220: 2020 7265 7375 6c74 203d 206e 6577 5f73    result = new_s
-00001230: 7667 5f72 6f6f 7428 302c 2031 2c20 322c  vg_root(0, 1, 2,
-00001240: 2033 2c20 6174 7472 3d22 7661 6c75 6522   3, attr="value"
-00001250: 290d 0a20 2020 2020 2020 2061 7373 6572  )..        asser
-00001260: 7420 7265 7375 6c74 2e61 7474 7269 6220  t result.attrib 
-00001270: 3d3d 2065 7870 6563 742e 6174 7472 6962  == expect.attrib
-00001280: 0d0a 0d0a 2020 2020 6465 6620 7465 7374  ....    def test
-00001290: 5f63 6f6e 666c 6963 7469 6e67 5f70 6172  _conflicting_par
-000012a0: 616d 7328 7365 6c66 2920 2d3e 204e 6f6e  ams(self) -> Non
-000012b0: 653a 0d0a 2020 2020 2020 2020 2222 2220  e:..        """ 
-000012c0: 4578 706c 6963 6974 2070 6172 616d 7320  Explicit params 
-000012d0: 6f76 6572 7772 6974 6520 7472 6169 6c69  overwrite traili
-000012e0: 6e67 2d75 6e64 6572 7363 6f72 652d 696e  ng-underscore-in
-000012f0: 6665 7272 6564 2070 6172 616d 7320 2222  ferred params ""
-00001300: 220d 0a20 2020 2020 2020 2065 7870 6563  "..        expec
-00001310: 7420 3d20 7376 675f 726f 6f74 280d 0a20  t = svg_root(.. 
-00001320: 2020 2020 2020 2020 2020 202a 2a7b 2276             **{"v
-00001330: 6965 7742 6f78 223a 2022 3020 3120 3220  iewBox": "0 1 2 
-00001340: 3322 2c20 2277 6964 7468 223a 2022 3222  3", "width": "2"
-00001350: 2c20 2268 6569 6768 7422 3a20 2233 3022  , "height": "30"
-00001360: 7d0d 0a20 2020 2020 2020 2029 0d0a 2020  }..        )..  
-00001370: 2020 2020 2020 7265 7375 6c74 203d 206e        result = n
-00001380: 6577 5f73 7667 5f72 6f6f 7428 302c 2031  ew_svg_root(0, 1
-00001390: 2c20 322c 2033 2c20 6865 6967 6874 3d33  , 2, 3, height=3
-000013a0: 3029 0d0a 2020 2020 2020 2020 6173 7365  0)..        asse
-000013b0: 7274 2072 6573 756c 742e 6174 7472 6962  rt result.attrib
-000013c0: 203d 3d20 6578 7065 6374 2e61 7474 7269   == expect.attri
-000013d0: 620d 0a0d 0a0d 0a63 6c61 7373 2054 6573  b......class Tes
-000013e0: 7454 6f73 7472 696e 674b 7761 7267 733a  tTostringKwargs:
-000013f0: 0d0a 2020 2020 2222 2250 6173 7320 7772  ..    """Pass wr
-00001400: 6974 655f 7376 6720 2a2a 6b77 6172 6773  ite_svg **kwargs
-00001410: 2074 6f20 6c78 6d6c 2e65 7472 6565 2e74   to lxml.etree.t
-00001420: 6f73 7472 696e 6722 2222 0d0a 0d0a 2020  ostring"""....  
-00001430: 2020 6465 6620 7465 7374 5f6e 6f5f 6172    def test_no_ar
-00001440: 6773 2873 656c 6629 202d 3e20 4e6f 6e65  gs(self) -> None
-00001450: 3a0d 0a20 2020 2020 2020 2022 2222 5376  :..        """Sv
-00001460: 6720 636f 6e74 656e 7420 6f6e 6c79 2077  g content only w
-00001470: 6865 6e20 6e6f 2074 6f73 7472 696e 6720  hen no tostring 
-00001480: 6b77 6172 6773 2222 220d 0a20 2020 2020  kwargs"""..     
-00001490: 2020 2062 6c61 6e6b 203d 2065 7472 6565     blank = etree
-000014a0: 2e45 6c65 6d65 6e74 2822 626c 616e 6b22  .Element("blank"
-000014b0: 290d 0a20 2020 2020 2020 2061 7373 6572  )..        asser
-000014c0: 7420 7376 675f 746f 7374 7269 6e67 2862  t svg_tostring(b
-000014d0: 6c61 6e6b 2920 3d3d 2062 223c 626c 616e  lank) == b"<blan
-000014e0: 6b2f 3e5c 6e22 0d0a 0d0a 2020 2020 6465  k/>\n"....    de
-000014f0: 6620 7465 7374 5f64 6566 6175 6c74 2873  f test_default(s
-00001500: 656c 6629 202d 3e20 4e6f 6e65 3a0d 0a20  elf) -> None:.. 
-00001510: 2020 2020 2020 2022 2222 4465 6661 756c         """Defaul
-00001520: 7420 7061 7261 6d73 2077 6865 6e20 786d  t params when xm
-00001530: 6c5f 6465 636c 6172 6174 696f 6e20 6973  l_declaration is
-00001540: 2054 7275 6522 2222 0d0a 2020 2020 2020   True"""..      
-00001550: 2020 626c 616e 6b20 3d20 6574 7265 652e    blank = etree.
-00001560: 456c 656d 656e 7428 2262 6c61 6e6b 2229  Element("blank")
-00001570: 0d0a 2020 2020 2020 2020 6173 7365 7274  ..        assert
-00001580: 2073 7667 5f74 6f73 7472 696e 6728 626c   svg_tostring(bl
-00001590: 616e 6b2c 2078 6d6c 5f64 6563 6c61 7261  ank, xml_declara
-000015a0: 7469 6f6e 3d54 7275 6529 2e73 706c 6974  tion=True).split
-000015b0: 2862 225c 6e22 2920 3d3d 205b 0d0a 2020  (b"\n") == [..  
-000015c0: 2020 2020 2020 2020 2020 6222 3c3f 786d            b"<?xm
-000015d0: 6c20 7665 7273 696f 6e3d 2731 2e30 2720  l version='1.0' 
-000015e0: 656e 636f 6469 6e67 3d27 5554 462d 3827  encoding='UTF-8'
-000015f0: 3f3e 222c 0d0a 2020 2020 2020 2020 2020  ?>",..          
-00001600: 2020 6227 3c21 444f 4354 5950 4520 7376    b'<!DOCTYPE sv
-00001610: 6720 5055 424c 4943 2022 2d2f 2f57 3343  g PUBLIC "-//W3C
-00001620: 2f2f 4454 4420 5356 4720 312e 312f 2f45  //DTD SVG 1.1//E
-00001630: 4e22 272c 0d0a 2020 2020 2020 2020 2020  N"',..          
-00001640: 2020 6227 2268 7474 703a 2f2f 7777 772e    b'"http://www.
-00001650: 7733 2e6f 7267 2f47 7261 7068 6963 732f  w3.org/Graphics/
-00001660: 5356 472f 312e 312f 4454 442f 7376 6731  SVG/1.1/DTD/svg1
-00001670: 312e 6474 6422 3e27 2c0d 0a20 2020 2020  1.dtd">',..     
-00001680: 2020 2020 2020 2062 223c 626c 616e 6b2f         b"<blank/
-00001690: 3e22 2c0d 0a20 2020 2020 2020 2020 2020  >",..           
-000016a0: 2062 2222 2c0d 0a20 2020 2020 2020 205d   b"",..        ]
-000016b0: 0d0a 0d0a 2020 2020 6465 6620 7465 7374  ....    def test
-000016c0: 5f6f 7665 7272 6964 655f 646f 6374 7970  _override_doctyp
-000016d0: 6528 7365 6c66 2920 2d3e 204e 6f6e 653a  e(self) -> None:
-000016e0: 0d0a 2020 2020 2020 2020 2222 224f 7665  ..        """Ove
-000016f0: 7272 6964 6520 6465 6661 756c 7420 7061  rride default pa
-00001700: 7261 6d73 2222 220d 0a20 2020 2020 2020  rams"""..       
-00001710: 2062 6c61 6e6b 203d 2065 7472 6565 2e45   blank = etree.E
-00001720: 6c65 6d65 6e74 2822 626c 616e 6b22 290d  lement("blank").
-00001730: 0a20 2020 2020 2020 2072 6573 756c 7420  .        result 
-00001740: 3d20 7376 675f 746f 7374 7269 6e67 2862  = svg_tostring(b
-00001750: 6c61 6e6b 2c20 786d 6c5f 6465 636c 6172  lank, xml_declar
-00001760: 6174 696f 6e3d 5472 7565 2c20 646f 6374  ation=True, doct
-00001770: 7970 653d 4e6f 6e65 290d 0a20 2020 2020  ype=None)..     
-00001780: 2020 2061 7373 6572 7420 7265 7375 6c74     assert result
-00001790: 2e73 706c 6974 2862 225c 6e22 2920 3d3d  .split(b"\n") ==
-000017a0: 205b 0d0a 2020 2020 2020 2020 2020 2020   [..            
-000017b0: 6222 3c3f 786d 6c20 7665 7273 696f 6e3d  b"<?xml version=
-000017c0: 2731 2e30 2720 656e 636f 6469 6e67 3d27  '1.0' encoding='
-000017d0: 5554 462d 3827 3f3e 222c 0d0a 2020 2020  UTF-8'?>",..    
-000017e0: 2020 2020 2020 2020 6222 3c62 6c61 6e6b          b"<blank
-000017f0: 2f3e 222c 0d0a 2020 2020 2020 2020 2020  />",..          
-00001800: 2020 6222 222c 0d0a 2020 2020 2020 2020    b"",..        
-00001810: 5d0d 0a0d 0a20 2020 2064 6566 2074 6573  ]....    def tes
-00001820: 745f 6f76 6572 7269 6465 5f65 6e63 6f64  t_override_encod
-00001830: 696e 6728 7365 6c66 2920 2d3e 204e 6f6e  ing(self) -> Non
-00001840: 653a 0d0a 2020 2020 2020 2020 2222 2244  e:..        """D
-00001850: 6566 6175 6c74 2070 6172 616d 7320 7768  efault params wh
-00001860: 656e 2078 6d6c 5f64 6563 6c61 7261 7469  en xml_declarati
-00001870: 6f6e 2069 7320 5472 7565 2222 220d 0a20  on is True""".. 
-00001880: 2020 2020 2020 2062 6c61 6e6b 203d 2065         blank = e
-00001890: 7472 6565 2e45 6c65 6d65 6e74 2822 626c  tree.Element("bl
-000018a0: 616e 6b22 290d 0a20 2020 2020 2020 2072  ank")..        r
-000018b0: 6573 756c 7420 3d20 7376 675f 746f 7374  esult = svg_tost
-000018c0: 7269 6e67 2862 6c61 6e6b 2c20 786d 6c5f  ring(blank, xml_
-000018d0: 6465 636c 6172 6174 696f 6e3d 5472 7565  declaration=True
-000018e0: 2c20 656e 636f 6469 6e67 3d22 6173 6369  , encoding="asci
-000018f0: 6922 290d 0a20 2020 2020 2020 2061 7373  i")..        ass
-00001900: 6572 7420 7265 7375 6c74 2e73 706c 6974  ert result.split
-00001910: 2862 225c 6e22 2920 3d3d 205b 0d0a 2020  (b"\n") == [..  
-00001920: 2020 2020 2020 2020 2020 6222 3c3f 786d            b"<?xm
-00001930: 6c20 7665 7273 696f 6e3d 2731 2e30 2720  l version='1.0' 
-00001940: 656e 636f 6469 6e67 3d27 6173 6369 6927  encoding='ascii'
-00001950: 3f3e 222c 0d0a 2020 2020 2020 2020 2020  ?>",..          
-00001960: 2020 6227 3c21 444f 4354 5950 4520 7376    b'<!DOCTYPE sv
-00001970: 6720 5055 424c 4943 2022 2d2f 2f57 3343  g PUBLIC "-//W3C
-00001980: 2f2f 4454 4420 5356 4720 312e 312f 2f45  //DTD SVG 1.1//E
-00001990: 4e22 272c 0d0a 2020 2020 2020 2020 2020  N"',..          
-000019a0: 2020 6227 2268 7474 703a 2f2f 7777 772e    b'"http://www.
-000019b0: 7733 2e6f 7267 2f47 7261 7068 6963 732f  w3.org/Graphics/
-000019c0: 5356 472f 312e 312f 4454 442f 7376 6731  SVG/1.1/DTD/svg1
-000019d0: 312e 6474 6422 3e27 2c0d 0a20 2020 2020  1.dtd">',..     
-000019e0: 2020 2020 2020 2062 223c 626c 616e 6b2f         b"<blank/
-000019f0: 3e22 2c0d 0a20 2020 2020 2020 2020 2020  >",..           
-00001a00: 2062 2222 2c0d 0a20 2020 2020 2020 205d   b"",..        ]
-00001a10: 0d0a 0d0a                                ....
+00000190: 7261 6c69 6768 742e 6d61 696e 2069 6d70  ralight.main imp
+000001a0: 6f72 7420 6e65 775f 7376 675f 726f 6f74  ort new_svg_root
+000001b0: 2c20 7772 6974 655f 7376 670d 0a66 726f  , write_svg..fro
+000001c0: 6d20 7376 675f 756c 7472 616c 6967 6874  m svg_ultralight
+000001d0: 2069 6d70 6f72 7420 4e53 4d41 500d 0a66   import NSMAP..f
+000001e0: 726f 6d20 7376 675f 756c 7472 616c 6967  rom svg_ultralig
+000001f0: 6874 2e73 7472 696e 675f 636f 6e76 6572  ht.string_conver
+00000200: 7369 6f6e 2069 6d70 6f72 7420 7376 675f  sion import svg_
+00000210: 746f 7374 7269 6e67 0d0a 0d0a 0d0a 4070  tostring......@p
+00000220: 7974 6573 742e 6669 7874 7572 650d 0a64  ytest.fixture..d
+00000230: 6566 2063 7373 5f73 6f75 7263 6528 293a  ef css_source():
+00000240: 0d0a 2020 2020 2222 2254 656d 706f 7261  ..    """Tempora
+00000250: 7279 2063 7373 2066 696c 6520 6f62 6a65  ry css file obje
+00000260: 6374 2077 6974 6820 6d65 616e 696e 676c  ct with meaningl
+00000270: 6573 7320 636f 6e74 656e 7473 2e22 2222  ess contents."""
+00000280: 0d0a 2020 2020 7769 7468 2074 656d 7066  ..    with tempf
+00000290: 696c 652e 4e61 6d65 6454 656d 706f 7261  ile.NamedTempora
+000002a0: 7279 4669 6c65 286d 6f64 653d 2277 222c  ryFile(mode="w",
+000002b0: 2064 656c 6574 653d 4661 6c73 6529 2061   delete=False) a
+000002c0: 7320 6373 735f 736f 7572 6365 3a0d 0a20  s css_source:.. 
+000002d0: 2020 2020 2020 205f 203d 2063 7373 5f73         _ = css_s
+000002e0: 6f75 7263 652e 7772 6974 6528 222f 2a2a  ource.write("/**
+000002f0: 2063 7373 2066 6f72 206d 7920 7072 6f6a   css for my proj
+00000300: 6563 7420 2a2a 2f22 290d 0a20 2020 2079  ect **/")..    y
+00000310: 6965 6c64 2063 7373 5f73 6f75 7263 652e  ield css_source.
+00000320: 6e61 6d65 0d0a 2020 2020 6f73 2e75 6e6c  name..    os.unl
+00000330: 696e 6b28 6373 735f 736f 7572 6365 2e6e  ink(css_source.n
+00000340: 616d 6529 0d0a 0d0a 0d0a 4070 7974 6573  ame)......@pytes
+00000350: 742e 6669 7874 7572 650d 0a64 6566 2074  t.fixture..def t
+00000360: 656d 705f 6669 6c65 6e61 6d65 286d 6f64  emp_filename(mod
+00000370: 653a 7374 7220 3d22 7722 293a 0d0a 2020  e:str ="w"):..  
+00000380: 2020 2222 2254 656d 706f 7261 7279 2066    """Temporary f
+00000390: 696c 6520 6f62 6a65 6374 2074 6f20 6361  ile object to ca
+000003a0: 7074 7572 6520 7465 7374 206f 7574 7075  pture test outpu
+000003b0: 742e 2222 220d 0a20 2020 2073 7667 5f6f  t."""..    svg_o
+000003c0: 7574 7075 7420 3d20 7465 6d70 6669 6c65  utput = tempfile
+000003d0: 2e4e 616d 6564 5465 6d70 6f72 6172 7946  .NamedTemporaryF
+000003e0: 696c 6528 6d6f 6465 3d6d 6f64 652c 2064  ile(mode=mode, d
+000003f0: 656c 6574 653d 4661 6c73 6529 0d0a 2020  elete=False)..  
+00000400: 2020 7376 675f 6f75 7470 7574 2e63 6c6f    svg_output.clo
+00000410: 7365 2829 0d0a 2020 2020 7969 656c 6420  se()..    yield 
+00000420: 7376 675f 6f75 7470 7574 2e6e 616d 650d  svg_output.name.
+00000430: 0a20 2020 206f 732e 756e 6c69 6e6b 2873  .    os.unlink(s
+00000440: 7667 5f6f 7574 7075 742e 6e61 6d65 290d  vg_output.name).
+00000450: 0a0d 0a0d 0a63 6c61 7373 2054 6573 7457  .....class TestW
+00000460: 7269 7465 5376 673a 0d0a 2020 2020 6465  riteSvg:..    de
+00000470: 6620 7465 7374 5f6c 696e 6b65 6428 7365  f test_linked(se
+00000480: 6c66 2c20 6373 735f 736f 7572 6365 2c20  lf, css_source, 
+00000490: 7465 6d70 5f66 696c 656e 616d 6529 202d  temp_filename) -
+000004a0: 3e20 4e6f 6e65 3a0d 0a20 2020 2020 2020  > None:..       
+000004b0: 2022 2222 496e 7365 7274 2073 7479 6c65   """Insert style
+000004c0: 7368 6565 7420 7265 6665 7265 6e63 6522  sheet reference"
+000004d0: 2222 0d0a 2020 2020 2020 2020 626c 616e  ""..        blan
+000004e0: 6b20 3d20 6574 7265 652e 456c 656d 656e  k = etree.Elemen
+000004f0: 7428 2262 6c61 6e6b 2229 0d0a 2020 2020  t("blank")..    
+00000500: 2020 2020 7772 6974 655f 7376 6728 0d0a      write_svg(..
+00000510: 2020 2020 2020 2020 2020 2020 7465 6d70              temp
+00000520: 5f66 696c 656e 616d 652c 2062 6c61 6e6b  _filename, blank
+00000530: 2c20 6373 735f 736f 7572 6365 2c20 646f  , css_source, do
+00000540: 5f6c 696e 6b5f 6373 733d 5472 7565 2c20  _link_css=True, 
+00000550: 786d 6c5f 6465 636c 6172 6174 696f 6e3d  xml_declaration=
+00000560: 5472 7565 2c0d 0a20 2020 2020 2020 2029  True,..        )
+00000570: 0d0a 2020 2020 2020 2020 7769 7468 206f  ..        with o
+00000580: 7065 6e28 7465 6d70 5f66 696c 656e 616d  pen(temp_filenam
+00000590: 652c 2022 7262 2229 2061 7320 7376 675f  e, "rb") as svg_
+000005a0: 6269 6e61 7279 3a0d 0a20 2020 2020 2020  binary:..       
+000005b0: 2020 2020 2073 7667 5f6c 696e 6573 203d       svg_lines =
+000005c0: 205b 782e 6465 636f 6465 2829 2066 6f72   [x.decode() for
+000005d0: 2078 2069 6e20 7376 675f 6269 6e61 7279   x in svg_binary
+000005e0: 2e72 6561 646c 696e 6573 2829 5d0d 0a0d  .readlines()]...
+000005f0: 0a20 2020 2020 2020 2072 656c 6174 6976  .        relativ
+00000600: 655f 6373 735f 7061 7468 203d 2050 6174  e_css_path = Pat
+00000610: 6828 6373 735f 736f 7572 6365 292e 7265  h(css_source).re
+00000620: 6c61 7469 7665 5f74 6f28 5061 7468 2874  lative_to(Path(t
+00000630: 656d 705f 6669 6c65 6e61 6d65 292e 7061  emp_filename).pa
+00000640: 7265 6e74 290d 0a20 2020 2020 2020 2061  rent)..        a
+00000650: 7373 6572 7420 7376 675f 6c69 6e65 7320  ssert svg_lines 
+00000660: 3d3d 205b 0d0a 2020 2020 2020 2020 2020  == [..          
+00000670: 2020 223c 3f78 6d6c 2076 6572 7369 6f6e    "<?xml version
+00000680: 3d27 312e 3027 2065 6e63 6f64 696e 673d  ='1.0' encoding=
+00000690: 2755 5446 2d38 273f 3e5c 6e22 2c0d 0a20  'UTF-8'?>\n",.. 
+000006a0: 2020 2020 2020 2020 2020 2027 3c21 444f             '<!DO
+000006b0: 4354 5950 4520 7376 6720 5055 424c 4943  CTYPE svg PUBLIC
+000006c0: 2022 2d2f 2f57 3343 2f2f 4454 4420 5356   "-//W3C//DTD SV
+000006d0: 4720 312e 312f 2f45 4e22 5c6e 272c 0d0a  G 1.1//EN"\n',..
+000006e0: 2020 2020 2020 2020 2020 2020 2722 6874              '"ht
+000006f0: 7470 3a2f 2f77 7777 2e77 332e 6f72 672f  tp://www.w3.org/
+00000700: 4772 6170 6869 6373 2f53 5647 2f31 2e31  Graphics/SVG/1.1
+00000710: 2f44 5444 2f73 7667 3131 2e64 7464 223e  /DTD/svg11.dtd">
+00000720: 5c6e 272c 0d0a 2020 2020 2020 2020 2020  \n',..          
+00000730: 2020 6627 3c3f 786d 6c2d 7374 796c 6573    f'<?xml-styles
+00000740: 6865 6574 2068 7265 663d 227b 7265 6c61  heet href="{rela
+00000750: 7469 7665 5f63 7373 5f70 6174 687d 2220  tive_css_path}" 
+00000760: 7479 7065 3d22 7465 7874 2f63 7373 223f  type="text/css"?
+00000770: 3e5c 6e27 2c0d 0a20 2020 2020 2020 2020  >\n',..         
+00000780: 2020 2022 3c62 6c61 6e6b 2f3e 5c6e 222c     "<blank/>\n",
+00000790: 0d0a 2020 2020 2020 2020 5d0d 0a0d 0a20  ..        ].... 
+000007a0: 2020 2064 6566 2074 6573 745f 6e6f 745f     def test_not_
+000007b0: 6c69 6e6b 6564 2873 656c 662c 2063 7373  linked(self, css
+000007c0: 5f73 6f75 7263 652c 2074 656d 705f 6669  _source, temp_fi
+000007d0: 6c65 6e61 6d65 2920 2d3e 204e 6f6e 653a  lename) -> None:
+000007e0: 0d0a 2020 2020 2020 2020 2222 2243 6f70  ..        """Cop
+000007f0: 7920 6373 735f 736f 7572 6365 2063 6f6e  y css_source con
+00000800: 7465 6e74 7320 696e 746f 2073 7667 2066  tents into svg f
+00000810: 696c 6522 2222 0d0a 2020 2020 2020 2020  ile"""..        
+00000820: 626c 616e 6b20 3d20 6574 7265 652e 456c  blank = etree.El
+00000830: 656d 656e 7428 2262 6c61 6e6b 2229 0d0a  ement("blank")..
+00000840: 2020 2020 2020 2020 7772 6974 655f 7376          write_sv
+00000850: 6728 7465 6d70 5f66 696c 656e 616d 652c  g(temp_filename,
+00000860: 2062 6c61 6e6b 2c20 6373 735f 736f 7572   blank, css_sour
+00000870: 6365 290d 0a20 2020 2020 2020 2077 6974  ce)..        wit
+00000880: 6820 6f70 656e 2874 656d 705f 6669 6c65  h open(temp_file
+00000890: 6e61 6d65 2c20 2272 6222 2920 6173 2073  name, "rb") as s
+000008a0: 7667 5f62 696e 6172 793a 0d0a 2020 2020  vg_binary:..    
+000008b0: 2020 2020 2020 2020 7376 675f 6c69 6e65          svg_line
+000008c0: 7320 3d20 5b78 2e64 6563 6f64 6528 2920  s = [x.decode() 
+000008d0: 666f 7220 7820 696e 2073 7667 5f62 696e  for x in svg_bin
+000008e0: 6172 792e 7265 6164 6c69 6e65 7328 295d  ary.readlines()]
+000008f0: 0d0a 0d0a 2020 2020 2020 2020 6173 7365  ....        asse
+00000900: 7274 2073 7667 5f6c 696e 6573 203d 3d20  rt svg_lines == 
+00000910: 5b0d 0a20 2020 2020 2020 2020 2020 2022  [..            "
+00000920: 3c62 6c61 6e6b 3e5c 6e22 2c0d 0a20 2020  <blank>\n",..   
+00000930: 2020 2020 2020 2020 2027 2020 3c73 7479           '  <sty
+00000940: 6c65 2074 7970 653d 2274 6578 742f 6373  le type="text/cs
+00000950: 7322 3e3c 215b 4344 4154 415b 5c6e 272c  s"><![CDATA[\n',
+00000960: 0d0a 2020 2020 2020 2020 2020 2020 222f  ..            "/
+00000970: 2a2a 2063 7373 2066 6f72 206d 7920 7072  ** css for my pr
+00000980: 6f6a 6563 7420 2a2a 2f5c 6e22 2c0d 0a20  oject **/\n",.. 
+00000990: 2020 2020 2020 2020 2020 2022 5d5d 3e3c             "]]><
+000009a0: 2f73 7479 6c65 3e5c 6e22 2c0d 0a20 2020  /style>\n",..   
+000009b0: 2020 2020 2020 2020 2022 3c2f 626c 616e           "</blan
+000009c0: 6b3e 5c6e 222c 0d0a 2020 2020 2020 2020  k>\n",..        
+000009d0: 5d0d 0a0d 0a20 2020 2064 6566 2074 6573  ]....    def tes
+000009e0: 745f 6373 735f 6e6f 6e65 2873 656c 662c  t_css_none(self,
+000009f0: 2074 656d 705f 6669 6c65 6e61 6d65 2920   temp_filename) 
+00000a00: 2d3e 204e 6f6e 653a 0d0a 2020 2020 2020  -> None:..      
+00000a10: 2020 2222 2244 6f20 6e6f 7420 6c69 6e6b    """Do not link
+00000a20: 206f 7220 636f 7079 2069 6e20 6373 7320   or copy in css 
+00000a30: 6966 206e 6f20 6373 735f 736f 7572 6365  if no css_source
+00000a40: 2069 7320 7061 7373 6564 2e22 2222 0d0a   is passed."""..
+00000a50: 2020 2020 2020 2020 626c 616e 6b20 3d20          blank = 
+00000a60: 6574 7265 652e 456c 656d 656e 7428 2262  etree.Element("b
+00000a70: 6c61 6e6b 2229 0d0a 2020 2020 2020 2020  lank")..        
+00000a80: 7772 6974 655f 7376 6728 7465 6d70 5f66  write_svg(temp_f
+00000a90: 696c 656e 616d 652c 2062 6c61 6e6b 2c20  ilename, blank, 
+00000aa0: 646f 5f6c 696e 6b5f 6373 733d 5472 7565  do_link_css=True
+00000ab0: 290d 0a20 2020 2020 2020 2077 6974 6820  )..        with 
+00000ac0: 6f70 656e 2874 656d 705f 6669 6c65 6e61  open(temp_filena
+00000ad0: 6d65 2c20 2272 6222 2920 6173 2073 7667  me, "rb") as svg
+00000ae0: 5f62 696e 6172 793a 0d0a 2020 2020 2020  _binary:..      
+00000af0: 2020 2020 2020 7376 675f 6c69 6e65 7320        svg_lines 
+00000b00: 3d20 5b78 2e64 6563 6f64 6528 2920 666f  = [x.decode() fo
+00000b10: 7220 7820 696e 2073 7667 5f62 696e 6172  r x in svg_binar
+00000b20: 792e 7265 6164 6c69 6e65 7328 295d 0d0a  y.readlines()]..
+00000b30: 0d0a 2020 2020 2020 2020 6173 7365 7274  ..        assert
+00000b40: 2073 7667 5f6c 696e 6573 203d 3d20 5b0d   svg_lines == [.
+00000b50: 0a20 2020 2020 2020 2020 2020 2022 3c62  .            "<b
+00000b60: 6c61 6e6b 2f3e 5c6e 222c 0d0a 2020 2020  lank/>\n",..    
+00000b70: 2020 2020 5d0d 0a0d 0a20 2020 2020 2020      ]....       
+00000b80: 2023 2074 6573 7420 7769 7468 2064 6f5f   # test with do_
+00000b90: 6c69 6e6b 5f63 7373 203d 2046 616c 7365  link_css = False
+00000ba0: 0d0a 2020 2020 2020 2020 7772 6974 655f  ..        write_
+00000bb0: 7376 6728 7465 6d70 5f66 696c 656e 616d  svg(temp_filenam
+00000bc0: 652c 2062 6c61 6e6b 290d 0a20 2020 2020  e, blank)..     
+00000bd0: 2020 2077 6974 6820 6f70 656e 2874 656d     with open(tem
+00000be0: 705f 6669 6c65 6e61 6d65 2c20 2272 6222  p_filename, "rb"
+00000bf0: 2920 6173 2073 7667 5f62 696e 6172 793a  ) as svg_binary:
+00000c00: 0d0a 2020 2020 2020 2020 2020 2020 7376  ..            sv
+00000c10: 675f 6c69 6e65 735f 6661 6c73 6520 3d20  g_lines_false = 
+00000c20: 5b78 2e64 6563 6f64 6528 2920 666f 7220  [x.decode() for 
+00000c30: 7820 696e 2073 7667 5f62 696e 6172 792e  x in svg_binary.
+00000c40: 7265 6164 6c69 6e65 7328 295d 0d0a 2020  readlines()]..  
+00000c50: 2020 2020 2020 6173 7365 7274 2073 7667        assert svg
+00000c60: 5f6c 696e 6573 5f66 616c 7365 203d 3d20  _lines_false == 
+00000c70: 7376 675f 6c69 6e65 730d 0a0d 0a0d 0a64  svg_lines......d
+00000c80: 6566 2073 7667 5f72 6f6f 7428 2a2a 6b77  ef svg_root(**kw
+00000c90: 6172 6773 2920 2d3e 2065 7472 6565 2e45  args) -> etree.E
+00000ca0: 6c65 6d65 6e74 3a0d 0a20 2020 2022 2222  lement:..    """
+00000cb0: 0d0a 2020 2020 4372 6561 7465 2061 6e20  ..    Create an 
+00000cc0: 7376 6720 726f 6f74 2066 726f 6d20 6174  svg root from at
+00000cd0: 7472 6962 7574 6520 6b77 6172 6773 0d0a  tribute kwargs..
+00000ce0: 0d0a 2020 2020 3a70 6172 616d 206b 7761  ..    :param kwa
+00000cf0: 7267 733a 2065 7861 6374 2073 7667 2061  rgs: exact svg a
+00000d00: 7474 7269 6275 7465 206e 616d 6573 0d0a  ttribute names..
+00000d10: 2020 2020 3a72 6574 7572 6e3a 2061 2076      :return: a v
+00000d20: 616c 6964 2072 6f6f 7420 746f 2074 6573  alid root to tes
+00000d30: 7420 6167 6169 6e73 740d 0a0d 0a20 2020  t against....   
+00000d40: 2054 6865 2070 726f 6365 7373 2069 7320   The process is 
+00000d50: 7468 6973 3a0d 0a20 2020 202a 2063 7265  this:..    * cre
+00000d60: 6174 6520 6120 726f 6f74 2068 6572 6520  ate a root here 
+00000d70: 7769 7468 2065 7870 6c69 6369 7420 6174  with explicit at
+00000d80: 7472 6962 7574 6573 0d0a 2020 2020 2a20  tributes..    * 
+00000d90: 6372 6561 7465 2061 2072 6f6f 7420 7769  create a root wi
+00000da0: 7468 2061 2066 756e 6374 696f 6e20 7468  th a function th
+00000db0: 6174 2069 6e66 6572 7320 6578 706c 6963  at infers explic
+00000dc0: 6974 2061 7474 7269 6275 7465 730d 0a20  it attributes.. 
+00000dd0: 2020 202a 2063 6f6d 7061 7265 2072 6573     * compare res
+00000de0: 756c 7473 0d0a 2020 2020 2222 220d 0a20  ults..    """.. 
+00000df0: 2020 206e 616d 6573 7061 6365 203d 2074     namespace = t
+00000e00: 7570 6c65 284e 534d 4150 2e69 7465 6d73  uple(NSMAP.items
+00000e10: 2829 290d 0a20 2020 2078 6d6c 6e73 203d  ())..    xmlns =
+00000e20: 205b 6627 786d 6c6e 733d 227b 6e61 6d65   [f'xmlns="{name
+00000e30: 7370 6163 655b 305d 5b31 5d7d 2227 5d0d  space[0][1]}"'].
+00000e40: 0a20 2020 2078 6d6c 6e73 202b 3d20 5b66  .    xmlns += [f
+00000e50: 2778 6d6c 6e73 3a7b 6b7d 3d22 7b76 7d22  'xmlns:{k}="{v}"
+00000e60: 2720 666f 7220 6b2c 2076 2069 6e20 6e61  ' for k, v in na
+00000e70: 6d65 7370 6163 655b 313a 5d5d 0d0a 2020  mespace[1:]]..  
+00000e80: 2020 6174 7472 6962 7574 6573 203d 2027    attributes = '
+00000e90: 2027 2e6a 6f69 6e28 5b66 277b 6b7d 3d22   '.join([f'{k}="
+00000ea0: 7b76 7d22 2720 666f 7220 6b2c 2076 2069  {v}"' for k, v i
+00000eb0: 6e20 6b77 6172 6773 2e69 7465 6d73 2829  n kwargs.items()
+00000ec0: 5d29 0d0a 2020 2020 7265 7475 726e 2065  ])..    return e
+00000ed0: 7472 6565 2e66 726f 6d73 7472 696e 6728  tree.fromstring(
+00000ee0: 6627 3c73 7667 207b 2220 222e 6a6f 696e  f'<svg {" ".join
+00000ef0: 2878 6d6c 6e73 297d 207b 6174 7472 6962  (xmlns)} {attrib
+00000f00: 7574 6573 7d2f 3e27 2e65 6e63 6f64 6528  utes}/>'.encode(
+00000f10: 2929 0d0a 0d0a 0d0a 636c 6173 7320 5465  ))......class Te
+00000f20: 7374 4e65 7753 7667 526f 6f74 3a0d 0a20  stNewSvgRoot:.. 
+00000f30: 2020 2064 6566 2074 6573 745f 6e73 6d61     def test_nsma
+00000f40: 7028 7365 6c66 2920 2d3e 204e 6f6e 653a  p(self) -> None:
+00000f50: 0d0a 2020 2020 2020 2020 2222 2220 4e53  ..        """ NS
+00000f60: 4d41 5020 7061 7373 6564 2062 7920 6465  MAP passed by de
+00000f70: 6661 756c 7420 616e 6420 7061 7273 6561  fault and parsea
+00000f80: 626c 6520 6279 206c 786d 6c20 2222 220d  ble by lxml """.
+00000f90: 0a20 2020 2020 2020 2072 6573 756c 7420  .        result 
+00000fa0: 3d20 6e65 775f 7376 675f 726f 6f74 2829  = new_svg_root()
+00000fb0: 0d0a 2020 2020 2020 2020 6173 7365 7274  ..        assert
+00000fc0: 2072 6573 756c 742e 6e73 6d61 7020 3d3d   result.nsmap ==
+00000fd0: 204e 534d 4150 0d0a 0d0a 2020 2020 6465   NSMAP....    de
+00000fe0: 6620 7465 7374 5f61 7267 735f 7061 7373  f test_args_pass
+00000ff0: 2873 656c 6629 202d 3e20 4e6f 6e65 3a0d  (self) -> None:.
+00001000: 0a20 2020 2020 2020 2022 2222 4172 6775  .        """Argu
+00001010: 6d65 6e74 7320 616e 6420 786d 6c6e 7320  ments and xmlns 
+00001020: 6170 7065 6172 2069 6e20 656c 656d 656e  appear in elemen
+00001030: 742e 0d0a 0d0a 2020 2020 2020 2020 4275  t.....        Bu
+00001040: 696c 6420 7468 6520 7376 6720 656c 656d  ild the svg elem
+00001050: 656e 7420 6e61 6d65 7370 6163 6520 6672  ent namespace fr
+00001060: 6f6d 204e 534d 4150 2061 6e64 2063 6f6d  om NSMAP and com
+00001070: 7061 7265 2074 6f20 6f75 7470 7574 2222  pare to output""
+00001080: 220d 0a20 2020 2020 2020 2065 7870 6563  "..        expec
+00001090: 7420 3d20 7376 675f 726f 6f74 280d 0a20  t = svg_root(.. 
+000010a0: 2020 2020 2020 2020 2020 202a 2a7b 2276             **{"v
+000010b0: 6965 7742 6f78 223a 2022 3020 3120 3220  iewBox": "0 1 2 
+000010c0: 3322 2c20 2277 6964 7468 223a 2022 3222  3", "width": "2"
+000010d0: 2c20 2268 6569 6768 7422 3a20 2233 227d  , "height": "3"}
+000010e0: 0d0a 2020 2020 2020 2020 290d 0a20 2020  ..        )..   
+000010f0: 2020 2020 2072 6573 756c 7420 3d20 6e65       result = ne
+00001100: 775f 7376 675f 726f 6f74 2830 2c20 312c  w_svg_root(0, 1,
+00001110: 2032 2c20 3329 0d0a 2020 2020 2020 2020   2, 3)..        
+00001120: 6173 7365 7274 2072 6573 756c 742e 6174  assert result.at
+00001130: 7472 6962 203d 3d20 6578 7065 6374 2e61  trib == expect.a
+00001140: 7474 7269 620d 0a0d 0a20 2020 2064 6566  ttrib....    def
+00001150: 2074 6573 745f 6164 6469 7469 6f6e 616c   test_additional
+00001160: 5f70 6172 616d 7328 7365 6c66 2920 2d3e  _params(self) ->
+00001170: 204e 6f6e 653a 0d0a 2020 2020 2020 2020   None:..        
+00001180: 2222 2250 6173 7320 6164 6469 7469 6f6e  """Pass addition
+00001190: 616c 2070 6172 616d 7322 2222 0d0a 2020  al params"""..  
+000011a0: 2020 2020 2020 6578 7065 6374 203d 2073        expect = s
+000011b0: 7667 5f72 6f6f 7428 0d0a 2020 2020 2020  vg_root(..      
+000011c0: 2020 2020 2020 2a2a 7b22 6174 7472 223a        **{"attr":
+000011d0: 2022 7661 6c75 6522 2c20 2276 6965 7742   "value", "viewB
+000011e0: 6f78 223a 2022 3020 3120 3220 3322 2c20  ox": "0 1 2 3", 
+000011f0: 2277 6964 7468 223a 2022 3222 2c20 2268  "width": "2", "h
+00001200: 6569 6768 7422 3a20 2233 227d 0d0a 2020  eight": "3"}..  
+00001210: 2020 2020 2020 290d 0a20 2020 2020 2020        )..       
+00001220: 2072 6573 756c 7420 3d20 6e65 775f 7376   result = new_sv
+00001230: 675f 726f 6f74 2830 2c20 312c 2032 2c20  g_root(0, 1, 2, 
+00001240: 332c 2061 7474 723d 2276 616c 7565 2229  3, attr="value")
+00001250: 0d0a 2020 2020 2020 2020 6173 7365 7274  ..        assert
+00001260: 2072 6573 756c 742e 6174 7472 6962 203d   result.attrib =
+00001270: 3d20 6578 7065 6374 2e61 7474 7269 620d  = expect.attrib.
+00001280: 0a0d 0a20 2020 2064 6566 2074 6573 745f  ...    def test_
+00001290: 636f 6e66 6c69 6374 696e 675f 7061 7261  conflicting_para
+000012a0: 6d73 2873 656c 6629 202d 3e20 4e6f 6e65  ms(self) -> None
+000012b0: 3a0d 0a20 2020 2020 2020 2022 2222 2045  :..        """ E
+000012c0: 7870 6c69 6369 7420 7061 7261 6d73 206f  xplicit params o
+000012d0: 7665 7277 7269 7465 2074 7261 696c 696e  verwrite trailin
+000012e0: 672d 756e 6465 7273 636f 7265 2d69 6e66  g-underscore-inf
+000012f0: 6572 7265 6420 7061 7261 6d73 2022 2222  erred params """
+00001300: 0d0a 2020 2020 2020 2020 6578 7065 6374  ..        expect
+00001310: 203d 2073 7667 5f72 6f6f 7428 0d0a 2020   = svg_root(..  
+00001320: 2020 2020 2020 2020 2020 2a2a 7b22 7669            **{"vi
+00001330: 6577 426f 7822 3a20 2230 2031 2032 2033  ewBox": "0 1 2 3
+00001340: 222c 2022 7769 6474 6822 3a20 2232 222c  ", "width": "2",
+00001350: 2022 6865 6967 6874 223a 2022 3330 227d   "height": "30"}
+00001360: 0d0a 2020 2020 2020 2020 290d 0a20 2020  ..        )..   
+00001370: 2020 2020 2072 6573 756c 7420 3d20 6e65       result = ne
+00001380: 775f 7376 675f 726f 6f74 2830 2c20 312c  w_svg_root(0, 1,
+00001390: 2032 2c20 332c 2068 6569 6768 743d 3330   2, 3, height=30
+000013a0: 290d 0a0d 0a63 6c61 7373 2054 6573 7454  )....class TestT
+000013b0: 6f73 7472 696e 674b 7761 7267 733a 0d0a  ostringKwargs:..
+000013c0: 2020 2020 2222 2250 6173 7320 7772 6974      """Pass writ
+000013d0: 655f 7376 6720 2a2a 6b77 6172 6773 2074  e_svg **kwargs t
+000013e0: 6f20 6c78 6d6c 2e65 7472 6565 2e74 6f73  o lxml.etree.tos
+000013f0: 7472 696e 6722 2222 0d0a 0d0a 2020 2020  tring"""....    
+00001400: 6465 6620 7465 7374 5f6e 6f5f 6172 6773  def test_no_args
+00001410: 2873 656c 6629 202d 3e20 4e6f 6e65 3a0d  (self) -> None:.
+00001420: 0a20 2020 2020 2020 2022 2222 5376 6720  .        """Svg 
+00001430: 636f 6e74 656e 7420 6f6e 6c79 2077 6865  content only whe
+00001440: 6e20 6e6f 2074 6f73 7472 696e 6720 6b77  n no tostring kw
+00001450: 6172 6773 2222 220d 0a20 2020 2020 2020  args"""..       
+00001460: 2062 6c61 6e6b 203d 2065 7472 6565 2e45   blank = etree.E
+00001470: 6c65 6d65 6e74 2822 626c 616e 6b22 290d  lement("blank").
+00001480: 0a20 2020 2020 2020 2061 7373 6572 7420  .        assert 
+00001490: 7376 675f 746f 7374 7269 6e67 2862 6c61  svg_tostring(bla
+000014a0: 6e6b 2920 3d3d 2062 223c 626c 616e 6b2f  nk) == b"<blank/
+000014b0: 3e5c 6e22 0d0a 0d0a 2020 2020 6465 6620  >\n"....    def 
+000014c0: 7465 7374 5f64 6566 6175 6c74 2873 656c  test_default(sel
+000014d0: 6629 202d 3e20 4e6f 6e65 3a0d 0a20 2020  f) -> None:..   
+000014e0: 2020 2020 2022 2222 4465 6661 756c 7420       """Default 
+000014f0: 7061 7261 6d73 2077 6865 6e20 786d 6c5f  params when xml_
+00001500: 6465 636c 6172 6174 696f 6e20 6973 2054  declaration is T
+00001510: 7275 6522 2222 0d0a 2020 2020 2020 2020  rue"""..        
+00001520: 626c 616e 6b20 3d20 6574 7265 652e 456c  blank = etree.El
+00001530: 656d 656e 7428 2262 6c61 6e6b 2229 0d0a  ement("blank")..
+00001540: 2020 2020 2020 2020 6173 7365 7274 2073          assert s
+00001550: 7667 5f74 6f73 7472 696e 6728 626c 616e  vg_tostring(blan
+00001560: 6b2c 2078 6d6c 5f64 6563 6c61 7261 7469  k, xml_declarati
+00001570: 6f6e 3d54 7275 6529 2e73 706c 6974 2862  on=True).split(b
+00001580: 225c 6e22 2920 3d3d 205b 0d0a 2020 2020  "\n") == [..    
+00001590: 2020 2020 2020 2020 6222 3c3f 786d 6c20          b"<?xml 
+000015a0: 7665 7273 696f 6e3d 2731 2e30 2720 656e  version='1.0' en
+000015b0: 636f 6469 6e67 3d27 5554 462d 3827 3f3e  coding='UTF-8'?>
+000015c0: 222c 0d0a 2020 2020 2020 2020 2020 2020  ",..            
+000015d0: 6227 3c21 444f 4354 5950 4520 7376 6720  b'<!DOCTYPE svg 
+000015e0: 5055 424c 4943 2022 2d2f 2f57 3343 2f2f  PUBLIC "-//W3C//
+000015f0: 4454 4420 5356 4720 312e 312f 2f45 4e22  DTD SVG 1.1//EN"
+00001600: 272c 0d0a 2020 2020 2020 2020 2020 2020  ',..            
+00001610: 6227 2268 7474 703a 2f2f 7777 772e 7733  b'"http://www.w3
+00001620: 2e6f 7267 2f47 7261 7068 6963 732f 5356  .org/Graphics/SV
+00001630: 472f 312e 312f 4454 442f 7376 6731 312e  G/1.1/DTD/svg11.
+00001640: 6474 6422 3e27 2c0d 0a20 2020 2020 2020  dtd">',..       
+00001650: 2020 2020 2062 223c 626c 616e 6b2f 3e22       b"<blank/>"
+00001660: 2c0d 0a20 2020 2020 2020 2020 2020 2062  ,..            b
+00001670: 2222 2c0d 0a20 2020 2020 2020 205d 0d0a  "",..        ]..
+00001680: 0d0a 2020 2020 6465 6620 7465 7374 5f6f  ..    def test_o
+00001690: 7665 7272 6964 655f 646f 6374 7970 6528  verride_doctype(
+000016a0: 7365 6c66 2920 2d3e 204e 6f6e 653a 0d0a  self) -> None:..
+000016b0: 2020 2020 2020 2020 2222 224f 7665 7272          """Overr
+000016c0: 6964 6520 6465 6661 756c 7420 7061 7261  ide default para
+000016d0: 6d73 2222 220d 0a20 2020 2020 2020 2062  ms"""..        b
+000016e0: 6c61 6e6b 203d 2065 7472 6565 2e45 6c65  lank = etree.Ele
+000016f0: 6d65 6e74 2822 626c 616e 6b22 290d 0a20  ment("blank").. 
+00001700: 2020 2020 2020 2072 6573 756c 7420 3d20         result = 
+00001710: 7376 675f 746f 7374 7269 6e67 2862 6c61  svg_tostring(bla
+00001720: 6e6b 2c20 786d 6c5f 6465 636c 6172 6174  nk, xml_declarat
+00001730: 696f 6e3d 5472 7565 2c20 646f 6374 7970  ion=True, doctyp
+00001740: 653d 4e6f 6e65 290d 0a20 2020 2020 2020  e=None)..       
+00001750: 2061 7373 6572 7420 7265 7375 6c74 2e73   assert result.s
+00001760: 706c 6974 2862 225c 6e22 2920 3d3d 205b  plit(b"\n") == [
+00001770: 0d0a 2020 2020 2020 2020 2020 2020 6222  ..            b"
+00001780: 3c3f 786d 6c20 7665 7273 696f 6e3d 2731  <?xml version='1
+00001790: 2e30 2720 656e 636f 6469 6e67 3d27 5554  .0' encoding='UT
+000017a0: 462d 3827 3f3e 222c 0d0a 2020 2020 2020  F-8'?>",..      
+000017b0: 2020 2020 2020 6222 3c62 6c61 6e6b 2f3e        b"<blank/>
+000017c0: 222c 0d0a 2020 2020 2020 2020 2020 2020  ",..            
+000017d0: 6222 222c 0d0a 2020 2020 2020 2020 5d0d  b"",..        ].
+000017e0: 0a0d 0a20 2020 2064 6566 2074 6573 745f  ...    def test_
+000017f0: 6f76 6572 7269 6465 5f65 6e63 6f64 696e  override_encodin
+00001800: 6728 7365 6c66 2920 2d3e 204e 6f6e 653a  g(self) -> None:
+00001810: 0d0a 2020 2020 2020 2020 2222 2244 6566  ..        """Def
+00001820: 6175 6c74 2070 6172 616d 7320 7768 656e  ault params when
+00001830: 2078 6d6c 5f64 6563 6c61 7261 7469 6f6e   xml_declaration
+00001840: 2069 7320 5472 7565 2222 220d 0a20 2020   is True"""..   
+00001850: 2020 2020 2062 6c61 6e6b 203d 2065 7472       blank = etr
+00001860: 6565 2e45 6c65 6d65 6e74 2822 626c 616e  ee.Element("blan
+00001870: 6b22 290d 0a20 2020 2020 2020 2072 6573  k")..        res
+00001880: 756c 7420 3d20 7376 675f 746f 7374 7269  ult = svg_tostri
+00001890: 6e67 2862 6c61 6e6b 2c20 786d 6c5f 6465  ng(blank, xml_de
+000018a0: 636c 6172 6174 696f 6e3d 5472 7565 2c20  claration=True, 
+000018b0: 656e 636f 6469 6e67 3d22 6173 6369 6922  encoding="ascii"
+000018c0: 290d 0a20 2020 2020 2020 2061 7373 6572  )..        asser
+000018d0: 7420 7265 7375 6c74 2e73 706c 6974 2862  t result.split(b
+000018e0: 225c 6e22 2920 3d3d 205b 0d0a 2020 2020  "\n") == [..    
+000018f0: 2020 2020 2020 2020 6222 3c3f 786d 6c20          b"<?xml 
+00001900: 7665 7273 696f 6e3d 2731 2e30 2720 656e  version='1.0' en
+00001910: 636f 6469 6e67 3d27 6173 6369 6927 3f3e  coding='ascii'?>
+00001920: 222c 0d0a 2020 2020 2020 2020 2020 2020  ",..            
+00001930: 6227 3c21 444f 4354 5950 4520 7376 6720  b'<!DOCTYPE svg 
+00001940: 5055 424c 4943 2022 2d2f 2f57 3343 2f2f  PUBLIC "-//W3C//
+00001950: 4454 4420 5356 4720 312e 312f 2f45 4e22  DTD SVG 1.1//EN"
+00001960: 272c 0d0a 2020 2020 2020 2020 2020 2020  ',..            
+00001970: 6227 2268 7474 703a 2f2f 7777 772e 7733  b'"http://www.w3
+00001980: 2e6f 7267 2f47 7261 7068 6963 732f 5356  .org/Graphics/SV
+00001990: 472f 312e 312f 4454 442f 7376 6731 312e  G/1.1/DTD/svg11.
+000019a0: 6474 6422 3e27 2c0d 0a20 2020 2020 2020  dtd">',..       
+000019b0: 2020 2020 2062 223c 626c 616e 6b2f 3e22       b"<blank/>"
+000019c0: 2c0d 0a20 2020 2020 2020 2020 2020 2062  ,..            b
+000019d0: 2222 2c0d 0a20 2020 2020 2020 205d 0d0a  "",..        ]..
```

