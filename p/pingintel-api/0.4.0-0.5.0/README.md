# Comparing `tmp/pingintel_api-0.4.0.tar.gz` & `tmp/pingintel_api-0.5.0.tar.gz`

## Comparing `pingintel_api-0.4.0.tar` & `pingintel_api-0.5.0.tar`

### file list

```diff
@@ -1,23 +1,21 @@
--rw-r--r--   0        0        0      486 2020-02-02 00:00:00.000000 pingintel_api-0.4.0/.pre-commit-config.yaml
--rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 pingintel_api-0.4.0/justfile
--rw-r--r--   0        0        0       15 2020-02-02 00:00:00.000000 pingintel_api-0.4.0/requirements.txt
--rw-r--r--   0        0        0      162 2020-02-02 00:00:00.000000 pingintel_api-0.4.0/examples/fix_sov.py
--rw-r--r--   0        0        0      379 2020-02-02 00:00:00.000000 pingintel_api-0.4.0/examples/pingvision_activity.py
--rw-r--r--   0        0        0     9170 2020-02-02 00:00:00.000000 pingintel_api-0.4.0/examples/test_sov.xlsx
--rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 pingintel_api-0.4.0/src/pingintel_api/__about__.py
--rw-r--r--   0        0        0      130 2020-02-02 00:00:00.000000 pingintel_api-0.4.0/src/pingintel_api/__init__.py
--rw-r--r--   0        0        0     4274 2020-02-02 00:00:00.000000 pingintel_api-0.4.0/src/pingintel_api/api_client_base.py
--rw-r--r--   0        0        0      149 2020-02-02 00:00:00.000000 pingintel_api-0.4.0/src/pingintel_api/constants.py
--rw-r--r--   0        0        0     3450 2020-02-02 00:00:00.000000 pingintel_api-0.4.0/src/pingintel_api/sovfixerapi_cmd.py
--rw-r--r--   0        0        0      728 2020-02-02 00:00:00.000000 pingintel_api-0.4.0/src/pingintel_api/utils.py
--rw-r--r--   0        0        0     1694 2020-02-02 00:00:00.000000 pingintel_api-0.4.0/src/pingintel_api/pingvision/pingvision_api_client.py
--rw-r--r--   0        0        0      219 2020-02-02 00:00:00.000000 pingintel_api-0.4.0/src/pingintel_api/pingvision/types.py
--rw-r--r--   0        0        0     8414 2020-02-02 00:00:00.000000 pingintel_api-0.4.0/src/pingintel_api/sov_fixer/sov_fixer_api_client.py
--rw-r--r--   0        0        0     2950 2020-02-02 00:00:00.000000 pingintel_api-0.4.0/src/pingintel_api/sov_fixer/types.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pingintel_api-0.4.0/tests/__init__.py
--rw-r--r--   0        0        0       73 2020-02-02 00:00:00.000000 pingintel_api-0.4.0/tests/tests.py
--rw-r--r--   0        0        0     3251 2020-02-02 00:00:00.000000 pingintel_api-0.4.0/.gitignore
--rw-r--r--   0        0        0     1100 2020-02-02 00:00:00.000000 pingintel_api-0.4.0/LICENSE
--rw-r--r--   0        0        0      395 2020-02-02 00:00:00.000000 pingintel_api-0.4.0/README.md
--rw-r--r--   0        0        0      757 2020-02-02 00:00:00.000000 pingintel_api-0.4.0/pyproject.toml
--rw-r--r--   0        0        0      917 2020-02-02 00:00:00.000000 pingintel_api-0.4.0/PKG-INFO
+-rw-r--r--   0        0        0      465 2020-02-02 00:00:00.000000 pingintel_api-0.5.0/.pre-commit-config.yaml
+-rw-r--r--   0        0        0       14 2020-02-02 00:00:00.000000 pingintel_api-0.5.0/requirements.txt
+-rw-r--r--   0        0        0      154 2020-02-02 00:00:00.000000 pingintel_api-0.5.0/examples/fix_sov.py
+-rw-r--r--   0        0        0      366 2020-02-02 00:00:00.000000 pingintel_api-0.5.0/examples/pingvision_activity.py
+-rw-r--r--   0        0        0     9170 2020-02-02 00:00:00.000000 pingintel_api-0.5.0/examples/test_sov.xlsx
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 pingintel_api-0.5.0/src/pingintel_api/__about__.py
+-rw-r--r--   0        0        0      208 2020-02-02 00:00:00.000000 pingintel_api-0.5.0/src/pingintel_api/__init__.py
+-rw-r--r--   0        0        0     4159 2020-02-02 00:00:00.000000 pingintel_api-0.5.0/src/pingintel_api/api_client_base.py
+-rw-r--r--   0        0        0      145 2020-02-02 00:00:00.000000 pingintel_api-0.5.0/src/pingintel_api/constants.py
+-rw-r--r--   0        0        0     3295 2020-02-02 00:00:00.000000 pingintel_api-0.5.0/src/pingintel_api/sovfixerapi_cmd.py
+-rw-r--r--   0        0        0      696 2020-02-02 00:00:00.000000 pingintel_api-0.5.0/src/pingintel_api/utils.py
+-rw-r--r--   0        0        0     1633 2020-02-02 00:00:00.000000 pingintel_api-0.5.0/src/pingintel_api/pingvision/pingvision_api_client.py
+-rw-r--r--   0        0        0      210 2020-02-02 00:00:00.000000 pingintel_api-0.5.0/src/pingintel_api/pingvision/types.py
+-rw-r--r--   0        0        0     8170 2020-02-02 00:00:00.000000 pingintel_api-0.5.0/src/pingintel_api/sov_fixer/sov_fixer_api_client.py
+-rw-r--r--   0        0        0     2830 2020-02-02 00:00:00.000000 pingintel_api-0.5.0/src/pingintel_api/sov_fixer/types.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pingintel_api-0.5.0/tests/__init__.py
+-rw-r--r--   0        0        0     3090 2020-02-02 00:00:00.000000 pingintel_api-0.5.0/.gitignore
+-rw-r--r--   0        0        0     1079 2020-02-02 00:00:00.000000 pingintel_api-0.5.0/LICENSE
+-rw-r--r--   0        0        0      379 2020-02-02 00:00:00.000000 pingintel_api-0.5.0/README.md
+-rw-r--r--   0        0        0      730 2020-02-02 00:00:00.000000 pingintel_api-0.5.0/pyproject.toml
+-rw-r--r--   0        0        0      917 2020-02-02 00:00:00.000000 pingintel_api-0.5.0/PKG-INFO
```

