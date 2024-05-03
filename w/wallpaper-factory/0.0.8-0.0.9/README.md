# Comparing `tmp/wallpaper_factory-0.0.8.tar.gz` & `tmp/wallpaper_factory-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wallpaper_factory-0.0.8.tar", last modified: Tue Apr 30 13:54:08 2024, max compression
+gzip compressed data, was "wallpaper_factory-0.0.9.tar", last modified: Tue Apr 30 19:43:59 2024, max compression
```

## Comparing `wallpaper_factory-0.0.8.tar` & `wallpaper_factory-0.0.9.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 marlonkunz   (501) staff       (20)        0 2024-04-30 13:54:08.180873 wallpaper_factory-0.0.8/
--rw-r--r--   0 marlonkunz   (501) staff       (20)    35149 2024-04-30 12:02:22.000000 wallpaper_factory-0.0.8/LICENSE
--rw-r--r--   0 marlonkunz   (501) staff       (20)     5924 2024-04-30 13:54:08.180669 wallpaper_factory-0.0.8/PKG-INFO
--rw-r--r--   0 marlonkunz   (501) staff       (20)     5749 2024-04-30 13:53:35.000000 wallpaper_factory-0.0.8/README.md
--rw-r--r--   0 marlonkunz   (501) staff       (20)       38 2024-04-30 13:54:08.180916 wallpaper_factory-0.0.8/setup.cfg
--rw-r--r--   0 marlonkunz   (501) staff       (20)      396 2024-04-30 13:53:58.000000 wallpaper_factory-0.0.8/setup.py
-drwxr-xr-x   0 marlonkunz   (501) staff       (20)        0 2024-04-30 13:54:08.177848 wallpaper_factory-0.0.8/src/
-drwxr-xr-x   0 marlonkunz   (501) staff       (20)        0 2024-04-30 13:54:08.179515 wallpaper_factory-0.0.8/src/wallpaper_factory/
--rw-r--r--   0 marlonkunz   (501) staff       (20)       61 2024-04-30 12:02:22.000000 wallpaper_factory-0.0.8/src/wallpaper_factory/__init__.py
--rw-r--r--   0 marlonkunz   (501) staff       (20)     2378 2024-04-30 13:33:15.000000 wallpaper_factory-0.0.8/src/wallpaper_factory/available_palletes.py
--rw-r--r--   0 marlonkunz   (501) staff       (20)     3719 2024-04-30 12:02:22.000000 wallpaper_factory-0.0.8/src/wallpaper_factory/main.py
-drwxr-xr-x   0 marlonkunz   (501) staff       (20)        0 2024-04-30 13:54:08.180443 wallpaper_factory-0.0.8/src/wallpaper_factory.egg-info/
--rw-r--r--   0 marlonkunz   (501) staff       (20)     5924 2024-04-30 13:54:08.000000 wallpaper_factory-0.0.8/src/wallpaper_factory.egg-info/PKG-INFO
--rw-r--r--   0 marlonkunz   (501) staff       (20)      406 2024-04-30 13:54:08.000000 wallpaper_factory-0.0.8/src/wallpaper_factory.egg-info/SOURCES.txt
--rw-r--r--   0 marlonkunz   (501) staff       (20)        1 2024-04-30 13:54:08.000000 wallpaper_factory-0.0.8/src/wallpaper_factory.egg-info/dependency_links.txt
--rw-r--r--   0 marlonkunz   (501) staff       (20)       74 2024-04-30 13:54:08.000000 wallpaper_factory-0.0.8/src/wallpaper_factory.egg-info/entry_points.txt
--rw-r--r--   0 marlonkunz   (501) staff       (20)       21 2024-04-30 13:54:08.000000 wallpaper_factory-0.0.8/src/wallpaper_factory.egg-info/requires.txt
--rw-r--r--   0 marlonkunz   (501) staff       (20)       18 2024-04-30 13:54:08.000000 wallpaper_factory-0.0.8/src/wallpaper_factory.egg-info/top_level.txt
+drwxr-xr-x   0 marlonkunz   (501) staff       (20)        0 2024-04-30 19:43:59.565056 wallpaper_factory-0.0.9/
+-rw-r--r--   0 marlonkunz   (501) staff       (20)    35149 2024-04-30 12:02:22.000000 wallpaper_factory-0.0.9/LICENSE
+-rw-r--r--   0 marlonkunz   (501) staff       (20)     5924 2024-04-30 19:43:59.564817 wallpaper_factory-0.0.9/PKG-INFO
+-rw-r--r--   0 marlonkunz   (501) staff       (20)     5749 2024-04-30 13:53:35.000000 wallpaper_factory-0.0.9/README.md
+-rw-r--r--   0 marlonkunz   (501) staff       (20)       38 2024-04-30 19:43:59.565100 wallpaper_factory-0.0.9/setup.cfg
+-rw-r--r--   0 marlonkunz   (501) staff       (20)      396 2024-04-30 19:43:32.000000 wallpaper_factory-0.0.9/setup.py
+drwxr-xr-x   0 marlonkunz   (501) staff       (20)        0 2024-04-30 19:43:59.561311 wallpaper_factory-0.0.9/src/
+drwxr-xr-x   0 marlonkunz   (501) staff       (20)        0 2024-04-30 19:43:59.563219 wallpaper_factory-0.0.9/src/wallpaper_factory/
+-rw-r--r--   0 marlonkunz   (501) staff       (20)       61 2024-04-30 12:02:22.000000 wallpaper_factory-0.0.9/src/wallpaper_factory/__init__.py
+-rw-r--r--   0 marlonkunz   (501) staff       (20)     2378 2024-04-30 13:33:15.000000 wallpaper_factory-0.0.9/src/wallpaper_factory/available_palletes.py
+-rw-r--r--   0 marlonkunz   (501) staff       (20)     4393 2024-04-30 19:43:15.000000 wallpaper_factory-0.0.9/src/wallpaper_factory/main.py
+drwxr-xr-x   0 marlonkunz   (501) staff       (20)        0 2024-04-30 19:43:59.564534 wallpaper_factory-0.0.9/src/wallpaper_factory.egg-info/
+-rw-r--r--   0 marlonkunz   (501) staff       (20)     5924 2024-04-30 19:43:59.000000 wallpaper_factory-0.0.9/src/wallpaper_factory.egg-info/PKG-INFO
+-rw-r--r--   0 marlonkunz   (501) staff       (20)      406 2024-04-30 19:43:59.000000 wallpaper_factory-0.0.9/src/wallpaper_factory.egg-info/SOURCES.txt
+-rw-r--r--   0 marlonkunz   (501) staff       (20)        1 2024-04-30 19:43:59.000000 wallpaper_factory-0.0.9/src/wallpaper_factory.egg-info/dependency_links.txt
+-rw-r--r--   0 marlonkunz   (501) staff       (20)       74 2024-04-30 19:43:59.000000 wallpaper_factory-0.0.9/src/wallpaper_factory.egg-info/entry_points.txt
+-rw-r--r--   0 marlonkunz   (501) staff       (20)       21 2024-04-30 19:43:59.000000 wallpaper_factory-0.0.9/src/wallpaper_factory.egg-info/requires.txt
+-rw-r--r--   0 marlonkunz   (501) staff       (20)       18 2024-04-30 19:43:59.000000 wallpaper_factory-0.0.9/src/wallpaper_factory.egg-info/top_level.txt
```

### Comparing `wallpaper_factory-0.0.8/LICENSE` & `wallpaper_factory-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `wallpaper_factory-0.0.8/PKG-INFO` & `wallpaper_factory-0.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wallpaper_factory
-Version: 0.0.8
+Version: 0.0.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: opencv-python
 Requires-Dist: pillow
 
 # Wallpaper Factory
```

