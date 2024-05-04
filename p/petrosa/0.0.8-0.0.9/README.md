# Comparing `tmp/petrosa-0.0.8.tar.gz` & `tmp/petrosa-0.0.9.tar.gz`

## Comparing `petrosa-0.0.8.tar` & `petrosa-0.0.9.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0        9 2020-02-02 00:00:00.000000 petrosa-0.0.8/petrosa/converters/.gitignore
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 petrosa-0.0.8/petrosa/converters/__init__.py
--rw-r--r--   0        0        0     2322 2020-02-02 00:00:00.000000 petrosa-0.0.8/petrosa/converters/backtests.py
--rw-r--r--   0        0        0     1502 2020-02-02 00:00:00.000000 petrosa-0.0.8/petrosa/converters/data.pickle
--rw-r--r--   0        0        0      173 2020-02-02 00:00:00.000000 petrosa-0.0.8/petrosa/converters/myparams.pickle
--rw-r--r--   0        0        0        5 2020-02-02 00:00:00.000000 petrosa-0.0.8/petrosa/converters/params.pickle
--rw-r--r--   0        0        0 12175544 2020-02-02 00:00:00.000000 petrosa-0.0.8/petrosa/converters/stats.pickle
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 petrosa-0.0.8/petrosa/ta/__init__.py
--rw-r--r--   0        0        0    22023 2020-02-02 00:00:00.000000 petrosa-0.0.8/petrosa/ta/strategies.py
--rw-r--r--   0        0        0      822 2020-02-02 00:00:00.000000 petrosa-0.0.8/petrosa/ta/utils.py
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 petrosa-0.0.8/.gitignore
--rw-r--r--   0        0        0     1063 2020-02-02 00:00:00.000000 petrosa-0.0.8/LICENSE
--rw-r--r--   0        0        0      170 2020-02-02 00:00:00.000000 petrosa-0.0.8/README.md
--rw-r--r--   0        0        0      616 2020-02-02 00:00:00.000000 petrosa-0.0.8/pyproject.toml
--rw-r--r--   0        0        0      716 2020-02-02 00:00:00.000000 petrosa-0.0.8/PKG-INFO
+-rw-r--r--   0        0        0        9 2020-02-02 00:00:00.000000 petrosa-0.0.9/petrosa/converters/.gitignore
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 petrosa-0.0.9/petrosa/converters/__init__.py
+-rw-r--r--   0        0        0     2325 2020-02-02 00:00:00.000000 petrosa-0.0.9/petrosa/converters/backtests.py
+-rw-r--r--   0        0        0     1502 2020-02-02 00:00:00.000000 petrosa-0.0.9/petrosa/converters/data.pickle
+-rw-r--r--   0        0        0      173 2020-02-02 00:00:00.000000 petrosa-0.0.9/petrosa/converters/myparams.pickle
+-rw-r--r--   0        0        0        5 2020-02-02 00:00:00.000000 petrosa-0.0.9/petrosa/converters/params.pickle
+-rw-r--r--   0        0        0 12175544 2020-02-02 00:00:00.000000 petrosa-0.0.9/petrosa/converters/stats.pickle
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 petrosa-0.0.9/petrosa/ta/__init__.py
+-rw-r--r--   0        0        0    22023 2020-02-02 00:00:00.000000 petrosa-0.0.9/petrosa/ta/strategies.py
+-rw-r--r--   0        0        0      822 2020-02-02 00:00:00.000000 petrosa-0.0.9/petrosa/ta/utils.py
+-rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 petrosa-0.0.9/.gitignore
+-rw-r--r--   0        0        0     1063 2020-02-02 00:00:00.000000 petrosa-0.0.9/LICENSE
+-rw-r--r--   0        0        0      170 2020-02-02 00:00:00.000000 petrosa-0.0.9/README.md
+-rw-r--r--   0        0        0      616 2020-02-02 00:00:00.000000 petrosa-0.0.9/pyproject.toml
+-rw-r--r--   0        0        0      716 2020-02-02 00:00:00.000000 petrosa-0.0.9/PKG-INFO
```

### Comparing `petrosa-0.0.8/petrosa/converters/backtests.py` & `petrosa-0.0.9/petrosa/converters/backtests.py`

 * *Files 1% similar despite different names*

```diff
@@ -36,15 +36,15 @@
         elif isinstance(stats[key], pd.Timestamp):
             ret_res[key] = stats[key].to_pydatetime()
         else:
             ret_res[key] = stats[key]
 
     return ret_res
 
-def result_maker(bt_stats, params, bt_test_params, test_type):        
+def result_maker(bt_stats, bt_params, bt_test_params, test_type):        
     if '_trades' in bt_stats:
         del(bt_stats['_trades'])
     if '_strategy' in bt_stats:
         del(bt_stats['_strategy'])
     if '_equity_curve' in bt_stats:
         del(bt_stats['_equity_curve'])
```

### Comparing `petrosa-0.0.8/petrosa/converters/data.pickle` & `petrosa-0.0.9/petrosa/converters/data.pickle`

 * *Files identical despite different names*

### Comparing `petrosa-0.0.8/petrosa/converters/stats.pickle` & `petrosa-0.0.9/petrosa/converters/stats.pickle`

 * *Files identical despite different names*

### Comparing `petrosa-0.0.8/petrosa/ta/strategies.py` & `petrosa-0.0.9/petrosa/ta/strategies.py`

 * *Files identical despite different names*

### Comparing `petrosa-0.0.8/petrosa/ta/utils.py` & `petrosa-0.0.9/petrosa/ta/utils.py`

 * *Files identical despite different names*

### Comparing `petrosa-0.0.8/LICENSE` & `petrosa-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `petrosa-0.0.8/pyproject.toml` & `petrosa-0.0.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "petrosa"
-version = "0.0.8"
+version = "0.0.9"
 authors = [
   { name="@yurisa2", email="yuri@sa2.com.br" },
 ]
 description = "utilities for PETROSA"
 readme = "README.md"
 requires-python = ">=3.7"
 dependencies = ["pandas==2.0.0",
```

### Comparing `petrosa-0.0.8/PKG-INFO` & `petrosa-0.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: petrosa
-Version: 0.0.8
+Version: 0.0.9
 Summary: utilities for PETROSA
 Project-URL: Homepage, https://github.com/pypa/sampleproject
 Project-URL: Bug Tracker, https://github.com/pypa/sampleproject/issues
 Author-email: "@yurisa2" <yuri@sa2.com.br>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

