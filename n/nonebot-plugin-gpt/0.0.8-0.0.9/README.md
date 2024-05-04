# Comparing `tmp/nonebot-plugin-gpt-0.0.8.tar.gz` & `tmp/nonebot-plugin-gpt-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot-plugin-gpt-0.0.8.tar", last modified: Wed Mar 13 08:16:26 2024, max compression
+gzip compressed data, was "nonebot-plugin-gpt-0.0.9.tar", last modified: Sun Mar 17 13:15:12 2024, max compression
```

## Comparing `nonebot-plugin-gpt-0.0.8.tar` & `nonebot-plugin-gpt-0.0.9.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0    35149 2024-03-13 08:16:23.161086 nonebot-plugin-gpt-0.0.8/LICENSE
--rw-r--r--   0        0        0     7325 2024-03-13 08:16:23.161086 nonebot-plugin-gpt-0.0.8/README.md
--rw-r--r--   0        0        0    11429 2024-03-13 08:16:23.161086 nonebot-plugin-gpt-0.0.8/nonebot_plugin_gpt/__init__.py
--rw-r--r--   0        0        0    27736 2024-03-13 08:16:23.161086 nonebot-plugin-gpt-0.0.8/nonebot_plugin_gpt/api.py
--rw-r--r--   0        0        0     4785 2024-03-13 08:16:23.161086 nonebot-plugin-gpt-0.0.8/nonebot_plugin_gpt/check.py
--rw-r--r--   0        0        0     5843 2024-03-13 08:16:23.161086 nonebot-plugin-gpt-0.0.8/nonebot_plugin_gpt/config.py
--rw-r--r--   0        0        0     2028 2024-03-13 08:16:23.161086 nonebot-plugin-gpt-0.0.8/nonebot_plugin_gpt/source.py
--rw-r--r--   0        0        0      745 2024-03-13 08:16:23.161086 nonebot-plugin-gpt-0.0.8/pyproject.toml
--rw-r--r--   0        0        0     7684 1970-01-01 00:00:00.000000 nonebot-plugin-gpt-0.0.8/PKG-INFO
+-rw-r--r--   0        0        0    35149 2024-03-17 13:15:02.897368 nonebot-plugin-gpt-0.0.9/LICENSE
+-rw-r--r--   0        0        0     7689 2024-03-17 13:15:02.901368 nonebot-plugin-gpt-0.0.9/README.md
+-rw-r--r--   0        0        0    11429 2024-03-17 13:15:02.901368 nonebot-plugin-gpt-0.0.9/nonebot_plugin_gpt/__init__.py
+-rw-r--r--   0        0        0    27887 2024-03-17 13:15:02.901368 nonebot-plugin-gpt-0.0.9/nonebot_plugin_gpt/api.py
+-rw-r--r--   0        0        0     4785 2024-03-17 13:15:02.901368 nonebot-plugin-gpt-0.0.9/nonebot_plugin_gpt/check.py
+-rw-r--r--   0        0        0     6239 2024-03-17 13:15:02.901368 nonebot-plugin-gpt-0.0.9/nonebot_plugin_gpt/config.py
+-rw-r--r--   0        0        0     2028 2024-03-17 13:15:02.901368 nonebot-plugin-gpt-0.0.9/nonebot_plugin_gpt/source.py
+-rw-r--r--   0        0        0      745 2024-03-17 13:15:02.901368 nonebot-plugin-gpt-0.0.9/pyproject.toml
+-rw-r--r--   0        0        0     8048 1970-01-01 00:00:00.000000 nonebot-plugin-gpt-0.0.9/PKG-INFO
```

### Comparing `nonebot-plugin-gpt-0.0.8/LICENSE` & `nonebot-plugin-gpt-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-gpt-0.0.8/README.md` & `nonebot-plugin-gpt-0.0.9/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -68,14 +68,21 @@
 
 打开 nonebot2 项目根目录下的 `pyproject.toml` 文件, 在 `[tool.nonebot]` 部分追加写入
 
     plugins = ["nonebot_plugin_gpt"]
 
 </details>
 
