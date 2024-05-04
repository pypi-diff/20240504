# Comparing `tmp/mptradelib-0.3.4.tar.gz` & `tmp/mptradelib-0.3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mptradelib-0.3.4.tar", max compression
+gzip compressed data, was "mptradelib-0.3.5.tar", max compression
```

## Comparing `mptradelib-0.3.4.tar` & `mptradelib-0.3.5.tar`

### file list

```diff
@@ -1,19 +1,19 @@
--rw-r--r--   0        0        0     3137 2024-05-03 13:20:41.913077 mptradelib-0.3.4/README.md
--rw-r--r--   0        0        0        0 2024-04-30 08:23:49.256174 mptradelib-0.3.4/mptradelib/__init__.py
--rw-r--r--   0        0        0     4572 2024-05-03 09:17:03.492484 mptradelib-0.3.4/mptradelib/backtest.py
--rw-r--r--   0        0        0        0 2024-04-30 08:23:49.266753 mptradelib-0.3.4/mptradelib/broker/__init__.py
--rw-r--r--   0        0        0     5728 2024-05-02 08:04:56.402627 mptradelib-0.3.4/mptradelib/broker/broker.py
--rw-r--r--   0        0        0     5818 2024-04-30 11:44:33.569478 mptradelib-0.3.4/mptradelib/broker/session.py
--rw-r--r--   0        0        0     2683 2024-05-01 14:36:23.728530 mptradelib-0.3.4/mptradelib/broker/ticker.py
--rw-r--r--   0        0        0        0 2024-05-03 11:19:20.268249 mptradelib-0.3.4/mptradelib/cli/__init__.py
--rw-r--r--   0        0        0     2330 2024-05-03 13:17:36.227537 mptradelib-0.3.4/mptradelib/cli/new.py
--rw-r--r--   0        0        0     4054 2024-05-03 03:52:00.848935 mptradelib-0.3.4/mptradelib/feed.py
--rw-r--r--   0        0        0     1864 2024-05-03 09:17:03.492902 mptradelib-0.3.4/mptradelib/livetrade.py
--rw-r--r--   0        0        0    34066 2024-05-01 10:05:54.173058 mptradelib-0.3.4/mptradelib/shoonya.py
--rw-r--r--   0        0        0     1097 2024-05-03 13:03:10.480806 mptradelib-0.3.4/mptradelib/templates/strategy/__init__.jinja
--rw-r--r--   0        0        0     1187 2024-05-03 13:10:47.542853 mptradelib-0.3.4/mptradelib/templates/strategy/backtest.jinja
--rw-r--r--   0        0        0      614 2024-05-03 12:29:43.201283 mptradelib-0.3.4/mptradelib/templates/strategy/livetrade.jinja
--rw-r--r--   0        0        0     1313 2024-04-30 08:23:49.272908 mptradelib-0.3.4/mptradelib/test_renko.py
--rw-r--r--   0        0        0      651 2024-04-30 08:25:03.006597 mptradelib-0.3.4/mptradelib/utils.py
--rw-r--r--   0        0        0      829 2024-05-03 13:07:16.260293 mptradelib-0.3.4/pyproject.toml
--rw-r--r--   0        0        0     4003 1970-01-01 00:00:00.000000 mptradelib-0.3.4/PKG-INFO
+-rw-r--r--   0        0        0     3137 2024-05-03 13:20:41.913077 mptradelib-0.3.5/README.md
+-rw-r--r--   0        0        0        0 2024-04-30 08:23:49.256174 mptradelib-0.3.5/mptradelib/__init__.py
+-rw-r--r--   0        0        0     4572 2024-05-03 09:17:03.492484 mptradelib-0.3.5/mptradelib/backtest.py
+-rw-r--r--   0        0        0        0 2024-04-30 08:23:49.266753 mptradelib-0.3.5/mptradelib/broker/__init__.py
+-rw-r--r--   0        0        0     5728 2024-05-02 08:04:56.402627 mptradelib-0.3.5/mptradelib/broker/broker.py
+-rw-r--r--   0        0        0     5818 2024-04-30 11:44:33.569478 mptradelib-0.3.5/mptradelib/broker/session.py
+-rw-r--r--   0        0        0     2683 2024-05-01 14:36:23.728530 mptradelib-0.3.5/mptradelib/broker/ticker.py
+-rw-r--r--   0        0        0        0 2024-05-03 11:19:20.268249 mptradelib-0.3.5/mptradelib/cli/__init__.py
+-rw-r--r--   0        0        0     2319 2024-05-04 08:59:40.290825 mptradelib-0.3.5/mptradelib/cli/new.py
+-rw-r--r--   0        0        0     4054 2024-05-03 03:52:00.848935 mptradelib-0.3.5/mptradelib/feed.py
+-rw-r--r--   0        0        0     1864 2024-05-03 09:17:03.492902 mptradelib-0.3.5/mptradelib/livetrade.py
+-rw-r--r--   0        0        0    34066 2024-05-01 10:05:54.173058 mptradelib-0.3.5/mptradelib/shoonya.py
+-rw-r--r--   0        0        0     1097 2024-05-03 13:03:10.480806 mptradelib-0.3.5/mptradelib/templates/strategy/__init__.jinja
+-rw-r--r--   0        0        0     1187 2024-05-03 13:10:47.542853 mptradelib-0.3.5/mptradelib/templates/strategy/backtest.jinja
+-rw-r--r--   0        0        0      614 2024-05-03 12:29:43.201283 mptradelib-0.3.5/mptradelib/templates/strategy/livetrade.jinja
+-rw-r--r--   0        0        0     1313 2024-04-30 08:23:49.272908 mptradelib-0.3.5/mptradelib/test_renko.py
+-rw-r--r--   0        0        0      651 2024-04-30 08:25:03.006597 mptradelib-0.3.5/mptradelib/utils.py
+-rw-r--r--   0        0        0      829 2024-05-04 08:59:52.570729 mptradelib-0.3.5/pyproject.toml
+-rw-r--r--   0        0        0     4003 1970-01-01 00:00:00.000000 mptradelib-0.3.5/PKG-INFO
```

### Comparing `mptradelib-0.3.4/README.md` & `mptradelib-0.3.5/README.md`

 * *Files identical despite different names*

### Comparing `mptradelib-0.3.4/mptradelib/backtest.py` & `mptradelib-0.3.5/mptradelib/backtest.py`

 * *Files identical despite different names*

### Comparing `mptradelib-0.3.4/mptradelib/broker/broker.py` & `mptradelib-0.3.5/mptradelib/broker/broker.py`

 * *Files identical despite different names*

### Comparing `mptradelib-0.3.4/mptradelib/broker/session.py` & `mptradelib-0.3.5/mptradelib/broker/session.py`

 * *Files identical despite different names*

### Comparing `mptradelib-0.3.4/mptradelib/broker/ticker.py` & `mptradelib-0.3.5/mptradelib/broker/ticker.py`

 * *Files identical despite different names*

### Comparing `mptradelib-0.3.4/mptradelib/cli/new.py` & `mptradelib-0.3.5/mptradelib/cli/new.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 logging.addLevelName(logging.INFO, 'info')
 
 libpath = os.path.abspath(os.path.join(sys.executable, f"../../lib/python{'.'.join(sys.version.split('.')[:2])}/site-packages/mptradelib"))
 if not os.path.exists(libpath):
     libpath = os.path.abspath('.')
 
 env = Environment(
-    loader=FileSystemLoader(os.path.join(libpath, "mptradelib/templates/strategy/")),
+    loader=FileSystemLoader(os.path.join(libpath, "templates/strategy/")),
     extensions=['jinja2_strcase.StrcaseExtension']
 )
 
 @click.group
 def commands():
     pass
