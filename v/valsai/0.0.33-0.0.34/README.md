# Comparing `tmp/valsai-0.0.33.tar.gz` & `tmp/valsai-0.0.34.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "valsai-0.0.33.tar", last modified: Sat May  4 01:47:16 2024, max compression
+gzip compressed data, was "valsai-0.0.34.tar", last modified: Sat May  4 17:49:08 2024, max compression
```

## Comparing `valsai-0.0.33.tar` & `valsai-0.0.34.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 langston   (501) staff       (20)        0 2024-05-04 01:47:16.454101 valsai-0.0.33/
--rw-r--r--   0 langston   (501) staff       (20)      370 2024-05-04 01:47:16.453611 valsai-0.0.33/PKG-INFO
--rw-r--r--   0 langston   (501) staff       (20)     2818 2024-05-04 01:41:04.000000 valsai-0.0.33/README.md
--rw-r--r--   0 langston   (501) staff       (20)       38 2024-05-04 01:47:16.454178 valsai-0.0.33/setup.cfg
--rw-r--r--   0 langston   (501) staff       (20)      619 2024-05-04 01:44:38.000000 valsai-0.0.33/setup.py
-drwxr-xr-x   0 langston   (501) staff       (20)        0 2024-05-04 01:47:16.443877 valsai-0.0.33/vals/
--rw-r--r--   0 langston   (501) staff       (20)        0 2024-05-04 01:41:09.000000 valsai-0.0.33/vals/__init__.py
-drwxr-xr-x   0 langston   (501) staff       (20)        0 2024-05-04 01:47:16.447193 valsai-0.0.33/vals/cli/
--rw-r--r--   0 langston   (501) staff       (20)        0 2024-05-04 01:41:09.000000 valsai-0.0.33/vals/cli/__init__.py
--rw-r--r--   0 langston   (501) staff       (20)     1423 2024-05-04 01:41:09.000000 valsai-0.0.33/vals/cli/auth.py
--rw-r--r--   0 langston   (501) staff       (20)      284 2024-05-04 01:41:09.000000 valsai-0.0.33/vals/cli/main.py
--rw-r--r--   0 langston   (501) staff       (20)     5045 2024-05-04 01:41:09.000000 valsai-0.0.33/vals/cli/rag.py
--rw-r--r--   0 langston   (501) staff       (20)     4348 2024-05-04 01:41:09.000000 valsai-0.0.33/vals/cli/run.py
--rw-r--r--   0 langston   (501) staff       (20)     4764 2024-05-04 01:41:09.000000 valsai-0.0.33/vals/cli/suite.py
--rw-r--r--   0 langston   (501) staff       (20)     1059 2024-05-04 01:41:09.000000 valsai-0.0.33/vals/cli/util.py
-drwxr-xr-x   0 langston   (501) staff       (20)        0 2024-05-04 01:47:16.450275 valsai-0.0.33/vals/sdk/
--rw-r--r--   0 langston   (501) staff       (20)        0 2024-05-04 01:41:09.000000 valsai-0.0.33/vals/sdk/__init__.py
--rw-r--r--   0 langston   (501) staff       (20)     3436 2024-05-04 01:41:09.000000 valsai-0.0.33/vals/sdk/auth.py
--rw-r--r--   0 langston   (501) staff       (20)      134 2024-05-04 01:41:09.000000 valsai-0.0.33/vals/sdk/exceptions.py
-drwxr-xr-x   0 langston   (501) staff       (20)        0 2024-05-04 01:47:16.451101 valsai-0.0.33/vals/sdk/jsonschemas/
--rw-r--r--   0 langston   (501) staff       (20)      550 2024-05-04 01:41:09.000000 valsai-0.0.33/vals/sdk/jsonschemas/run_params_schema.json
--rw-r--r--   0 langston   (501) staff       (20)     2482 2024-05-04 01:41:09.000000 valsai-0.0.33/vals/sdk/jsonschemas/suiteschema.json
--rw-r--r--   0 langston   (501) staff       (20)     6523 2024-05-04 01:41:09.000000 valsai-0.0.33/vals/sdk/run.py
--rw-r--r--   0 langston   (501) staff       (20)     2419 2024-05-04 01:41:09.000000 valsai-0.0.33/vals/sdk/sdk.py
--rw-r--r--   0 langston   (501) staff       (20)    11359 2024-05-04 01:41:09.000000 valsai-0.0.33/vals/sdk/suite.py
--rw-r--r--   0 langston   (501) staff       (20)     1727 2024-05-04 01:41:09.000000 valsai-0.0.33/vals/sdk/util.py
-drwxr-xr-x   0 langston   (501) staff       (20)        0 2024-05-04 01:47:16.452991 valsai-0.0.33/valsai.egg-info/
--rw-r--r--   0 langston   (501) staff       (20)      370 2024-05-04 01:47:16.000000 valsai-0.0.33/valsai.egg-info/PKG-INFO
--rw-r--r--   0 langston   (501) staff       (20)      549 2024-05-04 01:47:16.000000 valsai-0.0.33/valsai.egg-info/SOURCES.txt
--rw-r--r--   0 langston   (501) staff       (20)        1 2024-05-04 01:47:16.000000 valsai-0.0.33/valsai.egg-info/dependency_links.txt
--rw-r--r--   0 langston   (501) staff       (20)       43 2024-05-04 01:47:16.000000 valsai-0.0.33/valsai.egg-info/entry_points.txt
--rw-r--r--   0 langston   (501) staff       (20)       80 2024-05-04 01:47:16.000000 valsai-0.0.33/valsai.egg-info/requires.txt
--rw-r--r--   0 langston   (501) staff       (20)        5 2024-05-04 01:47:16.000000 valsai-0.0.33/valsai.egg-info/top_level.txt
+drwxr-xr-x   0 langston   (501) staff       (20)        0 2024-05-04 17:49:08.142785 valsai-0.0.34/
+-rw-r--r--   0 langston   (501) staff       (20)      366 2024-05-04 17:49:08.142349 valsai-0.0.34/PKG-INFO
+-rw-r--r--   0 langston   (501) staff       (20)     2829 2024-05-04 01:58:49.000000 valsai-0.0.34/README.md
+-rw-r--r--   0 langston   (501) staff       (20)       38 2024-05-04 17:49:08.142852 valsai-0.0.34/setup.cfg
+-rw-r--r--   0 langston   (501) staff       (20)      615 2024-05-04 17:48:41.000000 valsai-0.0.34/setup.py
+drwxr-xr-x   0 langston   (501) staff       (20)        0 2024-05-04 17:49:08.133226 valsai-0.0.34/vals/
+-rw-r--r--   0 langston   (501) staff       (20)        0 2024-05-04 01:41:09.000000 valsai-0.0.34/vals/__init__.py
+drwxr-xr-x   0 langston   (501) staff       (20)        0 2024-05-04 17:49:08.136130 valsai-0.0.34/vals/cli/
+-rw-r--r--   0 langston   (501) staff       (20)        0 2024-05-04 01:41:09.000000 valsai-0.0.34/vals/cli/__init__.py
+-rw-r--r--   0 langston   (501) staff       (20)     1424 2024-05-04 16:17:58.000000 valsai-0.0.34/vals/cli/auth.py
+-rw-r--r--   0 langston   (501) staff       (20)      284 2024-05-04 01:41:09.000000 valsai-0.0.34/vals/cli/main.py
+-rw-r--r--   0 langston   (501) staff       (20)     5048 2024-05-04 16:17:58.000000 valsai-0.0.34/vals/cli/rag.py
+-rw-r--r--   0 langston   (501) staff       (20)     4350 2024-05-04 16:17:59.000000 valsai-0.0.34/vals/cli/run.py
+-rw-r--r--   0 langston   (501) staff       (20)     4768 2024-05-04 16:17:59.000000 valsai-0.0.34/vals/cli/suite.py
+-rw-r--r--   0 langston   (501) staff       (20)     1061 2024-05-04 16:17:58.000000 valsai-0.0.34/vals/cli/util.py
+drwxr-xr-x   0 langston   (501) staff       (20)        0 2024-05-04 17:49:08.138788 valsai-0.0.34/vals/sdk/
+-rw-r--r--   0 langston   (501) staff       (20)        0 2024-05-04 01:41:09.000000 valsai-0.0.34/vals/sdk/__init__.py
+-rw-r--r--   0 langston   (501) staff       (20)     3415 2024-05-04 16:20:15.000000 valsai-0.0.34/vals/sdk/auth.py
+-rw-r--r--   0 langston   (501) staff       (20)      134 2024-05-04 01:41:09.000000 valsai-0.0.34/vals/sdk/exceptions.py
+drwxr-xr-x   0 langston   (501) staff       (20)        0 2024-05-04 17:49:08.139730 valsai-0.0.34/vals/sdk/jsonschemas/
+-rw-r--r--   0 langston   (501) staff       (20)      550 2024-05-04 01:41:09.000000 valsai-0.0.34/vals/sdk/jsonschemas/run_params_schema.json
+-rw-r--r--   0 langston   (501) staff       (20)     2482 2024-05-04 01:41:09.000000 valsai-0.0.34/vals/sdk/jsonschemas/suiteschema.json
+-rw-r--r--   0 langston   (501) staff       (20)     6526 2024-05-04 16:17:58.000000 valsai-0.0.34/vals/sdk/run.py
+-rw-r--r--   0 langston   (501) staff       (20)     2421 2024-05-04 16:17:58.000000 valsai-0.0.34/vals/sdk/sdk.py
+-rw-r--r--   0 langston   (501) staff       (20)    11362 2024-05-04 16:17:58.000000 valsai-0.0.34/vals/sdk/suite.py
+-rw-r--r--   0 langston   (501) staff       (20)     1685 2024-05-04 16:20:15.000000 valsai-0.0.34/vals/sdk/util.py
+drwxr-xr-x   0 langston   (501) staff       (20)        0 2024-05-04 17:49:08.141862 valsai-0.0.34/valsai.egg-info/
+-rw-r--r--   0 langston   (501) staff       (20)      366 2024-05-04 17:49:08.000000 valsai-0.0.34/valsai.egg-info/PKG-INFO
+-rw-r--r--   0 langston   (501) staff       (20)      549 2024-05-04 17:49:08.000000 valsai-0.0.34/valsai.egg-info/SOURCES.txt
+-rw-r--r--   0 langston   (501) staff       (20)        1 2024-05-04 17:49:08.000000 valsai-0.0.34/valsai.egg-info/dependency_links.txt
+-rw-r--r--   0 langston   (501) staff       (20)       43 2024-05-04 17:49:08.000000 valsai-0.0.34/valsai.egg-info/entry_points.txt
+-rw-r--r--   0 langston   (501) staff       (20)       80 2024-05-04 17:49:08.000000 valsai-0.0.34/valsai.egg-info/requires.txt
+-rw-r--r--   0 langston   (501) staff       (20)        5 2024-05-04 17:49:08.000000 valsai-0.0.34/valsai.egg-info/top_level.txt
```

### Comparing `valsai-0.0.33/README.md` & `valsai-0.0.34/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # PlaygroundRL CLI Tool
 
 ## Install
 
 ```
-pip install prl-cli
+pip install vals-cli
 ```
 
 ### _Internal: Install during development_
 
 ```
 cd legal-evaluator/cli
 pip install -e .
@@ -16,78 +16,78 @@
 ## Authentication
 
 Make an account at [https://platform.vals.ai](https://platform.vals.ai) and confirm your email.
 
 Log in locally with:
 
 ```commandline
