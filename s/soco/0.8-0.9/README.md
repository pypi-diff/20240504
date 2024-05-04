# Comparing `tmp/soco-0.8.tar.gz` & `tmp/soco-0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/soco-0.8.tar", last modified: Fri Jun  6 18:15:10 2014, max compression
+gzip compressed data, was "dist/soco-0.9.tar", last modified: Thu Sep 25 18:06:51 2014, max compression
```

## Comparing `soco-0.8.tar` & `soco-0.9.tar`

### file list

```diff
@@ -1,42 +1,50 @@
-drwxr-xr-x   0 stefan    (1000) stefan    (1000)        0 2014-06-06 18:15:10.000000 soco-0.8/
--rw-r--r--   0 stefan    (1000) stefan    (1000)      447 2014-06-05 21:22:30.000000 soco-0.8/AUTHORS.rst
--rw-r--r--   0 stefan    (1000) stefan    (1000)      340 2014-06-06 18:15:10.000000 soco-0.8/setup.cfg
-drwxr-xr-x   0 stefan    (1000) stefan    (1000)        0 2014-06-06 18:15:10.000000 soco-0.8/soco.egg-info/
--rw-r--r--   0 stefan    (1000) stefan    (1000)        5 2014-06-06 18:15:08.000000 soco-0.8/soco.egg-info/top_level.txt
--rw-r--r--   0 stefan    (1000) stefan    (1000)        1 2014-06-06 18:15:08.000000 soco-0.8/soco.egg-info/dependency_links.txt
--rw-r--r--   0 stefan    (1000) stefan    (1000)        8 2014-06-06 18:15:08.000000 soco-0.8/soco.egg-info/requires.txt
--rw-r--r--   0 stefan    (1000) stefan    (1000)      736 2014-06-06 18:15:10.000000 soco-0.8/soco.egg-info/SOURCES.txt
--rw-r--r--   0 stefan    (1000) stefan    (1000)     8909 2014-06-06 18:15:08.000000 soco-0.8/soco.egg-info/PKG-INFO
--rwxr-xr-x   0 stefan    (1000) stefan    (1000)     2685 2014-06-06 17:04:45.000000 soco-0.8/setup.py
--rw-r--r--   0 stefan    (1000) stefan    (1000)      122 2014-06-06 18:08:42.000000 soco-0.8/requirements-dev.txt
--rw-r--r--   0 stefan    (1000) stefan    (1000)     1140 2014-05-04 17:52:05.000000 soco-0.8/LICENSE.rst
-drwxr-xr-x   0 stefan    (1000) stefan    (1000)        0 2014-06-06 18:15:10.000000 soco-0.8/soco/
--rwxr-xr-x   0 stefan    (1000) stefan    (1000)    51578 2014-06-06 18:08:42.000000 soco-0.8/soco/core.py
-drwxr-xr-x   0 stefan    (1000) stefan    (1000)        0 2014-06-06 18:15:10.000000 soco-0.8/soco/plugins/
--rw-r--r--   0 stefan    (1000) stefan    (1000)     1328 2014-06-05 21:22:31.000000 soco-0.8/soco/plugins/example.py
--rw-r--r--   0 stefan    (1000) stefan    (1000)    19638 2014-06-06 17:04:45.000000 soco-0.8/soco/plugins/wimp.py
--rw-r--r--   0 stefan    (1000) stefan    (1000)     1090 2014-06-05 21:22:31.000000 soco-0.8/soco/plugins/__init__.py
--rw-r--r--   0 stefan    (1000) stefan    (1000)     7206 2014-06-05 21:22:31.000000 soco-0.8/soco/plugins/spotify.py
--rw-r--r--   0 stefan    (1000) stefan    (1000)      260 2014-06-05 21:22:31.000000 soco-0.8/soco/xml.py
--rw-r--r--   0 stefan    (1000) stefan    (1000)    50868 2014-06-06 17:04:45.000000 soco-0.8/soco/data_structures.py
--rw-r--r--   0 stefan    (1000) stefan    (1000)     5613 2014-06-05 21:22:31.000000 soco-0.8/soco/utils.py
--rw-r--r--   0 stefan    (1000) stefan    (1000)    28884 2014-06-06 17:04:45.000000 soco-0.8/soco/services.py
--rw-r--r--   0 stefan    (1000) stefan    (1000)     1067 2014-06-06 18:09:43.000000 soco-0.8/soco/__init__.py
--rwxr-xr-x   0 stefan    (1000) stefan    (1000)    13747 2014-06-06 17:04:45.000000 soco-0.8/soco/events.py
--rw-r--r--   0 stefan    (1000) stefan    (1000)     2213 2014-06-06 17:04:45.000000 soco-0.8/soco/groups.py
--rwxr-xr-x   0 stefan    (1000) stefan    (1000)     1127 2014-06-05 21:22:30.000000 soco-0.8/soco/exceptions.py
--rw-r--r--   0 stefan    (1000) stefan    (1000)     1294 2014-06-06 17:04:45.000000 soco-0.8/soco/compat.py
--rw-r--r--   0 stefan    (1000) stefan    (1000)        9 2014-05-04 17:52:05.000000 soco-0.8/requirements.txt
--rw-r--r--   0 stefan    (1000) stefan    (1000)     6104 2014-06-05 21:22:30.000000 soco-0.8/README.rst
--rw-r--r--   0 stefan    (1000) stefan    (1000)     8909 2014-06-06 18:15:10.000000 soco-0.8/PKG-INFO
--rw-r--r--   0 stefan    (1000) stefan    (1000)      129 2014-05-04 17:52:05.000000 soco-0.8/MANIFEST.in
-drwxr-xr-x   0 stefan    (1000) stefan    (1000)        0 2014-06-06 18:15:10.000000 soco-0.8/unittest/
--rwxr-xr-x   0 stefan    (1000) stefan    (1000)     9170 2013-10-22 15:31:57.000000 soco-0.8/unittest/execute_unittests.py
--rw-r--r--   0 stefan    (1000) stefan    (1000)    13547 2014-06-05 21:22:31.000000 soco-0.8/unittest/test_integration.py
--rw-r--r--   0 stefan    (1000) stefan    (1000)    16762 2014-01-21 19:08:44.000000 soco-0.8/unittest/soco_unittest.py
--rw-r--r--   0 stefan    (1000) stefan    (1000)     2913 2014-06-05 21:22:31.000000 soco-0.8/unittest/test_events.py
--rw-r--r--   0 stefan    (1000) stefan    (1000)      716 2014-04-25 17:48:23.000000 soco-0.8/unittest/test_singleton.py
--rw-r--r--   0 stefan    (1000) stefan    (1000)     1779 2014-06-05 21:22:31.000000 soco-0.8/unittest/test_utils.py
--rw-r--r--   0 stefan    (1000) stefan    (1000)      706 2014-06-05 21:22:31.000000 soco-0.8/unittest/conftest.py
--rw-r--r--   0 stefan    (1000) stefan    (1000)    23650 2014-06-06 17:04:45.000000 soco-0.8/unittest/test_data_structures.py
--rw-r--r--   0 stefan    (1000) stefan    (1000)     8194 2014-06-06 17:04:45.000000 soco-0.8/unittest/test_services.py
+drwxrwxr-x   0 stefan    (1000) stefan    (1000)        0 2014-09-25 18:06:51.000000 soco-0.9/
+-rw-rw-r--   0 stefan    (1000) stefan    (1000)      340 2014-09-25 18:06:51.000000 soco-0.9/setup.cfg
+-rw-rw-r--   0 stefan    (1000) stefan    (1000)      129 2014-08-27 15:58:02.000000 soco-0.9/MANIFEST.in
+-rw-rw-r--   0 stefan    (1000) stefan    (1000)        9 2014-08-27 15:58:02.000000 soco-0.9/requirements.txt
+-rw-rw-r--   0 stefan    (1000) stefan    (1000)     6104 2014-08-27 15:58:02.000000 soco-0.9/README.rst
+-rw-rw-r--   0 stefan    (1000) stefan    (1000)       85 2014-08-27 15:58:02.000000 soco-0.9/requirements-dev.txt
+drwxrwxr-x   0 stefan    (1000) stefan    (1000)        0 2014-09-25 18:06:51.000000 soco-0.9/unittest/
+-rw-rw-r--   0 stefan    (1000) stefan    (1000)      538 2014-08-27 15:58:02.000000 soco-0.9/unittest/test_alarms.py
+-rw-rw-r--   0 stefan    (1000) stefan    (1000)    13547 2014-08-27 15:58:02.000000 soco-0.9/unittest/test_integration.py
+-rw-rw-r--   0 stefan    (1000) stefan    (1000)     1032 2014-08-27 15:58:02.000000 soco-0.9/unittest/test_utils.py
+-rw-rw-r--   0 stefan    (1000) stefan    (1000)     3577 2014-09-25 17:51:14.000000 soco-0.9/unittest/test_events.py
+-rw-rw-r--   0 stefan    (1000) stefan    (1000)     2248 2014-08-27 15:58:02.000000 soco-0.9/unittest/test_cache.py
+-rw-rw-r--   0 stefan    (1000) stefan    (1000)     1550 2014-08-27 15:58:02.000000 soco-0.9/unittest/test_discovery.py
+-rw-r--r--   0 stefan    (1000) stefan    (1000)    16762 2013-12-29 13:45:32.000000 soco-0.9/unittest/soco_unittest.py
+-rw-rw-r--   0 stefan    (1000) stefan    (1000)     8194 2014-08-27 15:58:02.000000 soco-0.9/unittest/test_services.py
+-rw-rw-r--   0 stefan    (1000) stefan    (1000)    22913 2014-09-23 15:33:24.000000 soco-0.9/unittest/test_data_structures.py
+-rw-rw-r--   0 stefan    (1000) stefan    (1000)    12978 2014-08-27 15:58:02.000000 soco-0.9/unittest/test_ms_data_structures.py
+-rw-rw-r--   0 stefan    (1000) stefan    (1000)      706 2014-08-27 15:58:02.000000 soco-0.9/unittest/conftest.py
+-rw-rw-r--   0 stefan    (1000) stefan    (1000)    14819 2014-09-25 17:51:14.000000 soco-0.9/unittest/test_core.py
+-rwxr-xr-x   0 stefan    (1000) stefan    (1000)     9170 2013-12-10 16:25:42.000000 soco-0.9/unittest/execute_unittests.py
+-rw-rw-r--   0 stefan    (1000) stefan    (1000)     1273 2014-08-27 15:58:02.000000 soco-0.9/unittest/test_singleton.py
+drwxrwxr-x   0 stefan    (1000) stefan    (1000)        0 2014-09-25 18:06:51.000000 soco-0.9/soco/
+-rw-rw-r--   0 stefan    (1000) stefan    (1000)     5338 2014-08-27 15:58:02.000000 soco-0.9/soco/cache.py
+-rwxrwxr-x   0 stefan    (1000) stefan    (1000)    61447 2014-09-25 17:51:14.000000 soco-0.9/soco/core.py
+-rwxrwxr-x   0 stefan    (1000) stefan    (1000)    23179 2014-09-25 17:51:14.000000 soco-0.9/soco/events.py
+-rw-rw-r--   0 stefan    (1000) stefan    (1000)      611 2014-08-27 15:58:02.000000 soco-0.9/soco/config.py
+-rw-rw-r--   0 stefan    (1000) stefan    (1000)     4331 2014-08-27 15:58:02.000000 soco-0.9/soco/utils.py
+drwxrwxr-x   0 stefan    (1000) stefan    (1000)        0 2014-09-25 18:06:51.000000 soco-0.9/soco/plugins/
+-rw-rw-r--   0 stefan    (1000) stefan    (1000)     1320 2014-09-23 15:33:24.000000 soco-0.9/soco/plugins/example.py
+-rw-rw-r--   0 stefan    (1000) stefan    (1000)     7206 2014-08-27 15:58:02.000000 soco-0.9/soco/plugins/spotify.py
+-rw-rw-r--   0 stefan    (1000) stefan    (1000)    19682 2014-09-23 15:33:24.000000 soco-0.9/soco/plugins/wimp.py
+-rw-rw-r--   0 stefan    (1000) stefan    (1000)     1090 2014-08-27 15:58:02.000000 soco-0.9/soco/plugins/__init__.py
+-rwxrwxr-x   0 stefan    (1000) stefan    (1000)     1127 2014-08-27 15:58:02.000000 soco-0.9/soco/exceptions.py
+-rw-rw-r--   0 stefan    (1000) stefan    (1000)     1067 2014-09-25 18:00:24.000000 soco-0.9/soco/__init__.py
+-rw-rw-r--   0 stefan    (1000) stefan    (1000)    11381 2014-08-27 15:58:02.000000 soco-0.9/soco/alarms.py
+-rw-rw-r--   0 stefan    (1000) stefan    (1000)     1295 2014-08-27 15:58:02.000000 soco-0.9/soco/compat.py
+-rw-rw-r--   0 stefan    (1000) stefan    (1000)      260 2014-08-27 15:58:02.000000 soco-0.9/soco/xml.py
+-rw-rw-r--   0 stefan    (1000) stefan    (1000)     2213 2014-08-27 15:58:02.000000 soco-0.9/soco/groups.py
+-rw-rw-r--   0 stefan    (1000) stefan    (1000)    52149 2014-09-23 15:33:24.000000 soco-0.9/soco/data_structures.py
+-rw-rw-r--   0 stefan    (1000) stefan    (1000)    29277 2014-09-23 15:33:24.000000 soco-0.9/soco/services.py
+-rw-rw-r--   0 stefan    (1000) stefan    (1000)     1140 2014-08-27 15:58:02.000000 soco-0.9/LICENSE.rst
+-rw-rw-r--   0 stefan    (1000) stefan    (1000)     8909 2014-09-25 18:06:51.000000 soco-0.9/PKG-INFO
+-rwxrwxr-x   0 stefan    (1000) stefan    (1000)     2685 2014-08-27 15:58:02.000000 soco-0.9/setup.py
+-rw-rw-r--   0 stefan    (1000) stefan    (1000)      447 2014-08-27 15:58:02.000000 soco-0.9/AUTHORS.rst
+drwxrwxr-x   0 stefan    (1000) stefan    (1000)        0 2014-09-25 18:06:51.000000 soco-0.9/soco.egg-info/
+-rw-r--r--   0 stefan    (1000) stefan    (1000)        5 2014-09-25 18:06:43.000000 soco-0.9/soco.egg-info/top_level.txt
+-rw-r--r--   0 stefan    (1000) stefan    (1000)        1 2014-09-25 18:06:43.000000 soco-0.9/soco.egg-info/dependency_links.txt
+-rw-r--r--   0 stefan    (1000) stefan    (1000)     8909 2014-09-25 18:06:43.000000 soco-0.9/soco.egg-info/PKG-INFO
+-rw-r--r--   0 stefan    (1000) stefan    (1000)        8 2014-09-25 18:06:43.000000 soco-0.9/soco.egg-info/requires.txt
+-rw-r--r--   0 stefan    (1000) stefan    (1000)      912 2014-09-25 18:06:51.000000 soco-0.9/soco.egg-info/SOURCES.txt
```

### Comparing `soco-0.8/soco.egg-info/PKG-INFO` & `soco-0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: soco
-Version: 0.8
+Version: 0.9
 Summary:  SoCo (Sonos Controller) is a simple library to control Sonos speakers 
 Home-page: https://github.com/SoCo/SoCo
 Author: The SoCo-Team
 Author-email: python-soco@googlegroups.com
 License: MIT License
 Description: SoCo
         ====
