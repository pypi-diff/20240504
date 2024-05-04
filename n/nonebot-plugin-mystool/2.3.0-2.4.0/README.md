# Comparing `tmp/nonebot_plugin_mystool-2.3.0.tar.gz` & `tmp/nonebot_plugin_mystool-2.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_mystool-2.3.0.tar", max compression
+gzip compressed data, was "nonebot_plugin_mystool-2.4.0.tar", max compression
```

## Comparing `nonebot_plugin_mystool-2.3.0.tar` & `nonebot_plugin_mystool-2.4.0.tar`

### file list

```diff
@@ -1,31 +1,31 @@
--rw-r--r--   0        0        0     1065 2024-03-16 19:21:00.467337 nonebot_plugin_mystool-2.3.0/LICENSE
--rw-r--r--   0        0        0     3511 2024-03-16 19:21:00.467337 nonebot_plugin_mystool-2.3.0/README.md
--rw-r--r--   0        0        0     1850 2024-03-16 19:21:00.467337 nonebot_plugin_mystool-2.3.0/pyproject.toml
--rw-r--r--   0        0        0     2196 2024-03-16 19:21:00.467337 nonebot_plugin_mystool-2.3.0/src/nonebot_plugin_mystool/__init__.py
--rw-r--r--   0        0        0       23 2024-03-16 19:21:00.467337 nonebot_plugin_mystool-2.3.0/src/nonebot_plugin_mystool/_version.py
--rw-r--r--   0        0        0       61 2024-03-16 19:21:00.467337 nonebot_plugin_mystool-2.3.0/src/nonebot_plugin_mystool/api/__init__.py
--rw-r--r--   0        0        0    76471 2024-03-16 19:21:00.467337 nonebot_plugin_mystool-2.3.0/src/nonebot_plugin_mystool/api/common.py
--rw-r--r--   0        0        0    11733 2024-03-16 19:21:00.467337 nonebot_plugin_mystool-2.3.0/src/nonebot_plugin_mystool/api/game_sign_api.py
--rw-r--r--   0        0        0    23891 2024-03-16 19:21:00.467337 nonebot_plugin_mystool-2.3.0/src/nonebot_plugin_mystool/api/myb_missions_api.py
--rw-r--r--   0        0        0     4509 2024-03-16 19:21:00.467337 nonebot_plugin_mystool-2.3.0/src/nonebot_plugin_mystool/api/weibo.py
--rw-r--r--   0        0        0      179 2024-03-16 19:21:00.467337 nonebot_plugin_mystool-2.3.0/src/nonebot_plugin_mystool/command/__init__.py
--rw-r--r--   0        0        0     4372 2024-03-16 19:21:00.467337 nonebot_plugin_mystool-2.3.0/src/nonebot_plugin_mystool/command/address.py
--rw-r--r--   0        0        0      662 2024-03-16 19:21:00.467337 nonebot_plugin_mystool-2.3.0/src/nonebot_plugin_mystool/command/common.py
--rw-r--r--   0        0        0    24020 2024-03-16 19:21:00.471336 nonebot_plugin_mystool-2.3.0/src/nonebot_plugin_mystool/command/exchange.py
--rw-r--r--   0        0        0     2739 2024-03-16 19:21:00.471336 nonebot_plugin_mystool-2.3.0/src/nonebot_plugin_mystool/command/help.py
--rw-r--r--   0        0        0    13899 2024-03-16 19:21:00.471336 nonebot_plugin_mystool-2.3.0/src/nonebot_plugin_mystool/command/login.py
--rw-r--r--   0        0        0    35608 2024-03-16 19:21:00.471336 nonebot_plugin_mystool-2.3.0/src/nonebot_plugin_mystool/command/plan.py
--rw-r--r--   0        0        0    12588 2024-03-16 19:21:00.471336 nonebot_plugin_mystool-2.3.0/src/nonebot_plugin_mystool/command/setting.py
--rw-r--r--   0        0        0    12523 2024-03-16 19:21:00.471336 nonebot_plugin_mystool-2.3.0/src/nonebot_plugin_mystool/command/user_check.py
--rw-r--r--   0        0        0       64 2024-03-16 19:21:00.471336 nonebot_plugin_mystool-2.3.0/src/nonebot_plugin_mystool/model/__init__.py
--rw-r--r--   0        0        0    17184 2024-03-16 19:21:00.471336 nonebot_plugin_mystool-2.3.0/src/nonebot_plugin_mystool/model/common.py
--rw-r--r--   0        0        0    10762 2024-03-16 19:21:00.471336 nonebot_plugin_mystool-2.3.0/src/nonebot_plugin_mystool/model/config.py
--rw-r--r--   0        0        0    17518 2024-03-16 19:21:00.471336 nonebot_plugin_mystool-2.3.0/src/nonebot_plugin_mystool/model/data.py
--rw-r--r--   0        0        0       22 2024-03-16 19:21:00.471336 nonebot_plugin_mystool-2.3.0/src/nonebot_plugin_mystool/model/upgrade/__init__.py
--rw-r--r--   0        0        0     5004 2024-03-16 19:21:00.471336 nonebot_plugin_mystool-2.3.0/src/nonebot_plugin_mystool/model/upgrade/common.py
--rw-r--r--   0        0        0     9484 2024-03-16 19:21:00.471336 nonebot_plugin_mystool-2.3.0/src/nonebot_plugin_mystool/model/upgrade/configV2.py
--rw-r--r--   0        0        0    16456 2024-03-16 19:21:00.471336 nonebot_plugin_mystool-2.3.0/src/nonebot_plugin_mystool/model/upgrade/dataV2.py
--rw-r--r--   0        0        0       48 2024-03-16 19:21:00.471336 nonebot_plugin_mystool-2.3.0/src/nonebot_plugin_mystool/utils/__init__.py
--rw-r--r--   0        0        0    15757 2024-03-16 19:21:00.471336 nonebot_plugin_mystool-2.3.0/src/nonebot_plugin_mystool/utils/common.py
--rw-r--r--   0        0        0     5622 2024-03-16 19:21:00.471336 nonebot_plugin_mystool-2.3.0/src/nonebot_plugin_mystool/utils/good_image.py
--rw-r--r--   0        0        0     5270 1970-01-01 00:00:00.000000 nonebot_plugin_mystool-2.3.0/PKG-INFO
+-rw-r--r--   0        0        0     1065 2024-05-04 14:16:17.911417 nonebot_plugin_mystool-2.4.0/LICENSE
+-rw-r--r--   0        0        0     2679 2024-05-04 14:16:17.911417 nonebot_plugin_mystool-2.4.0/README.md
+-rw-r--r--   0        0        0     1850 2024-05-04 14:16:17.911417 nonebot_plugin_mystool-2.4.0/pyproject.toml
+-rw-r--r--   0        0        0     2316 2024-05-04 14:16:17.911417 nonebot_plugin_mystool-2.4.0/src/nonebot_plugin_mystool/__init__.py
+-rw-r--r--   0        0        0       23 2024-05-04 14:16:17.911417 nonebot_plugin_mystool-2.4.0/src/nonebot_plugin_mystool/_version.py
+-rw-r--r--   0        0        0       61 2024-05-04 14:16:17.911417 nonebot_plugin_mystool-2.4.0/src/nonebot_plugin_mystool/api/__init__.py
+-rw-r--r--   0        0        0    85119 2024-05-04 14:16:17.911417 nonebot_plugin_mystool-2.4.0/src/nonebot_plugin_mystool/api/common.py
+-rw-r--r--   0        0        0    11733 2024-05-04 14:16:17.911417 nonebot_plugin_mystool-2.4.0/src/nonebot_plugin_mystool/api/game_sign_api.py
+-rw-r--r--   0        0        0    23943 2024-05-04 14:16:17.911417 nonebot_plugin_mystool-2.4.0/src/nonebot_plugin_mystool/api/myb_missions_api.py
+-rw-r--r--   0        0        0     5365 2024-05-04 14:16:17.911417 nonebot_plugin_mystool-2.4.0/src/nonebot_plugin_mystool/api/weibo.py
+-rw-r--r--   0        0        0      179 2024-05-04 14:16:17.911417 nonebot_plugin_mystool-2.4.0/src/nonebot_plugin_mystool/command/__init__.py
+-rw-r--r--   0        0        0     4372 2024-05-04 14:16:17.911417 nonebot_plugin_mystool-2.4.0/src/nonebot_plugin_mystool/command/address.py
+-rw-r--r--   0        0        0      662 2024-05-04 14:16:17.911417 nonebot_plugin_mystool-2.4.0/src/nonebot_plugin_mystool/command/common.py
+-rw-r--r--   0        0        0    24207 2024-05-04 14:16:17.915417 nonebot_plugin_mystool-2.4.0/src/nonebot_plugin_mystool/command/exchange.py
+-rw-r--r--   0        0        0     2739 2024-05-04 14:16:17.915417 nonebot_plugin_mystool-2.4.0/src/nonebot_plugin_mystool/command/help.py
+-rw-r--r--   0        0        0    12213 2024-05-04 14:16:17.915417 nonebot_plugin_mystool-2.4.0/src/nonebot_plugin_mystool/command/login.py
+-rw-r--r--   0        0        0    36439 2024-05-04 14:16:17.915417 nonebot_plugin_mystool-2.4.0/src/nonebot_plugin_mystool/command/plan.py
+-rw-r--r--   0        0        0    14755 2024-05-04 14:16:17.915417 nonebot_plugin_mystool-2.4.0/src/nonebot_plugin_mystool/command/setting.py
+-rw-r--r--   0        0        0    12523 2024-05-04 14:16:17.915417 nonebot_plugin_mystool-2.4.0/src/nonebot_plugin_mystool/command/user_check.py
+-rw-r--r--   0        0        0       64 2024-05-04 14:16:17.915417 nonebot_plugin_mystool-2.4.0/src/nonebot_plugin_mystool/model/__init__.py
+-rw-r--r--   0        0        0    17494 2024-05-04 14:16:17.915417 nonebot_plugin_mystool-2.4.0/src/nonebot_plugin_mystool/model/common.py
+-rw-r--r--   0        0        0    11248 2024-05-04 14:16:17.915417 nonebot_plugin_mystool-2.4.0/src/nonebot_plugin_mystool/model/config.py
+-rw-r--r--   0        0        0    17776 2024-05-04 14:16:17.915417 nonebot_plugin_mystool-2.4.0/src/nonebot_plugin_mystool/model/data.py
+-rw-r--r--   0        0        0       22 2024-05-04 14:16:17.915417 nonebot_plugin_mystool-2.4.0/src/nonebot_plugin_mystool/model/upgrade/__init__.py
+-rw-r--r--   0        0        0     5004 2024-05-04 14:16:17.915417 nonebot_plugin_mystool-2.4.0/src/nonebot_plugin_mystool/model/upgrade/common.py
+-rw-r--r--   0        0        0     9484 2024-05-04 14:16:17.915417 nonebot_plugin_mystool-2.4.0/src/nonebot_plugin_mystool/model/upgrade/configV2.py
+-rw-r--r--   0        0        0    16456 2024-05-04 14:16:17.915417 nonebot_plugin_mystool-2.4.0/src/nonebot_plugin_mystool/model/upgrade/dataV2.py
+-rw-r--r--   0        0        0       48 2024-05-04 14:16:17.915417 nonebot_plugin_mystool-2.4.0/src/nonebot_plugin_mystool/utils/__init__.py
+-rw-r--r--   0        0        0    16124 2024-05-04 14:16:17.915417 nonebot_plugin_mystool-2.4.0/src/nonebot_plugin_mystool/utils/common.py
+-rw-r--r--   0        0        0     5622 2024-05-04 14:16:17.915417 nonebot_plugin_mystool-2.4.0/src/nonebot_plugin_mystool/utils/good_image.py
+-rw-r--r--   0        0        0     4438 1970-01-01 00:00:00.000000 nonebot_plugin_mystool-2.4.0/PKG-INFO
```

### Comparing `nonebot_plugin_mystool-2.3.0/LICENSE` & `nonebot_plugin_mystool-2.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_mystool-2.3.0/pyproject.toml` & `nonebot_plugin_mystool-2.4.0/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "nonebot-plugin-mystool"
-version = "v2.3.0"
+version = "v2.4.0"
 description = "QQ聊天、频道机器人插件 | 米游社工具-每日米游币任务、游戏签到、商品兑换、免抓包登录、原神崩铁便笺提醒"
 license = "MIT"
 authors = [
   "Ljzd-PRO <ljzd@office.ljzd-pro.asia>",
   "Everything0519 <598139245@qq.com>"
 ]
 readme = "README.md"
```

### Comparing `nonebot_plugin_mystool-2.3.0/src/nonebot_plugin_mystool/__init__.py` & `nonebot_plugin_mystool-2.4.0/src/nonebot_plugin_mystool/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,14 +11,15 @@
     "\n📦 {HEAD}地址 ➢ 设置收货地址ID"
     "\n🗓️ {HEAD}签到 ➢ 手动进行游戏签到"
     "\n📅 {HEAD}任务 ➢ 手动执行米游币任务"
     "\n🛒 {HEAD}兑换 ➢ 米游币商品兑换相关"
     "\n🎁 {HEAD}商品 ➢ 查看米游币商品信息(商品ID)"
     "\n📊 {HEAD}原神便笺 ➢ 查看原神实时便笺(原神树脂、洞天财瓮等)"
     "\n📊 {HEAD}铁道便笺 ➢ 查看星穹铁道实时便笺(开拓力、每日实训等)"
+    "\n👁️‍🗨️ {HEAD}wb兑换 ➢ 查看微博本期超话签到的兑换码(暂支持原神和星穹铁道)"
     "\n⚙️ {HEAD}设置 ➢ 设置是否开启通知、每日任务等相关选项"
     "\n🔑 {HEAD}账号设置 ➢ 设置设备平台、是否开启每日计划任务、频道任务"
     "\n🔔 {HEAD}通知设置 ➢ 设置是否开启每日米游币任务、游戏签到的结果通知"
     "\n🖨️ {HEAD}导出Cookies ➢ 导出绑定的米游社账号的Cookies数据"
     "\n🖇️ {HEAD}用户绑定 ➢ 绑定关联其他聊天平台或其他账号的用户数据"
     "\n📨 {HEAD}私信响应 ➢ 让机器人发送一条私信给你，主要用于QQ频道"
     "\n📖 {HEAD}帮助 ➢ 查看帮助信息"
