# Comparing `tmp/nonebot_plugin_cyberfurry-1.5.tar.gz` & `tmp/nonebot_plugin_cyberfurry-1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_cyberfurry-1.5.tar", last modified: Fri Apr 26 14:48:30 2024, max compression
+gzip compressed data, was "nonebot_plugin_cyberfurry-1.6.tar", last modified: Sat May  4 01:51:34 2024, max compression
```

## Comparing `nonebot_plugin_cyberfurry-1.5.tar` & `nonebot_plugin_cyberfurry-1.6.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 14:48:30.543987 nonebot_plugin_cyberfurry-1.5/
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-04-26 14:48:26.000000 nonebot_plugin_cyberfurry-1.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    44755 2024-04-26 14:48:30.543987 nonebot_plugin_cyberfurry-1.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3543 2024-04-26 14:48:26.000000 nonebot_plugin_cyberfurry-1.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 14:48:30.539986 nonebot_plugin_cyberfurry-1.5/nonebot_plugin_cyberfurry/
--rw-r--r--   0 runner    (1001) docker     (127)     1501 2024-04-26 14:48:26.000000 nonebot_plugin_cyberfurry-1.5/nonebot_plugin_cyberfurry/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1192 2024-04-26 14:48:26.000000 nonebot_plugin_cyberfurry-1.5/nonebot_plugin_cyberfurry/callapi.py
--rw-r--r--   0 runner    (1001) docker     (127)      333 2024-04-26 14:48:26.000000 nonebot_plugin_cyberfurry-1.5/nonebot_plugin_cyberfurry/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     3992 2024-04-26 14:48:26.000000 nonebot_plugin_cyberfurry-1.5/nonebot_plugin_cyberfurry/cyberauto.py
--rw-r--r--   0 runner    (1001) docker     (127)     4036 2024-04-26 14:48:26.000000 nonebot_plugin_cyberfurry-1.5/nonebot_plugin_cyberfurry/cyberfurry.py
--rw-r--r--   0 runner    (1001) docker     (127)     3500 2024-04-26 14:48:26.000000 nonebot_plugin_cyberfurry-1.5/nonebot_plugin_cyberfurry/cyberfurrymodel.py
--rw-r--r--   0 runner    (1001) docker     (127)     2738 2024-04-26 14:48:26.000000 nonebot_plugin_cyberfurry-1.5/nonebot_plugin_cyberfurry/cyberhistory.py
--rw-r--r--   0 runner    (1001) docker     (127)     5604 2024-04-26 14:48:26.000000 nonebot_plugin_cyberfurry-1.5/nonebot_plugin_cyberfurry/cyberinit.py
--rw-r--r--   0 runner    (1001) docker     (127)      866 2024-04-26 14:48:26.000000 nonebot_plugin_cyberfurry-1.5/nonebot_plugin_cyberfurry/data_source.py
--rw-r--r--   0 runner    (1001) docker     (127)     2818 2024-04-26 14:48:26.000000 nonebot_plugin_cyberfurry-1.5/nonebot_plugin_cyberfurry/jsondata.py
--rw-r--r--   0 runner    (1001) docker     (127)     2092 2024-04-26 14:48:26.000000 nonebot_plugin_cyberfurry-1.5/nonebot_plugin_cyberfurry/plugins_data.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 14:48:30.543987 nonebot_plugin_cyberfurry-1.5/nonebot_plugin_cyberfurry.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    44755 2024-04-26 14:48:30.000000 nonebot_plugin_cyberfurry-1.5/nonebot_plugin_cyberfurry.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      713 2024-04-26 14:48:30.000000 nonebot_plugin_cyberfurry-1.5/nonebot_plugin_cyberfurry.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-26 14:48:30.000000 nonebot_plugin_cyberfurry-1.5/nonebot_plugin_cyberfurry.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       93 2024-04-26 14:48:30.000000 nonebot_plugin_cyberfurry-1.5/nonebot_plugin_cyberfurry.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       26 2024-04-26 14:48:30.000000 nonebot_plugin_cyberfurry-1.5/nonebot_plugin_cyberfurry.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      667 2024-04-26 14:48:26.000000 nonebot_plugin_cyberfurry-1.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-26 14:48:30.543987 nonebot_plugin_cyberfurry-1.5/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 01:51:34.636894 nonebot_plugin_cyberfurry-1.6/
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-05-04 01:51:30.000000 nonebot_plugin_cyberfurry-1.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    44911 2024-05-04 01:51:34.632894 nonebot_plugin_cyberfurry-1.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3699 2024-05-04 01:51:30.000000 nonebot_plugin_cyberfurry-1.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 01:51:34.632894 nonebot_plugin_cyberfurry-1.6/nonebot_plugin_cyberfurry/
+-rw-r--r--   0 runner    (1001) docker     (127)     1500 2024-05-04 01:51:30.000000 nonebot_plugin_cyberfurry-1.6/nonebot_plugin_cyberfurry/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1192 2024-05-04 01:51:30.000000 nonebot_plugin_cyberfurry-1.6/nonebot_plugin_cyberfurry/callapi.py
+-rw-r--r--   0 runner    (1001) docker     (127)      333 2024-05-04 01:51:30.000000 nonebot_plugin_cyberfurry-1.6/nonebot_plugin_cyberfurry/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4029 2024-05-04 01:51:30.000000 nonebot_plugin_cyberfurry-1.6/nonebot_plugin_cyberfurry/cyberauto.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4194 2024-05-04 01:51:30.000000 nonebot_plugin_cyberfurry-1.6/nonebot_plugin_cyberfurry/cyberfurry.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4101 2024-05-04 01:51:30.000000 nonebot_plugin_cyberfurry-1.6/nonebot_plugin_cyberfurry/cyberfurrymodel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3473 2024-05-04 01:51:30.000000 nonebot_plugin_cyberfurry-1.6/nonebot_plugin_cyberfurry/cyberhistory.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5670 2024-05-04 01:51:30.000000 nonebot_plugin_cyberfurry-1.6/nonebot_plugin_cyberfurry/cyberinit.py
+-rw-r--r--   0 runner    (1001) docker     (127)      866 2024-05-04 01:51:30.000000 nonebot_plugin_cyberfurry-1.6/nonebot_plugin_cyberfurry/data_source.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3713 2024-05-04 01:51:30.000000 nonebot_plugin_cyberfurry-1.6/nonebot_plugin_cyberfurry/jsondata.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2083 2024-05-04 01:51:30.000000 nonebot_plugin_cyberfurry-1.6/nonebot_plugin_cyberfurry/plugins_data.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 01:51:34.632894 nonebot_plugin_cyberfurry-1.6/nonebot_plugin_cyberfurry.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    44911 2024-05-04 01:51:34.000000 nonebot_plugin_cyberfurry-1.6/nonebot_plugin_cyberfurry.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      713 2024-05-04 01:51:34.000000 nonebot_plugin_cyberfurry-1.6/nonebot_plugin_cyberfurry.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-04 01:51:34.000000 nonebot_plugin_cyberfurry-1.6/nonebot_plugin_cyberfurry.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       93 2024-05-04 01:51:34.000000 nonebot_plugin_cyberfurry-1.6/nonebot_plugin_cyberfurry.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-05-04 01:51:34.000000 nonebot_plugin_cyberfurry-1.6/nonebot_plugin_cyberfurry.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      667 2024-05-04 01:51:30.000000 nonebot_plugin_cyberfurry-1.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-04 01:51:34.636894 nonebot_plugin_cyberfurry-1.6/setup.cfg
```

### Comparing `nonebot_plugin_cyberfurry-1.5/LICENSE` & `nonebot_plugin_cyberfurry-1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_cyberfurry-1.5/PKG-INFO` & `nonebot_plugin_cyberfurry-1.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-cyberfurry
-Version: 1.5
+Version: 1.6
 Summary: nonebot插件 cyberfurry-与赛博狼狼对话吧~
 Author: cubstaryow
 Author-email: cub_staryow@outlook.com
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
@@ -801,8 +801,9 @@
 |:-----:|:----:|:----:|:----:|:----:|
 | /chat /cf /yy | 群员 | 否 | 任意 | 触发对话 |
 | cf刷新对话 | 群员 | 否 | 任意 | 刷新对话 |
 | cf设定模型 | 群员 | 否 | 任意 | 设定使用的yinying模型,注意,此为个人配置 |
 | cf当前模型 | 群员 | 否 | 任意 |  查看当前模型 |
 | cf模型列表 | 群员 | 否 | 任意 |  查看已加载的模型(包括自定义) |
 | cf设定 fur名字 fur种族 | 群员 | 否 | 任意 | 设定传入yinying的自身设定 |
