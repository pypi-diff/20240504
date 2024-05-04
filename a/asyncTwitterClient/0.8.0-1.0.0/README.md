# Comparing `tmp/asyncTwitterClient-0.8.0.tar.gz` & `tmp/asyncTwitterClient-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "asyncTwitterClient-0.8.0.tar", last modified: Mon Apr 29 22:09:46 2024, max compression
+gzip compressed data, was "asyncTwitterClient-1.0.0.tar", last modified: Sat May  4 05:47:19 2024, max compression
```

## Comparing `asyncTwitterClient-0.8.0.tar` & `asyncTwitterClient-1.0.0.tar`

### file list

```diff
@@ -1,27 +1,28 @@
-drwxrwxrwx   0        0        0        0 2024-04-29 22:09:46.390016 asyncTwitterClient-0.8.0/
--rw-rw-rw-   0        0        0    35149 2023-12-12 23:43:05.000000 asyncTwitterClient-0.8.0/LICENSE
--rw-rw-rw-   0        0        0     2293 2024-04-29 22:09:46.389016 asyncTwitterClient-0.8.0/PKG-INFO
--rw-rw-rw-   0        0        0     1441 2024-04-28 20:04:59.000000 asyncTwitterClient-0.8.0/README.md
-drwxrwxrwx   0        0        0        0 2024-04-29 22:09:46.385015 asyncTwitterClient-0.8.0/asyncTwitter/
--rw-rw-rw-   0        0        0        0 2023-11-01 20:45:28.000000 asyncTwitterClient-0.8.0/asyncTwitter/__init__.py
--rw-rw-rw-   0        0        0      185 2024-04-25 20:38:29.000000 asyncTwitterClient-0.8.0/asyncTwitter/__version__.py
--rw-rw-rw-   0        0        0    35054 2023-12-12 23:38:01.000000 asyncTwitterClient-0.8.0/asyncTwitter/account.py
--rw-rw-rw-   0        0        0    48329 2024-04-29 07:04:33.000000 asyncTwitterClient-0.8.0/asyncTwitter/asyncAccount.py
--rw-rw-rw-   0        0        0     8491 2024-04-29 05:50:48.000000 asyncTwitterClient-0.8.0/asyncTwitter/asyncLogin.py
--rw-rw-rw-   0        0        0    43697 2024-04-28 22:43:14.000000 asyncTwitterClient-0.8.0/asyncTwitter/asyncScraper.py
--rw-rw-rw-   0        0        0     8960 2024-04-25 02:06:24.000000 asyncTwitterClient-0.8.0/asyncTwitter/asyncSearch.py
--rw-rw-rw-   0        0        0     8507 2024-04-24 23:41:30.000000 asyncTwitterClient-0.8.0/asyncTwitter/asyncUtil.py
--rw-rw-rw-   0        0        0    33499 2024-04-24 23:41:30.000000 asyncTwitterClient-0.8.0/asyncTwitter/constants.py
--rw-rw-rw-   0        0        0     7022 2023-12-12 23:07:50.000000 asyncTwitterClient-0.8.0/asyncTwitter/login.py
--rw-rw-rw-   0        0        0    34714 2024-04-24 23:41:30.000000 asyncTwitterClient-0.8.0/asyncTwitter/scraper.py
--rw-rw-rw-   0        0        0     6511 2024-04-24 23:43:14.000000 asyncTwitterClient-0.8.0/asyncTwitter/search.py
--rw-rw-rw-   0        0        0     4863 2024-04-28 22:06:48.000000 asyncTwitterClient-0.8.0/asyncTwitter/twoCaptcha.py
--rw-rw-rw-   0        0        0     7679 2024-04-29 00:03:07.000000 asyncTwitterClient-0.8.0/asyncTwitter/util.py
-drwxrwxrwx   0        0        0        0 2024-04-29 22:09:46.388017 asyncTwitterClient-0.8.0/asyncTwitterClient.egg-info/
--rw-rw-rw-   0        0        0     2293 2024-04-29 22:09:46.000000 asyncTwitterClient-0.8.0/asyncTwitterClient.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      594 2024-04-29 22:09:46.000000 asyncTwitterClient-0.8.0/asyncTwitterClient.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-29 22:09:46.000000 asyncTwitterClient-0.8.0/asyncTwitterClient.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       70 2024-04-29 22:09:46.000000 asyncTwitterClient-0.8.0/asyncTwitterClient.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2024-04-29 22:09:46.000000 asyncTwitterClient-0.8.0/asyncTwitterClient.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-29 22:09:46.390016 asyncTwitterClient-0.8.0/setup.cfg
--rw-rw-rw-   0        0        0     1418 2024-04-29 22:09:26.000000 asyncTwitterClient-0.8.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-04 05:47:19.153936 asyncTwitterClient-1.0.0/
+-rw-rw-rw-   0        0        0    35149 2023-12-12 23:43:05.000000 asyncTwitterClient-1.0.0/LICENSE
+-rw-rw-rw-   0        0        0     1127 2024-05-04 05:47:19.152936 asyncTwitterClient-1.0.0/PKG-INFO
+-rw-rw-rw-   0        0        0     2059 2024-05-03 20:58:01.000000 asyncTwitterClient-1.0.0/README.md
+drwxrwxrwx   0        0        0        0 2024-05-04 05:47:19.129937 asyncTwitterClient-1.0.0/asyncTwitter/
+-rw-rw-rw-   0        0        0        0 2023-11-01 20:45:28.000000 asyncTwitterClient-1.0.0/asyncTwitter/__init__.py
+-rw-rw-rw-   0        0        0      185 2024-04-25 20:38:29.000000 asyncTwitterClient-1.0.0/asyncTwitter/__version__.py
+-rw-rw-rw-   0        0        0    35054 2023-12-12 23:38:01.000000 asyncTwitterClient-1.0.0/asyncTwitter/account.py
+-rw-rw-rw-   0        0        0    48819 2024-05-04 05:43:50.000000 asyncTwitterClient-1.0.0/asyncTwitter/asyncAccount.py
+-rw-rw-rw-   0        0        0     8734 2024-04-30 19:48:37.000000 asyncTwitterClient-1.0.0/asyncTwitter/asyncLogin.py
+-rw-rw-rw-   0        0        0    43717 2024-05-03 20:55:49.000000 asyncTwitterClient-1.0.0/asyncTwitter/asyncScraper.py
+-rw-rw-rw-   0        0        0    12252 2024-05-04 05:43:30.000000 asyncTwitterClient-1.0.0/asyncTwitter/asyncSearch.py
+-rw-rw-rw-   0        0        0    10070 2024-05-04 05:43:39.000000 asyncTwitterClient-1.0.0/asyncTwitter/asyncUtil.py
+-rw-rw-rw-   0        0        0    33499 2024-04-24 23:41:30.000000 asyncTwitterClient-1.0.0/asyncTwitter/constants.py
+-rw-rw-rw-   0        0        0     7022 2023-12-12 23:07:50.000000 asyncTwitterClient-1.0.0/asyncTwitter/login.py
+-rw-rw-rw-   0        0        0    34714 2024-04-24 23:41:30.000000 asyncTwitterClient-1.0.0/asyncTwitter/scraper.py
+-rw-rw-rw-   0        0        0     6511 2024-04-24 23:43:14.000000 asyncTwitterClient-1.0.0/asyncTwitter/search.py
+-rw-rw-rw-   0        0        0      451 2024-05-03 20:48:06.000000 asyncTwitterClient-1.0.0/asyncTwitter/test.py
+-rw-rw-rw-   0        0        0     4863 2024-04-28 22:06:48.000000 asyncTwitterClient-1.0.0/asyncTwitter/twoCaptcha.py
+-rw-rw-rw-   0        0        0     9041 2024-05-04 05:43:42.000000 asyncTwitterClient-1.0.0/asyncTwitter/util.py
+drwxrwxrwx   0        0        0        0 2024-05-04 05:47:19.151936 asyncTwitterClient-1.0.0/asyncTwitterClient.egg-info/
+-rw-rw-rw-   0        0        0     1127 2024-05-04 05:47:18.000000 asyncTwitterClient-1.0.0/asyncTwitterClient.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      615 2024-05-04 05:47:19.000000 asyncTwitterClient-1.0.0/asyncTwitterClient.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-04 05:47:18.000000 asyncTwitterClient-1.0.0/asyncTwitterClient.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       70 2024-05-04 05:47:18.000000 asyncTwitterClient-1.0.0/asyncTwitterClient.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2024-05-04 05:47:18.000000 asyncTwitterClient-1.0.0/asyncTwitterClient.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-04 05:47:19.153936 asyncTwitterClient-1.0.0/setup.cfg
+-rw-rw-rw-   0        0        0     1265 2024-05-04 05:46:58.000000 asyncTwitterClient-1.0.0/setup.py
```

### Comparing `asyncTwitterClient-0.8.0/LICENSE` & `asyncTwitterClient-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `asyncTwitterClient-0.8.0/README.md` & `asyncTwitterClient-1.0.0/README.md`

 * *Files 26% similar despite different names*

