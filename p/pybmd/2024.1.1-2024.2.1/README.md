# Comparing `tmp/pybmd-2024.1.1.tar.gz` & `tmp/pybmd-2024.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pybmd-2024.1.1.tar", last modified: Sun Feb  4 10:22:30 2024, max compression
+gzip compressed data, was "pybmd-2024.2.1.tar", last modified: Sat May  4 16:43:29 2024, max compression
```

## Comparing `pybmd-2024.1.1.tar` & `pybmd-2024.2.1.tar`

### file list

```diff
@@ -1,30 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-04 10:22:30.120607 pybmd-2024.1.1/
--rw-r--r--   0 runner    (1001) docker     (127)     7651 2024-02-04 10:22:00.000000 pybmd-2024.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1812 2024-02-04 10:22:30.120607 pybmd-2024.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1301 2024-02-04 10:22:00.000000 pybmd-2024.1.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-04 10:22:30.116607 pybmd-2024.1.1/pybmd/
--rw-r--r--   0 runner    (1001) docker     (127)      207 2024-02-04 10:22:00.000000 pybmd-2024.1.1/pybmd/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    14529 2024-02-04 10:22:00.000000 pybmd-2024.1.1/pybmd/bmd.py
--rw-r--r--   0 runner    (1001) docker     (127)      465 2024-02-04 10:22:00.000000 pybmd-2024.1.1/pybmd/error.py
--rw-r--r--   0 runner    (1001) docker     (127)     2559 2024-02-04 10:22:00.000000 pybmd-2024.1.1/pybmd/folder.py
--rw-r--r--   0 runner    (1001) docker     (127)      149 2024-02-04 10:22:00.000000 pybmd-2024.1.1/pybmd/fusion_comp.py
--rw-r--r--   0 runner    (1001) docker     (127)     1845 2024-02-04 10:22:00.000000 pybmd-2024.1.1/pybmd/gallery.py
--rw-r--r--   0 runner    (1001) docker     (127)      139 2024-02-04 10:22:00.000000 pybmd-2024.1.1/pybmd/gallery_still.py
--rw-r--r--   0 runner    (1001) docker     (127)     2585 2024-02-04 10:22:00.000000 pybmd-2024.1.1/pybmd/gallery_still_album.py
--rw-r--r--   0 runner    (1001) docker     (127)    12138 2024-02-04 10:22:00.000000 pybmd-2024.1.1/pybmd/media_pool.py
--rw-r--r--   0 runner    (1001) docker     (127)     8322 2024-02-04 10:22:00.000000 pybmd-2024.1.1/pybmd/media_pool_item.py
--rw-r--r--   0 runner    (1001) docker     (127)     4063 2024-02-04 10:22:00.000000 pybmd-2024.1.1/pybmd/media_storage.py
--rw-r--r--   0 runner    (1001) docker     (127)     9941 2024-02-04 10:22:00.000000 pybmd-2024.1.1/pybmd/project.py
--rw-r--r--   0 runner    (1001) docker     (127)     8466 2024-02-04 10:22:00.000000 pybmd-2024.1.1/pybmd/project_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)    10178 2024-02-04 10:22:00.000000 pybmd-2024.1.1/pybmd/settings.py
--rw-r--r--   0 runner    (1001) docker     (127)    20608 2024-02-04 10:22:00.000000 pybmd-2024.1.1/pybmd/timeline.py
--rw-r--r--   0 runner    (1001) docker     (127)    17872 2024-02-04 10:22:00.000000 pybmd-2024.1.1/pybmd/timeline_item.py
--rw-r--r--   0 runner    (1001) docker     (127)     3040 2024-02-04 10:22:00.000000 pybmd-2024.1.1/pybmd/toolkits.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-04 10:22:30.120607 pybmd-2024.1.1/pybmd.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1812 2024-02-04 10:22:30.000000 pybmd-2024.1.1/pybmd.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      509 2024-02-04 10:22:30.000000 pybmd-2024.1.1/pybmd.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-04 10:22:30.000000 pybmd-2024.1.1/pybmd.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-02-04 10:22:30.000000 pybmd-2024.1.1/pybmd.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-02-04 10:22:30.000000 pybmd-2024.1.1/pybmd.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-04 10:22:30.120607 pybmd-2024.1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      812 2024-02-04 10:22:00.000000 pybmd-2024.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 16:43:29.982374 pybmd-2024.2.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     7651 2024-05-04 16:43:02.000000 pybmd-2024.2.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1812 2024-05-04 16:43:29.982374 pybmd-2024.2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1301 2024-05-04 16:43:02.000000 pybmd-2024.2.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 16:43:29.982374 pybmd-2024.2.1/pybmd/
+-rw-r--r--   0 runner    (1001) docker     (127)      207 2024-05-04 16:43:02.000000 pybmd-2024.2.1/pybmd/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14598 2024-05-04 16:43:02.000000 pybmd-2024.2.1/pybmd/bmd.py
+-rw-r--r--   0 runner    (1001) docker     (127)      465 2024-05-04 16:43:02.000000 pybmd-2024.2.1/pybmd/error.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2559 2024-05-04 16:43:02.000000 pybmd-2024.2.1/pybmd/folder.py
+-rw-r--r--   0 runner    (1001) docker     (127)      149 2024-05-04 16:43:02.000000 pybmd-2024.2.1/pybmd/fusion_comp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1845 2024-05-04 16:43:02.000000 pybmd-2024.2.1/pybmd/gallery.py
+-rw-r--r--   0 runner    (1001) docker     (127)      139 2024-05-04 16:43:02.000000 pybmd-2024.2.1/pybmd/gallery_still.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2583 2024-05-04 16:43:02.000000 pybmd-2024.2.1/pybmd/gallery_still_album.py
+-rw-r--r--   0 runner    (1001) docker     (127)      499 2024-05-04 16:43:02.000000 pybmd-2024.2.1/pybmd/logging_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12138 2024-05-04 16:43:02.000000 pybmd-2024.2.1/pybmd/media_pool.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8322 2024-05-04 16:43:02.000000 pybmd-2024.2.1/pybmd/media_pool_item.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4063 2024-05-04 16:43:02.000000 pybmd-2024.2.1/pybmd/media_storage.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10133 2024-05-04 16:43:02.000000 pybmd-2024.2.1/pybmd/project.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8466 2024-05-04 16:43:02.000000 pybmd-2024.2.1/pybmd/project_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10178 2024-05-04 16:43:02.000000 pybmd-2024.2.1/pybmd/settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20608 2024-05-04 16:43:02.000000 pybmd-2024.2.1/pybmd/timeline.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17872 2024-05-04 16:43:02.000000 pybmd-2024.2.1/pybmd/timeline_item.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9861 2024-05-04 16:43:02.000000 pybmd-2024.2.1/pybmd/toolkits.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 16:43:29.982374 pybmd-2024.2.1/pybmd.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1812 2024-05-04 16:43:29.000000 pybmd-2024.2.1/pybmd.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      533 2024-05-04 16:43:29.000000 pybmd-2024.2.1/pybmd.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-04 16:43:29.000000 pybmd-2024.2.1/pybmd.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-04 16:43:29.000000 pybmd-2024.2.1/pybmd.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-04 16:43:29.000000 pybmd-2024.2.1/pybmd.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-04 16:43:29.982374 pybmd-2024.2.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      838 2024-05-04 16:43:02.000000 pybmd-2024.2.1/setup.py
```

### Comparing `pybmd-2024.1.1/LICENSE` & `pybmd-2024.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pybmd-2024.1.1/PKG-INFO` & `pybmd-2024.2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pybmd
-Version: 2024.1.1
+Version: 2024.2.1
 Summary: python library for Davinci Resolve(Repack)
 Home-page: https://github.com/WheheoHu/pybmd
 Author: wheheo
 Author-email: wheheohu@outlook.com
 Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 or later (LGPLv3+)
 Classifier: Operating System :: MacOS :: MacOS X
