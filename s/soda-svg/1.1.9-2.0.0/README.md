# Comparing `tmp/soda_svg-1.1.9.tar.gz` & `tmp/soda_svg-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "soda_svg-1.1.9.tar", max compression
+gzip compressed data, was "soda_svg-2.0.0.tar", max compression
```

## Comparing `soda_svg-1.1.9.tar` & `soda_svg-2.0.0.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0     1073 2023-04-26 16:43:52.177430 soda_svg-1.1.9/LICENSE
--rw-r--r--   0        0        0    13152 2023-04-26 16:43:52.177430 soda_svg-1.1.9/README.md
--rw-r--r--   0        0        0      515 2023-04-26 16:43:52.177430 soda_svg-1.1.9/pyproject.toml
--rw-r--r--   0        0        0      317 2023-04-26 16:43:52.177430 soda_svg-1.1.9/soda/__init__.py
--rw-r--r--   0        0        0      123 2023-04-26 16:43:52.177430 soda_svg-1.1.9/soda/config_mod.py
--rw-r--r--   0        0        0     2513 2023-04-26 16:43:52.177430 soda_svg-1.1.9/soda/custom_tags.py
--rw-r--r--   0        0        0     7357 2023-04-26 16:43:52.177430 soda_svg-1.1.9/soda/paths.py
--rw-r--r--   0        0        0    11689 2023-04-26 16:43:52.177430 soda_svg-1.1.9/soda/point.py
--rw-r--r--   0        0        0        0 2023-04-26 16:43:52.177430 soda_svg-1.1.9/soda/py.typed
--rw-r--r--   0        0        0    10460 2023-04-26 16:43:52.177430 soda_svg-1.1.9/soda/tags.py
--rw-r--r--   0        0        0     1838 2023-04-26 16:43:52.177430 soda_svg-1.1.9/soda/utils.py
--rw-r--r--   0        0        0      924 2023-04-26 16:43:52.177430 soda_svg-1.1.9/soda/xml_parse.py
--rw-r--r--   0        0        0    13838 1970-01-01 00:00:00.000000 soda_svg-1.1.9/PKG-INFO
+-rw-r--r--   0        0        0     1073 2024-05-04 19:00:10.210791 soda_svg-2.0.0/LICENSE
+-rw-r--r--   0        0        0    13304 2024-05-04 19:00:10.210791 soda_svg-2.0.0/README.md
+-rw-r--r--   0        0        0      633 2024-05-04 19:00:10.210791 soda_svg-2.0.0/pyproject.toml
+-rw-r--r--   0        0        0      317 2024-05-04 19:00:10.210791 soda_svg-2.0.0/soda/__init__.py
+-rw-r--r--   0        0        0      123 2024-05-04 19:00:10.210791 soda_svg-2.0.0/soda/config_mod.py
+-rw-r--r--   0        0        0     2489 2024-05-04 19:00:10.210791 soda_svg-2.0.0/soda/custom_tags.py
+-rw-r--r--   0        0        0     7357 2024-05-04 19:00:10.210791 soda_svg-2.0.0/soda/paths.py
+-rw-r--r--   0        0        0    11689 2024-05-04 19:00:10.210791 soda_svg-2.0.0/soda/point.py
+-rw-r--r--   0        0        0        0 2024-05-04 19:00:10.210791 soda_svg-2.0.0/soda/py.typed
+-rw-r--r--   0        0        0    11663 2024-05-04 19:00:10.210791 soda_svg-2.0.0/soda/tags.py
+-rw-r--r--   0        0        0     1838 2024-05-04 19:00:10.210791 soda_svg-2.0.0/soda/utils.py
+-rw-r--r--   0        0        0     1679 2024-05-04 19:00:10.210791 soda_svg-2.0.0/soda/xml_parse.py
+-rw-r--r--   0        0        0    14127 1970-01-01 00:00:00.000000 soda_svg-2.0.0/PKG-INFO
```

### Comparing `soda_svg-1.1.9/LICENSE` & `soda_svg-2.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `soda_svg-1.1.9/README.md` & `soda_svg-2.0.0/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -3,34 +3,44 @@
 [![GitHub Workflow Status](https://img.shields.io/github/actions/workflow/status/evtn/soda/build.yml?branch=lord)](https://github.com/evtn/soda/actions/workflows/build.yml)
 [![GitHub Workflow Status](https://img.shields.io/github/actions/workflow/status/evtn/soda/test.yml?branch=lord&label=tests)](https://github.com/evtn/soda/actions/workflows/test.yml)
 [![PyPI](https://img.shields.io/pypi/v/soda-svg)](https://pypi.org/project/soda-svg/)
 ![PyPI - Downloads](https://pepy.tech/badge/soda-svg)
 ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/soda-svg)
 [![Coveralls](https://img.shields.io/coverallsCoverage/github/evtn/soda?label=test%20coverage)](https://coveralls.io/github/evtn/soda?branch=lord)
 ![License](https://img.shields.io/github/license/evtn/soda)
-![Badge Count](https://img.shields.io/badge/badges-8-important)
-
+[![wordstreamer badge](https://img.shields.io/badge/renderable-what?label=wordstreamer&color=%2333bb33)](https://github.com/evtn/wordstreamer)
+![Badge Count](https://img.shields.io/badge/badges-9-important)
 
 Here's some basic usage:
 
+> [!NOTE]
+> Since soda 2.0.0, a Tag instance is also a [wordstreamer.Renderable](https://github.com/evtn/wordstreamer), which makes it possible to use things like:
+>
+> ```python
+> from wordstreamer import Renderer
+> from soda import Tag
+>
+> byte_stream = Renderer().byte_stream(Tag.rect()) # Iterable[bytes]
+> ```
+
 ```python
 from soda import Tag, Root
 
 # root is a custom svg tag
 root = Root(viewBox="0 0 10 10")(
     Tag.rect(width=10, height=10, fill="#ff5"),
     Tag.circle(cx=5, cy=5, r=4, fill="#222")
 )
 
 print(root.render(pretty=True))
 ```
 
 ## Installation
 
-Install `soda-svg` from PyPI, like `python -m pip install soda-svg`. 
+Install `soda-svg` from PyPI, like `python -m pip install soda-svg`.
 
 Note that `soda` on PyPI is a different package.
 
 ## Tag construction
 
 The main class of the module is `Tag`. You can create it with a constructor:
 
@@ -93,41 +103,41 @@
 ## Attribute conversion
 
 For convenience, leading and trailing underscores are removed by default, and underscores in the middle of words are replaced with hyphens:
 
 ```python
 from soda import Tag
 
