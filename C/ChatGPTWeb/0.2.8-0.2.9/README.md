# Comparing `tmp/ChatGPTWeb-0.2.8.tar.gz` & `tmp/ChatGPTWeb-0.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ChatGPTWeb-0.2.8.tar", last modified: Thu Jan 25 14:03:18 2024, max compression
+gzip compressed data, was "ChatGPTWeb-0.2.9.tar", last modified: Mon Jan 29 15:33:24 2024, max compression
```

## Comparing `ChatGPTWeb-0.2.8.tar` & `ChatGPTWeb-0.2.9.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0    27643 2024-01-25 14:03:11.689730 ChatGPTWeb-0.2.8/ChatGPTWeb/ChatGPTWeb.py
--rw-r--r--   0        0        0     6394 2024-01-25 14:03:11.689730 ChatGPTWeb-0.2.8/ChatGPTWeb/OpenAIAuth.py
--rw-r--r--   0        0        0       55 2024-01-25 14:03:11.689730 ChatGPTWeb-0.2.8/ChatGPTWeb/__init__.py
--rw-r--r--   0        0        0     2394 2024-01-25 14:03:11.689730 ChatGPTWeb-0.2.8/ChatGPTWeb/__main__.py
--rw-r--r--   0        0        0     7140 2024-01-25 14:03:11.689730 ChatGPTWeb-0.2.8/ChatGPTWeb/api.py
--rw-r--r--   0        0        0    15257 2024-01-25 14:03:11.689730 ChatGPTWeb-0.2.8/ChatGPTWeb/config.py
--rw-r--r--   0        0        0    35149 2024-01-25 14:03:11.689730 ChatGPTWeb-0.2.8/LICENSE
--rw-r--r--   0        0        0    10788 2024-01-25 14:03:11.689730 ChatGPTWeb-0.2.8/README.md
--rw-r--r--   0        0        0      518 2024-01-25 14:03:11.689730 ChatGPTWeb-0.2.8/pyproject.toml
--rw-r--r--   0        0        0    11110 1970-01-01 00:00:00.000000 ChatGPTWeb-0.2.8/PKG-INFO
+-rw-r--r--   0        0        0    28012 2024-01-29 15:33:17.706318 ChatGPTWeb-0.2.9/ChatGPTWeb/ChatGPTWeb.py
+-rw-r--r--   0        0        0     7037 2024-01-29 15:33:17.706318 ChatGPTWeb-0.2.9/ChatGPTWeb/OpenAIAuth.py
+-rw-r--r--   0        0        0       55 2024-01-29 15:33:17.706318 ChatGPTWeb-0.2.9/ChatGPTWeb/__init__.py
+-rw-r--r--   0        0        0     2394 2024-01-29 15:33:17.706318 ChatGPTWeb-0.2.9/ChatGPTWeb/__main__.py
+-rw-r--r--   0        0        0     7349 2024-01-29 15:33:17.706318 ChatGPTWeb-0.2.9/ChatGPTWeb/api.py
+-rw-r--r--   0        0        0    15418 2024-01-29 15:33:17.706318 ChatGPTWeb-0.2.9/ChatGPTWeb/config.py
+-rw-r--r--   0        0        0    35149 2024-01-29 15:33:17.706318 ChatGPTWeb-0.2.9/LICENSE
+-rw-r--r--   0        0        0    10788 2024-01-29 15:33:17.706318 ChatGPTWeb-0.2.9/README.md
+-rw-r--r--   0        0        0      518 2024-01-29 15:33:17.706318 ChatGPTWeb-0.2.9/pyproject.toml
+-rw-r--r--   0        0        0    11110 1970-01-01 00:00:00.000000 ChatGPTWeb-0.2.9/PKG-INFO
```

### Comparing `ChatGPTWeb-0.2.8/ChatGPTWeb/ChatGPTWeb.py` & `ChatGPTWeb-0.2.9/ChatGPTWeb/ChatGPTWeb.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 )
 
 class chatgpt:
     def __init__(self,
                  sessions: list[dict] = [],
                  proxy: typing.Optional[ProxySettings] = None,
                  chat_file: Path = Path("data", "chat_history", "conversation"),
-                 personality: Optional[Personality] = Personality([{"name": "cat", "value": "you are a cat now."}]),
+                 personality: Personality = Personality([{"name": "cat", "value": "you are a cat now."}]),
                  log_status: bool = True,
                  plugin: bool = False,
                  headless: bool = True,
                  begin_sleep_time: bool = True,
                  arkose_status: bool = False
 
                  ) -> None:
@@ -133,14 +133,21 @@
         """
         mkdir chat file path
         创建聊天文件目录
         """
         self.chat_file.mkdir(parents=True, exist_ok=True)
         session_file_dir = self.chat_file / "sessions"
         session_file_dir.mkdir(parents=True, exist_ok=True)
+        if self.chat_file == Path("data", "chat_history", "conversation"):
+            # 兼容性更新
+            self.conversation_dir = self.chat_file
+        else:
+            # 规范性更新
+            self.conversation_dir = self.chat_file / "conversation"
+            self.conversation_dir.mkdir(parents=True, exist_ok=True)
         self.cc_map = self.chat_file.joinpath("map.json")
         self.cc_map.touch()
         if not self.cc_map.stat().st_size:
             self.cc_map.write_text("{}")
 
     async def __keep_alive__(self, session: Session):
         url = url_check
@@ -245,15 +252,15 @@
         await asyncio.gather(*auth_tasks)
         # load page
         load_tasks += [self.load_page(session) for session in self.Sessions if session.status == Status.Login.value]
         await asyncio.gather(*load_tasks)
 
         self.manage["browser_contexts"] = self.browser.contexts
 
-        self.personality.read_data() # type: ignore
+        self.personality.read_data(self.chat_file) # type: ignore
         self.manage["start"] = True
         self.logger.info("start!")
         self.thread = threading.Thread(target=lambda: self.tmp(loop), daemon=True)
         self.thread.start()
 
     async def load_page(self, session: Session):
         '''start page | 载入初始页面'''
@@ -396,15 +403,15 @@
         if msg_data.status:
             await self.save_chat(msg_data, context_num)
         return msg_data
         
     async def save_chat(self, msg_data: MsgData, context_num: str):
         """save chat file
         保存聊天文件"""
