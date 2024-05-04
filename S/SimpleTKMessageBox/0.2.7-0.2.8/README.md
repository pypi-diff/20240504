# Comparing `tmp/SimpleTKMessageBox-0.2.7.tar.gz` & `tmp/SimpleTKMessageBox-0.2.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "SimpleTKMessageBox-0.2.7.tar", last modified: Sat May  4 10:14:39 2024, max compression
+gzip compressed data, was "SimpleTKMessageBox-0.2.8.tar", last modified: Sat May  4 12:14:04 2024, max compression
```

## Comparing `SimpleTKMessageBox-0.2.7.tar` & `SimpleTKMessageBox-0.2.8.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxrwxrwx   0        0        0        0 2024-05-04 10:14:39.417086 SimpleTKMessageBox-0.2.7/
--rw-rw-rw-   0        0        0       25 2024-04-27 11:31:25.000000 SimpleTKMessageBox-0.2.7/MANIFEST.in
--rw-rw-rw-   0        0        0      423 2024-05-04 10:14:39.405096 SimpleTKMessageBox-0.2.7/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-05-04 10:14:39.402097 SimpleTKMessageBox-0.2.7/SimpleTKMessageBox.egg-info/
--rw-rw-rw-   0        0        0      423 2024-05-04 10:14:38.000000 SimpleTKMessageBox-0.2.7/SimpleTKMessageBox.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      862 2024-05-04 10:14:38.000000 SimpleTKMessageBox-0.2.7/SimpleTKMessageBox.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-04 10:14:38.000000 SimpleTKMessageBox-0.2.7/SimpleTKMessageBox.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2024-05-04 10:14:38.000000 SimpleTKMessageBox-0.2.7/SimpleTKMessageBox.egg-info/requires.txt
--rw-rw-rw-   0        0        0       19 2024-05-04 10:14:38.000000 SimpleTKMessageBox-0.2.7/SimpleTKMessageBox.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-05-04 10:14:38.936361 SimpleTKMessageBox-0.2.7/SimpleTkMessageBox/
--rw-rw-rw-   0        0        0     3646 2024-05-04 10:13:55.000000 SimpleTKMessageBox-0.2.7/SimpleTkMessageBox/SimpleTkMessageBox.py
--rw-rw-rw-   0        0        0       59 2024-04-27 10:36:23.000000 SimpleTKMessageBox-0.2.7/SimpleTkMessageBox/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-04 10:14:38.998327 SimpleTKMessageBox-0.2.7/SimpleTkMessageBox/icons/
-drwxrwxrwx   0        0        0        0 2024-05-04 10:14:39.107263 SimpleTKMessageBox-0.2.7/SimpleTkMessageBox/icons/W10/
--rw-rw-rw-   0        0        0     1051 2024-04-23 17:11:13.000000 SimpleTKMessageBox-0.2.7/SimpleTkMessageBox/icons/W10/1.png
--rw-rw-rw-   0        0        0     1395 2024-04-23 17:11:13.000000 SimpleTKMessageBox-0.2.7/SimpleTkMessageBox/icons/W10/2.png
--rw-rw-rw-   0        0        0      725 2024-04-23 17:11:13.000000 SimpleTKMessageBox-0.2.7/SimpleTkMessageBox/icons/W10/3.png
--rw-rw-rw-   0        0        0     1423 2024-04-23 17:11:13.000000 SimpleTKMessageBox-0.2.7/SimpleTkMessageBox/icons/W10/4.png
--rw-rw-rw-   0        0        0     1145 2024-04-23 17:11:13.000000 SimpleTKMessageBox-0.2.7/SimpleTkMessageBox/icons/W10/5.png
-drwxrwxrwx   0        0        0        0 2024-05-04 10:14:39.159234 SimpleTKMessageBox-0.2.7/SimpleTkMessageBox/icons/W11/
--rw-rw-rw-   0        0        0     3154 2024-04-23 17:12:10.000000 SimpleTKMessageBox-0.2.7/SimpleTkMessageBox/icons/W11/1.png
--rw-rw-rw-   0        0        0     1847 2024-04-23 17:12:10.000000 SimpleTKMessageBox-0.2.7/SimpleTkMessageBox/icons/W11/2.png
--rw-rw-rw-   0        0        0     3264 2024-04-23 17:12:10.000000 SimpleTKMessageBox-0.2.7/SimpleTkMessageBox/icons/W11/3.png
--rw-rw-rw-   0        0        0     4962 2024-04-23 17:12:10.000000 SimpleTKMessageBox-0.2.7/SimpleTkMessageBox/icons/W11/4.png
--rw-rw-rw-   0        0        0     4565 2024-04-23 17:12:10.000000 SimpleTKMessageBox-0.2.7/SimpleTkMessageBox/icons/W11/5.png
-drwxrwxrwx   0        0        0        0 2024-05-04 10:14:39.381107 SimpleTKMessageBox-0.2.7/SimpleTkMessageBox/icons/W7/
--rw-rw-rw-   0        0        0     6639 2024-04-23 17:03:58.000000 SimpleTKMessageBox-0.2.7/SimpleTkMessageBox/icons/W7/1.png
--rw-rw-rw-   0        0        0     2797 2024-04-23 17:01:54.000000 SimpleTKMessageBox-0.2.7/SimpleTkMessageBox/icons/W7/2.png
--rw-rw-rw-   0        0        0     5154 2024-04-23 17:01:56.000000 SimpleTKMessageBox-0.2.7/SimpleTkMessageBox/icons/W7/3.png
--rw-rw-rw-   0        0        0     6070 2024-04-23 17:01:59.000000 SimpleTKMessageBox-0.2.7/SimpleTkMessageBox/icons/W7/4.png
--rw-rw-rw-   0        0        0     5708 2024-04-23 17:02:02.000000 SimpleTKMessageBox-0.2.7/SimpleTkMessageBox/icons/W7/5.png
--rw-rw-rw-   0        0        0     1406 2024-04-24 08:46:15.000000 SimpleTKMessageBox-0.2.7/SimpleTkMessageBox/icons/transparent.ico
--rw-rw-rw-   0        0        0       42 2024-05-04 10:14:39.418087 SimpleTKMessageBox-0.2.7/setup.cfg
--rw-rw-rw-   0        0        0     1334 2024-05-04 10:14:33.000000 SimpleTKMessageBox-0.2.7/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-04 12:14:04.098902 SimpleTKMessageBox-0.2.8/
+-rw-rw-rw-   0        0        0       25 2024-04-27 11:31:25.000000 SimpleTKMessageBox-0.2.8/MANIFEST.in
+-rw-rw-rw-   0        0        0      423 2024-05-04 12:14:04.089574 SimpleTKMessageBox-0.2.8/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-05-04 12:14:04.086644 SimpleTKMessageBox-0.2.8/SimpleTKMessageBox.egg-info/
+-rw-rw-rw-   0        0        0      423 2024-05-04 12:14:03.000000 SimpleTKMessageBox-0.2.8/SimpleTKMessageBox.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      862 2024-05-04 12:14:03.000000 SimpleTKMessageBox-0.2.8/SimpleTKMessageBox.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-04 12:14:03.000000 SimpleTKMessageBox-0.2.8/SimpleTKMessageBox.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        7 2024-05-04 12:14:03.000000 SimpleTKMessageBox-0.2.8/SimpleTKMessageBox.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       19 2024-05-04 12:14:03.000000 SimpleTKMessageBox-0.2.8/SimpleTKMessageBox.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-04 12:14:03.973816 SimpleTKMessageBox-0.2.8/SimpleTkMessageBox/
+-rw-rw-rw-   0        0        0     3840 2024-05-04 12:12:52.000000 SimpleTKMessageBox-0.2.8/SimpleTkMessageBox/SimpleTkMessageBox.py
+-rw-rw-rw-   0        0        0       59 2024-04-27 10:36:23.000000 SimpleTKMessageBox-0.2.8/SimpleTkMessageBox/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-04 12:14:03.983589 SimpleTKMessageBox-0.2.8/SimpleTkMessageBox/icons/
+drwxrwxrwx   0        0        0        0 2024-05-04 12:14:04.011460 SimpleTKMessageBox-0.2.8/SimpleTkMessageBox/icons/W10/
+-rw-rw-rw-   0        0        0     1051 2024-04-23 17:11:13.000000 SimpleTKMessageBox-0.2.8/SimpleTkMessageBox/icons/W10/1.png
+-rw-rw-rw-   0        0        0     1395 2024-04-23 17:11:13.000000 SimpleTKMessageBox-0.2.8/SimpleTkMessageBox/icons/W10/2.png
+-rw-rw-rw-   0        0        0      725 2024-04-23 17:11:13.000000 SimpleTKMessageBox-0.2.8/SimpleTkMessageBox/icons/W10/3.png
+-rw-rw-rw-   0        0        0     1423 2024-04-23 17:11:13.000000 SimpleTKMessageBox-0.2.8/SimpleTkMessageBox/icons/W10/4.png
+-rw-rw-rw-   0        0        0     1145 2024-04-23 17:11:13.000000 SimpleTKMessageBox-0.2.8/SimpleTkMessageBox/icons/W10/5.png
+drwxrwxrwx   0        0        0        0 2024-05-04 12:14:04.045632 SimpleTKMessageBox-0.2.8/SimpleTkMessageBox/icons/W11/
+-rw-rw-rw-   0        0        0     3154 2024-04-23 17:12:10.000000 SimpleTKMessageBox-0.2.8/SimpleTkMessageBox/icons/W11/1.png
+-rw-rw-rw-   0        0        0     1847 2024-04-23 17:12:10.000000 SimpleTKMessageBox-0.2.8/SimpleTkMessageBox/icons/W11/2.png
+-rw-rw-rw-   0        0        0     3264 2024-04-23 17:12:10.000000 SimpleTKMessageBox-0.2.8/SimpleTkMessageBox/icons/W11/3.png
+-rw-rw-rw-   0        0        0     4962 2024-04-23 17:12:10.000000 SimpleTKMessageBox-0.2.8/SimpleTkMessageBox/icons/W11/4.png
+-rw-rw-rw-   0        0        0     4565 2024-04-23 17:12:10.000000 SimpleTKMessageBox-0.2.8/SimpleTkMessageBox/icons/W11/5.png
+drwxrwxrwx   0        0        0        0 2024-05-04 12:14:04.075899 SimpleTKMessageBox-0.2.8/SimpleTkMessageBox/icons/W7/
+-rw-rw-rw-   0        0        0     6639 2024-04-23 17:03:58.000000 SimpleTKMessageBox-0.2.8/SimpleTkMessageBox/icons/W7/1.png
+-rw-rw-rw-   0        0        0     2797 2024-04-23 17:01:54.000000 SimpleTKMessageBox-0.2.8/SimpleTkMessageBox/icons/W7/2.png
+-rw-rw-rw-   0        0        0     5154 2024-04-23 17:01:56.000000 SimpleTKMessageBox-0.2.8/SimpleTkMessageBox/icons/W7/3.png
+-rw-rw-rw-   0        0        0     6070 2024-04-23 17:01:59.000000 SimpleTKMessageBox-0.2.8/SimpleTkMessageBox/icons/W7/4.png
+-rw-rw-rw-   0        0        0     5708 2024-04-23 17:02:02.000000 SimpleTKMessageBox-0.2.8/SimpleTkMessageBox/icons/W7/5.png
+-rw-rw-rw-   0        0        0     1406 2024-04-24 08:46:15.000000 SimpleTKMessageBox-0.2.8/SimpleTkMessageBox/icons/transparent.ico
+-rw-rw-rw-   0        0        0       42 2024-05-04 12:14:04.099881 SimpleTKMessageBox-0.2.8/setup.cfg
+-rw-rw-rw-   0        0        0     1334 2024-05-04 12:13:20.000000 SimpleTKMessageBox-0.2.8/setup.py
```

### Comparing `SimpleTKMessageBox-0.2.7/SimpleTKMessageBox.egg-info/SOURCES.txt` & `SimpleTKMessageBox-0.2.8/SimpleTKMessageBox.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `SimpleTKMessageBox-0.2.7/SimpleTkMessageBox/SimpleTkMessageBox.py` & `SimpleTKMessageBox-0.2.8/SimpleTkMessageBox/SimpleTkMessageBox.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from tkinter import ttk
 import tkinter
 import os
 import sys
 from PIL import Image, ImageTk 
+from tkinter import font
 import platform
 
 def ShowMSBox(master, Icon="Information", Title="Message Box", IconStyle="Windows 10", button1="", button2="", button3="", text="This is an info"):
     MsB = tkinter.Toplevel(master)
     StyleList = ["Windows 11","Windows 10", "Windows 7", "Personalized"]
     if not IconStyle in StyleList:
         raise ValueError("Invalid Style : " + IconStyle + ". It should be one of 'Windows 11', 'Windows 10', 'Windows 7' or 'Personalized'.")
@@ -83,21 +84,28 @@
     if button3!="":
         MsBbtn3 = ttk.Button(master=MsB, text=button3, command=btn3IsPushed)
         MsBbtn3.place(x=315, y=155)
         style = ttk.Style()
         style.configure("BW.TButton", background=colorFrame.cget("bg"))
         MsBbtn3.config(style="BW.TButton")
 
-    MsBtext = ttk.Label(MsB, text=text)
+    TKFONT = font.nametofont("TkDefaultFont")
+
+    MsBtext = ttk.Label(MsB, text=text, font=(TKFONT, 10))
     MsBtext.place(x=100, y=60)
-    WindowIcon = os.path.join(os.path.dirname(os.path.realpath(__file__)), 'icons', 'transparent.ico')
-    MsB.title(Title)
+
     if platform.system() == "Windows":
-        MsB.geometry("400x200")
-    else:
-        MsB.geometry("410x200")
+        WindowIcon = os.path.join(os.path.dirname(os.path.realpath(__file__)), 'icons', 'transparent.ico')
+        MsB.iconbitmap(WindowIcon)
+    MsB.title(Title)
+    MsB.geometry("400x200")
     MsB.resizable(False, False)
-    MsB.iconbitmap(WindowIcon)
     MsB.transient(master)
     MsB.grab_set()
     MsB.wait_window(MsB)
-    return button_pressed
+    return button_pressed
+
+root = tkinter.Tk()
+
+ShowMSBox(root, Icon="Information", Title="Test Message Box", text="This is a test message.")
+
+root.destroy()
```

