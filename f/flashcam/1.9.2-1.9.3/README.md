# Comparing `tmp/flashcam-1.9.2.tar.gz` & `tmp/flashcam-1.9.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flashcam-1.9.2.tar", last modified: Sun Apr 14 19:24:55 2024, max compression
+gzip compressed data, was "flashcam-1.9.3.tar", last modified: Sat Apr 20 18:27:34 2024, max compression
```

## Comparing `flashcam-1.9.2.tar` & `flashcam-1.9.3.tar`

### file list

```diff
@@ -1,50 +1,50 @@
-drwxrwxr-x   0 ojr       (1000) ojr       (1000)        0 2024-04-14 19:24:55.200695 flashcam-1.9.2/
--rw-r--r--   0 ojr       (1000) ojr       (1000)     1582 2024-04-14 19:24:55.200695 flashcam-1.9.2/PKG-INFO
--rw-rw-r--   0 ojr       (1000) ojr       (1000)      901 2024-04-14 19:24:51.000000 flashcam-1.9.2/README.md
-drwxrwxr-x   0 ojr       (1000) ojr       (1000)        0 2024-04-14 19:24:55.192695 flashcam-1.9.2/bin/
--rwxrwxr-x   0 ojr       (1000) ojr       (1000)    28426 2024-04-14 18:40:50.000000 flashcam-1.9.2/bin/flashcam
--rwxrwxr-x   0 ojr       (1000) ojr       (1000)      150 2023-11-02 08:34:00.000000 flashcam-1.9.2/bin/flashcam_join
--rwxrwxr-x   0 ojr       (1000) ojr       (1000)     3406 2023-11-02 08:34:00.000000 flashcam-1.9.2/bin/flashcam_org
--rwxrwxr-x   0 ojr       (1000) ojr       (1000)      865 2023-11-02 08:34:00.000000 flashcam-1.9.2/bin/flashcam_rep
--rwxrwxr-x   0 ojr       (1000) ojr       (1000)      679 2024-02-27 15:50:11.000000 flashcam-1.9.2/bin/flashcamg
-drwxrwxr-x   0 ojr       (1000) ojr       (1000)        0 2024-04-14 19:24:55.196695 flashcam-1.9.2/flashcam/
--rwxrwxr-x   0 ojr       (1000) ojr       (1000)      249 2023-11-02 08:34:00.000000 flashcam-1.9.2/flashcam/__init__.py
--rwxrwxr-x   0 ojr       (1000) ojr       (1000)     5401 2024-03-11 10:00:57.000000 flashcam-1.9.2/flashcam/base_camera2.py
--rwxrwxr-x   0 ojr       (1000) ojr       (1000)     8850 2024-03-08 14:33:40.000000 flashcam-1.9.2/flashcam/config.py
-drwxrwxr-x   0 ojr       (1000) ojr       (1000)        0 2024-04-14 19:24:55.200695 flashcam-1.9.2/flashcam/data/
--rw-rw-r--   0 ojr       (1000) ojr       (1000)    24159 2023-11-02 08:34:00.000000 flashcam-1.9.2/flashcam/data/BEAM_OFF.jpg
--rw-rw-r--   0 ojr       (1000) ojr       (1000)    27944 2023-11-02 08:34:00.000000 flashcam-1.9.2/flashcam/data/BEAM_ON_.jpg
--rw-rw-r--   0 ojr       (1000) ojr       (1000)    27715 2023-11-02 08:34:00.000000 flashcam-1.9.2/flashcam/data/DET_NRDY.jpg
--rw-rw-r--   0 ojr       (1000) ojr       (1000)    27483 2023-11-02 08:34:00.000000 flashcam-1.9.2/flashcam/data/DET_RDY_.jpg
--rw-rw-r--   0 ojr       (1000) ojr       (1000)    34404 2023-11-02 08:34:00.000000 flashcam-1.9.2/flashcam/data/digital-7.mono.ttf
--rw-rw-r--   0 ojr       (1000) ojr       (1000)    34360 2023-11-02 08:34:00.000000 flashcam-1.9.2/flashcam/data/digital-7.regular.ttf
--rw-rw-r--   0 ojr       (1000) ojr       (1000)    19991 2023-11-02 08:34:00.000000 flashcam-1.9.2/flashcam/data/monoskop.jpg
--rw-rw-r--   0 ojr       (1000) ojr       (1000)     7865 2023-11-02 08:34:00.000000 flashcam-1.9.2/flashcam/data/pattern_acircles.png
--rw-rw-r--   0 ojr       (1000) ojr       (1000)    22255 2023-11-02 08:34:00.000000 flashcam-1.9.2/flashcam/data/pattern_chessboard.png
--rw-rw-r--   0 ojr       (1000) ojr       (1000)    12496 2023-11-02 08:34:00.000000 flashcam-1.9.2/flashcam/data/small_pixel.ttf
--rw-rw-r--   0 ojr       (1000) ojr       (1000)    59930 2023-11-02 08:34:00.000000 flashcam-1.9.2/flashcam/data/win_rain.jpg
--rw-rw-r--   0 ojr       (1000) ojr       (1000)    91079 2023-11-02 08:34:00.000000 flashcam-1.9.2/flashcam/data/win_skull.jpg
--rw-rw-r--   0 ojr       (1000) ojr       (1000)    76270 2023-11-02 08:34:00.000000 flashcam-1.9.2/flashcam/data/win_storm.jpg
--rw-rw-r--   0 ojr       (1000) ojr       (1000)    61604 2023-11-02 08:34:00.000000 flashcam-1.9.2/flashcam/data/win_winter.jpg
--rw-rw-r--   0 ojr       (1000) ojr       (1000)    72731 2023-11-02 08:34:00.000000 flashcam-1.9.2/flashcam/data/windows.jpg
--rwxrwxr-x   0 ojr       (1000) ojr       (1000)     4173 2023-11-02 08:34:00.000000 flashcam-1.9.2/flashcam/direct.py
--rwxrwxr-x   0 ojr       (1000) ojr       (1000)     4572 2023-11-02 08:34:00.000000 flashcam-1.9.2/flashcam/izmq_receiver.py
--rwxrwxr-x   0 ojr       (1000) ojr       (1000)     4635 2024-03-08 14:33:40.000000 flashcam-1.9.2/flashcam/mmapwr.py
--rwxrwxr-x   0 ojr       (1000) ojr       (1000)    50705 2024-04-02 14:16:21.000000 flashcam-1.9.2/flashcam/real_camera.py
--rw-rw-r--   0 ojr       (1000) ojr       (1000)    43977 2024-04-02 04:35:37.000000 flashcam-1.9.2/flashcam/stream_enhancer.py
--rwxrwxr-x   0 ojr       (1000) ojr       (1000)    86593 2024-04-02 23:52:20.000000 flashcam-1.9.2/flashcam/uniwrec.py
--rw-rw-r--   0 ojr       (1000) ojr       (1000)     5092 2024-04-02 23:14:00.000000 flashcam-1.9.2/flashcam/uniwrec_io.py
--rw-rw-r--   0 ojr       (1000) ojr       (1000)     5142 2024-04-02 22:19:28.000000 flashcam-1.9.2/flashcam/uniwrec_keys.py
--rw-rw-r--   0 ojr       (1000) ojr       (1000)    16073 2024-04-02 23:42:21.000000 flashcam-1.9.2/flashcam/uniwrec_manip.py
--rwxrwxr-x   0 ojr       (1000) ojr       (1000)    13894 2024-04-02 19:22:46.000000 flashcam-1.9.2/flashcam/usbcheck.py
--rwxrwxr-x   0 ojr       (1000) ojr       (1000)    36471 2023-11-02 08:59:16.000000 flashcam-1.9.2/flashcam/v4lc.py
--rwxrwxr-x   0 ojr       (1000) ojr       (1000)       20 2024-04-14 19:24:54.000000 flashcam-1.9.2/flashcam/version.py
--rwxrwxr-x   0 ojr       (1000) ojr       (1000)    42054 2024-04-14 19:24:43.000000 flashcam-1.9.2/flashcam/web.py
-drwxrwxr-x   0 ojr       (1000) ojr       (1000)        0 2024-04-14 19:24:55.200695 flashcam-1.9.2/flashcam.egg-info/
--rw-r--r--   0 ojr       (1000) ojr       (1000)     1582 2024-04-14 19:24:54.000000 flashcam-1.9.2/flashcam.egg-info/PKG-INFO
--rw-rw-r--   0 ojr       (1000) ojr       (1000)     1049 2024-04-14 19:24:55.000000 flashcam-1.9.2/flashcam.egg-info/SOURCES.txt
--rw-rw-r--   0 ojr       (1000) ojr       (1000)        1 2024-04-14 19:24:54.000000 flashcam-1.9.2/flashcam.egg-info/dependency_links.txt
--rw-rw-r--   0 ojr       (1000) ojr       (1000)      165 2024-04-14 19:24:54.000000 flashcam-1.9.2/flashcam.egg-info/requires.txt
--rw-rw-r--   0 ojr       (1000) ojr       (1000)        9 2024-04-14 19:24:54.000000 flashcam-1.9.2/flashcam.egg-info/top_level.txt
--rw-rw-r--   0 ojr       (1000) ojr       (1000)       38 2024-04-14 19:24:55.200695 flashcam-1.9.2/setup.cfg
--rwxrwxr-x   0 ojr       (1000) ojr       (1000)     2275 2023-11-02 08:34:00.000000 flashcam-1.9.2/setup.py
+drwxrwxr-x   0 ojr       (1000) ojr       (1000)        0 2024-04-20 18:27:34.904369 flashcam-1.9.3/
+-rw-r--r--   0 ojr       (1000) ojr       (1000)     1582 2024-04-20 18:27:34.904369 flashcam-1.9.3/PKG-INFO
+-rw-rw-r--   0 ojr       (1000) ojr       (1000)      901 2024-04-20 18:27:32.000000 flashcam-1.9.3/README.md
+drwxrwxr-x   0 ojr       (1000) ojr       (1000)        0 2024-04-20 18:27:34.896369 flashcam-1.9.3/bin/
+-rwxrwxr-x   0 ojr       (1000) ojr       (1000)    28426 2024-04-14 18:40:50.000000 flashcam-1.9.3/bin/flashcam
+-rwxrwxr-x   0 ojr       (1000) ojr       (1000)      150 2023-11-02 08:34:00.000000 flashcam-1.9.3/bin/flashcam_join
+-rwxrwxr-x   0 ojr       (1000) ojr       (1000)     3406 2023-11-02 08:34:00.000000 flashcam-1.9.3/bin/flashcam_org
+-rwxrwxr-x   0 ojr       (1000) ojr       (1000)      865 2023-11-02 08:34:00.000000 flashcam-1.9.3/bin/flashcam_rep
+-rwxrwxr-x   0 ojr       (1000) ojr       (1000)      679 2024-02-27 15:50:11.000000 flashcam-1.9.3/bin/flashcamg
+drwxrwxr-x   0 ojr       (1000) ojr       (1000)        0 2024-04-20 18:27:34.900369 flashcam-1.9.3/flashcam/
+-rwxrwxr-x   0 ojr       (1000) ojr       (1000)      249 2023-11-02 08:34:00.000000 flashcam-1.9.3/flashcam/__init__.py
+-rwxrwxr-x   0 ojr       (1000) ojr       (1000)     5904 2024-04-20 18:27:19.000000 flashcam-1.9.3/flashcam/base_camera2.py
+-rwxrwxr-x   0 ojr       (1000) ojr       (1000)     8850 2024-03-08 14:33:40.000000 flashcam-1.9.3/flashcam/config.py
+drwxrwxr-x   0 ojr       (1000) ojr       (1000)        0 2024-04-20 18:27:34.900369 flashcam-1.9.3/flashcam/data/
+-rw-rw-r--   0 ojr       (1000) ojr       (1000)    24159 2023-11-02 08:34:00.000000 flashcam-1.9.3/flashcam/data/BEAM_OFF.jpg
+-rw-rw-r--   0 ojr       (1000) ojr       (1000)    27944 2023-11-02 08:34:00.000000 flashcam-1.9.3/flashcam/data/BEAM_ON_.jpg
+-rw-rw-r--   0 ojr       (1000) ojr       (1000)    27715 2023-11-02 08:34:00.000000 flashcam-1.9.3/flashcam/data/DET_NRDY.jpg
+-rw-rw-r--   0 ojr       (1000) ojr       (1000)    27483 2023-11-02 08:34:00.000000 flashcam-1.9.3/flashcam/data/DET_RDY_.jpg
+-rw-rw-r--   0 ojr       (1000) ojr       (1000)    34404 2023-11-02 08:34:00.000000 flashcam-1.9.3/flashcam/data/digital-7.mono.ttf
+-rw-rw-r--   0 ojr       (1000) ojr       (1000)    34360 2023-11-02 08:34:00.000000 flashcam-1.9.3/flashcam/data/digital-7.regular.ttf
+-rw-rw-r--   0 ojr       (1000) ojr       (1000)    19991 2023-11-02 08:34:00.000000 flashcam-1.9.3/flashcam/data/monoskop.jpg
+-rw-rw-r--   0 ojr       (1000) ojr       (1000)     7865 2023-11-02 08:34:00.000000 flashcam-1.9.3/flashcam/data/pattern_acircles.png
+-rw-rw-r--   0 ojr       (1000) ojr       (1000)    22255 2023-11-02 08:34:00.000000 flashcam-1.9.3/flashcam/data/pattern_chessboard.png
+-rw-rw-r--   0 ojr       (1000) ojr       (1000)    12496 2023-11-02 08:34:00.000000 flashcam-1.9.3/flashcam/data/small_pixel.ttf
+-rw-rw-r--   0 ojr       (1000) ojr       (1000)    59930 2023-11-02 08:34:00.000000 flashcam-1.9.3/flashcam/data/win_rain.jpg
+-rw-rw-r--   0 ojr       (1000) ojr       (1000)    91079 2023-11-02 08:34:00.000000 flashcam-1.9.3/flashcam/data/win_skull.jpg
+-rw-rw-r--   0 ojr       (1000) ojr       (1000)    76270 2023-11-02 08:34:00.000000 flashcam-1.9.3/flashcam/data/win_storm.jpg
+-rw-rw-r--   0 ojr       (1000) ojr       (1000)    61604 2023-11-02 08:34:00.000000 flashcam-1.9.3/flashcam/data/win_winter.jpg
+-rw-rw-r--   0 ojr       (1000) ojr       (1000)    72731 2023-11-02 08:34:00.000000 flashcam-1.9.3/flashcam/data/windows.jpg
+-rwxrwxr-x   0 ojr       (1000) ojr       (1000)     4173 2023-11-02 08:34:00.000000 flashcam-1.9.3/flashcam/direct.py
+-rwxrwxr-x   0 ojr       (1000) ojr       (1000)     4572 2023-11-02 08:34:00.000000 flashcam-1.9.3/flashcam/izmq_receiver.py
+-rwxrwxr-x   0 ojr       (1000) ojr       (1000)     4635 2024-03-08 14:33:40.000000 flashcam-1.9.3/flashcam/mmapwr.py
+-rwxrwxr-x   0 ojr       (1000) ojr       (1000)    51351 2024-04-20 18:27:19.000000 flashcam-1.9.3/flashcam/real_camera.py
+-rw-rw-r--   0 ojr       (1000) ojr       (1000)    43977 2024-04-02 04:35:37.000000 flashcam-1.9.3/flashcam/stream_enhancer.py
+-rwxrwxr-x   0 ojr       (1000) ojr       (1000)    86593 2024-04-02 23:52:20.000000 flashcam-1.9.3/flashcam/uniwrec.py
+-rw-rw-r--   0 ojr       (1000) ojr       (1000)     5092 2024-04-02 23:14:00.000000 flashcam-1.9.3/flashcam/uniwrec_io.py
+-rw-rw-r--   0 ojr       (1000) ojr       (1000)     5142 2024-04-02 22:19:28.000000 flashcam-1.9.3/flashcam/uniwrec_keys.py
+-rw-rw-r--   0 ojr       (1000) ojr       (1000)    16073 2024-04-02 23:42:21.000000 flashcam-1.9.3/flashcam/uniwrec_manip.py
+-rwxrwxr-x   0 ojr       (1000) ojr       (1000)    13894 2024-04-02 19:22:46.000000 flashcam-1.9.3/flashcam/usbcheck.py
+-rwxrwxr-x   0 ojr       (1000) ojr       (1000)    36471 2023-11-02 08:59:16.000000 flashcam-1.9.3/flashcam/v4lc.py
+-rwxrwxr-x   0 ojr       (1000) ojr       (1000)       20 2024-04-20 18:27:34.000000 flashcam-1.9.3/flashcam/version.py
+-rwxrwxr-x   0 ojr       (1000) ojr       (1000)    42054 2024-04-14 19:24:43.000000 flashcam-1.9.3/flashcam/web.py
+drwxrwxr-x   0 ojr       (1000) ojr       (1000)        0 2024-04-20 18:27:34.900369 flashcam-1.9.3/flashcam.egg-info/
+-rw-r--r--   0 ojr       (1000) ojr       (1000)     1582 2024-04-20 18:27:34.000000 flashcam-1.9.3/flashcam.egg-info/PKG-INFO
+-rw-rw-r--   0 ojr       (1000) ojr       (1000)     1049 2024-04-20 18:27:34.000000 flashcam-1.9.3/flashcam.egg-info/SOURCES.txt
+-rw-rw-r--   0 ojr       (1000) ojr       (1000)        1 2024-04-20 18:27:34.000000 flashcam-1.9.3/flashcam.egg-info/dependency_links.txt
+-rw-rw-r--   0 ojr       (1000) ojr       (1000)      165 2024-04-20 18:27:34.000000 flashcam-1.9.3/flashcam.egg-info/requires.txt
+-rw-rw-r--   0 ojr       (1000) ojr       (1000)        9 2024-04-20 18:27:34.000000 flashcam-1.9.3/flashcam.egg-info/top_level.txt
+-rw-rw-r--   0 ojr       (1000) ojr       (1000)       38 2024-04-20 18:27:34.904369 flashcam-1.9.3/setup.cfg
+-rwxrwxr-x   0 ojr       (1000) ojr       (1000)     2275 2023-11-02 08:34:00.000000 flashcam-1.9.3/setup.py
```

### Comparing `flashcam-1.9.2/PKG-INFO` & `flashcam-1.9.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flashcam
-Version: 1.9.2
+Version: 1.9.3
 Summary: Composition of scripts to control a web camera
 Home-page: https://gitlab.com/jaromrax/flashcam
 Author: jaromrax
 Author-email: jaromrax@gmail.com
 License: GPL2
 Description-Content-Type: text/markdown
 Requires-Dist: fire
