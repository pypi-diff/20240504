# Comparing `tmp/speedruncompy-0.3.3.tar.gz` & `tmp/speedruncompy-0.4.0.tar.gz`

## Comparing `speedruncompy-0.3.3.tar` & `speedruncompy-0.4.0.tar`

### file list

```diff
@@ -1,29 +1,32 @@
--rw-r--r--   0        0        0      218 2020-02-02 00:00:00.000000 speedruncompy-0.3.3/requirements.txt
--rw-r--r--   0        0        0     1630 2020-02-02 00:00:00.000000 speedruncompy-0.3.3/.github/workflows/python-package.yml
--rw-r--r--   0        0        0     1153 2020-02-02 00:00:00.000000 speedruncompy-0.3.3/.github/workflows/python-publish.yml
--rw-r--r--   0        0        0     1145 2020-02-02 00:00:00.000000 speedruncompy-0.3.3/examples/test.ipynb
--rw-r--r--   0        0        0     2698 2020-02-02 00:00:00.000000 speedruncompy-0.3.3/examples/test.py
--rw-r--r--   0        0        0     1169 2020-02-02 00:00:00.000000 speedruncompy-0.3.3/examples/testAsync.py
--rw-r--r--   0        0        0      541 2020-02-02 00:00:00.000000 speedruncompy-0.3.3/examples/testAuthFlow.py
--rw-r--r--   0        0        0      440 2020-02-02 00:00:00.000000 speedruncompy-0.3.3/examples/testBadRequest.py
--rw-r--r--   0        0        0      277 2020-02-02 00:00:00.000000 speedruncompy-0.3.3/examples/testData.py
--rw-r--r--   0        0        0     1655 2020-02-02 00:00:00.000000 speedruncompy-0.3.3/examples/testPaginated.py
--rw-r--r--   0        0        0      774 2020-02-02 00:00:00.000000 speedruncompy-0.3.3/examples/testRateLimit.py
--rw-r--r--   0        0        0       89 2020-02-02 00:00:00.000000 speedruncompy-0.3.3/src/speedruncompy/__init__.py
--rw-r--r--   0        0        0     7957 2020-02-02 00:00:00.000000 speedruncompy-0.3.3/src/speedruncompy/api.py
--rw-r--r--   0        0        0     2220 2020-02-02 00:00:00.000000 speedruncompy-0.3.3/src/speedruncompy/auth.py
--rw-r--r--   0        0        0    27184 2020-02-02 00:00:00.000000 speedruncompy-0.3.3/src/speedruncompy/datatypes.py
--rw-r--r--   0        0        0    50596 2020-02-02 00:00:00.000000 speedruncompy-0.3.3/src/speedruncompy/endpoints.py
--rw-r--r--   0        0        0     3784 2020-02-02 00:00:00.000000 speedruncompy-0.3.3/src/speedruncompy/enums.py
--rw-r--r--   0        0        0     2167 2020-02-02 00:00:00.000000 speedruncompy-0.3.3/src/speedruncompy/exceptions.py
--rw-r--r--   0        0        0     9615 2020-02-02 00:00:00.000000 speedruncompy-0.3.3/src/speedruncompy/responses.py
--rw-r--r--   0        0        0       15 2020-02-02 00:00:00.000000 speedruncompy-0.3.3/src/speedruncompy/scripts/__init__.py
--rw-r--r--   0        0        0      804 2020-02-02 00:00:00.000000 speedruncompy-0.3.3/src/speedruncompy/scripts/srcompy_login.py
--rw-r--r--   0        0        0     7455 2020-02-02 00:00:00.000000 speedruncompy-0.3.3/test/test_datatypes.py
--rw-r--r--   0        0        0    22369 2020-02-02 00:00:00.000000 speedruncompy-0.3.3/test/test_endpoints.py
--rw-r--r--   0        0        0     1171 2020-02-02 00:00:00.000000 speedruncompy-0.3.3/test/utils.py
--rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 speedruncompy-0.3.3/.gitignore
--rw-r--r--   0        0        0    26526 2020-02-02 00:00:00.000000 speedruncompy-0.3.3/LICENSE
--rw-r--r--   0        0        0     1389 2020-02-02 00:00:00.000000 speedruncompy-0.3.3/README.md
--rw-r--r--   0        0        0     1197 2020-02-02 00:00:00.000000 speedruncompy-0.3.3/pyproject.toml
--rw-r--r--   0        0        0     2272 2020-02-02 00:00:00.000000 speedruncompy-0.3.3/PKG-INFO
+-rw-r--r--   0        0        0     1552 2020-02-02 00:00:00.000000 speedruncompy-0.4.0/.github/workflows/python-package.yml
+-rw-r--r--   0        0        0     1153 2020-02-02 00:00:00.000000 speedruncompy-0.4.0/.github/workflows/python-publish.yml
+-rw-r--r--   0        0        0     1145 2020-02-02 00:00:00.000000 speedruncompy-0.4.0/examples/test.ipynb
+-rw-r--r--   0        0        0     2698 2020-02-02 00:00:00.000000 speedruncompy-0.4.0/examples/test.py
+-rw-r--r--   0        0        0     1169 2020-02-02 00:00:00.000000 speedruncompy-0.4.0/examples/testAsync.py
+-rw-r--r--   0        0        0      541 2020-02-02 00:00:00.000000 speedruncompy-0.4.0/examples/testAuthFlow.py
+-rw-r--r--   0        0        0      440 2020-02-02 00:00:00.000000 speedruncompy-0.4.0/examples/testBadRequest.py
+-rw-r--r--   0        0        0      277 2020-02-02 00:00:00.000000 speedruncompy-0.4.0/examples/testData.py
+-rw-r--r--   0        0        0     1655 2020-02-02 00:00:00.000000 speedruncompy-0.4.0/examples/testPaginated.py
+-rw-r--r--   0        0        0      774 2020-02-02 00:00:00.000000 speedruncompy-0.4.0/examples/testRateLimit.py
+-rw-r--r--   0        0        0      114 2020-02-02 00:00:00.000000 speedruncompy-0.4.0/src/speedruncompy/__init__.py
+-rw-r--r--   0        0        0    10032 2020-02-02 00:00:00.000000 speedruncompy-0.4.0/src/speedruncompy/api.py
+-rw-r--r--   0        0        0     2189 2020-02-02 00:00:00.000000 speedruncompy-0.4.0/src/speedruncompy/auth.py
+-rw-r--r--   0        0        0      444 2020-02-02 00:00:00.000000 speedruncompy-0.4.0/src/speedruncompy/config.py
+-rw-r--r--   0        0        0    48383 2020-02-02 00:00:00.000000 speedruncompy-0.4.0/src/speedruncompy/endpoints.py
+-rw-r--r--   0        0        0     6907 2020-02-02 00:00:00.000000 speedruncompy-0.4.0/src/speedruncompy/enums.py
+-rw-r--r--   0        0        0     2168 2020-02-02 00:00:00.000000 speedruncompy-0.4.0/src/speedruncompy/exceptions.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 speedruncompy-0.4.0/src/speedruncompy/py.typed
+-rw-r--r--   0        0        0    10355 2020-02-02 00:00:00.000000 speedruncompy-0.4.0/src/speedruncompy/responses.py
+-rw-r--r--   0        0        0      116 2020-02-02 00:00:00.000000 speedruncompy-0.4.0/src/speedruncompy/datatypes/__init__.py
+-rw-r--r--   0        0        0     7518 2020-02-02 00:00:00.000000 speedruncompy-0.4.0/src/speedruncompy/datatypes/_impl.py
+-rw-r--r--   0        0        0    23112 2020-02-02 00:00:00.000000 speedruncompy-0.4.0/src/speedruncompy/datatypes/defs.py
+-rw-r--r--   0        0        0       15 2020-02-02 00:00:00.000000 speedruncompy-0.4.0/src/speedruncompy/scripts/__init__.py
+-rw-r--r--   0        0        0      796 2020-02-02 00:00:00.000000 speedruncompy-0.4.0/src/speedruncompy/scripts/srcompy_login.py
+-rw-r--r--   0        0        0     7616 2020-02-02 00:00:00.000000 speedruncompy-0.4.0/test/test_datatypes.py
+-rw-r--r--   0        0        0    27645 2020-02-02 00:00:00.000000 speedruncompy-0.4.0/test/test_endpoints.py
+-rw-r--r--   0        0        0     1187 2020-02-02 00:00:00.000000 speedruncompy-0.4.0/test/utils.py
+-rw-r--r--   0        0        0      142 2020-02-02 00:00:00.000000 speedruncompy-0.4.0/.gitignore
+-rw-r--r--   0        0        0    26526 2020-02-02 00:00:00.000000 speedruncompy-0.4.0/LICENSE
+-rw-r--r--   0        0        0     3277 2020-02-02 00:00:00.000000 speedruncompy-0.4.0/README.md
+-rw-r--r--   0        0        0     1215 2020-02-02 00:00:00.000000 speedruncompy-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0     4203 2020-02-02 00:00:00.000000 speedruncompy-0.4.0/PKG-INFO
```