+<details open>
+<summary>升级插件版本</summary>
+
+    pip install nonebot-plugin-gpt -U
+
+</details>
+
 ## ⚙️ 配置
 
 在 nonebot2 项目的`.env`文件中添加下表中的必填配置
 
 | 配置项 | 必填 | 默认值 | 类型 | 说明 |
 |:-----:|:----:|:----:|:----:|:----:|
 | gpt_session | 是 | 无 | List[Dict[str,str]] | openai账号密码 |
@@ -87,14 +94,15 @@
 | begin_sleep_time | 否 | false | bool | 关闭启动等待时间（建议账号数量大于5开启） |
 | gpt_chat_priority | 否 | 90 | int | gpt聊天响应优先级 |
 | gpt_command_priority | 否 | 19 | int | gpt命令响应优先级 |
 | gpt_white_list_mode | 否 | true | bool | 聊天白名单模式 |
 | gpt_replay_to_replay | 否 | false | bool | 是否响应"回复消息" |
 | gpt_ban_str | 否 | 无 | List[str] | 黑名单屏蔽词列表 |
 | gpt_manage_ids | 否 | 无 | List[str] | 超管群/频道id，通过日志等方式获得 |
+| gpt_lgr_markdown| 否 | false | bool | 以拉格兰md消息回复 |
 
 ```bash
 # gpt配置示例
 # 当mode为空或者为openai时，建议提前手动登录一次获取session_token填入（成功使用后可删除session_token项），mode目前不支持苹果账号
 gpt_session='[
     {
         "email": "xxxx@hotmail.com",
@@ -136,14 +144,16 @@
 
 gpt_ban_str='[
     "我是猪",
     "你是猪",
 ]'
 # qq适配器使用的超管群id
 gpt_manage_ids=['qq group id......']
+# onebot适配器 拉格兰md消息兼容
+gpt_lgr_markdown=false
 
 # 插件需要一些其他的Nonebot基础配置，请检查是否存在
 # 机器人名
 nickname=["bot name"]
 # 超管QQ（onebot用）
 SUPERUSERS=["qq num"]
 
@@ -177,14 +187,19 @@
 <为必填内容>，(为选填内容)
 
 ## 常见问题
 ### 微软辅助邮箱验证
 当触发验证后，会在启动目录生成带有启动账号名称的文件，键入收到的验证码并保存，即可自动验证。留意日志输出提示
 
 ### 更新日志
+2024.03.17
+1. 优化了底层代码，减少错误，暂不支持gpt plus账号（待填坑）
+2. 支持拉格兰md发送
+
+
 2024.03.13
 1. 兼容拉格兰合并转发，修复合并转发失败的问题
 2. 添加自定义聊天前缀，现在可以不用@也能触发了
 
 
 2024.03.11
 1. 临时修复200问题（chatgpt新的websocket问题），最近好忙，等闲了的时候再优化，有什么问题都可以先提issue
```

#### html2text {}

