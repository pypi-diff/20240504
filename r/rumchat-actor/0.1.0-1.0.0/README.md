# Comparing `tmp/rumchat_actor-0.1.0.tar.gz` & `tmp/rumchat_actor-1.0.0.tar.gz`

## Comparing `rumchat_actor-0.1.0.tar` & `rumchat_actor-1.0.0.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 rumchat_actor-0.1.0/.github/workflows/python-publish.yml
--rw-r--r--   0        0        0    15876 2020-02-02 00:00:00.000000 rumchat_actor-0.1.0/src/rumchat_actor/__init__.py
--rw-r--r--   0        0        0     2292 2020-02-02 00:00:00.000000 rumchat_actor-0.1.0/src/rumchat_actor/common_commands.py
--rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 rumchat_actor-0.1.0/LICENSE.txt
--rw-r--r--   0        0        0     2076 2020-02-02 00:00:00.000000 rumchat_actor-0.1.0/README.md
--rw-r--r--   0        0        0      783 2020-02-02 00:00:00.000000 rumchat_actor-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     2796 2020-02-02 00:00:00.000000 rumchat_actor-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 rumchat_actor-1.0.0/.github/workflows/python-publish.yml
+-rw-r--r--   0        0        0    15936 2020-02-02 00:00:00.000000 rumchat_actor-1.0.0/src/rumchat_actor/__init__.py
+-rw-r--r--   0        0        0     2292 2020-02-02 00:00:00.000000 rumchat_actor-1.0.0/src/rumchat_actor/common_commands.py
+-rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 rumchat_actor-1.0.0/LICENSE.txt
+-rw-r--r--   0        0        0     2349 2020-02-02 00:00:00.000000 rumchat_actor-1.0.0/README.md
+-rw-r--r--   0        0        0      789 2020-02-02 00:00:00.000000 rumchat_actor-1.0.0/pyproject.toml
+-rw-r--r--   0        0        0     3075 2020-02-02 00:00:00.000000 rumchat_actor-1.0.0/PKG-INFO
```

### Comparing `rumchat_actor-0.1.0/.github/workflows/python-publish.yml` & `rumchat_actor-1.0.0/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `rumchat_actor-0.1.0/src/rumchat_actor/__init__.py` & `rumchat_actor-1.0.0/src/rumchat_actor/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -89,15 +89,15 @@
     def __init__(self, name, actor, cooldown = BROWSER_ACTION_DELAY, amount_cents = 0, allowed_badges = ["subscriber"], whitelist_badges = ["moderator"], target = None):
         """name: The !name of the command
     actor: The RumleChatActor host object
     amount_cents: The minimum cost of the command. Defaults to free
     allowed_badges: Badges which must be borne to use the command at all
     whitelist_badges: Badges which if borne give the user free-of-charge command access
     target: The function(message, actor) to call on successful command usage. Defaults to self.run"""
-        super().__init__(name, actor, cooldown = BROWSER_ACTION_DELAY, amount_cents = 0, whitelist_badges = ["moderator"], target = None)
+        super().__init__(name, actor, cooldown = BROWSER_ACTION_DELAY, amount_cents = 0, whitelist_badges = ["moderator"], target = target)
         #Admin can always call any command
         self.allowed_badges = ["admin"] + allowed_badges
 
     def call(self, message):
         """The command was called"""
         #the user does not have the required badge
         if not (True in [badge.slug in self.allowed_badges for badge in message.user.badges]):
@@ -193,15 +193,15 @@
         #History of the bot's messages so they do not get loop processed
         self.sent_messages = []
 
         #Send an initialization message to get wether we are moderator or not
         self.send_message(init_message)
 
         #Wait until we get that message
-        while (m := self.ssechat.next_chat_message()).user.username != self.username:
+        while (m := self.ssechat.get_message()).user.username != self.username:
             pass
 
         assert "moderator" in m.user.badges or "admin" in m.user.badges, "Actor cannot function without being a moderator"
 
         #Functions that are to be called on each message, must return False if the message was deleted
         self.message_actions = []
 
@@ -353,20 +353,20 @@
     def __process_message(self, message):
         """Process a single SSE Chat message"""
         #Do not do anything with the message if it matches one we sent before
         if message.text in self.sent_messages:
             return
 
         for action in self.message_actions:
-            if not action(message, self): #The message got deleted by an action
+            if message.message_id in self.ssechat.deleted_message_ids or not action(message, self): #The message got deleted, possibly by this action
                 return
 
         self.__run_if_command(message)
 
     def mainloop(self):
         """Run the actor forever"""
         while self.keep_running:
-            m = self.ssechat.next_chat_message()
+            m = self.ssechat.get_message()
             if not m: #Chat has closed
                 self.keep_running = False
                 return
             self.__process_message(m)
```

