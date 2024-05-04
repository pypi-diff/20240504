# Comparing `tmp/pritunl_api-1.1.8.tar.gz` & `tmp/pritunl_api-1.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pritunl_api-1.1.8.tar", max compression
+gzip compressed data, was "pritunl_api-1.1.9.tar", max compression
```

## Comparing `pritunl_api-1.1.8.tar` & `pritunl_api-1.1.9.tar`

### file list

```diff
@@ -1,12 +1,15 @@
--rw-r--r--   0        0        0     1097 2023-03-20 04:19:29.857393 pritunl_api-1.1.8/LICENSE
--rw-r--r--   0        0        0     5591 2023-04-15 05:35:33.875349 pritunl_api-1.1.8/README.md
--rw-r--r--   0        0        0    16025 2023-04-15 05:35:33.875712 pritunl_api-1.1.8/pritunl_api/__init__.py
--rw-r--r--   0        0        0        0 2023-03-27 16:22:56.215232 pritunl_api-1.1.8/pritunl_api/utils/__init__.py
--rw-r--r--   0        0        0      413 2023-03-27 16:22:56.215533 pritunl_api-1.1.8/pritunl_api/utils/genkey.py
--rw-r--r--   0        0        0      603 2023-03-27 16:22:56.215737 pritunl_api-1.1.8/pritunl_api/utils/query.py
--rw-r--r--   0        0        0     1166 2023-04-15 05:35:33.876034 pritunl_api-1.1.8/pritunl_api_cli/__init__.py
--rw-r--r--   0        0        0       52 2023-04-15 05:35:33.876314 pritunl_api-1.1.8/pritunl_api_cli/commands/__init__.py
--rw-r--r--   0        0        0      193 2023-04-15 05:35:33.876532 pritunl_api-1.1.8/pritunl_api_cli/commands/connection.py
--rw-r--r--   0        0        0     7238 2023-04-15 05:35:33.876867 pritunl_api-1.1.8/pritunl_api_cli/commands/users.py
--rw-r--r--   0        0        0     1953 2023-04-15 05:35:33.877177 pritunl_api-1.1.8/pyproject.toml
--rw-r--r--   0        0        0     7535 1970-01-01 00:00:00.000000 pritunl_api-1.1.8/PKG-INFO
+-rw-r--r--   0        0        0     1097 2023-03-20 04:19:29.857393 pritunl_api-1.1.9/LICENSE
+-rw-r--r--   0        0        0     5274 2023-04-18 10:07:57.895369 pritunl_api-1.1.9/README.md
+-rw-r--r--   0        0        0    16025 2023-04-15 05:35:33.875712 pritunl_api-1.1.9/pritunl_api/__init__.py
+-rw-r--r--   0        0        0        0 2023-03-27 16:22:56.215232 pritunl_api-1.1.9/pritunl_api/utils/__init__.py
+-rw-r--r--   0        0        0      397 2023-04-18 10:07:57.895981 pritunl_api-1.1.9/pritunl_api/utils/keygen.py
+-rw-r--r--   0        0        0      644 2023-04-18 10:07:57.896582 pritunl_api-1.1.9/pritunl_api/utils/query.py
+-rw-r--r--   0        0        0      808 2023-04-18 10:07:57.897125 pritunl_api-1.1.9/pritunl_api_cli/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-18 10:07:57.897291 pritunl_api-1.1.9/pritunl_api_cli/commands/__init__.py
+-rw-r--r--   0        0        0      203 2023-04-18 10:07:57.897879 pritunl_api-1.1.9/pritunl_api_cli/commands/api.py
+-rw-r--r--   0        0        0     1220 2023-04-18 10:07:57.898520 pritunl_api-1.1.9/pritunl_api_cli/commands/user.py
+-rw-r--r--   0        0        0       52 2023-04-18 10:07:57.898793 pritunl_api-1.1.9/pritunl_api_cli/core/__init__.py
+-rw-r--r--   0        0        0      226 2023-04-18 10:07:57.899337 pritunl_api-1.1.9/pritunl_api_cli/core/api.py
+-rw-r--r--   0        0        0     8777 2023-04-18 10:07:57.899806 pritunl_api-1.1.9/pritunl_api_cli/core/user.py
+-rw-r--r--   0        0        0     1953 2023-04-18 10:07:57.900459 pritunl_api-1.1.9/pyproject.toml
+-rw-r--r--   0        0        0     7218 1970-01-01 00:00:00.000000 pritunl_api-1.1.9/PKG-INFO
```

### Comparing `pritunl_api-1.1.8/LICENSE` & `pritunl_api-1.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `pritunl_api-1.1.8/README.md` & `pritunl_api-1.1.9/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Pritunl API Client for Python 3
+# Pritunl API Client for Python
 
 This is a simple [Pritunl](https://pritunl.com/) API Client written in Python 3.
 
 You need to refer to Pritunl [API Documentation](https://docs.pritunl.com/docs/api) to understand how to use this. This API client uses almost the same command as the [API Handlers](https://github.com/pritunl/pritunl-web/tree/master/handlers).
 
 ## Installation
 
@@ -115,108 +115,81 @@
 ```bash
 pritunl-api-cli --help
 ```
 
 ```txt
 Usage: pritunl-api-cli [OPTIONS] COMMAND [ARGS]...
 
