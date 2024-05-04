# Comparing `tmp/edgegap_service-1.6.0.tar.gz` & `tmp/edgegap_service-1.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "edgegap_service-1.6.0.tar", max compression
+gzip compressed data, was "edgegap_service-1.6.1.tar", max compression
```

## Comparing `edgegap_service-1.6.0.tar` & `edgegap_service-1.6.1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
--rw-r--r--   0        0        0     1993 2024-05-03 20:16:05.427940 edgegap_service-1.6.0/LICENSE
--rw-r--r--   0        0        0     2188 2024-05-03 20:16:05.427940 edgegap_service-1.6.0/README.md
--rw-r--r--   0        0        0       17 2024-05-03 20:16:05.427940 edgegap_service-1.6.0/edgegap_service/BUILD
--rw-r--r--   0        0        0      225 2024-05-03 20:16:05.427940 edgegap_service-1.6.0/edgegap_service/__init__.py
--rw-r--r--   0        0        0     2931 2024-05-03 20:16:05.427940 edgegap_service-1.6.0/edgegap_service/_configuration.py
--rw-r--r--   0        0        0      735 2024-05-03 20:16:05.427940 edgegap_service-1.6.0/edgegap_service/_documentation.py
--rw-r--r--   0        0        0      717 2024-05-03 20:16:05.427940 edgegap_service-1.6.0/edgegap_service/_environment.py
--rw-r--r--   0        0        0     2890 2024-05-03 20:16:05.427940 edgegap_service-1.6.0/edgegap_service/_scheduling.py
--rw-r--r--   0        0        0     8268 2024-05-03 20:16:05.427940 edgegap_service-1.6.0/edgegap_service/_service.py
--rw-r--r--   0        0        0      739 2024-05-03 20:16:05.427940 edgegap_service-1.6.0/edgegap_service/_templating.py
--rw-r--r--   0        0        0       17 2024-05-03 20:16:05.427940 edgegap_service-1.6.0/edgegap_service/health/BUILD
--rw-r--r--   0        0        0      102 2024-05-03 20:16:05.427940 edgegap_service-1.6.0/edgegap_service/health/__init__.py
--rw-r--r--   0        0        0     1453 2024-05-03 20:16:05.427940 edgegap_service-1.6.0/edgegap_service/health/_health.py
--rw-r--r--   0        0        0      394 2024-05-03 20:16:05.427940 edgegap_service-1.6.0/edgegap_service/health/_model.py
--rw-r--r--   0        0        0       17 2024-05-03 20:16:05.427940 edgegap_service-1.6.0/edgegap_service/health/checks/BUILD
--rw-r--r--   0        0        0      300 2024-05-03 20:16:05.427940 edgegap_service-1.6.0/edgegap_service/health/checks/__init__.py
--rw-r--r--   0        0        0      594 2024-05-03 20:16:05.427940 edgegap_service-1.6.0/edgegap_service/health/checks/_consul.py
--rw-r--r--   0        0        0      740 2024-05-03 20:16:05.427940 edgegap_service-1.6.0/edgegap_service/health/checks/_database.py
--rw-r--r--   0        0        0      577 2024-05-03 20:16:05.427940 edgegap_service-1.6.0/edgegap_service/health/checks/_interface.py
--rw-r--r--   0        0        0      329 2024-05-03 20:16:05.427940 edgegap_service-1.6.0/edgegap_service/health/checks/_model.py
--rw-r--r--   0        0        0      152 2024-05-03 20:16:05.427940 edgegap_service-1.6.0/edgegap_service/logging/__init__.py
--rw-r--r--   0        0        0     2135 2024-05-03 20:16:05.427940 edgegap_service-1.6.0/edgegap_service/logging/_configuration.py
--rw-r--r--   0        0        0     1657 2024-05-03 20:16:05.427940 edgegap_service-1.6.0/edgegap_service/logging/_logger.py
--rw-r--r--   0        0        0     1880 2024-05-03 20:16:05.427940 edgegap_service-1.6.0/edgegap_service/static/html/index.html
--rw-r--r--   0        0        0     4286 2024-05-03 20:16:05.427940 edgegap_service-1.6.0/edgegap_service/static/images/favicon.ico
--rw-r--r--   0        0        0      972 2024-05-03 20:16:50.488479 edgegap_service-1.6.0/pyproject.toml
--rw-r--r--   0        0        0     3260 1970-01-01 00:00:00.000000 edgegap_service-1.6.0/PKG-INFO
+-rw-r--r--   0        0        0     1993 2024-05-04 01:16:09.258725 edgegap_service-1.6.1/LICENSE
+-rw-r--r--   0        0        0     2188 2024-05-04 01:16:09.258725 edgegap_service-1.6.1/README.md
+-rw-r--r--   0        0        0       17 2024-05-04 01:16:09.258725 edgegap_service-1.6.1/edgegap_service/BUILD
+-rw-r--r--   0        0        0      291 2024-05-04 01:16:09.258725 edgegap_service-1.6.1/edgegap_service/__init__.py
+-rw-r--r--   0        0        0     2931 2024-05-04 01:16:09.258725 edgegap_service-1.6.1/edgegap_service/_configuration.py
+-rw-r--r--   0        0        0      735 2024-05-04 01:16:09.258725 edgegap_service-1.6.1/edgegap_service/_documentation.py
+-rw-r--r--   0        0        0      717 2024-05-04 01:16:09.258725 edgegap_service-1.6.1/edgegap_service/_environment.py
+-rw-r--r--   0        0        0     2951 2024-05-04 01:16:09.258725 edgegap_service-1.6.1/edgegap_service/_scheduling.py
+-rw-r--r--   0        0        0     8268 2024-05-04 01:16:09.258725 edgegap_service-1.6.1/edgegap_service/_service.py
+-rw-r--r--   0        0        0     1019 2024-05-04 01:16:09.258725 edgegap_service-1.6.1/edgegap_service/_templating.py
+-rw-r--r--   0        0        0       17 2024-05-04 01:16:09.258725 edgegap_service-1.6.1/edgegap_service/health/BUILD
+-rw-r--r--   0        0        0      102 2024-05-04 01:16:09.258725 edgegap_service-1.6.1/edgegap_service/health/__init__.py
+-rw-r--r--   0        0        0     1453 2024-05-04 01:16:09.258725 edgegap_service-1.6.1/edgegap_service/health/_health.py
+-rw-r--r--   0        0        0      394 2024-05-04 01:16:09.258725 edgegap_service-1.6.1/edgegap_service/health/_model.py
+-rw-r--r--   0        0        0       17 2024-05-04 01:16:09.258725 edgegap_service-1.6.1/edgegap_service/health/checks/BUILD
+-rw-r--r--   0        0        0      300 2024-05-04 01:16:09.258725 edgegap_service-1.6.1/edgegap_service/health/checks/__init__.py
+-rw-r--r--   0        0        0      594 2024-05-04 01:16:09.258725 edgegap_service-1.6.1/edgegap_service/health/checks/_consul.py
+-rw-r--r--   0        0        0      740 2024-05-04 01:16:09.258725 edgegap_service-1.6.1/edgegap_service/health/checks/_database.py
+-rw-r--r--   0        0        0      577 2024-05-04 01:16:09.258725 edgegap_service-1.6.1/edgegap_service/health/checks/_interface.py
+-rw-r--r--   0        0        0      329 2024-05-04 01:16:09.258725 edgegap_service-1.6.1/edgegap_service/health/checks/_model.py
+-rw-r--r--   0        0        0      152 2024-05-04 01:16:09.258725 edgegap_service-1.6.1/edgegap_service/logging/__init__.py
+-rw-r--r--   0        0        0     2135 2024-05-04 01:16:09.258725 edgegap_service-1.6.1/edgegap_service/logging/_configuration.py
+-rw-r--r--   0        0        0     1657 2024-05-04 01:16:09.258725 edgegap_service-1.6.1/edgegap_service/logging/_logger.py
+-rw-r--r--   0        0        0     1880 2024-05-04 01:16:09.258725 edgegap_service-1.6.1/edgegap_service/static/html/index.html
+-rw-r--r--   0        0        0     4286 2024-05-04 01:16:09.258725 edgegap_service-1.6.1/edgegap_service/static/images/favicon.ico
+-rw-r--r--   0        0        0      972 2024-05-04 01:16:38.946616 edgegap_service-1.6.1/pyproject.toml
+-rw-r--r--   0        0        0     3260 1970-01-01 00:00:00.000000 edgegap_service-1.6.1/PKG-INFO
```

### Comparing `edgegap_service-1.6.0/LICENSE` & `edgegap_service-1.6.1/LICENSE`

 * *Files identical despite different names*

### Comparing `edgegap_service-1.6.0/README.md` & `edgegap_service-1.6.1/README.md`

 * *Files identical despite different names*

### Comparing `edgegap_service-1.6.0/edgegap_service/_configuration.py` & `edgegap_service-1.6.1/edgegap_service/_configuration.py`

 * *Files identical despite different names*

### Comparing `edgegap_service-1.6.0/edgegap_service/_documentation.py` & `edgegap_service-1.6.1/edgegap_service/_documentation.py`

 * *Files identical despite different names*

### Comparing `edgegap_service-1.6.0/edgegap_service/_environment.py` & `edgegap_service-1.6.1/edgegap_service/_environment.py`

 * *Files identical despite different names*

### Comparing `edgegap_service-1.6.0/edgegap_service/_scheduling.py` & `edgegap_service-1.6.1/edgegap_service/_scheduling.py`

 * *Files 2% similar despite different names*

```diff
@@ -58,14 +58,15 @@
                 return await self.__instance.stop(identifier)
             except ValueError as e:
                 raise HTTPException(status_code=404, detail=str(e))
 
         @router.post('/run/{identifier}')
         async def run_rask(identifier: str, task_parameters: TaskParameters | None) -> Task:
             try:
