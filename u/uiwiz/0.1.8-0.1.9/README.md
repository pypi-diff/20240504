# Comparing `tmp/uiwiz-0.1.8.tar.gz` & `tmp/uiwiz-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "uiwiz-0.1.8.tar", max compression
+gzip compressed data, was "uiwiz-0.1.9.tar", max compression
```

## Comparing `uiwiz-0.1.8.tar` & `uiwiz-0.1.9.tar`

### file list

```diff
@@ -1,52 +1,52 @@
--rw-r--r--   0        0        0     1075 2024-01-17 20:38:36.584157 uiwiz-0.1.8/LICENSE
--rw-r--r--   0        0        0     1417 2024-01-17 20:38:36.584157 uiwiz-0.1.8/README.md
--rw-r--r--   0        0        0      669 2024-01-17 20:38:47.248183 uiwiz-0.1.8/pyproject.toml
--rw-r--r--   0        0        0      126 2024-01-17 20:38:36.584157 uiwiz-0.1.8/uiwiz/__init__.py
--rw-r--r--   0        0        0     6791 2024-01-17 20:38:36.584157 uiwiz-0.1.8/uiwiz/app.py
--rw-r--r--   0        0        0     8932 2024-01-17 20:38:36.584157 uiwiz-0.1.8/uiwiz/element.py
--rw-r--r--   0        0        0        0 2024-01-17 20:38:36.584157 uiwiz-0.1.8/uiwiz/elements/__init__.py
--rw-r--r--   0        0        0     1569 2024-01-17 20:38:36.584157 uiwiz-0.1.8/uiwiz/elements/aggrid.js
--rw-r--r--   0        0        0     1790 2024-01-17 20:38:36.584157 uiwiz-0.1.8/uiwiz/elements/aggrid.py
--rw-r--r--   0        0        0      583 2024-01-17 20:38:36.584157 uiwiz-0.1.8/uiwiz/elements/avatar.py
--rw-r--r--   0        0        0      881 2024-01-17 20:38:36.584157 uiwiz-0.1.8/uiwiz/elements/button.py
--rw-r--r--   0        0        0      377 2024-01-17 20:38:36.584157 uiwiz-0.1.8/uiwiz/elements/checkbox.py
--rw-r--r--   0        0        0      416 2024-01-17 20:38:36.584157 uiwiz-0.1.8/uiwiz/elements/code.py
--rw-r--r--   0        0        0      163 2024-01-17 20:38:36.584157 uiwiz-0.1.8/uiwiz/elements/col.py
--rw-r--r--   0        0        0      417 2024-01-17 20:38:36.584157 uiwiz-0.1.8/uiwiz/elements/datepicker.py
--rw-r--r--   0        0        0      363 2024-01-17 20:38:36.584157 uiwiz-0.1.8/uiwiz/elements/divider.py
--rw-r--r--   0        0        0     1800 2024-01-17 20:38:36.584157 uiwiz-0.1.8/uiwiz/elements/drawer.py
--rw-r--r--   0        0        0      530 2024-01-17 20:38:36.584157 uiwiz-0.1.8/uiwiz/elements/dropdown.py
--rw-r--r--   0        0        0      717 2024-01-17 20:38:36.584157 uiwiz-0.1.8/uiwiz/elements/extensions/bindable.py
--rw-r--r--   0        0        0      273 2024-01-17 20:38:36.584157 uiwiz-0.1.8/uiwiz/elements/footer.py
--rw-r--r--   0        0        0      483 2024-01-17 20:38:36.584157 uiwiz-0.1.8/uiwiz/elements/form.py
--rw-r--r--   0        0        0      156 2024-01-17 20:38:36.584157 uiwiz-0.1.8/uiwiz/elements/html.py
--rw-r--r--   0        0        0     1267 2024-01-17 20:38:36.584157 uiwiz-0.1.8/uiwiz/elements/input.py
--rw-r--r--   0        0        0      563 2024-01-17 20:38:36.584157 uiwiz-0.1.8/uiwiz/elements/label.py
--rw-r--r--   0        0        0      308 2024-01-17 20:38:36.584157 uiwiz-0.1.8/uiwiz/elements/link.py
--rw-r--r--   0        0        0      619 2024-01-17 20:38:36.584157 uiwiz-0.1.8/uiwiz/elements/markdown.py
--rw-r--r--   0        0        0      224 2024-01-17 20:38:36.584157 uiwiz-0.1.8/uiwiz/elements/nav.py
--rw-r--r--   0        0        0      313 2024-01-17 20:38:36.584157 uiwiz-0.1.8/uiwiz/elements/radio.py
--rw-r--r--   0        0        0      738 2024-01-17 20:38:36.584157 uiwiz-0.1.8/uiwiz/elements/range.py
--rw-r--r--   0        0        0      169 2024-01-17 20:38:36.584157 uiwiz-0.1.8/uiwiz/elements/row.py
--rw-r--r--   0        0        0     2166 2024-01-17 20:38:36.584157 uiwiz-0.1.8/uiwiz/elements/spinner.py
--rw-r--r--   0        0        0      956 2024-01-17 20:38:36.584157 uiwiz-0.1.8/uiwiz/elements/table.py
--rw-r--r--   0        0        0     1433 2024-01-17 20:38:36.584157 uiwiz-0.1.8/uiwiz/elements/tabs.py
--rw-r--r--   0        0        0      945 2024-01-17 20:38:36.584157 uiwiz-0.1.8/uiwiz/elements/textarea.py
--rw-r--r--   0        0        0     1882 2024-01-17 20:38:36.584157 uiwiz-0.1.8/uiwiz/elements/toast.py
--rw-r--r--   0        0        0      373 2024-01-17 20:38:36.584157 uiwiz-0.1.8/uiwiz/elements/toggle.py
--rw-r--r--   0        0        0      818 2024-01-17 20:38:36.584157 uiwiz-0.1.8/uiwiz/elements/upload.py
--rw-r--r--   0        0        0      240 2024-01-17 20:38:36.584157 uiwiz-0.1.8/uiwiz/event.py
--rw-r--r--   0        0        0      825 2024-01-17 20:38:36.584157 uiwiz-0.1.8/uiwiz/header_middelware.py
--rw-r--r--   0        0        0      397 2024-01-17 20:38:36.588157 uiwiz-0.1.8/uiwiz/static/app.css
--rw-r--r--   0        0        0     2752 2024-01-17 20:38:36.588157 uiwiz-0.1.8/uiwiz/static/codehighlight.css
--rw-r--r--   0        0        0  1737043 2024-01-17 20:38:36.592157 uiwiz-0.1.8/uiwiz/static/libs/aggrid-community.min.js
--rw-r--r--   0        0        0    30661 2024-01-17 20:38:36.592157 uiwiz-0.1.8/uiwiz/static/markdown.css
--rw-r--r--   0        0        0      281 2024-01-17 20:38:36.592157 uiwiz-0.1.8/uiwiz/svg/error.svg
--rw-r--r--   0        0        0      272 2024-01-17 20:38:36.592157 uiwiz-0.1.8/uiwiz/svg/info.svg
--rw-r--r--   0        0        0      245 2024-01-17 20:38:36.592157 uiwiz-0.1.8/uiwiz/svg/menu.svg
--rw-r--r--   0        0        0      258 2024-01-17 20:38:36.592157 uiwiz-0.1.8/uiwiz/svg/success.svg
--rw-r--r--   0        0        0      308 2024-01-17 20:38:36.592157 uiwiz-0.1.8/uiwiz/svg/svg_handler.py
--rw-r--r--   0        0        0      345 2024-01-17 20:38:36.592157 uiwiz-0.1.8/uiwiz/svg/warning.svg
--rw-r--r--   0        0        0     2950 2024-01-17 20:38:36.592157 uiwiz-0.1.8/uiwiz/templates/default.html
--rw-r--r--   0        0        0     1483 2024-01-17 20:38:36.592157 uiwiz-0.1.8/uiwiz/ui.py
--rw-r--r--   0        0        0     2147 1970-01-01 00:00:00.000000 uiwiz-0.1.8/PKG-INFO
+-rw-r--r--   0        0        0     1075 2024-01-22 20:49:01.320519 uiwiz-0.1.9/LICENSE
+-rw-r--r--   0        0        0     1417 2024-01-22 20:49:01.320519 uiwiz-0.1.9/README.md
+-rw-r--r--   0        0        0      669 2024-01-22 20:49:12.016656 uiwiz-0.1.9/pyproject.toml
+-rw-r--r--   0        0        0      126 2024-01-22 20:49:01.320519 uiwiz-0.1.9/uiwiz/__init__.py
+-rw-r--r--   0        0        0     7050 2024-01-22 20:49:01.320519 uiwiz-0.1.9/uiwiz/app.py
+-rw-r--r--   0        0        0     8914 2024-01-22 20:49:01.320519 uiwiz-0.1.9/uiwiz/element.py
+-rw-r--r--   0        0        0        0 2024-01-22 20:49:01.320519 uiwiz-0.1.9/uiwiz/elements/__init__.py
+-rw-r--r--   0        0        0     1578 2024-01-22 20:49:01.320519 uiwiz-0.1.9/uiwiz/elements/aggrid.js
+-rw-r--r--   0        0        0     1790 2024-01-22 20:49:01.320519 uiwiz-0.1.9/uiwiz/elements/aggrid.py
+-rw-r--r--   0        0        0      583 2024-01-22 20:49:01.320519 uiwiz-0.1.9/uiwiz/elements/avatar.py
+-rw-r--r--   0        0        0      646 2024-01-22 20:49:01.320519 uiwiz-0.1.9/uiwiz/elements/button.py
+-rw-r--r--   0        0        0      377 2024-01-22 20:49:01.320519 uiwiz-0.1.9/uiwiz/elements/checkbox.py
+-rw-r--r--   0        0        0      416 2024-01-22 20:49:01.320519 uiwiz-0.1.9/uiwiz/elements/code.py
+-rw-r--r--   0        0        0      163 2024-01-22 20:49:01.320519 uiwiz-0.1.9/uiwiz/elements/col.py
+-rw-r--r--   0        0        0      417 2024-01-22 20:49:01.320519 uiwiz-0.1.9/uiwiz/elements/datepicker.py
+-rw-r--r--   0        0        0      363 2024-01-22 20:49:01.320519 uiwiz-0.1.9/uiwiz/elements/divider.py
+-rw-r--r--   0        0        0     1800 2024-01-22 20:49:01.320519 uiwiz-0.1.9/uiwiz/elements/drawer.py
+-rw-r--r--   0        0        0      530 2024-01-22 20:49:01.320519 uiwiz-0.1.9/uiwiz/elements/dropdown.py
+-rw-r--r--   0        0        0      717 2024-01-22 20:49:01.320519 uiwiz-0.1.9/uiwiz/elements/extensions/bindable.py
+-rw-r--r--   0        0        0      273 2024-01-22 20:49:01.320519 uiwiz-0.1.9/uiwiz/elements/footer.py
+-rw-r--r--   0        0        0      567 2024-01-22 20:49:01.320519 uiwiz-0.1.9/uiwiz/elements/form.py
+-rw-r--r--   0        0        0      156 2024-01-22 20:49:01.320519 uiwiz-0.1.9/uiwiz/elements/html.py
+-rw-r--r--   0        0        0     1267 2024-01-22 20:49:01.324519 uiwiz-0.1.9/uiwiz/elements/input.py
+-rw-r--r--   0        0        0      551 2024-01-22 20:49:01.324519 uiwiz-0.1.9/uiwiz/elements/label.py
+-rw-r--r--   0        0        0      308 2024-01-22 20:49:01.324519 uiwiz-0.1.9/uiwiz/elements/link.py
+-rw-r--r--   0        0        0      619 2024-01-22 20:49:01.324519 uiwiz-0.1.9/uiwiz/elements/markdown.py
+-rw-r--r--   0        0        0      223 2024-01-22 20:49:01.324519 uiwiz-0.1.9/uiwiz/elements/nav.py
+-rw-r--r--   0        0        0      313 2024-01-22 20:49:01.324519 uiwiz-0.1.9/uiwiz/elements/radio.py
+-rw-r--r--   0        0        0      738 2024-01-22 20:49:01.324519 uiwiz-0.1.9/uiwiz/elements/range.py
+-rw-r--r--   0        0        0      169 2024-01-22 20:49:01.324519 uiwiz-0.1.9/uiwiz/elements/row.py
+-rw-r--r--   0        0        0     2166 2024-01-22 20:49:01.324519 uiwiz-0.1.9/uiwiz/elements/spinner.py
+-rw-r--r--   0        0        0      956 2024-01-22 20:49:01.324519 uiwiz-0.1.9/uiwiz/elements/table.py
+-rw-r--r--   0        0        0     1433 2024-01-22 20:49:01.324519 uiwiz-0.1.9/uiwiz/elements/tabs.py
+-rw-r--r--   0        0        0      905 2024-01-22 20:49:01.324519 uiwiz-0.1.9/uiwiz/elements/textarea.py
+-rw-r--r--   0        0        0     1882 2024-01-22 20:49:01.324519 uiwiz-0.1.9/uiwiz/elements/toast.py
+-rw-r--r--   0        0        0      373 2024-01-22 20:49:01.324519 uiwiz-0.1.9/uiwiz/elements/toggle.py
+-rw-r--r--   0        0        0      784 2024-01-22 20:49:01.324519 uiwiz-0.1.9/uiwiz/elements/upload.py
+-rw-r--r--   0        0        0      212 2024-01-22 20:49:01.324519 uiwiz-0.1.9/uiwiz/event.py
+-rw-r--r--   0        0        0      825 2024-01-22 20:49:01.324519 uiwiz-0.1.9/uiwiz/header_middelware.py
+-rw-r--r--   0        0        0      397 2024-01-22 20:49:01.324519 uiwiz-0.1.9/uiwiz/static/app.css
+-rw-r--r--   0        0        0     2752 2024-01-22 20:49:01.324519 uiwiz-0.1.9/uiwiz/static/codehighlight.css
+-rw-r--r--   0        0        0  1737043 2024-01-22 20:49:01.332519 uiwiz-0.1.9/uiwiz/static/libs/aggrid-community.min.js
+-rw-r--r--   0        0        0    30661 2024-01-22 20:49:01.332519 uiwiz-0.1.9/uiwiz/static/markdown.css
+-rw-r--r--   0        0        0      281 2024-01-22 20:49:01.332519 uiwiz-0.1.9/uiwiz/svg/error.svg
+-rw-r--r--   0        0        0      272 2024-01-22 20:49:01.332519 uiwiz-0.1.9/uiwiz/svg/info.svg
+-rw-r--r--   0        0        0      245 2024-01-22 20:49:01.332519 uiwiz-0.1.9/uiwiz/svg/menu.svg
+-rw-r--r--   0        0        0      258 2024-01-22 20:49:01.332519 uiwiz-0.1.9/uiwiz/svg/success.svg
+-rw-r--r--   0        0        0      308 2024-01-22 20:49:01.332519 uiwiz-0.1.9/uiwiz/svg/svg_handler.py
+-rw-r--r--   0        0        0      345 2024-01-22 20:49:01.332519 uiwiz-0.1.9/uiwiz/svg/warning.svg
+-rw-r--r--   0        0        0     2950 2024-01-22 20:49:01.332519 uiwiz-0.1.9/uiwiz/templates/default.html
+-rw-r--r--   0        0        0     1483 2024-01-22 20:49:01.332519 uiwiz-0.1.9/uiwiz/ui.py
+-rw-r--r--   0        0        0     2147 1970-01-01 00:00:00.000000 uiwiz-0.1.9/PKG-INFO
```

### Comparing `uiwiz-0.1.8/LICENSE` & `uiwiz-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `uiwiz-0.1.8/README.md` & `uiwiz-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `uiwiz-0.1.8/pyproject.toml` & `uiwiz-0.1.9/pyproject.toml`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "uiwiz"
-version = "0.1.8"
+version = "0.1.9"
 description = ""
 authors = ["Declow <Ditlev.stjerne@gmai.com>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = ">=3.9"
 uvicorn = "^0.23.2"
```

