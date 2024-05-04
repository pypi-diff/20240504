# Comparing `tmp/ipfabric_snow-0.1.0b2.tar.gz` & `tmp/ipfabric_snow-0.1.0b3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ipfabric_snow-0.1.0b2.tar", max compression
+gzip compressed data, was "ipfabric_snow-0.1.0b3.tar", max compression
```

## Comparing `ipfabric_snow-0.1.0b2.tar` & `ipfabric_snow-0.1.0b3.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0    16242 2023-12-11 18:52:29.746316 ipfabric_snow-0.1.0b2/README.md
--rw-r--r--   0        0        0     5665 2023-11-30 01:27:46.489880 ipfabric_snow-0.1.0b2/ipfabric_snow/apps/env_setup.py
--rw-r--r--   0        0        0     5503 2023-12-11 21:06:52.210134 ipfabric_snow-0.1.0b2/ipfabric_snow/apps/sync_devices.py
--rw-r--r--   0        0        0      849 2023-12-01 00:25:37.387080 ipfabric_snow-0.1.0b2/ipfabric_snow/main.py
--rw-r--r--   0        0        0     1893 2023-11-30 01:27:46.490229 ipfabric_snow-0.1.0b2/ipfabric_snow/utils/env_manager.py
--rw-r--r--   0        0        0     7987 2023-12-11 19:23:10.923483 ipfabric_snow-0.1.0b2/ipfabric_snow/utils/etl.py
--rw-r--r--   0        0        0     1652 2023-11-30 01:27:46.490432 ipfabric_snow-0.1.0b2/ipfabric_snow/utils/logger.py
--rw-r--r--   0        0        0     5941 2023-12-11 16:11:31.112062 ipfabric_snow-0.1.0b2/ipfabric_snow/utils/servicenow_client.py
--rw-r--r--   0        0        0      754 2023-12-11 17:47:08.595808 ipfabric_snow-0.1.0b2/pyproject.toml
--rw-r--r--   0        0        0    16920 1970-01-01 00:00:00.000000 ipfabric_snow-0.1.0b2/PKG-INFO
+-rw-r--r--   0        0        0    16233 2024-04-12 18:24:53.077340 ipfabric_snow-0.1.0b3/README.md
+-rw-r--r--   0        0        0     5657 2023-12-13 13:44:33.109907 ipfabric_snow-0.1.0b3/ipfabric_snow/apps/env_setup.py
+-rw-r--r--   0        0        0     5365 2024-04-12 18:24:53.100601 ipfabric_snow-0.1.0b3/ipfabric_snow/apps/sync_devices.py
+-rw-r--r--   0        0        0      832 2024-04-12 18:24:53.101055 ipfabric_snow-0.1.0b3/ipfabric_snow/main.py
+-rw-r--r--   0        0        0     1893 2023-11-30 01:27:46.490229 ipfabric_snow-0.1.0b3/ipfabric_snow/utils/env_manager.py
+-rw-r--r--   0        0        0     8104 2023-12-13 13:51:28.797461 ipfabric_snow-0.1.0b3/ipfabric_snow/utils/etl.py
+-rw-r--r--   0        0        0     1636 2023-12-13 13:44:33.115822 ipfabric_snow-0.1.0b3/ipfabric_snow/utils/logger.py
+-rw-r--r--   0        0        0     7380 2024-04-29 16:02:53.131040 ipfabric_snow-0.1.0b3/ipfabric_snow/utils/servicenow_client.py
+-rw-r--r--   0        0        0      774 2024-05-04 14:36:45.908328 ipfabric_snow-0.1.0b3/pyproject.toml
+-rw-r--r--   0        0        0    16910 1970-01-01 00:00:00.000000 ipfabric_snow-0.1.0b3/PKG-INFO
```

### Comparing `ipfabric_snow-0.1.0b2/README.md` & `ipfabric_snow-0.1.0b3/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 # ServiceNow Integration with IP Fabric
-This project syncs devices from IP Fabric's Inventory to Service Now's CMDB Network Gear Table.
+This project syncs devices from IP Fabric's Inventory to ServiceNow's CMDB Network Gear Table.
 
 ## CLI Utility Installation
 ```shell
 pip install ipfabric-snow
 ```