```diff
@@ -8,15 +8,16 @@
 é¡¹ç®çæ ¹ç®å½ä¸æå¼å½ä»¤è¡, è¾å¥ä»¥ä¸æä»¤å³å¯å®è£ nb plugin
 install nonebot-plugin-gpt ä½¿ç¨åç®¡çå¨å®è£ å¨ nonebot2
 é¡¹ç®çæä»¶ç®å½ä¸, æå¼å½ä»¤è¡, æ ¹æ®ä½ ä½¿ç¨çåç®¡çå¨,
 è¾å¥ç¸åºçå®è£å½ä»¤ pip pip install nonebot-plugin-gpt pdm pdm add
 nonebot-plugin-gpt poetry poetry add nonebot-plugin-gpt conda conda install
 nonebot-plugin-gpt æå¼ nonebot2 é¡¹ç®æ ¹ç®å½ä¸ç `pyproject.toml`
 æä»¶, å¨ `[tool.nonebot]` é¨åè¿½å åå¥ plugins =
-["nonebot_plugin_gpt"] ## âï¸ éç½® å¨ nonebot2
+["nonebot_plugin_gpt"] åçº§æä»¶çæ¬ pip install nonebot-plugin-gpt -U ##
+âï¸ éç½® å¨ nonebot2
 é¡¹ç®ç`.env`æä»¶ä¸­æ·»å ä¸è¡¨ä¸­çå¿å¡«éç½® | éç½®é¡¹ | å¿å¡« |
 é»è®¤å¼ | ç±»å | è¯´æ | |:-----:|:----:|:----:|:----:|:----:| |
 gpt_session | æ¯ | æ  | List[Dict[str,str]] | openaiè´¦å·å¯ç  | |
 gpt_proxy | å¦ | æ  | str | ä½¿ç¨çä»£ç | | arkose_status | å¦ | false |
 bool | gptæ¯å¦å¼å¯äºarkoseéªè¯ | | group_chat | å¦ | true | bool |
 ç¾¤éå¼å¯å¤äººè¯å« | | gpt_chat_start | å¦ | [] | list |
 èå¤©åç¼ï¼åènbå½ä»¤åç¼ | | gpt_chat_start_in_msg | å¦ | false |
@@ -24,25 +25,27 @@
 | bool | å³é­å¯å¨ç­å¾æ¶é´ï¼å»ºè®®è´¦å·æ°éå¤§äº5å¼å¯ï¼ | |
 gpt_chat_priority | å¦ | 90 | int | gptèå¤©ååºä¼åçº§ | |
 gpt_command_priority | å¦ | 19 | int | gptå½ä»¤ååºä¼åçº§ | |
 gpt_white_list_mode | å¦ | true | bool | èå¤©ç½ååæ¨¡å¼ | |
 gpt_replay_to_replay | å¦ | false | bool | æ¯å¦ååº"åå¤æ¶æ¯" | |
 gpt_ban_str | å¦ | æ  | List[str] | é»ååå±è½è¯åè¡¨ | |
 gpt_manage_ids | å¦ | æ  | List[str] | è¶ç®¡ç¾¤/
-é¢éidï¼éè¿æ¥å¿ç­æ¹å¼è·å¾ | ```bash # gptéç½®ç¤ºä¾ #
+é¢éidï¼éè¿æ¥å¿ç­æ¹å¼è·å¾ | | gpt_lgr_markdown| å¦ | false | bool
+| ä»¥ææ ¼å°mdæ¶æ¯åå¤ | ```bash # gptéç½®ç¤ºä¾ #
 å½modeä¸ºç©ºæèä¸ºopenaiæ¶ï¼å»ºè®®æåæå¨ç»å½ä¸æ¬¡è·åsession_tokenå¡«å¥ï¼æåä½¿ç¨åå¯å é¤session_tokené¡¹ï¼ï¼modeç®åä¸æ¯æè¹æè´¦å·
 gpt_session='[ { "email": "xxxx@hotmail.com", "password": "xxxx",
 "session_token": "ey....", }, { "email": "aaaa@gmail.com", "password": "xxxx",
 "mode": "google", }, { "email": "bbb@sss.com", "password": "xxxx", "mode":
 "microsoft", "help_email": "xxx@xx.com" }, ]' gpt_proxy='http://127.0.0.1:8080'
 arkose_status=false group_chat=true gpt_chat_start=[]
 gpt_chat_start_in_msg=false begin_sleep_time=true gpt_chat_priority=90
 gpt_command_priority=19 gpt_white_list_mode=true gpt_replay_to_replay=false
 gpt_ban_str='[ "ææ¯çª", "ä½ æ¯çª", ]' # qqééå¨ä½¿ç¨çè¶ç®¡ç¾¤id
-gpt_manage_ids=['qq group id......'] #
+gpt_manage_ids=['qq group id......'] # onebotééå¨ ææ ¼å°mdæ¶æ¯å¼å®¹
+gpt_lgr_markdown=false #
 æä»¶éè¦ä¸äºå¶ä»çNonebotåºç¡éç½®ï¼è¯·æ£æ¥æ¯å¦å­å¨ #
 æºå¨äººå nickname=["bot name"] # è¶ç®¡QQï¼onebotç¨ï¼ SUPERUSERS=["qq
 num"] ``` ## ð ä½¿ç¨ ### æä»¤è¡¨ | æä»¤ | ééå¨ | æé | éè¦@
 | èå´ | è¯´æ | |:-----:|:----:|:----:|:----:|:----:|:----:| | @bot
 èå¤©åå®¹... | å¼å®¹ | æ /ç½åå | æ¯ | ç¾¤è/ç§è/é¢é |
 @æèå«å+åå®¹ å¼å§èå¤©ï¼éææèç½ååæ¨¡å¼è®¾ç½®æ¹å | |
 åå§å | å¼å®¹ | æ /ç½åå | æ¯ | ç¾¤è/ç§è/é¢é | åå§å