### Comparing `pingintel_api-0.4.0/examples/test_sov.xlsx` & `pingintel_api-0.5.0/examples/test_sov.xlsx`

 * *Files identical despite different names*

### Comparing `pingintel_api-0.4.0/src/pingintel_api/api_client_base.py` & `pingintel_api-0.5.0/src/pingintel_api/api_client_base.py`

 * *Ordering differences only*

 * *Files 19% similar despite different names*

```diff
@@ -1,115 +1,115 @@
-import configparser
-import os
-from typing import IO, NotRequired, TypedDict, overload
-
-import requests
-
-from .utils import log
-
-from pingintel_api.__about__ import __version__
-
-
-class APIClientBase:
-    api_subdomain: str
-    api_base_domain: str
-    auth_token_env_name: str
-    product: str
-
-    @overload
-    def __init__(self, api_url: str, auth_token=None) -> None:
-        """Initialize the API client with an API URL and an optional auth token.
-
-        :param api_url: The URL of the API.  e.g. "https://vision.pingintel.com"
-        """
-        pass
-
-    @overload
-    def __init__(self, environment: str = "prod", auth_token=None) -> None: ...
-
-    def __init__(
-        self,
-        api_url: str | None = None,
-        environment: str | None = "prod",
-        auth_token=None,
-    ):
-        if api_url is None:
-            if environment is None:
-                raise ValueError("Need either api_url or environment.")
-            api_url = self.get_api_url_by_environment(environment)
-
-        if not auth_token and environment:
-            auth_token = self.get_auth_token_by_environment(environment)
-        if not auth_token:
-            auth_token = os.environ.get(self.auth_token_env_name)
-        if not auth_token:
-            config = configparser.ConfigParser()
-            config.read(os.path.expanduser("~/.pingintel.ini"))
-            if environment:
-                serverspace = self.get_serverspace_from_environment(environment)
-                try:
-                    auth_token = config.get(
-                        self.product, f"{self.auth_token_env_name}_{serverspace}"
-                    )
-                except (configparser.NoOptionError, configparser.NoSectionError):
-                    pass
-            if not auth_token:
-                try:
-                    auth_token = config.get(self.product, self.auth_token_env_name)
-                except (configparser.NoOptionError, configparser.NoSectionError):
-                    pass
-
-        if not auth_token:
-            raise ValueError(
-                f"Need --auth-token or {self.auth_token_env_name} environment variable set."
-            )
-        assert api_url
-        self.api_url = api_url
-        self.auth_token = auth_token
-        self.environment = environment if api_url is None else None
-        self.session = self._create_session()
-
-    def get(self, url, **kwargs):
-        log(f"GET {url}")
-        return self.session.get(url, **kwargs)
-
-    def _create_session(self):
-        session = requests.Session()
-
-        session.headers = {
-            "Authorization": f"Token {self.auth_token}",
-            "Accept-Encoding": "gzip",
-            "User-Agent": f"pingintel_api/{self.__class__.__name__}/{__version__}",
-        }
-        return session
-
-    def get_api_url_by_environment(self, environment: str) -> str:
-        if environment == "prod":
-            return f"https://{self.api_subdomain}.{self.api_base_domain}"
-        elif environment == "prod2":
-            return f"https://{self.api_subdomain}2.{self.api_base_domain}"
-        elif environment == "prodeu":
-            return f"https://{self.api_subdomain}.eu.{self.api_base_domain}"
-        elif environment == "local":
-            return "http://api-local.sovfixer.com"
-        else:
-            return f"https://{self.api_subdomain}-{environment}.{self.api_base_domain}"
-
-    def get_auth_token_by_environment(self, environment: str) -> str:
-        serverspace = self.get_serverspace_from_environment(environment)
-        auth_token = os.environ.get(f"PING_{serverspace}_AUTH_TOKEN".upper())
-
-    def get_serverspace_from_environment(self, environment: str) -> str:
-        if environment in ["staging", "staging2"]:
-            serverspace = "stg"
-        elif environment in ["prod", "prod2"]:
-            serverspace = "prd"
-        elif environment in ["prodeu", "prodeu2"]:
-            serverspace = "prdeu"
-        elif environment in ["dev", "dev2"]:
-            serverspace = "dev"
-        elif environment in ["local", "local2"]:
-            serverspace = "local"
-        else:
-            raise ValueError("Unknown environment.")
-
-        return serverspace
+import configparser
+import os
+from typing import IO, NotRequired, TypedDict, overload
+
+import requests
+
+from .utils import log
+
+from pingintel_api.__about__ import __version__
+
+
+class APIClientBase:
+    api_subdomain: str
+    api_base_domain: str
+    auth_token_env_name: str
+    product: str
+
+    @overload
+    def __init__(self, api_url: str, auth_token=None) -> None:
+        """Initialize the API client with an API URL and an optional auth token.
+
+        :param api_url: The URL of the API.  e.g. "https://vision.pingintel.com"
+        """
+        pass
+
+    @overload
+    def __init__(self, environment: str = "prod", auth_token=None) -> None: ...
+
+    def __init__(
+        self,
+        api_url: str | None = None,
+        environment: str | None = "prod",
+        auth_token=None,
+    ):
+        if api_url is None:
+            if environment is None:
+                raise ValueError("Need either api_url or environment.")
+            api_url = self.get_api_url_by_environment(environment)
+
+        if not auth_token and environment:
+            auth_token = self.get_auth_token_by_environment(environment)
+        if not auth_token:
+            auth_token = os.environ.get(self.auth_token_env_name)
+        if not auth_token:
+            config = configparser.ConfigParser()
+            config.read(os.path.expanduser("~/.pingintel.ini"))
+            if environment:
+                serverspace = self.get_serverspace_from_environment(environment)
+                try:
+                    auth_token = config.get(
+                        self.product, f"{self.auth_token_env_name}_{serverspace}"
+                    )
+                except (configparser.NoOptionError, configparser.NoSectionError):
+                    pass
+            if not auth_token:
+                try:
+                    auth_token = config.get(self.product, self.auth_token_env_name)
+                except (configparser.NoOptionError, configparser.NoSectionError):
+                    pass
+
+        if not auth_token:
+            raise ValueError(
+                f"Need --auth-token or {self.auth_token_env_name} environment variable set."
+            )
+        assert api_url
+        self.api_url = api_url
+        self.auth_token = auth_token
+        self.environment = environment if api_url is None else None
+        self.session = self._create_session()
+
+    def get(self, url, **kwargs):
+        log(f"GET {url}")
+        return self.session.get(url, **kwargs)
+
+    def _create_session(self):
+        session = requests.Session()
+
+        session.headers = {
+            "Authorization": f"Token {self.auth_token}",
+            "Accept-Encoding": "gzip",
+            "User-Agent": f"pingintel_api/{self.__class__.__name__}/{__version__}",
+        }
+        return session
+
+    def get_api_url_by_environment(self, environment: str) -> str:
+        if environment == "prod":
+            return f"https://{self.api_subdomain}.{self.api_base_domain}"
+        elif environment == "prod2":
+            return f"https://{self.api_subdomain}2.{self.api_base_domain}"
+        elif environment == "prodeu":
+            return f"https://{self.api_subdomain}.eu.{self.api_base_domain}"
+        elif environment == "local":
+            return "http://api-local.sovfixer.com"
+        else:
+            return f"https://{self.api_subdomain}-{environment}.{self.api_base_domain}"
+
+    def get_auth_token_by_environment(self, environment: str) -> str:
+        serverspace = self.get_serverspace_from_environment(environment)
+        auth_token = os.environ.get(f"PING_{serverspace}_AUTH_TOKEN".upper())
+
+    def get_serverspace_from_environment(self, environment: str) -> str:
+        if environment in ["staging", "staging2"]:
+            serverspace = "stg"
+        elif environment in ["prod", "prod2"]:
+            serverspace = "prd"
+        elif environment in ["prodeu", "prodeu2"]:
+            serverspace = "prdeu"
+        elif environment in ["dev", "dev2"]:
+            serverspace = "dev"
+        elif environment in ["local", "local2"]:
+            serverspace = "local"
+        else:
+            raise ValueError("Unknown environment.")
+
+        return serverspace
```

