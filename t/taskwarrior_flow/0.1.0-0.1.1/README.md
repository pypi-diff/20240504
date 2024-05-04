# Comparing `tmp/taskwarrior_flow-0.1.0.tar.gz` & `tmp/taskwarrior_flow-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "taskwarrior_flow-0.1.0.tar", max compression
+gzip compressed data, was "taskwarrior_flow-0.1.1.tar", max compression
```

## Comparing `taskwarrior_flow-0.1.0.tar` & `taskwarrior_flow-0.1.1.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0    11357 2024-05-03 03:34:34.326362 taskwarrior_flow-0.1.0/LICENSE
--rw-r--r--   0        0        0     1596 2024-05-03 11:14:54.149391 taskwarrior_flow-0.1.0/README.md
--rw-r--r--   0        0        0      850 2024-05-03 11:33:43.798095 taskwarrior_flow-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      858 2024-05-03 06:57:37.776383 taskwarrior_flow-0.1.0/tools/__init__.py
--rw-r--r--   0        0        0      761 2024-05-03 11:14:13.209646 taskwarrior_flow-0.1.0/tools/main.py
--rw-r--r--   0        0        0    12727 2024-05-03 05:38:58.259326 taskwarrior_flow-0.1.0/tools/utils.py
--rw-r--r--   0        0        0     2124 1970-01-01 00:00:00.000000 taskwarrior_flow-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0    11357 2024-05-04 09:20:20.622506 taskwarrior_flow-0.1.1/LICENSE
+-rw-r--r--   0        0        0     1126 2024-05-04 09:20:20.622506 taskwarrior_flow-0.1.1/README.md
+-rw-r--r--   0        0        0      868 2024-05-04 09:20:20.622506 taskwarrior_flow-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0      868 2024-05-04 09:20:20.622506 taskwarrior_flow-0.1.1/tools/__init__.py
+-rw-r--r--   0        0        0      761 2024-05-04 09:20:20.622506 taskwarrior_flow-0.1.1/tools/main.py
+-rw-r--r--   0        0        0    13156 2024-05-04 09:20:20.622506 taskwarrior_flow-0.1.1/tools/utils.py
+-rw-r--r--   0        0        0     1705 1970-01-01 00:00:00.000000 taskwarrior_flow-0.1.1/PKG-INFO
```

### Comparing `taskwarrior_flow-0.1.0/LICENSE` & `taskwarrior_flow-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `taskwarrior_flow-0.1.0/pyproject.toml` & `taskwarrior_flow-0.1.1/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,28 +1,29 @@
 [tool.poetry]
 name = "taskwarrior_flow"
-version = "0.1.0"
+version = "0.1.1"
 description = "Set of helpers for improving Taskwarrior workflow"
 authors = ["Ben Trinh <huantrinh1802@gmail.com>"]
 readme = "README.md"
 packages = [{ include = "tools" }]
 
 [tool.poetry.scripts]
 twf = 'tools.main:app'
 
 [tool.poetry.dependencies]
-python = "^3.11"
+python = "^3.10"
 typer = "^0.12.3"
 python-dateutil = "^2.8.2"
 questionary = "^2.0.1"
 
 [tool.poetry.group.dev.dependencies]
 ruff = "^0.1.3"
 mypy = "^1.6.1"
 types-python-dateutil = "^2.8.19.14"
+pytest = "^8.2.0"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.ruff]
 line-length = 120
```

### Comparing `taskwarrior_flow-0.1.0/tools/__init__.py` & `taskwarrior_flow-0.1.1/tools/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 import json
 import os
 
 config_file = os.environ.get("TW_CONFIG", f'{os.path.expanduser("~")}/.local/share/nvim/m_taskwarrior_d.json')
 if os.path.isfile(config_file):
-    with open(config_file) as f:
+    with open(config_file, 'r') as f:
         tw_config = json.load(f)
 else:
-    with open(config_file) as f:
+    with open(config_file, 'w') as f:
         tw_config = {
             "use_mtwd": False,
             "flow_config": {"default": {"data": "~/.task", "config": "~/.taskrc"}},
             "add_templates": {"data": []},
             "saved_queries": {"name_max_length": 0, "data": []},
         }
         f.write(json.dumps(tw_config))