@@ -76,13 +79,15 @@
 è¶ç®¡ç¾¤ | æ¯ | ç¾¤è/é¢é | çæcdk
 ¤å·/å¶ä»ä¿¡æ¯>ï¼ä»¥ç»å®ä¿¡æ¯æ¹å¼çæç½ååcdk | | åºç°å§ | qq
 | æ  | æ¯ | ç¾¤è/é¢é | åºç°å§ \
 >ï¼ä»¥ç»å®idå½¢å¼ä½¿ç¨cdkå å¥ç½åå | | ç»æå§ | qq | ç½åå |
 æ¯ | ç¾¤è/é¢é | ç»æå§ ï¼ç¨æ·èªä¸»è§£é¤ç½åå |
 ºå¿å¡«åå®¹>ï¼(ä¸ºéå¡«åå®¹) ## å¸¸è§é®é¢ ### å¾®è½¯è¾å©é®ç®±éªè¯
 å½è§¦åéªè¯åï¼ä¼å¨å¯å¨ç®å½çæå¸¦æå¯å¨è´¦å·åç§°çæä»¶ï¼é®å¥æ¶å°çéªè¯ç å¹¶ä¿å­ï¼å³å¯èªå¨éªè¯ãçææ¥å¿è¾åºæç¤º
-### æ´æ°æ¥å¿ 2024.03.13 1.
+### æ´æ°æ¥å¿ 2024.03.17 1.
+ä¼åäºåºå±ä»£ç ï¼åå°éè¯¯ï¼æä¸æ¯ægpt
+plusè´¦å·ï¼å¾å¡«åï¼ 2. æ¯æææ ¼å°mdåé 2024.03.13 1.
 å¼å®¹ææ ¼å°åå¹¶è½¬åï¼ä¿®å¤åå¹¶è½¬åå¤±è´¥çé®é¢ 2.
 æ·»å èªå®ä¹èå¤©åç¼ï¼ç°å¨å¯ä»¥ä¸ç¨@ä¹è½è§¦åäº 2024.03.11 1.
 ä¸´æ¶ä¿®å¤200é®é¢ï¼chatgptæ°çwebsocketé®é¢ï¼ï¼æè¿å¥½å¿ï¼ç­é²äºçæ¶ååä¼åï¼æä»ä¹é®é¢é½å¯ä»¥åæissue
 2024.02.19 1. ä¸´æ¶ä¿®å¤200é®é¢ ä¸ æ·»å  å¾®è½¯è¾å©é®ç®±éªè¯ ##
 å¾ç»­ èªç¨æºä¹äºï¼åå¿æ¹æ¹ååºæ¥ï¼å¾å¤ä¸è¥¿è¿æ²¡è¡¥å
```

### Comparing `nonebot-plugin-gpt-0.0.8/nonebot_plugin_gpt/__init__.py` & `nonebot-plugin-gpt-0.0.9/nonebot_plugin_gpt/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-gpt-0.0.8/nonebot_plugin_gpt/api.py` & `nonebot-plugin-gpt-0.0.9/nonebot_plugin_gpt/api.py`

 * *Files 1% similar despite different names*

```diff
@@ -115,14 +115,18 @@
         data.msg_send=text_handle
         data = await chatbot.continue_chat(data)
         tmp[id] = data.conversation_id
         grouppath.write_text(json.dumps(tmp))
         
     await ban_check(event,matcher,Message(data.msg_recv))
     
