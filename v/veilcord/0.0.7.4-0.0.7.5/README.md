# Comparing `tmp/veilcord-0.0.7.4.tar.gz` & `tmp/veilcord-0.0.7.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "veilcord-0.0.7.4.tar", last modified: Fri Dec 15 01:07:47 2023, max compression
+gzip compressed data, was "veilcord-0.0.7.5.tar", last modified: Sat May  4 12:57:38 2024, max compression
```

## Comparing `veilcord-0.0.7.4.tar` & `veilcord-0.0.7.5.tar`

### file list

```diff
@@ -1,22 +1,23 @@
-drwxrwxrwx   0        0        0        0 2023-12-15 01:07:47.643490 veilcord-0.0.7.4/
--rw-rw-rw-   0        0        0     1085 2023-05-20 20:15:11.000000 veilcord-0.0.7.4/LICENSE
--rw-rw-rw-   0        0        0     4114 2023-12-15 01:07:47.642492 veilcord-0.0.7.4/PKG-INFO
--rw-rw-rw-   0        0        0     2619 2023-12-11 21:01:24.000000 veilcord-0.0.7.4/README.md
--rw-rw-rw-   0        0        0       86 2023-05-08 02:01:12.000000 veilcord-0.0.7.4/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-12-15 01:07:47.643490 veilcord-0.0.7.4/setup.cfg
--rw-rw-rw-   0        0        0     1839 2023-12-15 01:07:28.000000 veilcord-0.0.7.4/setup.py
-drwxrwxrwx   0        0        0        0 2023-12-15 01:07:47.622359 veilcord-0.0.7.4/veilcord/
--rw-rw-rw-   0        0        0      708 2023-12-15 01:07:24.000000 veilcord-0.0.7.4/veilcord/__init__.py
--rw-rw-rw-   0        0        0    11998 2023-12-15 00:54:26.000000 veilcord-0.0.7.4/veilcord/__main__.py
--rw-rw-rw-   0        0        0     8400 2023-12-15 00:54:28.000000 veilcord-0.0.7.4/veilcord/__session__.py
--rw-rw-rw-   0        0        0     9530 2023-12-15 01:07:13.000000 veilcord-0.0.7.4/veilcord/__solver__.py
--rw-rw-rw-   0        0        0     2879 2023-12-11 18:00:10.000000 veilcord-0.0.7.4/veilcord/__udcord__.py
-drwxrwxrwx   0        0        0        0 2023-12-15 01:07:47.640465 veilcord-0.0.7.4/veilcord/types/
--rw-rw-rw-   0        0        0     4012 2023-12-15 00:45:08.000000 veilcord-0.0.7.4/veilcord/types/device.py
--rw-rw-rw-   0        0        0     2103 2023-12-11 15:08:48.000000 veilcord-0.0.7.4/veilcord/types/websocket.py
-drwxrwxrwx   0        0        0        0 2023-12-15 01:07:47.641419 veilcord-0.0.7.4/veilcord.egg-info/
--rw-rw-rw-   0        0        0     4114 2023-12-15 01:07:47.000000 veilcord-0.0.7.4/veilcord.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      365 2023-12-15 01:07:47.000000 veilcord-0.0.7.4/veilcord.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-12-15 01:07:47.000000 veilcord-0.0.7.4/veilcord.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      125 2023-12-15 01:07:47.000000 veilcord-0.0.7.4/veilcord.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-12-15 01:07:47.000000 veilcord-0.0.7.4/veilcord.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-04 12:57:38.833084 veilcord-0.0.7.5/
+-rw-rw-rw-   0        0        0     1085 2023-05-20 20:15:11.000000 veilcord-0.0.7.5/LICENSE
+-rw-rw-rw-   0        0        0     4111 2024-05-04 12:57:38.832237 veilcord-0.0.7.5/PKG-INFO
+-rw-rw-rw-   0        0        0     2619 2024-02-16 17:51:54.000000 veilcord-0.0.7.5/README.md
+-rw-rw-rw-   0        0        0       86 2023-05-08 02:01:12.000000 veilcord-0.0.7.5/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-05-04 12:57:38.833084 veilcord-0.0.7.5/setup.cfg
+-rw-rw-rw-   0        0        0     1837 2024-05-04 12:55:54.000000 veilcord-0.0.7.5/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-04 12:57:38.805199 veilcord-0.0.7.5/veilcord/
+-rw-rw-rw-   0        0        0      735 2024-02-16 17:56:45.000000 veilcord-0.0.7.5/veilcord/__init__.py
+-rw-rw-rw-   0        0        0    12878 2024-04-27 16:47:34.000000 veilcord-0.0.7.5/veilcord/__main__.py
+-rw-rw-rw-   0        0        0     8633 2024-04-27 16:47:31.000000 veilcord-0.0.7.5/veilcord/__session__.py
+-rw-rw-rw-   0        0        0     9655 2024-04-20 14:30:08.000000 veilcord-0.0.7.5/veilcord/__solver__.py
+-rw-rw-rw-   0        0        0     6226 2024-02-24 14:35:43.000000 veilcord-0.0.7.5/veilcord/__udcord__.py
+drwxrwxrwx   0        0        0        0 2024-05-04 12:57:38.829228 veilcord-0.0.7.5/veilcord/models/
+-rw-rw-rw-   0        0        0     4000 2024-04-27 16:36:20.000000 veilcord-0.0.7.5/veilcord/models/device.py
+-rw-rw-rw-   0        0        0     1202 2024-04-27 17:06:45.000000 veilcord-0.0.7.5/veilcord/models/dynamic.py
+-rw-rw-rw-   0        0        0     2741 2024-04-27 16:47:25.000000 veilcord-0.0.7.5/veilcord/models/websocket.py
+drwxrwxrwx   0        0        0        0 2024-05-04 12:57:38.831224 veilcord-0.0.7.5/veilcord.egg-info/
+-rw-rw-rw-   0        0        0     4111 2024-05-04 12:57:38.000000 veilcord-0.0.7.5/veilcord.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      394 2024-05-04 12:57:38.000000 veilcord-0.0.7.5/veilcord.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-04 12:57:38.000000 veilcord-0.0.7.5/veilcord.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      125 2024-05-04 12:57:38.000000 veilcord-0.0.7.5/veilcord.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2024-05-04 12:57:38.000000 veilcord-0.0.7.5/veilcord.egg-info/top_level.txt
```

### Comparing `veilcord-0.0.7.4/LICENSE` & `veilcord-0.0.7.5/LICENSE`

 * *Files identical despite different names*

### Comparing `veilcord-0.0.7.4/PKG-INFO` & `veilcord-0.0.7.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: veilcord
-Version: 0.0.7.4
+Version: 0.0.7.5
 Summary: VeilCord // @imvast
 Home-page: http://pypi.python.org/pypi/veilcord
 Author: @imvast
 Author-email: dev@vast.sh
 License: MIT
 Project-URL: Homepage, https://github.com/imvast
 Project-URL: Suggestions, https://github.com/imvast/veilcord/issues