-g = Tag.g(cla_ss_="test") 
+g = Tag.g(cla_ss_="test")
 
 print(g.render()) # <g cla-ss="test"/>
 
 ```
 
 To disable replacing behavior, use `config` class:
 
 ```python
 from soda import Tag, config as soda_config
 
 soda_config.replace_underscores = False
 
-g = Tag.g(cla_ss_="test") 
+g = Tag.g(cla_ss_="test")
 
 print(g.render()) # <g cla_ss="test"/>
 
 ```
 
 ...and to disable stripping of leading/traililng underscores:
 
 ```python
 from soda import Tag, config as soda_config
 
 soda_config.strip_underscores = False
 
-g = Tag.g(cla_ss_="test") 
+g = Tag.g(cla_ss_="test")
 
 print(g.render()) # <g cla-ss_="test"/>
 ```
 
 It's important to do that before tag creation, as all conversions are happening at the tag creation time:
 
 ```python
@@ -143,17 +153,17 @@
 print(g1.render()) # <g cla-ss="test"/>
 print(g2.render()) # <g cla_ss_="test"/>
 
 ```
 
 ## Creating a Tag from XML string
 
-*new in 1.1.0*
+_new in 1.1.0_
 
-You can use `Tag.from_str(xml_string)` to parse an XML document in that string.    
+You can use `Tag.from_str(xml_string)` to parse an XML document in that string.  
 Note that currently this doesn't preserve any comments or declarations of original document.
 
 ```python
 from soda import Tag, Root
 
 root = Root(viewBox="0 0 10 10")(
     Tag.rect(width=10, height=10, fill="#ff5"),
@@ -197,25 +207,23 @@
 
 
 print(XMLDeclaration(version="2.0", encoding="UTF-8").render()) # '<?xml version="2.0" encoding="UTF-8"?>'
 ```
 
 Default values for version and encoding are "1.0" and "UTF-8" respectively
 
-
 XML comments are used similarly:
 
 ```python
 from soda import XMLComment
 
 
 print(XMLComment("comment text!!").render()) # '<!-- comment text!! -->'
 ```
 
-
 ```python
 from soda import Tag, Literal
 
 Tag.g(Literal('<path d="M0 0 L10 0 Z"/>', escape=False))
 ```
 
 ## Accessing data
@@ -243,21 +251,20 @@
 print(tag[0]) # prints <a href="https://github.com/evtn/soda" />
 ```
 
 ~~Children can also be accessed directly through `tag.children` attribute.~~
 
 This is not necessary for most tasks as of 1.1.6 with new methods and iterator protocol:
 
-- `Tag.insert(int, Node)` inserts a node on an index. Be aware that `tag.children` is not flattened: `Tag.g("test", ["test1", "test2"]).insert(2, elem)` will insert `elem` *after* the array.
-- `Tag.append(Node)` appends one node to the tag.
-- `Tag.extend(*Node)` appends several nodes to the tag. *This is not the same as `.append([*Node])`*
-- `Tag.pop(int?)` pops one node from specified index. If index is not provided, pops the last one.
-- `Tag.iter_raw()` returns an iterable to get every Node of the tag. This doesn't dive into nested arrays, for that behaviour iterate over `Tag`
-- You can also iterate over the `Tag` itself to get every flat node of it (no arrays)
-
+-   `Tag.insert(int, Node)` inserts a node on an index. Be aware that `tag.children` is not flattened: `Tag.g("test", ["test1", "test2"]).insert(2, elem)` will insert `elem` _after_ the array.
+-   `Tag.append(Node)` appends one node to the tag.
+-   `Tag.extend(*Node)` appends several nodes to the tag. *This is not the same as `.append([*Node])`\*
+-   `Tag.pop(int?)` pops one node from specified index. If index is not provided, pops the last one.
+-   `Tag.iter_raw()` returns an iterable to get every Node of the tag. This doesn't dive into nested arrays, for that behaviour iterate over `Tag`
+-   You can also iterate over the `Tag` itself to get every flat node of it (no arrays)
 
 ## Fragments
 
 Fragments use concept similar to React's fragment. It renders just it's children:
 
 ```python
 from soda import Tag, Fragment
@@ -267,15 +274,15 @@
 )
 print(tag) # <g><a/><a/></g>
 
 ```
 
 ## Paths
 
-*new in 0.1.7*
+_new in 0.1.7_
 
 There is a builder for SVG path commands in soda:
 
 <svg viewBox="0 0 100 100">
     <rect width="100%" height="100%" fill="white"/>
     <path d="M 10,30
            A 20,20 0,0,1 50,30
@@ -385,15 +392,15 @@
 ```python
 print(Path.build(*commands, compact=True))
 # prints M10 30A20 20 0 0 1 50 30A20 20 0 0 1 50 30Q90 60 50 90Q10 60 10 30Z
 ```
 
 ## Points
 
-*new in 1.1.0*
+_new in 1.1.0_
 
 To work with coordinates, you can use `Point` class:
 
 ```python
 from soda import Point
 
 a = Point(1, 2)
@@ -460,26 +467,14 @@
 print(
     a.angle(
         a.rotate(radians=2)
     )
 ) # 2
 ```
 
-### Converting angles
-
-To convert between radians and degrees, use `radians_to_degrees` and `degrees_to_radians`:
-
-```python
-from soda.point import radians_to_degrees, degrees_to_radians
-from math import pi
-
-print(degrees_to_radians(90) / pi) # 0.5
-print(radians_to_degrees(degrees_to_radians(90))) # 90
-```
-
 ### Using as attributes
 
 `Point.as_` provides a convenient way of using points as tag attributes:
 
 ```python
 from soda import Tag, Point
```

### Comparing `soda_svg-1.1.9/soda/custom_tags.py` & `soda_svg-2.0.0/soda/custom_tags.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 from __future__ import annotations
 
 from base64 import b64encode
 from os import PathLike
-from typing import BinaryIO, Iterable
+from typing import BinaryIO
+
+from wordstreamer import Context, TokenStream
 from .tags import Literal, Node, Tag
 from pathlib import Path
 
 
 class Root(Tag):
     def __init__(
         self, *children: Node, use_namespace: bool = False, **attributes: Node
@@ -29,19 +31,18 @@
         super().__init__("xml", version=version, encoding=encoding)
 
 
 class XMLComment(Tag):
     def __init__(self, text: str):
         self.text = text
 
-    def build(self, tab_size: int = 0, tab_level: int = 0) -> Iterable[str]:
-        yield " " * (tab_size * tab_level)
+    def stream(self, context: Context) -> TokenStream:
         yield "<!--"
         yield " "
-        yield from Literal(self.text).build(0, 0)
+        yield from Literal(self.text).stream(context)
         yield " "
         yield "-->"
 
 
 class Image(Tag):
     """
```

### Comparing `soda_svg-1.1.9/soda/paths.py` & `soda_svg-2.0.0/soda/paths.py`

 * *Files identical despite different names*

### Comparing `soda_svg-1.1.9/soda/point.py` & `soda_svg-2.0.0/soda/point.py`

 * *Files identical despite different names*

### Comparing `soda_svg-1.1.9/soda/tags.py` & `soda_svg-2.0.0/soda/tags.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,20 +1,22 @@
 from __future__ import annotations
-from typing import Iterable, Iterator, Optional, Sequence, Union, overload
+from typing import Iterator, Optional, Sequence, Union, overload
+from wordstreamer import Renderable, Context, TokenStream
+from wordstreamer.stream_utils import separated
 
-FlatNode = Union["Tag", str, float]
+FlatNode = Union["Renderable", str, float]
 Node = Union[FlatNode, "list[Node]"]
 
 
 class MetaTag(type):
     def __getattr__(self, tag_name: str) -> Tag:
         return Tag(tag_name)
 
 
-class Tag(metaclass=MetaTag):
+class Tag(Renderable, metaclass=MetaTag):
     """
 
     Main class of the module, used to create tags.
 
     To create a simple `<tagname>` tag, use a shorthand: `Tag.tagname`.
 
     You can then call it to mutate its contents:
@@ -171,26 +173,35 @@
     def __repr__(self) -> str:
         return f"Tag<{self.tag_name} attributes: {len(self.attributes)}>children: {len(self.children)}</{self.tag_name}>"
 
     def __str__(self) -> str:
         return self.render()
 
     def build_child(
-        self, child: FlatNode, tab_size: int = 0, tab_level: int = 0
-    ) -> Iterable[str]:
+        self,
+        child: FlatNode,
+        context: Context,
+    ) -> TokenStream:
+        tab_level = self.get_tab_level(context) + 1
+        tab_size = self.get_tab_size(context)
+
         if isinstance(child, (float, int)):
-            yield from self.build_child(str(trunc(child)), tab_size, tab_level)
+            yield from self.build_child(str(trunc(child)), context)
             return
 
         if isinstance(child, str):
             yield " " * (tab_size * tab_level)
             yield escape(child)
+            return
 
-        else:
-            yield from child.build(tab_size, tab_level)
+        yield from child.stream(
+            context.derive(
+                tab_size=tab_size,
+            )
+        )
 
     def compare_attrs(self, other: Tag) -> bool:
         attrs1 = self.attributes
         attrs2 = other.attributes
 
         if attrs1.keys() ^ attrs2.keys():
             return False
@@ -229,17 +240,48 @@
 
         return (
             (self.tag_name == other.tag_name)
             and self.compare_attrs(other)
             and self.compare_children(other)
         )
 
-    def build(self, tab_size: int = 0, tab_level: int = 0) -> Iterable[str]:
+    def get_tab_size(self, context: Context) -> int:
+        tab_size = context.tab_size
+
+        if not isinstance(tab_size, int):
+            return 0
+
+        return tab_size
+
+    def get_tab_level(self, context: Context) -> int:
+        tab_level = context.tab_level
+
+        if not isinstance(tab_level, int):
+            return 0
+
+        return tab_level
+
+    def is_pretty(self, context: Context) -> bool:
+        tab_size = self.get_tab_size(context)
+
+        if not tab_size:
+            return False
+
+        return context.pretty is True
+
+    def build(self, context: Context) -> TokenStream:
+        """alias for Tag.stream for some compatibility with 1.x (not full since TokenStream != Iterable[str])"""
+        return self.stream(context)
+
+    def stream(self, context: Context) -> TokenStream:
+        tab_size = self.get_tab_size(context)
+        tab_level = self.get_tab_level(context)
+
         tag_name = self.tag_name
-        pretty = bool(tab_size)
+        pretty = self.is_pretty(context)
 
         tab = " " * tab_size
         tag_indent = " " * (tab_size * tab_level)
         separator = "\n" * pretty
         attr_space = "\n" if pretty else " "
         quote = '"'
 
@@ -271,28 +313,33 @@
             yield from newline_indented
 
         if self.children or not self.self_closing:
             yield self.brackets[2]  # >
 
         for child in self:
             yield separator
-            yield from self.build_child(child, tab_size, tab_level + 1)
+            yield from self.build_child(child, context)
 
         if self.children:
             yield from newline_indented
 
         if self.children or not self.self_closing:
             yield self.brackets[1]  # </
             yield tag_name
             yield self.brackets[2]  # >
         else:
             yield self.brackets[3]  # />
 
     def render(self, pretty: bool = False, tab_size: int = 2) -> str:
-        return "".join(self.build(tab_size * pretty))
+        return self.render_string(
+            {
+                "pretty": pretty,
+                "tab_size": tab_size * pretty,
+            }
+        )
 
     def prerender(self, pretty: bool = False) -> Literal:
         """Renders a tag into a non-escaping literal. Could speed up rendering of heavy tags."""
         return Literal(self.render(pretty), escape=False)
 
     @staticmethod
     def from_str(text: str) -> Tag:
@@ -306,16 +353,16 @@
         self.attributes = {}
         self.escape = escape
 
     def copy(self) -> Literal:
         assert isinstance(self.children[0], str)
         return Literal(self.children[0], self.escape)
 
-    def build(self, tab_size: int = 0, tab_level: int = 0) -> Iterable[str]:
-        separator = "\n" * bool(tab_size)
+    def stream(self, context: Context) -> TokenStream:
+        separator = "\n" * bool(self.is_pretty(context))
 
         for child in self.children:
             yield separator
 
             contents = str(child)
 
             if self.escape:
@@ -332,21 +379,23 @@
 
 class Fragment(Tag):
     """React-like fragment, renders just its children"""
 
     def __init__(self, *children: Node):
         super().__init__("soda:fragment", *children)
 
-    def build(self, tab_size: int = 0, tab_level: int = 0) -> Iterable[str]:
+    def build_children(self, context) -> TokenStream:
         for child in self:
-            yield from self.build_child(child, tab_size, tab_level)
+            yield from self.build_child(child, context)
 
-    def render(self, pretty: bool = False, tab_size: int = 2) -> str:
-        sep = "\n" * pretty
-        return sep.join(self.build(tab_size * pretty))
+    def stream(self, context: Context) -> TokenStream:
+        return separated(
+            *[self.build_child(child, context) for child in self],
+            separator="\n" * self.is_pretty(context),
+        )
 
     def copy(self) -> Fragment:
         return Fragment(*self.children)
 
 
 from .xml_parse import xml_to_tag
 from .utils import escape, node_iterator, normalize_ident, trunc
```

### Comparing `soda_svg-1.1.9/soda/utils.py` & `soda_svg-2.0.0/soda/utils.py`

 * *Files identical despite different names*

### Comparing `soda_svg-1.1.9/PKG-INFO` & `soda_svg-2.0.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,56 +1,69 @@
 Metadata-Version: 2.1
 Name: soda-svg
-Version: 1.1.9
+Version: 2.0.0
 Summary: Fast SVG generation tool
 Home-page: https://github.com/evtn/soda
 License: MIT
 Keywords: soda,svg,xml
 Author: Dmitry Gritsenko
 Author-email: soda@evtn.ru
-Requires-Python: >=3.7.0
+Requires-Python: >=3.8,<3.13
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
+Requires-Dist: lxml (>=5.2.1,<6.0.0)
+Requires-Dist: types-lxml (>=2024.4.14,<2025.0.0)
+Requires-Dist: wordstreamer (>=0.1.3,<0.2.0)
 Project-URL: Repository, https://github.com/evtn/soda
 Description-Content-Type: text/markdown
 
 # soda - a fast SVG generation tool
 
 [![GitHub Workflow Status](https://img.shields.io/github/actions/workflow/status/evtn/soda/build.yml?branch=lord)](https://github.com/evtn/soda/actions/workflows/build.yml)
 [![GitHub Workflow Status](https://img.shields.io/github/actions/workflow/status/evtn/soda/test.yml?branch=lord&label=tests)](https://github.com/evtn/soda/actions/workflows/test.yml)
 [![PyPI](https://img.shields.io/pypi/v/soda-svg)](https://pypi.org/project/soda-svg/)
 ![PyPI - Downloads](https://pepy.tech/badge/soda-svg)
 ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/soda-svg)
 [![Coveralls](https://img.shields.io/coverallsCoverage/github/evtn/soda?label=test%20coverage)](https://coveralls.io/github/evtn/soda?branch=lord)
 ![License](https://img.shields.io/github/license/evtn/soda)
-![Badge Count](https://img.shields.io/badge/badges-8-important)
-
+[![wordstreamer badge](https://img.shields.io/badge/renderable-what?label=wordstreamer&color=%2333bb33)](https://github.com/evtn/wordstreamer)
+![Badge Count](https://img.shields.io/badge/badges-9-important)
 
 Here's some basic usage:
 
+> [!NOTE]
+> Since soda 2.0.0, a Tag instance is also a [wordstreamer.Renderable](https://github.com/evtn/wordstreamer), which makes it possible to use things like:
+>
+> ```python
+> from wordstreamer import Renderer
+> from soda import Tag
+>
+> byte_stream = Renderer().byte_stream(Tag.rect()) # Iterable[bytes]
+> ```
+
 ```python
 from soda import Tag, Root
 
 # root is a custom svg tag
 root = Root(viewBox="0 0 10 10")(
     Tag.rect(width=10, height=10, fill="#ff5"),
     Tag.circle(cx=5, cy=5, r=4, fill="#222")
 )
 
 print(root.render(pretty=True))
 ```
 
 ## Installation
 
-Install `soda-svg` from PyPI, like `python -m pip install soda-svg`. 
+Install `soda-svg` from PyPI, like `python -m pip install soda-svg`.
 
 Note that `soda` on PyPI is a different package.
 
 ## Tag construction
 
 The main class of the module is `Tag`. You can create it with a constructor:
 
@@ -113,41 +126,41 @@
 ## Attribute conversion
 
 For convenience, leading and trailing underscores are removed by default, and underscores in the middle of words are replaced with hyphens:
 
 ```python
 from soda import Tag
 
-g = Tag.g(cla_ss_="test") 
+g = Tag.g(cla_ss_="test")
 
 print(g.render()) # <g cla-ss="test"/>
 
 ```
 
 To disable replacing behavior, use `config` class:
 
 ```python
 from soda import Tag, config as soda_config
 
 soda_config.replace_underscores = False
 
-g = Tag.g(cla_ss_="test") 
+g = Tag.g(cla_ss_="test")
 
 print(g.render()) # <g cla_ss="test"/>
 
 ```
 
 ...and to disable stripping of leading/traililng underscores:
 
 ```python
 from soda import Tag, config as soda_config
 
 soda_config.strip_underscores = False
 
-g = Tag.g(cla_ss_="test") 
+g = Tag.g(cla_ss_="test")
 
 print(g.render()) # <g cla-ss_="test"/>
 ```
 
 It's important to do that before tag creation, as all conversions are happening at the tag creation time:
 
 ```python
@@ -163,17 +176,17 @@
 print(g1.render()) # <g cla-ss="test"/>
 print(g2.render()) # <g cla_ss_="test"/>
 
 ```
 
 ## Creating a Tag from XML string
 
-*new in 1.1.0*
+_new in 1.1.0_
 
-You can use `Tag.from_str(xml_string)` to parse an XML document in that string.    
+You can use `Tag.from_str(xml_string)` to parse an XML document in that string.  
 Note that currently this doesn't preserve any comments or declarations of original document.
 
 ```python
 from soda import Tag, Root
 
 root = Root(viewBox="0 0 10 10")(
     Tag.rect(width=10, height=10, fill="#ff5"),
@@ -217,25 +230,23 @@
 
 
 print(XMLDeclaration(version="2.0", encoding="UTF-8").render()) # '<?xml version="2.0" encoding="UTF-8"?>'
 ```
 
 Default values for version and encoding are "1.0" and "UTF-8" respectively
 
-
 XML comments are used similarly:
 
 ```python
 from soda import XMLComment
 
 
 print(XMLComment("comment text!!").render()) # '<!-- comment text!! -->'
 ```
 
-
 ```python
 from soda import Tag, Literal
 
 Tag.g(Literal('<path d="M0 0 L10 0 Z"/>', escape=False))
 ```
 
 ## Accessing data
@@ -263,21 +274,20 @@
 print(tag[0]) # prints <a href="https://github.com/evtn/soda" />
 ```
 
 ~~Children can also be accessed directly through `tag.children` attribute.~~
 
 This is not necessary for most tasks as of 1.1.6 with new methods and iterator protocol:
 
-- `Tag.insert(int, Node)` inserts a node on an index. Be aware that `tag.children` is not flattened: `Tag.g("test", ["test1", "test2"]).insert(2, elem)` will insert `elem` *after* the array.
-- `Tag.append(Node)` appends one node to the tag.
-- `Tag.extend(*Node)` appends several nodes to the tag. *This is not the same as `.append([*Node])`*
-- `Tag.pop(int?)` pops one node from specified index. If index is not provided, pops the last one.
-- `Tag.iter_raw()` returns an iterable to get every Node of the tag. This doesn't dive into nested arrays, for that behaviour iterate over `Tag`
-- You can also iterate over the `Tag` itself to get every flat node of it (no arrays)
-
+-   `Tag.insert(int, Node)` inserts a node on an index. Be aware that `tag.children` is not flattened: `Tag.g("test", ["test1", "test2"]).insert(2, elem)` will insert `elem` _after_ the array.
+-   `Tag.append(Node)` appends one node to the tag.
+-   `Tag.extend(*Node)` appends several nodes to the tag. *This is not the same as `.append([*Node])`\*
+-   `Tag.pop(int?)` pops one node from specified index. If index is not provided, pops the last one.
+-   `Tag.iter_raw()` returns an iterable to get every Node of the tag. This doesn't dive into nested arrays, for that behaviour iterate over `Tag`
+-   You can also iterate over the `Tag` itself to get every flat node of it (no arrays)
 
 ## Fragments
 
 Fragments use concept similar to React's fragment. It renders just it's children:
 
 ```python
 from soda import Tag, Fragment
@@ -287,15 +297,15 @@
 )
 print(tag) # <g><a/><a/></g>
 
 ```
 
 ## Paths
 
-*new in 0.1.7*
+_new in 0.1.7_
 
 There is a builder for SVG path commands in soda:
 
 <svg viewBox="0 0 100 100">
     <rect width="100%" height="100%" fill="white"/>
     <path d="M 10,30
            A 20,20 0,0,1 50,30
@@ -405,15 +415,15 @@
 ```python
 print(Path.build(*commands, compact=True))
 # prints M10 30A20 20 0 0 1 50 30A20 20 0 0 1 50 30Q90 60 50 90Q10 60 10 30Z
 ```
 
 ## Points
 
-*new in 1.1.0*
+_new in 1.1.0_
 
 To work with coordinates, you can use `Point` class:
 
 ```python
 from soda import Point
 
 a = Point(1, 2)
@@ -480,26 +490,14 @@
 print(
     a.angle(
         a.rotate(radians=2)
     )
 ) # 2
 ```
 
-### Converting angles
-
-To convert between radians and degrees, use `radians_to_degrees` and `degrees_to_radians`:
-
-```python
-from soda.point import radians_to_degrees, degrees_to_radians
-from math import pi
-
-print(degrees_to_radians(90) / pi) # 0.5
-print(radians_to_degrees(degrees_to_radians(90))) # 90
-```
-
 ### Using as attributes
 
 `Point.as_` provides a convenient way of using points as tag attributes:
 
 ```python
 from soda import Tag, Point
```

