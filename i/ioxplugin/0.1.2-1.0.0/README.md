# Comparing `tmp/ioxplugin-0.1.2.tar.gz` & `tmp/ioxplugin-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ioxplugin-0.1.2.tar", last modified: Fri May  3 21:47:20 2024, max compression
+gzip compressed data, was "ioxplugin-1.0.0.tar", last modified: Fri May  3 22:50:25 2024, max compression
```

## Comparing `ioxplugin-0.1.2.tar` & `ioxplugin-1.0.0.tar`

### file list

```diff
@@ -1,34 +1,33 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 21:47:20.207457 ioxplugin-0.1.2/
--rw-r--r--   0 runner    (1001) docker     (127)      245 2024-05-03 21:47:16.000000 ioxplugin-0.1.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      653 2024-05-03 21:47:20.207457 ioxplugin-0.1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      147 2024-05-03 21:47:16.000000 ioxplugin-0.1.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 21:47:20.207457 ioxplugin-0.1.2/ioxplugin/
--rw-r--r--   0 runner    (1001) docker     (127)      165 2024-05-03 21:47:16.000000 ioxplugin-0.1.2/ioxplugin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    38141 2024-05-03 21:47:16.000000 ioxplugin-0.1.2/ioxplugin/ast_util.py
--rw-r--r--   0 runner    (1001) docker     (127)     6492 2024-05-03 21:47:16.000000 ioxplugin-0.1.2/ioxplugin/commands.py
--rw-r--r--   0 runner    (1001) docker     (127)     5298 2024-05-03 21:47:16.000000 ioxplugin-0.1.2/ioxplugin/editor.py
--rw-r--r--   0 runner    (1001) docker     (127)    10630 2024-05-03 21:47:16.000000 ioxplugin-0.1.2/ioxplugin/iox_node_gen.py
--rw-r--r--   0 runner    (1001) docker     (127)     2293 2024-05-03 21:47:16.000000 ioxplugin-0.1.2/ioxplugin/iox_profile.py
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-03 21:47:16.000000 ioxplugin-0.1.2/ioxplugin/ioxplugin.py
--rw-r--r--   0 runner    (1001) docker     (127)     1431 2024-05-03 21:47:16.000000 ioxplugin-0.1.2/ioxplugin/log.py
--rw-r--r--   0 runner    (1001) docker     (127)     2729 2024-05-03 21:47:16.000000 ioxplugin-0.1.2/ioxplugin/main_gen.py
--rw-r--r--   0 runner    (1001) docker     (127)     1034 2024-05-03 21:47:16.000000 ioxplugin-0.1.2/ioxplugin/new_project.py
--rw-r--r--   0 runner    (1001) docker     (127)     3598 2024-05-03 21:47:16.000000 ioxplugin-0.1.2/ioxplugin/node_properties.py
--rw-r--r--   0 runner    (1001) docker     (127)     6336 2024-05-03 21:47:16.000000 ioxplugin-0.1.2/ioxplugin/nodedef.py
--rw-r--r--   0 runner    (1001) docker     (127)     6319 2024-05-03 21:47:16.000000 ioxplugin-0.1.2/ioxplugin/plugin.py
--rw-r--r--   0 runner    (1001) docker     (127)     3571 2024-05-03 21:47:16.000000 ioxplugin-0.1.2/ioxplugin/plugin_meta.py
--rw-r--r--   0 runner    (1001) docker     (127)     1274 2024-05-03 21:47:16.000000 ioxplugin-0.1.2/ioxplugin/properties.py
--rw-r--r--   0 runner    (1001) docker     (127)      489 2024-05-03 21:47:16.000000 ioxplugin-0.1.2/ioxplugin/protocol.py
--rw-r--r--   0 runner    (1001) docker     (127)     2402 2024-05-03 21:47:16.000000 ioxplugin-0.1.2/ioxplugin/uom.py
--rw-r--r--   0 runner    (1001) docker     (127)      777 2024-05-03 21:47:16.000000 ioxplugin-0.1.2/ioxplugin/validator.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 21:47:20.207457 ioxplugin-0.1.2/ioxplugin.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      653 2024-05-03 21:47:20.000000 ioxplugin-0.1.2/ioxplugin.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      637 2024-05-03 21:47:20.000000 ioxplugin-0.1.2/ioxplugin.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-03 21:47:20.000000 ioxplugin-0.1.2/ioxplugin.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       28 2024-05-03 21:47:20.000000 ioxplugin-0.1.2/ioxplugin.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-03 21:47:20.000000 ioxplugin-0.1.2/ioxplugin.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-03 21:47:20.207457 ioxplugin-0.1.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      722 2024-05-03 21:47:16.000000 ioxplugin-0.1.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 21:47:20.207457 ioxplugin-0.1.2/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-03 21:47:16.000000 ioxplugin-0.1.2/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-03 21:47:16.000000 ioxplugin-0.1.2/tests/test_ioxplugin.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 22:50:25.379271 ioxplugin-1.0.0/
+-rw-r--r--   0 runner    (1001) docker     (127)      245 2024-05-03 22:50:21.000000 ioxplugin-1.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      653 2024-05-03 22:50:25.379271 ioxplugin-1.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      147 2024-05-03 22:50:21.000000 ioxplugin-1.0.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 22:50:25.379271 ioxplugin-1.0.0/ioxplugin/
+-rw-r--r--   0 runner    (1001) docker     (127)      674 2024-05-03 22:50:21.000000 ioxplugin-1.0.0/ioxplugin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    38141 2024-05-03 22:50:21.000000 ioxplugin-1.0.0/ioxplugin/ast_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6495 2024-05-03 22:50:21.000000 ioxplugin-1.0.0/ioxplugin/commands.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5300 2024-05-03 22:50:21.000000 ioxplugin-1.0.0/ioxplugin/editor.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10651 2024-05-03 22:50:21.000000 ioxplugin-1.0.0/ioxplugin/iox_node_gen.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2294 2024-05-03 22:50:21.000000 ioxplugin-1.0.0/ioxplugin/iox_profile.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1431 2024-05-03 22:50:21.000000 ioxplugin-1.0.0/ioxplugin/log.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2748 2024-05-03 22:50:21.000000 ioxplugin-1.0.0/ioxplugin/main_gen.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1034 2024-05-03 22:50:21.000000 ioxplugin-1.0.0/ioxplugin/new_project.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3601 2024-05-03 22:50:21.000000 ioxplugin-1.0.0/ioxplugin/node_properties.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6341 2024-05-03 22:50:21.000000 ioxplugin-1.0.0/ioxplugin/nodedef.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6326 2024-05-03 22:50:21.000000 ioxplugin-1.0.0/ioxplugin/plugin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3572 2024-05-03 22:50:21.000000 ioxplugin-1.0.0/ioxplugin/plugin_meta.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1275 2024-05-03 22:50:21.000000 ioxplugin-1.0.0/ioxplugin/properties.py
+-rw-r--r--   0 runner    (1001) docker     (127)      490 2024-05-03 22:50:21.000000 ioxplugin-1.0.0/ioxplugin/protocol.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2403 2024-05-03 22:50:21.000000 ioxplugin-1.0.0/ioxplugin/uom.py
+-rw-r--r--   0 runner    (1001) docker     (127)      778 2024-05-03 22:50:21.000000 ioxplugin-1.0.0/ioxplugin/validator.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 22:50:25.379271 ioxplugin-1.0.0/ioxplugin.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      653 2024-05-03 22:50:25.000000 ioxplugin-1.0.0/ioxplugin.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      614 2024-05-03 22:50:25.000000 ioxplugin-1.0.0/ioxplugin.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-03 22:50:25.000000 ioxplugin-1.0.0/ioxplugin.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-05-03 22:50:25.000000 ioxplugin-1.0.0/ioxplugin.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-03 22:50:25.000000 ioxplugin-1.0.0/ioxplugin.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-03 22:50:25.379271 ioxplugin-1.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      722 2024-05-03 22:50:21.000000 ioxplugin-1.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 22:50:25.379271 ioxplugin-1.0.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-03 22:50:21.000000 ioxplugin-1.0.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      207 2024-05-03 22:50:21.000000 ioxplugin-1.0.0/tests/test_ioxplugin.py
```

### Comparing `ioxplugin-0.1.2/PKG-INFO` & `ioxplugin-1.0.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ioxplugin
-Version: 0.1.2
+Version: 1.0.0
 Summary: IoX Plugin Helper Package
 Home-page: https://github.com/universaldevices/ioxplugin.git
 Author: Michel Kohanim
 Author-email: support@universal-devices.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `ioxplugin-0.1.2/ioxplugin/ast_util.py` & `ioxplugin-1.0.0/ioxplugin/ast_util.py`

 * *Files identical despite different names*

