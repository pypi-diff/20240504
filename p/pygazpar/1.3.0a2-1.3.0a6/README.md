# Comparing `tmp/pygazpar-1.3.0a2.tar.gz` & `tmp/pygazpar-1.3.0a6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pygazpar-1.3.0a2.tar", last modified: Wed Dec 28 18:44:25 2022, max compression
+gzip compressed data, was "pygazpar-1.3.0a6.tar", last modified: Sat May  4 15:16:22 2024, max compression
```

## Comparing `pygazpar-1.3.0a2.tar` & `pygazpar-1.3.0a6.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-28 18:44:25.000000 pygazpar-1.3.0a2/
--rw-r--r--   0 runner    (1001) docker     (123)     1073 2022-12-28 18:43:26.000000 pygazpar-1.3.0a2/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)      255 2022-12-28 18:43:26.000000 pygazpar-1.3.0a2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    20849 2022-12-28 18:44:25.000000 pygazpar-1.3.0a2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4846 2022-12-28 18:43:26.000000 pygazpar-1.3.0a2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-28 18:44:25.000000 pygazpar-1.3.0a2/pygazpar/
--rw-r--r--   0 runner    (1001) docker     (123)      309 2022-12-28 18:43:26.000000 pygazpar-1.3.0a2/pygazpar/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3177 2022-12-28 18:43:26.000000 pygazpar-1.3.0a2/pygazpar/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2595 2022-12-28 18:43:26.000000 pygazpar-1.3.0a2/pygazpar/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    18957 2022-12-28 18:43:26.000000 pygazpar-1.3.0a2/pygazpar/datasource.py
--rw-r--r--   0 runner    (1001) docker     (123)      898 2022-12-28 18:43:26.000000 pygazpar-1.3.0a2/pygazpar/enum.py
--rw-r--r--   0 runner    (1001) docker     (123)     5915 2022-12-28 18:43:26.000000 pygazpar-1.3.0a2/pygazpar/excelparser.py
--rw-r--r--   0 runner    (1001) docker     (123)     1804 2022-12-28 18:43:26.000000 pygazpar-1.3.0a2/pygazpar/jsonparser.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-28 18:44:25.000000 pygazpar-1.3.0a2/pygazpar/resources/
--rw-r--r--   0 runner    (1001) docker     (123)   199583 2022-12-28 18:43:26.000000 pygazpar-1.3.0a2/pygazpar/resources/daily_data_sample.json
--rw-r--r--   0 runner    (1001) docker     (123)        3 2022-12-28 18:43:26.000000 pygazpar-1.3.0a2/pygazpar/resources/hourly_data_sample.json
--rw-r--r--   0 runner    (1001) docker     (123)     3351 2022-12-28 18:43:26.000000 pygazpar-1.3.0a2/pygazpar/resources/monthly_data_sample.json
--rw-r--r--   0 runner    (1001) docker     (123)    15587 2022-12-28 18:43:26.000000 pygazpar-1.3.0a2/pygazpar/resources/weekly_data_sample.json
--rw-r--r--   0 runner    (1001) docker     (123)      446 2022-12-28 18:43:26.000000 pygazpar-1.3.0a2/pygazpar/resources/yearly_data_sample.json
--rw-r--r--   0 runner    (1001) docker     (123)       24 2022-12-28 18:44:24.000000 pygazpar-1.3.0a2/pygazpar/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-28 18:44:25.000000 pygazpar-1.3.0a2/pygazpar.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    20849 2022-12-28 18:44:25.000000 pygazpar-1.3.0a2/pygazpar.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      839 2022-12-28 18:44:25.000000 pygazpar-1.3.0a2/pygazpar.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2022-12-28 18:44:25.000000 pygazpar-1.3.0a2/pygazpar.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       53 2022-12-28 18:44:25.000000 pygazpar-1.3.0a2/pygazpar.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2022-12-28 18:44:25.000000 pygazpar-1.3.0a2/pygazpar.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       40 2022-12-28 18:44:25.000000 pygazpar-1.3.0a2/pygazpar.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       23 2022-12-28 18:44:25.000000 pygazpar-1.3.0a2/pygazpar.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-28 18:44:25.000000 pygazpar-1.3.0a2/samples/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-28 18:43:26.000000 pygazpar-1.3.0a2/samples/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      765 2022-12-28 18:43:26.000000 pygazpar-1.3.0a2/samples/excelSample.py
--rw-r--r--   0 runner    (1001) docker     (123)      736 2022-12-28 18:43:26.000000 pygazpar-1.3.0a2/samples/jsonSample.py
--rw-r--r--   0 runner    (1001) docker     (123)      387 2022-12-28 18:43:26.000000 pygazpar-1.3.0a2/samples/testSample.py
--rw-r--r--   0 runner    (1001) docker     (123)     1491 2022-12-28 18:44:25.000000 pygazpar-1.3.0a2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       38 2022-12-28 18:43:26.000000 pygazpar-1.3.0a2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-28 18:44:25.000000 pygazpar-1.3.0a2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-28 18:43:26.000000 pygazpar-1.3.0a2/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5134 2022-12-28 18:43:26.000000 pygazpar-1.3.0a2/tests/test_client.py
--rw-r--r--   0 runner    (1001) docker     (123)      818 2022-12-28 18:43:26.000000 pygazpar-1.3.0a2/tests/test_datafileparser.py
--rw-r--r--   0 runner    (1001) docker     (123)     5983 2022-12-28 18:43:26.000000 pygazpar-1.3.0a2/tests/test_datasource.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 15:16:22.928136 pygazpar-1.3.0a6/
+-rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-05-04 15:14:22.000000 pygazpar-1.3.0a6/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (127)      255 2024-05-04 15:14:22.000000 pygazpar-1.3.0a6/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    20961 2024-05-04 15:16:22.928136 pygazpar-1.3.0a6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4846 2024-05-04 15:14:22.000000 pygazpar-1.3.0a6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 15:16:22.928136 pygazpar-1.3.0a6/pygazpar/
+-rw-r--r--   0 runner    (1001) docker     (127)      309 2024-05-04 15:14:22.000000 pygazpar-1.3.0a6/pygazpar/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3177 2024-05-04 15:14:22.000000 pygazpar-1.3.0a6/pygazpar/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2595 2024-05-04 15:14:22.000000 pygazpar-1.3.0a6/pygazpar/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21374 2024-05-04 15:14:22.000000 pygazpar-1.3.0a6/pygazpar/datasource.py
+-rw-r--r--   0 runner    (1001) docker     (127)      898 2024-05-04 15:14:22.000000 pygazpar-1.3.0a6/pygazpar/enum.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5915 2024-05-04 15:14:22.000000 pygazpar-1.3.0a6/pygazpar/excelparser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1804 2024-05-04 15:14:22.000000 pygazpar-1.3.0a6/pygazpar/jsonparser.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 15:16:22.928136 pygazpar-1.3.0a6/pygazpar/resources/
+-rw-r--r--   0 runner    (1001) docker     (127)   199583 2024-05-04 15:14:22.000000 pygazpar-1.3.0a6/pygazpar/resources/daily_data_sample.json
+-rw-r--r--   0 runner    (1001) docker     (127)        3 2024-05-04 15:14:22.000000 pygazpar-1.3.0a6/pygazpar/resources/hourly_data_sample.json
+-rw-r--r--   0 runner    (1001) docker     (127)     3351 2024-05-04 15:14:22.000000 pygazpar-1.3.0a6/pygazpar/resources/monthly_data_sample.json
+-rw-r--r--   0 runner    (1001) docker     (127)    15587 2024-05-04 15:14:22.000000 pygazpar-1.3.0a6/pygazpar/resources/weekly_data_sample.json
+-rw-r--r--   0 runner    (1001) docker     (127)      446 2024-05-04 15:14:22.000000 pygazpar-1.3.0a6/pygazpar/resources/yearly_data_sample.json
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-04 15:16:21.000000 pygazpar-1.3.0a6/pygazpar/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 15:16:22.928136 pygazpar-1.3.0a6/pygazpar.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    20961 2024-05-04 15:16:22.000000 pygazpar-1.3.0a6/pygazpar.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      839 2024-05-04 15:16:22.000000 pygazpar-1.3.0a6/pygazpar.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-04 15:16:22.000000 pygazpar-1.3.0a6/pygazpar.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-05-04 15:16:22.000000 pygazpar-1.3.0a6/pygazpar.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-04 15:16:22.000000 pygazpar-1.3.0a6/pygazpar.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       40 2024-05-04 15:16:22.000000 pygazpar-1.3.0a6/pygazpar.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-04 15:16:22.000000 pygazpar-1.3.0a6/pygazpar.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 15:16:22.928136 pygazpar-1.3.0a6/samples/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-04 15:14:22.000000 pygazpar-1.3.0a6/samples/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      765 2024-05-04 15:14:22.000000 pygazpar-1.3.0a6/samples/excelSample.py
+-rw-r--r--   0 runner    (1001) docker     (127)      736 2024-05-04 15:14:22.000000 pygazpar-1.3.0a6/samples/jsonSample.py
+-rw-r--r--   0 runner    (1001) docker     (127)      387 2024-05-04 15:14:22.000000 pygazpar-1.3.0a6/samples/testSample.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1491 2024-05-04 15:16:22.932136 pygazpar-1.3.0a6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-04 15:14:22.000000 pygazpar-1.3.0a6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 15:16:22.928136 pygazpar-1.3.0a6/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-04 15:14:22.000000 pygazpar-1.3.0a6/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5111 2024-05-04 15:14:22.000000 pygazpar-1.3.0a6/tests/test_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)      818 2024-05-04 15:14:22.000000 pygazpar-1.3.0a6/tests/test_datafileparser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5983 2024-05-04 15:14:22.000000 pygazpar-1.3.0a6/tests/test_datasource.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `pygazpar-1.3.0a2/LICENSE.md` & `pygazpar-1.3.0a6/LICENSE.md`

 * *Files identical despite different names*