### Comparing `uiwiz-0.1.8/uiwiz/app.py` & `uiwiz-0.1.9/uiwiz/app.py`

 * *Files 7% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 import logging
 
 logger = logging.getLogger("uiwiz")
 logger.addHandler(logging.NullHandler())
 
 
 class UiwizApp(FastAPI):
-    ui_routes = {}
+    app_paths = {}
 
     def __init__(
         self,
         toast_delay: int = 2500,
         error_classes: str = "alert bg-[#FF8080]",
         theme: Optional[str] = None,
         *args,
@@ -104,14 +104,23 @@
                 content = f.read()
 
             content_type, _ = guess_type(filename)
             return Response(content, media_type=content_type)
 
         self.get(prefix + "{filename}")(get_extension)
 
+    def post(self, path: str, *args, **kwargs):
+        s = super()
+
+        def decorator(func: Callable, *args, **kwargs) -> Callable:
+            self.app_paths[func] = path
+            return s.post(path, *args, **kwargs)(func)
+
+        return decorator
+
     def page(
         self,
         path: str,
         *args,
         title: Optional[str] = "uiwiz",
         favicon: Optional[str] = None,
     ) -> Callable:
@@ -140,15 +149,15 @@
                     "request",
                     inspect.Parameter.POSITIONAL_OR_KEYWORD,
                     annotation=Request,
                 )
                 params.insert(0, request)
             decorated.__signature__ = inspect.Signature(params)
 