```diff
@@ -1,16 +1,36 @@
+# THIS PACKAGE + REPO IS UNDER CONSTANT DEVELOPMENT, DO NOT BE SURPRISED IF SOMETHING IS BROKEN. PLEASE REPORT ASAP TO ISSUES IF YOU FIND ANY ISSUES
+
+# HEAVILY RECOMMEND CLONING REPO INSTEAD OF USING PYPI PACKAGE AS LONG AS THIS MESSAGE IS HERE
+
+
 # asyncTwitterClient
 
 Async port of twitter-api-client
 
 ~ of 2024-04-24 this is being maintained as its being used in a project im being paid to maintain ~
 
 MASSIVE Thank you to Trevor Hobenshield @trevorhobenshield for making this!
 All I have done is changed the client to asyncClient 
 
+# Features (almost all are provided in original repo)
+
+```
+tweet (asyncAccount.py)
+reply (with or without images)
+quote (with or without images)
+retweet
+like
+pin tweets
+change user profile bio, username, avatar etc etc
+scrape user data, tweets, followers following etc (asyncScraper)
+search (asyncSearch.py)
+unlock account via arkose captcha solving (2captcha API)
+```
+
 # Key Differences
 
 ```
 supports unlocking account via account.unlockViaArkoseCaptcha()
 linted by ruff
 renames tweet and other functions to asyncTweet asyncReply etc
 all functions must be awaited
@@ -46,8 +66,8 @@
     twitter = AsyncAccount()
     await twitter.asyncAuthenticate(
         cookies={"ct0": "fuefjwegf89ewg9uiwg9", "auth_token": "je09giewg9iwg9j"}
     )
 
 if __name__ == "__main__":
     anyio.run(main)
-```
+```
```

### Comparing `asyncTwitterClient-0.8.0/asyncTwitter/account.py` & `asyncTwitterClient-1.0.0/asyncTwitter/account.py`

 * *Files identical despite different names*

### Comparing `asyncTwitterClient-0.8.0/asyncTwitter/asyncAccount.py` & `asyncTwitterClient-1.0.0/asyncTwitter/asyncAccount.py`

 * *Files 1% similar despite different names*

```diff
@@ -41,15 +41,14 @@
 except Exception:
     from ..asyncTwitter.twoCaptcha import TwoCaptcha
 
 from .asyncLogin import asyncLogin
 from httpx_socks import AsyncProxyTransport
 from urllib import parse
 
-
 class AsyncAccount:
     """The AsyncAccount class is used to interact with the Twitter API.
     It contains account specific methods like tweeting, liking, following, etc.
 
     a = AsyncAccount(debug=True, twoCaptchaApiKey="2CaptchaKey")
     await a.asyncAuthenticate(email="email", password="password", username="username", cookies="cookies.json", proxies="http://)
     await a.asyncTweet("Hello World!")
@@ -86,22 +85,24 @@
         self.v1_api = "https://api.twitter.com/1.1"
         self.v2_api = "https://twitter.com/i/api/2"
         self.logger = self._init_logger(**kwargs)
         self.rate_limits = {}
         self.twoCaptcha = TwoCaptcha(main=self, apiKey=twoCaptchaApiKey)
         self.proxyString = proxies
 
-        if httpxSocks:
+        if httpxSocks and proxies:
             self.proxies = {
                 "transport": AsyncProxyTransport.from_url(proxies),
                 "proxies": None,
             }
         else:
             self.proxies = {"transport": None, "proxies": proxies}
 
+        self.ogProxyString = proxies
+
         # print(f'AsyncAcc Logger: {self.logger}')
 
     async def unlockViaArkoseCaptcha(self) -> dict:
         """
         This method is used to unlock the account via Arkose Captcha.
         Provide the TwoCaptcha API key in the constructor/__init__ to use this method.
 
