# Comparing `tmp/genmax-0.1.6.tar.gz` & `tmp/genmax-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "genmax-0.1.6.tar", last modified: Fri May  3 04:17:15 2024, max compression
+gzip compressed data, was "genmax-0.1.7.tar", last modified: Sat May  4 05:09:48 2024, max compression
```

## Comparing `genmax-0.1.6.tar` & `genmax-0.1.7.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 raza       (501) staff       (20)        0 2024-05-03 04:17:15.931185 genmax-0.1.6/
--rw-r--r--   0 raza       (501) staff       (20)    11342 2024-01-10 00:50:20.000000 genmax-0.1.6/LICENSE
--rw-r--r--   0 raza       (501) staff       (20)     3341 2024-05-03 04:17:15.930442 genmax-0.1.6/PKG-INFO
--rw-r--r--   0 raza       (501) staff       (20)     2714 2024-02-28 05:36:01.000000 genmax-0.1.6/README.md
-drwxr-xr-x   0 raza       (501) staff       (20)        0 2024-05-03 04:17:15.929421 genmax-0.1.6/genmax.egg-info/
--rw-r--r--   0 raza       (501) staff       (20)     3341 2024-05-03 04:17:15.000000 genmax-0.1.6/genmax.egg-info/PKG-INFO
--rw-r--r--   0 raza       (501) staff       (20)      509 2024-05-03 04:17:15.000000 genmax-0.1.6/genmax.egg-info/SOURCES.txt
--rw-r--r--   0 raza       (501) staff       (20)        1 2024-05-03 04:17:15.000000 genmax-0.1.6/genmax.egg-info/dependency_links.txt
--rw-r--r--   0 raza       (501) staff       (20)       37 2024-05-03 04:17:15.000000 genmax-0.1.6/genmax.egg-info/entry_points.txt
--rw-r--r--   0 raza       (501) staff       (20)       79 2024-05-03 04:17:15.000000 genmax-0.1.6/genmax.egg-info/requires.txt
--rw-r--r--   0 raza       (501) staff       (20)        4 2024-05-03 04:17:15.000000 genmax-0.1.6/genmax.egg-info/top_level.txt
-drwxr-xr-x   0 raza       (501) staff       (20)        0 2024-05-03 04:17:15.922685 genmax-0.1.6/gmx/
--rw-r--r--   0 raza       (501) staff       (20)        0 2024-01-10 02:41:55.000000 genmax-0.1.6/gmx/__init__.py
-drwxr-xr-x   0 raza       (501) staff       (20)        0 2024-05-03 04:17:15.924330 genmax-0.1.6/gmx/cmd/
--rw-r--r--   0 raza       (501) staff       (20)        0 2023-11-12 17:23:49.000000 genmax-0.1.6/gmx/cmd/__init__.py
--rw-r--r--   0 raza       (501) staff       (20)      843 2024-02-28 02:56:14.000000 genmax-0.1.6/gmx/cmd/initialize.py
--rw-r--r--   0 raza       (501) staff       (20)     2900 2024-01-18 05:26:27.000000 genmax-0.1.6/gmx/cmd/project.py
--rw-r--r--   0 raza       (501) staff       (20)      997 2024-02-28 02:44:15.000000 genmax-0.1.6/gmx/cmd/workflow.py
--rw-r--r--   0 raza       (501) staff       (20)     1415 2024-02-28 05:29:54.000000 genmax-0.1.6/gmx/extensions.py
-drwxr-xr-x   0 raza       (501) staff       (20)        0 2024-05-03 04:17:15.928626 genmax-0.1.6/gmx/logic/
--rw-r--r--   0 raza       (501) staff       (20)        0 2024-01-10 02:47:59.000000 genmax-0.1.6/gmx/logic/__init__.py
--rw-r--r--   0 raza       (501) staff       (20)     1091 2024-01-18 04:47:59.000000 genmax-0.1.6/gmx/logic/common.py
--rw-r--r--   0 raza       (501) staff       (20)      556 2024-02-28 02:03:08.000000 genmax-0.1.6/gmx/logic/fileops.py
--rw-r--r--   0 raza       (501) staff       (20)     2203 2024-03-09 04:30:25.000000 genmax-0.1.6/gmx/logic/generation.py
--rw-r--r--   0 raza       (501) staff       (20)     1495 2024-01-14 01:43:19.000000 genmax-0.1.6/gmx/logic/preference.py
--rw-r--r--   0 raza       (501) staff       (20)     3117 2024-05-03 04:13:58.000000 genmax-0.1.6/gmx/logic/project.py
--rw-r--r--   0 raza       (501) staff       (20)      248 2024-02-26 20:32:50.000000 genmax-0.1.6/gmx/logic/runner.py
--rw-r--r--   0 raza       (501) staff       (20)     2653 2024-05-03 04:11:30.000000 genmax-0.1.6/gmx/logic/workflow.py
--rw-r--r--   0 raza       (501) staff       (20)      582 2024-01-14 23:24:29.000000 genmax-0.1.6/gmx/main.py
--rw-r--r--   0 raza       (501) staff       (20)       38 2024-05-03 04:17:15.931420 genmax-0.1.6/setup.cfg
--rw-r--r--   0 raza       (501) staff       (20)     1046 2024-05-03 04:15:33.000000 genmax-0.1.6/setup.py
+drwxr-xr-x   0 raza       (501) staff       (20)        0 2024-05-04 05:09:48.526929 genmax-0.1.7/
+-rw-r--r--   0 raza       (501) staff       (20)    11342 2024-01-10 00:50:20.000000 genmax-0.1.7/LICENSE
+-rw-r--r--   0 raza       (501) staff       (20)     3210 2024-05-04 05:09:48.526690 genmax-0.1.7/PKG-INFO
+-rw-r--r--   0 raza       (501) staff       (20)     2718 2024-05-03 04:30:55.000000 genmax-0.1.7/README.md
+drwxr-xr-x   0 raza       (501) staff       (20)        0 2024-05-04 05:09:48.522595 genmax-0.1.7/genmax.egg-info/
+-rw-r--r--   0 raza       (501) staff       (20)     3210 2024-05-04 05:09:48.000000 genmax-0.1.7/genmax.egg-info/PKG-INFO
+-rw-r--r--   0 raza       (501) staff       (20)      509 2024-05-04 05:09:48.000000 genmax-0.1.7/genmax.egg-info/SOURCES.txt
+-rw-r--r--   0 raza       (501) staff       (20)        1 2024-05-04 05:09:48.000000 genmax-0.1.7/genmax.egg-info/dependency_links.txt
+-rw-r--r--   0 raza       (501) staff       (20)       38 2024-05-04 05:09:48.000000 genmax-0.1.7/genmax.egg-info/entry_points.txt
+-rw-r--r--   0 raza       (501) staff       (20)       79 2024-05-04 05:09:48.000000 genmax-0.1.7/genmax.egg-info/requires.txt
+-rw-r--r--   0 raza       (501) staff       (20)        4 2024-05-04 05:09:48.000000 genmax-0.1.7/genmax.egg-info/top_level.txt
+drwxr-xr-x   0 raza       (501) staff       (20)        0 2024-05-04 05:09:48.523290 genmax-0.1.7/gmx/
+-rw-r--r--   0 raza       (501) staff       (20)        0 2024-01-10 02:41:55.000000 genmax-0.1.7/gmx/__init__.py
+drwxr-xr-x   0 raza       (501) staff       (20)        0 2024-05-04 05:09:48.524340 genmax-0.1.7/gmx/cmd/
+-rw-r--r--   0 raza       (501) staff       (20)        0 2023-11-12 17:23:49.000000 genmax-0.1.7/gmx/cmd/__init__.py
+-rw-r--r--   0 raza       (501) staff       (20)      843 2024-02-28 02:56:14.000000 genmax-0.1.7/gmx/cmd/initialize.py
+-rw-r--r--   0 raza       (501) staff       (20)     2900 2024-01-18 05:26:27.000000 genmax-0.1.7/gmx/cmd/project.py
+-rw-r--r--   0 raza       (501) staff       (20)      997 2024-02-28 02:44:15.000000 genmax-0.1.7/gmx/cmd/workflow.py
+-rw-r--r--   0 raza       (501) staff       (20)     1424 2024-05-04 04:04:03.000000 genmax-0.1.7/gmx/extensions.py
+drwxr-xr-x   0 raza       (501) staff       (20)        0 2024-05-04 05:09:48.526338 genmax-0.1.7/gmx/logic/
+-rw-r--r--   0 raza       (501) staff       (20)        0 2024-01-10 02:47:59.000000 genmax-0.1.7/gmx/logic/__init__.py
+-rw-r--r--   0 raza       (501) staff       (20)     1091 2024-01-18 04:47:59.000000 genmax-0.1.7/gmx/logic/common.py
+-rw-r--r--   0 raza       (501) staff       (20)      555 2024-05-04 05:06:35.000000 genmax-0.1.7/gmx/logic/fileops.py
+-rw-r--r--   0 raza       (501) staff       (20)     2561 2024-05-04 05:06:51.000000 genmax-0.1.7/gmx/logic/generation.py
+-rw-r--r--   0 raza       (501) staff       (20)     1495 2024-01-14 01:43:19.000000 genmax-0.1.7/gmx/logic/preference.py
+-rw-r--r--   0 raza       (501) staff       (20)     3117 2024-05-03 04:13:58.000000 genmax-0.1.7/gmx/logic/project.py
+-rw-r--r--   0 raza       (501) staff       (20)      248 2024-02-26 20:32:50.000000 genmax-0.1.7/gmx/logic/runner.py
+-rw-r--r--   0 raza       (501) staff       (20)     2685 2024-05-04 05:01:54.000000 genmax-0.1.7/gmx/logic/workflow.py
+-rw-r--r--   0 raza       (501) staff       (20)      582 2024-01-14 23:24:29.000000 genmax-0.1.7/gmx/main.py
+-rw-r--r--   0 raza       (501) staff       (20)       38 2024-05-04 05:09:48.527049 genmax-0.1.7/setup.cfg
+-rw-r--r--   0 raza       (501) staff       (20)     1046 2024-05-04 05:08:03.000000 genmax-0.1.7/setup.py
```

### Comparing `genmax-0.1.6/LICENSE` & `genmax-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `genmax-0.1.6/PKG-INFO` & `genmax-0.1.7/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,39 +1,35 @@
 Metadata-Version: 2.1
 Name: genmax
-Version: 0.1.6
+Version: 0.1.7
 Summary: A simple code generation tool.
 Home-page: https://https://github.com/razaibi/genmax/
 Author: Raza Balbale
 License: Apache 2.0
 Project-URL: Documentation, https://github.com/razaibi/genmax/README.md
 Project-URL: Source, https://github.com/razaibi/genmax
 Project-URL: Tracker, https://github.com/razaibi/genmax/
 Keywords: cli code generator automation
+Platform: UNKNOWN
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: PyYAML==6.0
-Requires-Dist: Jinja2==3.1.2
-Requires-Dist: pluralizer==1.2.0
-Requires-Dist: case-switcher==1.3.13
-Requires-Dist: typer==0.9.0
 
 ### Genmax
 
 Genmax is a simple code generation tool.
 
 #### Key Components
 
 - Projects
 
 Genmax organizes all files and content in projects. Every project has itown folder. Genmax projects can be created in any folder.
 
 - Flows
 
-Genmax projects have flows to group together multiple files to be generated. Flows are in **yml** format.
+Genmax projects have flows to group together multiple files to be generated. Flows are in **yaml.j2** format.
 
 - Data
 
 You can pass data to templates that help generate data. For example, you can dynamically pass the name of attributes if you are generating a class file.
 
 - Templates
 
@@ -115,7 +111,8 @@
 | output | Name and extension of the output file. |
 |||
 | Write to File ||
 | action | The name of the write_to_file action. |
 | template | Template to write to file. |
 | output | Name and extension of the output file. |
 |||
+
```