-prl login
+vals login
 ```
 
 This will create an auth token for you locally which is used in future commands. You will be prompted to re-login after the token expires (30 days).
 
 ## Overall Usage
 
 The CLI is run as follows:
 
 ```
-$ prl
+$ vals
 ```
 
 Use the `--help` flag at the top and subcommand level for guidance.
 
 Commands must be run from the pip environment the cli was installed in. Commands are split up into subcommand. Currently there are two subcommands:
 
-- `prl suite`: relating to creating / updating tests and suites
-- `prl run`: relating to creating and querying runs and run results.
+- `vals suite`: relating to creating / updating tests and suites
+- `vals run`: relating to creating and querying runs and run results.
 
 ## Create Test Suite
 
 Create a test suite from command line
 
 ```
-prl suite create --interactive
+vals suite create --interactive
 ```
 
 Create a test suite from JSON file
 
 ```
-prl suite create ./example_suite.json
+vals suite create ./example_suite.json
 ```
 
-The `prl suite create` commands will produce a link to the created test suite.
+The `vals suite create` commands will produce a link to the created test suite.
 
 ## Run
 
 The test suite id embedded at the end of the URL is used in run requests.
 
 Start a new run:
 
 ```
-prl run start [suite_id]
+vals run start [suite_id]
 ```
 
 ## Frozen LLM Outputs Workflow
 
 In some cases, it is useful to be able to shortcut the model API call to use a hard-coded output for evaluation. This can be used to evaluate the evaluator.
 
 To provide outputs, modify the JSON test suite file to include the string attribute `fixed_output`. See the example file `example_with_fixed_output.json`.
 
 Then, create the test suite as usual.
 
 ```