@@ -360,18 +361,18 @@
 
         self.email = email
         self.username = username
         self.password = password
         self.twitterId = False
         self.twitterRestId = False
         self.cookies = cookies
-
+        self.ogProxyString = proxies
         self.proxyString = proxies
 
-        if httpxSocks:
+        if httpxSocks and proxies:
             self.proxies = {
                 "transport": AsyncProxyTransport.from_url(proxies),
                 "proxies": None,
             }
         else:
             self.proxies = {"transport": None, "proxies": proxies}
 
@@ -1084,26 +1085,30 @@
         password: str,
         session: object,
         cookies: dict,
         **kwargs,
     ):
         # print(f'AsyncAcc Got: {email}, {username}, {password}, {session}, {kwargs}')
 
+        if self.debug:
+            self.logger.debug(f"{Fore.MAGENTA}Validating session with pString: {self.proxyString} selfProxies: {self.proxies} ogProxyString: {self.ogProxyString}{RESET}")
+
         # try validating cookies dict
         if isinstance(cookies, dict) and all(
             cookies.get(c) for c in {"ct0", "auth_token"}
         ):
             _session = AsyncClient(
                 cookies=cookies,
                 follow_redirects=True,
                 http2=True,
                 verify=False,
                 timeout=30,
                 **self.proxies,
             )
+            _session.authDetails = {"username": username, "password": password, "email": email}
             _session._init_with_cookies = True
             _session.headers.update(get_headers(_session))
             # print("Logging with cookies Dict 100%")
             if self.debug:
                 self.logger.debug(
                     f"{GREEN}{self.username} Logged in with cookies dict{RESET}"
                 )
@@ -1115,14 +1120,15 @@
                 cookies=orjson.loads(Path(cookies).read_bytes()),
                 follow_redirects=True,
                 http2=True,
                 verify=False,
                 timeout=30,
                 **self.proxies,
             )
+            _session.authDetails = {"username": username, "password": password, "email": email}
             _session._init_with_cookies = True
             _session.headers.update(get_headers(_session))
             if self.debug:
                 self.logger.debug(
                     f"{GREEN}{self.username} Logged in with cookies file{RESET}"
                 )
             return _session
```

### Comparing `asyncTwitterClient-0.8.0/asyncTwitter/asyncLogin.py` & `asyncTwitterClient-1.0.0/asyncTwitter/asyncLogin.py`

 * *Files 3% similar despite different names*

```diff
@@ -101,15 +101,15 @@
                     "subtask_id": "LoginEnterUserIdentifierSSO",
                     "settings_list": {
                         "setting_responses": [
                             {
                                 "key": "user_identifier",
                                 "response_data": {
                                     "text_data": {
-                                        "result": client.cookies.get("username")
+                                        "result": client.authDetails.get("username")
                                     }
                                 },
                             }
                         ],
                         "link": "next_link",
                     },
                 }
@@ -125,15 +125,15 @@
         "https://api.twitter.com/1.1/onboarding/task.json",
         json={
             "flow_token": client.cookies.get("flow_token"),
             "subtask_inputs": [
                 {
                     "subtask_id": "LoginEnterPassword",
                     "enter_password": {
-                        "password": client.cookies.get("password"),
+                        "password": client.authDetails.get("password"),
                         "link": "next_link",
                     },
                 }
             ],
         },
     )
 
@@ -224,14 +224,16 @@
             )
             return
         client = await asyncSolveConfirmationChallenge(client, **kwargs)
     return client
 
 
 async def asyncLogin(email: str, username: str, password: str, **kwargs) -> AsyncClient:
+    print(f"[{YELLOW}warning{RESET}] Using Proxy: {kwargs.get('proxies')} Transport: {kwargs.get('transport')}")
+    
     client = AsyncClient(
         cookies={
             #"email": email,
             #"username": username,
             #"password": password,
             "guest_token": None,
             "flow_token": None,
@@ -244,12 +246,17 @@
             "x-twitter-client-language": "en",
         },
         follow_redirects=True,
         http2=True,
         verify=False,
         **kwargs
     )
+    client.authDetails = {
+        "email": email,
+        "username": username,
+        "password": password,
+    }
 
     client = await asyncExecuteLoginFlow(client, **kwargs)
     if not client or client.cookies.get("flow_errors") == "true":
         return False
     return client
```

### Comparing `asyncTwitterClient-0.8.0/asyncTwitter/asyncScraper.py` & `asyncTwitterClient-1.0.0/asyncTwitter/asyncScraper.py`

 * *Files 0% similar despite different names*

```diff
@@ -956,15 +956,15 @@
 
         @param room: room id
         @param frequency: granularity of transcript. 1 for real-time, 2 for post-processed or "finalized" transcript
         @return: None
         """
 
         async def get(spaces: list[dict]):
-            client = init_session()
+            client = init_session(proxies=self.proxies)
             chats = await self._get_live_chats(client, spaces)
             await asyncio.gather(*(self._space_listener(c, frequency) for c in chats))
 
         spaces = self.asyncSpaces(rooms=[room])
         # asyncio.run(get(spaces))
         await get(spaces)
```

### Comparing `asyncTwitterClient-0.8.0/asyncTwitter/asyncSearch.py` & `asyncTwitterClient-1.0.0/asyncTwitter/asyncSearch.py`

 * *Files 26% similar despite different names*

```diff
@@ -10,14 +10,16 @@
 from logging import Logger
 from pathlib import Path
 from httpx import AsyncClient
 from .constants import Operation, LOG_CONFIG, GREEN, YELLOW, RESET
 from .asyncLogin import asyncLogin
 from .util import get_headers, find_key, build_params
 from functools import partial
+from colorama import Fore
+from httpx_socks import AsyncProxyTransport
 
 reset = "\x1b[0m"
 colors = [f"\x1b[{i}m" for i in range(31, 37)]
 
 
 class AsyncSearch:
     def __init__(
@@ -35,34 +37,72 @@
 
     async def asyncAuthenticate(
         self,
         email: str = None,
         username: str = None,
         password: str = None,
         session: AsyncClient = None,
+        proxies: str = None,
+        httpxSocks: bool = False,
+        cookies: dict = None,
         **kwargs,
-    ):
+    ) -> AsyncClient:
         """
         This is used to authenticate the account.
 