-                return await self.__instance.run(identifier, task_parameters.parameters)
+                params = task_parameters.parameters if task_parameters else None
+                return await self.__instance.run(identifier, params)
             except ValueError as e:
                 raise HTTPException(status_code=404, detail=str(e))
             except errors.ManualRunNotAllowedError as e:
                 raise HTTPException(status_code=403, detail=str(e))
 
         app.include_router(router)
```

### Comparing `edgegap_service-1.6.0/edgegap_service/_service.py` & `edgegap_service-1.6.1/edgegap_service/_service.py`

 * *Files identical despite different names*

### Comparing `edgegap_service-1.6.0/edgegap_service/_templating.py` & `edgegap_service-1.6.1/edgegap_service/_templating.py`

 * *Files 12% similar despite different names*

```diff
@@ -2,21 +2,29 @@
 
 from fastapi import templating
 
 from ._configuration import ServiceConfiguration
 
 
 class TemplateRenderer:
-    __templates: templating.Jinja2Templates = None
+    __templates: templating.Jinja2Templates | None = None
 
     @classmethod
     def get_templates(cls, configuration: ServiceConfiguration = None) -> templating.Jinja2Templates:
         if isinstance(configuration, ServiceConfiguration) and cls.__templates is None:
             static_folder = os.path.join(configuration.root_dir, configuration.static_dir)
             cls.__templates = templating.Jinja2Templates(directory=static_folder)
 