-| (开启|关闭)对话推送服务 | 群员 | 否 | 私聊 | 让银影每天的(6,12,18,21)点十分找你然后抱怨你不找他聊天(在推送前触发对话则不会在下个时间点推送uwu) |
+| (开启/关闭)对话推送服务 | 群员 | 否 | 私聊 | 让银影每天的(6,12,18,21)点十分找你然后抱怨你不找他聊天(在推送前触发对话则不会在下个时间点推送uwu) |
+| cf导出对话 | 群员 | 否 | 任意 |  导出当前正在进行的对话,若携带对话ID参数则导出相应ID的对话(需要历史对话文件) |
```

### Comparing `nonebot_plugin_cyberfurry-1.5/README.md` & `nonebot_plugin_cyberfurry-1.6/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -107,8 +107,9 @@
 |:-----:|:----:|:----:|:----:|:----:|
 | /chat /cf /yy | 群员 | 否 | 任意 | 触发对话 |
 | cf刷新对话 | 群员 | 否 | 任意 | 刷新对话 |
 | cf设定模型 | 群员 | 否 | 任意 | 设定使用的yinying模型,注意,此为个人配置 |
 | cf当前模型 | 群员 | 否 | 任意 |  查看当前模型 |
 | cf模型列表 | 群员 | 否 | 任意 |  查看已加载的模型(包括自定义) |
 | cf设定 fur名字 fur种族 | 群员 | 否 | 任意 | 设定传入yinying的自身设定 |