```

### Comparing `soco-0.8/setup.py` & `soco-0.9/setup.py`

 * *Files identical despite different names*

### Comparing `soco-0.8/LICENSE.rst` & `soco-0.9/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `soco-0.8/soco/core.py` & `soco-0.9/soco/core.py`

 * *Files 12% similar despite different names*

```diff
@@ -12,19 +12,22 @@
 from textwrap import dedent
 import re
 import itertools
 import requests
 
 from .services import DeviceProperties, ContentDirectory
 from .services import RenderingControl, AVTransport, ZoneGroupTopology
+from .services import AlarmClock
 from .groups import ZoneGroup
 from .exceptions import CannotCreateDIDLMetadata
-from .data_structures import get_ml_item, QueueItem, URI
+from .data_structures import get_ml_item, QueueItem, URI, MLSonosPlaylist,\
+    MLShare, SearchResult, Queue, MusicLibraryItem
 from .utils import really_utf8, camel_to_underscore
 from .xml import XML
+from soco import config
 
 LOGGER = logging.getLogger(__name__)
 
 
 def discover(timeout=1, include_invisible=False):
     """ Discover Sonos zones on the local network.
 
@@ -61,15 +64,15 @@
     # we care about is the IP address
     if response:
         _, addr = _sock.recvfrom(1024)
         # Now we have an IP, we can build a SoCo instance and query that player
         # for the topology to find the other players. It is much more efficient
         # to rely upon the Zone Player's ability to find the others, than to
         # wait for query responses from them ourselves.
-        zone = SoCo(addr[0])
+        zone = config.SOCO_CLASS(addr[0])
         if include_invisible:
             return zone.all_zones
         else:
             return zone.visible_zones
     else:
         return None
 
@@ -93,45 +96,54 @@
         import warnings
         warnings.warn("get_speaker_ips is deprecated. Use discover instead.")
         return [i.ip_address for i in discover()]
 
 
 class _ArgsSingleton(type):
     """ A metaclass which permits only a single instance of each derived class
-    to exist for any given set of positional arguments.
+    sharing the same `_class_group` class attribute to exist for any given set
+    of positional arguments.
 
-    Attempts to instantiate a second instance of a derived class will return
-    the existing instance.
+    Attempts to instantiate a second instance of a derived class, or another
+    class with the same `_class_group`, with the same args will return the
+    existing instance.
 
     For example:
 
     >>> class ArgsSingletonBase(object):
     ...     __metaclass__ = _ArgsSingleton
     ...
     >>> class First(ArgsSingletonBase):
+    ...     _class_group = "greeting"
     ...     def __init__(self, param):
     ...         pass
     ...
+    >>> class Second(ArgsSingletonBase):
+    ...     _class_group = "greeting"
+    ...     def __init__(self, param):
+    ...         pass
     >>> assert First('hi') is First('hi')
     >>> assert First('hi') is First('bye')
     AssertionError
+    >>> assert First('hi') is Second('hi')
 
      """
     _instances = {}
 
     def __call__(cls, *args, **kwargs):
-        if cls not in cls._instances:
-            cls._instances[cls] = {}
-        if args not in cls._instances[cls]:
-            cls._instances[cls][args] = super(_ArgsSingleton, cls).__call__(
+        key = cls._class_group if hasattr(cls, '_class_group') else cls
+        if key not in cls._instances:
+            cls._instances[key] = {}
+        if args not in cls._instances[key]:
+            cls._instances[key][args] = super(_ArgsSingleton, cls).__call__(
                 *args, **kwargs)
-        return cls._instances[cls][args]
+        return cls._instances[key][args]
 
 
-class _SocoSingletonBase(  # pylint: disable=too-few-public-methods
+class _SocoSingletonBase(  # pylint: disable=too-few-public-methods,no-init
         _ArgsSingleton(str('ArgsSingletonMeta'), (object,), {})):
     """ The base class for the SoCo class.
 
     Uses a Python 2 and 3 compatible method of declaring a metaclass. See, eg,
     here: http://www.artima.com/weblogs/viewpost.jsp?thread=236234 and
     here: http://mikewatkins.ca/2008/11/29/python-2-and-3-metaclasses/
 
@@ -164,52 +176,71 @@
         get_current_track_info -- Get information about the currently playing
                                   track.
         get_speaker_info -- Get information about the Sonos speaker.
         partymode -- Put all the speakers in the network in the same group.
         join -- Join this speaker to another "master" speaker.
         unjoin -- Remove this speaker from a group.
         get_queue -- Get information about the queue.
-        get_folders -- Get search folders from the music library
         get_artists -- Get artists from the music library
         get_album_artists -- Get album artists from the music library
         get_albums -- Get albums from the music library
         get_genres -- Get genres from the music library
         get_composers -- Get composers from the music library
         get_tracks -- Get tracks from the music library
         get_playlists -- Get playlists from the music library
         get_music_library_information -- Get information from the music library
         get_current_transport_info -- get speakers playing state
+        browse_by_idstring -- Browse (get sub-elements) a given type
         add_uri_to_queue -- Adds an URI to the queue
         add_to_queue -- Add a track to the end of the queue
         remove_from_queue -- Remove a track from the queue
         clear_queue -- Remove all tracks from queue
         get_favorite_radio_shows -- Get favorite radio shows from Sonos'
                                     Radio app.
         get_favorite_radio_stations -- Get favorite radio stations.
+        create_sonos_playlist -- Creates a new Sonos' playlist
+        add_item_to_sonos_playlist -- Adds a queueable item to a Sonos'
+                                       playlist
 
     Properties::
 
         uid -- The speaker's unique identifier
         mute -- The speaker's mute status.
         volume -- The speaker's volume.
         bass -- The speaker's bass EQ.
         treble -- The speaker's treble EQ.
         loudness -- The status of the speaker's loudness compensation.
+        cross_fade -- The status of the speaker's crossfade.
         status_light -- The state of the Sonos status light.
         player_name  -- The speaker's name.
         play_mode -- The queue's repeat/shuffle settings.
 
     .. warning::
 
         These properties are not cached and will obtain information over the
         network, so may take longer than expected to set or return a value. It
         may be a good idea for you to cache the value in your own code.
 
     """
 
+    _class_group = 'SoCo'
+
+    # Key words used when performing searches
+    SEARCH_TRANSLATION = {'artists': 'A:ARTIST',
+                          'album_artists': 'A:ALBUMARTIST',
+                          'albums': 'A:ALBUM',
+                          'genres': 'A:GENRE',
+                          'composers': 'A:COMPOSER',
+                          'tracks': 'A:TRACKS',
+                          'playlists': 'A:PLAYLISTS',
+                          'share': 'S:',
+                          'sonos_playlists': 'SQ:',
+                          'categories': 'A:'}
+
+    # pylint: disable=super-on-old-class
     def __init__(self, ip_address):
         # Note: Creation of a SoCo instance should be as cheap and quick as
         # possible. Do not make any network calls here
         super(SoCo, self).__init__()
         # Check if ip_address is a valid IPv4 representation.
         # Sonos does not (yet) support IPv6
         try:
@@ -223,27 +254,29 @@
         # The services which we use
         # pylint: disable=invalid-name
         self.avTransport = AVTransport(self)
         self.contentDirectory = ContentDirectory(self)
         self.deviceProperties = DeviceProperties(self)
         self.renderingControl = RenderingControl(self)
         self.zoneGroupTopology = ZoneGroupTopology(self)
+        self.alarmClock = AlarmClock(self)
 
         # Some private attributes
         self._all_zones = set()
         self._groups = set()
         self._is_bridge = None
         self._is_coordinator = False
         self._player_name = None
         self._uid = None
         self._visible_zones = set()
         self._zgs_cache = None
 
     def __str__(self):
-        return "<SoCo object at ip {0}>".format(self.ip_address)
+        return "<{0} object at ip {1}>".format(
+            self.__class__.__name__, self.ip_address)
 
     def __repr__(self):
         return '{0}("{1}")'.format(self.__class__.__name__, self.ip_address)
 
     @property
     def player_name(self):
         """  The speaker's name. A string. """
@@ -254,15 +287,15 @@
         # and take advantage of any caching
         self._parse_zone_group_state()
         return self._player_name
 
     @player_name.setter
     def player_name(self, playername):
         """ Set the speaker's name """
-        self.deviceProperties.SetZoneAtrributes([
+        self.deviceProperties.SetZoneAttributes([
             ('DesiredZoneName', playername),
             ('DesiredIcon', ''),
             ('DesiredConfiguration', '')
             ])
 
     @property
     def uid(self):
@@ -343,18 +376,17 @@
             ('InstanceID', 0),
             ])
         return result['PlayMode']
 
     @play_mode.setter
     def play_mode(self, playmode):
         """ Set the speaker's mode """
-        modes = ('NORMAL', 'SHUFFLE_NOREPEAT', 'SHUFFLE', 'REPEAT_ALL')
         playmode = playmode.upper()
-        if playmode not in modes:
-            raise KeyError('invalid play mode')
+        if playmode not in PLAY_MODES:
+            raise KeyError("'%s' is not a valid play mode" % playmode)
 
         self.avTransport.SetPlayMode([
             ('InstanceID', 0),
             ('NewPlayMode', playmode)
             ])
 
     @property
@@ -718,26 +750,27 @@
         self._all_zones.clear()
         self._visible_zones.clear()
         # Loop over each ZoneGroup Element
         for group_element in tree.findall('ZoneGroup'):
             coordinator_uid = group_element.attrib['Coordinator']
             group_uid = group_element.attrib['ID']
             members = set()
-            for member_element in group_element.iter('ZoneGroupMember'):
+            for member_element in group_element.findall('ZoneGroupMember'):
                 # Create a SoCo instance for each member. Because SoCo
                 # instances are singletons, this is cheap if they have already
                 # been created, and useful if they haven't. We can then
                 # update various properties for that instance.
                 member_attribs = member_element.attrib
                 ip_addr = member_attribs['Location'].\
                     split('//')[1].split(':')[0]
-                zone = SoCo(ip_addr)
+                zone = config.SOCO_CLASS(ip_addr)
                 zone._uid = member_attribs['UUID']
                 # If this element has the same UUID as the coordinator, it is
                 # the coordinator
+                group_coordinator = None
                 if zone._uid == coordinator_uid:
                     group_coordinator = zone
                     zone._is_coordinator = True
                 else:
                     zone._is_coordinator = False
                 zone._player_name = member_attribs['ZoneName']
                 # uid and is_bridge do not change, but it does no real harm to
@@ -1073,20 +1106,22 @@
             response['CurrentTransportState']
         playstate['current_transport_status'] = \
             response['CurrentTransportStatus']
         playstate['current_transport_speed'] = response['CurrentSpeed']
 
         return playstate
 
-    def get_queue(self, start=0, max_items=100):
+    def get_queue(self, start=0, max_items=100, full_album_art_uri=False):
         """ Get information about the queue
 
         :param start: Starting number of returned matches
         :param max_items: Maximum number of returned matches
-        :returns: A list of :py:class:`~.soco.data_structures.QueueItem`.
+        :param full_album_art_uri: If the album art URI should include the
+            IP address
+        :returns: A :py:class:`~.soco.data_structures.Queue` object
 
         This method is heavly based on Sam Soffes (aka soffes) ruby
         implementation
 
         """
         queue = []
         response = self.contentDirectory.Browse([
@@ -1094,183 +1129,306 @@
             ('BrowseFlag', 'BrowseDirectChildren'),
             ('Filter', '*'),
             ('StartingIndex', start),
             ('RequestedCount', max_items),
             ('SortCriteria', '')
             ])
         result = response['Result']
+
+        metadata = {}
+        for tag in ['NumberReturned', 'TotalMatches', 'UpdateID']:
+            metadata[camel_to_underscore(tag)] = int(response[tag])
+
+        # I'm not sure this necessary (any more). Even with an empty queue,
+        # there is still a result object. This shoud be investigated.
         if not result:
-            return queue
+            # pylint: disable=star-args
+            return Queue(queue, **metadata)
 
         result_dom = XML.fromstring(really_utf8(result))
         for element in result_dom.findall(
                 '{urn:schemas-upnp-org:metadata-1-0/DIDL-Lite/}item'):
             item = QueueItem.from_xml(element)
+            # Check if the album art URI should be fully qualified
+            if full_album_art_uri:
+                self._update_album_art_to_full_uri(item)
             queue.append(item)
 
-        return queue
+        # pylint: disable=star-args
+        return Queue(queue, **metadata)
 
-    def get_sonos_playlists(self, start=0, max_items=100):
+    def get_sonos_playlists(self, start=0, max_items=100,
+                            full_album_art_uri=False):
         """ Convenience method for:
             get_music_library_information('sonos_playlists')
             Refer to the docstring for that method
 
         """
         out = self.get_music_library_information(
             'sonos_playlists',
             start,
-            max_items)
+            max_items,
+            full_album_art_uri)
         return out
 
-    def get_artists(self, start=0, max_items=100):
+    def get_artists(self, start=0, max_items=100, full_album_art_uri=False):
         """ Convinience method for :py:meth:`get_music_library_information`
         with `search_type='artists'`. For details on remaining arguments refer
         to the docstring for that method.
 
         """
-        out = self.get_music_library_information('artists', start, max_items)
+        out = self.get_music_library_information('artists', start, max_items,
+                                                 full_album_art_uri)
         return out
 
-    def get_album_artists(self, start=0, max_items=100):
+    def get_album_artists(self, start=0, max_items=100,
+                          full_album_art_uri=False):
         """ Convinience method for :py:meth:`get_music_library_information`
         with `search_type='album_artists'`. For details on remaining arguments
         refer to the docstring for that method.
 
         """
         out = self.get_music_library_information('album_artists',
-                                                 start, max_items)
+                                                 start, max_items,
+                                                 full_album_art_uri)
         return out
 
-    def get_albums(self, start=0, max_items=100):
+    def get_albums(self, start=0, max_items=100, full_album_art_uri=False):
         """ Convinience method for :py:meth:`get_music_library_information`
         with `search_type='albums'`. For details on remaining arguments refer
         to the docstring for that method.
 
         """
-        out = self.get_music_library_information('albums', start, max_items)
+        out = self.get_music_library_information('albums', start, max_items,
+                                                 full_album_art_uri)
         return out
 
-    def get_genres(self, start=0, max_items=100):
+    def get_genres(self, start=0, max_items=100, full_album_art_uri=False):
         """ Convinience method for :py:meth:`get_music_library_information`
         with `search_type='genres'`. For details on remaining arguments refer
         to the docstring for that method.
 
         """
-        out = self.get_music_library_information('genres', start, max_items)
+        out = self.get_music_library_information('genres', start, max_items,
+                                                 full_album_art_uri)
         return out
 
-    def get_composers(self, start=0, max_items=100):
+    def get_composers(self, start=0, max_items=100, full_album_art_uri=False):
         """ Convinience method for :py:meth:`get_music_library_information`
         with `search_type='composers'`. For details on remaining arguments
         refer to the docstring for that method.
 
         """
-        out = self.get_music_library_information('composers', start, max_items)
+        out = self.get_music_library_information('composers', start, max_items,
+                                                 full_album_art_uri)
         return out
 
-    def get_tracks(self, start=0, max_items=100):
+    def get_tracks(self, start=0, max_items=100, full_album_art_uri=False):
         """ Convinience method for :py:meth:`get_music_library_information`
         with `search_type='tracks'`. For details on remaining arguments refer
         to the docstring for that method.
 
         """
-        out = self.get_music_library_information('tracks', start, max_items)
+        out = self.get_music_library_information('tracks', start, max_items,
+                                                 full_album_art_uri)
         return out
 
-    def get_playlists(self, start=0, max_items=100):
+    def get_playlists(self, start=0, max_items=100, full_album_art_uri=False):
         """ Convinience method for :py:meth:`get_music_library_information`
         with `search_type='playlists'`. For details on remaining arguments
         refer to the docstring for that method.
 
         NOTE: The playlists that are referred to here are the playlist (files)
         imported from the music library, they are not the Sonos playlists.
 
         """
-        out = self.get_music_library_information('playlists', start, max_items)
+        out = self.get_music_library_information('playlists', start, max_items,
+                                                 full_album_art_uri)
         return out
 
     def get_music_library_information(self, search_type, start=0,
-                                      max_items=100):
+                                      max_items=100, full_album_art_uri=False):
         """ Retrieve information about the music library
 
         :param search_type: The kind of information to retrieve. Can be one of:
             'artists', 'album_artists', 'albums', 'genres', 'composers',
             'tracks', 'share', 'sonos_playlists', and 'playlists', where
             playlists are the imported file based playlists from the
             music library
         :param start: Starting number of returned matches
         :param max_items: Maximum number of returned matches. NOTE: The maximum
             may be restricted by the unit, presumably due to transfer
             size consideration, so check the returned number against the
             requested.
-        :returns: A dictionary with metadata for the search, with the
-            keys 'number_returned', 'update_id', 'total_matches' and an
-            'item_list' list with the search results. The search results
-            are instances of one of
-            :py:class:`~.soco.data_structures.MLArtist`,
-            :py:class:`~.soco.data_structures.MLAlbumArtist`,
-            :py:class:`~.soco.data_structures.MLAlbum`,
-            :py:class:`~.soco.data_structures.MLGenre`,
-            :py:class:`~.soco.data_structures.MLComposer`,
-            :py:class:`~.soco.data_structures.MLTrack`,
-            :py:class:`~.soco.data_structures.MLShare`,
-            :py:class:`~.soco.data_structures.MLSonosPlaylist and
-            :py:class:`~.soco.data_structures.MLPlaylist` depending on the
-            type of the search.
+        :param full_album_art_uri: If the album art URI should include the
+            IP address
+        :returns: A :py:class:`~.soco.data_structures.SearchResult` object
         :raises: :py:class:`SoCoException` upon errors
 
         NOTE: The playlists that are returned with the 'playlists' search, are
         the playlists imported from (files in) the music library, they are not
         the Sonos playlists.
 
         The information about the which searches can be performed and the form
         of the query has been gathered from the Janos project:
         http://sourceforge.net/projects/janos/ Props to the authors of that
         project.
 
         """
-        search_translation = {'artists': 'A:ARTIST',
-                              'album_artists': 'A:ALBUMARTIST',
-                              'albums': 'A:ALBUM', 'genres': 'A:GENRE',
-                              'composers': 'A:COMPOSER', 'tracks': 'A:TRACKS',
-                              'playlists': 'A:PLAYLISTS', 'share': 'S:',
-                              'sonos_playlists': 'SQ:'}
-        search = search_translation[search_type]
+        search = self.SEARCH_TRANSLATION[search_type]
+        response, metadata = self._music_lib_search(search, start, max_items)
+        metadata['search_type'] = search_type
+
+        # Parse the results
+        dom = XML.fromstring(really_utf8(response['Result']))
+        item_list = []
+        for container in dom:
+            if search_type == 'sonos_playlists':
+                item = MLSonosPlaylist.from_xml(container)
+            elif search_type == 'share':
+                item = MLShare.from_xml(container)
+            else:
+                item = get_ml_item(container)
+            # Check if the album art URI should be fully qualified
+            if full_album_art_uri:
+                self._update_album_art_to_full_uri(item)
+            # Append the item to the list
+            item_list.append(item)
+
+        # pylint: disable=star-args
+        return SearchResult(item_list, **metadata)
+
+    def browse(self, ml_item=None, start=0, max_items=100,
+               full_album_art_uri=False):
+        """Browse (get sub-elements) a music library item
+
+        Keyword arguments:
+            ml_item (MusicLibraryItem): The MusicLibraryItem to browse, if left
+                out or passed None, the items at the base level will be
+                returned
+            start (int): The starting index of the results
+            max_items (int): The maximum number of items to return
+            full_album_art_uri(bool): If the album art URI should include the
+                IP address
+
+        Returns:
+            dict: A :py:class:`~.soco.data_structures.SearchResult` object
+
+        Raises:
+            AttributeError: If ``ml_item`` has no ``item_id`` attribute
+            SoCoUPnPException: With ``error_code='701'`` if the item cannot be
+                browsed
+        """
+        if ml_item is None:
+            search = 'A:'
+        else:
+            search = ml_item.item_id
+
+        response, metadata = self._music_lib_search(search, start, max_items)
+        metadata['search_type'] = 'browse'
+
+        # Parse the results
+        dom = XML.fromstring(really_utf8(response['Result']))
+        item_list = []
+        for container in dom:
+            item = get_ml_item(container)
+            # Check if the album art URI should be fully qualified
+            if full_album_art_uri:
+                self._update_album_art_to_full_uri(item)
+            item_list.append(item)
+
+        # pylint: disable=star-args
+        return SearchResult(item_list, **metadata)
+
+    # pylint: disable=too-many-arguments
+    def browse_by_idstring(self, search_type, idstring, start=0,
+                           max_items=100, full_album_art_uri=False):
+        """Browse (get sub-elements) a given type
+
+        :param search_type: The kind of information to retrieve. Can be one of:
+            'artists', 'album_artists', 'albums', 'genres', 'composers',
+            'tracks', 'share', 'sonos_playlists', and 'playlists', where
+            playlists are the imported file based playlists from the
+            music library
+        :param idstring: String ID to search for
+        :param start: Starting number of returned matches
+        :param max_items: Maximum number of returned matches. NOTE: The maximum
+            may be restricted by the unit, presumably due to transfer
+            size consideration, so check the returned number against the
+            requested.
+        :param full_album_art_uri: If the album art URI should include the
+                IP address
+        :returns: A dictionary with metadata for the search, with the
+            keys 'number_returned', 'update_id', 'total_matches' and an
+            'item_list' list with the search results.
+        """
+        search = self.SEARCH_TRANSLATION[search_type]
+
+        # Check if the string ID already has the type, if so we do not want to
+        # add one
+        if idstring.startswith(search):
+            search = ""
+
+        search_uri = "#{0}{1}".format(search, idstring)
+
+        search_item = MusicLibraryItem(uri=search_uri, title='', parent_id='')
+
+        # Call the base version
+        return self.browse(search_item, start, max_items, full_album_art_uri)
+
+    def _music_lib_search(self, search, start, max_items):
+        """Perform a music library search and extract search numbers
+
+        You can get an overview of all the relevant search prefixes (like
+        'A:') and their meaning with the request:
+
+        .. code ::
+
+         response = device.contentDirectory.Browse([
+             ('ObjectID', '0'),
+             ('BrowseFlag', 'BrowseDirectChildren'),
+             ('Filter', '*'),
+             ('StartingIndex', 0),
+             ('RequestedCount', 100),
+             ('SortCriteria', '')
+         ])
+
+        Args:
+            search (str): The ID to search
+            start: The index of the forst item to return
+            max_items: The maximum number of items to return
+
+        Returns:
+            tuple: (response, metadata) where response is the returned metadata
+                and metadata is a dict with the 'number_returned',
+                'total_matches' and 'update_id' integers
+        """
         response = self.contentDirectory.Browse([
             ('ObjectID', search),
             ('BrowseFlag', 'BrowseDirectChildren'),
             ('Filter', '*'),
             ('StartingIndex', start),
             ('RequestedCount', max_items),
             ('SortCriteria', '')
             ])
 
-        dom = XML.fromstring(really_utf8(response['Result']))
-
         # Get result information
-        out = {'item_list': [], 'search_type': search_type}
+        metadata = {}
         for tag in ['NumberReturned', 'TotalMatches', 'UpdateID']:
-            out[camel_to_underscore(tag)] = int(response[tag])
-
-        # Parse the results
-        for container in dom:
-            item = get_ml_item(container)
-            # Append the item to the list
-            out['item_list'].append(item)
-
-        return out
+            metadata[camel_to_underscore(tag)] = int(response[tag])
+        return response, metadata
 
     def add_uri_to_queue(self, uri):
         """Adds the URI to the queue
 
         :param uri: The URI to be added to the queue
         :type uri: str
         """
         item = URI(uri)
-        self.add_to_queue(item)
+        return self.add_to_queue(item)
 
     def add_to_queue(self, queueable_item):
         """ Adds a queueable item to the queue """
         # Check if teh required attributes are there
         for attribute in ['didl_metadata', 'uri']:
             if not hasattr(queueable_item, attribute):
                 message = 'queueable_item has no attribute {0}'.\
@@ -1403,16 +1561,92 @@
 
         result['total'] = response['TotalMatches']
         result['returned'] = len(favorites)
         result['favorites'] = favorites
 
         return result
 
+    def _update_album_art_to_full_uri(self, item):
+        """Updated the Album Art URI to be fully qualified
+
+        :param item: The item to update the URI for
+        """
+        if not getattr(item, 'album_art_uri', False):
+            return
+
+        # Add on the full album art link, as the URI version
+        # does not include the ipaddress
+        if not item.album_art_uri.startswith(('http:', 'https:')):
+            item.album_art_uri = 'http://' + self.ip_address + ':1400' +\
+                item.album_art_uri
+
+    def create_sonos_playlist(self, title):
+        """ Create a new Sonos' playlist .
+
+        :params title: Name of the playlist
+
+        :returns: An instance of
+            :py:class:`~.soco.data_structures.MLSonosPlaylist`
+
+        """
+        response = self.avTransport.CreateSavedQueue([
+            ('InstanceID', 0),
+            ('Title', title),
+            ('EnqueuedURI', ''),
+            ('EnqueuedURIMetaData', ''),
+            ])
+
+        obj_id = response['AssignedObjectID'].split(':', 2)[1]
+        uri = "file:///jffs/settings/savedqueues.rsq#{0}".format(obj_id)
+
+        return MLSonosPlaylist(uri, title, 'SQ:')
+
+    def add_item_to_sonos_playlist(self, queueable_item, sonos_playlist):
+        """ Adds a queueable item to a Sonos' playlist
+        :param queueable_item: the item to add to the Sonos' playlist
+        :param sonos_playlist: the Sonos' playlist to which the item should
+                               be added
+
+        """
+        # Check if the required attributes are there
+        for attribute in ['didl_metadata', 'uri']:
+            if not hasattr(queueable_item, attribute):
+                message = 'queueable_item has no attribute {0}'.\
+                    format(attribute)
+                raise AttributeError(message)
+        # Get the metadata
+        try:
+            metadata = XML.tostring(queueable_item.didl_metadata)
+        except CannotCreateDIDLMetadata as exception:
+            message = ('The queueable item could not be enqueued, because it '
+                       'raised a CannotCreateDIDLMetadata exception with the '
+                       'following message:\n{0}').format(str(exception))
+            raise ValueError(message)
+        if isinstance(metadata, str):
+            metadata = metadata.encode('utf-8')
+
+        response, _ = self._music_lib_search(sonos_playlist.item_id, 0, 1)
+        update_id = response['UpdateID']
+        self.avTransport.AddURIToSavedQueue([
+            ('InstanceID', 0),
+            ('UpdateID', update_id),
+            ('ObjectID', sonos_playlist.item_id),
+            ('EnqueuedURI', queueable_item.uri),
+            ('EnqueuedURIMetaData', metadata),
+            ('AddAtIndex', 4294967295)  # this field has always this value, we
+                                        # do not known the meaning of this
+                                        # "magic" number.
+            ])
 
 # definition section
 
 RADIO_STATIONS = 0
 RADIO_SHOWS = 1
 
 NS = {'dc': '{http://purl.org/dc/elements/1.1/}',
       'upnp': '{urn:schemas-upnp-org:metadata-1-0/upnp/}',
       '': '{urn:schemas-upnp-org:metadata-1-0/DIDL-Lite/}'}
+# Valid play modes
+PLAY_MODES = ('NORMAL', 'SHUFFLE_NOREPEAT', 'SHUFFLE', 'REPEAT_ALL')
+
+if config.SOCO_CLASS is None:
+    config.SOCO_CLASS = SoCo
```

### Comparing `soco-0.8/soco/plugins/example.py` & `soco-0.9/soco/plugins/example.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,15 +20,15 @@
         accept a soco instance which it passes on to the base class when
         calling super's __init__.  """
         super(ExamplePlugin, self).__init__(soco)
         self.username = username
 
     @property
     def name(self):