### Comparing `speedruncompy-0.3.3/.github/workflows/python-package.yml` & `speedruncompy-0.4.0/.github/workflows/python-package.yml`

 * *Files 14% similar despite different names*

```diff
@@ -22,25 +22,24 @@
     - name: Set up Python ${{ matrix.python-version }}
       uses: actions/setup-python@v3
       with:
         python-version: ${{ matrix.python-version }}
     - name: Install dependencies
       run: |
         python -m pip install --upgrade pip
-        python -m pip install flake8 pytest
-        if [ -f requirements.txt ]; then pip install -r requirements.txt; fi
+        python -m pip install flake8
     - name: Lint with flake8
       run: |
         # stop the build if there are Python syntax errors or undefined names
         flake8 . --count --select=E9,F63,F7,F82 --show-source --statistics
         # exit-zero treats all errors as warnings. The GitHub editor is 127 chars wide
         flake8 . --count --exit-zero --max-complexity=10 --max-line-length=127 --statistics
     - name: Interactive install
       run: |
-        python -m pip install -e .
+        python -m pip install -e .[test]
     - name: Test with pytest
       env:
         HORNET_PHPSESSID: ${{secrets.HORNET_PHPSESSID}}
         LOW_PHPSESSID: ${{secrets.LOW_PHPSESSID}}
         LOW_USERNAME: ${{secrets.LOW_USERNAME}}
         LOW_PASSWORD: ${{secrets.LOW_PASSWORD}}
         SKIP_HEAVY_TESTS: true
```

### Comparing `speedruncompy-0.3.3/.github/workflows/python-publish.yml` & `speedruncompy-0.4.0/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `speedruncompy-0.3.3/examples/test.ipynb` & `speedruncompy-0.4.0/examples/test.ipynb`

 * *Files identical despite different names*

### Comparing `speedruncompy-0.3.3/examples/test.py` & `speedruncompy-0.4.0/examples/test.py`

 * *Files identical despite different names*

### Comparing `speedruncompy-0.3.3/examples/testAsync.py` & `speedruncompy-0.4.0/examples/testAsync.py`

 * *Files identical despite different names*

### Comparing `speedruncompy-0.3.3/examples/testAuthFlow.py` & `speedruncompy-0.4.0/examples/testAuthFlow.py`

 * *Files identical despite different names*

### Comparing `speedruncompy-0.3.3/examples/testPaginated.py` & `speedruncompy-0.4.0/examples/testPaginated.py`

 * *Files identical despite different names*

### Comparing `speedruncompy-0.3.3/examples/testRateLimit.py` & `speedruncompy-0.4.0/examples/testRateLimit.py`

 * *Files identical despite different names*

### Comparing `speedruncompy-0.3.3/src/speedruncompy/api.py` & `speedruncompy-0.4.0/src/speedruncompy/api.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,163 +1,210 @@
 import base64, json
-from .exceptions import *
 import logging
 import asyncio, aiohttp
-from typing import Awaitable, Callable, Any
+import random
+from typing import Awaitable, Callable, Any, Generic, TypeVar
+
+from yarl import URL
+from copy import copy
 
-from .datatypes import Datatype, srcpyJSONEncoder, LenientDatatype
+from .datatypes import Datatype, srcpyJSONEncoder, LenientDatatype, Pagination
+from .exceptions import *
 
 API_URI = "https://www.speedrun.com/api/v2/"
 LANG = "en"
 ACCEPT = "application/json"
 DEFAULT_USER_AGENT = "speedruncompy/"
-COOKIE_PHPSESSID_REGEX = "(?:PHPSESSID=)([\w]*)(?:;)"
 
 _log = logging.getLogger("speedruncompy")
 
+
 class SpeedrunComPy():
     """Api class. Holds a unique PHPSESSID and user_agent, as well as its own logger."""
-    def __init__(self, user_agent = None) -> None:
-        self.cookie_jar = {}
-        self.user_agent = user_agent
+    def __init__(self, user_agent: str | None = None) -> None:
+        self.cookie_jar = aiohttp.CookieJar()
+        self._header = {"Accept-Language": LANG, "Accept": ACCEPT, "User-Agent": f"{DEFAULT_USER_AGENT}{user_agent}"}
         if user_agent is None:
             self._log = _log
         else:
             self._log = _log.getChild(user_agent)