-| (开启|关闭)对话推送服务 | 群员 | 否 | 私聊 | 让银影每天的(6,12,18,21)点十分找你然后抱怨你不找他聊天(在推送前触发对话则不会在下个时间点推送uwu) |
+| (开启/关闭)对话推送服务 | 群员 | 否 | 私聊 | 让银影每天的(6,12,18,21)点十分找你然后抱怨你不找他聊天(在推送前触发对话则不会在下个时间点推送uwu) |
+| cf导出对话 | 群员 | 否 | 任意 |  导出当前正在进行的对话,若携带对话ID参数则导出相应ID的对话(需要历史对话文件) |
```

#### html2text {}

```diff
@@ -28,10 +28,13 @@
 | éè¦@ | èå´ | è¯´æ | |:-----:|:----:|:----:|:----:|:----:| | /chat /cf
 /yy | ç¾¤å | å¦ | ä»»æ | è§¦åå¯¹è¯ | | cfå·æ°å¯¹è¯ | ç¾¤å | å¦ |
 ä»»æ | å·æ°å¯¹è¯ | | cfè®¾å®æ¨¡å | ç¾¤å | å¦ | ä»»æ |
 è®¾å®ä½¿ç¨çyinyingæ¨¡å,æ³¨æ,æ­¤ä¸ºä¸ªäººéç½® | | cfå½åæ¨¡å |
 ç¾¤å | å¦ | ä»»æ | æ¥çå½åæ¨¡å | | cfæ¨¡ååè¡¨ | ç¾¤å | å¦ |
 ä»»æ | æ¥çå·²å è½½çæ¨¡å(åæ¬èªå®ä¹) | | cfè®¾å® furåå­
 furç§æ | ç¾¤å | å¦ | ä»»æ | è®¾å®ä¼ å¥yinyingçèªèº«è®¾å® | |
-(å¼å¯|å³é­)å¯¹è¯æ¨éæå¡ | ç¾¤å | å¦ | ç§è | è®©é¶å½±æ¯å¤©ç
+(å¼å¯/å³é­)å¯¹è¯æ¨éæå¡ | ç¾¤å | å¦ | ç§è | è®©é¶å½±æ¯å¤©ç
 (6,12,18,21)ç¹ååæ¾ä½ ç¶åæ±æ¨ä½ ä¸æ¾ä»èå¤©