### Comparing `pygazpar-1.3.0a2/PKG-INFO` & `pygazpar-1.3.0a6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pygazpar
-Version: 1.3.0a2
+Version: 1.3.0a6
 Summary: Retrieve gas consumption from GrDF web site (French Gas Company)
 Home-page: https://github.com/ssenart/pygazpar
 Author: Stephane Senart
 Author-email: stephane.senart@gmail.com
 License: MIT
 Download-URL: https://github.com/ssenart/pygazpar/releases
 Project-URL: Home, https://github.com/ssenart/pygazpar
@@ -193,17 +193,20 @@
         Corresponding Home Assistant integration custom component is available [here](https://github.com/ssenart/home-assistant-gazpar).
         # Changelog
         All notable changes to this project will be documented in this file.
         
         The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
         and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).
         
-        ## [1.2.1](https://github.com/ssenart/PyGazpar/compare/1.2.0...1.2.1) - 2022-12-28
+        
+        ## [1.2.1](https://github.com/ssenart/PyGazpar/compare/1.2.0...1.2.1) - 2024-05-04
         
         ### Fixed
+        - [#64](https://github.com/ssenart/PyGazpar/issues/64): [Issue] Captcha failed issue.
+        
         - [#63](https://github.com/ssenart/PyGazpar/issues/63): [Bug] If the latest received consumption is Sunday, then the last weekly period is duplicated.
         
         ## [1.2.0](https://github.com/ssenart/PyGazpar/compare/1.1.6...1.2.0) - 2022-12-16
         
         ### Changed
         - [#59](https://github.com/ssenart/PyGazpar/issues/59): [Feature] Support both Excel and Json data source format from GrDF site.
```

### Comparing `pygazpar-1.3.0a2/README.md` & `pygazpar-1.3.0a6/README.md`

 * *Files identical despite different names*

### Comparing `pygazpar-1.3.0a2/pygazpar/__main__.py` & `pygazpar-1.3.0a6/pygazpar/__main__.py`

 * *Files identical despite different names*

### Comparing `pygazpar-1.3.0a2/pygazpar/client.py` & `pygazpar-1.3.0a6/pygazpar/client.py`

 * *Files identical despite different names*

### Comparing `pygazpar-1.3.0a2/pygazpar/datasource.py` & `pygazpar-1.3.0a6/pygazpar/datasource.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,29 +1,38 @@
 import logging
 import glob
 import os
 import json
+import time
 import pandas as pd
+import http.cookiejar
 from abc import ABC, abstractmethod
 from typing import Any, List, Dict, cast, Optional
 from requests import Session
 from datetime import date, timedelta
 from pygazpar.enum import Frequency, PropertyName
 from pygazpar.excelparser import ExcelParser
 from pygazpar.jsonparser import JsonParser
 
-AUTH_NONCE_URL = "https://monespace.grdf.fr/client/particulier/accueil"
-LOGIN_URL = "https://login.monespace.grdf.fr/sofit-account-api/api/v1/auth"
-LOGIN_HEADER = {"domain": "grdf.fr"}
-LOGIN_PAYLOAD = """{{
-    "email": "{0}",
+SESSION_TOKEN_URL = "https://connexion.grdf.fr/api/v1/authn"
+SESSION_TOKEN_PAYLOAD = """{{
+    "username": "{0}",
     "password": "{1}",
-    "capp": "meg",
-    "goto": "https://sofa-connexion.grdf.fr:443/openam/oauth2/externeGrdf/authorize?response_type=code&scope=openid%20profile%20email%20infotravaux%20%2Fv1%2Faccreditation%20%2Fv1%2Faccreditations%20%2Fdigiconso%2Fv1%20%2Fdigiconso%2Fv1%2Fconsommations%20new_meg&client_id=prod_espaceclient&state=0&redirect_uri=https%3A%2F%2Fmonespace.grdf.fr%2F_codexch&nonce={2}&by_pass_okta=1&capp=meg"}}"""
-
+    "options": {{
+        "multiOptionalFactorEnroll": "false",
+        "warnBeforePasswordExpired": "false"
+    }}
+}}"""
+
+AUTH_TOKEN_URL = "https://connexion.grdf.fr/login/sessionCookieRedirect"
+AUTH_TOKEN_PARAMS = """{{
+    "checkAccountSetupComplete": "true",
+    "token": "{0}",
+    "redirectUrl": "https://monespace.grdf.fr"
+}}"""
 
 Logger = logging.getLogger(__name__)
 
 MeterReading = Dict[str, Any]
 
 MeterReadings = List[MeterReading]
 
@@ -46,64 +55,67 @@
 
         self.__username = username
         self.__password = password
 
     # ------------------------------------------------------
     def load(self, pceIdentifier: str, startDate: date, endDate: date, frequencies: Optional[List[Frequency]] = None) -> MeterReadingsByFrequency:
 
-        session = Session()
-
-        session.headers.update(LOGIN_HEADER)
-
-        self._login(session, self.__username, self.__password)
+        auth_token = self._login(self.__username, self.__password)
 
-        res = self._loadFromSession(session, pceIdentifier, startDate, endDate, frequencies)
+        res = self._loadFromSession(auth_token, pceIdentifier, startDate, endDate, frequencies)
 
         Logger.debug("The data update terminates normally")
 
         return res
 
     # ------------------------------------------------------
-    def _login(self, session: Session, username: str, password: str):
+    def _login(self, username: str, password: str) -> str:
 
-        # Get auth_nonce token.
-        session.get(AUTH_NONCE_URL)
-        if "auth_nonce" not in session.cookies:
-            raise Exception("Login error: Cannot get auth_nonce token")
-        auth_nonce = session.cookies.get("auth_nonce")
+        session = Session()
+        session.headers.update({"domain": "grdf.fr"})
+        session.headers.update({"Content-Type": "application/json"})
+        session.headers.update({"X-Requested-With": "XMLHttpRequest"})
 
-        # Build the login payload as a json string.
-        payload = LOGIN_PAYLOAD.format(username, password, auth_nonce)
+        payload = SESSION_TOKEN_PAYLOAD.format(username, password)
 
-        # Build the login payload as a python object.
-        data = json.loads(payload)
+        response = session.post(SESSION_TOKEN_URL, data=payload)
 
-        # Send the login command.
-        response = session.post(LOGIN_URL, data=data)
+        if response.status_code != 200:
+            raise Exception(f"An error occurred while logging in. Status code: {response.status_code} - {response.text}")
 
-        # Check login result.
-        loginData = response.json()
+        session_token = response.json().get("sessionToken")
 
-        response.raise_for_status()
+        Logger.debug("Session token: %s", session_token)
+
+        jar = http.cookiejar.CookieJar()
+
+        session = Session()
+        session.headers.update({"Content-Type": "application/json"})
+        session.headers.update({"X-Requested-With": "XMLHttpRequest"})
+
+        params = json.loads(AUTH_TOKEN_PARAMS.format(session_token))
+
+        response = session.get(AUTH_TOKEN_URL, params=params, allow_redirects=True, cookies=jar)
+
+        if response.status_code != 200:
+            raise Exception(f"An error occurred while getting the auth token. Status code: {response.status_code} - {response.text}")
 
-        if "status" in loginData and "error" in loginData and loginData["status"] >= 400:
-            raise Exception(f"{loginData['error']} ({loginData['status']})")
+        auth_token = session.cookies.get("auth_token", domain="monespace.grdf.fr")
 
-        if "state" in loginData and loginData["state"] != "SUCCESS":
-            raise Exception(loginData["error"])
+        return auth_token
 
     @abstractmethod
-    def _loadFromSession(self, session: Session, pceIdentifier: str, startDate: date, endDate: date, frequencies: Optional[List[Frequency]] = None) -> MeterReadingsByFrequency:
+    def _loadFromSession(self, auth_token: str, pceIdentifier: str, startDate: date, endDate: date, frequencies: Optional[List[Frequency]] = None) -> MeterReadingsByFrequency:
         pass
 
 
 # ------------------------------------------------------------------------------------------------------------
 class ExcelWebDataSource(WebDataSource):
 
-    DATA_URL = "https://monespace.grdf.fr/api/e-conso/pce/consommation/informatives/telecharger?dateDebut={0}&dateFin={1}&frequence={3}&pceList%5B%5D={2}"
+    DATA_URL = "https://monespace.grdf.fr/api/e-conso/pce/consommation/informatives/telecharger?dateDebut={0}&dateFin={1}&frequence={3}&pceList[]={2}"
 
     DATE_FORMAT = "%Y-%m-%d"
 
     FREQUENCY_VALUES = {
         Frequency.HOURLY: "Horaire",
         Frequency.DAILY: "Journalier",
         Frequency.WEEKLY: "Hebdomadaire",
@@ -117,15 +129,15 @@
     def __init__(self, username: str, password: str, tmpDirectory: str):
 
         super().__init__(username, password)
 
         self.__tmpDirectory = tmpDirectory
 
     # ------------------------------------------------------
-    def _loadFromSession(self, session: Session, pceIdentifier: str, startDate: date, endDate: date, frequencies: Optional[List[Frequency]] = None) -> MeterReadingsByFrequency:
+    def _loadFromSession(self, auth_token: str, pceIdentifier: str, startDate: date, endDate: date, frequencies: Optional[List[Frequency]] = None) -> MeterReadingsByFrequency:
 
         res = {}
 
         # XLSX is in the TMP directory
         data_file_path_pattern = self.__tmpDirectory + '/' + ExcelWebDataSource.DATA_FILENAME
 
         # We remove an eventual existing data file (from a previous run that has not deleted it).
@@ -141,41 +153,71 @@
             # Get unique values.
             frequencyList = set(frequencies)
 
         for frequency in frequencyList:
             # Inject parameters.
             downloadUrl = ExcelWebDataSource.DATA_URL.format(startDate.strftime(ExcelWebDataSource.DATE_FORMAT), endDate.strftime(ExcelWebDataSource.DATE_FORMAT), pceIdentifier, ExcelWebDataSource.FREQUENCY_VALUES[frequency])
 
-            session.get(downloadUrl)  # First request does not return anything : strange...
-
             Logger.debug(f"Loading data of frequency {ExcelWebDataSource.FREQUENCY_VALUES[frequency]} from {startDate.strftime(ExcelWebDataSource.DATE_FORMAT)} to {endDate.strftime(ExcelWebDataSource.DATE_FORMAT)}")
 
-            self.__downloadFile(session, downloadUrl, self.__tmpDirectory)
+            # Retry mechanism.
+            retry = 10
+            while retry > 0:
+
+                # Create a session.
+                session = Session()
+                session.headers.update({"Host": "monespace.grdf.fr"})
+                session.headers.update({"Domain": "grdf.fr"})
+                session.headers.update({"X-Requested-With": "XMLHttpRequest"})
+                session.headers.update({"Accept": "application/json"})
+                session.cookies.set("auth_token", auth_token, domain="monespace.grdf.fr")
+
+                try:
+                    self.__downloadFile(session, downloadUrl, self.__tmpDirectory)
+                    break
+                except Exception as e:
+
+                    if retry == 1:
+                        raise e
+
+                    Logger.error("An error occurred while loading data. Retry in 3 seconds.")
+                    time.sleep(3)
+                    retry -= 1
 
             # Load the XLSX file into the data structure
             file_list = glob.glob(data_file_path_pattern)
 
             if len(file_list) == 0:
                 Logger.warning(f"Not any data file has been found in '{self.__tmpDirectory}' directory")
 
             for filename in file_list:
                 res[frequency.value] = ExcelParser.parse(filename, frequency if frequency != Frequency.YEARLY else Frequency.DAILY)
-                os.remove(filename)
+                try:
+                    # openpyxl does not close the file properly.
+                    os.remove(filename)
+                except Exception:
+                    pass
 
             # We compute yearly from daily data.
             if frequency == Frequency.YEARLY:
                 res[frequency.value] = FrequencyConverter.computeYearly(res[frequency.value])
 
         return res
 
     # ------------------------------------------------------
     def __downloadFile(self, session: Session, url: str, path: str):
 
         response = session.get(url)
 
+        if "text/html" in response.headers.get("Content-Type"):
+            raise Exception("An error occurred while loading data. Please check your credentials.")
+
+        if response.status_code != 200:
+            raise Exception(f"An error occurred while loading data. Status code: {response.status_code} - {response.text}")
+
         response.raise_for_status()
 
         filename = response.headers["Content-Disposition"].split("filename=")[1]
 
         open(f"{path}/{filename}", "wb").write(response.content)
 
 
@@ -206,46 +248,73 @@
 
         return res
 
 
 # ------------------------------------------------------------------------------------------------------------
 class JsonWebDataSource(WebDataSource):
 
-    DATA_URL = "https://monespace.grdf.fr/api/e-conso/pce/consommation/informatives?dateDebut={0}&dateFin={1}&pceList%5B%5D={2}"
+    DATA_URL = "https://monespace.grdf.fr/api/e-conso/pce/consommation/informatives?dateDebut={0}&dateFin={1}&pceList[]={2}"
 
     TEMPERATURES_URL = "https://monespace.grdf.fr/api/e-conso/pce/{0}/meteo?dateFinPeriode={1}&nbJours={2}"
 
     INPUT_DATE_FORMAT = "%Y-%m-%d"
 
     OUTPUT_DATE_FORMAT = "%d/%m/%Y"
 
     def __init__(self, username: str, password: str):
 
         super().__init__(username, password)
 
-    def _loadFromSession(self, session: Session, pceIdentifier: str, startDate: date, endDate: date, frequencies: Optional[List[Frequency]] = None) -> MeterReadingsByFrequency:
+    def _loadFromSession(self, auth_token: str, pceIdentifier: str, startDate: date, endDate: date, frequencies: Optional[List[Frequency]] = None) -> MeterReadingsByFrequency:
 
         res = {}
 
         computeByFrequency = {
             Frequency.HOURLY: FrequencyConverter.computeHourly,
             Frequency.DAILY: FrequencyConverter.computeDaily,
             Frequency.WEEKLY: FrequencyConverter.computeWeekly,
             Frequency.MONTHLY: FrequencyConverter.computeMonthly,
             Frequency.YEARLY: FrequencyConverter.computeYearly
         }
 
         # Data URL: Inject parameters.
         downloadUrl = JsonWebDataSource.DATA_URL.format(startDate.strftime(JsonWebDataSource.INPUT_DATE_FORMAT), endDate.strftime(JsonWebDataSource.INPUT_DATE_FORMAT), pceIdentifier)
 
-        # First request never returns data.
-        session.get(downloadUrl)
+        # Retry mechanism.
+        retry = 10
+        while retry > 0:
+
+            # Create a session.
+            session = Session()
+            session.headers.update({"Host": "monespace.grdf.fr"})
+            session.headers.update({"Domain": "grdf.fr"})
+            session.headers.update({"X-Requested-With": "XMLHttpRequest"})
+            session.headers.update({"Accept": "application/json"})
+            session.cookies.set("auth_token", auth_token, domain="monespace.grdf.fr")
+
+            try:
+                response = session.get(downloadUrl)
+
+                if "text/html" in response.headers.get("Content-Type"):
+                    raise Exception("An error occurred while loading data. Please check your credentials.")
+
+                if response.status_code != 200:
+                    raise Exception(f"An error occurred while loading data. Status code: {response.status_code} - {response.text}")
+
+                break
+            except Exception as e:
+
+                if retry == 1:
+                    raise e
+
+                Logger.error("An error occurred while loading data. Retry in 3 seconds.")
+                time.sleep(3)
+                retry -= 1
 
-        # Get consumption data.
-        data = session.get(downloadUrl).text
+        data = response.text
 
         # Temperatures URL: Inject parameters.
         endDate = date.today() - timedelta(days=1) if endDate >= date.today() else endDate
         days = min((endDate - startDate).days, 730)
         temperaturesUrl = JsonWebDataSource.TEMPERATURES_URL.format(pceIdentifier, endDate.strftime(JsonWebDataSource.INPUT_DATE_FORMAT), days)
 
         # Get weather data.
```

### Comparing `pygazpar-1.3.0a2/pygazpar/enum.py` & `pygazpar-1.3.0a6/pygazpar/enum.py`

 * *Files identical despite different names*

### Comparing `pygazpar-1.3.0a2/pygazpar/excelparser.py` & `pygazpar-1.3.0a6/pygazpar/excelparser.py`

 * *Files identical despite different names*

### Comparing `pygazpar-1.3.0a2/pygazpar/jsonparser.py` & `pygazpar-1.3.0a6/pygazpar/jsonparser.py`

 * *Files identical despite different names*

### Comparing `pygazpar-1.3.0a2/pygazpar/resources/daily_data_sample.json` & `pygazpar-1.3.0a6/pygazpar/resources/daily_data_sample.json`

 * *Files identical despite different names*

### Comparing `pygazpar-1.3.0a2/pygazpar/resources/monthly_data_sample.json` & `pygazpar-1.3.0a6/pygazpar/resources/monthly_data_sample.json`

 * *Files identical despite different names*

### Comparing `pygazpar-1.3.0a2/pygazpar/resources/weekly_data_sample.json` & `pygazpar-1.3.0a6/pygazpar/resources/weekly_data_sample.json`

 * *Files identical despite different names*

### Comparing `pygazpar-1.3.0a2/pygazpar.egg-info/PKG-INFO` & `pygazpar-1.3.0a6/pygazpar.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pygazpar
-Version: 1.3.0a2
+Version: 1.3.0a6
 Summary: Retrieve gas consumption from GrDF web site (French Gas Company)
 Home-page: https://github.com/ssenart/pygazpar
 Author: Stephane Senart
 Author-email: stephane.senart@gmail.com
 License: MIT
 Download-URL: https://github.com/ssenart/pygazpar/releases
 Project-URL: Home, https://github.com/ssenart/pygazpar
@@ -193,17 +193,20 @@
         Corresponding Home Assistant integration custom component is available [here](https://github.com/ssenart/home-assistant-gazpar).
         # Changelog
         All notable changes to this project will be documented in this file.
         
         The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
         and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).
         
-        ## [1.2.1](https://github.com/ssenart/PyGazpar/compare/1.2.0...1.2.1) - 2022-12-28
+        
+        ## [1.2.1](https://github.com/ssenart/PyGazpar/compare/1.2.0...1.2.1) - 2024-05-04
         
         ### Fixed
+        - [#64](https://github.com/ssenart/PyGazpar/issues/64): [Issue] Captcha failed issue.
+        
         - [#63](https://github.com/ssenart/PyGazpar/issues/63): [Bug] If the latest received consumption is Sunday, then the last weekly period is duplicated.
         
         ## [1.2.0](https://github.com/ssenart/PyGazpar/compare/1.1.6...1.2.0) - 2022-12-16
         
         ### Changed
         - [#59](https://github.com/ssenart/PyGazpar/issues/59): [Feature] Support both Excel and Json data source format from GrDF site.
```

### Comparing `pygazpar-1.3.0a2/pygazpar.egg-info/SOURCES.txt` & `pygazpar-1.3.0a6/pygazpar.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pygazpar-1.3.0a2/samples/excelSample.py` & `pygazpar-1.3.0a6/samples/excelSample.py`

 * *Files identical despite different names*

### Comparing `pygazpar-1.3.0a2/samples/jsonSample.py` & `pygazpar-1.3.0a6/samples/jsonSample.py`

 * *Files identical despite different names*

### Comparing `pygazpar-1.3.0a2/setup.cfg` & `pygazpar-1.3.0a6/setup.cfg`

 * *Files identical despite different names*

### Comparing `pygazpar-1.3.0a2/tests/test_client.py` & `pygazpar-1.3.0a6/tests/test_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -71,15 +71,15 @@
         client = Client(JsonWebDataSource(self.__username, self.__password))
 
         data = client.loadSince(self.__pceIdentifier, 365, [Frequency.MONTHLY])
 
         assert (len(data[Frequency.MONTHLY.value]) >= 12 and len(data[Frequency.MONTHLY.value]) <= 13)
 
     def test_yearly_jsonweb(self):
-        client = Client(ExcelWebDataSource(self.__username, self.__password, self.__tmp_directory))
+        client = Client(JsonWebDataSource(self.__username, self.__password))
 
         data = client.loadSince(self.__pceIdentifier, 365, [Frequency.YEARLY])
 
         assert (len(data[Frequency.YEARLY.value]) == 1)
 
     def test_daily_excelweb(self):
         client = Client(ExcelWebDataSource(self.__username, self.__password, self.__tmp_directory))
```

### Comparing `pygazpar-1.3.0a2/tests/test_datafileparser.py` & `pygazpar-1.3.0a6/tests/test_datafileparser.py`

 * *Files identical despite different names*

### Comparing `pygazpar-1.3.0a2/tests/test_datasource.py` & `pygazpar-1.3.0a6/tests/test_datasource.py`

 * *Files identical despite different names*

