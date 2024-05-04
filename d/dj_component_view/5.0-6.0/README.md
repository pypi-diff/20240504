# Comparing `tmp/dj_component_view-5.0.tar.gz` & `tmp/dj_component_view-6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dj_component_view-5.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "dj_component_view-6.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `dj_component_view-5.0.tar` & `dj_component_view-6.0.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     3078 2024-04-29 05:31:20.582104 dj_component_view-5.0/.gitignore
--rw-r--r--   0        0        0     1086 2024-04-29 05:24:52.851465 dj_component_view-5.0/LICENSE
--rw-r--r--   0        0        0     1839 2024-05-04 01:07:31.276056 dj_component_view-5.0/README.md
--rw-r--r--   0        0        0     2031 2024-05-04 01:06:17.774307 dj_component_view-5.0/dj_component_view.py
--rw-r--r--   0        0        0      500 2024-05-04 00:53:49.874700 dj_component_view-5.0/pyproject.toml
--rw-r--r--   0        0        0     2211 1970-01-01 00:00:00.000000 dj_component_view-5.0/PKG-INFO
+-rw-r--r--   0        0        0     3078 2024-04-29 05:31:20.582104 dj_component_view-6.0/.gitignore
+-rw-r--r--   0        0        0     1086 2024-04-29 05:24:52.851465 dj_component_view-6.0/LICENSE
+-rw-r--r--   0        0        0     1984 2024-05-04 01:49:50.951954 dj_component_view-6.0/README.md
+-rw-r--r--   0        0        0     1749 2024-05-04 01:45:19.627835 dj_component_view-6.0/dj_component_view.py
+-rw-r--r--   0        0        0      500 2024-05-04 01:30:17.767497 dj_component_view-6.0/pyproject.toml
+-rw-r--r--   0        0        0     2356 1970-01-01 00:00:00.000000 dj_component_view-6.0/PKG-INFO
```

### Comparing `dj_component_view-5.0/.gitignore` & `dj_component_view-6.0/.gitignore`

 * *Files identical despite different names*

### Comparing `dj_component_view-5.0/LICENSE` & `dj_component_view-6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `dj_component_view-5.0/README.md` & `dj_component_view-6.0/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -1,43 +1,46 @@
 # dj_component_view
 
-# TODO: update the readme
-
 This project lets you create reusable Django views from [jinjax](https://jinjax.scaletti.dev/) templates.
 
 ## Usage
 
-### Greeting.jinja
+### templates/components/Greeting.jinja
 
 ```jinja
 <h1>hello, {{ name }}</h1>
 ```
 
 ### views.py
 
 ```python
 from dj_component_view import ComponentView
 from djecorator import Route
 
 route = Route()
 
-@route("/greet")
+@route("/")
+class IndexView(ComponentView):
+    template = "components/Index.jinja"
+
+
+@route("/greet", name="greet")
 class GreetView(ComponentView):
-    component = "Greeting"
+    template = "components/Greeting.jinja"
 
     def context(self, request):
         return {
             "name": request.GET.get("name", "World"),
         }
 ```
 
-### index.html with [htmx](https://htmx.org)
+### templates/components/Index.jinja with [htmx](https://htmx.org)
 
 ```html
-<form hx-get="/greet" hx-trigger="submit">
+<form hx-get="{{ url('greet') }}" hx-trigger="submit">
   <input type="text" name="name" placeholder="Enter your name" />
   <button type="submit">Greet</button>
 </form>
 ```
 
 ### Specifying the Allowed HTTP Methods
 
@@ -46,15 +49,15 @@
 - If `methods` is set to `["GET"]`, only GET requests will be allowed.
 - If `methods` is set to `["POST"]`, only POST requests will be allowed.
 - If `methods` is set to `["GET", "POST"]`, both GET and POST requests will be allowed.
 
 ```python
 class CustomView(ComponentView):
     component = "CustomComponent"
-    methods = ["get"]
+    methods = ["post"]
 
     ...
 
 ```
 
 If the incoming request's method does not match any of the specified methods, a 405 Method Not Allowed response will be returned.
```

### Comparing `dj_component_view-5.0/dj_component_view.py` & `dj_component_view-6.0/dj_component_view.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,52 +1,48 @@
 from importlib import import_module
 from typing import Union
 
 from django.conf import settings
 from django.http import HttpResponse, HttpResponseNotAllowed
 from django.views import View