-        This used to be in __init__ but we can't await in __init__ so we have to do it here.
+        If email:username:pass is provided will attempt to login
+        If cookies ct0&auth_token are provided will attempt to validate the session using cookies.
+
+        Args:
+            email (str): Email of the account.
+            username (str): Username of the account.
+            password (str): Password of the account.
+            session (AsyncClient): Session to use.
+            proxies (str): Proxies to use.
+            cookies (dict): Cookies to use.
+            **kwargs: Additional arguments to pass to the logger.
+
+        Returns:
+            AsyncClient: The session authenticated session
         """
 
         self.email = email
         self.username = username
         self.password = password
         self.twitterId = False
         self.twitterRestId = False
-        self.cookies = kwargs.get("cookies")
-        self.proxies = kwargs.get("proxies")
+        self.cookies = cookies
+        self.ogProxyString = proxies
+        self.proxyString = proxies
+
+        if httpxSocks and proxies:
+            self.proxies = {
+                "transport": AsyncProxyTransport.from_url(proxies),
+                "proxies": None,
+            }
+        else:
+            self.proxies = {"transport": None, "proxies": proxies}
+
+        kwargs.update(**self.proxies)
+
+        # print(f'AsyncAcc Got: {email}, {username}, {password}, {session}, {self.cookies}, {self.proxies}')
 
         self.session = await self._async_validate_session(
-            self.email, self.username, self.password, session, **kwargs
+            email=self.email,
+            username=self.username,
+            password=self.password,
+            session=session,
+            cookies=self.cookies,
+            **kwargs,
         )
 
+        if not self.session:
+            self.logger.error(f"Failed to authenticate account: {self.username}")
+            return None
+
         return self.session
 
     async def asyncRun(
         self,
         queries: list[dict],
         limit: int = math.inf,
         out: str = "data/search_results",
@@ -73,29 +113,34 @@
         processResults = await self.process(queries, limit, out, **kwargs)
         return processResults
 
     async def process(
         self, queries: list[dict], limit: int, out: Path, **kwargs
     ) -> list:
         results = []
-        
+
         async with anyio.create_task_group() as tg:
             for count, query in enumerate(queries):
                 partialPaginate = partial(
-                    self.paginate, query=query, limit=limit, out=out, results=results, **kwargs
+                    self.paginate,
+                    query=query,
+                    limit=limit,
+                    out=out,
+                    results=results,
+                    **kwargs,
                 )
                 tg.start_soon(partialPaginate)
                 if self.debug:
                     self.logger.info(f"Ran {count} search query")
                 continue
-            
+
         return results
 
     async def paginate(
-        self, query: dict, limit: int, out: Path, results:list, **kwargs
+        self, query: dict, limit: int, out: Path, results: list, **kwargs
     ) -> list[dict]:
         params = {
             "variables": {
                 "count": 20,
                 "querySource": "typed_query",
                 "rawQuery": query["query"],
                 "product": query["category"],
@@ -107,19 +152,19 @@
         res = []
         cursor = ""
         total = set()
 
         while True:
             if cursor:
                 params["variables"]["cursor"] = cursor
-            
+
             backoffResults = await self.backoff(
                 lambda: self.get(self.session, params), **kwargs
             )
-            
+
             if not backoffResults:
                 if self.debug:
                     self.logger.debug("Failed to backoff")
                 continue
             data, entries, cursor = backoffResults
             res.extend(entries)
             if len(entries) <= 2 or len(total) >= limit:  # just cursors
@@ -136,15 +181,17 @@
 
     async def get(self, client: AsyncClient, params: dict) -> tuple:
         _, operationQueryID, operationName = Operation.SearchTimeline
         response = await client.get(
             f"https://twitter.com/i/api/graphql/{operationQueryID}/{operationName}",
             params=build_params(params),
         )
-        self.rate_limits[operationName] = {k: int(v) for k, v in response.headers.items() if 'rate-limit' in k}
+        self.rate_limits[operationName] = {
+            k: int(v) for k, v in response.headers.items() if "rate-limit" in k
+        }
         data = response.json()
         if self.debug:
             self.logger.info(f"Rate limits: {self.rate_limits[operationName]}")
         cursor = self.get_cursor(data)
         entries = [
             field
             for key in find_key(data, "entries")
@@ -194,61 +241,116 @@
             # set level of all other loggers to ERROR
             for name in logging.root.manager.loggerDict:
                 if name != logger_name:
                     logging.getLogger(name).setLevel(logging.ERROR)
 
             return logging.getLogger(logger_name)
 
-    @staticmethod
-    async def _async_validate_session(*args, **kwargs):
-        email, username, password, session = args
-
-        # validate credentials
-        if all((email, username, password)):
-            return await asyncLogin(email, username, password, **kwargs)
-
-        # invalid credentials, try validating session
-        if session and all(session.cookies.get(c) for c in {"ct0", "auth_token"}):
-            return session
+    async def _async_validate_session(
+        self,
+        email: str,
+        username: str,
+        password: str,
+        session: object,
+        cookies: dict,
+        **kwargs,
+    ):
+        # print(f'AsyncAcc Got: {email}, {username}, {password}, {session}, {kwargs}')
 
-        # invalid credentials and session
-        cookies = kwargs.get("cookies")
+        if self.debug:
+            self.logger.debug(
+                f"{Fore.MAGENTA}[asyncSearch] Validating session with proxyString: {self.proxyString} selfProxies: {self.proxies} ogProxyString: {self.ogProxyString}{RESET}"
+            )
 
         # try validating cookies dict
         if isinstance(cookies, dict) and all(
             cookies.get(c) for c in {"ct0", "auth_token"}
         ):
-            _session = AsyncClient(cookies=cookies, follow_redirects=True)
+            _session = AsyncClient(
+                cookies=cookies,
+                follow_redirects=True,
+                http2=True,
+                verify=False,
+                timeout=30,
+                **self.proxies,
+            )
+            _session.authDetails = {
+                "username": username,
+                "password": password,
+                "email": email,
+            }
+            _session._init_with_cookies = True
             _session.headers.update(get_headers(_session))
+            # print("Logging with cookies Dict 100%")
+            if self.debug:
+                self.logger.debug(
+                    f"{GREEN}[asyncSearch] {self.username} Logged in with cookies dict{RESET}"
+                )
             return _session
 
         # try validating cookies from file
         if isinstance(cookies, str):
             _session = AsyncClient(
-                cookies=orjson.loads(Path(cookies).read_bytes()), follow_redirects=True
+                cookies=orjson.loads(Path(cookies).read_bytes()),
+                follow_redirects=True,
+                http2=True,
+                verify=False,
+                timeout=30,
+                **self.proxies,
             )
+            _session.authDetails = {
+                "username": username,
+                "password": password,
+                "email": email,
+            }
+            _session._init_with_cookies = True
             _session.headers.update(get_headers(_session))
+            if self.debug:
+                self.logger.debug(
+                    f"{GREEN}[asyncSearch] {self.username} Logged in with cookies file{RESET}"
+                )
             return _session
 
-        raise Exception(
-            "Session not authenticated. "
-            "Please use an authenticated session or remove the `session` argument and try again."
-        )
+        # validate credentials
+        if all((email, username, password)) and not session and not cookies:
+            loginResults = await asyncLogin(email, username, password, **kwargs)
+
+            if not loginResults:
+                return False
+
+            session = loginResults
+
+            session._init_with_cookies = False
+            # print("Logging with user pass 100%")
+            if self.debug:
+                self.logger.debug(
+                    f"{GREEN}{self.username} Logged in with user/pass{RESET}"
+                )
+            return session
+
+        # invalid credentials, try validating session
+        if session and all(session.cookies.get(c) for c in {"ct0", "auth_token"}):
+            session._init_with_cookies = True
+            return session
+
+        return False
 
     def id(self) -> int:
-        """ Get User ID """
+        """Get User ID"""
         if not self.twid:
             potentialTwid = self.session.cookies.get("twid")
-            
+
             if not potentialTwid:
                 raise Exception("Session is missing twid cookie")
-            
+
             self.twid = int(potentialTwid.split("=")[-1].strip().rstrip())
-            
+
         return self.twid
 
     def save_cookies(self, fname: str = None, toFile=True):
-        """ Save cookies to file """
+        """Save cookies to file"""
         cookies = self.session.cookies
         if toFile:
-            Path(f'{fname or cookies.get("username")}.cookies').write_bytes(orjson.dumps(dict(cookies)))
-        return dict(cookies)
+            Path(f'{fname or cookies.get("username")}.cookies').write_bytes(
+                orjson.dumps(dict(cookies))
+            )
+        return dict(cookies)
```

### Comparing `asyncTwitterClient-0.8.0/asyncTwitter/asyncUtil.py` & `asyncTwitterClient-1.0.0/asyncTwitter/asyncUtil.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,37 +1,62 @@
 import random
 import re
 import time
+import string
+
 from logging import Logger
 from pathlib import Path
 from urllib.parse import urlsplit, urlencode, urlunsplit, parse_qs, quote
 
 import orjson
 from httpx import Response, AsyncClient
 
-from .constants import GREEN, MAGENTA, RED, RESET, ID_MAP
+from .constants import GREEN, MAGENTA, RED, RESET, ID_MAP, USER_AGENTS
+
+
+def generate_random_string(length):
+    characters = string.ascii_letters + string.digits
+    return "".join(random.choice(characters) for i in range(length))
+
+
+def randomLivePipelineSession():
+    # 'LivePipeline-Session': '4cc59a77-31a2-4ed0-8246-ada14c86d528',
+
+    return f"{generate_random_string(8)}-{generate_random_string(4)}-{generate_random_string(4)}-{generate_random_string(4)}-{generate_random_string(12)}"
+
+
+def randomTransactionId():
+    x_client_transaction_id = f"{generate_random_string(19)}/{generate_random_string(3)}/{generate_random_string(18)}+{generate_random_string(51)}"
+    return x_client_transaction_id
+
 
 
 async def async_init_session(proxies=None):
-    client = AsyncClient(headers={
-        'authorization': 'Bearer AAAAAAAAAAAAAAAAAAAAANRILgAAAAAAnNwIzUejRCOuH5E6I8xnZz4puTs=1Zv7ttfk8LF81IUq16cHjhLTvJu4FA33AGWWjCpTnA',
-        'user-agent': 'Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/113.0.0.0 Safari/537.36',
-    }, follow_redirects=True, proxies=proxies)
-    r = await client.post('https://api.twitter.com/1.1/guest/activate.json')
+    client = AsyncClient(
+        headers={
+            "authorization": "Bearer AAAAAAAAAAAAAAAAAAAAANRILgAAAAAAnNwIzUejRCOuH5E6I8xnZz4puTs=1Zv7ttfk8LF81IUq16cHjhLTvJu4FA33AGWWjCpTnA",
+            "user-agent": random.choice(USER_AGENTS),
+        },
+        follow_redirects=True,
+        proxies=proxies,
+    )
+    r = await client.post("https://api.twitter.com/1.1/guest/activate.json")
     r = r.json()
-    client.headers.update({
-        'content-type': 'application/json',
-        'x-guest-token': r['guest_token'],
-        'x-twitter-active-user': 'yes',
-    })
+    client.headers.update(
+        {
+            "content-type": "application/json",
+            "x-guest-token": r["guest_token"],
+            "x-twitter-active-user": "yes",
+        }
+    )
     return client
 
 
 def batch_ids(ids: list[int], char_limit: int = 4_500) -> list[dict]:
-    """ To avoid 431 errors """
+    """To avoid 431 errors"""
     length = 0
     res, batch = [], []
     for x in map(str, ids):
         curr_length = len(x)
         if length + curr_length > char_limit:
             res.append(batch)
             batch = []
@@ -46,91 +71,118 @@
 def build_params(params: dict) -> dict:
     return {k: orjson.dumps(v).decode() for k, v in params.items()}
 
 
 def save_json(r: Response, path: Path, name: str, **kwargs):
     try:
         data = r.json()
-        kwargs.pop('cursor', None)
-        out = path / '_'.join(map(str, kwargs.values()))
+        kwargs.pop("cursor", None)
+        out = path / "_".join(map(str, kwargs.values()))
         out.mkdir(parents=True, exist_ok=True)
-        (out / f'{time.time_ns()}_{name}.json').write_bytes(orjson.dumps(data))
+        (out / f"{time.time_ns()}_{name}.json").write_bytes(orjson.dumps(data))
     except Exception as e:
-        print(f'Failed to save data: {e}')
+        print(f"Failed to save data: {e}")
 
 
 def flatten(seq: list | tuple) -> list:
     flat = []
     for e in seq:
         if isinstance(e, list | tuple):
             flat.extend(flatten(e))
         else:
             flat.append(e)
     return flat
 
 
 def get_json(res: list[Response], **kwargs) -> list:
-    cursor = kwargs.get('cursor')
+    cursor = kwargs.get("cursor")
     temp = res
     if any(isinstance(r, (list, tuple)) for r in res):
         temp = flatten(res)
     results = []
     for r in temp:
         try:
             data = r.json()
             if cursor:
                 results.append([data, cursor])
             else:
                 results.append(data)
         except Exception as e:
-            print('Cannot parse JSON response', e)
+            print("Cannot parse JSON response", e)
     return results
 
 
 def set_qs(url: str, qs: dict, update=False, **kwargs) -> str:
     *_, q, f = urlsplit(url)
-    return urlunsplit((*_, urlencode(qs | parse_qs(q) if update else qs, doseq=True, quote_via=quote,
-                                     safe=kwargs.get('safe', '')), f))
+    return urlunsplit(
+        (
+            *_,
+            urlencode(
+                qs | parse_qs(q) if update else qs,
+                doseq=True,
+                quote_via=quote,
+                safe=kwargs.get("safe", ""),
+            ),
+            f,
+        )
+    )
 
 
 def get_cursor(data: list | dict) -> str:
     # inefficient, but need to deal with arbitrary schema
-    entries = find_key(data, 'entries')
+    entries = find_key(data, "entries")
     if entries:
         for entry in entries.pop():
-            entry_id = entry.get('entryId', '')
-            if ('cursor-bottom' in entry_id) or ('cursor-showmorethreads' in entry_id):
-                content = entry['content']
-                if itemContent := content.get('itemContent'):
-                    return itemContent['value']  # v2 cursor
-                return content['value']  # v1 cursor
+            entry_id = entry.get("entryId", "")
+            if ("cursor-bottom" in entry_id) or ("cursor-showmorethreads" in entry_id):
+                content = entry["content"]
+                if itemContent := content.get("itemContent"):
+                    return itemContent["value"]  # v2 cursor
+                return content["value"]  # v1 cursor
 
 
 def get_headers(session, **kwargs) -> dict:
     """
     Get the headers required for authenticated requests
     """
     cookies = session.cookies
     # todo httpx cookie issues
     try:
         if session._init_with_cookies:
-            cookies.delete('ct0', domain='.twitter.com')
+            cookies.delete("ct0", domain=".twitter.com")
     except Exception:
         ...
-    headers = kwargs | {
-        'authorization': 'Bearer AAAAAAAAAAAAAAAAAAAAANRILgAAAAAAnNwIzUejRCOuH5E6I8xnZz4puTs=1Zv7ttfk8LF81IUq16cHjhLTvJu4FA33AGWWjCpTnA',
-        'cookie': '; '.join(f'{k}={v}' for k, v in cookies.items()),
-        'referer': 'https://twitter.com/',
-        'user-agent': 'Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/113.0.0.0 Safari/537.36',
-        'x-csrf-token': cookies.get('ct0', ''),
-        'x-guest-token': cookies.get('guest_token', ''),
-        'x-twitter-auth-type': 'OAuth2Session' if cookies.get('auth_token') else '',
-        'x-twitter-active-user': 'yes',
-        'x-twitter-client-language': 'en',
-    }
+    headers = (
+        kwargs
+        | {
+            "User-Agent": random.choice(USER_AGENTS),
+            "Accept": "*/*",
+            "Accept-Language": "en-CA,en-US;q=0.7,en;q=0.3",
+            "authorization": "Bearer AAAAAAAAAAAAAAAAAAAAANRILgAAAAAAnNwIzUejRCOuH5E6I8xnZz4puTs=1Zv7ttfk8LF81IUq16cHjhLTvJu4FA33AGWWjCpTnA",
+            "LivePipeline-Session": randomLivePipelineSession(),  #'4cc59a77-31a2-4ed0-8246-ada14c86d528',
+            # "cookie": "; ".join(f"{k}={v}" for k, v in cookies.items()),
+            "Referer": "https://twitter.com/",
+            "x-csrf-token": cookies.get("ct0", ""),
+            "x-guest-token": cookies.get("guest_token", ""),
+            "x-twitter-auth-type": "OAuth2Session" if cookies.get("auth_token") else "",
+            "x-twitter-active-user": "yes",
+            "x-twitter-client-language": "en",
+            "Origin": "https://twitter.com",
+            "DNT": "1",
+            "Sec-GPC": "1",
+            "Sec-Fetch-Dest": "empty",
+            "Sec-Fetch-Mode": "cors",
+            "Sec-Fetch-Site": "same-site",
+            "Connection": "keep-alive",
+            "Pragma": "no-cache",
+            "Cache-Control": "no-cache",
+            # oLYdXdvdHrDENpgQRhn/c2v/cj3SoIX67EyajoIa5y+ZmpxGNKiEFT1WlnSFv1BrQUVHRaFLp1c2Xx1iMaGOeqYgtygDow
+            "x-client-transaction-id": randomTransactionId(),
+        }
+    )
     return dict(sorted({k.lower(): v for k, v in headers.items()}.items()))
 
 
 def find_key(obj: any, key: str) -> list:
     """
     Find all values of a given key within a nested dict or list of dicts
 
