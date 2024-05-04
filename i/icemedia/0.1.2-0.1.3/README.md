# Comparing `tmp/icemedia-0.1.2.tar.gz` & `tmp/icemedia-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "icemedia-0.1.2.tar", last modified: Wed Apr 10 06:20:26 2024, max compression
+gzip compressed data, was "icemedia-0.1.3.tar", last modified: Sat May  4 21:38:19 2024, max compression
```

## Comparing `icemedia-0.1.2.tar` & `icemedia-0.1.3.tar`

### file list

```diff
@@ -1,26 +1,27 @@
-drwxrwxr-x   0 daniel    (1000) daniel    (1000)        0 2024-04-10 06:20:26.063933 icemedia-0.1.2/
--rw-rw-r--   0 daniel    (1000) daniel    (1000)    26526 2024-04-05 18:14:06.000000 icemedia-0.1.2/LICENSE
--rw-r--r--   0 daniel    (1000) daniel    (1000)     8772 2024-04-10 06:20:26.063933 icemedia-0.1.2/PKG-INFO
--rw-rw-r--   0 daniel    (1000) daniel    (1000)     8216 2024-04-06 20:31:46.000000 icemedia-0.1.2/README.md
-drwxrwxr-x   0 daniel    (1000) daniel    (1000)        0 2024-04-10 06:20:26.063933 icemedia-0.1.2/icemedia/
--rw-rw-r--   0 daniel    (1000) daniel    (1000)        0 2024-04-05 18:15:47.000000 icemedia-0.1.2/icemedia/__init__.py
--rw-rw-r--   0 daniel    (1000) daniel    (1000)     9616 2024-04-10 05:25:46.000000 icemedia-0.1.2/icemedia/iceflow.py
--rw-rw-r--   0 daniel    (1000) daniel    (1000)    43774 2024-04-06 04:20:24.000000 icemedia-0.1.2/icemedia/iceflow_server.py
--rw-rw-r--   0 daniel    (1000) daniel    (1000)     7016 2024-04-05 23:26:04.000000 icemedia-0.1.2/icemedia/jack_client_subprocess.py
--rw-rw-r--   0 daniel    (1000) daniel    (1000)    36703 2024-04-10 05:33:55.000000 icemedia-0.1.2/icemedia/jack_tools.py
--rw-rw-r--   0 daniel    (1000) daniel    (1000)    20538 2024-04-10 05:33:09.000000 icemedia-0.1.2/icemedia/jsonrpyc.py
--rw-rw-r--   0 daniel    (1000) daniel    (1000)    24337 2024-04-06 02:27:57.000000 icemedia-0.1.2/icemedia/python_mpv_jsonipc.py
--rw-rw-r--   0 daniel    (1000) daniel    (1000)    22470 2024-04-06 20:31:46.000000 icemedia-0.1.2/icemedia/sound_player.py
-drwxrwxr-x   0 daniel    (1000) daniel    (1000)        0 2024-04-10 06:20:26.063933 icemedia-0.1.2/icemedia.egg-info/
--rw-r--r--   0 daniel    (1000) daniel    (1000)     8772 2024-04-10 06:20:25.000000 icemedia-0.1.2/icemedia.egg-info/PKG-INFO
--rw-rw-r--   0 daniel    (1000) daniel    (1000)      477 2024-04-10 06:20:25.000000 icemedia-0.1.2/icemedia.egg-info/SOURCES.txt
--rw-rw-r--   0 daniel    (1000) daniel    (1000)        1 2024-04-10 06:20:25.000000 icemedia-0.1.2/icemedia.egg-info/dependency_links.txt
--rw-rw-r--   0 daniel    (1000) daniel    (1000)       21 2024-04-10 06:20:25.000000 icemedia-0.1.2/icemedia.egg-info/requires.txt
--rw-rw-r--   0 daniel    (1000) daniel    (1000)       15 2024-04-10 06:20:25.000000 icemedia-0.1.2/icemedia.egg-info/top_level.txt
--rw-rw-r--   0 daniel    (1000) daniel    (1000)       38 2024-04-10 06:20:26.063933 icemedia-0.1.2/setup.cfg
--rw-rw-r--   0 daniel    (1000) daniel    (1000)      892 2024-04-10 05:37:18.000000 icemedia-0.1.2/setup.py
-drwxrwxr-x   0 daniel    (1000) daniel    (1000)        0 2024-04-10 06:20:26.063933 icemedia-0.1.2/tests/
--rw-rw-r--   0 daniel    (1000) daniel    (1000)        0 2023-11-08 06:36:16.000000 icemedia-0.1.2/tests/__init__.py
--rw-rw-r--   0 daniel    (1000) daniel    (1000)     3037 2024-04-06 01:34:27.000000 icemedia-0.1.2/tests/testGstStability.py
--rw-rw-r--   0 daniel    (1000) daniel    (1000)      938 2024-04-06 01:34:27.000000 icemedia-0.1.2/tests/testJack.py
--rw-rw-r--   0 daniel    (1000) daniel    (1000)      231 2024-04-06 02:25:55.000000 icemedia-0.1.2/tests/test_sound_player.py
+drwxrwxr-x   0 daniel    (1000) daniel    (1000)        0 2024-05-04 21:38:19.803892 icemedia-0.1.3/
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)    26526 2024-04-05 18:14:06.000000 icemedia-0.1.3/LICENSE
+-rw-r--r--   0 daniel    (1000) daniel    (1000)     8929 2024-05-04 21:38:19.803892 icemedia-0.1.3/PKG-INFO
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)     8373 2024-05-04 21:37:29.000000 icemedia-0.1.3/README.md
+drwxrwxr-x   0 daniel    (1000) daniel    (1000)        0 2024-05-04 21:38:19.803892 icemedia-0.1.3/icemedia/
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)        0 2024-04-05 18:15:47.000000 icemedia-0.1.3/icemedia/__init__.py
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)     9616 2024-04-10 05:25:46.000000 icemedia-0.1.3/icemedia/iceflow.py
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)    44440 2024-05-04 21:30:35.000000 icemedia-0.1.3/icemedia/iceflow_server.py
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)     7016 2024-04-05 23:26:04.000000 icemedia-0.1.3/icemedia/jack_client_subprocess.py
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)    36703 2024-04-10 05:33:55.000000 icemedia-0.1.3/icemedia/jack_tools.py
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)    20538 2024-04-10 05:33:09.000000 icemedia-0.1.3/icemedia/jsonrpyc.py
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)        0 2024-04-11 23:13:16.000000 icemedia-0.1.3/icemedia/py.typed
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)    24337 2024-04-06 02:27:57.000000 icemedia-0.1.3/icemedia/python_mpv_jsonipc.py
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)    22473 2024-04-14 01:55:10.000000 icemedia-0.1.3/icemedia/sound_player.py
+drwxrwxr-x   0 daniel    (1000) daniel    (1000)        0 2024-05-04 21:38:19.803892 icemedia-0.1.3/icemedia.egg-info/
+-rw-r--r--   0 daniel    (1000) daniel    (1000)     8929 2024-05-04 21:38:19.000000 icemedia-0.1.3/icemedia.egg-info/PKG-INFO
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)      495 2024-05-04 21:38:19.000000 icemedia-0.1.3/icemedia.egg-info/SOURCES.txt
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)        1 2024-05-04 21:38:19.000000 icemedia-0.1.3/icemedia.egg-info/dependency_links.txt
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)       21 2024-05-04 21:38:19.000000 icemedia-0.1.3/icemedia.egg-info/requires.txt
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)       15 2024-05-04 21:38:19.000000 icemedia-0.1.3/icemedia.egg-info/top_level.txt
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)       38 2024-05-04 21:38:19.803892 icemedia-0.1.3/setup.cfg
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)      892 2024-05-04 21:36:44.000000 icemedia-0.1.3/setup.py
+drwxrwxr-x   0 daniel    (1000) daniel    (1000)        0 2024-05-04 21:38:19.803892 icemedia-0.1.3/tests/
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)        0 2023-11-08 06:36:16.000000 icemedia-0.1.3/tests/__init__.py
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)     3037 2024-04-06 01:34:27.000000 icemedia-0.1.3/tests/testGstStability.py
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)      938 2024-04-06 01:34:27.000000 icemedia-0.1.3/tests/testJack.py
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)      231 2024-04-06 02:25:55.000000 icemedia-0.1.3/tests/test_sound_player.py
```

### Comparing `icemedia-0.1.2/LICENSE` & `icemedia-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `icemedia-0.1.2/PKG-INFO` & `icemedia-0.1.3/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,23 +1,7 @@
-Metadata-Version: 2.1
-Name: icemedia
-Version: 0.1.2
-Summary: A GStreamer wrapper with JACK connection management
-Home-page: https://github.com/EternityForest/iceflow
-Author: Daniel Dunn
-Author-email: dannydunn@eternityforest.com
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: GNU Lesser General Public License v2 or later (LGPLv2+)
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-License-File: LICENSE
-Requires-Dist: JACK-Client
-Requires-Dist: scullery
-
 # iceflow
 More comfortable wrapper for gstreamer and JACK
 
 
 ## Install
 
 ```