-            self.ui_routes[decorated] = path
+            self.app_paths[decorated] = path
 
             return self.get(path)(decorated)
 
         return decorator
 
     def ui(self, path: str) -> Callable:
         def decorator(func: Callable) -> Callable:
@@ -174,11 +183,11 @@
                 if p.annotation == inspect.Signature.empty:
                     p._annotation = Request
             if "request" not in {p.name for p in params}:
                 params.insert(0, request)
             decorated.__signature__ = inspect.Signature(params)
 
             if not self.route_exists(path):
-                self.ui_routes[decorated] = path
+                self.app_paths[decorated] = path
             return self.post(path)(decorated)
 
         return decorator
```

### Comparing `uiwiz-0.1.8/uiwiz/element.py` & `uiwiz-0.1.9/uiwiz/element.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import asyncio
 import os
 from pathlib import Path
-from typing import Callable, Optional
+from typing import Callable, Optional, Union
 import random
 from uiwiz.header_middelware import get_headers
 from uiwiz.event import Event
 
 # https://developer.mozilla.org/en-US/docs/Glossary/Void_element
 VOID_ELEMENTS = [
     "area",
@@ -238,46 +238,49 @@
     def before_render(self):
         pass
 
     def add_event_to_attributes(self):
         if self.event == {}:
             return
 
-        endpoint = self.event.get("endpoint")
+        self.attributes["hx-target"] = self.get_target(self.event.get("target"))
+        self.attributes["hx-swap"] = self.event.get("swap") if self.event.get("swap") is not None else "outerHTML"
+
+        func = self.event["func"]
+        endpoint = Frame.api.app_paths.get(func)
         if endpoint is None:
-            func = self.event["func"]
-            if endpoint := Frame.api.ui_routes.get(func):
-                pass
-            else:
-                generator = random.Random(self.id)
-                endpoint = "/" + "".join([str(generator.randrange(10)) for _ in range(20)])
-                Frame.api.ui(endpoint)(func)
-        target = self.event.get("target") if self.event.get("target") is not None else "this"
-        swap = self.event.get("swap") if self.event.get("swap") is not None else "outerHTML"
+            endpoint = f"/_uiwiz/hash/{func.__hash__()}"
+            Frame.api.ui(endpoint)(func)
 
         self.attributes["hx-post"] = endpoint
         if self.event.get("trigger"):
             self.attributes["hx-trigger"] = self.event["trigger"]
 
-        if isinstance(target, Callable):
-            self.attributes["hx-target"] = "#%s" % str(target())
-        else:
-            self.attributes["hx-target"] = target
-
-        self.attributes["hx-swap"] = swap
-
         if vals := self.event.get("vals"):
             self.attributes["hx-vals"] = vals
         if include := self.event.get("include"):
             self.attributes["hx-include"] = include
         if hx_encoding := self.event.get("hx-encoding"):
             self.attributes["hx-encoding"] = hx_encoding
         else:
             self.attributes["hx-ext"] = "json-enc"
 
+    def get_target(self, target: Union[Callable, str, "Element", None]) -> str:
+        _target = "this"
+        if target is None:
+            return _target
+
+        if isinstance(target, Callable):
+            return "#%s" % str(target())
+
+        if target != "this" and "#" not in target:
+            return "#" + target
+        else:
+            return target
+
     def render_js(self, lst_js: list[str]) -> str:
         lst = set()
         for lib in lst_js:
             lst.add('<script src="%s"></script>' % lib)
         return "".join(lst)
 
     def __str__(self) -> str:
```

### Comparing `uiwiz-0.1.8/uiwiz/elements/aggrid.js` & `uiwiz-0.1.9/uiwiz/elements/aggrid.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -44,11 +44,11 @@
         gridApi.setGridOption('columnDefs', cols);
         gridApi.setGridOption('rowData', rows);
     } else {
         const cols = JSON.parse(getAttributeFromElement(element, "hx-aggrid-cols"));
         const rows = JSON.parse(getAttributeFromElement(element, "hx-aggrid-rows"));
 
         gridApi = agGrid.createGrid(element, getGridOptions(cols, rows));
-        grids[element.id] = gridApi;
+        _uiWizardGrids[element.id] = gridApi;
     }
     return gridApi;
 }
