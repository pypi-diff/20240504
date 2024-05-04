# Comparing `tmp/CustomTkinterTitlebar-1.0.8.2.tar.gz` & `tmp/customtkintertitlebar-1.0.8.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "CustomTkinterTitlebar-1.0.8.2.tar", last modified: Fri Feb 16 00:38:56 2024, max compression
+gzip compressed data, was "customtkintertitlebar-1.0.8.3.tar", last modified: Sat May  4 11:01:33 2024, max compression
```

## Comparing `CustomTkinterTitlebar-1.0.8.2.tar` & `customtkintertitlebar-1.0.8.3.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 00:38:56.396381 CustomTkinterTitlebar-1.0.8.2/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 00:38:56.396381 CustomTkinterTitlebar-1.0.8.2/CustomTkinterTitlebar.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1921 2024-02-16 00:38:56.000000 CustomTkinterTitlebar-1.0.8.2/CustomTkinterTitlebar.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1018 2024-02-16 00:38:56.000000 CustomTkinterTitlebar-1.0.8.2/CustomTkinterTitlebar.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-16 00:38:56.000000 CustomTkinterTitlebar-1.0.8.2/CustomTkinterTitlebar.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-02-16 00:38:56.000000 CustomTkinterTitlebar-1.0.8.2/CustomTkinterTitlebar.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1078 2024-02-16 00:38:45.000000 CustomTkinterTitlebar-1.0.8.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       88 2024-02-16 00:38:45.000000 CustomTkinterTitlebar-1.0.8.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     1921 2024-02-16 00:38:56.396381 CustomTkinterTitlebar-1.0.8.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1119 2024-02-16 00:38:45.000000 CustomTkinterTitlebar-1.0.8.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 00:38:56.392381 CustomTkinterTitlebar-1.0.8.2/customtitlebar/
--rw-r--r--   0 runner    (1001) docker     (127)      290 2024-02-16 00:38:45.000000 CustomTkinterTitlebar-1.0.8.2/customtitlebar/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 00:38:56.392381 CustomTkinterTitlebar-1.0.8.2/customtitlebar/asset/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 00:38:56.396381 CustomTkinterTitlebar-1.0.8.2/customtitlebar/asset/dark/
--rw-r--r--   0 runner    (1001) docker     (127)      297 2024-02-16 00:38:45.000000 CustomTkinterTitlebar-1.0.8.2/customtitlebar/asset/dark/close_100.png
--rw-r--r--   0 runner    (1001) docker     (127)      346 2024-02-16 00:38:45.000000 CustomTkinterTitlebar-1.0.8.2/customtitlebar/asset/dark/close_50.png
--rw-r--r--   0 runner    (1001) docker     (127)      169 2024-02-16 00:38:45.000000 CustomTkinterTitlebar-1.0.8.2/customtitlebar/asset/dark/fullwin_100.png
--rw-r--r--   0 runner    (1001) docker     (127)      200 2024-02-16 00:38:45.000000 CustomTkinterTitlebar-1.0.8.2/customtitlebar/asset/dark/fullwin_50.png
--rw-r--r--   0 runner    (1001) docker     (127)      120 2024-02-16 00:38:45.000000 CustomTkinterTitlebar-1.0.8.2/customtitlebar/asset/dark/minisize_100.png
--rw-r--r--   0 runner    (1001) docker     (127)      123 2024-02-16 00:38:45.000000 CustomTkinterTitlebar-1.0.8.2/customtitlebar/asset/dark/minisize_50.png
--rw-r--r--   0 runner    (1001) docker     (127)      238 2024-02-16 00:38:45.000000 CustomTkinterTitlebar-1.0.8.2/customtitlebar/asset/dark/togglefull_100.png
--rw-r--r--   0 runner    (1001) docker     (127)      392 2024-02-16 00:38:45.000000 CustomTkinterTitlebar-1.0.8.2/customtitlebar/asset/dark/togglefull_50.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 00:38:56.396381 CustomTkinterTitlebar-1.0.8.2/customtitlebar/asset/light/
--rw-r--r--   0 runner    (1001) docker     (127)      340 2024-02-16 00:38:45.000000 CustomTkinterTitlebar-1.0.8.2/customtitlebar/asset/light/close_100.png
--rw-r--r--   0 runner    (1001) docker     (127)      428 2024-02-16 00:38:45.000000 CustomTkinterTitlebar-1.0.8.2/customtitlebar/asset/light/close_50.png
--rw-r--r--   0 runner    (1001) docker     (127)      211 2024-02-16 00:38:45.000000 CustomTkinterTitlebar-1.0.8.2/customtitlebar/asset/light/fullwin_100.png
--rw-r--r--   0 runner    (1001) docker     (127)      203 2024-02-16 00:38:45.000000 CustomTkinterTitlebar-1.0.8.2/customtitlebar/asset/light/fullwin_50.png
--rw-r--r--   0 runner    (1001) docker     (127)       94 2024-02-16 00:38:45.000000 CustomTkinterTitlebar-1.0.8.2/customtitlebar/asset/light/minisize_100.png
--rw-r--r--   0 runner    (1001) docker     (127)      106 2024-02-16 00:38:45.000000 CustomTkinterTitlebar-1.0.8.2/customtitlebar/asset/light/minisize_50.png
--rw-r--r--   0 runner    (1001) docker     (127)      259 2024-02-16 00:38:45.000000 CustomTkinterTitlebar-1.0.8.2/customtitlebar/asset/light/togglefull_100.png
--rw-r--r--   0 runner    (1001) docker     (127)      434 2024-02-16 00:38:45.000000 CustomTkinterTitlebar-1.0.8.2/customtitlebar/asset/light/togglefull_50.png
--rw-r--r--   0 runner    (1001) docker     (127)    57022 2024-02-16 00:38:45.000000 CustomTkinterTitlebar-1.0.8.2/customtitlebar/asset/tk.ico
--rw-r--r--   0 runner    (1001) docker     (127)      595 2024-02-16 00:38:45.000000 CustomTkinterTitlebar-1.0.8.2/customtitlebar/data.py
--rw-r--r--   0 runner    (1001) docker     (127)    11371 2024-02-16 00:38:45.000000 CustomTkinterTitlebar-1.0.8.2/customtitlebar/titlebar.py
--rw-r--r--   0 runner    (1001) docker     (127)      135 2024-02-16 00:38:45.000000 CustomTkinterTitlebar-1.0.8.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-16 00:38:56.396381 CustomTkinterTitlebar-1.0.8.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1114 2024-02-16 00:38:45.000000 CustomTkinterTitlebar-1.0.8.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 11:01:33.524961 customtkintertitlebar-1.0.8.3/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 11:01:33.524961 customtkintertitlebar-1.0.8.3/CustomTkinterTitlebar.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1821 2024-05-04 11:01:33.000000 customtkintertitlebar-1.0.8.3/CustomTkinterTitlebar.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1018 2024-05-04 11:01:33.000000 customtkintertitlebar-1.0.8.3/CustomTkinterTitlebar.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-04 11:01:33.000000 customtkintertitlebar-1.0.8.3/CustomTkinterTitlebar.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-04 11:01:33.000000 customtkintertitlebar-1.0.8.3/CustomTkinterTitlebar.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1078 2024-05-04 11:01:29.000000 customtkintertitlebar-1.0.8.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       88 2024-05-04 11:01:29.000000 customtkintertitlebar-1.0.8.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1821 2024-05-04 11:01:33.524961 customtkintertitlebar-1.0.8.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1119 2024-05-04 11:01:29.000000 customtkintertitlebar-1.0.8.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 11:01:33.524961 customtkintertitlebar-1.0.8.3/customtitlebar/
+-rw-r--r--   0 runner    (1001) docker     (127)      298 2024-05-04 11:01:29.000000 customtkintertitlebar-1.0.8.3/customtitlebar/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 11:01:33.524961 customtkintertitlebar-1.0.8.3/customtitlebar/asset/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 11:01:33.524961 customtkintertitlebar-1.0.8.3/customtitlebar/asset/dark/
+-rw-r--r--   0 runner    (1001) docker     (127)      297 2024-05-04 11:01:29.000000 customtkintertitlebar-1.0.8.3/customtitlebar/asset/dark/close_100.png
+-rw-r--r--   0 runner    (1001) docker     (127)      346 2024-05-04 11:01:29.000000 customtkintertitlebar-1.0.8.3/customtitlebar/asset/dark/close_50.png
+-rw-r--r--   0 runner    (1001) docker     (127)      169 2024-05-04 11:01:29.000000 customtkintertitlebar-1.0.8.3/customtitlebar/asset/dark/fullwin_100.png
+-rw-r--r--   0 runner    (1001) docker     (127)      200 2024-05-04 11:01:29.000000 customtkintertitlebar-1.0.8.3/customtitlebar/asset/dark/fullwin_50.png
+-rw-r--r--   0 runner    (1001) docker     (127)      120 2024-05-04 11:01:29.000000 customtkintertitlebar-1.0.8.3/customtitlebar/asset/dark/minisize_100.png
+-rw-r--r--   0 runner    (1001) docker     (127)      123 2024-05-04 11:01:29.000000 customtkintertitlebar-1.0.8.3/customtitlebar/asset/dark/minisize_50.png
+-rw-r--r--   0 runner    (1001) docker     (127)      238 2024-05-04 11:01:29.000000 customtkintertitlebar-1.0.8.3/customtitlebar/asset/dark/togglefull_100.png
+-rw-r--r--   0 runner    (1001) docker     (127)      392 2024-05-04 11:01:29.000000 customtkintertitlebar-1.0.8.3/customtitlebar/asset/dark/togglefull_50.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 11:01:33.524961 customtkintertitlebar-1.0.8.3/customtitlebar/asset/light/
+-rw-r--r--   0 runner    (1001) docker     (127)      340 2024-05-04 11:01:29.000000 customtkintertitlebar-1.0.8.3/customtitlebar/asset/light/close_100.png
+-rw-r--r--   0 runner    (1001) docker     (127)      428 2024-05-04 11:01:29.000000 customtkintertitlebar-1.0.8.3/customtitlebar/asset/light/close_50.png
+-rw-r--r--   0 runner    (1001) docker     (127)      211 2024-05-04 11:01:29.000000 customtkintertitlebar-1.0.8.3/customtitlebar/asset/light/fullwin_100.png
+-rw-r--r--   0 runner    (1001) docker     (127)      203 2024-05-04 11:01:29.000000 customtkintertitlebar-1.0.8.3/customtitlebar/asset/light/fullwin_50.png
+-rw-r--r--   0 runner    (1001) docker     (127)       94 2024-05-04 11:01:29.000000 customtkintertitlebar-1.0.8.3/customtitlebar/asset/light/minisize_100.png
+-rw-r--r--   0 runner    (1001) docker     (127)      106 2024-05-04 11:01:29.000000 customtkintertitlebar-1.0.8.3/customtitlebar/asset/light/minisize_50.png
+-rw-r--r--   0 runner    (1001) docker     (127)      259 2024-05-04 11:01:29.000000 customtkintertitlebar-1.0.8.3/customtitlebar/asset/light/togglefull_100.png
+-rw-r--r--   0 runner    (1001) docker     (127)      434 2024-05-04 11:01:29.000000 customtkintertitlebar-1.0.8.3/customtitlebar/asset/light/togglefull_50.png
+-rw-r--r--   0 runner    (1001) docker     (127)    57022 2024-05-04 11:01:29.000000 customtkintertitlebar-1.0.8.3/customtitlebar/asset/tk.ico
+-rw-r--r--   0 runner    (1001) docker     (127)      715 2024-05-04 11:01:29.000000 customtkintertitlebar-1.0.8.3/customtitlebar/data.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12747 2024-05-04 11:01:29.000000 customtkintertitlebar-1.0.8.3/customtitlebar/titlebar.py
+-rw-r--r--   0 runner    (1001) docker     (127)      135 2024-05-04 11:01:29.000000 customtkintertitlebar-1.0.8.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-04 11:01:33.524961 customtkintertitlebar-1.0.8.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1017 2024-05-04 11:01:29.000000 customtkintertitlebar-1.0.8.3/setup.py
```

### Comparing `CustomTkinterTitlebar-1.0.8.2/CustomTkinterTitlebar.egg-info/PKG-INFO` & `customtkintertitlebar-1.0.8.3/CustomTkinterTitlebar.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,20 +1,18 @@
 Metadata-Version: 2.1
 Name: CustomTkinterTitlebar