@@ -179,18 +163,18 @@
 
 #### sullery.jack.start_managing()
 Start the worker thread and enable management functions
 
 
 ## icemedia.iceflow module
 
-This is a wrapper around GStreamer that handles a lot of the more obnoxious parts for you.  
-You'll need to install Gstreamer and it's bindings yourself, they are not in Pip.  
+This is a wrapper around GStreamer that handles a lot of the more obnoxious parts for you.
+You'll need to install Gstreamer and it's bindings yourself, they are not in Pip.
 
-To do this on debian-based systems, try these packages on apt, you only 
+To do this on debian-based systems, try these packages on apt, you only
 need the plugins you actually want to use. GStreamer also will use any LADSPA plugins it finds.
 
  - python3-gi
  - python3-gst-1.0
  - gstreamer1.0-plugins-good
  - gstreamer1.0-plugins-bad
  - gstreamer1.0-plugins-ugly
@@ -220,19 +204,22 @@
 time.sleep(5)
 n.stop()
 ```
 
 ### icemedia.iceflow.GStreamerPipeline
 This is the base class for making GStreamer apps
 
-#### GStreamerPipeline.add_element(elementType, name=None connect_to_output=None, connect_when_available=None, \*\*kwargs)
+#### GStreamerPipeline.add_element(elementType, name=None connect_to_output=None, connect_when_available=None, auto_insert_audio_convert=False, \*\*kwargs)
 
 Adds an element to the pipe and returns a weakref proxy. Normally, this will connect to the last added
 element, but you can explicitly pass a an object to connect to.
 
+If auto_insert_audio_convert is set, then if connecting the elements fails,
+will retry with an audioconvert element in between.
+
 if connect_when_available is True, then the elements will be connected later,
 at runtime, when the pad exists.  This is needed for some Gst elements that have dynamic pads.
 
 The `**kwargs` are used to set properties of the element.
 
 This function returns an ElementProxy.  It acts like a GStreamer element but it is actually
 a proxy object, because the actual pipeline is in a separate background process.
```