+  Pritunl API CLI
+
 Options:
   --version  Show the version and exit.
   --help     Show this message and exit.
 
 Commands:
-  create-user
-  delete-user
-  get-user
-  status
-  update-user
+  api
+  user
 ```
 
-For available command options and syntax, use the feature command help option.
+To show the available commands for a feature
 
 ```bash
-pritunl-api-cli create-user --help
+pritunl-api-cli user --help
 ```
 
-```text
-Usage: pritunl-api-cli create-user [OPTIONS]
+```txt
+Usage: pritunl-api-cli user [OPTIONS] COMMAND [ARGS]...
 
 Options:
-  --org-name TEXT
-  --user-name TEXT
-  --user-email TEXT
-  --pin TEXT
-  --yubikey-id TEXT
-  --from-csv-file PATH
-  --help                Show this message and exit.
-```
-
-#### Create User
-
-_Example 1: Create a Single User_
-
-```bash
-pritunl-api-cli create-user \
-  --org-name develop-network \
-  --user-name developer_1 \
-  --user-email developer_1@domain.tld
-```
-
-_Example 2: Create Users from CSV_
+  --help  Show this message and exit.
 
-```bash
-pritunl-api-cli create-user \
-  --from-csv-file ./users.csv
+Commands:
+  create
+  delete
+  get
+  update
 ```
 
-#### Delete User
+For available command options and syntax, use the feature command argument help option.
 
 ```bash
-pritunl-api-cli delete-user \
-  --org-name develop-network \
-  --user-name developer_1
+pritunl-api-cli user create --help
 ```
 
-#### Get User Information with Profile Key
+```text
+Usage: pritunl-api-cli user create [OPTIONS]
 
-```bash
-pritunl-api-cli get-user \
-  --org-name develop-network \
-  --user-name developer_1
+Options:
+  --org-name TEXT
+  --user-name TEXT
+  --user-email TEXT
+  --pin TEXT
+  --yubikey-id TEXT
+  --from-csv PATH
+  --help             Show this message and exit.                Show this message and exit.
 ```
 
-> Or get user profile advanced information
+_Example 1: Create a Single User_
 
 ```bash
-pritunl-api-cli get-user \
-  --org-name develop-network \
-  --user-name developer_1 \
-  --show-advanced-details
+pritunl-api-cli user create \
+  --org-name pritunl-dev \
+  --user-name john.doe \
+  --user-email john.doe@domain.tld
 ```
 
-#### Update a User
-
-To disable a user
+_Example 2: Create Users from CSV_
 
 ```bash