### Comparing `wallpaper_factory-0.0.8/README.md` & `wallpaper_factory-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `wallpaper_factory-0.0.8/src/wallpaper_factory/available_palletes.py` & `wallpaper_factory-0.0.9/src/wallpaper_factory/available_palletes.py`

 * *Files identical despite different names*

### Comparing `wallpaper_factory-0.0.8/src/wallpaper_factory/main.py` & `wallpaper_factory-0.0.9/src/wallpaper_factory/main.py`

 * *Files 12% similar despite different names*

```diff
@@ -42,16 +42,31 @@
         image_name.pop()
         image_name.append("_denoised")
         image_name = "".join(image_name)
         image_name = image_name + ".png"
         new_path.append(image_name)
         new_path = "/".join(new_path)
         cv2.imwrite(new_path, new_image)
+        # remove black background that somehow happens while denoising
+        if not (0, 0, 0, 255) in available_colors:
+            remove_bg_after_denoise(new_path)
         print("saved denoised version at " + new_path)
 
+    # remove bg from image after bg is added in denoising
+    def remove_bg_after_denoise(image_path: str):
+        image = Image.open(image_path)
+        image = image.convert("RGBA")
+        pix = image.load()
+        for x in range(image.size[0]):
+            for y in range(image.size[1]):
+                if type(pix[x, y]) is tuple and not pix[x, y] == (0, 0, 0, 0):
+                    if pix[x, y] == (0, 0, 0, 255):
+                        pix[x, y] = (0, 0, 0, 0)
+        image.save(image_path)
+
     # get the image path to the image the user wants to convert
     # to the prefered color scheme
     image_path = os.path.abspath(input("Path of the image you want to recolor: "))
 
     # recolor the image and write it to the original directory
     # as <color-scheme>_<original-name>.png
     def recolor_image(path: str):
```

### Comparing `wallpaper_factory-0.0.8/src/wallpaper_factory.egg-info/PKG-INFO` & `wallpaper_factory-0.0.9/src/wallpaper_factory.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wallpaper_factory
-Version: 0.0.8
+Version: 0.0.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: opencv-python
 Requires-Dist: pillow
 
 # Wallpaper Factory
```