```

### Comparing `flashcam-1.9.2/README.md` & `flashcam-1.9.3/README.md`

 * *Files identical despite different names*

### Comparing `flashcam-1.9.2/bin/flashcam` & `flashcam-1.9.3/bin/flashcam`

 * *Files identical despite different names*

### Comparing `flashcam-1.9.2/bin/flashcam_org` & `flashcam-1.9.3/bin/flashcam_org`

 * *Files identical despite different names*

### Comparing `flashcam-1.9.2/bin/flashcam_rep` & `flashcam-1.9.3/bin/flashcam_rep`

 * *Files identical despite different names*

### Comparing `flashcam-1.9.2/bin/flashcamg` & `flashcam-1.9.3/bin/flashcamg`

 * *Files identical despite different names*

### Comparing `flashcam-1.9.2/flashcam/base_camera2.py` & `flashcam-1.9.3/flashcam/base_camera2.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,45 +1,46 @@
 import time
 import threading
 import datetime
-
 import os
-
 import flashcam.config as config
 
-
-
 try:
     from greenlet import getcurrent as get_ident
 except ImportError:
     print("i... error importing from greenlet ............")
     try:
         from thread import get_ident
     except ImportError:
         from _thread import get_ident
 
-
-
-
-
 class CameraEvent(object):