### Comparing `genmax-0.1.6/README.md` & `genmax-0.1.7/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 - Projects
 
 Genmax organizes all files and content in projects. Every project has itown folder. Genmax projects can be created in any folder.
 
 - Flows
 
-Genmax projects have flows to group together multiple files to be generated. Flows are in **yml** format.
+Genmax projects have flows to group together multiple files to be generated. Flows are in **yaml.j2** format.
 
 - Data
 
 You can pass data to templates that help generate data. For example, you can dynamically pass the name of attributes if you are generating a class file.
 
 - Templates
```

### Comparing `genmax-0.1.6/genmax.egg-info/PKG-INFO` & `genmax-0.1.7/genmax.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,39 +1,35 @@
 Metadata-Version: 2.1
 Name: genmax
-Version: 0.1.6
+Version: 0.1.7
 Summary: A simple code generation tool.
 Home-page: https://https://github.com/razaibi/genmax/
 Author: Raza Balbale
 License: Apache 2.0
 Project-URL: Documentation, https://github.com/razaibi/genmax/README.md
 Project-URL: Source, https://github.com/razaibi/genmax
 Project-URL: Tracker, https://github.com/razaibi/genmax/
 Keywords: cli code generator automation
+Platform: UNKNOWN
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: PyYAML==6.0
-Requires-Dist: Jinja2==3.1.2
-Requires-Dist: pluralizer==1.2.0
-Requires-Dist: case-switcher==1.3.13
-Requires-Dist: typer==0.9.0
 
 ### Genmax
 
 Genmax is a simple code generation tool.
 
 #### Key Components
 
 - Projects
 
 Genmax organizes all files and content in projects. Every project has itown folder. Genmax projects can be created in any folder.
 
 - Flows
 