```

### Comparing `pybmd-2024.1.1/README.md` & `pybmd-2024.2.1/README.md`

 * *Files identical despite different names*

### Comparing `pybmd-2024.1.1/pybmd/bmd.py` & `pybmd-2024.2.1/pybmd/bmd.py`

 * *Files 0% similar despite different names*

```diff
@@ -164,16 +164,16 @@
         self.AUTO_CAPTION_TELETEXT=self.local_davinci.AUTO_CAPTION_TELETEXT
         self.AUTO_CAPTION_NETFLIX=self.local_davinci.AUTO_CAPTION_NETFLIX
         
        
         self.AUTO_CAPTION_LINE_SINGLE=self.local_davinci.AUTO_CAPTION_LINE_SINGLE
         self.AUTO_CAPTION_LINE_DOUBLE=self.local_davinci.AUTO_CAPTION_LINE_DOUBLE
         
-        
-        
+        global RESOLVE_VERSION
+        RESOLVE_VERSION=self.local_davinci.GetVersion()
         
     def init_davinci(self, davinci_ip,auto_start):
         """init and return Davinci Resolve object
 
         Args:
             davinci_ip (str, optional): Default value is local (127.0.0.1).
```

### Comparing `pybmd-2024.1.1/pybmd/folder.py` & `pybmd-2024.2.1/pybmd/folder.py`

 * *Files identical despite different names*

### Comparing `pybmd-2024.1.1/pybmd/gallery.py` & `pybmd-2024.2.1/pybmd/gallery.py`

 * *Files identical despite different names*

### Comparing `pybmd-2024.1.1/pybmd/gallery_still_album.py` & `pybmd-2024.2.1/pybmd/gallery_still_album.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from os import path
 from typing import List
 from pybmd.gallery_still import GalleryStill
 
 from enum import Enum
 
 
-class StillFormats(Enum):
+class StillFormat(Enum):
     """StillFormats"""
     DPX = "dpx"
     CIN = "cin"
     TIF = "tif"
     JPG = "jpg"
     PNG = "png"
     PPM = "ppm"
@@ -24,15 +24,15 @@
         self.gallery_still_album = gallery_still_album
 
     def delete_stills(self, gallery_stills: List[GalleryStill]) -> bool:
         """Delete the given gallery stills from the album."""
         gallery_still_list = [still.gallery_still for still in gallery_stills]
         return self.gallery_still_album.DeleteStills(gallery_still_list)
 
-    def export_stills(self, gallery_stills: List[GalleryStill], folder_path: str, file_prefix: str, format: StillFormats) -> bool:
+    def export_stills(self, gallery_stills: List[GalleryStill], folder_path: str, file_prefix: str, format: StillFormat) -> bool:
         """Exports list of GalleryStill objects 'galleryStill' to directory 'folderPath', with filename prefix 'filePrefix', using file format 'format' 
 
         Args:
             gallery_stills (List[GalleryStill]): a list of GalleryStill objects to export
             folder_path (str): folder path to export to
             file_prefix (str): filename prefix for exported files
             format (StillFormats): StillFormat Object to use for export format