-    """An Event-like class that signals all active clients when a new frame is
-    available.
-    """
+    """An Event-like class that signals TO all active clients when a new frame is available.
 
+    `CameraEvent` is a custom class that mimics the behavior of `threading.Event` but is tailored for managing the state of frames in a camera service where multiple clients might be waiting for new frames to be available.
+    """
     def __init__(self):
+        """
+        dict of events - they are 'getcurrent' from greenlet
+        """
         self.events = {}
 
     def wait(self):
-        """Invoked from each client's thread to wait for the next frame."""
+        """Invoked from each client's thread to wait for the next frame.
+        `get_ident` is a function used to uniquely identify the current thread (or greenlet). It's used to differentiate between different clients (threads) that are waiting for new frames.
+        """
         ident = get_ident()
         if ident not in self.events:
             # this is a new client
             # add an entry for it in the self.events dict
             # each entry has two elements, a threading.Event() and a timestamp
+
+#            `threading.Event` is a synchronization primitive that can be used to manage the state.
+#            An event can be set or cleared; threads can wait for an event to be set.
+
             self.events[ident] = [threading.Event(), time.time()]
         return self.events[ident][0].wait()
 
     def set(self):
         """Invoked by the camera thread when a new frame is available."""
         now = time.time()
         remove = None
