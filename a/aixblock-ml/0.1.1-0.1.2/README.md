# Comparing `tmp/aixblock_ml-0.1.1.tar.gz` & `tmp/aixblock_ml-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aixblock_ml-0.1.1.tar", max compression
+gzip compressed data, was "aixblock_ml-0.1.2.tar", max compression
```

## Comparing `aixblock_ml-0.1.1.tar` & `aixblock_ml-0.1.2.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0      331 2024-05-04 00:02:04.849352 aixblock_ml-0.1.1/README.md
--rw-r--r--   0        0        0       84 2024-04-25 14:31:58.829455 aixblock_ml-0.1.1/aixblock_ml/__init__.py
--rw-r--r--   0        0        0    10484 2024-04-15 02:31:16.790340 aixblock_ml-0.1.1/aixblock_ml/api.py
--rw-r--r--   0        0        0      267 2024-04-01 06:20:49.118665 aixblock_ml-0.1.1/aixblock_ml/default_configs/Dockerfile
--rw-r--r--   0        0        0     2686 2024-04-15 02:26:57.535131 aixblock_ml-0.1.1/aixblock_ml/default_configs/README.md
--rw-r--r--   0        0        0     3854 2024-05-03 23:57:13.318089 aixblock_ml-0.1.1/aixblock_ml/default_configs/_wsgi.py
--rw-r--r--   0        0        0     3854 2024-04-04 03:08:16.489309 aixblock_ml-0.1.1/aixblock_ml/default_configs/_wsgi.py.tmpl
--rw-r--r--   0        0        0      559 2024-04-03 08:23:03.374688 aixblock_ml-0.1.1/aixblock_ml/default_configs/docker-compose.yml
--rw-r--r--   0        0        0     1141 2024-05-04 00:29:14.036344 aixblock_ml-0.1.1/aixblock_ml/default_configs/model.py
--rw-r--r--   0        0        0      344 2024-05-04 00:57:37.951240 aixblock_ml-0.1.1/aixblock_ml/default_configs/requirements.txt
--rw-r--r--   0        0        0     1899 2024-04-01 06:20:49.123299 aixblock_ml-0.1.1/aixblock_ml/exceptions.py
--rw-r--r--   0        0        0     2357 2024-04-01 06:43:06.660882 aixblock_ml-0.1.1/aixblock_ml/helpers.py
--rw-r--r--   0        0        0    35738 2024-04-24 07:46:56.510948 aixblock_ml-0.1.1/aixblock_ml/model.py
--rw-r--r--   0        0        0     8882 2024-05-04 00:45:51.954615 aixblock_ml-0.1.1/aixblock_ml/server.py
--rw-r--r--   0        0        0        6 2024-04-01 06:20:49.127187 aixblock_ml-0.1.1/aixblock_ml/templates/preview.html
--rw-r--r--   0        0        0     1987 2024-04-03 08:23:03.033057 aixblock_ml-0.1.1/aixblock_ml/utils.py
--rw-r--r--   0        0        0      325 2024-05-04 01:01:19.841185 aixblock_ml-0.1.1/pyproject.toml
--rw-r--r--   0        0        0      714 1970-01-01 00:00:00.000000 aixblock_ml-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0      331 2024-05-04 00:02:04.849352 aixblock_ml-0.1.2/README.md
+-rw-r--r--   0        0        0       84 2024-04-25 14:31:58.829455 aixblock_ml-0.1.2/aixblock_ml/__init__.py
+-rw-r--r--   0        0        0    10484 2024-04-15 02:31:16.790340 aixblock_ml-0.1.2/aixblock_ml/api.py
+-rw-r--r--   0        0        0      267 2024-04-01 06:20:49.118665 aixblock_ml-0.1.2/aixblock_ml/default_configs/Dockerfile
+-rw-r--r--   0        0        0     2686 2024-04-15 02:26:57.535131 aixblock_ml-0.1.2/aixblock_ml/default_configs/README.md
+-rw-r--r--   0        0        0     3854 2024-05-03 23:57:13.318089 aixblock_ml-0.1.2/aixblock_ml/default_configs/_wsgi.py
+-rw-r--r--   0        0        0     3854 2024-04-04 03:08:16.489309 aixblock_ml-0.1.2/aixblock_ml/default_configs/_wsgi.py.tmpl
+-rw-r--r--   0        0        0      559 2024-04-03 08:23:03.374688 aixblock_ml-0.1.2/aixblock_ml/default_configs/docker-compose.yml
+-rw-r--r--   0        0        0     1141 2024-05-04 00:29:14.036344 aixblock_ml-0.1.2/aixblock_ml/default_configs/model.py
+-rw-r--r--   0        0        0      346 2024-05-04 01:19:58.591957 aixblock_ml-0.1.2/aixblock_ml/default_configs/requirements.txt
+-rw-r--r--   0        0        0     1899 2024-04-01 06:20:49.123299 aixblock_ml-0.1.2/aixblock_ml/exceptions.py
+-rw-r--r--   0        0        0     2357 2024-04-01 06:43:06.660882 aixblock_ml-0.1.2/aixblock_ml/helpers.py
+-rw-r--r--   0        0        0    35738 2024-04-24 07:46:56.510948 aixblock_ml-0.1.2/aixblock_ml/model.py
+-rw-r--r--   0        0        0     8838 2024-05-04 01:40:25.481684 aixblock_ml-0.1.2/aixblock_ml/server.py
+-rw-r--r--   0        0        0        6 2024-04-01 06:20:49.127187 aixblock_ml-0.1.2/aixblock_ml/templates/preview.html
+-rw-r--r--   0        0        0     1987 2024-04-03 08:23:03.033057 aixblock_ml-0.1.2/aixblock_ml/utils.py
+-rw-r--r--   0        0        0      325 2024-05-04 01:40:41.044977 aixblock_ml-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0      714 1970-01-01 00:00:00.000000 aixblock_ml-0.1.2/PKG-INFO
```

### Comparing `aixblock_ml-0.1.1/aixblock_ml/api.py` & `aixblock_ml-0.1.2/aixblock_ml/api.py`

 * *Files identical despite different names*

### Comparing `aixblock_ml-0.1.1/aixblock_ml/default_configs/README.md` & `aixblock_ml-0.1.2/aixblock_ml/default_configs/README.md`

 * *Files identical despite different names*

### Comparing `aixblock_ml-0.1.1/aixblock_ml/default_configs/_wsgi.py` & `aixblock_ml-0.1.2/aixblock_ml/default_configs/_wsgi.py`

 * *Files identical despite different names*

### Comparing `aixblock_ml-0.1.1/aixblock_ml/default_configs/_wsgi.py.tmpl` & `aixblock_ml-0.1.2/aixblock_ml/default_configs/_wsgi.py.tmpl`

 * *Files identical despite different names*

### Comparing `aixblock_ml-0.1.1/aixblock_ml/default_configs/docker-compose.yml` & `aixblock_ml-0.1.2/aixblock_ml/default_configs/docker-compose.yml`

 * *Files identical despite different names*

### Comparing `aixblock_ml-0.1.1/aixblock_ml/default_configs/model.py` & `aixblock_ml-0.1.2/aixblock_ml/default_configs/model.py`

 * *Files identical despite different names*

### Comparing `aixblock_ml-0.1.1/aixblock_ml/exceptions.py` & `aixblock_ml-0.1.2/aixblock_ml/exceptions.py`

 * *Files identical despite different names*

### Comparing `aixblock_ml-0.1.1/aixblock_ml/helpers.py` & `aixblock_ml-0.1.2/aixblock_ml/helpers.py`

 * *Files identical despite different names*

### Comparing `aixblock_ml-0.1.1/aixblock_ml/model.py` & `aixblock_ml-0.1.2/aixblock_ml/model.py`

 * *Files identical despite different names*

### Comparing `aixblock_ml-0.1.1/aixblock_ml/server.py` & `aixblock_ml-0.1.2/aixblock_ml/server.py`

 * *Files 2% similar despite different names*

```diff
@@ -35,15 +35,15 @@
 
     # init sub-command parser
     parser_init = subparsers.add_parser('init', help='Initialize AIxBlock', parents=[root_parser])
     parser_init.add_argument(
         'project_name',
         help='Path to directory where project state will be initialized')
     parser_init.add_argument(
-        '--script', '--from', dest='script',default='aixblock_ml/default_configs/model.py:MyModel',
+        '--script', '--from', dest='script',default='model.py:MyModel',
         help='Machine learning script of the following format: /my/script/path:ModelClass')
     parser_init.add_argument(
         '--force', dest='force', action='store_true',
         help='Force recreating the project if exists')
 
     # start sub-command parser
     parser_start = subparsers.add_parser('start', help='Initialize AIxBlock', parents=[root_parser])
@@ -114,15 +114,15 @@
         raise FileExistsError('Model directory already exists. Please remove it or use --force option.')
 
     default_configs_dir = os.path.join(os.path.dirname(__file__), 'default_configs')
     shutil.copytree(default_configs_dir, output_dir, ignore=shutil.ignore_patterns('*.tmpl'))
 
     # extract script name and model class
     if not args.script:
-        args.script = 'default_configs/model.py:MyModel'
+        args.script = 'model.py:MyModel'
         logger.warning('You don\'t specify script path: by default, "./model.py" is used')
         script_path = 'model.py:MyModel'
     else:
         script_path = args.script
 
     def model_def_in_path(path):
         is_windows_path = path[1:].startswith(':\\')
```

### Comparing `aixblock_ml-0.1.1/aixblock_ml/utils.py` & `aixblock_ml-0.1.2/aixblock_ml/utils.py`

 * *Files identical despite different names*

### Comparing `aixblock_ml-0.1.1/PKG-INFO` & `aixblock_ml-0.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aixblock_ml
-Version: 0.1.1
+Version: 0.1.2
 Summary: 
 Author: TonyShark
 Author-email: quoi@wow-ai.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

