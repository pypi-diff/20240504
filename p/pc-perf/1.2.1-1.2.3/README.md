# Comparing `tmp/pc-perf-1.2.1.tar.gz` & `tmp/pc-perf-1.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pc-perf-1.2.1.tar", last modified: Sat May  4 05:19:24 2024, max compression
+gzip compressed data, was "pc-perf-1.2.3.tar", last modified: Sat May  4 06:33:02 2024, max compression
```

## Comparing `pc-perf-1.2.1.tar` & `pc-perf-1.2.3.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 root         (0) staff       (20)        0 2024-05-04 05:19:24.311389 pc-perf-1.2.1/
--rw-r--r--   0 root         (0) staff       (20)    35149 2024-04-28 09:32:22.000000 pc-perf-1.2.1/LICENSE
--rw-r--r--   0 root         (0) staff       (20)     1393 2024-05-04 05:19:24.311177 pc-perf-1.2.1/PKG-INFO
--rw-r--r--   0 root         (0) staff       (20)   377856 2024-04-28 09:32:22.000000 pc-perf-1.2.1/PresentMon.exe
--rw-r--r--   0 root         (0) staff       (20)     1238 2024-04-30 11:28:59.000000 pc-perf-1.2.1/README.md
-drwxr-xr-x   0 root         (0) staff       (20)        0 2024-05-04 05:19:24.308593 pc-perf-1.2.1/core/
--rw-r--r--   0 root         (0) staff       (20)     2509 2024-05-03 17:30:18.000000 pc-perf-1.2.1/core/monitor.py
--rw-r--r--   0 root         (0) staff       (20)     9861 2024-05-03 17:30:18.000000 pc-perf-1.2.1/core/pc_tools.py
--rw-r--r--   0 root         (0) staff       (20)     6903 2024-05-02 16:29:09.000000 pc-perf-1.2.1/dao.py
--rw-r--r--   0 root         (0) staff       (20)      648 2024-04-28 09:32:22.000000 pc-perf-1.2.1/log.py
-drwxr-xr-x   0 root         (0) staff       (20)        0 2024-05-04 05:19:24.310896 pc-perf-1.2.1/pc_perf.egg-info/
--rw-r--r--   0 root         (0) staff       (20)     1393 2024-05-04 05:19:24.000000 pc-perf-1.2.1/pc_perf.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) staff       (20)      349 2024-05-04 05:19:24.000000 pc-perf-1.2.1/pc_perf.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) staff       (20)        1 2024-05-04 05:19:24.000000 pc-perf-1.2.1/pc_perf.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) staff       (20)       41 2024-05-04 05:19:24.000000 pc-perf-1.2.1/pc_perf.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) staff       (20)      260 2024-05-04 05:19:24.000000 pc-perf-1.2.1/pc_perf.egg-info/requires.txt
--rw-r--r--   0 root         (0) staff       (20)       38 2024-05-04 05:19:24.000000 pc-perf-1.2.1/pc_perf.egg-info/top_level.txt
--rw-r--r--   0 root         (0) staff       (20)     4851 2024-05-04 03:07:45.000000 pc-perf-1.2.1/pc_perf.py
--rw-r--r--   0 root         (0) staff       (20)       38 2024-05-04 05:19:24.311433 pc-perf-1.2.1/setup.cfg
--rw-r--r--   0 root         (0) staff       (20)     2541 2024-05-04 05:19:19.000000 pc-perf-1.2.1/setup.py
--rw-r--r--   0 root         (0) staff       (20)     1625 2024-05-04 03:16:45.000000 pc-perf-1.2.1/task_handle.py
-drwxr-xr-x   0 root         (0) staff       (20)        0 2024-05-04 05:19:24.309814 pc-perf-1.2.1/test_result/
--rw-r--r--   0 root         (0) staff       (20)    30701 2024-05-02 16:25:39.000000 pc-perf-1.2.1/test_result/index.html
--rw-r--r--   0 root         (0) staff       (20)     3868 2024-05-04 03:09:43.000000 pc-perf-1.2.1/util.py
+drwxr-xr-x   0 root         (0) staff       (20)        0 2024-05-04 06:33:02.785429 pc-perf-1.2.3/
+-rw-r--r--   0 root         (0) staff       (20)    35149 2024-04-28 09:32:22.000000 pc-perf-1.2.3/LICENSE
+-rw-r--r--   0 root         (0) staff       (20)     1424 2024-05-04 06:33:02.785195 pc-perf-1.2.3/PKG-INFO
+-rw-r--r--   0 root         (0) staff       (20)   377856 2024-04-28 09:32:22.000000 pc-perf-1.2.3/PresentMon.exe
+-rw-r--r--   0 root         (0) staff       (20)     1343 2024-05-04 06:31:15.000000 pc-perf-1.2.3/README.md
+drwxr-xr-x   0 root         (0) staff       (20)        0 2024-05-04 06:33:02.782444 pc-perf-1.2.3/core/
+-rw-r--r--   0 root         (0) staff       (20)     2509 2024-05-04 06:31:15.000000 pc-perf-1.2.3/core/monitor.py
+-rw-r--r--   0 root         (0) staff       (20)     9873 2024-05-04 06:31:15.000000 pc-perf-1.2.3/core/pc_tools.py
+-rw-r--r--   0 root         (0) staff       (20)     6903 2024-05-04 06:31:15.000000 pc-perf-1.2.3/dao.py
+-rw-r--r--   0 root         (0) staff       (20)      648 2024-04-28 09:32:22.000000 pc-perf-1.2.3/log.py
+drwxr-xr-x   0 root         (0) staff       (20)        0 2024-05-04 06:33:02.784880 pc-perf-1.2.3/pc_perf.egg-info/
+-rw-r--r--   0 root         (0) staff       (20)     1424 2024-05-04 06:33:02.000000 pc-perf-1.2.3/pc_perf.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) staff       (20)      349 2024-05-04 06:33:02.000000 pc-perf-1.2.3/pc_perf.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) staff       (20)        1 2024-05-04 06:33:02.000000 pc-perf-1.2.3/pc_perf.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) staff       (20)       41 2024-05-04 06:33:02.000000 pc-perf-1.2.3/pc_perf.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) staff       (20)      276 2024-05-04 06:33:02.000000 pc-perf-1.2.3/pc_perf.egg-info/requires.txt
+-rw-r--r--   0 root         (0) staff       (20)       38 2024-05-04 06:33:02.000000 pc-perf-1.2.3/pc_perf.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) staff       (20)     4851 2024-05-04 06:31:15.000000 pc-perf-1.2.3/pc_perf.py
+-rw-r--r--   0 root         (0) staff       (20)       38 2024-05-04 06:33:02.785479 pc-perf-1.2.3/setup.cfg
+-rw-r--r--   0 root         (0) staff       (20)     2568 2024-05-04 06:33:01.000000 pc-perf-1.2.3/setup.py
+-rw-r--r--   0 root         (0) staff       (20)     1571 2024-05-04 06:31:15.000000 pc-perf-1.2.3/task_handle.py
+drwxr-xr-x   0 root         (0) staff       (20)        0 2024-05-04 06:33:02.783736 pc-perf-1.2.3/test_result/
+-rw-r--r--   0 root         (0) staff       (20)    30701 2024-05-02 16:25:39.000000 pc-perf-1.2.3/test_result/index.html
+-rw-r--r--   0 root         (0) staff       (20)     3868 2024-05-04 06:31:15.000000 pc-perf-1.2.3/util.py
```

### Comparing `pc-perf-1.2.1/LICENSE` & `pc-perf-1.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pc-perf-1.2.1/PKG-INFO` & `pc-perf-1.2.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pc-perf
-Version: 1.2.1
+Version: 1.2.3
 Summary: pc 进程性能测试平台，支持 windows / mac / linux 平台进程cpu、memory、fps（仅支持windows下OpenGL  DirectX 引擎应用）、gpu、thread_num、handle_num 等指标的实时监控和可视化展示
 Home-page: https://github.com/15525730080/pc_perf
 Author: 范博洲
 Author-email: 15525730080@163.com
 License: MIT
 Keywords: pc fps cpu memory gpu monitor
 Classifier: Development Status :: 3 - Alpha