### Comparing `ioxplugin-0.1.2/ioxplugin/commands.py` & `ioxplugin-1.0.0/ioxplugin/commands.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,17 +3,17 @@
 """
 Class for handling node commands
 Copyright (C) 2024 Universal Devices
 """
 
 import json
 import os
-from editor import Editors 
-from log import LOGGER
-from validator import validate_id, getValidName
+from .editor import Editors 
+from .log import LOGGER
+from .validator import validate_id, getValidName
 
 
 class CommandParam:
 
     def __init__(self, param):
         self.id = None
         self.name = None
```

### Comparing `ioxplugin-0.1.2/ioxplugin/editor.py` & `ioxplugin-1.0.0/ioxplugin/editor.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,16 +3,16 @@
 """
 Plugin schema processor and validator
 Copyright (C) 2024 Universal Devices
 """
 
 import json
 import os
-from log import LOGGER
-from validator import validate_id
+from .log import LOGGER
+from .validator import validate_id
 
 class EditorDetails:
 
     def __init__(self, editor):
         self.id=None
         self.uom=None
         self.min=None
```

### Comparing `ioxplugin-0.1.2/ioxplugin/iox_node_gen.py` & `ioxplugin-1.0.0/ioxplugin/iox_node_gen.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import ast, astor
-from nodedef import NodeDefDetails, NodeProperties
-from commands import CommandDetails, CommandParam
-from log import LOGGER
-from validator import getValidName
-import ast_util 
-from uom import UOMs
-from editor import Editors
+from .nodedef import NodeDefDetails, NodeProperties
+from .commands import CommandDetails, CommandParam
+from .log import LOGGER
+from .validator import getValidName
+from ioxplugin import ast_util 
+from .uom import UOMs
+from .editor import Editors
 
 class IoXNodeGen():
     def __init__(self, nodedef:NodeDefDetails, path:str):
         if nodedef == None or path == None:
             LOGGER.critical("need node def and the path to save the python file")
             raise Exception ("need node def and the path to save the python file")