-pritunl-api-cli update-user \
-  --org-name develop-network \
-  --user-name developer_1 \
-  --disable
+pritunl-api-cli user create \
+  --from-csv ./users.csv
 ```
 
-To enable a user with new PIN
+> For more comprehensive CLI examples checkout the blog post [Managing Enterprise VPN using Pritunl API CLI](http://nathanielvarona.github.io/posts/managing-enterprise-vpn-using-pritunl-api-cli/).
 
-```bash
-pritunl-api-cli update-user \
-  --org-name developer-network \
-  --user-name developer_1 \
-  --enable
-  --pin 123456
-```
 
 ## API Development
 
 ### Using Virtual Environment
 
 Create a virtual environment and activate it.
```

### Comparing `pritunl_api-1.1.8/pritunl_api/__init__.py` & `pritunl_api-1.1.9/pritunl_api/__init__.py`

 * *Files identical despite different names*

### Comparing `pritunl_api-1.1.8/pritunl_api/utils/query.py` & `pritunl_api-1.1.9/pritunl_api/utils/query.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,19 +1,21 @@
-def org_user(pritunl_obj, org_name, user_name=None):
+def org_user(pritunl, org_name, user_name=None):
     def __get_org_by_name(orgs_obj, org_name):
         for org in orgs_obj:
             if org['name'] == org_name:
                 return org
         return None
 
     def __get_user_by_name(users_obj, user_name):
         for user in users_obj:
             if user["name"] == user_name:
                 return user
         return None
 
-    org = __get_org_by_name(pritunl_obj.organization.get(), org_name)
+    org = __get_org_by_name(pritunl.organization.get(), org_name)
+    user = pritunl.user.get(org_id=org['id'])
 
     if user_name:
-        user = __get_user_by_name(pritunl_obj.user.get(org_id=org['id']), user_name)
+        user = __get_user_by_name(pritunl.user.get(org_id=org['id']), user_name)
         return org, user
-    return org
+
+    return org, user
```

### Comparing `pritunl_api-1.1.8/pritunl_api_cli/commands/users.py` & `pritunl_api-1.1.9/pritunl_api_cli/core/user.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,64 +1,88 @@
 import csv
 import json
 from urllib.parse import urlparse
 
 from . import pritunl
 
 from pritunl_api.utils.query import org_user
-from pritunl_api.utils.genkey import profile_key
+from pritunl_api.utils.keygen import profile_key
 
 import click
 
 from rich import print_json
 from rich.console import Console
 from rich.table import Table
 
 console = Console()
 
 
-def get_user(**kwargs):
+def get(**kwargs):
     table = Table(
         title=f"User Profile and Key Information:",
         title_style="bold green",
         title_justify="left"
         )
 
+    table.add_column("Status", justify="left", style="green", no_wrap=True)
     table.add_column("User Name", justify="left", style="cyan", no_wrap=True)
     table.add_column("Organization", justify="left", style="magenta")
     table.add_column("Profile URL [italic red](Expires after 24 hours)[/italic red]", justify="left", style="green")
     table.add_column("Profile URI [italic red](Expires after 24 hours)[/italic red]", justify="left", style="green")
 
-    org, user = org_user(pritunl_obj=pritunl, org_name=kwargs['org_name'], user_name=kwargs['user_name'])
+    if kwargs['all_users']:
+        org, user = org_user(pritunl=pritunl, org_name=kwargs['org_name'])
+        users = list(filter(lambda x: x['type'] == 'client', user))
+
+        if users:
+            for user in users:
+                key_uri_url, key_view_url = profile_key(pritunl=pritunl, org_id=org['id'], usr_id=user['id'])
+
+                status = []
+                status.append("[red]Disabled[/red]" if user['disabled'] else "[green]Enabled[/green]")
+                status.append("[green]With PIN[/green]" if user['pin'] else "[yellow]No PIN[/yellow]")
 
-    if user:
-        key_uri_url, key_view_url = profile_key(pritunl_obj=pritunl, org_id=org['id'], usr_id=user['id'])
+                table.add_row(f"{status}", f"{user['name']}", f"{org['name']}", f"{key_view_url}", f"{key_uri_url}")
 