-Project-URL: Support, https://discord.gg/vast
+Project-URL: Support, https://t.me/skiddos
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
```

#### html2text {}

```diff
@@ -1,12 +1,12 @@
-Metadata-Version: 2.1 Name: veilcord Version: 0.0.7.4 Summary: VeilCord /
+Metadata-Version: 2.1 Name: veilcord Version: 0.0.7.5 Summary: VeilCord /
 / @imvast Home-page: http://pypi.python.org/pypi/veilcord Author: @imvast
 Author-email: dev@vast.sh License: MIT Project-URL: Homepage, https://
 github.com/imvast Project-URL: Suggestions, https://github.com/imvast/veilcord/
-issues Project-URL: Support, https://discord.gg/vast Classifier: Development
+issues Project-URL: Support, https://t.me/skiddos Classifier: Development
 Status :: 3 - Alpha Classifier: Intended Audience :: Developers Classifier:
 License :: OSI Approved :: MIT License Classifier: Natural Language :: English
 Classifier: Programming Language :: Python Classifier: Programming Language ::
 Python :: 3 Classifier: Programming Language :: Python :: 3.8 Classifier:
 Programming Language :: Python :: 3.9 Classifier: Programming Language ::
 Python :: 3.10 Classifier: Programming Language :: Python :: 3.11 Classifier:
 Topic :: Scientific/Engineering Classifier: Topic :: Scientific/Engineering ::
```

### Comparing `veilcord-0.0.7.4/README.md` & `veilcord-0.0.7.5/README.md`

 * *Files identical despite different names*

### Comparing `veilcord-0.0.7.4/setup.py` & `veilcord-0.0.7.5/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 #! /usr/bin/env python
 
 from setuptools import setup, find_packages
 