-Genmax projects have flows to group together multiple files to be generated. Flows are in **yml** format.
+Genmax projects have flows to group together multiple files to be generated. Flows are in **yaml.j2** format.
 
 - Data
 
 You can pass data to templates that help generate data. For example, you can dynamically pass the name of attributes if you are generating a class file.
 
 - Templates
 
@@ -115,7 +111,8 @@
 | output | Name and extension of the output file. |
 |||
 | Write to File ||
 | action | The name of the write_to_file action. |
 | template | Template to write to file. |
 | output | Name and extension of the output file. |
 |||
+
```

### Comparing `genmax-0.1.6/gmx/cmd/initialize.py` & `genmax-0.1.7/gmx/cmd/initialize.py`

 * *Files identical despite different names*

### Comparing `genmax-0.1.6/gmx/cmd/project.py` & `genmax-0.1.7/gmx/cmd/project.py`

 * *Files identical despite different names*

### Comparing `genmax-0.1.6/gmx/cmd/workflow.py` & `genmax-0.1.7/gmx/cmd/workflow.py`

 * *Files identical despite different names*

### Comparing `genmax-0.1.6/gmx/extensions.py` & `genmax-0.1.7/gmx/extensions.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,30 +1,31 @@
 from pluralizer import Pluralizer
 import caseswitcher
 import secrets
 import uuid
 
 pz = Pluralizer()
 
