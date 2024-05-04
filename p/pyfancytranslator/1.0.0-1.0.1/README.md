# Comparing `tmp/pyfancytranslator-1.0.0.tar.gz` & `tmp/pyfancytranslator-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyfancytranslator-1.0.0.tar", last modified: Fri May  3 13:40:41 2024, max compression
+gzip compressed data, was "pyfancytranslator-1.0.1.tar", last modified: Fri May  3 13:56:34 2024, max compression
```

## Comparing `pyfancytranslator-1.0.0.tar` & `pyfancytranslator-1.0.1.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2024-05-03 13:40:41.148953 pyfancytranslator-1.0.0/
-drwxrwxrwx   0        0        0        0 2024-05-03 13:40:41.141453 pyfancytranslator-1.0.0/FancyTranslator/
--rw-rw-rw-   0        0        0      174 2024-05-03 11:48:29.000000 pyfancytranslator-1.0.0/FancyTranslator/__init__.py
--rw-rw-rw-   0        0        0     6362 2024-05-03 13:19:21.000000 pyfancytranslator-1.0.0/FancyTranslator/classes.py
--rw-rw-rw-   0        0        0     2587 2024-05-03 13:40:41.147956 pyfancytranslator-1.0.0/PKG-INFO
--rw-rw-rw-   0        0        0     1992 2024-05-03 13:23:01.000000 pyfancytranslator-1.0.0/README.md
-drwxrwxrwx   0        0        0        0 2024-05-03 13:40:41.146959 pyfancytranslator-1.0.0/pyfancytranslator.egg-info/
--rw-rw-rw-   0        0        0     2587 2024-05-03 13:40:41.000000 pyfancytranslator-1.0.0/pyfancytranslator.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      252 2024-05-03 13:40:41.000000 pyfancytranslator-1.0.0/pyfancytranslator.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-03 13:40:41.000000 pyfancytranslator-1.0.0/pyfancytranslator.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       16 2024-05-03 13:40:41.000000 pyfancytranslator-1.0.0/pyfancytranslator.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      716 2024-05-03 11:58:11.000000 pyfancytranslator-1.0.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-05-03 13:40:41.148953 pyfancytranslator-1.0.0/setup.cfg
--rw-rw-rw-   0        0        0       39 2024-05-03 13:27:10.000000 pyfancytranslator-1.0.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-03 13:56:34.619759 pyfancytranslator-1.0.1/
+drwxrwxrwx   0        0        0        0 2024-05-03 13:56:34.610495 pyfancytranslator-1.0.1/FancyTranslator/
+-rw-rw-rw-   0        0        0      174 2024-05-03 11:48:29.000000 pyfancytranslator-1.0.1/FancyTranslator/__init__.py
+-rw-rw-rw-   0        0        0     6362 2024-05-03 13:19:21.000000 pyfancytranslator-1.0.1/FancyTranslator/classes.py
+-rw-rw-rw-   0        0        0     2596 2024-05-03 13:56:34.618574 pyfancytranslator-1.0.1/PKG-INFO
+-rw-rw-rw-   0        0        0     2001 2024-05-03 13:55:21.000000 pyfancytranslator-1.0.1/README.md
+drwxrwxrwx   0        0        0        0 2024-05-03 13:56:34.617067 pyfancytranslator-1.0.1/pyfancytranslator.egg-info/
+-rw-rw-rw-   0        0        0     2596 2024-05-03 13:56:34.000000 pyfancytranslator-1.0.1/pyfancytranslator.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      252 2024-05-03 13:56:34.000000 pyfancytranslator-1.0.1/pyfancytranslator.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-03 13:56:34.000000 pyfancytranslator-1.0.1/pyfancytranslator.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       16 2024-05-03 13:56:34.000000 pyfancytranslator-1.0.1/pyfancytranslator.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      716 2024-05-03 13:55:21.000000 pyfancytranslator-1.0.1/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-05-03 13:56:34.619759 pyfancytranslator-1.0.1/setup.cfg
+-rw-rw-rw-   0        0        0       39 2024-05-03 13:27:10.000000 pyfancytranslator-1.0.1/setup.py
```

### Comparing `pyfancytranslator-1.0.0/FancyTranslator/classes.py` & `pyfancytranslator-1.0.1/FancyTranslator/classes.py`

 * *Files identical despite different names*

### Comparing `pyfancytranslator-1.0.0/PKG-INFO` & `pyfancytranslator-1.0.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: pyfancytranslator
-Version: 1.0.0
+Version: 1.0.1
 Summary: A well built translator with placeholders
 Author-email: Ashenguard <ashenguard@agmstudio.xyz>
 Project-URL: Homepage, https://github.com/agm-studio/fancytranslator
 Project-URL: Bug Tracker, https://github.com/agm-studio/fancytranslator/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.12
 Description-Content-Type: text/markdown
 
-# EasySQL
+# Fancy Translator
 ![Downloads](https://pepy.tech/badge/pyfancytranslator)
 ![Downloads](https://pepy.tech/badge/pyfancytranslator/week)
 ![Downloads](https://pepy.tech/badge/pyfancytranslator/month)  
 This library allow you to run setup a translator with ease. Just provide it the translations files and access them when ever you need them
 
 ### Having an issue?
 You can always find someone on our discord server here:
```

### Comparing `pyfancytranslator-1.0.0/README.md` & `pyfancytranslator-1.0.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# EasySQL
+# Fancy Translator
 ![Downloads](https://pepy.tech/badge/pyfancytranslator)
 ![Downloads](https://pepy.tech/badge/pyfancytranslator/week)
 ![Downloads](https://pepy.tech/badge/pyfancytranslator/month)  
 This library allow you to run setup a translator with ease. Just provide it the translations files and access them when ever you need them
 
 ### Having an issue?
 You can always find someone on our discord server here:
```

### Comparing `pyfancytranslator-1.0.0/pyfancytranslator.egg-info/PKG-INFO` & `pyfancytranslator-1.0.1/pyfancytranslator.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: pyfancytranslator
-Version: 1.0.0
+Version: 1.0.1
 Summary: A well built translator with placeholders
 Author-email: Ashenguard <ashenguard@agmstudio.xyz>
 Project-URL: Homepage, https://github.com/agm-studio/fancytranslator
 Project-URL: Bug Tracker, https://github.com/agm-studio/fancytranslator/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.12
 Description-Content-Type: text/markdown
 
-# EasySQL
+# Fancy Translator
 ![Downloads](https://pepy.tech/badge/pyfancytranslator)
 ![Downloads](https://pepy.tech/badge/pyfancytranslator/week)
 ![Downloads](https://pepy.tech/badge/pyfancytranslator/month)  
 This library allow you to run setup a translator with ease. Just provide it the translations files and access them when ever you need them
 
 ### Having an issue?
 You can always find someone on our discord server here:
```

### Comparing `pyfancytranslator-1.0.0/pyproject.toml` & `pyfancytranslator-1.0.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "pyfancytranslator"
-version = "1.0.0"
+version = "1.0.1"
 authors = [
     { name = "Ashenguard", email = "ashenguard@agmstudio.xyz" },
 ]
 description = "A well built translator with placeholders"
 readme = "README.md"
 requires-python = ">=3.12"
 classifiers = [
```