-        path = self.chat_file / msg_data.conversation_id
+        path = self.conversation_dir / msg_data.conversation_id
         path.touch()
         if not path.stat().st_size:
             tmp = {
                 "conversation_id": msg_data.conversation_id,
                 "message": [{
                     "input": msg_data.msg_send,
                     "output": msg_data.msg_recv,
@@ -432,15 +439,15 @@
             map_tmp[str(context_num)] = []
             map_tmp[str(context_num)].append(msg_data.conversation_id)
             self.cc_map.write_text(json.dumps(map_tmp))
 
     async def load_chat(self, msg_data: MsgData):
         """load chat file
         读取聊天文件"""
-        path = self.chat_file.joinpath(msg_data.conversation_id)
+        path = self.conversation_dir.joinpath(msg_data.conversation_id)
         path.touch()
         if not path.stat().st_size:
             # self.logger.warning(f"不存在{msg_data.conversation_id}历史记录文件")
             return {
                 "conversation_id": msg_data.conversation_id,
                 "message": []
             }
@@ -614,15 +621,15 @@
         """
         personality = {"name":"cat1","value":"you are a cat now1."}
 
         add personality,please input json just like this.
         添加人格 ,请传像这样的json数据
         """
         self.personality.add_dict_to_list(personality) # type: ignore
-        self.personality.flush_data() # type: ignore
+        self.personality.flush_data(self.chat_file) # type: ignore
 
     async def show_personality_list(self):
         """show_personality_list
         展示人格列表"""
         return self.personality.show_name() # type: ignore
 
     async def del_personality(self, name: str):
```

### Comparing `ChatGPTWeb-0.2.8/ChatGPTWeb/OpenAIAuth.py` & `ChatGPTWeb-0.2.9/ChatGPTWeb/OpenAIAuth.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 # Credits to github.com/rawandahmad698/PyChatGPT
 import asyncio
 from logging import Logger
 import re
-from typing import Literal, Optional
+from typing import Literal
 import urllib.parse
 from playwright.async_api import Route as ARoute, Request as ARequest
 from playwright.async_api import Page as APage
 from playwright.async_api import BrowserContext
 from playwright.async_api import Response
 from playwright_stealth import stealth_async
 
+from .config import url_check
 
 class Error(Exception):
     """
     Base error class
     """
 
     location: str
@@ -34,15 +35,15 @@
     def __init__(
             self,
             email: str,
             password: str,
             page: "APage",
             logger: Logger,
             browser_contexts,
-            mode: Optional[Literal["openai", "google", "microsoft"]] = "openai",
+            mode: Literal["openai", "google", "microsoft"] = "openai",
             loop=None
     ):
         self.email_address = email
         self.password = password
         self.page = page
         self.logger = logger
         self.browser_contexts = browser_contexts
@@ -154,28 +155,40 @@
         try:
             await self.login_page.wait_for_url("https://chat.openai.com/")
         except Exception as e:
             self.logger.warning(e)
             # Try Again
             await self.login_page.wait_for_url("https://chat.openai.com/")
 
+        async with self.login_page.expect_response(url_check, timeout=20000) as a:
+            res = await self.login_page.goto(url_check, timeout=20000)
+        res = await a.value
+        if res.status == 200 and res.url == url_check:
+            await asyncio.sleep(3)
+            await self.login_page.wait_for_load_state('load')
+            json_data = await self.login_page.evaluate(
+                '() => JSON.parse(document.querySelector("body").innerText)')
+            access_token = json_data['accessToken']
+            return access_token
+        return None
     
 
 
     async def get_session_token(self):
         self.login_page = await self.browser_contexts.new_page()
         await stealth_async(self.login_page)
+        access_token = None
         try:
-            await self.normal_begin()
+            access_token = await self.normal_begin()
         except Exception as e:
             self.logger.warning(f"save screenshot {self.email_address}_login_error.png,login error:{e}")
             await self.login_page.screenshot(path=f"{self.email_address}_login_error.png")
         finally:
             cookies = await self.browser_contexts.cookies()
             await self.login_page.close()
             
         try:
-            return next(filter(lambda x: x.get("name") == "__Secure-next-auth.session-token", cookies), None)
+            return next(filter(lambda x: x.get("name") == "__Secure-next-auth.session-token", cookies), None),access_token
         except Exception as e:
             self.logger.warning(f"get cookie error:{e}")
         
-        return None
+        return None,None
```

### Comparing `ChatGPTWeb-0.2.8/ChatGPTWeb/__main__.py` & `ChatGPTWeb-0.2.9/ChatGPTWeb/__main__.py`

 * *Files identical despite different names*

### Comparing `ChatGPTWeb-0.2.8/ChatGPTWeb/api.py` & `ChatGPTWeb-0.2.9/ChatGPTWeb/api.py`

 * *Files 3% similar despite different names*

```diff
@@ -107,14 +107,17 @@
             if cookie:
                 session.session_token = SetCookieParam(
                     url="https://chat.openai.com",
                     name="__Secure-next-auth.session-token",
                     value=cookie["value"] # type: ignore
                 ) # type: ignore
                 update_session_token(session,chat_file,logger)
+            else:
+                # no session-token,re login
+                session.status = Status.Update.value
             token = await res.json()
             if "error" in token and session.status != Status.Logingin.value:
                 session.status = Status.Update.value
 
         else:
             logger.error(f"flush {session.email} cf cookie error!")
     else:
@@ -128,17 +131,18 @@
         auth = AsyncAuth0(email=session.email, password=session.password, page=session.page, # type: ignore
                             mode=session.mode,
                             browser_contexts=session.browser_contexts,
                             logger=logger,
                             # loop=self.browser_event_loop
                             )
         session.status = Status.Logingin.value
-        t = await auth.get_session_token()
-        if t:
-            session.session_token = t
+        cookie, access_token = await auth.get_session_token()
+        if cookie and access_token:
+            session.session_token = cookie
+            session.access_token = access_token
             session.status = Status.Login.value
             session.login_state = True
             logger.info(f"{session.email} login success")
         else:
             logger.warning(f"{session.email} login error,waiting for next try")
             session.status = Status.Update.value
```

### Comparing `ChatGPTWeb-0.2.8/ChatGPTWeb/config.py` & `ChatGPTWeb-0.2.9/ChatGPTWeb/config.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 import uuid
 import json
 import logging
 from dataclasses import dataclass
 import datetime
 from enum import Enum
 from typing import TypedDict, Optional, Literal, List, Dict
+from pathlib import Path
 import random
 import urllib.parse
 import time
 import base64
 
 from playwright._impl._api_structures import Cookie
 from playwright.async_api import Page, BrowserContext
@@ -39,66 +40,69 @@
     access_token: str = ""
     session_token: Cookie|None = None
     status: str = ""
     login_state: bool = False
     browser_contexts: BrowserContext|None = None
     page: Page|None = None
     type: str = ""
-    mode:Optional[Literal["openai", "google", "microsoft"]] = "openai"
+    mode: Literal["openai", "google", "microsoft"] = "openai"
     last_active: 'datetime.datetime' = datetime.datetime.now()
     input_session_token = session_token
     
     def __post_init__(self):
         if self.input_session_token is None:
             self.input_session_token = self.session_token
 
     @property
     def is_valid(self):
         # TODO::
         return True
 
 
 class Personality:
-    def __init__(self, init_list: List[Dict[str, str]]):
-        self.init_list = []
+    def __init__(self, 
+                 init_list: List[Dict[str, str]] = [],
+                 path = Path() / "data" / "chat_history" / "personality"):
+        self.init_list = init_list
+        self.path = path
         init_list += self.read_data()
         for item in init_list:
             if str(item) not in [str(x) for x in self.init_list]:
                 self.init_list.append(item)
 
     def show_name(self):
         name = [f"{index + 1}. {x.get('name')}" for index, x in enumerate(self.init_list)]
         return '\n'.join(name)
 
-    def get_value_by_name(self, name: str) -> str:
+    def get_value_by_name(self, name: str) -> str|None:
         return next((x.get("value") for x in self.init_list if x.get("name") == name), "")
 
     def add_dict_to_list(self, new_dict: dict):
         self.init_list.append(new_dict)
 
     def save_data(self):
         tmp = '\n'.join([json.dumps(x) for x in self.init_list])
         try:
-            with open("data/chat_history/personality", "w") as f:
+            with open(self.path, "w") as f:
                 f.write(tmp)
         except:
             pass
 
     @classmethod
-    def read_data(self):
+    def read_data(cls,path:str|Path="data/chat_history/personality"):
         try:
-            with open("data/chat_history/personality", "r") as f:
+            with open(path, "r") as f:
                 init_list = [json.loads(x) for x in f.read().split("\n")]
         except:
             init_list = []
         return init_list
 
-    def flush_data(self):
+    def flush_data(self,path: Path):
         self.save_data()
-        self.read_data()
+        self.read_data(path)
 
     def del_data_by_name(self, name: str):
         for item in self.init_list:
             if item.get('name') == name:
                 self.init_list.remove(item)
         self.save_data()
```

### Comparing `ChatGPTWeb-0.2.8/LICENSE` & `ChatGPTWeb-0.2.9/LICENSE`

 * *Files identical despite different names*

### Comparing `ChatGPTWeb-0.2.8/README.md` & `ChatGPTWeb-0.2.9/README.md`

 * *Files identical despite different names*

### Comparing `ChatGPTWeb-0.2.8/pyproject.toml` & `ChatGPTWeb-0.2.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "ChatGPTWeb"
-version = "0.2.8"
+version = "0.2.9"
 description = "ChatGPT PlayWright API"
 authors = [
     { name = "nek0us", email = "nekouss@mail.com" },
 ]
 dependencies = [
     "playwright",
     "aioconsole",
```

### Comparing `ChatGPTWeb-0.2.8/PKG-INFO` & `ChatGPTWeb-0.2.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ChatGPTWeb
-Version: 0.2.8
+Version: 0.2.9
 Summary: ChatGPT PlayWright API
 License: GPL3
 Author-email: nek0us <nekouss@mail.com>
 Requires-Python: >=3.10
 Project-URL: Homepage, https://github.com/nek0us/ChatGPT
 Project-URL: Repository, https://github.com/nek0us/ChatGPT
 Description-Content-Type: text/markdown
```