+    if config_gpt.gpt_lgr_markdown and isinstance(event,MessageEvent):
+        await tools.send_text2md(data.msg_recv)
+        await matcher.finish()
+
     await matcher.finish(replace_name(data).msg_recv)
     
 
 async def reset_history(event: MessageEvent|QQMessageEvent,chatbot: chatgpt):
     '''重置'''
     matcher: Matcher = current_matcher.get()
     await ban_check(event,matcher)
```

### Comparing `nonebot-plugin-gpt-0.0.8/nonebot_plugin_gpt/check.py` & `nonebot-plugin-gpt-0.0.9/nonebot_plugin_gpt/check.py`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-gpt-0.0.8/nonebot_plugin_gpt/config.py` & `nonebot-plugin-gpt-0.0.9/nonebot_plugin_gpt/config.py`

 * *Files 4% similar despite different names*

```diff
@@ -17,14 +17,15 @@
     begin_sleep_time: bool = False
     gpt_chat_priority: int = 90
     gpt_command_priority: int = 19
     gpt_white_list_mode: bool = True
     gpt_replay_to_replay: bool = False
     gpt_ban_str: Optional[List[str]]|str = []
     gpt_manage_ids: list = []
+    gpt_lgr_markdown: bool = False
     
     @validator("gpt_manage_ids", always=True, pre=True)
     def check_gpt_manage_ids(cls,v):
         if isinstance(v,list):
             if v != []:
                 logger.success(f"已开启 官方管理群 gpt_manage_ids {v}")
             else:
@@ -146,10 +147,18 @@
                 else:
                     logger.warning(f"未配置 gpt 屏蔽词")
                 return v 
             logger.warning(f"未配置 gpt 屏蔽词")
         except Exception as e:
             logger.warning(f"未配置 gpt 屏蔽词")
 
-                            
+    @validator("gpt_lgr_markdown", always=True, pre=True)
+    def check_gpt_lgr_markdown(cls,v):
+        if isinstance(v,bool):
+            if v:
+                logger.success(f"已开启 gpt_lgr_markdown 拉格兰MarkDown转换")
+            else:
+                logger.success(f"已关闭 gpt_lgr_markdown 拉格兰MarkDown转换")
+            return v               
+                 
 config_gpt = Config.parse_obj(get_driver().config)
 config_nb = get_driver().config
```

### Comparing `nonebot-plugin-gpt-0.0.8/nonebot_plugin_gpt/source.py` & `nonebot-plugin-gpt-0.0.9/nonebot_plugin_gpt/source.py`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-gpt-0.0.8/pyproject.toml` & `nonebot-plugin-gpt-0.0.9/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 [project]
 name = "nonebot-plugin-gpt"
-version = "0.0.8"
+version = "0.0.9"
 description = "Nonebot2's plugin of ChatGPT "
 authors = [
     { name = "nek0us", email = "nekouss@mail.com" },
 ]
 dependencies = [
-    "ChatGPTWeb>=0.2.13",
+    "ChatGPTWeb>=0.2.14",
     "nonebot_adapter_onebot>=2.3.1",
-    "nonebot-plugin-sendmsg-by-bots>=0.1.1",
+    "nonebot-plugin-sendmsg-by-bots>=0.1.2",
     "nonebot_adapter_qq>=1.3.5",
     "nonebot2>=2.0.0",
     "more_itertools",
     "nonebot_plugin_htmlrender",
     "nonebot_plugin_localstore",
 ]
 requires-python = ">=3.10"
```

### Comparing `nonebot-plugin-gpt-0.0.8/PKG-INFO` & `nonebot-plugin-gpt-0.0.9/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-gpt
-Version: 0.0.8
+Version: 0.0.9
 Summary: Nonebot2's plugin of ChatGPT 
 License: GPL3
 Author-email: nek0us <nekouss@mail.com>
 Requires-Python: >=3.10
 Project-URL: Homepage, https://github.com/nek0us/nonebot-plugin-gpt
 Project-URL: Repository, https://github.com/nek0us/nonebot-plugin-gpt
 Description-Content-Type: text/markdown
@@ -79,14 +79,21 @@
 
 打开 nonebot2 项目根目录下的 `pyproject.toml` 文件, 在 `[tool.nonebot]` 部分追加写入
 
     plugins = ["nonebot_plugin_gpt"]
 
 </details>
 