@@ -28,7 +28,8 @@
 Requires-Dist: pynvml==11.5.0
 Requires-Dist: SQLAlchemy==2.0.29
 Requires-Dist: SQLAlchemy_serializer==1.4.12
 Requires-Dist: starlette==0.37.2
 Requires-Dist: uvicorn==0.29.0
 Requires-Dist: aiosqlite==0.20.0
 Requires-Dist: APScheduler==3.10.4
+Requires-Dist: greenlet==3.0.3
```

### Comparing `pc-perf-1.2.1/PresentMon.exe` & `pc-perf-1.2.3/PresentMon.exe`

 * *Files identical despite different names*

### Comparing `pc-perf-1.2.1/README.md` & `pc-perf-1.2.3/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 # pc_perf
 pc 进程性能测试平台，支持 windows / mac / linux 平台普通进程、window游戏GUI进程的
 cpu、memory、fps（仅支持windowsOpenGL  DirectX 引擎应用 unity u3d应用）、gpu、thread_num、handle_num 等指标的实时监控和可视化展示
 
 # 启动入口
-    方式0（推荐）：
-    直接下载二进制运行：https://github.com/15525730080/pc_perf/releases
+    方式0：
+    直接下载二进制运行：https://github.com/15525730080/pc_perf/releases, 二进制文件打包需要针对各个平台有一定成本所以更新不及时。推荐方式2。
     
     方式1：
     git clone https://github.com/15525730080/pc_perf.git
     pip install -r requirements.txt
     #需要使用管理员权限启动才可以获取到windows fps ！！！
     python pc_perf.py 
     
-    方式2：
+    方式2（推荐）：
     #需要使用管理员权限启动才可以获取到windows fps ！！！
