# Comparing `tmp/pyassorted-0.8.0.tar.gz` & `tmp/pyassorted-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyassorted-0.8.0.tar", max compression
+gzip compressed data, was "pyassorted-0.9.0.tar", max compression
```

## Comparing `pyassorted-0.8.0.tar` & `pyassorted-0.9.0.tar`

### file list

```diff
@@ -1,39 +1,42 @@
--rw-r--r--   0        0        0     1066 2023-08-06 14:02:38.505835 pyassorted-0.8.0/LICENSE
--rw-r--r--   0        0        0     7120 2023-08-06 14:02:38.505995 pyassorted-0.8.0/README.md
--rw-r--r--   0        0        0       52 2023-08-06 14:02:38.507714 pyassorted-0.8.0/pyassorted/__init__.py
--rw-r--r--   0        0        0      151 2024-02-28 14:11:40.501280 pyassorted-0.8.0/pyassorted/asyncio/__init__.py
--rw-r--r--   0        0        0     5410 2024-02-29 17:24:01.782089 pyassorted-0.8.0/pyassorted/asyncio/executor.py
--rw-r--r--   0        0        0     2943 2023-08-06 14:02:38.507966 pyassorted-0.8.0/pyassorted/asyncio/io.py
--rw-r--r--   0        0        0     1017 2023-08-06 14:02:38.508029 pyassorted-0.8.0/pyassorted/asyncio/utils.py
--rw-r--r--   0        0        0       60 2023-08-06 14:02:38.508113 pyassorted-0.8.0/pyassorted/cache/__init__.py
--rw-r--r--   0        0        0     8108 2023-08-06 14:02:38.508198 pyassorted-0.8.0/pyassorted/cache/cache.py
--rw-r--r--   0        0        0        0 2023-08-06 14:02:38.508271 pyassorted-0.8.0/pyassorted/collections/__init__.py
--rw-r--r--   0        0        0     4047 2023-08-06 14:02:38.508371 pyassorted-0.8.0/pyassorted/collections/sqlitedict.py
--rw-r--r--   0        0        0      147 2023-08-06 14:02:38.508459 pyassorted-0.8.0/pyassorted/datetime/__init__.py
--rw-r--r--   0        0        0     2121 2023-08-07 14:17:33.360824 pyassorted-0.8.0/pyassorted/datetime/datetime.py
--rw-r--r--   0        0        0     2013 2023-08-06 14:02:38.508580 pyassorted-0.8.0/pyassorted/datetime/timer.py
--rw-r--r--   0        0        0        0 2023-08-06 14:02:38.508638 pyassorted-0.8.0/pyassorted/encrypt/__init__.py
--rw-r--r--   0        0        0     2257 2023-08-06 14:02:38.508731 pyassorted-0.8.0/pyassorted/encrypt/io.py
--rw-r--r--   0        0        0      846 2023-08-28 14:00:39.995607 pyassorted-0.8.0/pyassorted/fs/__init__.py
--rw-r--r--   0        0        0       54 2023-08-06 14:02:38.508820 pyassorted-0.8.0/pyassorted/hash/__init__.py
--rw-r--r--   0        0        0      403 2023-08-06 14:02:38.508878 pyassorted-0.8.0/pyassorted/hash/_string.py
--rw-r--r--   0        0        0     2602 2023-08-06 14:02:38.508980 pyassorted-0.8.0/pyassorted/io/__init__.py
--rw-r--r--   0        0        0     2364 2023-08-06 14:02:38.509047 pyassorted-0.8.0/pyassorted/io/watch.py
--rw-r--r--   0        0        0       55 2023-08-06 14:02:38.509130 pyassorted-0.8.0/pyassorted/lock/__init__.py
--rw-r--r--   0        0        0     4191 2023-08-06 14:02:38.509215 pyassorted-0.8.0/pyassorted/lock/filelock.py
--rw-r--r--   0        0        0     1313 2024-02-27 14:30:18.173381 pyassorted-0.8.0/pyassorted/lock/key_lock.py
--rw-r--r--   0        0        0        0 2023-09-03 13:09:26.646892 pyassorted-0.8.0/pyassorted/logger/__init__.py
--rw-r--r--   0        0        0     1532 2023-09-03 13:09:26.647225 pyassorted-0.8.0/pyassorted/logger/formatter.py
--rw-r--r--   0        0        0        0 2023-09-03 13:09:26.647298 pyassorted-0.8.0/pyassorted/numerals/__init__.py
--rw-r--r--   0        0        0      114 2023-09-03 13:09:26.647545 pyassorted-0.8.0/pyassorted/numerals/rand.py
--rw-r--r--   0        0        0        0 2023-08-06 14:02:38.509271 pyassorted-0.8.0/pyassorted/standard/__init__.py
--rw-r--r--   0        0        0     2788 2023-08-06 14:02:38.509356 pyassorted-0.8.0/pyassorted/standard/language_code.py
--rw-r--r--   0        0        0      129 2023-08-06 14:02:38.509447 pyassorted-0.8.0/pyassorted/string/__init__.py
--rw-r--r--   0        0        0      841 2023-08-06 14:02:38.509509 pyassorted-0.8.0/pyassorted/string/rand.py
--rw-r--r--   0        0        0     1928 2024-02-27 14:30:18.173809 pyassorted-0.8.0/pyassorted/string/replace.py
--rw-r--r--   0        0        0     1737 2023-08-06 14:02:38.509668 pyassorted-0.8.0/pyassorted/string/validator.py
--rw-r--r--   0        0        0       18 2024-02-29 17:31:43.030356 pyassorted-0.8.0/pyassorted/version.py
--rw-r--r--   0        0        0        0 2024-02-27 14:30:18.173931 pyassorted-0.8.0/pyassorted/warn/__init__.py
--rw-r--r--   0        0        0      605 2024-02-27 14:30:18.174229 pyassorted-0.8.0/pyassorted/warn/base.py
--rw-r--r--   0        0        0      684 2024-02-29 17:31:27.656488 pyassorted-0.8.0/pyproject.toml
--rw-r--r--   0        0        0     7858 1970-01-01 00:00:00.000000 pyassorted-0.8.0/PKG-INFO
+-rw-r--r--   0        0        0     1066 2023-08-06 14:02:38.505835 pyassorted-0.9.0/LICENSE
+-rw-r--r--   0        0        0     7120 2023-08-06 14:02:38.505995 pyassorted-0.9.0/README.md
+-rw-r--r--   0        0        0       52 2023-08-06 14:02:38.507714 pyassorted-0.9.0/pyassorted/__init__.py
+-rw-r--r--   0        0        0      151 2024-02-28 14:11:40.501280 pyassorted-0.9.0/pyassorted/asyncio/__init__.py
+-rw-r--r--   0        0        0     5410 2024-02-29 17:24:01.782089 pyassorted-0.9.0/pyassorted/asyncio/executor.py
+-rw-r--r--   0        0        0     2943 2023-08-06 14:02:38.507966 pyassorted-0.9.0/pyassorted/asyncio/io.py
+-rw-r--r--   0        0        0     1017 2023-08-06 14:02:38.508029 pyassorted-0.9.0/pyassorted/asyncio/utils.py
+-rw-r--r--   0        0        0       60 2023-08-06 14:02:38.508113 pyassorted-0.9.0/pyassorted/cache/__init__.py
+-rw-r--r--   0        0        0     8108 2023-08-06 14:02:38.508198 pyassorted-0.9.0/pyassorted/cache/cache.py
+-rw-r--r--   0        0        0        0 2023-08-06 14:02:38.508271 pyassorted-0.9.0/pyassorted/collections/__init__.py
+-rw-r--r--   0        0        0     4047 2023-08-06 14:02:38.508371 pyassorted-0.9.0/pyassorted/collections/sqlitedict.py
+-rw-r--r--   0        0        0      147 2023-08-06 14:02:38.508459 pyassorted-0.9.0/pyassorted/datetime/__init__.py
+-rw-r--r--   0        0        0     2121 2023-08-07 14:17:33.360824 pyassorted-0.9.0/pyassorted/datetime/datetime.py
+-rw-r--r--   0        0        0     2013 2023-08-06 14:02:38.508580 pyassorted-0.9.0/pyassorted/datetime/timer.py
+-rw-r--r--   0        0        0        0 2023-08-06 14:02:38.508638 pyassorted-0.9.0/pyassorted/encrypt/__init__.py
+-rw-r--r--   0        0        0     2257 2023-08-06 14:02:38.508731 pyassorted-0.9.0/pyassorted/encrypt/io.py
+-rw-r--r--   0        0        0      846 2023-08-28 14:00:39.995607 pyassorted-0.9.0/pyassorted/fs/__init__.py
+-rw-r--r--   0        0        0       54 2023-08-06 14:02:38.508820 pyassorted-0.9.0/pyassorted/hash/__init__.py
+-rw-r--r--   0        0        0      403 2023-08-06 14:02:38.508878 pyassorted-0.9.0/pyassorted/hash/_string.py
+-rw-r--r--   0        0        0     2602 2023-08-06 14:02:38.508980 pyassorted-0.9.0/pyassorted/io/__init__.py
+-rw-r--r--   0        0        0     2364 2023-08-06 14:02:38.509047 pyassorted-0.9.0/pyassorted/io/watch.py
+-rw-r--r--   0        0        0       55 2023-08-06 14:02:38.509130 pyassorted-0.9.0/pyassorted/lock/__init__.py
+-rw-r--r--   0        0        0     4191 2023-08-06 14:02:38.509215 pyassorted-0.9.0/pyassorted/lock/filelock.py
+-rw-r--r--   0        0        0     1313 2024-02-27 14:30:18.173381 pyassorted-0.9.0/pyassorted/lock/key_lock.py
+-rw-r--r--   0        0        0        0 2023-09-03 13:09:26.646892 pyassorted-0.9.0/pyassorted/logger/__init__.py
+-rw-r--r--   0        0        0     1532 2023-09-03 13:09:26.647225 pyassorted-0.9.0/pyassorted/logger/formatter.py
+-rw-r--r--   0        0        0        0 2023-09-03 13:09:26.647298 pyassorted-0.9.0/pyassorted/numerals/__init__.py
+-rw-r--r--   0        0        0      114 2023-09-03 13:09:26.647545 pyassorted-0.9.0/pyassorted/numerals/rand.py
+-rw-r--r--   0        0        0        0 2023-08-06 14:02:38.509271 pyassorted-0.9.0/pyassorted/standard/__init__.py
+-rw-r--r--   0        0        0     2788 2023-08-06 14:02:38.509356 pyassorted-0.9.0/pyassorted/standard/language_code.py
+-rw-r--r--   0        0        0      315 2024-05-04 07:56:11.501639 pyassorted-0.9.0/pyassorted/string/__init__.py
+-rw-r--r--   0        0        0     1657 2024-05-04 07:56:11.501749 pyassorted-0.9.0/pyassorted/string/find.py
+-rw-r--r--   0        0        0      841 2023-08-06 14:02:38.509509 pyassorted-0.9.0/pyassorted/string/rand.py
+-rw-r--r--   0        0        0     2726 2024-05-04 07:56:11.502067 pyassorted-0.9.0/pyassorted/string/replace.py
+-rw-r--r--   0        0        0     1737 2023-08-06 14:02:38.509668 pyassorted-0.9.0/pyassorted/string/validator.py
+-rw-r--r--   0        0        0       96 2024-05-04 07:14:44.997622 pyassorted-0.9.0/pyassorted/types/__init__.py
+-rw-r--r--   0        0        0      429 2024-05-04 07:14:44.998047 pyassorted-0.9.0/pyassorted/types/_inspect.py
+-rw-r--r--   0        0        0       18 2024-05-04 07:56:56.380135 pyassorted-0.9.0/pyassorted/version.py
+-rw-r--r--   0        0        0        0 2024-02-27 14:30:18.173931 pyassorted-0.9.0/pyassorted/warn/__init__.py
+-rw-r--r--   0        0        0      605 2024-02-27 14:30:18.174229 pyassorted-0.9.0/pyassorted/warn/base.py
+-rw-r--r--   0        0        0      685 2024-05-04 07:56:49.808448 pyassorted-0.9.0/pyproject.toml
+-rw-r--r--   0        0        0     7709 1970-01-01 00:00:00.000000 pyassorted-0.9.0/PKG-INFO
```

### Comparing `pyassorted-0.8.0/LICENSE` & `pyassorted-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pyassorted-0.8.0/README.md` & `pyassorted-0.9.0/README.md`

 * *Files identical despite different names*

### Comparing `pyassorted-0.8.0/pyassorted/asyncio/executor.py` & `pyassorted-0.9.0/pyassorted/asyncio/executor.py`

 * *Files identical despite different names*

### Comparing `pyassorted-0.8.0/pyassorted/asyncio/io.py` & `pyassorted-0.9.0/pyassorted/asyncio/io.py`

 * *Files identical despite different names*

### Comparing `pyassorted-0.8.0/pyassorted/asyncio/utils.py` & `pyassorted-0.9.0/pyassorted/asyncio/utils.py`

 * *Files identical despite different names*

### Comparing `pyassorted-0.8.0/pyassorted/cache/cache.py` & `pyassorted-0.9.0/pyassorted/cache/cache.py`

 * *Files identical despite different names*

### Comparing `pyassorted-0.8.0/pyassorted/collections/sqlitedict.py` & `pyassorted-0.9.0/pyassorted/collections/sqlitedict.py`

 * *Files identical despite different names*

### Comparing `pyassorted-0.8.0/pyassorted/datetime/datetime.py` & `pyassorted-0.9.0/pyassorted/datetime/datetime.py`

 * *Files identical despite different names*

### Comparing `pyassorted-0.8.0/pyassorted/datetime/timer.py` & `pyassorted-0.9.0/pyassorted/datetime/timer.py`

 * *Files identical despite different names*

### Comparing `pyassorted-0.8.0/pyassorted/encrypt/io.py` & `pyassorted-0.9.0/pyassorted/encrypt/io.py`

 * *Files identical despite different names*

### Comparing `pyassorted-0.8.0/pyassorted/fs/__init__.py` & `pyassorted-0.9.0/pyassorted/fs/__init__.py`

 * *Files identical despite different names*

### Comparing `pyassorted-0.8.0/pyassorted/io/__init__.py` & `pyassorted-0.9.0/pyassorted/io/__init__.py`

 * *Files identical despite different names*

### Comparing `pyassorted-0.8.0/pyassorted/io/watch.py` & `pyassorted-0.9.0/pyassorted/io/watch.py`

 * *Files identical despite different names*

### Comparing `pyassorted-0.8.0/pyassorted/lock/filelock.py` & `pyassorted-0.9.0/pyassorted/lock/filelock.py`

 * *Files identical despite different names*

### Comparing `pyassorted-0.8.0/pyassorted/lock/key_lock.py` & `pyassorted-0.9.0/pyassorted/lock/key_lock.py`

 * *Files identical despite different names*

### Comparing `pyassorted-0.8.0/pyassorted/logger/formatter.py` & `pyassorted-0.9.0/pyassorted/logger/formatter.py`

 * *Files identical despite different names*

### Comparing `pyassorted-0.8.0/pyassorted/standard/language_code.py` & `pyassorted-0.9.0/pyassorted/standard/language_code.py`

 * *Files identical despite different names*

### Comparing `pyassorted-0.8.0/pyassorted/string/rand.py` & `pyassorted-0.9.0/pyassorted/string/rand.py`

 * *Files identical despite different names*

### Comparing `pyassorted-0.8.0/pyassorted/string/replace.py` & `pyassorted-0.9.0/pyassorted/string/replace.py`

 * *Files 12% similar despite different names*

```diff
@@ -7,57 +7,85 @@
     NoBracket = 0
     Parenthesis = 1
     CurlyBrackets = 2
     SquareBrackets = 3
 
 
 def multiple_replace(
-    d: Dict[Text, Text], text: Text, wraped_by: Bracket = Bracket.NoBracket
+    d: Dict[Text, Text], text: Text, wrapped_by: Bracket = Bracket.NoBracket
 ) -> Text:
     """Replace 'd' keys with 'd' values in 'text' string.
 
     Parameters
     ----------
     d : Dict[Text, Text]
         Dictionary with keys to be replaced by values.
     text : Text
         Text to be replaced.
-    wraped_by : Bracket, optional
+    wrapped_by : Bracket, optional
         If specified, the keys will be wrapped by the specified bracket type.
         If not specified, the keys will be replaced without any wrapping.
         The default is Bracket.NoBracket.
 
     Returns
     -------
     Text
         Text with replaced keys.
 
     Raises
     ------
     ValueError
-        If 'wraped_by' is not a valid Bracket type.
+        If 'wrapped_by' is not a valid Bracket type.
 
     Examples
     --------
     >>> d = {"var1": "Hello", "var2": "World"}
     >>> text = "var1 var2"
     >>> multiple_replace(d, text)
     'Hello World'
     """
 
