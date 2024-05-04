# Comparing `tmp/Excalibur2-2.2.tar.gz` & `tmp/excalibur2-2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Excalibur2-2.2.tar", last modified: Thu Feb  8 15:54:11 2024, max compression
+gzip compressed data, was "excalibur2-2.3.tar", last modified: Sat May  4 08:37:21 2024, max compression
```

## Comparing `Excalibur2-2.2.tar` & `excalibur2-2.3.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0 lctfer    (1000) lctfer    (1000)        0 2024-02-08 16:29:02.981382 Excalibur2-2.2/
--rwxrwxrwx   0 lctfer    (1000) lctfer    (1000)     1074 2024-02-07 08:25:01.000000 Excalibur2-2.2/LICENSE
--rwxrwxrwx   0 lctfer    (1000) lctfer    (1000)     1393 2024-02-08 16:29:02.975378 Excalibur2-2.2/PKG-INFO
--rwxrwxrwx   0 lctfer    (1000) lctfer    (1000)     1036 2024-02-08 13:56:53.000000 Excalibur2-2.2/README.md
--rwxrwxrwx   0 lctfer    (1000) lctfer    (1000)      457 2024-02-08 16:28:46.000000 Excalibur2-2.2/pyproject.toml
--rwxrwxrwx   0 lctfer    (1000) lctfer    (1000)       38 2024-02-08 16:29:02.988808 Excalibur2-2.2/setup.cfg
-drwxrwxrwx   0 lctfer    (1000) lctfer    (1000)        0 2024-02-08 16:27:23.000000 Excalibur2-2.2/src/
-drwxrwxrwx   0 lctfer    (1000) lctfer    (1000)        0 2024-02-08 16:29:02.805775 Excalibur2-2.2/src/Excalibur2/
--rwxrwxrwx   0 lctfer    (1000) lctfer    (1000)    14055 2024-02-08 16:04:32.000000 Excalibur2-2.2/src/Excalibur2/Excalibur2.py
--rwxrwxrwx   0 lctfer    (1000) lctfer    (1000)    14510 2024-02-08 16:13:41.000000 Excalibur2-2.2/src/Excalibur2/__init__.py
--rwxrwxrwx   0 lctfer    (1000) lctfer    (1000)     3194 2024-02-08 15:13:57.000000 Excalibur2-2.2/src/Excalibur2/__update__.py
-drwxrwxrwx   0 lctfer    (1000) lctfer    (1000)        0 2024-02-08 16:29:02.960322 Excalibur2-2.2/src/Excalibur2.egg-info/
--rwxrwxrwx   0 lctfer    (1000) lctfer    (1000)     1393 2024-02-08 16:29:02.000000 Excalibur2-2.2/src/Excalibur2.egg-info/PKG-INFO
--rwxrwxrwx   0 lctfer    (1000) lctfer    (1000)      269 2024-02-08 16:29:02.000000 Excalibur2-2.2/src/Excalibur2.egg-info/SOURCES.txt
--rwxrwxrwx   0 lctfer    (1000) lctfer    (1000)        1 2024-02-08 16:29:02.000000 Excalibur2-2.2/src/Excalibur2.egg-info/dependency_links.txt
--rwxrwxrwx   0 lctfer    (1000) lctfer    (1000)       11 2024-02-08 16:29:02.000000 Excalibur2-2.2/src/Excalibur2.egg-info/top_level.txt
+drwxrwxrwx   0 lctfer    (1000) lctfer    (1000)        0 2024-05-04 08:37:21.910179 excalibur2-2.3/
+-rwxrwxrwx   0 lctfer    (1000) lctfer    (1000)     1074 2024-02-07 08:25:01.000000 excalibur2-2.3/LICENSE
+-rwxrwxrwx   0 lctfer    (1000) lctfer    (1000)     1453 2024-05-04 08:37:21.903488 excalibur2-2.3/PKG-INFO
+-rwxrwxrwx   0 lctfer    (1000) lctfer    (1000)     1100 2024-02-09 14:59:03.000000 excalibur2-2.3/README.md
+-rwxrwxrwx   0 lctfer    (1000) lctfer    (1000)      531 2024-05-04 08:31:12.000000 excalibur2-2.3/pyproject.toml
+-rwxrwxrwx   0 lctfer    (1000) lctfer    (1000)       38 2024-05-04 08:37:21.910179 excalibur2-2.3/setup.cfg
+drwxrwxrwx   0 lctfer    (1000) lctfer    (1000)        0 2024-05-04 08:37:21.606259 excalibur2-2.3/src/
+drwxrwxrwx   0 lctfer    (1000) lctfer    (1000)        0 2024-05-04 08:37:21.739727 excalibur2-2.3/src/Excalibur2/
+-rwxrwxrwx   0 lctfer    (1000) lctfer    (1000)    14055 2024-02-08 16:04:32.000000 excalibur2-2.3/src/Excalibur2/Excalibur2.py
+-rwxrwxrwx   0 lctfer    (1000) lctfer    (1000)    14681 2024-05-01 04:50:05.000000 excalibur2-2.3/src/Excalibur2/__init__.py
+-rwxrwxrwx   0 lctfer    (1000) lctfer    (1000)     3194 2024-02-08 15:13:57.000000 excalibur2-2.3/src/Excalibur2/__update__.py
+drwxrwxrwx   0 lctfer    (1000) lctfer    (1000)        0 2024-05-04 08:37:21.885995 excalibur2-2.3/src/Excalibur2.egg-info/
+-rwxrwxrwx   0 lctfer    (1000) lctfer    (1000)     1453 2024-05-04 08:37:21.000000 excalibur2-2.3/src/Excalibur2.egg-info/PKG-INFO
+-rwxrwxrwx   0 lctfer    (1000) lctfer    (1000)      269 2024-05-04 08:37:21.000000 excalibur2-2.3/src/Excalibur2.egg-info/SOURCES.txt
+-rwxrwxrwx   0 lctfer    (1000) lctfer    (1000)        1 2024-05-04 08:37:21.000000 excalibur2-2.3/src/Excalibur2.egg-info/dependency_links.txt
+-rwxrwxrwx   0 lctfer    (1000) lctfer    (1000)       11 2024-05-04 08:37:21.000000 excalibur2-2.3/src/Excalibur2.egg-info/top_level.txt
```

### Comparing `Excalibur2-2.2/LICENSE` & `excalibur2-2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `Excalibur2-2.2/PKG-INFO` & `excalibur2-2.3/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Excalibur2
-Version: 2.2
+Version: 2.3
 Summary: A simple tool for pwn learners
 Author-email: lmarch2 <2524158037@qq.cm>
 Project-URL: Homepage, https://lmarch2.top/
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
@@ -23,14 +23,18 @@
 
 ## Install
 
 Install Excalibur2 by 
 
 > pip3 install Excalibur2
 
+check for updates
+
+>  python3 -m Excalibur2.\_\_update\_\_
+
 update package
 
 > pip3 install Excalibur2 --upgrade
 
 ## Help
 
 python built-in help
```