### Comparing `SimpleTKMessageBox-0.2.7/SimpleTkMessageBox/icons/W10/1.png` & `SimpleTKMessageBox-0.2.8/SimpleTkMessageBox/icons/W10/1.png`

 * *Files identical despite different names*

### Comparing `SimpleTKMessageBox-0.2.7/SimpleTkMessageBox/icons/W10/2.png` & `SimpleTKMessageBox-0.2.8/SimpleTkMessageBox/icons/W10/2.png`

 * *Files identical despite different names*

### Comparing `SimpleTKMessageBox-0.2.7/SimpleTkMessageBox/icons/W10/3.png` & `SimpleTKMessageBox-0.2.8/SimpleTkMessageBox/icons/W10/3.png`

 * *Files identical despite different names*

### Comparing `SimpleTKMessageBox-0.2.7/SimpleTkMessageBox/icons/W10/4.png` & `SimpleTKMessageBox-0.2.8/SimpleTkMessageBox/icons/W10/4.png`

 * *Files identical despite different names*

### Comparing `SimpleTKMessageBox-0.2.7/SimpleTkMessageBox/icons/W10/5.png` & `SimpleTKMessageBox-0.2.8/SimpleTkMessageBox/icons/W10/5.png`

 * *Files identical despite different names*

### Comparing `SimpleTKMessageBox-0.2.7/SimpleTkMessageBox/icons/W11/1.png` & `SimpleTKMessageBox-0.2.8/SimpleTkMessageBox/icons/W11/1.png`

 * *Files identical despite different names*