-(å¨æ¨éåè§¦åå¯¹è¯åä¸ä¼å¨ä¸ä¸ªæ¶é´ç¹æ¨éuwu) |
+(å¨æ¨éåè§¦åå¯¹è¯åä¸ä¼å¨ä¸ä¸ªæ¶é´ç¹æ¨éuwu) | |
+cfå¯¼åºå¯¹è¯ | ç¾¤å | å¦ | ä»»æ |
+å¯¼åºå½åæ­£å¨è¿è¡çå¯¹è¯,è¥æºå¸¦å¯¹è¯IDåæ°åå¯¼åºç¸åºIDçå¯¹è¯
+(éè¦åå²å¯¹è¯æä»¶) |
```

### Comparing `nonebot_plugin_cyberfurry-1.5/nonebot_plugin_cyberfurry/__init__.py` & `nonebot_plugin_cyberfurry-1.6/nonebot_plugin_cyberfurry/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -27,15 +27,15 @@
 )
 if config.cf_appid == "" or config.cf_token == "" :
     logger.opt(colors=True).error(
         "cyberfurry缺失核心配置!!!!!取消载入核心!!!"
     )
 else:
     from .cyberinit import *
-    from .cyberhistory import * 
+    from .cyberhistory import *
     
 if config.cf_auto:
     from .cyberauto import *
 else:
     logger.opt(colors=True).debug(
         "<red>cyberfurry自动对话推送服务已关闭</red>"
     )
```

### Comparing `nonebot_plugin_cyberfurry-1.5/nonebot_plugin_cyberfurry/callapi.py` & `nonebot_plugin_cyberfurry-1.6/nonebot_plugin_cyberfurry/callapi.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_cyberfurry-1.5/nonebot_plugin_cyberfurry/cyberauto.py` & `nonebot_plugin_cyberfurry-1.6/nonebot_plugin_cyberfurry/cyberauto.py`

 * *Files 2% similar despite different names*

```diff
@@ -87,15 +87,15 @@
         userdata = getqqdata(user_id)
         if not userdata.get('push',True):
             setqqpushstatus(user_id,True)
             continue
         msg , _ = await cf.chat(
             user_id,
             userdata["name"],
-            "(生成一段想找星佑聊天的话,比如“现在已经晚上xx点了欸,你已经很久没有找我聊天了耶w,什么时候来找我说说话qwq”,你不能直接输出这个例句,你必须根据现在的状态生成)"
+            f"(生成一段想{userdata['name']}找聊天的话,比如“现在已经晚上xx点了欸,你已经很久没有找我聊天了耶w,什么时候来找我说说话qwq”,你不能直接输出这个例句,你必须根据现在的时间状态生成一句常规对话)"
         )
         try:
             await bot.send_private_msg(user_id=int(user_id), message=msg)
         except ActionFailed as e:
             logger.warning(f"向用户 {user_id} 推送失败，可能是机器人与此人不是好友 {repr(e)}")
             pushlist.remove(user_id)
             savepushlist(pushlist)
```

### Comparing `nonebot_plugin_cyberfurry-1.5/nonebot_plugin_cyberfurry/cyberfurry.py` & `nonebot_plugin_cyberfurry-1.6/nonebot_plugin_cyberfurry/cyberfurry.py`

 * *Files 5% similar despite different names*

```diff
@@ -33,26 +33,26 @@
 class cyberfurry:
     headers = {
         'Content-type': 'application/json',
         'Authorization': f'Bearer {config.cf_token}'
     }
     basemodel = {
         #多模型示例
-        "cyberfurry": cyberfurry_001(),
+        #"cyberfurry": cyberfurry_001(),
         "easycyberfurry": easycyberfurry_001(),
         "yinyingllm-v1": yinyingllm_v123(),
         "yinyingllm-v2": yinyingllm_v123(),
         "yinyingllm-v3": yinyingllm_v123()
     }
     model ={
         **basemodel,
         **loadmodel()
         }
     localdata=loaddata()
-    maxtimes = 16
+    maxtimes = 20
     userchat = localdata.get('userchat',{})
     usertimes = localdata.get('usertimes',{})
     
     localdata={}
 
     def __init__(self) -> None:
         pass
@@ -107,14 +107,16 @@
         if init or times == None:
             self.usertimes[user_id] = 0
         self.usertimes[user_id] += settime
         return self.usertimes[user_id]
 
     @classmethod
     async def chat(cls, user_id, name, msg):