-vers = "0.0.7.4"
+vers = "0.0.7.5"
 
 setup(
     name="veilcord",
     version=vers,
     description="VeilCord // @imvast",
     long_description_content_type="text/markdown",
     long_description=open("README.md", encoding="utf-8").read(),
     packages=[
         "veilcord",
-        "veilcord.types",
+        "veilcord.models",
     ],  # find_packages(exclude=["tests"], include=["types"]),
     author="@imvast",
     url=f"http://pypi.python.org/pypi/veilcord",
     author_email="dev@vast.sh",
     license="MIT",
     classifiers=[
         "Development Status :: 3 - Alpha",
@@ -35,15 +35,15 @@
         "Topic :: Scientific/Engineering :: Visualization",
         "Topic :: Software Development :: Libraries",
         "Topic :: Utilities",
     ],
     project_urls={
         "Homepage": "https://github.com/imvast",
         "Suggestions": "https://github.com/imvast/veilcord/issues",
-        "Support": "https://discord.gg/vast",
+        "Support": "https://t.me/skiddos",
     },
     python_requires="~=3.8",
     install_requires=[
         "terminut>=0.0.0.901",
         "colorama>=0.4.6",
         "requests>=2.30.0",
         "httpx>=0.25.0",
```

### Comparing `veilcord-0.0.7.4/veilcord/__init__.py` & `veilcord-0.0.7.5/veilcord/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 __author__ = "github.com/imvast"
 __title__ = "VeilCord"
-__version__ = "0.0.7.4"
+__version__ = "0.0.7.5"
 
 from .__main__ import *
 from .__solver__ import *
+from .__udcord__ import *
 
 from os import system
 from sys import executable
 from terminut import printf as print
 from requests import get
 
 try:
```

### Comparing `veilcord-0.0.7.4/veilcord/__main__.py` & `veilcord-0.0.7.5/veilcord/__main__.py`

 * *Files 7% similar despite different names*

```diff
@@ -3,25 +3,24 @@
 """
 @Author: github.com/imvast
 @Date: 7/31/2023
 """
 
 from .__session__ import SessionManager
 
-from base64 import b64encode
+from re2 import search, findall
 from json import dumps
-from tls_client import Session
+from httpx import AsyncClient
+from base64 import b64encode
 from typing import Optional, Literal, List, Union, Tuple
-from json import dumps
-from .types.websocket import ReadyData
-from requests import get
-from re2 import search, findall
 from asyncio import run, gather
-from httpx import AsyncClient
-from .types.device import AgentProperties, DiscordProperties, Agents
+from requests import get
+from tls_client import Session
+from .models.device import AgentProperties, DiscordProperties, Agents
+from .models.dynamic import DataObject
 
 
 # def timeit(func): # debugging
 #     def wrapper(*args, **kwargs):
 #         start_time = time()
 #         result = func(*args, **kwargs)
 #         end_time = time()
@@ -30,73 +29,78 @@
 #         return result
 #     return wrapper
 
 
 class HTTPClient:
     def __init__(self):
         self.session = Session(
-            client_identifier="firefox_119", random_tls_extension_order=True
+            client_identifier="firefox_120", random_tls_extension_order=True
         )
 
 
 class VeilCord:
     def __init__(
         self,
         session: Optional[Session] = HTTPClient().session,
         device_type: Literal["browser", "mobile", "app"] = "browser",
         user_agent: Optional[str] = None,
         device_version: Optional[str] = None,
         build_num: Optional[int] = None,
     ) -> None:
         self.session = HTTPClient().session if session is None else session
         self.currentBuildNUM = VeilCord.getBuildNum() if not build_num else build_num
+        self.nativeBuildNum = VeilCord.getNativeBuildNum()
         self.currentCapNum = VeilCord.getCapabilitiesNum()
         self.device_type = device_type
-        
+
         if device_type == "browser":
             self.agent = Agents.Browser()
         elif device_type == "mobile":
             self.agent = Agents.Mobile()
         elif device_type == "app":
             self.agent = Agents.Desktop()
         else:
             raise ValueError(
                 "An invalid device_type was provided. Acceptable values: ['browser', 'mobile', 'app']"
             )
-            
+
         self.user_agent = self.agent.user_agent if user_agent is None else user_agent
 
         try:
-            self.browser, self.bversion = AgentProperties.extract_browser(self.user_agent)
+            self.browser, self.bversion = AgentProperties.extract_browser(
+                self.user_agent
+            )
         except:
             self.browser = "Firefox"
-            self.bversion = device_version if device_version else "119.0"
+            self.bversion = device_version if device_version else "120.0"
 
     # session mg
 
     def openSession(self, custom_rpc: dict = None) -> SessionManager:
         return SessionManager(
             self.user_agent,
             self.currentBuildNUM,
+            self.nativeBuildNum,
             self.device_type,
             self.currentCapNum,
             custom_rpc,
         )
 
     def getSession(
         self,
         token: str,
         session: SessionManager = None,
         keep_alive: bool = False,
         show_hb: bool = False,
-    ) -> Tuple[ReadyData, Union[str, None]]:
+    ) -> Tuple[DataObject, Union[str, None]]:
         if session is None:
             session = SessionManager(
                 self.user_agent,
                 self.currentBuildNUM,
+                self.nativeBuildNum,
                 self.device_type,
                 self.currentCapNum,
             )
             if keep_alive:
                 raise SyntaxError("Session cannot be null with keepAlive enabled.")
         ready_data, session_id = run(session.get_session(token, keep_alive, show_hb))
         return ready_data, session_id
@@ -110,15 +114,14 @@
     ):
         xsup_common = {
             "os": self.agent.device_type,
             "system_locale": "en-US",
             "browser_user_agent": self.user_agent,
             "browser_version": self.bversion,
             "browser": "",
-            "device": "",
             "release_channel": "stable",
             "client_build_number": build_num if build_num else self.currentBuildNUM,
         }
         if self.device_type == "mobile":
             xsup = {
                 "os": self.agent.device_type,
                 "browser": "Discord Android",
@@ -130,38 +133,43 @@
                 "os_version": "31",
                 "client_build_number": 1750160087099,
             }
         elif self.device_type == "browser":
             xsup = {
                 **xsup_common,
                 "browser": self.browser,
+                "device": "",
                 "os_version": "10",
+                "referrer": "",
+                "referring_domain": "",
+                "referrer_current": "",
+                "referring_domain_current": "",
             }
         elif self.device_type == "app":