-        return 'Example Plugin for {name}'.format(name=self.username)
+        return 'Example Plugin for {0}'.format(self.username)
 
     def music_plugin_play(self):
         """ Play some music
 
         This is just a reimplementation of the ordinary play function, to show
         how we can use the general upnp methods from soco """
```

### Comparing `soco-0.8/soco/plugins/wimp.py` & `soco-0.9/soco/plugins/wimp.py`

 * *Files 2% similar despite different names*

```diff
@@ -235,14 +235,15 @@
         """
         # Check input
         if search_type not in ['artists', 'albums', 'tracks', 'playlists']:
             message = 'The requested search {0} is not valid'\
                 .format(search_type)
             raise ValueError(message)
         # Transform search: tracks -> tracksearch
+        # pylint: disable=bad-format-string
         search_type = '{0}earch'.format(search_type)
         parent_id = SEARCH_PREFIX.format(search_type=search_type,
                                          search=search)
 
         # Perform search
         body = self._search_body(search_type, search, start, max_items)
         headers = _get_header('search')
```

### Comparing `soco-0.8/soco/plugins/__init__.py` & `soco-0.9/soco/plugins/__init__.py`

 * *Files identical despite different names*

### Comparing `soco-0.8/soco/plugins/spotify.py` & `soco-0.9/soco/plugins/spotify.py`

 * *Files identical despite different names*

### Comparing `soco-0.8/soco/data_structures.py` & `soco-0.9/soco/data_structures.py`

 * *Files 14% similar despite different names*

```diff
@@ -3,15 +3,19 @@
 
 
 """ This module contains all the data structures for the information objects
 such as music tracks or genres
 
 """
 
-from __future__ import unicode_literals
+from __future__ import unicode_literals, print_function
+
+import warnings
+warnings.simplefilter('always', DeprecationWarning)
+import textwrap
 
 from .xml import XML
 from .exceptions import CannotCreateDIDLMetadata
 from .utils import really_unicode, camel_to_underscore
 
 
 def ns_tag(ns_id, tag):
@@ -20,19 +24,19 @@
 
     """
     return '{{{0}}}{1}'.format(NS[ns_id], tag)
 
 
 def get_ml_item(xml):
     """Return the music library item that corresponds to xml. The class is
-    identified by getting the parentID and making a lookup in the
-    PARENT_ID_TO_CLASS module variable dictionary.
+    identified by getting the UPNP class making a lookup in the
+    DIDL_CLASS_TO_CLASS module variable dictionary.
 
     """