@@ -83,31 +84,19 @@
 
     #actual_dm_conf = {}
 
     def __init__(self):
         """Start the background camera thread if it isn't running yet.
         all the parameters on cmdline will go to Thread and thread is launched
         """
-
-        #--------------------------- TRYING TO CHANGE THE PARAMETER'S passage
-        # config.load_config()  THIS IS IN WEB.PY
-
-        # self.actual_dm_conf = {'target_frame':config.CONFIG['target_frame'],
-        #         'average':  config.CONFIG['average'],
-        #         'threshold':config.CONFIG['threshold'],
-        #         'blur':     config.CONFIG['blur']}
-        # print("i... basecamera2",  self.actual_dm_conf )
-
-
-
         if BaseCamera.thread is None:
             BaseCamera.last_access = time.time()
 
             # start background frame thread - the classmethod _thread
-            print("D.. launching _thread")
+            print("D.. launching BaseCamera _thread")
             BaseCamera.thread = threading.Thread(target=self._thread   )
             BaseCamera.thread.start()
 
             # wait until frames are available
             while self.get_frame() is None:
                 time.sleep(0)
 
@@ -119,37 +108,41 @@
         BaseCamera.event.wait()
         BaseCamera.event.clear()
 
         return BaseCamera.frame, BaseCamera.nframes, BaseCamera.capture_time
 
     @staticmethod
     def frames( ):