### Comparing `icemedia-0.1.2/README.md` & `icemedia-0.1.3/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,7 +1,23 @@
+Metadata-Version: 2.1
+Name: icemedia
+Version: 0.1.3
+Summary: A GStreamer wrapper with JACK connection management
+Home-page: https://github.com/EternityForest/iceflow
+Author: Daniel Dunn
+Author-email: dannydunn@eternityforest.com
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: GNU Lesser General Public License v2 or later (LGPLv2+)
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.6
+Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: JACK-Client
+Requires-Dist: scullery
+
 # iceflow
 More comfortable wrapper for gstreamer and JACK
 
 
 ## Install
 
 ```
@@ -163,18 +179,18 @@
 
 #### sullery.jack.start_managing()
 Start the worker thread and enable management functions
 
 
 ## icemedia.iceflow module
 
-This is a wrapper around GStreamer that handles a lot of the more obnoxious parts for you.  
-You'll need to install Gstreamer and it's bindings yourself, they are not in Pip.  
+This is a wrapper around GStreamer that handles a lot of the more obnoxious parts for you.
+You'll need to install Gstreamer and it's bindings yourself, they are not in Pip.
 
-To do this on debian-based systems, try these packages on apt, you only 
+To do this on debian-based systems, try these packages on apt, you only
 need the plugins you actually want to use. GStreamer also will use any LADSPA plugins it finds.
 
  - python3-gi
  - python3-gst-1.0
  - gstreamer1.0-plugins-good
  - gstreamer1.0-plugins-bad
  - gstreamer1.0-plugins-ugly
@@ -204,19 +220,22 @@
 time.sleep(5)
 n.stop()
 ```
 
 ### icemedia.iceflow.GStreamerPipeline
 This is the base class for making GStreamer apps
 