@@ -163,86 +215,95 @@
 
     return helper(obj, key, [])
 
 
 def log(logger: Logger, level: int, r: Response):
     def stat(r, txt, data):
         if level >= 1:
-            logger.debug(f'{r.url.path}')
+            logger.debug(f"{r.url.path}")
         if level >= 2:
-            logger.debug(f'{r.url}')
+            logger.debug(f"{r.url}")
         if level >= 3:
-            logger.debug(f'{txt}')
+            logger.debug(f"{txt}")
         if level >= 4:
-            logger.debug(f'{data}')
+            logger.debug(f"{data}")
 
         try:
-            limits = {k: v for k, v in r.headers.items() if 'x-rate-limit' in k}
+            limits = {k: v for k, v in r.headers.items() if "x-rate-limit" in k}
             current_time = int(time.time())
-            wait = int(r.headers.get('x-rate-limit-reset', current_time)) - current_time
-            remaining = limits.get('x-rate-limit-remaining')
-            limit = limits.get('x-rate-limit-limit')
+            wait = int(r.headers.get("x-rate-limit-reset", current_time)) - current_time
+            remaining = limits.get("x-rate-limit-remaining")
+            limit = limits.get("x-rate-limit-limit")
             logger.debug(f"remaining: {MAGENTA}{remaining}/{limit}{RESET} requests")