-        table.add_row(f"{user['name']}", f"{org['name']}", f"{key_view_url}", f"{key_uri_url}")
         console.print(table)
 
-        if kwargs['show_advanced_details']:
-            console.print(
-                f"Advanced Details:",
-                style="blue bold"
-            )
-            print_json(json.dumps(user))
     else:
-        console.print(f"[bold red]No user profile found![/bold red]")
+        org, user = org_user(pritunl=pritunl, org_name=kwargs['org_name'], user_name=kwargs['user_name'])
+        if user:
+            key_uri_url, key_view_url = profile_key(pritunl=pritunl, org_id=org['id'], usr_id=user['id'])
+
+            status = []
+            status.append("[red]Disabled[/red]" if user['disabled'] else "[green]Enabled[/green]")
+            status.append("[green]With PIN[/green]" if user['pin'] else "[yellow]No PIN[/yellow]")
 
+            table.add_row(f"{status}", f"{user['name']}", f"{org['name']}", f"{key_view_url}", f"{key_uri_url}")
+            console.print(table)
+        else:
+            console.print(f"[bold red]No user profile found![/bold red]")
 
-def create_user(**kwargs):
+    if kwargs['show_advanced_details']:
+        console.print(
+            f"Advanced Details:",
+            style="blue bold"
+        )
+        if kwargs['all_users']:
+            print_json(json.dumps(users))
+        else:
+            print_json(json.dumps(user))
+
+
+def create(**kwargs):
     table = Table(
         title=f"User Profile Created and Key Information:",
         title_style="bold green",
         title_justify="left",
         show_lines=True
         )
 
-    table.add_column("Action", justify="left", style="green", no_wrap=True)
+    table.add_column("Actions", justify="left", style="green", no_wrap=True)
     table.add_column("User Name", justify="left", style="cyan", no_wrap=True)
     table.add_column("User Email", justify="left", style="cyan", no_wrap=True)
     table.add_column("Organization", justify="left", style="magenta")
     table.add_column("Profile URL [italic red](Expires after 24 hours)[/italic red]", justify="left", style="green")
     table.add_column("Profile URI [italic red](Expires after 24 hours)[/italic red]", justify="left", style="green")
 
     def __create_user(org_id, user_name, user_email):
@@ -73,109 +97,125 @@
         if kwargs['yubikey_id']:
             user_data["auth_type"] = "yubico"
             user_data["yubico_id"] = kwargs['yubikey_id'][:12]
 
         create_user = pritunl.user.post(org_id=org_id, data=user_data)
 
         for user in create_user:
-            key_uri_url, key_view_url = profile_key(pritunl_obj=pritunl, org_id=org['id'], usr_id=user['id'])
+            key_uri_url, key_view_url = profile_key(pritunl=pritunl, org_id=org['id'], usr_id=user['id'])
 
-            table.add_row(f"[green]Created[/green]", f"{user['name']}", f"{user['email']}", f"{user['organization_name']}", f"{key_view_url}", f"{key_uri_url}")
+            actions.append("[green]Created[/green]")
 
-    if kwargs['org_name'] and kwargs['user_name'] and kwargs['user_email'] and not kwargs['from_csv_file']:
-        org, user = org_user(pritunl_obj=pritunl, org_name=kwargs['org_name'], user_name=kwargs['user_name'])
+            table.add_row(f"{actions}", f"{user['name']}", f"{user['email']}", f"{user['organization_name']}", f"{key_view_url}", f"{key_uri_url}")
+
+    if kwargs['org_name'] and kwargs['user_name'] and kwargs['user_email'] and not kwargs['from_csv']:
+        org, user = org_user(pritunl=pritunl, org_name=kwargs['org_name'], user_name=kwargs['user_name'])
+        actions = []
 
         if not user:
             __create_user(org_id=org['id'], user_name=kwargs['user_name'], user_email=kwargs['user_email'])
         else:
-            key_uri_url, key_view_url = profile_key(pritunl_obj=pritunl, org_id=org['id'], usr_id=user['id'])
-            table.add_row(f"[yellow]Skipped[/yellow]", f"{user['name']}", f"{user['email']}", f"{user['organization_name']}", f"{key_view_url}", f"{key_uri_url}")
+            key_uri_url, key_view_url = profile_key(pritunl=pritunl, org_id=org['id'], usr_id=user['id'])
+            actions.append("[yellow]Skipped[/yellow]")
+            table.add_row(f"{actions}", f"{user['name']}", f"{user['email']}", f"{user['organization_name']}", f"{key_view_url}", f"{key_uri_url}")
 
         console.print(table)
 
-    elif kwargs['from_csv_file'] and not kwargs['org_name'] and not kwargs['user_name'] and not kwargs['user_email']:
+    elif kwargs['from_csv'] and not kwargs['org_name'] and not kwargs['user_name'] and not kwargs['user_email']:
         csv_list = []
-        with open(kwargs['from_csv_file']) as csvfile:
+        with open(kwargs['from_csv']) as csvfile:
             reader = csv.DictReader(csvfile, skipinitialspace=True)
             for row in reader:
                 csv_list.append(row)
 
         for row in csv_list:
-            org, user = org_user(pritunl_obj=pritunl, org_name=row['Organization'], user_name=row['Username'])
+            org, user = org_user(pritunl=pritunl, org_name=row['Organization'], user_name=row['Username'])
+            actions = []
+
             if not user:
                 __create_user(org_id=org['id'], user_name=row['Username'], user_email=row['Email'])
             else:
-                key_uri_url, key_view_url = profile_key(pritunl_obj=pritunl, org_id=org['id'], usr_id=user['id'])
-                table.add_row(f"[yellow]Skipped[/yellow]", f"{user['name']}", f"{user['email']}", f"{user['organization_name']}", f"{key_view_url}", f"{key_uri_url}")
+                key_uri_url, key_view_url = profile_key(pritunl=pritunl, org_id=org['id'], usr_id=user['id'])
+                actions.append("[yellow]Skipped[/yellow]")
+                table.add_row(f"{actions}", f"{user['name']}", f"{user['email']}", f"{user['organization_name']}", f"{key_view_url}", f"{key_uri_url}")
 
         console.print(table)
 
     else:
-        if not kwargs['org_name'] and not kwargs['user_name'] and not kwargs['user_email'] and not kwargs['from_csv_file']:
+        if not kwargs['org_name'] and not kwargs['user_name'] and not kwargs['user_email'] and not kwargs['from_csv']:
             raise click.UsageError('Error: You entered with empty options.')
         else:
             raise click.UsageError('Error: You entered an invalid combination of options.')
 
 
-def update_user(**kwargs):
-
+def update(**kwargs):
     table = Table(
         title=f"User Profile Update and Key Information:",
         title_style="bold green",
         title_justify="left",
         )
 
-    table.add_column("Action", justify="left", style="green", no_wrap=True)
+    table.add_column("Actions", justify="left", style="green", no_wrap=True)
     table.add_column("User Name", justify="left", style="cyan", no_wrap=True)
     table.add_column("Organization", justify="left", style="magenta")
     table.add_column("Profile URL [italic red](Expires after 24 hours)[/italic red]", justify="left", style="green")
     table.add_column("Profile URI [italic red](Expires after 24 hours)[/italic red]", justify="left", style="green")
 
-    org, user = org_user(pritunl_obj=pritunl, org_name=kwargs['org_name'], user_name=kwargs['user_name'])
+    org, user = org_user(pritunl=pritunl, org_name=kwargs['org_name'], user_name=kwargs['user_name'])
 
     if user:
         user_data = {
             'name': user['name'],
             'email': user['email'],
             'disabled': False,
         }
 
-        if kwargs['pin']:
-            user_data["pin"] = kwargs['pin']
+        actions = []
 
         if kwargs['disable']:
             user_data.update({'disabled': True})
