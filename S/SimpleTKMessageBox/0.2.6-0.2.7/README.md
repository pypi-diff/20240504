# Comparing `tmp/SimpleTKMessageBox-0.2.6.tar.gz` & `tmp/SimpleTKMessageBox-0.2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "SimpleTKMessageBox-0.2.6.tar", last modified: Thu May  2 12:18:32 2024, max compression
+gzip compressed data, was "SimpleTKMessageBox-0.2.7.tar", last modified: Sat May  4 10:14:39 2024, max compression
```

## Comparing `SimpleTKMessageBox-0.2.6.tar` & `SimpleTKMessageBox-0.2.7.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxrwxrwx   0        0        0        0 2024-05-02 12:18:32.183501 SimpleTKMessageBox-0.2.6/
--rw-rw-rw-   0        0        0       25 2024-04-27 11:31:25.000000 SimpleTKMessageBox-0.2.6/MANIFEST.in
--rw-rw-rw-   0        0        0      423 2024-05-02 12:18:32.179503 SimpleTKMessageBox-0.2.6/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-05-02 12:18:32.176504 SimpleTKMessageBox-0.2.6/SimpleTKMessageBox.egg-info/
--rw-rw-rw-   0        0        0      423 2024-05-02 12:18:31.000000 SimpleTKMessageBox-0.2.6/SimpleTKMessageBox.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      862 2024-05-02 12:18:31.000000 SimpleTKMessageBox-0.2.6/SimpleTKMessageBox.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-02 12:18:31.000000 SimpleTKMessageBox-0.2.6/SimpleTKMessageBox.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2024-05-02 12:18:31.000000 SimpleTKMessageBox-0.2.6/SimpleTKMessageBox.egg-info/requires.txt
--rw-rw-rw-   0        0        0       19 2024-05-02 12:18:31.000000 SimpleTKMessageBox-0.2.6/SimpleTKMessageBox.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-05-02 12:18:31.946637 SimpleTKMessageBox-0.2.6/SimpleTkMessageBox/
--rw-rw-rw-   0        0        0     3427 2024-05-02 12:18:10.000000 SimpleTKMessageBox-0.2.6/SimpleTkMessageBox/SimpleTkMessageBox.py
--rw-rw-rw-   0        0        0       59 2024-04-27 10:36:23.000000 SimpleTKMessageBox-0.2.6/SimpleTkMessageBox/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-02 12:18:31.952633 SimpleTKMessageBox-0.2.6/SimpleTkMessageBox/icons/
-drwxrwxrwx   0        0        0        0 2024-05-02 12:18:32.015597 SimpleTKMessageBox-0.2.6/SimpleTkMessageBox/icons/W10/
--rw-rw-rw-   0        0        0     1051 2024-04-23 17:11:13.000000 SimpleTKMessageBox-0.2.6/SimpleTkMessageBox/icons/W10/1.png
--rw-rw-rw-   0        0        0     1395 2024-04-23 17:11:13.000000 SimpleTKMessageBox-0.2.6/SimpleTkMessageBox/icons/W10/2.png
--rw-rw-rw-   0        0        0      725 2024-04-23 17:11:13.000000 SimpleTKMessageBox-0.2.6/SimpleTkMessageBox/icons/W10/3.png
--rw-rw-rw-   0        0        0     1423 2024-04-23 17:11:13.000000 SimpleTKMessageBox-0.2.6/SimpleTkMessageBox/icons/W10/4.png
--rw-rw-rw-   0        0        0     1145 2024-04-23 17:11:13.000000 SimpleTKMessageBox-0.2.6/SimpleTkMessageBox/icons/W10/5.png
-drwxrwxrwx   0        0        0        0 2024-05-02 12:18:32.087555 SimpleTKMessageBox-0.2.6/SimpleTkMessageBox/icons/W11/
--rw-rw-rw-   0        0        0     3154 2024-04-23 17:12:10.000000 SimpleTKMessageBox-0.2.6/SimpleTkMessageBox/icons/W11/1.png
--rw-rw-rw-   0        0        0     1847 2024-04-23 17:12:10.000000 SimpleTKMessageBox-0.2.6/SimpleTkMessageBox/icons/W11/2.png
--rw-rw-rw-   0        0        0     3264 2024-04-23 17:12:10.000000 SimpleTKMessageBox-0.2.6/SimpleTkMessageBox/icons/W11/3.png
--rw-rw-rw-   0        0        0     4962 2024-04-23 17:12:10.000000 SimpleTKMessageBox-0.2.6/SimpleTkMessageBox/icons/W11/4.png
--rw-rw-rw-   0        0        0     4565 2024-04-23 17:12:10.000000 SimpleTKMessageBox-0.2.6/SimpleTkMessageBox/icons/W11/5.png
-drwxrwxrwx   0        0        0        0 2024-05-02 12:18:32.172506 SimpleTKMessageBox-0.2.6/SimpleTkMessageBox/icons/W7/
--rw-rw-rw-   0        0        0     6639 2024-04-23 17:03:58.000000 SimpleTKMessageBox-0.2.6/SimpleTkMessageBox/icons/W7/1.png
--rw-rw-rw-   0        0        0     2797 2024-04-23 17:01:54.000000 SimpleTKMessageBox-0.2.6/SimpleTkMessageBox/icons/W7/2.png
--rw-rw-rw-   0        0        0     5154 2024-04-23 17:01:56.000000 SimpleTKMessageBox-0.2.6/SimpleTkMessageBox/icons/W7/3.png
--rw-rw-rw-   0        0        0     6070 2024-04-23 17:01:59.000000 SimpleTKMessageBox-0.2.6/SimpleTkMessageBox/icons/W7/4.png
--rw-rw-rw-   0        0        0     5708 2024-04-23 17:02:02.000000 SimpleTKMessageBox-0.2.6/SimpleTkMessageBox/icons/W7/5.png
--rw-rw-rw-   0        0        0     1406 2024-04-24 08:46:15.000000 SimpleTKMessageBox-0.2.6/SimpleTkMessageBox/icons/transparent.ico
--rw-rw-rw-   0        0        0       42 2024-05-02 12:18:32.184500 SimpleTKMessageBox-0.2.6/setup.cfg
--rw-rw-rw-   0        0        0     1334 2024-05-02 12:18:18.000000 SimpleTKMessageBox-0.2.6/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-04 10:14:39.417086 SimpleTKMessageBox-0.2.7/
+-rw-rw-rw-   0        0        0       25 2024-04-27 11:31:25.000000 SimpleTKMessageBox-0.2.7/MANIFEST.in
+-rw-rw-rw-   0        0        0      423 2024-05-04 10:14:39.405096 SimpleTKMessageBox-0.2.7/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-05-04 10:14:39.402097 SimpleTKMessageBox-0.2.7/SimpleTKMessageBox.egg-info/
+-rw-rw-rw-   0        0        0      423 2024-05-04 10:14:38.000000 SimpleTKMessageBox-0.2.7/SimpleTKMessageBox.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      862 2024-05-04 10:14:38.000000 SimpleTKMessageBox-0.2.7/SimpleTKMessageBox.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-04 10:14:38.000000 SimpleTKMessageBox-0.2.7/SimpleTKMessageBox.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        7 2024-05-04 10:14:38.000000 SimpleTKMessageBox-0.2.7/SimpleTKMessageBox.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       19 2024-05-04 10:14:38.000000 SimpleTKMessageBox-0.2.7/SimpleTKMessageBox.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-04 10:14:38.936361 SimpleTKMessageBox-0.2.7/SimpleTkMessageBox/
+-rw-rw-rw-   0        0        0     3646 2024-05-04 10:13:55.000000 SimpleTKMessageBox-0.2.7/SimpleTkMessageBox/SimpleTkMessageBox.py
+-rw-rw-rw-   0        0        0       59 2024-04-27 10:36:23.000000 SimpleTKMessageBox-0.2.7/SimpleTkMessageBox/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-04 10:14:38.998327 SimpleTKMessageBox-0.2.7/SimpleTkMessageBox/icons/
+drwxrwxrwx   0        0        0        0 2024-05-04 10:14:39.107263 SimpleTKMessageBox-0.2.7/SimpleTkMessageBox/icons/W10/
+-rw-rw-rw-   0        0        0     1051 2024-04-23 17:11:13.000000 SimpleTKMessageBox-0.2.7/SimpleTkMessageBox/icons/W10/1.png
+-rw-rw-rw-   0        0        0     1395 2024-04-23 17:11:13.000000 SimpleTKMessageBox-0.2.7/SimpleTkMessageBox/icons/W10/2.png
+-rw-rw-rw-   0        0        0      725 2024-04-23 17:11:13.000000 SimpleTKMessageBox-0.2.7/SimpleTkMessageBox/icons/W10/3.png
+-rw-rw-rw-   0        0        0     1423 2024-04-23 17:11:13.000000 SimpleTKMessageBox-0.2.7/SimpleTkMessageBox/icons/W10/4.png
+-rw-rw-rw-   0        0        0     1145 2024-04-23 17:11:13.000000 SimpleTKMessageBox-0.2.7/SimpleTkMessageBox/icons/W10/5.png
+drwxrwxrwx   0        0        0        0 2024-05-04 10:14:39.159234 SimpleTKMessageBox-0.2.7/SimpleTkMessageBox/icons/W11/
+-rw-rw-rw-   0        0        0     3154 2024-04-23 17:12:10.000000 SimpleTKMessageBox-0.2.7/SimpleTkMessageBox/icons/W11/1.png
+-rw-rw-rw-   0        0        0     1847 2024-04-23 17:12:10.000000 SimpleTKMessageBox-0.2.7/SimpleTkMessageBox/icons/W11/2.png
+-rw-rw-rw-   0        0        0     3264 2024-04-23 17:12:10.000000 SimpleTKMessageBox-0.2.7/SimpleTkMessageBox/icons/W11/3.png
+-rw-rw-rw-   0        0        0     4962 2024-04-23 17:12:10.000000 SimpleTKMessageBox-0.2.7/SimpleTkMessageBox/icons/W11/4.png
+-rw-rw-rw-   0        0        0     4565 2024-04-23 17:12:10.000000 SimpleTKMessageBox-0.2.7/SimpleTkMessageBox/icons/W11/5.png
+drwxrwxrwx   0        0        0        0 2024-05-04 10:14:39.381107 SimpleTKMessageBox-0.2.7/SimpleTkMessageBox/icons/W7/
+-rw-rw-rw-   0        0        0     6639 2024-04-23 17:03:58.000000 SimpleTKMessageBox-0.2.7/SimpleTkMessageBox/icons/W7/1.png
+-rw-rw-rw-   0        0        0     2797 2024-04-23 17:01:54.000000 SimpleTKMessageBox-0.2.7/SimpleTkMessageBox/icons/W7/2.png
+-rw-rw-rw-   0        0        0     5154 2024-04-23 17:01:56.000000 SimpleTKMessageBox-0.2.7/SimpleTkMessageBox/icons/W7/3.png
+-rw-rw-rw-   0        0        0     6070 2024-04-23 17:01:59.000000 SimpleTKMessageBox-0.2.7/SimpleTkMessageBox/icons/W7/4.png
+-rw-rw-rw-   0        0        0     5708 2024-04-23 17:02:02.000000 SimpleTKMessageBox-0.2.7/SimpleTkMessageBox/icons/W7/5.png
+-rw-rw-rw-   0        0        0     1406 2024-04-24 08:46:15.000000 SimpleTKMessageBox-0.2.7/SimpleTkMessageBox/icons/transparent.ico
+-rw-rw-rw-   0        0        0       42 2024-05-04 10:14:39.418087 SimpleTKMessageBox-0.2.7/setup.cfg
+-rw-rw-rw-   0        0        0     1334 2024-05-04 10:14:33.000000 SimpleTKMessageBox-0.2.7/setup.py
```

### Comparing `SimpleTKMessageBox-0.2.6/SimpleTKMessageBox.egg-info/SOURCES.txt` & `SimpleTKMessageBox-0.2.7/SimpleTKMessageBox.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `SimpleTKMessageBox-0.2.6/SimpleTkMessageBox/SimpleTkMessageBox.py` & `SimpleTKMessageBox-0.2.7/SimpleTkMessageBox/SimpleTkMessageBox.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from tkinter import ttk
 import tkinter
 import os
 import sys
 from PIL import Image, ImageTk 
+import platform
 
 def ShowMSBox(master, Icon="Information", Title="Message Box", IconStyle="Windows 10", button1="", button2="", button3="", text="This is an info"):
     MsB = tkinter.Toplevel(master)
     StyleList = ["Windows 11","Windows 10", "Windows 7", "Personalized"]
     if not IconStyle in StyleList:
         raise ValueError("Invalid Style : " + IconStyle + ". It should be one of 'Windows 11', 'Windows 10', 'Windows 7' or 'Personalized'.")
 
@@ -33,14 +34,18 @@
         else:
             raise ValueError("Invalid Icon : " + Icon + ". It should be one of 'Warning', 'Check', 'Error', 'Question', or 'Information'.")
     
     if IconStyle == "Personalized":
         Path = Icon
     else:
         Path = os.path.join(os.path.dirname(os.path.realpath(__file__)), 'icons', Style, IconPath)
+
+    whiteWall = ttk.Frame(master=MsB, width=1000, height=1000, borderwidth=0)
+    whiteWall.place(x=0, y=0)
+
     photo = Image.open(os.path.realpath(Path))
     photo = photo.resize((64, 64))
     photo = ImageTk.PhotoImage(photo)
     image = ttk.Label(master=MsB, text="", image=photo)
     image.place(x=20, y=35)
 
     colorFrame = tkinter.Frame(master=MsB, bg="#e2e2e2", width=400, height=100)
@@ -82,14 +87,17 @@
         style.configure("BW.TButton", background=colorFrame.cget("bg"))
         MsBbtn3.config(style="BW.TButton")
 
     MsBtext = ttk.Label(MsB, text=text)
     MsBtext.place(x=100, y=60)
     WindowIcon = os.path.join(os.path.dirname(os.path.realpath(__file__)), 'icons', 'transparent.ico')
     MsB.title(Title)
-    MsB.geometry("400x200")
+    if platform.system() == "Windows":
+        MsB.geometry("400x200")
+    else:
+        MsB.geometry("410x200")
     MsB.resizable(False, False)
     MsB.iconbitmap(WindowIcon)
     MsB.transient(master)
     MsB.grab_set()
     MsB.wait_window(MsB)
     return button_pressed
```