```

### Comparing `nonebot_plugin_mystool-2.3.0/src/nonebot_plugin_mystool/api/common.py` & `nonebot_plugin_mystool-2.4.0/src/nonebot_plugin_mystool/api/common.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,22 @@
+import json
 import time
 from typing import List, Optional, Tuple, Dict, Any, Union, Type
-from urllib.parse import urlencode
+from urllib.parse import urlencode, urlparse, parse_qs
 
 import httpx
 import tenacity
 from pydantic import ValidationError, BaseModel
 from requests.utils import dict_from_cookiejar
 
 from ..model import GameRecord, GameInfo, Good, Address, BaseApiStatus, MmtData, GeetestResult, \
     GetCookieStatus, \
     CreateMobileCaptchaStatus, GetGoodDetailStatus, ExchangeStatus, GeetestResultV4, GenshinNote, GenshinNoteStatus, \
     GetFpStatus, StarRailNoteStatus, StarRailNote, UserAccount, BBSCookies, ExchangePlan, ExchangeResult, plugin_env, \
-    plugin_config
+    plugin_config, QueryGameTokenQrCodeStatus
 from ..utils import generate_device_id, logger, generate_ds, \
     get_async_retry, generate_seed_id, generate_fp_locally
 
 URL_LOGIN_TICKET_BY_CAPTCHA = "https://webapi.account.mihoyo.com/Api/login_by_mobilecaptcha"
 URL_LOGIN_TICKET_BY_PASSWORD = "https://webapi.account.mihoyo.com/Api/login_by_password"
 URL_MULTI_TOKEN_BY_LOGIN_TICKET = ("https://api-takumi.mihoyo.com/auth/api/getMultiTokenByLoginTicket?login_ticket={0}"
                                    "&token_types=3&uid={1}")
@@ -43,14 +44,18 @@
 URL_GET_DEVICE_FP = "https://public-data-api.mihoyo.com/device-fp/api/getFp"
 URL_GENSHEN_NOTE_BBS = "https://api-takumi-record.mihoyo.com/game_record/app/genshin/api/dailyNote"
 URL_GENSHEN_NOTE_WIDGET = "https://api-takumi-record.mihoyo.com/game_record/genshin/aapi/widget/v2"
 URL_STARRAIL_NOTE_BBS = "https://api-takumi-record.mihoyo.com/game_record/app/hkrpg/api/note"
 URL_STARRAIL_NOTE_WIDGET = "https://api-takumi-record.mihoyo.com/game_record/app/hkrpg/aapi/widget"
 URL_CREATE_VERIFICATION = "https://bbs-api.miyoushe.com/misc/api/createVerification?is_high=true"
 URL_VERIFY_VERIFICATION = "https://bbs-api.miyoushe.com/misc/api/verifyVerification"