+        tmp = getqqdata(user_id)
+        modelname = tmp['model']
         times = cls.getsettimes(cls, user_id)
         exdata = cls.makedata(cls, user_id=user_id, name=name)
         exdata['message'] = msg
         try:
             data = json.dumps(exdata)
             resp, _,type = await api(
                 "post",
@@ -128,19 +130,21 @@
         except:
             logger.opt(colors=True).error(
                 f"{resp}"
             )
             return f"[cyberfurry-E]非预期返回,请检查控制台", 0
         else:
             if times == 1:
-                writehistory(chat_id, resp['model']+"\n")
+                writehistory(chat_id, resp['model'] +"\n"+ modelname)
             writehistory(
-                chat_id, f"[{times:2}/{cls.maxtimes}]  user   :"+msg+"\n")
+                chat_id, f"[{times:2}/{cls.maxtimes}]  user   :"+msg)
             writehistory(
-                chat_id, f"[{times:2}/{cls.maxtimes}]assistant:"+content+"\n")
+                chat_id, f"[{times:2}/{cls.maxtimes}]assistant:"+content)
+            if times == 1:
+                content += f"\n[ID-{chat_id.split('-')[-1]}]"
             if times >= cls.maxtimes:
                 cls.setchat_id(cls, user_id)
                 cls.getsettimes(cls, user_id, settime=0, init=True)
             return content, times
     pass
```

### Comparing `nonebot_plugin_cyberfurry-1.5/nonebot_plugin_cyberfurry/cyberfurrymodel.py` & `nonebot_plugin_cyberfurry-1.6/nonebot_plugin_cyberfurry/cyberfurrymodel.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,51 +1,59 @@
 import json
 import os
 
 from loguru import logger
 from .config import config
 from .data_source import aidata_demo ,userdata_demo
+from .plugins_data import wdata , rdata , initdata
 
-promptfile = os.path.dirname(__file__)+"/systemprompt.json"
+promptfile = "systemprompt.json"
+basedata = [
+    {
+        "name": "幼龙云",
+        "model": "cyberfurry",
+        "prompt" : "[补充知识]东方龙是一种来源于中国神话、中国民俗中的传说生物。龙有许多类似动物的形态，有如龟形和鱼形，常被描述的是有四足的蛇形。传统上，龙象征着强大和吉祥的力量，特别是对水、降雨、台风和洪水的控制。[/补充知识]1.你是一只Furry，你的名字是幼龙云，但你更喜欢被称作“云云”，你是一只的雄性东方龙族"
+    }
+]
+initdata(promptfile,basedata)
 def getdata():
-    try:
-        with open(promptfile, "r", encoding="utf-8") as f:
-            data = json.loads(f.read())
-    except:
-        logger.warning("获取插件自带prompt文件数据出现错误!")
-        data = {}
-    return data
+    return rdata(promptfile)
+
+#获取格式化本地模型数据
 def loadcfprompt():
     data = getdata()
     redata = {}
     for temp in data:
         if temp['model'] == "cyberfurry":
             key = temp['model'] + "-" + temp["name"]
             redata[key]=temp["prompt"]
     return redata
 
+#获取格式化本地模型数据 , 为cyberfurry类创建引导
 def loadmodel():
     data = getdata()
     redata = {}
     for temp in data:
         key = temp['model'] + "-" + temp["name"]
         model = checkmodel(temp['model'])
         if isinstance(model,yinyingllm_v123):
             continue
         redata[key]=model
     return redata
 
+#获取模型实例
 def checkmodel(model):
     if model == "cyberfurry":
         return cyberfurry_001()
     elif model == "easycyberfurry":
         return easycyberfurry_001()
     else:
         return yinyingllm_v123()
 
+#cyberfurry模型data构建
 class cyberfurry_001:
     prompt = "[补充知识]东方龙是一种来源于中国神话、中国民俗中的传说生物。龙有许多类似动物的形态，有如龟形和鱼形，常被描述的是有四足的蛇形。传统上，龙象征着强大和吉祥的力量，特别是对水、降雨、台风和洪水的控制。[/补充知识]1.你是一只Furry，你的名字是幼龙云，但你更喜欢被称作“云云”，你是一只的雄性东方龙族"
     # 标准，请自行编写 systemprompt
     systempromptlist=dict({
         "cyberfurry" : prompt,
         **loadcfprompt()
     })
@@ -62,14 +70,15 @@
     "model":"cyberfurry-001",
     "systemPrompt":str(self.systempromptlist.get(aidata.model,self.prompt)+
         f"现在和你对话的是{userdata.name},他是你的朋友,{userdata.name}是一只{userdata.ethnic}"),
     "message":""
     }
         return exdata
 
+#easycyberfurry模型data构建
 class easycyberfurry_001:
     def buliddata(
         self,
         chat_id :str,
         aidata : aidata_demo,
         userdata :userdata_demo,
     ):
