# Comparing `tmp/cocorum-0.5.1.tar.gz` & `tmp/cocorum-0.5.2.tar.gz`

## Comparing `cocorum-0.5.1.tar` & `cocorum-0.5.2.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0   343002 2020-02-02 00:00:00.000000 cocorum-0.5.1/cocorum_icon.png
--rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 cocorum-0.5.1/requirements.txt
--rw-r--r--   0        0        0     1108 2020-02-02 00:00:00.000000 cocorum-0.5.1/.github/workflows/python-publish.yml
--rw-r--r--   0        0        0    20084 2020-02-02 00:00:00.000000 cocorum-0.5.1/src/cocorum/__init__.py
--rw-r--r--   0        0        0     1700 2020-02-02 00:00:00.000000 cocorum-0.5.1/src/cocorum/localvars.py
--rw-r--r--   0        0        0    13806 2020-02-02 00:00:00.000000 cocorum-0.5.1/src/cocorum/ssechat.py
--rw-r--r--   0        0        0     1983 2020-02-02 00:00:00.000000 cocorum-0.5.1/src/cocorum/utils.py
--rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 cocorum-0.5.1/LICENSE.txt
--rw-r--r--   0        0        0     2580 2020-02-02 00:00:00.000000 cocorum-0.5.1/README.md
--rw-r--r--   0        0        0      946 2020-02-02 00:00:00.000000 cocorum-0.5.1/pyproject.toml
--rw-r--r--   0        0        0     3434 2020-02-02 00:00:00.000000 cocorum-0.5.1/PKG-INFO
+-rw-r--r--   0        0        0   343002 2020-02-02 00:00:00.000000 cocorum-0.5.2/cocorum_icon.png
+-rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 cocorum-0.5.2/requirements.txt
+-rw-r--r--   0        0        0     1108 2020-02-02 00:00:00.000000 cocorum-0.5.2/.github/workflows/python-publish.yml
+-rw-r--r--   0        0        0    20037 2020-02-02 00:00:00.000000 cocorum-0.5.2/src/cocorum/__init__.py
+-rw-r--r--   0        0        0     1700 2020-02-02 00:00:00.000000 cocorum-0.5.2/src/cocorum/localvars.py
+-rw-r--r--   0        0        0    14404 2020-02-02 00:00:00.000000 cocorum-0.5.2/src/cocorum/ssechat.py
+-rw-r--r--   0        0        0     1983 2020-02-02 00:00:00.000000 cocorum-0.5.2/src/cocorum/utils.py
+-rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 cocorum-0.5.2/LICENSE.txt
+-rw-r--r--   0        0        0     2580 2020-02-02 00:00:00.000000 cocorum-0.5.2/README.md
+-rw-r--r--   0        0        0      946 2020-02-02 00:00:00.000000 cocorum-0.5.2/pyproject.toml
+-rw-r--r--   0        0        0     3434 2020-02-02 00:00:00.000000 cocorum-0.5.2/PKG-INFO
```

### Comparing `cocorum-0.5.1/cocorum_icon.png` & `cocorum-0.5.2/cocorum_icon.png`

 * *Files identical despite different names*

### Comparing `cocorum-0.5.1/.github/workflows/python-publish.yml` & `cocorum-0.5.2/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `cocorum-0.5.1/src/cocorum/__init__.py` & `cocorum-0.5.2/src/cocorum/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -88,16 +88,15 @@
         """The user's profile picture as a bytes string"""
         if not self.profile_pic_url: #The profile picture is blank
             return b''
 
         if not self.__profile_pic: #We never queried the profile pic before
             #TODO make this timeout assignable
             response = requests.get(self.profile_pic_url, timeout = DEFAULT_TIMEOUT)
-            if response.status_code != 200:
-                raise Exception("Status code " + str(response.status_code))
+            assert response.status_code == 200, "Status code " + str(response.status_code)
 
             self.__profile_pic = response.content
 
         return self.__profile_pic
 
 class Follower(UserAction):
     """Rumble follower"""
@@ -465,16 +464,15 @@
         if time.time() - self.last_refresh_time > self.refresh_rate:
             self.refresh()
 
     def refresh(self):
         """Reload data from the API"""
         self.last_refresh_time = time.time()
         response = requests.get(self.api_url, headers = HEADERS, timeout = self.request_timeout)
-        if response.status_code != 200:
-            raise Exception("Status code " + str(response.status_code))
+        assert response.status_code == 200, "Status code " + str(response.status_code)
 
         self._json = response.json()
 
         #Remove livestream references that are no longer listed
         listed_ids = [json["id"] for json in self._json["livestreams"]]
         for stream_id in self.__livestreams.copy():
             if stream_id not in listed_ids:
@@ -490,15 +488,15 @@
             except KeyError: #The livestream has not been stored yet
                 self.__livestreams[json["id"]] = Livestream(json, self)
 
     @property
     def data_timestamp(self):
         """The timestamp on the last data refresh"""
         #Definitely don't ever trigger a refresh on this
-        self._json["now"]
+        return self._json["now"]
 
     @property
     def api_type(self):
         """Type of API URL in use, user or channel"""
         return self["type"]
 
     @property
```

