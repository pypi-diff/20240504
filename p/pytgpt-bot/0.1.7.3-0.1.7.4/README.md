# Comparing `tmp/pytgpt_bot-0.1.7.3.tar.gz` & `tmp/pytgpt_bot-0.1.7.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytgpt_bot-0.1.7.3.tar", last modified: Wed May  1 04:54:51 2024, max compression
+gzip compressed data, was "pytgpt_bot-0.1.7.4.tar", last modified: Sat May  4 10:05:23 2024, max compression
```

## Comparing `pytgpt_bot-0.1.7.3.tar` & `pytgpt_bot-0.1.7.4.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 04:54:51.358818 pytgpt_bot-0.1.7.3/
--rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-05-01 04:54:30.000000 pytgpt_bot-0.1.7.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     8266 2024-05-01 04:54:51.358818 pytgpt_bot-0.1.7.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     6482 2024-05-01 04:54:30.000000 pytgpt_bot-0.1.7.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 04:54:51.358818 pytgpt_bot-0.1.7.3/pytgpt_bot/
--rw-r--r--   0 runner    (1001) docker     (127)      225 2024-05-01 04:54:30.000000 pytgpt_bot-0.1.7.3/pytgpt_bot/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       42 2024-05-01 04:54:30.000000 pytgpt_bot-0.1.7.3/pytgpt_bot/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3358 2024-05-01 04:54:30.000000 pytgpt_bot-0.1.7.3/pytgpt_bot/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)      891 2024-05-01 04:54:30.000000 pytgpt_bot-0.1.7.3/pytgpt_bot/config.py
--rw-r--r--   0 runner    (1001) docker     (127)      990 2024-05-01 04:54:30.000000 pytgpt_bot-0.1.7.3/pytgpt_bot/db.py
--rw-r--r--   0 runner    (1001) docker     (127)     2798 2024-05-01 04:54:30.000000 pytgpt_bot-0.1.7.3/pytgpt_bot/filters.py
--rw-r--r--   0 runner    (1001) docker     (127)    28809 2024-05-01 04:54:30.000000 pytgpt_bot-0.1.7.3/pytgpt_bot/main.py
--rw-r--r--   0 runner    (1001) docker     (127)     1799 2024-05-01 04:54:30.000000 pytgpt_bot-0.1.7.3/pytgpt_bot/models.py
--rw-r--r--   0 runner    (1001) docker     (127)     4057 2024-05-01 04:54:30.000000 pytgpt_bot-0.1.7.3/pytgpt_bot/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 04:54:51.358818 pytgpt_bot-0.1.7.3/pytgpt_bot.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     8266 2024-05-01 04:54:51.000000 pytgpt_bot-0.1.7.3/pytgpt_bot.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      416 2024-05-01 04:54:51.000000 pytgpt_bot-0.1.7.3/pytgpt_bot.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-01 04:54:51.000000 pytgpt_bot-0.1.7.3/pytgpt_bot.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       52 2024-05-01 04:54:51.000000 pytgpt_bot-0.1.7.3/pytgpt_bot.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       97 2024-05-01 04:54:51.000000 pytgpt_bot-0.1.7.3/pytgpt_bot.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-01 04:54:51.000000 pytgpt_bot-0.1.7.3/pytgpt_bot.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-01 04:54:51.358818 pytgpt_bot-0.1.7.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2384 2024-05-01 04:54:30.000000 pytgpt_bot-0.1.7.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 10:05:23.740556 pytgpt_bot-0.1.7.4/
+-rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-05-04 10:04:59.000000 pytgpt_bot-0.1.7.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     8266 2024-05-04 10:05:23.740556 pytgpt_bot-0.1.7.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6482 2024-05-04 10:04:59.000000 pytgpt_bot-0.1.7.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 10:05:23.740556 pytgpt_bot-0.1.7.4/pytgpt_bot/
+-rw-r--r--   0 runner    (1001) docker     (127)      225 2024-05-04 10:04:59.000000 pytgpt_bot-0.1.7.4/pytgpt_bot/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       42 2024-05-04 10:04:59.000000 pytgpt_bot-0.1.7.4/pytgpt_bot/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3358 2024-05-04 10:04:59.000000 pytgpt_bot-0.1.7.4/pytgpt_bot/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)      891 2024-05-04 10:04:59.000000 pytgpt_bot-0.1.7.4/pytgpt_bot/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1044 2024-05-04 10:04:59.000000 pytgpt_bot-0.1.7.4/pytgpt_bot/db.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2798 2024-05-04 10:04:59.000000 pytgpt_bot-0.1.7.4/pytgpt_bot/filters.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28868 2024-05-04 10:04:59.000000 pytgpt_bot-0.1.7.4/pytgpt_bot/main.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1799 2024-05-04 10:04:59.000000 pytgpt_bot-0.1.7.4/pytgpt_bot/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3689 2024-05-04 10:04:59.000000 pytgpt_bot-0.1.7.4/pytgpt_bot/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 10:05:23.740556 pytgpt_bot-0.1.7.4/pytgpt_bot.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     8266 2024-05-04 10:05:23.000000 pytgpt_bot-0.1.7.4/pytgpt_bot.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      416 2024-05-04 10:05:23.000000 pytgpt_bot-0.1.7.4/pytgpt_bot.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-04 10:05:23.000000 pytgpt_bot-0.1.7.4/pytgpt_bot.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-05-04 10:05:23.000000 pytgpt_bot-0.1.7.4/pytgpt_bot.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       97 2024-05-04 10:05:23.000000 pytgpt_bot-0.1.7.4/pytgpt_bot.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-04 10:05:23.000000 pytgpt_bot-0.1.7.4/pytgpt_bot.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-04 10:05:23.740556 pytgpt_bot-0.1.7.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2384 2024-05-04 10:04:59.000000 pytgpt_bot-0.1.7.4/setup.py
```

### Comparing `pytgpt_bot-0.1.7.3/LICENSE` & `pytgpt_bot-0.1.7.4/LICENSE`

 * *Files identical despite different names*

### Comparing `pytgpt_bot-0.1.7.3/PKG-INFO` & `pytgpt_bot-0.1.7.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytgpt-bot
-Version: 0.1.7.3
+Version: 0.1.7.4
 Summary: AI powered Telegram bot for chatting, text-to-image and text-to-speech conversions
 Home-page: https://github.com/Simatwa/pytgpt-bot
 Author: Smartwa
 Author-email: simatwacaleb@proton.me
 Maintainer: Smartwa
 License: MIT
 Project-URL: Bug Report, https://github.com/Simatwa/pytgpt-bot/issues/new