### Comparing `SimpleTKMessageBox-0.2.6/SimpleTkMessageBox/icons/W10/1.png` & `SimpleTKMessageBox-0.2.7/SimpleTkMessageBox/icons/W10/1.png`

 * *Files identical despite different names*

### Comparing `SimpleTKMessageBox-0.2.6/SimpleTkMessageBox/icons/W10/2.png` & `SimpleTKMessageBox-0.2.7/SimpleTkMessageBox/icons/W10/2.png`

 * *Files identical despite different names*

### Comparing `SimpleTKMessageBox-0.2.6/SimpleTkMessageBox/icons/W10/3.png` & `SimpleTKMessageBox-0.2.7/SimpleTkMessageBox/icons/W10/3.png`

 * *Files identical despite different names*

### Comparing `SimpleTKMessageBox-0.2.6/SimpleTkMessageBox/icons/W10/4.png` & `SimpleTKMessageBox-0.2.7/SimpleTkMessageBox/icons/W10/4.png`

 * *Files identical despite different names*

### Comparing `SimpleTKMessageBox-0.2.6/SimpleTkMessageBox/icons/W10/5.png` & `SimpleTKMessageBox-0.2.7/SimpleTkMessageBox/icons/W10/5.png`

 * *Files identical despite different names*

### Comparing `SimpleTKMessageBox-0.2.6/SimpleTkMessageBox/icons/W11/1.png` & `SimpleTKMessageBox-0.2.7/SimpleTkMessageBox/icons/W11/1.png`

 * *Files identical despite different names*