-#### GStreamerPipeline.add_element(elementType, name=None connect_to_output=None, connect_when_available=None, \*\*kwargs)
+#### GStreamerPipeline.add_element(elementType, name=None connect_to_output=None, connect_when_available=None, auto_insert_audio_convert=False, \*\*kwargs)
 
 Adds an element to the pipe and returns a weakref proxy. Normally, this will connect to the last added
 element, but you can explicitly pass a an object to connect to.
 
+If auto_insert_audio_convert is set, then if connecting the elements fails,
+will retry with an audioconvert element in between.
+
 if connect_when_available is True, then the elements will be connected later,
 at runtime, when the pad exists.  This is needed for some Gst elements that have dynamic pads.
 
 The `**kwargs` are used to set properties of the element.
 
 This function returns an ElementProxy.  It acts like a GStreamer element but it is actually
 a proxy object, because the actual pipeline is in a separate background process.
```

### Comparing `icemedia-0.1.2/icemedia/iceflow.py` & `icemedia-0.1.3/icemedia/iceflow.py`

 * *Files identical despite different names*

### Comparing `icemedia-0.1.2/icemedia/iceflow_server.py` & `icemedia-0.1.3/icemedia/iceflow_server.py`

 * *Files 2% similar despite different names*

```diff
@@ -31,19 +31,17 @@
 
 Gst.init(None)
 
 jackChannels = {}
 
 stopflag = [0]
 
-# Overridden later
-print = print
-
 
 def dummy_func(*a, **k):
+    _ = a, k
     "RPC replaces this with the thing it calls"
 
 
 rpc = [dummy_func]
 
 
 def call_rpc_if_exists(*a, **k):
@@ -284,22 +282,19 @@
                     "Could not link" + str(a) + str(b) + " reason " + str(x)
                 )
     finally:
         if unref:
             pass  # b.unref()
 
 
-def elementInfo(e):
-    r = Gst.Registry.get()  # noqa
-
-
 elementsByShortId = weakref.WeakValueDictionary()
 
 
 def Element(n, name=None):
+    _ = name
     e = Gst.ElementFactory.make(n, None)
     elementsByShortId[id(e)] = e
     if e:
         return e
     else:
         raise ValueError("No such element exists: " + n)
 
@@ -374,15 +369,15 @@
                         # Todo actually handle some errors?
                         exitSignal.append(True)
                         # After pipeline deleted, we clean up
                         if hasattr(self, "pipeline") and hasattr(self, "bus"):
                             try:
                                 with self.seeklock:
                                     self.pipeline.set_state(Gst.State.NULL)
-                            except Exception:
+                            except Exception:  # noqa
                                 pass
                             self._waitForState(Gst.State.NULL, 3600000)
 
                             raise
                         else:
                             return
 
@@ -431,16 +426,18 @@
     e.getSinks()[0].getNegotiatedCaps()
 
 
 def linkClosureMaker(
     self, src, dest, connect_when_available, eid, deleteAfterUse=False
 ):
     "This has t be outside, it can't leak a ref to self's strong reference into the closure or it may leak memory"
+    _ = src
 
     def linkFunction(element, pad, dummy):
+        _ = dummy
         s = pad.query_caps(None).to_string()
         if isinstance(connect_when_available, str):
             if connect_when_available not in s:
                 return
 
         if eid in self().waitingCallbacks:
             link(element, dest)
@@ -531,15 +528,15 @@
         self.shouldRunThread = True
         self.wasEverRunning = True
 
         self.knownThreads = {}
         self.startTime = 0
 
         def dummy(*a, **k):
-            pass
+            _ = (a, k)
 
         if realtime:
             self._syncmessage = wrfunc(
                 weakref.WeakMethod(self.syncMessage), fail_return=Gst.BusSyncReply.PASS
             )
             self.bus.set_sync_handler(self._syncmessage, 0, dummy)
         self.pollthread = None
@@ -690,26 +687,27 @@
                 if self.realtime:
                     try:
                         self.setcurrent_threadPriority(1, self.realtime)
                     except Exception:
                         log.exception("Error setting realtime priority")
             return Gst.BusSyncReply.PASS
         except Exception:
-            return Gst.BusSyncReply.PASS
             print(traceback.format_exc())
+            return Gst.BusSyncReply.PASS
 
     def makeElement(self, n, name=None):
         with self.lock:
             e = Element(n, name)
             self.elementTypesById[id(e)] = n
             self.pipeline.add(e)
             return e
 
     # Low level wrapper just for filtering out args we don't care about
     def _on_eos(self, *a, **k):