+            self.agent: Agents.Desktop
             xsup = {
                 **xsup_common,
                 "browser": self.browser,
-                "client_version": browser_vers if browser_vers else "1.0.9023",
-                "os_version": "10.0.22621",
+                "client_version": browser_vers if browser_vers else self.agent.Xsup.client_version,
+                "os_version": self.agent.Xsup.os_version,
                 "os_arch": "x64",
-                "browser_version": "22.3.2",
-                "native_build_number": 35236,
+                "app_arch": "ia32",
+                "browser_version": "22.3.26",
+                "native_build_number": self.nativeBuildNum,
             }
         else:
             raise ValueError(
                 "An invalid type for generateXProp() was provided. Acceptable values: ['browser', 'mobile', 'app']"
             )
 
         xsup["client_event_source"] = None
-        xsup["referrer"] = ""
-        xsup["referring_domain"] = ""
-        xsup["referrer_current"] = ""
-        xsup["referring_domain_current"] = ""
 
-        return b64encode(dumps(dict(sorted(xsup.items())), separators=(",", ":")).encode()).decode()
+        return b64encode(
+            dumps(dict(sorted(xsup.items())), separators=(",", ":")).encode()
+        ).decode()
 
     def getFingerprint(
         self,
         xsup: Optional[str] = None,
         withCookies: Optional[bool] = True,
         cookieType: Literal["json", "cookiejar"] = "cookiejar",
         custom_headers: dict = None,
@@ -256,39 +264,43 @@
                 return BUILD_NUM
         except:
             pass
 
     @staticmethod
     def getBuildNum() -> int:
         """
-        Fetches the current discord build number. 
-        - Currently takes about 1.2 seconds.
+        Fetches the current discord build number.
+        - Currently takes about 0.9 seconds.
 
         Returns:
             int: The current build number
         """
+
         async def async_getBuildNum():
             try:
                 async with AsyncClient() as session:
                     res = await session.get("https://discord.com/login")
                     res.raise_for_status()
                     matches = list(
                         reversed(findall(r'<script src="([^"]+)"[^>]*>', res.text))
                     )
 
-                    tasks = [VeilCord.fetch_build_num(session, match) for match in matches]
+                    tasks = [
+                        VeilCord.fetch_build_num(session, match) for match in matches
+                    ]
                     results = await gather(*tasks)
 
                     for result in results:
                         if result is not None:
                             return result
 
                     return 245033
             except:
                 return 245033
+
         return run(async_getBuildNum())
 
     @staticmethod
     def getCapabilitiesNum() -> int:
         return 16381
         try:
             cookie = {
@@ -305,14 +317,30 @@
             cappattern = r"capabilities:(\d+)"
             match = search(cappattern, script_content)
 
             return int(match.group(1)) if match else 16381
         except:
             return 16381  # last known
 
+    @staticmethod
+    def getNativeBuildNum() -> int:
+        return int(
+            get(
+                "https://updates.discord.com/distributions/app/manifests/latest",
+                params={
+                    "install_id": "0",
+                    "channel": "stable",
+                    "platform": "win",
+                    "arch": "x86",
+                },
+                headers={"user-agent": "Discord-Updater/1", "accept-encoding": "gzip"},
+            ).json()["metadata_version"]
+        )
+
+    @staticmethod
     def extractCode(invite) -> Union[str, None]:
         """Extracts the invite code from a Discord invite link"""
         code_regex = r"(?:(?:http:\/\/|https:\/\/)?discord\.gg\/|discordapp\.com\/invite\/|discord\.com\/invite\/)?([a-zA-Z0-9-]+)"
         match = search(code_regex, invite)
         if match:
             try:
                 return match.group(1)
```

### Comparing `veilcord-0.0.7.4/veilcord/__session__.py` & `veilcord-0.0.7.5/veilcord/__session__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,20 +1,22 @@
 from websocket import WebSocket, WebSocketConnectionClosedException
-from json import dumps, loads
 from terminut import printf as print
 from asyncio import sleep, create_task
+from typing import Tuple
+from json import dumps, loads
 from re import search
-from .types.websocket import ReadyData, D_Data
+from .models.dynamic import DataObject
 
 
 class SessionManager:
     def __init__(
         self,
         user_agent,
         build_num,
+        native_buildnum,
         device_type,
         capabilities_num,
         cst_presence: dict = None,
     ):
         self.session_id = None
         self.session_task = None
         self.session_on = False
@@ -29,14 +31,15 @@
             "Sec-WebSocket-Extensions": "permessage-deflate",
             "User-Agent": user_agent,
         }
         self.ws = WebSocket()
 
         self.user_agent = user_agent
         self.build_num = build_num
+        self.native_buildnum = native_buildnum
         self.device_type = device_type
         self.capabilities_num = capabilities_num
         self.custom_presence = cst_presence
         browser_patterns = {
             "Discord Client": r"discord/([\d.]+)",
             "Chrome": r"Chrome/([\d.]+)",
             "Firefox": r"Firefox/([\d.]+)",
@@ -47,15 +50,15 @@
 
         for browser, pattern in browser_patterns.items():
             match = search(pattern, user_agent)
             if match:
                 self.browser = browser
                 self.bversion = match.group(1)
 
-    async def _wsconn(self, token) -> [ReadyData, str]:
+    async def _wsconn(self, token) -> Tuple[DataObject, str]:
         self.ws.connect(
             "wss://gateway.discord.gg/?encoding=json&v=9", header=self.socket_headers
         )
         message = {
             "op": 2,
             "d": {
                 "token": token,
@@ -65,29 +68,31 @@
                     "browser_user_agent": self.user_agent,
                     "device": "",
                     "system_locale": "en-US",
                     "release_channel": "stable",
                     "client_build_number": self.build_num,
                     "client_event_source": None,
                 },
-                "presence": {
-                    "status": "online",
-                    "since": 0,
-                    "activities": [
-                        {
-                            "name": "Custom Status",
-                            "type": 4,
-                            "state": "made by @imvast",
-                            "emoji": "",
-                        }
-                    ],
-                    "afk": False,
-                }
-                if not self.custom_presence
-                else self.custom_presence,
+                "presence": (
+                    {
+                        "status": "online",
+                        "since": 0,
+                        "activities": [
+                            {
+                                "name": "Custom Status",
+                                "type": 4,
+                                "state": "made by @imvast",
+                                "emoji": "",
+                            }
+                        ],
+                        "afk": False,
+                    }
+                    if not self.custom_presence
+                    else self.custom_presence
+                ),
                 "compress": False,
                 "client_state": {
                     "guild_versions": {},
                     "highest_last_message_id": "0",
                     "read_state_version": 0,
                     "user_guild_settings_version": -1,
                     "user_settings_version": -1,
@@ -104,34 +109,34 @@
             message["d"]["properties"]["referrer"] = ("",)
             message["d"]["properties"]["referring_domain"] = ("",)
             message["d"]["properties"]["referrer_current"] = ("",)
             message["d"]["properties"]["referring_domain_current"] = ("",)
         elif self.device_type == "app":
             message["d"]["properties"]["browser"] = "Discord Client"
             message["d"]["properties"]["browser_version"] = "22.3.2"
-            message["d"]["properties"]["client_version"] = "1.0.9015"
-            message["d"]["properties"]["os_version"] = "10.0.22621"
+            message["d"]["properties"]["client_version"] = "1.0.9033"
+            message["d"]["properties"]["os_version"] = "10.0.22631"
             message["d"]["properties"]["os_arch"] = "x64"
-            message["d"]["properties"]["native_build_number"] = 32266
-        # elif self.device_type == "mobile":
-        #     message["d"]["properties"] = {
-        #         "os": "iOS",
-        #         "browser": "Discord iOS",
-        #         "device": "iPhone14,5",
-        #         "system_locale": "en-US",
-        #         "client_version": "202.0",
-        #         "release_channel": "stable",
-        #         "device_vendor_id": "",
-        #         "browser_user_agent": "",
-        #         "browser_version": "",
-        #         "os_version": "17.0",
-        #         "client_build_number": 51852,
-        #         "client_event_source": None,
-        #         "design_id": 0
-        #     }
+            message["d"]["properties"]["native_build_number"] = 43813
+        elif self.device_type == "mobile":
+            message["d"]["properties"] = {
+                "os": "iOS",
+                "browser": "Discord iOS",
+                "device": "iPhone14,5",
+                "system_locale": "en-US",
+                "client_version": "202.0",
+                "release_channel": "stable",
+                "device_vendor_id": "",
+                "browser_user_agent": "",
+                "browser_version": "",
+                "os_version": "17.0",
+                "client_build_number": 51852,
+                "client_event_source": None,
+                "design_id": 0,
+            }
 
         else:
             raise ValueError(
                 "An invalid device_type was provided for getSession() | Acceptable values: ['browser', 'app']"
             )
 
         self.ws.send(dumps(message))
@@ -149,32 +154,34 @@
                     },
                 }
             )
         )
         READY_DATA = "unfetched"
         for _ in range(5):
             try:
-                result = loads(self.ws.recv())
+                result: dict = loads(self.ws.recv())
             except WebSocketConnectionClosedException as e:
                 return "invalid token", "invalid token"
             except:
                 continue
-            
+
             if result.get("op") == 9:
                 print("Invalid token provided.")
                 self.ws.close()
                 return None, "Invalid token"
-                
+
             if result.get("t") == "READY":
-                READY_DATA = ReadyData(
-                    t=result.get("t"),
-                    s=result.get("s"),
-                    op=result.get("op"),
-                    d=D_Data(**result.get("d")),
-                )
+                # print(result)
+                # READY_DATA = ReadyData(
+                #     t=result.get("t"),
+                #     s=result.get("s"),
+                #     op=result.get("op"),
+                #     d=D_Data(**result.get("d")),
+                # )
+                READY_DATA = DataObject(result)
             if "heartbeat_interval" in dumps(result):
                 self.rpBeat = result["d"].get("heartbeat_interval")
             if "session_id" in dumps(result):
                 self.session_id = result["d"].get("session_id")
                 break
         return READY_DATA, self.session_id
 
@@ -187,15 +194,15 @@
                 await sleep(self.rpBeat / 1000)
             except Exception as e:
                 print(f"(!) Error sending HB: {e}")
                 break
 
     async def get_session(
         self, token: str, keep_alive: bool = False, show_hb: bool = False
-    ) -> [ReadyData, str]:
+    ) -> Tuple[DataObject, str]:
         try:
             ready_data, session_id = await self._wsconn(token)
             if keep_alive:
                 # print("[WARN] KeepAlive is experimental.", showTimestamp=False)
                 self.session_on = True
                 self.session_task = create_task(self.keepSessionAlive(show_hb))
                 return ready_data, session_id
