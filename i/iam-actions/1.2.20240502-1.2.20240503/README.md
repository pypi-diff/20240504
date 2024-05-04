# Comparing `tmp/iam_actions-1.2.20240502.tar.gz` & `tmp/iam_actions-1.2.20240503.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "iam_actions-1.2.20240502.tar", max compression
+gzip compressed data, was "iam_actions-1.2.20240503.tar", max compression
```

## Comparing `iam_actions-1.2.20240502.tar` & `iam_actions-1.2.20240503.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0     1071 2024-05-02 02:18:40.934717 iam_actions-1.2.20240502/LICENSE
--rw-r--r--   0        0        0     2302 2024-05-02 02:18:40.934717 iam_actions-1.2.20240502/README.md
--rw-r--r--   0        0        0      228 2024-05-02 02:18:40.934717 iam_actions-1.2.20240502/iam_actions/__init__.py
--rw-r--r--   0        0        0  4824523 2024-05-02 02:20:22.234313 iam_actions-1.2.20240502/iam_actions/actions.json
--rw-r--r--   0        0        0      496 2024-05-02 02:18:40.934717 iam_actions-1.2.20240502/iam_actions/data.py
--rw-r--r--   0        0        0       80 2024-05-02 02:18:40.934717 iam_actions-1.2.20240502/iam_actions/generate/__init__.py
--rw-r--r--   0        0        0     3097 2024-05-02 02:18:40.934717 iam_actions-1.2.20240502/iam_actions/generate/action_map.py
--rw-r--r--   0        0        0    23329 2024-05-02 02:18:40.934717 iam_actions-1.2.20240502/iam_actions/generate/aws_docs.py
--rw-r--r--   0        0        0     3739 2024-05-02 02:18:40.934717 iam_actions-1.2.20240502/iam_actions/generate/generate.py
--rw-r--r--   0        0        0     3272 2024-05-02 02:18:40.934717 iam_actions-1.2.20240502/iam_actions/generate/notifier.py
--rw-r--r--   0        0        0     1902 2024-05-02 02:18:40.934717 iam_actions-1.2.20240502/iam_actions/generate/resource_type.py
--rw-r--r--   0        0        0     2277 2024-05-02 02:18:40.934717 iam_actions-1.2.20240502/iam_actions/generate/services.py
--rw-r--r--   0        0        0   627645 2024-05-02 02:20:22.234313 iam_actions-1.2.20240502/iam_actions/policies.json
--rw-r--r--   0        0        0   209154 2024-05-02 02:20:22.234313 iam_actions-1.2.20240502/iam_actions/resourcetypes.json
--rw-r--r--   0        0        0   609039 2024-05-02 02:20:22.234313 iam_actions-1.2.20240502/iam_actions/services.json
--rw-r--r--   0        0        0     1154 2024-05-02 02:20:22.894311 iam_actions-1.2.20240502/pyproject.toml
--rw-r--r--   0        0        0     3024 1970-01-01 00:00:00.000000 iam_actions-1.2.20240502/setup.py
--rw-r--r--   0        0        0     2915 1970-01-01 00:00:00.000000 iam_actions-1.2.20240502/PKG-INFO
+-rw-r--r--   0        0        0     1071 2024-05-03 02:21:09.387521 iam_actions-1.2.20240503/LICENSE
+-rw-r--r--   0        0        0     2302 2024-05-03 02:21:09.387521 iam_actions-1.2.20240503/README.md
+-rw-r--r--   0        0        0      228 2024-05-03 02:21:09.387521 iam_actions-1.2.20240503/iam_actions/__init__.py
+-rw-r--r--   0        0        0  4825636 2024-05-03 02:23:06.800053 iam_actions-1.2.20240503/iam_actions/actions.json
+-rw-r--r--   0        0        0      496 2024-05-03 02:21:09.387521 iam_actions-1.2.20240503/iam_actions/data.py
+-rw-r--r--   0        0        0       80 2024-05-03 02:21:09.387521 iam_actions-1.2.20240503/iam_actions/generate/__init__.py
+-rw-r--r--   0        0        0     3097 2024-05-03 02:21:09.387521 iam_actions-1.2.20240503/iam_actions/generate/action_map.py
+-rw-r--r--   0        0        0    23329 2024-05-03 02:21:09.387521 iam_actions-1.2.20240503/iam_actions/generate/aws_docs.py
+-rw-r--r--   0        0        0     3739 2024-05-03 02:21:09.387521 iam_actions-1.2.20240503/iam_actions/generate/generate.py
+-rw-r--r--   0        0        0     3272 2024-05-03 02:21:09.387521 iam_actions-1.2.20240503/iam_actions/generate/notifier.py
+-rw-r--r--   0        0        0     1902 2024-05-03 02:21:09.387521 iam_actions-1.2.20240503/iam_actions/generate/resource_type.py
+-rw-r--r--   0        0        0     2277 2024-05-03 02:21:09.387521 iam_actions-1.2.20240503/iam_actions/generate/services.py
+-rw-r--r--   0        0        0   627685 2024-05-03 02:23:06.800053 iam_actions-1.2.20240503/iam_actions/policies.json
+-rw-r--r--   0        0        0   209301 2024-05-03 02:23:06.800053 iam_actions-1.2.20240503/iam_actions/resourcetypes.json
+-rw-r--r--   0        0        0   609078 2024-05-03 02:23:06.800053 iam_actions-1.2.20240503/iam_actions/services.json
+-rw-r--r--   0        0        0     1154 2024-05-03 02:23:07.448056 iam_actions-1.2.20240503/pyproject.toml
+-rw-r--r--   0        0        0     3024 1970-01-01 00:00:00.000000 iam_actions-1.2.20240503/setup.py
+-rw-r--r--   0        0        0     2915 1970-01-01 00:00:00.000000 iam_actions-1.2.20240503/PKG-INFO
```

### Comparing `iam_actions-1.2.20240502/LICENSE` & `iam_actions-1.2.20240503/LICENSE`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20240502/README.md` & `iam_actions-1.2.20240503/README.md`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20240502/iam_actions/actions.json` & `iam_actions-1.2.20240503/iam_actions/actions.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9999776581881522%*

 * *Differences: {"'sms-voice'": "{'ListTagsForResource': {'resources': {insert: [(4, 'ProtectConfiguration'), (5, "*

 * *                "'Registration'), (6, 'RegistrationAttachment'), (8, "*

 * *                "'VerifiedDestinationNumber')]}}, 'TagResource': {'resources': {insert: [(4, "*

 * *                "'ProtectConfiguration')]}}, 'UntagResource': {'resources': {insert: [(4, "*

 * *                "'ProtectConfiguration')]}}, 'DescribeProtectConfigurations': {'access_level': "*

 * *                "'Read', 'description': 'Grants permissio […]*

```diff
@@ -151937,20 +151937,23 @@
             "resources": [
                 "PhoneNumber",
                 "Pool",
                 "SenderId"
             ]
         },
         "AssociateProtectConfiguration": {
-            "access_level": "Undocumented",
+            "access_level": "Write",
             "action": "AssociateProtectConfiguration",
             "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "description": "Grants permission to associate a protect configuration to a configuration set",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "ConfigurationSet",
+                "ProtectConfiguration"
+            ]
         },
         "CreateConfigurationSet": {
             "access_level": "Write",
             "action": "CreateConfigurationSet",
             "condition_keys": [],
             "description": "Create a new configuration set. After you create the configuration set, you can add one or more event destinations to it.",
             "orphan": false,
@@ -151996,18 +151999,21 @@
             "orphan": false,
             "resources": [
                 "PhoneNumber",
                 "SenderId"
             ]
         },
         "CreateProtectConfiguration": {
-            "access_level": "Undocumented",
+            "access_level": "Write",
             "action": "CreateProtectConfiguration",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "condition_keys": [
+                "aws:RequestTag/${TagKey}",
+                "aws:TagKeys"
+            ],
+            "description": "Grants permission to create a protect configuration",
             "orphan": false,
             "resources": []
         },
         "CreateRegistration": {
             "access_level": "Write",
             "action": "CreateRegistration",
             "condition_keys": [
@@ -152058,18 +152064,18 @@
                 "aws:TagKeys"
             ],
             "description": "Grants permission to create a verified destination number",
             "orphan": false,
             "resources": []
         },
         "DeleteAccountDefaultProtectConfiguration": {
-            "access_level": "Undocumented",
+            "access_level": "Write",
             "action": "DeleteAccountDefaultProtectConfiguration",
             "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "description": "Grants permission to delete the account default protect configuration",
             "orphan": false,
             "resources": []
         },
         "DeleteConfigurationSet": {
             "access_level": "Write",
             "action": "DeleteConfigurationSet",
             "condition_keys": [],
@@ -152123,18 +152129,18 @@
             "orphan": false,
             "resources": [
                 "PhoneNumber",
                 "Pool"
             ]
         },
         "DeleteMediaMessageSpendLimitOverride": {
-            "access_level": "Undocumented",
+            "access_level": "Write",
             "action": "DeleteMediaMessageSpendLimitOverride",
             "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "description": "Grants permission to delete an override for your account's media messaging monthly spend limit",
             "orphan": false,
             "resources": []
         },
         "DeleteOptOutList": {
             "access_level": "Write",
             "action": "DeleteOptOutList",
             "condition_keys": [],
@@ -152161,20 +152167,22 @@
             "description": "Grants permission to delete a pool",
             "orphan": false,
             "resources": [
                 "Pool"
             ]
         },
         "DeleteProtectConfiguration": {
-            "access_level": "Undocumented",
+            "access_level": "Write",
             "action": "DeleteProtectConfiguration",
             "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "description": "Grants permission to delete a protect configuration",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "ProtectConfiguration"
+            ]
         },
         "DeleteRegistration": {
             "access_level": "Write",
             "action": "DeleteRegistration",
             "condition_keys": [],
             "description": "Grants permission to delete a registration",
             "orphan": false,
@@ -152302,20 +152310,22 @@
             "description": "Grants permission to describe the pools in your account",
             "orphan": false,
             "resources": [
                 "Pool"
             ]
         },
         "DescribeProtectConfigurations": {
-            "access_level": "Undocumented",
+            "access_level": "Read",
             "action": "DescribeProtectConfigurations",
             "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "description": "Grants permission to describe the protect configurations in your account",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "ProtectConfiguration"
+            ]
         },
         "DescribeRegistrationAttachments": {
             "access_level": "Read",
             "action": "DescribeRegistrationAttachments",
             "condition_keys": [],
             "description": "Grants permission to describe the registration attachments in your account",
             "orphan": false,
@@ -152414,20 +152424,23 @@
             "resources": [
                 "PhoneNumber",
                 "Pool",
                 "SenderId"
             ]
         },
         "DisassociateProtectConfiguration": {
-            "access_level": "Undocumented",
+            "access_level": "Write",
             "action": "DisassociateProtectConfiguration",
             "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "description": "Grants permission to disassociate a protect configuration from a configuration set",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "ConfigurationSet",
+                "ProtectConfiguration"
+            ]
         },
         "DiscardRegistrationVersion": {
             "access_level": "Write",
             "action": "DiscardRegistrationVersion",
             "condition_keys": [],
             "description": "Grants permission to discard the latest version of a given registration",
             "orphan": false,
@@ -152440,20 +152453,22 @@
             "action": "GetConfigurationSetEventDestinations",
             "condition_keys": [],
             "description": "Obtain information about an event destination, including the types of events it reports, the Amazon Resource Name (ARN) of the destination, and the name of the event destination.",
             "orphan": false,
             "resources": []
         },
         "GetProtectConfigurationCountryRuleSet": {
-            "access_level": "Undocumented",
+            "access_level": "Read",
             "action": "GetProtectConfigurationCountryRuleSet",
             "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "description": "Grants permission to get the country rule set for a protect configuration",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "ProtectConfiguration"
+            ]
         },
         "ListConfigurationSets": {
             "access_level": "Read",
             "action": "ListConfigurationSets",
             "condition_keys": [],
             "description": "Return a list of configuration sets. This operation only returns the configuration sets that are associated with your account in the current AWS Region.",
             "orphan": false,
@@ -152486,15 +152501,19 @@
             "description": "Grants permission to list the tags for a resource",
             "orphan": false,
             "resources": [
                 "ConfigurationSet",
                 "OptOutList",
                 "PhoneNumber",
                 "Pool",
-                "SenderId"
+                "ProtectConfiguration",
+                "Registration",
+                "RegistrationAttachment",
+                "SenderId",
+                "VerifiedDestinationNumber"
             ]
         },
         "PutKeyword": {
             "access_level": "Write",
             "action": "PutKeyword",
             "condition_keys": [],
             "description": "Grants permission to create or update a keyword for a pool or origination phone number",
@@ -152577,20 +152596,23 @@
             "resources": [
                 "PhoneNumber",
                 "Pool",
                 "SenderId"
             ]
         },
         "SendMediaMessage": {
-            "access_level": "Undocumented",
+            "access_level": "Write",
             "action": "SendMediaMessage",
             "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "description": "Grants permission to send a media message to a destination phone number",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "PhoneNumber",
+                "Pool"
+            ]
         },
         "SendTextMessage": {
             "access_level": "Write",
             "action": "SendTextMessage",
             "condition_keys": [],
             "description": "Grants permission to send a text message to a destination phone number",
             "orphan": false,
@@ -152605,20 +152627,22 @@
             "action": "SendVoiceMessage",
             "condition_keys": [],
             "description": "Create a new voice message and send it to a recipient's phone number.",
             "orphan": false,
             "resources": []
         },
         "SetAccountDefaultProtectConfiguration": {
-            "access_level": "Undocumented",
+            "access_level": "Write",
             "action": "SetAccountDefaultProtectConfiguration",
             "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "description": "Grants permission to set a default protect configuration for the account",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "ProtectConfiguration"
+            ]
         },
         "SetDefaultMessageType": {
             "access_level": "Write",
             "action": "SetDefaultMessageType",
             "condition_keys": [],
             "description": "Grants permission to set the default message type for a configuration set",
             "orphan": false,
@@ -152633,18 +152657,18 @@
             "description": "Grants permission to set the default sender ID for a configuration set",
             "orphan": false,
             "resources": [
                 "ConfigurationSet"
             ]
         },
         "SetMediaMessageSpendLimitOverride": {
-            "access_level": "Undocumented",
+            "access_level": "Write",
             "action": "SetMediaMessageSpendLimitOverride",
             "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "description": "Grants permission to set an override for your account's media messaging monthly spend limit",
             "orphan": false,
             "resources": []
         },
         "SetTextMessageSpendLimitOverride": {
             "access_level": "Write",
             "action": "SetTextMessageSpendLimitOverride",
             "condition_keys": [],
@@ -152680,14 +152704,15 @@
             "description": "Grants permission to add tags to a resource",
             "orphan": false,
             "resources": [
                 "ConfigurationSet",
                 "OptOutList",
                 "PhoneNumber",
                 "Pool",
+                "ProtectConfiguration",
                 "Registration",
                 "RegistrationAttachment",
                 "SenderId",
                 "VerifiedDestinationNumber"
             ]
         },
         "UntagResource": {
@@ -152699,14 +152724,15 @@
             "description": "Grants permission to remove tags from a resource",
             "orphan": false,
             "resources": [
                 "ConfigurationSet",
                 "OptOutList",
                 "PhoneNumber",
                 "Pool",
+                "ProtectConfiguration",
                 "Registration",
                 "RegistrationAttachment",
                 "SenderId",
                 "VerifiedDestinationNumber"
             ]
         },
         "UpdateConfigurationSetEventDestination": {
@@ -152744,28 +152770,32 @@
             "description": "Grants permission to update a pool's configuration",
             "orphan": false,
             "resources": [
                 "Pool"
             ]
         },
         "UpdateProtectConfiguration": {
-            "access_level": "Undocumented",
+            "access_level": "Write",
             "action": "UpdateProtectConfiguration",
             "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "description": "Grants permission to update a protect configuration",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "ProtectConfiguration"
+            ]
         },
         "UpdateProtectConfigurationCountryRuleSet": {
-            "access_level": "Undocumented",
+            "access_level": "Write",
             "action": "UpdateProtectConfigurationCountryRuleSet",
             "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "description": "Grants permission to update a country rule set for a protect configuration",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "ProtectConfiguration"
+            ]
         },
         "UpdateSenderId": {
             "access_level": "Write",
             "action": "UpdateSenderId",
             "condition_keys": [],
             "description": "Grants permission to update a sender ID's configuration",
             "orphan": false,
```

### Comparing `iam_actions-1.2.20240502/iam_actions/generate/action_map.py` & `iam_actions-1.2.20240503/iam_actions/generate/action_map.py`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20240502/iam_actions/generate/aws_docs.py` & `iam_actions-1.2.20240503/iam_actions/generate/aws_docs.py`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20240502/iam_actions/generate/generate.py` & `iam_actions-1.2.20240503/iam_actions/generate/generate.py`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20240502/iam_actions/generate/notifier.py` & `iam_actions-1.2.20240503/iam_actions/generate/notifier.py`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20240502/iam_actions/generate/resource_type.py` & `iam_actions-1.2.20240503/iam_actions/generate/resource_type.py`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20240502/iam_actions/generate/services.py` & `iam_actions-1.2.20240503/iam_actions/generate/services.py`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20240502/iam_actions/policies.json` & `iam_actions-1.2.20240503/iam_actions/policies.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9999974655312247%*

 * *Differences: {"'serviceMap'": "{'Amazon Neptune Analytics': {'conditionKeys': {insert: [(3, "*

 * *                 "'neptune-graph:PublicConnectivity')]}}}"}*

```diff
@@ -18114,15 +18114,16 @@
                 "WriteDataViaQuery"
             ],
             "HasResource": true,
             "StringPrefix": "neptune-graph",
             "conditionKeys": [
                 "aws:RequestTag/${TagKey}",
                 "aws:ResourceTag/${TagKey}",
-                "aws:TagKeys"
+                "aws:TagKeys",
+                "neptune-graph:PublicConnectivity"
             ]
         },
         "Amazon Nimble Studio": {
             "ARNFormat": "arn:aws:nimble:${Region}:${Account}:${ResourceType}/${ResourcePath}",
             "ARNRegex": "^arn:aws:nimble:.+:.+:.+",
             "Actions": [
                 "AcceptEulas",
```

### Comparing `iam_actions-1.2.20240502/iam_actions/resourcetypes.json` & `iam_actions-1.2.20240503/iam_actions/resourcetypes.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9998586372632174%*

 * *Differences: {"'sms-voice'": "{'ProtectConfiguration': OrderedDict([('arn_pattern', "*

 * *                "'arn:*:sms-voice:*:*:protect-configuration/*'), ('condition_keys', "*

 * *                "'aws:ResourceTag/${TagKey}')])}"}*

```diff
@@ -6263,14 +6263,18 @@
             "arn_pattern": "arn:*:sms-voice:*:*:phone-number/*",
             "condition_keys": "aws:ResourceTag/${TagKey}"
         },
         "Pool": {
             "arn_pattern": "arn:*:sms-voice:*:*:pool/*",
             "condition_keys": "aws:ResourceTag/${TagKey}"
         },
+        "ProtectConfiguration": {
+            "arn_pattern": "arn:*:sms-voice:*:*:protect-configuration/*",
+            "condition_keys": "aws:ResourceTag/${TagKey}"
+        },
         "Registration": {
             "arn_pattern": "arn:*:sms-voice:*:*:registration/*",
             "condition_keys": "aws:ResourceTag/${TagKey}"
         },
         "RegistrationAttachment": {
             "arn_pattern": "arn:*:sms-voice:*:*:registration-attachment/*",
             "condition_keys": "aws:ResourceTag/${TagKey}"
```

### Comparing `iam_actions-1.2.20240502/iam_actions/services.json` & `iam_actions-1.2.20240503/iam_actions/services.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9999734944868532%*

 * *Differences: {"'neptune-graph'": "{'ConditionKeys': {insert: [(3, 'neptune-graph:PublicConnectivity')]}}"}*

```diff
@@ -15835,15 +15835,16 @@
             "UntagResource",
             "UpdateGraph",
             "WriteDataViaQuery"
         ],
         "ConditionKeys": [
             "aws:RequestTag/${TagKey}",
             "aws:ResourceTag/${TagKey}",
-            "aws:TagKeys"
+            "aws:TagKeys",
+            "neptune-graph:PublicConnectivity"
         ],
         "HasResource": true,
         "ServiceNames": [
             "Amazon Neptune Analytics"
         ]
     },
     "network-firewall": {
```

### Comparing `iam_actions-1.2.20240502/pyproject.toml` & `iam_actions-1.2.20240503/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "iam-actions"
-version = "1.2.20240502"
+version = "1.2.20240503"
 description = "JSON of AWS policy components"
 authors = ["Constable <info@constableapp.com>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/constableapp/iam_actions"
 packages = [{include = "iam_actions"}]
```

### Comparing `iam_actions-1.2.20240502/setup.py` & `iam_actions-1.2.20240503/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 ['iam_actions', 'iam_actions.generate']
 
 package_data = \
 {'': ['*']}
 
 setup_kwargs = {
     'name': 'iam-actions',
-    'version': '1.2.20240502',
+    'version': '1.2.20240503',
     'description': 'JSON of AWS policy components',
     'long_description': '# iam_actions\n\n`iam_actions` is a python module which contains a dictionary of AWS IAM information. Ideally, it is a complete catalog of all AWS services, actions, and resource types. The information is scraped from the AWS documentation pages.\n\nNightly, the scraping service runs, and publishes a new version with the date appended. \n\nThe package is meant to be used as a consumable package, but it also contains the code to generate the definitions for packaging.\n\nThere are three "roots" that you can consume: actions, resource_types, and services. They all currently return as dict\'s. *However, in a future release, it will be returned as python data structures*\n\n## Actions\n\nActions is a listing of all the actions for a given service. The structure is as follows:\n```\n{\n    "service_name": {\n        "action_name: {\n            "access_level": access_level,\n            "action": action_name,\n            "condition_keys": [condition_key1, ...],\n            "description": description\n        }\n    }\n}\n```\n\nTherefore, you can find information about an action as follows\n\n```\n>>> iam_actions.actions[\'s3\'][\'GetObject\']\n{\'access_level\': \'Read\', \'action\': \'GetObject\', \'condition_keys\': [\'s3:AccessPointNetworkOrigin\', \'s3:DataAccessPointAccount\', \'s3:DataAccessPointArn\', \'s3:ExistingObjectTag/<key>\', \'s3:ResourceAccount\', \'s3:TlsVersion\', \'s3:authType\', \'s3:signatureAge\', \'s3:signatureversion\', \'s3:x-amz-content-sha256\'], \'description\': \'Grants permission to retrieve objects from Amazon S3\', \'orphan\': False, \'resources\': [\'object\']}\n```\n\n## Services\n\nServices list information about the service. The structure is as follows:\n\n```\n{\n    "service_name": {\n        "Actions": [action1, ...]\n        "ServiceNames": [service_name1, ...]\n        "ARNFormats": [arn_format1, ...]\n        "ConditionKeys": [condition_key1, ...]\n        "HasResource": bool\n    }\n}\n```\n\n## Resource Types\n\nResource Types list information about the resource types for the service. The structure is as follows:\n\n```\n{\n    "service_name": {\n        "resource_name": {\n            "arn_pattern": arn_pattern,\n            "condition_keys": [condition_key1, ...]\n        }\n    }\n}\n```\n\n## Usage\n\n```python\nimport iam_actions\n\nprint(item_actions.services)\nprint(item_actions.actions)\nprint(item_actions.resource_types)\n```\n',
     'author': 'Constable',
     'author_email': 'info@constableapp.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/constableapp/iam_actions',
```

### Comparing `iam_actions-1.2.20240502/PKG-INFO` & `iam_actions-1.2.20240503/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iam-actions
-Version: 1.2.20240502
+Version: 1.2.20240503
 Summary: JSON of AWS policy components
 Home-page: https://github.com/constableapp/iam_actions
 License: MIT
 Author: Constable
 Author-email: info@constableapp.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

