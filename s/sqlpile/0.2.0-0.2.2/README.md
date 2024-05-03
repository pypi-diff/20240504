# Comparing `tmp/sqlpile-0.2.0.tar.gz` & `tmp/sqlpile-0.2.2.tar.gz`

## Comparing `sqlpile-0.2.0.tar` & `sqlpile-0.2.2.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0        7 2020-02-02 00:00:00.000000 sqlpile-0.2.0/.python-version
--rw-r--r--   0        0        0     2313 2020-02-02 00:00:00.000000 sqlpile-0.2.0/requirements-dev.lock
--rw-r--r--   0        0        0     2266 2020-02-02 00:00:00.000000 sqlpile-0.2.0/requirements.lock
--rw-r--r--   0        0        0       41 2020-02-02 00:00:00.000000 sqlpile-0.2.0/.vscode/settings.json
--rw-r--r--   0        0        0     8663 2020-02-02 00:00:00.000000 sqlpile-0.2.0/docs/CODE_STYLE.md
--rw-r--r--   0        0        0  2731400 2020-02-02 00:00:00.000000 sqlpile-0.2.0/docs/imgs/good-oop.png
--rw-r--r--   0        0        0       56 2020-02-02 00:00:00.000000 sqlpile-0.2.0/src/sqlpile/__init__.py
--rw-r--r--   0        0        0      574 2020-02-02 00:00:00.000000 sqlpile-0.2.0/src/sqlpile/abcs.py
--rw-r--r--   0        0        0     1845 2020-02-02 00:00:00.000000 sqlpile-0.2.0/src/sqlpile/config.py
--rw-r--r--   0        0        0    14735 2020-02-02 00:00:00.000000 sqlpile-0.2.0/src/sqlpile/core.py
--rw-r--r--   0        0        0     1231 2020-02-02 00:00:00.000000 sqlpile-0.2.0/src/sqlpile/database.py
--rw-r--r--   0        0        0     1529 2020-02-02 00:00:00.000000 sqlpile-0.2.0/src/sqlpile/main.py
--rw-r--r--   0        0        0     2014 2020-02-02 00:00:00.000000 sqlpile-0.2.0/src/sqlpile/utils.py
--rw-r--r--   0        0        0       93 2020-02-02 00:00:00.000000 sqlpile-0.2.0/.gitignore
--rw-r--r--   0        0        0     1620 2020-02-02 00:00:00.000000 sqlpile-0.2.0/README.md
--rw-r--r--   0        0        0      940 2020-02-02 00:00:00.000000 sqlpile-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     2393 2020-02-02 00:00:00.000000 sqlpile-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0        7 2020-02-02 00:00:00.000000 sqlpile-0.2.2/.python-version
+-rw-r--r--   0        0        0     2313 2020-02-02 00:00:00.000000 sqlpile-0.2.2/requirements-dev.lock
+-rw-r--r--   0        0        0     2266 2020-02-02 00:00:00.000000 sqlpile-0.2.2/requirements.lock
+-rw-r--r--   0        0        0       41 2020-02-02 00:00:00.000000 sqlpile-0.2.2/.vscode/settings.json
+-rw-r--r--   0        0        0     8663 2020-02-02 00:00:00.000000 sqlpile-0.2.2/docs/CODE_STYLE.md
+-rw-r--r--   0        0        0  2731400 2020-02-02 00:00:00.000000 sqlpile-0.2.2/docs/imgs/good-oop.png
+-rw-r--r--   0        0        0       56 2020-02-02 00:00:00.000000 sqlpile-0.2.2/src/sqlpile/__init__.py
+-rw-r--r--   0        0        0      574 2020-02-02 00:00:00.000000 sqlpile-0.2.2/src/sqlpile/abcs.py
+-rw-r--r--   0        0        0     1921 2020-02-02 00:00:00.000000 sqlpile-0.2.2/src/sqlpile/config.py
+-rw-r--r--   0        0        0    14738 2020-02-02 00:00:00.000000 sqlpile-0.2.2/src/sqlpile/core.py
+-rw-r--r--   0        0        0     1231 2020-02-02 00:00:00.000000 sqlpile-0.2.2/src/sqlpile/database.py
+-rw-r--r--   0        0        0     1529 2020-02-02 00:00:00.000000 sqlpile-0.2.2/src/sqlpile/main.py
+-rw-r--r--   0        0        0     2014 2020-02-02 00:00:00.000000 sqlpile-0.2.2/src/sqlpile/utils.py
+-rw-r--r--   0        0        0       93 2020-02-02 00:00:00.000000 sqlpile-0.2.2/.gitignore
+-rw-r--r--   0        0        0     1620 2020-02-02 00:00:00.000000 sqlpile-0.2.2/README.md
+-rw-r--r--   0        0        0      940 2020-02-02 00:00:00.000000 sqlpile-0.2.2/pyproject.toml
+-rw-r--r--   0        0        0     2393 2020-02-02 00:00:00.000000 sqlpile-0.2.2/PKG-INFO
```

### Comparing `sqlpile-0.2.0/requirements-dev.lock` & `sqlpile-0.2.2/requirements-dev.lock`

 * *Files identical despite different names*

### Comparing `sqlpile-0.2.0/requirements.lock` & `sqlpile-0.2.2/requirements.lock`

 * *Files identical despite different names*

### Comparing `sqlpile-0.2.0/docs/CODE_STYLE.md` & `sqlpile-0.2.2/docs/CODE_STYLE.md`

 * *Files identical despite different names*

### Comparing `sqlpile-0.2.0/docs/imgs/good-oop.png` & `sqlpile-0.2.2/docs/imgs/good-oop.png`

 * *Files identical despite different names*

### Comparing `sqlpile-0.2.0/src/sqlpile/abcs.py` & `sqlpile-0.2.2/src/sqlpile/abcs.py`

 * *Files identical despite different names*

### Comparing `sqlpile-0.2.0/src/sqlpile/config.py` & `sqlpile-0.2.2/src/sqlpile/config.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,17 +1,19 @@
 from functools import cached_property
 from pathlib import Path
 
 from pydantic import ConfigDict, Field, SecretStr, computed_field
