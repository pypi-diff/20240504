# Comparing `tmp/aixblock_ml-0.0.9.tar.gz` & `tmp/aixblock_ml-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aixblock_ml-0.0.9.tar", max compression
+gzip compressed data, was "aixblock_ml-0.1.0.tar", max compression
```

## Comparing `aixblock_ml-0.0.9.tar` & `aixblock_ml-0.1.0.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0      341 2024-04-16 16:09:41.363976 aixblock_ml-0.0.9/README.md
--rw-r--r--   0        0        0       84 2024-04-04 08:01:18.783734 aixblock_ml-0.0.9/aixblock_ml/__init__.py
--rw-r--r--   0        0        0    10484 2024-04-15 02:31:16.790340 aixblock_ml-0.0.9/aixblock_ml/api.py
--rw-r--r--   0        0        0      267 2024-04-01 06:20:49.118665 aixblock_ml-0.0.9/aixblock_ml/default_configs/Dockerfile
--rw-r--r--   0        0        0     2686 2024-04-15 02:26:57.535131 aixblock_ml-0.0.9/aixblock_ml/default_configs/README.md
--rw-r--r--   0        0        0     3854 2024-04-04 03:08:16.490661 aixblock_ml-0.0.9/aixblock_ml/default_configs/_wsgi.py
--rw-r--r--   0        0        0     3854 2024-04-04 03:08:16.489309 aixblock_ml-0.0.9/aixblock_ml/default_configs/_wsgi.py.tmpl
--rw-r--r--   0        0        0      559 2024-04-03 08:23:03.374688 aixblock_ml-0.0.9/aixblock_ml/default_configs/docker-compose.yml
--rw-r--r--   0        0        0     2129 2024-04-15 02:26:57.535807 aixblock_ml-0.0.9/aixblock_ml/default_configs/model.py
--rw-r--r--   0        0        0       90 2024-04-01 06:20:49.122796 aixblock_ml-0.0.9/aixblock_ml/default_configs/requirements.txt
--rw-r--r--   0        0        0     1899 2024-04-01 06:20:49.123299 aixblock_ml-0.0.9/aixblock_ml/exceptions.py
--rw-r--r--   0        0        0     2357 2024-04-01 06:43:06.660882 aixblock_ml-0.0.9/aixblock_ml/helpers.py
--rw-r--r--   0        0        0    35738 2024-04-24 07:46:56.510948 aixblock_ml-0.0.9/aixblock_ml/model.py
--rw-r--r--   0        0        0     7477 2024-04-15 02:26:57.534982 aixblock_ml-0.0.9/aixblock_ml/server.py
--rw-r--r--   0        0        0        6 2024-04-01 06:20:49.127187 aixblock_ml-0.0.9/aixblock_ml/templates/preview.html
--rw-r--r--   0        0        0     1987 2024-04-03 08:23:03.033057 aixblock_ml-0.0.9/aixblock_ml/utils.py
--rw-r--r--   0        0        0      325 2024-04-24 07:49:23.133712 aixblock_ml-0.0.9/pyproject.toml
--rw-r--r--   0        0        0      724 1970-01-01 00:00:00.000000 aixblock_ml-0.0.9/PKG-INFO
+-rw-r--r--   0        0        0      331 2024-05-04 00:02:04.849352 aixblock_ml-0.1.0/README.md
+-rw-r--r--   0        0        0       84 2024-04-25 14:31:58.829455 aixblock_ml-0.1.0/aixblock_ml/__init__.py
+-rw-r--r--   0        0        0    10484 2024-04-15 02:31:16.790340 aixblock_ml-0.1.0/aixblock_ml/api.py
+-rw-r--r--   0        0        0      267 2024-04-01 06:20:49.118665 aixblock_ml-0.1.0/aixblock_ml/default_configs/Dockerfile
+-rw-r--r--   0        0        0     2686 2024-04-15 02:26:57.535131 aixblock_ml-0.1.0/aixblock_ml/default_configs/README.md
+-rw-r--r--   0        0        0     3854 2024-05-03 23:57:13.318089 aixblock_ml-0.1.0/aixblock_ml/default_configs/_wsgi.py
+-rw-r--r--   0        0        0     3854 2024-04-04 03:08:16.489309 aixblock_ml-0.1.0/aixblock_ml/default_configs/_wsgi.py.tmpl
+-rw-r--r--   0        0        0      559 2024-04-03 08:23:03.374688 aixblock_ml-0.1.0/aixblock_ml/default_configs/docker-compose.yml
+-rw-r--r--   0        0        0     1141 2024-05-04 00:29:14.036344 aixblock_ml-0.1.0/aixblock_ml/default_configs/model.py
+-rw-r--r--   0        0        0       90 2024-04-01 06:20:49.122796 aixblock_ml-0.1.0/aixblock_ml/default_configs/requirements.txt
+-rw-r--r--   0        0        0     1899 2024-04-01 06:20:49.123299 aixblock_ml-0.1.0/aixblock_ml/exceptions.py
+-rw-r--r--   0        0        0     2357 2024-04-01 06:43:06.660882 aixblock_ml-0.1.0/aixblock_ml/helpers.py
+-rw-r--r--   0        0        0    35738 2024-04-24 07:46:56.510948 aixblock_ml-0.1.0/aixblock_ml/model.py
+-rw-r--r--   0        0        0     8882 2024-05-04 00:45:51.954615 aixblock_ml-0.1.0/aixblock_ml/server.py
+-rw-r--r--   0        0        0        6 2024-04-01 06:20:49.127187 aixblock_ml-0.1.0/aixblock_ml/templates/preview.html
+-rw-r--r--   0        0        0     1987 2024-04-03 08:23:03.033057 aixblock_ml-0.1.0/aixblock_ml/utils.py
+-rw-r--r--   0        0        0      325 2024-05-04 00:46:23.627388 aixblock_ml-0.1.0/pyproject.toml
+-rw-r--r--   0        0        0      714 1970-01-01 00:00:00.000000 aixblock_ml-0.1.0/PKG-INFO
```

### Comparing `aixblock_ml-0.0.9/aixblock_ml/api.py` & `aixblock_ml-0.1.0/aixblock_ml/api.py`

 * *Files identical despite different names*

### Comparing `aixblock_ml-0.0.9/aixblock_ml/default_configs/README.md` & `aixblock_ml-0.1.0/aixblock_ml/default_configs/README.md`

 * *Files identical despite different names*

### Comparing `aixblock_ml-0.0.9/aixblock_ml/default_configs/_wsgi.py` & `aixblock_ml-0.1.0/aixblock_ml/default_configs/_wsgi.py`

 * *Files 4% similar despite different names*

```diff
@@ -23,15 +23,15 @@
     "handlers": [
       "console"
     ],
     "propagate": True
   }}
 }})
 