```

### Comparing `taskwarrior_flow-0.1.0/tools/main.py` & `taskwarrior_flow-0.1.1/tools/main.py`

 * *Files identical despite different names*

### Comparing `taskwarrior_flow-0.1.0/tools/utils.py` & `taskwarrior_flow-0.1.1/tools/utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 import json
 import re
 import subprocess
-from typing import Annotated
+from typing import Annotated, Callable, TypedDict
 
 import questionary
 import typer
 from prompt_toolkit.shortcuts import CompleteStyle
 from rich import print as rprint
 
-from tools import config_file, group_mappings, tw_config, group_mappings_completion
+from tools import config_file, group_mappings, group_mappings_completion, tw_config
 
 utils = typer.Typer()
 question_style = questionary.Style(
     [
         ("qmark", "fg:#007777 bold"),  # token in front of the question
         ("question", "bold"),  # question text
         ("answer", "fg:white bg:#007777 "),  # submitted answer text behind the question
@@ -33,44 +33,55 @@
     ),
     "tags": questionary.autocomplete(
         "Enter tags", choices=tags, style=question_style, complete_style=CompleteStyle.MULTI_COLUMN
     ),
 }
 
 
+class FunctionsGroup(TypedDict):
+    func: Callable
+    help: str
+
+
 def safe_ask(question):
     try:
         response = question.unsafe_ask()
         return response
     except KeyboardInterrupt:
-        print('Cancelled by user')
+        print("Cancelled by user")
         return None
 
 
 def create_query(*_):
-    query_instruction = "Use '|' for separate the filter and the report\ni.e. `project:TW | next`\n" if tw_config["use_mtwd"] else None
-    response = safe_ask(questionary.form(
-        name=questionary.text("Enter name", style=question_style),
-        query=questionary.text("Enter query", style=question_style, instruction=query_instruction),
-    ))
+    query_instruction = (
+        "Use '|' for separate the filter and the report\ni.e. `project:TW | next`\n" if tw_config["use_mtwd"] else None
+    )
+    response = safe_ask(
+        questionary.form(
+            name=questionary.text("Enter name", style=question_style),
+            query=questionary.text("Enter query", style=question_style, instruction=query_instruction),
+        )
+    )
     if response is None:
         return
     if response["name"] != "" and response["query"] != "":
         if tw_config["saved_queries"]["name_max_length"] < len(response["name"]):
             tw_config["saved_queries"]["name_max_length"] = len(response["name"])
         with open(config_file, "w") as f:
             tw_config["saved_queries"]["data"].append(response)
             f.write(json.dumps(tw_config))
 
 
 def create_template(*_):
-    response = safe_ask(questionary.form(
-        name=questionary.text("Enter name", style=question_style),
-        command=questionary.text("Enter command", style=question_style),
-    ))
+    response = safe_ask(
+        questionary.form(
+            name=questionary.text("Enter name", style=question_style),
+            command=questionary.text("Enter command", style=question_style),
+        )
+    )
     if response is None:
         return
     template = {"name": response["name"], "command": response["command"], "fields": {}}
     print("<---------Fields--------->")
     field_name = "placeholder"
     while field_name != "":
         field_name = safe_ask(questionary.text("Enter field name", style=question_style))
@@ -88,17 +99,17 @@
 
 
 def create_task(group):
     templates = [
         questionary.Choice(title=template["name"], value=index, shortcut_key=str(index + 1))
         for index, template in enumerate(tw_config["add_templates"]["data"])
     ]
-    chosen_template = safe_ask(questionary.rawselect(
-        "Select template", choices=templates, use_jk_keys=True, style=question_style
-    ))
+    chosen_template = safe_ask(
+        questionary.rawselect("Select template", choices=templates, use_jk_keys=True, style=question_style)
+    )
     if chosen_template is None:
         return
     questions = {}
     for name, field in tw_config["add_templates"]["data"][chosen_template]["fields"].items():
         if name in preset_questions:
             questions[name] = preset_questions[name]
         else:
@@ -136,60 +147,68 @@
                         f"TASKDATA=~/.task_test /opt/homebrew/bin/task {uuid} annotate {annotate}",
                         capture_output=True,
                         text=True,
                         shell=True,
                     )
 
 
