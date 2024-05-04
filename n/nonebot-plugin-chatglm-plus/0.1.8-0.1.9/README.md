# Comparing `tmp/nonebot_plugin_chatglm_plus-0.1.8-py3-none-any.whl.zip` & `tmp/nonebot_plugin_chatglm_plus-0.1.9-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,8 @@
-Zip file size: 5954 bytes, number of entries: 6
--rwxrwxrwx  2.0 unx    12645 b- defN 24-Mar-22 05:31 nonebot_plugin_chatglm_plus/__init__.py
--rwxrwxrwx  2.0 unx     1365 b- defN 24-Mar-22 05:31 nonebot_plugin_chatglm_plus/config.py
--rwxrwxrwx  2.0 unx      501 b- defN 24-Mar-22 05:31 nonebot_plugin_chatglm_plus-0.1.8.dist-info/METADATA
--rwxrwxrwx  2.0 unx       92 b- defN 24-Mar-22 05:31 nonebot_plugin_chatglm_plus-0.1.8.dist-info/WHEEL
--rwxrwxrwx  2.0 unx       28 b- defN 24-Mar-22 05:31 nonebot_plugin_chatglm_plus-0.1.8.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      568 b- defN 24-Mar-22 05:31 nonebot_plugin_chatglm_plus-0.1.8.dist-info/RECORD
-6 files, 15199 bytes uncompressed, 4908 bytes compressed:  67.7%
+Zip file size: 5970 bytes, number of entries: 6
+-rwxrwxrwx  2.0 unx    12859 b- defN 24-May-04 03:10 nonebot_plugin_chatglm_plus/__init__.py
+-rwxrwxrwx  2.0 unx     1365 b- defN 24-May-04 03:10 nonebot_plugin_chatglm_plus/config.py
+-rwxrwxrwx  2.0 unx      501 b- defN 24-May-04 03:12 nonebot_plugin_chatglm_plus-0.1.9.dist-info/METADATA
+-rwxrwxrwx  2.0 unx       92 b- defN 24-May-04 03:12 nonebot_plugin_chatglm_plus-0.1.9.dist-info/WHEEL
+-rwxrwxrwx  2.0 unx       28 b- defN 24-May-04 03:12 nonebot_plugin_chatglm_plus-0.1.9.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      568 b- defN 24-May-04 03:12 nonebot_plugin_chatglm_plus-0.1.9.dist-info/RECORD
+6 files, 15413 bytes uncompressed, 4924 bytes compressed:  68.1%
```

## zipnote {}

```diff
@@ -1,19 +1,19 @@
 Filename: nonebot_plugin_chatglm_plus/__init__.py
 Comment: 
 
 Filename: nonebot_plugin_chatglm_plus/config.py
 Comment: 
 
-Filename: nonebot_plugin_chatglm_plus-0.1.8.dist-info/METADATA
+Filename: nonebot_plugin_chatglm_plus-0.1.9.dist-info/METADATA
 Comment: 
 
-Filename: nonebot_plugin_chatglm_plus-0.1.8.dist-info/WHEEL
+Filename: nonebot_plugin_chatglm_plus-0.1.9.dist-info/WHEEL
 Comment: 
 
-Filename: nonebot_plugin_chatglm_plus-0.1.8.dist-info/top_level.txt
+Filename: nonebot_plugin_chatglm_plus-0.1.9.dist-info/top_level.txt
 Comment: 
 
-Filename: nonebot_plugin_chatglm_plus-0.1.8.dist-info/RECORD
+Filename: nonebot_plugin_chatglm_plus-0.1.9.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## nonebot_plugin_chatglm_plus/__init__.py