-        """"Generator that returns frames from the camera."""
+        """"
+        Generator that returns frames from the camera. IT is called in _thread,
+        but it is defined in the daughter - real_camera @staticmethod def frames() -
+        where the camera object is init.
+        """
         raise RuntimeError('Must be implemented by subclasses.')
 
     #
     # this is where thisclass really starts to work when viewrConnects.
     #   calling .frames() => returns an iterator/generator
     #
     @classmethod
     def killme(cls):
         cls.kill = True
 
 
-
     @classmethod
     def _thread(cls):
         """Camera background thread.
         I try to get all neede parametaers here.
         """
             # print("i... inside _thread:", framekind, average, blur)
         frames_iterator = cls.frames( )
         cls.kill = False
 
         for frame in frames_iterator:
+            #print("D... tracking 1")
             # leave on error, i mean it permanent
             if (frame is None) or (len(frame)<100):
                 # BaseCamera.thread = None
                 print("X... no frame in _thread")
                 # return
             BaseCamera.frame = frame
             BaseCamera.event.set()  # send signal to clients
@@ -162,10 +155,11 @@
             if False:
                 print('X... Stopping camera thread due to inactivity.')
                 frames_iterator.close()
                 break
             if cls.kill:
                 print("D... killing self in base_cam")
                 break
