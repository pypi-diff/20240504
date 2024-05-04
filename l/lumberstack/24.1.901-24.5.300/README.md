# Comparing `tmp/lumberstack-24.1.901.tar.gz` & `tmp/lumberstack-24.5.300.tar.gz`

## Comparing `lumberstack-24.1.901.tar` & `lumberstack-24.5.300.tar`

### file list

```diff
@@ -1,11 +1,14 @@
--rw-r--r--   0        0        0        7 2020-02-02 00:00:00.000000 lumberstack-24.1.901/.python-version
--rw-r--r--   0        0        0      592 2020-02-02 00:00:00.000000 lumberstack-24.1.901/Makefile
--rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 lumberstack-24.1.901/requirements.txt
--rw-r--r--   0        0        0      549 2020-02-02 00:00:00.000000 lumberstack-24.1.901/todo.md
--rw-r--r--   0        0        0       93 2020-02-02 00:00:00.000000 lumberstack-24.1.901/src/lumberstack/__init__.py
--rw-r--r--   0        0        0     5037 2020-02-02 00:00:00.000000 lumberstack-24.1.901/src/lumberstack/lumberstack.py
--rw-r--r--   0        0        0     3173 2020-02-02 00:00:00.000000 lumberstack-24.1.901/.gitignore
--rw-r--r--   0        0        0     1462 2020-02-02 00:00:00.000000 lumberstack-24.1.901/LICENSE
--rw-r--r--   0        0        0     1515 2020-02-02 00:00:00.000000 lumberstack-24.1.901/README.md
--rw-r--r--   0        0        0      624 2020-02-02 00:00:00.000000 lumberstack-24.1.901/pyproject.toml
--rw-r--r--   0        0        0     2073 2020-02-02 00:00:00.000000 lumberstack-24.1.901/PKG-INFO
+-rw-r--r--   0        0        0        7 2020-02-02 00:00:00.000000 lumberstack-24.5.300/.python-version
+-rw-r--r--   0        0        0      592 2020-02-02 00:00:00.000000 lumberstack-24.5.300/Makefile
+-rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 lumberstack-24.5.300/requirements.txt
+-rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 lumberstack-24.5.300/src/lumberstack/__init__.py
+-rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 lumberstack-24.5.300/src/lumberstack/constants.py
+-rw-r--r--   0        0        0      923 2020-02-02 00:00:00.000000 lumberstack-24.5.300/src/lumberstack/custom_handler.py
+-rw-r--r--   0        0        0     2994 2020-02-02 00:00:00.000000 lumberstack-24.5.300/src/lumberstack/discord.py
+-rw-r--r--   0        0        0      285 2020-02-02 00:00:00.000000 lumberstack-24.5.300/src/lumberstack/exceptions.py
+-rw-r--r--   0        0        0     7552 2020-02-02 00:00:00.000000 lumberstack-24.5.300/src/lumberstack/lumberstack.py
+-rw-r--r--   0        0        0     3173 2020-02-02 00:00:00.000000 lumberstack-24.5.300/.gitignore
+-rw-r--r--   0        0        0     1462 2020-02-02 00:00:00.000000 lumberstack-24.5.300/LICENSE
+-rw-r--r--   0        0        0     1515 2020-02-02 00:00:00.000000 lumberstack-24.5.300/README.md
+-rw-r--r--   0        0        0      624 2020-02-02 00:00:00.000000 lumberstack-24.5.300/pyproject.toml
+-rw-r--r--   0        0        0     2073 2020-02-02 00:00:00.000000 lumberstack-24.5.300/PKG-INFO
```

### Comparing `lumberstack-24.1.901/Makefile` & `lumberstack-24.5.300/Makefile`

 * *Files identical despite different names*

### Comparing `lumberstack-24.1.901/src/lumberstack/lumberstack.py` & `lumberstack-24.5.300/src/lumberstack/lumberstack.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,20 +1,41 @@
 import datetime, inspect, logging, os, sys, time, typing
 from logging import Logger, Handler
+from .constants import *
+from .custom_handler import CustomHandler
 
 # Documentation from logging library
 # CRITICAL = 50
 # FATAL = CRITICAL
 # ERROR = 40
 # WARNING = 30
 # WARN = WARNING
 # INFO = 20
 # DEBUG = 10
 # NOTSET = 0
 