-from pydantic_settings import BaseSettings
+from pydantic_settings import BaseSettings, SettingsConfigDict
 
 
 class ApplicationSettings(BaseSettings):
-    model_config: ConfigDict = ConfigDict(
-        arbitrary_types_allowed=True, case_sensitive=False
+    model_config: ConfigDict = SettingsConfigDict(
+        arbitrary_types_allowed=True,
+        case_sensitive=False,
+        env_file=(".env", ".env.dev"),
     )
     app_name: str = "sqlpile"
     database_name: str = "default"
     memory_database_type: str = "sqlite"
     local_database_type: str = "duckdb"
     app_data_dir: Path = Field(
         default_factory=lambda: Path.home() / ".app_data" / "sqlpile" / "databases"
```

### Comparing `sqlpile-0.2.0/src/sqlpile/core.py` & `sqlpile-0.2.2/src/sqlpile/core.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 import concurrent.futures
 import threading
 import time
 import uuid
-from concurrent.futures import ThreadPoolExecutor
 from contextlib import contextmanager
 from typing import Any
 
 from sqlalchemy import Sequence, create_engine
 from sqlalchemy.orm import Session, sessionmaker
 
 from sqlpile.abcs import BaseCache
@@ -67,14 +66,16 @@
                 if retry and retries < max_retries:
                     retries += 1
                     time.sleep(retry_delay)
                     retry_delay *= 2  # Exponential backoff
                     continue
                 else:
                     raise e
+            finally:
+                session.close()
 
     def get_serial_key(self, key) -> bytes:
         return create_hash_key(key)
 
     def get_serial_value(self, value) -> bytes:
         return get_serialize_value(value)
         # serialized_value = self._serializer_compressor.serialize(value)
```

### Comparing `sqlpile-0.2.0/src/sqlpile/database.py` & `sqlpile-0.2.2/src/sqlpile/database.py`

 * *Files identical despite different names*

### Comparing `sqlpile-0.2.0/src/sqlpile/main.py` & `sqlpile-0.2.2/src/sqlpile/main.py`

 * *Files identical despite different names*

### Comparing `sqlpile-0.2.0/src/sqlpile/utils.py` & `sqlpile-0.2.2/src/sqlpile/utils.py`

 * *Files identical despite different names*

### Comparing `sqlpile-0.2.0/README.md` & `sqlpile-0.2.2/README.md`

 * *Files identical despite different names*

### Comparing `sqlpile-0.2.0/pyproject.toml` & `sqlpile-0.2.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "sqlpile"
-version = "0.2.0"
+version = "0.2.2"
 description = "Add your description here"
 authors = [{ name = "Kevin Hill", email = "kivo360@gmail.com" }]
 dependencies = [
     "sqlalchemy>=2.0.29",
     "psycopg[binary]>=3.1.18",
     "cloudpickle>=3.0.0",
     "lz4>=4.3.3",
```

### Comparing `sqlpile-0.2.0/PKG-INFO` & `sqlpile-0.2.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: sqlpile
-Version: 0.2.0
+Version: 0.2.2
 Summary: Add your description here
 Author-email: Kevin Hill <kivo360@gmail.com>
 Requires-Python: >=3.8
 Requires-Dist: aiosqlite>=0.20.0
 Requires-Dist: asyncer>=0.0.7
 Requires-Dist: cloudpickle>=3.0.0
 Requires-Dist: cytoolz>=0.12.3
```

