# Comparing `tmp/cocorum-0.5.2.tar.gz` & `tmp/cocorum-0.5.3.tar.gz`

## Comparing `cocorum-0.5.2.tar` & `cocorum-0.5.3.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0   343002 2020-02-02 00:00:00.000000 cocorum-0.5.2/cocorum_icon.png
--rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 cocorum-0.5.2/requirements.txt
--rw-r--r--   0        0        0     1108 2020-02-02 00:00:00.000000 cocorum-0.5.2/.github/workflows/python-publish.yml
--rw-r--r--   0        0        0    20037 2020-02-02 00:00:00.000000 cocorum-0.5.2/src/cocorum/__init__.py
--rw-r--r--   0        0        0     1700 2020-02-02 00:00:00.000000 cocorum-0.5.2/src/cocorum/localvars.py
--rw-r--r--   0        0        0    14404 2020-02-02 00:00:00.000000 cocorum-0.5.2/src/cocorum/ssechat.py
--rw-r--r--   0        0        0     1983 2020-02-02 00:00:00.000000 cocorum-0.5.2/src/cocorum/utils.py
--rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 cocorum-0.5.2/LICENSE.txt
--rw-r--r--   0        0        0     2580 2020-02-02 00:00:00.000000 cocorum-0.5.2/README.md
--rw-r--r--   0        0        0      946 2020-02-02 00:00:00.000000 cocorum-0.5.2/pyproject.toml
--rw-r--r--   0        0        0     3434 2020-02-02 00:00:00.000000 cocorum-0.5.2/PKG-INFO
+-rw-r--r--   0        0        0   343002 2020-02-02 00:00:00.000000 cocorum-0.5.3/cocorum_icon.png
+-rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 cocorum-0.5.3/requirements.txt
+-rw-r--r--   0        0        0     1108 2020-02-02 00:00:00.000000 cocorum-0.5.3/.github/workflows/python-publish.yml
+-rw-r--r--   0        0        0    20037 2020-02-02 00:00:00.000000 cocorum-0.5.3/src/cocorum/__init__.py
+-rw-r--r--   0        0        0     1700 2020-02-02 00:00:00.000000 cocorum-0.5.3/src/cocorum/localvars.py
+-rw-r--r--   0        0        0    14502 2020-02-02 00:00:00.000000 cocorum-0.5.3/src/cocorum/ssechat.py
+-rw-r--r--   0        0        0     1983 2020-02-02 00:00:00.000000 cocorum-0.5.3/src/cocorum/utils.py
+-rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 cocorum-0.5.3/LICENSE.txt
+-rw-r--r--   0        0        0     2580 2020-02-02 00:00:00.000000 cocorum-0.5.3/README.md
+-rw-r--r--   0        0        0      946 2020-02-02 00:00:00.000000 cocorum-0.5.3/pyproject.toml
+-rw-r--r--   0        0        0     3434 2020-02-02 00:00:00.000000 cocorum-0.5.3/PKG-INFO
```

### Comparing `cocorum-0.5.2/cocorum_icon.png` & `cocorum-0.5.3/cocorum_icon.png`

 * *Files identical despite different names*

### Comparing `cocorum-0.5.2/.github/workflows/python-publish.yml` & `cocorum-0.5.3/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `cocorum-0.5.2/src/cocorum/__init__.py` & `cocorum-0.5.3/src/cocorum/__init__.py`

 * *Files identical despite different names*

### Comparing `cocorum-0.5.2/src/cocorum/localvars.py` & `cocorum-0.5.3/src/cocorum/localvars.py`

 * *Files identical despite different names*

### Comparing `cocorum-0.5.2/src/cocorum/ssechat.py` & `cocorum-0.5.3/src/cocorum/ssechat.py`

 * *Files 3% similar despite different names*