-def lcase(x): return x[0].lower() + x[1:]
+def lcase(x): 
+    return x[0].lower() + x[1:]
 def lowercase(x): return str(x).lower()
 def uppercase(x): return str(x).upper()
 def joinify(column_name, item_list): return ','.join(i[column_name] for i in item_list)
 def pluralize(x): return pz.pluralize(x)
 def camel(x): return caseswitcher.to_camel(x)
 def kebab(x): return caseswitcher.to_kebab(x)
 def pascale(x): return caseswitcher.to_pascal(x)
 def dot(x): return caseswitcher.to_dot(x)
 def title(x): return caseswitcher.to_title(x)
 def snake(x): return caseswitcher.to_snake(x)
 def path(x): return caseswitcher.to_path(x)
 def gen_uuid(): return str(uuid.uuid4())
 def secret(): return secrets.token_hex(16)
 def secret_complex(): return secrets.token_hex(64)
-def env(env_file_name, config_key):
+def get_env(env_file_name, config_key):
     try:
         with open(f'{env_file_name}.env', 'r') as file:
             for line in file:
                 # Splitting each line by '=' and stripping whitespace
                 key_value = line.strip().split('=', 1)
                 if len(key_value) == 2:
                     key, value = key_value
```

### Comparing `genmax-0.1.6/gmx/logic/common.py` & `genmax-0.1.7/gmx/logic/common.py`

 * *Files identical despite different names*

### Comparing `genmax-0.1.6/gmx/logic/fileops.py` & `genmax-0.1.7/gmx/logic/fileops.py`

 * *Files 22% similar despite different names*

```diff
@@ -4,16 +4,17 @@
 
 class FileOpsLogic:
     def __init__(self) -> None:
         pass
 
     @staticmethod
     def write_to_file(item):