@@ -205,14 +212,13 @@
             if self.session_on:
                 self.session_on = False  # Stop the keep-alive loop
                 await self.session_task  # Wait for the task to complete
             return
 
     def get_active_ws(self):
         return self.ws
-        
 
     def close_session(self):
         self.session_on = False
         if self.session_task is None:
             return print("(!) Cannot close an unopened session.")
         self.session_task.cancel()
```

### Comparing `veilcord-0.0.7.4/veilcord/__solver__.py` & `veilcord-0.0.7.5/veilcord/__solver__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,124 +1,125 @@
 import time
 import requests
 from terminut import log
 from typing import Dict
 from enum import Enum
 
 
-class CaptchaService(Enum):
+class Services(Enum):
     CAPSOLVER = "https://api.capsolver.com"
     ANTICAPTCHA = "https://api.anti-captcha.com"
     CAPBYPASS = "https://api.capbypass.com"
     CAPMONSTER = "https://api.capmonster.cloud"
-    HCOPTCHA = "https://api.hcoptcha.online/api"
+    HCOPTCHA = "https://api.hcoptcha.com/api"
     CAPGURU = "http://api.captcha.guru"
     _24CAP = "https://24captcha.online"
     DORTCAP = "https://api.dortware.club"
-    AB5CAP = "ab5solver"
+    DEXVCAP = "http://api.dexv.lol"
+
+    @staticmethod
+    def get_services():
+        return {service.name: service.value for service in Services}
 
 
-class CaptchaSolver:
+class Solver:
     def __init__(
         self,
         session: requests.Session,
         service: str = "CAPSOLVER",
         cap_key: str = None,
         site_key: str = "4c672d35-0701-42b2-88c3-78380b0db560",
         site_url: str = "https://discord.com",
         rq_data: str = None,
-        user_agent: str = "Mozilla/5.0 (Windows NT 10.0; Win64; x64; rv:109.0) Gecko/20100101 Firefox/119.0",
+        user_agent: str = "Mozilla/5.0 (Windows NT 10.0; Win64; x64; rv:109.0) Gecko/20100101 Firefox/122.0",
     ):
         if not cap_key:
             raise ValueError("A captcha service key is required to solve the captcha.")
 
         self.session = session
-        self.service = CaptchaService[service]
+        self.service = Services[service]
         self.cap_key = cap_key
         self.site_key = site_key
         self.site_url = (
             site_url if site_url.startswith("http") else f"https://{site_url}"
         )
         self.rq_data = rq_data
         self.user_agent = user_agent
 
     def solve_captcha(self) -> str:
         domain = self.service.value
-        
+
         solver_functions = {
-            CaptchaService.HCOPTCHA: self.solve_hcop,
-            CaptchaService.DORTCAP: self.dortcap_solver,
-            CaptchaService.AB5CAP: self.ab5solver,
-            CaptchaService.CAPGURU: self.solve_secondary,
-            CaptchaService._24CAP: self.solve_secondary
+            Services.HCOPTCHA: self.solve_hcop,
+            Services.DORTCAP: self.dortcap_solver,
+            Services.CAPGURU: self.solve_secondary,
+            Services._24CAP: self.solve_secondary,
         }
 
         if self.service in solver_functions:
             return solver_functions[self.service](domain)
-        elif "capsolver" in domain:
-            return self.solve_generic(domain, task_type="HCaptchaTurboTask")
         else:
             return self.solve_generic(domain)
 
     def solve_generic(self, domain: str, task_type: str = "HCaptchaTask") -> str:
         try:
             data = {
                 "clientKey": self.cap_key,
                 "task": {
                     "type": task_type,
                     "websiteURL": self.site_url,
                     "websiteKey": self.site_key,
-                    "enterprisePayload": {"rqdata": self.rq_data}
-                    if self.rq_data
-                    else None,
+                    "enterprisePayload": (
+                        {"rqdata": self.rq_data} if self.rq_data else None
+                    ),
                     "userAgent": self.user_agent,
                     "proxy": self.get_proxy_from_session(self.session),
                 },
             }
             resp1 = requests.post(f"{domain}/createTask", json=data)
             if resp1.status_code != 200:
                 raise requests.exceptions.RequestException(
                     f"Request failed with status code: {resp1.status_code}"
                 )
 
             invalid_errs = [
+                "ERROR_WRONG_USER_KEY"
                 "ERROR_KEY_DENIED_ACCESS",
                 "ERROR_KEY_DOES_NOT_EXIST",
                 "ERROR_ZERO_BALANCE",
             ]
             if any(error_name in resp1.text for error_name in invalid_errs):
                 log.error("Invalid Captcha Service Key!")
                 return ""
 
             resp_json = resp1.json()
             if resp_json.get("errorId") == 0:
                 task_id = resp_json.get("taskId")