+from django.shortcuts import render
 
 
 class ComponentView(View):
-    component = None
-    methods = ["GET"]
+    template = None
+    methods = ["GET", "POST"]
 
     def get_catalog(self):
         for template_engine in settings.TEMPLATES:
             if template_engine["BACKEND"] == "django.template.backends.jinja2.Jinja2":
                 env_string = template_engine["OPTIONS"]["environment"]
                 module_path, function_name = env_string.rsplit(".", 1)
                 module = import_module(module_path)
                 environment_function = getattr(module, function_name)
                 return environment_function().globals["catalog"]
         raise ValueError("Jinja2 template engine not found in settings.")
 
-    def render_to_response(self, context):
-        catalog = self.get_catalog()
-        catalog.jinja_env.globals.update(context)
-        if not self.component:
-            raise ValueError("ComponentView subclasses must define a component.")
-        return HttpResponse(str(catalog.render(self.component, **context)))
 
     def dispatch(self, request, *args, **kwargs):
         if request.method.lower() not in (method.lower() for method in self.methods):
             return HttpResponseNotAllowed(self.methods)
         return super().dispatch(request, *args, **kwargs)
     
     def _base_get_post(self, request, *args, **kwargs):
-        rendered = self.render(request)
+        ctx = self.render(request)
+        template = self.template
 
-        if isinstance(rendered, HttpResponse):
-            return rendered
-        elif rendered is None:
-            rendered = {}
-
-        rendered.setdefault("request", request)
-
-        return self.render_to_response(rendered)
+        if isinstance(ctx, HttpResponse):
+            return ctx
+        
+        return render(
+            request=request,
+            template_name=template,
+            context=ctx,
+        )
 
     def get(self, request, *args, **kwargs):
         return self._base_get_post(request, *args, **kwargs)
 
     def post(self, request, *args, **kwargs):
         return self._base_get_post(request, *args, **kwargs)
```

### Comparing `dj_component_view-5.0/PKG-INFO` & `dj_component_view-6.0/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,54 +1,57 @@
 Metadata-Version: 2.1
 Name: dj_component_view
-Version: 5.0
+Version: 6.0
 Summary: Django component view for jinjax
 Author-email: Stephan Fitzpatrick <knowsuchagency@gmail.com>
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: MIT License
 Requires-Dist: django
 Requires-Dist: jinjax
 Project-URL: Source, https://github.com/knowsuchagency/dj_component_view
 
 # dj_component_view
 
-# TODO: update the readme
-
 This project lets you create reusable Django views from [jinjax](https://jinjax.scaletti.dev/) templates.
 
 ## Usage
 
-### Greeting.jinja
+### templates/components/Greeting.jinja
 
 ```jinja
 <h1>hello, {{ name }}</h1>
 ```
 
 ### views.py
 
 ```python
 from dj_component_view import ComponentView
 from djecorator import Route
 
 route = Route()
 
-@route("/greet")
+@route("/")
+class IndexView(ComponentView):
+    template = "components/Index.jinja"
+
+
+@route("/greet", name="greet")
 class GreetView(ComponentView):
-    component = "Greeting"
+    template = "components/Greeting.jinja"
 
     def context(self, request):
         return {
             "name": request.GET.get("name", "World"),
         }
 ```
 
-### index.html with [htmx](https://htmx.org)
+### templates/components/Index.jinja with [htmx](https://htmx.org)
 
 ```html
-<form hx-get="/greet" hx-trigger="submit">
+<form hx-get="{{ url('greet') }}" hx-trigger="submit">
   <input type="text" name="name" placeholder="Enter your name" />
   <button type="submit">Greet</button>
 </form>
 ```
 
 ### Specifying the Allowed HTTP Methods
 
@@ -57,15 +60,15 @@
 - If `methods` is set to `["GET"]`, only GET requests will be allowed.
 - If `methods` is set to `["POST"]`, only POST requests will be allowed.
 - If `methods` is set to `["GET", "POST"]`, both GET and POST requests will be allowed.
 
 ```python
 class CustomView(ComponentView):
     component = "CustomComponent"
-    methods = ["get"]
+    methods = ["post"]
 
     ...
 
 ```
 
 If the incoming request's method does not match any of the specified methods, a 405 Method Not Allowed response will be returned.
```