### Comparing `SimpleTKMessageBox-0.2.7/SimpleTkMessageBox/icons/W11/2.png` & `SimpleTKMessageBox-0.2.8/SimpleTkMessageBox/icons/W11/2.png`

 * *Files identical despite different names*

### Comparing `SimpleTKMessageBox-0.2.7/SimpleTkMessageBox/icons/W11/3.png` & `SimpleTKMessageBox-0.2.8/SimpleTkMessageBox/icons/W11/3.png`

 * *Files identical despite different names*

### Comparing `SimpleTKMessageBox-0.2.7/SimpleTkMessageBox/icons/W11/4.png` & `SimpleTKMessageBox-0.2.8/SimpleTkMessageBox/icons/W11/4.png`

 * *Files identical despite different names*

### Comparing `SimpleTKMessageBox-0.2.7/SimpleTkMessageBox/icons/W11/5.png` & `SimpleTKMessageBox-0.2.8/SimpleTkMessageBox/icons/W11/5.png`

 * *Files identical despite different names*

### Comparing `SimpleTKMessageBox-0.2.7/SimpleTkMessageBox/icons/W7/1.png` & `SimpleTKMessageBox-0.2.8/SimpleTkMessageBox/icons/W7/1.png`

 * *Files identical despite different names*

### Comparing `SimpleTKMessageBox-0.2.7/SimpleTkMessageBox/icons/W7/2.png` & `SimpleTKMessageBox-0.2.8/SimpleTkMessageBox/icons/W7/2.png`

 * *Files identical despite different names*