+URL_FETCH_GAME_TOKEN_QRCODE = "https://hk4e-sdk.mihoyo.com/hk4e_cn/combo/panda/qrcode/fetch"
+URL_QUERY_GAME_TOKEN_QRCODE = "https://hk4e-sdk.mihoyo.com/hk4e_cn/combo/panda/qrcode/query"
+URL_GET_TOKEN_BY_GAME_TOKEN = "https://api-takumi.mihoyo.com/account/ma-cn-session/app/getTokenByGameToken"
+URL_GET_COOKIE_TOKEN_BY_GAME_TOKEN = "https://api-takumi.mihoyo.com/auth/api/getCookieAccountInfoByGameToken"
 
 HEADERS_WEBAPI = {
     "Host": "webapi.account.mihoyo.com",
     "Connection": "keep-alive",
     "sec-ch-ua": plugin_env.device_config.UA,
     "DNT": "1",
     "x-rpc-device_model": plugin_env.device_config.X_RPC_DEVICE_MODEL_PC,
@@ -333,17 +338,17 @@
 
     def __init__(self, content: Dict[str, Any]):
         super().__init__(content=content)
 
         self.data = self.content.get("data")
 
         for key in ["retcode", "status"]:
-            if not self.retcode:
+            if self.retcode is None:
                 self.retcode = self.content.get(key)
-                if not self.retcode:
+                if self.retcode is None:
                     self.retcode = self.data.get(key) if self.data else None
 
         self.message: Optional[str] = None
         for key in ["message", "msg"]:
             if not self.message:
                 self.message = self.content.get(key)
                 if not self.message:
@@ -1675,7 +1680,194 @@
         if is_incorrect_return(e):
             logger.exception("验证人机验证结果(verify_verification) - 服务器没有正确返回")
             logger.debug(f"网络请求返回: {res.text}")
             return BaseApiStatus(incorrect_return=True)
         else:
             logger.exception("验证人机验证结果(verify_verification) - 请求失败")
             return BaseApiStatus(network_error=True)
+
+
+async def fetch_game_token_qrcode(
+        device_id: str,
+        app_id: str = "1",
+        retry: bool = True
+) -> Tuple[BaseApiStatus, Optional[Tuple[str, str]]]:
+    """
+    获取米游社扫码登录（GameToken）二维码
+
+    :param device_id: 设备ID
+    :param app_id: 登录的应用标识符
+    :param retry: 是否允许重试
+    :return 其中 ``Tuple[str, str]`` 为二维码URL和用于查询二维码扫描状态的 ``token``
+    """
+    try:
+        async for attempt in get_async_retry(retry):
+            with attempt:
+                content = {
+                    "app_id": app_id,
+                    "device": device_id,
+                }
+                async with httpx.AsyncClient() as client:
+                    res = await client.post(
+                        URL_FETCH_GAME_TOKEN_QRCODE,
+                        json=content,
+                        timeout=plugin_config.preference.timeout
+                    )
+                api_result = ApiResultHandler(res.json())
+                if api_result.retcode == 0:
+                    qrcode_url = api_result.data["url"]
+                    url = urlparse(qrcode_url)
+                    return BaseApiStatus(success=True), (qrcode_url, parse_qs(url.query)["ticket"][0])
+                else:
+                    logger.debug(f"网络请求返回: {res.text}")
+                    return BaseApiStatus(), None
+    except tenacity.RetryError as e:
+        if is_incorrect_return(e):
+            logger.exception("获取米游社扫码登录(fetch_game_token_qrcode) - 服务器没有正确返回")
+            logger.debug(f"网络请求返回: {res.text}")
+            return BaseApiStatus(incorrect_return=True), None
+        else:
+            logger.exception("获取米游社扫码登录(fetch_game_token_qrcode) - 请求失败")
+            return BaseApiStatus(network_error=True), None
+
+
+async def query_game_token_qrcode(
+        ticket: str,
+        device_id: str,
+        app_id: str = "1",
+        retry: bool = True
+) -> Tuple[QueryGameTokenQrCodeStatus, Optional[Tuple[str, str]]]:
+    """
+    查询米游社扫码登录（GameToken）二维码扫描状态
+
+    :param ticket: 生成二维码时返回的 URL 参数中 ``ticket`` 字段的值
+    :param device_id: 设备ID
+    :param app_id: 登录的应用标识符
+    :param retry: 是否允许重试
+    :return 其中 ``Tuple[str, str]`` 为米游社账号ID和 GameToken
+    """
+    try:
+        async for attempt in get_async_retry(retry):
+            with attempt:
+                content = {
+                    "app_id": app_id,
+                    "device": device_id,
+                    "ticket": ticket
+                }
+                async with httpx.AsyncClient() as client:
+                    res = await client.post(
+                        URL_QUERY_GAME_TOKEN_QRCODE,
+                        json=content,
+                        timeout=plugin_config.preference.timeout
+                    )
+                api_result = ApiResultHandler(res.json())
+                if api_result.retcode == 0:
+                    if api_result.data["stat"] == "Init":
+                        return QueryGameTokenQrCodeStatus(qrcode_init=True), None
+                    elif api_result.data["stat"] == "Scanned":
+                        return QueryGameTokenQrCodeStatus(qrcode_scanned=True), None
+                    else:
+                        payload_raw = api_result.data["payload"]["raw"]
+                        parsed_payload: Dict[str, str] = json.loads(payload_raw)
+                        return QueryGameTokenQrCodeStatus(success=True), (
+                            parsed_payload["uid"],
+                            parsed_payload["token"]
+                        )
+                elif api_result.retcode == -106:
+                    return QueryGameTokenQrCodeStatus(qrcode_expired=True), None
+                else:
+                    return QueryGameTokenQrCodeStatus(), None
+    except tenacity.RetryError as e:
+        if is_incorrect_return(e):
+            logger.exception("查询米游社扫码登录(query_game_token_qrcode) - 服务器没有正确返回")
+            logger.debug(f"网络请求返回: {res.text}")
+            return QueryGameTokenQrCodeStatus(incorrect_return=True), None
+        else:
+            logger.exception("查询米游社扫码登录(query_game_token_qrcode) - 请求失败")
+            return QueryGameTokenQrCodeStatus(network_error=True), None
+
+
+async def get_token_by_game_token(
+        bbs_uid: str,
+        game_token: str,
+        retry: bool = True
+) -> Tuple[BaseApiStatus, Optional[BBSCookies]]:
+    """
+    通过 GameToken 获取 STokenV2 和 mid
+
+    :param bbs_uid: 米游社账号 UID
+    :param game_token: 有效的 GameToken
+    :param retry: 是否允许重试
+    """
+    try:
+        async for attempt in get_async_retry(retry):
+            with attempt:
+                content = {
+                    "account_id": int(bbs_uid),
+                    "game_token": game_token
+                }
+                async with httpx.AsyncClient() as client:
+                    res = await client.post(
+                        URL_GET_TOKEN_BY_GAME_TOKEN,
+                        headers={"x-rpc-app_id": "bll8iq97cem8"},
+                        json=content,
+                        timeout=plugin_config.preference.timeout
+                    )
+                api_result = ApiResultHandler(res.json())
+                if api_result.retcode == 0:
+                    stoken_v2 = api_result.data["token"]["token"]
+                    mid = api_result.data["user_info"]["mid"]
+                    return BaseApiStatus(success=True), BBSCookies(stoken_v2=stoken_v2, mid=mid)
+                else:
+                    logger.debug(f"网络请求返回: {res.text}")
+                    return BaseApiStatus(), None
+    except tenacity.RetryError as e:
+        if is_incorrect_return(e):
+            logger.exception("通过 GameToken 获取 SToken(get_token_by_game_token) - 服务器没有正确返回")
+            logger.debug(f"网络请求返回: {res.text}")
+            return BaseApiStatus(incorrect_return=True), None
+        else:
+            logger.exception("通过 GameToken 获取 SToken(get_token_by_game_token) - 请求失败")
+            return BaseApiStatus(network_error=True), None
+
+
+async def get_cookie_token_by_game_token(
+        bbs_uid: str,
+        game_token: str,
+        retry: bool = True
+) -> Tuple[BaseApiStatus, Optional[BBSCookies]]:
+    """
+    通过 GameToken 获取 CookieToken
+
+    :param bbs_uid: 米游社账号 UID
+    :param game_token: 有效的 GameToken
+    :param retry: 是否允许重试
+    """
+    try:
+        async for attempt in get_async_retry(retry):
+            with attempt:
+                content = {
+                    "account_id": int(bbs_uid),
+                    "game_token": game_token
+                }
+                async with httpx.AsyncClient() as client:
+                    res = await client.post(
+                        URL_GET_COOKIE_TOKEN_BY_GAME_TOKEN,
+                        headers={"x-rpc-app_id": "bll8iq97cem8"},
+                        json=content,
+                        timeout=plugin_config.preference.timeout
+                    )
+                api_result = ApiResultHandler(res.json())
+                if api_result.retcode == 0:
+                    cookie_token = api_result.data["token"]["token"]
+                    return BaseApiStatus(success=True), BBSCookies(cookie_token=cookie_token)
+                else:
+                    logger.debug(f"网络请求返回: {res.text}")
+                    return BaseApiStatus(), None
+    except tenacity.RetryError as e:
+        if is_incorrect_return(e):
+            logger.exception("通过 GameToken 获取 CookieToken(get_cookie_token_by_game_token) - 服务器没有正确返回")
+            logger.debug(f"网络请求返回: {res.text}")
+            return BaseApiStatus(incorrect_return=True), None
+        else:
+            logger.exception("通过 GameToken 获取 CookieToken(get_cookie_token_by_game_token) - 请求失败")
+            return BaseApiStatus(network_error=True), None
```

### Comparing `nonebot_plugin_mystool-2.3.0/src/nonebot_plugin_mystool/api/game_sign_api.py` & `nonebot_plugin_mystool-2.4.0/src/nonebot_plugin_mystool/api/game_sign_api.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_mystool-2.3.0/src/nonebot_plugin_mystool/api/myb_missions_api.py` & `nonebot_plugin_mystool-2.4.0/src/nonebot_plugin_mystool/api/myb_missions_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 import httpx
 import tenacity
 
 from ..api.common import ApiResultHandler, is_incorrect_return, create_verification, \
     verify_verification
 from ..model import BaseApiStatus, MissionStatus, MissionData, \
-    MissionState, UserAccount, plugin_config, plugin_env
+    MissionState, UserAccount, plugin_config, plugin_env, UserData
 from ..utils import logger, generate_ds, \
     get_async_retry, get_validate
 
 URL_SIGN = "https://bbs-api.mihoyo.com/apihub/app/api/signIn"
 URL_GET_POST = "https://bbs-api.miyoushe.com/post/api/feeds/posts?fresh_action=1&gids={}&is_first_initialize=false" \
                "&last_id="
 URL_READ = "https://bbs-api.miyoushe.com/post/api/getPostFull?post_id={}"
@@ -105,15 +105,15 @@
 
         :param account: 账号对象
         """
         self.account = account
         self.headers = HEADERS_BASE.copy()
         self.headers["x-rpc-device_id"] = account.device_id_android
 
-    async def sign(self, retry: bool = True) -> Tuple[MissionStatus, Optional[int]]:
+    async def sign(self, user: UserData, retry: bool = True) -> Tuple[MissionStatus, Optional[int]]:
         """
         签到
 
         :param retry: 是否允许重试
         :return: (BaseApiStatus, 签到获得的米游币数量)
         """
         content = {"gids": self.gids}
@@ -142,18 +142,18 @@
                             f"米游币任务 - 讨论区签到: 用户 {self.account.display_name} DS 校验失败")
                         logger.debug(f"网络请求返回: {res.text}")
                         return MissionStatus(invalid_ds=True), None
                     elif api_result.retcode == 1034:
                         logger.error(
                             f"米游币任务 - 讨论区签到: 用户 {self.account.display_name} 需要完成人机验证")
                         logger.debug(f"网络请求返回: {res.text}")
-                        if plugin_config.preference.geetest_url:
+                        if plugin_config.preference.geetest_url or user.geetest_url:
                             create_status, mmt_data = await create_verification(self.account)
                             if create_status:
-                                if geetest_result := await get_validate(mmt_data.gt, mmt_data.challenge):
+                                if geetest_result := await get_validate(user, mmt_data.gt, mmt_data.challenge):
                                     if await verify_verification(mmt_data, geetest_result, self.account):
                                         logger.success(
                                             f"米游币任务 - 讨论区签到: 用户 {self.account.display_name} 人机验证通过")
                                         continue
                         else:
                             logger.info(
                                 f"米游币任务 - 讨论区签到: 用户 {self.account.display_name} 未配置极验人机验证打码平台")
```

### Comparing `nonebot_plugin_mystool-2.3.0/src/nonebot_plugin_mystool/api/weibo.py` & `nonebot_plugin_mystool-2.4.0/src/nonebot_plugin_mystool/api/weibo.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,13 +1,14 @@
+import random
 import re
 from urllib.parse import unquote
 
 import httpx
 
-from ..model import UserAccount
+from ..model import UserData
 from ..utils import logger
 
 
 def cookie_to_dict(cookie):
     if cookie and '=' in cookie:
         cookie = dict([line.strip().split('=', 1) for line in cookie.split(';')])
     return cookie
@@ -35,20 +36,20 @@
                 else:
                     yield v
             if isinstance(v, (list, dict)):
                 yield from _nested_lookup(v, key, with_keys=with_keys)
 
 
 class WeiboCode:
-    def __init__(self, account: UserAccount):
+    def __init__(self, account: UserData):
         self.params = cookie_to_dict(account.weibo_params.replace('&', ';')) if account.weibo_params else None
         """params: s=xxxxxx; gsid=xxxxxx; aid=xxxxxx; from=xxxxxx"""
         self.cookie = cookie_to_dict(account.weibo_cookie)
         self.container_id = {'原神': '100808fc439dedbb06ca5fd858848e521b8716',
-                             '星铁': '100808e1f868bf9980f09ab6908787d7eaf0f0'}
+                             '崩铁': '100808e1f868bf9980f09ab6908787d7eaf0f0'}
         self.ua = 'WeiboOverseas/4.4.6 (iPhone; iOS 14.0.1; Scale/2.00)'
         self.headers = {'User-Agent': self.ua}
         self.follow_data_url = 'https://api.weibo.cn/2/cardlist'
         self.sign_url = 'https://api.weibo.cn/2/page/button'
         self.event_url = 'https://m.weibo.cn/api/container/getIndex?containerid={container_id}_-_activity_list'
         self.draw_url = 'https://games.weibo.cn/prize/aj/lottery'
 
@@ -59,51 +60,72 @@
         for key, value in self.container_id.items():
             url = self.event_url.replace('{container_id}', value)
             async with httpx.AsyncClient() as client:
                 response = await client.get(url)
             responses = response.json()
             group = nested_lookup(responses, 'group', fetch_first=True)
             if group:
-                ticket_id[key] = [i
-                                  for id in group
-                                  for i in re.findall(r'ticket_id=(\d*)', unquote(unquote(id['scheme'])))]
+                ticket_id[key] = {}
+                ticket_id[key]['id'] = [i
+                                        for id in group
+                                        for i in re.findall(r'ticket_id=(\d*)', unquote(unquote(id['scheme'])))]
+                ticket_id[key]['img'] = group[random.randint(0, len(group) - 1)]['pic']
             else:
-                logger.info(f'{key}超话未存在活动签到')
+                logger.info(f'{key}超话当前没有兑换码')
         if not ticket_id:
-            return None
-        return ticket_id
+            return "超话无兑换码活动"
+        else:
+            return ticket_id
 
     async def get_code(self, id: str):
         url = self.draw_url
         self.headers.update({
             'Referer': f'https://games.weibo.cn/prize/lottery?ua={self.ua}&from=10E2295010&ticket_id={id}&ext='
         })
         data = {
             'ext': '', 'ticket_id': id, 'aid': self.params['aid'], 'from': self.params['from']
         }
         async with httpx.AsyncClient() as client:
             response = await client.get(url, params=data, headers=self.headers, cookies=self.cookie)
-        responses = response.json()
-        code = responses['data']['prize_data']['card_no'] if responses['msg'] == 'success' or responses[
-            'msg'] == 'recently' else False
-        if responses['msg'] == 'fail':
-            responses['msg'] = responses['data']['fail_desc1']
-        result = {'success': True, 'id': id, 'code': code} if code else {'success': False, 'id': id,
-                                                                         'response': responses['msg']}
-        return result['code'] if result['success'] else responses['msg']
+        if response.status_code == 200:
+            responses = response.json()
+            code = responses['data']['prize_data']['card_no'] if responses['msg'] == 'success' or responses[
+                'msg'] == 'recently' else False
+            if responses['msg'] == 'fail':
+                responses['msg'] = responses['data']['fail_desc1']
+            result = {'success': True, 'id': id, 'code': code} if code else {'success': False, 'id': id,
+                                                                             'response': responses['msg']}
+            return result['code'] if result['success'] else responses['msg']
+        else:
+            return '获取失败，请重新设置wb_cookie'
 
     async def get_code_list(self):
-        ticket_id = await self.get_ticket_id
-        msg = ""
-        code = {key: [] for key in ticket_id.keys()}
-        for key, value in ticket_id.items():
-            for item in value:
-                code[key].append(await self.get_code(item))
-        for key, values in code.items():
-            msg += f"{key}微博兑换码：" \
-                   "\n1️⃣" \
-                   f"  \n{values[0]}" \
-                   "\n2️⃣" \
-                   f"  \n{values[1]}" \
-                   "\n3️⃣" \
-                   f"  \n{values[2]}"
-        return msg
+        ticket_id = await self.get_ticket_id  # 有活动则返回一个dict，没活动则返回一个str
+        '''
+        ticket_id = {
+            '原神/崩铁': {
+                'id': [],
+                'img': ''
+            }
+        }
+        '''
+        if isinstance(ticket_id, dict):
+            msg = ""
+            code = {key: [] for key in ticket_id.keys()}
+            for key, value in ticket_id.items():
+                for k, v in value.items():
+                    if k == 'id':
+                        for item in v:
+                            code[key].append(await self.get_code(item))
+                    elif k == 'img':
+                        img = v
+            for key, values in code.items():
+                msg += f"<{key}>超话兑换码：" \
+                       "\n1️⃣" \
+                       f"  \n{values[0]}" \
+                       "\n2️⃣" \
+                       f"  \n{values[1]}" \
+                       "\n3️⃣" \
+                       f"  \n{values[2]}"
+            return msg, img
+        else:
+            return ticket_id
```

### Comparing `nonebot_plugin_mystool-2.3.0/src/nonebot_plugin_mystool/command/address.py` & `nonebot_plugin_mystool-2.4.0/src/nonebot_plugin_mystool/command/address.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_mystool-2.3.0/src/nonebot_plugin_mystool/command/common.py` & `nonebot_plugin_mystool-2.4.0/src/nonebot_plugin_mystool/command/common.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_mystool-2.3.0/src/nonebot_plugin_mystool/command/exchange.py` & `nonebot_plugin_mystool-2.4.0/src/nonebot_plugin_mystool/command/exchange.py`

 * *Files 1% similar despite different names*

```diff
@@ -165,15 +165,16 @@
     if command_2 == '+':
         good_dict = {
             'bh3': (await get_good_list('bh3'))[1],
             'ys': (await get_good_list('hk4e'))[1],
             'bh2': (await get_good_list('bh2'))[1],
             'xq': (await get_good_list('hkrpg'))[1],
             'wd': (await get_good_list('nxx'))[1],
-            'bbs': (await get_good_list('bbs'))[1]
+            'bbs': (await get_good_list('bbs'))[1],
+            'nap': (await get_good_list('nap'))[1]
         }
         flag = True
         break_flag = False
         good = None
         for good_list in good_dict.values():
             goods_on_sell = filter(lambda x: not x.time_end and x.time_limited, good_list)
             for good in goods_on_sell:
@@ -216,15 +217,15 @@
             await matcher.finish(f'⚠️该商品暂时不可以兑换，请重新设置')
 
     elif command_2 == '-':
         plans = PluginDataManager.plugin_data.users[event.get_user_id()].exchange_plans
         if plans:
             for plan in plans:
                 if plan.good.goods_id == good_id:
-                    plans.remove(plan)
+                    plans.discard(plan)
                     PluginDataManager.write_plugin_data()
                     for i in range(plugin_config.preference.exchange_thread_count):
                         scheduler.remove_job(job_id=f"exchange-plan-{hash(plan)}-{i}")
                     await matcher.finish('兑换计划删除成功')
             await matcher.finish(f"您没有设置商品ID为 {good_id} 的兑换哦~")
         else:
             await matcher.finish("您还没有配置兑换计划哦~")
@@ -308,14 +309,15 @@
 
 @get_good_image.got("content", prompt="请发送您要查看的商品类别:"
                                       "\n- 崩坏3"
                                       "\n- 原神"
                                       "\n- 崩坏2"
                                       "\n- 崩坏：星穹铁道"
                                       "\n- 未定事件簿"
+                                      "\n- 绝区零"
                                       "\n- 米游社"
                                       "\n若是商品图片与米游社商品不符或报错 请发送“更新”哦~"
                                       "\n—— 🚪发送“退出”以结束")
 async def _(event: Union[GeneralMessageEvent], arg=ArgPlainText("content")):
     """
     根据传入的商品类别，发送对应的商品列表图片
     """
@@ -329,14 +331,16 @@
         arg = ('bh2', '崩坏2')
     elif arg in ['崩坏：星穹铁道', '星铁', '星穹铁道', '铁道', '轨子', '星穹', 'xq']:
         arg = ('hkrpg', '崩坏：星穹铁道')
     elif arg in ['未定', '未定事件簿', 'wd']:
         arg = ('nxx', '未定事件簿')
     elif arg in ['大别野', '米游社', '综合']:
         arg = ('bbs', '米游社')
+    elif arg in ['绝区零']:
+        arg = ('nap', '绝区零')
     elif arg == '更新':
         threading.Thread(target=generate_image, kwargs={"is_auto": False}).start()
         await get_good_image.finish('⏳后台正在生成商品信息图片，请稍后查询')
     else:
         await get_good_image.reject('⚠️您的输入有误，请重新输入')
 
     img_path = time.strftime(
@@ -533,18 +537,18 @@
             # 删除旧图片
             if name.endswith('.jpg'):
                 os.remove(os.path.join(root, name))
 
     if plugin_config.good_list_image_config.MULTI_PROCESS:
         _lock: Lock = Manager().Lock()
         with Pool() as pool:
-            for game in "bh3", "hk4e", "bh2", "hkrpg", "nxx", "bbs":
+            for game in "bh3", "hk4e", "bh2", "hkrpg", "nxx", "bbs", "nap":
                 pool.apply_async(image_process,
                                  args=(game, _lock),
                                  callback=callback)
             pool.close()
             pool.join()
     else:
-        for game in "bh3", "hk4e", "bh2", "hkrpg", "nxx", "bbs":
+        for game in "bh3", "hk4e", "bh2", "hkrpg", "nxx", "bbs", "nap":
             image_process(game)
 
     logger.info(f"{plugin_config.preference.log_head}已完成所有分区的商品列表图片生成")
```

### Comparing `nonebot_plugin_mystool-2.3.0/src/nonebot_plugin_mystool/command/help.py` & `nonebot_plugin_mystool-2.4.0/src/nonebot_plugin_mystool/command/help.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_mystool-2.3.0/src/nonebot_plugin_mystool/command/login.py` & `nonebot_plugin_mystool-2.4.0/src/nonebot_plugin_mystool/command/login.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,26 +1,30 @@
+import asyncio
 import json
 from typing import Union
 
 from nonebot import on_command
-from nonebot.adapters.qq import MessageSegment as QQGuildMessageSegment, DirectMessageCreateEvent
+from nonebot.adapters.onebot.v11 import MessageEvent as OneBotV11MessageEvent, MessageSegment as OneBotV11MessageSegment
+from nonebot.adapters.qq import MessageSegment as QQGuildMessageSegment, DirectMessageCreateEvent, \
+    MessageEvent as QQGuildMessageEvent
 from nonebot.adapters.qq.exception import AuditException
 from nonebot.exception import ActionFailed
 from nonebot.internal.matcher import Matcher
 from nonebot.internal.params import ArgStr
-from nonebot.params import ArgPlainText, T_State
+from nonebot.params import T_State
 
-from ..api.common import get_login_ticket_by_captcha, get_multi_token_by_login_ticket, \
-    get_stoken_v2_by_v1, \
-    get_ltoken_by_stoken, get_cookie_token_by_stoken, get_device_fp, create_mmt, create_mobile_captcha
+from ..api.common import get_ltoken_by_stoken, get_cookie_token_by_stoken, get_device_fp, fetch_game_token_qrcode, \
+    query_game_token_qrcode, \
+    get_token_by_game_token, get_cookie_token_by_game_token
 from ..command.common import CommandRegistry
-from ..model import CreateMobileCaptchaStatus, PluginDataManager, plugin_config, UserAccount, UserData, CommandUsage
+from ..model import PluginDataManager, plugin_config, UserAccount, UserData, CommandUsage, BBSCookies, \
+    QueryGameTokenQrCodeStatus, GetCookieStatus
 from ..utils import logger, COMMAND_BEGIN, GeneralMessageEvent, GeneralPrivateMessageEvent, \
     GeneralGroupMessageEvent, \
-    generate_qr_img, get_validate, read_blacklist, read_whitelist, generate_device_id
+    read_blacklist, read_whitelist, generate_device_id, generate_qr_img
 
 __all__ = ["get_cookie", "output_cookies"]
 
 get_cookie = on_command(plugin_config.preference.command_start + '登录', priority=4, block=True)
 
 CommandRegistry.set_usage(
     get_cookie,
@@ -29,197 +33,166 @@
         description="跟随指引，通过电话获取短信方式绑定米游社账户，配置完成后会自动开启签到、米游币任务，后续可制定米游币自动兑换计划。"
     )
 )
 
 
 @get_cookie.handle()
 async def handle_first_receive(event: Union[GeneralMessageEvent]):
-    if isinstance(event, GeneralGroupMessageEvent):
-        await get_cookie.finish("⚠️为了保护您的隐私，请私聊进行登录。")
     user_num = len(set(PluginDataManager.plugin_data.users.values()))  # 由于加入了用户数据绑定功能，可能存在重复的用户数据对象，需要去重
     if plugin_config.preference.enable_blacklist:
         if event.get_user_id() in read_blacklist():
             await get_cookie.finish("⚠️您已被加入黑名单，无法使用本功能")
     elif plugin_config.preference.enable_whitelist:
         if event.get_user_id() not in read_whitelist():
             await get_cookie.finish("⚠️您不在白名单内，无法使用本功能")
     if user_num <= plugin_config.preference.max_user or plugin_config.preference.max_user in [-1, 0]:
-        # QQ频道可能无法发送链接，需要发送二维码
-        login_url = "https://user.mihoyo.com/#/login/captcha"
-        msg_text = "登录过程概览：\n" \
-                   "1.发送手机号\n" \
-                   "2.{browse_way}，输入手机号并获取验证码（不要在网页上登录）\n" \
-                   "3.发送验证码给QQ机器人，完成登录\n" \
-                   "🚪过程中发送“退出”即可退出"
-        try:
-            await get_cookie.send(msg_text.format(browse_way=f"前往 {login_url}"))
-        except ActionFailed:
-            logger.exception("发送包含URL链接的登录消息失败")
-            msg_img = QQGuildMessageSegment.file_image(generate_qr_img(login_url))
-            try:
-                await get_cookie.send(msg_img)
-                await get_cookie.send(msg_text.format(browse_way="扫描二维码，进入米哈游官方登录页"))
-            except (ActionFailed, AuditException) as e:
-                if isinstance(e, ActionFailed):
-                    logger.exception("发送包含二维码的登录消息失败")
-                    await get_cookie.send(msg_text.format(
-                        browse_way="前往米哈游官方登录页") + "\n\n⚠️发送二维码失败，请自行搜索米哈游通行证登录页")
-    else:
-        await get_cookie.finish('⚠️目前可支持使用用户数已经满啦~')
-
-
-@get_cookie.got('phone', prompt='1.请发送您的手机号：')
-async def _(event: Union[GeneralPrivateMessageEvent], state: T_State, phone: str = ArgPlainText('phone')):
-    if phone == '退出':
-        await get_cookie.finish("🚪已成功退出")
-    if not phone.isdigit():
-        await get_cookie.reject("⚠️手机号应为数字，请重新输入")
-    if len(phone) != 11:
-        await get_cookie.reject("⚠️手机号应为11位数字，请重新输入")
-    else:
-        state['phone'] = phone
-    user = PluginDataManager.plugin_data.users.get(event.get_user_id())
-    if user:
-        account_filter = filter(lambda x: x.phone_number == phone, user.accounts.values())
-        account = next(account_filter, None)
-        device_id = account.phone_number if account else None
-    else:
-        device_id = None
-    mmt_status, mmt_data, device_id, _ = await create_mmt(device_id=device_id)
-    state['device_id'] = device_id
-    if mmt_status:
-        if not mmt_data.gt:
-            captcha_status, _ = await create_mobile_captcha(phone_number=phone, mmt_data=mmt_data, device_id=device_id)
-            if captcha_status:
-                await get_cookie.send("检测到无需进行人机验证，已发送短信验证码，请查收")
-                return
-        elif plugin_config.preference.geetest_url:
-            await get_cookie.send("⏳正在尝试完成人机验证，请稍后...")
-            # TODO: 人机验证待支持 GT4
-            geetest_result = await get_validate(gt=mmt_data.gt)
-            captcha_status, _ = await create_mobile_captcha(
-                phone_number=phone,
-                mmt_data=mmt_data,
-                geetest_result=geetest_result,
-                use_v4=False,
-                device_id=device_id
-            )
-            if captcha_status:
-                await get_cookie.send("已发送短信验证码，请查收")
-                return
-            elif captcha_status.incorrect_geetest:
-                await get_cookie.send("⚠️尝试进行人机验证失败，请手动获取短信验证码")
-        else:
-            captcha_status = CreateMobileCaptchaStatus()
-        if captcha_status.invalid_phone_number:
-            await get_cookie.reject("⚠️手机号无效，请重新发送手机号")
-        elif captcha_status.not_registered:
-            await get_cookie.reject("⚠️手机号未注册，请注册后重新发送手机号")
-
-    await get_cookie.send('2.前往米哈游官方登录页，获取验证码（不要登录！）')
-
-
-@get_cookie.got("captcha", prompt='3.请发送验证码：')
-async def _(event: Union[GeneralPrivateMessageEvent], state: T_State, captcha: str = ArgPlainText('captcha')):
-    phone_number: str = state['phone']
-    device_id: str = state['device_id']
-    if captcha == '退出':
-        await get_cookie.finish("🚪已成功退出")
-    if not captcha.isdigit():
-        await get_cookie.reject("⚠️验证码应为数字，请重新输入")
-    else:
+        # 获取用户数据对象
         user_id = event.get_user_id()
         PluginDataManager.plugin_data.users.setdefault(user_id, UserData())
         user = PluginDataManager.plugin_data.users[user_id]
         # 如果是QQ频道，需要记录频道ID
         if isinstance(event, DirectMessageCreateEvent):
             user.qq_guild[user_id] = event.channel_id
-        # 1. 通过短信验证码获取 login_ticket / 使用已有 login_ticket
-        login_status, cookies = await get_login_ticket_by_captcha(phone_number, int(captcha), device_id)
-        if login_status:
-            logger.success(f"用户 {cookies.bbs_uid} 成功获取 login_ticket: {cookies.login_ticket}")
-            account = PluginDataManager.plugin_data.users[user_id].accounts.get(cookies.bbs_uid)
-            """当前的账户数据对象"""
-            if not account or not account.cookies:
-                user.accounts.update({
-                    cookies.bbs_uid: UserAccount(
-                        phone_number=phone_number,
-                        cookies=cookies,
-                        device_id_ios=device_id,
-                        device_id_android=generate_device_id())
-                })
-                account = user.accounts[cookies.bbs_uid]
+
+        # 1. 获取 GameToken 登录二维码
+        device_id = generate_device_id()
+        login_status, fetch_qrcode_ret = await fetch_game_token_qrcode(
+            device_id,
+            plugin_config.preference.game_token_app_id
+        )
+        if fetch_qrcode_ret:
+            qrcode_url, qrcode_ticket = fetch_qrcode_ret
+            await get_cookie.send("请用米游社App扫描下面的二维码进行登录")
+            image_bytes = generate_qr_img(qrcode_url)
+            if isinstance(event, OneBotV11MessageEvent):
+                msg_img = OneBotV11MessageSegment.image(image_bytes)
+            elif isinstance(event, QQGuildMessageEvent):
+                msg_img = QQGuildMessageSegment.file_image(image_bytes)
             else:
-                account.cookies.update(cookies)
-            fp_status, account.device_fp = await get_device_fp(device_id)
-            if fp_status:
-                logger.success(f"用户 {cookies.bbs_uid} 成功获取 device_fp: {account.device_fp}")
-            PluginDataManager.write_plugin_data()
-
-            # 2. 通过 login_ticket 获取 stoken 和 ltoken
-            if login_status or account:
-                login_status, cookies = await get_multi_token_by_login_ticket(account.cookies)
-                if login_status:
-                    logger.success(f"用户 {phone_number} 成功获取 stoken: {cookies.stoken}")
+                await get_cookie.finish("⚠️发送二维码失败，无法登录")
+                return
+            try:
+                await get_cookie.send(msg_img)
+            except (ActionFailed, AuditException) as e:
+                if isinstance(e, ActionFailed):
+                    logger.exception("发送包含二维码的登录消息失败")
+                    await get_cookie.finish("⚠️发送二维码失败，无法登录")
+
+            # 2. 从二维码登录获取 GameToken
+            qrcode_query_times = round(
+                plugin_config.preference.qrcode_wait_time / plugin_config.preference.qrcode_query_interval
+            )
+            bbs_uid, game_token = None, None
+            for _ in range(qrcode_query_times):
+                login_status, query_qrcode_ret = await query_game_token_qrcode(
+                    qrcode_ticket,
+                    device_id,
+                    plugin_config.preference.game_token_app_id
+                )
+                if query_qrcode_ret:
+                    bbs_uid, game_token = query_qrcode_ret
+                    logger.success(f"用户 {bbs_uid} 成功获取 game_token: {game_token}")
+                    break
+                elif login_status.qrcode_expired:
+                    get_cookie.finish("⚠️二维码已过期，登录失败")
+                elif not login_status:
+                    await asyncio.sleep(plugin_config.preference.qrcode_query_interval)
+                    continue
+
+            if bbs_uid and game_token:
+                cookies = BBSCookies()
+                cookies.bbs_uid = bbs_uid
+                account = PluginDataManager.plugin_data.users[user_id].accounts.get(bbs_uid)
+                """当前的账户数据对象"""
+                if not account or not account.cookies:
+                    user.accounts.update({
+                        bbs_uid: UserAccount(
+                            phone_number=None,
+                            cookies=cookies,
+                            device_id_ios=device_id,
+                            device_id_android=generate_device_id())
+                    })
+                    account = user.accounts[bbs_uid]
+                else:
                     account.cookies.update(cookies)
-                    PluginDataManager.write_plugin_data()
+                fp_status, account.device_fp = await get_device_fp(device_id)
+                if fp_status:
+                    logger.success(f"用户 {bbs_uid} 成功获取 device_fp: {account.device_fp}")
+                PluginDataManager.write_plugin_data()
 
-                    # 3. 通过 stoken_v1 获取 stoken_v2 和 mid
-                    login_status, cookies = await get_stoken_v2_by_v1(account.cookies, device_id)
+                if login_status:
+                    # 3. 通过 GameToken 获取 stoken_v2
+                    login_status, cookies = await get_token_by_game_token(bbs_uid, game_token)
                     if login_status:
-                        logger.success(f"用户 {phone_number} 成功获取 stoken_v2: {cookies.stoken_v2}")
+                        logger.success(f"用户 {bbs_uid} 成功获取 stoken_v2: {cookies.stoken_v2}")
                         account.cookies.update(cookies)
                         PluginDataManager.write_plugin_data()
 
-                        # 4. 通过 stoken_v2 获取 ltoken
-                        login_status, cookies = await get_ltoken_by_stoken(account.cookies, device_id)
-                        if login_status:
-                            logger.success(f"用户 {phone_number} 成功获取 ltoken: {cookies.ltoken}")
-                            account.cookies.update(cookies)
-                            PluginDataManager.write_plugin_data()
+                        if account.cookies.stoken_v2:
+                            # 5. 通过 stoken_v2 获取 ltoken
+                            login_status, cookies = await get_ltoken_by_stoken(account.cookies, device_id)
+                            if login_status:
+                                logger.success(f"用户 {bbs_uid} 成功获取 ltoken: {cookies.ltoken}")
+                                account.cookies.update(cookies)
+                                PluginDataManager.write_plugin_data()
 
-                            # 5. 通过 stoken_v2 获取 cookie_token
+                            # 6.1. 通过 stoken_v2 获取 cookie_token
                             login_status, cookies = await get_cookie_token_by_stoken(account.cookies, device_id)
                             if login_status:
-                                logger.success(f"用户 {phone_number} 成功获取 cookie_token: {cookies.cookie_token}")
+                                logger.success(f"用户 {bbs_uid} 成功获取 cookie_token: {cookies.cookie_token}")
                                 account.cookies.update(cookies)
                                 PluginDataManager.write_plugin_data()
 
-                                logger.success(f"{plugin_config.preference.log_head}米游社账户 {phone_number} 绑定成功")
-                                await get_cookie.finish(f"🎉米游社账户 {phone_number} 绑定成功")
+                                logger.success(
+                                    f"{plugin_config.preference.log_head}米游社账户 {bbs_uid} 绑定成功")
+                                await get_cookie.finish(f"🎉米游社账户 {bbs_uid} 绑定成功")
+                        else:
+                            # 6.2. 通过 GameToken 获取 cookie_token
+                            login_status, cookies = await get_cookie_token_by_game_token(bbs_uid, game_token)
+                            if login_status:
+                                logger.success(f"用户 {bbs_uid} 成功获取 cookie_token: {cookies.cookie_token}")
+                                account.cookies.update(cookies)
+                                PluginDataManager.write_plugin_data()
+            else:
+                get_cookie.finish("⚠️获取二维码扫描状态超时，请尝试重新登录")
 
         if not login_status:
             notice_text = "⚠️登录失败："
-            if login_status.incorrect_captcha:
-                notice_text += "验证码错误！"
-            elif login_status.login_expired:
+            if isinstance(login_status, QueryGameTokenQrCodeStatus):
+                if login_status.qrcode_expired:
+                    notice_text += "登录二维码已过期！"
+            if isinstance(login_status, GetCookieStatus):
+                if login_status.missing_bbs_uid:
+                    notice_text += "Cookies缺少 bbs_uid（例如 ltuid, stuid）"
+                elif login_status.missing_login_ticket:
+                    notice_text += "Cookies缺少 login_ticket！"
+                elif login_status.missing_cookie_token:
+                    notice_text += "Cookies缺少 cookie_token！"
+                elif login_status.missing_stoken:
+                    notice_text += "Cookies缺少 stoken！"
+                elif login_status.missing_stoken_v1:
+                    notice_text += "Cookies缺少 stoken_v1"
+                elif login_status.missing_stoken_v2:
+                    notice_text += "Cookies缺少 stoken_v2"
+                elif login_status.missing_mid:
+                    notice_text += "Cookies缺少 mid"
+            if login_status.login_expired:
                 notice_text += "登录失效！"
             elif login_status.incorrect_return:
                 notice_text += "服务器返回错误！"
             elif login_status.network_error:
                 notice_text += "网络连接失败！"
-            elif login_status.missing_bbs_uid:
-                notice_text += "Cookies缺少 bbs_uid（例如 ltuid, stuid）"
-            elif login_status.missing_login_ticket:
-                notice_text += "Cookies缺少 login_ticket！"
-            elif login_status.missing_cookie_token:
-                notice_text += "Cookies缺少 cookie_token！"
-            elif login_status.missing_stoken:
-                notice_text += "Cookies缺少 stoken！"
-            elif login_status.missing_stoken_v1:
-                notice_text += "Cookies缺少 stoken_v1"
-            elif login_status.missing_stoken_v2:
-                notice_text += "Cookies缺少 stoken_v2"
-            elif login_status.missing_mid:
-                notice_text += "Cookies缺少 mid"
             else:
                 notice_text += "未知错误！"
             notice_text += " 如果部分步骤成功，你仍然可以尝试获取收货地址、兑换等功能"
             await get_cookie.finish(notice_text)
 
+    else:
+        await get_cookie.finish('⚠️目前可支持使用用户数已经满啦~')
+
 
 output_cookies = on_command(
     plugin_config.preference.command_start + '导出Cookies',
     aliases={plugin_config.preference.command_start + '导出Cookie', plugin_config.preference.command_start + '导出账号',
              plugin_config.preference.command_start + '导出cookie',
              plugin_config.preference.command_start + '导出cookies'}, priority=4,
     block=True)
```

### Comparing `nonebot_plugin_mystool-2.3.0/src/nonebot_plugin_mystool/command/plan.py` & `nonebot_plugin_mystool-2.4.0/src/nonebot_plugin_mystool/command/plan.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,15 +24,16 @@
 from ..model import (MissionStatus, PluginDataManager, plugin_config, UserData, CommandUsage, GenshinNoteNotice,
                      StarRailNoteNotice)
 from ..utils import get_file, logger, COMMAND_BEGIN, GeneralMessageEvent, GeneralGroupMessageEvent, \
     send_private_msg, get_all_bind, \
     get_unique_users, get_validate, read_admin_list
 
 __all__ = [
-    "manually_game_sign", "manually_bbs_sign", "manually_genshin_note_check", "manually_starrail_note_check"
+    "manually_game_sign", "manually_bbs_sign", "manually_genshin_note_check",
+    "manually_starrail_note_check", "manually_weibo_check"
 ]
 
 manually_game_sign = on_command(plugin_config.preference.command_start + '签到', priority=5, block=True)
 
 CommandRegistry.set_usage(
     manually_game_sign,
     CommandUsage(
@@ -188,16 +189,14 @@
     manually_starrail_note_check,
     CommandUsage(
         name="星穹铁道便笺",
         description="手动查看星穹铁道实时便笺，即开拓力、每日实训、每周模拟宇宙积分等信息"
     )
 )
 
-weibo_check = on_command(plugin_config.preference.command_start + '微博兑换码', priority=5, block=True)
-
 
 @manually_starrail_note_check.handle()
 async def _(event: Union[GeneralMessageEvent], matcher: Matcher):
     """
     手动查看星穹铁道便笺（sr）
     """
     user_id = event.get_user_id()
@@ -259,18 +258,18 @@
             else:
                 signed = info.is_sign
 
             # 若没签到，则进行签到功能；若获取今日签到情况失败，仍可继续
             if (get_info_status and not info.is_sign) or not get_info_status:
                 sign_status, mmt_data = await signer.sign(account.platform)
                 if sign_status.need_verify:
-                    if plugin_config.preference.geetest_url:
+                    if plugin_config.preference.geetest_url or user.geetest_url:
                         if matcher:
                             await matcher.send("⏳正在尝试完成人机验证，请稍后...")
-                        geetest_result = await get_validate(mmt_data.gt, mmt_data.challenge)
+                        geetest_result = await get_validate(user, mmt_data.gt, mmt_data.challenge)
                         sign_status, _ = await signer.sign(account.platform, mmt_data, geetest_result)
 
                 if not sign_status and (user.enable_notice or matcher):
                     if sign_status.login_expired:
                         message = f"⚠️账户 {account.display_name} 🎮『{signer.name}』签到时服务器返回登录失效，请尝试重新登录绑定账户"
                     elif sign_status.need_verify:
                         message = (f"⚠️账户 {account.display_name} 🎮『{signer.name}』签到时可能遇到验证码拦截，"
@@ -407,15 +406,15 @@
                     MissionStatus(),
                     MissionStatus(),
                     MissionStatus()
                 )
                 sign_points: Optional[int] = None
                 for key_name in missions_state.state_dict:
                     if key_name == BaseMission.SIGN:
-                        sign_status, sign_points = await mission_obj.sign()
+                        sign_status, sign_points = await mission_obj.sign(user)
                     elif key_name == BaseMission.VIEW:
                         read_status = await mission_obj.read()
                     elif key_name == BaseMission.LIKE:
                         like_status = await mission_obj.like()
                     elif key_name == BaseMission.SHARE:
                         share_status = await mission_obj.share()
 
@@ -646,28 +645,51 @@
             if matcher:
                 await matcher.send(msg)
             else:
                 for user_id in user_ids:
                     await send_private_msg(user_id=user_id, message=msg)
 
 
-async def weibo_code_check(user: UserData, user_ids: Iterable[str]):
+async def weibo_code_check(user: UserData, user_ids: Iterable[str], matcher: Matcher = None):
     """
     是否开启微博兑换码功能的函数，并发送给用户任务执行消息。
 
     :param user: 用户对象
     :param user_ids: 发送通知的所有用户ID
+    :param matcher: nonebot ``Matcher``
     """
-    for account in user.accounts.values():
-        if account.enable_weibo:
-            # account = UserAccount(account) 
-            weibo = WeiboCode(account)
-            msg = await weibo.get_code_list()
-            for user_id in user_ids:
-                await send_private_msg(user_id=user_id, message=msg)
+    msg, img = None, None
+    if user.enable_weibo:
+        # account = UserAccount(account) 
+        weibo = WeiboCode(user)
+        result = await weibo.get_code_list()
+        try:
+            if isinstance(result, tuple):
+                msg, img = result
+            else:
+                msg = result
+        except Exception:
+            pass
+        if matcher:
+            if img:
+                onebot_img_msg = OneBotV11MessageSegment.image(await get_file(img))
+                messages = msg + onebot_img_msg
+            else:
+                messages = msg
+            await matcher.send(messages)
+        else:
+            if img and '无' not in msg:
+                saa_img = Image(await get_file(img))
+                messages = msg + saa_img
+                for user_id in user_ids:
+                    await send_private_msg(user_id=user_id, message=messages)
+    else:
+        message = "未开启微博功能"
+        if matcher:
+            await matcher.send(message)
 
 
 @scheduler.scheduled_job("cron", hour='0', minute='0', id="daily_goodImg_update")
 def daily_update():
     """
     每日图片生成函数
     """
@@ -717,15 +739,18 @@
     logger.info(f"{plugin_config.preference.log_head}开始执行微博自动任务")
     for user_id, user in get_unique_users():
         user_ids = [user_id] + list(get_all_bind(user_id))
         await weibo_code_check(user=user, user_ids=user_ids)
     logger.info(f"{plugin_config.preference.log_head}微博自动任务执行完成")
 
 
-@weibo_check.handle()
+manually_weibo_check = on_command(plugin_config.preference.command_start + 'wb兑换', priority=5, block=True)
+
+
+@manually_weibo_check.handle()
 async def weibo_schedule(event: Union[GeneralMessageEvent], matcher: Matcher):
     if isinstance(event, GeneralGroupMessageEvent):
         await matcher.send("⚠️为了保护您的隐私，请私聊进行查询。")
     else:
         user_id = event.get_user_id()
         user = PluginDataManager.plugin_data.users.get(user_id)
-        await weibo_code_check(user=user, user_ids=[user_id])
+        await weibo_code_check(user=user, user_ids=[user_id], matcher=matcher)
```

### Comparing `nonebot_plugin_mystool-2.3.0/src/nonebot_plugin_mystool/command/setting.py` & `nonebot_plugin_mystool-2.4.0/src/nonebot_plugin_mystool/command/setting.py`

 * *Files 11% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from nonebot import on_command
 from nonebot.internal.params import ArgStr
 from nonebot.matcher import Matcher
 from nonebot.params import T_State
 
 from ..api import BaseMission
 from ..command.common import CommandRegistry
-from ..model import PluginDataManager, plugin_config, UserAccount, CommandUsage
+from ..model import PluginDataManager, plugin_config, UserAccount, CommandUsage, UserData
 from ..utils import COMMAND_BEGIN, GeneralMessageEvent
 
 __all__ = ["setting", "account_setting", "global_setting"]
 
 setting = on_command(plugin_config.preference.command_start + '设置', priority=4, block=True)
 
 CommandRegistry.set_usage(
@@ -69,14 +69,15 @@
     """
     if bbs_uid == '退出':
         await matcher.finish('🚪已成功退出')
 
     user_account = PluginDataManager.plugin_data.users[event.get_user_id()].accounts
     if not (account := user_account.get(bbs_uid)):
         await account_setting.reject('⚠️您发送的账号不在以上账号内，请重新发送')
+    state["user"] = PluginDataManager.plugin_data.users[event.get_user_id()]
     state['account'] = account
     state["prepare_to_delete"] = False
 
     user_setting = ""
     user_setting += f"1️⃣ 米游币任务自动执行：{'开' if account.enable_mission else '关'}"
     user_setting += f"\n2️⃣ 游戏自动签到：{'开' if account.enable_game_sign else '关'}"
     platform_show = "iOS" if account.platform == "ios" else "安卓"
@@ -93,17 +94,18 @@
             )
         )
     )
     user_setting += f"\n\n5️⃣ 实时便笺体力提醒：{'开' if account.enable_resin else '关'}"
     user_setting += f"\n6️⃣更改便笺体力提醒阈值 \
                       \n   当前原神提醒阈值：{account.user_resin_threshold} \
                       \n   当前崩铁提醒阈值：{account.user_stamina_threshold}"