### Comparing `pingintel_api-0.4.0/src/pingintel_api/utils.py` & `pingintel_api-0.5.0/src/pingintel_api/utils.py`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,32 +1,32 @@
-import time
-from timeit import default_timer as timer
-
-import click
-import requests
-from requests.exceptions import HTTPError
-
-global start_time
-start_time = None
-
-
-def log(msg):
-    global start_time
-    if start_time is None:
-        start_time = timer()
-    elapsed = timer() - start_time
-    timestamp = time.strftime("%Y-%m-%d %H:%M:%S")
-    click.echo(f"[{timestamp} T+{elapsed:.1f}s] {msg}")
-
-
-def raise_for_status(response: requests.Response):
-    if response.ok:
-        return
-
-    error_msg = response.text
-    log(f"{response.status_code} {response.reason}: {error_msg}")
-
-    raise HTTPError(error_msg, response=response)
-
-
-def is_fileobj(source):
-    return hasattr(source, "read")
+import time
+from timeit import default_timer as timer
+
+import click
+import requests
+from requests.exceptions import HTTPError
+
+global start_time
+start_time = None
+
+
+def log(msg):
+    global start_time
+    if start_time is None:
+        start_time = timer()
+    elapsed = timer() - start_time
+    timestamp = time.strftime("%Y-%m-%d %H:%M:%S")
+    click.echo(f"[{timestamp} T+{elapsed:.1f}s] {msg}")
+
+
+def raise_for_status(response: requests.Response):
+    if response.ok:
+        return
+
+    error_msg = response.text
+    log(f"{response.status_code} {response.reason}: {error_msg}")
+
+    raise HTTPError(error_msg, response=response)
+
+
+def is_fileobj(source):
+    return hasattr(source, "read")
```

### Comparing `pingintel_api-0.4.0/src/pingintel_api/pingvision/pingvision_api_client.py` & `pingintel_api-0.5.0/src/pingintel_api/pingvision/pingvision_api_client.py`

 * *Ordering differences only*

 * *Files 27% similar despite different names*

```diff
@@ -1,61 +1,61 @@
-#!/usr/bin/env python
-
-# Copyright 2021-2024 Ping Data Intelligence
-
-import logging
-import os
-import pprint
-import time
-from timeit import default_timer as timer
-from typing import IO, NotRequired, TypedDict, overload
-
-import click
-import requests
-
-from pingintel_api.api_client_base import APIClientBase
-
-from .. import constants as c
-from ..utils import is_fileobj, log, raise_for_status
-from . import types as t
-
-logger = logging.getLogger(__name__)
-
-
-class PingVisionAPIClient(APIClientBase):
-    api_subdomain = "api"
-    api_base_domain = "vision.pingintel.com"
-    auth_token_env_name = "PINGVISION_AUTH_TOKEN"
-    product = "pingvision"
-
-   
-    def list_submission_activity(
-        self,
-        cursor_id: str | None = None,
-        prev_cursor_id: str | None = None,
-        page_size: int | None = None,
-        fields: list[str] | None = None,
-        search: str | None = None,
-        organization__short_name: str | None = None,
-    ) -> t.PingVisionListActivityResponse:
-        url = self.api_url + "/api/v1/activity"
-
-        data = {}
-        if cursor_id:
-            data["cursor_id"] = cursor_id
-        if prev_cursor_id:
-            data["prev_cursor_id"] = prev_cursor_id
-        if page_size:
-            data["page_size"] = page_size
-        if fields:
-            data["fields"] = fields
-        if search:
-            data["search"] = search
-        if organization__short_name:
-            data["organization__short_name"] = organization__short_name
-
-        response = self.get(url, data=data)
-
-        raise_for_status(response)
-
-        response_data = response.json()
-        return response_data
+#!/usr/bin/env python
+
+# Copyright 2021-2024 Ping Data Intelligence
+
+import logging
+import os
+import pprint
+import time
+from timeit import default_timer as timer
+from typing import IO, NotRequired, TypedDict, overload
+
+import click
+import requests
+
+from pingintel_api.api_client_base import APIClientBase
+
+from .. import constants as c
+from ..utils import is_fileobj, log, raise_for_status
+from . import types as t
+
+logger = logging.getLogger(__name__)
+
+
+class PingVisionAPIClient(APIClientBase):
+    api_subdomain = "api"
+    api_base_domain = "vision.pingintel.com"
+    auth_token_env_name = "PINGVISION_AUTH_TOKEN"
+    product = "pingvision"
+
+   
+    def list_submission_activity(
+        self,
+        cursor_id: str | None = None,
+        prev_cursor_id: str | None = None,
+        page_size: int | None = None,
+        fields: list[str] | None = None,
+        search: str | None = None,
+        organization__short_name: str | None = None,
+    ) -> t.PingVisionListActivityResponse:
+        url = self.api_url + "/api/v1/activity"
+
+        data = {}
+        if cursor_id:
+            data["cursor_id"] = cursor_id
+        if prev_cursor_id:
+            data["prev_cursor_id"] = prev_cursor_id
+        if page_size:
+            data["page_size"] = page_size
+        if fields:
+            data["fields"] = fields
+        if search:
+            data["search"] = search
+        if organization__short_name:
+            data["organization__short_name"] = organization__short_name
+
+        response = self.get(url, data=data)
+
+        raise_for_status(response)
+
+        response_data = response.json()
+        return response_data
```

### Comparing `pingintel_api-0.4.0/src/pingintel_api/sov_fixer/sov_fixer_api_client.py` & `pingintel_api-0.5.0/src/pingintel_api/sov_fixer/sov_fixer_api_client.py`

 * *Ordering differences only*

 * *Files 25% similar despite different names*

```diff
@@ -1,244 +1,244 @@
-#!/usr/bin/env python
-
-# Copyright 2021-2024 Ping Data Intelligence
-
-import logging
-import os
-import pprint
-import time
-from typing import IO, NotRequired, TypedDict, overload
-
-import click
-import requests
-
-from pingintel_api.api_client_base import APIClientBase
-
-from .. import constants as c
-from ..utils import is_fileobj, log, raise_for_status
-from . import types as t
-
-logger = logging.getLogger(__name__)
-
-
-class SOVFixerAPIClient(APIClientBase):
-    api_subdomain = "api"
-    api_base_domain = "sovfixer.com"
-    auth_token_env_name = "SOVFIXER_AUTH_TOKEN"
-    product = "sovfixer"
-
-    SOV_STATUS = t.SOV_STATUS
-    SOV_RESULT_STATUS = t.SOV_RESULT_STATUS
-
-    def fix_sov_async_start(
-        self,
-        file: IO[bytes] | str,
-        document_type,
-        filename=None,
-        callback_url=None,
-        output_formats=None,
-        client_ref=None,
-        integrations=None,
-        delegate_to: str | None = None,
-    ):
-        url = self.api_url + "/api/v1/sov"
-
-        if is_fileobj(file):
-            if filename is None:
-                raise ValueError("Need filename if file is a file object.")
-
-            files = {"file": (filename, file)}
-        else:
-            if not os.path.exists(file):
-                raise click.ClickException(f"Path {file} does not exist.")
-
-            files = {"file": open(file, "rb")}
-
-        data = {}
-        if callback_url:
-            data["callback_url"] = callback_url
-        if document_type:
-            data["document_type"] = document_type
-        if output_formats:
-            data["output_formats"] = output_formats
-        if client_ref:
-            data["client_ref"] = client_ref
-        if integrations is not None:
-            data["integrations"] = integrations
-        if delegate_to is not None:
-            data["delegate_to"] = delegate_to
-
-        response = self.session.post(url, files=files, data=data)
-        if response.status_code == 200:
-            pprint.pprint(response.json())
-        else:
-            pprint.pprint(response.text)
-
-        raise_for_status(response)
-
-        response_data = response.json()
-        sov_id = response_data["id"]
-        message = response_data["message"]
-        status_url = self.api_url + f"/api/v1/sov/{sov_id}"
-        log(
-            f"+ Dispatched {sov_id}: {message}.  Now, polling for results at {status_url}."
-        )
-        return response_data
-
-    def fix_sov_async_check_progress(self, sovid_or_start_ret) -> t.FixSOVResponse:
-        if isinstance(sovid_or_start_ret, dict):
-            sov_id = sovid_or_start_ret["id"]
-        else:
-            sov_id = sovid_or_start_ret
-
-        status_url = self.api_url + f"/api/v1/sov/{sov_id}?include_progress=true"
-        # params = {"id": sov_id}
-
-        response = self.session.get(status_url)
-        # pprint.pprint(response.json())
-        raise_for_status(response)
-
-        response_data: t.FixSOVResponse = response.json()
-        # request_status = response_data["request"]["status"]
-        return response_data
-
-    def fix_sov_download(self, output_ret, actually_write=False, output_path=None):
-        output_url = output_ret["url"]
-        if (
-            self.environment
-            and self.environment == "local2"
-            and "api-local.sovfixer.com" in output_url
-        ):
-            output_url = output_url.replace("api-local.sovfixer.com", "localhost:8000")
-
-        output_description = output_ret["description"]
-        output_filename = output_ret["filename"]
-        if output_path is None:
-            output_path = output_filename
-
-        log(f"Requesting output from {output_url}...")
-        with self.session.get(output_url, stream=True) as response:
-            raise_for_status(response)
-            filesize_mb = int(response.headers.get("content-length", 0)) / 1024 / 1024
-            pprint.pprint(dict(response.headers))
-            log(f"  - Streaming {output_description} output ({filesize_mb:.2f} MB)...")
-
-            if actually_write:
-                with open(output_path, "wb") as fd:
-                    for chunk in response.iter_content(chunk_size=1024 * 1024):
-                        fd.write(chunk)
-            log(f"  - Downloaded {output_description} output: {output_path}.")
-        return output_path if actually_write else None
-
-    def fix_sov(
-        self,
-        filename,
-        *,
-        document_type: str = "SOV",
-        callback_url=None,
-        actually_write=False,
-        output_formats=None,
-        client_ref=None,
-    ):
-        sov_fixer_client = self
-        start_response = sov_fixer_client.fix_sov_async_start(
-            filename,
-            document_type=document_type,
-            callback_url=callback_url,
-            output_formats=output_formats,
-            client_ref=client_ref,
-        )
-
-        while 1:
-            response_data = sov_fixer_client.fix_sov_async_check_progress(
-                start_response
-            )
-            # raise_for_status(response_data)
-            # pprint.pprint(response_data)
-
-            request_status = response_data["request"]["status"]
-            pct_complete = response_data["request"]["pct_complete"]
-            last_status = response_data["request"]["last_health_status"]
-
-            POLL_SECS = 2.5
-            if request_status == "PENDING":
-                log("  - Has not yet been queued for processing.")
-                time.sleep(POLL_SECS)
-            elif request_status == "IN_PROGRESS":
-                log(f"  - Still in progress ({pct_complete}% complete): {last_status}")
-                time.sleep(POLL_SECS)
-            else:
-                break
-
-        result_status = response_data["result"]["status"]
-        result_message = response_data["result"]["message"]
-        log(f"+ Finished with result {result_status}: {result_message}")
-
-        if result_status == "SUCCESS":
-            log("Complete!  Fetching outputs.")
-            for output in response_data["result"]["outputs"]:
-                output_url = output["url"]
-                if (
-                    self.environment
-                    and self.environment == "local2"
-                    and "api-local.sovfixer.com" in output_url
-                ):
-                    output_url = output_url.replace(
-                        "api-local.sovfixer.com", "localhost:8000"
-                    )
-
-                output_filename = output["filename"]
-
-                output_path = output_filename
-
-                if actually_write:
-                    if os.path.exists(output_path):
-                        yesno = input(
-                            f"Do you want to overwrite the existing file {output_path} [y/N]? "
-                        )
-                        if yesno.lower() != "y":
-                            continue
-
-                sov_fixer_client.fix_sov_download(
-                    output,
-                    actually_write=actually_write,
-                    output_path=output_path,
-                )
-            return True
-        else:
-            log("* Parsing failed!  Raw API output:")
-            log(response_data)
-            return False
-
-    def list_activity(
-        self,
-        cursor_id=None,
-        prev_cursor_id=None,
-        page_size=50,
-        fields=None,
-        search=None,
-        origin=None,
-        status=None,
-        organization__short_name=None,
-    ) -> t.ActivityResponse:
-        parameters = {}
-        if cursor_id:
-            parameters["cursor_id"] = cursor_id
-        elif prev_cursor_id:
-            parameters["prev_cursor_id"] = prev_cursor_id
-        if page_size:
-            parameters["page_size"] = page_size
-        if fields:
-            parameters["fields"] = fields
-        if search:
-            parameters["search"] = search
-        if origin:
-            parameters["origin"] = origin
-        if status:
-            parameters["status"] = status
-        if organization__short_name:
-            parameters["organization__short_name"] = organization__short_name
-
-        url = self.api_url + "/api/v1/sov/activity"
-        response = self.session.get(url, params=parameters)
-        raise_for_status(response)
-        return response.json()
+#!/usr/bin/env python
+
+# Copyright 2021-2024 Ping Data Intelligence
+
+import logging
+import os
+import pprint
+import time
+from typing import IO, NotRequired, TypedDict, overload
+
+import click
+import requests
+
+from pingintel_api.api_client_base import APIClientBase
+
+from .. import constants as c
+from ..utils import is_fileobj, log, raise_for_status
+from . import types as t
+
+logger = logging.getLogger(__name__)
+
+
+class SOVFixerAPIClient(APIClientBase):
+    api_subdomain = "api"
+    api_base_domain = "sovfixer.com"
+    auth_token_env_name = "SOVFIXER_AUTH_TOKEN"
+    product = "sovfixer"
+
+    SOV_STATUS = t.SOV_STATUS
+    SOV_RESULT_STATUS = t.SOV_RESULT_STATUS
+
+    def fix_sov_async_start(
+        self,
+        file: IO[bytes] | str,
+        document_type,
+        filename=None,
+        callback_url=None,
+        output_formats=None,
+        client_ref=None,
+        integrations=None,
+        delegate_to: str | None = None,
+    ):
+        url = self.api_url + "/api/v1/sov"
+
+        if is_fileobj(file):
+            if filename is None:
+                raise ValueError("Need filename if file is a file object.")
+
+            files = {"file": (filename, file)}
+        else:
+            if not os.path.exists(file):
+                raise click.ClickException(f"Path {file} does not exist.")
+
+            files = {"file": open(file, "rb")}
+
+        data = {}
+        if callback_url:
+            data["callback_url"] = callback_url
+        if document_type:
+            data["document_type"] = document_type
+        if output_formats:
+            data["output_formats"] = output_formats
+        if client_ref:
+            data["client_ref"] = client_ref
+        if integrations is not None:
+            data["integrations"] = integrations
+        if delegate_to is not None:
+            data["delegate_to"] = delegate_to
+
+        response = self.session.post(url, files=files, data=data)
+        if response.status_code == 200:
+            pprint.pprint(response.json())
+        else:
+            pprint.pprint(response.text)
+
+        raise_for_status(response)
+
+        response_data = response.json()
+        sov_id = response_data["id"]
+        message = response_data["message"]
+        status_url = self.api_url + f"/api/v1/sov/{sov_id}"
+        log(
+            f"+ Dispatched {sov_id}: {message}.  Now, polling for results at {status_url}."
+        )
+        return response_data
+
+    def fix_sov_async_check_progress(self, sovid_or_start_ret) -> t.FixSOVResponse:
+        if isinstance(sovid_or_start_ret, dict):
+            sov_id = sovid_or_start_ret["id"]
+        else:
+            sov_id = sovid_or_start_ret
+
+        status_url = self.api_url + f"/api/v1/sov/{sov_id}?include_progress=true"
+        # params = {"id": sov_id}
+
+        response = self.session.get(status_url)
+        # pprint.pprint(response.json())
+        raise_for_status(response)
+
+        response_data: t.FixSOVResponse = response.json()
+        # request_status = response_data["request"]["status"]
+        return response_data
+
+    def fix_sov_download(self, output_ret, actually_write=False, output_path=None):
+        output_url = output_ret["url"]
+        if (
+            self.environment
+            and self.environment == "local2"
+            and "api-local.sovfixer.com" in output_url
+        ):
+            output_url = output_url.replace("api-local.sovfixer.com", "localhost:8000")
+
+        output_description = output_ret["description"]
+        output_filename = output_ret["filename"]
+        if output_path is None:
+            output_path = output_filename
+
+        log(f"Requesting output from {output_url}...")
+        with self.session.get(output_url, stream=True) as response:
+            raise_for_status(response)
+            filesize_mb = int(response.headers.get("content-length", 0)) / 1024 / 1024
+            pprint.pprint(dict(response.headers))
+            log(f"  - Streaming {output_description} output ({filesize_mb:.2f} MB)...")
+
+            if actually_write:
+                with open(output_path, "wb") as fd:
+                    for chunk in response.iter_content(chunk_size=1024 * 1024):
+                        fd.write(chunk)
+            log(f"  - Downloaded {output_description} output: {output_path}.")
+        return output_path if actually_write else None
+
+    def fix_sov(
+        self,
+        filename,
+        *,
+        document_type: str = "SOV",
+        callback_url=None,
+        actually_write=False,
+        output_formats=None,
+        client_ref=None,
+    ):
+        sov_fixer_client = self
+        start_response = sov_fixer_client.fix_sov_async_start(
+            filename,
+            document_type=document_type,
+            callback_url=callback_url,
+            output_formats=output_formats,
+            client_ref=client_ref,
+        )
+
+        while 1:
+            response_data = sov_fixer_client.fix_sov_async_check_progress(
+                start_response
+            )
+            # raise_for_status(response_data)
+            # pprint.pprint(response_data)
+
+            request_status = response_data["request"]["status"]
+            pct_complete = response_data["request"]["pct_complete"]
+            last_status = response_data["request"]["last_health_status"]
+
+            POLL_SECS = 2.5
+            if request_status == "PENDING":
+                log("  - Has not yet been queued for processing.")
+                time.sleep(POLL_SECS)
+            elif request_status == "IN_PROGRESS":
+                log(f"  - Still in progress ({pct_complete}% complete): {last_status}")
+                time.sleep(POLL_SECS)
+            else:
+                break
+
+        result_status = response_data["result"]["status"]
+        result_message = response_data["result"]["message"]
+        log(f"+ Finished with result {result_status}: {result_message}")
+
+        if result_status == "SUCCESS":
+            log("Complete!  Fetching outputs.")
+            for output in response_data["result"]["outputs"]:
+                output_url = output["url"]
+                if (
+                    self.environment
+                    and self.environment == "local2"
+                    and "api-local.sovfixer.com" in output_url
+                ):
+                    output_url = output_url.replace(
+                        "api-local.sovfixer.com", "localhost:8000"
+                    )
+
+                output_filename = output["filename"]
+
+                output_path = output_filename
+
+                if actually_write:
+                    if os.path.exists(output_path):
+                        yesno = input(
+                            f"Do you want to overwrite the existing file {output_path} [y/N]? "
+                        )
+                        if yesno.lower() != "y":
+                            continue
+
+                sov_fixer_client.fix_sov_download(
+                    output,
+                    actually_write=actually_write,
+                    output_path=output_path,
+                )
+            return True
+        else:
+            log("* Parsing failed!  Raw API output:")
+            log(response_data)
+            return False
+
+    def list_activity(
+        self,
+        cursor_id=None,
+        prev_cursor_id=None,
+        page_size=50,
+        fields=None,
+        search=None,
+        origin=None,
+        status=None,
+        organization__short_name=None,
+    ) -> t.ActivityResponse:
+        parameters = {}
+        if cursor_id:
+            parameters["cursor_id"] = cursor_id
+        elif prev_cursor_id:
+            parameters["prev_cursor_id"] = prev_cursor_id
+        if page_size:
+            parameters["page_size"] = page_size
+        if fields:
+            parameters["fields"] = fields
+        if search:
+            parameters["search"] = search
+        if origin:
+            parameters["origin"] = origin
+        if status:
+            parameters["status"] = status
+        if organization__short_name:
+            parameters["organization__short_name"] = organization__short_name
+
+        url = self.api_url + "/api/v1/sov/activity"
+        response = self.session.get(url, params=parameters)
+        raise_for_status(response)
+        return response.json()
```

### Comparing `pingintel_api-0.4.0/LICENSE` & `pingintel_api-0.5.0/LICENSE`

 * *Ordering differences only*

 * *Files 17% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-MIT License
-
-Copyright (c) 2024 Ping Data Intelligence
-
-Permission is hereby granted, free of charge, to any person obtaining a copy
-of this software and associated documentation files (the "Software"), to deal
-in the Software without restriction, including without limitation the rights
-to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-copies of the Software, and to permit persons to whom the Software is
-furnished to do so, subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in all
-copies or substantial portions of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-SOFTWARE.
+MIT License
+
+Copyright (c) 2024 Ping Data Intelligence
+
+Permission is hereby granted, free of charge, to any person obtaining a copy
+of this software and associated documentation files (the "Software"), to deal
+in the Software without restriction, including without limitation the rights
+to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+copies of the Software, and to permit persons to whom the Software is
+furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in all
+copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+SOFTWARE.
```