@@ -28,15 +28,15 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: pytelegrambotapi==4.17.0
-Requires-Dist: python-tgpt==0.6.6
+Requires-Dist: python-tgpt==0.7.0
 Requires-Dist: python-dotenv==1.0.0
 Requires-Dist: click==8.1.3
 Requires-Dist: SQLAlchemy==2.0.29
 
 <p align="center">
 <a href="https://github.com/Simatwa/pytgpt-bot/blob/main/LICENSE"><img alt="License" src="https://img.shields.io/static/v1?logo=MIT&color=Blue&message=MIT&label=License"/></a>
 <a href="#"><img alt="Python version" src="https://img.shields.io/pypi/pyversions/pytgpt-bot"/></a>
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: pytgpt-bot Version: 0.1.7.3 Summary: AI powered
+Metadata-Version: 2.1 Name: pytgpt-bot Version: 0.1.7.4 Summary: AI powered
 Telegram bot for chatting, text-to-image and text-to-speech conversions Home-
 page: https://github.com/Simatwa/pytgpt-bot Author: Smartwa Author-email:
 simatwacaleb@proton.me Maintainer: Smartwa License: MIT Project-URL: Bug
 Report, https://github.com/Simatwa/pytgpt-bot/issues/new Project-URL: Homepage,
 https://github.com/Simatwa/pytgpt-bot Project-URL: Source Code, https://
 github.com/Simatwa/pytgpt-bot Project-URL: Issue Tracker, https://github.com/
 Simatwa/pytgpt-bot/issues Project-URL: Download, https://github.com/Simatwa/
@@ -16,15 +16,15 @@
 Language :: Python Classifier: Topic :: Software Development :: Libraries ::
 Python Modules Classifier: Topic :: Scientific/Engineering :: Artificial
 Intelligence Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
 Language :: Python :: 3.10 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12 Requires-Python: >=3.10
 Description-Content-Type: text/markdown License-File: LICENSE Requires-Dist:
-pytelegrambotapi==4.17.0 Requires-Dist: python-tgpt==0.6.6 Requires-Dist:
+pytelegrambotapi==4.17.0 Requires-Dist: python-tgpt==0.7.0 Requires-Dist:
 python-dotenv==1.0.0 Requires-Dist: click==8.1.3 Requires-Dist:
 SQLAlchemy==2.0.29
 _[_L_i_c_e_n_s_e_]_[_P_y_t_h_o_n_ _v_e_r_s_i_o_n_]_[_P_y_P_i_]_[_B_l_a_c_k_]_[_D_o_w_n_l_o_a_d_s_]_[_h_t_t_p_s_:_/_/_h_i_t_s_._s_e_e_y_o_u_f_a_r_m_._c_o_m_/
    _a_p_i_/_c_o_u_n_t_/_i_n_c_r_/_b_a_d_g_e_._s_v_g_?_u_r_l_=_h_t_t_p_s_%_3_A_%_2_F_%_2_F_g_i_t_h_u_b_._c_o_m_/_S_i_m_a_t_w_a_/_p_y_t_g_p_t_-_b_o_t_]
                                   _[_w_a_k_a_t_i_m_e_]
                       ************ WWeellccoommee ttoo _pp_yy_tt_gg_pp_tt_--_bb_oo_tt ************
 This is a Telegram bot based on [python-tgpt](https://github.com/Simatwa/
```

### Comparing `pytgpt_bot-0.1.7.3/README.md` & `pytgpt_bot-0.1.7.4/README.md`

 * *Files identical despite different names*

### Comparing `pytgpt_bot-0.1.7.3/pytgpt_bot/cli.py` & `pytgpt_bot-0.1.7.4/pytgpt_bot/cli.py`

 * *Files identical despite different names*

### Comparing `pytgpt_bot-0.1.7.3/pytgpt_bot/config.py` & `pytgpt_bot-0.1.7.4/pytgpt_bot/config.py`

 * *Files identical despite different names*

### Comparing `pytgpt_bot-0.1.7.3/pytgpt_bot/db.py` & `pytgpt_bot-0.1.7.4/pytgpt_bot/db.py`

 * *Files 7% similar despite different names*

```diff
@@ -21,14 +21,15 @@
         chat = session.query(Chat).filter_by(id=id).first()
         if chat:
             # chat exist
             self.chat = chat
         else:
             self.chat = Chat(id=id)
             session.add(self.chat)
+            session.commit()  # For the sake of async
 
     @property
     def is_admin(self) -> bool:
         """Checks user admin status"""
         return self.chat.id == admin_id
 
     def delete(self) -> None:
```

### Comparing `pytgpt_bot-0.1.7.3/pytgpt_bot/filters.py` & `pytgpt_bot-0.1.7.4/pytgpt_bot/filters.py`

 * *Files identical despite different names*

### Comparing `pytgpt_bot-0.1.7.3/pytgpt_bot/main.py` & `pytgpt_bot-0.1.7.4/pytgpt_bot/main.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import asyncio
 from telebot.async_telebot import AsyncTeleBot
 import telebot.util as telebot_util
 import pytgpt.imager as image_generator
 from pytgpt.utils import Audio as audio_generator
 from pytgpt.utils import Conversation
 from pytgpt.utils import AwesomePrompts
-from pytgpt.gpt4free import GPT4FREE
+from pytgpt.gpt4free import AsyncGPT4FREE
 from functools import wraps
 from sqlalchemy import text
 from uuid import uuid4
 
 from pytgpt_bot import __version__, __repo__
 
 from pytgpt_bot.config import (
@@ -434,15 +434,15 @@
 @bot.channel_post_handler(commands=["check"], is_chat_admin=True)
 @handler_formatter()
 async def check_current_settings(message: telebot.types.Message):
     """Check current user settings"""
     chat = User(message).chat
     current_user_settings = (
         f"Is Active :  `{chat.is_active}`\n"
-        f"Chat Length : `{len(chat.history)}`\n"
+        f"Chat Length : `{len(chat.history) if chat.history else 0}`\n"
         f"Speech Voice : `{chat.voice}`\n"
         f"Chat Provider : `{chat.provider}`\n"
         f"Chat Intro : `{chat.intro}`"
     )
     return await bot.reply_to(
         message,
         current_user_settings,
@@ -696,22 +696,24 @@
     conversation = Conversation(max_tokens=max_tokens)
     conversation.chat_history = user.chat.history
     conversation_prompt = conversation.gen_complete_prompt(
         message.text, intro=user.chat.intro
     )
     await bot.send_chat_action(message.chat.id, "typing")
 
-    provider_class = provider_map.get(user.chat.provider, GPT4FREE)
+    provider_class = provider_map.get(user.chat.provider, AsyncGPT4FREE)
     provider_class_kwargs: dict = dict(is_conversation=False, timeout=timeout)
 
     if user.chat.provider in g4f_providers:
         # gp4f provider
         provider_class_kwargs["provider"] = user.chat.provider
 
-    ai_response = provider_class(**provider_class_kwargs).chat(conversation_prompt)
+    ai_response = await provider_class(**provider_class_kwargs).chat(
+        conversation_prompt
+    )
     conversation.update_chat_history(
         prompt=message.text, response=ai_response, force=True
     )
     user.chat.history = conversation.chat_history
     await send_long_text(
         message, ai_response, as_reply=False if message.from_user else True
     )
@@ -778,15 +780,15 @@
             f"Error while handling inline query - [{user_id}] : {e.args[1] if e.args and len(e.args)>1 else e}"
         )
 
 
 @bot.message_handler(is_chat_active=True)
 @bot.channel_post_handler(is_chat_active=True, is_bot_tagged=True)
 async def any_other_action(message):
-    return bot.reply_to(
+    return await bot.reply_to(
         message,
         usage_info,
         reply_markup=make_delete_markup(message),
         parse_mode="Markdown",
     )
```

### Comparing `pytgpt_bot-0.1.7.3/pytgpt_bot/models.py` & `pytgpt_bot-0.1.7.4/pytgpt_bot/models.py`

 * *Files identical despite different names*

### Comparing `pytgpt_bot-0.1.7.3/pytgpt_bot/utils.py` & `pytgpt_bot-0.1.7.4/pytgpt_bot/utils.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,32 +1,19 @@
 from os import makedirs, environ
 from pytgpt.utils import api_static_dir
-
-from pytgpt.opengpt import OPENGPT
-from pytgpt.koboldai import KOBOLDAI
-from pytgpt.phind import PHIND
-from pytgpt.llama2 import LLAMA2
-from pytgpt.blackboxai import BLACKBOXAI
-from pytgpt.perplexity import PERPLEXITY
-from pytgpt.yepchat import YEPCHAT
-from pytgpt.auto import AUTO
+from pytgpt.async_providers import tgpt_mapper as provider_map
+from pytgpt.auto import AsyncAUTO
 from random import choice
 import telebot
 import pytgpt.gpt4free.utils as g4f_util
 
-provider_map: dict[str, object] = {
-    "opengpt": OPENGPT,
-    "koboldai": KOBOLDAI,
-    "phind": PHIND,
-    "llama2": LLAMA2,
-    "blackboxai": BLACKBOXAI,
-    "perplexity": PERPLEXITY,
-    "yepchat": YEPCHAT,
-    "auto": AUTO,
-}
+provider_map.update(
+    dict(auto=AsyncAUTO),
+)
+
 
 emojis: dict[str, list[str]] = {
     "angry": [
         "😠",  # Angry Face
         "😡",  # Pouting Face
         "😤",  # Face with Steam From Nose
         "😖",  # Confounded Face
```

### Comparing `pytgpt_bot-0.1.7.3/pytgpt_bot.egg-info/PKG-INFO` & `pytgpt_bot-0.1.7.4/pytgpt_bot.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytgpt-bot
-Version: 0.1.7.3
+Version: 0.1.7.4
 Summary: AI powered Telegram bot for chatting, text-to-image and text-to-speech conversions
 Home-page: https://github.com/Simatwa/pytgpt-bot
 Author: Smartwa
 Author-email: simatwacaleb@proton.me
 Maintainer: Smartwa
 License: MIT
 Project-URL: Bug Report, https://github.com/Simatwa/pytgpt-bot/issues/new
@@ -28,15 +28,15 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: pytelegrambotapi==4.17.0
-Requires-Dist: python-tgpt==0.6.6
+Requires-Dist: python-tgpt==0.7.0
 Requires-Dist: python-dotenv==1.0.0
 Requires-Dist: click==8.1.3
 Requires-Dist: SQLAlchemy==2.0.29
 
 <p align="center">
 <a href="https://github.com/Simatwa/pytgpt-bot/blob/main/LICENSE"><img alt="License" src="https://img.shields.io/static/v1?logo=MIT&color=Blue&message=MIT&label=License"/></a>
 <a href="#"><img alt="Python version" src="https://img.shields.io/pypi/pyversions/pytgpt-bot"/></a>
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: pytgpt-bot Version: 0.1.7.3 Summary: AI powered
+Metadata-Version: 2.1 Name: pytgpt-bot Version: 0.1.7.4 Summary: AI powered
 Telegram bot for chatting, text-to-image and text-to-speech conversions Home-
 page: https://github.com/Simatwa/pytgpt-bot Author: Smartwa Author-email:
 simatwacaleb@proton.me Maintainer: Smartwa License: MIT Project-URL: Bug
 Report, https://github.com/Simatwa/pytgpt-bot/issues/new Project-URL: Homepage,
 https://github.com/Simatwa/pytgpt-bot Project-URL: Source Code, https://
 github.com/Simatwa/pytgpt-bot Project-URL: Issue Tracker, https://github.com/
 Simatwa/pytgpt-bot/issues Project-URL: Download, https://github.com/Simatwa/
@@ -16,15 +16,15 @@
 Language :: Python Classifier: Topic :: Software Development :: Libraries ::
 Python Modules Classifier: Topic :: Scientific/Engineering :: Artificial
 Intelligence Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
 Language :: Python :: 3.10 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12 Requires-Python: >=3.10
 Description-Content-Type: text/markdown License-File: LICENSE Requires-Dist:
-pytelegrambotapi==4.17.0 Requires-Dist: python-tgpt==0.6.6 Requires-Dist:
+pytelegrambotapi==4.17.0 Requires-Dist: python-tgpt==0.7.0 Requires-Dist:
 python-dotenv==1.0.0 Requires-Dist: click==8.1.3 Requires-Dist:
 SQLAlchemy==2.0.29
 _[_L_i_c_e_n_s_e_]_[_P_y_t_h_o_n_ _v_e_r_s_i_o_n_]_[_P_y_P_i_]_[_B_l_a_c_k_]_[_D_o_w_n_l_o_a_d_s_]_[_h_t_t_p_s_:_/_/_h_i_t_s_._s_e_e_y_o_u_f_a_r_m_._c_o_m_/
    _a_p_i_/_c_o_u_n_t_/_i_n_c_r_/_b_a_d_g_e_._s_v_g_?_u_r_l_=_h_t_t_p_s_%_3_A_%_2_F_%_2_F_g_i_t_h_u_b_._c_o_m_/_S_i_m_a_t_w_a_/_p_y_t_g_p_t_-_b_o_t_]
                                   _[_w_a_k_a_t_i_m_e_]
                       ************ WWeellccoommee ttoo _pp_yy_tt_gg_pp_tt_--_bb_oo_tt ************
 This is a Telegram bot based on [python-tgpt](https://github.com/Simatwa/
```

### Comparing `pytgpt_bot-0.1.7.3/setup.py` & `pytgpt_bot-0.1.7.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     full_path: Path = ROOT_PATH / path
     return full_path.read_text(encoding="utf-8")
 
 
 setup(
     name="pytgpt-bot",
     packages=["pytgpt_bot"],
-    version="0.1.7.3",
+    version="0.1.7.4",
     license="MIT",
     author="Smartwa",
     maintainer="Smartwa",
     author_email="simatwacaleb@proton.me",
     description="AI powered Telegram bot for chatting, text-to-image and text-to-speech conversions",
     url="https://github.com/Simatwa/pytgpt-bot",
     project_urls={
@@ -31,15 +31,15 @@
     entry_points={
         "console_scripts": [
             "pytgpt-bot = pytgpt_bot.cli:entry",
         ],
     },
     install_requires=[
         "pytelegrambotapi==4.17.0",
-        "python-tgpt==0.6.6",
+        "python-tgpt==0.7.0",
         "python-dotenv==1.0.0",
         "click==8.1.3",
         "SQLAlchemy==2.0.29",
     ],
     python_requires=">=3.10",
     keywords=[
         "ai",
```

