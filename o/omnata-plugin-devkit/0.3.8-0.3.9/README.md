# Comparing `tmp/omnata_plugin_devkit-0.3.8.tar.gz` & `tmp/omnata_plugin_devkit-0.3.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "omnata_plugin_devkit-0.3.8.tar", max compression
+gzip compressed data, was "omnata_plugin_devkit-0.3.9.tar", max compression
```

## Comparing `omnata_plugin_devkit-0.3.8.tar` & `omnata_plugin_devkit-0.3.9.tar`

### file list

```diff
@@ -1,46 +1,46 @@
--rw-r--r--   0        0        0    26526 2024-02-13 08:55:19.820329 omnata_plugin_devkit-0.3.8/LICENSE
--rw-r--r--   0        0        0      357 2024-02-13 08:55:19.820329 omnata_plugin_devkit-0.3.8/README.md
--rw-r--r--   0        0        0      683 2024-02-13 08:55:19.820329 omnata_plugin_devkit-0.3.8/pyproject.toml
--rw-r--r--   0        0        0        0 2024-02-13 08:55:19.820329 omnata_plugin_devkit-0.3.8/src/omnata_plugin_devkit/__init__.py
--rw-r--r--   0        0        0    12862 2024-02-13 08:55:19.820329 omnata_plugin_devkit-0.3.8/src/omnata_plugin_devkit/airbyte_wrapper.py
--rw-r--r--   0        0        0     6701 2024-02-13 08:55:19.820329 omnata_plugin_devkit-0.3.8/src/omnata_plugin_devkit/cli/__init__.py
--rw-r--r--   0        0        0    39347 2024-02-13 08:55:19.820329 omnata_plugin_devkit-0.3.8/src/omnata_plugin_devkit/development_session.py
--rw-r--r--   0        0        0      508 2024-02-13 08:55:19.820329 omnata_plugin_devkit-0.3.8/src/omnata_plugin_devkit/initialiser.py
--rw-r--r--   0        0        0     1694 2024-02-13 08:55:19.820329 omnata_plugin_devkit-0.3.8/src/omnata_plugin_devkit/jinja_templates/API_LIMITS.sql.jinja
--rw-r--r--   0        0        0     2660 2024-02-13 08:55:19.820329 omnata_plugin_devkit-0.3.8/src/omnata_plugin_devkit/jinja_templates/CONFIGURATION_FORM.sql.jinja
--rw-r--r--   0        0        0     9426 2024-02-13 08:55:19.820329 omnata_plugin_devkit-0.3.8/src/omnata_plugin_devkit/jinja_templates/CONFIGURE_APIS.sql.jinja
--rw-r--r--   0        0        0     1251 2024-02-13 08:55:19.820329 omnata_plugin_devkit-0.3.8/src/omnata_plugin_devkit/jinja_templates/CONNECTION_FORM.sql.jinja
--rw-r--r--   0        0        0     1869 2024-02-13 08:55:19.820329 omnata_plugin_devkit-0.3.8/src/omnata_plugin_devkit/jinja_templates/CONNECTION_TEST.sql.jinja
--rw-r--r--   0        0        0     1441 2024-02-13 08:55:19.820329 omnata_plugin_devkit-0.3.8/src/omnata_plugin_devkit/jinja_templates/CONSTRUCT_FORM_OPTION.sql.jinja
--rw-r--r--   0        0        0     1312 2024-02-13 08:55:19.824329 omnata_plugin_devkit-0.3.8/src/omnata_plugin_devkit/jinja_templates/CREATE_BILLING_EVENTS.sql.jinja
--rw-r--r--   0        0        0      842 2024-02-13 08:55:19.824329 omnata_plugin_devkit-0.3.8/src/omnata_plugin_devkit/jinja_templates/CREATE_GENERIC_SECRET_OBJECT.sql.jinja
--rw-r--r--   0        0        0     1542 2024-02-13 08:55:19.824329 omnata_plugin_devkit-0.3.8/src/omnata_plugin_devkit/jinja_templates/CREATE_GENERIC_SECRET_OBJECT_FROM_EXISTING.sql.jinja
--rw-r--r--   0        0        0     1406 2024-02-13 08:55:19.824329 omnata_plugin_devkit-0.3.8/src/omnata_plugin_devkit/jinja_templates/CREATE_NETWORK_RULE_OBJECT.sql.jinja
--rw-r--r--   0        0        0     1296 2024-02-13 08:55:19.824329 omnata_plugin_devkit-0.3.8/src/omnata_plugin_devkit/jinja_templates/CREATE_NETWORK_RULE_OBJECT_FROM_EXISTING.sql.jinja
--rw-r--r--   0        0        0     1140 2024-02-13 08:55:19.824329 omnata_plugin_devkit-0.3.8/src/omnata_plugin_devkit/jinja_templates/CREATE_OAUTH_SECRET_OBJECT.sql.jinja
--rw-r--r--   0        0        0     2176 2024-02-13 08:55:19.824329 omnata_plugin_devkit-0.3.8/src/omnata_plugin_devkit/jinja_templates/INBOUND_LIST_STREAMS.sql.jinja
--rw-r--r--   0        0        0     1448 2024-02-13 08:55:19.824329 omnata_plugin_devkit-0.3.8/src/omnata_plugin_devkit/jinja_templates/NETWORK_ADDRESSES.sql.jinja
--rw-r--r--   0        0        0     2434 2024-02-13 08:55:19.824329 omnata_plugin_devkit-0.3.8/src/omnata_plugin_devkit/jinja_templates/NGROK_POST_TUNNEL_FIELDS.sql.jinja
--rw-r--r--   0        0        0     1642 2024-02-13 08:55:19.824329 omnata_plugin_devkit-0.3.8/src/omnata_plugin_devkit/jinja_templates/OUTBOUND_RECORD_VALIDATOR.sql.jinja
--rw-r--r--   0        0        0      836 2024-02-13 08:55:19.824329 omnata_plugin_devkit-0.3.8/src/omnata_plugin_devkit/jinja_templates/PENDING_API_CONFIGURATION.sql.jinja
--rw-r--r--   0        0        0     1737 2024-02-13 08:55:19.824329 omnata_plugin_devkit-0.3.8/src/omnata_plugin_devkit/jinja_templates/POST_INSTALL_ACTIONS.sql.jinja
--rw-r--r--   0        0        0      801 2024-02-13 08:55:19.824329 omnata_plugin_devkit-0.3.8/src/omnata_plugin_devkit/jinja_templates/RETRIEVE_NETWORK_RULE_OBJECT.sql.jinja
--rw-r--r--   0        0        0     1663 2024-02-13 08:55:19.824329 omnata_plugin_devkit-0.3.8/src/omnata_plugin_devkit/jinja_templates/RETRIEVE_SECRETS.sql.jinja
--rw-r--r--   0        0        0     1245 2024-02-13 08:55:19.824329 omnata_plugin_devkit-0.3.8/src/omnata_plugin_devkit/jinja_templates/SYNC.sql.jinja
--rw-r--r--   0        0        0      852 2024-02-13 08:55:19.824329 omnata_plugin_devkit-0.3.8/src/omnata_plugin_devkit/jinja_templates/TEST_CALLBACK.sql.jinja
--rw-r--r--   0        0        0     1964 2024-02-13 08:55:19.824329 omnata_plugin_devkit-0.3.8/src/omnata_plugin_devkit/jinja_templates/TEST_OAUTH_TOKEN_EXISTS.sql.jinja
--rw-r--r--   0        0        0     4501 2024-02-13 08:55:19.824329 omnata_plugin_devkit-0.3.8/src/omnata_plugin_devkit/jinja_templates/TUNNEL_TEST.sql.jinja
--rw-r--r--   0        0        0     2498 2024-02-13 08:55:19.824329 omnata_plugin_devkit-0.3.8/src/omnata_plugin_devkit/jinja_templates/UPDATE_API_CONFIGURATION.sql.jinja
--rw-r--r--   0        0        0     2027 2024-02-13 08:55:19.824329 omnata_plugin_devkit-0.3.8/src/omnata_plugin_devkit/jinja_templates/UPDATE_GENERIC_SECRET_OBJECT.sql.jinja
--rw-r--r--   0        0        0      717 2024-02-13 08:55:19.824329 omnata_plugin_devkit-0.3.8/src/omnata_plugin_devkit/jinja_templates/UPDATE_GENERIC_SECRET_OBJECT_OLD.sql.jinja
--rw-r--r--   0        0        0     1101 2024-02-13 08:55:19.824329 omnata_plugin_devkit-0.3.8/src/omnata_plugin_devkit/jinja_templates/UPDATE_NETWORK_RULE_OBJECT.sql.jinja
--rw-r--r--   0        0        0      443 2024-02-13 08:55:19.824329 omnata_plugin_devkit-0.3.8/src/omnata_plugin_devkit/jinja_templates/manifest.yml.jinja
--rw-r--r--   0        0        0     4661 2024-02-13 08:55:19.824329 omnata_plugin_devkit-0.3.8/src/omnata_plugin_devkit/native_app_packaging.py
--rw-r--r--   0        0        0     2572 2024-02-13 08:55:19.824329 omnata_plugin_devkit-0.3.8/src/omnata_plugin_devkit/plugin_registration.py
--rw-r--r--   0        0        0      596 2024-02-13 08:55:19.824329 omnata_plugin_devkit-0.3.8/src/omnata_plugin_devkit/plugin_template/icon.svg
--rw-r--r--   0        0        0    10691 2024-02-13 08:55:19.824329 omnata_plugin_devkit-0.3.8/src/omnata_plugin_devkit/plugin_template/plugin.py
--rw-r--r--   0        0        0       30 2024-02-13 08:55:19.824329 omnata_plugin_devkit-0.3.8/src/omnata_plugin_devkit/plugin_template/requirements.txt
--rw-r--r--   0        0        0    31937 2024-02-13 08:55:19.824329 omnata_plugin_devkit-0.3.8/src/omnata_plugin_devkit/plugin_uploader.py
--rw-r--r--   0        0        0   100083 2024-02-13 08:55:19.824329 omnata_plugin_devkit-0.3.8/src/omnata_plugin_devkit/streamlit/plugin_configuration.py
--rw-r--r--   0        0        0    14918 2024-02-13 08:55:19.824329 omnata_plugin_devkit-0.3.8/src/omnata_plugin_devkit/test_step_definitions.py
--rw-r--r--   0        0        0     1037 1970-01-01 00:00:00.000000 omnata_plugin_devkit-0.3.8/PKG-INFO
+-rw-r--r--   0        0        0    26526 2024-02-15 06:29:41.206178 omnata_plugin_devkit-0.3.9/LICENSE
+-rw-r--r--   0        0        0      357 2024-02-15 06:29:41.206178 omnata_plugin_devkit-0.3.9/README.md
+-rw-r--r--   0        0        0      683 2024-02-15 06:29:41.210178 omnata_plugin_devkit-0.3.9/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-02-15 06:29:41.210178 omnata_plugin_devkit-0.3.9/src/omnata_plugin_devkit/__init__.py
+-rw-r--r--   0        0        0    12862 2024-02-15 06:29:41.210178 omnata_plugin_devkit-0.3.9/src/omnata_plugin_devkit/airbyte_wrapper.py
+-rw-r--r--   0        0        0     6701 2024-02-15 06:29:41.210178 omnata_plugin_devkit-0.3.9/src/omnata_plugin_devkit/cli/__init__.py
+-rw-r--r--   0        0        0    39347 2024-02-15 06:29:41.210178 omnata_plugin_devkit-0.3.9/src/omnata_plugin_devkit/development_session.py
+-rw-r--r--   0        0        0      508 2024-02-15 06:29:41.210178 omnata_plugin_devkit-0.3.9/src/omnata_plugin_devkit/initialiser.py
+-rw-r--r--   0        0        0     1694 2024-02-15 06:29:41.210178 omnata_plugin_devkit-0.3.9/src/omnata_plugin_devkit/jinja_templates/API_LIMITS.sql.jinja
+-rw-r--r--   0        0        0     2660 2024-02-15 06:29:41.210178 omnata_plugin_devkit-0.3.9/src/omnata_plugin_devkit/jinja_templates/CONFIGURATION_FORM.sql.jinja
+-rw-r--r--   0        0        0    10515 2024-02-15 06:29:41.210178 omnata_plugin_devkit-0.3.9/src/omnata_plugin_devkit/jinja_templates/CONFIGURE_APIS.sql.jinja
+-rw-r--r--   0        0        0     1251 2024-02-15 06:29:41.210178 omnata_plugin_devkit-0.3.9/src/omnata_plugin_devkit/jinja_templates/CONNECTION_FORM.sql.jinja
+-rw-r--r--   0        0        0     1869 2024-02-15 06:29:41.210178 omnata_plugin_devkit-0.3.9/src/omnata_plugin_devkit/jinja_templates/CONNECTION_TEST.sql.jinja
+-rw-r--r--   0        0        0     1441 2024-02-15 06:29:41.210178 omnata_plugin_devkit-0.3.9/src/omnata_plugin_devkit/jinja_templates/CONSTRUCT_FORM_OPTION.sql.jinja
+-rw-r--r--   0        0        0     1312 2024-02-15 06:29:41.210178 omnata_plugin_devkit-0.3.9/src/omnata_plugin_devkit/jinja_templates/CREATE_BILLING_EVENTS.sql.jinja
+-rw-r--r--   0        0        0      842 2024-02-15 06:29:41.210178 omnata_plugin_devkit-0.3.9/src/omnata_plugin_devkit/jinja_templates/CREATE_GENERIC_SECRET_OBJECT.sql.jinja
+-rw-r--r--   0        0        0     1542 2024-02-15 06:29:41.210178 omnata_plugin_devkit-0.3.9/src/omnata_plugin_devkit/jinja_templates/CREATE_GENERIC_SECRET_OBJECT_FROM_EXISTING.sql.jinja
+-rw-r--r--   0        0        0     1406 2024-02-15 06:29:41.210178 omnata_plugin_devkit-0.3.9/src/omnata_plugin_devkit/jinja_templates/CREATE_NETWORK_RULE_OBJECT.sql.jinja
+-rw-r--r--   0        0        0     1296 2024-02-15 06:29:41.210178 omnata_plugin_devkit-0.3.9/src/omnata_plugin_devkit/jinja_templates/CREATE_NETWORK_RULE_OBJECT_FROM_EXISTING.sql.jinja
+-rw-r--r--   0        0        0     1140 2024-02-15 06:29:41.210178 omnata_plugin_devkit-0.3.9/src/omnata_plugin_devkit/jinja_templates/CREATE_OAUTH_SECRET_OBJECT.sql.jinja
+-rw-r--r--   0        0        0     2176 2024-02-15 06:29:41.210178 omnata_plugin_devkit-0.3.9/src/omnata_plugin_devkit/jinja_templates/INBOUND_LIST_STREAMS.sql.jinja
+-rw-r--r--   0        0        0     1448 2024-02-15 06:29:41.210178 omnata_plugin_devkit-0.3.9/src/omnata_plugin_devkit/jinja_templates/NETWORK_ADDRESSES.sql.jinja
+-rw-r--r--   0        0        0     2434 2024-02-15 06:29:41.210178 omnata_plugin_devkit-0.3.9/src/omnata_plugin_devkit/jinja_templates/NGROK_POST_TUNNEL_FIELDS.sql.jinja
+-rw-r--r--   0        0        0     1642 2024-02-15 06:29:41.210178 omnata_plugin_devkit-0.3.9/src/omnata_plugin_devkit/jinja_templates/OUTBOUND_RECORD_VALIDATOR.sql.jinja
+-rw-r--r--   0        0        0      836 2024-02-15 06:29:41.210178 omnata_plugin_devkit-0.3.9/src/omnata_plugin_devkit/jinja_templates/PENDING_API_CONFIGURATION.sql.jinja
+-rw-r--r--   0        0        0     1737 2024-02-15 06:29:41.210178 omnata_plugin_devkit-0.3.9/src/omnata_plugin_devkit/jinja_templates/POST_INSTALL_ACTIONS.sql.jinja
+-rw-r--r--   0        0        0      801 2024-02-15 06:29:41.210178 omnata_plugin_devkit-0.3.9/src/omnata_plugin_devkit/jinja_templates/RETRIEVE_NETWORK_RULE_OBJECT.sql.jinja
+-rw-r--r--   0        0        0     1663 2024-02-15 06:29:41.210178 omnata_plugin_devkit-0.3.9/src/omnata_plugin_devkit/jinja_templates/RETRIEVE_SECRETS.sql.jinja
+-rw-r--r--   0        0        0     1245 2024-02-15 06:29:41.210178 omnata_plugin_devkit-0.3.9/src/omnata_plugin_devkit/jinja_templates/SYNC.sql.jinja
+-rw-r--r--   0        0        0      852 2024-02-15 06:29:41.210178 omnata_plugin_devkit-0.3.9/src/omnata_plugin_devkit/jinja_templates/TEST_CALLBACK.sql.jinja
+-rw-r--r--   0        0        0     1964 2024-02-15 06:29:41.210178 omnata_plugin_devkit-0.3.9/src/omnata_plugin_devkit/jinja_templates/TEST_OAUTH_TOKEN_EXISTS.sql.jinja
+-rw-r--r--   0        0        0     4501 2024-02-15 06:29:41.210178 omnata_plugin_devkit-0.3.9/src/omnata_plugin_devkit/jinja_templates/TUNNEL_TEST.sql.jinja
+-rw-r--r--   0        0        0     2498 2024-02-15 06:29:41.210178 omnata_plugin_devkit-0.3.9/src/omnata_plugin_devkit/jinja_templates/UPDATE_API_CONFIGURATION.sql.jinja
+-rw-r--r--   0        0        0     2027 2024-02-15 06:29:41.210178 omnata_plugin_devkit-0.3.9/src/omnata_plugin_devkit/jinja_templates/UPDATE_GENERIC_SECRET_OBJECT.sql.jinja
+-rw-r--r--   0        0        0      717 2024-02-15 06:29:41.210178 omnata_plugin_devkit-0.3.9/src/omnata_plugin_devkit/jinja_templates/UPDATE_GENERIC_SECRET_OBJECT_OLD.sql.jinja
+-rw-r--r--   0        0        0     1101 2024-02-15 06:29:41.210178 omnata_plugin_devkit-0.3.9/src/omnata_plugin_devkit/jinja_templates/UPDATE_NETWORK_RULE_OBJECT.sql.jinja
+-rw-r--r--   0        0        0      443 2024-02-15 06:29:41.210178 omnata_plugin_devkit-0.3.9/src/omnata_plugin_devkit/jinja_templates/manifest.yml.jinja
+-rw-r--r--   0        0        0     4661 2024-02-15 06:29:41.210178 omnata_plugin_devkit-0.3.9/src/omnata_plugin_devkit/native_app_packaging.py
+-rw-r--r--   0        0        0     2572 2024-02-15 06:29:41.210178 omnata_plugin_devkit-0.3.9/src/omnata_plugin_devkit/plugin_registration.py
+-rw-r--r--   0        0        0      596 2024-02-15 06:29:41.210178 omnata_plugin_devkit-0.3.9/src/omnata_plugin_devkit/plugin_template/icon.svg
+-rw-r--r--   0        0        0    10691 2024-02-15 06:29:41.210178 omnata_plugin_devkit-0.3.9/src/omnata_plugin_devkit/plugin_template/plugin.py
+-rw-r--r--   0        0        0       30 2024-02-15 06:29:41.210178 omnata_plugin_devkit-0.3.9/src/omnata_plugin_devkit/plugin_template/requirements.txt
+-rw-r--r--   0        0        0    31937 2024-02-15 06:29:41.210178 omnata_plugin_devkit-0.3.9/src/omnata_plugin_devkit/plugin_uploader.py
+-rw-r--r--   0        0        0   100083 2024-02-15 06:29:41.214177 omnata_plugin_devkit-0.3.9/src/omnata_plugin_devkit/streamlit/plugin_configuration.py
+-rw-r--r--   0        0        0    14918 2024-02-15 06:29:41.214177 omnata_plugin_devkit-0.3.9/src/omnata_plugin_devkit/test_step_definitions.py
+-rw-r--r--   0        0        0     1037 1970-01-01 00:00:00.000000 omnata_plugin_devkit-0.3.9/PKG-INFO
```

### Comparing `omnata_plugin_devkit-0.3.8/LICENSE` & `omnata_plugin_devkit-0.3.9/LICENSE`

 * *Files identical despite different names*

### Comparing `omnata_plugin_devkit-0.3.8/pyproject.toml` & `omnata_plugin_devkit-0.3.9/pyproject.toml`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "omnata-plugin-devkit"
-version = "0.3.8"
+version = "0.3.9"
 description = ""
 authors = ["James Weakley <james.weakley@omnata.com>"]
 readme = "README.md"
 packages = [{ include = "omnata_plugin_devkit", from = "src" }]
 
 [tool.poetry.dependencies]
 python = "~3.10"
```

