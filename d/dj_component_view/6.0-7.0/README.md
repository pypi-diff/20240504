# Comparing `tmp/dj_component_view-6.0.tar.gz` & `tmp/dj_component_view-7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dj_component_view-6.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "dj_component_view-7.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `dj_component_view-6.0.tar` & `dj_component_view-7.0.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     3078 2024-04-29 05:31:20.582104 dj_component_view-6.0/.gitignore
--rw-r--r--   0        0        0     1086 2024-04-29 05:24:52.851465 dj_component_view-6.0/LICENSE
--rw-r--r--   0        0        0     1984 2024-05-04 01:49:50.951954 dj_component_view-6.0/README.md
--rw-r--r--   0        0        0     1749 2024-05-04 01:45:19.627835 dj_component_view-6.0/dj_component_view.py
--rw-r--r--   0        0        0      500 2024-05-04 01:30:17.767497 dj_component_view-6.0/pyproject.toml
--rw-r--r--   0        0        0     2356 1970-01-01 00:00:00.000000 dj_component_view-6.0/PKG-INFO
+-rw-r--r--   0        0        0     3078 2024-04-29 05:31:20.582104 dj_component_view-7.0/.gitignore
+-rw-r--r--   0        0        0     1086 2024-04-29 05:24:52.851465 dj_component_view-7.0/LICENSE
+-rw-r--r--   0        0        0     1838 2024-05-04 02:42:09.140597 dj_component_view-7.0/README.md
+-rw-r--r--   0        0        0     2031 2024-05-04 02:11:54.379254 dj_component_view-7.0/dj_component_view.py
+-rw-r--r--   0        0        0      500 2024-05-04 02:12:03.540239 dj_component_view-7.0/pyproject.toml
+-rw-r--r--   0        0        0     2210 1970-01-01 00:00:00.000000 dj_component_view-7.0/PKG-INFO
```

### Comparing `dj_component_view-6.0/.gitignore` & `dj_component_view-7.0/.gitignore`

 * *Files identical despite different names*

### Comparing `dj_component_view-6.0/LICENSE` & `dj_component_view-7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `dj_component_view-6.0/README.md` & `dj_component_view-7.0/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -1,43 +1,38 @@
 # dj_component_view
 
 This project lets you create reusable Django views from [jinjax](https://jinjax.scaletti.dev/) templates.
 
 ## Usage
 
-### templates/components/Greeting.jinja
+### Greeting.jinja
 
 ```jinja
 <h1>hello, {{ name }}</h1>
 ```
 
 ### views.py
 
 ```python
 from dj_component_view import ComponentView
 from djecorator import Route
 
 route = Route()
 
-@route("/")
-class IndexView(ComponentView):
-    template = "components/Index.jinja"
-
-
 @route("/greet", name="greet")
 class GreetView(ComponentView):
-    template = "components/Greeting.jinja"
+    component = "Greeting"
 
-    def context(self, request):
+    def render(self, request):
         return {
             "name": request.GET.get("name", "World"),
         }
 ```
 
-### templates/components/Index.jinja with [htmx](https://htmx.org)
+### index.html with [htmx](https://htmx.org)
 
 ```html
 <form hx-get="{{ url('greet') }}" hx-trigger="submit">
   <input type="text" name="name" placeholder="Enter your name" />
   <button type="submit">Greet</button>
 </form>
 ```
```

### Comparing `dj_component_view-6.0/dj_component_view.py` & `dj_component_view-7.0/dj_component_view.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,48 +1,52 @@
 from importlib import import_module
 from typing import Union
 
 from django.conf import settings
 from django.http import HttpResponse, HttpResponseNotAllowed
 from django.views import View
-from django.shortcuts import render
 
 
 class ComponentView(View):
-    template = None
-    methods = ["GET", "POST"]
+    component = None
+    methods = ["GET"]
 
     def get_catalog(self):
         for template_engine in settings.TEMPLATES:
             if template_engine["BACKEND"] == "django.template.backends.jinja2.Jinja2":
                 env_string = template_engine["OPTIONS"]["environment"]
                 module_path, function_name = env_string.rsplit(".", 1)
                 module = import_module(module_path)
                 environment_function = getattr(module, function_name)
                 return environment_function().globals["catalog"]
         raise ValueError("Jinja2 template engine not found in settings.")
 
+    def render_to_response(self, context):
+        catalog = self.get_catalog()
+        catalog.jinja_env.globals.update(context)
+        if not self.component:
+            raise ValueError("ComponentView subclasses must define a component.")
+        return HttpResponse(str(catalog.render(self.component, **context)))
 
     def dispatch(self, request, *args, **kwargs):
         if request.method.lower() not in (method.lower() for method in self.methods):
             return HttpResponseNotAllowed(self.methods)
         return super().dispatch(request, *args, **kwargs)
     
     def _base_get_post(self, request, *args, **kwargs):
-        ctx = self.render(request)
-        template = self.template
+        rendered = self.render(request)
 
-        if isinstance(ctx, HttpResponse):
-            return ctx
-        
-        return render(
-            request=request,
-            template_name=template,
-            context=ctx,
-        )
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
```

### Comparing `dj_component_view-6.0/PKG-INFO` & `dj_component_view-7.0/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,54 +1,49 @@
 Metadata-Version: 2.1
 Name: dj_component_view
-Version: 6.0
+Version: 7.0
 Summary: Django component view for jinjax
 Author-email: Stephan Fitzpatrick <knowsuchagency@gmail.com>
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: MIT License
 Requires-Dist: django
 Requires-Dist: jinjax
 Project-URL: Source, https://github.com/knowsuchagency/dj_component_view
 
 # dj_component_view
 
 This project lets you create reusable Django views from [jinjax](https://jinjax.scaletti.dev/) templates.
 
 ## Usage
 
-### templates/components/Greeting.jinja
+### Greeting.jinja
 
 ```jinja
 <h1>hello, {{ name }}</h1>
 ```
 
 ### views.py
 
 ```python
 from dj_component_view import ComponentView
 from djecorator import Route
 
 route = Route()
 
-@route("/")
-class IndexView(ComponentView):
-    template = "components/Index.jinja"
-
-
 @route("/greet", name="greet")
 class GreetView(ComponentView):
-    template = "components/Greeting.jinja"
+    component = "Greeting"
 
-    def context(self, request):
+    def render(self, request):
         return {
             "name": request.GET.get("name", "World"),
         }
 ```
 
-### templates/components/Index.jinja with [htmx](https://htmx.org)
+### index.html with [htmx](https://htmx.org)
 
 ```html
 <form hx-get="{{ url('greet') }}" hx-trigger="submit">
   <input type="text" name="name" placeholder="Enter your name" />
   <button type="submit">Greet</button>
 </form>
 ```
```