-prl suite create ./example_with_fixed_output.json
+vals suite create ./example_with_fixed_output.json
 ```
 
 By default, running this test suite (via the website or CLI command) will still use the API to generate outputs. The `--use_fixed_output` flag must be provided.
 
 Example:
 
 ```
-prl suite run [suite_id] --use_fixed_output
+vals suite run [suite_id] --use_fixed_output
 ```
 
 ## Example JSON files:
 
 `example_suite.json`
 
 ```json
```

### Comparing `valsai-0.0.33/setup.py` & `valsai-0.0.34/setup.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import find_packages, setup
 
 setup(
     name="valsai",
-    version="0.0.33",
+    version="0.0.34",
     author="Langston Nashold, Rayan Krishnan",
     packages=find_packages(),
     include_package_data=True,
     package_data={"": ["jsonschemas/*"]},
     install_requires=[
         "Click",
         "gql",
@@ -20,9 +20,9 @@
         "requests-toolbelt",
     ],
     entry_points={
         "console_scripts": [
             "vals = vals.cli.main:cli",
         ],
     },
-    url="http://pypi.python.org/pypi/prl-cli/",
+    url="https://pypi.org/project/valsai/",
 )
```

### Comparing `valsai-0.0.33/vals/cli/auth.py` & `valsai-0.0.34/vals/cli/auth.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import json
 import os
 import time
 
 import boto3
 import click