-    cls = PARENT_ID_TO_CLASS[xml.get('parentID')]
+    cls = DIDL_CLASS_TO_CLASS[xml.find(ns_tag('upnp', 'class')).text]
     return cls.from_xml(xml=xml)
 
 
 def get_ms_item(xml, service, parent_id):
     """Return the music service item that corresponds to xml. The class is
     identified by getting the type from the 'itemType' tag
     """
@@ -63,19 +67,23 @@
 
     def __init__(self):
         """Initialize the content as an empty dict."""
         self.content = {}
 
     def __eq__(self, playable_item):
         """Return the equals comparison result to another ``playable_item``."""
+        if not isinstance(playable_item, MusicInfoItem):
+            return False
         return self.content == playable_item.content
 
     def __ne__(self, playable_item):
         """Return the not equals comparison result to another ``playable_item``
         """
+        if not isinstance(playable_item, MusicInfoItem):
+            return True
         return self.content != playable_item.content
 
     def __repr__(self):
         """Return the repr value for the item.
 
         The repr is on the form::
 
@@ -110,60 +118,58 @@
 
 ###############################################################################
 # MUSIC LIBRARY                                                               #
 ###############################################################################
 class MusicLibraryItem(MusicInfoItem):
     """Abstract class for a queueable item from the music library.
 
-    :ivar parent_id: The parent ID for the music library item is ``None``,
-        since it is a abstract class and it should be overwritten in the sub
-        classes
+    :ivar item_class: The DIDL Lite class for the music library item is
+        ``None``, since it is a abstract class and it should be overwritten in
+        the sub classes
     :ivar _translation: The dictionary-key-to-xml-tag-and-namespace-
         translation used when instantiating a MusicLibraryItems from XML. The
         default value is shown below. This default value applies to most sub
         classes and the rest should overwrite it.
 
         .. code-block:: python
 
             # key: (ns, tag)
             _translation = {
                 'title': ('dc', 'title'),
-                'uri': ('', 'res'),
-                'item_class': ('upnp', 'class')
+                'uri': ('', 'res')
             }
 
     """
-    parent_id = None
+    item_class = None
     # key: (ns, tag)
     _translation = {
         'title': ('dc', 'title'),
-        'uri': ('', 'res'),
-        'item_class': ('upnp', 'class')
+        'uri': ('', 'res')
     }
 
-    def __init__(self, uri, title, item_class, **kwargs):
+    def __init__(self, uri, title, parent_id, **kwargs):
         r"""Initialize the MusicLibraryItem from parameter arguments.
 
         :param uri: The URI for the item
         :param title: The title for the item
-        :param item_class: The UPnP class for the item
+        :param parent_id: The parent ID for the item
         :param \*\*kwargs: Extra information items to form the music library
             item from. Valid keys are ``album``, ``album_art_uri``,
             ``creator`` and ``original_track_number``.
             ``original_track_number`` is an int, all other values are
             unicode objects.
 
         """
         super(MusicLibraryItem, self).__init__()
 
         # Parse the input arguments
-        arguments = {'uri': uri, 'title': title, 'item_class': item_class}
+        arguments = {'uri': uri, 'title': title, 'parent_id': parent_id}
         arguments.update(kwargs)
         for key, value in arguments.items():
-            if key in self._translation:
+            if key in self._translation or key == 'parent_id':
                 self.content[key] = value
             else:
                 raise ValueError(
                     'The key \'{0}\' is not allowed as an argument. Only '
                     'these keys are allowed: {1}'.
                     format(key, str(self._translation.keys())))
 
@@ -175,40 +181,47 @@
             top element usually is a DIDL-LITE item (NS['']) element. Inside
             the item element should be the (namespace, tag_name) elements
             in the dictionary-key-to-xml-tag-and-namespace-translation
             described in the class docstring.
 
         """
         content = {}
+        # Get values from _translation
         for key, value in cls._translation.items():
             result = xml.find(ns_tag(*value))
             if result is None:
                 content[key] = None
+            elif result.text is None:
+                content[key] = None
             else:
                 # The xml objects should contain utf-8 internally
                 content[key] = really_unicode(result.text)
-        args = [content.pop(arg) for arg in ['uri', 'title', 'item_class']]
+
+        # Extract the parent ID
+        content['parent_id'] = xml.get('parentID')
+
+        # Convert type for original track number
         if content.get('original_track_number') is not None:
             content['original_track_number'] = \
                 int(content['original_track_number'])
-        return cls(*args, **content)
+        return cls.from_dict(content)
 
     @classmethod
     def from_dict(cls, content):
         """Return an instance of this class, created from a dict with
         parameters.
 
         :param content: Dict with information for the music library item.
             Required and valid arguments are the same as for the
             ``__init__`` method.
 
         """
         # Make a copy since this method will modify the input dict
         content_in = content.copy()
-        args = [content_in.pop(arg) for arg in ['uri', 'title', 'item_class']]
+        args = [content_in.pop(arg) for arg in ['uri', 'title', 'parent_id']]
         return cls(*args, **content_in)
 
     @property
     def to_dict(self):
         """Get the dict representation of the instance."""
         return self.content.copy()
 
@@ -296,21 +309,21 @@
         return self.content['uri']
 
     @uri.setter
     def uri(self, uri):  # pylint: disable=C0111
         self.content['uri'] = uri
 
     @property
-    def item_class(self):
-        """Get and set the UPnP object class as an unicode object."""
-        return self.content['item_class']
+    def parent_id(self):
+        """Get and set the parent ID."""
+        return self.content['parent_id']
 
-    @item_class.setter
-    def item_class(self, item_class):  # pylint: disable=C0111
-        self.content['item_class'] = item_class
+    @parent_id.setter
+    def parent_id(self, parent_id):  # pylint: disable=C0111
+        self.content['parent_id'] = parent_id
 
 
 class MLTrack(MusicLibraryItem):
     """Class that represents a music library track.
 
     :ivar parent_id: The parent ID for the MLTrack is 'A:TRACKS'
     :ivar _translation: The dictionary-key-to-xml-tag-and-namespace-
@@ -322,48 +335,30 @@
             # key: (ns, tag)
             _translation = {
                 'title': ('dc', 'title'),
                 'creator': ('dc', 'creator'),
                 'album': ('upnp', 'album'),
                 'album_art_uri': ('upnp', 'albumArtURI'),
                 'uri': ('', 'res'),
-                'original_track_number': ('upnp', 'originalTrackNumber'),
-                'item_class': ('upnp', 'class')
+                'original_track_number': ('upnp', 'originalTrackNumber')
             }
 
     """
 
-    parent_id = 'A:TRACKS'
+    item_class = 'object.item.audioItem.musicTrack'
     # name: (ns, tag)
     _translation = {
         'title': ('dc', 'title'),
         'creator': ('dc', 'creator'),
         'album': ('upnp', 'album'),
         'album_art_uri': ('upnp', 'albumArtURI'),
         'uri': ('', 'res'),
-        'original_track_number': ('upnp', 'originalTrackNumber'),
-        'item_class': ('upnp', 'class')
+        'original_track_number': ('upnp', 'originalTrackNumber')
     }
 
-    def __init__(self, uri, title,
-                 item_class='object.item.audioItem.musicTrack', **kwargs):
-        r"""Instantiate the MLTrack item by passing the arguments to the
-        super class :py:meth:`.MusicLibraryItem.__init__`.
-
-        :param uri: The URI for the track
-        :param title: The title of the track
-        :param item_class: The UPnP class for the track. The default value is:
-            ``object.item.audioItem.musicTrack``
-        :param \*\*kwargs: Optional extra information items, valid keys are:
-            ``album``, ``album_art_uri``, ``creator``,
-            ``original_track_number``. ``original_track_number`` is an ``int``.
-            All other values are unicode objects.
-        """
-        MusicLibraryItem.__init__(self, uri, title, item_class, **kwargs)
-
     @property
     def item_id(self):  # pylint: disable=C0103
         """Return the id."""
         out = self.content['uri']
         if 'x-file-cifs' in out:
             # URI's for MusicTracks starts with x-file-cifs, where cifs most
             # likely refer to Common Internet File System. For unknown reasons
@@ -410,57 +405,41 @@
     def original_track_number(self, original_track_number):
         self.content['original_track_number'] = original_track_number
 
 
 class MLAlbum(MusicLibraryItem):
     """Class that represents a music library album.
 
-    :ivar parent_id: The parent ID for the MLTrack is 'A:ALBUM'
+    :ivar item_class: The item_class for MLTrack is
+        'object.container.album.musicAlbum'
     :ivar _translation: The dictionary-key-to-xml-tag-and-namespace-
         translation used when instantiating a MLAlbum from XML. The value is
         shown below
 
         .. code-block :: python
 
             # key: (ns, tag)
             _translation = {
                 'title': ('dc', 'title'),
                 'creator': ('dc', 'creator'),
                 'album_art_uri': ('upnp', 'albumArtURI'),
-                'uri': ('', 'res'),
-                'item_class': ('upnp', 'class')
+                'uri': ('', 'res')
             }
 
     """
 
-    parent_id = 'A:ALBUM'
+    item_class = 'object.container.album.musicAlbum'
     # name: (ns, tag)
     _translation = {
         'title': ('dc', 'title'),
         'creator': ('dc', 'creator'),
         'album_art_uri': ('upnp', 'albumArtURI'),
-        'uri': ('', 'res'),
-        'item_class': ('upnp', 'class')
+        'uri': ('', 'res')
     }
 
-    def __init__(self, uri, title,
-                 item_class='object.container.album.musicAlbum', **kwargs):
-        r"""Instantiate the MLAlbum item by passing the arguments to the
-        super class :py:meth:`.MusicLibraryItem.__init__`.
-
-        :param uri: The URI for the alum
-        :param title: The title of the album
-        :param item_class: The UPnP class for the album. The default value is:
-            ``object.container.album.musicAlbum``
-        :param \*\*kwargs: Optional extra information items, valid keys are:
-            ``album_art_uri`` and ``creator``. All value should be unicode
-            objects.
-        """
-        MusicLibraryItem.__init__(self, uri, title, item_class, **kwargs)
-
     @property
     def creator(self):
         """Get and set the creator as an unicode object."""
         return self.content.get('creator')
 
     @creator.setter
     def creator(self, creator):  # pylint: disable=C0111
@@ -475,198 +454,171 @@
     def album_art_uri(self, album_art_uri):  # pylint: disable=C0111
         self.content['album_art_uri'] = album_art_uri
 
 
 class MLArtist(MusicLibraryItem):
     """Class that represents a music library artist.
 
-    :ivar parent_id: The parent ID for the MLArtist is 'A:ARTIST'
+    :ivar item_class: The item_class for MLArtist is
+        'object.container.person.musicArtist'
     :ivar _translation: The dictionary-key-to-xml-tag-and-namespace-
         translation used when instantiating a MLArtist from XML is inherited
         from :py:class:`.MusicLibraryItem`.
     """
 
-    parent_id = 'A:ARTIST'
+    item_class = 'object.container.person.musicArtist'
 
-    def __init__(self, uri, title,
-                 item_class='object.container.person.musicArtist'):
+    def __init__(self, uri, title, parent_id):
         """Instantiate the MLArtist item by passing the arguments to the
         super class :py:meth:`.MusicLibraryItem.__init__`.
 
         :param uri: The URI for the artist
         :param title: The title of the artist
-        :param item_class: The UPnP class for the artist. The default value is:
-            ``object.container.person.musicArtist``
+        :param item_class: The parent ID for the artist
         """
-        MusicLibraryItem.__init__(self, uri, title, item_class)
-
-
-class MLAlbumArtist(MusicLibraryItem):
-    """Class that represents a music library album artist.
-
-    :ivar parent_id: The parent ID for the MLAlbumArtist is 'A:ALBUMARTIST'
-    :ivar _translation: The dictionary-key-to-xml-tag-and-namespace-
-        translation used when instantiating a MLAlbumArtist from XML is
-        inherited from :py:class:`.MusicLibraryItem`.
-
-    """
-
-    parent_id = 'A:ALBUMARTIST'
-
-    def __init__(self, uri, title,
-                 item_class='object.container.person.musicArtist'):
-        """Instantiate the MLAlbumArtist item by passing the arguments to the
-        super class :py:meth:`.MusicLibraryItem.__init__`.
-
-        :param uri: The URI for the alum artist
-        :param title: The title of the album artist
-        :param item_class: The UPnP class for the album artist. The default
-            value is: ``object.container.person.musicArtist``
-
-        """
-        MusicLibraryItem.__init__(self, uri, title, item_class)
+        MusicLibraryItem.__init__(self, uri, title, parent_id)
 
 
 class MLGenre(MusicLibraryItem):
     """Class that represents a music library genre.
 
-    :ivar parent_id: The parent ID for the MLGenre is 'A:GENRE'
+    :ivar item_class: The item class for the MLGenre is
+        'object.container.genre.musicGenre'
     :ivar _translation: The dictionary-key-to-xml-tag-and-namespace-
         translation used when instantiating a MLGenre from XML is inherited
         from :py:class:`.MusicLibraryItem`.
 
     """
 
-    parent_id = 'A:GENRE'
-
-    def __init__(self, uri, title,
-                 item_class='object.container.genre.musicGenre'):
-        """Instantiate the MLGenre item by passing the arguments to the
-        super class :py:meth:`.MusicLibraryItem.__init__`.
-
-        :param uri: The URI for the genre
-        :param title: The title of the genre
-        :param item_class: The UPnP class for the genre. The default value is:
-            ``object.container.genre.musicGenre``
-
-        """
-        MusicLibraryItem.__init__(self, uri, title, item_class)
+    item_class = 'object.container.genre.musicGenre'
 
 
 class MLComposer(MusicLibraryItem):
     """Class that represents a music library composer.
 
-    :ivar parent_id: The parent ID for the MLComposer is 'A:COMPOSER'
+    :ivar item_class: The item_class for MLComposer is
+        'object.container.person.composer'
     :ivar _translation: The dictionary-key-to-xml-tag-and-namespace-
         translation used when instantiating a MLComposer from XML is inherited
         from :py:class:`.MusicLibraryItem`.
 
     """
 
-    parent_id = 'A:COMPOSER'
-
-    def __init__(self, uri, title,
-                 item_class='object.container.person.composer'):
-        """Instantiate the MLComposer item by passing the arguments to the
-        super class :py:meth:`.MusicLibraryItem.__init__`.
-
-        :param uri: The URI for the composer
-        :param title: The title of the composer
-        :param item_class: The UPnP class for the composer. The default value
-            is: ``object.container.person.composer``
-
-        """
-        MusicLibraryItem.__init__(self, uri, title, item_class)
+    item_class = 'object.container.person.composer'
 
 
 class MLPlaylist(MusicLibraryItem):
     """Class that represents a music library play list.
 
-    :ivar parent_id: The parent ID for the MLPlaylist is 'A:PLAYLIST'
+    :ivar item_class: The item_class for the MLPlaylist is
+        'object.container.playlistContainer'
     :ivar _translation: The dictionary-key-to-xml-tag-and-namespace-
         translation used when instantiating a MLPlaylist from XML is inherited
         from :py:class:`.MusicLibraryItem`.
 
     """
 