-from AIXBLOCK_ml.api import init_app
+from aixblock_ml.api import init_app
 from {script} import {model_class}
 
 
 _DEFAULT_CONFIG_PATH = os.path.join(os.path.dirname(__file__), 'config.json')
 
 
 def get_kwargs_from_config(config_path=_DEFAULT_CONFIG_PATH):
```

### Comparing `aixblock_ml-0.0.9/aixblock_ml/default_configs/_wsgi.py.tmpl` & `aixblock_ml-0.1.0/aixblock_ml/default_configs/_wsgi.py.tmpl`

 * *Files identical despite different names*

### Comparing `aixblock_ml-0.0.9/aixblock_ml/default_configs/docker-compose.yml` & `aixblock_ml-0.1.0/aixblock_ml/default_configs/docker-compose.yml`

 * *Files identical despite different names*

### Comparing `aixblock_ml-0.0.9/aixblock_ml/exceptions.py` & `aixblock_ml-0.1.0/aixblock_ml/exceptions.py`

 * *Files identical despite different names*

### Comparing `aixblock_ml-0.0.9/aixblock_ml/helpers.py` & `aixblock_ml-0.1.0/aixblock_ml/helpers.py`

 * *Files identical despite different names*

### Comparing `aixblock_ml-0.0.9/aixblock_ml/model.py` & `aixblock_ml-0.1.0/aixblock_ml/model.py`

 * *Files identical despite different names*

### Comparing `aixblock_ml-0.0.9/aixblock_ml/server.py` & `aixblock_ml-0.1.0/aixblock_ml/server.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,57 +1,62 @@
+import inspect
 import os
 import subprocess
 import logging
 import argparse
 import shutil
 
 import colorama
 import re
 
 from colorama import Fore
 