-from prl.sdk.auth import CREDS_PATH, PRL_PATH, get_client_id
+from vals.sdk.auth import CREDS_PATH, PRL_PATH, get_client_id
 
 
 @click.command(name="login")
 def login_command():
     """
     Authenticate with PlaygroundRL CLI
     """
```

### Comparing `valsai-0.0.33/vals/cli/rag.py` & `valsai-0.0.34/vals/cli/rag.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 import json
 from typing import Any, Dict
 
 import click
 import requests
 from gql import gql
-from prl.cli.util import display_error_and_exit, prompt_user_for_rag_suite
-from prl.sdk.auth import get_auth_token
-from prl.sdk.util import be_host, get_client, list_rag_suites
+from vals.cli.util import display_error_and_exit, prompt_user_for_rag_suite
+from vals.sdk.auth import get_auth_token
+from vals.sdk.util import be_host, get_client, list_rag_suites
 
 
 @click.group(name="rag")
 def rag_group():
     """
     Commands relating to starting rag evaluations.
     """
```

### Comparing `valsai-0.0.33/vals/cli/run.py` & `valsai-0.0.34/vals/cli/run.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 import json
 from datetime import datetime
 from io import BytesIO
 
 import click
-from prl.sdk.run import (
+from vals.sdk.run import (
     get_csv,
     get_run_results,
     get_run_url,
     run_status,
     run_summary,
     start_run,
 )
-from prl.sdk.util import fe_host
+from vals.sdk.util import fe_host
 
 from ..sdk.exceptions import PrlException
 from .util import display_error_and_exit, prompt_user_for_suite
 
 
 @click.group(name="run")
 def run_group():
```

### Comparing `valsai-0.0.33/vals/cli/suite.py` & `valsai-0.0.34/vals/cli/suite.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 import json
 import sys
 from io import TextIOWrapper
 from typing import Any, Dict
 
 import click
-from prl.cli.util import display_error_and_exit, prompt_user_for_suite
-from prl.sdk.exceptions import PrlException
-from prl.sdk.suite import create_suite, list_test_suites, pull_suite, update_suite
-from prl.sdk.util import fe_host
+from vals.cli.util import display_error_and_exit, prompt_user_for_suite
+from vals.sdk.exceptions import PrlException
+from vals.sdk.suite import create_suite, list_test_suites, pull_suite, update_suite
+from vals.sdk.util import fe_host
 
 
 @click.group(name="suite")
 def suite_group():
     """
     Start, create, or view tests and test suites
     """
```

### Comparing `valsai-0.0.33/vals/cli/util.py` & `valsai-0.0.34/vals/cli/util.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import sys
 
 import click
-from prl.sdk.suite import list_test_suites
-from prl.sdk.util import list_rag_suites
+from vals.sdk.suite import list_test_suites
+from vals.sdk.util import list_rag_suites
 
 
 def prompt_user_for_rag_suite():
     suites = list_rag_suites()
     click.echo("Rag Suites:")
     click.echo(
         "\n".join([f"{i}: {s['id']} {s['query']}" for i, s in enumerate(suites)])
```

### Comparing `valsai-0.0.33/vals/sdk/auth.py` & `valsai-0.0.34/vals/sdk/auth.py`

 * *Files 10% similar despite different names*

```diff
@@ -4,32 +4,32 @@
 import time
 
 import boto3
 import click
 
 PRL_PATH = os.path.expanduser("~/.prl")
 CREDS_PATH = os.path.join(PRL_PATH, "creds.json")
-PLAYGROUND_ENV = os.getenv("PLAYGROUND_ENV")
+VALS_ENV = os.getenv("VALS_ENV")
 
 DEFAULT_REGION = "us-east-1"
 
 
 def get_client_id(in_europe: bool, using_api_key: bool):
     if using_api_key:
         if in_europe:
             return "6cv1hchrihac7dtsmjac1dukn6"
-        elif PLAYGROUND_ENV in ["LOCAL", "DEV"]:
+        elif VALS_ENV in ["LOCAL", "DEV"]:
             return "7scu563gabte768gtml5v5uids"
         else:
             # Normal Prod user pool
             return "6t1s1a2g43ggqkn8timajdl0nn"
     else:
         if in_europe:
             return "4asi3qr1jga1l1kvc6cqpqdsad"
-        elif PLAYGROUND_ENV in ["LOCAL", "DEV"]:
+        elif VALS_ENV in ["LOCAL", "DEV"]:
             return "59blf1klr2lejsd3uanpk3b0r4"
         else:
             # Normal Prod user pool
             return "7r5tn1kic6i262mv86g6etn3oj"
 
 
 def get_region():
@@ -60,16 +60,16 @@
     else:
         region_name = DEFAULT_REGION
 
     client = boto3.client("cognito-idp", region_name=region_name)
 
     if "access_expiry" not in auth_dict or time.time() > auth_dict["access_expiry"]:
         # API Key is specified in environment
-        if "PRL_API_KEY" in os.environ:
-            refresh_token = os.environ["PRL_API_KEY"]
+        if "VALS_API_KEY" in os.environ:
+            refresh_token = os.environ["VALS_API_KEY"]
             client_id = get_client_id(region_name == "eu-north-1", True)
         # We're using the prl login workflow.
         elif "refresh_token" in auth_dict:
             refresh_token = auth_dict["refresh_token"]
             client_id = auth_dict["client_id"]
         # No refresh token, so not logged in
         else:
@@ -80,15 +80,15 @@
             response = client.initiate_auth(
                 AuthFlow="REFRESH_TOKEN_AUTH",
                 AuthParameters={"REFRESH_TOKEN": refresh_token},
                 ClientId=client_id,
             )
         except Exception as e:
             click.echo(
-                "Either your session has expired or an invalid API Key was provided. Run prl login, or update your PRL_API_KEY environment variable."
+                "Either your session has expired or an invalid API Key was provided. Run prl login, or update your VALS_API_KEY environment variable."
             )
             sys.exit()
 
         auth_dict = {
             **auth_dict,
             "access_token": response["AuthenticationResult"]["AccessToken"],
             "id_token": response["AuthenticationResult"]["IdToken"],
```

### Comparing `valsai-0.0.33/vals/sdk/jsonschemas/run_params_schema.json` & `valsai-0.0.34/vals/sdk/jsonschemas/run_params_schema.json`

 * *Files identical despite different names*

### Comparing `valsai-0.0.33/vals/sdk/jsonschemas/suiteschema.json` & `valsai-0.0.34/vals/sdk/jsonschemas/suiteschema.json`

 * *Files identical despite different names*

### Comparing `valsai-0.0.33/vals/sdk/run.py` & `valsai-0.0.34/vals/sdk/run.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 import json
 import time
 from typing import Any, Dict, List
 
 import requests
 from gql import gql
 from jsonschema import ValidationError, validate
-from prl.sdk.auth import get_auth_token
-from prl.sdk.exceptions import PrlException
-from prl.sdk.util import RUN_SCHEMA_PATH, be_host, fe_host, get_client
+from vals.sdk.auth import get_auth_token
+from vals.sdk.exceptions import PrlException
+from vals.sdk.util import RUN_SCHEMA_PATH, be_host, fe_host, get_client
 
 # Rudimentary cache for pulling params
 _default_params = None
 
 
 def _get_default_parameters() -> Dict[str, Any]:
     global _default_params
```

### Comparing `valsai-0.0.33/vals/sdk/sdk.py` & `valsai-0.0.34/vals/sdk/sdk.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 from functools import wraps
 from time import time
 from typing import Callable
 
 import attrs
 import click
 from openai import OpenAI
-from prl.cli.suite import pull_suite, update_suite
-from prl.sdk.run import get_run_url, start_run
 from tqdm import tqdm
+from vals.cli.suite import pull_suite, update_suite
+from vals.sdk.run import get_run_url, start_run
 
 in_tokens = 0
 out_tokens = 0
 
 
 def parse_test_suite_id_from_url(test_suite_url: str) -> str:
     start_index = test_suite_url.find("test_suite_id=") + len("test_suite_id=")
```

### Comparing `valsai-0.0.33/vals/sdk/suite.py` & `valsai-0.0.34/vals/sdk/suite.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 import json
 import os
 from typing import Any, Dict, List
 
 import requests
 from gql import gql
 from jsonschema import ValidationError, validate
-from prl.sdk.auth import get_auth_token
-from prl.sdk.exceptions import PrlException
-from prl.sdk.util import SUITE_SCHEMA_PATH, be_host, get_client
+from vals.sdk.auth import get_auth_token
+from vals.sdk.exceptions import PrlException
+from vals.sdk.util import SUITE_SCHEMA_PATH, be_host, get_client
 
 OPERATORS = [
     "includes",
     "logical_includes",
     "excludes",
     "equals",
     "mostly_equals",
```

### Comparing `valsai-0.0.33/vals/sdk/util.py` & `valsai-0.0.34/vals/sdk/util.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,54 +1,54 @@
 import os
 
 from gql import Client, gql
 from gql.transport.requests import RequestsHTTPTransport
 
 from .auth import get_auth_token, get_region
 
-PLAYGROUND_ENV = os.getenv("PLAYGROUND_ENV")
+VALS_ENV = os.getenv("VALS_ENV")
 SCHEMA_PATH = os.path.join(os.path.dirname(__file__), "jsonschemas")
 SUITE_SCHEMA_PATH = os.path.join(SCHEMA_PATH, "suiteschema.json")
 RUN_SCHEMA_PATH = os.path.join(SCHEMA_PATH, "run_params_schema.json")
 
 client_ = None
 
 
 def be_host():
     region = get_region()
     if region == "eu-north-1":
         return "https://europebe.playgroundrl.com"
-    if PLAYGROUND_ENV == "LOCAL":
+    if VALS_ENV == "LOCAL":
         return "http://localhost:8000"
-    if PLAYGROUND_ENV == "DEV":
+    if VALS_ENV == "DEV":
         return "https://devbe.playgroundrl.com"
 
     return "https://prodbe.playgroundrl.com"
 
 
 def fe_host():
     region = get_region()
     if region == "eu-north-1":
         return "https://eu.playgroundrl.com"
-    if PLAYGROUND_ENV == "LOCAL":
+    if VALS_ENV == "LOCAL":
         return "http://localhost:3000"
-    if PLAYGROUND_ENV == "DEV":
+    if VALS_ENV == "DEV":
         return "https://dev.platform.vals.ai"
 
     return "https://platform.vals.ai"
 
 
 def get_client():
     global client_
     if client_ is None:
 
         transport = RequestsHTTPTransport(
             url=f"{be_host()}/graphql/",
             headers={"Authorization": get_auth_token()},
-            verify=PLAYGROUND_ENV != "LOCAL",
+            verify=VALS_ENV != "LOCAL",
         )
         client_ = Client(transport=transport, fetch_schema_from_transport=True)
     return client_
 
 
 def list_rag_suites():
     query = gql(
```

### Comparing `valsai-0.0.33/valsai.egg-info/SOURCES.txt` & `valsai-0.0.34/valsai.egg-info/SOURCES.txt`

 * *Files identical despite different names*