-            logger.debug(f'reset:     {MAGENTA}{(wait / 60):.2f}{RESET} minutes')
+            logger.debug(f"reset:     {MAGENTA}{(wait / 60):.2f}{RESET} minutes")
         except Exception as e:
-            logger.error(f'Rate limit info unavailable: {e}')
+            logger.error(f"Rate limit info unavailable: {e}")
 
     try:
         status = r.status_code
-        txt, data, = r.text, r.json()
-        if 'json' in r.headers.get('content-type', ''):
-            if data.get('errors') and not find_key(data, 'instructions'):
-                logger.error(f'[{RED}error{RESET}] {status} {data}')
+        (
+            txt,
+            data,
+        ) = r.text, r.json()
+        if "json" in r.headers.get("content-type", ""):
+            if data.get("errors") and not find_key(data, "instructions"):
+                logger.error(f"[{RED}error{RESET}] {status} {data}")
             else:
                 logger.debug(fmt_status(status))
                 stat(r, txt, data)
         else:
             logger.debug(fmt_status(status))
             stat(r, txt, {})
     except Exception as e:
-        logger.error(f'Failed to log: {e}')
+        logger.error(f"Failed to log: {e}")
 
 
 def fmt_status(status: int) -> str:
     color = None
     if 200 <= status < 300:
         color = GREEN
     elif 300 <= status < 400:
         color = MAGENTA
     elif 400 <= status < 600:
         color = RED