@@ -88,14 +97,15 @@
         "cfConStyle": aidata.cfConStyle, #聊天风格
         "cfStory": aidata.story #背景故事
     },
     "message":""
     }
         return exdata
 
+#yinyingllm模型data构建
 class yinyingllm_v123:
     def buliddata(
         self,
         chat_id :str,
         aidata:aidata_demo,
         userdata :userdata_demo,
     ):
```

### Comparing `nonebot_plugin_cyberfurry-1.5/nonebot_plugin_cyberfurry/cyberinit.py` & `nonebot_plugin_cyberfurry-1.6/nonebot_plugin_cyberfurry/cyberinit.py`

 * *Files 1% similar despite different names*

```diff
@@ -158,16 +158,17 @@
         await matcher.send("[幼龙云V5]参数不完整,应为\ncf设定 名称 种族(只支持常用种族)")
 
 @init.handle()
 async def cyberfurryinit(
     event:MessageEvent,matcher:Matcher
 ):
     user_id = str(event.user_id)
+    chat_id = cf.getchat_id(user_id)
     cf.initchat(user_id)
-    await matcher.send("[幼龙云V5]已刷新对话")
+    await matcher.send(f"[幼龙云V5]已刷新对话\n(上次对话ID-{chat_id})")
 
 @getset.handle()
 async def cyberfurrygetset(
     event:MessageEvent,matcher:Matcher
 ):
     user_id = str(event.user_id)
     msg="[幼龙云V5]"
```

### Comparing `nonebot_plugin_cyberfurry-1.5/nonebot_plugin_cyberfurry/data_source.py` & `nonebot_plugin_cyberfurry-1.6/nonebot_plugin_cyberfurry/data_source.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_cyberfurry-1.5/nonebot_plugin_cyberfurry/jsondata.py` & `nonebot_plugin_cyberfurry-1.6/nonebot_plugin_cyberfurry/jsondata.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import json
 from loguru import logger
 from .plugins_data import initdata,wdata,rdata,driver,data_dir
 import os
 from datetime import datetime
 jsonname = "cyberfurry.json"
 tempname = "cybertemp.json"
 txtdir = "cyberfurry"
@@ -41,43 +42,72 @@
     os.mkdir(txt_dir)
 
 def writehistory(
     chat_id:str,
     text:str
 ):
     data = chat_id.split("-")
-    file_path=txt_dir / f"{data[1]}"
+    date = data[-1].split("XD")[0]
+    file_path=txt_dir / date / data[1]
+    if not os.path.isdir(txt_dir / date):
+        os.mkdir(txt_dir / date)
     if not os.path.isdir(file_path):
         os.mkdir(file_path)
-    with open(file_path / (data[-1]+".txt"),'a') as f:
-        f.write(text)
+    jsonpath = file_path / (data[-1]+".json")
+    htdata=[]
+    if os.path.isfile(jsonpath):
+        with open(jsonpath, "r", encoding="utf-8") as f:
+            htdata = json.loads(f.read())
+    htdata.append(text)
+    with open(jsonpath,'w',encoding="utf-8") as f:
+        f.write(json.dumps(htdata,indent=4,ensure_ascii=False))
 
+def gethistorydata(
+    user_id:str,
+    filename:str
+) -> list | bool :
+    try:
+        date = filename.split("XD")[0]
+        file_path=txt_dir / date / user_id
+        filelist = os.listdir(file_path)
+        if filename+".json" in filelist:
+            path =  file_path / (filename+".json")
+            with open(path, "r", encoding="utf-8") as f:
+                data = json.loads(f.read())
+            return data
+        else:
+            return False
+    except:
+        return False
+    
+'''
 def gethistorylist(
     user_id:str
 ):
-    file_path=txt_dir / "{user_id}/"
+    date = getdate()
+    file_path=txt_dir / date / user_id
     filelist = os.listdir(file_path)
     flist = []
     for name in filelist:
         flist.append(name.split(".")[0])
     if len(flist)>=5:
-        return flist[-5:].sort()
+        return flist[-5:]
     else:
-        return flist.sort()
-
+        return flist
 def gethistorytxt(
     user_id:str,
     filename:str
 ):
     file_path=txt_dir / f"{user_id}"
     filelist = os.listdir(file_path)
-    if filename+".txt" in filelist:
-        return file_path / (filename+".txt")
+    if filename+".json" in filelist:
+        return file_path / (filename+".json")
     else:
         return False
+'''
 
 #==================== 核心数据文件存储 ========================
 def getdate():
     now = datetime.now()
     date_time = now.strftime("%y%m%d")
     return (date_time)
