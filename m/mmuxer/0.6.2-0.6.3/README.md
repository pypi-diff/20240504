# Comparing `tmp/mmuxer-0.6.2.tar.gz` & `tmp/mmuxer-0.6.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mmuxer-0.6.2.tar", last modified: Thu May  2 20:11:55 2024, max compression
+gzip compressed data, was "mmuxer-0.6.3.tar", last modified: Sat May  4 16:44:06 2024, max compression
```

## Comparing `mmuxer-0.6.2.tar` & `mmuxer-0.6.3.tar`

### file list

```diff
@@ -1,33 +1,34 @@
--rw-r--r--   0        0        0    34523 2024-05-02 20:11:41.409973 mmuxer-0.6.2/LICENSE
--rw-r--r--   0        0        0     3579 2024-05-02 20:11:41.409973 mmuxer-0.6.2/README.md
--rw-r--r--   0        0        0       12 2024-05-02 20:11:41.413972 mmuxer-0.6.2/mmuxer/MANIFEST.in
--rw-r--r--   0        0        0       22 2024-05-02 20:11:53.370069 mmuxer-0.6.2/mmuxer/__init__.py
--rw-r--r--   0        0        0     2318 2024-05-02 20:11:41.413972 mmuxer-0.6.2/mmuxer/__main__.py
--rw-r--r--   0        0        0        0 2024-05-02 20:11:41.413972 mmuxer-0.6.2/mmuxer/cli/__init__.py
--rw-r--r--   0        0        0     3272 2024-05-02 20:11:41.413972 mmuxer-0.6.2/mmuxer/cli/folder.py
--rw-r--r--   0        0        0     1675 2024-05-02 20:11:41.413972 mmuxer-0.6.2/mmuxer/cli/run.py
--rw-r--r--   0        0        0      850 2024-05-02 20:11:41.413972 mmuxer-0.6.2/mmuxer/cli/sieve_export.py
--rw-r--r--   0        0        0     5588 2024-05-02 20:11:41.413972 mmuxer-0.6.2/mmuxer/config_state.py
--rw-r--r--   0        0        0     3268 2024-05-02 20:11:41.413972 mmuxer-0.6.2/mmuxer/mailbox.py
--rw-r--r--   0        0        0        0 2024-05-02 20:11:41.413972 mmuxer-0.6.2/mmuxer/models/__init__.py
--rw-r--r--   0        0        0     3042 2024-05-02 20:11:41.413972 mmuxer-0.6.2/mmuxer/models/action.py
--rw-r--r--   0        0        0      486 2024-05-02 20:11:41.413972 mmuxer-0.6.2/mmuxer/models/common.py
--rw-r--r--   0        0        0     4338 2024-05-02 20:11:41.413972 mmuxer-0.6.2/mmuxer/models/condition.py
--rw-r--r--   0        0        0      946 2024-05-02 20:11:41.413972 mmuxer-0.6.2/mmuxer/models/enums.py
--rw-r--r--   0        0        0     2309 2024-05-02 20:11:41.413972 mmuxer-0.6.2/mmuxer/models/rule.py
--rw-r--r--   0        0        0     1990 2024-05-02 20:11:41.413972 mmuxer-0.6.2/mmuxer/models/script.py
--rw-r--r--   0        0        0      797 2024-05-02 20:11:41.413972 mmuxer-0.6.2/mmuxer/models/settings.py
--rw-r--r--   0        0        0     4995 2024-05-02 20:11:41.413972 mmuxer-0.6.2/mmuxer/models/sieve.py
--rw-r--r--   0        0        0     3288 2024-05-02 20:11:41.413972 mmuxer-0.6.2/mmuxer/utils.py
--rw-r--r--   0        0        0     2133 2024-05-02 20:11:41.417972 mmuxer-0.6.2/mmuxer/workers.py
--rw-r--r--   0        0        0     1356 2024-05-02 20:11:55.558085 mmuxer-0.6.2/pyproject.toml
--rw-r--r--   0        0        0        0 2024-05-02 20:11:41.417972 mmuxer-0.6.2/tests/__init__.py
--rw-r--r--   0        0        0     1477 2024-05-02 20:11:41.417972 mmuxer-0.6.2/tests/conftest.py
--rw-r--r--   0        0        0      536 2024-05-02 20:11:41.417972 mmuxer-0.6.2/tests/data/models/rules.yaml
--rw-r--r--   0        0        0    36154 2024-05-02 20:11:41.417972 mmuxer-0.6.2/tests/imap_server.py
--rw-r--r--   0        0        0      248 2024-05-02 20:11:41.417972 mmuxer-0.6.2/tests/models/test_parse_rule.py
--rw-r--r--   0        0        0     2515 2024-05-02 20:11:41.417972 mmuxer-0.6.2/tests/models/test_sieve.py
--rw-r--r--   0        0        0     1893 2024-05-02 20:11:41.417972 mmuxer-0.6.2/tests/test_actions.py
--rw-r--r--   0        0        0     1391 2024-05-02 20:11:41.417972 mmuxer-0.6.2/tests/test_condition.py
--rw-r--r--   0        0        0     2869 2024-05-02 20:11:41.417972 mmuxer-0.6.2/tests/test_utils.py
--rw-r--r--   0        0        0     4167 1970-01-01 00:00:00.000000 mmuxer-0.6.2/PKG-INFO
+-rw-r--r--   0        0        0    34523 2024-05-04 16:43:59.000275 mmuxer-0.6.3/LICENSE
+-rw-r--r--   0        0        0     3579 2024-05-04 16:43:59.000275 mmuxer-0.6.3/README.md
+-rw-r--r--   0        0        0       12 2024-05-04 16:43:59.004275 mmuxer-0.6.3/mmuxer/MANIFEST.in
+-rw-r--r--   0        0        0       22 2024-05-04 16:44:04.392286 mmuxer-0.6.3/mmuxer/__init__.py
+-rw-r--r--   0        0        0     2318 2024-05-04 16:43:59.004275 mmuxer-0.6.3/mmuxer/__main__.py
+-rw-r--r--   0        0        0        0 2024-05-04 16:43:59.004275 mmuxer-0.6.3/mmuxer/cli/__init__.py
+-rw-r--r--   0        0        0     3271 2024-05-04 16:43:59.004275 mmuxer-0.6.3/mmuxer/cli/folder.py
+-rw-r--r--   0        0        0     1804 2024-05-04 16:43:59.004275 mmuxer-0.6.3/mmuxer/cli/run.py
+-rw-r--r--   0        0        0      850 2024-05-04 16:43:59.004275 mmuxer-0.6.3/mmuxer/cli/sieve_export.py
+-rw-r--r--   0        0        0     5588 2024-05-04 16:43:59.004275 mmuxer-0.6.3/mmuxer/config_state.py
+-rw-r--r--   0        0        0     2306 2024-05-04 16:43:59.004275 mmuxer-0.6.3/mmuxer/mailbox.py
+-rw-r--r--   0        0        0        0 2024-05-04 16:43:59.004275 mmuxer-0.6.3/mmuxer/models/__init__.py
+-rw-r--r--   0        0        0     3042 2024-05-04 16:43:59.004275 mmuxer-0.6.3/mmuxer/models/action.py
+-rw-r--r--   0        0        0      620 2024-05-04 16:43:59.004275 mmuxer-0.6.3/mmuxer/models/common.py
+-rw-r--r--   0        0        0     4355 2024-05-04 16:43:59.004275 mmuxer-0.6.3/mmuxer/models/condition.py
+-rw-r--r--   0        0        0      946 2024-05-04 16:43:59.008275 mmuxer-0.6.3/mmuxer/models/enums.py
+-rw-r--r--   0        0        0     2309 2024-05-04 16:43:59.008275 mmuxer-0.6.3/mmuxer/models/rule.py
+-rw-r--r--   0        0        0     1990 2024-05-04 16:43:59.008275 mmuxer-0.6.3/mmuxer/models/script.py
+-rw-r--r--   0        0        0      797 2024-05-04 16:43:59.008275 mmuxer-0.6.3/mmuxer/models/settings.py
+-rw-r--r--   0        0        0     4995 2024-05-04 16:43:59.008275 mmuxer-0.6.3/mmuxer/models/sieve.py
+-rw-r--r--   0        0        0     3288 2024-05-04 16:43:59.008275 mmuxer-0.6.3/mmuxer/utils.py
+-rw-r--r--   0        0        0     2133 2024-05-04 16:43:59.008275 mmuxer-0.6.3/mmuxer/workers.py
+-rw-r--r--   0        0        0     1356 2024-05-04 16:44:06.688291 mmuxer-0.6.3/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-05-04 16:43:59.008275 mmuxer-0.6.3/tests/__init__.py
+-rw-r--r--   0        0        0      920 2024-05-04 16:43:59.008275 mmuxer-0.6.3/tests/commands/test_tidy.py
+-rw-r--r--   0        0        0     1494 2024-05-04 16:43:59.008275 mmuxer-0.6.3/tests/conftest.py
+-rw-r--r--   0        0        0      536 2024-05-04 16:43:59.008275 mmuxer-0.6.3/tests/data/models/rules.yaml
+-rw-r--r--   0        0        0    36570 2024-05-04 16:43:59.008275 mmuxer-0.6.3/tests/imap_server.py
+-rw-r--r--   0        0        0      248 2024-05-04 16:43:59.008275 mmuxer-0.6.3/tests/models/test_parse_rule.py
+-rw-r--r--   0        0        0     2515 2024-05-04 16:43:59.008275 mmuxer-0.6.3/tests/models/test_sieve.py
+-rw-r--r--   0        0        0     1893 2024-05-04 16:43:59.008275 mmuxer-0.6.3/tests/test_actions.py
+-rw-r--r--   0        0        0     1391 2024-05-04 16:43:59.008275 mmuxer-0.6.3/tests/test_condition.py
+-rw-r--r--   0        0        0     2869 2024-05-04 16:43:59.008275 mmuxer-0.6.3/tests/test_utils.py
+-rw-r--r--   0        0        0     4167 1970-01-01 00:00:00.000000 mmuxer-0.6.3/PKG-INFO
```

### Comparing `mmuxer-0.6.2/LICENSE` & `mmuxer-0.6.3/LICENSE`

 * *Files identical despite different names*

### Comparing `mmuxer-0.6.2/README.md` & `mmuxer-0.6.3/README.md`

 * *Files identical despite different names*

### Comparing `mmuxer-0.6.2/mmuxer/__main__.py` & `mmuxer-0.6.3/mmuxer/__main__.py`

 * *Files identical despite different names*

### Comparing `mmuxer-0.6.2/mmuxer/cli/folder.py` & `mmuxer-0.6.3/mmuxer/cli/folder.py`

 * *Files 0% similar despite different names*

```diff
@@ -93,9 +93,9 @@
 
 @app.command(rich_help_panel="Bulk operations")
 def move_emails(source_folder: str, dest_folder: str):
     """Move all emails in `source_folder` to `dest_folder`"""
 
     box = state.mailbox
     box.folder.set(source_folder)