### Comparing `cocorum-0.5.1/src/cocorum/localvars.py` & `cocorum-0.5.2/src/cocorum/localvars.py`

 * *Files identical despite different names*

### Comparing `cocorum-0.5.1/src/cocorum/ssechat.py` & `cocorum-0.5.2/src/cocorum/ssechat.py`

 * *Files 3% similar despite different names*

```diff
@@ -80,16 +80,15 @@
         """The chatter's profile picture as a bytes string"""
         if not self.profile_pic_url: #The profile picture is blank
             return b''
 
         if not self.__profile_pic: #We never queried the profile pic before
             #TODO make the timeout configurable
             response = requests.get(self.profile_pic_url, timeout = DEFAULT_TIMEOUT)
-            if response.status_code != 200:
-                raise Exception("Status code " + str(response.status_code))
+            assert response.status_code == 200, "Status code " + str(response.status_code)
 
             self.__profile_pic = response.content
 
         return self.__profile_pic
 
 class SSEChatUser(SSEChatter):
     """User in SSE chat"""
@@ -190,16 +189,15 @@
 
     @property
     def icon(self):
         """The badge's icon as a bytestring"""
         if not self.__icon: #We never queried the icon before
             #TODO make the timeout configurable
             response = requests.get(self.icon_url, timeout = DEFAULT_TIMEOUT)
-            if response.status_code != 200:
-                raise Exception("Status code " + str(response.status_code))
+            assert response.status_code == 200, "Status code " + str(response.status_code)
 
             self.__icon = response.content
 
         return self.__icon
 
 class SSEChatMessage(SSEChatObject):
     """A single chat message from the SSE API"""
@@ -322,14 +320,15 @@
             return self.next_jsondata()
 
         return json.loads(message.data)
 
     def parse_init_data(self, jsondata):
         """Extract initial chat data from the SSE init message JSON"""
         if jsondata["type"] != "init":
+            print(jsondata)
             raise ValueError("That is not init json")
 
         #Parse pre-connection messages, users, and channels
         self.update_mailbox(jsondata)
         self.update_users(jsondata)
         self.update_channels(jsondata)
 
@@ -376,16 +375,31 @@
 
     def next_chat_message(self):
         """Return the next chat message (parsing any additional data), waits for it to come in, returns None if chat closed"""
         if not self.__mailbox: #We don't already have messages
             jsondata = self.next_jsondata()
             if not jsondata: #The chat has closed or a blank event
                 return
-            if jsondata["type"] != "messages":
-                raise ValueError("API did not send a messages message")
 
-            #Parse messages, users, and channels
-            self.update_mailbox(jsondata)
-            self.update_users(jsondata)
-            self.update_channels(jsondata)
+            #Messages were deleted, remove them from our mailbox if we have them
+            if jsondata["type"] == "delete_messages":
+                print("Messages were deleted. SSE handling not implemented.")
+#                 for message in self.__mailbox[:]:
+#                     if str(message.message_id) in jsondata["data"]["message_ids"]:
+#                         self.__mailbox.remove(message)
+#
+#                 if not self.__mailbox:
+#                     NotImplemented
+
+            #New chat messages came in
+            elif jsondata["type"] == "messages":
+                #Parse messages, users, and channels
+                self.update_mailbox(jsondata)
+                self.update_users(jsondata)
+                self.update_channels(jsondata)
+
+            #Unimplemented event type
+            else:
+                print("API sent an unimplemented SSE event type")
+                print(jsondata)
 
         return self.__mailbox.pop(0) #Return the first message in the mailbox, and then remove it from there
```

### Comparing `cocorum-0.5.1/src/cocorum/utils.py` & `cocorum-0.5.2/src/cocorum/utils.py`

 * *Files identical despite different names*

### Comparing `cocorum-0.5.1/LICENSE.txt` & `cocorum-0.5.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `cocorum-0.5.1/README.md` & `cocorum-0.5.2/README.md`

 * *Files identical despite different names*

### Comparing `cocorum-0.5.1/pyproject.toml` & `cocorum-0.5.2/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "cocorum"
-version = "0.5.1"
+version = "0.5.2"
 keywords = ["rumble", "api", "wrapper", "livestream"]
 authors = [
   { name="Wilbur Jaywright", email="zargulthewizard@outlook.com" },
 ]
 description = "An unofficial Python wrapper for the Rumble Live Stream API v1.0 (beta)"
 readme = "README.md"
 requires-python = ">=3.8"
```

### Comparing `cocorum-0.5.1/PKG-INFO` & `cocorum-0.5.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: cocorum
-Version: 0.5.1
+Version: 0.5.2
 Summary: An unofficial Python wrapper for the Rumble Live Stream API v1.0 (beta)
 Project-URL: Homepage, https://github.com/thelabcat/rumble-api-wrapper-py
 Project-URL: Issues, https://github.com/thelabcat/rumble-api-wrapper-py/issues
 Project-URL: Rumble Live Stream API docs, https://rumblefaq.groovehq.com/help/how-to-use-rumble-s-live-stream-api
 Author-email: Wilbur Jaywright <zargulthewizard@outlook.com>
 License-File: LICENSE.txt
 Keywords: api,livestream,rumble,wrapper
```