-        env = Environment(loader=FileSystemLoader(
-            os.path.join(item['project_path'], 'templates')
-            )
+        template_path = os.path.join(
+                item['project_path'], 
+                'templates', 
+                item['template']
         )
-        template = env.get_template(item['template'])
-        # Render the template with the source data
-        output = template.render()
+        with open(template_path, 'r') as file:
+            template_content = file.read()
+        output = template_content
         CommonLogic.write_content_to_file(output, item['output'])
```

### Comparing `genmax-0.1.6/gmx/logic/generation.py` & `genmax-0.1.7/gmx/logic/generation.py`

 * *Files 17% similar despite different names*

```diff
@@ -4,16 +4,15 @@
 import gmx.extensions as ex
 from gmx.logic.common import CommonLogic
 
 class GenerationLogic:
     def __init__(self) -> None:
         pass
 
-    @staticmethod
-    def apply_extensions(env):
+    def apply_extensions(self, env):
         env.globals['lcase'] = ex.lcase
         env.globals['lowercase'] = ex.lowercase
         env.globals['uppercase'] = ex.uppercase
         env.globals['joinify'] = ex.joinify
         env.globals['pluralize'] = ex.pluralize
         env.globals['camel'] = ex.camel
         env.globals['kebab'] = ex.kebab
@@ -21,44 +20,54 @@
         env.globals['dot'] = ex.dot
         env.globals['title'] = ex.title
         env.globals['snake'] = ex.snake
         env.globals['path'] = ex.path
         env.globals['uuid'] = ex.gen_uuid
         env.globals['secret'] = ex.secret
         env.globals['secret_complex'] = ex.secret_complex
-        env.globals['env'] = ex.env
+        env.globals['get_env'] = ex.get_env
         return env
 
-    @staticmethod
-    def generate_workflow(workflow_string, flow_data):
+    def generate_workflow(self, workflow_string, flow_data):
         workflow_template = Template(workflow_string)
-        workflow_template.environment = GenerationLogic.apply_extensions(
+        workflow_template.environment = self.apply_extensions(
             workflow_template.environment
         )
         rendered_workflow = workflow_template.render(data=flow_data)
         return rendered_workflow
 
-    @staticmethod
-    def generate(item):
-        env = Environment(loader=FileSystemLoader(
-            os.path.join(item['project_path'], 'templates')
-            )
-        )
-        env = GenerationLogic.apply_extensions(env)
+    def generate(self, item):
+
         # Load the source data
+        data = None
         try:
             data_path = os.path.join(
                 item['project_path'], 
                 'data', 
                 item['data']
             )
-            with open(
-                data_path
-                ) as f:
-                data = yaml.load(f, Loader=yaml.FullLoader)                
-        except:
-            print(f'Error reading {data_path}.')
-        # Load the template
-        template = env.get_template(item['template'])
-        # Render the template with the source data
-        output = template.render(data=data)
-        CommonLogic.write_content_to_file(output, item['output'])
+            with open(data_path) as f:
+                data = yaml.load(f, Loader=yaml.FullLoader)
+        except FileNotFoundError as e:
+            print(f'Error: File {data_path} not found.')
+        except Exception as e:
+            print(f'Error: {e}')
+
+
+        if data:
+            try:
+                template_path = os.path.join(
+                        item['project_path'], 
+                        'templates', 
+                        item['template']
+                )
+                template_content=""
+                with open(template_path, 'r') as file:
+                    template_content = file.read()
+                template = Template(template_content)
+                template.environment = self.apply_extensions(
+                    template.environment
+                )
+                output = template.render(data=data)
+                CommonLogic.write_content_to_file(output, item['output'])
+            except Exception as e:
+                print(f'Error rendering template: {e}')
```

### Comparing `genmax-0.1.6/gmx/logic/preference.py` & `genmax-0.1.7/gmx/logic/preference.py`

 * *Files identical despite different names*

### Comparing `genmax-0.1.6/gmx/logic/project.py` & `genmax-0.1.7/gmx/logic/project.py`

 * *Files identical despite different names*

### Comparing `genmax-0.1.6/gmx/logic/workflow.py` & `genmax-0.1.7/gmx/logic/workflow.py`

 * *Files 8% similar despite different names*

```diff
@@ -50,16 +50,17 @@
             item['project_path'] = project_path
             self._switch_action(
                 item["action"],
                 item
             )
 
     def _switch_action(self, argument, param):
+        generator = GenerationLogic()
         switcher = {
-            "generate": GenerationLogic.generate,
+            "generate": generator.generate,
             "write_to_file": FileOpsLogic.write_to_file,
             "run_command": RunnerLogic.run_command
         }
         # Get the function from switcher dictionary
         func = switcher.get(argument, self._default_action)
         # Execute the function and return its result
         return func(param)
```

### Comparing `genmax-0.1.6/gmx/main.py` & `genmax-0.1.7/gmx/main.py`

 * *Files identical despite different names*

### Comparing `genmax-0.1.6/setup.py` & `genmax-0.1.7/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setup(
     name='genmax',
-    version='0.1.6',
+    version='0.1.7',
     author='Raza Balbale',
     description='A simple code generation tool.',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://https://github.com/razaibi/genmax/',
     project_urls={
         'Documentation': 'https://github.com/razaibi/genmax/README.md',
```