+        _ = (a, k)
         with self.lock:
             self.on_eos()
 
     def on_eos(self):
         self.on_stream_finished()
         call_rpc_if_exists("on_stream_finished", [])
 
@@ -733,14 +731,15 @@
                 if time.monotonic() - t > 10:
                     raise RuntimeError("Timeout")
 
         if not self._stopped:
             self.stop()
 
     def _on_message(self, bus, message, userdata):
+        _ = bus, userdata
         s = message.get_structure()
         if s:
             self.on_message(message.src, s.get_name(), s)
 
         return True
 
     # def appsinkhandler(self,appsink, user_data):
@@ -789,14 +788,15 @@
                 )
             if s.get_value("final"):
                 call_rpc_if_exists(
                     "onSTTMessageFinal", [str(src), s.get_value("final")]
                 )
 
     def on_error(self, bus, msg, userdata):
+        _ = bus, userdata
         with self.lock:
             logging.debug("Error {}: {}, {}".format(msg.src.name, *msg.parse_error()))
 
     def _on_segment_done(self, *a):
         with self.lock:
             self.on_segment_done()
             return True
@@ -1115,14 +1115,15 @@
         self,
         t,
         name=None,
         connect_when_available=False,
         connectWhenAvailable=False,
         connect_to_output=None,
         connectToOutput=None,
+        auto_insert_audio_convert=False,
         sidechain=False,
         **kwargs,
     ):
         # TODO: remove Legacy hack eventually
         connect_to_output = connect_to_output or connectToOutput
         connect_when_available = connect_when_available or connectWhenAvailable
         with self.lock:
@@ -1197,15 +1198,24 @@
                             eid,
                         )
 
                         self.waitingCallbacks[eid] = f
                         # Dummy 1 param because some have claimed to get segfaults without
                         connect_to_output.connect("pad-added", f, 1)
                     else:
-                        link(connect_to_output, e)
+                        try:
+                            link(connect_to_output, e)
+                        except Exception:
+                            if auto_insert_audio_convert:
+                                c = self.add_element(
+                                    "audioconvert", connect_to_output=connect_to_output
+                                )
+                                link(c, e)
+                            else:
+                                raise
 
             # Sidechain means don't set this element as the
             # automatic thing that the next entry links to
             if not sidechain:
                 self.elements.append(e)
             else:
                 self.sidechainElements.append(e)
@@ -1312,22 +1322,28 @@
 
 def main():
     global gstp
 
     gstp = GStreamerPipeline()
     # Replace the dummy we put there for the linter
     rpc[0] = jsonrpyc.RPC(target=gstp)
-    # def print(*a):
-    #     rpc[0]("print", [str(a)])
 
     while 1:
         time.sleep(1)
 
         if (not check_pid(ppid)) or stopflag[0]:
+            try:
+                gstp.stop()
+            except Exception:  # noqa
+                pass
             sys.exit()
 
         if not os.getppid() == ppid:
+            try:
+                gstp.stop()
+            except Exception:  # noqa
+                pass
             return
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `icemedia-0.1.2/icemedia/jack_client_subprocess.py` & `icemedia-0.1.3/icemedia/jack_client_subprocess.py`

 * *Files identical despite different names*

### Comparing `icemedia-0.1.2/icemedia/jack_tools.py` & `icemedia-0.1.3/icemedia/jack_tools.py`

 * *Files identical despite different names*

### Comparing `icemedia-0.1.2/icemedia/jsonrpyc.py` & `icemedia-0.1.3/icemedia/jsonrpyc.py`

 * *Files identical despite different names*

### Comparing `icemedia-0.1.2/icemedia/python_mpv_jsonipc.py` & `icemedia-0.1.3/icemedia/python_mpv_jsonipc.py`

 * *Files identical despite different names*

### Comparing `icemedia-0.1.2/icemedia/sound_player.py` & `icemedia-0.1.3/icemedia/sound_player.py`

 * *Files 2% similar despite different names*