-create_groups = {"task": {"help": "Add a new task based on template", "func": create_task}, "template": {"help": "Add a new task template", "func": create_template}, "query": {"help": "Add a new query for viewing tasks", "func": create_query}}
+create_groups: dict[str, FunctionsGroup] = {
+    "task": {"help": "Add a new task based on template", "func": create_task},
+    "template": {"help": "Add a new task template", "func": create_template},
+    "query": {"help": "Add a new query for viewing tasks", "func": create_query},
+}
 
 
 def create_group_completion():
     autocompletions = []
     for key, value in create_groups.items():
-        autocompletions.append((key, value['help']))
+        autocompletions.append((key, value["help"]))
     return autocompletions
 
 
 @utils.command("add", help="Add task, query, and template")
 def task_create(
     name: Annotated[str, typer.Argument(autocompletion=create_group_completion)] = "task",
     group: Annotated[str, typer.Option("--group", "-g", autocompletion=group_mappings_completion)] = "default",
 ):
-    create_groups[name]['func'](group)
+    create_groups[name]["func"](group)
 
 
 def edit_template():
     templates = [
         questionary.Choice(title=template["name"], value=index, shortcut_key=str(index + 1))
         for index, template in enumerate(tw_config["add_templates"]["data"])
     ]
-    chosen_template = safe_ask(questionary.rawselect(
-        "Select template", choices=templates, use_jk_keys=True, style=question_style
-    ))
+    chosen_template = safe_ask(
+        questionary.rawselect("Select template", choices=templates, use_jk_keys=True, style=question_style)
+    )
     if chosen_template is None:
         return
-    response = safe_ask(questionary.form(
-        name=questionary.text(
-            "Enter name", style=question_style, default=tw_config["add_templates"]["data"][chosen_template]["name"]
-        ),
-        command=questionary.text(
-            "Enter command",
-            style=question_style,
-            default=tw_config["add_templates"]["data"][chosen_template]["command"],
-        ),
-    ))
+    response = safe_ask(
+        questionary.form(
+            name=questionary.text(
+                "Enter name", style=question_style, default=tw_config["add_templates"]["data"][chosen_template]["name"]
+            ),
+            command=questionary.text(
+                "Enter command",
+                style=question_style,
+                default=tw_config["add_templates"]["data"][chosen_template]["command"],
+            ),
+        )
+    )
     if response is None:
         return
     template = {"name": response["name"], "command": response["command"], "fields": {}}
     for name, field_template in tw_config["add_templates"]["data"][chosen_template]["fields"].items():
-        response = safe_ask(questionary.form(
-            name=questionary.text("Enter field name", style=question_style, default=name),
-            template=questionary.text("Enter field template", style=question_style, default=field_template),
-        ))
+        response = safe_ask(
+            questionary.form(
+                name=questionary.text("Enter field name", style=question_style, default=name),
+                template=questionary.text("Enter field template", style=question_style, default=field_template),
+            )
+        )
         if response is None:
             return
         template["fields"][response["name"]] = response["template"]
     field_name = "placeholder"
     while field_name != "":
         field_name = safe_ask(questionary.text("Enter field name", style=question_style))
         if field_name is None:
@@ -209,97 +228,109 @@
     max_length = tw_config["saved_queries"]["name_max_length"]
     queries = [
         questionary.Choice(
             title=f"{query['name'].ljust(max_length)} | {query['query']}", value=index, shortcut_key=str(index + 1)
         )
         for index, query in enumerate(tw_config["saved_queries"]["data"])
     ]
-    chosen_query = safe_ask(questionary.rawselect("Select query", choices=queries, use_jk_keys=True, style=question_style))
+    chosen_query = safe_ask(
+        questionary.rawselect("Select query", choices=queries, use_jk_keys=True, style=question_style)
+    )
     if chosen_query is None:
         return