```

### Comparing `ioxplugin-0.1.2/ioxplugin/iox_profile.py` & `ioxplugin-1.0.0/ioxplugin/iox_profile.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 
 #!/usr/bin/env python3
 
 """
 Manage profiles (editor, nls, and nodedef)
 Copyright (C) 2024 Universal Devices
 """
-from log import LOGGER
+from .log import LOGGER
 import os
 
 NLS_PATH="nls"
 EDITOR_PATH="editor"
 NODEDEF_PATH="nodedef"
 
 NLS_FILE="en_us.txt"
```

### Comparing `ioxplugin-0.1.2/ioxplugin/log.py` & `ioxplugin-1.0.0/ioxplugin/log.py`

 * *Files identical despite different names*

### Comparing `ioxplugin-0.1.2/ioxplugin/main_gen.py` & `ioxplugin-1.0.0/ioxplugin/main_gen.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 
 import astor
-from nodedef import NodeDefs, NodeDefDetails, NodeProperties
-from plugin_meta import PluginMetaData
-from log import LOGGER
-import ast_util
-from iox_node_gen import IoXNodeGen
+from .nodedef import NodeDefs, NodeDefDetails, NodeProperties
+from .plugin_meta import PluginMetaData
+from .log import LOGGER
+from ioxplugin import ast_util
+from .iox_node_gen import IoXNodeGen
 
 
 class PluginMain:
     def __init__(self, path:str, plugin_info:PluginMetaData, node_defs:NodeDefs):
         self.plugin_info=plugin_info
         self.node_defs=node_defs
         self.path = path
```

### Comparing `ioxplugin-0.1.2/ioxplugin/new_project.py` & `ioxplugin-1.0.0/ioxplugin/new_project.py`

 * *Files identical despite different names*

### Comparing `ioxplugin-0.1.2/ioxplugin/node_properties.py` & `ioxplugin-1.0.0/ioxplugin/node_properties.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 #!/usr/bin/env python3
 
 """
 Class for handling node properties
 Copyright (C) 2024 Universal Devices
 """
 
-from editor import Editors
-from log import LOGGER
-from validator import validate_id 
+from .editor import Editors
+from .log import LOGGER
+from .validator import validate_id 
 
 
 
 class NodePropertyDetails:
     def __init__(self, node_property):
         self.id = None
         self.name = None
```

### Comparing `ioxplugin-0.1.2/ioxplugin/nodedef.py` & `ioxplugin-1.0.0/ioxplugin/nodedef.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 #!/usr/bin/env python3
 
 """
 Class for handling node definitions 
 Copyright (C) 2024 Universal Devices
 """
 
-from node_properties import NodeProperties
-from commands import Commands
-from log import LOGGER
-from validator import validate_id
-from protocol import Protocol
+from .node_properties import NodeProperties
+from .commands import Commands
+from .log import LOGGER
+from .validator import validate_id
+from .protocol import Protocol
 
 
 class NodeDefDetails:
     def __init__(self, node):
         self.id = None
         self.name = None
         self.parent = None