-    return f'[{color}{status}{RESET}]'
+    return f"[{color}{status}{RESET}]"
 
 
 def get_ids(data: list | dict, operation: tuple) -> set:
     expr = ID_MAP[operation[-1]]
-    return {k for k in find_key(data, 'entryId') if re.search(expr, k)}
+    return {k for k in find_key(data, "entryId") if re.search(expr, k)}
 
 
 def dump(path: str, **kwargs):
     fname, data = list(kwargs.items())[0]
     out = Path(path)
     out.mkdir(exist_ok=True, parents=True)
-    (out / f'{fname}_{time.time_ns()}.json').write_bytes(
-        orjson.dumps(data, option=orjson.OPT_INDENT_2 | orjson.OPT_SORT_KEYS))
+    (out / f"{fname}_{time.time_ns()}.json").write_bytes(
+        orjson.dumps(data, option=orjson.OPT_INDENT_2 | orjson.OPT_SORT_KEYS)
+    )
 
 
 def get_code(cls, retries=5) -> str | None:
-    """ Get verification code from Proton Mail inbox """
+    """Get verification code from Proton Mail inbox"""
 
     def poll_inbox():
         inbox = cls.inbox()
-        for c in inbox.get('Conversations', []):
-            if c['Senders'][0]['Address'] == 'info@twitter.com':
-                exprs = ['Your Twitter confirmation code is (.+)', '(.+) is your Twitter verification code']
-                if temp := list(filter(None, (re.search(expr, c['Subject']) for expr in exprs))):
+        for c in inbox.get("Conversations", []):
+            if c["Senders"][0]["Address"] == "info@twitter.com":
+                exprs = [
+                    "Your Twitter confirmation code is (.+)",
+                    "(.+) is your Twitter verification code",
+                ]
+                if temp := list(
+                    filter(None, (re.search(expr, c["Subject"]) for expr in exprs))
+                ):
                     return temp[0].group(1)
 
     for i in range(retries + 1):
         if code := poll_inbox():
             return code
         if i == retries:
-            print('Max retries exceeded')
+            print("Max retries exceeded")
             return
-        t = 2 ** i + random.random()
+        t = 2**i + random.random()
         print(f'Retrying in {f"{t:.2f}"} seconds')
         time.sleep(t)
```

### Comparing `asyncTwitterClient-0.8.0/asyncTwitter/constants.py` & `asyncTwitterClient-1.0.0/asyncTwitter/constants.py`

 * *Files identical despite different names*

### Comparing `asyncTwitterClient-0.8.0/asyncTwitter/login.py` & `asyncTwitterClient-1.0.0/asyncTwitter/login.py`

 * *Files identical despite different names*

### Comparing `asyncTwitterClient-0.8.0/asyncTwitter/scraper.py` & `asyncTwitterClient-1.0.0/asyncTwitter/scraper.py`

 * *Files identical despite different names*

### Comparing `asyncTwitterClient-0.8.0/asyncTwitter/search.py` & `asyncTwitterClient-1.0.0/asyncTwitter/search.py`

 * *Files identical despite different names*

### Comparing `asyncTwitterClient-0.8.0/asyncTwitter/twoCaptcha.py` & `asyncTwitterClient-1.0.0/asyncTwitter/twoCaptcha.py`

 * *Files identical despite different names*

### Comparing `asyncTwitterClient-0.8.0/asyncTwitter/util.py` & `asyncTwitterClient-1.0.0/asyncTwitter/util.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,27 +1,49 @@
 import random
 import re
 import time
+import string
+
 from logging import Logger
 from pathlib import Path
 from urllib.parse import urlsplit, urlencode, urlunsplit, parse_qs, quote
 
 import orjson
-from httpx import Response, Client
+from httpx import Response, AsyncClient
+
+from .constants import GREEN, MAGENTA, RED, RESET, ID_MAP, USER_AGENTS
+
+
+def generate_random_string(length):
+    characters = string.ascii_letters + string.digits
+    return "".join(random.choice(characters) for i in range(length))
+
+
+def randomLivePipelineSession():
+    # 'LivePipeline-Session': '4cc59a77-31a2-4ed0-8246-ada14c86d528',
+
+    return f"{generate_random_string(8)}-{generate_random_string(4)}-{generate_random_string(4)}-{generate_random_string(4)}-{generate_random_string(12)}"
+
 