-    user_setting += "\n7️⃣⚠️删除账户数据"
+    user_setting += "\n7️⃣设置微博相关功能"
+    user_setting += "\n8️⃣⚠️删除账户数据"
 
-    await account_setting.send(user_setting + '\n\n您要更改哪一项呢？请发送 1 / 2 / 3 / 4 / 5 / 6 / 7'
+    await account_setting.send(user_setting + '\n\n您要更改哪一项呢？请发送 1 / 2 / 3 / 4 / 5 / 6 / 7/ 8'
                                               '\n🚪发送“退出”即可退出')
 
 
 @account_setting.got('setting_id')
 async def _(event: Union[GeneralMessageEvent], state: T_State, setting_id=ArgStr()):
     """
     根据所选更改相应账户的相应设置
@@ -148,15 +150,26 @@
             "请发送想要修改体力提醒阈值的游戏编号："
             "\n1. 原神"
             "\n2. 崩坏：星穹铁道"
             "\n\n🚪发送“退出”即可退出"
         )
         state["setting_item"] = "setting_notice_value"
         return
-    elif setting_id == '7':
+    elif setting_id == "7":
+        user: UserData = state["user"]
+        msg = ""
+        msg += "请发送想要设置的微博参数："
+        msg += f"\n1. 微博签到与兑换：{'开' if user.enable_weibo else '关'}"
+        msg += "\n2. 微博cookie" \
+               "\n3. 微博params" \
+               "\n\n🚪发送“退出”即可退出"
+        await account_setting.send(msg)
+        state["setting_item"] = "weibo_value"
+        return
+    elif setting_id == '8':
         state["prepare_to_delete"] = True
         await account_setting.reject(f"⚠️确认删除账号 {account.display_name} ？发送 \"确认删除\" 以确定。")
     elif setting_id == '确认删除' and state["prepare_to_delete"]:
         user_account.pop(account.bbs_uid)
         PluginDataManager.write_plugin_data()
         await account_setting.finish(f"已删除账号 {account.display_name} 的数据")
     else:
@@ -183,14 +196,36 @@
                 "可用范围 [0, 240]"
                 "\n\n🚪发送“退出”即可退出"
             )
             state["setting_item"] = "setting_notice_value_sr"
         else:
             await account_setting.reject("⚠️您的输入有误，请重新输入")
 
+    elif state["setting_item"] == "weibo_value":
+        user: UserData = state["user"]
+        if notice_game == "1":
+            user.enable_weibo = not user.enable_weibo
+            PluginDataManager.write_plugin_data()
+            await account_setting.finish(f"微博签到与兑换功能已 {'✅开启' if user.enable_weibo else '❌关闭'}")
+        elif notice_game == "2":
+            await account_setting.send(
+                "请微博cookie："
+                "发送格式不带cookie="
+                "\n\n🚪发送“退出”即可退出"
+            )
+            state["setting_item"] = "setting_weibo_value_cookie"
+        elif notice_game == "3":
+            await account_setting.send(
+                "请微博params："
+                "发送格式不带params="
+                "params必要参数: s、gsid、aid、from"
+                "\n\n🚪发送“退出”即可退出"
+            )
+            state["setting_item"] = "setting_weibo_value_params"
+
 
 @account_setting.got('setting_value')
 async def _(_: Union[GeneralMessageEvent], state: T_State, setting_value=ArgStr()):
     if setting_value == '退出':
         await account_setting.finish('🚪已成功退出')
     account: UserAccount = state['account']
 
@@ -237,14 +272,26 @@
                 mission_games.append(game_name)
 
         account.mission_games = mission_games
         PluginDataManager.write_plugin_data()
         setting_value = setting_value.replace(" ", "、")
         await account_setting.finish(f"💬执行米游币任务的频道已更改为『{setting_value}』")
 
+    # 做区分，以下应用在用户数据中，而非米游社数据中
+    user: UserData = state["user"]
+    print(user)
+    if state["setting_item"] == "setting_weibo_value_cookie":
+        user.weibo_cookie = str(setting_value)
+        PluginDataManager.write_plugin_data()
+        await account_setting.finish("设置微博cookie成功")
+    elif state["setting_item"] == "setting_weibo_value_params":
+        user.weibo_params = str(setting_value)
+        PluginDataManager.write_plugin_data()
+        await account_setting.finish("设置微博params成功")
+
 
 global_setting = on_command(plugin_config.preference.command_start + '通知设置', priority=5, block=True)
 
 CommandRegistry.set_usage(
     global_setting,
     CommandUsage(
         name="通知设置",
```

### Comparing `nonebot_plugin_mystool-2.3.0/src/nonebot_plugin_mystool/command/user_check.py` & `nonebot_plugin_mystool-2.4.0/src/nonebot_plugin_mystool/command/user_check.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_mystool-2.3.0/src/nonebot_plugin_mystool/model/common.py` & `nonebot_plugin_mystool-2.4.0/src/nonebot_plugin_mystool/model/common.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 from pydantic import BaseModel
 
 __all__ = ["root_path", "data_path", "BaseModelWithSetter", "BaseModelWithUpdate", "Good", "GameRecord", "GameInfo",
            "Address", "MmtData",
            "Award", "GameSignInfo", "MissionData", "MissionState", "GenshinNote", "StarRailNote", "GenshinNoteNotice",
            "StarRailNoteNotice", "BaseApiStatus", "CreateMobileCaptchaStatus", "GetCookieStatus", "GetGoodDetailStatus",
            "ExchangeStatus", "MissionStatus", "GetFpStatus", "BoardStatus", "GenshinNoteStatus", "StarRailNoteStatus",
-           "GeetestResult", "GeetestResultV4", "CommandUsage"]
+           "QueryGameTokenQrCodeStatus", "GeetestResult", "GeetestResultV4", "CommandUsage"]
 
 root_path = Path(__name__).parent.absolute()
 '''NoneBot2 机器人根目录'''
 
 data_path = root_path / "data" / "nonebot-plugin-mystool"
 '''插件数据保存目录'''
 
@@ -621,14 +621,26 @@
     """
     星铁实时便笺 返回结果
     """
     no_starrail_account = False
     """用户没有任何星铁账户"""
 
 
+class QueryGameTokenQrCodeStatus(BaseApiStatus):
+    """
+    星铁实时便笺 返回结果
+    """
+    qrcode_expired = False
+    """二维码已过期"""
+    qrcode_init = False
+    """二维码未扫描"""
+    qrcode_scanned = False
+    """二维码已扫描但未确认"""
+
+
 GeetestResult = NamedTuple("GeetestResult", validate=str, seccode=str)
 """人机验证结果数据"""
 
 
 class GeetestResultV4(BaseModel):
     """
     GEETEST GT4 人机验证结果数据
```

### Comparing `nonebot_plugin_mystool-2.3.0/src/nonebot_plugin_mystool/model/config.py` & `nonebot_plugin_mystool-2.4.0/src/nonebot_plugin_mystool/model/config.py`

 * *Files 2% similar despite different names*

```diff
@@ -67,14 +67,16 @@
     '''插件内部命令头(若为""空字符串则不启用)'''
     sleep_time: float = 2
     '''任务操作冷却时间(如米游币任务)'''
     plan_time: str = "00:30"
     '''每日自动签到和米游社任务的定时任务执行时间，格式为HH:MM'''
     resin_interval: int = 60
     '''每次检查原神便笺间隔，单位为分钟'''
+    global_geetest: bool = True
+    '''是否开启使用全局极验Geetest，默认开启'''
     geetest_url: Optional[str]
     '''极验Geetest人机验证打码接口URL'''
     geetest_params: Optional[Dict[str, Any]] = None
     '''极验Geetest人机验证打码API发送的参数（除gt，challenge外）'''
     geetest_json: Optional[Dict[str, Any]] = {
         "gt": "{gt}",
         "challenge": "{challenge}"
@@ -90,14 +92,20 @@
     """是否启用用户白名单"""
     whitelist_path: Optional[Path] = data_path / "whitelist.txt"
     """用户白名单文件路径"""
     enable_admin_list: bool = False
     """是否启用管理员名单"""
     admin_list_path: Optional[Path] = data_path / "admin_list.txt"
     """管理员名单文件路径"""
+    game_token_app_id: str = "1"
+    """米游社二维码登录的应用标识符（可用的任何值都没有区别，但是必须传递此参数）"""
+    qrcode_query_interval: float = 1
+    """检查米游社登录二维码扫描情况的请求间隔（单位：秒）"""
+    qrcode_wait_time: float = 120
+    """等待米游社登录二维码扫描的最长时间（单位：秒）"""
 
     @validator("log_path", allow_reuse=True)
     def _(cls, v: Optional[Path]):
         absolute_path = v.absolute()
         if not os.path.exists(absolute_path) or not os.path.isfile(absolute_path):
             absolute_parent = absolute_path.parent
             try:
@@ -251,15 +259,14 @@
             f.write(str_data)
     except (AttributeError, TypeError, ValueError, PermissionError):
         logger.exception(f"创建插件配置文件失败，请检查是否有权限读取和写入 {plugin_config_path}")
         raise
     else:
         logger.info(f"插件配置文件 {plugin_config_path} 不存在，已创建默认插件配置文件。")
 
-
 # TODO: 可能产生 #271 的问题 https://github.com/Ljzd-PRO/nonebot-plugin-mystool/issues/271
 # @_driver.on_startup
 # def _():
 #     """将 ``PluginMetadata.config`` 设为定义的插件配置对象 ``plugin_config``"""
 #     plugin = nonebot.plugin.get_plugin(plugin_config.preference.plugin_name)
 #     plugin.metadata.config = plugin_config
```

### Comparing `nonebot_plugin_mystool-2.3.0/src/nonebot_plugin_mystool/model/data.py` & `nonebot_plugin_mystool-2.4.0/src/nonebot_plugin_mystool/model/data.py`

 * *Files 2% similar despite different names*

```diff
@@ -230,35 +230,28 @@
 
     device_id_ios: str
     """iOS设备用 deviceID"""
     device_id_android: str
     """安卓设备用 deviceID"""
     device_fp: Optional[str]
     """iOS设备用 deviceFp"""
-
     enable_mission: bool = True
     '''是否开启米游币任务计划'''
     enable_game_sign: bool = True
     '''是否开启米游社游戏签到计划'''
     enable_resin: bool = True
     '''是否开启便笺提醒'''
-    enable_weibo: bool = False
-    '''是否开启微博兑换码功能'''
     platform: Literal["ios", "android"] = "ios"
     '''设备平台'''
     mission_games: List[str] = ["BBSMission"]
     '''在哪些板块执行米游币任务计划 为 BaseMission 子类名称'''
     user_stamina_threshold: int = 240
     '''崩铁便笺体力提醒阈值，0为一直提醒'''
     user_resin_threshold: int = 160
     '''原神便笺树脂提醒阈值，0为一直提醒'''
-    weibo_cookie: str = ""
-    '''微博查询活动签到用的 cookie'''
-    weibo_params: str = ""
-    '''微博查询活动签到用的 params'''
 
     def __init__(self, **data: Any):
         if not data.get("device_id_ios") or not data.get("device_id_android"):
             from ..utils import generate_device_id
             if not data.get("device_id_ios"):
                 data.setdefault("device_id_ios", generate_device_id())
             if not data.get("device_id_android"):
@@ -279,15 +272,15 @@
 
     @property
     def display_name(self):
         """
         显示名称
         """
         from ..utils.common import blur_phone
-        return f"{self.bbs_uid}({blur_phone(self.phone_number)})"
+        return f"{self.bbs_uid}({blur_phone(self.phone_number)})" if self.phone_number else self.bbs_uid
 
 
 class ExchangePlan(BaseModel):
     """
     兑换计划数据类
     """
 
@@ -370,14 +363,24 @@
     用户数据类
 
     >>> userdata = UserData()
     >>> hash(userdata)
     """
     enable_notice: bool = True
     """是否开启通知"""
+    enable_weibo: bool = False
+    '''是否开启微博兑换码功能'''
+    weibo_cookie: str = ""
+    '''微博查询活动签到用的 cookie'''
+    weibo_params: str = ""
+    '''微博查询活动签到用的 params'''
+    geetest_url: Optional[str]
+    '''极验Geetest人机验证打码接口URL'''
+    geetest_params: Optional[Dict[str, Any]] = None
+    '''极验Geetest人机验证打码API发送的参数（除gt，challenge外）'''
     uuid: Optional[str] = None
     """用户UUID密钥，用于不同NoneBot适配器平台之间的数据同步，因此不可泄露"""
     qq_guild: Optional[Dict[str, int]] = {}
     """储存用户所在的QQ频道ID {用户ID : 频道ID}"""
     qq_guilds: Optional[Dict[str, List[int]]] = Field(default={}, exclude=True)
     """旧版（v2.1.0 之前）储存用户所在的QQ频道ID {用户ID : [频道ID]}"""
     exchange_plans: Union[Set[ExchangePlan], List[ExchangePlan]] = set()
```

### Comparing `nonebot_plugin_mystool-2.3.0/src/nonebot_plugin_mystool/model/upgrade/common.py` & `nonebot_plugin_mystool-2.4.0/src/nonebot_plugin_mystool/model/upgrade/common.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_mystool-2.3.0/src/nonebot_plugin_mystool/model/upgrade/configV2.py` & `nonebot_plugin_mystool-2.4.0/src/nonebot_plugin_mystool/model/upgrade/configV2.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_mystool-2.3.0/src/nonebot_plugin_mystool/model/upgrade/dataV2.py` & `nonebot_plugin_mystool-2.4.0/src/nonebot_plugin_mystool/model/upgrade/dataV2.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_mystool-2.3.0/src/nonebot_plugin_mystool/utils/common.py` & `nonebot_plugin_mystool-2.4.0/src/nonebot_plugin_mystool/utils/common.py`

 * *Files 2% similar despite different names*

```diff
@@ -229,47 +229,55 @@
         t = str(int(time.time()))
         r = str(random.randint(100000, 200000))
         c = hashlib.md5(
             f"salt={salt}&t={t}&r={r}&b={data}&q={params}".encode()).hexdigest()
         return f"{t},{r},{c}"
 
 
-async def get_validate(gt: str = None, challenge: str = None, retry: bool = True):
+async def get_validate(user: UserData, gt: str = None, challenge: str = None, retry: bool = True):
     """
     使用打码平台获取人机验证validate
 
     :param gt: 验证码gt
     :param challenge: challenge
     :param retry: 是否允许重试
     :return: 如果配置了平台URL，且 gt, challenge 不为空，返回 GeetestResult
     """
-    if not (gt and challenge) or not plugin_config.preference.geetest_url:
-        return GeetestResult("", "")
-    params = {"gt": gt, "challenge": challenge}
-    params.update(plugin_config.preference.geetest_params)
+    if not plugin_config.preference.global_geetest:
+        if not (gt and challenge) or not user.geetest_url:
+            return GeetestResult("", "")
+        geetest_url = user.geetest_url
+        params = {"gt": gt, "challenge": challenge}
+        params.update(user.geetest_params)
+    else:
+        if not (gt and challenge) or not plugin_config.preference.geetest_url:
+            return GeetestResult("", "")
+        geetest_url = plugin_config.preference.geetest_url
+        params = {"gt": gt, "challenge": challenge}
+        params.update(plugin_config.preference.geetest_params)
     content = deepcopy(plugin_config.preference.geetest_json or Preference().geetest_json)
     for key, value in content.items():
         if isinstance(value, str):
             content[key] = value.format(gt=gt, challenge=challenge)
     try:
         async for attempt in get_async_retry(retry):
             with attempt:
                 async with httpx.AsyncClient() as client:
                     res = await client.post(
-                        plugin_config.preference.geetest_url,
+                        geetest_url,
                         params=params,
                         json=content,
                         timeout=60
                     )
                 geetest_data = res.json()
                 validate = geetest_data['data']['validate']
                 seccode = geetest_data['data'].get('seccode') or f"{validate}|jordan"
                 logger.debug(f"{plugin_config.preference.log_head}人机验证结果：{geetest_data}")
                 return GeetestResult(validate=validate, seccode=seccode)
-    except tenacity.RetryError:
+    except tenacity.RetryError as e:
         logger.exception(f"{plugin_config.preference.log_head}获取人机验证validate失败")
 
 
 def generate_seed_id(length: int = 8) -> str:
     """
     生成随机的 seed_id（即长度为8的十六进制数）
```

### Comparing `nonebot_plugin_mystool-2.3.0/src/nonebot_plugin_mystool/utils/good_image.py` & `nonebot_plugin_mystool-2.4.0/src/nonebot_plugin_mystool/utils/good_image.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_mystool-2.3.0/PKG-INFO` & `nonebot_plugin_mystool-2.4.0/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 00000000: 4d65 7461 6461 7461 2d56 6572 7369 6f6e  Metadata-Version
 00000010: 3a20 322e 310a 4e61 6d65 3a20 6e6f 6e65  : 2.1.Name: none
 00000020: 626f 742d 706c 7567 696e 2d6d 7973 746f  bot-plugin-mysto
-00000030: 6f6c 0a56 6572 7369 6f6e 3a20 322e 332e  ol.Version: 2.3.
+00000030: 6f6c 0a56 6572 7369 6f6e 3a20 322e 342e  ol.Version: 2.4.
 00000040: 300a 5375 6d6d 6172 793a 2051 51e8 818a  0.Summary: QQ...
 00000050: e5a4 a9e3 8081 e9a2 91e9 8193 e69c bae5  ................
 00000060: 99a8 e4ba bae6 8f92 e4bb b620 7c20 e7b1  ........... | ..
 00000070: b3e6 b8b8 e7a4 bee5 b7a5 e585 b72d e6af  .............-..
 00000080: 8fe6 97a5 e7b1 b3e6 b8b8 e5b8 81e4 bbbb  ................
 00000090: e58a a1e3 8081 e6b8 b8e6 888f e7ad bee5  ................
 000000a0: 88b0 e380 81e5 9586 e593 81e5 8591 e68d  ................
@@ -166,165 +166,113 @@
 00000a50: 6765 295d 2868 7474 7073 3a2f 2f67 6974  ge)](https://git
 00000a60: 6875 622e 636f 6d2f 4c6a 7a64 2d50 524f  hub.com/Ljzd-PRO
 00000a70: 2f6e 6f6e 6562 6f74 2d70 6c75 6769 6e2d  /nonebot-plugin-
 00000a80: 6d79 7374 6f6f 6c2f 636f 6d6d 6974 732f  mystool/commits/
 00000a90: 6465 7629 0a0a 2320 6d79 7354 6f6f 6c20  dev)..# mysTool 
 00000aa0: 2d20 e7b1 b3e6 b8b8 e7a4 bee8 be85 e58a  - ..............
 00000ab0: a9e5 b7a5 e585 b7e6 8f92 e4bb b60a 0a23  ...............#