+            actions.append("[red]Disabled[/red]")
+        else:
+            actions.append("[green]Enabled[/green]")
+
+        if kwargs['pin']:
+            user_data["pin"] = kwargs['pin']
+            actions.append("[green]Set PIN[/green]")
+        else:
+            actions.append("[green]As is PIN State[/green]")
 
         response = pritunl.user.put(org_id=org['id'], usr_id=user['id'], data=user_data)
 
         if response:
-            key_uri_url, key_view_url = profile_key(pritunl_obj=pritunl, org_id=org['id'], usr_id=user['id'])
-            table.add_row(f"[yellow]Updated[/yellow]", f"{user['name']}", f"{user['organization_name']}", f"{key_view_url}", f"{key_uri_url}")
+            key_uri_url, key_view_url = profile_key(pritunl=pritunl, org_id=org['id'], usr_id=user['id'])
+            table.add_row(f"{actions}", f"{user['name']}", f"{user['organization_name']}", f"{key_view_url}", f"{key_uri_url}")
             console.print(table)
 
     else:
         console.print(f"[bold red]No user profile to update![/bold red]")
 
 
-def delete_user(**kwargs):
-
+def delete(**kwargs):
     table = Table(
         title=f"User Profile Delete:",
         title_style="bold green",
         title_justify="left",
         )
 
-    table.add_column("Action", justify="left", style="green", no_wrap=True)
+    table.add_column("Actions", justify="left", style="green", no_wrap=True)
     table.add_column("User Name", justify="left", style="cyan", no_wrap=True)
     table.add_column("Organization", justify="left", style="magenta")
 
-    org, user = org_user(pritunl_obj=pritunl, org_name=kwargs['org_name'], user_name=kwargs['user_name'])
+    org, user = org_user(pritunl=pritunl, org_name=kwargs['org_name'], user_name=kwargs['user_name'])
 
     if user:
+        actions = []
         response = pritunl.user.delete(org_id=org['id'], usr_id=user['id'])
 
         if response:
-            table.add_row(f"[red]Deleted[/red]", f"{user['name']}", f"{user['organization_name']}")
+            actions.append("[red]Deleted[/red]")
+
+            table.add_row(f"{actions}", f"{user['name']}", f"{user['organization_name']}")
             console.print(table)
 
     else:
         console.print(f"[bold red]No user profile to delete![/bold red]")