-    if wraped_by is Bracket.NoBracket:
+    if wrapped_by is Bracket.NoBracket:
         regex = re.compile(r"%s" % "|".join(map(re.escape, d.keys())))
-    elif wraped_by is Bracket.Parenthesis:
+    elif wrapped_by is Bracket.Parenthesis:
         regex = re.compile(r"\(\s*(%s)\s*\)" % "|".join(map(re.escape, d.keys())))
-    elif wraped_by is Bracket.SquareBrackets:
+    elif wrapped_by is Bracket.SquareBrackets:
         regex = re.compile(r"\[\s*(%s)\s*\]" % "|".join(map(re.escape, d.keys())))
-    elif wraped_by is Bracket.CurlyBrackets:
+    elif wrapped_by is Bracket.CurlyBrackets:
         regex = re.compile(r"{\s*(%s)\s*}" % "|".join(map(re.escape, d.keys())))
     else:
-        raise ValueError(f"Invalid Bracket type: {wraped_by}")
+        raise ValueError(f"Invalid Bracket type: {wrapped_by}")
 
-    if wraped_by is Bracket.Parenthesis:
+    if wrapped_by is Bracket.Parenthesis:
         return regex.sub(lambda mo: d[mo.group().strip("() \t\n\r")], text)
-    if wraped_by is Bracket.SquareBrackets:
+    if wrapped_by is Bracket.SquareBrackets:
         return regex.sub(lambda mo: d[mo.group().strip("[] \t\n\r")], text)
     else:
         return regex.sub(lambda mo: d[mo.group().strip("{} \t\n\r")], text)