+<details open>
+<summary>升级插件版本</summary>
+
+    pip install nonebot-plugin-gpt -U
+
+</details>
+
 ## ⚙️ 配置
 
 在 nonebot2 项目的`.env`文件中添加下表中的必填配置
 
 | 配置项 | 必填 | 默认值 | 类型 | 说明 |
 |:-----:|:----:|:----:|:----:|:----:|
 | gpt_session | 是 | 无 | List[Dict[str,str]] | openai账号密码 |
@@ -98,14 +105,15 @@
 | begin_sleep_time | 否 | false | bool | 关闭启动等待时间（建议账号数量大于5开启） |
 | gpt_chat_priority | 否 | 90 | int | gpt聊天响应优先级 |
 | gpt_command_priority | 否 | 19 | int | gpt命令响应优先级 |
 | gpt_white_list_mode | 否 | true | bool | 聊天白名单模式 |
 | gpt_replay_to_replay | 否 | false | bool | 是否响应"回复消息" |
 | gpt_ban_str | 否 | 无 | List[str] | 黑名单屏蔽词列表 |
 | gpt_manage_ids | 否 | 无 | List[str] | 超管群/频道id，通过日志等方式获得 |
+| gpt_lgr_markdown| 否 | false | bool | 以拉格兰md消息回复 |
 
 ```bash
 # gpt配置示例
 # 当mode为空或者为openai时，建议提前手动登录一次获取session_token填入（成功使用后可删除session_token项），mode目前不支持苹果账号
 gpt_session='[
     {
         "email": "xxxx@hotmail.com",
@@ -147,14 +155,16 @@
 
 gpt_ban_str='[
     "我是猪",
     "你是猪",
 ]'
 # qq适配器使用的超管群id
 gpt_manage_ids=['qq group id......']
+# onebot适配器 拉格兰md消息兼容
+gpt_lgr_markdown=false
 
 # 插件需要一些其他的Nonebot基础配置，请检查是否存在
 # 机器人名
 nickname=["bot name"]
 # 超管QQ（onebot用）
 SUPERUSERS=["qq num"]
 
@@ -188,14 +198,19 @@
 <为必填内容>，(为选填内容)
 
 ## 常见问题
 ### 微软辅助邮箱验证
 当触发验证后，会在启动目录生成带有启动账号名称的文件，键入收到的验证码并保存，即可自动验证。留意日志输出提示
 
 ### 更新日志
+2024.03.17
+1. 优化了底层代码，减少错误，暂不支持gpt plus账号（待填坑）
+2. 支持拉格兰md发送
+
+
 2024.03.13
 1. 兼容拉格兰合并转发，修复合并转发失败的问题
 2. 添加自定义聊天前缀，现在可以不用@也能触发了
 
 
 2024.03.11
 1. 临时修复200问题（chatgpt新的websocket问题），最近好忙，等闲了的时候再优化，有什么问题都可以先提issue
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: nonebot-plugin-gpt Version: 0.0.8 Summary:
+Metadata-Version: 2.1 Name: nonebot-plugin-gpt Version: 0.0.9 Summary:
 Nonebot2's plugin of ChatGPT License: GPL3 Author-email: nek0us
 mail.com> Requires-Python: >=3.10 Project-URL: Homepage, https://github.com/
 nek0us/nonebot-plugin-gpt Project-URL: Repository, https://github.com/nek0us/
 nonebot-plugin-gpt Description-Content-Type: text/markdown
                               _[_N_o_n_e_B_o_t_P_l_u_g_i_n_L_o_g_o_]
                               [NoneBotPluginText]
        # nonebot-plugin-gpt _â¨ NoneBot GPT â¨__[_l_i_c_e_n_s_e_]_[_p_y_p_i_][python]
@@ -13,15 +13,16 @@
 é¡¹ç®çæ ¹ç®å½ä¸æå¼å½ä»¤è¡, è¾å¥ä»¥ä¸æä»¤å³å¯å®è£ nb plugin
 install nonebot-plugin-gpt ä½¿ç¨åç®¡çå¨å®è£ å¨ nonebot2
 é¡¹ç®çæä»¶ç®å½ä¸, æå¼å½ä»¤è¡, æ ¹æ®ä½ ä½¿ç¨çåç®¡çå¨,
 è¾å¥ç¸åºçå®è£å½ä»¤ pip pip install nonebot-plugin-gpt pdm pdm add
 nonebot-plugin-gpt poetry poetry add nonebot-plugin-gpt conda conda install
 nonebot-plugin-gpt æå¼ nonebot2 é¡¹ç®æ ¹ç®å½ä¸ç `pyproject.toml`
 æä»¶, å¨ `[tool.nonebot]` é¨åè¿½å åå¥ plugins =
-["nonebot_plugin_gpt"] ## âï¸ éç½® å¨ nonebot2
+["nonebot_plugin_gpt"] åçº§æä»¶çæ¬ pip install nonebot-plugin-gpt -U ##
+âï¸ éç½® å¨ nonebot2
 é¡¹ç®ç`.env`æä»¶ä¸­æ·»å ä¸è¡¨ä¸­çå¿å¡«éç½® | éç½®é¡¹ | å¿å¡« |
 é»è®¤å¼ | ç±»å | è¯´æ | |:-----:|:----:|:----:|:----:|:----:| |
 gpt_session | æ¯ | æ  | List[Dict[str,str]] | openaiè´¦å·å¯ç  | |
 gpt_proxy | å¦ | æ  | str | ä½¿ç¨çä»£ç | | arkose_status | å¦ | false |
 bool | gptæ¯å¦å¼å¯äºarkoseéªè¯ | | group_chat | å¦ | true | bool |
 ç¾¤éå¼å¯å¤äººè¯å« | | gpt_chat_start | å¦ | [] | list |
 èå¤©åç¼ï¼åènbå½ä»¤åç¼ | | gpt_chat_start_in_msg | å¦ | false |
@@ -29,25 +30,27 @@
 | bool | å³é­å¯å¨ç­å¾æ¶é´ï¼å»ºè®®è´¦å·æ°éå¤§äº5å¼å¯ï¼ | |
 gpt_chat_priority | å¦ | 90 | int | gptèå¤©ååºä¼åçº§ | |
 gpt_command_priority | å¦ | 19 | int | gptå½ä»¤ååºä¼åçº§ | |
 gpt_white_list_mode | å¦ | true | bool | èå¤©ç½ååæ¨¡å¼ | |
 gpt_replay_to_replay | å¦ | false | bool | æ¯å¦ååº"åå¤æ¶æ¯" | |
 gpt_ban_str | å¦ | æ  | List[str] | é»ååå±è½è¯åè¡¨ | |
 gpt_manage_ids | å¦ | æ  | List[str] | è¶ç®¡ç¾¤/
-é¢éidï¼éè¿æ¥å¿ç­æ¹å¼è·å¾ | ```bash # gptéç½®ç¤ºä¾ #
+é¢éidï¼éè¿æ¥å¿ç­æ¹å¼è·å¾ | | gpt_lgr_markdown| å¦ | false | bool
+| ä»¥ææ ¼å°mdæ¶æ¯åå¤ | ```bash # gptéç½®ç¤ºä¾ #
 å½modeä¸ºç©ºæèä¸ºopenaiæ¶ï¼å»ºè®®æåæå¨ç»å½ä¸æ¬¡è·åsession_tokenå¡«å¥ï¼æåä½¿ç¨åå¯å é¤session_tokené¡¹ï¼ï¼modeç®åä¸æ¯æè¹æè´¦å·
 gpt_session='[ { "email": "xxxx@hotmail.com", "password": "xxxx",
 "session_token": "ey....", }, { "email": "aaaa@gmail.com", "password": "xxxx",
 "mode": "google", }, { "email": "bbb@sss.com", "password": "xxxx", "mode":
 "microsoft", "help_email": "xxx@xx.com" }, ]' gpt_proxy='http://127.0.0.1:8080'
 arkose_status=false group_chat=true gpt_chat_start=[]
 gpt_chat_start_in_msg=false begin_sleep_time=true gpt_chat_priority=90
 gpt_command_priority=19 gpt_white_list_mode=true gpt_replay_to_replay=false
 gpt_ban_str='[ "ææ¯çª", "ä½ æ¯çª", ]' # qqééå¨ä½¿ç¨çè¶ç®¡ç¾¤id
-gpt_manage_ids=['qq group id......'] #
+gpt_manage_ids=['qq group id......'] # onebotééå¨ ææ ¼å°mdæ¶æ¯å¼å®¹
+gpt_lgr_markdown=false #
 æä»¶éè¦ä¸äºå¶ä»çNonebotåºç¡éç½®ï¼è¯·æ£æ¥æ¯å¦å­å¨ #
 æºå¨äººå nickname=["bot name"] # è¶ç®¡QQï¼onebotç¨ï¼ SUPERUSERS=["qq
 num"] ``` ## ð ä½¿ç¨ ### æä»¤è¡¨ | æä»¤ | ééå¨ | æé | éè¦@
 | èå´ | è¯´æ | |:-----:|:----:|:----:|:----:|:----:|:----:| | @bot
 èå¤©åå®¹... | å¼å®¹ | æ /ç½åå | æ¯ | ç¾¤è/ç§è/é¢é |
 @æèå«å+åå®¹ å¼å§èå¤©ï¼éææèç½ååæ¨¡å¼è®¾ç½®æ¹å | |
 åå§å | å¼å®¹ | æ /ç½åå | æ¯ | ç¾¤è/ç§è/é¢é | åå§å