-## Service Now Configuration
-Please see the [Service Now Configuration](docs/IP_Fabric_Service_Now_Application/index.md) section for details on how to configure Service Now for use with this integration.
+## ServiceNow Configuration
+Please see the [ServiceNow Configuration](docs/IP_Fabric_Service_Now_Application/index.md) section for details on how to configure ServiceNow for use with this integration.
 
 
 ## Environment Setup
 Copy sample.env to .env and fill in the necessary details.
 During the setup, you'll be prompted to enter the necessary environment variables including URLs and authentication details for both ServiceNow and IP Fabric.
 
 ## Quick Start 
-To sync devices from IP Fabric to Service Now, run:
+To sync devices from IP Fabric to ServiceNow, run:
 
 ```shell
 ipfabric-snow sync devices 
 ```
 If the environment is not properly set up, you'll be prompted to set it up. Follow the prompts to provide the necessary details.
 
 ```shell
@@ -34,41 +34,41 @@
 │ --log-json              --no-log-json             Log in JSON format [default: no-log-json]                                                                                                    │
 │ --install-completion                              Install completion for the current shell.                                                                                                    │
 │ --show-completion                                 Show completion for the current shell, to copy it or customize the installation.                                                             │
 │ --help                                            Show this message and exit.                                                                                                                  │
 ╰────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────╯
 ╭─ Commands ─────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────╮
 │ env                     Setup environment variables                                                                                                                                            │
-│ sync                    Sync Inventory data with Service Now                                                                                                                                   │
+│ sync                    Sync Inventory data with ServiceNow                                                                                                                                    │
 ╰────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────╯
 ```
 ```shell
 ❯ ipfabric-snow sync --help
                                                                                                                                                                                                                                                              
  Usage: ipfabric-snow sync [OPTIONS] COMMAND [ARGS]...                                                                                                                                                                                                       
                                                                                                                                                                                                                                                              
- Sync Inventory data with Service Now                                                                                                                                                                                                                        
+ Sync Inventory data with ServiceNow                                                                                                                                                                                                                        
                                                                                                                                                                                                                                                              
 ╭─ Options ─────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────╮
 │ --help          Show this message and exit.                                                                                                                                                                                                               │
 ╰───────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────╯
 ╭─ Commands ────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────╮
-│ devices                                  Sync devices from IP Fabric to Service Now                                                                                                                                                                       │
+│ devices                                  Sync devices from IP Fabric to ServiceNow                                                                                                                                                                        │
 ╰───────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────╯
 ```
 ```shell
  ipfabric-snow sync devices --help
 ```
 ```shell                                                                                                                                                                  
 Usage: ipfabric-snow sync devices [OPTIONS] [STAGING_TABLE_NAME]                                                                                                                                 
                                                                                                                                                                                                   
- Sync devices from IP Fabric to Service Now                                                                                                                                                       
+ Sync devices from IP Fabric to ServiceNow                                                                                                                                                       
                                                                                                                                                                                                   
 ╭─ Arguments ────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────╮
-│   staging_table_name      [STAGING_TABLE_NAME]  The name of the Service Now staging table to use. [default: x_1249630_ipf_devices]                                                             │
+│   staging_table_name      [STAGING_TABLE_NAME]  The name of the ServiceNow staging table to use. [default: x_1249630_ipf_devices]                                                              │
 ╰────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────╯
 ╭─ Options ──────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────╮
 │ --show-diff         --no-show-diff                  Display the data difference [default: no-show-diff]                                                                                        │
 │ --diff-source                              TEXT     Specify the main source for diff, either IPF or SNOW [default: IPF]                                                                        │
 │ --write-diff        --no-write-diff                 Enable or disable writing the diff to a file [default: no-write-diff]                                                                      │
 │ --diff-file                                TEXT     Path to save the diff file, if desired [default: data/{date_time}_diff_{diff_source}.json]                                                 │
 │ --dry-run           --no-dry-run                    Perform a dry run without making any changes [default: no-dry-run]                                                                         │
@@ -92,13 +92,13 @@
 ```
 #### Invoke
 This project uses [Invoke](https://www.pyinvoke.org/) for task automation. To see a list of available tasks, run:
 ```shell
 invoke --list
 ```
 #### Clearing the Netgear Table
-During Development, you may want to clear the netgear table in Service Now.
+During Development, you may want to clear the netgear table in ServiceNow.
 To clear the netgear table, run:
 ```shell
 ❯ invoke clear-netgear-table
 ```
-Any Changes to Service Now Application should be merged into the main_snow_app branch
+Any Changes to ServiceNow Application should be merged into the main_snow_app branch
```

### Comparing `ipfabric_snow-0.1.0b2/ipfabric_snow/apps/env_setup.py` & `ipfabric_snow-0.1.0b3/ipfabric_snow/apps/env_setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -117,16 +117,16 @@
     missing_vars = []
     for service_name in ["SNOW", "IPF"]:
         user_var = f"{service_name}_USER"
         pass_var = f"{service_name}_PASS"
         token_var = f"{service_name}_TOKEN"
 
         if not (
-                env_vars.get(token_var)
-                or (env_vars.get(user_var) and env_vars.get(pass_var))
+            env_vars.get(token_var)
+            or (env_vars.get(user_var) and env_vars.get(pass_var))
         ):
             missing_vars.extend([user_var, pass_var, token_var])
 
     for var in ["IPF_URL", "SNOW_URL"]:
         if not env_vars.get(var):
             missing_vars.append(var)
```

### Comparing `ipfabric_snow-0.1.0b2/ipfabric_snow/apps/sync_devices.py` & `ipfabric_snow-0.1.0b3/ipfabric_snow/apps/sync_devices.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 from ipfabric_snow.utils.logger import ipf_logger as logger
 from ipfabric_snow.utils.servicenow_client import Snow
 
 sync_devices_app = typer.Typer()
 
 # IPF_IGNORE_CLOUD_DEVICES_FILTER = {'or': [{'vendor': ['eq', 'azure']}, {'vendor': ['eq', 'aws']}, {'vendor': ['eq', 'gcp']}]}
 
+
 def get_snow_auth(env_vars):
     token = env_vars.get("SNOW_TOKEN")
     username = env_vars.get("SNOW_USER")
     password = env_vars.get("SNOW_PASS")
 
     if token:
         return token
@@ -41,53 +42,53 @@
             sn_model.vendors.create_vendor(vendor)
 
     for location in unique_locations:
         if location not in snow_locations:
             sn_model.location.create_location(location)
 
 
-@sync_devices_app.command("devices", help="Sync devices from IP Fabric to Service Now")
+@sync_devices_app.command("devices", help="Sync devices from IP Fabric to ServiceNow")
 def sync_devices(
-        staging_table_name: typing_extensions.Annotated[
-            typing.Optional[str],
-            typer.Argument(
-                help="The name of the Service Now staging table to use.",
-                # todo: insert link to docs
-            ),
-        ] = "x_1249630_ipf_devices",
-        show_diff: bool = typer.Option(False, help="Display the data difference"),
-        diff_source: str = typer.Option(
-            "IPF", help="Specify the main source for diff, either IPF or SNOW"
-        ),
-        write_diff: bool = typer.Option(
-            False, help="Enable or disable writing the diff to a file"
-        ),
-        diff_file: str = typer.Option(
-            "data/{date_time}_diff_{diff_source}.json",
-            help="Path to save the diff file, if desired",
-        ),
-        dry_run: bool = typer.Option(
-            False, help="Perform a dry run without making any changes"
-        ),
-        ipf_snapshot: str = typer.Option(
-            "$last", help="IP Fabric snapshot ID to use for the sync"
-        ),
-        cmdb_table_name: str = typer.Option(
-            default="cmdb_ci_netgear",
-            help="Name of the cmdb table to pull data from. Defaults to cmdb_ci_netgear",
-            hidden=True
-        ),
-        timeout: int = typer.Option(10, help="timeout for httpx requests"),
-        output_verbose: bool = typer.Option(
-            False,
-            help="adds more detail to the output. Identifies which keys changed per device",
-        ),
+    staging_table_name: typing_extensions.Annotated[
+        typing.Optional[str],
+        typer.Argument(
+            help="The name of the ServiceNow staging table to use.",
+            # todo: insert link to docs
+        ),
+    ] = "x_1249630_ipf_devices",
+    show_diff: bool = typer.Option(False, help="Display the data difference"),
+    diff_source: str = typer.Option(
+        "IPF", help="Specify the main source for diff, either IPF or SNOW"
+    ),
+    write_diff: bool = typer.Option(
+        False, help="Enable or disable writing the diff to a file"
+    ),
+    diff_file: str = typer.Option(
+        "data/{date_time}_diff_{diff_source}.json",
+        help="Path to save the diff file, if desired",
+    ),
+    dry_run: bool = typer.Option(
+        False, help="Perform a dry run without making any changes"
+    ),
+    ipf_snapshot: str = typer.Option(
+        "$last", help="IP Fabric snapshot ID to use for the sync"
+    ),
+    cmdb_table_name: str = typer.Option(
+        default="cmdb_ci_netgear",
+        help="Name of the cmdb table to pull data from. Defaults to cmdb_ci_netgear",
+        hidden=True,
+    ),
+    timeout: int = typer.Option(10, help="timeout for httpx requests"),
+    output_verbose: bool = typer.Option(
+        False,
+        help="adds more detail to the output. Identifies which keys changed per device",
+    ),
 ):
     """
-    Sync devices from IP Fabric to Service Now
+    Sync devices from IP Fabric to ServiceNow
     """
     if staging_table_name is None and not dry_run:
         logger.error(
             "No staging table name provided. Either provide a staging table name or enable dry run mode."
         )
         raise typer.Exit(code=1)
     all_vars = ensure_environment_is_setup()
@@ -101,39 +102,39 @@
 
     ipf = IPFClient(base_url=all_vars["IPF_URL"], auth=auth, snapshot_id=ipf_snapshot)
     auth = get_snow_auth(all_vars)
     sn_client = Snow(auth=auth, url=all_vars["SNOW_URL"], httpx_timeout=timeout)
 
     current_snow_data = sn_client.request_client.get_all_records(cmdb_table_name)
     all_snow_devices = current_snow_data["result"]
-    logger.info(f"Found {len(all_snow_devices)} devices in Service Now")
+    logger.info(f"Found {len(all_snow_devices)} devices in ServiceNow")
 
     all_devices = ipf.inventory.devices.all()
     # if we need to ignore cloud items from the inventory, we can add this filter
     # all_devices_to_ignore = ipf.inventory.devices.all(filters=IPF_IGNORE_CLOUD_DEVICES_FILTER)
     # all_devices = [device for device in ipf.inventory.devices.all() if device not in all_devices_to_ignore]
     logger.info(f"Found {len(all_devices)} devices in IP Fabric")
 
     main_source = diff_source.upper()
 
     if not dry_run:
         sn_client.request_client.insert_staging_record(
             staging_table_name, {"records": all_devices}
         )
     else:
-        logger.info("Dry run enabled, no data will be sent to Service Now")
+        logger.info("Dry run enabled, no data will be sent to ServiceNow")
 
     if show_diff or write_diff:
         etl_utility = ETLUtility(
             all_devices,
             all_snow_devices,
             data_source=main_source,
             verbose=output_verbose,
             check_env=False,
-            env_vars=all_vars
+            env_vars=all_vars,
         )
 
         etl_utility.transform_data()
         diff = etl_utility.compute_diff()
 
         if show_diff:
             print(diff)
```

### Comparing `ipfabric_snow-0.1.0b2/ipfabric_snow/main.py` & `ipfabric_snow-0.1.0b3/ipfabric_snow/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,24 +3,24 @@
 from ipfabric_snow.apps.env_setup import env_setup_app
 from ipfabric_snow.apps.sync_devices import sync_devices_app
 from ipfabric_snow.utils.logger import setup_logging
 
 app = typer.Typer()
 app.add_typer(env_setup_app, name="env", help="Setup environment variables")
 app.add_typer(
-    sync_devices_app, name="sync", help="Sync Inventory data with Service Now"
+    sync_devices_app, name="sync", help="Sync Inventory data with ServiceNow"
 )
 
 
 @app.callback()
 def logging_configuration(
-        log_level: str = typer.Option("INFO", help="Log level"),
-        log_to_file: bool = typer.Option(True, help="Log to file"),
-        log_file_name: str = typer.Option("ipf_serviceNow.log", help="Log file name"),
-        log_json: bool = typer.Option(False, help="Log in JSON format"),
+    log_level: str = typer.Option("INFO", help="Log level"),
+    log_to_file: bool = typer.Option(True, help="Log to file"),
+    log_file_name: str = typer.Option("ipf_serviceNow.log", help="Log file name"),
+    log_json: bool = typer.Option(False, help="Log in JSON format"),
 ):
     setup_logging(log_level, log_to_file, log_file_name, log_json)
 
 
 def main():
     app()
```

### Comparing `ipfabric_snow-0.1.0b2/ipfabric_snow/utils/env_manager.py` & `ipfabric_snow-0.1.0b3/ipfabric_snow/utils/env_manager.py`

 * *Files identical despite different names*

### Comparing `ipfabric_snow-0.1.0b2/ipfabric_snow/utils/etl.py` & `ipfabric_snow-0.1.0b3/ipfabric_snow/utils/etl.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,21 +15,21 @@
     "model": "device_type"
     # firmware_version handled separately
 }
 
 
 class ETLUtility:
     def __init__(
-            self,
-            ipf_data: List[dict],
-            snow_data: List[dict],
-            data_source: Union[Literal["IPF", "SNOW"], str],
-            verbose: bool = False,
-            check_env: bool = True,
-            env_vars: dict = None,
+        self,
+        ipf_data: List[dict],
+        snow_data: List[dict],
+        data_source: Union[Literal["IPF", "SNOW"], str],
+        verbose: bool = False,
+        check_env: bool = True,
+        env_vars: dict = None,
     ):
         if check_env:
             self.env_vars = ensure_environment_is_setup()
         else:
             if env_vars is None or not isinstance(env_vars, dict):
                 raise ValueError(
                     "If check_env is False, env_vars must be a dictionary containing the required environment variables"
@@ -57,17 +57,19 @@
         transformed_data_list = [
             self.transform_ipf_data(data, mapping_dict) for data in ipf_data_list
         ]
         return transformed_data_list
 
     @staticmethod
     def transform_ipf_data(data, mapping_dict):
-        transformed_data = {mapping_dict[key]: data[key] for key in mapping_dict if key in data}
-        if 'family' in data and 'version' in data:
-            transformed_data['firmware_version'] = f"{data['family']}-{data['version']}"
+        transformed_data = {
+            mapping_dict[key]: data[key] for key in mapping_dict if key in data
+        }
+        if "family" in data and "version" in data:
+            transformed_data["firmware_version"] = f"{data['family']}-{data['version']}"
         return transformed_data
 
     def transform_servicenow_to_ipfabric(self, sn_data_list, mapping_dict=None):
         if not mapping_dict:
             mapping_dict = self.mapping_dict
         reversed_mapping = {v: k for k, v in mapping_dict.items()}
         transformed_data_list = [
@@ -91,17 +93,17 @@
             key: snow_data[key] for key in reversed_mapping if key in snow_data
         }
         return self.process_vendor_and_location(filtered_data)
 
     def process_vendor_and_location(self, data):
         def update_data_from_cache(data_dict, key, cache, to_lower=False):
             if (
-                    key in data_dict
-                    and isinstance(data_dict[key], dict)
-                    and "value" in data_dict[key]
+                key in data_dict
+                and isinstance(data_dict[key], dict)
+                and "value" in data_dict[key]
             ):
                 sys_id = data_dict[key]["value"]
                 cached_name = cache.get(sys_id)
                 if cached_name:
                     data_dict[key] = cached_name.lower() if to_lower else cached_name
                 else:
                     data_dict[key] = sys_id
@@ -144,24 +146,28 @@
         }
         added = [ipf_map[key] for key in ipf_map if key not in snow_map]
         removed = [snow_map[key] for key in snow_map if key not in ipf_map]
         for unique_key, ipf_item in ipf_map.items():
             if unique_key in snow_map:
                 snow_item = snow_map[unique_key]
                 if ipf_item.get("serial_number") == snow_item.get(
-                        "serial_number"
+                    "serial_number"
                 ) or ipf_item.get("sn") == snow_item.get("sn"):
                     differences = {
                         key: self.normalize_empty_strings(ipf_item.get(key))
                         for key in ipf_item
-                        if self.normalize_empty_strings(ipf_item.get(key)) != self.normalize_empty_strings(
-                            snow_item.get(key))
+                        if self.normalize_empty_strings(ipf_item.get(key))
+                        != self.normalize_empty_strings(snow_item.get(key))
                     }