```

### Comparing `pritunl_api-1.1.8/pyproject.toml` & `pritunl_api-1.1.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pritunl-api"
-version = "1.1.8"
+version = "1.1.9"
 description = "Pritunl API Client for Python"
 authors = ["Nathaniel Varona <nathaniel.varona+pypi@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 
 classifiers = [
     "Development Status :: 4 - Beta",
@@ -48,12 +48,12 @@
 rich = {version = "13.3.2", optional = true}
 
 [tool.poetry.extras]
 repl =  ["ipython", "ptpython"]
 cli = ["click", "rich"]
 
 [tool.poetry.scripts]
-pritunl-api-cli = { callable = "pritunl_api_cli:run", extras = ["cli"] }
+pritunl-api-cli = { callable = "pritunl_api_cli:cli", extras = ["cli"] }
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `pritunl_api-1.1.8/PKG-INFO` & `pritunl_api-1.1.9/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pritunl-api
-Version: 1.1.8
+Version: 1.1.9
 Summary: Pritunl API Client for Python
 License: MIT
 Author: Nathaniel Varona
 Author-email: nathaniel.varona+pypi@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
@@ -37,15 +37,15 @@
 Project-URL: Downloads, https://github.com/nathanielvarona/pritunl-api-python
 Project-URL: Documentation, https://github.com/nathanielvarona/pritunl-api-python
 Project-URL: Homepage, https://github.com/nathanielvarona/pritunl-api-python
 Project-URL: Source, https://github.com/nathanielvarona/pritunl-api-python
 Project-URL: Tracker, https://github.com/nathanielvarona/pritunl-api-python
 Description-Content-Type: text/markdown
 
-# Pritunl API Client for Python 3
+# Pritunl API Client for Python
 
 This is a simple [Pritunl](https://pritunl.com/) API Client written in Python 3.
 
 You need to refer to Pritunl [API Documentation](https://docs.pritunl.com/docs/api) to understand how to use this. This API client uses almost the same command as the [API Handlers](https://github.com/pritunl/pritunl-web/tree/master/handlers).
 
 ## Installation
 
@@ -158,108 +158,81 @@
 ```bash
 pritunl-api-cli --help
 ```
 
 ```txt
 Usage: pritunl-api-cli [OPTIONS] COMMAND [ARGS]...
 
+  Pritunl API CLI
+
 Options:
   --version  Show the version and exit.
   --help     Show this message and exit.
 
 Commands:
-  create-user
-  delete-user
-  get-user
-  status
-  update-user
+  api
+  user
 ```
 
-For available command options and syntax, use the feature command help option.
+To show the available commands for a feature
 
 ```bash
-pritunl-api-cli create-user --help
+pritunl-api-cli user --help
 ```
 
-```text
-Usage: pritunl-api-cli create-user [OPTIONS]
+```txt
+Usage: pritunl-api-cli user [OPTIONS] COMMAND [ARGS]...
 
 Options:
-  --org-name TEXT
-  --user-name TEXT
-  --user-email TEXT
-  --pin TEXT
-  --yubikey-id TEXT
-  --from-csv-file PATH
-  --help                Show this message and exit.
-```
-
-#### Create User
-
-_Example 1: Create a Single User_
-
-```bash
-pritunl-api-cli create-user \
-  --org-name develop-network \
-  --user-name developer_1 \
-  --user-email developer_1@domain.tld
-```
-
-_Example 2: Create Users from CSV_
+  --help  Show this message and exit.
 
-```bash
-pritunl-api-cli create-user \
-  --from-csv-file ./users.csv
+Commands:
+  create
+  delete
+  get
+  update
 ```
 
-#### Delete User
+For available command options and syntax, use the feature command argument help option.
 
 ```bash
-pritunl-api-cli delete-user \
-  --org-name develop-network \
-  --user-name developer_1
+pritunl-api-cli user create --help
 ```
 
-#### Get User Information with Profile Key
+```text
+Usage: pritunl-api-cli user create [OPTIONS]
 
-```bash
-pritunl-api-cli get-user \
-  --org-name develop-network \
-  --user-name developer_1
+Options:
+  --org-name TEXT
+  --user-name TEXT
+  --user-email TEXT
+  --pin TEXT
+  --yubikey-id TEXT
+  --from-csv PATH
+  --help             Show this message and exit.                Show this message and exit.
 ```
 
-> Or get user profile advanced information
+_Example 1: Create a Single User_
 
 ```bash
-pritunl-api-cli get-user \
-  --org-name develop-network \
-  --user-name developer_1 \
-  --show-advanced-details
+pritunl-api-cli user create \
+  --org-name pritunl-dev \
+  --user-name john.doe \
+  --user-email john.doe@domain.tld
 ```
 
-#### Update a User
-
-To disable a user
+_Example 2: Create Users from CSV_
 
 ```bash
-pritunl-api-cli update-user \
-  --org-name develop-network \
-  --user-name developer_1 \
-  --disable
+pritunl-api-cli user create \
+  --from-csv ./users.csv
 ```
 
-To enable a user with new PIN
+> For more comprehensive CLI examples checkout the blog post [Managing Enterprise VPN using Pritunl API CLI](http://nathanielvarona.github.io/posts/managing-enterprise-vpn-using-pritunl-api-cli/).
 
-```bash
-pritunl-api-cli update-user \
-  --org-name developer-network \
-  --user-name developer_1 \
-  --enable
-  --pin 123456
-```
 
 ## API Development
 
 ### Using Virtual Environment
 
 Create a virtual environment and activate it.
```