-00000ac0: 2320 f09f 93a3 20e6 9bb4 e696 b0e5 8685  # .... .........
-00000ad0: e5ae b90a 0a3e 205b 2149 4d50 4f52 5441  .....> [!IMPORTA
-00000ae0: 4e54 5d0a 3e20 7632 2e30 2e30 20e7 aa81  NT].> v2.0.0 ...
-00000af0: e7a0 b4e6 80a7 e69b b4e6 96b0 0a3e 2068  .............> h
-00000b00: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
-00000b10: 6d2f 4c6a 7a64 2d50 524f 2f6e 6f6e 6562  m/Ljzd-PRO/noneb
-00000b20: 6f74 2d70 6c75 6769 6e2d 6d79 7374 6f6f  ot-plugin-mystoo
-00000b30: 6c2f 7265 6c65 6173 6573 2f74 6167 2f76  l/releases/tag/v
-00000b40: 322e 302e 300a 0a23 2323 2032 3032 342e  2.0.0..### 2024.
-00000b50: 332e 3820 2d20 7632 2e33 2e30 0a0a 2323  3.8 - v2.3.0..##
-00000b60: 2323 20f0 9f92 a120 e696 b0e7 89b9 e680  ## .... ........
-00000b70: a70a 2d20 e5a2 9ee5 8aa0 e5be aee5 8d9a  ..- ............
-00000b80: e8b6 85e8 af9d e585 91e6 8da2 e7a0 81e6  ................
-00000b90: 8ea8 e980 81e5 8a9f e883 bd20 2d20 6279  ........... - by
-00000ba0: 2040 4a6f 7365 616e 646c 7575 6520 2823   @Joseandluue (#
-00000bb0: 3237 3229 0a2d 20e6 9bb4 e694 b9e6 af8f  272).- .........
-00000bc0: e697 a5e4 bbbb e58a a1e6 89a7 e8a1 8ce9  ................
-00000bd0: a1ba e5ba 8fe3 8082 e585 88e6 89a7 e8a1  ................
-00000be0: 8ce6 b8b8 e688 8fe7 adbe e588 b0ef bc8c  ................
-00000bf0: e586 8de6 89a7 e8a1 8ce7 b1b3 e6b8 b8e5  ................
-00000c00: b881 e4bb bbe5 8aa1 efbc 8ce4 bba5 e999  ................
-00000c10: 8de4 bd8e e689 a7e8 a18c e7b1 b3e6 b8b8  ................
-00000c20: e5b8 81e4 bbbb e58a a1e6 97b6 e587 bae7  ................
-00000c30: 8eb0 e4ba bae6 9cba e9aa 8ce8 af81 e79a  ................
-00000c40: 84e6 a682 e78e 8720 2d20 6279 2040 5361  ....... - by @Sa
-00000c50: 6b61 6d61 6b69 6969 7a61 796f 6920 404a  kamakiiizayoi @J
-00000c60: 6f73 6561 6e64 6c75 7565 0a0a 2323 2323  oseandluue..####
-00000c70: 20f0 9f90 9b20 4275 6720 e4bf aee5 a48d   .... Bug ......
-00000c80: 0a2d 20e4 bfae e5a4 8de6 af8f e697 a5e4  .- .............
-00000c90: bbbb e58a a1e8 87aa e58a a8e8 bf9b e8a1  ................
-00000ca0: 8ce6 b8b8 e688 8fe7 adbe e588 b0e5 908e  ................
-00000cb0: efbc 8c51 51e8 818a e5a4 a9e7 9a84 e4b8  ...QQ...........
-00000cc0: bbe5 8aa8 e7a7 81e4 bfa1 e68e a8e9 8081  ................
-00000cd0: e5a4 b1e8 b4a5 e79a 84e9 97ae e9a2 9820  ............... 
-00000ce0: 2823 3237 3029 0a2d 20e6 9bb4 e694 b920  (#270).- ...... 
-00000cf0: 6055 7365 7241 6363 6f75 6e74 2e6d 6973  `UserAccount.mis
-00000d00: 7369 6f6e 5f67 616d 6573 60ef bc88 e794  sion_games`.....
-00000d10: a8e6 88b7 e7b1 b3e6 b8b8 e5b8 81e4 bbbb  ................
-00000d20: e58a a1e7 9bae e6a0 87e5 8886 e58c baef  ................
-00000d30: bc89 20e9 bb98 e8ae a4e5 80bc e4b8 ba20  .. ............ 
-00000d40: 605b 2242 4253 4d69 7373 696f 6e22 5d60  `["BBSMission"]`
-00000d50: efbc 8ce5 b9b6 e59c a8e6 89a7 e8a1 8ce6  ................
-00000d60: 97b6 e6a3 80e6 9fa5 e8af a5e9 858d e7bd  ................
-00000d70: aee6 98af e590 a6e6 9caa e7a9 ba20 2823  ............. (#
-00000d80: 3236 3129 0a2d 20e4 bfae e5a4 8de5 8faf  261).- .........
-00000d90: e883 bde5 87ba e78e b0e7 9a84 e590 afe5  ................
-00000da0: 8aa8 e5a4 b1e8 b4a5 e79a 84e9 97ae e9a2  ................
-00000db0: 98ef bc88 6041 7474 7269 6275 7465 4572  ....`AttributeEr
-00000dc0: 726f 723a 2027 4e6f 6e65 5479 7065 2720  ror: 'NoneType' 
-00000dd0: 6f62 6a65 6374 2068 6173 206e 6f20 6174  object has no at
-00000de0: 7472 6962 7574 6520 276d 6574 6164 6174  tribute 'metadat
-00000df0: 6127 60ef bc89 2028 2332 3731 290a 0a23  a'`... (#271)..#
-00000e00: 2320 e29a a120 e58a 9fe8 83bd e592 8ce7  # ... ..........
-00000e10: 89b9 e680 a70a 0a2d 20e6 94af e68c 8151  .......- ......Q
-00000e20: 51e8 818a e5a4 a9e5 928c 5151 e9a2 91e9  Q.........QQ....
-00000e30: 8193 0a2d 20e7 9fad e4bf a1e9 aa8c e8af  ...- ...........
-00000e40: 81e7 99bb e5bd 95ef bc8c e585 8de6 8a93  ................
-00000e50: e58c 85e8 8eb7 e58f 9620 436f 6f6b 6965  ......... Cookie
-00000e60: 0a2d 20e8 87aa e58a a8e5 ae8c e688 90e6  .- .............
-00000e70: af8f e697 a5e7 b1b3 e6b8 b8e5 b881 e4bb  ................
-00000e80: bbe5 8aa1 0a2d 20e8 87aa e58a a8e8 bf9b  .....- .........
-00000e90: e8a1 8ce6 b8b8 e688 8fe7 adbe e588 b00a  ................
-00000ea0: 2d20 e58f afe5 88b6 e5ae 9ae7 b1b3 e6b8  - ..............
-00000eb0: b8e5 b881 e595 86e5 9381 e585 91e6 8da2  ................
-00000ec0: e8ae a1e5 8892 efbc 8ce5 88b0 e782 b9e5  ................
-00000ed0: 8591 e68d a2ef bc88 e59b a0e5 8aa0 e585  ................
-00000ee0: a5e4 ba86 e4ba bae6 9cba e9aa 8ce8 af81  ................
-00000ef0: efbc 8ce6 8890 e58a 9fe7 8e87 e8be 83e4  ................
-00000f00: bd8e efbc 890a 2d20 e58f afe6 94af e68c  ......- ........
-00000f10: 81e5 a49a e4b8 aa20 5151 20e8 b4a6 e58f  ....... QQ .....
-00000f20: b7ef bc8c e6af 8fe4 b8aa 2051 5120 e8b4  .......... QQ ..
-00000f30: a6e5 8fb7 e58f afe7 bb91 e5ae 9ae5 a49a  ................
-00000f40: e4b8 aae7 b1b3 e593 88e6 b8b8 e8b4 a6e6  ................
-00000f50: 88b7 0a2d 2051 5120 e68e a8e9 8081 e689  ...- QQ ........
-00000f60: a7e8 a18c e7bb 93e6 9e9c e980 9ae7 9fa5  ................
-00000f70: 0a2d 20e5 8e9f e7a5 9ee3 8081 e5b4 a9e5  .- .............
-00000f80: 9d8f efbc 9ae6 989f e7a9 b9e9 9381 e981  ................
-00000f90: 93e7 8ab6 e680 81e4 bebf e7ac bae9 809a  ................
-00000fa0: e79f a50a 2d20 e58f afe4 b8ba e799 bbe5  ....- ..........
-00000fb0: bd95 e380 81e6 af8f e697 a5e7 b1b3 e6b8  ................
-00000fc0: b8e5 b881 e4bb bbe5 8aa1 e380 81e6 b8b8  ................
-00000fd0: e688 8fe7 adbe e588 b0e9 858d e7bd aee4  ................
-00000fe0: baba e69c bae9 aa8c e8af 81e6 8993 e7a0  ................
-00000ff0: 81e5 b9b3 e58f b00a 2d20 e58f afe9 858d  ........- ......
-00001000: e7bd aee7 94a8 e688 b7e9 bb91 e590 8de5  ................
-00001010: 8d95 2fe7 99bd e590 8de5 8d95 0a0a 2323  ../...........##
-00001020: 20f0 9f93 9620 e4bd bfe7 94a8 e8af b4e6   .... ..........
-00001030: 988e 0a0a 2323 2320 f09f 9ba0 efb8 8f20  ....### ....... 
-00001040: 4e6f 6e65 426f 7432 20e6 9cba e599 a8e4  NoneBot2 .......
-00001050: baba e983 a8e7 bdb2 e592 8ce6 8f92 e4bb  ................
-00001060: b6e5 ae89 e8a3 850a 0ae8 afb7 e69f a5e7  ................
-00001070: 9c8b 202d 3e20 5bf0 9f94 9749 6e73 7461  .. -> [....Insta
-00001080: 6c6c 6174 696f 6e5d 2868 7474 7073 3a2f  llation](https:/
-00001090: 2f67 6974 6875 622e 636f 6d2f 4c6a 7a64  /github.com/Ljzd
-000010a0: 2d50 524f 2f6e 6f6e 6562 6f74 2d70 6c75  -PRO/nonebot-plu
-000010b0: 6769 6e2d 6d79 7374 6f6f 6c2f 7769 6b69  gin-mystool/wiki
-000010c0: 2f49 6e73 7461 6c6c 6174 696f 6e29 0a0a  /Installation)..
-000010d0: 2323 2320 f09f 9396 20e6 8f92 e4bb b6e5  ### .... .......
-000010e0: 85b7 e4bd 93e4 bdbf e794 a8e8 afb4 e698  ................
-000010f0: 8e0a 0ae8 afb7 e69f a5e7 9c8b 202d 3e20  ............ -> 
-00001100: 5bf0 9f94 9757 696b 6920 e696 87e6 a1a3  [....Wiki ......
-00001110: 5d28 6874 7470 733a 2f2f 6769 7468 7562  ](https://github
-00001120: 2e63 6f6d 2f4c 6a7a 642d 5052 4f2f 6e6f  .com/Ljzd-PRO/no
-00001130: 6e65 626f 742d 706c 7567 696e 2d6d 7973  nebot-plugin-mys
-00001140: 746f 6f6c 2f77 696b 6929 0a0a 2323 2320  tool/wiki)..### 
-00001150: e29d 9320 e88e b7e5 8f96 e68f 92e4 bbb6  ... ............
-00001160: e5b8 aee5 8aa9 e4bf a1e6 81af 0a0a 2323  ..............##
-00001170: 2323 20e6 8f92 e4bb b6e5 91bd e4bb a40a  ## .............
-00001180: 0a60 6060 0a2f e5b8 aee5 8aa9 0a60 6060  .```./.......```
-00001190: 0a0a 3e20 5b21 4e4f 5445 5d0a 3e20 e6ad  ..> [!NOTE].> ..
-000011a0: a4e5 a484 e6b2 a1e6 9c89 e4bd bfe7 94a8  ................
-000011b0: 205b f09f 9497 20e6 8f92 e4bb b6e5 91bd   [.... .........
-000011c0: e4bb a4e5 a4b4 5d28 6874 7470 733a 2f2f  ......](https://
-000011d0: 6769 7468 7562 2e63 6f6d 2f4c 6a7a 642d  github.com/Ljzd-
-000011e0: 5052 4f2f 6e6f 6e65 626f 742d 706c 7567  PRO/nonebot-plug
-000011f0: 696e 2d6d 7973 746f 6f6c 2f77 696b 692f  in-mystool/wiki/
-00001200: 436f 6e66 6967 7572 6174 696f 6e2d 5072  Configuration-Pr
-00001210: 6566 6572 656e 6365 2363 6f6d 6d61 6e64  eference#command
-00001220: 5f73 7461 7274 290a 0a23 2320 e585 b6e4  _start)..## ....
-00001230: bb96 0a0a 2323 2320 e8b4 a1e7 8cae 0a3c  ....### .......<
-00001240: 6120 6872 6566 3d22 6874 7470 733a 2f2f  a href="https://
-00001250: 6769 7468 7562 2e63 6f6d 2f4c 6a7a 642d  github.com/Ljzd-
-00001260: 5052 4f2f 6e6f 6e65 626f 742d 706c 7567  PRO/nonebot-plug
-00001270: 696e 2d6d 7973 746f 6f6c 2f67 7261 7068  in-mystool/graph
-00001280: 732f 636f 6e74 7269 6275 746f 7273 223e  s/contributors">
-00001290: 0a20 203c 696d 6720 7372 633d 2268 7474  .  <img src="htt
-000012a0: 7073 3a2f 2f63 6f6e 7472 6962 2e72 6f63  ps://contrib.roc
-000012b0: 6b73 2f69 6d61 6765 3f72 6570 6f3d 4c6a  ks/image?repo=Lj
-000012c0: 7a64 2d50 524f 2f6e 6f6e 6562 6f74 2d70  zd-PRO/nonebot-p
-000012d0: 6c75 6769 6e2d 6d79 7374 6f6f 6c26 6d61  lugin-mystool&ma
-000012e0: 783d 3130 3030 2220 616c 743d 22e8 b4a1  x=1000" alt="...
-000012f0: e78c aee8 8085 222f 3e0a 3c2f 613e 0a0a  ......"/>.</a>..
-00001300: 2323 2320 f09f 94a8 20e5 bc80 e58f 91e7  ### .... .......
-00001310: 8988 e588 86e6 94af 0a5b 2a2a f09f 94a8  .........[**....
-00001320: 6465 762a 2a5d 2868 7474 7073 3a2f 2f67  dev**](https://g
-00001330: 6974 6875 622e 636f 6d2f 4c6a 7a64 2d50  ithub.com/Ljzd-P
-00001340: 524f 2f6e 6f6e 6562 6f74 2d70 6c75 6769  RO/nonebot-plugi
-00001350: 6e2d 6d79 7374 6f6f 6c2f 7472 6565 2f64  n-mystool/tree/d
-00001360: 6576 290a 0a23 2323 20f0 9f93 8320 e6ba  ev)..### .... ..
-00001370: 90e7 a081 e8af b4e6 988e 0a5b f09f 9383  ...........[....
-00001380: 536f 7572 6365 2d53 7472 7563 7475 7265  Source-Structure
-00001390: 5d28 6874 7470 733a 2f2f 6769 7468 7562  ](https://github
-000013a0: 2e63 6f6d 2f4c 6a7a 642d 5052 4f2f 6e6f  .com/Ljzd-PRO/no
-000013b0: 6e65 626f 742d 706c 7567 696e 2d6d 7973  nebot-plugin-mys
-000013c0: 746f 6f6c 2f77 696b 692f 536f 7572 6365  tool/wiki/Source
-000013d0: 2d53 7472 7563 7475 7265 290a 0a23 2323  -Structure)..###
-000013e0: 20e9 8082 e985 8d20 5be7 bbaa e5b1 b1e7   ...... [.......
-000013f0: 9c9f e5af bb42 6f74 5d28 6874 7470 733a  .....Bot](https:
-00001400: 2f2f 6769 7468 7562 2e63 6f6d 2f48 6962  //github.com/Hib
-00001410: 694b 6965 722f 7a68 656e 7875 6e5f 626f  iKier/zhenxun_bo
-00001420: 7429 20e7 9a84 e588 86e6 94af 0a2d 2068  t) ..........- h
-00001430: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
-00001440: 6d2f 4d57 544a 432f 7a68 656e 7875 6e2d  m/MWTJC/zhenxun-
-00001450: 706c 7567 696e 2d6d 7973 746f 6f6c 0a2d  plugin-mystool.-
-00001460: 2068 7474 7073 3a2f 2f67 6974 6875 622e   https://github.
-00001470: 636f 6d2f 6179 616b 6173 756b 692f 6e6f  com/ayakasuki/no
-00001480: 6e65 626f 742d 706c 7567 696e 2d6d 7973  nebot-plugin-mys
-00001490: 746f 6f6c 0a0a                           tool..
+00000ac0: 2320 e29a a120 e58a 9fe8 83bd e592 8ce7  # ... ..........
+00000ad0: 89b9 e680 a70a 0a2d 20e6 94af e68c 8151  .......- ......Q
+00000ae0: 51e8 818a e5a4 a9e5 928c 5151 e9a2 91e9  Q.........QQ....
+00000af0: 8193 0a2d 20e7 9fad e4bf a1e9 aa8c e8af  ...- ...........
+00000b00: 81e7 99bb e5bd 95ef bc8c e585 8de6 8a93  ................
+00000b10: e58c 85e8 8eb7 e58f 9620 436f 6f6b 6965  ......... Cookie
+00000b20: 0a2d 20e8 87aa e58a a8e5 ae8c e688 90e6  .- .............
+00000b30: af8f e697 a5e7 b1b3 e6b8 b8e5 b881 e4bb  ................
+00000b40: bbe5 8aa1 0a2d 20e8 87aa e58a a8e8 bf9b  .....- .........
+00000b50: e8a1 8ce6 b8b8 e688 8fe7 adbe e588 b00a  ................
+00000b60: 2d20 e58f afe5 88b6 e5ae 9ae7 b1b3 e6b8  - ..............
+00000b70: b8e5 b881 e595 86e5 9381 e585 91e6 8da2  ................
+00000b80: e8ae a1e5 8892 efbc 8ce5 88b0 e782 b9e5  ................
+00000b90: 8591 e68d a2ef bc88 e59b a0e5 8aa0 e585  ................
+00000ba0: a5e4 ba86 e4ba bae6 9cba e9aa 8ce8 af81  ................
+00000bb0: efbc 8ce6 8890 e58a 9fe7 8e87 e8be 83e4  ................
+00000bc0: bd8e efbc 890a 2d20 e58f afe6 94af e68c  ......- ........
+00000bd0: 81e5 a49a e4b8 aa20 5151 20e8 b4a6 e58f  ....... QQ .....
+00000be0: b7ef bc8c e6af 8fe4 b8aa 2051 5120 e8b4  .......... QQ ..
+00000bf0: a6e5 8fb7 e58f afe7 bb91 e5ae 9ae5 a49a  ................
+00000c00: e4b8 aae7 b1b3 e593 88e6 b8b8 e8b4 a6e6  ................
+00000c10: 88b7 0a2d 2051 5120 e68e a8e9 8081 e689  ...- QQ ........
+00000c20: a7e8 a18c e7bb 93e6 9e9c e980 9ae7 9fa5  ................
+00000c30: 0a2d 20e5 8e9f e7a5 9ee3 8081 e5b4 a9e5  .- .............
+00000c40: 9d8f efbc 9ae6 989f e7a9 b9e9 9381 e981  ................
+00000c50: 93e7 8ab6 e680 81e4 bebf e7ac bae9 809a  ................
+00000c60: e79f a50a 2d20 e58f afe4 b8ba e799 bbe5  ....- ..........
+00000c70: bd95 e380 81e6 af8f e697 a5e7 b1b3 e6b8  ................
+00000c80: b8e5 b881 e4bb bbe5 8aa1 e380 81e6 b8b8  ................
+00000c90: e688 8fe7 adbe e588 b0e9 858d e7bd aee4  ................
+00000ca0: baba e69c bae9 aa8c e8af 81e6 8993 e7a0  ................
+00000cb0: 81e5 b9b3 e58f b00a 2d20 e58f afe9 858d  ........- ......
+00000cc0: e7bd aee7 94a8 e688 b7e9 bb91 e590 8de5  ................
+00000cd0: 8d95 2fe7 99bd e590 8de5 8d95 0a0a 2323  ../...........##
+00000ce0: 20f0 9f93 9620 e4bd bfe7 94a8 e8af b4e6   .... ..........
+00000cf0: 988e 0a0a 2323 2320 f09f 9ba0 efb8 8f20  ....### ....... 
+00000d00: 4e6f 6e65 426f 7432 20e6 9cba e599 a8e4  NoneBot2 .......
+00000d10: baba e983 a8e7 bdb2 e592 8ce6 8f92 e4bb  ................
+00000d20: b6e5 ae89 e8a3 850a 0ae8 afb7 e69f a5e7  ................
+00000d30: 9c8b 202d 3e20 5bf0 9f94 9749 6e73 7461  .. -> [....Insta
+00000d40: 6c6c 6174 696f 6e5d 2868 7474 7073 3a2f  llation](https:/
+00000d50: 2f67 6974 6875 622e 636f 6d2f 4c6a 7a64  /github.com/Ljzd
+00000d60: 2d50 524f 2f6e 6f6e 6562 6f74 2d70 6c75  -PRO/nonebot-plu
+00000d70: 6769 6e2d 6d79 7374 6f6f 6c2f 7769 6b69  gin-mystool/wiki
+00000d80: 2f49 6e73 7461 6c6c 6174 696f 6e29 0a0a  /Installation)..
+00000d90: 2323 2320 f09f 9396 20e6 8f92 e4bb b6e5  ### .... .......
+00000da0: 85b7 e4bd 93e4 bdbf e794 a8e8 afb4 e698  ................
+00000db0: 8e0a 0ae8 afb7 e69f a5e7 9c8b 202d 3e20  ............ -> 
+00000dc0: 5bf0 9f94 9757 696b 6920 e696 87e6 a1a3  [....Wiki ......
+00000dd0: 5d28 6874 7470 733a 2f2f 6769 7468 7562  ](https://github
+00000de0: 2e63 6f6d 2f4c 6a7a 642d 5052 4f2f 6e6f  .com/Ljzd-PRO/no
+00000df0: 6e65 626f 742d 706c 7567 696e 2d6d 7973  nebot-plugin-mys
+00000e00: 746f 6f6c 2f77 696b 6929 0a0a 2323 2320  tool/wiki)..### 
+00000e10: e29d 9320 e88e b7e5 8f96 e68f 92e4 bbb6  ... ............
+00000e20: e5b8 aee5 8aa9 e4bf a1e6 81af 0a0a 2323  ..............##
+00000e30: 2323 20e6 8f92 e4bb b6e5 91bd e4bb a40a  ## .............
+00000e40: 0a60 6060 0a2f e5b8 aee5 8aa9 0a60 6060  .```./.......```
+00000e50: 0a0a 3e20 5b21 4e4f 5445 5d0a 3e20 e6ad  ..> [!NOTE].> ..
+00000e60: a4e5 a484 e6b2 a1e6 9c89 e4bd bfe7 94a8  ................
+00000e70: 205b f09f 9497 20e6 8f92 e4bb b6e5 91bd   [.... .........
+00000e80: e4bb a4e5 a4b4 5d28 6874 7470 733a 2f2f  ......](https://
+00000e90: 6769 7468 7562 2e63 6f6d 2f4c 6a7a 642d  github.com/Ljzd-
+00000ea0: 5052 4f2f 6e6f 6e65 626f 742d 706c 7567  PRO/nonebot-plug
+00000eb0: 696e 2d6d 7973 746f 6f6c 2f77 696b 692f  in-mystool/wiki/
+00000ec0: 436f 6e66 6967 7572 6174 696f 6e2d 5072  Configuration-Pr
+00000ed0: 6566 6572 656e 6365 2363 6f6d 6d61 6e64  eference#command
+00000ee0: 5f73 7461 7274 290a 0a23 2320 e585 b6e4  _start)..## ....
+00000ef0: bb96 0a0a 2323 2320 e8b4 a1e7 8cae 0a3c  ....### .......<
+00000f00: 6120 6872 6566 3d22 6874 7470 733a 2f2f  a href="https://
+00000f10: 6769 7468 7562 2e63 6f6d 2f4c 6a7a 642d  github.com/Ljzd-
+00000f20: 5052 4f2f 6e6f 6e65 626f 742d 706c 7567  PRO/nonebot-plug
+00000f30: 696e 2d6d 7973 746f 6f6c 2f67 7261 7068  in-mystool/graph
+00000f40: 732f 636f 6e74 7269 6275 746f 7273 223e  s/contributors">
+00000f50: 0a20 203c 696d 6720 7372 633d 2268 7474  .  <img src="htt
+00000f60: 7073 3a2f 2f63 6f6e 7472 6962 2e72 6f63  ps://contrib.roc
+00000f70: 6b73 2f69 6d61 6765 3f72 6570 6f3d 4c6a  ks/image?repo=Lj
+00000f80: 7a64 2d50 524f 2f6e 6f6e 6562 6f74 2d70  zd-PRO/nonebot-p
+00000f90: 6c75 6769 6e2d 6d79 7374 6f6f 6c26 6d61  lugin-mystool&ma
+00000fa0: 783d 3130 3030 2220 616c 743d 22e8 b4a1  x=1000" alt="...
+00000fb0: e78c aee8 8085 222f 3e0a 3c2f 613e 0a0a  ......"/>.</a>..
+00000fc0: 2323 2320 f09f 94a8 20e5 bc80 e58f 91e7  ### .... .......
+00000fd0: 8988 e588 86e6 94af 0a5b 2a2a f09f 94a8  .........[**....
+00000fe0: 6465 762a 2a5d 2868 7474 7073 3a2f 2f67  dev**](https://g
+00000ff0: 6974 6875 622e 636f 6d2f 4c6a 7a64 2d50  ithub.com/Ljzd-P
+00001000: 524f 2f6e 6f6e 6562 6f74 2d70 6c75 6769  RO/nonebot-plugi
+00001010: 6e2d 6d79 7374 6f6f 6c2f 7472 6565 2f64  n-mystool/tree/d
+00001020: 6576 290a 0a23 2323 20f0 9f93 8320 e6ba  ev)..### .... ..
+00001030: 90e7 a081 e8af b4e6 988e 0a5b f09f 9383  ...........[....
+00001040: 536f 7572 6365 2d53 7472 7563 7475 7265  Source-Structure
+00001050: 5d28 6874 7470 733a 2f2f 6769 7468 7562  ](https://github
+00001060: 2e63 6f6d 2f4c 6a7a 642d 5052 4f2f 6e6f  .com/Ljzd-PRO/no
+00001070: 6e65 626f 742d 706c 7567 696e 2d6d 7973  nebot-plugin-mys
+00001080: 746f 6f6c 2f77 696b 692f 536f 7572 6365  tool/wiki/Source
+00001090: 2d53 7472 7563 7475 7265 290a 0a23 2323  -Structure)..###
+000010a0: 20e9 8082 e985 8d20 5be7 bbaa e5b1 b1e7   ...... [.......
+000010b0: 9c9f e5af bb42 6f74 5d28 6874 7470 733a  .....Bot](https:
+000010c0: 2f2f 6769 7468 7562 2e63 6f6d 2f48 6962  //github.com/Hib
+000010d0: 694b 6965 722f 7a68 656e 7875 6e5f 626f  iKier/zhenxun_bo
+000010e0: 7429 20e7 9a84 e588 86e6 94af 0a2d 2068  t) ..........- h
+000010f0: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
+00001100: 6d2f 4d57 544a 432f 7a68 656e 7875 6e2d  m/MWTJC/zhenxun-
+00001110: 706c 7567 696e 2d6d 7973 746f 6f6c 0a2d  plugin-mystool.-
+00001120: 2068 7474 7073 3a2f 2f67 6974 6875 622e   https://github.
+00001130: 636f 6d2f 6179 616b 6173 756b 692f 6e6f  com/ayakasuki/no
+00001140: 6e65 626f 742d 706c 7567 696e 2d6d 7973  nebot-plugin-mys
+00001150: 746f 6f6c 0a0a                           tool..
```