-Version: 1.0.8.2
+Version: 1.0.8.3
 Summary: This is a 📚project can help you to have a custom titlebar! 这是一个可以创建自定义标题栏的📚项目
 Home-page: https://github.com/littlewhitecloud/CustomTkinterTitlebar
 Author: littlewhitecloud
 Author-email: q1141926647@163.com
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # _自定义标题栏_ _CustomTkinterTitlebar_
```

### Comparing `CustomTkinterTitlebar-1.0.8.2/CustomTkinterTitlebar.egg-info/SOURCES.txt` & `customtkintertitlebar-1.0.8.3/CustomTkinterTitlebar.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `CustomTkinterTitlebar-1.0.8.2/LICENSE` & `customtkintertitlebar-1.0.8.3/LICENSE`

 * *Files identical despite different names*

### Comparing `CustomTkinterTitlebar-1.0.8.2/PKG-INFO` & `customtkintertitlebar-1.0.8.3/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,20 +1,18 @@
 Metadata-Version: 2.1
 Name: CustomTkinterTitlebar
-Version: 1.0.8.2
+Version: 1.0.8.3
 Summary: This is a 📚project can help you to have a custom titlebar! 这是一个可以创建自定义标题栏的📚项目
 Home-page: https://github.com/littlewhitecloud/CustomTkinterTitlebar
 Author: littlewhitecloud
 Author-email: q1141926647@163.com
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # _自定义标题栏_ _CustomTkinterTitlebar_
```

### Comparing `CustomTkinterTitlebar-1.0.8.2/README.md` & `customtkintertitlebar-1.0.8.3/README.md`

 * *Files identical despite different names*

### Comparing `CustomTkinterTitlebar-1.0.8.2/customtitlebar/asset/tk.ico` & `customtkintertitlebar-1.0.8.3/customtitlebar/asset/tk.ico`

 * *Files identical despite different names*

### Comparing `CustomTkinterTitlebar-1.0.8.2/customtitlebar/data.py` & `customtkintertitlebar-1.0.8.3/customtitlebar/data.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,19 +1,25 @@
 from ctypes import POINTER, Structure, c_int
 from ctypes.wintypes import HWND, RECT, UINT
 
 WM_NCCALCSIZE = 0x0083
