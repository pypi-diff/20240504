# Comparing `tmp/setux_repl-0.4.1.tar.gz` & `tmp/setux_repl-0.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/setux_repl-0.4.1.tar", last modified: Sun Aug 23 20:38:56 2020, max compression
+gzip compressed data, was "dist/setux_repl-0.4.2.tar", last modified: Sun Aug 23 20:54:32 2020, max compression
```

## Comparing `setux_repl-0.4.1.tar` & `setux_repl-0.4.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 louis     (4444) louis     (4444)        0 2020-08-23 20:38:56.000000 setux_repl-0.4.1/
--rw-r--r--   0 louis     (4444) louis     (4444)     1208 2020-08-23 20:38:56.000000 setux_repl-0.4.1/PKG-INFO
--rw-r--r--   0 louis     (4444) louis     (4444)      226 2020-08-09 09:57:06.000000 setux_repl-0.4.1/README.rst
--rw-r--r--   0 louis     (4444) louis     (4444)       80 2020-08-23 20:38:56.000000 setux_repl-0.4.1/setup.cfg
--rw-r--r--   0 louis     (4444) louis     (4444)     1203 2020-08-11 07:40:59.000000 setux_repl-0.4.1/setup.py
-drwxr-xr-x   0 louis     (4444) louis     (4444)        0 2020-08-23 20:38:56.000000 setux_repl-0.4.1/setux/
-drwxr-xr-x   0 louis     (4444) louis     (4444)        0 2020-08-23 20:38:56.000000 setux_repl-0.4.1/setux/repl/
--rw-r--r--   0 louis     (4444) louis     (4444)      162 2020-08-23 20:38:33.000000 setux_repl-0.4.1/setux/repl/__init__.py
--rw-r--r--   0 louis     (4444) louis     (4444)     2035 2020-08-23 20:38:33.000000 setux_repl-0.4.1/setux/repl/commands.py
--rw-r--r--   0 louis     (4444) louis     (4444)     1131 2020-08-23 20:38:33.000000 setux_repl-0.4.1/setux/repl/helps.py
--rw-r--r--   0 louis     (4444) louis     (4444)     1656 2020-08-23 10:13:07.000000 setux_repl-0.4.1/setux/repl/repl.py
-drwxr-xr-x   0 louis     (4444) louis     (4444)        0 2020-08-23 20:38:56.000000 setux_repl-0.4.1/setux_repl.egg-info/
--rw-r--r--   0 louis     (4444) louis     (4444)     1208 2020-08-23 20:38:56.000000 setux_repl-0.4.1/setux_repl.egg-info/PKG-INFO
--rw-r--r--   0 louis     (4444) louis     (4444)      250 2020-08-23 20:38:56.000000 setux_repl-0.4.1/setux_repl.egg-info/SOURCES.txt
--rw-r--r--   0 louis     (4444) louis     (4444)        1 2020-08-23 20:38:56.000000 setux_repl-0.4.1/setux_repl.egg-info/dependency_links.txt
--rw-r--r--   0 louis     (4444) louis     (4444)        6 2020-08-23 20:38:56.000000 setux_repl-0.4.1/setux_repl.egg-info/top_level.txt
+drwxr-xr-x   0 louis     (4444) louis     (4444)        0 2020-08-23 20:54:32.000000 setux_repl-0.4.2/
+-rw-r--r--   0 louis     (4444) louis     (4444)     1208 2020-08-23 20:54:32.000000 setux_repl-0.4.2/PKG-INFO
+-rw-r--r--   0 louis     (4444) louis     (4444)      226 2020-08-09 09:57:06.000000 setux_repl-0.4.2/README.rst
+-rw-r--r--   0 louis     (4444) louis     (4444)       80 2020-08-23 20:54:32.000000 setux_repl-0.4.2/setup.cfg
+-rw-r--r--   0 louis     (4444) louis     (4444)     1203 2020-08-11 07:40:59.000000 setux_repl-0.4.2/setup.py
+drwxr-xr-x   0 louis     (4444) louis     (4444)        0 2020-08-23 20:54:32.000000 setux_repl-0.4.2/setux/
+drwxr-xr-x   0 louis     (4444) louis     (4444)        0 2020-08-23 20:54:32.000000 setux_repl-0.4.2/setux/repl/
+-rw-r--r--   0 louis     (4444) louis     (4444)      162 2020-08-23 20:41:11.000000 setux_repl-0.4.2/setux/repl/__init__.py
+-rw-r--r--   0 louis     (4444) louis     (4444)     2328 2020-08-23 20:40:38.000000 setux_repl-0.4.2/setux/repl/commands.py
+-rw-r--r--   0 louis     (4444) louis     (4444)     1221 2020-08-23 20:40:38.000000 setux_repl-0.4.2/setux/repl/helps.py
+-rw-r--r--   0 louis     (4444) louis     (4444)     1656 2020-08-23 10:13:07.000000 setux_repl-0.4.2/setux/repl/repl.py
+drwxr-xr-x   0 louis     (4444) louis     (4444)        0 2020-08-23 20:54:32.000000 setux_repl-0.4.2/setux_repl.egg-info/
+-rw-r--r--   0 louis     (4444) louis     (4444)     1208 2020-08-23 20:54:32.000000 setux_repl-0.4.2/setux_repl.egg-info/PKG-INFO
+-rw-r--r--   0 louis     (4444) louis     (4444)      250 2020-08-23 20:54:32.000000 setux_repl-0.4.2/setux_repl.egg-info/SOURCES.txt
+-rw-r--r--   0 louis     (4444) louis     (4444)        1 2020-08-23 20:54:32.000000 setux_repl-0.4.2/setux_repl.egg-info/dependency_links.txt
+-rw-r--r--   0 louis     (4444) louis     (4444)        6 2020-08-23 20:54:32.000000 setux_repl-0.4.2/setux_repl.egg-info/top_level.txt
```

### Comparing `setux_repl-0.4.1/PKG-INFO` & `setux_repl-0.4.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: setux_repl
-Version: 0.4.1
+Version: 0.4.2
 Summary: System deployment
 Home-page: https://framagit.org/louis-riviere-xyz/setux_repl
 Author: Louis RIVIERE
 Author-email: louis@riviere.xyz
 License: MIT
 Description: ###########
          setux repl
