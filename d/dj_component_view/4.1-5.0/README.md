# Comparing `tmp/dj_component_view-4.1.tar.gz` & `tmp/dj_component_view-5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dj_component_view-4.1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "dj_component_view-5.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `dj_component_view-4.1.tar` & `dj_component_view-5.0.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     3078 2024-04-29 05:31:20.582104 dj_component_view-4.1/.gitignore
--rw-r--r--   0        0        0     1086 2024-04-29 05:24:52.851465 dj_component_view-4.1/LICENSE
--rw-r--r--   0        0        0     1812 2024-05-03 22:50:36.952253 dj_component_view-4.1/README.md
--rw-r--r--   0        0        0     1835 2024-05-04 00:20:49.007878 dj_component_view-4.1/dj_component_view.py
--rw-r--r--   0        0        0      500 2024-05-04 00:21:34.369041 dj_component_view-4.1/pyproject.toml
--rw-r--r--   0        0        0     2184 1970-01-01 00:00:00.000000 dj_component_view-4.1/PKG-INFO
+-rw-r--r--   0        0        0     3078 2024-04-29 05:31:20.582104 dj_component_view-5.0/.gitignore
+-rw-r--r--   0        0        0     1086 2024-04-29 05:24:52.851465 dj_component_view-5.0/LICENSE
+-rw-r--r--   0        0        0     1839 2024-05-04 01:07:31.276056 dj_component_view-5.0/README.md
+-rw-r--r--   0        0        0     2031 2024-05-04 01:06:17.774307 dj_component_view-5.0/dj_component_view.py
+-rw-r--r--   0        0        0      500 2024-05-04 00:53:49.874700 dj_component_view-5.0/pyproject.toml
+-rw-r--r--   0        0        0     2211 1970-01-01 00:00:00.000000 dj_component_view-5.0/PKG-INFO
```

### Comparing `dj_component_view-4.1/.gitignore` & `dj_component_view-5.0/.gitignore`

 * *Files identical despite different names*

### Comparing `dj_component_view-4.1/LICENSE` & `dj_component_view-5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `dj_component_view-4.1/README.md` & `dj_component_view-5.0/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 # dj_component_view
 
+# TODO: update the readme
+
 This project lets you create reusable Django views from [jinjax](https://jinjax.scaletti.dev/) templates.
 
 ## Usage
 
 ### Greeting.jinja
 
 ```jinja
```

### Comparing `dj_component_view-4.1/dj_component_view.py` & `dj_component_view-5.0/dj_component_view.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 from importlib import import_module
+from typing import Union
 
 from django.conf import settings
 from django.http import HttpResponse, HttpResponseNotAllowed
 from django.views import View
 
 
 class ComponentView(View):
@@ -28,19 +29,26 @@
 
     def dispatch(self, request, *args, **kwargs):
         if request.method.lower() not in (method.lower() for method in self.methods):
             return HttpResponseNotAllowed(self.methods)
         return super().dispatch(request, *args, **kwargs)
     
     def _base_get_post(self, request, *args, **kwargs):
-        context = self.context(request)
-        context.setdefault("request", request)
-        return self.render_to_response(context)
+        rendered = self.render(request)
+
+        if isinstance(rendered, HttpResponse):
+            return rendered
+        elif rendered is None:
+            rendered = {}
+
+        rendered.setdefault("request", request)
+
+        return self.render_to_response(rendered)
 
     def get(self, request, *args, **kwargs):
         return self._base_get_post(request, *args, **kwargs)
 
     def post(self, request, *args, **kwargs):
         return self._base_get_post(request, *args, **kwargs)
 
-    def context(self, request):
+    def render(self, request) -> Union[dict, HttpResponse, None]:
         return {}
```

### Comparing `dj_component_view-4.1/PKG-INFO` & `dj_component_view-5.0/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,20 +1,22 @@
 Metadata-Version: 2.1
 Name: dj_component_view
-Version: 4.1
+Version: 5.0
 Summary: Django component view for jinjax
 Author-email: Stephan Fitzpatrick <knowsuchagency@gmail.com>
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: MIT License
 Requires-Dist: django
 Requires-Dist: jinjax
 Project-URL: Source, https://github.com/knowsuchagency/dj_component_view
 
 # dj_component_view
 
+# TODO: update the readme
+
 This project lets you create reusable Django views from [jinjax](https://jinjax.scaletti.dev/) templates.
 
 ## Usage
 
 ### Greeting.jinja
 
 ```jinja
```