-        if isinstance(cls.__templates, templating.Jinja2Templates):
-            return cls.__templates
+        if not isinstance(cls.__templates, templating.Jinja2Templates):
+            raise Exception(
+                'Templating is not a Jinja2Templates instance, please pass a valid ServiceConfiguration first',
+            )
+
+        return cls.__templates
 
     @classmethod
-    def depends_templates(cls):
+    def depends_templates(cls) -> templating.Jinja2Templates:
         return cls.get_templates()
+
+    @classmethod
+    def clear_templates(cls) -> None:
+        cls.__templates = None
```

### Comparing `edgegap_service-1.6.0/edgegap_service/health/_health.py` & `edgegap_service-1.6.1/edgegap_service/health/_health.py`

 * *Files identical despite different names*

### Comparing `edgegap_service-1.6.0/edgegap_service/health/checks/_consul.py` & `edgegap_service-1.6.1/edgegap_service/health/checks/_consul.py`

 * *Files identical despite different names*

### Comparing `edgegap_service-1.6.0/edgegap_service/health/checks/_database.py` & `edgegap_service-1.6.1/edgegap_service/health/checks/_database.py`

 * *Files identical despite different names*

### Comparing `edgegap_service-1.6.0/edgegap_service/health/checks/_interface.py` & `edgegap_service-1.6.1/edgegap_service/health/checks/_interface.py`

 * *Files identical despite different names*

### Comparing `edgegap_service-1.6.0/edgegap_service/logging/_configuration.py` & `edgegap_service-1.6.1/edgegap_service/logging/_configuration.py`

 * *Files identical despite different names*

### Comparing `edgegap_service-1.6.0/edgegap_service/logging/_logger.py` & `edgegap_service-1.6.1/edgegap_service/logging/_logger.py`

 * *Files identical despite different names*

### Comparing `edgegap_service-1.6.0/edgegap_service/static/html/index.html` & `edgegap_service-1.6.1/edgegap_service/static/html/index.html`

 * *Files identical despite different names*

### Comparing `edgegap_service-1.6.0/edgegap_service/static/images/favicon.ico` & `edgegap_service-1.6.1/edgegap_service/static/images/favicon.ico`

 * *Files identical despite different names*

### Comparing `edgegap_service-1.6.0/pyproject.toml` & `edgegap_service-1.6.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "edgegap-service"
-version = "1.6.0"
+version = "1.6.1"
 description = "The Edgegap Service library includes various tools and helpers for creating FastAPI Service with easy integration. It is designed for use within the Edgegap organization."
 authors = ["Bastien Roy <bastien@edgegap.com>"]
 readme = "README.md"
 include = ["static/*"]
 
 
 [tool.poetry.dependencies]
```

### Comparing `edgegap_service-1.6.0/PKG-INFO` & `edgegap_service-1.6.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: edgegap-service
-Version: 1.6.0
+Version: 1.6.1
 Summary: The Edgegap Service library includes various tools and helpers for creating FastAPI Service with easy integration. It is designed for use within the Edgegap organization.
 Author: Bastien Roy
 Author-email: bastien@edgegap.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

