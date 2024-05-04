# Comparing `tmp/thundra_ai-0.0.8.tar.gz` & `tmp/thundra_ai-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "thundra_ai-0.0.8.tar", max compression
+gzip compressed data, was "thundra_ai-0.0.9.tar", max compression
```

## Comparing `thundra_ai-0.0.8.tar` & `thundra_ai-0.0.9.tar`

### file list

```diff
@@ -1,32 +1,32 @@
--rw-r--r--   0        0        0    11357 2024-03-14 04:46:04.249062 thundra_ai-0.0.8/LICENSE
--rw-r--r--   0        0        0     2495 2024-03-14 04:46:04.249062 thundra_ai-0.0.8/README.md
--rw-r--r--   0        0        0    91913 2024-03-14 04:46:04.249062 thundra_ai-0.0.8/assets/logo.jpg
--rw-r--r--   0        0        0      872 2024-03-14 04:46:20.661187 thundra_ai-0.0.8/pyproject.toml
--rw-r--r--   0        0        0       61 2024-03-14 04:46:04.249062 thundra_ai-0.0.8/thundra/__main__.py
--rw-r--r--   0        0        0     1126 2024-03-14 04:46:04.249062 thundra_ai-0.0.8/thundra/agents.py
--rw-r--r--   0        0        0      664 2024-03-14 04:46:04.249062 thundra_ai-0.0.8/thundra/chain.py
--rw-r--r--   0        0        0     9306 2024-03-14 04:46:04.249062 thundra_ai-0.0.8/thundra/cli.py
--rw-r--r--   0        0        0     6923 2024-03-14 04:46:04.249062 thundra_ai-0.0.8/thundra/command.py
--rw-r--r--   0        0        0     1032 2024-03-14 04:46:04.249062 thundra_ai-0.0.8/thundra/config.py
--rw-r--r--   0        0        0       77 2024-03-14 04:46:04.249062 thundra_ai-0.0.8/thundra/core/__init__.py
--rw-r--r--   0        0        0     1226 2024-03-14 04:46:04.249062 thundra_ai-0.0.8/thundra/core/graph.py
--rw-r--r--   0        0        0      744 2024-03-14 04:46:04.249062 thundra_ai-0.0.8/thundra/core/llm.py
--rw-r--r--   0        0        0     2762 2024-03-14 04:46:04.249062 thundra_ai-0.0.8/thundra/core/memory.py
--rw-r--r--   0        0        0      874 2024-03-14 04:46:04.249062 thundra_ai-0.0.8/thundra/evaluater.py
--rw-r--r--   0        0        0     1381 2024-03-14 04:46:04.249062 thundra_ai-0.0.8/thundra/ipc.py
--rw-r--r--   0        0        0     2811 2024-03-14 04:46:04.249062 thundra_ai-0.0.8/thundra/middleware.py
--rw-r--r--   0        0        0     7155 2024-03-14 04:46:04.249062 thundra_ai-0.0.8/thundra/plugins.py
--rw-r--r--   0        0        0     4973 2024-03-14 04:46:04.249062 thundra_ai-0.0.8/thundra/profiler/__init__.py
--rw-r--r--   0        0        0       94 2024-03-14 04:46:04.249062 thundra_ai-0.0.8/thundra/storage/__init__.py
--rw-r--r--   0        0        0     2532 2024-03-14 04:46:04.249062 thundra_ai-0.0.8/thundra/storage/file.py
--rw-r--r--   0        0        0     2064 2024-03-14 04:46:04.249062 thundra_ai-0.0.8/thundra/templates/README.md
--rw-r--r--   0        0        0     2786 2024-03-14 04:46:04.253062 thundra_ai-0.0.8/thundra/templates/app/agents/base.py
--rw-r--r--   0        0        0     2060 2024-03-14 04:46:04.253062 thundra_ai-0.0.8/thundra/templates/app/agents/yt.py
--rw-r--r--   0        0        0     3499 2024-03-14 04:46:04.253062 thundra_ai-0.0.8/thundra/templates/app/app.py
--rw-r--r--   0        0        0     2073 2024-03-14 04:46:04.253062 thundra_ai-0.0.8/thundra/templates/app/commands/base.py
--rw-r--r--   0        0        0      683 2024-03-14 04:46:04.253062 thundra_ai-0.0.8/thundra/templates/app/middleware/auto_save_media.py
--rw-r--r--   0        0        0     1541 2024-03-14 04:46:04.253062 thundra_ai-0.0.8/thundra/templates/thundra.toml
--rw-r--r--   0        0        0     1951 2024-03-14 04:46:04.253062 thundra_ai-0.0.8/thundra/test.py
--rw-r--r--   0        0        0     1306 2024-03-14 04:46:04.253062 thundra_ai-0.0.8/thundra/types.py
--rw-r--r--   0        0        0     5774 2024-03-14 04:46:04.253062 thundra_ai-0.0.8/thundra/utils.py
--rw-r--r--   0        0        0     3391 1970-01-01 00:00:00.000000 thundra_ai-0.0.8/PKG-INFO
+-rw-r--r--   0        0        0    11357 2024-03-15 11:11:34.155304 thundra_ai-0.0.9/LICENSE
+-rw-r--r--   0        0        0     2495 2024-03-15 11:11:34.155304 thundra_ai-0.0.9/README.md
+-rw-r--r--   0        0        0    91913 2024-03-15 11:11:34.155304 thundra_ai-0.0.9/assets/logo.jpg
+-rw-r--r--   0        0        0      895 2024-03-15 11:11:46.387331 thundra_ai-0.0.9/pyproject.toml
+-rw-r--r--   0        0        0       61 2024-03-15 11:11:34.159304 thundra_ai-0.0.9/thundra/__main__.py
+-rw-r--r--   0        0        0     1126 2024-03-15 11:11:34.159304 thundra_ai-0.0.9/thundra/agents.py
+-rw-r--r--   0        0        0      664 2024-03-15 11:11:34.159304 thundra_ai-0.0.9/thundra/chain.py
+-rw-r--r--   0        0        0    10285 2024-03-15 11:11:34.159304 thundra_ai-0.0.9/thundra/cli.py
+-rw-r--r--   0        0        0     6923 2024-03-15 11:11:34.159304 thundra_ai-0.0.9/thundra/command.py
+-rw-r--r--   0        0        0     1032 2024-03-15 11:11:34.159304 thundra_ai-0.0.9/thundra/config.py
+-rw-r--r--   0        0        0       77 2024-03-15 11:11:34.159304 thundra_ai-0.0.9/thundra/core/__init__.py
+-rw-r--r--   0        0        0     1226 2024-03-15 11:11:34.159304 thundra_ai-0.0.9/thundra/core/graph.py
+-rw-r--r--   0        0        0      744 2024-03-15 11:11:34.159304 thundra_ai-0.0.9/thundra/core/llm.py
+-rw-r--r--   0        0        0     2762 2024-03-15 11:11:34.159304 thundra_ai-0.0.9/thundra/core/memory.py
+-rw-r--r--   0        0        0      874 2024-03-15 11:11:34.159304 thundra_ai-0.0.9/thundra/evaluater.py
+-rw-r--r--   0        0        0     1381 2024-03-15 11:11:34.159304 thundra_ai-0.0.9/thundra/ipc.py
+-rw-r--r--   0        0        0     2811 2024-03-15 11:11:34.159304 thundra_ai-0.0.9/thundra/middleware.py
+-rw-r--r--   0        0        0     7155 2024-03-15 11:11:34.159304 thundra_ai-0.0.9/thundra/plugins.py
+-rw-r--r--   0        0        0     4973 2024-03-15 11:11:34.159304 thundra_ai-0.0.9/thundra/profiler/__init__.py
+-rw-r--r--   0        0        0       94 2024-03-15 11:11:34.159304 thundra_ai-0.0.9/thundra/storage/__init__.py
+-rw-r--r--   0        0        0     2532 2024-03-15 11:11:34.159304 thundra_ai-0.0.9/thundra/storage/file.py
+-rw-r--r--   0        0        0     2064 2024-03-15 11:11:34.159304 thundra_ai-0.0.9/thundra/templates/README.md
+-rw-r--r--   0        0        0     2786 2024-03-15 11:11:34.159304 thundra_ai-0.0.9/thundra/templates/app/agents/base.py
+-rw-r--r--   0        0        0     2060 2024-03-15 11:11:34.159304 thundra_ai-0.0.9/thundra/templates/app/agents/yt.py
+-rw-r--r--   0        0        0     3348 2024-03-15 11:11:34.159304 thundra_ai-0.0.9/thundra/templates/app/app.py
+-rw-r--r--   0        0        0     2073 2024-03-15 11:11:34.159304 thundra_ai-0.0.9/thundra/templates/app/commands/base.py
+-rw-r--r--   0        0        0      683 2024-03-15 11:11:34.159304 thundra_ai-0.0.9/thundra/templates/app/middleware/auto_save_media.py
+-rw-r--r--   0        0        0     1541 2024-03-15 11:11:34.159304 thundra_ai-0.0.9/thundra/templates/thundra.toml
+-rw-r--r--   0        0        0     1951 2024-03-15 11:11:34.159304 thundra_ai-0.0.9/thundra/test.py
+-rw-r--r--   0        0        0     1306 2024-03-15 11:11:34.159304 thundra_ai-0.0.9/thundra/types.py
+-rw-r--r--   0        0        0     5774 2024-03-15 11:11:34.159304 thundra_ai-0.0.9/thundra/utils.py
+-rw-r--r--   0        0        0     3436 1970-01-01 00:00:00.000000 thundra_ai-0.0.9/PKG-INFO
```

### Comparing `thundra_ai-0.0.8/LICENSE` & `thundra_ai-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `thundra_ai-0.0.8/README.md` & `thundra_ai-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `thundra_ai-0.0.8/assets/logo.jpg` & `thundra_ai-0.0.9/assets/logo.jpg`

 * *Files identical despite different names*

### Comparing `thundra_ai-0.0.8/pyproject.toml` & `thundra_ai-0.0.9/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "thundra-ai"
-version = "0.0.8"
+version = "0.0.9"
 description = "Neonize Abstraction"
 authors = ["krypton-byte <rosid6434@gmail.com>"]
 license = "Apache 2.0"
 readme = "README.md"
 packages = [{include="thundra"}]
 include=[
     "assets/logo.jpg"
@@ -19,14 +19,15 @@
 neonize = "^0.0.9"
 pytube = "^15.0.0"
 langchain = "^0.1.11"
 tomli-w = "^1.0.0"
 langchain-openai = "^0.0.8"
 graphviz = "^0.20.1"
 appdirs = "^1.4.4"
+watchfiles = "^0.21.0"
 
 
 [[tool.poetry.source]]
 name = "thundra-ai"
 url = "https://github.com/krypton-byte/thundra"
 priority = "primary"
```

### Comparing `thundra_ai-0.0.8/thundra/agents.py` & `thundra_ai-0.0.9/thundra/agents.py`

 * *Files identical despite different names*

### Comparing `thundra_ai-0.0.8/thundra/chain.py` & `thundra_ai-0.0.9/thundra/chain.py`

 * *Files identical despite different names*

### Comparing `thundra_ai-0.0.8/thundra/cli.py` & `thundra_ai-0.0.9/thundra/cli.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,32 +1,39 @@
 from pathlib import Path
 from typing import List
 import zipfile
 from neonize.client import re
+import logging
 from tomli_w import dumps
-
+import shlex
 import argparse, os
 import tomllib
 import shutil
 import sys
 import os
-
+from neonize.utils import log
 from thundra.profiler import Profiler, VirtualEnv
-
+import watchfiles
 
 arg = argparse.ArgumentParser()
 action = arg.add_subparsers(title="action", dest="action", required=True)
 action.add_parser("install")
 create = action.add_parser(name="create")
 create.add_argument("--name", type=str, nargs=1)
 
 run = action.add_parser(name="run")
 run.add_argument(
     "--phone-number", type=str, help="using pairphone as authentication, default qr"
 )
+run.add_argument(
+    "--dev", action="store_true", default=False, help="activate dev mode (auto reload)"
+)
+run.add_argument(
+    "--verbose", action="store_true", default=False, help="set log level to verbose"
+)
 run.add_argument("--workspace", type=str, help="Profile ID of workspace")
 run.add_argument("--db", type=str, help="Profile ID of db")
 run.add_argument("--push-notification", action="store_true", default=False)
 test = action.add_parser(name="test")
 
 plugins = action.add_parser("plugin")
 types = plugins.add_subparsers(title="type", dest="plugin_action", required=True)
@@ -113,54 +120,69 @@
             for package in config_toml["plugins"].values():
                 PluginSource(
                     package["username"], package["repository"]
                 ).download_from_sha(package["sha"], package["branch"]).install()
         case "run":
             from .utils import workdir
 
-            profiler = Profiler.get_profiler()
-            with open(workdir.db / "thundra.toml") as file:
-                workdir_db = workdir.db / tomllib.loads(file.read())["thundra"]["db"]
-            if parse.workspace:
-                profile = profiler.get_profile(parse.workspace)
-                workdir.workspace_dir = Path(profile.workspace)
-                os.chdir(workdir.workspace)
-                if workdir.db.__str__() == ".":
+            if parse.dev:
+                cmd = sys.orig_argv.copy()
+                cmd.remove("--dev")
+                if "--verbose" not in cmd:
+                    cmd.append("--verbose")
+                watchfiles.run_process(
+                    ".",
+                    watch_filter=lambda mode, file: file.endswith(".py"),
+                    target=shlex.join(cmd),
+                )
+            else:
+                profiler = Profiler.get_profiler()
+                with open(workdir.db / "thundra.toml") as file:
+                    workdir_db = (
+                        workdir.db / tomllib.loads(file.read())["thundra"]["db"]
+                    )
+                if parse.workspace:
+                    profile = profiler.get_profile(parse.workspace)
+                    workdir.workspace_dir = Path(profile.workspace)
+                    os.chdir(workdir.workspace)
+                    if workdir.db.__str__() == ".":
+                        workdir.db = Path(profile.db_path()).parent
+                        workdir_db = profile.db_path()
+                if parse.db:
+                    profile = profiler.get_profile(parse.db)
                     workdir.db = Path(profile.db_path()).parent
                     workdir_db = profile.db_path()
-            if parse.db:
-                profile = profiler.get_profile(parse.db)
-                workdir.db = Path(profile.db_path()).parent
-                workdir_db = profile.db_path()
-            from .config import config_toml
+                from .config import config_toml
 
-            os.environ.update(config_toml["thundra"].get("env", {}))
-            VirtualEnv.get_env().activate(workdir.workspace.__str__())
-            from .utils import workdir
-            from .agents import agent
-            from .command import command
-            from .middleware import middleware
-
-            print("🚀 starting %r" % config_toml["thundra"]["name"])
-            config_toml["thundra"]["db"] = workdir_db.__str__()
-            sys.path.insert(0, workdir.workspace_dir.__str__())
-            dirs, client = config_toml["thundra"]["app"].split(":")
-            app = __import__(dirs)
-            sys.path.remove(workdir.workspace_dir.__str__())
-            print(
-                f"🤖 {agent.__len__()} Agents, 🚦 {middleware.__len__()} Middlewares, and 📢 {command.__len__()} Commands"
-            )
-            for attr in dirs.split(".")[1:]:
-                app = getattr(app, attr)
-            if parse.phone_number:
-                app.__getattribute__(client).PairPhone(
-                    parse.phone_number, parse.push_notification
+                os.environ.update(config_toml["thundra"].get("env", {}))
+                VirtualEnv.get_env().activate(workdir.workspace.__str__())
+                from .utils import workdir
+                from .agents import agent
+                from .command import command
+                from .middleware import middleware
+
+                print("🚀 starting %r" % config_toml["thundra"]["name"])
+                config_toml["thundra"]["db"] = workdir_db.__str__()
+                sys.path.insert(0, workdir.workspace_dir.__str__())
+                dirs, client = config_toml["thundra"]["app"].split(":")
+                app = __import__(dirs)
+                if parse.verbose:
+                    log.setLevel(logging.DEBUG)
+                sys.path.remove(workdir.workspace_dir.__str__())
+                print(
+                    f"🤖 {agent.__len__()} Agents, 🚦 {middleware.__len__()} Middlewares, and 📢 {command.__len__()} Commands"
                 )
-            else:
-                app.__getattribute__(client).connect()
+                for attr in dirs.split(".")[1:]:
+                    app = getattr(app, attr)
+                if parse.phone_number:
+                    app.__getattribute__(client).PairPhone(
+                        parse.phone_number, parse.push_notification
+                    )
+                else:
+                    app.__getattribute__(client).connect()
         case "plugin":
             from .plugins import PluginSource, Plugin
 
             match parse.plugin_action:
                 case "install":
                     try:
                         username, repo = parse.git_url[0].split("/")
```

### Comparing `thundra_ai-0.0.8/thundra/command.py` & `thundra_ai-0.0.9/thundra/command.py`

 * *Files identical despite different names*

### Comparing `thundra_ai-0.0.8/thundra/config.py` & `thundra_ai-0.0.9/thundra/config.py`

 * *Files identical despite different names*

### Comparing `thundra_ai-0.0.8/thundra/core/graph.py` & `thundra_ai-0.0.9/thundra/core/graph.py`

 * *Files identical despite different names*

### Comparing `thundra_ai-0.0.8/thundra/core/llm.py` & `thundra_ai-0.0.9/thundra/core/llm.py`

 * *Files identical despite different names*

### Comparing `thundra_ai-0.0.8/thundra/core/memory.py` & `thundra_ai-0.0.9/thundra/core/memory.py`

 * *Files identical despite different names*

### Comparing `thundra_ai-0.0.8/thundra/evaluater.py` & `thundra_ai-0.0.9/thundra/evaluater.py`

 * *Files identical despite different names*

### Comparing `thundra_ai-0.0.8/thundra/ipc.py` & `thundra_ai-0.0.9/thundra/ipc.py`

 * *Files identical despite different names*

### Comparing `thundra_ai-0.0.8/thundra/middleware.py` & `thundra_ai-0.0.9/thundra/middleware.py`

 * *Files identical despite different names*

### Comparing `thundra_ai-0.0.8/thundra/plugins.py` & `thundra_ai-0.0.9/thundra/plugins.py`

 * *Files identical despite different names*

### Comparing `thundra_ai-0.0.8/thundra/profiler/__init__.py` & `thundra_ai-0.0.9/thundra/profiler/__init__.py`

 * *Files identical despite different names*

### Comparing `thundra_ai-0.0.8/thundra/storage/file.py` & `thundra_ai-0.0.9/thundra/storage/file.py`

 * *Files identical despite different names*

### Comparing `thundra_ai-0.0.8/thundra/templates/README.md` & `thundra_ai-0.0.9/thundra/templates/README.md`

 * *Files identical despite different names*

### Comparing `thundra_ai-0.0.8/thundra/templates/app/agents/base.py` & `thundra_ai-0.0.9/thundra/templates/app/agents/base.py`

 * *Files identical despite different names*

### Comparing `thundra_ai-0.0.8/thundra/templates/app/agents/yt.py` & `thundra_ai-0.0.9/thundra/templates/app/agents/yt.py`

 * *Files identical despite different names*

### Comparing `thundra_ai-0.0.8/thundra/templates/app/app.py` & `thundra_ai-0.0.9/thundra/templates/app/app.py`

 * *Files 6% similar despite different names*

```diff
@@ -40,18 +40,14 @@
         Profiler.add_profile(
             Profile(
                 workspace=workdir.workspace_dir.__str__(),
                 phonenumber=me_jid.User,
                 pushname=me.PushName,
             )
         )
-    # def set_debug(x: bytes):
-    #     getLogger().setLevel([NOTSET, DEBUG][int(x.decode())])
-
-    # lexz.set_handler("debug", set_debug)
     setattr(client, "my_tag", Jid2String(JIDToNonAD(me_jid)))
     setattr(client, "my_number", me_jid.User)
 
 
 def save_to_storage(message: MessageEv):
     try:
         msg = get_message_type(message.Message)
@@ -91,9 +87,8 @@
                 client.reply_message(
                     execute_agent(context, client, message).invoke(yamlx)["output"],
                     quoted=message,
                 )
 
 
 if __name__ == "__main__":
-    # app.connect()
-    pass
+    app.connect()
```

### Comparing `thundra_ai-0.0.8/thundra/templates/app/commands/base.py` & `thundra_ai-0.0.9/thundra/templates/app/commands/base.py`

 * *Files identical despite different names*

### Comparing `thundra_ai-0.0.8/thundra/templates/app/middleware/auto_save_media.py` & `thundra_ai-0.0.9/thundra/templates/app/middleware/auto_save_media.py`

 * *Files identical despite different names*

### Comparing `thundra_ai-0.0.8/thundra/templates/thundra.toml` & `thundra_ai-0.0.9/thundra/templates/thundra.toml`

 * *Files identical despite different names*

### Comparing `thundra_ai-0.0.8/thundra/test.py` & `thundra_ai-0.0.9/thundra/test.py`

 * *Files identical despite different names*

### Comparing `thundra_ai-0.0.8/thundra/types.py` & `thundra_ai-0.0.9/thundra/types.py`

 * *Files identical despite different names*

### Comparing `thundra_ai-0.0.8/thundra/utils.py` & `thundra_ai-0.0.9/thundra/utils.py`

 * *Files identical despite different names*

### Comparing `thundra_ai-0.0.8/PKG-INFO` & `thundra_ai-0.0.9/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: thundra-ai
-Version: 0.0.8
+Version: 0.0.9
 Summary: Neonize Abstraction
 Home-page: https://github.com/krypton-byte/thundra
 License: Apache 2.0
 Keywords: neonize,whatsapp,framework,websocket,bot
 Author: krypton-byte
 Author-email: rosid6434@gmail.com
 Requires-Python: >=3.11,<4.0
@@ -15,14 +15,15 @@
 Requires-Dist: appdirs (>=1.4.4,<2.0.0)
 Requires-Dist: graphviz (>=0.20.1,<0.21.0)
 Requires-Dist: langchain (>=0.1.11,<0.2.0)
 Requires-Dist: langchain-openai (>=0.0.8,<0.0.9)
 Requires-Dist: neonize (>=0.0.9,<0.0.10)
 Requires-Dist: pytube (>=15.0.0,<16.0.0)
 Requires-Dist: tomli-w (>=1.0.0,<2.0.0)
+Requires-Dist: watchfiles (>=0.21.0,<0.22.0)
 Project-URL: Repository, https://github.com/krypton-byte/thundra.git
 Description-Content-Type: text/markdown
 
 ## <p align="center">Thundra</p>
 <p align="center"><img src="https://raw.githubusercontent.com/krypton-byte/thundra/master/assets/logo.jpg" width="150px"/></p>
 
 Thundra is a framework designed to streamline the development of WhatsApp bots and automations. It provides a solid foundation and abstraction layer to simplify the process of creating and managing WhatsApp bots for various purposes.
```

