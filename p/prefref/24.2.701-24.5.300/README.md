# Comparing `tmp/prefref-24.2.701.tar.gz` & `tmp/prefref-24.5.300.tar.gz`

## Comparing `prefref-24.2.701.tar` & `prefref-24.5.300.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0        7 2020-02-02 00:00:00.000000 prefref-24.2.701/.python-version
--rw-r--r--   0        0        0      576 2020-02-02 00:00:00.000000 prefref-24.2.701/Makefile
--rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 prefref-24.2.701/requirements.txt
--rw-r--r--   0        0        0      525 2020-02-02 00:00:00.000000 prefref-24.2.701/todo.md
--rw-r--r--   0        0        0      168 2020-02-02 00:00:00.000000 prefref-24.2.701/src/prefref/__init__.py
--rw-r--r--   0        0        0      919 2020-02-02 00:00:00.000000 prefref-24.2.701/src/prefref/examples.py
--rw-r--r--   0        0        0      882 2020-02-02 00:00:00.000000 prefref-24.2.701/src/prefref/exceptions.py
--rw-r--r--   0        0        0    18666 2020-02-02 00:00:00.000000 prefref-24.2.701/src/prefref/prefref.py
--rw-r--r--   0        0        0     3185 2020-02-02 00:00:00.000000 prefref-24.2.701/.gitignore
--rw-r--r--   0        0        0     1462 2020-02-02 00:00:00.000000 prefref-24.2.701/LICENSE
--rw-r--r--   0        0        0      897 2020-02-02 00:00:00.000000 prefref-24.2.701/README.md
--rw-r--r--   0        0        0      695 2020-02-02 00:00:00.000000 prefref-24.2.701/pyproject.toml
--rw-r--r--   0        0        0     1526 2020-02-02 00:00:00.000000 prefref-24.2.701/PKG-INFO
+-rw-r--r--   0        0        0        7 2020-02-02 00:00:00.000000 prefref-24.5.300/.python-version
+-rw-r--r--   0        0        0      576 2020-02-02 00:00:00.000000 prefref-24.5.300/Makefile
+-rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 prefref-24.5.300/requirements.txt
+-rw-r--r--   0        0        0      525 2020-02-02 00:00:00.000000 prefref-24.5.300/todo.md
+-rw-r--r--   0        0        0      168 2020-02-02 00:00:00.000000 prefref-24.5.300/src/prefref/__init__.py
+-rw-r--r--   0        0        0      919 2020-02-02 00:00:00.000000 prefref-24.5.300/src/prefref/examples.py
+-rw-r--r--   0        0        0      882 2020-02-02 00:00:00.000000 prefref-24.5.300/src/prefref/exceptions.py
+-rw-r--r--   0        0        0    18744 2020-02-02 00:00:00.000000 prefref-24.5.300/src/prefref/prefref.py
+-rw-r--r--   0        0        0     3185 2020-02-02 00:00:00.000000 prefref-24.5.300/.gitignore
+-rw-r--r--   0        0        0     1462 2020-02-02 00:00:00.000000 prefref-24.5.300/LICENSE
+-rw-r--r--   0        0        0      897 2020-02-02 00:00:00.000000 prefref-24.5.300/README.md
+-rw-r--r--   0        0        0      695 2020-02-02 00:00:00.000000 prefref-24.5.300/pyproject.toml
+-rw-r--r--   0        0        0     1526 2020-02-02 00:00:00.000000 prefref-24.5.300/PKG-INFO
```

### Comparing `prefref-24.2.701/Makefile` & `prefref-24.5.300/Makefile`

 * *Files identical despite different names*

### Comparing `prefref-24.2.701/todo.md` & `prefref-24.5.300/todo.md`

 * *Files identical despite different names*

### Comparing `prefref-24.2.701/src/prefref/examples.py` & `prefref-24.5.300/src/prefref/examples.py`

 * *Files identical despite different names*

### Comparing `prefref-24.2.701/src/prefref/exceptions.py` & `prefref-24.5.300/src/prefref/exceptions.py`

 * *Files identical despite different names*

### Comparing `prefref-24.2.701/src/prefref/prefref.py` & `prefref-24.5.300/src/prefref/prefref.py`

 * *Files 2% similar despite different names*

```diff
@@ -102,15 +102,16 @@
 
     # add a config_filepath if needed, defaulted to './config.json'
     if any(not o.no_file for o in self.__dict__.values()) and not 'config_filepath' in self.__dict__:
       self.config_filepath = Config_Option(
         name='config_filepath',
         value_type=str,
         default_value='./config.json',
-        help_text='filepath for json config file'
+        help_text='filepath for json config file',
+        value='./config.json'
       )
 
     # deny restricted option names (i.e. 'required' and 'help')
     for r in self.restricted_option_names:
       if r in self.__dict__:
         option: Config_Option = self.__dict__[r]
         if not option.no_arg_parse and (option.arg_key == None or option.arg_key == option.name):
@@ -174,19 +175,19 @@
   logger = None
 
   # config providers
   providers: list[Config_Provider] = [Config_Provider.ARG, Config_Provider.ENV, Config_Provider.JSON]
 
 
   # default constructor
-  def __init__(self, options: Config_Options, app_name: str, app_desc: str, config_filepath: str = './config.json', logger = None, providers: list[Config_Provider] = [Config_Provider.ARG, Config_Provider.ENV, Config_Provider.JSON], unknown_args_fatal: bool = False, reduce_options_to_key_value: bool = True) -> None:
+  def __init__(self, options: Config_Options, app_name: str, app_desc: str, config_filepath: str = None, logger = None, providers: list[Config_Provider] = [Config_Provider.ARG, Config_Provider.ENV, Config_Provider.JSON], unknown_args_fatal: bool = False, reduce_options_to_key_value: bool = True) -> None:
     self.options = options
     self.app_name = app_name
     self.app_desc = app_desc