```diff
@@ -292,14 +292,15 @@
 
 class SSEChat():
     """Access the Rumble SSE chat api"""
     def __init__(self, stream_id):
         self.stream_id = utils.stream_id_ensure_b36(stream_id)
 
         self.__mailbox = [] #A mailbox if you will
+        self.deleted_message_ids = [] #IDs of messages that were deleted, as reported by the client
         self.users = {} #Dictionary of users by user ID
         self.channels = {} #Dictionary of channels by channel ID
         self.badges = {}
 
         #Connect to the API
         self.url = SSE_CHAT_URL.format(stream_id_b10 = self.stream_id_b10)
         self.client = sseclient.SSEClient(self.url)
@@ -338,20 +339,27 @@
         self.rants_enabled = jsondata["data"]["config"]["rants"]["enable"]
         #subscription TODO
         #rant levels TODO
         self.message_length_max = jsondata["data"]["config"]["message_length_max"]
 
     def update_mailbox(self, jsondata):
         """Parse chat messages from an SSE data JSON"""
+        #Add new messages
         self.__mailbox += [SSEChatMessage(message_json, self) for message_json in jsondata["data"]["messages"]]
 
     def clear_mailbox(self):
         """Delete anything in the mailbox"""
         self.__mailbox = []
 
+    def clear_deleted_message_ids(self):
+        """Clear and return the list of deleted message IDs"""
+        del_m = self.deleted_message_ids.copy()
+        self.deleted_message_ids = []
+        return del_m
+
     def update_users(self, jsondata):
         """Update our dictionary of users from an SSE data JSON"""
         for user_json in jsondata["data"]["users"]:
             try:
                 self.users[user_json["id"]]._jsondata = user_json #Update an existing user's JSON
             except KeyError: #User is new
                 self.users[user_json["id"]] = SSEChatUser(user_json, self)
@@ -369,37 +377,32 @@
         self.badges = {badge_slug : SSEChatUserBadge(badge_slug, jsondata["data"]["config"]["badges"][badge_slug], self) for badge_slug in jsondata["data"]["config"]["badges"].keys()}
 
     @property
     def stream_id_b10(self):
         """The chat ID in user"""
         return utils.stream_id_36_to_10(self.stream_id)
 
+    @property
     def next_chat_message(self):
         """Return the next chat message (parsing any additional data), waits for it to come in, returns None if chat closed"""
         if not self.__mailbox: #We don't already have messages
-            jsondata = self.next_jsondata()
+            #JSON data is coming in, but it isn't of messages type'
+            while (jsondata := self.next_jsondata()) and jsondata["type"] != "messages":
+
+                #Messages were deleted
+                if jsondata["type"] in ("delete_messages", "delete_non_rant_messages"):
+                    self.deleted_message_ids += jsondata["data"]["message_ids"]
+
+                #Unimplemented event type
+                else:
+                    print("API sent an unimplemented SSE event type")
+                    print(jsondata)
+
             if not jsondata: #The chat has closed or a blank event
                 return
 
-            #Messages were deleted, remove them from our mailbox if we have them
-            if jsondata["type"] == "delete_messages":
-                print("Messages were deleted. SSE handling not implemented.")
-#                 for message in self.__mailbox[:]:
-#                     if str(message.message_id) in jsondata["data"]["message_ids"]:
-#                         self.__mailbox.remove(message)
-#
-#                 if not self.__mailbox:
-#                     NotImplemented
-
-            #New chat messages came in
-            elif jsondata["type"] == "messages":
-                #Parse messages, users, and channels
-                self.update_mailbox(jsondata)
-                self.update_users(jsondata)
-                self.update_channels(jsondata)
-
-            #Unimplemented event type
-            else:
-                print("API sent an unimplemented SSE event type")
-                print(jsondata)
+            #Parse messages, users, and channels
+            self.update_mailbox(jsondata)
+            self.update_users(jsondata)
+            self.update_channels(jsondata)
 
         return self.__mailbox.pop(0) #Return the first message in the mailbox, and then remove it from there
```

### Comparing `cocorum-0.5.2/src/cocorum/utils.py` & `cocorum-0.5.3/src/cocorum/utils.py`

 * *Files identical despite different names*

### Comparing `cocorum-0.5.2/LICENSE.txt` & `cocorum-0.5.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `cocorum-0.5.2/README.md` & `cocorum-0.5.3/README.md`

 * *Files identical despite different names*

### Comparing `cocorum-0.5.2/pyproject.toml` & `cocorum-0.5.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "cocorum"
-version = "0.5.2"
+version = "0.5.3"
 keywords = ["rumble", "api", "wrapper", "livestream"]
 authors = [
   { name="Wilbur Jaywright", email="zargulthewizard@outlook.com" },
 ]
 description = "An unofficial Python wrapper for the Rumble Live Stream API v1.0 (beta)"
 readme = "README.md"
 requires-python = ">=3.8"
```

### Comparing `cocorum-0.5.2/PKG-INFO` & `cocorum-0.5.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: cocorum
-Version: 0.5.2
+Version: 0.5.3
 Summary: An unofficial Python wrapper for the Rumble Live Stream API v1.0 (beta)
 Project-URL: Homepage, https://github.com/thelabcat/rumble-api-wrapper-py
 Project-URL: Issues, https://github.com/thelabcat/rumble-api-wrapper-py/issues
 Project-URL: Rumble Live Stream API docs, https://rumblefaq.groovehq.com/help/how-to-use-rumble-s-live-stream-api
 Author-email: Wilbur Jaywright <zargulthewizard@outlook.com>
 License-File: LICENSE.txt
 Keywords: api,livestream,rumble,wrapper
```