-    parent_id = 'A:PLAYLISTS'
-
-    def __init__(self, uri, title,
-                 item_class='object.container.playlistContainer'):
-        """Instantiate the MLPlaylist item by passing the arguments to the
-        super class :py:meth:`.MusicLibraryItem.__init__`.
-
-        :param uri: The URI for the playlist
-        :param title: The title of the playlist
-        :param item_class: The UPnP class for the playlist. The default value
-            is: ``object.container.playlistContainer``
-
-        """
-        MusicLibraryItem.__init__(self, uri, title, item_class)
+    item_class = 'object.container.playlistContainer'
 
     @property
     def item_id(self):  # pylint: disable=C0103
         """Returns the id."""
         out = self.content['uri']
         if 'x-file-cifs' in out:
             out = out.replace('x-file-cifs', 'S')
         else:
-            out = None
+            out = super(MLPlaylist, self).item_id
         return out
 
 
 class MLSonosPlaylist(MusicLibraryItem):
     """ Class that represents a sonos playlist.
 
-    :ivar parent_id: The parent ID for the MLSonosPlaylist is 'SQ:'
+    :ivar item_class: The item_class for MLSonosPlaylist is
+        'object.container.playlistContainer'
     :ivar _translation: The dictionary-key-to-xml-tag-and-namespace-
         translation used when instantiating MLSonosPlaylist from
         XML is inherited from :py:class:`.MusicLibraryItem`.
 
     """
 
-    parent_id = 'SQ:'
+    item_class = 'object.container.playlistContainer'
 
-    def __init__(self, uri, title,
-                 item_class='object.container.playlistContainer'):
-        """ Instantiate the MLSonosPlaylist item by passing the arguments to
-        the super class :py:meth:`.MusicLibraryItem.__init__`.
-
-        :param uri: The URI for the playlist
-        :param title: The title of the playlist
-        :param item_class: The UPnP class for the playlist. The default value
-            is: ``object.container.playlistContainer``
-
-        """
-        MusicLibraryItem.__init__(self, uri, title, item_class)
+    @property
+    def item_id(self):  # pylint: disable=C0103
+        """Returns the id."""
+        out = 'SQ:' + super(MLSonosPlaylist, self).item_id
+        return out
 
 
 class MLShare(MusicLibraryItem):
     """Class that represents a music library share.
 
-    :ivar parent_id: The parent ID for the MLShare is 'S:'
+    :ivar item_class: The item_class for the MLShare is 'object.container'
     :ivar _translation: The dictionary-key-to-xml-tag-and-namespace-
         translation used when instantiating a MLShare from XML is inherited
         from :py:class:`.MusicLibraryItem`.
 
     """
 
-    parent_id = 'S:'
+    item_class = 'object.container'
+
+
+class MLCategory(MusicLibraryItem):
+    """Class that represents a music library category.
+
+    :ivar item_class: The item_class for the MLCategory is 'object.container'
+    :ivar _translation: The dictionary-key-to-xml-tag-and-namespace-
+        translation used when instantiating a MLCategory from XML is inherited
+        from :py:class:`.MusicLibraryItem`.
+
+    """
+
+    item_class = 'object.container'
+
+
+class MLAlbumList(MusicLibraryItem):
+    """Class that represents a music library album list.
+
+    :ivar item_class: The item_class for MLAlbumList is
+        'object.container.albumlist'
+    :ivar _translation: The dictionary-key-to-xml-tag-and-namespace-
+        translation used when instantiating a MLAlbumList from XML is inherited
+        from :py:class:`.MusicLibraryItem`.
+
+    """
+
+    item_class = 'object.container.albumlist'
+
+
+class MLSameArtist(MusicLibraryItem):
+    """Class that represents all by the artist.
+
+    This type is returned by browsing an artist or a composer
+
+    :ivar item_class: The item_class for MLSameArtist is
+        'object.container.playlistContainer.sameArtist'
+    :ivar _translation: The dictionary-key-to-xml-tag-and-namespace-
+        translation used when instantiating a MLSameArtist from XML is
+        inherited from :py:class:`.MusicLibraryItem`.
+
+    """
+
+    item_class = 'object.container.playlistContainer.sameArtist'
 
-    def __init__(self, uri, title, item_class='object.container'):
-        """Instantiate the MLShare item by passing the arguments to the
+    def __init__(self, uri, title, parent_id):
+        """Instantiate the MLSameArtist item by passing the arguments to the
         super class :py:meth:`.MusicLibraryItem.__init__`.
 