```diff
@@ -215,15 +215,15 @@
 
 
 class PlayerHolder(object):
     def __init__(self, p: MPV) -> None:
         self.player = p
         self.usesCounter = 0
         self.conf = [0]
-        self.isConfigured = False
+        self.is_configured = False
         self.lastvol = -99089798
         self.conf_speed = 1
         self.loop_conf = -1
         self.alreadyMadeReplacement = False
         self.lastjack = "hgfdxcghjkufdszcxghjkuyfgdx"
 
 
@@ -269,22 +269,22 @@
             with objectPoolLock:
                 if len(objectPool):
                     self.player = objectPool.pop()
                 else:
                     self.player = PlayerHolder(MPV())
 
             # Avoid somewhat slow RPC calls if we can
-            if not self.player.isConfigured:
+            if not self.player.is_configured:
                 cname = "kplayer" + str(time.monotonic()) + "_out"
                 self.player.player.vid = "no"
                 self.player.player.keep_open = "yes"
                 self.player.player.ao = "jack,pulse,alsa"
                 self.player.player.jack_name = cname
                 self.player.player.gapless_audio = "weak"
-                self.player.player.isConfigured = True
+                self.player.player.is_configured = True
 
             if speed != self.player.conf_speed:
                 self.player.player.audio_pitch_correction = False
                 self.player.player.speed = speed
 
             if not loop == self.player.loop_conf:
                 # For legavy reasons some stuff used tens of millions instead of actual infinite loop.
```

### Comparing `icemedia-0.1.2/icemedia.egg-info/PKG-INFO` & `icemedia-0.1.3/icemedia.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: icemedia
-Version: 0.1.2
+Version: 0.1.3
 Summary: A GStreamer wrapper with JACK connection management
 Home-page: https://github.com/EternityForest/iceflow
 Author: Daniel Dunn
 Author-email: dannydunn@eternityforest.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v2 or later (LGPLv2+)
 Classifier: Operating System :: OS Independent
@@ -179,18 +179,18 @@
 
 #### sullery.jack.start_managing()
 Start the worker thread and enable management functions
 
 
 ## icemedia.iceflow module
 
-This is a wrapper around GStreamer that handles a lot of the more obnoxious parts for you.  
-You'll need to install Gstreamer and it's bindings yourself, they are not in Pip.  
+This is a wrapper around GStreamer that handles a lot of the more obnoxious parts for you.
+You'll need to install Gstreamer and it's bindings yourself, they are not in Pip.
 
-To do this on debian-based systems, try these packages on apt, you only 
+To do this on debian-based systems, try these packages on apt, you only
 need the plugins you actually want to use. GStreamer also will use any LADSPA plugins it finds.
 
  - python3-gi
  - python3-gst-1.0
  - gstreamer1.0-plugins-good
  - gstreamer1.0-plugins-bad
  - gstreamer1.0-plugins-ugly
@@ -220,19 +220,22 @@
 time.sleep(5)
 n.stop()
 ```
 
 ### icemedia.iceflow.GStreamerPipeline
 This is the base class for making GStreamer apps
 
-#### GStreamerPipeline.add_element(elementType, name=None connect_to_output=None, connect_when_available=None, \*\*kwargs)
+#### GStreamerPipeline.add_element(elementType, name=None connect_to_output=None, connect_when_available=None, auto_insert_audio_convert=False, \*\*kwargs)
 
 Adds an element to the pipe and returns a weakref proxy. Normally, this will connect to the last added
 element, but you can explicitly pass a an object to connect to.
 
+If auto_insert_audio_convert is set, then if connecting the elements fails,
+will retry with an audioconvert element in between.
+
 if connect_when_available is True, then the elements will be connected later,
 at runtime, when the pad exists.  This is needed for some Gst elements that have dynamic pads.
 
 The `**kwargs` are used to set properties of the element.
 
 This function returns an ElementProxy.  It acts like a GStreamer element but it is actually
 a proxy object, because the actual pipeline is in a separate background process.
```

### Comparing `icemedia-0.1.2/setup.py` & `icemedia-0.1.3/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="icemedia",
-    version="0.1.2",
+    version="0.1.3",
     author="Daniel Dunn",
     author_email="dannydunn@eternityforest.com",
     description="A GStreamer wrapper with JACK connection management",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/EternityForest/iceflow",
     packages=setuptools.find_packages(),
```

### Comparing `icemedia-0.1.2/tests/testGstStability.py` & `icemedia-0.1.3/tests/testGstStability.py`

 * *Files identical despite different names*

### Comparing `icemedia-0.1.2/tests/testJack.py` & `icemedia-0.1.3/tests/testJack.py`

 * *Files identical despite different names*