```

### Comparing `mptradelib-0.3.4/mptradelib/feed.py` & `mptradelib-0.3.5/mptradelib/feed.py`

 * *Files identical despite different names*

### Comparing `mptradelib-0.3.4/mptradelib/livetrade.py` & `mptradelib-0.3.5/mptradelib/livetrade.py`

 * *Files identical despite different names*

### Comparing `mptradelib-0.3.4/mptradelib/shoonya.py` & `mptradelib-0.3.5/mptradelib/shoonya.py`

 * *Files identical despite different names*

### Comparing `mptradelib-0.3.4/mptradelib/templates/strategy/__init__.jinja` & `mptradelib-0.3.5/mptradelib/templates/strategy/__init__.jinja`

 * *Files identical despite different names*

### Comparing `mptradelib-0.3.4/mptradelib/templates/strategy/backtest.jinja` & `mptradelib-0.3.5/mptradelib/templates/strategy/backtest.jinja`

 * *Files identical despite different names*

### Comparing `mptradelib-0.3.4/mptradelib/templates/strategy/livetrade.jinja` & `mptradelib-0.3.5/mptradelib/templates/strategy/livetrade.jinja`

 * *Files identical despite different names*

### Comparing `mptradelib-0.3.4/mptradelib/test_renko.py` & `mptradelib-0.3.5/mptradelib/test_renko.py`

 * *Files identical despite different names*

### Comparing `mptradelib-0.3.4/mptradelib/utils.py` & `mptradelib-0.3.5/mptradelib/utils.py`

 * *Files identical despite different names*

### Comparing `mptradelib-0.3.4/pyproject.toml` & `mptradelib-0.3.5/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "mptradelib"
-version = "0.3.4"
+version = "0.3.5"
 description = ""
 authors = ["Abhilash Nanda <wishabhilash@gmail.com>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.10"
 pydantic = "2.7.1"
```

### Comparing `mptradelib-0.3.4/PKG-INFO` & `mptradelib-0.3.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mptradelib
-Version: 0.3.4
+Version: 0.3.5
 Summary: 
 Author: Abhilash Nanda
 Author-email: wishabhilash@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