-        :param uri: The URI for the share
-        :param title: The title of the share
-        :param item_class: The UPnP class for the share. The default value is:
-            ``object.container``
+        :param uri: The URI for the composer
+        :param title: The title of the composer
+        :param item_class: The parent ID for the composer
 
         """
-        MusicLibraryItem.__init__(self, uri, title, item_class)
+        MusicLibraryItem.__init__(self, uri, title, parent_id)
 
 
 ###############################################################################
 # MUSIC LIBRARY                                                               #
 ###############################################################################
 class URI(MusicInfoItem):
     """General purpose class that represents a audio file URI"""
@@ -1354,19 +1306,123 @@
     def __init__(self, title, item_id, extended_id, service_id, **kwargs):
         content = {'title': title, 'item_id': item_id,
                    'extended_id': extended_id, 'service_id': service_id}
         content.update(kwargs)
         super(MSCollection, self).__init__(**content)
 
 
-PARENT_ID_TO_CLASS = {'A:TRACKS': MLTrack, 'A:ALBUM': MLAlbum,
-                      'A:ARTIST': MLArtist, 'A:ALBUMARTIST': MLAlbumArtist,
-                      'A:GENRE': MLGenre, 'A:COMPOSER': MLComposer,
-                      'A:PLAYLISTS': MLPlaylist, 'S:': MLShare,
-                      'SQ:': MLSonosPlaylist}
+###############################################################################
+# CONTAINERS                                                                  #
+###############################################################################
+class ListOfMusicInfoItems(list):
+    """Abstract container class for a list of music information items"""
+
+    def __init__(self, items, number_returned, total_matches, update_id):
+        super(ListOfMusicInfoItems, self).__init__(items)
+        self._metadata = {
+            'item_list': list(items),
+            'number_returned': number_returned,
+            'total_matches': total_matches,
+            'update_id': update_id,
+        }
+
+    def __getitem__(self, key):
+        """Legacy get metadata by string key or list item(s) by index
+
+        DEPRECATION: This overriding form of __getitem__ will be removed in
+        the 3rd release after 0.8. The metadata can be fetched via the named
+        attributes
+        """
+        if key in self._metadata:
+            if key == 'item_list':
+                message = """
+                Calling [\'item_list\'] on search results to obtain the objects
+                is no longer necessary, since the object returned from searches
+                now is a list. This deprecated way of getting the items will
+                be removed from the third release after 0.8."""
+            else:
+                message = """
+                Getting metadata items by indexing the search result like a
+                dictionary [\'{0}\'] is deprecated. Please use the named
+                attribute {1}.{0} instead. The deprecated way of retrieving the
+                metadata will be removed from the third release after
+                0.8""".format(key, self.__class__.__name__)
+            message = textwrap.dedent(message).replace('\n', ' ').lstrip()
+            warnings.warn(message, DeprecationWarning, stacklevel=2)
+            return self._metadata[key]
+        else:
+            return super(ListOfMusicInfoItems, self).__getitem__(key)
+
+    @property
+    def number_returned(self):
+        """The number of returned matches"""
+        return self._metadata['number_returned']
+
+    @property
+    def total_matches(self):
+        """The number of total matches"""
+        return self._metadata['total_matches']
+
+    @property
+    def update_id(self):
+        """The update ID"""
+        return self._metadata['update_id']
+
+
+class SearchResult(ListOfMusicInfoItems):
+    """Container class that represents a search or browse result
+
+    (browse is just a special case of search)
+    """
+
+    def __init__(self, items, search_type, number_returned,
+                 total_matches, update_id):
+        super(SearchResult, self).__init__(
+            items, number_returned, total_matches, update_id
+        )
+        self._metadata['search_type'] = search_type
+
+    def __repr__(self):
+        return '{0}(items={1}, search_type=\'{2}\')'.format(
+            self.__class__.__name__,
+            super(SearchResult, self).__repr__(),
+            self.search_type)
+
+    @property
+    def search_type(self):
+        """The search type"""
+        return self._metadata['search_type']
+
+
+class Queue(ListOfMusicInfoItems):
+    """Container class that represents a queue"""
+
+    def __init__(self, items, number_returned, total_matches, update_id):
+        super(Queue, self).__init__(
+            items, number_returned, total_matches, update_id
+        )
+
+    def __repr__(self):
+        return '{0}(items={1})'.format(
+            self.__class__.__name__,
+            super(Queue, self).__repr__(),
+            )
+
+
+DIDL_CLASS_TO_CLASS = {'object.item.audioItem.musicTrack': MLTrack,
+                       'object.container.album.musicAlbum': MLAlbum,
+                       'object.container.person.musicArtist': MLArtist,
+                       'object.container.genre.musicGenre': MLGenre,
+                       'object.container.person.composer': MLComposer,
+                       'object.container.playlistContainer': MLPlaylist,
+                       'object.container': MLCategory,
+                       'object.container.albumlist': MLAlbumList,
+                       'object.container.playlistContainer.sameArtist':
+                           MLSameArtist}
+
 
 MS_TYPE_TO_CLASS = {'artist': MSArtist, 'album': MSAlbum, 'track': MSTrack,
                     'albumList': MSAlbumList, 'favorites': MSFavorites,
                     'collection': MSCollection, 'playlist': MSPlaylist,
                     'artistTrackList': MSArtistTracklist}
 
 NS = {
```

### Comparing `soco-0.8/soco/utils.py` & `soco-0.9/soco/cache.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,118 +1,91 @@
 # -*- coding: utf-8 -*-
+""" Caching """
 
-""" Provides general utility functions to be used across modules """
+from __future__ import unicode_literals
 
-from __future__ import unicode_literals, absolute_import
-
-import re
 import threading
 from time import time
-from .compat import StringType, UnicodeType, dumps
-
-
-def really_unicode(in_string):
-    """
-    Ensures s is returned as a unicode string and not just a string through
-    a series of progressively relaxed decodings
 
-    """
-    if type(in_string) is StringType:
-        for args in (('utf-8',), ('latin-1',), ('ascii', 'replace')):
-            try:
-                # pylint: disable=star-args
-                in_string = in_string.decode(*args)
-                break
-            except UnicodeDecodeError:
-                continue
-    if type(in_string) is not UnicodeType:
-        raise ValueError('%s is not a string at all.' % in_string)
-    return in_string
-
-
-def really_utf8(in_string):
-    """ First decodes s via really_unicode to ensure it can successfully be
-    encoded as utf-8 This is required since just calling encode on a string
-    will often cause python to perform a coerced strict auto-decode as ascii
-    first and will result in a UnicodeDecodeError being raised After
-    really_unicode returns a safe unicode string, encode as 'utf-8' and return
-    the utf-8 encoded string.
+from .compat import dumps
+from soco import config
 
-    """
-    return really_unicode(in_string).encode('utf-8')
 
+class _BaseCache(object):
+    """A base class for the cache.
 
-FIRST_CAP_RE = re.compile('(.)([A-Z][a-z]+)')
-ALL_CAP_RE = re.compile('([a-z0-9])([A-Z])')
+    Does nothing by itself."""
+    # pylint: disable=no-self-use, unused-argument
+    def __init__(self, default_timeout=0):
+        super(_BaseCache, self).__init__()
+        self._cache = {}
+        # : The default caching interval in seconds.
+        self.default_timeout = default_timeout
+        #: Is the cache enabled? True or False
+        self.enabled = True
 
+    def get(self, *args, **kwargs):
+        """
+        Get an item from the cache for this combination of args and kwargs.
+        Returns None, indicating that no item has been found.
+        """
+        return None
 
-def camel_to_underscore(string):
-    """ Convert camelcase to lowercase and underscore
-    Recipy from http://stackoverflow.com/a/1176023
-    """
-    string = FIRST_CAP_RE.sub(r'\1_\2', string)
-    return ALL_CAP_RE.sub(r'\1_\2', string).lower()
+    def put(self, *args, **kwargs):
+        """
+        Put an item into the cache, for this combination of args and
+        kwargs.
+        """
+        pass
 
+    def delete(self, *args, **kwargs):
+        """
+        Delete an item from the cache for this combination of args and
+        kwargs.
+        """
+        pass
 
-def prettify(unicode_text):
-    """Return a pretty-printed version of a unicode XML string. Useful for
-    debugging.
+    def clear(self):
+        """
+        Empty the whole cache.
+        """
+        pass
 
-    """
-    import xml.dom.minidom
-    reparsed = xml.dom.minidom.parseString(unicode_text.encode('utf-8'))
-    return reparsed.toprettyxml(indent="  ", newl="\n")
 
+class NullCache(_BaseCache):
+    """A cache which does nothing. Useful for debugging."""
+    pass
 
-class TimedCache(object):
 
+class TimedCache(_BaseCache):
     """ A simple thread-safe cache for caching method return values
 
     At present, the cache can theoretically grow and grow, since entries are
     not automatically purged, though in practice this is unlikely since there
     are not that many different combinations of arguments in the places where
     it is used in SoCo, so not that many different cache entries will be
     created. If this becomes a problem, use a thread and timer to purge the
     cache, or rewrite this to use LRU logic!
 
     """
 
     def __init__(self, default_timeout=0):
         super(TimedCache, self).__init__()
-        self._cache = {}
         # A thread lock for the cache
         self._cache_lock = threading.Lock()
-        #: The default caching interval in seconds. Set to 0
-        #: to disable the cache by default
-        self.default_timeout = default_timeout
-
-    @staticmethod
-    def make_key(args, kwargs):
-        """
-        Generate a unique, hashable, representation of the args and kwargs
-
-        """
-        # This is not entirely straightforward, since args and kwargs may
-        # contain mutable items and unicode. Possibiities include using
-        # __repr__, frozensets, and code from Py3's LRU cache. But pickle
-        # works, and although it is not as fast as some methods, it is good
-        # enough at the moment
-        cache_key = dumps((args, kwargs))
-        return cache_key
 
     def get(self, *args, **kwargs):
-
-        """
-
-        Get an item from the cache for this combination of args and kwargs.
+        """Get an item from the cache for this combination of args and kwargs.
 
         Return None if no unexpired item is found. This means that there is no
         point storing an item in the cache if it is None.
 
         """
+        if not self.enabled:
+            return None
         # Look in the cache to see if there is an unexpired item. If there is
         # we can just return the cached result.
         cache_key = self.make_key(args, kwargs)
         # Lock and load
         with self._cache_lock:
             if cache_key in self._cache:
                 expirytime, item = self._cache[cache_key]
@@ -122,24 +95,25 @@
                 else:
                     # An expired item is present - delete it
                     del self._cache[cache_key]
         # Nothing found
         return None
 
     def put(self, item, *args, **kwargs):
-
         """ Put an item into the cache, for this combination of args and
         kwargs.
 
         If `timeout` is specified as one of the keyword arguments, the item
         will remain available for retrieval for `timeout` seconds. If `timeout`
         is None or not specified, the default cache timeout for this cache will
         be used. Specify a `timeout` of 0 (or ensure that the default timeout
         for this cache is 0) if this item is not to be cached."""
 
+        if not self.enabled:
+            return
         # Check for a timeout keyword, store and remove it.
         timeout = kwargs.pop('timeout', None)
         if timeout is None:
             timeout = self.default_timeout
         cache_key = self.make_key(args, kwargs)
         # Store the item, along with the time at which it will expire
         with self._cache_lock:
@@ -155,7 +129,37 @@
             except KeyError:
                 pass
 
     def clear(self):
         """Empty the whole cache"""
         with self._cache_lock:
             self._cache.clear()
+
+    @staticmethod
+    def make_key(*args, **kwargs):
+        """
+        Generate a unique, hashable, representation of the args and kwargs
+
+        """
+        # This is not entirely straightforward, since args and kwargs may
+        # contain mutable items and unicode. Possibilities include using
+        # __repr__, frozensets, and code from Py3's LRU cache. But pickle
+        # works, and although it is not as fast as some methods, it is good
+        # enough at the moment
+        cache_key = dumps((args, kwargs))
+        return cache_key
+
+
+class Cache(_BaseCache):
+    """A factory class which returns an instance of a cache subclass.
+
+    If config.CACHE_ENABLED is False, the dummy inactive cache will be returned
+    """
+
+    def __new__(cls, *args, **kwargs):
+        if config.CACHE_ENABLED:
+            new_cls = TimedCache
+        else:
+            new_cls = NullCache
+        instance = super(Cache, cls).__new__(new_cls)
+        instance.__init__(*args, **kwargs)
+        return instance
```

### Comparing `soco-0.8/soco/services.py` & `soco-0.9/soco/services.py`

 * *Files 2% similar despite different names*

```diff
@@ -40,31 +40,32 @@
 
 
 from collections import namedtuple
 from xml.sax.saxutils import escape
 import logging
 
 import requests
+from .cache import Cache
 from .exceptions import SoCoUPnPException, UnknownSoCoException
-from .utils import prettify, TimedCache
+from .utils import prettify
 from .events import Subscription
 from .xml import XML
 
 log = logging.getLogger(__name__)  # pylint: disable=C0103
 # logging.basicConfig()
 # log.setLevel(logging.INFO)
 
 Action = namedtuple('Action', 'name, in_args, out_args')
 Argument = namedtuple('Argument', 'name, vartype')
 
 # A shared cache for ZoneGroupState. Each zone has the same info, so when a
 # SoCo instance is asked for group info, we can cache it and return it when
 # another instance is asked. To do this we need a cache to be shared between
 # instances
-zone_group_state_shared_cache = TimedCache()
+zone_group_state_shared_cache = Cache()
 
 
 # pylint: disable=too-many-instance-attributes
 class Service(object):
     """ An class representing a UPnP service. The base class for all Sonos
     Service classes
 
@@ -101,15 +102,15 @@
         # Service control protocol description
         self.scpd_url = '/xml/{0}{1}.xml'.format(
             self.service_type, self.version)
         # Eventing subscription
         self.event_subscription_url = '/{0}/Event'.format(self.service_type)
         #: A cache for storing the result of network calls. By default, this is
         #: TimedCache(default_timeout=0). See :class:`TimedCache`
-        self.cache = TimedCache(default_timeout=0)
+        self.cache = Cache(default_timeout=0)
         log.debug(
             "Created service %s, ver %s, id %s, base_url %s, control_url %s",
             self.service_type, self.version, self.service_id, self.base_url,
             self.control_url)
 
         # From table 3.3 in
         # http://upnp.org/specs/arch/UPnP-arch-DeviceArchitecture-v1.1.pdf
@@ -191,14 +192,15 @@
 
         """
         if args is None:
             args = []
 
         tags = []
         for name, value in args:
+            # pylint: disable=bad-format-string
             tag = "<{name}>{value}</{name}>".format(
                 name=name, value=escape("%s" % value, {'"': "&quot;"}))
             # % converts to unicode because we are using unicode literals.
             # Avoids use of 'unicode' function which does not exist in python 3
             tags.append(tag)
 
         xml = "".join(tags)
@@ -277,14 +279,15 @@
         #           <argumentName>in arg value</argumentName>
         #           ... other in args and their values go here, if any
         #       </u:actionName>
         #   </s:Body>
         # </s:Envelope>
 
         arguments = self.wrap_arguments(args)
+        # pylint: disable=bad-format-string
         body = self.soap_body_template.format(
             arguments=arguments, action=action, service_type=self.service_type,
             version=self.version)
         soap_action_template = \
             "urn:schemas-upnp-org:service:{service_type}:{version}#{action}"
         soap_action = soap_action_template.format(
             service_type=self.service_type, version=self.version,
@@ -409,33 +412,36 @@
                 error_xml=xml_error
                 )
         else:
             # Unknown error, so just return the entire response
             log.error("Unknown error received from %s", self.soco.ip_address)
             raise UnknownSoCoException(xml_error)
 
-    def subscribe(self, requested_timeout=None, event_queue=None):
+    def subscribe(
+            self, requested_timeout=None, auto_renew=False, event_queue=None):
         """Subscribe to the service's events.
 
         If requested_timeout is provided, a subscription valid for that number
         of seconds will be requested, but not guaranteed. Check
         :attrib:`Subscription.timeout` on return to find out what period of
-        validity is actually allocated.
+        validity is actually allocated. If auto_renew is True, the subscription
+        will be automatically renewed just before it expires, if possible
 
         event_queue is a thread-safe queue object onto which events will be
         put. If None, a Queue object will be created and used.
 
         Returns a Subscription object, representing the new subscription
 
         To unsubscribe, call the `unsubscribe` method on the returned object.
 
         """
         subscription = Subscription(
             self, event_queue)
-        subscription.subscribe(requested_timeout=requested_timeout)
+        subscription.subscribe(
+            requested_timeout=requested_timeout, auto_renew=auto_renew)
         return subscription
 
     def _update_cache_on_event(self, event):
         """ Update the cache when an event is received.
 
         This will be called before an event is put onto the event queue. Events
         will often indicate that the Sonos device's state has changed, so this
@@ -526,14 +532,18 @@
                 yield (name, vartype)
 
 
 class AlarmClock(Service):
     """ Sonos alarm service, for setting and getting time and alarms. """
     def __init__(self, soco):
         super(AlarmClock, self).__init__(soco)
+        self.UPNP_ERRORS.update(
+            {
+                801: 'Already an alarm for this time',
+            })
 
 
 class MusicServices(Service):
     """ Sonos music services service, for functions related to 3rd party
     music services. """
     def __init__(self, soco):
         super(MusicServices, self).__init__(soco)
```

### Comparing `soco-0.8/soco/__init__.py` & `soco-0.9/soco/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 # There is no need for all strings here to be unicode, and Py2 cannot import
 # modules with unicode names
 # https://github.com/SoCo/SoCo/issues/98
 # from __future__ import unicode_literals
 
 # Will be parsed by setup.py to determine package metadata
 __author__ = 'The SoCo-Team <python-soco@googlegroups.com>'
-__version__ = '0.8'
+__version__ = '0.9'
 __website__ = 'https://github.com/SoCo/SoCo'
 __license__ = 'MIT License'
 
 
 from .core import discover, SoCo, SonosDiscovery
 from .exceptions import SoCoException, UnknownSoCoException
```

### Comparing `soco-0.8/soco/groups.py` & `soco-0.9/soco/groups.py`

 * *Files identical despite different names*

### Comparing `soco-0.8/soco/exceptions.py` & `soco-0.9/soco/exceptions.py`

 * *Files identical despite different names*

### Comparing `soco-0.8/soco/compat.py` & `soco-0.9/soco/compat.py`

 * *Files 0% similar despite different names*

```diff
@@ -18,15 +18,15 @@
     from SimpleHTTPServer import SimpleHTTPRequestHandler  # nopep8
     from urllib2 import urlopen, URLError  # nopep8
     from urllib import quote_plus  # nopep8
     import SocketServer as socketserver  # nopep8
     from Queue import Queue  # nopep8
     from types import StringType, UnicodeType  # nopep8
 
-try:  # python 2.7 - this has to be done the other way rund
+try:  # python 2.7 - this has to be done the other way round
     from cPickle import dumps  # nopep8
 except ImportError:  # python 3
     from pickle import dumps  # nopep8
 
 # Support Python 2.6
 try:  # Python 2.7+
     from logging import NullHandler  # nopep8
```

### Comparing `soco-0.8/README.rst` & `soco-0.9/README.rst`

 * *Files identical despite different names*

### Comparing `soco-0.8/PKG-INFO` & `soco-0.9/soco.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: soco
-Version: 0.8
+Version: 0.9
 Summary:  SoCo (Sonos Controller) is a simple library to control Sonos speakers 
 Home-page: https://github.com/SoCo/SoCo
 Author: The SoCo-Team
 Author-email: python-soco@googlegroups.com
 License: MIT License
 Description: SoCo
         ====
```

### Comparing `soco-0.8/unittest/execute_unittests.py` & `soco-0.9/unittest/execute_unittests.py`

 * *Files identical despite different names*

### Comparing `soco-0.8/unittest/test_integration.py` & `soco-0.9/unittest/test_integration.py`

 * *Files identical despite different names*

### Comparing `soco-0.8/unittest/soco_unittest.py` & `soco-0.9/unittest/soco_unittest.py`

 * *Files identical despite different names*

### Comparing `soco-0.8/unittest/test_events.py` & `soco-0.9/unittest/test_events.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 # -*- coding: utf-8 -*-
 """ Tests for the services module """
 
 from __future__ import unicode_literals
-from soco.events import parse_event_xml
+import pytest
+from soco.events import parse_event_xml, Event
 
 DUMMY_EVENT = """
 <e:propertyset xmlns:e="urn:schemas-upnp-org:event-1-0">
     <e:property>
         <ZoneGroupState>&lt;ZoneGroups&gt;&lt;
             ZoneGroup Coordinator="RINCON_000XXX01400"
             ID="RINCON_000XXX1400:56"&gt;&lt;
@@ -58,13 +59,32 @@
     <e:property>
         <ZonePlayerUUIDsInGroup>RINCON_000XXX1400</ZonePlayerUUIDsInGroup>
     </e:property>
 </e:propertyset>
 """
 
 
+def test_event_object():
+    # Basic initialisation
+    dummy_event = Event('123', '456', 'dummy', {'zone': 'kitchen'})
+    assert dummy_event.sid == '123'
+    assert dummy_event.seq == '456'
+    assert dummy_event.service =='dummy'
+    assert dummy_event.variables == {'zone':'kitchen'}
+    # attribute access
+    assert dummy_event.zone == 'kitchen'
+    # Should not access non-existent attributes
+    with pytest.raises(AttributeError):
+        var = dummy_event.non_existent
+    # Should be read only
+    with pytest.raises(TypeError):
+        dummy_event.new_var = 4
+    with pytest.raises(TypeError):
+        dummy_event.sid = 4
+
+
 def test_event_parsing():
     event_dict = parse_event_xml(DUMMY_EVENT)
-    assert event_dict['ZoneGroupState']
-    assert event_dict['AlarmRunSequence'] == 'RINCON_000EXXXXXX0:56:0'
-    assert event_dict['ZoneGroupID'] == "RINCON_000XXXX01400:57"
+    assert event_dict['zone_group_state']
+    assert event_dict['alarm_run_sequence'] == 'RINCON_000EXXXXXX0:56:0'
+    assert event_dict['zone_group_id'] == "RINCON_000XXXX01400:57"
```

### Comparing `soco-0.8/unittest/test_utils.py` & `soco-0.9/unittest/test_cache.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,17 +1,25 @@
 # -*- coding: utf-8 -*-
-""" Tests for the utils module """
+""" Tests for the cache module """
 
 from __future__ import unicode_literals
-from soco.utils import TimedCache
+from soco.cache import Cache, NullCache, TimedCache
+
+def test_instance_creation():
+    assert isinstance(Cache(), TimedCache)
+    from soco import config
+    config.CACHE_ENABLED = False
+    assert isinstance(Cache(), NullCache)
+    config.CACHE_ENABLED = True
+
 
 def test_cache_put_get():
     "Test putting items into, and getting them from, the cache"
     from time import sleep
-    cache = TimedCache()
+    cache = Cache()
     cache.put("item", 'some', kw='args', timeout=3)
     assert not cache.get('some', 'otherargs') == "item"
     assert cache.get('some', kw='args') == "item"
     sleep(2)
     assert cache.get('some', kw='args') == "item"
     sleep(2)
     assert not cache.get('some', kw='args') == "item"
@@ -20,34 +28,44 @@
     cache.put("item", 'some', 'args', and_a='keyword', timeout=3)
     assert cache.get('some', 'args', and_a='keyword') == "item"
     assert not cache.get(
         'some', 'otherargs', and_a='keyword') == "item"
 
 def test_cache_clear_del():
     "Test removal of items and clearing the cache"
-    cache = TimedCache()
+    cache = Cache()
     cache.put("item", "some", kw="args", timeout=2)
     # Check it's there
     assert cache.get('some', kw='args') == "item"
     # delete it
     cache.delete('some', kw='args')
     assert not cache.get('some', kw='args') == "item"
     # put it back
     cache.put("item", "some", kw="args", timeout=3)
     cache.clear()
     assert not cache.get('some', kw='args') == "item"
 
 def test_with_typical_args():
-    cache = TimedCache()
+    cache = Cache()
     cache.put ("result", 'SetAVTransportURI', [
             ('InstanceID', 1),
             ('CurrentURI', 'URI2'),
             ('CurrentURIMetaData', 'abcd'),
             ('Unicode', 'μИⅠℂ☺ΔЄ💋')
             ], timeout=3)
     assert cache.get('SetAVTransportURI', [
             ('InstanceID', 1),
             ('CurrentURI', 'URI2'),
             ('CurrentURIMetaData', 'abcd'),
             ('Unicode', 'μИⅠℂ☺ΔЄ💋')
             ]) == "result"
 
+def test_cache_disable():
+    cache = Cache()
+    assert cache.enabled == True
+    cache.enabled = False
+    cache.put("item", 'args', timeout=3)
+    assert cache.get('args') == None
+    # Check it's there
+    assert cache.get('some', kw='args') == None
+
+
```

### Comparing `soco-0.8/unittest/conftest.py` & `soco-0.9/unittest/conftest.py`

 * *Files identical despite different names*

### Comparing `soco-0.8/unittest/test_data_structures.py` & `soco-0.9/unittest/test_data_structures.py`

 * *Files 13% similar despite different names*

```diff
@@ -26,15 +26,17 @@
     <upnp:class>{item_class}</upnp:class>
     <desc id="cdudn"
      nameSpace="urn:schemas-rinconnetworks-com:metadata-1-0/">
     RINCON_AssociatedZPUDN</desc></item></DIDL-Lite>
     """
 XML_TEMPLATE = textwrap.dedent(XML_TEMPLATE).replace('\n', '').strip()
 
-# Example XML and the content dict to compare with
+##############################################################################
+# Example XML and the content dict to compare with for ML items              #
+##############################################################################
 TRACK_XML = """
 <item xmlns="urn:schemas-upnp-org:metadata-1-0/DIDL-Lite/"
  xmlns:dc="http://purl.org/dc/elements/1.1/"
  xmlns:upnp="urn:schemas-upnp-org:metadata-1-0/upnp/"
  id="S://TLE-SERVER/share/ogg/Mozart%20-%20Orpheus%20Orchestra_convert/
 5-Mozart-...%20-II%20Adagio.ogg" parentID="A:TRACKS" restricted="true">
   <res protocolInfo="x-file-cifs:*:application/ogg:*">x-file-cifs://TLE-SERVER/
@@ -56,15 +58,15 @@
     'uri': 'x-file-cifs://TLE-SERVER/\nshare/ogg/Mozart'
            '%20-%20Orpheus%20Orchestra_convert/5-Mozart-...%20-II%20'
            '\nAdagio.ogg',
     'album_art_uri': '/getaa?u=x-file-cifs%3a%2f%2fTLE-SERVER'
                      '\n%2fshare%2fogg%2fMozart%2520-%2520Orpheus%2520'
                      'Orchestra_convert%2f5-Mozart-\n...%2520-II%2520'
                      'Adagio.ogg&v=2',
-    'item_class': 'object.item.audioItem.musicTrack',
+    'parent_id': 'A:TRACKS',
     'original_track_number': 5}
 ALBUM_XML = """
 <container xmlns="urn:schemas-upnp-org:metadata-1-0/DIDL-Lite/"
  xmlns:dc="http://purl.org/dc/elements/1.1/"
  xmlns:upnp="urn:schemas-upnp-org:metadata-1-0/upnp/"
  id="A:ALBUM/...and%20Justice%20for%20All" parentID="A:ALBUM"
  restricted="true">
@@ -76,15 +78,15 @@
   <upnp:albumArtURI>/getaa?u=x-file-cifs%3a%2f%2fTLE-SERVER%2fshare%2fogg%2f
 Metallica%2520-%2520and%2520Justice%2520for%2520All%2f01%2520-%2520Blackened.
 ogg&amp;v=2</upnp:albumArtURI>
 </container>"""
 ALBUM_XML = ALBUM_XML.replace('\n', '')
 ALBUM_DICT = {
     'title': '...and Justice for All',
-    'item_class': 'object.container.album.musicAlbum',
+    'parent_id': 'A:ALBUM',
     'uri': 'x-rincon-playlist:RINCON_000E5884455C01400#A:ALBUM/...and%20'
            'Justice%20for%20All',
     'album_art_uri': '/getaa?u=x-file-cifs%3a%2f%2fTLE-SERVER%2fshare%2fogg'
                      '%2fMetallica%2520-%2520and%2520Justice%2520for%2520All'
                      '%2f01%2520-%2520Blackened.ogg&v=2',
     'creator': 'Metallica'}
 ARTIST_XML = """
@@ -95,49 +97,31 @@
   <dc:title>10 Years</dc:title>
   <upnp:class>object.container.person.musicArtist</upnp:class>
   <res protocolInfo="x-rincon-playlist:*:*:*">x-rincon-playlist:
 RINCON_000E5884455C01400#A:ARTIST/10%20Years</res>
 </container>"""
 ARTIST_XML = ARTIST_XML.replace('\n', '')
 ARTIST_DICT = {
-    'item_class': 'object.container.person.musicArtist',
+    'parent_id': 'A:ARTIST',
     'uri': 'x-rincon-playlist:RINCON_000E5884455C01400#A:ARTIST/10%20Years',
     'title': '10 Years'
 }
-ALBUMARTIST_XML = """
-<container xmlns="urn:schemas-upnp-org:metadata-1-0/DIDL-Lite/"
- xmlns:dc="http://purl.org/dc/elements/1.1/"
- xmlns:upnp="urn:schemas-upnp-org:metadata-1-0/upnp/"
- id="A:ALBUMARTIST/3%20Doors%20Down" parentID="A:ALBUMARTIST"
- restricted="true">
-  <dc:title>3 Doors Down</dc:title>
-  <upnp:class>object.container.person.musicArtist</upnp:class>
-  <res protocolInfo="x-rincon-playlist:*:*:*">x-rincon-playlist:RINCON_
-000E5884455C01400#A:ALBUMARTIST/3%20Doors%20Down</res>
-</container>"""
-ALBUMARTIST_XML = ALBUMARTIST_XML.replace('\n', '')
-ALBUMARTIST_DICT = {
-    'item_class': 'object.container.person.musicArtist',
-    'uri': 'x-rincon-playlist:RINCON_000E5884455C01400#A:ALBUMARTIST/'
-           '3%20Doors%20Down',
-    'title': '3 Doors Down'
-}
 GENRE_XML = """
 <container xmlns="urn:schemas-upnp-org:metadata-1-0/DIDL-Lite/"
  xmlns:dc="http://purl.org/dc/elements/1.1/"
  xmlns:upnp="urn:schemas-upnp-org:metadata-1-0/upnp/" id="A:GENRE/Acid"
  parentID="A:GENRE" restricted="true">
   <dc:title>Acid</dc:title>
   <upnp:class>object.container.genre.musicGenre</upnp:class>
   <res protocolInfo="x-rincon-playlist:*:*:*">x-rincon-playlist:
 RINCON_000E5884455C01400#A:GENRE/Acid</res>
 </container>"""
 GENRE_XML = GENRE_XML.replace('\n', '')
 GENRE_DICT = {
-    'item_class': 'object.container.genre.musicGenre',
+    'parent_id': 'A:GENRE',
     'uri': 'x-rincon-playlist:RINCON_000E5884455C01400#A:GENRE/Acid',
     'title': 'Acid'
 }
 COMPOSER_XML = """
 <container xmlns="urn:schemas-upnp-org:metadata-1-0/DIDL-Lite/"
  xmlns:dc="http://purl.org/dc/elements/1.1/"
  xmlns:upnp="urn:schemas-upnp-org:metadata-1-0/upnp/"
@@ -147,15 +131,15 @@
   <upnp:class>object.container.person.composer</upnp:class>
   <res protocolInfo="x-rincon-playlist:*:*:*">x-rincon-playlist:RINCON_
 000E5884455C01400#A:COMPOSER/A.%20Kiedis%2fFlea%2fJ.%20Frusciante%2fC.%20
 Smith</res>
 </container>"""
 COMPOSER_XML = COMPOSER_XML.replace('\n', '')
 COMPOSER_DICT = {
-    'item_class': 'object.container.person.composer',
+    'parent_id': 'A:COMPOSER',
     'uri': 'x-rincon-playlist:RINCON_000E5884455C01400#A:COMPOSER/'
            'A.%20Kiedis%2fFlea%2fJ.%20Frusciante%2fC.%20Smith',
     'title': 'A. Kiedis/Flea/J. Frusciante/C. Smith'
 }
 PLAYLIST_XML = """
 <container xmlns="urn:schemas-upnp-org:metadata-1-0/DIDL-Lite/"
  xmlns:dc="http://purl.org/dc/elements/1.1/"
@@ -170,15 +154,15 @@
 .m3u</res>
   <dc:title>-=Trentem&#248;ller - The Trentem&#248;ller Chronicles (CD 1).m3u
 </dc:title>
   <upnp:class>object.container.playlistContainer</upnp:class>
 </container>"""
 PLAYLIST_XML = PLAYLIST_XML.replace('\n', '')
 PLAYLIST_DICT = {
-    'item_class': 'object.container.playlistContainer',
+    'parent_id': 'A:PLAYLISTS',
     'uri': 'x-file-cifs://TLE-SERVER/share/mp3/Trentem%c3%b8ller%20-%20The%20'
            'Trentem%c3%b8ller%20Chronicles/-%3dTrentem%c3%b8ller%20-%20The%20'
            'Trentem%c3%b8ller%20Chronicles%20(CD%201).m3u',
     'title': '-=Trentem\xf8ller - The Trentem\xf8ller Chronicles (CD 1).m3u'}
 SONOS_PLAYLIST_XML = """
 <container xmlns="urn:schemas-upnp-org:metadata-1-0/DIDL-Lite/"
  xmlns:dc="http://purl.org/dc/elements/1.1/"
@@ -187,33 +171,50 @@
  restricted="true">
   <res protocolInfo="x-file-cifs:*:audio/mpegurl:*">file:///jffs/settings/savedqueues.rsq#13 title: Koop</res>
   <dc:title>Koop</dc:title>
   <upnp:class>object.container.playlistContainer</upnp:class>
 </container>"""
 SONOS_PLAYLIST_XML = SONOS_PLAYLIST_XML.replace('\n', '')
 SONOS_PLAYLIST_DICT = {
-    'item_class': 'object.container.playlistContainer',
+    'parent_id': 'SQ:',
     'uri': 'file:///jffs/settings/savedqueues.rsq#13 title: Koop',
     'title': 'Koop'}
 SHARE_XML = """
 <container xmlns="urn:schemas-upnp-org:metadata-1-0/DIDL-Lite/"
  xmlns:dc="http://purl.org/dc/elements/1.1/"
  xmlns:upnp="urn:schemas-upnp-org:metadata-1-0/upnp/" id="S://TLE-SERVER/share"
  parentID="S:" restricted="true">
   <dc:title>//TLE-SERVER/share</dc:title>
   <upnp:class>object.container</upnp:class>
   <res protocolInfo="x-rincon-playlist:*:*:*">x-rincon-playlist:RINCON_
 000E5884455C01400#S://TLE-SERVER/share</res>
 </container>"""
 SHARE_XML = SHARE_XML.replace('\n', '')
 SHARE_DICT = {
-    'item_class': 'object.container',
+    'parent_id': 'S:',
     'uri': 'x-rincon-playlist:RINCON_000E5884455C01400#S://TLE-SERVER/share',
     'title': '//TLE-SERVER/share'
 }
+ALBUMLIST_XML = """
+<container xmlns="urn:schemas-upnp-org:metadata-1-0/DIDL-Lite/"
+ xmlns:dc="http://purl.org/dc/elements/1.1/"
+ xmlns:upnp="urn:schemas-upnp-org:metadata-1-0/upnp/" id="A:ALBUM"
+ parentID="A:" restricted="true">
+  <dc:title>Albums</dc:title>
+  <upnp:class>object.container.albumlist</upnp:class>
+  <res protocolInfo="x-rincon-playlist:*:*:*">x-rincon-playlist:RINCON_
+000E5884455C01400#A:ALBUM</res>
+</container>
+"""
+ALBUMLIST_XML = ALBUMLIST_XML.replace('\n', '')
+ALBUMLIST_DICT = {
+    'parent_id': 'A:',
+    'uri': 'x-rincon-playlist:RINCON_000E5884455C01400#A:ALBUM',
+    'title': 'Albums'
+}
 QUEUE_XML1 = """
 <item xmlns="urn:schemas-upnp-org:metadata-1-0/DIDL-Lite/"
  xmlns:dc="http://purl.org/dc/elements/1.1/"
  xmlns:upnp="urn:schemas-upnp-org:metadata-1-0/upnp/" id="Q:0/1" parentID="Q:0"
  restricted="true">
   <res duration="0:04:43" protocolInfo="sonos.com-mms:*:audio/x-ms-wma:*">
 x-sonos-mms:AnyArtistTrack%3a126778459?sid=50&amp;flags=32</res>
@@ -227,15 +228,15 @@
 QUEUE_XML1 = QUEUE_XML1.replace('\n', '')
 QUEUE_DICT1 = {
     'album': 'Almost Gracefully',
     'creator': 'Randi Laubek',
     'title': 'Airworthy',
     'uri': 'x-sonos-mms:AnyArtistTrack%3a126778459?sid=50&flags=32',
     'album_art_uri': '/getaa?s=1&u=x-sonos-mms%3aAnyArtistTrack%253a126778459'
-    '%3fsid%3d50%26flags%3d32',
+                     '%3fsid%3d50%26flags%3d32',
     'item_class': 'object.item.audioItem.musicTrack',
     'original_track_number': None
 }
 
 QUEUE_XML2 = """
 <item xmlns="urn:schemas-upnp-org:metadata-1-0/DIDL-Lite/"
  xmlns:dc="http://purl.org/dc/elements/1.1/"
@@ -256,23 +257,24 @@
 """
 QUEUE_XML2 = QUEUE_XML2.replace('\n', '')
 QUEUE_DICT2 = {
     'album': 'Philharmonics',
     'creator': 'Agnes Obel',
     'title': 'Falling, Catching',
     'uri': 'x-file-cifs://TLE-SERVER/share/flac/Agnes%20Obel%20-%20'
-    'Philharmonics/1%20-%20Falling,%20Catching.flac',
+           'Philharmonics/1%20-%20Falling,%20Catching.flac',
     'album_art_uri': '/getaa?u=x-file-cifs%3a%2f%2fTLE-SERVER%2fshare%2fflac'
-    '%2fAgnes%2520Obel%2520-%2520Philharmonics%2f1%2520-%2520Falling,'
-    '%2520Catching.flac&v=2',
+                     '%2fAgnes%2520Obel%2520-%2520Philharmonics%2f1%2520-'
+                     '%2520Falling,%2520Catching.flac&v=2',
     'item_class': 'object.item.audioItem.musicTrack',
     'original_track_number': 1
 }
 
 
+
 # Helper test functions
 def set_and_get_test(instance, content, key):
     """Test get and set of a single unicode attribute
 
     :param instance: The object to be tested
     :param content: The content dict that contains the test values
     :param key: The name of the attribute and key in content to test
@@ -283,15 +285,15 @@
     # Test if the attribute value can be changed and return the new value
     setattr(instance, key, original + '!addition¡')
     assert getattr(instance, key) == original + '!addition¡'
     # Reset
     setattr(instance, key, original)
 
 
-def common_tests(parent_id, item_id, instance, content, item_xml, item_dict):
+def common_tests(item_class, item_id, instance, content, item_xml, item_dict):
     """Test all the common methods inherited from MusicLibraryItem
 
     :param parent_id: The parent ID of the class
     :param item_id: The expected item_id result for instance
     :param instance: The main object to be tested
     :param content: The content dict that corresponds to instance
     :param item_xml: A real XML example for from_xml
@@ -309,98 +311,56 @@
     # Test item_id
     assert instance.item_id == item_id
 
     # Test didl_metadata
     content1 = content.copy()
     content1.pop('title')
     title = 'Dummy title with non ascii chars &#230;&#248;&#229;'
-    xml = XML_TEMPLATE.format(parent_id=parent_id, item_id=item_id,
+    xml = XML_TEMPLATE.format(item_class=item_class, item_id=item_id,
                               title=title, **content1)
-    assert XML.tostring(instance.didl_metadata).decode() == xml
-
-    # Test common attributes
-    for key in ['uri', 'title', 'item_class']:
-        set_and_get_test(instance, content, key)
-
-    # Test equals (should fail if we change any attribute)
-    assert instance == instance3
-    for key in content.keys():
-        original = getattr(instance3, key)
-        if key == 'original_track_number':
-            setattr(instance3, key, original + 1)
-        else:
-            setattr(instance3, key, original + '!addition¡')
-        assert instance != instance3
-        setattr(instance3, key, original)
 
-    # Test default class and None for un-assigned attributes
-    instance4 = instance.__class__(content['uri'], content['title'])
-    assert instance4.item_class == item_dict['item_class']
-    for key in content.keys():
-        if key not in ['uri', 'title', 'item_class']:
-            assert getattr(instance4, key) is None
-
-
-def common_tests_queue(parent_id, instance, content, item_xml,
-                       item_dict):
-    """Test all the common methods inherited from MusicLibraryItem
-
-    :param parent_id: The parent ID of the class
-    :param item_id: The expected item_id result for instance
-    :param instance: The main object to be tested
-    :param content: The content dict that corresponds to instance
-    :param item_xml: A real XML example for from_xml
-    :param item_dict: The content dict result corresponding to item_xml
-    """
-    # from_xml, this test uses real data examples
-    instance2 = instance.__class__.from_xml(
-        XML.fromstring(item_xml.encode('utf8')))
-    assert instance2.to_dict == item_dict
-
-    # from_dict and to_dict
-    instance3 = instance.__class__.from_dict(content)
-    assert instance3.to_dict == content
+    assert XML.tostring(instance.didl_metadata).decode() == xml
 
     # Test common attributes
-    for key in ['uri', 'title', 'item_class']:
+    for key in ['uri', 'title', 'parent_id']:
         set_and_get_test(instance, content, key)
 
     # Test equals (should fail if we change any attribute)
     assert instance == instance3
     for key in content.keys():
         original = getattr(instance3, key)
         if key == 'original_track_number':
             setattr(instance3, key, original + 1)
         else:
             setattr(instance3, key, original + '!addition¡')
         assert instance != instance3
         setattr(instance3, key, original)
 
-    # Test default class and None for un-assigned attributes
-    instance4 = instance.__class__(content['uri'], content['title'])
-    assert instance4.item_class == item_dict['item_class']
+    # Test None for un-assigned attributes
+    instance4 = instance.__class__(content['uri'], content['title'],
+                                   content['parent_id'])
     for key in content.keys():
-        if key not in ['uri', 'title', 'item_class']:
+        if key not in ['uri', 'title', 'parent_id']:
             assert getattr(instance4, key) is None
 
 
 # The functions that test the different classes
 def test_mltrack():
     """Test the MLTrack class"""
     # Set the tests up
     uri = 'x-file-cifs://dummy_uri'
     kwargs = {'album': ALBUM, 'album_art_uri': ART_URI, 'creator': CREATOR,
               'original_track_number': 47}
-    content = {'uri': uri, 'title': TITLE, 'item_class': 'dummy.class'}
+    content = {'uri': uri, 'title': TITLE, 'parent_id': 'A:TRACKS'}
     content.update(kwargs)
-    track = data_structures.MLTrack(uri, TITLE, 'dummy.class', **kwargs)
+    track = data_structures.MLTrack(uri, TITLE, 'A:TRACKS', **kwargs)
 
     # Run tests on inherited methods and attributes
-    common_tests('A:TRACKS', 'S://dummy_uri', track, content, TRACK_XML,
-                 TRACK_DICT)
+    common_tests('object.item.audioItem.musicTrack', 'S://dummy_uri',
+                 track, content, TRACK_XML, TRACK_DICT)
 
     # Test class specific attributes
     for key in ['album', 'album_art_uri', 'creator']:
         set_and_get_test(track, content, key)
 
     assert track.original_track_number == 47
     track.original_track_number = 42
@@ -409,140 +369,146 @@
 
 
 def test_mlalbum():
     """Test the MLAlbum class"""
     # Set the tests up
     uri = 'x-rincon-playlist:RINCON_000E5884455C01400#A:ALBUM/dummy_album'
     kwargs = {'album_art_uri': ART_URI, 'creator': CREATOR}
-    album = data_structures.MLAlbum(uri, TITLE, 'dummy.class', **kwargs)
+    album = data_structures.MLAlbum(uri, TITLE, 'A:ALBUM', **kwargs)
 
     # Run tests on inherited methods and attributes
-    content = {'uri': uri, 'title': TITLE, 'item_class': 'dummy.class'}
+    content = {'uri': uri, 'title': TITLE, 'parent_id': 'A:ALBUM'}
     content.update(kwargs)
-    common_tests('A:ALBUM', 'A:ALBUM/dummy_album', album, content, ALBUM_XML,
-                 ALBUM_DICT)
+    common_tests('object.container.album.musicAlbum', 'A:ALBUM/dummy_album',
+                 album, content, ALBUM_XML, ALBUM_DICT)
 
     # Test class specific attributes
     for key in ['album_art_uri', 'creator']:
         set_and_get_test(album, content, key)
 
 
 def test_mlartist():
     """Test the MLArtist class"""
     # Set the tests up
     uri = 'x-rincon-playlist:RINCON_000E5884455C01400#A:ARTIST/10%20Years'
-    artist = data_structures.MLArtist(uri, TITLE, 'dummy.class')
+    artist = data_structures.MLArtist(uri, TITLE, 'A:ARTIST')
 
     # Run tests on inherited methods and attributes
-    content = {'uri': uri, 'title': TITLE, 'item_class': 'dummy.class'}
-    common_tests('A:ARTIST', 'A:ARTIST/10%20Years', artist, content,
-                 ARTIST_XML, ARTIST_DICT)
-
-
-def test_mlalbumartist():
-    """Test the MLAlbumArtist class"""
-    # Set the tests up
-    uri = 'x-rincon-playlist:RINCON_000E5884455C01400#A:ALBUMARTIST/'\
-          '3%20Doors%20Down'
-    albumartist = data_structures.MLAlbumArtist(uri, TITLE, 'dummy.class')
-
-    # Run tests on inherited methods and attributes
-    content = {'uri': uri, 'title': TITLE, 'item_class': 'dummy.class'}
-    common_tests('A:ALBUMARTIST', 'A:ALBUMARTIST/3%20Doors%20Down',
-                 albumartist, content, ALBUMARTIST_XML, ALBUMARTIST_DICT)
+    content = {'uri': uri, 'title': TITLE, 'parent_id': 'A:ARTIST'}
+    common_tests('object.container.person.musicArtist', 'A:ARTIST/10%20Years',
+                 artist, content, ARTIST_XML, ARTIST_DICT)
 
 
 def test_mlgenre():
     """Test the MLGenre class"""
     # Set the tests up
     uri = 'x-rincon-playlist:RINCON_000E5884455C01400#A:GENRE/Acid'
-    genre = data_structures.MLGenre(uri, TITLE, 'dummy.class')
+    genre = data_structures.MLGenre(uri, TITLE, 'A:GENRE')
 
     # Run tests on inherited methods and attributes
-    content = {'uri': uri, 'title': TITLE, 'item_class': 'dummy.class'}
-    common_tests('A:GENRE', 'A:GENRE/Acid', genre, content,
-                 GENRE_XML, GENRE_DICT)
+    content = {'uri': uri, 'title': TITLE, 'parent_id': 'A:GENRE'}
+    common_tests('object.container.genre.musicGenre', 'A:GENRE/Acid', genre,
+                 content, GENRE_XML, GENRE_DICT)
 
 
 def test_mlcomposer():
     """Test the MLComposer class"""
     # Set the tests up
     uri = 'x-rincon-playlist:RINCON_000E5884455C01400#A:COMPOSER/A.%20Kiedis'\
           '%2fFlea%2fJ.%20Frusciante%2fC.%20Smith'
-    composer = data_structures.MLComposer(uri, TITLE, 'dummy.class')
+    composer = data_structures.MLComposer(uri, TITLE, 'A:COMPOSER')
 
     # Run tests on inherited methods and attributes
-    content = {'uri': uri, 'title': TITLE, 'item_class': 'dummy.class'}
+    content = {'uri': uri, 'title': TITLE, 'parent_id': 'A:COMPOSER'}
     common_tests(
-        'A:COMPOSER',
+        'object.container.person.composer',
         'A:COMPOSER/A.%20Kiedis%2fFlea%2fJ.%20Frusciante%2fC.%20Smith',
         composer, content, COMPOSER_XML, COMPOSER_DICT
     )
 
 
 def test_mlplaylist():
     """Test the MLPlaylist class"""
     # Set the tests up
     uri = 'x-file-cifs://TLE-SERVER/share/mp3/Trentem%c3%b8ller%20-%20The%20'\
           'Trentem%c3%b8ller%20Chronicles/-%3dTrentem%c3%b8ller%20-%20The%20'\
           'Trentem%c3%b8ller%20Chronicles%20(CD%201).m3u'
-    playlist = data_structures.MLPlaylist(uri, TITLE, 'dummy.class')
+    playlist = data_structures.MLPlaylist(uri, TITLE, 'A:PLAYLISTS')
 
     # Run tests on inherited methods and attributes
-    content = {'uri': uri, 'title': TITLE, 'item_class': 'dummy.class'}
-    common_tests('A:PLAYLISTS', 'S://TLE-SERVER/share/mp3/Trentem%c3%b8ller'
+    content = {'uri': uri, 'title': TITLE, 'parent_id': 'A:PLAYLISTS'}
+    common_tests('object.container.playlistContainer',
+                 'S://TLE-SERVER/share/mp3/Trentem%c3%b8ller'
                  '%20-%20The%20Trentem%c3%b8ller%20Chronicles/-%3d'
                  'Trentem%c3%b8ller%20-%20The%20Trentem%c3%b8ller%20'
                  'Chronicles%20(CD%201).m3u', playlist, content,
                  PLAYLIST_XML, PLAYLIST_DICT)
 
 
 def test_mlsonosplaylist():
     """Test the MLSonosPlaylist class"""
     # Set the tests up
     uri = 'file:///jffs/settings/savedqueues.rsq#13 title: Koop'
-    playlist = data_structures.MLSonosPlaylist(uri, TITLE, 'dummy.class')
+    playlist = data_structures.MLSonosPlaylist(uri, TITLE, 'SQ:')
 
     # Run tests on inherited methods and attributes
-    content = {'uri': uri, 'title': TITLE, 'item_class': 'dummy.class'}
-    common_tests('SQ:', '13 title: Koop',
+    content = {'uri': uri, 'title': TITLE, 'parent_id': 'SQ:'}
+    common_tests('object.container.playlistContainer', 'SQ:13 title: Koop',
                  playlist, content, SONOS_PLAYLIST_XML, SONOS_PLAYLIST_DICT)
 
 
 def test_mlshare():
     """Test the MLShare class"""
     # Set the tests up
     uri = 'x-rincon-playlist:RINCON_000E5884455C01400#S://TLE-SERVER/share'
-    share = data_structures.MLShare(uri, TITLE, 'dummy.class')
+    share = data_structures.MLShare(uri, TITLE, 'S:')
 
     # Run tests on inherited methods and attributes
-    content = {'uri': uri, 'title': TITLE, 'item_class': 'dummy.class'}
-    common_tests('S:', 'S://TLE-SERVER/share', share, content,
+    content = {'uri': uri, 'title': TITLE, 'parent_id': 'S:'}
+    common_tests('object.container', 'S://TLE-SERVER/share', share, content,
                  SHARE_XML, SHARE_DICT)
 
 
+def test_mlalbumlist():
+    """Test the MLAlbumList class"""
+    # Sets the tests up
+    uri = 'x-rincon-playlist:RINCON_000E5884455C01400#A:ALBUM'
+    albumlist = data_structures.MLAlbumList(uri, TITLE, 'A:')
+
+    # Run tests on inherited methods and attributes
+    content = {'uri': uri, 'title': TITLE, 'parent_id': 'A:'}
+    common_tests('object.container.albumlist', 'A:ALBUM', albumlist, content,
+                 ALBUMLIST_XML, ALBUMLIST_DICT)
+
+
 def test_ns_tag():
     """Test the ns_tag module function"""
     namespaces = ['http://purl.org/dc/elements/1.1/',
                   'urn:schemas-upnp-org:metadata-1-0/upnp/',
                   'urn:schemas-upnp-org:metadata-1-0/DIDL-Lite/']
     for ns_in, namespace in zip(['dc', 'upnp', ''], namespaces):
         res = data_structures.ns_tag(ns_in, 'testtag')
         correct = '{{{0}}}{1}'.format(namespace, 'testtag')
         assert res == correct
 
 
 def test_get_ml_item():
     """Test the get_ml_item medule function"""
-    xmls = [TRACK_XML, ALBUM_XML, ARTIST_XML, ALBUMARTIST_XML, GENRE_XML,
-            COMPOSER_XML, PLAYLIST_XML, SHARE_XML]
-    classes = [data_structures.MLTrack, data_structures.MLAlbum,
-               data_structures.MLArtist, data_structures.MLAlbumArtist,
-               data_structures.MLGenre, data_structures.MLComposer,
-               data_structures.MLPlaylist, data_structures.MLShare]
+    xmls = [TRACK_XML,
+            ALBUM_XML,
+            ARTIST_XML,
+            GENRE_XML,
+            COMPOSER_XML,
+            PLAYLIST_XML]
+    classes = [data_structures.MLTrack,
+               data_structures.MLAlbum,
+               data_structures.MLArtist,
+               data_structures.MLGenre,
+               data_structures.MLComposer,
+               data_structures.MLPlaylist]
     for xml, class_ in zip(xmls, classes):
         etree = XML.fromstring(xml.encode('utf-8'))
         item = data_structures.get_ml_item(etree)
         assert item.__class__ == class_
 
 
 def test_queue_item():
@@ -551,16 +517,44 @@
     uri = 'x-file-cifs://dummy_uri'
     kwargs = {'album': ALBUM, 'album_art_uri': ART_URI, 'creator': CREATOR,
               'original_track_number': 47}
     content = {'uri': uri, 'title': TITLE, 'item_class': 'dummy.class'}
     content.update(kwargs)
     track = data_structures.QueueItem(uri, TITLE, 'dummy.class', **kwargs)
 
-    # Run tests on inherited methods and attributes
-    common_tests_queue('Q:0', track, content, QUEUE_XML1, QUEUE_DICT1)
+    # from_xml, this test uses real data examples
+    instance2 = track.__class__.from_xml(
+        XML.fromstring(QUEUE_XML1.encode('utf8')))
+    assert instance2.to_dict == QUEUE_DICT1
+
+    # from_dict and to_dict
+    instance3 = track.__class__.from_dict(content)
+    assert instance3.to_dict == content
+
+    # Test common attributes
+    for key in ['uri', 'title', 'item_class']:
+        set_and_get_test(track, content, key)
+
+    # Test equals (should fail if we change any attribute)
+    assert track == instance3
+    for key in content.keys():
+        original = getattr(instance3, key)
+        if key == 'original_track_number':
+            setattr(instance3, key, original + 1)
+        else:
+            setattr(instance3, key, original + '!addition¡')
+        assert track != instance3
+        setattr(instance3, key, original)
+
+    # Test default class and None for un-assigned attributes
+    instance4 = track.__class__(content['uri'], content['title'])
+    assert instance4.item_class == QUEUE_DICT1['item_class']
+    for key in content.keys():
+        if key not in ['uri', 'title', 'item_class']:
+            assert getattr(instance4, key) is None
 
     # Test class specific attributes
     for key in ['album', 'album_art_uri', 'creator']:
         set_and_get_test(track, content, key)
 
     assert track.original_track_number == 47
     track.original_track_number = 42
```

### Comparing `soco-0.8/unittest/test_services.py` & `soco-0.9/unittest/test_services.py`

 * *Files identical despite different names*