### Comparing `omnata_plugin_devkit-0.3.8/src/omnata_plugin_devkit/airbyte_wrapper.py` & `omnata_plugin_devkit-0.3.9/src/omnata_plugin_devkit/airbyte_wrapper.py`

 * *Files identical despite different names*

### Comparing `omnata_plugin_devkit-0.3.8/src/omnata_plugin_devkit/cli/__init__.py` & `omnata_plugin_devkit-0.3.9/src/omnata_plugin_devkit/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `omnata_plugin_devkit-0.3.8/src/omnata_plugin_devkit/development_session.py` & `omnata_plugin_devkit-0.3.9/src/omnata_plugin_devkit/development_session.py`

 * *Files identical despite different names*

### Comparing `omnata_plugin_devkit-0.3.8/src/omnata_plugin_devkit/jinja_templates/API_LIMITS.sql.jinja` & `omnata_plugin_devkit-0.3.9/src/omnata_plugin_devkit/jinja_templates/API_LIMITS.sql.jinja`

 * *Files identical despite different names*

### Comparing `omnata_plugin_devkit-0.3.8/src/omnata_plugin_devkit/jinja_templates/CONFIGURATION_FORM.sql.jinja` & `omnata_plugin_devkit-0.3.9/src/omnata_plugin_devkit/jinja_templates/CONFIGURATION_FORM.sql.jinja`

 * *Files identical despite different names*

