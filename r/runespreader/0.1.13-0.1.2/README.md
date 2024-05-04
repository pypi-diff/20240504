# Comparing `tmp/runespreader-0.1.13.tar.gz` & `tmp/runespreader-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "runespreader-0.1.13.tar", max compression
+gzip compressed data, was "runespreader-0.1.2.tar", max compression
```

## Comparing `runespreader-0.1.13.tar` & `runespreader-0.1.2.tar`

### file list

```diff
@@ -1,11 +1,9 @@
--rw-r--r--   0        0        0      689 2023-08-16 22:45:28.406723 runespreader-0.1.13/README.md
--rw-r--r--   0        0        0      664 2024-05-04 17:28:03.705199 runespreader-0.1.13/pyproject.toml
--rw-r--r--   0        0        0        0 2023-08-16 18:46:04.324251 runespreader-0.1.13/runespreader/__init__.py
--rw-r--r--   0        0        0     2755 2024-05-04 16:54:46.669508 runespreader-0.1.13/runespreader/bot.py
--rw-r--r--   0        0        0      857 2024-05-04 16:54:46.669508 runespreader-0.1.13/runespreader/clickhouse.py
--rw-r--r--   0        0        0     4175 2024-05-04 16:54:46.669508 runespreader-0.1.13/runespreader/spreader.py
--rw-r--r--   0        0        0     7374 2024-05-04 16:54:46.669508 runespreader-0.1.13/runespreader/spreadfinder.py
--rw-r--r--   0        0        0        0 2023-08-16 18:46:04.324251 runespreader-0.1.13/tests/__init__.py
--rw-r--r--   0        0        0     3890 2023-08-16 18:46:04.324251 runespreader-0.1.13/tests/nlp_test.py
--rw-r--r--   0        0        0     2417 2023-08-16 18:46:04.324251 runespreader-0.1.13/tests/runespreader_mock.py
--rw-r--r--   0        0        0     1515 1970-01-01 00:00:00.000000 runespreader-0.1.13/PKG-INFO
+-rw-r--r--   0        0        0      689 2023-08-16 22:45:31.558712 runespreader-0.1.2/README.md
+-rw-r--r--   0        0        0      629 2024-05-04 15:47:07.541107 runespreader-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-08-10 00:12:11.834904 runespreader-0.1.2/runespreader/__init__.py
+-rw-r--r--   0        0        0     2746 2024-05-04 15:44:33.953590 runespreader-0.1.2/runespreader/bot.py
+-rw-r--r--   0        0        0      848 2024-05-04 15:46:13.345284 runespreader-0.1.2/runespreader/clickhouse.py
+-rw-r--r--   0        0        0     4175 2024-03-31 21:45:12.882085 runespreader-0.1.2/runespreader/runespreader.py
+-rw-r--r--   0        0        0     7365 2024-05-04 15:45:40.733387 runespreader-0.1.2/runespreader/spreadfinder.py
+-rw-r--r--   0        0        0     1528 2024-05-04 15:44:54.977527 runespreader-0.1.2/runespreader/spreadseer.py
+-rw-r--r--   0        0        0     1514 1970-01-01 00:00:00.000000 runespreader-0.1.2/PKG-INFO
```

### Comparing `runespreader-0.1.13/README.md` & `runespreader-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `runespreader-0.1.13/pyproject.toml` & `runespreader-0.1.2/pyproject.toml`

 * *Files 23% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 [tool.poetry]
 name = "runespreader"
-version = "0.1.13"
+version = "0.1.2"
 description = ""
 authors = ["Charles Warren <ciwarren@mtu.edu>"]
-include = ["runespreader", "tests"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.11"
 pandas = "^2.0.3"
 clickhouse-driver = "^0.2.6"
 pyyaml = "^6.0.1"
@@ -24,9 +23,11 @@
 
 [tool.poetry.scripts]
 spreader = "runespreader.spreaderfinder:main"
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
+
+
 [tool.black]
 line-length = 80
```

### Comparing `runespreader-0.1.13/runespreader/bot.py` & `runespreader-0.1.2/runespreader/bot.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import os
 import re
 
 import discord
 import yaml
 
-from runespreader.spreader import Runespreader
+from runespreader import Runespreader
 
 
 async def parse_intent(message: str, r) -> str:
     time_expression = re.compile(r"((?:hour)|(?:minute)|(?:day)|(?:week))")
     number_expression = re.compile(r"(\d+)")
 
     def find_item(message):
```

### Comparing `runespreader-0.1.13/runespreader/clickhouse.py` & `runespreader-0.1.2/runespreader/clickhouse.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import os
 import time
 
 import pandas as pd
 import yaml
 from clickhouse_driver import Client
 
-from runespreader.spreader import Runespreader
+from runespreader import Runespreader
 
 config = yaml.load(
     open(f"{os.path.expanduser('~')}/.config/runespreader"), Loader=yaml.Loader
 )
 
 
 print("starting...")
```

### Comparing `runespreader-0.1.13/runespreader/spreader.py` & `runespreader-0.1.2/runespreader/runespreader.py`

 * *Files identical despite different names*

### Comparing `runespreader-0.1.13/runespreader/spreadfinder.py` & `runespreader-0.1.2/runespreader/spreadfinder.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 import numpy as np
 import pandas as pd
 import requests
 import yaml
 from clickhouse_driver import Client
 from requests import get
 
-from runespreader.spreader import Runespreader
+from runespreader import Runespreader
 
 
 def embed_field(name, value):
     return {"name": name, "value": value, "inline": True}
 
 
 def refresh_vol_list(config):
```

### Comparing `runespreader-0.1.13/PKG-INFO` & `runespreader-0.1.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: runespreader
-Version: 0.1.13
+Version: 0.1.2
 Summary: 
 Author: Charles Warren
 Author-email: ciwarren@mtu.edu
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: anyio (>=3.7.1,<4.0.0)
```