-    
-    def set_phpsessid(self, phpsessid):
-        self.cookie_jar["PHPSESSID"] = phpsessid
-    
-    def get_phpsessid(self):
-        return self.cookie_jar.get("PHPSESSID", None)
+
+    def _get_PHPSESSID(self) -> str | None:
+        cookie = self.cookie_jar.filter_cookies(URL("/")).get("PHPSESSID")
+        return None if cookie is None else cookie.value
+
+    def _set_PHPSESSID(self, phpsessid):
+        self.cookie_jar.update_cookies({"PHPSESSID": phpsessid})
+    
+    PHPSESSID = property(_get_PHPSESSID, _set_PHPSESSID)
+    """Login token. Set by `PutAuthLogin`, or you may set it manually to a logged in session."""
+
+    @staticmethod
+    def _encode_r(params: dict):
+        """Encodes a parameter dict into url-base64 encoded min-json, ready for use as `_r` in a GET URL."""
+        paramsjson = bytes(json.dumps(params, separators=(",", ":"), cls=srcpyJSONEncoder).strip(), "utf-8")
+        return base64.urlsafe_b64encode(paramsjson).replace(b"=", b"").decode()
 
     async def do_get(self, endpoint: str, params: dict = {}) -> tuple[bytes, int]:
-        _header = {"Accept-Language": LANG, "Accept": ACCEPT, "User-Agent": f"{DEFAULT_USER_AGENT}{self.user_agent}"}
         # Params passed to the API by the site are json-base64 encoded, even though std params are supported.
         # We will do the same in case param support is retracted.
-        paramsjson = bytes(json.dumps(params, separators=(",", ":"), cls=srcpyJSONEncoder).strip(), "utf-8")
-        _r = base64.urlsafe_b64encode(paramsjson).replace(b"=", b"").decode()
-        self._log.debug(f"GET {endpoint} w/ params {paramsjson}")
-        async with aiohttp.ClientSession() as session:
-            async with session.get(url=f"{API_URI}{endpoint}", headers=_header, params={"_r": _r}) as response:
+        self._log.debug(f"GET {endpoint} w/ params {params}")
+        async with aiohttp.ClientSession(headers=self._header, cookie_jar=self.cookie_jar) as session:
+            async with session.get(url=f"{API_URI}{endpoint}", params={"_r": self._encode_r(params)}) as response:
                 return (await response.read(), response.status)
         
-    async def do_post(self, endpoint:str, params: dict = {}, _setCookie=True) -> tuple[bytes, int]:
-        _header = {"Accept-Language": LANG, "Accept": ACCEPT, "User-Agent": f"{DEFAULT_USER_AGENT}{self.user_agent}"}
+    async def do_post(self, endpoint: str, params: dict = {}, _setCookie=True) -> tuple[bytes, int]:
+        # Construct a dummy jar if we wish to ignore Set_Cookie responses (only on PutAuthLogin and PutAuthSignup)
+        if _setCookie: liveJar = self.cookie_jar
+        else:
+            liveJar = aiohttp.CookieJar()
+            liveJar.update_cookies(self.cookie_jar._cookies)
         self._log.debug(f"POST {endpoint} w/ params {params}")
-        async with aiohttp.ClientSession(json_serialize=lambda o: json.dumps(o, separators=(",", ":"), cls=srcpyJSONEncoder)) as session:
-            async with session.post(url=f"{API_URI}{endpoint}", headers=_header,
-                                    cookies=self.cookie_jar, json=params) as response:
-                if _setCookie and response.cookies:
-                    for k, cookie in response.cookies.items():
-                        self.cookie_jar.update({cookie.key: cookie.value})
-                return (await response.read(), response.status) 
+        async with aiohttp.ClientSession(json_serialize=lambda o: json.dumps(o, separators=(",", ":"), cls=srcpyJSONEncoder),
+                                         headers=self._header, cookie_jar=liveJar) as session:
+            async with session.post(url=f"{API_URI}{endpoint}", json=params) as response:
+                return (await response.read(), response.status)
+
 
 _default = SpeedrunComPy()
 
+
 def set_default_PHPSESSID(phpsessionid):
-    _default.cookie_jar.update({"PHPSESSID": phpsessionid})
+    _default.PHPSESSID = phpsessionid
+
 