```

### Comparing `uiwiz-0.1.8/uiwiz/elements/aggrid.py` & `uiwiz-0.1.9/uiwiz/elements/aggrid.py`

 * *Files identical despite different names*

### Comparing `uiwiz-0.1.8/uiwiz/elements/avatar.py` & `uiwiz-0.1.9/uiwiz/elements/avatar.py`

 * *Files identical despite different names*

### Comparing `uiwiz-0.1.8/uiwiz/elements/button.py` & `uiwiz-0.1.9/uiwiz/elements/form.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,31 +1,24 @@
-from typing import Callable, Union
+from typing import Callable, Optional, Union
 from uiwiz.element import Element
 
 
-class Button(Element):
-    root_class: str = "btn "
+class Form(Element):
+    root_class: str = "col "
 
-    def __init__(self, title: str) -> None:
-        super().__init__(tag="button")
-        self.content = title
+    def __init__(self) -> None:
+        super().__init__("form")
         self.classes()
-        self.inline = True
 
-    def on_click(
-        self, func: Callable = None, endpoint=None, target: Union[Callable, str, Element] = None, swap: str = None
-    ) -> "Button":
-        _target = ""
-        if isinstance(target, str):
-            _target = "#" + target
-        if isinstance(target, Element):
-            _target = "#" + target.id
-        if isinstance(target, Callable):
-            _target = target
+    def on_submit(
+        self,
+        func: Optional[Callable] = None,
+        target: Union[Callable, str, Element] = None,
+        swap: Optional[str] = "beforeend",
+    ):
         self.event = {
             "func": func,
-            "trigger": "click",
-            "endpoint": endpoint,
-            "target": _target,
+            "trigger": "submit",
+            "target": target,
             "swap": swap,
         }
         return self