+            #print("D... tracking F")
         BaseCamera.thread = None
         print("X... leaving _thread")
         ### print("X... never get here........................")
```

### Comparing `flashcam-1.9.2/flashcam/config.py` & `flashcam-1.9.3/flashcam/config.py`

 * *Files identical despite different names*

### Comparing `flashcam-1.9.2/flashcam/data/BEAM_OFF.jpg` & `flashcam-1.9.3/flashcam/data/BEAM_OFF.jpg`

 * *Files identical despite different names*

### Comparing `flashcam-1.9.2/flashcam/data/BEAM_ON_.jpg` & `flashcam-1.9.3/flashcam/data/BEAM_ON_.jpg`

 * *Files identical despite different names*

### Comparing `flashcam-1.9.2/flashcam/data/DET_NRDY.jpg` & `flashcam-1.9.3/flashcam/data/DET_NRDY.jpg`

 * *Files identical despite different names*

### Comparing `flashcam-1.9.2/flashcam/data/DET_RDY_.jpg` & `flashcam-1.9.3/flashcam/data/DET_RDY_.jpg`

 * *Files identical despite different names*

### Comparing `flashcam-1.9.2/flashcam/data/digital-7.mono.ttf` & `flashcam-1.9.3/flashcam/data/digital-7.mono.ttf`

 * *Files identical despite different names*

### Comparing `flashcam-1.9.2/flashcam/data/digital-7.regular.ttf` & `flashcam-1.9.3/flashcam/data/digital-7.regular.ttf`

 * *Files identical despite different names*

### Comparing `flashcam-1.9.2/flashcam/data/monoskop.jpg` & `flashcam-1.9.3/flashcam/data/monoskop.jpg`

 * *Files identical despite different names*

### Comparing `flashcam-1.9.2/flashcam/data/pattern_acircles.png` & `flashcam-1.9.3/flashcam/data/pattern_acircles.png`

 * *Files identical despite different names*

### Comparing `flashcam-1.9.2/flashcam/data/pattern_chessboard.png` & `flashcam-1.9.3/flashcam/data/pattern_chessboard.png`

 * *Files identical despite different names*

### Comparing `flashcam-1.9.2/flashcam/data/small_pixel.ttf` & `flashcam-1.9.3/flashcam/data/small_pixel.ttf`

 * *Files identical despite different names*

### Comparing `flashcam-1.9.2/flashcam/data/win_rain.jpg` & `flashcam-1.9.3/flashcam/data/win_rain.jpg`

 * *Files identical despite different names*

### Comparing `flashcam-1.9.2/flashcam/data/win_skull.jpg` & `flashcam-1.9.3/flashcam/data/win_skull.jpg`

 * *Files identical despite different names*

### Comparing `flashcam-1.9.2/flashcam/data/win_storm.jpg` & `flashcam-1.9.3/flashcam/data/win_storm.jpg`

 * *Files identical despite different names*

### Comparing `flashcam-1.9.2/flashcam/data/win_winter.jpg` & `flashcam-1.9.3/flashcam/data/win_winter.jpg`

 * *Files identical despite different names*

### Comparing `flashcam-1.9.2/flashcam/data/windows.jpg` & `flashcam-1.9.3/flashcam/data/windows.jpg`

 * *Files identical despite different names*

### Comparing `flashcam-1.9.2/flashcam/direct.py` & `flashcam-1.9.3/flashcam/direct.py`

 * *Files identical despite different names*

### Comparing `flashcam-1.9.2/flashcam/izmq_receiver.py` & `flashcam-1.9.3/flashcam/izmq_receiver.py`

 * *Files identical despite different names*

### Comparing `flashcam-1.9.2/flashcam/mmapwr.py` & `flashcam-1.9.3/flashcam/mmapwr.py`

 * *Files identical despite different names*

### Comparing `flashcam-1.9.2/flashcam/real_camera.py` & `flashcam-1.9.3/flashcam/real_camera.py`

 * *Files 0% similar despite different names*

```diff
@@ -809,29 +809,38 @@
                         # PROBLEM TO SOLVE
                         #    i wait for re-demand from client........ seem to work.....
                         #
                         if expression == "switch_res":
                             switch_res = value #not(switch_res)
                             print("i...              EXPERIMENTAL SWITCH RESOLUTION now=", switch_res)
                             if switch_res:
+                                #maxres = "640x480"
                                 maxres = get_resolutions( vidnum )[-1] # from usb_check
                                 config.CONFIG['resolution'] = maxres
                                 print("D.... resolution to MAX", maxres)
                                 # cap.close()
                                 #cap, vidnum, s9009 = camera.init_cam()
+                                try:
+                                    width,height = maxres.split("x")
+                                    cap.set(cv2.CAP_PROP_FRAME_WIDTH, int(width) )
+                                    cap.set(cv2.CAP_PROP_FRAME_HEIGHT, int(height))
+                                except:
+                                    print("X... problem on setting  resolution:", maxres)
 
 
                             else:
                                 config.CONFIG['resolution'] = "640x480"
                                 print("D.... resolution to 640x480")
                                 #cap.release()
                                 #cap, vidnum, s9009 = camera.init_cam()
+                                cap.set(cv2.CAP_PROP_FRAME_WIDTH, 640)
+                                cap.set(cv2.CAP_PROP_FRAME_HEIGHT, 480)
 
                             res = config.CONFIG['resolution']
-                            break
+                            #break # THIS BEAKS INIT, work on PC, not well on RPI
 
 
                     if save_image_png:  # camera_screenshot PNG Full quality
                         print("D... HERE I SAVE  image camera_screenshot_PNG Full Quality")
                         if config.CONFIG['datapath'][-1] == "/":
                             pngname = dt.datetime.now().strftime("%Y%m%d_%H%M%S.%f")
                             pngname = pngname[:-5].replace(".","_")