### Comparing `omnata_plugin_devkit-0.3.8/src/omnata_plugin_devkit/jinja_templates/CONFIGURE_APIS.sql.jinja` & `omnata_plugin_devkit-0.3.9/src/omnata_plugin_devkit/jinja_templates/CONFIGURE_APIS.sql.jinja`

 * *Files 5% similar despite different names*

```diff
@@ -181,14 +181,37 @@
                         SECRETS = (${secrets.join(',')})`
         snowflake.log("info", `Executing SQL: ${sqlText}`);
         snowflake.createStatement( {
             sqlText:sqlText,
             binds:[]
         } ).execute();
     }
+    // same thing for stored procs (treat them as UDFs really)
+    var sqlText = `select PROCEDURE_NAME||
+                            '('||array_to_string(REGEXP_EXTRACT_ALL(replace(ARGUMENT_SIGNATURE,', ',','),'\\\\s\\\\w+'),',')||')' as         
+                            PROC_SIGNATURE
+                    from INFORMATION_SCHEMA.PROCEDURES
+                    where PROCEDURE_SCHEMA='UDFS'
+                    and PROCEDURE_LANGUAGE in ('JAVA','PYTHON')`;
+    snowflake.log("info", `Executing SQL: ${sqlText}`);
+    var udfResults = snowflake.createStatement( {
+        sqlText: sqlText,
+        binds:[]
+    } ).execute();
+    while (udfResults.next()) {
+        var udfSig = udfResults.getColumnValue(1);
+        var sqlText = `alter procedure UDFS.${udfSig}
+                    set EXTERNAL_ACCESS_INTEGRATIONS = (${integrationNames.join(',')}),
+                        SECRETS = (${secrets.join(',')})`
+        snowflake.log("info", `Executing SQL: ${sqlText}`);
+        snowflake.createStatement( {
+            sqlText:sqlText,
+            binds:[]
+        } ).execute();
+    }
     // write the latest list of applied external access integrations back to the registration table
     var appliedIntegrationsResults = snowflake.createStatement( {
         sqlText: `update DATA.OMNATA_REGISTRATION
                     set EXTERNAL_ACCESS_INTEGRATIONS_APPLIED = PARSE_JSON(?)`,
         binds:[JSON.stringify(externalAccessIntegrations)]
     } ).execute();
     return {
```

### Comparing `omnata_plugin_devkit-0.3.8/src/omnata_plugin_devkit/jinja_templates/CONNECTION_FORM.sql.jinja` & `omnata_plugin_devkit-0.3.9/src/omnata_plugin_devkit/jinja_templates/CONNECTION_FORM.sql.jinja`

 * *Files identical despite different names*

### Comparing `omnata_plugin_devkit-0.3.8/src/omnata_plugin_devkit/jinja_templates/CONNECTION_TEST.sql.jinja` & `omnata_plugin_devkit-0.3.9/src/omnata_plugin_devkit/jinja_templates/CONNECTION_TEST.sql.jinja`

 * *Files identical despite different names*

### Comparing `omnata_plugin_devkit-0.3.8/src/omnata_plugin_devkit/jinja_templates/CONSTRUCT_FORM_OPTION.sql.jinja` & `omnata_plugin_devkit-0.3.9/src/omnata_plugin_devkit/jinja_templates/CONSTRUCT_FORM_OPTION.sql.jinja`

 * *Files identical despite different names*

### Comparing `omnata_plugin_devkit-0.3.8/src/omnata_plugin_devkit/jinja_templates/CREATE_BILLING_EVENTS.sql.jinja` & `omnata_plugin_devkit-0.3.9/src/omnata_plugin_devkit/jinja_templates/CREATE_BILLING_EVENTS.sql.jinja`

 * *Files identical despite different names*

### Comparing `omnata_plugin_devkit-0.3.8/src/omnata_plugin_devkit/jinja_templates/CREATE_GENERIC_SECRET_OBJECT.sql.jinja` & `omnata_plugin_devkit-0.3.9/src/omnata_plugin_devkit/jinja_templates/CREATE_GENERIC_SECRET_OBJECT.sql.jinja`

 * *Files identical despite different names*

### Comparing `omnata_plugin_devkit-0.3.8/src/omnata_plugin_devkit/jinja_templates/CREATE_GENERIC_SECRET_OBJECT_FROM_EXISTING.sql.jinja` & `omnata_plugin_devkit-0.3.9/src/omnata_plugin_devkit/jinja_templates/CREATE_GENERIC_SECRET_OBJECT_FROM_EXISTING.sql.jinja`

 * *Files identical despite different names*

### Comparing `omnata_plugin_devkit-0.3.8/src/omnata_plugin_devkit/jinja_templates/CREATE_NETWORK_RULE_OBJECT.sql.jinja` & `omnata_plugin_devkit-0.3.9/src/omnata_plugin_devkit/jinja_templates/CREATE_NETWORK_RULE_OBJECT.sql.jinja`

 * *Files identical despite different names*

### Comparing `omnata_plugin_devkit-0.3.8/src/omnata_plugin_devkit/jinja_templates/CREATE_NETWORK_RULE_OBJECT_FROM_EXISTING.sql.jinja` & `omnata_plugin_devkit-0.3.9/src/omnata_plugin_devkit/jinja_templates/CREATE_NETWORK_RULE_OBJECT_FROM_EXISTING.sql.jinja`

 * *Files identical despite different names*

### Comparing `omnata_plugin_devkit-0.3.8/src/omnata_plugin_devkit/jinja_templates/CREATE_OAUTH_SECRET_OBJECT.sql.jinja` & `omnata_plugin_devkit-0.3.9/src/omnata_plugin_devkit/jinja_templates/CREATE_OAUTH_SECRET_OBJECT.sql.jinja`

 * *Files identical despite different names*

### Comparing `omnata_plugin_devkit-0.3.8/src/omnata_plugin_devkit/jinja_templates/INBOUND_LIST_STREAMS.sql.jinja` & `omnata_plugin_devkit-0.3.9/src/omnata_plugin_devkit/jinja_templates/INBOUND_LIST_STREAMS.sql.jinja`

 * *Files identical despite different names*

### Comparing `omnata_plugin_devkit-0.3.8/src/omnata_plugin_devkit/jinja_templates/NETWORK_ADDRESSES.sql.jinja` & `omnata_plugin_devkit-0.3.9/src/omnata_plugin_devkit/jinja_templates/NETWORK_ADDRESSES.sql.jinja`

 * *Files identical despite different names*

### Comparing `omnata_plugin_devkit-0.3.8/src/omnata_plugin_devkit/jinja_templates/NGROK_POST_TUNNEL_FIELDS.sql.jinja` & `omnata_plugin_devkit-0.3.9/src/omnata_plugin_devkit/jinja_templates/NGROK_POST_TUNNEL_FIELDS.sql.jinja`

 * *Files identical despite different names*

### Comparing `omnata_plugin_devkit-0.3.8/src/omnata_plugin_devkit/jinja_templates/OUTBOUND_RECORD_VALIDATOR.sql.jinja` & `omnata_plugin_devkit-0.3.9/src/omnata_plugin_devkit/jinja_templates/OUTBOUND_RECORD_VALIDATOR.sql.jinja`

 * *Files identical despite different names*

### Comparing `omnata_plugin_devkit-0.3.8/src/omnata_plugin_devkit/jinja_templates/PENDING_API_CONFIGURATION.sql.jinja` & `omnata_plugin_devkit-0.3.9/src/omnata_plugin_devkit/jinja_templates/PENDING_API_CONFIGURATION.sql.jinja`

 * *Files identical despite different names*

### Comparing `omnata_plugin_devkit-0.3.8/src/omnata_plugin_devkit/jinja_templates/POST_INSTALL_ACTIONS.sql.jinja` & `omnata_plugin_devkit-0.3.9/src/omnata_plugin_devkit/jinja_templates/POST_INSTALL_ACTIONS.sql.jinja`

 * *Files identical despite different names*

### Comparing `omnata_plugin_devkit-0.3.8/src/omnata_plugin_devkit/jinja_templates/RETRIEVE_NETWORK_RULE_OBJECT.sql.jinja` & `omnata_plugin_devkit-0.3.9/src/omnata_plugin_devkit/jinja_templates/RETRIEVE_NETWORK_RULE_OBJECT.sql.jinja`

 * *Files identical despite different names*

### Comparing `omnata_plugin_devkit-0.3.8/src/omnata_plugin_devkit/jinja_templates/RETRIEVE_SECRETS.sql.jinja` & `omnata_plugin_devkit-0.3.9/src/omnata_plugin_devkit/jinja_templates/RETRIEVE_SECRETS.sql.jinja`

 * *Files identical despite different names*

### Comparing `omnata_plugin_devkit-0.3.8/src/omnata_plugin_devkit/jinja_templates/SYNC.sql.jinja` & `omnata_plugin_devkit-0.3.9/src/omnata_plugin_devkit/jinja_templates/SYNC.sql.jinja`

 * *Files identical despite different names*

### Comparing `omnata_plugin_devkit-0.3.8/src/omnata_plugin_devkit/jinja_templates/TEST_CALLBACK.sql.jinja` & `omnata_plugin_devkit-0.3.9/src/omnata_plugin_devkit/jinja_templates/TEST_CALLBACK.sql.jinja`

 * *Files identical despite different names*

### Comparing `omnata_plugin_devkit-0.3.8/src/omnata_plugin_devkit/jinja_templates/TEST_OAUTH_TOKEN_EXISTS.sql.jinja` & `omnata_plugin_devkit-0.3.9/src/omnata_plugin_devkit/jinja_templates/TEST_OAUTH_TOKEN_EXISTS.sql.jinja`

 * *Files identical despite different names*

### Comparing `omnata_plugin_devkit-0.3.8/src/omnata_plugin_devkit/jinja_templates/TUNNEL_TEST.sql.jinja` & `omnata_plugin_devkit-0.3.9/src/omnata_plugin_devkit/jinja_templates/TUNNEL_TEST.sql.jinja`

 * *Files identical despite different names*

### Comparing `omnata_plugin_devkit-0.3.8/src/omnata_plugin_devkit/jinja_templates/UPDATE_API_CONFIGURATION.sql.jinja` & `omnata_plugin_devkit-0.3.9/src/omnata_plugin_devkit/jinja_templates/UPDATE_API_CONFIGURATION.sql.jinja`

 * *Files identical despite different names*

### Comparing `omnata_plugin_devkit-0.3.8/src/omnata_plugin_devkit/jinja_templates/UPDATE_GENERIC_SECRET_OBJECT.sql.jinja` & `omnata_plugin_devkit-0.3.9/src/omnata_plugin_devkit/jinja_templates/UPDATE_GENERIC_SECRET_OBJECT.sql.jinja`

 * *Files identical despite different names*

### Comparing `omnata_plugin_devkit-0.3.8/src/omnata_plugin_devkit/jinja_templates/UPDATE_GENERIC_SECRET_OBJECT_OLD.sql.jinja` & `omnata_plugin_devkit-0.3.9/src/omnata_plugin_devkit/jinja_templates/UPDATE_GENERIC_SECRET_OBJECT_OLD.sql.jinja`

 * *Files identical despite different names*

### Comparing `omnata_plugin_devkit-0.3.8/src/omnata_plugin_devkit/jinja_templates/UPDATE_NETWORK_RULE_OBJECT.sql.jinja` & `omnata_plugin_devkit-0.3.9/src/omnata_plugin_devkit/jinja_templates/UPDATE_NETWORK_RULE_OBJECT.sql.jinja`

 * *Files identical despite different names*

### Comparing `omnata_plugin_devkit-0.3.8/src/omnata_plugin_devkit/native_app_packaging.py` & `omnata_plugin_devkit-0.3.9/src/omnata_plugin_devkit/native_app_packaging.py`

 * *Files identical despite different names*

### Comparing `omnata_plugin_devkit-0.3.8/src/omnata_plugin_devkit/plugin_registration.py` & `omnata_plugin_devkit-0.3.9/src/omnata_plugin_devkit/plugin_registration.py`

 * *Files identical despite different names*

### Comparing `omnata_plugin_devkit-0.3.8/src/omnata_plugin_devkit/plugin_template/icon.svg` & `omnata_plugin_devkit-0.3.9/src/omnata_plugin_devkit/plugin_template/icon.svg`

 * *Files identical despite different names*

### Comparing `omnata_plugin_devkit-0.3.8/src/omnata_plugin_devkit/plugin_template/plugin.py` & `omnata_plugin_devkit-0.3.9/src/omnata_plugin_devkit/plugin_template/plugin.py`

 * *Files identical despite different names*

### Comparing `omnata_plugin_devkit-0.3.8/src/omnata_plugin_devkit/plugin_uploader.py` & `omnata_plugin_devkit-0.3.9/src/omnata_plugin_devkit/plugin_uploader.py`

 * *Files identical despite different names*

### Comparing `omnata_plugin_devkit-0.3.8/src/omnata_plugin_devkit/streamlit/plugin_configuration.py` & `omnata_plugin_devkit-0.3.9/src/omnata_plugin_devkit/streamlit/plugin_configuration.py`

 * *Files identical despite different names*

### Comparing `omnata_plugin_devkit-0.3.8/src/omnata_plugin_devkit/test_step_definitions.py` & `omnata_plugin_devkit-0.3.9/src/omnata_plugin_devkit/test_step_definitions.py`

 * *Files identical despite different names*

### Comparing `omnata_plugin_devkit-0.3.8/PKG-INFO` & `omnata_plugin_devkit-0.3.9/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: omnata-plugin-devkit
-Version: 0.3.8
+Version: 0.3.9
 Summary: 
 Author: James Weakley
 Author-email: james.weakley@omnata.com
 Requires-Python: >=3.10,<3.11
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Requires-Dist: behave (>=1.2,<2.0)
```