```

### Comparing `pybmd-2024.1.1/pybmd/media_pool.py` & `pybmd-2024.2.1/pybmd/media_pool.py`

 * *Files identical despite different names*

### Comparing `pybmd-2024.1.1/pybmd/media_pool_item.py` & `pybmd-2024.2.1/pybmd/media_pool_item.py`

 * *Files identical despite different names*

### Comparing `pybmd-2024.1.1/pybmd/media_storage.py` & `pybmd-2024.2.1/pybmd/media_storage.py`

 * *Files identical despite different names*

### Comparing `pybmd-2024.1.1/pybmd/project.py` & `pybmd-2024.2.1/pybmd/project.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-
-
 from dataclasses import asdict
 from typing import Any, Dict, List
 from pybmd.gallery import Gallery
 from pybmd.media_pool import MediaPool
 
 from pybmd.timeline import Timeline
 from pybmd.settings import RenderSetting
@@ -51,15 +49,20 @@
 
     def get_current_render_mode(self) -> int:
         """Returns the render mode: 0 - Individual clips, 1 - Single clip."""
         return self.project.GetCurrentRenderMode()
 
     def get_current_timeline(self) -> Timeline:
         """Returns the currently loaded Timeline."""
-        return Timeline(timeline=self.project.GetCurrentTimeline())
+        current_timeline = self.project.GetCurrentTimeline()
+        if current_timeline is not None:
+            return Timeline(self.project.GetCurrentTimeline())
+        else:
+            raise TypeError("No current timeline,Please open a timeline")
+        
 
     def get_gallery(self) -> Gallery:
         """Returns the Gallery object."""
         return Gallery(self.project.GetGallery())
 
     def get_media_pool(self) -> MediaPool:
         """Returns the MediaPool object."""
```

### Comparing `pybmd-2024.1.1/pybmd/project_manager.py` & `pybmd-2024.2.1/pybmd/project_manager.py`

 * *Files identical despite different names*

### Comparing `pybmd-2024.1.1/pybmd/settings.py` & `pybmd-2024.2.1/pybmd/settings.py`

 * *Files identical despite different names*

### Comparing `pybmd-2024.1.1/pybmd/timeline.py` & `pybmd-2024.2.1/pybmd/timeline.py`

 * *Files 0% similar despite different names*

```diff
@@ -84,15 +84,15 @@
 class Timeline():
     """Timeline Object"""
 
     def __init__(self, timeline):
         self.timeline = timeline
 
     def __repr__(self) -> str:
-        return f'Timeline:f{self.get_name()}'
+        return f'Timeline: {self.get_name()}'
 
     def add_marker(self, frame_id: str, color: str, name: str, note: str, duration: str, custom_data: str) -> bool:
         """Creates a new marker at given frameId position and with given marker information. 
 
         Args:
             frame_id (str): frame position of the marker.
             color (str): color of the marker.
```

### Comparing `pybmd-2024.1.1/pybmd/timeline_item.py` & `pybmd-2024.2.1/pybmd/timeline_item.py`

 * *Files identical despite different names*

### Comparing `pybmd-2024.1.1/pybmd.egg-info/PKG-INFO` & `pybmd-2024.2.1/pybmd.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pybmd
-Version: 2024.1.1
+Version: 2024.2.1
 Summary: python library for Davinci Resolve(Repack)
 Home-page: https://github.com/WheheoHu/pybmd
 Author: wheheo
 Author-email: wheheohu@outlook.com
 Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 or later (LGPLv3+)
 Classifier: Operating System :: MacOS :: MacOS X
```

### Comparing `pybmd-2024.1.1/setup.py` & `pybmd-2024.2.1/setup.py`

 * *Files 17% similar despite different names*

```diff
@@ -11,14 +11,15 @@
     description="python library for Davinci Resolve(Repack)",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/WheheoHu/pybmd",
     packages=setuptools.find_packages(),
     install_requires=[
           'psutil',
+          'dftt-timecode'
       ],
     classifiers=[
         "Programming Language :: Python :: 3.10",
         "License :: OSI Approved :: GNU Lesser General Public License v3 or later (LGPLv3+)",
         "Operating System :: MacOS :: MacOS X",
         "Operating System :: Microsoft :: Windows"
     ],
```