### Comparing `SimpleTKMessageBox-0.2.7/SimpleTkMessageBox/icons/W7/3.png` & `SimpleTKMessageBox-0.2.8/SimpleTkMessageBox/icons/W7/3.png`

 * *Files identical despite different names*

### Comparing `SimpleTKMessageBox-0.2.7/SimpleTkMessageBox/icons/W7/4.png` & `SimpleTKMessageBox-0.2.8/SimpleTkMessageBox/icons/W7/4.png`

 * *Files identical despite different names*

### Comparing `SimpleTKMessageBox-0.2.7/SimpleTkMessageBox/icons/W7/5.png` & `SimpleTKMessageBox-0.2.8/SimpleTkMessageBox/icons/W7/5.png`

 * *Files identical despite different names*

### Comparing `SimpleTKMessageBox-0.2.7/SimpleTkMessageBox/icons/transparent.ico` & `SimpleTKMessageBox-0.2.8/SimpleTkMessageBox/icons/transparent.ico`

 * *Files identical despite different names*

### Comparing `SimpleTKMessageBox-0.2.7/setup.py` & `SimpleTKMessageBox-0.2.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from setuptools import setup, find_packages
 setup(
 name='SimpleTKMessageBox',
-version='0.2.7',
+version='0.2.8',
 author='Gustoon',
 author_email='no.email@gmail.com',
 description='A simple tkinter message box',
 long_description="""
 See documentation at https://github.com/Gustoon/SimpleTkMessageBox
 """,
 packages=find_packages(),
```