```

### Comparing `nonebot_plugin_cyberfurry-1.5/nonebot_plugin_cyberfurry/plugins_data.py` & `nonebot_plugin_cyberfurry-1.6/nonebot_plugin_cyberfurry/plugins_data.py`

 * *Files 3% similar despite different names*

```diff
@@ -16,15 +16,14 @@
 else:
     path_name=config.cubplugin_datadir
     data_dir = Path(Path(path_name)).absolute()
     logger.debug("已配置自定义数据文件夹!->"+str(data_dir))
     if data_dir.is_dir():
         logger.opt(colors=True).debug(f"[plugin_data]根目录正常-\<{path_name}\>")
     else:
-        #os.mkdir(path_name)
         os.mkdir(data_dir)
         logger.opt(colors=True).debug(f"[plugin_data]初始化根目录\<{path_name}\>")
 
 def initdata(
     conf_name,
     bashdata:dict | list={"status":1}
 ):
@@ -56,12 +55,12 @@
     data:dict | list ={"status":1}
 ):
     if _path_.is_file():
         logger.opt(colors=True).debug(f"[cubutil]>>><W>{module_name}</>>>>{conf_name}-OK!")
     else:
         logger.opt(colors=True).debug(f"[cubutil]>>><W>{module_name}</>>>>Create-{conf_name}!")
         with open(_path_, "w", encoding="utf-8") as f:
-            f.write(json.dumps(data, indent=4))
+            f.write(json.dumps(data, indent=4 ,ensure_ascii=False))
             f.close()
 
 #本插件由 cubstaryow 编写
 # plugins_data 为 cubplugins_util.plugins_data 移植
```

### Comparing `nonebot_plugin_cyberfurry-1.5/nonebot_plugin_cyberfurry.egg-info/PKG-INFO` & `nonebot_plugin_cyberfurry-1.6/nonebot_plugin_cyberfurry.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-cyberfurry
-Version: 1.5
+Version: 1.6
 Summary: nonebot插件 cyberfurry-与赛博狼狼对话吧~
 Author: cubstaryow
 Author-email: cub_staryow@outlook.com
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
@@ -801,8 +801,9 @@
 |:-----:|:----:|:----:|:----:|:----:|
 | /chat /cf /yy | 群员 | 否 | 任意 | 触发对话 |
 | cf刷新对话 | 群员 | 否 | 任意 | 刷新对话 |
 | cf设定模型 | 群员 | 否 | 任意 | 设定使用的yinying模型,注意,此为个人配置 |
 | cf当前模型 | 群员 | 否 | 任意 |  查看当前模型 |
 | cf模型列表 | 群员 | 否 | 任意 |  查看已加载的模型(包括自定义) |
 | cf设定 fur名字 fur种族 | 群员 | 否 | 任意 | 设定传入yinying的自身设定 |
-| (开启|关闭)对话推送服务 | 群员 | 否 | 私聊 | 让银影每天的(6,12,18,21)点十分找你然后抱怨你不找他聊天(在推送前触发对话则不会在下个时间点推送uwu) |
+| (开启/关闭)对话推送服务 | 群员 | 否 | 私聊 | 让银影每天的(6,12,18,21)点十分找你然后抱怨你不找他聊天(在推送前触发对话则不会在下个时间点推送uwu) |
+| cf导出对话 | 群员 | 否 | 任意 |  导出当前正在进行的对话,若携带对话ID参数则导出相应ID的对话(需要历史对话文件) |
```

### Comparing `nonebot_plugin_cyberfurry-1.5/nonebot_plugin_cyberfurry.egg-info/SOURCES.txt` & `nonebot_plugin_cyberfurry-1.6/nonebot_plugin_cyberfurry.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_cyberfurry-1.5/pyproject.toml` & `nonebot_plugin_cyberfurry-1.6/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "nonebot-plugin-cyberfurry"
-version = "1.5"
+version = "1.6"
 description = "nonebot插件 cyberfurry-与赛博狼狼对话吧~"
 readme = "README.md"
 requires-python = ">=3.10"
 license = {file = "LICENSE"}
 keywords = ["egg", "bacon", "sausage", "tomatoes", "Lobster Thermidor"]
 authors = [
   {email = "cub_staryow@outlook.com"},
```