-    self.config_filepath = config_filepath
+    self.config_filepath = config_filepath if config_filepath is not None else options.config_filepath.value if 'config_filepath' in options.__dict__ else './config.json'
     self.logger = _Config_Logger_(logger=logger)
     self.providers = providers
     self.unknown_console_args = []
 
     self._config_options_: Config_Options = options
     self._json_values_: dict = {}
     self._env_values_: dict = {}
@@ -200,16 +201,16 @@
     # read in default values
     for key in self.options.__dict__:
       self.options.__dict__[key].value = self.options.__dict__[key].default_value
 
 
     # json
     if Config_Provider.JSON in self.providers:
-      self.logger.debug(f'Loading JSON file: {self.options.config_filepath.value}')
-      self._json_values_ = self.initial_json_handler(config_filepath=self.options.config_filepath.value, options=self.options)
+      self.logger.debug(f'Loading JSON file: {self.config_filepath}')
+      self._json_values_ = self.initial_json_handler(config_filepath=self.config_filepath, options=self.options)
       for key in self._json_values_:
         if key in self.options.__dict__:
           self.options.__dict__[key].value = self._json_values_[key]
 
 
     # read in environment variables
     if Config_Provider.ENV in self.providers:
@@ -223,15 +224,15 @@
           # if the option is in the environment variable dictionary
           if option.env_var in os.environ:
 
             self.logger.debug(f'Found environment variable: {option.env_var}')
 
             # handle bool types differently to support 'is_flag' boolean types
             if bool == option.value_type:
-              if option.is_flag or None is os.environ[option.env_var] or '' is os.environ[option.env_var]:
+              if option.is_flag or None is os.environ[option.env_var] or '' == os.environ[option.env_var]:
                 self.options.__dict__[key].value = True
                 self._env_values_[key] = True
               else:
                 self.options.__dict__[key].value = "true" == os.environ[option.env_var].lower()
                 self._env_values_[key] = "true" == os.environ[option.env_var].lower()
 
             # cast ints and floats as such
@@ -328,15 +329,15 @@
       return self.read_json_config()
     else:
       return self.create_json_config(options=options)
   
 
   # read the json file
   def read_json_config(self) -> dict:
-    self.logger.debug(f'Reading JSON file: {self.options.config_filepath.value}')
+    self.logger.debug(f'Reading JSON file: {self.config_filepath}')
     config_json = open(self.config_filepath)
     if config_json:
       json_content = json.load(config_json)
       for key in json_content:
         value = json_content[key]
         if isinstance(value, str) and value.startswith('b"'):
           value = value.lstrip('b"').rstrip('"')
@@ -355,15 +356,15 @@
         content[key] = option.value
     self.write_json_config(content=content)
     return self.read_json_config()
 
 
   # write values to json file, converting some values for proper storage
   def write_json_config(self, content: dict = {}) -> dict:
-    self.logger.debug(f'Writing JSON file: {self.options.config_filepath.value}')
+    self.logger.debug(f'Writing JSON file: {self.config_filepath}')
     json_content = {}
     for key in content:
       value = content[key]
       if isinstance(value, bytes):
         json_content[key] = 'b"' + value.decode('utf8').replace("'", '"') + '"'
       elif isinstance(value, type(None)):
         json_content[key] = None
@@ -375,15 +376,15 @@
       else:
         json_content[key] = value
     with open(file=self.config_filepath, mode='w') as f:
       f.write(json.dumps(json_content, indent=4))
     return json_content
 
   def update_json_config(self, key: str, value: 'typing.any') -> dict:
-    self.logger.debug(f'Updating JSON file: {self.options.config_filepath.value}')
+    self.logger.debug(f'Updating JSON file: {self.config_filepath}')
     self.logger.debug(f'{key} = {value}')
     json_content = self.read_json_config()
     json_content[key] = value
     return self.write_json_config(content=json_content)
 
 
   # generate dynamic argparse
```

### Comparing `prefref-24.2.701/.gitignore` & `prefref-24.5.300/.gitignore`

 * *Files identical despite different names*

### Comparing `prefref-24.2.701/LICENSE` & `prefref-24.5.300/LICENSE`

 * *Files identical despite different names*

### Comparing `prefref-24.2.701/README.md` & `prefref-24.5.300/README.md`

 * *Files identical despite different names*

### Comparing `prefref-24.2.701/pyproject.toml` & `prefref-24.5.300/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "prefref"
-version = "24.02.0701"
+version = "24.05.0300"
 authors = [
   { name="ghostdisco", email="pypi@ghostdisco.me" },
 ]
 description = "A basic config package that reads a JSON config file, environment variables, and console arguments (prioritized in that order)"
 readme = "README.md"
 requires-python = ">=3.8.1"
 classifiers = [
```

### Comparing `prefref-24.2.701/PKG-INFO` & `prefref-24.5.300/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: prefref
-Version: 24.2.701
+Version: 24.5.300
 Summary: A basic config package that reads a JSON config file, environment variables, and console arguments (prioritized in that order)
 Project-URL: Homepage, https://github.com/ghostdisco/prefref
 Project-URL: Issues, https://github.com/ghostdisco/prefref/issues
 Author-email: ghostdisco <pypi@ghostdisco.me>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
```

