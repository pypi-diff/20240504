# Comparing `tmp/mpyg321-2.1.1.tar.gz` & `tmp/mpyg321-2.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mpyg321-2.1.1.tar", last modified: Thu Jan  5 01:20:13 2023, max compression
+gzip compressed data, was "mpyg321-2.2.0.tar", last modified: Sat May  4 21:42:37 2024, max compression
```

## Comparing `mpyg321-2.1.1.tar` & `mpyg321-2.2.0.tar`

### file list

```diff
@@ -1,20 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-05 01:20:13.444287 mpyg321-2.1.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-01-05 01:20:03.000000 mpyg321-2.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2869 2023-01-05 01:20:13.444287 mpyg321-2.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2446 2023-01-05 01:20:03.000000 mpyg321-2.1.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-05 01:20:13.444287 mpyg321-2.1.1/mpyg321/
--rw-r--r--   0 runner    (1001) docker     (123)     7005 2023-01-05 01:20:03.000000 mpyg321-2.1.1/mpyg321/BasePlayer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1777 2023-01-05 01:20:03.000000 mpyg321-2.1.1/mpyg321/MPyg123Player.py
--rw-r--r--   0 runner    (1001) docker     (123)      790 2023-01-05 01:20:03.000000 mpyg321-2.1.1/mpyg321/MPyg321Player.py
--rw-r--r--   0 runner    (1001) docker     (123)      809 2023-01-05 01:20:03.000000 mpyg321-2.1.1/mpyg321/MpygError.py
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-01-05 01:20:03.000000 mpyg321-2.1.1/mpyg321/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3040 2023-01-05 01:20:03.000000 mpyg321-2.1.1/mpyg321/consts.py
--rw-r--r--   0 runner    (1001) docker     (123)      296 2023-01-05 01:20:03.000000 mpyg321-2.1.1/mpyg321/mpyg321.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-05 01:20:13.444287 mpyg321-2.1.1/mpyg321.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2869 2023-01-05 01:20:13.000000 mpyg321-2.1.1/mpyg321.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      330 2023-01-05 01:20:13.000000 mpyg321-2.1.1/mpyg321.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-05 01:20:13.000000 mpyg321-2.1.1/mpyg321.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-01-05 01:20:13.000000 mpyg321-2.1.1/mpyg321.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-01-05 01:20:13.000000 mpyg321-2.1.1/mpyg321.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-01-05 01:20:13.444287 mpyg321-2.1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      667 2023-01-05 01:20:03.000000 mpyg321-2.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 21:42:37.405925 mpyg321-2.2.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-05-04 21:42:33.000000 mpyg321-2.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2892 2024-05-04 21:42:37.405925 mpyg321-2.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2446 2024-05-04 21:42:33.000000 mpyg321-2.2.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 21:42:37.405925 mpyg321-2.2.0/mpyg321/
+-rw-r--r--   0 runner    (1001) docker     (127)     8978 2024-05-04 21:42:33.000000 mpyg321-2.2.0/mpyg321/BasePlayer.py
+-rw-r--r--   0 runner    (1001) docker     (127)      399 2024-05-04 21:42:33.000000 mpyg321-2.2.0/mpyg321/EventContext.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2064 2024-05-04 21:42:33.000000 mpyg321-2.2.0/mpyg321/MPyg123Player.py
+-rw-r--r--   0 runner    (1001) docker     (127)      838 2024-05-04 21:42:33.000000 mpyg321-2.2.0/mpyg321/MPyg321Player.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1083 2024-05-04 21:42:33.000000 mpyg321-2.2.0/mpyg321/MpygError.py
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-04 21:42:33.000000 mpyg321-2.2.0/mpyg321/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2995 2024-05-04 21:42:33.000000 mpyg321-2.2.0/mpyg321/consts.py
+-rw-r--r--   0 runner    (1001) docker     (127)      296 2024-05-04 21:42:33.000000 mpyg321-2.2.0/mpyg321/mpyg321.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 21:42:37.405925 mpyg321-2.2.0/mpyg321.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2892 2024-05-04 21:42:37.000000 mpyg321-2.2.0/mpyg321.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      354 2024-05-04 21:42:37.000000 mpyg321-2.2.0/mpyg321.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-04 21:42:37.000000 mpyg321-2.2.0/mpyg321.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-04 21:42:37.000000 mpyg321-2.2.0/mpyg321.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-04 21:42:37.000000 mpyg321-2.2.0/mpyg321.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-04 21:42:37.405925 mpyg321-2.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      667 2024-05-04 21:42:33.000000 mpyg321-2.2.0/setup.py
```

### Comparing `mpyg321-2.1.1/LICENSE` & `mpyg321-2.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `mpyg321-2.1.1/PKG-INFO` & `mpyg321-2.2.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 Metadata-Version: 2.1
 Name: mpyg321
-Version: 2.1.1
+Version: 2.2.0
 Summary: mpg321 wrapper for python - command line music player
 Home-page: https://github.com/4br3mm0rd/mpyg321
 Author: 4br3mm0rd
 Author-email: 4br3mm0rd@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: pexpect
 
 [![Downloads](https://pepy.tech/badge/mpyg321)](https://pepy.tech/project/mpyg321)
 [![Downloads](https://pepy.tech/badge/mpyg321/month)](https://pepy.tech/project/mpyg321)
 [![Downloads](https://pepy.tech/badge/mpyg321/week)](https://pepy.tech/project/mpyg321)
 # mpyg321
 
 mpyg321 is a simple python wrapper for mpg321 and mpg123. It allows you to easily play mp3 sounds in python, do basic operations on the music and implement callbacks for events like the end of a sound.
```

