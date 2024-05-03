# Comparing `tmp/dj_component_view-3.0.1.tar.gz` & `tmp/dj_component_view-4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dj_component_view-3.0.1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "dj_component_view-4.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `dj_component_view-3.0.1.tar` & `dj_component_view-4.0.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     3078 2024-04-29 05:31:20.582104 dj_component_view-3.0.1/.gitignore
--rw-r--r--   0        0        0     1086 2024-04-29 05:24:52.851465 dj_component_view-3.0.1/LICENSE
--rw-r--r--   0        0        0     1820 2024-04-29 22:51:24.901841 dj_component_view-3.0.1/README.md
--rw-r--r--   0        0        0     1614 2024-04-29 22:45:49.350973 dj_component_view-3.0.1/dj_component_view.py
--rw-r--r--   0        0        0      502 2024-04-29 22:51:53.501026 dj_component_view-3.0.1/pyproject.toml
--rw-r--r--   0        0        0     2194 1970-01-01 00:00:00.000000 dj_component_view-3.0.1/PKG-INFO
+-rw-r--r--   0        0        0     3078 2024-04-29 05:31:20.582104 dj_component_view-4.0/.gitignore
+-rw-r--r--   0        0        0     1086 2024-04-29 05:24:52.851465 dj_component_view-4.0/LICENSE
+-rw-r--r--   0        0        0     1812 2024-05-03 22:50:36.952253 dj_component_view-4.0/README.md
+-rw-r--r--   0        0        0     1693 2024-05-03 22:48:48.105321 dj_component_view-4.0/dj_component_view.py
+-rw-r--r--   0        0        0      500 2024-05-03 22:52:01.541159 dj_component_view-4.0/pyproject.toml
+-rw-r--r--   0        0        0     2184 1970-01-01 00:00:00.000000 dj_component_view-4.0/PKG-INFO
```

### Comparing `dj_component_view-3.0.1/.gitignore` & `dj_component_view-4.0/.gitignore`

 * *Files identical despite different names*

### Comparing `dj_component_view-3.0.1/LICENSE` & `dj_component_view-4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `dj_component_view-3.0.1/README.md` & `dj_component_view-4.0/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -3,16 +3,14 @@
 This project lets you create reusable Django views from [jinjax](https://jinjax.scaletti.dev/) templates.
 
 ## Usage
 
 ### Greeting.jinja
 
 ```jinja