-
+import os
+import logging
+import sys
+import importlib
+import importlib.util
 # from .model import get_all_classes_inherited_AIxBlockMLBase
-
+from aixblock_ml.model import AIxBlockMLBase
 
 colorama.init()
 logger = logging.getLogger(__name__)
 
 
 def get_args():
     root_parser = argparse.ArgumentParser(add_help=False)
 
     root_parser.add_argument(
         '--root-dir', dest='root_dir', default='.',
         help='Projects root directory')
 
-    parser = argparse.ArgumentParser(description='Label studio')
+    parser = argparse.ArgumentParser(description='AIxBlock')
     subparsers = parser.add_subparsers(dest='command', help='Available commands')
     subparsers.required = True
 
     # init sub-command parser
-    parser_init = subparsers.add_parser('init', help='Initialize Label Studio', parents=[root_parser])
+    parser_init = subparsers.add_parser('init', help='Initialize AIxBlock', parents=[root_parser])
     parser_init.add_argument(
         'project_name',
         help='Path to directory where project state will be initialized')
     parser_init.add_argument(
-        '--script', '--from', dest='script',
+        '--script', '--from', dest='script',default='aixblock_ml/default_configs/model.py:MyModel',
         help='Machine learning script of the following format: /my/script/path:ModelClass')
     parser_init.add_argument(
         '--force', dest='force', action='store_true',
         help='Force recreating the project if exists')
 
     # start sub-command parser
-    parser_start = subparsers.add_parser('start', help='Initialize Label Studio', parents=[root_parser])
+    parser_start = subparsers.add_parser('start', help='Initialize AIxBlock', parents=[root_parser])
     parser_start.add_argument(
         'project_name',
         help='Path to directory where project state will be initialized')
 
     # start deploy to gcp