```diff
@@ -71,16 +71,20 @@
             file.write(',\n{"role": "user", "content": "' + text + '"}')
     else:
         with open(f'{log_dir}/{id}.json', 'w') as file:
             file.write('{"role": "user", "content": "' + text + '"}')
 
 #AI输出
 def ai_out(id, text):
-    with open(f'{log_dir}/{id}.json', 'a') as file:
-        file.write(',\n{"role": "assistant", "content": "' + text + '"}')
+    if os.path.exists(f"{log_dir}/{id}.json"):
+        with open(f'{log_dir}/{id}.json', 'a') as file:
+            file.write(',\n{"role": "assistant", "content": "' + text + '"}')
+    else:
+        with open(f'{log_dir}/{id}.json', 'w') as file:
+            file.write('{"role": "assistant", "content": "' + text + '"}')
 
 
 #用户识别图片（仅GLM-4V可用）
 def user_img(id,url,text):
     if os.path.exists(f"{log_dir}/{id}.json"):
         with open(f'{log_dir}/{id}.json', 'a') as file:
             file.write(',\n{"role": "user","content": [{"type": "text","text": "'+text+'"},{"type": "image_url","image_url": {"url" : "'+url+'"} }]}')
@@ -115,14 +119,16 @@
 if len(api_key) == 0:
     logger.error("[ChatGLM]未正确配置API-Key！！！")
     logger.error("[ChatGLM]未正确配置API-Key！！！")
     logger.error("[ChatGLM]未正确配置API-Key！！！")
 
 if len(prompt) != 0 and len(nickname) != 0:
     logger.info("[ChatGLM]加载预设："+nickname)
+    if hard_prompt == True:
+        logger.info("硬预设启用")
     rg = True
 else:
     logger.info("[ChatGLM]预设未启用")
     rg = False
 
 logger.info("[ChatGLM]使用模型："+config.glm_model)
 
@@ -146,77 +152,77 @@
     """
     await ai_help.finish(msg)
 
 @ai.handle()
 async def _handle(gid: str = SessionId(SessionIdType.GROUP),text: Message = CommandArg()):
     if len(text) != 0:
         text = str(text)
-        id = gid
+        id = gid.replace(" ","_")
         #对用户输入进行转义防止炸json
         text_r = text.replace("\n","\\n")
         #读取聊天记录
         if len(api_key) != 0:
             if rg == False:
+                user_in(id,text_r)
                 with open(f'{log_dir}/{id}.json', 'r') as file:
                     history = file.read()
                 history = str(history)
-                user_in(id,text_r)
                 history = f"""
                 [
                 {history}
                 ]
                 """
             else:
                 if hard_prompt == False:
                     user_in(id,text_r)
                     with open(f'{log_dir}/{id}.json', 'r') as file:
                         history = file.read()
                     history = str(history)
                     s_prompt = '{"role": "system", "content": "'+prompt+'\\n接下来，请你进入\\"'+nickname+'\\"这个角色与大家对话。请记住你是'+nickname+'，你不能说你是程序或者AI,你是有血有肉、有真实情感的"},'
                     history = f"""
                     [
-                    {s_prompt}               
+                    {s_prompt}
                     {history}
                     ]
                     """
                 #硬预设启用
                 else:
                     text_r = text_r + f'({prompt}\\n接下来，请你进入\\"{nickname}\\"这个角色与大家对话。请记住你是{nickname}，你不能说你是程序或者AI,你是有血有肉、有真实情感的)'
                     user_in(id,text_r)
                     with open(f'{log_dir}/{id}.json', 'r') as file:
                         history = file.read()
                     history = str(history)
                     history = f"""
                     [
                     {history}
                     ]
-                    """                
+                    """
             try:
                 history = json.loads(history)
                 auth = generate_token(api_key)
                 try:
                     res = str(await req_glm(auth,history))
                     res_raw = res.replace("\n","\\n")
                     ai_out(id,res_raw)
                     await ai.finish(res)
                 except httpx.HTTPError as e:
                     res = f"请求接口出错～\n返回结果：{e}"
                     await ai.finish(res)
             except json.JSONDecodeError:
                 await ai.finish(f"聊天记录似乎炸了？\n请使用/{cmd} !reset 来重置")
-                
+
         else:
             await ai.finish("API-Key未正确配置！")
-            
+
     else:
         await ai.finish(f"消息不能为空\n可使用/{cmd} !help 命令查看帮助")
 
 @ai_img.handle()
 async def _handle(gid: str = SessionId(SessionIdType.GROUP),args: Message = CommandArg()):
-    id = gid   
+    id = gid.replace(" ","_")
     args = str(args)
     argl = args.split()
     if config.glm_model == "glm-4v":
         if len(argl) != 0:
             url = argl[0]
             text = argl[1]
             text_r = text.replace("\n","\\n")
@@ -251,15 +257,15 @@
                         with open(f'{log_dir}/{id}.json', 'r') as file:
                             history = file.read()
                         history = str(history)
                         history = f"""
                         [
                         {history}
                         ]
-                        """                                            
+                        """
                 history = json.loads(history)
                 auth = generate_token(api_key)
                 try:
                     res = str(await req_glm(auth,history))
                     res_raw = res.replace("\n","\\n")
                     ai_out(id,res_raw)
                     await ai.finish(res)
@@ -270,15 +276,15 @@
                 await ai.finish("API-Key未正确配置！")
 
         else:
             await ai_img.finish(f"参数不足！\n用法：/{cmd} !img [图片直链url] [你的文本消息]")
     else:
         await ai_img.finish(f"目前使用的模型为{config.glm_model}，不支持图片识别，请使用glm-4v模型")
 
-    
+
 #AI画图
 @ai_draw.handle()
 async def _handle(arg: Message = CommandArg()):
     arg = str(arg)
     if draw_on == True:
         try:
             auth = generate_token(api_key)
@@ -290,23 +296,23 @@
     else:
         await ai_draw.finish("未开启AI画图功能")
 
 
 
 @reset.handle()
 async def _handle(gid: str = SessionId(SessionIdType.GROUP)):
-    id = gid
+    id = gid.replace(" ","_")
     try:
-        os.remove(f"{log_dir}/{id}.json")
+        os.remove(f"{log_dir}/{id.replace(' ','.')}.json")
         await reset.finish("已清除聊天记录")
     except FileNotFoundError:
         await reset.finish("当前还没有会话哦！")
 
 
-    
+
 
 #异步请求AI
 async def req_glm(auth_token, usr_message):
     headers = {
         "Authorization": f"Bearer {auth_token}"
     }
     if max_token == 0:
@@ -318,15 +324,15 @@
     else:
         data = {
             "model": config.glm_model,
             "max_tokens": max_token,
             "temperature": config.glm_temperature,
             "messages": usr_message
         }
-    
+
     async with httpx.AsyncClient(timeout=httpx.Timeout(connect=10, read=config.glm_timeout, write=20, pool=30)) as client:
         res = await client.post(base_url, headers=headers, json=data)
         res = res.json()
     try:
         res_raw = res['choices'][0]['message']['content']
     except Exception as e:
         res_raw = res
@@ -345,8 +351,8 @@
     async with httpx.AsyncClient(timeout=httpx.Timeout(connect=10, read=config.glm_timeout, write=20, pool=30)) as client:
         res = await client.post(draw_url, headers=headers, json=data)
         res = res.json()
     try:
         res_raw = res['data'][0]['url']
     except Exception as e:
         res_raw = res
-    return res_raw
+    return res_raw
```