-    for msg in box.fetch(bulk=True):
+    for msg in box.fetch(bulk=100):
         box.move(msg.uid, dest_folder)
```

### Comparing `mmuxer-0.6.2/mmuxer/cli/run.py` & `mmuxer-0.6.3/mmuxer/cli/run.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,42 +1,50 @@
 import logging
 from pathlib import Path
+from typing import Union
 
 import typer
 
 from mmuxer.config_state import state
 from mmuxer.models.rule import apply_list
 from mmuxer.utils import config_file_typer_option
 from mmuxer.workers import MonitorWorker, WatcherWorker
 
 logger = logging.getLogger(__name__)
 
 
-def tidy(
-    config_file: Path = config_file_typer_option,
-    folder: str = typer.Option(None, help="Folder to fetch the messages from"),
-    dry_run: bool = typer.Option(False, help="Print actions instead of running them"),
+def _tidy(
+    folder: Union[str, None],
+    dry_run: bool,
 ):
-    """Run once, on all messages of the INBOX (or the given folder)."""
-    state.load_config_file(config_file)
-    state.create_mailbox()
     box = state.mailbox
     if folder is not None:
         box.folder.set(folder)
     counter = 0
-    for msg in box.fetch(bulk=True):
+    for msg in box.fetch(bulk=100):
         msg.associated_folder = folder
         apply_list(state.rules, box, msg, dry_run)
         for script in state.scripts:
             script.apply(msg, dry_run=dry_run)
         counter += 1
     print()
     print(f"{counter} messages parsed.")
 
 
+def tidy(
+    config_file: Path = config_file_typer_option,
+    folder: Union[str, None] = typer.Option(None, help="Folder to fetch the messages from"),
+    dry_run: bool = typer.Option(False, help="Print actions instead of running them"),
+):
+    """Run once, on all messages of the INBOX (or the given folder)."""
+    state.load_config_file(config_file)
+    state.create_mailbox()
+    _tidy(folder, dry_run)
+
+
 def monitor(
     config_file: Path = config_file_typer_option,
     folder: str = typer.Option(None, help="Folder to fetch the messages from"),
     dry_run: bool = typer.Option(False, help="Print actions instead of running them"),
     auto_reload: bool = typer.Option(
         False, help="Auto-reload config file on modification (EXPERIMENTAL)"
     ),
```

### Comparing `mmuxer-0.6.2/mmuxer/cli/sieve_export.py` & `mmuxer-0.6.3/mmuxer/cli/sieve_export.py`

 * *Files identical despite different names*

### Comparing `mmuxer-0.6.2/mmuxer/config_state.py` & `mmuxer-0.6.3/mmuxer/config_state.py`

 * *Files identical despite different names*

### Comparing `mmuxer-0.6.2/mmuxer/models/action.py` & `mmuxer-0.6.3/mmuxer/models/action.py`

 * *Files identical despite different names*

### Comparing `mmuxer-0.6.2/mmuxer/models/condition.py` & `mmuxer-0.6.3/mmuxer/models/condition.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 import logging
 from abc import abstractmethod
 from collections.abc import Sequence
 from typing import ForwardRef, List, Union
 
 from imap_tools import MailMessage
+from pydantic import ConfigDict
 
 from .common import BaseModel
 from .enums import ComparisonOperator
 
 
 class IBaseCondition(BaseModel):
-    class Config:
-        frozen = True
+    model_config = ConfigDict(frozen=True)
 
     operator: ComparisonOperator = ComparisonOperator.CONTAINS
 
     @abstractmethod
     def get_value(self, message: MailMessage) -> str:
         """Extract value from the message, used as value to which the rule is applied to."""
         pass
@@ -152,12 +152,12 @@
         return not self.NOT.eval(message)
 
     def to_sieve(self) -> str:
         """Used to render sieve files"""
         return f"not {self.NOT.to_sieve()}"
 
 
-All.update_forward_refs()
-Any.update_forward_refs()
-Not.update_forward_refs()
+All.model_rebuild()
+Any.model_rebuild()
+Not.model_rebuild()
 
 Condition = Union[BaseCondition, All, Any, Not]
```

### Comparing `mmuxer-0.6.2/mmuxer/models/enums.py` & `mmuxer-0.6.3/mmuxer/models/enums.py`

 * *Files identical despite different names*

### Comparing `mmuxer-0.6.2/mmuxer/models/rule.py` & `mmuxer-0.6.3/mmuxer/models/rule.py`

 * *Files identical despite different names*

### Comparing `mmuxer-0.6.2/mmuxer/models/script.py` & `mmuxer-0.6.3/mmuxer/models/script.py`

 * *Files identical despite different names*

### Comparing `mmuxer-0.6.2/mmuxer/models/settings.py` & `mmuxer-0.6.3/mmuxer/models/settings.py`

 * *Files identical despite different names*

### Comparing `mmuxer-0.6.2/mmuxer/models/sieve.py` & `mmuxer-0.6.3/mmuxer/models/sieve.py`

 * *Files identical despite different names*

### Comparing `mmuxer-0.6.2/mmuxer/utils.py` & `mmuxer-0.6.3/mmuxer/utils.py`

 * *Files identical despite different names*

### Comparing `mmuxer-0.6.2/mmuxer/workers.py` & `mmuxer-0.6.3/mmuxer/workers.py`

 * *Files identical despite different names*

### Comparing `mmuxer-0.6.2/pyproject.toml` & `mmuxer-0.6.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -7,24 +7,24 @@
 readme = "README.md"
 requires-python = ">=3.9"
 dependencies = [
     "typer[all]>=0.7, <0.8",
     "pydantic>2",
     "pydantic-settings",
     "pyyaml",
-    "imap-tools==v1.5.0",
+    "imap-tools==v1.6.0",
     "certifi",
     "watchfiles >= 0.18",
     "boolean.py >= 4.0",
 ]
 classifiers = [
     "Topic :: Communications :: Email :: Filters",
 ]
 dynamic = []
-version = "0.6.2"
+version = "0.6.3"
 
 [project.license]
 text = "AGPL-3.0"
 
 [project.scripts]
 mmuxer = "mmuxer.__main__:app"
```

### Comparing `mmuxer-0.6.2/tests/conftest.py` & `mmuxer-0.6.3/tests/conftest.py`

 * *Files 10% similar despite different names*

```diff
@@ -32,25 +32,25 @@
         return (Path(__file__).parent / "data" / filename).read_text()
 
     return inner
 
 
 @pytest.fixture
 def make_message(mailbox):
-    def inner(user="u", box="INBOX", **kwargs):
+    def inner(user="u", box="INBOX", subject="subject", **kwargs):
         if "to" in kwargs:
             assert isinstance(kwargs["to"], list), "`to` must be a list"
         payload = (
             base64.b32encode(
                 json.dumps(
                     {
                         **{
                             "to": ["to@ok.com"],
                             "from_": "from@ok.com",
-                            "subject": "subject",
+                            "subject": subject,
                         },
                         **kwargs,
                     }
                 ).encode()
             )
             .replace(b"=", b"a")
             .decode()
```

### Comparing `mmuxer-0.6.2/tests/data/models/rules.yaml` & `mmuxer-0.6.3/tests/data/models/rules.yaml`

 * *Files identical despite different names*

### Comparing `mmuxer-0.6.2/tests/imap_server.py` & `mmuxer-0.6.3/tests/imap_server.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,14 +19,15 @@
 import email
 import email.mime.multipart
 import email.mime.nonmultipart
 import json
 import logging
 import re
 import sys
+import traceback
 import uuid
 from collections import deque
 from copy import deepcopy
 from datetime import datetime, timedelta
 from email._policybase import Compat32
 from email.header import Header
 from email.message import Message
@@ -201,15 +202,15 @@
 
         return update_wrapper(wrapper, func)
 
     return decorator
 
 
 command_re = re.compile(
-    rb'((DONE)|(?P<tag>\w+) (?P<cmd>[\w]+)([\w \.#@:\*"\(\)\{\}\[\]\+\-\\\%/]+)?$)'
+    rb'((DONE)|(?P<tag>\w+) (?P<cmd>[\w]+)([\w \.#@:\*"\(\)\{\}\[\]\+\-\\\%/,]+)?$)'
 )
 FETCH_HEADERS_RE = re.compile(r".*BODY.PEEK\[HEADER.FIELDS \((?P<headers>.+)\)\].*")
 
 
 class ImapProtocol(asyncio.Protocol):
     IDLE_STILL_HERE_PERIOD_SECONDS = 10
     DEFAULT_QUOTA = 5000
@@ -244,14 +245,15 @@
     def data_received(self, data):
         print("DATA received", data, self.user_login)
         if self.append_literal_command is not None:
             self.append_literal(data)
             return
         for cmd_line in data.splitlines():
             if command_re.match(cmd_line) is None:
+                print("BAD Error in IMAP command : Unknown command (%r)." % cmd_line)
                 self.send_untagged_line(
                     "BAD Error in IMAP command : Unknown command (%r)." % cmd_line
                 )
             else:
                 command_array = [token.strip('"') for token in cmd_line.decode().rstrip().split()]
                 print("COMMANd", command_array)
                 if self.state is not IDLE:
@@ -274,15 +276,20 @@
         command = command_array[0].lower()
         parameters = command_array[1:]
         if command == "uid":
             command = command_array[1].lower()
             parameters = ["uid"] + command_array[2:]
         if not hasattr(self, command):
             return self.error(tag, 'Command "%s" not implemented' % command)
-        self.loop.call_later(self.delay_seconds, lambda: getattr(self, command)(tag, *parameters))
+        try:
+            getattr(self, command)(tag, *parameters)
+            # self.loop.call_later(self.delay_seconds, lambda: getattr(self, command)(tag, *parameters))
+        except Exception:
+            print(f"Failure when running {command} {tag} {parameters}")
+            traceback.print_exc(file=sys.stdout)
 
     def send_untagged_line(self, response, encoding="utf-8", continuation=False, max_chunk_size=0):
         self.send_raw_untagged_line(
             response.encode(encoding=encoding), continuation, max_chunk_size
         )
 
     def send_raw_untagged_line(self, raw_response, continuation=False, max_chunk_size=0):
@@ -498,14 +505,16 @@
             if match.group(2) == "*":
                 return range(start, sys.maxsize)
 
             end = int(match.group(2))
             if end <= 0 or end < start:
                 raise InvalidUidSet()
             return range(start, end + 1)
+        elif "," in uid_pattern:
+            return [int(x) for x in uid_pattern.split(",")]
         return [int(uid_pattern)]
 
     def _build_fetch_response(self, message, parts, by_uid=True):
         response = (
             ("%d FETCH (UID %s" % (message.id, message.uid)).encode()
             if by_uid
             else ("%d FETCH (" % message.id).encode()
```

### Comparing `mmuxer-0.6.2/tests/models/test_sieve.py` & `mmuxer-0.6.3/tests/models/test_sieve.py`

 * *Files identical despite different names*

### Comparing `mmuxer-0.6.2/tests/test_actions.py` & `mmuxer-0.6.3/tests/test_actions.py`

 * *Files identical despite different names*

### Comparing `mmuxer-0.6.2/tests/test_condition.py` & `mmuxer-0.6.3/tests/test_condition.py`

 * *Files identical despite different names*

### Comparing `mmuxer-0.6.2/tests/test_utils.py` & `mmuxer-0.6.3/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `mmuxer-0.6.2/PKG-INFO` & `mmuxer-0.6.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: mmuxer
-Version: 0.6.2
+Version: 0.6.3
 Summary: Manage mail from your server.
 Author-Email: Mathias Millet <mathias@mmill.eu>
 License: AGPL-3.0
 Classifier: Topic :: Communications :: Email :: Filters
 Requires-Python: >=3.9
 Requires-Dist: typer[all]<0.8,>=0.7
 Requires-Dist: pydantic>2
 Requires-Dist: pydantic-settings
 Requires-Dist: pyyaml
-Requires-Dist: imap-tools==v1.5.0
+Requires-Dist: imap-tools==v1.6.0
 Requires-Dist: certifi
 Requires-Dist: watchfiles>=0.18
 Requires-Dist: boolean.py>=4.0
 Requires-Dist: cysystemd>=1.5.0; extra == "systemd"
 Provides-Extra: systemd
 Description-Content-Type: text/markdown
```