+WM_NCHITTEST = 0x0084
+
+WS_CAPTION = 0x00C00000
+WS_VISIBLE = 0x10000000
+WS_THICKFRAME = 0x00040000
 
 SWP_NOSIZE = 0x0001
 SWP_NOREDRAW = 0x0008
 SWP_FRAMECHANGED = 0x0020
 
 SW_MAXIMIZE = 3
 SW_NORMAL = 1
 
+GWL_STYLE = -16
 GWL_WNDPROC = -4
 
 
 class PWINDOWPOS(Structure):
     _fields_ = [
         ("hWnd", HWND),
         ("hwndInsertAfter", HWND),
```

### Comparing `CustomTkinterTitlebar-1.0.8.2/customtitlebar/titlebar.py` & `customtkintertitlebar-1.0.8.3/customtitlebar/titlebar.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,19 +1,18 @@
 """A special window for custom titlebar"""
 
 from ctypes import WINFUNCTYPE, c_char_p, c_uint64, windll
 from pathlib import Path
-from tkinter import Button, Event, Frame, Label, Tk
+from tkinter import Button, Event, Frame, Label, Tk, Toplevel
 from typing import Any, Mapping
 
 from darkdetect import isDark
 from PIL import Image, ImageTk
 
 from .data import *
-
 env = Path(__file__).parent
 
 
 class CTT(Tk):
     """Custom Tkinter Titlebar Window Class"""
 
     def __init__(self, theme: str = "auto") -> None:
@@ -45,19 +44,25 @@
         self.max_img = ImageTk.PhotoImage(Image.open(self.path / "togglefull_50.png"))
         self.close_hov_img = ImageTk.PhotoImage(Image.open(self.path / "close_100.png"))
         self.min_hov_img = ImageTk.PhotoImage(Image.open(self.path / "minisize_100.png"))
         self.full_hov_img = ImageTk.PhotoImage(Image.open(self.path / "fullwin_100.png"))
         self.max_hov_img = ImageTk.PhotoImage(Image.open(self.path / "togglefull_100.png"))
 
         self.titlebar = Frame(self, bg=self.bg, height=30)
-        self.icon = Label(self.titlebar, bg=self.bg)
-        self.text = Label(self.titlebar, bg=self.bg, fg=self.colors[self.fg])
-        self.min = Button(self.titlebar, bg=self.bg, bd=0, width=44, relief="flat")
-        self.max = Button(self.titlebar, bg=self.bg, bd=0, width=44, relief="flat")
-        self.exit = Button(self.titlebar, bg=self.bg, bd=0, width=44, relief="flat")
+        self.buttongroup = Frame(self.titlebar, bg=self.bg)
+        self.infogroup = Frame(self.titlebar, bg=self.bg)
+        self.icon = Label(self.infogroup, bg=self.bg)
+        self.text = Label(self.infogroup, bg=self.bg, fg=self.colors[self.fg])
+
+        self.min = Button(self.buttongroup)
+        self.max = Button(self.buttongroup)
+        self.exit = Button(self.buttongroup)
+
+        for widget in (self.min, self.max, self.exit):
+            widget.config(bg=self.bg, bd=0, width=44, height=30, relief="flat")
 
         self.exit.config(
             activebackground=self.colors[f"{self.theme}exit_bg"],
             image=self.close_hov_img,
             command=self.quit,
         )
         self.min.config(
@@ -88,20 +93,22 @@
             widget.bind("<ButtonPress-1>", self.dragging)
             widget.bind("<B1-Motion>", self.moving)
 
         self.titlebar.bind("<Double-Button-1>", self.maximize)
 
         self.setup()
 
-        self.icon.pack(fill="y", side="left", padx=5, pady=5)
-        self.text.pack(fill="y", side="left", pady=5, padx=5)
+        self.icon.pack(fill="x", side="left")
+        self.text.pack(fill="x", side="left")
         self.exit.pack(fill="y", side="right")
         self.max.pack(fill="y", side="right")
         self.min.pack(fill="y", side="right")
-        self.titlebar.pack(fill="x", side="top")
+        self.infogroup.pack(fill = "x", side = "left", padx=5, pady=5)
+        self.buttongroup.pack(fill = "y", side="right")
+        self.titlebar.pack(fill="x", side="top", expand=False)
         self.titlebar.pack_propagate(False)
 
     # Window
     def setup(self) -> None:
         """Window Setup"""
 
         def handle(hwnd: int, msg: int, wp: int, lp: int) -> int:
@@ -115,21 +122,21 @@
         self.geometry(f"{self.width}x{self.height}")
         self.iconbitmap(str(env / "asset" / "tk.ico"))
 
         self.hwnd = windll.user32.FindWindowW(c_char_p(None), "Tk")
 
         old, new = "old", "new"
         prototype = WINFUNCTYPE(c_uint64, c_uint64, c_uint64, c_uint64, c_uint64)
+
         globals()[old] = None
         globals()[new] = prototype(handle)
         globals()[old] = windll.user32.GetWindowLongPtrA(self.hwnd, GWL_WNDPROC)
         windll.user32.SetWindowLongPtrA(self.hwnd, GWL_WNDPROC, globals()[new])
 
         self.update()
-        self.focus_force()
 
     def dragging(self, event: Event) -> None:
         """Drag the window"""
         self.x = event.x
         self.y = event.y
 
     def moving(self, event: Event) -> None:
@@ -151,15 +158,14 @@
         """Maximize Window"""
         self.fullscreen = True
 
         self.max.config(image=self.max_hov_img, command=self.resize)
         self.titlebar.bind("<Double-Button-1>", self.resize)
 
         windll.user32.ShowWindow(self.hwnd, SW_MAXIMIZE)
-        # TODO: leave a place for the taskbar
 
     def resize(self, _: Event | None = None) -> None:
         """Resize window"""
         self.fullscreen = False
         self.max.config(image=self.full_hov_img, command=self.maximize)
         self.titlebar.bind("<Double-Button-1>", self.maximize)
 
@@ -226,14 +232,15 @@
         self.withdraw()
         self.deiconify()
 
     # Functions
     def title(self, text: str) -> None:
         """Rebuild tkinter's title"""
         # TODO: show "..." if title is too long
+
         self.text.config(text=text)
         self.wm_title(text)
 
     def iconphoto(self, image: str) -> None:
         """Rebuild tkinter's iconphoto"""
         self.img = ImageTk.PhotoImage(Image.open(image).resize((16, 16)))
         self.icon.config(image=self.img)
@@ -247,31 +254,35 @@
             return
         self.img = ImageTk.PhotoImage(Image.open(image).resize((16, 16)))
         self.icon.config(image=self.img)
 
     # TODO: parse  %sx%s+%s+%s
     def geometry(self, size: str) -> None:
         """Rebuild tkinter's geometry"""
-        self.width, self.height = size.split("x")[0], size.split("x")[1]
+        tmp = size.split('+')[0].split('x')
+        self.width, self.height = tmp[0], tmp[1]
+
         self.wm_geometry(size)
 
     def settheme(self, theme: str) -> None:
         """Config the theme"""
 
         def autotheme() -> str:
             return "dark" if isDark() else "light"
 
-        self.theme = theme
         if theme not in ("dark", "light", "auto"):  # Check the theme
             print(
                 f"Warning: Now the theme is `{theme}`, not matching `D(d)ark` `L(l)ight` `A(a)uto`, using auto mode instead"
             )
             self.theme = autotheme()
-        elif theme == "auto":
+
+        if theme == "auto":
             self.theme = autotheme()
+        else:
+            self.theme = theme
 
         self.bg = self.colors[self.theme]
         self.nf = self.colors[f"{self.theme}_nf"]
         self.fg = "light" if self.theme == "dark" else "dark"
         self.config(background=self.colors[f"{self.theme}_bg"])
         self.update()
 
@@ -288,12 +299,44 @@
                 else self.max.config(image=self.full_hov_img if self.onfocus else self.full_img)
             )
         self.text.config(foreground="white" if self.onfocus else "grey")
 
         if self.theme == "light" and self.onfocus:
             self.text.config(foreground=self.colors[self.fg])
 
-    def focusout(self, _: Event | None = None) -> None:
-        self.setcolor(False)
+    def focusout(self, _: Event | None = None) -> None: self.setcolor(False)
+    def focusin(self, _: Event | None = None) -> None: self.setcolor(True)
+
+class Dialog(Toplevel):
+
+    def __init__(self) -> None:
+        super().__init__()
+
+        self.overrideredirect(True)
+        self.setup()
+
+    def setup(self) -> None:
+
+        def handle(hwnd: int, msg: int, wp: int, lp: int) -> int:
+            if msg == WM_NCCALCSIZE and wp:
+                lpncsp = NCCALCSIZE_PARAMS.from_address(lp)
+                lpncsp.rgrc[0].top -= 6
+
+            return windll.user32.CallWindowProcW(*map(c_uint64, (globals()[old], hwnd, msg, wp, lp)))
+
+        self.title("Tk")
+        self.geometry("300x400")
+        self.iconbitmap("")
+
+        self.hwnd = windll.user32.FindWindowW(c_char_p(None), "Tk")
+
+        windll.user32.SetWindowLongA(self.hwnd, GWL_STYLE, WS_VISIBLE | WS_THICKFRAME)
 
-    def focusin(self, _: Event | None = None) -> None:
-        self.setcolor(True)
+        old, new = "old", "new"
+        prototype = WINFUNCTYPE(c_uint64, c_uint64, c_uint64, c_uint64, c_uint64)
+        globals()[old] = None
+        globals()[new] = prototype(handle)
+        globals()[old] = windll.user32.GetWindowLongPtrA(self.hwnd, GWL_WNDPROC)
+        windll.user32.SetWindowLongPtrA(self.hwnd, GWL_WNDPROC, globals()[new])
+
+        self.update()
+        self.focus_force()
```

### Comparing `CustomTkinterTitlebar-1.0.8.2/setup.py` & `customtkintertitlebar-1.0.8.3/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,30 +1,28 @@
 from distutils.core import setup
 
 with open("README.md", "r", encoding="utf-8") as readme:
     long_description = readme.read()
 
-requires = ["Pillow>=9.0.0", "darkdetect>=0.8.0"]
+requires = ["Pillow>=10.2.0", "darkdetect>=0.8.0"]
 
 setup(
     name="CustomTkinterTitlebar",
-    version="1.0.8.2",
+    version="1.0.8.3",
     author="littlewhitecloud",
     author_email="q1141926647@163.com",
     description="This is a 📚project can help you to have a custom titlebar! 这是一个可以创建自定义标题栏的📚项目",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/littlewhitecloud/CustomTkinterTitlebar",
     package="customtitlebar",
     license="MIT",
     include_package_data=True,
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "License :: OSI Approved :: MIT License",
-        "Programming Language :: Python :: 3.8",
-        "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
         "Programming Language :: Python :: 3.11",
         "Programming Language :: Python :: 3.12",
     ],
 )
```