@@ -81,13 +84,15 @@
 è¶ç®¡ç¾¤ | æ¯ | ç¾¤è/é¢é | çæcdk
 ¤å·/å¶ä»ä¿¡æ¯>ï¼ä»¥ç»å®ä¿¡æ¯æ¹å¼çæç½ååcdk | | åºç°å§ | qq
 | æ  | æ¯ | ç¾¤è/é¢é | åºç°å§ \
 >ï¼ä»¥ç»å®idå½¢å¼ä½¿ç¨cdkå å¥ç½åå | | ç»æå§ | qq | ç½åå |
 æ¯ | ç¾¤è/é¢é | ç»æå§ ï¼ç¨æ·èªä¸»è§£é¤ç½åå |
 ºå¿å¡«åå®¹>ï¼(ä¸ºéå¡«åå®¹) ## å¸¸è§é®é¢ ### å¾®è½¯è¾å©é®ç®±éªè¯
 å½è§¦åéªè¯åï¼ä¼å¨å¯å¨ç®å½çæå¸¦æå¯å¨è´¦å·åç§°çæä»¶ï¼é®å¥æ¶å°çéªè¯ç å¹¶ä¿å­ï¼å³å¯èªå¨éªè¯ãçææ¥å¿è¾åºæç¤º
-### æ´æ°æ¥å¿ 2024.03.13 1.
+### æ´æ°æ¥å¿ 2024.03.17 1.
+ä¼åäºåºå±ä»£ç ï¼åå°éè¯¯ï¼æä¸æ¯ægpt
+plusè´¦å·ï¼å¾å¡«åï¼ 2. æ¯æææ ¼å°mdåé 2024.03.13 1.
 å¼å®¹ææ ¼å°åå¹¶è½¬åï¼ä¿®å¤åå¹¶è½¬åå¤±è´¥çé®é¢ 2.
 æ·»å èªå®ä¹èå¤©åç¼ï¼ç°å¨å¯ä»¥ä¸ç¨@ä¹è½è§¦åäº 2024.03.11 1.
 ä¸´æ¶ä¿®å¤200é®é¢ï¼chatgptæ°çwebsocketé®é¢ï¼ï¼æè¿å¥½å¿ï¼ç­é²äºçæ¶ååä¼åï¼æä»ä¹é®é¢é½å¯ä»¥åæissue
 2024.02.19 1. ä¸´æ¶ä¿®å¤200é®é¢ ä¸ æ·»å  å¾®è½¯è¾å©é®ç®±éªè¯ ##
 å¾ç»­ èªç¨æºä¹äºï¼åå¿æ¹æ¹ååºæ¥ï¼å¾å¤ä¸è¥¿è¿æ²¡è¡¥å
```