```

### Comparing `uiwiz-0.1.8/uiwiz/elements/drawer.py` & `uiwiz-0.1.9/uiwiz/elements/drawer.py`

 * *Files identical despite different names*

### Comparing `uiwiz-0.1.8/uiwiz/elements/dropdown.py` & `uiwiz-0.1.9/uiwiz/elements/dropdown.py`

 * *Files identical despite different names*

### Comparing `uiwiz-0.1.8/uiwiz/elements/extensions/bindable.py` & `uiwiz-0.1.9/uiwiz/elements/extensions/bindable.py`

 * *Files identical despite different names*

### Comparing `uiwiz-0.1.8/uiwiz/elements/input.py` & `uiwiz-0.1.9/uiwiz/elements/input.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,22 +1,23 @@
-from typing import Callable
+from typing import Callable, Optional
 from uiwiz.element import Element
 
 
 class Input(Element):
     root_class: str = "input "
     _classes: str = "input-bordered w-full max-w-xs"
 
     def __init__(
         self,
         placeholder: str = None,
         name=None,
-        on_change: Callable = None,
-        target: Callable = None,
+        on_change: Optional[Callable] = None,
+        target: Optional[Callable] = None,
         trigger: str = "input",
+        swap: Optional[str] = "swap",
     ) -> None:
         """Input
 
         This element is used for input data
 
         :param placeholder: Text to show before input
         :param name: Used in the attributes name sent back in json
@@ -30,13 +31,11 @@
         self.attributes["placeholder"] = placeholder
         self.attributes["autocomplete"] = "off"
         self.inline = True
 
         if on_change:
             self.event = {
                 "func": on_change,
-                "inputs": None,
                 "trigger": trigger,
-                "endpoint": None,
                 "target": target,
-                "swap": "swap",
+                "swap": swap,
             }
```

### Comparing `uiwiz-0.1.8/uiwiz/elements/label.py` & `uiwiz-0.1.9/uiwiz/elements/label.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 from typing import Optional
 from uiwiz.element import Element
 from uiwiz.elements.extensions.bindable import Bindable
 
 
 class Label(Bindable):
-    _classes: str = "label "
+    root_class: str = "label "
 
     def __init__(self, text: Optional[str] = None, for_: Element = None) -> None:
         super().__init__(tag="label")
         self.inline = True
         if text:
             self.content = text
         if for_:
             self.attributes["for"] = for_.id
-        self.classes(Label._classes)
+        self.classes()
 
     def set_text(self, text: str) -> "Label":
         self.content = text
         return self
```

### Comparing `uiwiz-0.1.8/uiwiz/elements/markdown.py` & `uiwiz-0.1.9/uiwiz/elements/markdown.py`

 * *Files identical despite different names*

### Comparing `uiwiz-0.1.8/uiwiz/elements/range.py` & `uiwiz-0.1.9/uiwiz/elements/range.py`

 * *Files identical despite different names*

### Comparing `uiwiz-0.1.8/uiwiz/elements/spinner.py` & `uiwiz-0.1.9/uiwiz/elements/spinner.py`

 * *Files identical despite different names*

### Comparing `uiwiz-0.1.8/uiwiz/elements/table.py` & `uiwiz-0.1.9/uiwiz/elements/table.py`

 * *Files identical despite different names*

### Comparing `uiwiz-0.1.8/uiwiz/elements/tabs.py` & `uiwiz-0.1.9/uiwiz/elements/tabs.py`

 * *Files identical despite different names*

### Comparing `uiwiz-0.1.8/uiwiz/elements/textarea.py` & `uiwiz-0.1.9/uiwiz/elements/textarea.py`

 * *Files 20% similar despite different names*

```diff
@@ -9,27 +9,26 @@
     def __init__(
         self,
         placeholder: str = None,
         name="input",
         on_change: Callable = None,
         target: Callable = None,
         trigger: str = "input",
+        swap: str = "swap",
     ) -> None:
         super().__init__("textarea")
         self.attributes["name"] = name
         self.attributes["placeholder"] = placeholder
         self.inline = True
         self.classes(TextArea._classes)
 
         if on_change:
             self.event = {
                 "func": on_change,
-                "inputs": None,
                 "trigger": trigger,
-                "endpoint": None,
                 "target": target,
-                "swap": "swap",
+                "swap": swap,
             }
 
     @property
     def placeholder(self) -> Optional[str]:
         return self.attributes["placeholder"]
```

### Comparing `uiwiz-0.1.8/uiwiz/elements/toast.py` & `uiwiz-0.1.9/uiwiz/elements/toast.py`

 * *Files identical despite different names*

### Comparing `uiwiz-0.1.8/uiwiz/elements/upload.py` & `uiwiz-0.1.9/uiwiz/elements/upload.py`

 * *Files 19% similar despite different names*

```diff
@@ -19,12 +19,11 @@
         self.attributes["type"] = "file"
         self.attributes["name"] = name
         self.classes(Upload._classes)
 
         self.event = {
             "func": on_upload,
             "trigger": trigger,
-            "endpoint": endpoint,
             "target": target,
             "swap": swap,
             "hx-encoding": "multipart/form-data",
         }
```

### Comparing `uiwiz-0.1.8/uiwiz/header_middelware.py` & `uiwiz-0.1.9/uiwiz/header_middelware.py`

 * *Files identical despite different names*

### Comparing `uiwiz-0.1.8/uiwiz/static/codehighlight.css` & `uiwiz-0.1.9/uiwiz/static/codehighlight.css`

 * *Files identical despite different names*

### Comparing `uiwiz-0.1.8/uiwiz/static/libs/aggrid-community.min.js` & `uiwiz-0.1.9/uiwiz/static/libs/aggrid-community.min.js`

 * *Files identical despite different names*

### Comparing `uiwiz-0.1.8/uiwiz/static/markdown.css` & `uiwiz-0.1.9/uiwiz/static/markdown.css`

 * *Files identical despite different names*

### Comparing `uiwiz-0.1.8/uiwiz/templates/default.html` & `uiwiz-0.1.9/uiwiz/templates/default.html`

 * *Files identical despite different names*

### Comparing `uiwiz-0.1.8/uiwiz/ui.py` & `uiwiz-0.1.9/uiwiz/ui.py`

 * *Files identical despite different names*

### Comparing `uiwiz-0.1.8/PKG-INFO` & `uiwiz-0.1.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: uiwiz
-Version: 0.1.8
+Version: 0.1.9
 Summary: 
 Author: Declow
 Author-email: Ditlev.stjerne@gmai.com
 Requires-Python: >=3.9
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