-                    if self.normalize_firmware_version(ipf_item) != self.normalize_firmware_version(snow_item):
-                        differences['firmware_version'] = ipf_item.get('firmware_version', '')
+                    if self.normalize_firmware_version(
+                        ipf_item
+                    ) != self.normalize_firmware_version(snow_item):
+                        differences["firmware_version"] = ipf_item.get(
+                            "firmware_version", ""
+                        )
                     if differences:
                         change_details = {"from": snow_item, "to": ipf_item}
                         if self.verbose:
                             change_details["details"] = [
                                 {
                                     "field": key,
                                     "old_value": snow_item.get(key),
@@ -180,18 +186,18 @@
         if not os.path.exists(dirs):
             os.makedirs(dirs)
         with open(file_path, "w") as file:
             json.dump(diff, file, indent=4)
 
     @staticmethod
     def normalize_empty_strings(value):
-        return None if value == '' else value
+        return None if value == "" else value
 
     @staticmethod
     def normalize_firmware_version(device_data):
-        family = device_data.get('family', '')
-        version = device_data.get('version', '')
-        return f"{family}-{version}" if family or version else device_data.get('firmware_version', '')
-
-
-
-
+        family = device_data.get("family", "")
+        version = device_data.get("version", "")
+        return (
+            f"{family}-{version}"
+            if family or version
+            else device_data.get("firmware_version", "")
+        )
```

### Comparing `ipfabric_snow-0.1.0b2/ipfabric_snow/utils/logger.py` & `ipfabric_snow-0.1.0b3/ipfabric_snow/utils/logger.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,18 +2,18 @@
 import sys
 
 import dotenv
 from loguru import logger
 
 
 def setup_logging(
-        log_level: str = None,
-        log_to_file: bool = None,
-        log_file_name: str = None,
-        log_json: bool = None,
+    log_level: str = None,
+    log_to_file: bool = None,
+    log_file_name: str = None,
+    log_json: bool = None,
 ):
     dotenv_path = dotenv.find_dotenv()
     if dotenv_path:
         dotenv.load_dotenv(dotenv_path)
     else:
         logger.warning("No .env file found. Using system environment variables.")
```

### Comparing `ipfabric_snow-0.1.0b2/ipfabric_snow/utils/servicenow_client.py` & `ipfabric_snow-0.1.0b3/ipfabric_snow/utils/servicenow_client.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,32 +1,36 @@
 # servicenow_client.py
 import json
 
 import httpx
 from httpx import HTTPError
+from loguru import logger
 
 
 class RequestSession:
-    def __init__(self, url, auth, httpx_timeout=10):
+    def __init__(self, url, auth, api_url, httpx_timeout=10):
         client = httpx.Client()
         client.auth = auth
         client.timeout = httpx_timeout
         self._base_url = url
-        self._api_url = url + "/api/now/"
+        if not api_url:
+            self._api_url = url + "/api/now/"
+        else:
+            self._api_url = url + api_url
         self._request_sesh = client
 
-    def _get(self, path):
-        self._response = self._request_sesh.get(self._api_url + f"{path}")
+    def _get(self, path, params=None):
+        self._response = self._request_sesh.get(self._api_url + f"{path}", params=params)
         self._response.raise_for_status()
         self._response_json = self._response.json()
         return self._response_json
 
     def _post(self, path, payload):
         self._response = self._request_sesh.post(
-            self._api_url + f"{path}", json=payload
+            self._api_url + f"{path}", data=payload
         )
         self._response.raise_for_status()
         self._response_json = self._response.json()
         return self._response_json
 
     def _post_files(self, path, parameters, file):
         self._request_sesh.headers.update({"Content-Type": "image/jpeg"})
@@ -135,15 +139,14 @@
 
     @property
     def net_gear(self):
         return NetGear(**self._sesh_dict)
 
 
 class CMDB_Table(RequestSession):
-
     def __init__(self, table_name, **kwargs):
         super().__init__(**kwargs)
         self.table_name = table_name
 
     def get_all(self):
         return self._get(f"table/{self.table_name}")
 
@@ -160,20 +163,53 @@
 
 
 class NetGear(CMDB_Table):
     def __init__(self, **kwargs):
         super().__init__("cmdb_ci_netgear", **kwargs)
 
 
+class Change(RequestSession):
+    def __init__(self, **kwargs):
+        logger.warning("Change class instantiated, this is still experimental. Use with caution. Not recommended for production.")
+        kwargs['api_url'] = "/api/sn_chg_rest/"
+        super().__init__(**kwargs)
+
+    def get_all(self, params=None):
+        return self._get("change", params=params)
+
+    def get_by_sys_id(self, sysid):
+        return self._get(f"change/{sysid}")
+
+    def create_change_request(self, description, change_type="Standard",):
+        payload = dict()
+        payload["chg_model"] = change_type
+        payload["short_description"] = description
+        payload["description"] = description
+        payload["type"] = "Standard"
+        payload = json.dumps(payload)
+        return self._post("change", payload=payload)
+
+    def get_change_states(self, sysid):
+        return self._get(f"change/{sysid}/nextstates")
+
+    def get_standard_change(self, sysid):
+        self._get("change/standard/{sysid}")
+
+    def update_change_request(self, sysid, payload):
+        payload = json.dumps(payload)
+        return self._patch(f"change/{sysid}", payload=payload)
+
+
 class Snow:
-    def __init__(self, auth, url, httpx_timeout=10):
+    def __init__(self, auth, url, httpx_timeout=10, api_url=None):
         sesh_dict = dict()
         sesh_dict["auth"] = auth
         sesh_dict["url"] = url
         sesh_dict["httpx_timeout"] = httpx_timeout
+        sesh_dict["api_url"] = api_url
         self._sesh_dict = sesh_dict
 
     @property
     def incidents(self):
         return Incidents(**self._sesh_dict)
 
     @property
@@ -187,7 +223,11 @@
     @property
     def cmdb(self):
         return CmdbCi(self._sesh_dict)
 
     @property
     def request_client(self):
         return RequestSession(**self._sesh_dict)
+
+    @property
+    def change_client(self):
+        return Change(**self._sesh_dict)
```

### Comparing `ipfabric_snow-0.1.0b2/pyproject.toml` & `ipfabric_snow-0.1.0b3/pyproject.toml`

 * *Files 17% similar despite different names*

```diff
@@ -1,31 +1,32 @@
 [tool.poetry]
 name = "ipfabric-snow"
-version = "0.1.0b2"
-description = "Integration with Service Now and IP Fabric"
+version = "0.1.0b3"
+description = "Integration with ServiceNow and IP Fabric"
 authors = ["Cristian Cordero <cristian.cordero@ipfabric.io>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "ipfabric_snow"}]
 
 [tool.poetry.dependencies]
 python = "^3.10"
-ipfabric = "^6.3.2"
+ipfabric = "^6.7.3"
 typer = {extras = ["all"], version = "^0.9.0"}
 loguru = "^0.7.2"
-rich = "^13.6.0"
+rich = "^13.7.1"
 
 
 [tool.poetry.group.dev.dependencies]
-mkdocs = "^1.5.3"
-pymdown-extensions = "^10.5"
-mkdocs-material = "^9.4.14"
+mkdocs = "^1.6.0"
+pymdown-extensions = "^10.8.1"
+mkdocs-material = "^9.5.21"
 mdx-truly-sane-lists = "^1.3"
 mkdocs-awesome-pages-plugin = "^2.9.2"
 invoke = "^2.2.0"
+black = "^23.12.1"
 
 [tool.poetry.scripts]
 ipfabric-snow = 'ipfabric_snow.main:main'
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `ipfabric_snow-0.1.0b2/PKG-INFO` & `ipfabric_snow-0.1.0b3/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,43 +1,43 @@
 Metadata-Version: 2.1
 Name: ipfabric-snow
-Version: 0.1.0b2
-Summary: Integration with Service Now and IP Fabric
+Version: 0.1.0b3
+Summary: Integration with ServiceNow and IP Fabric
 License: MIT
 Author: Cristian Cordero
 Author-email: cristian.cordero@ipfabric.io
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
-Requires-Dist: ipfabric (>=6.3.2,<7.0.0)
+Requires-Dist: ipfabric (>=6.7.3,<7.0.0)
 Requires-Dist: loguru (>=0.7.2,<0.8.0)
-Requires-Dist: rich (>=13.6.0,<14.0.0)
+Requires-Dist: rich (>=13.7.1,<14.0.0)
 Requires-Dist: typer[all] (>=0.9.0,<0.10.0)
 Description-Content-Type: text/markdown
 
 # ServiceNow Integration with IP Fabric
-This project syncs devices from IP Fabric's Inventory to Service Now's CMDB Network Gear Table.
+This project syncs devices from IP Fabric's Inventory to ServiceNow's CMDB Network Gear Table.
 
 ## CLI Utility Installation
 ```shell
 pip install ipfabric-snow
 ```
-## Service Now Configuration
-Please see the [Service Now Configuration](docs/IP_Fabric_Service_Now_Application/index.md) section for details on how to configure Service Now for use with this integration.
+## ServiceNow Configuration
+Please see the [ServiceNow Configuration](docs/IP_Fabric_Service_Now_Application/index.md) section for details on how to configure ServiceNow for use with this integration.
 
 
 ## Environment Setup
 Copy sample.env to .env and fill in the necessary details.
 During the setup, you'll be prompted to enter the necessary environment variables including URLs and authentication details for both ServiceNow and IP Fabric.
 
 ## Quick Start 
-To sync devices from IP Fabric to Service Now, run:
+To sync devices from IP Fabric to ServiceNow, run:
 
 ```shell
 ipfabric-snow sync devices 
 ```
 If the environment is not properly set up, you'll be prompted to set it up. Follow the prompts to provide the necessary details.
 
 ```shell
@@ -53,41 +53,41 @@
 │ --log-json              --no-log-json             Log in JSON format [default: no-log-json]                                                                                                    │
 │ --install-completion                              Install completion for the current shell.                                                                                                    │
 │ --show-completion                                 Show completion for the current shell, to copy it or customize the installation.                                                             │
 │ --help                                            Show this message and exit.                                                                                                                  │
 ╰────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────╯
 ╭─ Commands ─────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────╮
 │ env                     Setup environment variables                                                                                                                                            │
-│ sync                    Sync Inventory data with Service Now                                                                                                                                   │
+│ sync                    Sync Inventory data with ServiceNow                                                                                                                                    │
 ╰────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────╯
 ```
 ```shell
 ❯ ipfabric-snow sync --help
                                                                                                                                                                                                                                                              
  Usage: ipfabric-snow sync [OPTIONS] COMMAND [ARGS]...                                                                                                                                                                                                       
                                                                                                                                                                                                                                                              
- Sync Inventory data with Service Now                                                                                                                                                                                                                        
+ Sync Inventory data with ServiceNow                                                                                                                                                                                                                        
                                                                                                                                                                                                                                                              
 ╭─ Options ─────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────╮
 │ --help          Show this message and exit.                                                                                                                                                                                                               │
 ╰───────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────╯
 ╭─ Commands ────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────╮
-│ devices                                  Sync devices from IP Fabric to Service Now                                                                                                                                                                       │
+│ devices                                  Sync devices from IP Fabric to ServiceNow                                                                                                                                                                        │
 ╰───────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────╯
 ```
 ```shell
  ipfabric-snow sync devices --help
 ```
 ```shell                                                                                                                                                                  
 Usage: ipfabric-snow sync devices [OPTIONS] [STAGING_TABLE_NAME]                                                                                                                                 
                                                                                                                                                                                                   
- Sync devices from IP Fabric to Service Now                                                                                                                                                       
+ Sync devices from IP Fabric to ServiceNow                                                                                                                                                       
                                                                                                                                                                                                   
 ╭─ Arguments ────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────╮
-│   staging_table_name      [STAGING_TABLE_NAME]  The name of the Service Now staging table to use. [default: x_1249630_ipf_devices]                                                             │
+│   staging_table_name      [STAGING_TABLE_NAME]  The name of the ServiceNow staging table to use. [default: x_1249630_ipf_devices]                                                              │
 ╰────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────╯
 ╭─ Options ──────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────╮
 │ --show-diff         --no-show-diff                  Display the data difference [default: no-show-diff]                                                                                        │
 │ --diff-source                              TEXT     Specify the main source for diff, either IPF or SNOW [default: IPF]                                                                        │
 │ --write-diff        --no-write-diff                 Enable or disable writing the diff to a file [default: no-write-diff]                                                                      │
 │ --diff-file                                TEXT     Path to save the diff file, if desired [default: data/{date_time}_diff_{diff_source}.json]                                                 │
 │ --dry-run           --no-dry-run                    Perform a dry run without making any changes [default: no-dry-run]                                                                         │
@@ -111,14 +111,14 @@
 ```
 #### Invoke
 This project uses [Invoke](https://www.pyinvoke.org/) for task automation. To see a list of available tasks, run:
 ```shell
 invoke --list
 ```
 #### Clearing the Netgear Table
-During Development, you may want to clear the netgear table in Service Now.
+During Development, you may want to clear the netgear table in ServiceNow.
 To clear the netgear table, run:
 ```shell
 ❯ invoke clear-netgear-table
 ```
-Any Changes to Service Now Application should be merged into the main_snow_app branch
+Any Changes to ServiceNow Application should be merged into the main_snow_app branch
```