-    pip install pc-perf
+    pip install -U pc-perf
     python -m pc_perf  
 
     
 
 # 创建任务
 ![image](https://github.com/15525730080/pc_perf/assets/153100629/91995e83-6fc6-4350-84d1-24704f1bccce)
```

### Comparing `pc-perf-1.2.1/core/monitor.py` & `pc-perf-1.2.3/core/monitor.py`

 * *Files identical despite different names*

### Comparing `pc-perf-1.2.1/core/pc_tools.py` & `pc-perf-1.2.3/core/pc_tools.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 from log import log
 from core.monitor import Monitor
 
 SUPPORT_GPU = True
 try:
     pynvml.nvmlInit()
 except:
-    traceback.print_exc()
+    log.error(traceback.format_exc())
     log.info("本设备gpu获取不适配")
     SUPPORT_GPU = False
 from PIL import ImageGrab
 
 
 def print_json(msg):
     log.info(json.dumps(msg))
```

### Comparing `pc-perf-1.2.1/dao.py` & `pc-perf-1.2.3/dao.py`

 * *Files identical despite different names*

### Comparing `pc-perf-1.2.1/log.py` & `pc-perf-1.2.3/log.py`

 * *Files identical despite different names*

### Comparing `pc-perf-1.2.1/pc_perf.egg-info/PKG-INFO` & `pc-perf-1.2.3/pc_perf.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pc-perf
-Version: 1.2.1
+Version: 1.2.3
 Summary: pc 进程性能测试平台，支持 windows / mac / linux 平台进程cpu、memory、fps（仅支持windows下OpenGL  DirectX 引擎应用）、gpu、thread_num、handle_num 等指标的实时监控和可视化展示
 Home-page: https://github.com/15525730080/pc_perf
 Author: 范博洲
 Author-email: 15525730080@163.com
 License: MIT
 Keywords: pc fps cpu memory gpu monitor
 Classifier: Development Status :: 3 - Alpha
@@ -28,7 +28,8 @@
 Requires-Dist: pynvml==11.5.0
 Requires-Dist: SQLAlchemy==2.0.29
 Requires-Dist: SQLAlchemy_serializer==1.4.12
 Requires-Dist: starlette==0.37.2
 Requires-Dist: uvicorn==0.29.0
 Requires-Dist: aiosqlite==0.20.0
 Requires-Dist: APScheduler==3.10.4
+Requires-Dist: greenlet==3.0.3
```

### Comparing `pc-perf-1.2.1/pc_perf.py` & `pc-perf-1.2.3/pc_perf.py`

 * *Files identical despite different names*

### Comparing `pc-perf-1.2.1/setup.py` & `pc-perf-1.2.3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from setuptools import setup, find_packages
 
 setup(
     # 包的名称，通常与包的目录名称相同
     name='pc-perf',
 
     # 版本号，遵循语义化版本控制规则
-    version='1.2.1',
+    version='1.2.3',
 
     # 项目简短描述
     description='pc 进程性能测试平台，支持 windows / mac / linux 平台进程cpu、memory、fps（仅支持windows下OpenGL  DirectX 引擎应用）、gpu、thread_num、handle_num 等指标的实时监控和可视化展示',
 
     # 项目的URL，通常是项目主页或源代码仓库
     url='https://github.com/15525730080/pc_perf',
 
@@ -37,15 +37,16 @@
         "PyGetWindow==0.0.9",
         "pynvml==11.5.0",
         "SQLAlchemy==2.0.29",
         "SQLAlchemy_serializer==1.4.12",
         "starlette==0.37.2",
         "uvicorn==0.29.0",
         "aiosqlite==0.20.0",
-        "APScheduler==3.10.4"
+        "APScheduler==3.10.4",
+        "greenlet==3.0.3"
     ],
 
     # 从包中自动寻找所有的子包和子模块
     py_modules=['dao', 'log', 'task_handle', 'util', 'pc_perf', 'core'],
     packages=['core'],
     
     # 包含数据文件，比如配置文件
```

### Comparing `pc-perf-1.2.1/task_handle.py` & `pc-perf-1.2.3/task_handle.py`

 * *Files 11% similar despite different names*

```diff
@@ -37,19 +37,17 @@
     @staticmethod
     def stop_handle(monitor_pid):
         logger.info("Stopping task handle and subprocesses... {0}".format(monitor_pid))
         # kill the pc_perf subprocess
         current_process = psutil.Process(monitor_pid)
         try:
             for child in current_process.children(recursive=True):
-                child.kill()
-                child.wait(0.2)
+                os.kill(child.pid, 9)
         except Exception as e:
             logger.error(e)
         finally:
             try:
-                current_process.kill()
-                current_process.wait(1)
+                os.kill(current_process.pid, 9)
             except:
                 logger.error(traceback.format_exc())
```

### Comparing `pc-perf-1.2.1/test_result/index.html` & `pc-perf-1.2.3/test_result/index.html`

 * *Files identical despite different names*

### Comparing `pc-perf-1.2.1/util.py` & `pc-perf-1.2.3/util.py`

 * *Files identical despite different names*