-{#def name #}
-
 <h1>hello, {{ name }}</h1>
 ```
 
 ### views.py
 
 ```python
 from dj_component_view import ComponentView
@@ -22,53 +20,53 @@
 
 @route("/greet")
 class GreetView(ComponentView):
     component = "Greeting"
 
     def context(self, request):
         return {
-            # by default, the view expects a POST request
-            "name": request.POST.get("name", "World"),
+            "name": request.GET.get("name", "World"),
         }
 ```
 
 ### index.html with [htmx](https://htmx.org)
 
 ```html
-<form hx-post="/greet" hx-trigger="submit">
+<form hx-get="/greet" hx-trigger="submit">
   <input type="text" name="name" placeholder="Enter your name" />
   <button type="submit">Greet</button>
 </form>
 ```
 
-### Specifying the Allowed HTTP Method
+### Specifying the Allowed HTTP Methods
 
-You can set the method class variable in your ComponentView subclass to specify the allowed HTTP method for the view. The default value is None, which means both GET and POST methods are allowed.
+You can set the `methods` class variable in your ComponentView subclass to specify the allowed HTTP methods for the view. The default value is `["GET"]`.
 
-- If `method` is set to `"GET"`, only GET requests will be allowed.
-- If `method` is set to `"POST"`, only POST requests will be allowed.
+- If `methods` is set to `["GET"]`, only GET requests will be allowed.
+- If `methods` is set to `["POST"]`, only POST requests will be allowed.
+- If `methods` is set to `["GET", "POST"]`, both GET and POST requests will be allowed.
 
 ```python
 class CustomView(ComponentView):
     component = "CustomComponent"
-    method = "get"
+    methods = ["get"]
 
     ...
 
 ```
 
-If the incoming request's method does not match the specified method, a 405 Method Not Allowed response will be returned.
+If the incoming request's method does not match any of the specified methods, a 405 Method Not Allowed response will be returned.
 
 ### Overriding the get and post Methods
 
 If you need more control over the handling of GET and POST requests, you can override the get and post methods in your ComponentView subclass.
 
 ```python
 @route("/custom")
 class CustomView(ComponentView):
     component = "CustomComponent"
-    method = "get"
+    methods = ["get"]
 
     def get(self, request, *args, **kwargs):
         # Custom implementation of the GET method
         ...
 ```
```

### Comparing `dj_component_view-3.0.1/dj_component_view.py` & `dj_component_view-4.0/dj_component_view.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,35 +3,36 @@
 from django.conf import settings
 from django.http import HttpResponse, HttpResponseNotAllowed
 from django.views import View
 
 
 class ComponentView(View):
     component = None
-    method = "POST"
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
 
     def render_to_response(self, context):
         catalog = self.get_catalog()
+        catalog.jinja_env.globals.update(context)
         if not self.component:
             raise ValueError("ComponentView subclasses must define a component.")
         return HttpResponse(str(catalog.render(self.component, **context)))
 
     def dispatch(self, request, *args, **kwargs):
-        if request.method.lower() != self.method.lower():
-            return HttpResponseNotAllowed([self.method])
+        if request.method.lower() not in (method.lower() for method in self.methods):
+            return HttpResponseNotAllowed(self.methods)
         return super().dispatch(request, *args, **kwargs)
 
     def get(self, request, *args, **kwargs):
         context = self.context(request)
         return self.render_to_response(context)
 
     def post(self, request, *args, **kwargs):
```

### Comparing `dj_component_view-3.0.1/PKG-INFO` & `dj_component_view-4.0/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dj_component_view
-Version: 3.0.1
+Version: 4.0
 Summary: Django component view for jinjax
 Author-email: Stephan Fitzpatrick <knowsuchagency@gmail.com>
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: MIT License
 Requires-Dist: django
 Requires-Dist: jinjax
 Project-URL: Source, https://github.com/knowsuchagency/dj_component_view
@@ -14,16 +14,14 @@
 This project lets you create reusable Django views from [jinjax](https://jinjax.scaletti.dev/) templates.
 
 ## Usage
 
 ### Greeting.jinja
 
 ```jinja
-{#def name #}
-
 <h1>hello, {{ name }}</h1>
 ```
 
 ### views.py
 
 ```python
 from dj_component_view import ComponentView
@@ -33,54 +31,54 @@
 
 @route("/greet")
 class GreetView(ComponentView):
     component = "Greeting"
 
     def context(self, request):
         return {
-            # by default, the view expects a POST request
-            "name": request.POST.get("name", "World"),
+            "name": request.GET.get("name", "World"),
         }
 ```
 
 ### index.html with [htmx](https://htmx.org)
 
 ```html
-<form hx-post="/greet" hx-trigger="submit">
+<form hx-get="/greet" hx-trigger="submit">
   <input type="text" name="name" placeholder="Enter your name" />
   <button type="submit">Greet</button>
 </form>
 ```
 
-### Specifying the Allowed HTTP Method
+### Specifying the Allowed HTTP Methods
 
-You can set the method class variable in your ComponentView subclass to specify the allowed HTTP method for the view. The default value is None, which means both GET and POST methods are allowed.
+You can set the `methods` class variable in your ComponentView subclass to specify the allowed HTTP methods for the view. The default value is `["GET"]`.
 
-- If `method` is set to `"GET"`, only GET requests will be allowed.
-- If `method` is set to `"POST"`, only POST requests will be allowed.
+- If `methods` is set to `["GET"]`, only GET requests will be allowed.
+- If `methods` is set to `["POST"]`, only POST requests will be allowed.
+- If `methods` is set to `["GET", "POST"]`, both GET and POST requests will be allowed.
 
 ```python
 class CustomView(ComponentView):
     component = "CustomComponent"
-    method = "get"
+    methods = ["get"]
 
     ...
 
 ```
 
-If the incoming request's method does not match the specified method, a 405 Method Not Allowed response will be returned.
+If the incoming request's method does not match any of the specified methods, a 405 Method Not Allowed response will be returned.
 
 ### Overriding the get and post Methods
 
 If you need more control over the handling of GET and POST requests, you can override the get and post methods in your ComponentView subclass.
 
 ```python
 @route("/custom")
 class CustomView(ComponentView):
     component = "CustomComponent"
-    method = "get"
+    methods = ["get"]
 
     def get(self, request, *args, **kwargs):
         # Custom implementation of the GET method
         ...
 ```
```