### Comparing `mpyg321-2.1.1/README.md` & `mpyg321-2.2.0/README.md`

 * *Files identical despite different names*

### Comparing `mpyg321-2.1.1/mpyg321/BasePlayer.py` & `mpyg321-2.2.0/mpyg321/BasePlayer.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,36 +1,45 @@
 """
 Mpyg BasePlayer base class
 This class contains all the functions that are common
 both to mpg321 and mpg123.
 All the players implement this base class and add their
 specific feature.
 """
-import pexpect
+
 import subprocess
 from threading import Thread
-from .MpygError import *
+
+import pexpect
+
 from .consts import *
+from .EventContext import *
+from .MpygError import *
 
 
 class BasePlayer:
     """Base class for players"""
+
     player = None
     status = None
     output_processor = None
     song_path = ""
     loop = False
     performance_mode = True
-    suitable_versions = []        # mpg123 and/or mpg321 - set inside subclass
-    default_player = None         # mpg123 or mpg321 - set inside subclass
-    player_version = None         # defined inside check_player
+    suitable_versions = []  # mpg123 and/or mpg321 - set inside subclass
+    default_player = None  # mpg123 or mpg321 - set inside subclass
+    player_version = None  # defined inside check_player
     mpg_outs = []
+    _events = {}
 
-    def __init__(self, player=None, audiodevice=None, performance_mode=True, custom_args=""):
+    def __init__(
+        self, player=None, audiodevice=None, performance_mode=True, custom_args=""
+    ):
         """Builds the player and creates the callbacks"""
+        self._events = {e: [] for e in MPyg321Events}
         self.set_player(player, audiodevice, custom_args)
         self.output_processor = Thread(target=self.process_output)
         self.output_processor.daemon = True
         self.performance_mode = performance_mode
         self.output_processor.start()
 
     def check_player(self, player):
@@ -40,19 +49,21 @@
             output = subprocess.check_output([cmd, "--version"])
             for version in self.suitable_versions:
                 if version in str(output):
                     self.player_version = version
             if self.player_version is None:
                 raise MPygPlayerNotFoundError(
                     """No suitable player found: you might be using the wrong \
-player (Mpyg321Player or Mpyg123Player)""")
+player (Mpyg321Player or Mpyg123Player)"""
+                )
         except subprocess.SubprocessError:
             raise MPygPlayerNotFoundError(
                 """No suitable player found: you might need to install
-                mpg123""")
+                mpg123"""
+            )
 
     def set_player(self, player, audiodevice, custom_args):
         """Sets the player"""
         if player is None:
             player = self.default_player
         self.check_player(player)
         args = " " + custom_args if custom_args != "" else ""
@@ -61,14 +72,47 @@
         self.player = pexpect.spawn(str(player) + " " + args)
         self.player.delaybeforesend = None
         self.status = PlayerStatus.INSTANCIATED
         # Setting extended mpg_outs for version specific behaviors
         self.mpg_outs = mpg_outs.copy()
         self.mpg_outs.extend(mpg_outs_ext[self.player_version])
 
+    def on(self, event_name):
+        """Decorator to register event callbacks."""
+
+        def decorator(func):
+            if event_name not in self._events:
+                raise MPygUnknownEventNameError(
+                    f"Subscribed callback to a non existing event {event_name}."
+                )
+            self._events[event_name].append(func)
+            return func
+
+        return decorator
+
+    def subscribe_event(self, event_name, callback):
+        if event_name not in self._events:
+            raise MPygUnknownEventNameError(
+                f"Subscribed callback to a non existing event {event_name}."
+            )
+        self._events[event_name].append(callback)
+
+    def _trigger_event(self, event_name, context=None):
+        """Trigger all callbacks associated with an event."""
+        if context is None:
+            context = MPyg321EventContext(self)
+        if event_name in self._events:
+            for callback in self._events[event_name]:
+                try:
+                    callback(context)
+                except Exception:
+                    raise MPygEventListenerError(
+                        "Error while executiong event callback"
+                    )
+
     def process_output(self):
         """Parses the output"""
         mpg_codes = [v["mpg_code"] for v in self.mpg_outs]
         while True:
             index = self.player.expect(mpg_codes)
             action = self.mpg_outs[index]["action"]
             if action == "music_stop":