### Comparing `SimpleTKMessageBox-0.2.6/SimpleTkMessageBox/icons/W11/2.png` & `SimpleTKMessageBox-0.2.7/SimpleTkMessageBox/icons/W11/2.png`

 * *Files identical despite different names*

### Comparing `SimpleTKMessageBox-0.2.6/SimpleTkMessageBox/icons/W11/3.png` & `SimpleTKMessageBox-0.2.7/SimpleTkMessageBox/icons/W11/3.png`

 * *Files identical despite different names*

### Comparing `SimpleTKMessageBox-0.2.6/SimpleTkMessageBox/icons/W11/4.png` & `SimpleTKMessageBox-0.2.7/SimpleTkMessageBox/icons/W11/4.png`

 * *Files identical despite different names*

### Comparing `SimpleTKMessageBox-0.2.6/SimpleTkMessageBox/icons/W11/5.png` & `SimpleTKMessageBox-0.2.7/SimpleTkMessageBox/icons/W11/5.png`

 * *Files identical despite different names*

### Comparing `SimpleTKMessageBox-0.2.6/SimpleTkMessageBox/icons/W7/1.png` & `SimpleTKMessageBox-0.2.7/SimpleTkMessageBox/icons/W7/1.png`

 * *Files identical despite different names*

### Comparing `SimpleTKMessageBox-0.2.6/SimpleTkMessageBox/icons/W7/2.png` & `SimpleTKMessageBox-0.2.7/SimpleTkMessageBox/icons/W7/2.png`

 * *Files identical despite different names*