-    response = safe_ask(questionary.form(
-        name=questionary.text(
-            "Enter name", style=question_style, default=tw_config["saved_queries"]["data"][chosen_query]["name"]
-        ),
-        query=questionary.text(
-            "Enter query", style=question_style, default=tw_config["saved_queries"]["data"][chosen_query]["query"]
-        ),
-    ))
+    response = safe_ask(
+        questionary.form(
+            name=questionary.text(
+                "Enter name", style=question_style, default=tw_config["saved_queries"]["data"][chosen_query]["name"]
+            ),
+            query=questionary.text(
+                "Enter query", style=question_style, default=tw_config["saved_queries"]["data"][chosen_query]["query"]
+            ),
+        )
+    )
     if response is None:
         return
     if response["name"] != "" and response["query"] != "":
         if tw_config["saved_queries"]["name_max_length"] < len(response["name"]):
             tw_config["saved_queries"]["name_max_length"] = len(response["name"])
         with open(config_file, "w") as f:
             tw_config["saved_queries"]["data"][chosen_query] = response
             f.write(json.dumps(tw_config))
 
 
-edit_groups = {"template": {"help": "Edit task template", "func": edit_template}, "query": {"help": "Edit view query", "func": edit_query}}
+edit_groups: dict[str, FunctionsGroup] = {
+    "template": {"help": "Edit task template", "func": edit_template},
+    "query": {"help": "Edit view query", "func": edit_query},
+}
 
 
 def edit_group_completion():
     autocompletions = []
     for group, group_info in edit_groups.items():
         autocompletions.append((group, group_info["help"]))
     return autocompletions
 
 
 @utils.command("edit", help="Edit query, and template")
 def task_edit(
     name: Annotated[str, typer.Argument(autocompletion=edit_group_completion)] = "template",
 ):
-    edit_groups[name]['func']()
+    edit_groups[name]["func"]()
 
 
 def view_task():
     max_length = tw_config["saved_queries"]["name_max_length"]
     queries = [
         questionary.Choice(
             title=f"{query['name'].ljust(max_length)} | {query['query']}", value=index, shortcut_key=str(index + 1)
         )
         for index, query in enumerate(tw_config["saved_queries"]["data"])
     ]
-    chosen_query = safe_ask(questionary.rawselect("Select query", choices=queries, use_jk_keys=True, style=question_style))
+    chosen_query = safe_ask(
+        questionary.rawselect("Select query", choices=queries, use_jk_keys=True, style=question_style)
+    )
     if chosen_query is None:
         return
     command = tw_config["saved_queries"]["data"][chosen_query]["query"].replace("|", " ")
     output = subprocess.run(f"task rc._forcecolor:on {command}", shell=True, capture_output=True, text=True)
     print(output.stdout)
 
 
 def view_template():
     templates = [
         questionary.Choice(title=template["name"], value=index, shortcut_key=str(index + 1))
         for index, template in enumerate(tw_config["add_templates"]["data"])
     ]
-    chosen_template = safe_ask(questionary.rawselect(
-        "Select template", choices=templates, use_jk_keys=True, style=question_style
-    ))
+    chosen_template = safe_ask(
+        questionary.rawselect("Select template", choices=templates, use_jk_keys=True, style=question_style)
+    )
     if chosen_template is None:
         return
     header = f'[bold]Template:[/bold] {tw_config["add_templates"]["data"][chosen_template]["name"]}'
     field_header = f'{"-"*10}Fields{"-"*10}'
     rprint(
         f"""{header}
 [bold]Command:[/bold] {tw_config["add_templates"]["data"][chosen_template]["command"]}
 [bold]{field_header}[/bold]"""
     )
     for name, field_template in tw_config["add_templates"]["data"][chosen_template]["fields"].items():
         rprint(f"{name.ljust(16)} | {field_template}")
 
 
-view_groups = {"task": {"help": "View tasks based on saved queries", "func": view_task}, "template": {"help": "View the details of the template", "func": view_template}}
+view_groups: dict[str, FunctionsGroup] = {
+    "task": {"help": "View tasks based on saved queries", "func": view_task},
+    "template": {"help": "View the details of the template", "func": view_template},
+}
 
 
 def view_group_completion():
     autocompletions = []
     for key, value in view_groups.items():
-        autocompletions.append((key, value['help']))
+        autocompletions.append((key, value["help"]))
     return autocompletions
 
 
 @utils.command("view", help="View task and template")
 def task_view(
     name: Annotated[str, typer.Argument(autocompletion=view_group_completion)] = "task",
 ):
-    view_groups[name]['func']()
+    view_groups[name]["func"]()
```