## Comparing `nonebot_plugin_chatglm_plus-0.1.8.dist-info/RECORD` & `nonebot_plugin_chatglm_plus-0.1.9.dist-info/RECORD`

 * *Files 24% similar despite different names*

```diff
@@ -1,6 +1,6 @@
-nonebot_plugin_chatglm_plus/__init__.py,sha256=pzmi3j_TszV4E8U2Gt33VlRfpGsrwDByS7rWsbD8o-U,12645
+nonebot_plugin_chatglm_plus/__init__.py,sha256=10xXEYmdeF4cX89pokwmV-gxkgXYvfm85vq_0vhUjuM,12859
 nonebot_plugin_chatglm_plus/config.py,sha256=aKCLlu_s1zIuRFiY20TpEHnO_IuuXXNSsKbv4nucGbw,1365
-nonebot_plugin_chatglm_plus-0.1.8.dist-info/METADATA,sha256=UD6k2Xzh0ctzfm1K2vqIeAHJ6IkzJ6g2s2lRrlYJA4I,501
-nonebot_plugin_chatglm_plus-0.1.8.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
-nonebot_plugin_chatglm_plus-0.1.8.dist-info/top_level.txt,sha256=YtSJTzABy_yXFiA2MC1RPrbeh82bUD5EU0RENr6_CiI,28
-nonebot_plugin_chatglm_plus-0.1.8.dist-info/RECORD,,
+nonebot_plugin_chatglm_plus-0.1.9.dist-info/METADATA,sha256=5sB0JC7xEk3eVy7eRtWYTnPyVo-2C6ycWYQ0qwLJlbk,501
+nonebot_plugin_chatglm_plus-0.1.9.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
+nonebot_plugin_chatglm_plus-0.1.9.dist-info/top_level.txt,sha256=YtSJTzABy_yXFiA2MC1RPrbeh82bUD5EU0RENr6_CiI,28
+nonebot_plugin_chatglm_plus-0.1.9.dist-info/RECORD,,
```