+class _Dummy_Logger_:
+  def __init__(self, name: str = 'dummy') -> None:
+    self.base = logging.getLogger(name=name)
+    self.base.debug = _Dummy_Logger_._dummy_log_
+    self.base.info = _Dummy_Logger_._dummy_log_
+    self.base.warn = _Dummy_Logger_._dummy_log_
+    self.base.warning = _Dummy_Logger_._dummy_log_
+    self.base.error = _Dummy_Logger_._dummy_log_
+    self.base.critical = _Dummy_Logger_._dummy_log_
+
+  @staticmethod
+  def _dummy_log_(arg0: 'typing.any' = None, arg1: 'typing.any' = None, 
+                  arg2: 'typing.any' = None, arg3: 'typing.any' = None, 
+                  arg4: 'typing.any' = None, arg5: 'typing.any' = None):
+    pass
+
+root_formatting: logging.Formatter = DEFAULT_FORMAT_STRING
+mute_errors: bool
+
 class Lumberstack:
   last_msg: str = None
   history: list[str] = []
 
   def __init__(self, name: str = os.path.basename(inspect.stack()[1].filename), log_level_override: int = None, retain_history: bool = False, capitalize_messages: bool = True) -> None:
     
     self.name = name if 'lumberstack' not in name else os.path.basename(inspect.stack()[1].filename)
@@ -24,49 +45,81 @@
     self.base = logging.getLogger(name=self.name)
 
     if log_level_override:
       self.base.setLevel(level=log_level_override)
 
   # run once from __main__
   @staticmethod
-  def global_init(timezone: time.struct_time = time.localtime, log_filename: str = None, log_level: int = logging.INFO, format: str = '%(asctime)s %(name)s %(levelname)s: %(message)s', console_output: bool = True, custom_handlers: list[Handler] = None):
+  def global_init(timezone: time.struct_time = time.localtime, log_filename: str = None, log_level: int = logging.INFO, format_str: str = DEFAULT_FORMAT_STRING, console_output: bool = True, custom_handlers: list[logging.Handler] | list[CustomHandler] = None, mute_errors_from_lumberstack: bool = False):
 
     # initialize global instance of logger module
     logging.Formatter.converter = timezone
-    logging.basicConfig(filename=log_filename, level=log_level, format=format)
+    logging.basicConfig(filename=log_filename, level=log_level, format=format_str)
     root_logger = logging.getLogger()
-    formatting = logging.Formatter(fmt=format)
+    global root_formatting
+    root_formatting = logging.Formatter(fmt=format_str)
+    global mute_errors
+    mute_errors = mute_errors_from_lumberstack
 
     # remove default handlers
     for h in root_logger.handlers:
       root_logger.removeHandler(hdlr=h)
-    
+
     # set file handler
     if log_filename:
       fh = logging.FileHandler(filename=log_filename)
-      fh.setFormatter(formatting)
+      fh.setFormatter(root_formatting)
       root_logger.addHandler(hdlr=fh)
-      if log_level < logging.INFO:
+      if not mute_errors and log_level < logging.INFO:
         Lumberstack(name='lumberstack').debug(f'File Handler Added: {log_filename}')
-    
+
     # set console handler
     if console_output:
       ch = logging.StreamHandler(stream=sys.stdout)
-      ch.setFormatter(formatting)
+      ch.setFormatter(root_formatting)
       root_logger.addHandler(hdlr=ch)
-      if log_level < logging.INFO:
+      if not mute_errors and log_level < logging.INFO:
         Lumberstack(name='lumberstack').debug(f'Console Handler Added: STDOUT')
     
     # add custom handlers
     if custom_handlers:
-      for h in custom_handlers:
-        h.setFormatter(formatting)
-        root_logger.addHandler(hdlr=h)
-        if log_level < logging.INFO:
-          Lumberstack(name='lumberstack').debug(f'Custom Handler Added: {h.get_name()}')
+      Lumberstack.add_handlers(handlers=custom_handlers)
+
+    # mute me if you desire
+    if mute_errors:
+      Lumberstack.mute_library_logging(libraries='lumberstack')
+
+  # add a handler
+  @staticmethod
+  def add_handlers(handlers: Handler | list[Handler] | CustomHandler | list[CustomHandler]) -> None:
+    if isinstance(handlers, Handler):
+      handlers = [handlers]
+    elif isinstance(handlers, CustomHandler):
+      handlers = [handlers]
+
+    global root_formatting
+    for h in handlers:
+
+      # use our root_formatting if one has not been set
+      if not h.formatter:
+        h.setFormatter(root_formatting)
+
+      # remove timestamp if set to do so by CustomHandler
+      if isinstance(h, CustomHandler):
+        if h.remove_timestamp and h.formatter._fmt:
+          if isinstance(h.formatter._style, logging.PercentStyle):
+            h.setFormatter(logging.Formatter(h.formatter._fmt.replace('%(asctime)s', '').strip()))
+          elif isinstance(h.formatter._style, logging.StrFormatStyle):
+            h.setFormatter(logging.Formatter(h.formatter._fmt.replace('{asctime}', '').strip()))
+          elif isinstance(h.formatter._style, logging.StrFormatStyle):
+            h.setFormatter(logging.Formatter(h.formatter._fmt.replace('${asctime}', '').strip()))
+      
+      logging.getLogger().addHandler(hdlr=h)
+      Lumberstack(name='lumberstack').debug(f'Handler Added: {type(h).__name__}{" - " + h.name if h.name else ""}')
+
 
   # retrieve logger by name
   @staticmethod
   def get_logger(name: str) -> Logger:
     return logging.getLogger(name)
 
   # update log level of a list of libraries (i.e. requests)