```

### Comparing `setux_repl-0.4.1/setup.py` & `setux_repl-0.4.2/setup.py`

 * *Files identical despite different names*

### Comparing `setux_repl-0.4.1/setux/repl/commands.py` & `setux_repl-0.4.2/setux/repl/commands.py`

 * *Files 12% similar despite different names*

```diff
@@ -83,7 +83,20 @@
 def disable(target, arg):
     target.Service.disable(arg)
 
 def download(target, arg):
     url, dst = arg.split(' ') if ' ' in arg else arg, None
     target.deploy('download', url=url, dst=dst)
 
+def outrun(target, arg):
+    log = target.outrun
+    if log:
+        print(open(log).read())
+    else:
+        print('target outrun not defined')
+
+def outlog(target, arg):
+    log = target.outlog
+    if log:
+        print(open(log).read())
+    else:
+        print('target outlog not defined')
```

### Comparing `setux_repl-0.4.1/setux/repl/helps.py` & `setux_repl-0.4.2/setux/repl/helps.py`

 * *Files 9% similar despite different names*

```diff
@@ -44,8 +44,12 @@
     disable = '''disable service
     ''',
     download = '''download file
     ''',
     logs = '''show log file
         arg = level (default to "info")
     ''',
+    outrun = '''show commands history
+    ''',
+    outlog = '''show commands log
+    ''',
 )
```

### Comparing `setux_repl-0.4.1/setux/repl/repl.py` & `setux_repl-0.4.2/setux/repl/repl.py`

 * *Files identical despite different names*

### Comparing `setux_repl-0.4.1/setux_repl.egg-info/PKG-INFO` & `setux_repl-0.4.2/setux_repl.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: setux-repl
-Version: 0.4.1
+Version: 0.4.2
 Summary: System deployment
 Home-page: https://framagit.org/louis-riviere-xyz/setux_repl
 Author: Louis RIVIERE
 Author-email: louis@riviere.xyz
 License: MIT
 Description: ###########
          setux repl
```