-    parser_deploy = subparsers.add_parser('deploy', help='Deploy Label Studio', parents=[root_parser])
+    parser_deploy = subparsers.add_parser('deploy', help='Deploy AIxBlock', parents=[root_parser])
     parser_deploy.add_argument(
         'provider',
         help='Provider where to deploy')
     parser_deploy.add_argument(
         'project_name',
         help='Path to directory where project state will be initialized')
     parser_deploy.add_argument(
@@ -72,67 +77,93 @@
     parser_deploy.add_argument(
         '--aixblock-api-key', dest='AIXBLOCK_api_key', required=True,
         help='AIxBlockAPI key')
 
     args, subargs = parser.parse_known_args()
     return args, subargs
 
-
+def get_all_classes_inherited_AIxBlockMLBase(script_file):
+    names = set()
+    abs_path = os.path.abspath(script_file)
+    module_name = os.path.splitext(os.path.basename(script_file))[0]
+    sys.path.append(os.path.dirname(abs_path))
+    try:
+        module = importlib.import_module(module_name)
+    except ModuleNotFoundError as e:
+        print(Fore.RED + 'Can\'t import module "' + module_name + f'", reason: {e}.\n'
+              'If you are looking for examples, you can find a dummy model.py here:\n' +
+              Fore.LIGHTYELLOW_EX + 'https://wow-ai.com/tutorials/dummy_model.html')
+        module = None
+        exit(-1)
+
+    for name, obj in inspect.getmembers(module, inspect.isclass):
+        print(name)
+        if name == AIxBlockMLBase.__name__:
+            continue
+        if issubclass(obj, AIxBlockMLBase):
+            names.add(name)
+        for base in obj.__bases__:
+            if AIxBlockMLBase.__name__ == base.__name__:
+                names.add(name)
+    sys.path.pop()
+    return list(names)
 def create_dir(args):
     output_dir = os.path.join(args.root_dir, args.project_name)
     if os.path.exists(output_dir) and args.force:
         shutil.rmtree(output_dir)
     elif os.path.exists(output_dir):
         raise FileExistsError('Model directory already exists. Please remove it or use --force option.')
 
     default_configs_dir = os.path.join(os.path.dirname(__file__), 'default_configs')
     shutil.copytree(default_configs_dir, output_dir, ignore=shutil.ignore_patterns('*.tmpl'))
 
     # extract script name and model class
     if not args.script:
+        args.script = 'default_configs/model.py:MyModel'
         logger.warning('You don\'t specify script path: by default, "./model.py" is used')
-        script_path = 'model.py'
+        script_path = 'model.py:MyModel'
     else:
         script_path = args.script
 
     def model_def_in_path(path):
         is_windows_path = path[1:].startswith(':\\')
         return ':' in path[2:] if is_windows_path else ':' in path
 
     if model_def_in_path(script_path):
         script_path, model_class = args.script.rsplit(':', 1)
-    # else:
-    #     model_classes = get_all_classes_inherited_AIxBlockMLBase(script_path)
-    #     if len(model_classes) > 1:
-    #         raise ValueError(
-    #             'You don\'t specify target model class, and we\'ve found {num} possible candidates within {script}. '
-    #             'Please specify explicitly which one should be used using the following format:\n '
-    #             '{script}:{model_class}'.format(num=len(model_classes), script=script_path, model_class=model_classes[0]))
-    #     model_class = model_classes[0]
+    else:
+        model_classes = get_all_classes_inherited_AIxBlockMLBase(script_path)
+        if len(model_classes) > 1:
+            raise ValueError(
+                'You don\'t specify target model class, and we\'ve found {num} possible candidates within {script}. '
+                'Please specify explicitly which one should be used using the following format:\n '
+                '{script}:{model_class}'.format(num=len(model_classes), script=script_path, model_class=model_classes[0]))
+        model_class = model_classes[0]
 
     if not os.path.exists(script_path):
         raise FileNotFoundError(script_path)
 
     def use(filename):
         filepath = os.path.join(os.path.dirname(script_path), filename)
         if os.path.exists(filepath):
             shutil.copy2(filepath, output_dir)
 
     script_base_name = os.path.basename(script_path)
     use(script_base_name)
     use('requirements.txt')
     use('README.md')
-
+  
     wsgi_script_file = os.path.join(default_configs_dir, '_wsgi.py.tmpl')
     with open(wsgi_script_file) as f:
         wsgi_script = f.read()
     wsgi_script = wsgi_script.format(
         script=os.path.splitext(script_base_name)[0],
         model_class=model_class
     )
+    # wsgi_script = wsgi_script.replace("model_class", model_class).replace("script", os.path.splitext(script_base_name)[0])
     wsgi_name = os.path.basename(wsgi_script_file).split('.tmpl', 1)[0]
     with open(os.path.join(output_dir, wsgi_name), mode='w') as fout:
         fout.write(wsgi_script)
 
     print(Fore.GREEN + 'Congratulations! ML Backend has been successfully initialized in ' + output_dir)
     print(Fore.RESET + 'Now start it by using:\n' + Fore.CYAN + 'aixblock-ml start ' + output_dir)
```

### Comparing `aixblock_ml-0.0.9/aixblock_ml/utils.py` & `aixblock_ml-0.1.0/aixblock_ml/utils.py`

 * *Files identical despite different names*

### Comparing `aixblock_ml-0.0.9/PKG-INFO` & `aixblock_ml-0.1.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: aixblock_ml
-Version: 0.0.9
+Version: 0.1.0
 Summary: 
 Author: TonyShark
 Author-email: quoi@wow-ai.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Description-Content-Type: text/markdown
 
 aixblock ml
 pip install -e .
-aixblock-ml create my_ml_backend
+aixblock-ml init my_ml_backend
 aixblock-ml start my_ml_backend
 aixblock-ml start my_ml_backend -p 9091
 
 aixblock-ml deploy gcp {ml-backend-local-dir} \
 --from={model-python-script} \
 --gcp-project-id {gcp-project-id} \
---label-studio-host {https://aixblock.org} \
---label-studio-api-key {YOUR-AIXBLOCK-API-KEY}
+--aixblock-host {https://aixblock.org} \
+--aixblock-api-key {YOUR-AIXBLOCK-API-KEY}
```