@@ -80,31 +133,34 @@
   def force_update_library_levels(libraries: list[str] = [], log_level: int = logging.root.level):
     if log_level == 0:
       log_level = 100
     
     for l in libraries:
       logger = Lumberstack.get_logger(name=l)
       if log_level > logging.DEBUG:
-        logger.debug = Lumberstack._dummy_log_
+        logger.debug = _Dummy_Logger_._dummy_log_
       if log_level > logging.INFO:
-        logger.info = Lumberstack._dummy_log_
+        logger.info = _Dummy_Logger_._dummy_log_
       if log_level > logging.WARN:
-        logger.warn = Lumberstack._dummy_log_
-        logger.warning = Lumberstack._dummy_log_
+        logger.warn = _Dummy_Logger_._dummy_log_
+        logger.warning = _Dummy_Logger_._dummy_log_
       if log_level > logging.ERROR:
-        logger.error = Lumberstack._dummy_log_
+        logger.error = _Dummy_Logger_._dummy_log_
       if log_level > logging.FATAL:
-        logger.fatal = Lumberstack._dummy_log_
-        logger.critical = Lumberstack._dummy_log_
+        logger.fatal = _Dummy_Logger_._dummy_log_
+        logger.critical = _Dummy_Logger_._dummy_log_
 
+  # forcibly mute a logger
   @staticmethod
-  def _dummy_log_(arg0: 'typing.any' = None, arg1: 'typing.any' = None, 
-                  arg2: 'typing.any' = None, arg3: 'typing.any' = None, 
-                  arg4: 'typing.any' = None, arg5: 'typing.any' = None):
-    pass
+  def mute_library_logging(libraries: str | list[str]):
+    Lumberstack.force_update_library_levels(libraries=[libraries] if isinstance(libraries, str) else libraries, log_level=100)
+
+  @property
+  def _my_logger_(self):
+    return Lumberstack(name='lumberstack')
 
   def critical(self, msg):
     self._log_(msg=msg, level=logging.CRITICAL)
 
   def error(self, msg):
     self._log_(msg=msg, level=logging.ERROR)
 
@@ -120,15 +176,18 @@
   def _log_(self, msg: str, level: int):
     if logging.root.level <= 0 or logging.root.level > 50:
       return
 
     try:
       msg = str(msg)
     except Exception as error:
-      raise Exception(error)
+      level_name = logging.getLevelName(level=level)
+      self._my_logger_.error(f'failed to log {level_name} message, could not cast to string value... see following error for details')
+      self._my_logger_.error(str(error))
+      return
 
     if self.capitalize_messages:
       msg = f'{msg[0].upper()}{msg[1:]}'
 
     # set last message and append message history
     if logging.root.level <= level:
```

### Comparing `lumberstack-24.1.901/.gitignore` & `lumberstack-24.5.300/.gitignore`

 * *Files identical despite different names*

### Comparing `lumberstack-24.1.901/LICENSE` & `lumberstack-24.5.300/LICENSE`

 * *Files identical despite different names*

### Comparing `lumberstack-24.1.901/README.md` & `lumberstack-24.5.300/README.md`

 * *Files identical despite different names*

### Comparing `lumberstack-24.1.901/pyproject.toml` & `lumberstack-24.5.300/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "lumberstack"
-version = "24.01.0901"
+version = "24.05.0300"
 authors = [
   { name="ghostdisco", email="pypi@ghostdisco.me" },
 ]
 description = "A simple abstraction of the logging package"
 readme = "README.md"
 requires-python = ">=3.8.1"
 classifiers = [
```

### Comparing `lumberstack-24.1.901/PKG-INFO` & `lumberstack-24.5.300/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: lumberstack
-Version: 24.1.901
+Version: 24.5.300
 Summary: A simple abstraction of the logging package
 Project-URL: Homepage, https://github.com/ghostdisco/lumberstack
 Project-URL: Issues, https://github.com/ghostdisco/lumberstack/issues
 Author-email: ghostdisco <pypi@ghostdisco.me>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
```