```

### Comparing `ioxplugin-0.1.2/ioxplugin/plugin.py` & `ioxplugin-1.0.0/ioxplugin/plugin.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,21 +3,21 @@
 """
 Plugin schema processor and validator
 Copyright (C) 2024 Universal Devices
 """
 
 #import fastjsonschema
 import json
-from nodedef import NodeDefs
-from editor import Editors
-from plugin_meta import PluginMetaData
-from log import init_ext_logging, LOGGER
-from iox_profile import ProfileWriter
-from iox_node_gen import IoXNodeGen
-from main_gen import PluginMain
+from .nodedef import NodeDefs
+from .editor import Editors
+from .plugin_meta import PluginMetaData
+from .log import init_ext_logging, LOGGER
+from .iox_profile import ProfileWriter
+from .iox_node_gen import IoXNodeGen
+from .main_gen import PluginMain
 import argparse
 
 
 PLUGIN_SCHEMA_FILE="schemas/plugin.schema.json"
 
 CMD_SCHEMA="schemas/commands.schema.json"
 EDITOR_SCHEMA="schemas/editor.schema.json"
```

### Comparing `ioxplugin-0.1.2/ioxplugin/plugin_meta.py` & `ioxplugin-1.0.0/ioxplugin/plugin_meta.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 #!/usr/bin/env python3
 
 """
 Class for handling plugin metadata 
 Copyright (C) 2024 Universal Devices
 """
 
-from log import LOGGER
+from .log import LOGGER
 
 class PluginMetaData:
 
     def __init__(self, metadata):
         self.metadata=metadata
 
     def getName(self):
```

### Comparing `ioxplugin-0.1.2/ioxplugin/properties.py` & `ioxplugin-1.0.0/ioxplugin/properties.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 """
 Python class representing all properties 
 Copyright (C) 2024 Universal Devices
 """
 
 import json
 import os
-from log import LOGGER
+from .log import LOGGER
 
 PROPERTIES_SCHEMA_FILE="schemas/properties.schema.json"
 
 class PropertyDetails:
     def __init__(self, elements):
         try:
             val = elements['enum'][0]
```

### Comparing `ioxplugin-0.1.2/ioxplugin/uom.py` & `ioxplugin-1.0.0/ioxplugin/uom.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 """
 Python class representing all UOMs and options
 Copyright (C) 2024 Universal Devices
 """
 
 import json
 import os
-from log import LOGGER
+from .log import LOGGER
 
 UOM_SCHEMA_FILE="schemas/uom.schema.json"
 
 INDEX_UOM = 25
 PERCENT_UOM = 51
 
 class UOMOption:
```

### Comparing `ioxplugin-0.1.2/ioxplugin/validator.py` & `ioxplugin-1.0.0/ioxplugin/validator.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 
 #!/usr/bin/env python3
 
 """
 Useful validation routines
 Copyright (C) 2024 Universal Devices
 """
-from log import LOGGER
+from .log import LOGGER
 import re
 
 def validate_id(id)->bool:
     try:
         if id == None or id == '':
             LOGGER.critical('validate_id - id does not exist ... ') 
             return False
```

### Comparing `ioxplugin-0.1.2/ioxplugin.egg-info/PKG-INFO` & `ioxplugin-1.0.0/ioxplugin.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ioxplugin
-Version: 0.1.2
+Version: 1.0.0
 Summary: IoX Plugin Helper Package
 Home-page: https://github.com/universaldevices/ioxplugin.git
 Author: Michel Kohanim
 Author-email: support@universal-devices.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `ioxplugin-0.1.2/ioxplugin.egg-info/SOURCES.txt` & `ioxplugin-1.0.0/ioxplugin.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -3,15 +3,14 @@
 setup.py
 ioxplugin/__init__.py
 ioxplugin/ast_util.py
 ioxplugin/commands.py
 ioxplugin/editor.py
 ioxplugin/iox_node_gen.py
 ioxplugin/iox_profile.py
-ioxplugin/ioxplugin.py
 ioxplugin/log.py
 ioxplugin/main_gen.py
 ioxplugin/new_project.py
 ioxplugin/node_properties.py
 ioxplugin/nodedef.py
 ioxplugin/plugin.py
 ioxplugin/plugin_meta.py
```

### Comparing `ioxplugin-0.1.2/setup.py` & `ioxplugin-1.0.0/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='ioxplugin',
-    version='0.1.2',
+    version='1.0.0',
     packages=find_packages(),
     description='IoX Plugin Helper Package',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     author='Michel Kohanim',
     author_email='support@universal-devices.com',
     url='https://github.com/universaldevices/ioxplugin.git',
```