```

### Comparing `flashcam-1.9.2/flashcam/stream_enhancer.py` & `flashcam-1.9.3/flashcam/stream_enhancer.py`

 * *Files identical despite different names*

### Comparing `flashcam-1.9.2/flashcam/uniwrec.py` & `flashcam-1.9.3/flashcam/uniwrec.py`

 * *Files identical despite different names*

### Comparing `flashcam-1.9.2/flashcam/uniwrec_io.py` & `flashcam-1.9.3/flashcam/uniwrec_io.py`

 * *Files identical despite different names*

### Comparing `flashcam-1.9.2/flashcam/uniwrec_keys.py` & `flashcam-1.9.3/flashcam/uniwrec_keys.py`

 * *Files identical despite different names*

### Comparing `flashcam-1.9.2/flashcam/uniwrec_manip.py` & `flashcam-1.9.3/flashcam/uniwrec_manip.py`

 * *Files identical despite different names*

### Comparing `flashcam-1.9.2/flashcam/usbcheck.py` & `flashcam-1.9.3/flashcam/usbcheck.py`

 * *Files identical despite different names*

### Comparing `flashcam-1.9.2/flashcam/v4lc.py` & `flashcam-1.9.3/flashcam/v4lc.py`

 * *Files identical despite different names*

### Comparing `flashcam-1.9.2/flashcam/web.py` & `flashcam-1.9.3/flashcam/web.py`

 * *Files identical despite different names*

### Comparing `flashcam-1.9.2/flashcam.egg-info/PKG-INFO` & `flashcam-1.9.3/flashcam.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flashcam
-Version: 1.9.2
+Version: 1.9.3
 Summary: Composition of scripts to control a web camera
 Home-page: https://gitlab.com/jaromrax/flashcam
 Author: jaromrax
 Author-email: jaromrax@gmail.com
 License: GPL2
 Description-Content-Type: text/markdown
 Requires-Dist: fire
```

### Comparing `flashcam-1.9.2/flashcam.egg-info/SOURCES.txt` & `flashcam-1.9.3/flashcam.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `flashcam-1.9.2/setup.py` & `flashcam-1.9.3/setup.py`

 * *Files identical despite different names*