-                resp = self.wait_and_get_solution(domain, task_id)
+                
+                data = {"clientKey": self.cap_key, "taskId": task_id}
+                res = requests.post(f"{domain}/getTaskResult", json=data)
+                status = res.json().get("status")
+
+                while status == "processing":
+                    time.sleep(1)
+                    res = requests.post(f"{domain}/getTaskResult", json=data)
+                    status = res.json().get("status")
+
+                resp = res.json() if status == "ready" else None
+            
                 if resp:
                     return resp.get("solution").get("gRecaptchaResponse", "")
                 else:
                     return self.solve_generic(domain)
             else:
                 return self.solve_generic(domain)
         except requests.exceptions.RequestException as e:
             log.error(f"Error solving captcha: {e}")
             return ""
 
-    def wait_and_get_solution(self, domain: str, task_id: str) -> Dict:
-        data = {"clientKey": self.cap_key, "taskId": task_id}
-        resp = requests.post(f"{domain}/getTaskResult", json=data)
-        status = resp.json().get("status")
-
-        while status == "processing":
-            time.sleep(1)
-            resp = requests.post(f"{domain}/getTaskResult", json=data)
-            status = resp.json().get("status")
-
-        return resp.json() if status == "ready" else None
-
     def solve_hcop(self, domain: str) -> str:
         try:
             task_type = "hcaptchaEnterprise"
             data = {
                 "api_key": self.cap_key,
                 "task_type": task_type,
                 "data": {
@@ -162,19 +163,25 @@
     def solve_secondary(self, domain: str) -> str:
         try:
             payload = {
                 "key": self.cap_key,
                 "method": "hcaptcha",
                 "sitekey": self.site_key,
                 "pageurl": self.site_url,
-                "userAgent": self.user_agent,
+                "enterprise": True,
                 "json": 1,
             }
             res = requests.post(f"{domain}/in.php", json=payload)
-            if "ERROR_WRONG_USER_KEY" in res.text:
+            invalid_errs = [
+                "ERROR_WRONG_USER_KEY"
+                "ERROR_KEY_DENIED_ACCESS",
+                "ERROR_KEY_DOES_NOT_EXIST",
+                "ERROR_ZERO_BALANCE",
+            ]
+            if any(error_name in res.text for error_name in invalid_errs):
                 log.error("Invalid Captcha Service Key!")
                 return ""
 
             request_id = res.json().get("request")
             resp = self.wait_for_secondary_solution(domain, request_id)
             return resp if resp else ""
         except requests.exceptions.RequestException as e:
@@ -202,36 +209,37 @@
             "site_url": self.site_url,
         }
         res = requests.post(f"{domain}/solve/hcaptcha-pay-per-use", json=payload)
         if token := res.json().get("token"):
             return token
         return self.dortcap_solver(domain)
 
-    def ab5solver(self, domain: str):
+    def solve_nocapai(self, _):
+        apikey = "apikey"
+        token_api = "https://token.nocaptchaai.com/token"
+
+        headers = {"Content-Type": "application/json", "apikey": apikey}
+        payload = {
+            "type": "hcaptcha",
+            "url": self.site_url,
+            "sitekey": self.site_key,
+            "useragent": self.user_agent,
+        }
+
+        response = requests.post(token_api, json=payload, headers=headers).json()
+        time.sleep(5)
+
         while True:
-            payload = {
-                "url": self.site_url,
-                "sitekey": self.site_key,
-                "proxy": self.get_proxy_from_session(self.session),
-            }
-            if self.rq_data != "":
-                payload["rqdata"] = self.rq_data
-            if self.user_agent != "":
-                payload["userAgent"] = self.user_agent
-
-            headers = {"authorization": self.cap_key}
-
-            try:
-                response = requests.get(
-                    "https://api.ab5.wtf/solve", params=payload, headers=headers
-                )
-                if "pass" in response.text:
-                    return response.json()["pass"]
-            except Exception as e:
-                continue
+            sts = requests.get(response["url"], headers=headers).json()
+            if sts["status"] == "processed":
+                return sts["token"]
+            elif sts["status"] == "failed":
+                print("fail to solve dogshit solver nocaptchaiai")
+
+            time.sleep(1)
 
     @staticmethod
     def get_proxy_from_session(session: requests.Session) -> str:
         proxy = session.proxies.get("http")
         if proxy:
             protocol, session_proxy = proxy.split("://")
             user_pass, host_port = (
```

### Comparing `veilcord-0.0.7.4/veilcord/types/device.py` & `veilcord-0.0.7.5/veilcord/models/device.py`

 * *Files 5% similar despite different names*

```diff
@@ -22,23 +22,21 @@
             "Safari": r"Safari/([\d.]+)",
             "Opera": r"OPR/([\d.]+)|Opera/([\d.]+)",
         }
 
         for browser, pattern in browser_patterns.items():
             match = search(pattern, user_agent)
             if match:
-                browser_name = str(browser)
-                browser_version = str(match.group(1))
-                return [browser_name, browser_version]
+                return [browser, str(match.group(1))]
 
-        return ["Firefox", "119.0"]
+        return ["Firefox", "125.0"]
 
 
 class DiscordProperties:
-    build_number: int = 254518
+    BUILD_NUMBER: int = 268356
 
     @dataclass
     class X_Super_Properties:
         os:                  Optional[str] = None
         browser:             Optional[str] = None
         device:              Optional[str] = None
         system_locale:       Optional[str] = None
@@ -46,58 +44,60 @@
         release_channel:     Optional[str] = None
         device_vendor_id:    Optional[str] = None
         os_version:          Optional[str] = None
         client_build_number: Optional[int] = None
         browser_user_agent:  Optional[str] = None
         browser_version:     Optional[str] = None
         os_arch:             Optional[str] = None
+        app_arch:            Optional[str] = None
         native_build_number: Optional[int] = None
 
         def to_dict(self):
-            return {key: value for key, value in asdict(self).items() if value is not None}
+            return {key: value for key, value in asdict(self).items() if value}
 
     @dataclass
     class X_Track(X_Super_Properties):
         build_number: Optional[int] = 9999
 
 class Agents:
     @dataclass
     class Browser:
         device_type: str = "Windows"
-        user_agent: str = "Mozilla/5.0 (Windows NT 10.0; Win64; x64; rv:109.0) Gecko/20100101 Firefox/119.0"
+        user_agent: str = "Mozilla/5.0 (Windows NT 10.0; Win64; x64; rv:122.0) Gecko/20100101 Firefox/122.0"
         browser_name, browser_version = AgentProperties.extract_browser(user_agent)
 
         Xsup = DiscordProperties.X_Super_Properties(
             os=device_type,
             browser=browser_name,
             device="",
             system_locale="en-US",
             browser_user_agent=user_agent,
             browser_version=browser_version,
             os_version="10",
             release_channel="stable",
-            client_build_number=str(DiscordProperties.build_number),
+            client_build_number=str(DiscordProperties.BUILD_NUMBER),
         )
 
     @dataclass
     class Desktop:
-        user_agent: str = "Mozilla/5.0 (Windows NT 10.0; WOW64) AppleWebKit/537.36 (KHTML, like Gecko) discord/1.0.9025 Chrome/108.0.5359.215 Electron/22.3.12 Safari/537.36"
+        user_agent: str = "Mozilla/5.0 (Windows NT 10.0; WOW64) AppleWebKit/537.36 (KHTML, like Gecko) discord/1.0.9034 Chrome/108.0.5359.215 Electron/22.3.26 Safari/537.36"
         device_type = "Windows"
         Xsup = DiscordProperties.X_Super_Properties(
             os=device_type,
             browser="Discord Client",
             release_channel="stable",
-            client_version="1.0.9025",
-            os_version="10.0.22621",
+            client_version="1.0.9034",
+            os_version="10.0.22631",
             os_arch="x64",
+            app_arch="ia32",
             system_locale="en-US",
             browser_user_agent=user_agent,
-            browser_version="22.3.2",
-            client_build_number=str(DiscordProperties.build_number),
-            native_build_number=35236,
+            browser_version="22.3.26", # Electron version
+            client_build_number=str(DiscordProperties.BUILD_NUMBER),
+            native_build_number=44142,
         )
 
     @dataclass
     class Mobile:
         user_agent_mobile = "Discord-Android/170014;RNA"
         device_type: str = "Android"
```

### Comparing `veilcord-0.0.7.4/veilcord.egg-info/PKG-INFO` & `veilcord-0.0.7.5/veilcord.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: veilcord
-Version: 0.0.7.4
+Version: 0.0.7.5
 Summary: VeilCord // @imvast
 Home-page: http://pypi.python.org/pypi/veilcord
 Author: @imvast
 Author-email: dev@vast.sh
 License: MIT
 Project-URL: Homepage, https://github.com/imvast
 Project-URL: Suggestions, https://github.com/imvast/veilcord/issues
-Project-URL: Support, https://discord.gg/vast
+Project-URL: Support, https://t.me/skiddos
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
```

#### html2text {}

```diff
@@ -1,12 +1,12 @@
-Metadata-Version: 2.1 Name: veilcord Version: 0.0.7.4 Summary: VeilCord /
+Metadata-Version: 2.1 Name: veilcord Version: 0.0.7.5 Summary: VeilCord /
 / @imvast Home-page: http://pypi.python.org/pypi/veilcord Author: @imvast
 Author-email: dev@vast.sh License: MIT Project-URL: Homepage, https://
 github.com/imvast Project-URL: Suggestions, https://github.com/imvast/veilcord/
-issues Project-URL: Support, https://discord.gg/vast Classifier: Development
+issues Project-URL: Support, https://t.me/skiddos Classifier: Development
 Status :: 3 - Alpha Classifier: Intended Audience :: Developers Classifier:
 License :: OSI Approved :: MIT License Classifier: Natural Language :: English
 Classifier: Programming Language :: Python Classifier: Programming Language ::
 Python :: 3 Classifier: Programming Language :: Python :: 3.8 Classifier:
 Programming Language :: Python :: 3.9 Classifier: Programming Language ::
 Python :: 3.10 Classifier: Programming Language :: Python :: 3.11 Classifier:
 Topic :: Scientific/Engineering Classifier: Topic :: Scientific/Engineering ::
```