-from .constants import GREEN, MAGENTA, RED, RESET, ID_MAP
+def randomTransactionId():
+    x_client_transaction_id = f"{generate_random_string(19)}/{generate_random_string(3)}/{generate_random_string(18)}+{generate_random_string(51)}"
+    return x_client_transaction_id
 
 
-def init_session():
-    client = Client(
+def init_session(**kwargs):
+    client = AsyncClient(
         headers={
             "authorization": "Bearer AAAAAAAAAAAAAAAAAAAAANRILgAAAAAAnNwIzUejRCOuH5E6I8xnZz4puTs=1Zv7ttfk8LF81IUq16cHjhLTvJu4FA33AGWWjCpTnA",
-            "user-agent": "Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/113.0.0.0 Safari/537.36",
+            "user-agent": random.choice(USER_AGENTS),
         },
         follow_redirects=True,
+        http2=True,
+        timeout=30,
+        verify=False,
+        **kwargs,
     )
     r = client.post("https://api.twitter.com/1.1/guest/activate.json").json()
     client.headers.update(
         {
             "content-type": "application/json",
             "x-guest-token": r["guest_token"],
             "x-twitter-active-user": "yes",
@@ -126,25 +148,42 @@
     cookies = session.cookies
     # todo httpx cookie issues
     try:
         if session._init_with_cookies:
             cookies.delete("ct0", domain=".twitter.com")
     except Exception:
         ...
-    headers = kwargs | {
-        "authorization": "Bearer AAAAAAAAAAAAAAAAAAAAANRILgAAAAAAnNwIzUejRCOuH5E6I8xnZz4puTs=1Zv7ttfk8LF81IUq16cHjhLTvJu4FA33AGWWjCpTnA",
-        "cookie": "; ".join(f"{k}={v}" for k, v in cookies.items()),
-        "referer": "https://twitter.com/",
-        "user-agent": "Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/113.0.0.0 Safari/537.36",
-        "x-csrf-token": cookies.get("ct0", ""),
-        "x-guest-token": cookies.get("guest_token", ""),
-        "x-twitter-auth-type": "OAuth2Session" if cookies.get("auth_token") else "",
-        "x-twitter-active-user": "yes",
-        "x-twitter-client-language": "en",
-    }
+    headers = (
+        kwargs
+        | {
+            "User-Agent": random.choice(USER_AGENTS),
+            "Accept": "*/*",
+            "Accept-Language": "en-CA,en-US;q=0.7,en;q=0.3",
+            "authorization": "Bearer AAAAAAAAAAAAAAAAAAAAANRILgAAAAAAnNwIzUejRCOuH5E6I8xnZz4puTs=1Zv7ttfk8LF81IUq16cHjhLTvJu4FA33AGWWjCpTnA",
+            "LivePipeline-Session": randomLivePipelineSession(),  #'4cc59a77-31a2-4ed0-8246-ada14c86d528',
+            # "cookie": "; ".join(f"{k}={v}" for k, v in cookies.items()),
+            "Referer": "https://twitter.com/",
+            "x-csrf-token": cookies.get("ct0", ""),
+            "x-guest-token": cookies.get("guest_token", ""),
+            "x-twitter-auth-type": "OAuth2Session" if cookies.get("auth_token") else "",
+            "x-twitter-active-user": "yes",
+            "x-twitter-client-language": "en",
+            "Origin": "https://twitter.com",
+            "DNT": "1",
+            "Sec-GPC": "1",
+            "Sec-Fetch-Dest": "empty",
+            "Sec-Fetch-Mode": "cors",
+            "Sec-Fetch-Site": "same-site",
+            "Connection": "keep-alive",
+            "Pragma": "no-cache",
+            "Cache-Control": "no-cache",
+            # oLYdXdvdHrDENpgQRhn/c2v/cj3SoIX67EyajoIa5y+ZmpxGNKiEFT1WlnSFv1BrQUVHRaFLp1c2Xx1iMaGOeqYgtygDow
+            "x-client-transaction-id": randomTransactionId(),
+        }
+    )
     return dict(sorted({k.lower(): v for k, v in headers.items()}.items()))
 
 
 def find_key(obj: any, key: str) -> list:
     """
     Find all values of a given key within a nested dict or list of dicts
 
@@ -175,25 +214,28 @@
                 L.extend(helper(obj[k], key, []))
         return L
 
     return helper(obj, key, [])
 
 
 def log(logger: Logger, resp: Response):
-    #x-rate-limit-reset
-    #x-rate-limit-remaining
-    #x-rate-limit-limit
-    
+    # x-rate-limit-reset
+    # x-rate-limit-remaining
+    # x-rate-limit-limit
+
     limitRemaining = resp.headers.get("x-rate-limit-remaining", 0)
     limitReset = resp.headers.get("x-rate-limit-reset", 0)
     limit = resp.headers.get("x-rate-limit-limit", 0)
-    
-    logger.info(f"[{resp.status_code}] {resp.url} | Rate limit: {limitRemaining}/{limit} resets in {limitReset}")
+
+    logger.info(
+        f"[{resp.status_code}] {resp.url} | Rate limit: {limitRemaining}/{limit} resets in {limitReset}"
+    )
     return True
 
+
 def fmt_status(status: int) -> str:
     color = None
     if 200 <= status < 300:
         color = GREEN
     elif 300 <= status < 400:
         color = MAGENTA
     elif 400 <= status < 600:
```

### Comparing `asyncTwitterClient-0.8.0/asyncTwitterClient.egg-info/SOURCES.txt` & `asyncTwitterClient-1.0.0/asyncTwitterClient.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 asyncTwitter/asyncScraper.py
 asyncTwitter/asyncSearch.py
 asyncTwitter/asyncUtil.py
 asyncTwitter/constants.py
 asyncTwitter/login.py
 asyncTwitter/scraper.py
 asyncTwitter/search.py
+asyncTwitter/test.py
 asyncTwitter/twoCaptcha.py
 asyncTwitter/util.py
 asyncTwitterClient.egg-info/PKG-INFO
 asyncTwitterClient.egg-info/SOURCES.txt
 asyncTwitterClient.egg-info/dependency_links.txt
 asyncTwitterClient.egg-info/requires.txt
 asyncTwitterClient.egg-info/top_level.txt
```