@@ -105,14 +149,15 @@
             self.player.sendline("PAUSE")
             self.status = PlayerStatus.PAUSED
 
     def resume(self):
         """Resume the player"""
         if self.status == PlayerStatus.PAUSED:
             self.player.sendline("PAUSE")
+            self._trigger_event(MPyg321Events.USER_RESUME)
             self.on_user_resume()
 
     def stop(self):
         """Stops the player"""
         self.player.sendline("STOP")
         self.status = PlayerStatus.STOPPING
 
@@ -129,68 +174,78 @@
         """Process errors encountered by the player"""
         output = self.player.readline().decode("utf-8")
 
         # Check error in list of errors
         for mpg_error in mpg_errors:
             if mpg_error["message"] in output:
                 action = mpg_error["action"]
+                context = MPyg321ErrorContext(self, action, output)
+                self._trigger_event(MPyg321Events.ERROR, context)
                 if action == "generic_error":
                     raise MPygError(output)
                 if action == "file_error":
                     raise MPygFileError(output)
                 if action == "command_error":
                     raise MPygCommandError(output)
                 if action == "argument_error":
                     raise MPygArgumentError(output)
                 if action == "eq_error":
                     raise MPygEQError
                 if action == "seek_error":
                     raise MPygSeekError
 
         # Some other error occurred
+        context = MPyg321ErrorContext(self, "unknown_error", output)
+        self._trigger_event(MPyg321Events.ERROR, context)
         raise MPygError(output)
 
     def set_song(self, path):
         """song_path setter"""
         self.song_path = path
 
     def set_loop(self, loop):
-        """"loop setter"""
+        """loop setter"""
         self.loop = loop
 
     # # # Internal Callbacks # # #
     def on_music_stop_int(self):
         """Internal callback when the music is stopped"""
         if self.status == PlayerStatus.STOPPING:
             self.on_user_stop_int()
             self.status = PlayerStatus.STOPPED
         else:
             self.on_end_of_song_int()
 
     def on_user_stop_int(self):
         """Internal callback when the user stops the music."""
+        self._trigger_event(MPyg321Events.ANY_STOP)
         self.on_any_stop()
+        self._trigger_event(MPyg321Events.USER_STOP)
         self.on_user_stop()
 
     def on_user_pause_int(self):
         """Internal callback when user pauses the music"""
+        self._trigger_event(MPyg321Events.ANY_STOP)
         self.on_any_stop()
+        self._trigger_event(MPyg321Events.USER_PAUSE)
         self.on_user_pause()
 
     def on_user_start_or_resume_int(self):
         """Internal callback when user resumes the music"""
         self.status = PlayerStatus.PLAYING
 
     def on_end_of_song_int(self):
         """Internal callback when the song ends"""
-        if(self.loop):
+        if self.loop:
             self.play()
         else:
             # The music doesn't stop if it is looped
+            self._trigger_event(MPyg321Events.ANY_STOP)
             self.on_any_stop()
+        self._trigger_event(MPyg321Events.MUSIC_END)
         self.on_music_end()
 
     # # # Public Callbacks # # #
     def on_any_stop(self):
         """Callback when the music stops for any reason"""
         pass
 
@@ -201,11 +256,11 @@
     def on_user_resume(self):
         """Callback when user resumes the music"""
         pass
 
     def on_user_stop(self):
         """Callback when user stops music"""
         pass
- 
+
     def on_music_end(self):
         """Callback when music ends"""
         pass
```

### Comparing `mpyg321-2.1.1/mpyg321.egg-info/PKG-INFO` & `mpyg321-2.2.0/mpyg321.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 Metadata-Version: 2.1
 Name: mpyg321
-Version: 2.1.1
+Version: 2.2.0
 Summary: mpg321 wrapper for python - command line music player
 Home-page: https://github.com/4br3mm0rd/mpyg321
 Author: 4br3mm0rd
 Author-email: 4br3mm0rd@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: pexpect
 
 [![Downloads](https://pepy.tech/badge/mpyg321)](https://pepy.tech/project/mpyg321)
 [![Downloads](https://pepy.tech/badge/mpyg321/month)](https://pepy.tech/project/mpyg321)
 [![Downloads](https://pepy.tech/badge/mpyg321/week)](https://pepy.tech/project/mpyg321)
 # mpyg321
 
 mpyg321 is a simple python wrapper for mpg321 and mpg123. It allows you to easily play mp3 sounds in python, do basic operations on the music and implement callbacks for events like the end of a sound.
```

### Comparing `mpyg321-2.1.1/setup.py` & `mpyg321-2.2.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="mpyg321",
-    version="2.1.1",
+    version="2.2.0",
     author="4br3mm0rd",
     author_email="4br3mm0rd@gmail.com",
     description="mpg321 wrapper for python - command line music player",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/4br3mm0rd/mpyg321",
     packages=setuptools.find_packages(),
```