### Comparing `rumchat_actor-0.1.0/src/rumchat_actor/common_commands.py` & `rumchat_actor-1.0.0/src/rumchat_actor/common_commands.py`

 * *Files identical despite different names*

### Comparing `rumchat_actor-0.1.0/LICENSE.txt` & `rumchat_actor-1.0.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `rumchat_actor-0.1.0/README.md` & `rumchat_actor-1.0.0/README.md`

 * *Files 19% similar despite different names*

```diff
@@ -37,7 +37,12 @@
 actor.register_command(name = "tester", command = lambda message, actor: print(f"Test command run by {message.user.username}"))
 
 #Run the bot continuously
 actor.mainloop()
 ```
 
 You would write this script, and run it as your local Rumble Chat Actor instance. Note that it currently does not exit on its own when a livestream ends.
+Hope this helps!
+
+I, Wilbur Jaywright, and my brand, Marswide BGL, have no official association with Rumble Corp. beyond that of a normal user and/or channel on the Rumble Video platform. This wrapper is not officially endorsed by Rumble Corp. or its subsidiaries.
+
+S.D.G.
```

### Comparing `rumchat_actor-0.1.0/pyproject.toml` & `rumchat_actor-1.0.0/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "rumchat_actor"
-version = "0.1.0"
+version = "1.0.0"
 keywords = ["rumble", "chat", "livestream", "bot"]
 authors = [
   { name="Wilbur Jaywright", email="zargulthewizard@outlook.com" },
 ]
 description = "Automatically interact with your Rumble livestream chats."
 readme = "README.md"
 requires-python = ">=3.8"
 dependencies = [
-  "cocorum",
+  "cocorum>=1.0.0",
   "selenium",
   ]
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: GNU Affero General Public License v3",
     "Operating System :: OS Independent",
-    "Development Status :: 3 - Alpha",
+    "Development Status :: 4 - Beta",
 ]
 
 [project.urls]
 Homepage = "https://github.com/thelabcat/rum-chat-actor"
 Issues = "https://github.com/thelabcat/rumble-api-wrapper-py/issues"
```

### Comparing `rumchat_actor-0.1.0/PKG-INFO` & `rumchat_actor-1.0.0/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.3
 Name: rumchat_actor
-Version: 0.1.0
+Version: 1.0.0
 Summary: Automatically interact with your Rumble livestream chats.
 Project-URL: Homepage, https://github.com/thelabcat/rum-chat-actor
 Project-URL: Issues, https://github.com/thelabcat/rumble-api-wrapper-py/issues
 Author-email: Wilbur Jaywright <zargulthewizard@outlook.com>
 License-File: LICENSE.txt
 Keywords: bot,chat,livestream,rumble
-Classifier: Development Status :: 3 - Alpha
+Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.8
-Requires-Dist: cocorum
+Requires-Dist: cocorum>=1.0.0
 Requires-Dist: selenium
 Description-Content-Type: text/markdown
 
 # Rumble Chat Actor
 Automatically interact with your Rumble livestream chats.
 
 This project requires the following python libraries:
@@ -55,7 +55,12 @@
 actor.register_command(name = "tester", command = lambda message, actor: print(f"Test command run by {message.user.username}"))
 
 #Run the bot continuously
 actor.mainloop()
 ```
 
 You would write this script, and run it as your local Rumble Chat Actor instance. Note that it currently does not exit on its own when a livestream ends.
+Hope this helps!
+
+I, Wilbur Jaywright, and my brand, Marswide BGL, have no official association with Rumble Corp. beyond that of a normal user and/or channel on the Rumble Video platform. This wrapper is not officially endorsed by Rumble Corp. or its subsidiaries.
+
+S.D.G.
```