-class BaseRequest():
-    def __init__(self, 
+R = TypeVar('R', bound=Datatype)
+
+
+class BaseRequest(Generic[R]):
+    def __init__(self,
                  method: Callable[[str, dict[str, Any]], Awaitable[tuple[bytes, int]]],
-                 endpoint: str, 
-                 returns: type = LenientDatatype,
+                 endpoint: str,
+                 returns: type[R],
                  **params):
         self.method = method
         self.endpoint = endpoint
         self.params = params
         self.return_type = returns
     
     def update_params(self, **kwargs):
         """Updates parameters using values set in kwargs"""
         self.params.update(kwargs)
 
-    def perform(self, retries=5, delay=1, **kwargs) -> Datatype:
+    def perform(self, retries=5, delay=1, autovary=False, **kwargs) -> R:
         """Synchronously perform the request.
         
         NB: This uses its own event loop, so if using `asyncio` use `perform_async()` instead."""
         try:
-            return asyncio.run(self.perform_async(retries, delay, **kwargs))
-        except RuntimeError as e:
+            return asyncio.run(self.perform_async(retries, delay, autovary, **kwargs))
+        except RuntimeError:
             raise AIOException("Synchronous interface called from asynchronous context - use `await perform_async` instead.") from None
     
-    async def perform_async(self, retries=5, delay=1, **kwargs) -> Datatype:
+    async def perform_async(self, retries=5, delay=1, autovary=False, **kwargs) -> R:
         """Asynchronously perform the request. Remember to `await` me!"""
+        if autovary is True: kwargs |= {"vary": random.randint(1, 1000000000)}
         self.response = await self.method(self.endpoint, self.params | kwargs)
         content = self.response[0]
         status = self.response[1]
 
         if (status >= 500 and status <= 599) or status == 408:
             if retries > 0:
-                _log.error(f"SRC returned error {status} {content}. Retrying with delay {delay}:")
-                for attempt in range(0, retries+1):
+                _log.error(f"SRC returned error {status} {content!r}. Retrying with delay {delay}:")
+                for attempt in range(0, retries + 1):
                     self.response = await self.method(self.endpoint, self.params)
                     content = self.response[0]
                     status = self.response[1]
-                    if not (status >= 500 and status <= 599) or status == 408: 
+                    if not (status >= 500 and status <= 599) or status == 408:
                         break
-                    _log.error(f"Retry {attempt} returned error {status} {content}")
+                    _log.error(f"Retry {attempt} returned error {status} {content!r}")
                     await asyncio.sleep(delay)
                 else:
                     if status == 408: raise RequestTimeout(self)
                     else: raise ServerException(self)
         
-        if status == 400: raise BadRequest(self)
-        if status == 401: raise Unauthorized(self)
-        if status == 403: raise Forbidden(self)
-        if status == 404: raise NotFound(self)
-        if status == 405: raise MethodNotAllowed(self)
-        if status == 408: raise RequestTimeout(self)
-        if status == 429: raise RateLimitExceeded(self)
+        match status:
+            case 400: raise BadRequest(self)
+            case 401: raise Unauthorized(self)
+            case 403: raise Forbidden(self)
+            case 404: raise NotFound(self)
+            case 405: raise MethodNotAllowed(self)
+            case 408: raise RequestTimeout(self)
+            case 429: raise RateLimitExceeded(self)
 
         if (status >= 500 and status <= 599): raise ServerException(self)
 
         if status < 200 or status > 299:
-            _log.error(f"Unknown response error returned from SRC! {status} {self.response[0]}")
+            _log.error(f"Unknown response error returned from SRC! {status} {self.response[0]!r}")
             raise APIException(self)
 
         return self.return_type(json.loads(content.decode()))
 
-class BasePaginatedRequest(BaseRequest):
-    def _combine_results(self, pages: dict):
-        _log.warning(f"""perform_all or perform_all_async on {type(self).__name__} is NOT yet implemented!
-                     
-                     Use _perform_all_raw() or _perform_all_async_raw() to protect against future updates.""")
-        return pages
 
-    def perform_all(self, retries=5, delay=1) -> dict:
+class BasePaginatedRequest(BaseRequest[R], Generic[R]):
+    def _combine_results(self, pages: dict[int, R]) -> R:
+        raise NotImplementedError(f"perform_all or perform_all_async on {type(self).__name__} is NOT yet implemented! Use _perform_all_raw() or _perform_all_async_raw()")
+
+    def _get_pagination(self, p: R) -> Pagination:
+        """Locates the pagination object on a response. Overriden on certain subclasses."""
+        return p["pagination"]
+    
+    @staticmethod
+    def _combine_keys(pages: dict[int, R], main_keys: list[str], merge_keys: list[str]) -> R:
+        """Merge multiple pages. `main_keys` are appended, `merge_keys` are deduplicated by id."""
+        accumulator: R = copy(pages[1])
+        accuDicts: dict[str, dict[str, Datatype]] = {key: dict() for key in merge_keys}
+        
+        iterator = iter(pages.items())
+        next(iterator)  # skip first page (already in accumulator)
+        for i, p in iterator:
+            for main_key in main_keys:
+                accumulator[main_key] += p[main_key]
+            for key in merge_keys:
+                if p[key] is None: continue  # Guard against None fields
+                accuDicts[key].update({item["id"]: item for item in p[key]})
+        
+        for key in merge_keys:
+            accumulator[key] = list(accuDicts[key].values())
+        
+        return accumulator
+    
+    def perform_all(self, retries=5, delay=1, autovary=False, max_pages=0, **kwargs) -> R:
         """Returns a combined dict of all pages. `pagination` is removed."""
-        pages = self._perform_all_raw(retries, delay)
+        pages = self._perform_all_raw(retries, delay, autovary, max_pages, **kwargs)
         return self._combine_results(pages)
     
-    def _perform_all_raw(self, retries=5, delay=1) -> dict[int, dict]:
+    def _perform_all_raw(self, retries=5, delay=1, autovary=False, max_pages=0, **kwargs) -> dict[int, R]:
         """Get all pages and return a dict of {pageNo : pageData}."""
         try:
-            return asyncio.run(self._perform_all_async_raw(retries, delay))
-        except RuntimeError as e:
+            return asyncio.run(self._perform_all_async_raw(retries, delay, autovary, max_pages, **kwargs))
+        except RuntimeError:
             raise AIOException("Synchronous interface called from asynchronous context - use `await perform_async` instead.") from None
     
-    async def perform_all_async(self, retries=5, delay=1) -> dict:
+    async def perform_all_async(self, retries=5, delay=1, autovary=False, max_pages=0, **kwargs) -> R:
         """Returns a combined dict of all pages. `pagination` is removed."""
-        pages = await self._perform_all_async_raw(retries, delay)
+        pages = await self._perform_all_async_raw(retries, delay, autovary, max_pages, **kwargs)
         return self._combine_results(pages)
     
-    async def _perform_all_async_raw(self, retries=5, delay=1) -> dict[int, dict]:
+    async def _perform_all_async_raw(self, retries=5, delay=1, autovary=False, max_pages=0, **kwargs) -> dict[int, R]:
         """Get all pages and return a dict of {pageNo : pageData}."""
-        self.pages: dict[int, Datatype] = {}
-        self.pages[1] = await self.perform_async(retries, delay, page=1)
-        numpages = self.pages[1]["pagination"]["pages"]
+        self.pages: dict[int, R] = {}
+        vary = 0 if not autovary else random.randint(1, 1000000000)
+        self.pages[1] = await self.perform_async(retries, delay, page=1, vary=vary, **kwargs)
+        numpages = self._get_pagination(self.pages[1])["pages"]
+        if max_pages >= 1:
+            numpages = min(numpages, max_pages)
         if numpages > 1:
-            results = await asyncio.gather(*[self.perform_async(retries, delay, page=p) for p in range(2, numpages + 1)])
-            self.pages.update({p + 2:result for p, result in enumerate(results)})
+            results = await asyncio.gather(*[self.perform_async(retries, delay, vary=vary, page=p, **kwargs) for p in range(2, numpages + 1)])
+            self.pages.update({p + 2: result for p, result in enumerate(results)})
         return self.pages
 
-class GetRequest(BaseRequest):
-    def __init__(self, endpoint, returns:type=LenientDatatype, _api:SpeedrunComPy|None=None, **params) -> None:
+
+class GetRequest(BaseRequest[R], Generic[R]):
+    def __init__(self, endpoint, returns: type = LenientDatatype, _api: SpeedrunComPy | None = None, **params) -> None:
         if _api is None: _api = _default
         super().__init__(method=_api.do_get, endpoint=endpoint, returns=returns, **params)
 
-class PostRequest(BaseRequest):
-    def __init__(self, endpoint, returns:type=LenientDatatype, _api:SpeedrunComPy|None=None, **params) -> None:
+
+class PostRequest(BaseRequest[R], Generic[R]):
+    def __init__(self, endpoint, returns: type = LenientDatatype, _api: SpeedrunComPy | None = None, **params) -> None:
         if _api is None: _api = _default
         super().__init__(method=_api.do_post, endpoint=endpoint, returns=returns, **params)
```

### Comparing `speedruncompy-0.3.3/src/speedruncompy/auth.py` & `speedruncompy-0.4.0/src/speedruncompy/auth.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,51 +1,51 @@
 import logging
 from .exceptions import AuthException, NotFound
 from .api import SpeedrunComPy, _default
 from .endpoints import PutAuthLogin, PutAuthLogout, GetSession
 
 log = logging.getLogger("speedruncompy.auth")
 
-def login(username: str, pwd: str, _api: SpeedrunComPy = _default, tokenEntry = False):
+def login(username: str, pwd: str, _api: SpeedrunComPy = _default, tokenEntry: bool = False):
     """Quick workflow to set sessid using username & pwd. Will prompt for 2FA if tokenEntry is True, otherwise will return False."""
     try:
-        result: dict = PutAuthLogin(username, pwd, _api=_api).perform()
+        result = PutAuthLogin(username, pwd, _api=_api).perform()
     except NotFound:
         print("Password is incorrect!")
         return False
     if result.get("loggedIn", False):
         log.info("Logged in using username & password")
         return True
     if result.get("tokenChallengeSent", False):
         if tokenEntry:
             log.warning("2FA is enabled - Not logged in!")
             key = input("Enter 2FA token: ")
-            result: dict = PutAuthLogin(username, pwd, key, _api=_api).perform()
+            result = PutAuthLogin(username, pwd, key, _api=_api).perform()
             if result.get("loggedIn", False):
                 log.info("Logged in using 2fa")
                 return True
             else:
                 log.error("2FA code rejected! Not logged in")
         else:
             log.info("2FA code required, not logged in.")
     return False
 
 def login_PHPSESSID(sessID: str, _api: SpeedrunComPy = _default):
     """Login using PHPSESSID. Uses GetSession to check if session is logged in."""
-    _api.set_phpsessid(sessID)
-    result: dict = GetSession(_api=_api).perform()
+    _api.PHPSESSID = sessID
+    result = GetSession(_api=_api).perform()
     if not result["session"]["signedIn"]:
         log.error("Provided PHPSESSID is not logged in - use speedruncompy.auth.login() instead")
         return False
     log.info(f"Logged in as {result['session']['user']['name']} using PHPSESSID")
     return True
 
 def logout(_api: SpeedrunComPy = _default):
     PutAuthLogout(_api=_api).perform()
     return True
 
 def get_CSRF(_api: SpeedrunComPy = _default):
     """Get the csrfToken of the currently logged in user, required for some endpoints."""
-    result: dict[str, dict] = GetSession(_api=_api).perform()
+    result = GetSession(_api=_api).perform()
     if not result["session"].get("signedIn", False):
         raise AuthException("Not logged in, cannot retrieve csrfToken")
-    return result["session"].get("csrfToken")
+    return result["session"].get("csrfToken")
```

### Comparing `speedruncompy-0.3.3/src/speedruncompy/exceptions.py` & `speedruncompy-0.4.0/src/speedruncompy/exceptions.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -52,8 +52,8 @@
     Timeout is estimated via direct testing.
     """
     def __init__(self, caller, *args):
         self.timeout = 1500
         super().__init__(caller, *args)
 
 class ServerException(APIException):
-    """The server threw a 5xx error code, meaning there was an internal exception. These will trigger retries."""
+    """The server threw a 5xx error code, meaning there was an internal exception. These will trigger retries."""
```

### Comparing `speedruncompy-0.3.3/src/speedruncompy/responses.py` & `speedruncompy-0.4.0/src/speedruncompy/responses.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,18 +1,26 @@
 from .datatypes import *
 from typing import Any
 
-class r_DefaultResponse(dict):
-    ...
+class r_Empty(Datatype):
+    """No Content"""
+
+class r_Ok(Datatype):
+    """Response only including `ok`."""
+    ok: bool
+
+    def __bool__(self): return self.ok
+
 
 """GET responses"""
 
+
 class r_GetArticle(Datatype):
     article: Article
-    relatedArticleList: Any # Currently unknown typed list, leaving as Any for now
+    relatedArticleList: list[Article]
     gameList: list[Game]
     userList: list[User]
 
 class r_GetArticleList(Datatype):
     articleList: list[Article]
     pagination: Pagination
     gameList: list[Game]
@@ -23,28 +31,33 @@
     game: Game
     moderatorList: list[ChallengeModerator]
     standingList: list[ChallengeStanding]
     theme: Theme
     userList: list[User]
     challengeRunCount: int
     gameFollowerCount: int
+    titleList: list[Title]
 
 class r_GetChallengeLeaderboard(Datatype):
     challengeRunList: list[ChallengeRun]
     playerList: list[Player]
     userList: list[User]
     pagination: Pagination
 
 class r_GetChallengeRun(Datatype):
     challenge: Challenge
     challengeRun: ChallengeRun
     game: Game
     playerList: list[Player]
     userList: list[User]
 
+class r_GetChallengeGlobalRankingList(Datatype):
+    rankingList: list[GlobalChallengeRanking]
+    userList: list[User]
+
 class r_GetCommentList(Datatype):
     commentable: Commentable
     commentList: list[Comment]
     likeList: list[Like]
     userList: list[User]
     pagination: Pagination
 
@@ -57,21 +70,21 @@
     game: Game
     categories: list[Category]
     levels: list[Level]
     moderators: list[GameModerator]
     platforms: list[Platform]
     regions: list[Region]
     runCounts: list[RunCount]
-    theme: Optional[Theme]
+    theme: OptField[Theme]
     users: list[User]
     values: list[Value]
     variables: list[Variable]
 
 class r_GetGameLeaderboard(Datatype):
-    leaderboard: Leaderboard # not funny. didn't laugh
+    leaderboard: Leaderboard  # not funny. didn't laugh
 
 class r_GetGameLeaderboard2(Datatype):
     runList: list[Run]
     playerList: list[Player]
     pagination: Pagination
 
 class r_GetGameLevelSummary(Datatype):
@@ -96,15 +109,15 @@
     gameStats: list[GameStats]
     stats: GameStats
     relatedGames: list[Game]
     seriesList: list[Series]
     theme: Theme
     threadList: list[Thread]
     users: list[User]
-    challengeList: list[Challenge] #TODO: Check (Any)
+    challengeList: list[Challenge]
     challengeCount: int
     guideCount: int
     levelCount: int
     newsCount: int
     relatedCount: int
     resourceCount: int
     streamCount: int
@@ -115,15 +128,15 @@
     users: list[User]
 
 class r_GetGuideList(Datatype):
     guideList: list[Guide]
     users: list[User]
 
 class r_GetHomeSummary(Datatype):
-    stream: Optional[Stream]
+    stream: OptField[Stream]
 
 class r_GetLatestLeaderboard(Datatype):
     categories: list[Category]
     games: list[Game]
     levels: list[Level]
     players: list[Player]
     regions: list[Region]
@@ -143,34 +156,47 @@
 class r_GetResourceList(Datatype):
     resourceList: list[Resource]
     users: list[User]
 
 class r_GetRun(Datatype):
     game: Game
     category: Category
-    level: Optional[Level]
-    platform: Optional[Platform]
+    level: OptField[Level]
+    platform: OptField[Platform]
     players: list[Player]
-    region: Optional[Region]
+    region: OptField[Region]
     run: Run
     users: list[User]
     values: list[Value]
     variables: list[Variable]
 
 class r_GetSearch(Datatype):
     gameList: list[Game]
     newsList: list[News]
-    pageList: list[Article] #TODO: check
+    pageList: list[Article]  # TODO: check
     seriesList: list[Series]
     userList: list[User]
+    challengeList: list[Challenge]
 
 class r_GetSeriesList(Datatype):
     seriesList: list[Series]
     pagination: Pagination
 
+class r_GetSeriesSummary(Datatype):
+    series: Series
+    forum: Forum
+    gameList: list[Game]
+    moderatorList: list[SeriesModerator]
+    theme: Theme
+    threadList: list[Thread]
+    userList: list[User]
+    gameCount: int
+    streamCount: int
+    threadCount: int
+
 class r_GetStreamList(Datatype):
     gameList: list[Game]
     streamList: list[Stream]
     userList: list[User]
     pagination: Pagination
 
 class r_GetThread(Datatype):
@@ -189,37 +215,68 @@
     categories: list[Category]
     games: list[Game]
     levels: list[Level]
     platforms: list[Platform]
     regions: list[Region]
     runs: list[Run]
     user: User
-    userProfile: UserLeaderboardProfile
+    userProfile: UserReducedProfile
     users: list[User]
     """Always empty"""
     players: list[Player]
     values: list[Value]
     variables: list[Variable]
-    followedGameIds: None
+    followedGameIds: Optional[Any]
     """Unused null key"""
     challengeList: list[Challenge]
     challengeRunList: list[ChallengeRun]
 
+class r_GetUserSummary(Datatype):
+    user: User
+    userProfile: UserReducedProfile
+    userStats: UserStats
+    userGameFollowerStats: list[UserGameFollow]
+    """Empty list if the user has set game follows to private."""
+    userGameModeratorStats: list[UserModerationStats]
+    userGameRunnerStats: list[UserGameRunnerStats]
+    userSocialConnectionList: list[UserSocialConnection]
+    games: list[Game]
+    theme: Theme
+    titleList: list[Title]
+
 class r_GetUserPopoverData(Datatype):
     user: User
-    userProfile: UserLeaderboardProfile
+    userProfile: UserReducedProfile
     userStats: UserStats
     userSocialConnectionList: list[UserSocialConnection]
     games: list[Game]
     """Contains games sometimes:tm:"""
+    titleList: list[Title]
+
+class r_GetTitleList(Datatype):
+    titleList: list[Title]
+
+class r_GetTitle(Datatype):
+    title: Title
+
 
 """POST responses"""
 
+
 class r_GetAuditLogList(Datatype):
     auditLogList: list[AuditLogEntry]
+    userList: list[User]
+    gameList: list[Game]
+    categoryList: list[Category]
+    levelList: Optional[list[Level]]
+    """WARN: is None when empty rather than []."""
+    variableList: list[Variable]
+    valueList: list[Value]
+    runList: list[Run]
+    pagination: Pagination
 
 class r_GetCommentable(Datatype):
     commentable: Commentable
 
 class r_GetConversationMessages(Datatype):
     conversation: Conversation
     participants: list[ConversationParticipant]
@@ -240,26 +297,31 @@
     settings: GameSettings
     moderatorList: list[GameModerator]
     theme: Theme
     gameList: list[Game]
     userList: list[User]
 
 class r_GetModerationGames(Datatype):
-    games: list[Game]
-    gameModerationStats: list[GameModerationStats]
+    games: Optional[list[Game]]
+    """Is null when not logged in."""
+    gameModerationStats: Optional[list[GameModerationStats]]
+    """Is null when not logged in."""
 
 class r_GetModerationRuns(Datatype):
-    categories:  list[Category]
+    categories: list[Category]
     games: list[Game]
     levels: list[Level]
     pagination: Pagination
     platforms: list[Platform]
     players: list[Player]
     regions: list[Region]
     runs: list[Run]
+    values: list[Value]
+    variables: list[Variable]
+    users: list[User]
 
 class r_GetNotifications(Datatype):
     unreadCount: int
     notifications: list[Notification]
     pagination: Pagination
 
 class r_GetRunSettings(Datatype):
@@ -273,139 +335,85 @@
     theme: Theme
     userList: list[User]
 
 class r_GetSession(Datatype):
     session: Session
 
 class r_GetThemeSettings(Datatype):
-    settings: ThemeSettings
-    theme: Theme
+    """NB: if no theme is set then this response will be empty"""
+    settings: OptField[ThemeSettings]
+    theme: OptField[Theme]
 
 class r_GetThreadReadStatus(Datatype):
     threadReadStatusList: list[ThreadReadStatus]
 
 class r_GetTickets(Datatype):
     ticketList: list[Ticket]
-    ticketNoteList: Any #TODO: document
+    ticketNoteList: list[TicketNote]
+    """Admins can see all notes, users can see messages here."""
     pagination: Pagination
     userList: list[User]
     gameList: list[Game]
+    userModCountList: list[UserCount]
+    userRunCountList: list[UserCount]
 
 class r_GetUserBlocks(Datatype):
     userBlocks: list[UserBlock]
 
 class r_GetUserSettings(Datatype):
     settings: UserSettings
     gameFollowerList: list[GameFollower]
     gameModeratorList: list[GameModerator]
     notificationSettings: list[NotificationSetting]
     userSocialConnectionList: list[UserSocialConnection]
     gameList: list[Game]
     themeList: list[Theme]
-    supporterCreditList: Any #TODO: document
-    supportCodeList: Any #TODO: document
-    supporterSubscription: Optional[Any]
+    titleList: list[Title]
+    supporterCreditList: list[SupporterCredit]
+    supporterCodeList: list[SupporterCode]
+    supporterSubscription: OptField[SupporterSubscription]
     experimentList: Any
     enabledExperimentIds: Any
 
 class r_GetUserSupporterData(Datatype):
     supporterEndDate: int
     boostEndDate: int
 
+class r_PutUserSupporterNewSubscription(Datatype):
+    subscription: SupporterSubscription
+    paymentIntentClientSecret: str
+
 class r_PutAuthLogin(Datatype):
     loggedIn: bool
-    tokenChallengeSent: Optional[bool]
-
-class r_PutAuthLogout(Datatype):
-    """No content"""
+    tokenChallengeSent: OptField[bool]
 
 class r_PutAuthSignup(Datatype):
     loggedIn: bool
-    tokenChallengeSent: Optional[bool]
-
-class r_PutComment(Datatype):
-    """No content"""
-
-class r_PutCommentableSettings(Datatype):
-    """No content"""
-
-class r_PutCommentDelete(Datatype):
-    """No content"""
-
-class r_PutCommentRestore(Datatype):
-    """No content"""
+    tokenChallengeSent: OptField[bool]
 
 class r_PutConversation(Datatype):
     ok: bool
     conversationId: str
     messageId: str
 
 class r_PutConversationMessage(Datatype):
     ok: bool
     conversationId: str
     messageId: str
 
 class r_PutGame(Datatype):
     game: Game
 
-class r_PutGameBoostGrant(Datatype):
-    """No content"""
-
-class r_PutGameModerator(Datatype):
-    """No content"""
-
-class r_PutGameModeratorDelete(Datatype):
-    """No content"""
-
-class r_PutGameSettings(Datatype):
-    """No content"""
-
-class r_PutRunAssignee(Datatype):
-    """No content"""
-
-class r_PutRunDelete(Datatype):
-    """No content"""
-
 class r_PutRunSettings(Datatype):
     runId: str
 
-class r_PutRunVerification(Datatype):
-    ok: bool
-
-class r_PutSeriesGame(Datatype):
-    """No content"""
-
-class r_PutSeriesGameDelete(Datatype):
-    """No content"""
-
-class r_PutSessionPing(Datatype):
-    """No content"""
-
 class r_PutThread(Datatype):
     thread: Thread
 
-class r_PutThreadDelete(Datatype):
-    """No content"""
-
-class r_PutThreadLocked(Datatype):
-    """No content"""
-
-class r_PutThreadRead(Datatype):
-    """No content"""
-
-class r_PutThreadSticky(Datatype):
-    """No content"""
-
 class r_PutTicket(Datatype):
     ticketId: str
 
 class r_PutUserSettings(Datatype):
     settings: UserSettings
 
-class r_PutUserSocialConnection(Datatype):
-    """No content"""
-
-class r_PutUserSocialConnectionDelete(Datatype):
-    """No content"""
-
 class r_PutUserUpdatePassword(Datatype):
-    ... #TODO: document
+    ...  # TODO: document
```

### Comparing `speedruncompy-0.3.3/src/speedruncompy/scripts/srcompy_login.py` & `speedruncompy-0.4.0/src/speedruncompy/scripts/srcompy_login.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,25 +1,26 @@
 """
-Basic script to login a new SRC session & get its session ID. 
+Basic script to login a new SRC session & get its session ID.
 
 Useful if you do not want to bother adding standard login code to your program & storing a username/password.
 
 Especially useful if you have 2FA enabled!
 """
 
 from speedruncompy import auth, api
 from getpass import getpass
 
 def main():
-    print("This script logs you in & returns a session ID for use with auth.lopinPHPSESSID()")
+    print("This script logs you in & returns a session ID for use with auth.loginPHPSESSID()")
     print("Please note that while your password is excluded from the terminal log, your PHPSESSID is not.")
     username = input("Enter username: ")
     password = getpass("Enter password: ")
-    loggedin = auth.login(username, password, tokenEntry = True)
+    loggedin = auth.login(username, password, tokenEntry=True)
     if not loggedin:
         print("Not logged in!")
         exit()
 
-    print(api._default.get_phpsessid())
+    print(api._default.PHPSESSID)
+
 
 if __name__ == "__main__":
     main()
```

### Comparing `speedruncompy-0.3.3/test/test_datatypes.py` & `speedruncompy-0.4.0/test/test_datatypes.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,101 +1,107 @@
 import asyncio
 import os
 from random import randint, sample
 
 from speedruncompy.datatypes import *
-from speedruncompy import datatypes
+from speedruncompy import config as srccfg
 from speedruncompy.endpoints import *
+from speedruncompy.exceptions import IncompleteDatatype
 
 from utils import check_datatype_coverage
 
 import pytest, pytest_asyncio, logging
 
 logging.getLogger().setLevel(logging.DEBUG)
 
-game_id = "76rqmld8" # Hollow Knight
-category_id = "02q8o4p2" # Any%
-challenge_id = "42ymr396" # Ghostrunner 2
+if "SKIP_HEAVY_TESTS" in os.environ:
+    SKIP_HEAVY_TESTS = bool(os.environ["SKIP_HEAVY_TESTS"])
+else:
+    SKIP_HEAVY_TESTS = True
+
+game_id = "76rqmld8"  # Hollow Knight
+category_id = "02q8o4p2"  # Any%
+challenge_id = "42ymr396"  # Ghostrunner 2
 
 # All tests are done with strict type conformance to catch errors early
 # In downstream this is default False, and warnings are given instead of errors.
 # See `TestDatatypes.test_Missing_Fields_Loose` for behaviour without STRICT.
-datatypes.STRICT_TYPE_CONFORMANCE = True
+srccfg.COERCION = 1
 
 @pytest.fixture()
 def loose_type_conformance():
-    datatypes.STRICT_TYPE_CONFORMANCE = False
+    srccfg.COERCION = 0
     yield
-    datatypes.STRICT_TYPE_CONFORMANCE = True
+    srccfg.COERCION = 1
 
 @pytest.fixture()
 def disable_type_checking():
-    datatypes.DISABLE_TYPE_CONFORMANCE = True
+    srccfg.COERCION = -1
     yield
-    datatypes.DISABLE_TYPE_CONFORMANCE = False
+    srccfg.COERCION = 1
 
 class TestDatatypes():
     def test_Datatype_conformance(self):
         """General dictlike conformance."""
         dt_raw = {"some": "data", "that's": True}
         different = {"some": "data", "that's": False}
         dt = Datatype(dt_raw)
-        assert dt["some"] == dt_raw["some"] # Dict access conformance
+        assert dt["some"] == dt_raw["some"]  # Dict access conformance
         with pytest.raises(KeyError): dt["a"]
-        assert dt == dt_raw # Equivalence
+        assert dt == dt_raw  # Equivalence
         assert not (dt == different)
-        assert not (dt != dt_raw) # Nonequivalence
+        assert not (dt != dt_raw)  # Nonequivalence
         assert dt != different
         
-        assert dt.some == "data" # Attribute get
-        dt.some = "different data" # Attribute set
+        assert dt.some == "data"  # Attribute get
+        dt.some = "different data"  # Attribute set
         assert dt.some == "different data"
         assert dt["some"] == "different data"
-        dt["some"] = "data" # Dictlike set
+        dt["some"] = "data"  # Dictlike set
         assert dt["some"] == "data"
         assert dt.some == "data"
         extra = {"new": "kvp"}
         dt |= extra
         assert "some" in dt
         assert "that's" in dt
         assert "new" in dt
 
     def test_Missing_Fields_Loose(self, caplog: pytest.LogCaptureFixture, loose_type_conformance: None):
         """Missing fields should raise a warning"""
         with caplog.at_level(logging.WARNING):
-            var_value_raw = {"variableId": "v"} # Missing valueId
+            var_value_raw = {"variableId": "v"}  # Missing valueId
             vv = VarValue(var_value_raw)
-            assert vv == var_value_raw # Construction still worked
+            assert vv == var_value_raw  # Construction still worked
         assert "Datatype VarValue constructed missing mandatory fields ['valueId']" in caplog.text
 
     def test_Missing_Fields(self):
         """Missing fields should raise an error in Strict mode"""
-        var_value_raw = {"variableId": "v"} # Missing valueId
+        var_value_raw = {"variableId": "v"}  # Missing valueId
         with pytest.raises(IncompleteDatatype):
-            VarValue(var_value_raw) # Construction fails due to strictness
+            VarValue(var_value_raw)  # Construction fails due to strictness
 
     raw_run_settings = {"runId": "a", "gameId": "b", "categoryId": "c",
-            "playerNames": ["p"],
-            "time": {"hour": 0, "minute": 1, "second": 2, "millisecond": 3},
-            "platformId": "p", "emulator": False,
-            "video": "url", "comment": "comment", "date": 11111,
-            "values": [{"variableId": "38dopp1l", "valueId": "4lxogy4l"},
-                {"variableId": "onvkzmlm", "valueId": "gq7o3rnl"}]}
+                        "playerNames": ["p"],
+                        "time": {"hour": 0, "minute": 1, "second": 2, "millisecond": 3},
+                        "platformId": "p", "emulator": False,
+                        "video": "url", "comment": "comment", "date": 11111,
+                        "values": [{"variableId": "38dopp1l", "valueId": "4lxogy4l"},
+                                   {"variableId": "onvkzmlm", "valueId": "gq7o3rnl"}]}
     
     def test_RunSettings(self, caplog: pytest.LogCaptureFixture):
         raw = self.raw_run_settings.copy()
-        settings = RunSettings(raw) # Does not fail w/ strict typechecking, as missing field timeWithLoads is opt
+        settings = RunSettings(raw)  # Does not fail w/ strict typechecking, as missing field timeWithLoads is opt
 
-        assert settings.timeWithLoads is None # Missing attribute defaults to None
+        assert settings.timeWithLoads is None  # Missing attribute defaults to None
         with pytest.raises(AttributeError, match="'RunSettings' object has no attribute 'aaaa'"):
-            settings.aaaa # Nonexistant attribute still raises AttributeError
+            settings.aaaa  # Nonexistant attribute still raises AttributeError
         
         assert isinstance(settings.values[0], VarValue)
 
-@pytest.mark.skipif("SKIP_HEAVY_TESTS" in os.environ, reason="Skip on automated runs")
+@pytest.mark.skipif(SKIP_HEAVY_TESTS, reason="SKIP_HEAVY_TESTS == True")
 class TestDatatypes_Integration_Heavy():
     """
     Heavy testing meant to be semi-exhaustive, that will most likely hit rate limits on repeat runs.
 
     Call list:
     GetGameList: all pages (<100) + 1 random page
     GetGameData: 200
@@ -128,15 +134,15 @@
         return overall
     
     @pytest_asyncio.fixture(scope="session")
     async def small_game_subset_leaderboards(self, small_game_subset_categories: list[tuple[r_GetGameData, str]]) -> list[r_GetGameLeaderboard2]:
         """1 leaderboard per game, 1 page per board (to avoid rate limit on an average > 2 boards per game)"""
         return await asyncio.gather(*[GetGameLeaderboard2(gameId=g.game.id, categoryId=c).perform_async() for g, c in small_game_subset_categories])
 
-    def test_Runs(self, small_game_subset_leaderboards: list[r_GetGameLeaderboard2]):        
+    def test_Runs(self, small_game_subset_leaderboards: list[r_GetGameLeaderboard2]):
         for board in small_game_subset_leaderboards:
             for run in board.runList:
                 check_datatype_coverage(run)
     
     def test_Challenge_Runs(self):
         source = GetChallengeLeaderboard(challenge_id).perform()
         if len(source.challengeRunList) == 0: return
@@ -167,8 +173,8 @@
         for board in small_game_subset_leaderboards:
             for player in board.playerList:
                 check_datatype_coverage(player)
 
     def test_User(self):
         source = GetChallengeLeaderboard(challenge_id).perform()
         for user in source.userList:
-            check_datatype_coverage(user)
+            check_datatype_coverage(user)
```

### Comparing `speedruncompy-0.3.3/test/utils.py` & `speedruncompy-0.4.0/test/utils.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,33 +1,30 @@
-from typing import get_origin, get_args, Optional, Union, get_type_hints
+from types import NoneType
+from typing import get_origin, get_args, get_type_hints
 from speedruncompy.datatypes import Datatype
+from speedruncompy.datatypes._impl import _OptFieldMarker, degrade_union
 
 def get_true_type(t: type):
-    origin = get_origin(t)
-    if origin is None: return t
-    else:
-        args = get_args(t)
-        if origin is Union or origin is Optional:
-            return args[0]
-        else:
-            return origin
+    return degrade_union(t, NoneType, _OptFieldMarker)
 
 def check_datatype_coverage(dt: Datatype):
     keys = set(dt.keys())
-    hints = get_type_hints(dt)
+    try:
+        hints = get_type_hints(dt)
+    except TypeError: hints = dict()  # Errors on empty datatype
     hintNames = set(hints)
     unseenAttrs = keys.difference(hintNames)
     assert unseenAttrs == set(), f"{type(dt)} missing keys: {[a + ' = ' + str(dt[a]) for a in unseenAttrs]}"
     for attr, subtype in hints.items():
         true = get_true_type(subtype)
         if issubclass(true, Datatype):
             if dt[attr] is not None:
                 check_datatype_coverage(dt[attr])
-        elif true is list:
+        elif get_origin(true) is list:
             list_type = get_args(subtype)[0]
             if issubclass(list_type, Datatype):
                 for item in dt[attr]:
                     check_datatype_coverage(item)
 
 def check_pages(pages: dict[int, Datatype]):
     for p, page in pages.items():
-        check_datatype_coverage(page)
+        check_datatype_coverage(page)
```

### Comparing `speedruncompy-0.3.3/LICENSE` & `speedruncompy-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `speedruncompy-0.3.3/pyproject.toml` & `speedruncompy-0.4.0/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -33,15 +33,16 @@
 packages = [
     "src/speedruncompy"
 ]
 
 [project.optional-dependencies]
 test = [
     "pytest",
-    "pytest-asyncio"
+    "pytest-asyncio",
+    "pytest-cov"
 ]
 
 [project.urls]
 Homepage = "https://github.com/ManicJamie/speedruncompy"
 Repository = "https://github.com/ManicJamie/speedruncompy.git"
 "Bug Tracker" = "https://github.com/ManicJamie/speedruncompy/issues"
```