+
+
+def limit_consecutive_newlines(text: Text, max_newlines: int = 2) -> Text:
+    """Limit consecutive newlines in a string.
+
+    Parameters
+    ----------
+    text : Text
+        Input text with newlines.
+    max_newlines : int, optional
+        Maximum number of consecutive newlines allowed. The default is 2.
+
+    Returns
+    -------
+    Text
+        Text with limited consecutive newlines.
+
+    Examples
+    --------
+    >>> text = "Hello\n\n\n\n\nWorld"
+    >>> limit_consecutive_newlines(text)
+    'Hello\n\nWorld'
+    """
+
+    # Creating a regex pattern to match more than `max_newlines` newlines
+    pattern = r"\n{" + str(max_newlines + 1) + ",}"
+    # Replace found patterns with `max_newlines` amount of newline characters
+    return re.sub(pattern, "\n" * max_newlines, text)
```

### Comparing `pyassorted-0.8.0/pyassorted/string/validator.py` & `pyassorted-0.9.0/pyassorted/string/validator.py`

 * *Files identical despite different names*

### Comparing `pyassorted-0.8.0/pyassorted/warn/base.py` & `pyassorted-0.9.0/pyassorted/warn/base.py`

 * *Files identical despite different names*

### Comparing `pyassorted-0.8.0/pyproject.toml` & `pyassorted-0.9.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 [tool.poetry]
 authors = ["Allen Chou <f1470891079@gmail.com>"]
 description = "A library has light-weight assorted utils in Prue-Python."
 license = "MIT"
 name = "pyassorted"
 readme = "README.md"
-version = "0.8.0"
+version = "0.9.0"
 
 [tool.poetry.dependencies]
-python = ">=3.7.0, <4.0.0"
+python = ">=3.10.0, <4.0.0"
 pytz = "*"
 rich = "*"
 typing-extensions = "*"
 
 [tool.poetry.group.dev.dependencies]
 black = "*"
 flake8 = "*"
```

### Comparing `pyassorted-0.8.0/PKG-INFO` & `pyassorted-0.9.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,20 +1,17 @@
 Metadata-Version: 2.1
 Name: pyassorted
-Version: 0.8.0
+Version: 0.9.0
 Summary: A library has light-weight assorted utils in Prue-Python.
 License: MIT
 Author: Allen Chou
 Author-email: f1470891079@gmail.com
-Requires-Python: >=3.7.0,<4.0.0
+Requires-Python: >=3.10.0,<4.0.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: pytz
 Requires-Dist: rich
 Requires-Dist: typing-extensions
 Description-Content-Type: text/markdown
```