### Comparing `SimpleTKMessageBox-0.2.6/SimpleTkMessageBox/icons/W7/3.png` & `SimpleTKMessageBox-0.2.7/SimpleTkMessageBox/icons/W7/3.png`

 * *Files identical despite different names*

### Comparing `SimpleTKMessageBox-0.2.6/SimpleTkMessageBox/icons/W7/4.png` & `SimpleTKMessageBox-0.2.7/SimpleTkMessageBox/icons/W7/4.png`

 * *Files identical despite different names*

### Comparing `SimpleTKMessageBox-0.2.6/SimpleTkMessageBox/icons/W7/5.png` & `SimpleTKMessageBox-0.2.7/SimpleTkMessageBox/icons/W7/5.png`

 * *Files identical despite different names*

### Comparing `SimpleTKMessageBox-0.2.6/SimpleTkMessageBox/icons/transparent.ico` & `SimpleTKMessageBox-0.2.7/SimpleTkMessageBox/icons/transparent.ico`

 * *Files identical despite different names*

### Comparing `SimpleTKMessageBox-0.2.6/setup.py` & `SimpleTKMessageBox-0.2.7/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from setuptools import setup, find_packages
 setup(
 name='SimpleTKMessageBox',
-version='0.2.6',
+version='0.2.7',
 author='Gustoon',
 author_email='no.email@gmail.com',
 description='A simple tkinter message box',
 long_description="""
 See documentation at https://github.com/Gustoon/SimpleTkMessageBox
 """,
 packages=find_packages(),
```