### Comparing `Excalibur2-2.2/README.md` & `excalibur2-2.3/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -10,14 +10,18 @@
 
 ## Install
 
 Install Excalibur2 by 
 
 > pip3 install Excalibur2
 
+check for updates
+
+>  python3 -m Excalibur2.\_\_update\_\_
+
 update package
 
 > pip3 install Excalibur2 --upgrade
 
 ## Help
 
 python built-in help
```

### Comparing `Excalibur2-2.2/src/Excalibur2/Excalibur2.py` & `excalibur2-2.3/src/Excalibur2/Excalibur2.py`

 * *Files identical despite different names*

### Comparing `Excalibur2-2.2/src/Excalibur2/__init__.py` & `excalibur2-2.3/src/Excalibur2/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -34,14 +34,23 @@
 
 #-----------------------------------------------------------------------------------------
 # Settings
 #-----------------------------------------------------------------------------------------
 
 
 
+def default(mode):
+	if mode == 'm':
+		setterminal("tmux","new-window")
+		contextset()
+	elif mode == 'h':
+		setterminal("tmux","splitw","-h")
+		contextset()
+
+
 # Set up debugging terminal (especially efficient on WSL2)
 # 如何在WSL2上使用tmux调试请看https://lmarch2.top/posts/19b7c9d1/
 def setterminal(termin='tmux',*args):
 	'''
 	------
 	Descriptions
 	set debug terminal
@@ -55,15 +64,15 @@
 	------
 	Returns
 	None
 	'''
 	if(len(args)<=0):
 		context.terminal = [termin, 'splitw', '-h']
 	else:
-		context.terminal = [termin,args]
+		context.terminal = [termin,*args]
 
 def contextset(ar = 64, de = 1):
 	'''
 	------
 	Descriptions
 	set your structure and debug mode
 	设置文件架构和调试模式
@@ -466,16 +475,17 @@
 	agu : flag of using libc (1) or libcsearcher (0) 
 	offset : the offset between leaked addr and base addr of func
 
 	------
 	Returns
 	binsh, system
 	'''
-	libc = globals()['libc']
+
 	if agu :
+		libc = globals()['libc']
 		base_addr = real_addr - libc.symbols[fun] - offset
 		setlibcbase(base_addr)
 		system = libc.symbols['system'] + base_addr
 		binsh = libc.search(b'/bin/sh').__next__() + base_addr
 		print("\n >>>>  The base addr is ",hex(base_addr),'\n')
 		print("\n >>>>  The bin_addr ",hex(binsh),'\n')		
 		print("\n >>>>  The system addr is ",hex(system),'\n')
```

### Comparing `Excalibur2-2.2/src/Excalibur2/__update__.py` & `excalibur2-2.3/src/Excalibur2/__update__.py`

 * *Files identical despite different names*

### Comparing `Excalibur2-2.2/src/Excalibur2.egg-info/PKG-INFO` & `excalibur2-2.3/src/Excalibur2.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Excalibur2
-Version: 2.2
+Version: 2.3
 Summary: A simple tool for pwn learners
 Author-email: lmarch2 <2524158037@qq.cm>
 Project-URL: Homepage, https://lmarch2.top/
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
@@ -23,14 +23,18 @@
 
 ## Install
 
 Install Excalibur2 by 
 
 > pip3 install Excalibur2
 
+check for updates
+
+>  python3 -m Excalibur2.\_\_update\_\_
+
 update package
 
 > pip3 install Excalibur2 --upgrade
 
 ## Help
 
 python built-in help
```

