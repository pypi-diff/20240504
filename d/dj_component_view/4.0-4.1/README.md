# Comparing `tmp/dj_component_view-4.0.tar.gz` & `tmp/dj_component_view-4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dj_component_view-4.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "dj_component_view-4.1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `dj_component_view-4.0.tar` & `dj_component_view-4.1.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     3078 2024-04-29 05:31:20.582104 dj_component_view-4.0/.gitignore
--rw-r--r--   0        0        0     1086 2024-04-29 05:24:52.851465 dj_component_view-4.0/LICENSE
--rw-r--r--   0        0        0     1812 2024-05-03 22:50:36.952253 dj_component_view-4.0/README.md
--rw-r--r--   0        0        0     1693 2024-05-03 22:48:48.105321 dj_component_view-4.0/dj_component_view.py
--rw-r--r--   0        0        0      500 2024-05-03 22:52:01.541159 dj_component_view-4.0/pyproject.toml
--rw-r--r--   0        0        0     2184 1970-01-01 00:00:00.000000 dj_component_view-4.0/PKG-INFO
+-rw-r--r--   0        0        0     3078 2024-04-29 05:31:20.582104 dj_component_view-4.1/.gitignore
+-rw-r--r--   0        0        0     1086 2024-04-29 05:24:52.851465 dj_component_view-4.1/LICENSE
+-rw-r--r--   0        0        0     1812 2024-05-03 22:50:36.952253 dj_component_view-4.1/README.md
+-rw-r--r--   0        0        0     1835 2024-05-04 00:20:49.007878 dj_component_view-4.1/dj_component_view.py
+-rw-r--r--   0        0        0      500 2024-05-04 00:21:34.369041 dj_component_view-4.1/pyproject.toml
+-rw-r--r--   0        0        0     2184 1970-01-01 00:00:00.000000 dj_component_view-4.1/PKG-INFO
```

### Comparing `dj_component_view-4.0/.gitignore` & `dj_component_view-4.1/.gitignore`

 * *Files identical despite different names*

### Comparing `dj_component_view-4.0/LICENSE` & `dj_component_view-4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `dj_component_view-4.0/README.md` & `dj_component_view-4.1/README.md`

 * *Files identical despite different names*

### Comparing `dj_component_view-4.0/dj_component_view.py` & `dj_component_view-4.1/dj_component_view.py`

 * *Files 16% similar despite different names*

```diff
@@ -26,18 +26,21 @@
             raise ValueError("ComponentView subclasses must define a component.")
         return HttpResponse(str(catalog.render(self.component, **context)))
 
     def dispatch(self, request, *args, **kwargs):
         if request.method.lower() not in (method.lower() for method in self.methods):
             return HttpResponseNotAllowed(self.methods)
         return super().dispatch(request, *args, **kwargs)
-
-    def get(self, request, *args, **kwargs):
+    
+    def _base_get_post(self, request, *args, **kwargs):
         context = self.context(request)
+        context.setdefault("request", request)
         return self.render_to_response(context)
 
+    def get(self, request, *args, **kwargs):
+        return self._base_get_post(request, *args, **kwargs)
+
     def post(self, request, *args, **kwargs):
-        context = self.context(request)
-        return self.render_to_response(context)
+        return self._base_get_post(request, *args, **kwargs)
 
     def context(self, request):
         return {}
```

### Comparing `dj_component_view-4.0/PKG-INFO` & `dj_component_view-4.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dj_component_view
-Version: 4.0
+Version: 4.1
 Summary: Django component view for jinjax
 Author-email: Stephan Fitzpatrick <knowsuchagency@gmail.com>
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: MIT License
 Requires-Dist: django
 Requires-Dist: jinjax
 Project-URL: Source, https://github.com/knowsuchagency/dj_component_view
```