### Comparing `pingintel_api-0.4.0/pyproject.toml` & `pingintel_api-0.5.0/pyproject.toml`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -1,28 +1,28 @@
-[build-system]
-requires = ["hatchling"]
-build-backend = "hatchling.build"
-
-[project]
-name = "pingintel-api"
-dynamic = ["version"]
-authors = [
-  { name="Scott Stafford", email="scott@pingintel.com" },
-]
-description = "Python-based client to Ping Data Intelligence APIs"
-readme = "README.md"
-requires-python = ">=3.11"
-classifiers = [
-    "Programming Language :: Python :: 3",
-    "License :: OSI Approved :: MIT License",
-    "Operating System :: OS Independent",
-]
-
-[project.urls]
-Homepage = "https://github.com/pingintel/pingintel-api"
-Issues = "https://github.com/pingintel/pingintel-api/issues"
-
-[tool.hatch.version]
-path = "src/pingintel_api/__about__.py"
-
-[project.scripts]
+[build-system]
+requires = ["hatchling"]
+build-backend = "hatchling.build"
+
+[project]
+name = "pingintel-api"
+dynamic = ["version"]
+authors = [
+  { name="Scott Stafford", email="scott@pingintel.com" },
+]
+description = "Python-based client to Ping Data Intelligence APIs"
+readme = "README.md"
+requires-python = ">=3.11"
+classifiers = [
+    "Programming Language :: Python :: 3",
+    "License :: OSI Approved :: MIT License",
+    "Operating System :: OS Independent",
+]
+
+[project.urls]
+Homepage = "https://github.com/pingintel/pingintel-api"
+Issues = "https://github.com/pingintel/pingintel-api/issues"
+
+[tool.hatch.version]
+path = "src/pingintel_api/__about__.py"
+
+[project.scripts]
 sovfixerapi = "pingintel_api.sovfixerapi_cmd:main"
```

### Comparing `pingintel_api-0.4.0/PKG-INFO` & `pingintel_api-0.5.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: pingintel-api
-Version: 0.4.0
+Version: 0.5.0
 Summary: Python-based client to Ping Data Intelligence APIs
 Project-URL: Homepage, https://github.com/pingintel/pingintel-api
 Project-URL: Issues, https://github.com/pingintel/pingintel-api/issues
 Author-email: Scott Stafford <scott@pingintel.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

